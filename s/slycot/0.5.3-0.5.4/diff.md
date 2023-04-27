# Comparing `tmp/slycot-0.5.3.tar.gz` & `tmp/slycot-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slycot-0.5.3.tar", last modified: Wed Dec 21 09:30:10 2022, max compression
+gzip compressed data, was "slycot-0.5.4.tar", last modified: Thu Apr 27 19:48:48 2023, max compression
```

## Comparing `slycot-0.5.3.tar` & `slycot-0.5.4.tar`

### file list

```diff
@@ -1,2042 +1,2055 @@
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.684944 slycot-0.5.3/
--rw-r--r--   0 ben       (1000) users      (100)      191 2022-07-16 10:42:02.000000 slycot-0.5.3/.coveragerc
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.040930 slycot-0.5.3/.github/
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.040930 slycot-0.5.3/.github/conda-env/
--rw-r--r--   0 ben       (1000) users      (100)       57 2022-12-21 09:29:38.000000 slycot-0.5.3/.github/conda-env/build-env.yml
--rw-r--r--   0 ben       (1000) users      (100)      270 2022-12-21 09:29:38.000000 slycot-0.5.3/.github/conda-env/test-env.yml
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.040930 slycot-0.5.3/.github/scripts/
--rw-r--r--   0 ben       (1000) users      (100)     1186 2021-01-30 12:23:36.000000 slycot-0.5.3/.github/scripts/run-tests.sh
--rw-r--r--   0 ben       (1000) users      (100)      988 2021-02-07 11:42:42.000000 slycot-0.5.3/.github/scripts/set-conda-test-matrix.py
--rw-r--r--   0 ben       (1000) users      (100)      865 2021-01-30 12:23:36.000000 slycot-0.5.3/.github/scripts/set-pip-test-matrix.py
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.040930 slycot-0.5.3/.github/workflows/
--rw-r--r--   0 ben       (1000) users      (100)    12871 2022-11-23 20:17:18.000000 slycot-0.5.3/.github/workflows/slycot-build-and-test.yml
--rw-r--r--   0 ben       (1000) users      (100)      130 2021-01-22 23:20:08.000000 slycot-0.5.3/.gitignore
--rw-r--r--   0 ben       (1000) users      (100)      136 2021-03-17 11:49:25.000000 slycot-0.5.3/.gitmodules
--rw-r--r--   0 ben       (1000) users      (100)      328 2021-01-22 23:20:08.000000 slycot-0.5.3/AUTHORS
--rw-r--r--   0 ben       (1000) users      (100)      758 2022-11-08 14:30:23.000000 slycot-0.5.3/CMakeLists.txt
--rw-r--r--   0 ben       (1000) users      (100)      750 2021-01-22 23:20:08.000000 slycot-0.5.3/COPYING
--rw-r--r--   0 ben       (1000) users      (100)      334 2022-10-30 11:05:45.000000 slycot-0.5.3/MANIFEST.in
--rw-r--r--   0 ben       (1000) users      (100)    10351 2022-12-21 09:30:10.684944 slycot-0.5.3/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (100)     9065 2022-11-23 20:17:18.000000 slycot-0.5.3/README.rst
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.040930 slycot-0.5.3/conda-recipe/
--rw-r--r--   0 ben       (1000) users      (100)      195 2022-05-03 20:29:21.000000 slycot-0.5.3/conda-recipe/bld.bat
--rw-r--r--   0 ben       (1000) users      (100)      178 2022-05-03 20:29:21.000000 slycot-0.5.3/conda-recipe/build.sh
--rw-r--r--   0 ben       (1000) users      (100)     1561 2022-12-21 09:29:38.000000 slycot-0.5.3/conda-recipe/meta.yaml
--rw-r--r--   0 ben       (1000) users      (100)    18092 2021-01-22 23:20:08.000000 slycot-0.5.3/gpl-2.0.txt
--rw-r--r--   0 ben       (1000) users      (100)     1622 2022-12-21 09:29:38.000000 slycot-0.5.3/pyproject.toml
--rw-r--r--   0 ben       (1000) users      (100)       38 2022-12-21 09:30:10.684944 slycot-0.5.3/setup.cfg
--rw-r--r--   0 ben       (1000) users      (100)     2120 2022-10-30 11:05:45.000000 slycot-0.5.3/setup.py
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.048930 slycot-0.5.3/slycot/
--rw-r--r--   0 ben       (1000) users      (100)    22431 2022-12-21 09:29:38.000000 slycot-0.5.3/slycot/CMakeLists.txt
--rw-r--r--   0 ben       (1000) users      (100)     1546 2022-10-30 11:05:45.000000 slycot-0.5.3/slycot/__init__.py
--rw-r--r--   0 ben       (1000) users      (100)    85946 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/analysis.py
--rw-r--r--   0 ben       (1000) users      (100)     9082 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/examples.py
--rw-r--r--   0 ben       (1000) users      (100)     8737 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/exceptions.py
--rw-r--r--   0 ben       (1000) users      (100)    30976 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/math.py
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.048930 slycot-0.5.3/slycot/src/
--rw-r--r--   0 ben       (1000) users      (100)      668 2021-03-17 11:49:25.000000 slycot-0.5.3/slycot/src/Readme.md
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.052930 slycot-0.5.3/slycot/src/SLICOT-Reference/
--rw-r--r--   0 ben       (1000) users      (100)       58 2021-02-07 20:42:18.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/.git
--rw-r--r--   0 ben       (1000) users      (100)     1862 2022-05-29 11:35:56.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/Contributors.md
--rw-r--r--   0 ben       (1000) users      (100)     1514 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/LICENSE
--rw-r--r--   0 ben       (1000) users      (100)     3224 2022-05-29 11:35:56.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/README.md
--rw-r--r--   0 ben       (1000) users      (100)    17990 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/ReleaseNotes.md
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.060930 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/
--rw-r--r--   0 ben       (1000) users      (100)      492 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB01103.dat
--rw-r--r--   0 ben       (1000) users      (100)     1737 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB01104.dat
--rw-r--r--   0 ben       (1000) users      (100)     1312 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB01105.dat
--rw-r--r--   0 ben       (1000) users      (100)    13457 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB01106.dat
--rw-r--r--   0 ben       (1000) users      (100)    10508 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB012091.dat
--rw-r--r--   0 ben       (1000) users      (100)     8597 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB012092.dat
--rw-r--r--   0 ben       (1000) users      (100)    11788 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB01404.dat
--rw-r--r--   0 ben       (1000) users      (100)      240 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB02105.dat
--rw-r--r--   0 ben       (1000) users      (100)      288 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB02106.dat
--rw-r--r--   0 ben       (1000) users      (100)      363 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB02107.dat
--rw-r--r--   0 ben       (1000) users      (100)      420 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB02108.dat
--rw-r--r--   0 ben       (1000) users      (100)     1190 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB02110.dat
--rw-r--r--   0 ben       (1000) users      (100)     1435 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB02111.dat
--rw-r--r--   0 ben       (1000) users      (100)     6612 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB02113.dat
--rw-r--r--   0 ben       (1000) users      (100)      296 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01103.dat
--rw-r--r--   0 ben       (1000) users      (100)      969 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01104.dat
--rw-r--r--   0 ben       (1000) users      (100)     1312 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01105.dat
--rw-r--r--   0 ben       (1000) users      (100)    13457 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01106.dat
--rw-r--r--   0 ben       (1000) users      (100)     1849 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01107.dat
--rw-r--r--   0 ben       (1000) users      (100)     1297 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01108.dat
--rw-r--r--   0 ben       (1000) users      (100)    38186 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01109.dat
--rw-r--r--   0 ben       (1000) users      (100)      961 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01110.dat
--rw-r--r--   0 ben       (1000) users      (100)     1020 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01203.dat
--rw-r--r--   0 ben       (1000) users      (100)      101 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012051.dat
--rw-r--r--   0 ben       (1000) users      (100)      394 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012052.dat
--rw-r--r--   0 ben       (1000) users      (100)      886 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012053.dat
--rw-r--r--   0 ben       (1000) users      (100)     1542 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012054.dat
--rw-r--r--   0 ben       (1000) users      (100)     2410 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012055.dat
--rw-r--r--   0 ben       (1000) users      (100)     3489 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012056.dat
--rw-r--r--   0 ben       (1000) users      (100)     9561 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012057.dat
--rw-r--r--   0 ben       (1000) users      (100)      375 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01206.dat
--rw-r--r--   0 ben       (1000) users      (100)    11346 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01304.dat
--rw-r--r--   0 ben       (1000) users      (100)      244 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD02106.dat
--rw-r--r--   0 ben       (1000) users      (100)      296 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD02107.dat
--rw-r--r--   0 ben       (1000) users      (100)      332 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD02108.dat
--rw-r--r--   0 ben       (1000) users      (100)      430 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD02109.dat
--rw-r--r--   0 ben       (1000) users      (100)     1190 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD02111.dat
--rw-r--r--   0 ben       (1000) users      (100)      185 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD02112.dat
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.300935 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/
--rw-r--r--   0 ben       (1000) users      (100)    10439 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB01MD.html
--rw-r--r--   0 ben       (1000) users      (100)    13617 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB01ND.html
--rw-r--r--   0 ben       (1000) users      (100)    15601 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB01OD.html
--rw-r--r--   0 ben       (1000) users      (100)    10500 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB04MD.html
--rw-r--r--   0 ben       (1000) users      (100)    16184 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05MD.html
--rw-r--r--   0 ben       (1000) users      (100)    15634 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05ND.html
--rw-r--r--   0 ben       (1000) users      (100)    14975 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05OD.html
--rw-r--r--   0 ben       (1000) users      (100)    13669 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05PD.html
--rw-r--r--   0 ben       (1000) users      (100)    15645 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05QD.html
--rw-r--r--   0 ben       (1000) users      (100)    16003 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05RD.html
--rw-r--r--   0 ben       (1000) users      (100)     6652 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05SD.html
--rw-r--r--   0 ben       (1000) users      (100)     8104 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB07MD.html
--rw-r--r--   0 ben       (1000) users      (100)     8808 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB07ND.html
--rw-r--r--   0 ben       (1000) users      (100)     5754 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08MD.html
--rw-r--r--   0 ben       (1000) users      (100)     5828 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08MZ.html
--rw-r--r--   0 ben       (1000) users      (100)    19657 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08ND.html
--rw-r--r--   0 ben       (1000) users      (100)    20520 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08NW.html
--rw-r--r--   0 ben       (1000) users      (100)     6715 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08NX.html
--rw-r--r--   0 ben       (1000) users      (100)     8474 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08NY.html
--rw-r--r--   0 ben       (1000) users      (100)    20172 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08NZ.html
--rw-r--r--   0 ben       (1000) users      (100)    14482 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09AD.html
--rw-r--r--   0 ben       (1000) users      (100)    10136 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09AX.html
--rw-r--r--   0 ben       (1000) users      (100)    15744 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09BD.html
--rw-r--r--   0 ben       (1000) users      (100)    10850 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09BX.html
--rw-r--r--   0 ben       (1000) users      (100)    16037 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09CD.html
--rw-r--r--   0 ben       (1000) users      (100)    10067 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09CX.html
--rw-r--r--   0 ben       (1000) users      (100)    10626 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09DD.html
--rw-r--r--   0 ben       (1000) users      (100)    18851 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09ED.html
--rw-r--r--   0 ben       (1000) users      (100)    19104 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09FD.html
--rw-r--r--   0 ben       (1000) users      (100)    20632 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09GD.html
--rw-r--r--   0 ben       (1000) users      (100)    23079 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09HD.html
--rw-r--r--   0 ben       (1000) users      (100)    13053 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09HX.html
--rw-r--r--   0 ben       (1000) users      (100)     6109 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09HY.html
--rw-r--r--   0 ben       (1000) users      (100)    38139 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09ID.html
--rw-r--r--   0 ben       (1000) users      (100)    13673 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09IX.html
--rw-r--r--   0 ben       (1000) users      (100)    16029 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09IY.html
--rw-r--r--   0 ben       (1000) users      (100)    34224 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09JD.html
--rw-r--r--   0 ben       (1000) users      (100)    14431 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09JV.html
--rw-r--r--   0 ben       (1000) users      (100)    14420 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09JW.html
--rw-r--r--   0 ben       (1000) users      (100)     4647 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09JX.html
--rw-r--r--   0 ben       (1000) users      (100)    31860 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09KD.html
--rw-r--r--   0 ben       (1000) users      (100)    15796 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09KX.html
--rw-r--r--   0 ben       (1000) users      (100)    16846 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09MD.html
--rw-r--r--   0 ben       (1000) users      (100)    18265 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09ND.html
--rw-r--r--   0 ben       (1000) users      (100)    11723 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13AD.html
--rw-r--r--   0 ben       (1000) users      (100)     5121 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13AX.html
--rw-r--r--   0 ben       (1000) users      (100)    12848 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13BD.html
--rw-r--r--   0 ben       (1000) users      (100)     9237 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13CD.html
--rw-r--r--   0 ben       (1000) users      (100)    15801 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13DD.html
--rw-r--r--   0 ben       (1000) users      (100)     9352 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13DX.html
--rw-r--r--   0 ben       (1000) users      (100)     8381 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13ED.html
--rw-r--r--   0 ben       (1000) users      (100)     8583 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13FD.html
--rw-r--r--   0 ben       (1000) users      (100)    26176 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13ID.html
--rw-r--r--   0 ben       (1000) users      (100)     9468 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13MD.html
--rw-r--r--   0 ben       (1000) users      (100)     6806 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB8NXZ.html
--rw-r--r--   0 ben       (1000) users      (100)     6359 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AG07BD.html
--rw-r--r--   0 ben       (1000) users      (100)    30005 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AG08BD.html
--rw-r--r--   0 ben       (1000) users      (100)     9124 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AG08BY.html
--rw-r--r--   0 ben       (1000) users      (100)    29847 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AG08BZ.html
--rw-r--r--   0 ben       (1000) users      (100)     9318 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AG8BYZ.html
--rw-r--r--   0 ben       (1000) users      (100)    24747 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BB01AD.html
--rw-r--r--   0 ben       (1000) users      (100)    22080 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BB02AD.html
--rw-r--r--   0 ben       (1000) users      (100)    12650 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BB03AD.html
--rw-r--r--   0 ben       (1000) users      (100)    12644 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BB04AD.html
--rw-r--r--   0 ben       (1000) users      (100)    11789 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BD01AD.html
--rw-r--r--   0 ben       (1000) users      (100)    10951 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BD02AD.html
--rw-r--r--   0 ben       (1000) users      (100)   114864 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DAESolver.html
--rw-r--r--   0 ben       (1000) users      (100)     4784 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DE01OD.html
--rw-r--r--   0 ben       (1000) users      (100)     5679 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DE01PD.html
--rw-r--r--   0 ben       (1000) users      (100)     7489 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DF01MD.html
--rw-r--r--   0 ben       (1000) users      (100)     5966 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DG01MD.html
--rw-r--r--   0 ben       (1000) users      (100)     9284 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DG01ND.html
--rw-r--r--   0 ben       (1000) users      (100)     5403 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DG01OD.html
--rw-r--r--   0 ben       (1000) users      (100)     4704 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DK01MD.html
--rw-r--r--   0 ben       (1000) users      (100)    17140 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FB01QD.html
--rw-r--r--   0 ben       (1000) users      (100)    17900 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FB01RD.html
--rw-r--r--   0 ben       (1000) users      (100)    20362 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FB01SD.html
--rw-r--r--   0 ben       (1000) users      (100)    20707 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FB01TD.html
--rw-r--r--   0 ben       (1000) users      (100)    13220 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FB01VD.html
--rw-r--r--   0 ben       (1000) users      (100)    14387 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FD01AD.html
--rw-r--r--   0 ben       (1000) users      (100)    16749 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FSQP.html
--rw-r--r--   0 ben       (1000) users      (100)    47491 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01AD.html
--rw-r--r--   0 ben       (1000) users      (100)    51068 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01BD.html
--rw-r--r--   0 ben       (1000) users      (100)    54820 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01CD.html
--rw-r--r--   0 ben       (1000) users      (100)    15536 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01MD.html
--rw-r--r--   0 ben       (1000) users      (100)    11259 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01MY.html
--rw-r--r--   0 ben       (1000) users      (100)     9283 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01ND.html
--rw-r--r--   0 ben       (1000) users      (100)     3923 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01OD.html
--rw-r--r--   0 ben       (1000) users      (100)     2303 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01OY.html
--rw-r--r--   0 ben       (1000) users      (100)    16939 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01PD.html
--rw-r--r--   0 ben       (1000) users      (100)    10622 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01PX.html
--rw-r--r--   0 ben       (1000) users      (100)    15620 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01PY.html
--rw-r--r--   0 ben       (1000) users      (100)    14429 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01QD.html
--rw-r--r--   0 ben       (1000) users      (100)     9362 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01RD.html
--rw-r--r--   0 ben       (1000) users      (100)    66249 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB03AD.html
--rw-r--r--   0 ben       (1000) users      (100)    67654 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB03BD.html
--rw-r--r--   0 ben       (1000) users      (100)    29374 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/KINSOL.html
--rw-r--r--   0 ben       (1000) users      (100)     2075 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA01AD.html
--rw-r--r--   0 ben       (1000) users      (100)     2318 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA01BD.html
--rw-r--r--   0 ben       (1000) users      (100)     2330 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA01BZ.html
--rw-r--r--   0 ben       (1000) users      (100)     2340 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA01CD.html
--rw-r--r--   0 ben       (1000) users      (100)     2319 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02AD.html
--rw-r--r--   0 ben       (1000) users      (100)     2690 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02AZ.html
--rw-r--r--   0 ben       (1000) users      (100)     2688 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02BD.html
--rw-r--r--   0 ben       (1000) users      (100)     2697 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02BZ.html
--rw-r--r--   0 ben       (1000) users      (100)     2534 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02CD.html
--rw-r--r--   0 ben       (1000) users      (100)     2543 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02CZ.html
--rw-r--r--   0 ben       (1000) users      (100)     3744 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02DD.html
--rw-r--r--   0 ben       (1000) users      (100)     2295 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02ED.html
--rw-r--r--   0 ben       (1000) users      (100)     2370 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02ES.html
--rw-r--r--   0 ben       (1000) users      (100)     3288 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02EZ.html
--rw-r--r--   0 ben       (1000) users      (100)     2165 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02FD.html
--rw-r--r--   0 ben       (1000) users      (100)     3516 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02GD.html
--rw-r--r--   0 ben       (1000) users      (100)     3518 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02GZ.html
--rw-r--r--   0 ben       (1000) users      (100)     2783 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02HD.html
--rw-r--r--   0 ben       (1000) users      (100)     2840 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02HZ.html
--rw-r--r--   0 ben       (1000) users      (100)     3590 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02ID.html
--rw-r--r--   0 ben       (1000) users      (100)     3876 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02IZ.html
--rw-r--r--   0 ben       (1000) users      (100)     3100 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02JD.html
--rw-r--r--   0 ben       (1000) users      (100)     3097 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02JZ.html
--rw-r--r--   0 ben       (1000) users      (100)     3244 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02MD.html
--rw-r--r--   0 ben       (1000) users      (100)     3296 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02MZ.html
--rw-r--r--   0 ben       (1000) users      (100)     3477 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02NZ.html
--rw-r--r--   0 ben       (1000) users      (100)     2874 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02OD.html
--rw-r--r--   0 ben       (1000) users      (100)     3055 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02OZ.html
--rw-r--r--   0 ben       (1000) users      (100)     1934 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02PD.html
--rw-r--r--   0 ben       (1000) users      (100)     1934 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02PZ.html
--rw-r--r--   0 ben       (1000) users      (100)     5585 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01KD.html
--rw-r--r--   0 ben       (1000) users      (100)     7364 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01LD.html
--rw-r--r--   0 ben       (1000) users      (100)     4306 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01MD.html
--rw-r--r--   0 ben       (1000) users      (100)     4367 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01ND.html
--rw-r--r--   0 ben       (1000) users      (100)     5063 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OC.html
--rw-r--r--   0 ben       (1000) users      (100)     6957 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OD.html
--rw-r--r--   0 ben       (1000) users      (100)     4460 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OE.html
--rw-r--r--   0 ben       (1000) users      (100)     4424 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OH.html
--rw-r--r--   0 ben       (1000) users      (100)     4565 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OO.html
--rw-r--r--   0 ben       (1000) users      (100)     4248 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OS.html
--rw-r--r--   0 ben       (1000) users      (100)     4425 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OT.html
--rw-r--r--   0 ben       (1000) users      (100)     5070 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01PD.html
--rw-r--r--   0 ben       (1000) users      (100)     4478 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01QD.html
--rw-r--r--   0 ben       (1000) users      (100)     6803 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RB.html
--rw-r--r--   0 ben       (1000) users      (100)     7487 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RD.html
--rw-r--r--   0 ben       (1000) users      (100)     6252 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RH.html
--rw-r--r--   0 ben       (1000) users      (100)     6120 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RT.html
--rw-r--r--   0 ben       (1000) users      (100)     6493 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RU.html
--rw-r--r--   0 ben       (1000) users      (100)     3741 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RW.html
--rw-r--r--   0 ben       (1000) users      (100)     6760 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RX.html
--rw-r--r--   0 ben       (1000) users      (100)     5823 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RY.html
--rw-r--r--   0 ben       (1000) users      (100)     2601 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01SD.html
--rw-r--r--   0 ben       (1000) users      (100)     3055 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01SS.html
--rw-r--r--   0 ben       (1000) users      (100)     5348 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01TD.html
--rw-r--r--   0 ben       (1000) users      (100)     4261 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01UD.html
--rw-r--r--   0 ben       (1000) users      (100)     4763 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01UW.html
--rw-r--r--   0 ben       (1000) users      (100)     6040 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01UX.html
--rw-r--r--   0 ben       (1000) users      (100)     5183 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01UY.html
--rw-r--r--   0 ben       (1000) users      (100)     5259 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01UZ.html
--rw-r--r--   0 ben       (1000) users      (100)     5144 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01VD.html
--rw-r--r--   0 ben       (1000) users      (100)     6315 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01WD.html
--rw-r--r--   0 ben       (1000) users      (100)     3472 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01XD.html
--rw-r--r--   0 ben       (1000) users      (100)     3482 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01XY.html
--rw-r--r--   0 ben       (1000) users      (100)     6292 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01YD.html
--rw-r--r--   0 ben       (1000) users      (100)     6768 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01ZD.html
--rw-r--r--   0 ben       (1000) users      (100)    13036 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02CD.html
--rw-r--r--   0 ben       (1000) users      (100)     9730 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02CU.html
--rw-r--r--   0 ben       (1000) users      (100)    10630 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02CV.html
--rw-r--r--   0 ben       (1000) users      (100)     5892 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02CX.html
--rw-r--r--   0 ben       (1000) users      (100)     5642 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02CY.html
--rw-r--r--   0 ben       (1000) users      (100)    20569 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02DD.html
--rw-r--r--   0 ben       (1000) users      (100)     9491 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02ED.html
--rw-r--r--   0 ben       (1000) users      (100)    13962 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02FD.html
--rw-r--r--   0 ben       (1000) users      (100)    11272 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02GD.html
--rw-r--r--   0 ben       (1000) users      (100)    12422 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02HD.html
--rw-r--r--   0 ben       (1000) users      (100)    12167 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02ID.html
--rw-r--r--   0 ben       (1000) users      (100)    12349 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02JD.html
--rw-r--r--   0 ben       (1000) users      (100)    13496 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02JX.html
--rw-r--r--   0 ben       (1000) users      (100)    11412 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02KD.html
--rw-r--r--   0 ben       (1000) users      (100)    17097 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02MD.html
--rw-r--r--   0 ben       (1000) users      (100)    23196 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02ND.html
--rw-r--r--   0 ben       (1000) users      (100)     6968 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02NY.html
--rw-r--r--   0 ben       (1000) users      (100)     6734 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02OD.html
--rw-r--r--   0 ben       (1000) users      (100)    14113 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02PD.html
--rw-r--r--   0 ben       (1000) users      (100)    13193 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02QD.html
--rw-r--r--   0 ben       (1000) users      (100)     6224 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02QY.html
--rw-r--r--   0 ben       (1000) users      (100)     3421 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02RD.html
--rw-r--r--   0 ben       (1000) users      (100)     3392 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02RZ.html
--rw-r--r--   0 ben       (1000) users      (100)     6547 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02SD.html
--rw-r--r--   0 ben       (1000) users      (100)     3116 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02SZ.html
--rw-r--r--   0 ben       (1000) users      (100)     3482 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02TD.html
--rw-r--r--   0 ben       (1000) users      (100)     3523 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02TZ.html
--rw-r--r--   0 ben       (1000) users      (100)     9952 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02UD.html
--rw-r--r--   0 ben       (1000) users      (100)     2940 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02UU.html
--rw-r--r--   0 ben       (1000) users      (100)     3015 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02UV.html
--rw-r--r--   0 ben       (1000) users      (100)     4976 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02UW.html
--rw-r--r--   0 ben       (1000) users      (100)     6361 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02VD.html
--rw-r--r--   0 ben       (1000) users      (100)    10790 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02WD.html
--rw-r--r--   0 ben       (1000) users      (100)    11049 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02XD.html
--rw-r--r--   0 ben       (1000) users      (100)     6862 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02YD.html
--rw-r--r--   0 ben       (1000) users      (100)     4795 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AB.html
--rw-r--r--   0 ben       (1000) users      (100)     4021 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AD.html
--rw-r--r--   0 ben       (1000) users      (100)     4428 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AE.html
--rw-r--r--   0 ben       (1000) users      (100)     4176 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AF.html
--rw-r--r--   0 ben       (1000) users      (100)     4668 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AG.html
--rw-r--r--   0 ben       (1000) users      (100)     4818 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AH.html
--rw-r--r--   0 ben       (1000) users      (100)     4433 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AI.html
--rw-r--r--   0 ben       (1000) users      (100)     2213 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BA.html
--rw-r--r--   0 ben       (1000) users      (100)     4210 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BB.html
--rw-r--r--   0 ben       (1000) users      (100)     4704 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BC.html
--rw-r--r--   0 ben       (1000) users      (100)    19841 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BD.html
--rw-r--r--   0 ben       (1000) users      (100)     2808 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BE.html
--rw-r--r--   0 ben       (1000) users      (100)     3090 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BF.html
--rw-r--r--   0 ben       (1000) users      (100)    15953 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BZ.html
--rw-r--r--   0 ben       (1000) users      (100)     8066 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03CD.html
--rw-r--r--   0 ben       (1000) users      (100)     4103 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03CZ.html
--rw-r--r--   0 ben       (1000) users      (100)     7308 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03DD.html
--rw-r--r--   0 ben       (1000) users      (100)     3424 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03DZ.html
--rw-r--r--   0 ben       (1000) users      (100)     6126 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03ED.html
--rw-r--r--   0 ben       (1000) users      (100)     5606 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03FD.html
--rw-r--r--   0 ben       (1000) users      (100)    24239 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03FZ.html
--rw-r--r--   0 ben       (1000) users      (100)     4706 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03GD.html
--rw-r--r--   0 ben       (1000) users      (100)     3247 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03GZ.html
--rw-r--r--   0 ben       (1000) users      (100)     4609 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03HD.html
--rw-r--r--   0 ben       (1000) users      (100)     2663 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03HZ.html
--rw-r--r--   0 ben       (1000) users      (100)    12632 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03ID.html
--rw-r--r--   0 ben       (1000) users      (100)    11941 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03IZ.html
--rw-r--r--   0 ben       (1000) users      (100)     9167 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03JD.html
--rw-r--r--   0 ben       (1000) users      (100)     9461 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03JP.html
--rw-r--r--   0 ben       (1000) users      (100)     8428 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03JZ.html
--rw-r--r--   0 ben       (1000) users      (100)    10505 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03KA.html
--rw-r--r--   0 ben       (1000) users      (100)    10138 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03KB.html
--rw-r--r--   0 ben       (1000) users      (100)     4596 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03KC.html
--rw-r--r--   0 ben       (1000) users      (100)    19898 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03KD.html
--rw-r--r--   0 ben       (1000) users      (100)     6458 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03KE.html
--rw-r--r--   0 ben       (1000) users      (100)    19519 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03LD.html
--rw-r--r--   0 ben       (1000) users      (100)    20543 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03LF.html
--rw-r--r--   0 ben       (1000) users      (100)    13796 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03LP.html
--rw-r--r--   0 ben       (1000) users      (100)    20532 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03LZ.html
--rw-r--r--   0 ben       (1000) users      (100)    11706 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03MD.html
--rw-r--r--   0 ben       (1000) users      (100)     8716 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03ND.html
--rw-r--r--   0 ben       (1000) users      (100)     3862 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03NY.html
--rw-r--r--   0 ben       (1000) users      (100)    10579 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03OD.html
--rw-r--r--   0 ben       (1000) users      (100)     7560 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03OY.html
--rw-r--r--   0 ben       (1000) users      (100)    11371 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03PD.html
--rw-r--r--   0 ben       (1000) users      (100)     7563 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03PY.html
--rw-r--r--   0 ben       (1000) users      (100)    11372 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QD.html
--rw-r--r--   0 ben       (1000) users      (100)    15736 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QG.html
--rw-r--r--   0 ben       (1000) users      (100)     2854 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QV.html
--rw-r--r--   0 ben       (1000) users      (100)     5601 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QW.html
--rw-r--r--   0 ben       (1000) users      (100)     2159 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QX.html
--rw-r--r--   0 ben       (1000) users      (100)     4231 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QY.html
--rw-r--r--   0 ben       (1000) users      (100)    15483 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03RD.html
--rw-r--r--   0 ben       (1000) users      (100)     5894 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03RW.html
--rw-r--r--   0 ben       (1000) users      (100)     5960 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03RX.html
--rw-r--r--   0 ben       (1000) users      (100)     5886 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03RY.html
--rw-r--r--   0 ben       (1000) users      (100)    10701 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03RZ.html
--rw-r--r--   0 ben       (1000) users      (100)     9360 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03SD.html
--rw-r--r--   0 ben       (1000) users      (100)    15914 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03TD.html
--rw-r--r--   0 ben       (1000) users      (100)     6348 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03TS.html
--rw-r--r--   0 ben       (1000) users      (100)     8365 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03UD.html
--rw-r--r--   0 ben       (1000) users      (100)    13418 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03VD.html
--rw-r--r--   0 ben       (1000) users      (100)     8636 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03VW.html
--rw-r--r--   0 ben       (1000) users      (100)     4913 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03VY.html
--rw-r--r--   0 ben       (1000) users      (100)     5909 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03WA.html
--rw-r--r--   0 ben       (1000) users      (100)    16586 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03WD.html
--rw-r--r--   0 ben       (1000) users      (100)     2900 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03WX.html
--rw-r--r--   0 ben       (1000) users      (100)    26175 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03XD.html
--rw-r--r--   0 ben       (1000) users      (100)    18234 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03XP.html
--rw-r--r--   0 ben       (1000) users      (100)     7577 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03XS.html
--rw-r--r--   0 ben       (1000) users      (100)    11313 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03XU.html
--rw-r--r--   0 ben       (1000) users      (100)    32413 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03XZ.html
--rw-r--r--   0 ben       (1000) users      (100)     7348 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03YA.html
--rw-r--r--   0 ben       (1000) users      (100)     8262 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03YD.html
--rw-r--r--   0 ben       (1000) users      (100)     4071 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03YT.html
--rw-r--r--   0 ben       (1000) users      (100)    11772 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03ZA.html
--rw-r--r--   0 ben       (1000) users      (100)    26201 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03ZD.html
--rw-r--r--   0 ben       (1000) users      (100)    31322 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04AD.html
--rw-r--r--   0 ben       (1000) users      (100)    26755 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04AZ.html
--rw-r--r--   0 ben       (1000) users      (100)    25688 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04BD.html
--rw-r--r--   0 ben       (1000) users      (100)    17542 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04BP.html
--rw-r--r--   0 ben       (1000) users      (100)    22893 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04BZ.html
--rw-r--r--   0 ben       (1000) users      (100)    14349 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04CD.html
--rw-r--r--   0 ben       (1000) users      (100)     4345 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DB.html
--rw-r--r--   0 ben       (1000) users      (100)     8778 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DD.html
--rw-r--r--   0 ben       (1000) users      (100)     3914 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DI.html
--rw-r--r--   0 ben       (1000) users      (100)    14725 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DL.html
--rw-r--r--   0 ben       (1000) users      (100)    18014 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DP.html
--rw-r--r--   0 ben       (1000) users      (100)     8775 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DS.html
--rw-r--r--   0 ben       (1000) users      (100)    11041 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DY.html
--rw-r--r--   0 ben       (1000) users      (100)     9752 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DZ.html
--rw-r--r--   0 ben       (1000) users      (100)    22966 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04ED.html
--rw-r--r--   0 ben       (1000) users      (100)    19126 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04FD.html
--rw-r--r--   0 ben       (1000) users      (100)    13143 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04FP.html
--rw-r--r--   0 ben       (1000) users      (100)     7117 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04GD.html
--rw-r--r--   0 ben       (1000) users      (100)    11547 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04HD.html
--rw-r--r--   0 ben       (1000) users      (100)     5262 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04ID.html
--rw-r--r--   0 ben       (1000) users      (100)     5201 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04IY.html
--rw-r--r--   0 ben       (1000) users      (100)     5253 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04IZ.html
--rw-r--r--   0 ben       (1000) users      (100)     4973 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04JD.html
--rw-r--r--   0 ben       (1000) users      (100)     5324 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04KD.html
--rw-r--r--   0 ben       (1000) users      (100)     5303 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04LD.html
--rw-r--r--   0 ben       (1000) users      (100)     6063 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04MD.html
--rw-r--r--   0 ben       (1000) users      (100)     5862 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04ND.html
--rw-r--r--   0 ben       (1000) users      (100)     3582 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04NY.html
--rw-r--r--   0 ben       (1000) users      (100)     8981 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04OD.html
--rw-r--r--   0 ben       (1000) users      (100)     5731 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04OW.html
--rw-r--r--   0 ben       (1000) users      (100)     2719 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04OX.html
--rw-r--r--   0 ben       (1000) users      (100)     3460 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04OY.html
--rw-r--r--   0 ben       (1000) users      (100)     7386 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04PA.html
--rw-r--r--   0 ben       (1000) users      (100)    15575 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04PB.html
--rw-r--r--   0 ben       (1000) users      (100)    15043 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04PU.html
--rw-r--r--   0 ben       (1000) users      (100)     3532 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04PY.html
--rw-r--r--   0 ben       (1000) users      (100)     7869 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04QB.html
--rw-r--r--   0 ben       (1000) users      (100)     7879 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04QC.html
--rw-r--r--   0 ben       (1000) users      (100)     6010 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04QF.html
--rw-r--r--   0 ben       (1000) users      (100)     6804 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04QS.html
--rw-r--r--   0 ben       (1000) users      (100)     7404 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04QU.html
--rw-r--r--   0 ben       (1000) users      (100)     6522 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04RB.html
--rw-r--r--   0 ben       (1000) users      (100)     5954 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04RU.html
--rw-r--r--   0 ben       (1000) users      (100)     5581 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04SU.html
--rw-r--r--   0 ben       (1000) users      (100)    24478 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04TB.html
--rw-r--r--   0 ben       (1000) users      (100)    23832 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04TS.html
--rw-r--r--   0 ben       (1000) users      (100)     1743 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04TU.html
--rw-r--r--   0 ben       (1000) users      (100)    11241 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04UD.html
--rw-r--r--   0 ben       (1000) users      (100)    19661 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04VD.html
--rw-r--r--   0 ben       (1000) users      (100)     6393 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04WD.html
--rw-r--r--   0 ben       (1000) users      (100)     5114 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04WP.html
--rw-r--r--   0 ben       (1000) users      (100)     7581 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04WR.html
--rw-r--r--   0 ben       (1000) users      (100)     5975 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04WU.html
--rw-r--r--   0 ben       (1000) users      (100)    22354 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04XD.html
--rw-r--r--   0 ben       (1000) users      (100)     5375 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04XY.html
--rw-r--r--   0 ben       (1000) users      (100)    17947 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04YD.html
--rw-r--r--   0 ben       (1000) users      (100)     7428 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04YW.html
--rw-r--r--   0 ben       (1000) users      (100)    13508 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04ZD.html
--rw-r--r--   0 ben       (1000) users      (100)    10998 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB05MD.html
--rw-r--r--   0 ben       (1000) users      (100)     6164 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB05MY.html
--rw-r--r--   0 ben       (1000) users      (100)     7875 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB05ND.html
--rw-r--r--   0 ben       (1000) users      (100)     8093 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB05OD.html
--rw-r--r--   0 ben       (1000) users      (100)     3553 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB05OY.html
--rw-r--r--   0 ben       (1000) users      (100)     8896 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB3JZP.html
--rw-r--r--   0 ben       (1000) users      (100)    13887 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB3LZP.html
--rw-r--r--   0 ben       (1000) users      (100)     7524 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB3OYZ.html
--rw-r--r--   0 ben       (1000) users      (100)     7661 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB3PYZ.html
--rw-r--r--   0 ben       (1000) users      (100)     4369 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB4DBZ.html
--rw-r--r--   0 ben       (1000) users      (100)    15077 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB4DLZ.html
--rw-r--r--   0 ben       (1000) users      (100)    18237 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB4DPZ.html
--rw-r--r--   0 ben       (1000) users      (100)     5880 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01MD.html
--rw-r--r--   0 ben       (1000) users      (100)     4529 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01ND.html
--rw-r--r--   0 ben       (1000) users      (100)     4766 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01OD.html
--rw-r--r--   0 ben       (1000) users      (100)     4743 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01PD.html
--rw-r--r--   0 ben       (1000) users      (100)     3058 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01PY.html
--rw-r--r--   0 ben       (1000) users      (100)     7907 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01QD.html
--rw-r--r--   0 ben       (1000) users      (100)     7648 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01RD.html
--rw-r--r--   0 ben       (1000) users      (100)     7121 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01SD.html
--rw-r--r--   0 ben       (1000) users      (100)     8273 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01TD.html
--rw-r--r--   0 ben       (1000) users      (100)     4837 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01VD.html
--rw-r--r--   0 ben       (1000) users      (100)     5788 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01WD.html
--rw-r--r--   0 ben       (1000) users      (100)     6217 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01XD.html
--rw-r--r--   0 ben       (1000) users      (100)    12146 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC03MD.html
--rw-r--r--   0 ben       (1000) users      (100)    15153 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC03ND.html
--rw-r--r--   0 ben       (1000) users      (100)     3563 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC03NX.html
--rw-r--r--   0 ben       (1000) users      (100)    31857 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MD03AD.html
--rw-r--r--   0 ben       (1000) users      (100)    42765 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MD03BD.html
--rw-r--r--   0 ben       (1000) users      (100)     4559 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MD03BX.html
--rw-r--r--   0 ben       (1000) users      (100)     7702 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MD03BY.html
--rw-r--r--   0 ben       (1000) users      (100)     4827 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01AD.html
--rw-r--r--   0 ben       (1000) users      (100)     4531 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01AY.html
--rw-r--r--   0 ben       (1000) users      (100)     7321 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BD.html
--rw-r--r--   0 ben       (1000) users      (100)    11887 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BP.html
--rw-r--r--   0 ben       (1000) users      (100)    10913 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BQ.html
--rw-r--r--   0 ben       (1000) users      (100)    10679 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BR.html
--rw-r--r--   0 ben       (1000) users      (100)     8905 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BS.html
--rw-r--r--   0 ben       (1000) users      (100)     5469 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BU.html
--rw-r--r--   0 ben       (1000) users      (100)     4500 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BV.html
--rw-r--r--   0 ben       (1000) users      (100)     4562 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BW.html
--rw-r--r--   0 ben       (1000) users      (100)     3600 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BX.html
--rw-r--r--   0 ben       (1000) users      (100)     5910 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BY.html
--rw-r--r--   0 ben       (1000) users      (100)   136171 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/ODESolver.html
--rw-r--r--   0 ben       (1000) users      (100)    16252 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01BD.html
--rw-r--r--   0 ben       (1000) users      (100)     3400 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01BX.html
--rw-r--r--   0 ben       (1000) users      (100)     3764 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01BY.html
--rw-r--r--   0 ben       (1000) users      (100)    11714 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01DD.html
--rw-r--r--   0 ben       (1000) users      (100)     4084 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01FY.html
--rw-r--r--   0 ben       (1000) users      (100)     8033 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01MD.html
--rw-r--r--   0 ben       (1000) users      (100)    15794 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02MD.html
--rw-r--r--   0 ben       (1000) users      (100)    12703 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02MT.html
--rw-r--r--   0 ben       (1000) users      (100)     6955 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02MU.html
--rw-r--r--   0 ben       (1000) users      (100)    14519 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02MX.html
--rw-r--r--   0 ben       (1000) users      (100)    19786 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02ND.html
--rw-r--r--   0 ben       (1000) users      (100)    22787 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02OD.html
--rw-r--r--   0 ben       (1000) users      (100)    13696 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02OY.html
--rw-r--r--   0 ben       (1000) users      (100)    12944 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02PD.html
--rw-r--r--   0 ben       (1000) users      (100)    18656 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02QD.html
--rw-r--r--   0 ben       (1000) users      (100)    29677 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02RD.html
--rw-r--r--   0 ben       (1000) users      (100)     7860 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02RU.html
--rw-r--r--   0 ben       (1000) users      (100)    20132 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02SD.html
--rw-r--r--   0 ben       (1000) users      (100)    16880 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MD.html
--rw-r--r--   0 ben       (1000) users      (100)     4787 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MU.html
--rw-r--r--   0 ben       (1000) users      (100)     4952 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MV.html
--rw-r--r--   0 ben       (1000) users      (100)     4954 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MW.html
--rw-r--r--   0 ben       (1000) users      (100)     4625 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MX.html
--rw-r--r--   0 ben       (1000) users      (100)     4346 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MY.html
--rw-r--r--   0 ben       (1000) users      (100)    19084 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OD.html
--rw-r--r--   0 ben       (1000) users      (100)     5036 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OR.html
--rw-r--r--   0 ben       (1000) users      (100)     6434 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OS.html
--rw-r--r--   0 ben       (1000) users      (100)     7554 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OT.html
--rw-r--r--   0 ben       (1000) users      (100)    11168 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OU.html
--rw-r--r--   0 ben       (1000) users      (100)     2853 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OV.html
--rw-r--r--   0 ben       (1000) users      (100)     6980 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OY.html
--rw-r--r--   0 ben       (1000) users      (100)    13769 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OZ.html
--rw-r--r--   0 ben       (1000) users      (100)     8896 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03PD.html
--rw-r--r--   0 ben       (1000) users      (100)    16046 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03QD.html
--rw-r--r--   0 ben       (1000) users      (100)     6720 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03QX.html
--rw-r--r--   0 ben       (1000) users      (100)     6912 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03QY.html
--rw-r--r--   0 ben       (1000) users      (100)     8782 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03RD.html
--rw-r--r--   0 ben       (1000) users      (100)    16068 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03SD.html
--rw-r--r--   0 ben       (1000) users      (100)     6749 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03SX.html
--rw-r--r--   0 ben       (1000) users      (100)     6954 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03SY.html
--rw-r--r--   0 ben       (1000) users      (100)    18474 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03TD.html
--rw-r--r--   0 ben       (1000) users      (100)    18566 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03UD.html
--rw-r--r--   0 ben       (1000) users      (100)     8750 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04MD.html
--rw-r--r--   0 ben       (1000) users      (100)     3239 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04MR.html
--rw-r--r--   0 ben       (1000) users      (100)     3790 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04MU.html
--rw-r--r--   0 ben       (1000) users      (100)     3082 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04MW.html
--rw-r--r--   0 ben       (1000) users      (100)     3700 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04MY.html
--rw-r--r--   0 ben       (1000) users      (100)     9874 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04ND.html
--rw-r--r--   0 ben       (1000) users      (100)     3392 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04NV.html
--rw-r--r--   0 ben       (1000) users      (100)     3315 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04NW.html
--rw-r--r--   0 ben       (1000) users      (100)     4094 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04NX.html
--rw-r--r--   0 ben       (1000) users      (100)     3937 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04NY.html
--rw-r--r--   0 ben       (1000) users      (100)    23369 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04OD.html
--rw-r--r--   0 ben       (1000) users      (100)     6221 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04OW.html
--rw-r--r--   0 ben       (1000) users      (100)    17243 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04PD.html
--rw-r--r--   0 ben       (1000) users      (100)     4812 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04PX.html
--rw-r--r--   0 ben       (1000) users      (100)     5906 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04PY.html
--rw-r--r--   0 ben       (1000) users      (100)     9171 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04QD.html
--rw-r--r--   0 ben       (1000) users      (100)     3418 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04QR.html
--rw-r--r--   0 ben       (1000) users      (100)     4038 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04QU.html
--rw-r--r--   0 ben       (1000) users      (100)     3825 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04QY.html
--rw-r--r--   0 ben       (1000) users      (100)    10147 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04RD.html
--rw-r--r--   0 ben       (1000) users      (100)     4099 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04RV.html
--rw-r--r--   0 ben       (1000) users      (100)     4004 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04RW.html
--rw-r--r--   0 ben       (1000) users      (100)     4129 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04RX.html
--rw-r--r--   0 ben       (1000) users      (100)     3892 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04RY.html
--rw-r--r--   0 ben       (1000) users      (100)    10303 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB06ND.html
--rw-r--r--   0 ben       (1000) users      (100)    16757 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08CD.html
--rw-r--r--   0 ben       (1000) users      (100)    16279 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08DD.html
--rw-r--r--   0 ben       (1000) users      (100)    16704 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08ED.html
--rw-r--r--   0 ben       (1000) users      (100)    16086 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08FD.html
--rw-r--r--   0 ben       (1000) users      (100)     5887 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08GD.html
--rw-r--r--   0 ben       (1000) users      (100)     5904 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08HD.html
--rw-r--r--   0 ben       (1000) users      (100)     9740 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08MD.html
--rw-r--r--   0 ben       (1000) users      (100)     9769 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08ND.html
--rw-r--r--   0 ben       (1000) users      (100)     8466 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB09MD.html
--rw-r--r--   0 ben       (1000) users      (100)    15099 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10AD.html
--rw-r--r--   0 ben       (1000) users      (100)    17568 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10DD.html
--rw-r--r--   0 ben       (1000) users      (100)    16969 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10ED.html
--rw-r--r--   0 ben       (1000) users      (100)    19334 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10FD.html
--rw-r--r--   0 ben       (1000) users      (100)    14445 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10HD.html
--rw-r--r--   0 ben       (1000) users      (100)    12091 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10ID.html
--rw-r--r--   0 ben       (1000) users      (100)     4986 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10JD.html
--rw-r--r--   0 ben       (1000) users      (100)    12209 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10KD.html
--rw-r--r--   0 ben       (1000) users      (100)     7335 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10LD.html
--rw-r--r--   0 ben       (1000) users      (100)    11444 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10MD.html
--rw-r--r--   0 ben       (1000) users      (100)     8357 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10PD.html
--rw-r--r--   0 ben       (1000) users      (100)     8970 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10QD.html
--rw-r--r--   0 ben       (1000) users      (100)     9068 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10RD.html
--rw-r--r--   0 ben       (1000) users      (100)     9549 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10SD.html
--rw-r--r--   0 ben       (1000) users      (100)     7290 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10TD.html
--rw-r--r--   0 ben       (1000) users      (100)     7429 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10UD.html
--rw-r--r--   0 ben       (1000) users      (100)     7168 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10VD.html
--rw-r--r--   0 ben       (1000) users      (100)     6885 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10WD.html
--rw-r--r--   0 ben       (1000) users      (100)     8488 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10YD.html
--rw-r--r--   0 ben       (1000) users      (100)    13619 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10ZD.html
--rw-r--r--   0 ben       (1000) users      (100)     5413 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10ZP.html
--rw-r--r--   0 ben       (1000) users      (100)    26050 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB16AD.html
--rw-r--r--   0 ben       (1000) users      (100)    11953 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB16AY.html
--rw-r--r--   0 ben       (1000) users      (100)    20947 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB16BD.html
--rw-r--r--   0 ben       (1000) users      (100)    20320 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB16CD.html
--rw-r--r--   0 ben       (1000) users      (100)     7885 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB16CY.html
--rw-r--r--   0 ben       (1000) users      (100)    25246 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG02AD.html
--rw-r--r--   0 ben       (1000) users      (100)     9176 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG02CV.html
--rw-r--r--   0 ben       (1000) users      (100)    20509 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG02CW.html
--rw-r--r--   0 ben       (1000) users      (100)    11453 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG02CX.html
--rw-r--r--   0 ben       (1000) users      (100)    26693 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG02ND.html
--rw-r--r--   0 ben       (1000) users      (100)    18998 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03AD.html
--rw-r--r--   0 ben       (1000) users      (100)     4900 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03AX.html
--rw-r--r--   0 ben       (1000) users      (100)     4904 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03AY.html
--rw-r--r--   0 ben       (1000) users      (100)    21145 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BD.html
--rw-r--r--   0 ben       (1000) users      (100)     2202 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BR.html
--rw-r--r--   0 ben       (1000) users      (100)     8774 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BS.html
--rw-r--r--   0 ben       (1000) users      (100)     8144 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BT.html
--rw-r--r--   0 ben       (1000) users      (100)     9513 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BU.html
--rw-r--r--   0 ben       (1000) users      (100)     8957 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BV.html
--rw-r--r--   0 ben       (1000) users      (100)     5993 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BW.html
--rw-r--r--   0 ben       (1000) users      (100)     6413 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BX.html
--rw-r--r--   0 ben       (1000) users      (100)     2137 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BY.html
--rw-r--r--   0 ben       (1000) users      (100)    17385 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BZ.html
--rw-r--r--   0 ben       (1000) users      (100)    10967 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01ID.html
--rw-r--r--   0 ben       (1000) users      (100)    12670 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01IZ.html
--rw-r--r--   0 ben       (1000) users      (100)    13785 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01KD.html
--rw-r--r--   0 ben       (1000) users      (100)     6012 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01KX.html
--rw-r--r--   0 ben       (1000) users      (100)    13179 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01LD.html
--rw-r--r--   0 ben       (1000) users      (100)    10518 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01MD.html
--rw-r--r--   0 ben       (1000) users      (100)    10322 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01ND.html
--rw-r--r--   0 ben       (1000) users      (100)    11881 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01PD.html
--rw-r--r--   0 ben       (1000) users      (100)    14488 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01PX.html
--rw-r--r--   0 ben       (1000) users      (100)    11397 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01TD.html
--rw-r--r--   0 ben       (1000) users      (100)    15344 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01UD.html
--rw-r--r--   0 ben       (1000) users      (100)     8516 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01UX.html
--rw-r--r--   0 ben       (1000) users      (100)    15763 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01UY.html
--rw-r--r--   0 ben       (1000) users      (100)     7267 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01VD.html
--rw-r--r--   0 ben       (1000) users      (100)     5246 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01VY.html
--rw-r--r--   0 ben       (1000) users      (100)    10570 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01WD.html
--rw-r--r--   0 ben       (1000) users      (100)    10223 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01WX.html
--rw-r--r--   0 ben       (1000) users      (100)     5255 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01XD.html
--rw-r--r--   0 ben       (1000) users      (100)     5226 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01XZ.html
--rw-r--r--   0 ben       (1000) users      (100)     3679 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01YD.html
--rw-r--r--   0 ben       (1000) users      (100)    12176 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01ZD.html
--rw-r--r--   0 ben       (1000) users      (100)    19113 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB03AD.html
--rw-r--r--   0 ben       (1000) users      (100)    17777 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04AD.html
--rw-r--r--   0 ben       (1000) users      (100)    15787 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04BD.html
--rw-r--r--   0 ben       (1000) users      (100)     6117 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04BV.html
--rw-r--r--   0 ben       (1000) users      (100)     5382 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04BW.html
--rw-r--r--   0 ben       (1000) users      (100)     5139 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04BX.html
--rw-r--r--   0 ben       (1000) users      (100)    16621 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04CD.html
--rw-r--r--   0 ben       (1000) users      (100)    13598 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB05AD.html
--rw-r--r--   0 ben       (1000) users      (100)     8563 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TC01OD.html
--rw-r--r--   0 ben       (1000) users      (100)    14230 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TC04AD.html
--rw-r--r--   0 ben       (1000) users      (100)    11526 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TC05AD.html
--rw-r--r--   0 ben       (1000) users      (100)    22198 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TD03AD.html
--rw-r--r--   0 ben       (1000) users      (100)    15544 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TD04AD.html
--rw-r--r--   0 ben       (1000) users      (100)     6497 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TD05AD.html
--rw-r--r--   0 ben       (1000) users      (100)     9014 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01MD.html
--rw-r--r--   0 ben       (1000) users      (100)     4857 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01MX.html
--rw-r--r--   0 ben       (1000) users      (100)     5910 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01MY.html
--rw-r--r--   0 ben       (1000) users      (100)     9858 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01ND.html
--rw-r--r--   0 ben       (1000) users      (100)     6824 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01OD.html
--rw-r--r--   0 ben       (1000) users      (100)     6918 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01PD.html
--rw-r--r--   0 ben       (1000) users      (100)     9938 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01QD.html
--rw-r--r--   0 ben       (1000) users      (100)     8293 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01RD.html
--rw-r--r--   0 ben       (1000) users      (100)    13334 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01AD.html
--rw-r--r--   0 ben       (1000) users      (100)    14133 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01AZ.html
--rw-r--r--   0 ben       (1000) users      (100)     9575 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01BD.html
--rw-r--r--   0 ben       (1000) users      (100)    10163 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01CD.html
--rw-r--r--   0 ben       (1000) users      (100)    10070 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01DD.html
--rw-r--r--   0 ben       (1000) users      (100)    14972 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01ED.html
--rw-r--r--   0 ben       (1000) users      (100)    17454 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01FD.html
--rw-r--r--   0 ben       (1000) users      (100)    18546 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01FZ.html
--rw-r--r--   0 ben       (1000) users      (100)    14896 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01GD.html
--rw-r--r--   0 ben       (1000) users      (100)    23717 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01HD.html
--rw-r--r--   0 ben       (1000) users      (100)    13936 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01HU.html
--rw-r--r--   0 ben       (1000) users      (100)    12488 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01HX.html
--rw-r--r--   0 ben       (1000) users      (100)    13501 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01HY.html
--rw-r--r--   0 ben       (1000) users      (100)    24383 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01ID.html
--rw-r--r--   0 ben       (1000) users      (100)    19140 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01JD.html
--rw-r--r--   0 ben       (1000) users      (100)    22568 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01JY.html
--rw-r--r--   0 ben       (1000) users      (100)     7330 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01KD.html
--rw-r--r--   0 ben       (1000) users      (100)     7299 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01KZ.html
--rw-r--r--   0 ben       (1000) users      (100)    18445 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01LD.html
--rw-r--r--   0 ben       (1000) users      (100)    10696 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01LY.html
--rw-r--r--   0 ben       (1000) users      (100)    18837 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01MD.html
--rw-r--r--   0 ben       (1000) users      (100)    20675 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01ND.html
--rw-r--r--   0 ben       (1000) users      (100)     7633 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01NX.html
--rw-r--r--   0 ben       (1000) users      (100)     4151 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01OA.html
--rw-r--r--   0 ben       (1000) users      (100)     4170 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01OB.html
--rw-r--r--   0 ben       (1000) users      (100)     5550 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01OD.html
--rw-r--r--   0 ben       (1000) users      (100)     5569 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01OZ.html
--rw-r--r--   0 ben       (1000) users      (100)    20042 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01PD.html
--rw-r--r--   0 ben       (1000) users      (100)    20693 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01QD.html
--rw-r--r--   0 ben       (1000) users      (100)     6679 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01WD.html
--rw-r--r--   0 ben       (1000) users      (100)     6292 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01BD.html
--rw-r--r--   0 ben       (1000) users      (100)     7121 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01CD.html
--rw-r--r--   0 ben       (1000) users      (100)     5050 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01DD.html
--rw-r--r--   0 ben       (1000) users      (100)     5123 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01MD.html
--rw-r--r--   0 ben       (1000) users      (100)     3291 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01MZ.html
--rw-r--r--   0 ben       (1000) users      (100)     7217 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01ND.html
--rw-r--r--   0 ben       (1000) users      (100)     2790 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UE01MD.html
--rw-r--r--   0 ben       (1000) users      (100)      978 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/readme
--rw-r--r--   0 ben       (1000) users      (100)    42799 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/doc/support.html
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.428938 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/
--rw-r--r--   0 ben       (1000) users      (100)      124 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB01MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      464 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB01MD.res
--rw-r--r--   0 ben       (1000) users      (100)      149 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB01ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      575 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB01ND.res
--rw-r--r--   0 ben       (1000) users      (100)      321 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB01OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      539 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB01OD.res
--rw-r--r--   0 ben       (1000) users      (100)      168 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB04MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      332 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB04MD.res
--rw-r--r--   0 ben       (1000) users      (100)      376 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      839 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05MD.res
--rw-r--r--   0 ben       (1000) users      (100)      370 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      842 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05ND.res
--rw-r--r--   0 ben       (1000) users      (100)      376 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      986 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05OD.res
--rw-r--r--   0 ben       (1000) users      (100)      380 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05PD.dat
--rw-r--r--   0 ben       (1000) users      (100)      842 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05PD.res
--rw-r--r--   0 ben       (1000) users      (100)      382 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05QD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1170 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05QD.res
--rw-r--r--   0 ben       (1000) users      (100)      356 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05RD.dat
--rw-r--r--   0 ben       (1000) users      (100)      567 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05RD.res
--rw-r--r--   0 ben       (1000) users      (100)      179 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB07MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      368 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB07MD.res
--rw-r--r--   0 ben       (1000) users      (100)      200 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB07ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      475 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB07ND.res
--rw-r--r--   0 ben       (1000) users      (100)      510 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB08ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      877 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB08ND.res
--rw-r--r--   0 ben       (1000) users      (100)      510 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB08NW.dat
--rw-r--r--   0 ben       (1000) users      (100)      913 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB08NW.res
--rw-r--r--   0 ben       (1000) users      (100)      868 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB08NZ.dat
--rw-r--r--   0 ben       (1000) users      (100)      923 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB08NZ.res
--rw-r--r--   0 ben       (1000) users      (100)      820 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      754 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09AD.res
--rw-r--r--   0 ben       (1000) users      (100)      888 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09BD.dat
--rw-r--r--   0 ben       (1000) users      (100)      848 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09BD.res
--rw-r--r--   0 ben       (1000) users      (100)      876 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09CD.dat
--rw-r--r--   0 ben       (1000) users      (100)      848 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09CD.res
--rw-r--r--   0 ben       (1000) users      (100)      927 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09DD.dat
--rw-r--r--   0 ben       (1000) users      (100)      775 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09DD.res
--rw-r--r--   0 ben       (1000) users      (100)      865 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09ED.dat
--rw-r--r--   0 ben       (1000) users      (100)      851 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09ED.res
--rw-r--r--   0 ben       (1000) users      (100)      815 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09FD.dat
--rw-r--r--   0 ben       (1000) users      (100)      769 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09FD.res
--rw-r--r--   0 ben       (1000) users      (100)      882 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09GD.dat
--rw-r--r--   0 ben       (1000) users      (100)      867 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09GD.res
--rw-r--r--   0 ben       (1000) users      (100)      882 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09HD.dat
--rw-r--r--   0 ben       (1000) users      (100)      880 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09HD.res
--rw-r--r--   0 ben       (1000) users      (100)      736 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09ID.dat
--rw-r--r--   0 ben       (1000) users      (100)      401 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09ID.res
--rw-r--r--   0 ben       (1000) users      (100)      716 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09JD.dat
--rw-r--r--   0 ben       (1000) users      (100)      585 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09JD.res
--rw-r--r--   0 ben       (1000) users      (100)      713 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09KD.dat
--rw-r--r--   0 ben       (1000) users      (100)      585 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09KD.res
--rw-r--r--   0 ben       (1000) users      (100)      807 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      753 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09MD.res
--rw-r--r--   0 ben       (1000) users      (100)      875 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      851 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09ND.res
--rw-r--r--   0 ben       (1000) users      (100)      787 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      208 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13AD.res
--rw-r--r--   0 ben       (1000) users      (100)      855 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13BD.dat
--rw-r--r--   0 ben       (1000) users      (100)       77 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13BD.res
--rw-r--r--   0 ben       (1000) users      (100)      394 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13CD.dat
--rw-r--r--   0 ben       (1000) users      (100)      131 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13CD.res
--rw-r--r--   0 ben       (1000) users      (100)      436 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13DD.dat
--rw-r--r--   0 ben       (1000) users      (100)      131 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13DD.res
--rw-r--r--   0 ben       (1000) users      (100)      257 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13ED.dat
--rw-r--r--   0 ben       (1000) users      (100)      611 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13ED.res
--rw-r--r--   0 ben       (1000) users      (100)      282 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13FD.dat
--rw-r--r--   0 ben       (1000) users      (100)      471 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13FD.res
--rw-r--r--   0 ben       (1000) users      (100)     1302 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13ID.dat
--rw-r--r--   0 ben       (1000) users      (100)     1435 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13ID.res
--rw-r--r--   0 ben       (1000) users      (100)      700 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13MD.dat
--rw-r--r--   0 ben       (1000) users      (100)       99 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13MD.res
--rw-r--r--   0 ben       (1000) users      (100)     1450 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AG08BD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1701 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AG08BD.res
--rw-r--r--   0 ben       (1000) users      (100)     1942 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AG08BZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     1736 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AG08BZ.res
--rw-r--r--   0 ben       (1000) users      (100)       72 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BB01AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      517 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BB01AD.res
--rw-r--r--   0 ben       (1000) users      (100)       74 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BB02AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      499 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BB02AD.res
--rw-r--r--   0 ben       (1000) users      (100)       52 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BB03AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      998 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BB03AD.res
--rw-r--r--   0 ben       (1000) users      (100)       52 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BB04AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      998 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BB04AD.res
--rw-r--r--   0 ben       (1000) users      (100)       34 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BD01AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      396 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BD01AD.res
--rw-r--r--   0 ben       (1000) users      (100)       34 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BD02AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      377 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BD02AD.res
--rw-r--r--   0 ben       (1000) users      (100)      192 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DE01OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      176 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DE01OD.res
--rw-r--r--   0 ben       (1000) users      (100)      198 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DE01PD.dat
--rw-r--r--   0 ben       (1000) users      (100)      176 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DE01PD.res
--rw-r--r--   0 ben       (1000) users      (100)      218 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DF01MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      358 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DF01MD.res
--rw-r--r--   0 ben       (1000) users      (100)      192 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DG01MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      315 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DG01MD.res
--rw-r--r--   0 ben       (1000) users      (100)      200 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DG01ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      342 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DG01ND.res
--rw-r--r--   0 ben       (1000) users      (100)      115 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DG01OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      294 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DG01OD.res
--rw-r--r--   0 ben       (1000) users      (100)      120 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DK01MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      220 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/DK01MD.res
--rw-r--r--   0 ben       (1000) users      (100)      550 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01QD.dat
--rw-r--r--   0 ben       (1000) users      (100)      338 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01QD.res
--rw-r--r--   0 ben       (1000) users      (100)      550 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01RD.dat
--rw-r--r--   0 ben       (1000) users      (100)      338 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01RD.res
--rw-r--r--   0 ben       (1000) users      (100)      636 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01SD.dat
--rw-r--r--   0 ben       (1000) users      (100)      384 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01SD.res
--rw-r--r--   0 ben       (1000) users      (100)      630 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01TD.dat
--rw-r--r--   0 ben       (1000) users      (100)      384 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01TD.res
--rw-r--r--   0 ben       (1000) users      (100)      612 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01VD.dat
--rw-r--r--   0 ben       (1000) users      (100)      430 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01VD.res
--rw-r--r--   0 ben       (1000) users      (100)       50 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FD01AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      223 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FD01AD.res
--rw-r--r--   0 ben       (1000) users      (100)    20108 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB01AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      230 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB01AD.res
--rw-r--r--   0 ben       (1000) users      (100)    20119 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB01BD.dat
--rw-r--r--   0 ben       (1000) users      (100)      796 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB01BD.res
--rw-r--r--   0 ben       (1000) users      (100)    20125 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB01CD.dat
--rw-r--r--   0 ben       (1000) users      (100)      475 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB01CD.res
--rw-r--r--   0 ben       (1000) users      (100)    34954 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB03AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      780 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB03AD.res
--rw-r--r--   0 ben       (1000) users      (100)    34946 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB03BD.dat
--rw-r--r--   0 ben       (1000) users      (100)      812 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB03BD.res
--rw-r--r--   0 ben       (1000) users      (100)      334 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB01TD.dat
--rw-r--r--   0 ben       (1000) users      (100)      291 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB01TD.res
--rw-r--r--   0 ben       (1000) users      (100)      161 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02CD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1076 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02CD.res
--rw-r--r--   0 ben       (1000) users      (100)      262 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02DD.dat
--rw-r--r--   0 ben       (1000) users      (100)     3296 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02DD.res
--rw-r--r--   0 ben       (1000) users      (100)      516 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02ED.dat
--rw-r--r--   0 ben       (1000) users      (100)      233 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02ED.res
--rw-r--r--   0 ben       (1000) users      (100)      185 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02FD.dat
--rw-r--r--   0 ben       (1000) users      (100)      509 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02FD.res
--rw-r--r--   0 ben       (1000) users      (100)      165 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02GD.dat
--rw-r--r--   0 ben       (1000) users      (100)      452 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02GD.res
--rw-r--r--   0 ben       (1000) users      (100)      196 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02HD.dat
--rw-r--r--   0 ben       (1000) users      (100)      812 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02HD.res
--rw-r--r--   0 ben       (1000) users      (100)      522 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02ID.dat
--rw-r--r--   0 ben       (1000) users      (100)      304 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02ID.res
--rw-r--r--   0 ben       (1000) users      (100)      351 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02JD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1312 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02JD.res
--rw-r--r--   0 ben       (1000) users      (100)      657 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02JX.dat
--rw-r--r--   0 ben       (1000) users      (100)     1728 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02JX.res
--rw-r--r--   0 ben       (1000) users      (100)      551 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02KD.dat
--rw-r--r--   0 ben       (1000) users      (100)      180 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02KD.res
--rw-r--r--   0 ben       (1000) users      (100)      287 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      227 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02MD.res
--rw-r--r--   0 ben       (1000) users      (100)      307 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      776 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02ND.res
--rw-r--r--   0 ben       (1000) users      (100)      190 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02QD.dat
--rw-r--r--   0 ben       (1000) users      (100)      220 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02QD.res
--rw-r--r--   0 ben       (1000) users      (100)      323 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02SD.dat
--rw-r--r--   0 ben       (1000) users      (100)      288 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02SD.res
--rw-r--r--   0 ben       (1000) users      (100)      262 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02VD.dat
--rw-r--r--   0 ben       (1000) users      (100)      243 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02VD.res
--rw-r--r--   0 ben       (1000) users      (100)      250 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03BD.dat
--rw-r--r--   0 ben       (1000) users      (100)      889 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03BD.res
--rw-r--r--   0 ben       (1000) users      (100)      925 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03BZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     2500 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03BZ.res
--rw-r--r--   0 ben       (1000) users      (100)      515 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03FZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     2448 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03FZ.res
--rw-r--r--   0 ben       (1000) users      (100)      254 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03KD.dat
--rw-r--r--   0 ben       (1000) users      (100)      880 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03KD.res
--rw-r--r--   0 ben       (1000) users      (100)      709 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03LD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1177 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03LD.res
--rw-r--r--   0 ben       (1000) users      (100)     1018 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03LF.dat
--rw-r--r--   0 ben       (1000) users      (100)     1516 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03LF.res
--rw-r--r--   0 ben       (1000) users      (100)      410 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03LZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     2008 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03LZ.res
--rw-r--r--   0 ben       (1000) users      (100)      114 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      298 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03MD.res
--rw-r--r--   0 ben       (1000) users      (100)      107 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      259 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03ND.res
--rw-r--r--   0 ben       (1000) users      (100)      242 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      153 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03OD.res
--rw-r--r--   0 ben       (1000) users      (100)      242 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03PD.dat
--rw-r--r--   0 ben       (1000) users      (100)      155 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03PD.res
--rw-r--r--   0 ben       (1000) users      (100)      176 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03QD.dat
--rw-r--r--   0 ben       (1000) users      (100)      511 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03QD.res
--rw-r--r--   0 ben       (1000) users      (100)      283 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03QG.dat
--rw-r--r--   0 ben       (1000) users      (100)      943 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03QG.res
--rw-r--r--   0 ben       (1000) users      (100)      478 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03RD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1458 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03RD.res
--rw-r--r--   0 ben       (1000) users      (100)      143 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03SD.dat
--rw-r--r--   0 ben       (1000) users      (100)      200 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03SD.res
--rw-r--r--   0 ben       (1000) users      (100)      897 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03TD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1689 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03TD.res
--rw-r--r--   0 ben       (1000) users      (100)      147 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03UD.dat
--rw-r--r--   0 ben       (1000) users      (100)      556 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03UD.res
--rw-r--r--   0 ben       (1000) users      (100)      168 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03VD.dat
--rw-r--r--   0 ben       (1000) users      (100)      691 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03VD.res
--rw-r--r--   0 ben       (1000) users      (100)      176 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03WD.dat
--rw-r--r--   0 ben       (1000) users      (100)      895 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03WD.res
--rw-r--r--   0 ben       (1000) users      (100)     1424 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XD.dat
--rw-r--r--   0 ben       (1000) users      (100)     6093 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XD.res
--rw-r--r--   0 ben       (1000) users      (100)     1350 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XP.dat
--rw-r--r--   0 ben       (1000) users      (100)     3194 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XP.res
--rw-r--r--   0 ben       (1000) users      (100)      694 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     8586 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XZ.res
--rw-r--r--   0 ben       (1000) users      (100)     3578 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03ZD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1515 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03ZD.res
--rw-r--r--   0 ben       (1000) users      (100)     1333 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04AD.dat
--rw-r--r--   0 ben       (1000) users      (100)     3991 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04AD.res
--rw-r--r--   0 ben       (1000) users      (100)      515 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04AZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     4121 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04AZ.res
--rw-r--r--   0 ben       (1000) users      (100)      713 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04BD.dat
--rw-r--r--   0 ben       (1000) users      (100)     2623 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04BD.res
--rw-r--r--   0 ben       (1000) users      (100)      405 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04BZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     3043 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04BZ.res
--rw-r--r--   0 ben       (1000) users      (100)      837 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1166 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DD.res
--rw-r--r--   0 ben       (1000) users      (100)      382 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DL.dat
--rw-r--r--   0 ben       (1000) users      (100)      944 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DL.res
--rw-r--r--   0 ben       (1000) users      (100)      262 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DP.dat
--rw-r--r--   0 ben       (1000) users      (100)      780 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DP.res
--rw-r--r--   0 ben       (1000) users      (100)      837 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DS.dat
--rw-r--r--   0 ben       (1000) users      (100)      932 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DS.res
--rw-r--r--   0 ben       (1000) users      (100)      187 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DY.dat
--rw-r--r--   0 ben       (1000) users      (100)      493 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DY.res
--rw-r--r--   0 ben       (1000) users      (100)      867 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     1790 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DZ.res
--rw-r--r--   0 ben       (1000) users      (100)     1047 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04ED.dat
--rw-r--r--   0 ben       (1000) users      (100)     2192 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04ED.res
--rw-r--r--   0 ben       (1000) users      (100)      776 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04FD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1600 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04FD.res
--rw-r--r--   0 ben       (1000) users      (100)      256 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04GD.dat
--rw-r--r--   0 ben       (1000) users      (100)      380 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04GD.res
--rw-r--r--   0 ben       (1000) users      (100)      141 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      295 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04MD.res
--rw-r--r--   0 ben       (1000) users      (100)      202 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      328 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04OD.res
--rw-r--r--   0 ben       (1000) users      (100)      598 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04PB.dat
--rw-r--r--   0 ben       (1000) users      (100)     1789 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04PB.res
--rw-r--r--   0 ben       (1000) users      (100)      598 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04PU.dat
--rw-r--r--   0 ben       (1000) users      (100)     1789 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04PU.res
--rw-r--r--   0 ben       (1000) users      (100)     1074 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04TB.dat
--rw-r--r--   0 ben       (1000) users      (100)     3303 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04TB.res
--rw-r--r--   0 ben       (1000) users      (100)     1074 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04TS.dat
--rw-r--r--   0 ben       (1000) users      (100)     3303 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04TS.res
--rw-r--r--   0 ben       (1000) users      (100)      224 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04UD.dat
--rw-r--r--   0 ben       (1000) users      (100)      457 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04UD.res
--rw-r--r--   0 ben       (1000) users      (100)      142 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04VD.dat
--rw-r--r--   0 ben       (1000) users      (100)      885 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04VD.res
--rw-r--r--   0 ben       (1000) users      (100)      313 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04XD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1129 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04XD.res
--rw-r--r--   0 ben       (1000) users      (100)      132 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04YD.dat
--rw-r--r--   0 ben       (1000) users      (100)      268 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04YD.res
--rw-r--r--   0 ben       (1000) users      (100)      117 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04ZD.dat
--rw-r--r--   0 ben       (1000) users      (100)      865 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04ZD.res
--rw-r--r--   0 ben       (1000) users      (100)      142 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB05MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      715 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB05MD.res
--rw-r--r--   0 ben       (1000) users      (100)      208 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB05ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      554 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB05ND.res
--rw-r--r--   0 ben       (1000) users      (100)      105 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB05OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      320 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB05OD.res
--rw-r--r--   0 ben       (1000) users      (100)      382 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB4DLZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     1251 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB4DLZ.res
--rw-r--r--   0 ben       (1000) users      (100)      261 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB4DPZ.dat
--rw-r--r--   0 ben       (1000) users      (100)      971 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB4DPZ.res
--rw-r--r--   0 ben       (1000) users      (100)       80 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      349 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01MD.res
--rw-r--r--   0 ben       (1000) users      (100)       81 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      132 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01ND.res
--rw-r--r--   0 ben       (1000) users      (100)       99 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      355 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01OD.res
--rw-r--r--   0 ben       (1000) users      (100)       99 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01PD.dat
--rw-r--r--   0 ben       (1000) users      (100)      265 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01PD.res
--rw-r--r--   0 ben       (1000) users      (100)       85 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01QD.dat
--rw-r--r--   0 ben       (1000) users      (100)      287 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01QD.res
--rw-r--r--   0 ben       (1000) users      (100)      101 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01RD.dat
--rw-r--r--   0 ben       (1000) users      (100)      245 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01RD.res
--rw-r--r--   0 ben       (1000) users      (100)       78 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01SD.dat
--rw-r--r--   0 ben       (1000) users      (100)      382 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01SD.res
--rw-r--r--   0 ben       (1000) users      (100)       68 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01TD.dat
--rw-r--r--   0 ben       (1000) users      (100)      126 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01TD.res
--rw-r--r--   0 ben       (1000) users      (100)       47 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01VD.dat
--rw-r--r--   0 ben       (1000) users      (100)      128 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01VD.res
--rw-r--r--   0 ben       (1000) users      (100)       92 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01WD.dat
--rw-r--r--   0 ben       (1000) users      (100)      387 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01WD.res
--rw-r--r--   0 ben       (1000) users      (100)      109 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01XD.dat
--rw-r--r--   0 ben       (1000) users      (100)      316 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC01XD.res
--rw-r--r--   0 ben       (1000) users      (100)      310 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC03MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      458 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC03MD.res
--rw-r--r--   0 ben       (1000) users      (100)      429 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC03ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      608 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC03ND.res
--rw-r--r--   0 ben       (1000) users      (100)      104 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MD03AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      211 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MD03AD.res
--rw-r--r--   0 ben       (1000) users      (100)      137 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MD03BD.dat
--rw-r--r--   0 ben       (1000) users      (100)      243 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MD03BD.res
--rw-r--r--   0 ben       (1000) users      (100)      367 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB01BD.dat
--rw-r--r--   0 ben       (1000) users      (100)      461 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB01BD.res
--rw-r--r--   0 ben       (1000) users      (100)      274 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB01DD.dat
--rw-r--r--   0 ben       (1000) users      (100)      139 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB01DD.res
--rw-r--r--   0 ben       (1000) users      (100)      202 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB01MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      118 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB01MD.res
--rw-r--r--   0 ben       (1000) users      (100)      142 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      113 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02MD.res
--rw-r--r--   0 ben       (1000) users      (100)      173 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      153 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02ND.res
--rw-r--r--   0 ben       (1000) users      (100)      185 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02OD.dat
--rw-r--r--   0 ben       (1000) users      (100)       98 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02OD.res
--rw-r--r--   0 ben       (1000) users      (100)      131 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02PD.dat
--rw-r--r--   0 ben       (1000) users      (100)      196 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02PD.res
--rw-r--r--   0 ben       (1000) users      (100)      142 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02QD.dat
--rw-r--r--   0 ben       (1000) users      (100)      217 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02QD.res
--rw-r--r--   0 ben       (1000) users      (100)      166 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02RD.dat
--rw-r--r--   0 ben       (1000) users      (100)      218 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02RD.res
--rw-r--r--   0 ben       (1000) users      (100)      136 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02SD.dat
--rw-r--r--   0 ben       (1000) users      (100)      217 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB02SD.res
--rw-r--r--   0 ben       (1000) users      (100)      172 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      172 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03MD.res
--rw-r--r--   0 ben       (1000) users      (100)      286 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      390 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03OD.res
--rw-r--r--   0 ben       (1000) users      (100)      178 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03QD.dat
--rw-r--r--   0 ben       (1000) users      (100)      291 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03QD.res
--rw-r--r--   0 ben       (1000) users      (100)      178 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03SD.dat
--rw-r--r--   0 ben       (1000) users      (100)      291 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03SD.res
--rw-r--r--   0 ben       (1000) users      (100)      178 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03TD.dat
--rw-r--r--   0 ben       (1000) users      (100)      291 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03TD.res
--rw-r--r--   0 ben       (1000) users      (100)      178 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03UD.dat
--rw-r--r--   0 ben       (1000) users      (100)      291 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB03UD.res
--rw-r--r--   0 ben       (1000) users      (100)      162 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      185 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04MD.res
--rw-r--r--   0 ben       (1000) users      (100)      373 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      200 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04ND.res
--rw-r--r--   0 ben       (1000) users      (100)      340 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      621 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04OD.res
--rw-r--r--   0 ben       (1000) users      (100)      198 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04PD.dat
--rw-r--r--   0 ben       (1000) users      (100)      327 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04PD.res
--rw-r--r--   0 ben       (1000) users      (100)      235 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04QD.dat
--rw-r--r--   0 ben       (1000) users      (100)      258 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04QD.res
--rw-r--r--   0 ben       (1000) users      (100)      531 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04RD.dat
--rw-r--r--   0 ben       (1000) users      (100)      290 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04RD.res
--rw-r--r--   0 ben       (1000) users      (100)      315 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB06ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      161 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB06ND.res
--rw-r--r--   0 ben       (1000) users      (100)      853 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08CD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1452 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08CD.res
--rw-r--r--   0 ben       (1000) users      (100)      853 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08DD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1369 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08DD.res
--rw-r--r--   0 ben       (1000) users      (100)      858 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08ED.dat
--rw-r--r--   0 ben       (1000) users      (100)     1452 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08ED.res
--rw-r--r--   0 ben       (1000) users      (100)      858 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08FD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1369 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08FD.res
--rw-r--r--   0 ben       (1000) users      (100)       64 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      417 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08MD.res
--rw-r--r--   0 ben       (1000) users      (100)       57 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      365 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08ND.res
--rw-r--r--   0 ben       (1000) users      (100)      190 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB09MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      264 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB09MD.res
--rw-r--r--   0 ben       (1000) users      (100)      729 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10DD.dat
--rw-r--r--   0 ben       (1000) users      (100)      913 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10DD.res
--rw-r--r--   0 ben       (1000) users      (100)      721 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10ED.dat
--rw-r--r--   0 ben       (1000) users      (100)      899 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10ED.res
--rw-r--r--   0 ben       (1000) users      (100)      726 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10FD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1290 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10FD.res
--rw-r--r--   0 ben       (1000) users      (100)      721 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10HD.dat
--rw-r--r--   0 ben       (1000) users      (100)      987 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10HD.res
--rw-r--r--   0 ben       (1000) users      (100)      452 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10ID.dat
--rw-r--r--   0 ben       (1000) users      (100)      816 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10ID.res
--rw-r--r--   0 ben       (1000) users      (100)      389 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10KD.dat
--rw-r--r--   0 ben       (1000) users      (100)      860 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10KD.res
--rw-r--r--   0 ben       (1000) users      (100)      462 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10ZD.dat
--rw-r--r--   0 ben       (1000) users      (100)      959 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10ZD.res
--rw-r--r--   0 ben       (1000) users      (100)      349 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB16AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      450 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB16AD.res
--rw-r--r--   0 ben       (1000) users      (100)     1097 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB16BD.dat
--rw-r--r--   0 ben       (1000) users      (100)      641 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB16BD.res
--rw-r--r--   0 ben       (1000) users      (100)     1289 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB16CD.dat
--rw-r--r--   0 ben       (1000) users      (100)      431 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB16CD.res
--rw-r--r--   0 ben       (1000) users      (100)      221 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SG02AD.dat
--rw-r--r--   0 ben       (1000) users      (100)       98 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SG02AD.res
--rw-r--r--   0 ben       (1000) users      (100)      197 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SG02ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      153 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SG02ND.res
--rw-r--r--   0 ben       (1000) users      (100)      272 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SG03AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      199 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SG03AD.res
--rw-r--r--   0 ben       (1000) users      (100)      209 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SG03BD.dat
--rw-r--r--   0 ben       (1000) users      (100)      185 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SG03BD.res
--rw-r--r--   0 ben       (1000) users      (100)     2609 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     3661 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB01ND.f
--rw-r--r--   0 ben       (1000) users      (100)     2876 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     3191 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB04MD.f
--rw-r--r--   0 ben       (1000) users      (100)     5048 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05MD.f
--rw-r--r--   0 ben       (1000) users      (100)     4743 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05ND.f
--rw-r--r--   0 ben       (1000) users      (100)     5039 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05OD.f
--rw-r--r--   0 ben       (1000) users      (100)     4542 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05PD.f
--rw-r--r--   0 ben       (1000) users      (100)     5440 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05QD.f
--rw-r--r--   0 ben       (1000) users      (100)     5738 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05RD.f
--rw-r--r--   0 ben       (1000) users      (100)     3310 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB07MD.f
--rw-r--r--   0 ben       (1000) users      (100)     2918 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB07ND.f
--rw-r--r--   0 ben       (1000) users      (100)     8781 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB08ND.f
--rw-r--r--   0 ben       (1000) users      (100)     9589 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB08NW.f
--rw-r--r--   0 ben       (1000) users      (100)     8818 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB08NZ.f
--rw-r--r--   0 ben       (1000) users      (100)     3481 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09AD.f
--rw-r--r--   0 ben       (1000) users      (100)     3936 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09BD.f
--rw-r--r--   0 ben       (1000) users      (100)     4168 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09CD.f
--rw-r--r--   0 ben       (1000) users      (100)     3430 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09DD.f
--rw-r--r--   0 ben       (1000) users      (100)     4356 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09ED.f
--rw-r--r--   0 ben       (1000) users      (100)     3655 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09FD.f
--rw-r--r--   0 ben       (1000) users      (100)     4046 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09GD.f
--rw-r--r--   0 ben       (1000) users      (100)     4278 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09HD.f
--rw-r--r--   0 ben       (1000) users      (100)     9369 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09ID.f
--rw-r--r--   0 ben       (1000) users      (100)     8111 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09JD.f
--rw-r--r--   0 ben       (1000) users      (100)     7213 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09KD.f
--rw-r--r--   0 ben       (1000) users      (100)     3557 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09MD.f
--rw-r--r--   0 ben       (1000) users      (100)     4017 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09ND.f
--rw-r--r--   0 ben       (1000) users      (100)     2702 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13AD.f
--rw-r--r--   0 ben       (1000) users      (100)     3017 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13BD.f
--rw-r--r--   0 ben       (1000) users      (100)     3095 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13CD.f
--rw-r--r--   0 ben       (1000) users      (100)     3885 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13DD.f
--rw-r--r--   0 ben       (1000) users      (100)     1660 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13ED.f
--rw-r--r--   0 ben       (1000) users      (100)     1809 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13FD.f
--rw-r--r--   0 ben       (1000) users      (100)     4964 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13ID.f
--rw-r--r--   0 ben       (1000) users      (100)     2381 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13MD.f
--rw-r--r--   0 ben       (1000) users      (100)    17103 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAG08BD.f
--rw-r--r--   0 ben       (1000) users      (100)    16231 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAG08BZ.f
--rw-r--r--   0 ben       (1000) users      (100)      856 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01ID.dat
--rw-r--r--   0 ben       (1000) users      (100)     1520 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01ID.res
--rw-r--r--   0 ben       (1000) users      (100)     1202 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01IZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     2874 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01IZ.res
--rw-r--r--   0 ben       (1000) users      (100)      545 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01KD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1147 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01KD.res
--rw-r--r--   0 ben       (1000) users      (100)      545 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01LD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1140 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01LD.res
--rw-r--r--   0 ben       (1000) users      (100)      388 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      611 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01MD.res
--rw-r--r--   0 ben       (1000) users      (100)      300 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      482 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01ND.res
--rw-r--r--   0 ben       (1000) users      (100)      180 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01PD.dat
--rw-r--r--   0 ben       (1000) users      (100)      448 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01PD.res
--rw-r--r--   0 ben       (1000) users      (100)      180 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01PX.dat
--rw-r--r--   0 ben       (1000) users      (100)      513 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01PX.res
--rw-r--r--   0 ben       (1000) users      (100)      350 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01TD.dat
--rw-r--r--   0 ben       (1000) users      (100)      728 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01TD.res
--rw-r--r--   0 ben       (1000) users      (100)      193 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01UD.dat
--rw-r--r--   0 ben       (1000) users      (100)      687 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01UD.res
--rw-r--r--   0 ben       (1000) users      (100)      199 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01UY.dat
--rw-r--r--   0 ben       (1000) users      (100)      690 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01UY.res
--rw-r--r--   0 ben       (1000) users      (100)      518 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01WD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1078 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01WD.res
--rw-r--r--   0 ben       (1000) users      (100)      524 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01WX.dat
--rw-r--r--   0 ben       (1000) users      (100)      914 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01WX.res
--rw-r--r--   0 ben       (1000) users      (100)      168 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01ZD.dat
--rw-r--r--   0 ben       (1000) users      (100)      582 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01ZD.res
--rw-r--r--   0 ben       (1000) users      (100)      193 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB03AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      805 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB03AD.res
--rw-r--r--   0 ben       (1000) users      (100)      227 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB04AD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1308 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB04AD.res
--rw-r--r--   0 ben       (1000) users      (100)      232 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB04BD.dat
--rw-r--r--   0 ben       (1000) users      (100)      667 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB04BD.res
--rw-r--r--   0 ben       (1000) users      (100)      226 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB04CD.dat
--rw-r--r--   0 ben       (1000) users      (100)      972 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB04CD.res
--rw-r--r--   0 ben       (1000) users      (100)      186 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB05AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      298 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB05AD.res
--rw-r--r--   0 ben       (1000) users      (100)     6131 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBB01AD.f
--rw-r--r--   0 ben       (1000) users      (100)     6421 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBB02AD.f
--rw-r--r--   0 ben       (1000) users      (100)     3572 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBB03AD.f
--rw-r--r--   0 ben       (1000) users      (100)     3572 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBB04AD.f
--rw-r--r--   0 ben       (1000) users      (100)     3189 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBD01AD.f
--rw-r--r--   0 ben       (1000) users      (100)     3184 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBD02AD.f
--rw-r--r--   0 ben       (1000) users      (100)      204 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TC01OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      513 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TC01OD.res
--rw-r--r--   0 ben       (1000) users      (100)      209 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TC04AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      582 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TC04AD.res
--rw-r--r--   0 ben       (1000) users      (100)      223 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TC05AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      153 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TC05AD.res
--rw-r--r--   0 ben       (1000) users      (100)      227 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TD03AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      954 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TD03AD.res
--rw-r--r--   0 ben       (1000) users      (100)      215 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TD04AD.dat
--rw-r--r--   0 ben       (1000) users      (100)      673 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TD04AD.res
--rw-r--r--   0 ben       (1000) users      (100)      122 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TD05AD.dat
--rw-r--r--   0 ben       (1000) users      (100)       79 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TD05AD.res
--rw-r--r--   0 ben       (1000) users      (100)     1626 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDE01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     1656 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDE01PD.f
--rw-r--r--   0 ben       (1000) users      (100)     1865 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDF01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     1453 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDG01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     1796 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDG01ND.f
--rw-r--r--   0 ben       (1000) users      (100)     1370 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDG01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     1396 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDK01MD.f
--rw-r--r--   0 ben       (1000) users      (100)      467 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      443 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01MD.res
--rw-r--r--   0 ben       (1000) users      (100)      473 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      443 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01ND.res
--rw-r--r--   0 ben       (1000) users      (100)      222 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01OD.dat
--rw-r--r--   0 ben       (1000) users      (100)      390 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01OD.res
--rw-r--r--   0 ben       (1000) users      (100)      222 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01PD.dat
--rw-r--r--   0 ben       (1000) users      (100)      390 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01PD.res
--rw-r--r--   0 ben       (1000) users      (100)      203 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01QD.dat
--rw-r--r--   0 ben       (1000) users      (100)      515 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01QD.res
--rw-r--r--   0 ben       (1000) users      (100)      213 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01RD.dat
--rw-r--r--   0 ben       (1000) users      (100)      350 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01RD.res
--rw-r--r--   0 ben       (1000) users      (100)     4289 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFB01QD.f
--rw-r--r--   0 ben       (1000) users      (100)     4324 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFB01RD.f
--rw-r--r--   0 ben       (1000) users      (100)     4826 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFB01SD.f
--rw-r--r--   0 ben       (1000) users      (100)     4921 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFB01TD.f
--rw-r--r--   0 ben       (1000) users      (100)     3470 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFB01VD.f
--rw-r--r--   0 ben       (1000) users      (100)     4073 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFD01AD.f
--rw-r--r--   0 ben       (1000) users      (100)      529 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01AD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1058 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01AD.res
--rw-r--r--   0 ben       (1000) users      (100)      656 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01AZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     1586 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01AZ.res
--rw-r--r--   0 ben       (1000) users      (100)      306 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01CD.dat
--rw-r--r--   0 ben       (1000) users      (100)      732 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01CD.res
--rw-r--r--   0 ben       (1000) users      (100)      304 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01DD.dat
--rw-r--r--   0 ben       (1000) users      (100)      728 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01DD.res
--rw-r--r--   0 ben       (1000) users      (100)      363 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01ED.dat
--rw-r--r--   0 ben       (1000) users      (100)     1098 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01ED.res
--rw-r--r--   0 ben       (1000) users      (100)      363 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01FD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1098 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01FD.res
--rw-r--r--   0 ben       (1000) users      (100)      555 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01FZ.dat
--rw-r--r--   0 ben       (1000) users      (100)     1898 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01FZ.res
--rw-r--r--   0 ben       (1000) users      (100)      395 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01GD.dat
--rw-r--r--   0 ben       (1000) users      (100)      571 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01GD.res
--rw-r--r--   0 ben       (1000) users      (100)      878 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01HD.dat
--rw-r--r--   0 ben       (1000) users      (100)     2565 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01HD.res
--rw-r--r--   0 ben       (1000) users      (100)      879 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01ID.dat
--rw-r--r--   0 ben       (1000) users      (100)     2565 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01ID.res
--rw-r--r--   0 ben       (1000) users      (100)     1280 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01JD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1589 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01JD.res
--rw-r--r--   0 ben       (1000) users      (100)     1299 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01JY.dat
--rw-r--r--   0 ben       (1000) users      (100)     1511 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01JY.res
--rw-r--r--   0 ben       (1000) users      (100)      370 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01LD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1146 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01LD.res
--rw-r--r--   0 ben       (1000) users      (100)      364 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01MD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1298 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01MD.res
--rw-r--r--   0 ben       (1000) users      (100)      370 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01ND.dat
--rw-r--r--   0 ben       (1000) users      (100)     1295 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01ND.res
--rw-r--r--   0 ben       (1000) users      (100)      411 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01PD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1202 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01PD.res
--rw-r--r--   0 ben       (1000) users      (100)      387 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01QD.dat
--rw-r--r--   0 ben       (1000) users      (100)     1305 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01QD.res
--rw-r--r--   0 ben       (1000) users      (100)     4674 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TIB01AD.f
--rw-r--r--   0 ben       (1000) users      (100)    10136 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TIB01BD.f
--rw-r--r--   0 ben       (1000) users      (100)    11013 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TIB01CD.f
--rw-r--r--   0 ben       (1000) users      (100)    10254 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TIB03AD.f
--rw-r--r--   0 ben       (1000) users      (100)    10794 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TIB03BD.f
--rw-r--r--   0 ben       (1000) users      (100)     1597 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB01TD.f
--rw-r--r--   0 ben       (1000) users      (100)     3338 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02CD.f
--rw-r--r--   0 ben       (1000) users      (100)     6602 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02DD.f
--rw-r--r--   0 ben       (1000) users      (100)     3281 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02ED.f
--rw-r--r--   0 ben       (1000) users      (100)     5862 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02FD.f
--rw-r--r--   0 ben       (1000) users      (100)     2407 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02GD.f
--rw-r--r--   0 ben       (1000) users      (100)     3214 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02HD.f
--rw-r--r--   0 ben       (1000) users      (100)     3747 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02ID.f
--rw-r--r--   0 ben       (1000) users      (100)     3046 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02JD.f
--rw-r--r--   0 ben       (1000) users      (100)     3356 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02JX.f
--rw-r--r--   0 ben       (1000) users      (100)     3726 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02KD.f
--rw-r--r--   0 ben       (1000) users      (100)     3670 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02MD.f
--rw-r--r--   0 ben       (1000) users      (100)     5206 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02ND.f
--rw-r--r--   0 ben       (1000) users      (100)     3052 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02QD.f
--rw-r--r--   0 ben       (1000) users      (100)     2859 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02SD.f
--rw-r--r--   0 ben       (1000) users      (100)     1803 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02VD.f
--rw-r--r--   0 ben       (1000) users      (100)     4924 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03BD.f
--rw-r--r--   0 ben       (1000) users      (100)     3602 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03BZ.f
--rw-r--r--   0 ben       (1000) users      (100)     5398 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03FZ.f
--rw-r--r--   0 ben       (1000) users      (100)     7940 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03KD.f
--rw-r--r--   0 ben       (1000) users      (100)     4137 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03LD.f
--rw-r--r--   0 ben       (1000) users      (100)     4454 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03LF.f
--rw-r--r--   0 ben       (1000) users      (100)     4535 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03LZ.f
--rw-r--r--   0 ben       (1000) users      (100)     2879 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03MD.f
--rw-r--r--   0 ben       (1000) users      (100)     2271 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03ND.f
--rw-r--r--   0 ben       (1000) users      (100)     2331 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03OD.f
--rw-r--r--   0 ben       (1000) users      (100)     2313 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03PD.f
--rw-r--r--   0 ben       (1000) users      (100)     2575 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03QD.f
--rw-r--r--   0 ben       (1000) users      (100)     3318 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03QG.f
--rw-r--r--   0 ben       (1000) users      (100)     2702 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03RD.f
--rw-r--r--   0 ben       (1000) users      (100)     2048 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03SD.f
--rw-r--r--   0 ben       (1000) users      (100)     3589 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03TD.f
--rw-r--r--   0 ben       (1000) users      (100)     2335 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03UD.f
--rw-r--r--   0 ben       (1000) users      (100)     4783 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03VD.f
--rw-r--r--   0 ben       (1000) users      (100)     6571 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03WD.f
--rw-r--r--   0 ben       (1000) users      (100)     8081 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03XD.f
--rw-r--r--   0 ben       (1000) users      (100)     4731 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03XP.f
--rw-r--r--   0 ben       (1000) users      (100)     9814 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03XZ.f
--rw-r--r--   0 ben       (1000) users      (100)     6151 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03ZD.f
--rw-r--r--   0 ben       (1000) users      (100)     5410 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04AD.f
--rw-r--r--   0 ben       (1000) users      (100)     4897 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04AZ.f
--rw-r--r--   0 ben       (1000) users      (100)     5120 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04BD.f
--rw-r--r--   0 ben       (1000) users      (100)     4121 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04BZ.f
--rw-r--r--   0 ben       (1000) users      (100)     2309 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DD.f
--rw-r--r--   0 ben       (1000) users      (100)     3255 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DL.f
--rw-r--r--   0 ben       (1000) users      (100)     3860 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DP.f
--rw-r--r--   0 ben       (1000) users      (100)     2310 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DS.f
--rw-r--r--   0 ben       (1000) users      (100)     2620 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DY.f
--rw-r--r--   0 ben       (1000) users      (100)     2322 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DZ.f
--rw-r--r--   0 ben       (1000) users      (100)     4204 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04ED.f
--rw-r--r--   0 ben       (1000) users      (100)     3923 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04FD.f
--rw-r--r--   0 ben       (1000) users      (100)     2546 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04GD.f
--rw-r--r--   0 ben       (1000) users      (100)     1553 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04MD.f
--rw-r--r--   0 ben       (1000) users      (100)     3012 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04OD.f
--rw-r--r--   0 ben       (1000) users      (100)     6984 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04PB.f
--rw-r--r--   0 ben       (1000) users      (100)     6928 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04PU.f
--rw-r--r--   0 ben       (1000) users      (100)    11087 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04TB.f
--rw-r--r--   0 ben       (1000) users      (100)    10989 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04TS.f
--rw-r--r--   0 ben       (1000) users      (100)     2615 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04UD.f
--rw-r--r--   0 ben       (1000) users      (100)     5407 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04VD.f
--rw-r--r--   0 ben       (1000) users      (100)     5537 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04XD.f
--rw-r--r--   0 ben       (1000) users      (100)     4693 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04YD.f
--rw-r--r--   0 ben       (1000) users      (100)     4008 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04ZD.f
--rw-r--r--   0 ben       (1000) users      (100)     2442 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB05MD.f
--rw-r--r--   0 ben       (1000) users      (100)     1965 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB05ND.f
--rw-r--r--   0 ben       (1000) users      (100)     2221 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB05OD.f
--rw-r--r--   0 ben       (1000) users      (100)     3307 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB4DLZ.f
--rw-r--r--   0 ben       (1000) users      (100)     3908 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB4DPZ.f
--rw-r--r--   0 ben       (1000) users      (100)     1519 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     1429 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01ND.f
--rw-r--r--   0 ben       (1000) users      (100)     1513 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     1415 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01PD.f
--rw-r--r--   0 ben       (1000) users      (100)     2703 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01QD.f
--rw-r--r--   0 ben       (1000) users      (100)     2548 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01RD.f
--rw-r--r--   0 ben       (1000) users      (100)     1846 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01SD.f
--rw-r--r--   0 ben       (1000) users      (100)     2305 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01TD.f
--rw-r--r--   0 ben       (1000) users      (100)     1092 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01VD.f
--rw-r--r--   0 ben       (1000) users      (100)     1764 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01WD.f
--rw-r--r--   0 ben       (1000) users      (100)     2019 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01XD.f
--rw-r--r--   0 ben       (1000) users      (100)     4003 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC03MD.f
--rw-r--r--   0 ben       (1000) users      (100)     3529 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC03ND.f
--rw-r--r--   0 ben       (1000) users      (100)     6760 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMD03AD.f
--rw-r--r--   0 ben       (1000) users      (100)     8675 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMD03BD.f
--rw-r--r--   0 ben       (1000) users      (100)     4493 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB01BD.f
--rw-r--r--   0 ben       (1000) users      (100)     3045 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB01DD.f
--rw-r--r--   0 ben       (1000) users      (100)     2184 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     2265 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02MD.f
--rw-r--r--   0 ben       (1000) users      (100)     4500 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02ND.f
--rw-r--r--   0 ben       (1000) users      (100)     4522 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02OD.f
--rw-r--r--   0 ben       (1000) users      (100)     2725 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02PD.f
--rw-r--r--   0 ben       (1000) users      (100)     5322 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02QD.f
--rw-r--r--   0 ben       (1000) users      (100)     3755 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02RD.f
--rw-r--r--   0 ben       (1000) users      (100)     5709 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02SD.f
--rw-r--r--   0 ben       (1000) users      (100)     2570 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03MD.f
--rw-r--r--   0 ben       (1000) users      (100)     3826 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03OD.f
--rw-r--r--   0 ben       (1000) users      (100)     4112 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03QD.f
--rw-r--r--   0 ben       (1000) users      (100)     4113 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03SD.f
--rw-r--r--   0 ben       (1000) users      (100)     3841 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03TD.f
--rw-r--r--   0 ben       (1000) users      (100)     3891 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03UD.f
--rw-r--r--   0 ben       (1000) users      (100)     2489 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04MD.f
--rw-r--r--   0 ben       (1000) users      (100)     2351 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04ND.f
--rw-r--r--   0 ben       (1000) users      (100)     4682 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04OD.f
--rw-r--r--   0 ben       (1000) users      (100)     3439 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04PD.f
--rw-r--r--   0 ben       (1000) users      (100)     2489 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04QD.f
--rw-r--r--   0 ben       (1000) users      (100)     2351 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04RD.f
--rw-r--r--   0 ben       (1000) users      (100)     3234 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB06ND.f
--rw-r--r--   0 ben       (1000) users      (100)     4673 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08CD.f
--rw-r--r--   0 ben       (1000) users      (100)     4643 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08DD.f
--rw-r--r--   0 ben       (1000) users      (100)     4722 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08ED.f
--rw-r--r--   0 ben       (1000) users      (100)     4636 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08FD.f
--rw-r--r--   0 ben       (1000) users      (100)     2150 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08MD.f
--rw-r--r--   0 ben       (1000) users      (100)     2148 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08ND.f
--rw-r--r--   0 ben       (1000) users      (100)     2589 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB09MD.f
--rw-r--r--   0 ben       (1000) users      (100)     4764 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10DD.f
--rw-r--r--   0 ben       (1000) users      (100)     4416 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10ED.f
--rw-r--r--   0 ben       (1000) users      (100)     6195 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10FD.f
--rw-r--r--   0 ben       (1000) users      (100)     4211 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10HD.f
--rw-r--r--   0 ben       (1000) users      (100)     3852 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10ID.f
--rw-r--r--   0 ben       (1000) users      (100)     3888 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10KD.f
--rw-r--r--   0 ben       (1000) users      (100)     3936 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10ZD.f
--rw-r--r--   0 ben       (1000) users      (100)     5626 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB16AD.f
--rw-r--r--   0 ben       (1000) users      (100)     4575 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB16BD.f
--rw-r--r--   0 ben       (1000) users      (100)     4157 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB16CD.f
--rw-r--r--   0 ben       (1000) users      (100)     4795 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSG02AD.f
--rw-r--r--   0 ben       (1000) users      (100)     4896 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSG02ND.f
--rw-r--r--   0 ben       (1000) users      (100)     3023 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSG03AD.f
--rw-r--r--   0 ben       (1000) users      (100)     2804 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSG03BD.f
--rw-r--r--   0 ben       (1000) users      (100)     2609 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01ID.f
--rw-r--r--   0 ben       (1000) users      (100)     2616 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01IZ.f
--rw-r--r--   0 ben       (1000) users      (100)     3640 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01KD.f
--rw-r--r--   0 ben       (1000) users      (100)     3635 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01LD.f
--rw-r--r--   0 ben       (1000) users      (100)     2768 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     2765 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01ND.f
--rw-r--r--   0 ben       (1000) users      (100)     3327 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01PD.f
--rw-r--r--   0 ben       (1000) users      (100)     3756 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01PX.f
--rw-r--r--   0 ben       (1000) users      (100)     3207 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01TD.f
--rw-r--r--   0 ben       (1000) users      (100)     4374 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01UD.f
--rw-r--r--   0 ben       (1000) users      (100)     4427 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01UY.f
--rw-r--r--   0 ben       (1000) users      (100)     3329 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01WD.f
--rw-r--r--   0 ben       (1000) users      (100)     3138 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01WX.f
--rw-r--r--   0 ben       (1000) users      (100)     3331 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01ZD.f
--rw-r--r--   0 ben       (1000) users      (100)     6546 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB03AD.f
--rw-r--r--   0 ben       (1000) users      (100)     6189 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB04AD.f
--rw-r--r--   0 ben       (1000) users      (100)     4337 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB04BD.f
--rw-r--r--   0 ben       (1000) users      (100)     4345 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB04CD.f
--rw-r--r--   0 ben       (1000) users      (100)     3851 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB05AD.f
--rw-r--r--   0 ben       (1000) users      (100)     3124 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTC01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     4364 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTC04AD.f
--rw-r--r--   0 ben       (1000) users      (100)     3568 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTC05AD.f
--rw-r--r--   0 ben       (1000) users      (100)     6815 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTD03AD.f
--rw-r--r--   0 ben       (1000) users      (100)     5053 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTD04AD.f
--rw-r--r--   0 ben       (1000) users      (100)     2058 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTD05AD.f
--rw-r--r--   0 ben       (1000) users      (100)     2997 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     3068 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01ND.f
--rw-r--r--   0 ben       (1000) users      (100)     2198 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     2200 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01PD.f
--rw-r--r--   0 ben       (1000) users      (100)     3009 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01QD.f
--rw-r--r--   0 ben       (1000) users      (100)     2805 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01RD.f
--rw-r--r--   0 ben       (1000) users      (100)     5099 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01AD.f
--rw-r--r--   0 ben       (1000) users      (100)     5140 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01AZ.f
--rw-r--r--   0 ben       (1000) users      (100)     3202 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01CD.f
--rw-r--r--   0 ben       (1000) users      (100)     3195 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01DD.f
--rw-r--r--   0 ben       (1000) users      (100)     4578 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01ED.f
--rw-r--r--   0 ben       (1000) users      (100)     4585 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01FD.f
--rw-r--r--   0 ben       (1000) users      (100)     4724 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01FZ.f
--rw-r--r--   0 ben       (1000) users      (100)     4252 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01GD.f
--rw-r--r--   0 ben       (1000) users      (100)     4497 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01HD.f
--rw-r--r--   0 ben       (1000) users      (100)     4589 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01ID.f
--rw-r--r--   0 ben       (1000) users      (100)     3901 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01JD.f
--rw-r--r--   0 ben       (1000) users      (100)     4176 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01JY.f
--rw-r--r--   0 ben       (1000) users      (100)     4555 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01LD.f
--rw-r--r--   0 ben       (1000) users      (100)     4870 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     4884 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01ND.f
--rw-r--r--   0 ben       (1000) users      (100)     5235 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01PD.f
--rw-r--r--   0 ben       (1000) users      (100)     5440 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01QD.f
--rw-r--r--   0 ben       (1000) users      (100)     1943 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TUD01BD.f
--rw-r--r--   0 ben       (1000) users      (100)     1965 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TUD01CD.f
--rw-r--r--   0 ben       (1000) users      (100)     1545 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TUD01DD.f
--rw-r--r--   0 ben       (1000) users      (100)     1332 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TUD01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     1962 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TUD01ND.f
--rw-r--r--   0 ben       (1000) users      (100)      375 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01BD.dat
--rw-r--r--   0 ben       (1000) users      (100)      856 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01BD.res
--rw-r--r--   0 ben       (1000) users      (100)      114 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01CD.dat
--rw-r--r--   0 ben       (1000) users      (100)      856 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01CD.res
--rw-r--r--   0 ben       (1000) users      (100)      163 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01DD.dat
--rw-r--r--   0 ben       (1000) users      (100)      615 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01DD.res
--rw-r--r--   0 ben       (1000) users      (100)      161 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01MD.dat
--rw-r--r--   0 ben       (1000) users      (100)      377 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01MD.res
--rw-r--r--   0 ben       (1000) users      (100)      388 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01ND.dat
--rw-r--r--   0 ben       (1000) users      (100)      853 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01ND.res
--rw-r--r--   0 ben       (1000) users      (100)    57273 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/makefile
--rw-r--r--   0 ben       (1000) users      (100)     1108 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/examples/readme
--rw-r--r--   0 ben       (1000) users      (100)    38876 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/libindex.html
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.680944 slycot-0.5.3/slycot/src/SLICOT-Reference/src/
--rw-r--r--   0 ben       (1000) users      (100)    13388 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB01MD.f
--rw-r--r--   0 ben       (1000) users      (100)    16256 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB01ND.f
--rw-r--r--   0 ben       (1000) users      (100)    19924 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB01OD.f
--rw-r--r--   0 ben       (1000) users      (100)    10651 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB04MD.f
--rw-r--r--   0 ben       (1000) users      (100)    17577 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05MD.f
--rw-r--r--   0 ben       (1000) users      (100)    18119 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05ND.f
--rw-r--r--   0 ben       (1000) users      (100)    12969 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05OD.f
--rw-r--r--   0 ben       (1000) users      (100)    11939 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05PD.f
--rw-r--r--   0 ben       (1000) users      (100)    13523 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05QD.f
--rw-r--r--   0 ben       (1000) users      (100)    13196 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05RD.f
--rw-r--r--   0 ben       (1000) users      (100)    11707 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05SD.f
--rw-r--r--   0 ben       (1000) users      (100)     6122 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB07MD.f
--rw-r--r--   0 ben       (1000) users      (100)     9978 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB07ND.f
--rw-r--r--   0 ben       (1000) users      (100)     9436 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08MD.f
--rw-r--r--   0 ben       (1000) users      (100)     9597 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08MZ.f
--rw-r--r--   0 ben       (1000) users      (100)    18491 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08ND.f
--rw-r--r--   0 ben       (1000) users      (100)    19794 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08NW.f
--rw-r--r--   0 ben       (1000) users      (100)    15224 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08NX.f
--rw-r--r--   0 ben       (1000) users      (100)    19969 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08NY.f
--rw-r--r--   0 ben       (1000) users      (100)    18880 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08NZ.f
--rw-r--r--   0 ben       (1000) users      (100)    12486 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09AD.f
--rw-r--r--   0 ben       (1000) users      (100)    19246 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09AX.f
--rw-r--r--   0 ben       (1000) users      (100)    13362 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09BD.f
--rw-r--r--   0 ben       (1000) users      (100)    22818 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09BX.f
--rw-r--r--   0 ben       (1000) users      (100)    13288 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09CD.f
--rw-r--r--   0 ben       (1000) users      (100)    19074 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09CX.f
--rw-r--r--   0 ben       (1000) users      (100)     8214 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09DD.f
--rw-r--r--   0 ben       (1000) users      (100)    17903 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09ED.f
--rw-r--r--   0 ben       (1000) users      (100)    24413 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09FD.f
--rw-r--r--   0 ben       (1000) users      (100)    25869 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09GD.f
--rw-r--r--   0 ben       (1000) users      (100)    25636 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09HD.f
--rw-r--r--   0 ben       (1000) users      (100)    24665 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09HX.f
--rw-r--r--   0 ben       (1000) users      (100)    12631 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09HY.f
--rw-r--r--   0 ben       (1000) users      (100)    43280 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09ID.f
--rw-r--r--   0 ben       (1000) users      (100)    24534 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09IX.f
--rw-r--r--   0 ben       (1000) users      (100)    31554 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09IY.f
--rw-r--r--   0 ben       (1000) users      (100)    58312 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09JD.f
--rw-r--r--   0 ben       (1000) users      (100)    35740 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09JV.f
--rw-r--r--   0 ben       (1000) users      (100)    36169 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09JW.f
--rw-r--r--   0 ben       (1000) users      (100)     7640 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09JX.f
--rw-r--r--   0 ben       (1000) users      (100)    34205 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09KD.f
--rw-r--r--   0 ben       (1000) users      (100)    31362 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09KX.f
--rw-r--r--   0 ben       (1000) users      (100)    16581 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09MD.f
--rw-r--r--   0 ben       (1000) users      (100)    17609 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09ND.f
--rw-r--r--   0 ben       (1000) users      (100)    11668 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13AD.f
--rw-r--r--   0 ben       (1000) users      (100)     9087 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13AX.f
--rw-r--r--   0 ben       (1000) users      (100)    13106 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13BD.f
--rw-r--r--   0 ben       (1000) users      (100)    18030 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13CD.f
--rw-r--r--   0 ben       (1000) users      (100)    64623 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13DD.f
--rw-r--r--   0 ben       (1000) users      (100)    18226 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13DX.f
--rw-r--r--   0 ben       (1000) users      (100)    10636 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13ED.f
--rw-r--r--   0 ben       (1000) users      (100)    12761 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13FD.f
--rw-r--r--   0 ben       (1000) users      (100)    33585 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13ID.f
--rw-r--r--   0 ben       (1000) users      (100)    59291 2022-05-29 11:35:56.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13MD.f
--rw-r--r--   0 ben       (1000) users      (100)    15752 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB8NXZ.f
--rw-r--r--   0 ben       (1000) users      (100)     8517 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AG07BD.f
--rw-r--r--   0 ben       (1000) users      (100)    21364 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AG08BD.f
--rw-r--r--   0 ben       (1000) users      (100)    22470 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AG08BY.f
--rw-r--r--   0 ben       (1000) users      (100)    21945 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AG08BZ.f
--rw-r--r--   0 ben       (1000) users      (100)    23110 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/AG8BYZ.f
--rw-r--r--   0 ben       (1000) users      (100)    49714 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/BB01AD.f
--rw-r--r--   0 ben       (1000) users      (100)    37531 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/BB02AD.f
--rw-r--r--   0 ben       (1000) users      (100)    17019 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/BB03AD.f
--rw-r--r--   0 ben       (1000) users      (100)    16276 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/BB04AD.f
--rw-r--r--   0 ben       (1000) users      (100)    34360 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/BD01AD.f
--rw-r--r--   0 ben       (1000) users      (100)    19237 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/BD02AD.f
--rw-r--r--   0 ben       (1000) users      (100)     4698 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/DE01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     6053 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/DE01PD.f
--rw-r--r--   0 ben       (1000) users      (100)     7666 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/DF01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     6054 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/DG01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     7843 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/DG01ND.f
--rw-r--r--   0 ben       (1000) users      (100)     2011 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/DG01NY.f
--rw-r--r--   0 ben       (1000) users      (100)     8970 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/DG01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     4200 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/DK01MD.f
--rw-r--r--   0 ben       (1000) users      (100)    16908 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/FB01QD.f
--rw-r--r--   0 ben       (1000) users      (100)    19438 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/FB01RD.f
--rw-r--r--   0 ben       (1000) users      (100)    22667 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/FB01SD.f
--rw-r--r--   0 ben       (1000) users      (100)    24240 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/FB01TD.f
--rw-r--r--   0 ben       (1000) users      (100)    13042 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/FB01VD.f
--rw-r--r--   0 ben       (1000) users      (100)    12706 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/FD01AD.f
--rw-r--r--   0 ben       (1000) users      (100)    30121 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01AD.f
--rw-r--r--   0 ben       (1000) users      (100)    31877 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01BD.f
--rw-r--r--   0 ben       (1000) users      (100)    34315 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01CD.f
--rw-r--r--   0 ben       (1000) users      (100)    53910 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01MD.f
--rw-r--r--   0 ben       (1000) users      (100)    41860 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01MY.f
--rw-r--r--   0 ben       (1000) users      (100)    27606 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01ND.f
--rw-r--r--   0 ben       (1000) users      (100)     5773 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     4591 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01OY.f
--rw-r--r--   0 ben       (1000) users      (100)    49760 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01PD.f
--rw-r--r--   0 ben       (1000) users      (100)    15760 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01PX.f
--rw-r--r--   0 ben       (1000) users      (100)    29354 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01PY.f
--rw-r--r--   0 ben       (1000) users      (100)    39165 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01QD.f
--rw-r--r--   0 ben       (1000) users      (100)    26853 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01RD.f
--rw-r--r--   0 ben       (1000) users      (100)    44357 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB03AD.f
--rw-r--r--   0 ben       (1000) users      (100)    45297 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB03BD.f
--rw-r--r--   0 ben       (1000) users      (100)     2094 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA01AD.f
--rw-r--r--   0 ben       (1000) users      (100)     3459 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA01BD.f
--rw-r--r--   0 ben       (1000) users      (100)     3392 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA01BZ.f
--rw-r--r--   0 ben       (1000) users      (100)     2829 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA01CD.f
--rw-r--r--   0 ben       (1000) users      (100)     2429 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02AD.f
--rw-r--r--   0 ben       (1000) users      (100)     3403 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02AZ.f
--rw-r--r--   0 ben       (1000) users      (100)     2871 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02BD.f
--rw-r--r--   0 ben       (1000) users      (100)     2924 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02BZ.f
--rw-r--r--   0 ben       (1000) users      (100)     2823 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02CD.f
--rw-r--r--   0 ben       (1000) users      (100)     2824 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02CZ.f
--rw-r--r--   0 ben       (1000) users      (100)     4469 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02DD.f
--rw-r--r--   0 ben       (1000) users      (100)     2270 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02ED.f
--rw-r--r--   0 ben       (1000) users      (100)     2467 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02ES.f
--rw-r--r--   0 ben       (1000) users      (100)     5565 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02EZ.f
--rw-r--r--   0 ben       (1000) users      (100)     2410 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02FD.f
--rw-r--r--   0 ben       (1000) users      (100)     4175 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02GD.f
--rw-r--r--   0 ben       (1000) users      (100)     4206 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02GZ.f
--rw-r--r--   0 ben       (1000) users      (100)     4319 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02HD.f
--rw-r--r--   0 ben       (1000) users      (100)     4244 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02HZ.f
--rw-r--r--   0 ben       (1000) users      (100)     9148 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02ID.f
--rw-r--r--   0 ben       (1000) users      (100)    11211 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02IZ.f
--rw-r--r--   0 ben       (1000) users      (100)     5035 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02JD.f
--rw-r--r--   0 ben       (1000) users      (100)     5106 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02JZ.f
--rw-r--r--   0 ben       (1000) users      (100)     5458 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02MD.f
--rw-r--r--   0 ben       (1000) users      (100)     6061 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02MZ.f
--rw-r--r--   0 ben       (1000) users      (100)     5882 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02NZ.f
--rw-r--r--   0 ben       (1000) users      (100)     4177 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02OD.f
--rw-r--r--   0 ben       (1000) users      (100)     4746 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02OZ.f
--rw-r--r--   0 ben       (1000) users      (100)     2393 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02PD.f
--rw-r--r--   0 ben       (1000) users      (100)     2405 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02PZ.f
--rw-r--r--   0 ben       (1000) users      (100)    10622 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01KD.f
--rw-r--r--   0 ben       (1000) users      (100)    14826 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01LD.f
--rw-r--r--   0 ben       (1000) users      (100)     8084 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     7549 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01ND.f
--rw-r--r--   0 ben       (1000) users      (100)    10606 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OC.f
--rw-r--r--   0 ben       (1000) users      (100)    13117 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     8786 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OE.f
--rw-r--r--   0 ben       (1000) users      (100)     8790 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OH.f
--rw-r--r--   0 ben       (1000) users      (100)     5643 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OO.f
--rw-r--r--   0 ben       (1000) users      (100)     9428 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OS.f
--rw-r--r--   0 ben       (1000) users      (100)     7743 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OT.f
--rw-r--r--   0 ben       (1000) users      (100)     8349 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01PD.f
--rw-r--r--   0 ben       (1000) users      (100)     8842 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01QD.f
--rw-r--r--   0 ben       (1000) users      (100)    17110 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RB.f
--rw-r--r--   0 ben       (1000) users      (100)    10977 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RD.f
--rw-r--r--   0 ben       (1000) users      (100)    11083 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RH.f
--rw-r--r--   0 ben       (1000) users      (100)     8955 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RT.f
--rw-r--r--   0 ben       (1000) users      (100)     9024 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RU.f
--rw-r--r--   0 ben       (1000) users      (100)     6974 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RW.f
--rw-r--r--   0 ben       (1000) users      (100)    10594 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RX.f
--rw-r--r--   0 ben       (1000) users      (100)    13778 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RY.f
--rw-r--r--   0 ben       (1000) users      (100)     2910 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01SD.f
--rw-r--r--   0 ben       (1000) users      (100)     3817 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01SS.f
--rw-r--r--   0 ben       (1000) users      (100)     4379 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01TD.f
--rw-r--r--   0 ben       (1000) users      (100)     6907 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01UD.f
--rw-r--r--   0 ben       (1000) users      (100)    11842 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01UW.f
--rw-r--r--   0 ben       (1000) users      (100)    11999 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01UX.f
--rw-r--r--   0 ben       (1000) users      (100)    14764 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01UY.f
--rw-r--r--   0 ben       (1000) users      (100)    17828 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01UZ.f
--rw-r--r--   0 ben       (1000) users      (100)    46653 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01VD.f
--rw-r--r--   0 ben       (1000) users      (100)    10509 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01WD.f
--rw-r--r--   0 ben       (1000) users      (100)     5901 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01XD.f
--rw-r--r--   0 ben       (1000) users      (100)     4971 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01XY.f
--rw-r--r--   0 ben       (1000) users      (100)    10183 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01YD.f
--rw-r--r--   0 ben       (1000) users      (100)    14210 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01ZD.f
--rw-r--r--   0 ben       (1000) users      (100)    21939 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02CD.f
--rw-r--r--   0 ben       (1000) users      (100)    36346 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02CU.f
--rw-r--r--   0 ben       (1000) users      (100)    27075 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02CV.f
--rw-r--r--   0 ben       (1000) users      (100)    10027 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02CX.f
--rw-r--r--   0 ben       (1000) users      (100)    11454 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02CY.f
--rw-r--r--   0 ben       (1000) users      (100)    21105 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02DD.f
--rw-r--r--   0 ben       (1000) users      (100)    15867 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02ED.f
--rw-r--r--   0 ben       (1000) users      (100)    12794 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02FD.f
--rw-r--r--   0 ben       (1000) users      (100)    19214 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02GD.f
--rw-r--r--   0 ben       (1000) users      (100)    19161 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02HD.f
--rw-r--r--   0 ben       (1000) users      (100)    20760 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02ID.f
--rw-r--r--   0 ben       (1000) users      (100)    20166 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02JD.f
--rw-r--r--   0 ben       (1000) users      (100)    24476 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02JX.f
--rw-r--r--   0 ben       (1000) users      (100)    26986 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02KD.f
--rw-r--r--   0 ben       (1000) users      (100)    22436 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02MD.f
--rw-r--r--   0 ben       (1000) users      (100)    33633 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02ND.f
--rw-r--r--   0 ben       (1000) users      (100)     8480 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02NY.f
--rw-r--r--   0 ben       (1000) users      (100)     8391 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02OD.f
--rw-r--r--   0 ben       (1000) users      (100)    21111 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02PD.f
--rw-r--r--   0 ben       (1000) users      (100)    17866 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02QD.f
--rw-r--r--   0 ben       (1000) users      (100)    11424 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02QY.f
--rw-r--r--   0 ben       (1000) users      (100)     5068 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02RD.f
--rw-r--r--   0 ben       (1000) users      (100)     5800 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02RZ.f
--rw-r--r--   0 ben       (1000) users      (100)     3921 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02SD.f
--rw-r--r--   0 ben       (1000) users      (100)     4204 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02SZ.f
--rw-r--r--   0 ben       (1000) users      (100)     6055 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02TD.f
--rw-r--r--   0 ben       (1000) users      (100)     6506 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02TZ.f
--rw-r--r--   0 ben       (1000) users      (100)    21891 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02UD.f
--rw-r--r--   0 ben       (1000) users      (100)     4298 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02UU.f
--rw-r--r--   0 ben       (1000) users      (100)     5288 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02UV.f
--rw-r--r--   0 ben       (1000) users      (100)     9764 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02UW.f
--rw-r--r--   0 ben       (1000) users      (100)     5427 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02VD.f
--rw-r--r--   0 ben       (1000) users      (100)    14883 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02WD.f
--rw-r--r--   0 ben       (1000) users      (100)    14038 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02XD.f
--rw-r--r--   0 ben       (1000) users      (100)    11492 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02YD.f
--rw-r--r--   0 ben       (1000) users      (100)     8287 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AB.f
--rw-r--r--   0 ben       (1000) users      (100)     7205 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AD.f
--rw-r--r--   0 ben       (1000) users      (100)     9318 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AE.f
--rw-r--r--   0 ben       (1000) users      (100)    11962 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AF.f
--rw-r--r--   0 ben       (1000) users      (100)    10070 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AG.f
--rw-r--r--   0 ben       (1000) users      (100)     9224 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AH.f
--rw-r--r--   0 ben       (1000) users      (100)     8238 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AI.f
--rw-r--r--   0 ben       (1000) users      (100)     2521 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BA.f
--rw-r--r--   0 ben       (1000) users      (100)    13821 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BB.f
--rw-r--r--   0 ben       (1000) users      (100)    12109 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BC.f
--rw-r--r--   0 ben       (1000) users      (100)    74389 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BD.f
--rw-r--r--   0 ben       (1000) users      (100)     4537 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BE.f
--rw-r--r--   0 ben       (1000) users      (100)     4194 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BF.f
--rw-r--r--   0 ben       (1000) users      (100)     3982 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BG.f
--rw-r--r--   0 ben       (1000) users      (100)    41418 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BZ.f
--rw-r--r--   0 ben       (1000) users      (100)    20675 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03CD.f
--rw-r--r--   0 ben       (1000) users      (100)     4343 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03CZ.f
--rw-r--r--   0 ben       (1000) users      (100)    23535 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03DD.f
--rw-r--r--   0 ben       (1000) users      (100)     3354 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03DZ.f
--rw-r--r--   0 ben       (1000) users      (100)    12531 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03ED.f
--rw-r--r--   0 ben       (1000) users      (100)    10235 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03FD.f
--rw-r--r--   0 ben       (1000) users      (100)    44919 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03FZ.f
--rw-r--r--   0 ben       (1000) users      (100)    11486 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03GD.f
--rw-r--r--   0 ben       (1000) users      (100)     3617 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03GZ.f
--rw-r--r--   0 ben       (1000) users      (100)     9116 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03HD.f
--rw-r--r--   0 ben       (1000) users      (100)     2768 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03HZ.f
--rw-r--r--   0 ben       (1000) users      (100)    62943 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03ID.f
--rw-r--r--   0 ben       (1000) users      (100)    24855 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03IZ.f
--rw-r--r--   0 ben       (1000) users      (100)    47137 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03JD.f
--rw-r--r--   0 ben       (1000) users      (100)    68854 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03JP.f
--rw-r--r--   0 ben       (1000) users      (100)    18233 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03JZ.f
--rw-r--r--   0 ben       (1000) users      (100)    23179 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03KA.f
--rw-r--r--   0 ben       (1000) users      (100)    60190 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03KB.f
--rw-r--r--   0 ben       (1000) users      (100)     8080 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03KC.f
--rw-r--r--   0 ben       (1000) users      (100)    18160 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03KD.f
--rw-r--r--   0 ben       (1000) users      (100)    28149 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03KE.f
--rw-r--r--   0 ben       (1000) users      (100)    29739 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03LD.f
--rw-r--r--   0 ben       (1000) users      (100)    36822 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03LF.f
--rw-r--r--   0 ben       (1000) users      (100)    30052 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03LP.f
--rw-r--r--   0 ben       (1000) users      (100)    34359 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03LZ.f
--rw-r--r--   0 ben       (1000) users      (100)    11933 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03MD.f
--rw-r--r--   0 ben       (1000) users      (100)     1887 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03MY.f
--rw-r--r--   0 ben       (1000) users      (100)     6868 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03ND.f
--rw-r--r--   0 ben       (1000) users      (100)     5657 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03NY.f
--rw-r--r--   0 ben       (1000) users      (100)    11339 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03OD.f
--rw-r--r--   0 ben       (1000) users      (100)    13160 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03OY.f
--rw-r--r--   0 ben       (1000) users      (100)    11797 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03PD.f
--rw-r--r--   0 ben       (1000) users      (100)    13361 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03PY.f
--rw-r--r--   0 ben       (1000) users      (100)    11081 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QD.f
--rw-r--r--   0 ben       (1000) users      (100)    16223 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QG.f
--rw-r--r--   0 ben       (1000) users      (100)     3672 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QV.f
--rw-r--r--   0 ben       (1000) users      (100)     6582 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QW.f
--rw-r--r--   0 ben       (1000) users      (100)     2780 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QX.f
--rw-r--r--   0 ben       (1000) users      (100)     4892 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QY.f
--rw-r--r--   0 ben       (1000) users      (100)    21728 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03RD.f
--rw-r--r--   0 ben       (1000) users      (100)     7988 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03RW.f
--rw-r--r--   0 ben       (1000) users      (100)     7566 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03RX.f
--rw-r--r--   0 ben       (1000) users      (100)     8127 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03RY.f
--rw-r--r--   0 ben       (1000) users      (100)    20412 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03RZ.f
--rw-r--r--   0 ben       (1000) users      (100)    11275 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03SD.f
--rw-r--r--   0 ben       (1000) users      (100)    22798 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03TD.f
--rw-r--r--   0 ben       (1000) users      (100)    26590 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03TS.f
--rw-r--r--   0 ben       (1000) users      (100)    11053 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03UD.f
--rw-r--r--   0 ben       (1000) users      (100)    10269 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03VD.f
--rw-r--r--   0 ben       (1000) users      (100)    25576 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03VW.f
--rw-r--r--   0 ben       (1000) users      (100)     7335 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03VY.f
--rw-r--r--   0 ben       (1000) users      (100)    19411 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03WA.f
--rw-r--r--   0 ben       (1000) users      (100)    32750 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03WD.f
--rw-r--r--   0 ben       (1000) users      (100)     4415 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03WX.f
--rw-r--r--   0 ben       (1000) users      (100)    33154 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03XD.f
--rw-r--r--   0 ben       (1000) users      (100)    22195 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03XP.f
--rw-r--r--   0 ben       (1000) users      (100)    16760 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03XS.f
--rw-r--r--   0 ben       (1000) users      (100)   112885 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03XU.f
--rw-r--r--   0 ben       (1000) users      (100)    28625 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03XZ.f
--rw-r--r--   0 ben       (1000) users      (100)     9976 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03YA.f
--rw-r--r--   0 ben       (1000) users      (100)    17926 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03YD.f
--rw-r--r--   0 ben       (1000) users      (100)     9465 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03YT.f
--rw-r--r--   0 ben       (1000) users      (100)    56706 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03ZA.f
--rw-r--r--   0 ben       (1000) users      (100)    41509 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03ZD.f
--rw-r--r--   0 ben       (1000) users      (100)    58674 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04AD.f
--rw-r--r--   0 ben       (1000) users      (100)    38788 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04AZ.f
--rw-r--r--   0 ben       (1000) users      (100)    49771 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04BD.f
--rw-r--r--   0 ben       (1000) users      (100)    57956 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04BP.f
--rw-r--r--   0 ben       (1000) users      (100)    34475 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04BZ.f
--rw-r--r--   0 ben       (1000) users      (100)   143552 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04CD.f
--rw-r--r--   0 ben       (1000) users      (100)     6281 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DB.f
--rw-r--r--   0 ben       (1000) users      (100)    14837 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DD.f
--rw-r--r--   0 ben       (1000) users      (100)     5916 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DI.f
--rw-r--r--   0 ben       (1000) users      (100)    28402 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DL.f
--rw-r--r--   0 ben       (1000) users      (100)    43810 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DP.f
--rw-r--r--   0 ben       (1000) users      (100)    15019 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DS.f
--rw-r--r--   0 ben       (1000) users      (100)    11159 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DY.f
--rw-r--r--   0 ben       (1000) users      (100)    15971 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DZ.f
--rw-r--r--   0 ben       (1000) users      (100)    43773 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04ED.f
--rw-r--r--   0 ben       (1000) users      (100)    38139 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04FD.f
--rw-r--r--   0 ben       (1000) users      (100)    43589 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04FP.f
--rw-r--r--   0 ben       (1000) users      (100)     7408 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04GD.f
--rw-r--r--   0 ben       (1000) users      (100)   100661 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04HD.f
--rw-r--r--   0 ben       (1000) users      (100)     8471 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04ID.f
--rw-r--r--   0 ben       (1000) users      (100)     9918 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04IY.f
--rw-r--r--   0 ben       (1000) users      (100)     8689 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04IZ.f
--rw-r--r--   0 ben       (1000) users      (100)     7426 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04JD.f
--rw-r--r--   0 ben       (1000) users      (100)     6976 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04KD.f
--rw-r--r--   0 ben       (1000) users      (100)     6964 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04LD.f
--rw-r--r--   0 ben       (1000) users      (100)     7884 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04MD.f
--rw-r--r--   0 ben       (1000) users      (100)     8320 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04ND.f
--rw-r--r--   0 ben       (1000) users      (100)    11316 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04NY.f
--rw-r--r--   0 ben       (1000) users      (100)     8103 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04OD.f
--rw-r--r--   0 ben       (1000) users      (100)     8066 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04OW.f
--rw-r--r--   0 ben       (1000) users      (100)     2680 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04OX.f
--rw-r--r--   0 ben       (1000) users      (100)     9773 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04OY.f
--rw-r--r--   0 ben       (1000) users      (100)    48131 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04PA.f
--rw-r--r--   0 ben       (1000) users      (100)    11721 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04PB.f
--rw-r--r--   0 ben       (1000) users      (100)    11802 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04PU.f
--rw-r--r--   0 ben       (1000) users      (100)    18073 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04PY.f
--rw-r--r--   0 ben       (1000) users      (100)    16042 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04QB.f
--rw-r--r--   0 ben       (1000) users      (100)    40151 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04QC.f
--rw-r--r--   0 ben       (1000) users      (100)    19849 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04QF.f
--rw-r--r--   0 ben       (1000) users      (100)     9582 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04QS.f
--rw-r--r--   0 ben       (1000) users      (100)    16626 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04QU.f
--rw-r--r--   0 ben       (1000) users      (100)    12060 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04RB.f
--rw-r--r--   0 ben       (1000) users      (100)    10865 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04RU.f
--rw-r--r--   0 ben       (1000) users      (100)     7730 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04SU.f
--rw-r--r--   0 ben       (1000) users      (100)    28603 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TB.f
--rw-r--r--   0 ben       (1000) users      (100)    17849 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TS.f
--rw-r--r--   0 ben       (1000) users      (100)    13875 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TT.f
--rw-r--r--   0 ben       (1000) users      (100)     2000 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TU.f
--rw-r--r--   0 ben       (1000) users      (100)     5494 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TV.f
--rw-r--r--   0 ben       (1000) users      (100)     5856 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TW.f
--rw-r--r--   0 ben       (1000) users      (100)    14165 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TX.f
--rw-r--r--   0 ben       (1000) users      (100)     7949 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TY.f
--rw-r--r--   0 ben       (1000) users      (100)    13148 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04UD.f
--rw-r--r--   0 ben       (1000) users      (100)    19456 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04VD.f
--rw-r--r--   0 ben       (1000) users      (100)    13767 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04VX.f
--rw-r--r--   0 ben       (1000) users      (100)    15537 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04WD.f
--rw-r--r--   0 ben       (1000) users      (100)     7221 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04WP.f
--rw-r--r--   0 ben       (1000) users      (100)    12725 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04WR.f
--rw-r--r--   0 ben       (1000) users      (100)    13414 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04WU.f
--rw-r--r--   0 ben       (1000) users      (100)    24819 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04XD.f
--rw-r--r--   0 ben       (1000) users      (100)     8185 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04XY.f
--rw-r--r--   0 ben       (1000) users      (100)    22848 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04YD.f
--rw-r--r--   0 ben       (1000) users      (100)    17365 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04YW.f
--rw-r--r--   0 ben       (1000) users      (100)    17268 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04ZD.f
--rw-r--r--   0 ben       (1000) users      (100)    12341 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB05MD.f
--rw-r--r--   0 ben       (1000) users      (100)    11110 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB05MY.f
--rw-r--r--   0 ben       (1000) users      (100)    11292 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB05ND.f
--rw-r--r--   0 ben       (1000) users      (100)    17518 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB05OD.f
--rw-r--r--   0 ben       (1000) users      (100)     4629 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB05OY.f
--rw-r--r--   0 ben       (1000) users      (100)    26707 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB3JZP.f
--rw-r--r--   0 ben       (1000) users      (100)    34693 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB3LZP.f
--rw-r--r--   0 ben       (1000) users      (100)    13198 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB3OYZ.f
--rw-r--r--   0 ben       (1000) users      (100)    13642 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB3PYZ.f
--rw-r--r--   0 ben       (1000) users      (100)     6338 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB4DBZ.f
--rw-r--r--   0 ben       (1000) users      (100)    28572 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB4DLZ.f
--rw-r--r--   0 ben       (1000) users      (100)    42410 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB4DPZ.f
--rw-r--r--   0 ben       (1000) users      (100)     4100 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     3081 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01ND.f
--rw-r--r--   0 ben       (1000) users      (100)     3473 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     3787 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01PD.f
--rw-r--r--   0 ben       (1000) users      (100)     3654 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01PY.f
--rw-r--r--   0 ben       (1000) users      (100)     5622 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01QD.f
--rw-r--r--   0 ben       (1000) users      (100)     7890 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01RD.f
--rw-r--r--   0 ben       (1000) users      (100)     7131 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01SD.f
--rw-r--r--   0 ben       (1000) users      (100)     1931 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01SW.f
--rw-r--r--   0 ben       (1000) users      (100)     1370 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01SX.f
--rw-r--r--   0 ben       (1000) users      (100)     3260 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01SY.f
--rw-r--r--   0 ben       (1000) users      (100)     9206 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01TD.f
--rw-r--r--   0 ben       (1000) users      (100)     8228 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01VD.f
--rw-r--r--   0 ben       (1000) users      (100)     3732 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01WD.f
--rw-r--r--   0 ben       (1000) users      (100)    10210 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01XD.f
--rw-r--r--   0 ben       (1000) users      (100)    10781 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC03MD.f
--rw-r--r--   0 ben       (1000) users      (100)    17534 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC03ND.f
--rw-r--r--   0 ben       (1000) users      (100)     4126 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC03NX.f
--rw-r--r--   0 ben       (1000) users      (100)    13886 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC03NY.f
--rw-r--r--   0 ben       (1000) users      (100)    37710 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03AD.f
--rw-r--r--   0 ben       (1000) users      (100)     4762 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BA.f
--rw-r--r--   0 ben       (1000) users      (100)     6981 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BB.f
--rw-r--r--   0 ben       (1000) users      (100)    48883 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BD.f
--rw-r--r--   0 ben       (1000) users      (100)     3164 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BF.f
--rw-r--r--   0 ben       (1000) users      (100)     7376 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BX.f
--rw-r--r--   0 ben       (1000) users      (100)    16092 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BY.f
--rw-r--r--   0 ben       (1000) users      (100)     7044 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01AD.f
--rw-r--r--   0 ben       (1000) users      (100)    10532 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01AY.f
--rw-r--r--   0 ben       (1000) users      (100)     3162 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BA.f
--rw-r--r--   0 ben       (1000) users      (100)     4561 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BB.f
--rw-r--r--   0 ben       (1000) users      (100)    13015 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BD.f
--rw-r--r--   0 ben       (1000) users      (100)     3184 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BE.f
--rw-r--r--   0 ben       (1000) users      (100)     5216 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BF.f
--rw-r--r--   0 ben       (1000) users      (100)    23050 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BP.f
--rw-r--r--   0 ben       (1000) users      (100)    16554 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BQ.f
--rw-r--r--   0 ben       (1000) users      (100)    23814 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BR.f
--rw-r--r--   0 ben       (1000) users      (100)    19648 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BS.f
--rw-r--r--   0 ben       (1000) users      (100)    12213 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BU.f
--rw-r--r--   0 ben       (1000) users      (100)     6865 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BV.f
--rw-r--r--   0 ben       (1000) users      (100)     6950 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BW.f
--rw-r--r--   0 ben       (1000) users      (100)     4484 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BX.f
--rw-r--r--   0 ben       (1000) users      (100)     8822 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BY.f
--rw-r--r--   0 ben       (1000) users      (100)    28040 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01BD.f
--rw-r--r--   0 ben       (1000) users      (100)     4214 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01BX.f
--rw-r--r--   0 ben       (1000) users      (100)     9930 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01BY.f
--rw-r--r--   0 ben       (1000) users      (100)    22024 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01DD.f
--rw-r--r--   0 ben       (1000) users      (100)     9194 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01FY.f
--rw-r--r--   0 ben       (1000) users      (100)    11162 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     1669 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02CX.f
--rw-r--r--   0 ben       (1000) users      (100)    20210 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MD.f
--rw-r--r--   0 ben       (1000) users      (100)     1234 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MR.f
--rw-r--r--   0 ben       (1000) users      (100)     1394 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MS.f
--rw-r--r--   0 ben       (1000) users      (100)    21487 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MT.f
--rw-r--r--   0 ben       (1000) users      (100)    15692 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MU.f
--rw-r--r--   0 ben       (1000) users      (100)     1229 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MV.f
--rw-r--r--   0 ben       (1000) users      (100)     1374 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MW.f
--rw-r--r--   0 ben       (1000) users      (100)    25300 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MX.f
--rw-r--r--   0 ben       (1000) users      (100)    30639 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02ND.f
--rw-r--r--   0 ben       (1000) users      (100)    32249 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OD.f
--rw-r--r--   0 ben       (1000) users      (100)     1695 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OU.f
--rw-r--r--   0 ben       (1000) users      (100)     1732 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OV.f
--rw-r--r--   0 ben       (1000) users      (100)     1690 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OW.f
--rw-r--r--   0 ben       (1000) users      (100)     1706 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OX.f
--rw-r--r--   0 ben       (1000) users      (100)    25732 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OY.f
--rw-r--r--   0 ben       (1000) users      (100)    24947 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02PD.f
--rw-r--r--   0 ben       (1000) users      (100)    28828 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02QD.f
--rw-r--r--   0 ben       (1000) users      (100)    45011 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02RD.f
--rw-r--r--   0 ben       (1000) users      (100)    16519 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02RU.f
--rw-r--r--   0 ben       (1000) users      (100)    32171 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02SD.f
--rw-r--r--   0 ben       (1000) users      (100)    21077 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MD.f
--rw-r--r--   0 ben       (1000) users      (100)    14414 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MU.f
--rw-r--r--   0 ben       (1000) users      (100)     8829 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MV.f
--rw-r--r--   0 ben       (1000) users      (100)     8541 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MW.f
--rw-r--r--   0 ben       (1000) users      (100)    25043 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MX.f
--rw-r--r--   0 ben       (1000) users      (100)    20390 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MY.f
--rw-r--r--   0 ben       (1000) users      (100)    32135 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OD.f
--rw-r--r--   0 ben       (1000) users      (100)    13413 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OR.f
--rw-r--r--   0 ben       (1000) users      (100)    19607 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OS.f
--rw-r--r--   0 ben       (1000) users      (100)    35867 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OT.f
--rw-r--r--   0 ben       (1000) users      (100)    15269 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OU.f
--rw-r--r--   0 ben       (1000) users      (100)     2994 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OV.f
--rw-r--r--   0 ben       (1000) users      (100)    23490 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OY.f
--rw-r--r--   0 ben       (1000) users      (100)    30928 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OZ.f
--rw-r--r--   0 ben       (1000) users      (100)    13488 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03PD.f
--rw-r--r--   0 ben       (1000) users      (100)    24244 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03QD.f
--rw-r--r--   0 ben       (1000) users      (100)    12125 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03QX.f
--rw-r--r--   0 ben       (1000) users      (100)    13679 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03QY.f
--rw-r--r--   0 ben       (1000) users      (100)    13267 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03RD.f
--rw-r--r--   0 ben       (1000) users      (100)    24627 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03SD.f
--rw-r--r--   0 ben       (1000) users      (100)    12292 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03SX.f
--rw-r--r--   0 ben       (1000) users      (100)    13989 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03SY.f
--rw-r--r--   0 ben       (1000) users      (100)    20057 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03TD.f
--rw-r--r--   0 ben       (1000) users      (100)    20251 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03UD.f
--rw-r--r--   0 ben       (1000) users      (100)    12558 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04MD.f
--rw-r--r--   0 ben       (1000) users      (100)     5298 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04MR.f
--rw-r--r--   0 ben       (1000) users      (100)     4877 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04MU.f
--rw-r--r--   0 ben       (1000) users      (100)     4564 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04MW.f
--rw-r--r--   0 ben       (1000) users      (100)     4179 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04MY.f
--rw-r--r--   0 ben       (1000) users      (100)    13096 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04ND.f
--rw-r--r--   0 ben       (1000) users      (100)     5040 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04NV.f
--rw-r--r--   0 ben       (1000) users      (100)     4359 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04NW.f
--rw-r--r--   0 ben       (1000) users      (100)    10570 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04NX.f
--rw-r--r--   0 ben       (1000) users      (100)     7719 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04NY.f
--rw-r--r--   0 ben       (1000) users      (100)    38542 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04OD.f
--rw-r--r--   0 ben       (1000) users      (100)    17741 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04OW.f
--rw-r--r--   0 ben       (1000) users      (100)    24585 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04PD.f
--rw-r--r--   0 ben       (1000) users      (100)    14233 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04PX.f
--rw-r--r--   0 ben       (1000) users      (100)    40219 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04PY.f
--rw-r--r--   0 ben       (1000) users      (100)    13259 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04QD.f
--rw-r--r--   0 ben       (1000) users      (100)     5313 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04QR.f
--rw-r--r--   0 ben       (1000) users      (100)     5712 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04QU.f
--rw-r--r--   0 ben       (1000) users      (100)     4665 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04QY.f
--rw-r--r--   0 ben       (1000) users      (100)    13047 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04RD.f
--rw-r--r--   0 ben       (1000) users      (100)     6565 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04RV.f
--rw-r--r--   0 ben       (1000) users      (100)     5371 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04RW.f
--rw-r--r--   0 ben       (1000) users      (100)    13195 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04RX.f
--rw-r--r--   0 ben       (1000) users      (100)     7736 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04RY.f
--rw-r--r--   0 ben       (1000) users      (100)    10670 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB06ND.f
--rw-r--r--   0 ben       (1000) users      (100)    12742 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08CD.f
--rw-r--r--   0 ben       (1000) users      (100)    20654 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08DD.f
--rw-r--r--   0 ben       (1000) users      (100)    12831 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08ED.f
--rw-r--r--   0 ben       (1000) users      (100)    22423 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08FD.f
--rw-r--r--   0 ben       (1000) users      (100)     7978 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08GD.f
--rw-r--r--   0 ben       (1000) users      (100)     8539 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08HD.f
--rw-r--r--   0 ben       (1000) users      (100)    14316 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08MD.f
--rw-r--r--   0 ben       (1000) users      (100)     2407 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08MY.f
--rw-r--r--   0 ben       (1000) users      (100)    12182 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08ND.f
--rw-r--r--   0 ben       (1000) users      (100)     1789 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08NY.f
--rw-r--r--   0 ben       (1000) users      (100)     7496 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB09MD.f
--rw-r--r--   0 ben       (1000) users      (100)    30294 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10AD.f
--rw-r--r--   0 ben       (1000) users      (100)    34738 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10DD.f
--rw-r--r--   0 ben       (1000) users      (100)    16346 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10ED.f
--rw-r--r--   0 ben       (1000) users      (100)    16906 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10FD.f
--rw-r--r--   0 ben       (1000) users      (100)    12718 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10HD.f
--rw-r--r--   0 ben       (1000) users      (100)    18316 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10ID.f
--rw-r--r--   0 ben       (1000) users      (100)    10650 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10JD.f
--rw-r--r--   0 ben       (1000) users      (100)    20934 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10KD.f
--rw-r--r--   0 ben       (1000) users      (100)    13819 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10LD.f
--rw-r--r--   0 ben       (1000) users      (100)    23576 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10MD.f
--rw-r--r--   0 ben       (1000) users      (100)    17239 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10PD.f
--rw-r--r--   0 ben       (1000) users      (100)    19644 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10QD.f
--rw-r--r--   0 ben       (1000) users      (100)    23673 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10RD.f
--rw-r--r--   0 ben       (1000) users      (100)    20581 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10SD.f
--rw-r--r--   0 ben       (1000) users      (100)    10872 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10TD.f
--rw-r--r--   0 ben       (1000) users      (100)    13495 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10UD.f
--rw-r--r--   0 ben       (1000) users      (100)    12236 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10VD.f
--rw-r--r--   0 ben       (1000) users      (100)     9207 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10WD.f
--rw-r--r--   0 ben       (1000) users      (100)    21377 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10YD.f
--rw-r--r--   0 ben       (1000) users      (100)    29986 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10ZD.f
--rw-r--r--   0 ben       (1000) users      (100)    10582 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10ZP.f
--rw-r--r--   0 ben       (1000) users      (100)    28304 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB16AD.f
--rw-r--r--   0 ben       (1000) users      (100)    31201 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB16AY.f
--rw-r--r--   0 ben       (1000) users      (100)    24504 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB16BD.f
--rw-r--r--   0 ben       (1000) users      (100)    19937 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB16CD.f
--rw-r--r--   0 ben       (1000) users      (100)    12843 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB16CY.f
--rw-r--r--   0 ben       (1000) users      (100)    34716 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG02AD.f
--rw-r--r--   0 ben       (1000) users      (100)    17103 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG02CV.f
--rw-r--r--   0 ben       (1000) users      (100)   116531 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG02CW.f
--rw-r--r--   0 ben       (1000) users      (100)    25459 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG02CX.f
--rw-r--r--   0 ben       (1000) users      (100)    47210 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG02ND.f
--rw-r--r--   0 ben       (1000) users      (100)    23750 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03AD.f
--rw-r--r--   0 ben       (1000) users      (100)    21210 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03AX.f
--rw-r--r--   0 ben       (1000) users      (100)    21191 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03AY.f
--rw-r--r--   0 ben       (1000) users      (100)    34718 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BD.f
--rw-r--r--   0 ben       (1000) users      (100)     5365 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BR.f
--rw-r--r--   0 ben       (1000) users      (100)    22062 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BS.f
--rw-r--r--   0 ben       (1000) users      (100)    19412 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BT.f
--rw-r--r--   0 ben       (1000) users      (100)    25072 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BU.f
--rw-r--r--   0 ben       (1000) users      (100)    22444 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BV.f
--rw-r--r--   0 ben       (1000) users      (100)    13950 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BW.f
--rw-r--r--   0 ben       (1000) users      (100)    26021 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BX.f
--rw-r--r--   0 ben       (1000) users      (100)     2033 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BY.f
--rw-r--r--   0 ben       (1000) users      (100)    32696 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BZ.f
--rw-r--r--   0 ben       (1000) users      (100)     6189 2021-02-21 11:35:22.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SLCT_DLATZM.f
--rw-r--r--   0 ben       (1000) users      (100)     6252 2021-02-21 11:35:22.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/SLCT_ZLATZM.f
--rw-r--r--   0 ben       (1000) users      (100)    11518 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01ID.f
--rw-r--r--   0 ben       (1000) users      (100)    11693 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01IZ.f
--rw-r--r--   0 ben       (1000) users      (100)    11816 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01KD.f
--rw-r--r--   0 ben       (1000) users      (100)     8224 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01KX.f
--rw-r--r--   0 ben       (1000) users      (100)    11735 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01LD.f
--rw-r--r--   0 ben       (1000) users      (100)    10505 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01MD.f
--rw-r--r--   0 ben       (1000) users      (100)    10706 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01ND.f
--rw-r--r--   0 ben       (1000) users      (100)    12198 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01PD.f
--rw-r--r--   0 ben       (1000) users      (100)    17370 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01PX.f
--rw-r--r--   0 ben       (1000) users      (100)     9848 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01TD.f
--rw-r--r--   0 ben       (1000) users      (100)     4161 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01TY.f
--rw-r--r--   0 ben       (1000) users      (100)    17290 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01UD.f
--rw-r--r--   0 ben       (1000) users      (100)    10382 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01UX.f
--rw-r--r--   0 ben       (1000) users      (100)    22004 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01UY.f
--rw-r--r--   0 ben       (1000) users      (100)    16941 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01VD.f
--rw-r--r--   0 ben       (1000) users      (100)     9543 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01VY.f
--rw-r--r--   0 ben       (1000) users      (100)     8088 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01WD.f
--rw-r--r--   0 ben       (1000) users      (100)     9704 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01WX.f
--rw-r--r--   0 ben       (1000) users      (100)     8006 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01XD.f
--rw-r--r--   0 ben       (1000) users      (100)     7878 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01XZ.f
--rw-r--r--   0 ben       (1000) users      (100)     4568 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01YD.f
--rw-r--r--   0 ben       (1000) users      (100)    14799 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01ZD.f
--rw-r--r--   0 ben       (1000) users      (100)    26079 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB03AD.f
--rw-r--r--   0 ben       (1000) users      (100)     4777 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB03AY.f
--rw-r--r--   0 ben       (1000) users      (100)    13925 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04AD.f
--rw-r--r--   0 ben       (1000) users      (100)     8158 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04AY.f
--rw-r--r--   0 ben       (1000) users      (100)    21420 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04BD.f
--rw-r--r--   0 ben       (1000) users      (100)    10662 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04BV.f
--rw-r--r--   0 ben       (1000) users      (100)     8554 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04BW.f
--rw-r--r--   0 ben       (1000) users      (100)     6965 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04BX.f
--rw-r--r--   0 ben       (1000) users      (100)    20498 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04CD.f
--rw-r--r--   0 ben       (1000) users      (100)    17929 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB05AD.f
--rw-r--r--   0 ben       (1000) users      (100)     6850 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TC01OD.f
--rw-r--r--   0 ben       (1000) users      (100)    16163 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TC04AD.f
--rw-r--r--   0 ben       (1000) users      (100)    13038 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TC05AD.f
--rw-r--r--   0 ben       (1000) users      (100)    21042 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TD03AD.f
--rw-r--r--   0 ben       (1000) users      (100)     5436 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TD03AY.f
--rw-r--r--   0 ben       (1000) users      (100)    14731 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TD04AD.f
--rw-r--r--   0 ben       (1000) users      (100)     8657 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TD05AD.f
--rw-r--r--   0 ben       (1000) users      (100)     6781 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01MD.f
--rw-r--r--   0 ben       (1000) users      (100)    13198 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01MX.f
--rw-r--r--   0 ben       (1000) users      (100)    11789 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01MY.f
--rw-r--r--   0 ben       (1000) users      (100)     8179 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01ND.f
--rw-r--r--   0 ben       (1000) users      (100)     4826 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01OD.f
--rw-r--r--   0 ben       (1000) users      (100)     4931 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01PD.f
--rw-r--r--   0 ben       (1000) users      (100)     7255 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01QD.f
--rw-r--r--   0 ben       (1000) users      (100)     6435 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01RD.f
--rw-r--r--   0 ben       (1000) users      (100)    15534 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01AD.f
--rw-r--r--   0 ben       (1000) users      (100)    15790 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01AZ.f
--rw-r--r--   0 ben       (1000) users      (100)    15683 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01BD.f
--rw-r--r--   0 ben       (1000) users      (100)     8797 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01CD.f
--rw-r--r--   0 ben       (1000) users      (100)     8968 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01DD.f
--rw-r--r--   0 ben       (1000) users      (100)    28377 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01ED.f
--rw-r--r--   0 ben       (1000) users      (100)    26004 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01FD.f
--rw-r--r--   0 ben       (1000) users      (100)    26204 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01FZ.f
--rw-r--r--   0 ben       (1000) users      (100)    16187 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01GD.f
--rw-r--r--   0 ben       (1000) users      (100)    19720 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01HD.f
--rw-r--r--   0 ben       (1000) users      (100)    29831 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01HU.f
--rw-r--r--   0 ben       (1000) users      (100)    23696 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01HX.f
--rw-r--r--   0 ben       (1000) users      (100)    31804 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01HY.f
--rw-r--r--   0 ben       (1000) users      (100)    21425 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01ID.f
--rw-r--r--   0 ben       (1000) users      (100)    23430 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01JD.f
--rw-r--r--   0 ben       (1000) users      (100)    39681 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01JY.f
--rw-r--r--   0 ben       (1000) users      (100)    11157 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01KD.f
--rw-r--r--   0 ben       (1000) users      (100)    11457 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01KZ.f
--rw-r--r--   0 ben       (1000) users      (100)    19227 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01LD.f
--rw-r--r--   0 ben       (1000) users      (100)    27137 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01LY.f
--rw-r--r--   0 ben       (1000) users      (100)    16640 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01MD.f
--rw-r--r--   0 ben       (1000) users      (100)    19789 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01ND.f
--rw-r--r--   0 ben       (1000) users      (100)    11559 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01NX.f
--rw-r--r--   0 ben       (1000) users      (100)     5401 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01OA.f
--rw-r--r--   0 ben       (1000) users      (100)     5582 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01OB.f
--rw-r--r--   0 ben       (1000) users      (100)    11395 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01OD.f
--rw-r--r--   0 ben       (1000) users      (100)    11772 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01OZ.f
--rw-r--r--   0 ben       (1000) users      (100)    19572 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01PD.f
--rw-r--r--   0 ben       (1000) users      (100)    19304 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01QD.f
--rw-r--r--   0 ben       (1000) users      (100)    10460 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01WD.f
--rw-r--r--   0 ben       (1000) users      (100)     3375 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01BD.f
--rw-r--r--   0 ben       (1000) users      (100)     4803 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01CD.f
--rw-r--r--   0 ben       (1000) users      (100)     3066 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01DD.f
--rw-r--r--   0 ben       (1000) users      (100)     4214 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01MD.f
--rw-r--r--   0 ben       (1000) users      (100)     4155 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01MZ.f
--rw-r--r--   0 ben       (1000) users      (100)     5338 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01ND.f
--rw-r--r--   0 ben       (1000) users      (100)     8563 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/UE01MD.f
--rw-r--r--   0 ben       (1000) users      (100)      198 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/delctg.f
--rw-r--r--   0 ben       (1000) users      (100)     8443 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/makefile
--rw-r--r--   0 ben       (1000) users      (100)      348 2021-02-07 14:11:14.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/readme
--rw-r--r--   0 ben       (1000) users      (100)      186 2022-07-09 12:47:33.000000 slycot-0.5.3/slycot/src/SLICOT-Reference/src/select.f
--rw-r--r--   0 ben       (1000) users      (100)      207 2021-01-22 23:20:08.000000 slycot-0.5.3/slycot/src/XERBLA.f
--rw-r--r--   0 ben       (1000) users      (100)      335 2021-01-22 23:20:08.000000 slycot-0.5.3/slycot/src/_helper.pyf
--rw-r--r--   0 ben       (1000) users      (100)      292 2021-01-22 23:20:08.000000 slycot-0.5.3/slycot/src/_wrapper.pyf
--rw-r--r--   0 ben       (1000) users      (100)    23086 2022-12-19 11:28:53.000000 slycot-0.5.3/slycot/src/analysis.pyf
--rw-r--r--   0 ben       (1000) users      (100)      252 2021-01-22 23:20:08.000000 slycot-0.5.3/slycot/src/ftruefalse.f
--rw-r--r--   0 ben       (1000) users      (100)     6368 2022-12-19 11:28:53.000000 slycot-0.5.3/slycot/src/math.pyf
--rw-r--r--   0 ben       (1000) users      (100)    46295 2022-07-09 14:31:14.000000 slycot-0.5.3/slycot/src/synthesis.pyf
--rw-r--r--   0 ben       (1000) users      (100)    28949 2021-01-22 23:20:08.000000 slycot-0.5.3/slycot/src/transform.pyf
--rw-r--r--   0 ben       (1000) users      (100)   107860 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/synthesis.py
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.684944 slycot-0.5.3/slycot/tests/
--rw-r--r--   0 ben       (1000) users      (100)      359 2021-01-22 23:20:08.000000 slycot-0.5.3/slycot/tests/CMakeLists.txt
--rw-r--r--   0 ben       (1000) users      (100)        0 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/__init__.py
--rw-r--r--   0 ben       (1000) users      (100)     1936 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_ab01.py
--rw-r--r--   0 ben       (1000) users      (100)     3063 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_ab08n.py
--rw-r--r--   0 ben       (1000) users      (100)     4107 2022-05-29 11:49:04.000000 slycot-0.5.3/slycot/tests/test_ab13md.py
--rw-r--r--   0 ben       (1000) users      (100)     4145 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_ag08bd.py
--rw-r--r--   0 ben       (1000) users      (100)     2434 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_analysis.py
--rw-r--r--   0 ben       (1000) users      (100)     1952 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_examples.py
--rw-r--r--   0 ben       (1000) users      (100)     4390 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_exceptions.py
--rw-r--r--   0 ben       (1000) users      (100)    14232 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_mb.py
--rw-r--r--   0 ben       (1000) users      (100)     1575 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_mc.py
--rw-r--r--   0 ben       (1000) users      (100)     8712 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_sb.py
--rw-r--r--   0 ben       (1000) users      (100)     1531 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_sg02ad.py
--rw-r--r--   0 ben       (1000) users      (100)     2591 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_sg03ad.py
--rw-r--r--   0 ben       (1000) users      (100)     8898 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_tb05ad.py
--rw-r--r--   0 ben       (1000) users      (100)     8707 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_td04ad.py
--rw-r--r--   0 ben       (1000) users      (100)     2573 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_tg01ad.py
--rw-r--r--   0 ben       (1000) users      (100)     4403 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_tg01fd.py
--rw-r--r--   0 ben       (1000) users      (100)      914 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/tests/test_transform.py
--rw-r--r--   0 ben       (1000) users      (100)    55443 2022-07-10 10:32:17.000000 slycot-0.5.3/slycot/transform.py
--rw-r--r--   0 ben       (1000) users      (100)      160 2022-12-21 09:30:09.000000 slycot-0.5.3/slycot/version.py
-drwxr-xr-x   0 ben       (1000) users      (100)        0 2022-12-21 09:30:10.048930 slycot-0.5.3/slycot.egg-info/
--rw-r--r--   0 ben       (1000) users      (100)    10351 2022-12-21 09:30:10.000000 slycot-0.5.3/slycot.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (100)    89064 2022-12-21 09:30:10.000000 slycot-0.5.3/slycot.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) users      (100)        1 2022-12-21 09:30:10.000000 slycot-0.5.3/slycot.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) users      (100)        6 2022-12-21 09:30:10.000000 slycot-0.5.3/slycot.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) users      (100)        7 2022-12-21 09:30:10.000000 slycot-0.5.3/slycot.egg-info/top_level.txt
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:48.058601 slycot-0.5.4/
+-rw-r--r--   0 ben       (1000) users      (100)      191 2022-07-16 10:42:02.000000 slycot-0.5.4/.coveragerc
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.374582 slycot-0.5.4/.github/
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.374582 slycot-0.5.4/.github/conda-env/
+-rw-r--r--   0 ben       (1000) users      (100)       57 2022-12-21 09:29:38.000000 slycot-0.5.4/.github/conda-env/build-env.yml
+-rw-r--r--   0 ben       (1000) users      (100)      270 2022-12-21 09:29:38.000000 slycot-0.5.4/.github/conda-env/test-env.yml
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.374582 slycot-0.5.4/.github/scripts/
+-rw-r--r--   0 ben       (1000) users      (100)     1186 2021-01-30 12:23:36.000000 slycot-0.5.4/.github/scripts/run-tests.sh
+-rw-r--r--   0 ben       (1000) users      (100)      988 2021-02-07 11:42:42.000000 slycot-0.5.4/.github/scripts/set-conda-test-matrix.py
+-rw-r--r--   0 ben       (1000) users      (100)      865 2021-01-30 12:23:36.000000 slycot-0.5.4/.github/scripts/set-pip-test-matrix.py
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.374582 slycot-0.5.4/.github/workflows/
+-rw-r--r--   0 ben       (1000) users      (100)    13081 2023-03-24 20:29:27.000000 slycot-0.5.4/.github/workflows/slycot-build-and-test.yml
+-rw-r--r--   0 ben       (1000) users      (100)      130 2021-01-22 23:20:08.000000 slycot-0.5.4/.gitignore
+-rw-r--r--   0 ben       (1000) users      (100)      136 2021-03-17 11:49:25.000000 slycot-0.5.4/.gitmodules
+-rw-r--r--   0 ben       (1000) users      (100)      328 2021-01-22 23:20:08.000000 slycot-0.5.4/AUTHORS
+-rw-r--r--   0 ben       (1000) users      (100)      758 2022-11-08 14:30:23.000000 slycot-0.5.4/CMakeLists.txt
+-rw-r--r--   0 ben       (1000) users      (100)      750 2021-01-22 23:20:08.000000 slycot-0.5.4/COPYING
+-rw-r--r--   0 ben       (1000) users      (100)      334 2022-10-30 11:05:45.000000 slycot-0.5.4/MANIFEST.in
+-rw-r--r--   0 ben       (1000) users      (100)    10373 2023-04-27 19:48:48.058601 slycot-0.5.4/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (100)     9065 2022-11-23 20:17:18.000000 slycot-0.5.4/README.rst
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.378582 slycot-0.5.4/conda-recipe/
+-rw-r--r--   0 ben       (1000) users      (100)      195 2022-05-03 20:29:21.000000 slycot-0.5.4/conda-recipe/bld.bat
+-rw-r--r--   0 ben       (1000) users      (100)      178 2022-05-03 20:29:21.000000 slycot-0.5.4/conda-recipe/build.sh
+-rw-r--r--   0 ben       (1000) users      (100)     1568 2023-03-24 20:29:44.000000 slycot-0.5.4/conda-recipe/meta.yaml
+-rw-r--r--   0 ben       (1000) users      (100)    18092 2021-01-22 23:20:08.000000 slycot-0.5.4/gpl-2.0.txt
+-rw-r--r--   0 ben       (1000) users      (100)     1622 2023-04-25 19:02:16.000000 slycot-0.5.4/pyproject.toml
+-rw-r--r--   0 ben       (1000) users      (100)       38 2023-04-27 19:48:48.058601 slycot-0.5.4/setup.cfg
+-rw-r--r--   0 ben       (1000) users      (100)     2149 2023-04-26 07:25:53.000000 slycot-0.5.4/setup.py
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.382582 slycot-0.5.4/slycot/
+-rw-r--r--   0 ben       (1000) users      (100)    22431 2022-12-21 09:29:38.000000 slycot-0.5.4/slycot/CMakeLists.txt
+-rw-r--r--   0 ben       (1000) users      (100)     1546 2022-10-30 11:05:45.000000 slycot-0.5.4/slycot/__init__.py
+-rw-r--r--   0 ben       (1000) users      (100)    85946 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/analysis.py
+-rw-r--r--   0 ben       (1000) users      (100)     9082 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/examples.py
+-rw-r--r--   0 ben       (1000) users      (100)     8737 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/exceptions.py
+-rw-r--r--   0 ben       (1000) users      (100)    30976 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/math.py
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.386582 slycot-0.5.4/slycot/src/
+-rw-r--r--   0 ben       (1000) users      (100)      668 2021-03-17 11:49:25.000000 slycot-0.5.4/slycot/src/Readme.md
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.390583 slycot-0.5.4/slycot/src/SLICOT-Reference/
+-rw-r--r--   0 ben       (1000) users      (100)       58 2021-02-07 20:42:18.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/.git
+-rw-r--r--   0 ben       (1000) users      (100)     1862 2022-05-29 11:35:56.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/Contributors.md
+-rw-r--r--   0 ben       (1000) users      (100)     4169 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/Installation.md
+-rw-r--r--   0 ben       (1000) users      (100)     1514 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/LICENSE
+-rw-r--r--   0 ben       (1000) users      (100)     3256 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/README.md
+-rw-r--r--   0 ben       (1000) users      (100)    19422 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/ReleaseNotes.md
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.402583 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/
+-rw-r--r--   0 ben       (1000) users      (100)      492 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB01103.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1737 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB01104.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1312 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB01105.dat
+-rw-r--r--   0 ben       (1000) users      (100)    13457 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB01106.dat
+-rw-r--r--   0 ben       (1000) users      (100)    10508 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB012091.dat
+-rw-r--r--   0 ben       (1000) users      (100)     8597 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB012092.dat
+-rw-r--r--   0 ben       (1000) users      (100)    11788 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB01404.dat
+-rw-r--r--   0 ben       (1000) users      (100)      240 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB02105.dat
+-rw-r--r--   0 ben       (1000) users      (100)      288 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB02106.dat
+-rw-r--r--   0 ben       (1000) users      (100)      363 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB02107.dat
+-rw-r--r--   0 ben       (1000) users      (100)      420 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB02108.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1190 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB02110.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1435 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB02111.dat
+-rw-r--r--   0 ben       (1000) users      (100)     6612 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB02113.dat
+-rw-r--r--   0 ben       (1000) users      (100)      296 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01103.dat
+-rw-r--r--   0 ben       (1000) users      (100)      969 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01104.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1312 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01105.dat
+-rw-r--r--   0 ben       (1000) users      (100)    13457 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01106.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1849 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01107.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1297 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01108.dat
+-rw-r--r--   0 ben       (1000) users      (100)    38186 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01109.dat
+-rw-r--r--   0 ben       (1000) users      (100)      961 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01110.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1020 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01203.dat
+-rw-r--r--   0 ben       (1000) users      (100)      101 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012051.dat
+-rw-r--r--   0 ben       (1000) users      (100)      394 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012052.dat
+-rw-r--r--   0 ben       (1000) users      (100)      886 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012053.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1542 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012054.dat
+-rw-r--r--   0 ben       (1000) users      (100)     2410 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012055.dat
+-rw-r--r--   0 ben       (1000) users      (100)     3489 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012056.dat
+-rw-r--r--   0 ben       (1000) users      (100)     9561 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012057.dat
+-rw-r--r--   0 ben       (1000) users      (100)      375 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01206.dat
+-rw-r--r--   0 ben       (1000) users      (100)    11346 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01304.dat
+-rw-r--r--   0 ben       (1000) users      (100)      244 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD02106.dat
+-rw-r--r--   0 ben       (1000) users      (100)      296 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD02107.dat
+-rw-r--r--   0 ben       (1000) users      (100)      332 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD02108.dat
+-rw-r--r--   0 ben       (1000) users      (100)      430 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD02109.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1190 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD02111.dat
+-rw-r--r--   0 ben       (1000) users      (100)      185 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD02112.dat
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.650590 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/
+-rw-r--r--   0 ben       (1000) users      (100)    10439 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13617 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB01ND.html
+-rw-r--r--   0 ben       (1000) users      (100)    15601 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB01OD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10500 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB04MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    16184 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15634 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05ND.html
+-rw-r--r--   0 ben       (1000) users      (100)    14975 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05OD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13669 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05PD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15645 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05QD.html
+-rw-r--r--   0 ben       (1000) users      (100)    16003 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05RD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6652 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05SD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8104 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB07MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8808 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB07ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     5754 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5828 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08MZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    19657 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08ND.html
+-rw-r--r--   0 ben       (1000) users      (100)    20520 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08NW.html
+-rw-r--r--   0 ben       (1000) users      (100)     6715 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08NX.html
+-rw-r--r--   0 ben       (1000) users      (100)     8474 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08NY.html
+-rw-r--r--   0 ben       (1000) users      (100)    20172 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08NZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    14482 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10136 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09AX.html
+-rw-r--r--   0 ben       (1000) users      (100)    15744 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09BD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10850 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09BX.html
+-rw-r--r--   0 ben       (1000) users      (100)    16037 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09CD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10067 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09CX.html
+-rw-r--r--   0 ben       (1000) users      (100)    10626 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09DD.html
+-rw-r--r--   0 ben       (1000) users      (100)    18851 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09ED.html
+-rw-r--r--   0 ben       (1000) users      (100)    19104 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09FD.html
+-rw-r--r--   0 ben       (1000) users      (100)    20632 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09GD.html
+-rw-r--r--   0 ben       (1000) users      (100)    23079 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09HD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13053 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09HX.html
+-rw-r--r--   0 ben       (1000) users      (100)     6109 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09HY.html
+-rw-r--r--   0 ben       (1000) users      (100)    38139 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09ID.html
+-rw-r--r--   0 ben       (1000) users      (100)    13673 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09IX.html
+-rw-r--r--   0 ben       (1000) users      (100)    16029 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09IY.html
+-rw-r--r--   0 ben       (1000) users      (100)    34224 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09JD.html
+-rw-r--r--   0 ben       (1000) users      (100)    14431 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09JV.html
+-rw-r--r--   0 ben       (1000) users      (100)    14420 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09JW.html
+-rw-r--r--   0 ben       (1000) users      (100)     4647 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09JX.html
+-rw-r--r--   0 ben       (1000) users      (100)    31860 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09KD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15796 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09KX.html
+-rw-r--r--   0 ben       (1000) users      (100)    16846 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    18265 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09ND.html
+-rw-r--r--   0 ben       (1000) users      (100)    11723 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13AD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5121 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13AX.html
+-rw-r--r--   0 ben       (1000) users      (100)    12848 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13BD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9237 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13CD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15801 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13DD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9352 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13DX.html
+-rw-r--r--   0 ben       (1000) users      (100)     8381 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13ED.html
+-rw-r--r--   0 ben       (1000) users      (100)     8583 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13FD.html
+-rw-r--r--   0 ben       (1000) users      (100)    26176 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13ID.html
+-rw-r--r--   0 ben       (1000) users      (100)     9468 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6806 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB8NXZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     6359 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AG07BD.html
+-rw-r--r--   0 ben       (1000) users      (100)    30005 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AG08BD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9124 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AG08BY.html
+-rw-r--r--   0 ben       (1000) users      (100)    29847 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AG08BZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     9318 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AG8BYZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    24747 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BB01AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    22080 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BB02AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    12650 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BB03AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    12644 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BB04AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    11789 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BD01AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10951 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BD02AD.html
+-rw-r--r--   0 ben       (1000) users      (100)   114864 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DAESolver.html
+-rw-r--r--   0 ben       (1000) users      (100)     4784 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DE01OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5679 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DE01PD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7489 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DF01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5966 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DG01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9284 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DG01ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     5403 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DG01OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4704 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DK01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    17140 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FB01QD.html
+-rw-r--r--   0 ben       (1000) users      (100)    17900 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FB01RD.html
+-rw-r--r--   0 ben       (1000) users      (100)    20362 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FB01SD.html
+-rw-r--r--   0 ben       (1000) users      (100)    20707 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FB01TD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13220 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FB01VD.html
+-rw-r--r--   0 ben       (1000) users      (100)    14387 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FD01AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    16749 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FSQP.html
+-rw-r--r--   0 ben       (1000) users      (100)    47491 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    51068 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01BD.html
+-rw-r--r--   0 ben       (1000) users      (100)    54820 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01CD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15536 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    11259 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01MY.html
+-rw-r--r--   0 ben       (1000) users      (100)     9283 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     3923 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2303 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01OY.html
+-rw-r--r--   0 ben       (1000) users      (100)    16939 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01PD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10622 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01PX.html
+-rw-r--r--   0 ben       (1000) users      (100)    15620 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01PY.html
+-rw-r--r--   0 ben       (1000) users      (100)    14429 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01QD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9362 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01RD.html
+-rw-r--r--   0 ben       (1000) users      (100)    66249 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB03AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    67654 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB03BD.html
+-rw-r--r--   0 ben       (1000) users      (100)    29374 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/KINSOL.html
+-rw-r--r--   0 ben       (1000) users      (100)     2075 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA01AD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2318 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA01BD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2330 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA01BZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     2340 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA01CD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2319 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02AD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2690 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02AZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     2688 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02BD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2697 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02BZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     2534 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02CD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2543 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02CZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     3744 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02DD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2295 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02ED.html
+-rw-r--r--   0 ben       (1000) users      (100)     2370 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02ES.html
+-rw-r--r--   0 ben       (1000) users      (100)     3288 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02EZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     2165 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02FD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3516 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02GD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3518 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02GZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     2783 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02HD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2840 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02HZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     3590 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02ID.html
+-rw-r--r--   0 ben       (1000) users      (100)     3876 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02IZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     3100 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02JD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3097 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02JZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     3244 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3296 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02MZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     3477 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02NZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     2874 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3055 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02OZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     1934 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02PD.html
+-rw-r--r--   0 ben       (1000) users      (100)     1934 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02PZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     5585 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01KD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7364 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01LD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4306 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4367 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     5063 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OC.html
+-rw-r--r--   0 ben       (1000) users      (100)     6957 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4460 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OE.html
+-rw-r--r--   0 ben       (1000) users      (100)     4424 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OH.html
+-rw-r--r--   0 ben       (1000) users      (100)     4565 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OO.html
+-rw-r--r--   0 ben       (1000) users      (100)     4248 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OS.html
+-rw-r--r--   0 ben       (1000) users      (100)     4425 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OT.html
+-rw-r--r--   0 ben       (1000) users      (100)     5070 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01PD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4478 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01QD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6803 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RB.html
+-rw-r--r--   0 ben       (1000) users      (100)     7487 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6252 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RH.html
+-rw-r--r--   0 ben       (1000) users      (100)     6120 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RT.html
+-rw-r--r--   0 ben       (1000) users      (100)     6493 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RU.html
+-rw-r--r--   0 ben       (1000) users      (100)     3741 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RW.html
+-rw-r--r--   0 ben       (1000) users      (100)     6760 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RX.html
+-rw-r--r--   0 ben       (1000) users      (100)     5823 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RY.html
+-rw-r--r--   0 ben       (1000) users      (100)     2601 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01SD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3055 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01SS.html
+-rw-r--r--   0 ben       (1000) users      (100)     5348 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01TD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4261 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01UD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4763 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01UW.html
+-rw-r--r--   0 ben       (1000) users      (100)     6040 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01UX.html
+-rw-r--r--   0 ben       (1000) users      (100)     5183 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01UY.html
+-rw-r--r--   0 ben       (1000) users      (100)     5259 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01UZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     5144 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01VD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6315 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01WD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3472 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01XD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3482 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01XY.html
+-rw-r--r--   0 ben       (1000) users      (100)     6292 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01YD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6768 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01ZD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13036 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02CD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9730 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02CU.html
+-rw-r--r--   0 ben       (1000) users      (100)    10630 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02CV.html
+-rw-r--r--   0 ben       (1000) users      (100)     5892 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02CX.html
+-rw-r--r--   0 ben       (1000) users      (100)     5642 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02CY.html
+-rw-r--r--   0 ben       (1000) users      (100)    20569 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02DD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9491 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02ED.html
+-rw-r--r--   0 ben       (1000) users      (100)    13962 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02FD.html
+-rw-r--r--   0 ben       (1000) users      (100)    11272 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02GD.html
+-rw-r--r--   0 ben       (1000) users      (100)    12422 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02HD.html
+-rw-r--r--   0 ben       (1000) users      (100)    12167 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02ID.html
+-rw-r--r--   0 ben       (1000) users      (100)    12349 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02JD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13496 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02JX.html
+-rw-r--r--   0 ben       (1000) users      (100)    11412 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02KD.html
+-rw-r--r--   0 ben       (1000) users      (100)    17097 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    23196 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     6968 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02NY.html
+-rw-r--r--   0 ben       (1000) users      (100)     6734 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02OD.html
+-rw-r--r--   0 ben       (1000) users      (100)    14113 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02PD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13193 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02QD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6224 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02QY.html
+-rw-r--r--   0 ben       (1000) users      (100)     3421 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02RD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3392 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02RZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     6547 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02SD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3116 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02SZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     3482 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02TD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3523 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02TZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     9952 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02UD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2940 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02UU.html
+-rw-r--r--   0 ben       (1000) users      (100)     3015 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02UV.html
+-rw-r--r--   0 ben       (1000) users      (100)     4976 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02UW.html
+-rw-r--r--   0 ben       (1000) users      (100)     6361 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02VD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10790 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02WD.html
+-rw-r--r--   0 ben       (1000) users      (100)    11049 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02XD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6862 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02YD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4795 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AB.html
+-rw-r--r--   0 ben       (1000) users      (100)     4021 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4428 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AE.html
+-rw-r--r--   0 ben       (1000) users      (100)     4176 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AF.html
+-rw-r--r--   0 ben       (1000) users      (100)     4668 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AG.html
+-rw-r--r--   0 ben       (1000) users      (100)     4818 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AH.html
+-rw-r--r--   0 ben       (1000) users      (100)     4433 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AI.html
+-rw-r--r--   0 ben       (1000) users      (100)     2213 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BA.html
+-rw-r--r--   0 ben       (1000) users      (100)     4210 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BB.html
+-rw-r--r--   0 ben       (1000) users      (100)     4704 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BC.html
+-rw-r--r--   0 ben       (1000) users      (100)    19841 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2808 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BE.html
+-rw-r--r--   0 ben       (1000) users      (100)     3090 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BF.html
+-rw-r--r--   0 ben       (1000) users      (100)    15953 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     8066 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03CD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4103 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03CZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     7308 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03DD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3424 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03DZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     6126 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03ED.html
+-rw-r--r--   0 ben       (1000) users      (100)     5606 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03FD.html
+-rw-r--r--   0 ben       (1000) users      (100)    24239 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03FZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     4706 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03GD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3525 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03GZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     4609 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03HD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2907 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03HZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    12632 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03ID.html
+-rw-r--r--   0 ben       (1000) users      (100)    11941 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03IZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     9167 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03JD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9461 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03JP.html
+-rw-r--r--   0 ben       (1000) users      (100)     8428 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03JZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    10505 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03KA.html
+-rw-r--r--   0 ben       (1000) users      (100)    10138 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03KB.html
+-rw-r--r--   0 ben       (1000) users      (100)     4596 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03KC.html
+-rw-r--r--   0 ben       (1000) users      (100)    19898 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03KD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6458 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03KE.html
+-rw-r--r--   0 ben       (1000) users      (100)    19519 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03LD.html
+-rw-r--r--   0 ben       (1000) users      (100)    20543 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03LF.html
+-rw-r--r--   0 ben       (1000) users      (100)    13796 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03LP.html
+-rw-r--r--   0 ben       (1000) users      (100)    20532 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03LZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    11706 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8716 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     3862 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03NY.html
+-rw-r--r--   0 ben       (1000) users      (100)    10579 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7560 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03OY.html
+-rw-r--r--   0 ben       (1000) users      (100)    11371 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03PD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7563 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03PY.html
+-rw-r--r--   0 ben       (1000) users      (100)    11372 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15736 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QG.html
+-rw-r--r--   0 ben       (1000) users      (100)     2854 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QV.html
+-rw-r--r--   0 ben       (1000) users      (100)     5601 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QW.html
+-rw-r--r--   0 ben       (1000) users      (100)     2159 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QX.html
+-rw-r--r--   0 ben       (1000) users      (100)     4231 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QY.html
+-rw-r--r--   0 ben       (1000) users      (100)    15483 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03RD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5894 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03RW.html
+-rw-r--r--   0 ben       (1000) users      (100)     5960 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03RX.html
+-rw-r--r--   0 ben       (1000) users      (100)     5886 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03RY.html
+-rw-r--r--   0 ben       (1000) users      (100)    10701 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03RZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     9360 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03SD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15914 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03TD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6348 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03TS.html
+-rw-r--r--   0 ben       (1000) users      (100)     8365 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03UD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13418 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03VD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8636 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03VW.html
+-rw-r--r--   0 ben       (1000) users      (100)     4913 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03VY.html
+-rw-r--r--   0 ben       (1000) users      (100)     5909 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03WA.html
+-rw-r--r--   0 ben       (1000) users      (100)    16586 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03WD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2900 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03WX.html
+-rw-r--r--   0 ben       (1000) users      (100)    26175 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03XD.html
+-rw-r--r--   0 ben       (1000) users      (100)    18234 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03XP.html
+-rw-r--r--   0 ben       (1000) users      (100)     7577 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03XS.html
+-rw-r--r--   0 ben       (1000) users      (100)    11313 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03XU.html
+-rw-r--r--   0 ben       (1000) users      (100)    32413 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03XZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     7348 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03YA.html
+-rw-r--r--   0 ben       (1000) users      (100)     8262 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03YD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4071 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03YT.html
+-rw-r--r--   0 ben       (1000) users      (100)    11772 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03ZA.html
+-rw-r--r--   0 ben       (1000) users      (100)    26201 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03ZD.html
+-rw-r--r--   0 ben       (1000) users      (100)    31322 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    26755 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04AZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    25688 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04BD.html
+-rw-r--r--   0 ben       (1000) users      (100)    17595 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04BP.html
+-rw-r--r--   0 ben       (1000) users      (100)    22893 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04BZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    14349 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04CD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4345 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DB.html
+-rw-r--r--   0 ben       (1000) users      (100)     8778 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3914 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DI.html
+-rw-r--r--   0 ben       (1000) users      (100)    14725 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DL.html
+-rw-r--r--   0 ben       (1000) users      (100)    18014 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DP.html
+-rw-r--r--   0 ben       (1000) users      (100)     8775 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DS.html
+-rw-r--r--   0 ben       (1000) users      (100)    11041 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DY.html
+-rw-r--r--   0 ben       (1000) users      (100)     9752 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    22966 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04ED.html
+-rw-r--r--   0 ben       (1000) users      (100)    19126 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04FD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13143 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04FP.html
+-rw-r--r--   0 ben       (1000) users      (100)     7117 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04GD.html
+-rw-r--r--   0 ben       (1000) users      (100)    11547 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04HD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5262 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04ID.html
+-rw-r--r--   0 ben       (1000) users      (100)     5201 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04IY.html
+-rw-r--r--   0 ben       (1000) users      (100)     5253 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04IZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     4973 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04JD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5324 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04KD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5303 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04LD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6063 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5862 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     3582 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04NY.html
+-rw-r--r--   0 ben       (1000) users      (100)     8981 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5731 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04OW.html
+-rw-r--r--   0 ben       (1000) users      (100)     2719 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04OX.html
+-rw-r--r--   0 ben       (1000) users      (100)     3460 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04OY.html
+-rw-r--r--   0 ben       (1000) users      (100)     7386 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04PA.html
+-rw-r--r--   0 ben       (1000) users      (100)    15575 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04PB.html
+-rw-r--r--   0 ben       (1000) users      (100)    15043 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04PU.html
+-rw-r--r--   0 ben       (1000) users      (100)     3532 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04PY.html
+-rw-r--r--   0 ben       (1000) users      (100)     7869 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04QB.html
+-rw-r--r--   0 ben       (1000) users      (100)     7879 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04QC.html
+-rw-r--r--   0 ben       (1000) users      (100)     6010 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04QF.html
+-rw-r--r--   0 ben       (1000) users      (100)     6804 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04QS.html
+-rw-r--r--   0 ben       (1000) users      (100)     7404 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04QU.html
+-rw-r--r--   0 ben       (1000) users      (100)     6522 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04RB.html
+-rw-r--r--   0 ben       (1000) users      (100)     5954 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04RU.html
+-rw-r--r--   0 ben       (1000) users      (100)     5581 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04SU.html
+-rw-r--r--   0 ben       (1000) users      (100)    24478 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04TB.html
+-rw-r--r--   0 ben       (1000) users      (100)    23832 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04TS.html
+-rw-r--r--   0 ben       (1000) users      (100)     1743 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04TU.html
+-rw-r--r--   0 ben       (1000) users      (100)    11241 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04UD.html
+-rw-r--r--   0 ben       (1000) users      (100)    19661 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04VD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6393 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04WD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5114 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04WP.html
+-rw-r--r--   0 ben       (1000) users      (100)     7581 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04WR.html
+-rw-r--r--   0 ben       (1000) users      (100)     5975 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04WU.html
+-rw-r--r--   0 ben       (1000) users      (100)    22354 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04XD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5375 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04XY.html
+-rw-r--r--   0 ben       (1000) users      (100)    17947 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04YD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7428 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04YW.html
+-rw-r--r--   0 ben       (1000) users      (100)    13508 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04ZD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10998 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB05MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6164 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB05MY.html
+-rw-r--r--   0 ben       (1000) users      (100)     7875 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB05ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     8093 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB05OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3553 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB05OY.html
+-rw-r--r--   0 ben       (1000) users      (100)     8896 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB3JZP.html
+-rw-r--r--   0 ben       (1000) users      (100)    13887 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB3LZP.html
+-rw-r--r--   0 ben       (1000) users      (100)     7524 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB3OYZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     7661 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB3PYZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     4369 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB4DBZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    15077 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB4DLZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    18237 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB4DPZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     5880 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4529 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     4766 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4743 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01PD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3058 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01PY.html
+-rw-r--r--   0 ben       (1000) users      (100)     7907 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01QD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7648 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01RD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7121 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01SD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8273 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01TD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4837 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01VD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5788 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01WD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6217 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01XD.html
+-rw-r--r--   0 ben       (1000) users      (100)    12146 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC03MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15153 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC03ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     3563 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC03NX.html
+-rw-r--r--   0 ben       (1000) users      (100)    31857 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MD03AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    42765 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MD03BD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4559 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MD03BX.html
+-rw-r--r--   0 ben       (1000) users      (100)     7702 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MD03BY.html
+-rw-r--r--   0 ben       (1000) users      (100)     4827 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01AD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4531 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01AY.html
+-rw-r--r--   0 ben       (1000) users      (100)     7321 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BD.html
+-rw-r--r--   0 ben       (1000) users      (100)    11887 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BP.html
+-rw-r--r--   0 ben       (1000) users      (100)    10913 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BQ.html
+-rw-r--r--   0 ben       (1000) users      (100)    10679 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BR.html
+-rw-r--r--   0 ben       (1000) users      (100)     8905 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BS.html
+-rw-r--r--   0 ben       (1000) users      (100)     5469 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BU.html
+-rw-r--r--   0 ben       (1000) users      (100)     4500 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BV.html
+-rw-r--r--   0 ben       (1000) users      (100)     4562 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BW.html
+-rw-r--r--   0 ben       (1000) users      (100)     3600 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BX.html
+-rw-r--r--   0 ben       (1000) users      (100)     5910 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BY.html
+-rw-r--r--   0 ben       (1000) users      (100)   136171 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/ODESolver.html
+-rw-r--r--   0 ben       (1000) users      (100)    16252 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01BD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3400 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01BX.html
+-rw-r--r--   0 ben       (1000) users      (100)     3764 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01BY.html
+-rw-r--r--   0 ben       (1000) users      (100)    11714 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01DD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4084 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01FY.html
+-rw-r--r--   0 ben       (1000) users      (100)     8033 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15794 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    12703 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02MT.html
+-rw-r--r--   0 ben       (1000) users      (100)     6955 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02MU.html
+-rw-r--r--   0 ben       (1000) users      (100)    14519 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02MX.html
+-rw-r--r--   0 ben       (1000) users      (100)    19786 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02ND.html
+-rw-r--r--   0 ben       (1000) users      (100)    22787 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02OD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13696 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02OY.html
+-rw-r--r--   0 ben       (1000) users      (100)    12944 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02PD.html
+-rw-r--r--   0 ben       (1000) users      (100)    18656 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02QD.html
+-rw-r--r--   0 ben       (1000) users      (100)    29677 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02RD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7860 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02RU.html
+-rw-r--r--   0 ben       (1000) users      (100)    20132 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02SD.html
+-rw-r--r--   0 ben       (1000) users      (100)    16880 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4787 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MU.html
+-rw-r--r--   0 ben       (1000) users      (100)     4952 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MV.html
+-rw-r--r--   0 ben       (1000) users      (100)     4954 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MW.html
+-rw-r--r--   0 ben       (1000) users      (100)     4625 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MX.html
+-rw-r--r--   0 ben       (1000) users      (100)     4346 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MY.html
+-rw-r--r--   0 ben       (1000) users      (100)    19084 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5036 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OR.html
+-rw-r--r--   0 ben       (1000) users      (100)     6434 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OS.html
+-rw-r--r--   0 ben       (1000) users      (100)     7554 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OT.html
+-rw-r--r--   0 ben       (1000) users      (100)    11168 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OU.html
+-rw-r--r--   0 ben       (1000) users      (100)     2853 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OV.html
+-rw-r--r--   0 ben       (1000) users      (100)     6980 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OY.html
+-rw-r--r--   0 ben       (1000) users      (100)    13769 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     8896 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03PD.html
+-rw-r--r--   0 ben       (1000) users      (100)    16046 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03QD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6720 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03QX.html
+-rw-r--r--   0 ben       (1000) users      (100)     6912 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03QY.html
+-rw-r--r--   0 ben       (1000) users      (100)     8782 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03RD.html
+-rw-r--r--   0 ben       (1000) users      (100)    16068 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03SD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6749 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03SX.html
+-rw-r--r--   0 ben       (1000) users      (100)     6954 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03SY.html
+-rw-r--r--   0 ben       (1000) users      (100)    18474 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03TD.html
+-rw-r--r--   0 ben       (1000) users      (100)    18566 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03UD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8750 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3239 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04MR.html
+-rw-r--r--   0 ben       (1000) users      (100)     3790 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04MU.html
+-rw-r--r--   0 ben       (1000) users      (100)     3082 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04MW.html
+-rw-r--r--   0 ben       (1000) users      (100)     3700 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04MY.html
+-rw-r--r--   0 ben       (1000) users      (100)     9874 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     3392 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04NV.html
+-rw-r--r--   0 ben       (1000) users      (100)     3315 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04NW.html
+-rw-r--r--   0 ben       (1000) users      (100)     4094 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04NX.html
+-rw-r--r--   0 ben       (1000) users      (100)     3937 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04NY.html
+-rw-r--r--   0 ben       (1000) users      (100)    23369 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6221 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04OW.html
+-rw-r--r--   0 ben       (1000) users      (100)    17243 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04PD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4812 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04PX.html
+-rw-r--r--   0 ben       (1000) users      (100)     5906 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04PY.html
+-rw-r--r--   0 ben       (1000) users      (100)     9171 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04QD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3418 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04QR.html
+-rw-r--r--   0 ben       (1000) users      (100)     4038 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04QU.html
+-rw-r--r--   0 ben       (1000) users      (100)     3825 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04QY.html
+-rw-r--r--   0 ben       (1000) users      (100)    10147 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04RD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4099 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04RV.html
+-rw-r--r--   0 ben       (1000) users      (100)     4004 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04RW.html
+-rw-r--r--   0 ben       (1000) users      (100)     4129 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04RX.html
+-rw-r--r--   0 ben       (1000) users      (100)     3892 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04RY.html
+-rw-r--r--   0 ben       (1000) users      (100)    10303 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB06ND.html
+-rw-r--r--   0 ben       (1000) users      (100)    16757 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08CD.html
+-rw-r--r--   0 ben       (1000) users      (100)    16279 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08DD.html
+-rw-r--r--   0 ben       (1000) users      (100)    16704 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08ED.html
+-rw-r--r--   0 ben       (1000) users      (100)    16086 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08FD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5887 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08GD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5904 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08HD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9740 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9769 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     8466 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB09MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15099 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    17568 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10DD.html
+-rw-r--r--   0 ben       (1000) users      (100)    16969 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10ED.html
+-rw-r--r--   0 ben       (1000) users      (100)    19334 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10FD.html
+-rw-r--r--   0 ben       (1000) users      (100)    14445 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10HD.html
+-rw-r--r--   0 ben       (1000) users      (100)    12091 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10ID.html
+-rw-r--r--   0 ben       (1000) users      (100)     4986 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10JD.html
+-rw-r--r--   0 ben       (1000) users      (100)    12209 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10KD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7335 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10LD.html
+-rw-r--r--   0 ben       (1000) users      (100)    11444 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8357 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10PD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8970 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10QD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9068 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10RD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9549 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10SD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7290 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10TD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7429 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10UD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7168 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10VD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6885 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10WD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8488 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10YD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13619 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10ZD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5413 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10ZP.html
+-rw-r--r--   0 ben       (1000) users      (100)    26050 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB16AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    11953 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB16AY.html
+-rw-r--r--   0 ben       (1000) users      (100)    20947 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB16BD.html
+-rw-r--r--   0 ben       (1000) users      (100)    20320 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB16CD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7885 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB16CY.html
+-rw-r--r--   0 ben       (1000) users      (100)    25246 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG02AD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9176 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG02CV.html
+-rw-r--r--   0 ben       (1000) users      (100)    20509 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG02CW.html
+-rw-r--r--   0 ben       (1000) users      (100)    11453 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG02CX.html
+-rw-r--r--   0 ben       (1000) users      (100)    26693 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG02ND.html
+-rw-r--r--   0 ben       (1000) users      (100)    18998 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03AD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4900 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03AX.html
+-rw-r--r--   0 ben       (1000) users      (100)     4904 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03AY.html
+-rw-r--r--   0 ben       (1000) users      (100)    21145 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BD.html
+-rw-r--r--   0 ben       (1000) users      (100)     2202 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BR.html
+-rw-r--r--   0 ben       (1000) users      (100)     8774 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BS.html
+-rw-r--r--   0 ben       (1000) users      (100)     8144 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BT.html
+-rw-r--r--   0 ben       (1000) users      (100)     9513 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BU.html
+-rw-r--r--   0 ben       (1000) users      (100)     8957 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BV.html
+-rw-r--r--   0 ben       (1000) users      (100)     5993 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BW.html
+-rw-r--r--   0 ben       (1000) users      (100)     6413 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BX.html
+-rw-r--r--   0 ben       (1000) users      (100)     2137 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BY.html
+-rw-r--r--   0 ben       (1000) users      (100)    17385 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    10967 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01ID.html
+-rw-r--r--   0 ben       (1000) users      (100)    12670 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01IZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    13785 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01KD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6012 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01KX.html
+-rw-r--r--   0 ben       (1000) users      (100)    13179 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01LD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10518 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10322 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01ND.html
+-rw-r--r--   0 ben       (1000) users      (100)    11881 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01PD.html
+-rw-r--r--   0 ben       (1000) users      (100)    14488 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01PX.html
+-rw-r--r--   0 ben       (1000) users      (100)    11397 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01TD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15344 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01UD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8516 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01UX.html
+-rw-r--r--   0 ben       (1000) users      (100)    15763 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01UY.html
+-rw-r--r--   0 ben       (1000) users      (100)     7267 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01VD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5246 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01VY.html
+-rw-r--r--   0 ben       (1000) users      (100)    10570 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01WD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10223 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01WX.html
+-rw-r--r--   0 ben       (1000) users      (100)     5255 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01XD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5226 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01XZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     3679 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01YD.html
+-rw-r--r--   0 ben       (1000) users      (100)    12176 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01ZD.html
+-rw-r--r--   0 ben       (1000) users      (100)    19113 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB03AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    17777 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15787 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04BD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6117 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04BV.html
+-rw-r--r--   0 ben       (1000) users      (100)     5382 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04BW.html
+-rw-r--r--   0 ben       (1000) users      (100)     5139 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04BX.html
+-rw-r--r--   0 ben       (1000) users      (100)    16621 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04CD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13598 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB05AD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8563 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TC01OD.html
+-rw-r--r--   0 ben       (1000) users      (100)    14230 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TC04AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    11526 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TC05AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    22198 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TD03AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    15544 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TD04AD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6497 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TD05AD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9014 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     4857 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01MX.html
+-rw-r--r--   0 ben       (1000) users      (100)     5910 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01MY.html
+-rw-r--r--   0 ben       (1000) users      (100)     9858 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     6824 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6918 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01PD.html
+-rw-r--r--   0 ben       (1000) users      (100)     9938 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01QD.html
+-rw-r--r--   0 ben       (1000) users      (100)     8293 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01RD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13334 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01AD.html
+-rw-r--r--   0 ben       (1000) users      (100)    14133 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01AZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     9575 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01BD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10163 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01CD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10070 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01DD.html
+-rw-r--r--   0 ben       (1000) users      (100)    14972 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01ED.html
+-rw-r--r--   0 ben       (1000) users      (100)    17454 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01FD.html
+-rw-r--r--   0 ben       (1000) users      (100)    18546 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01FZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    14896 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01GD.html
+-rw-r--r--   0 ben       (1000) users      (100)    23717 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01HD.html
+-rw-r--r--   0 ben       (1000) users      (100)    13936 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01HU.html
+-rw-r--r--   0 ben       (1000) users      (100)    12488 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01HX.html
+-rw-r--r--   0 ben       (1000) users      (100)    13501 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01HY.html
+-rw-r--r--   0 ben       (1000) users      (100)    24383 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01ID.html
+-rw-r--r--   0 ben       (1000) users      (100)    19140 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01JD.html
+-rw-r--r--   0 ben       (1000) users      (100)    22568 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01JY.html
+-rw-r--r--   0 ben       (1000) users      (100)     7330 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01KD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7299 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01KZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    18445 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01LD.html
+-rw-r--r--   0 ben       (1000) users      (100)    10696 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01LY.html
+-rw-r--r--   0 ben       (1000) users      (100)    18837 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)    20675 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     7633 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01NX.html
+-rw-r--r--   0 ben       (1000) users      (100)     4151 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01OA.html
+-rw-r--r--   0 ben       (1000) users      (100)     4170 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01OB.html
+-rw-r--r--   0 ben       (1000) users      (100)     5550 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01OD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5569 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01OZ.html
+-rw-r--r--   0 ben       (1000) users      (100)    20042 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01PD.html
+-rw-r--r--   0 ben       (1000) users      (100)    20693 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01QD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6679 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01WD.html
+-rw-r--r--   0 ben       (1000) users      (100)     6292 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01BD.html
+-rw-r--r--   0 ben       (1000) users      (100)     7121 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01CD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5050 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01DD.html
+-rw-r--r--   0 ben       (1000) users      (100)     5123 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)     3291 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01MZ.html
+-rw-r--r--   0 ben       (1000) users      (100)     7217 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01ND.html
+-rw-r--r--   0 ben       (1000) users      (100)     3046 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UE01MD.html
+-rw-r--r--   0 ben       (1000) users      (100)      978 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/readme
+-rw-r--r--   0 ben       (1000) users      (100)    42799 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/doc/support.html
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.782593 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/
+-rw-r--r--   0 ben       (1000) users      (100)      124 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB01MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      464 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB01MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      149 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB01ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      575 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB01ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      321 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB01OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      539 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB01OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      168 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB04MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      332 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB04MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      376 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      839 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      370 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      842 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      376 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      986 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      380 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05PD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      842 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05PD.res
+-rw-r--r--   0 ben       (1000) users      (100)      382 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05QD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1170 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05QD.res
+-rw-r--r--   0 ben       (1000) users      (100)      356 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05RD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      567 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05RD.res
+-rw-r--r--   0 ben       (1000) users      (100)      179 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB07MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      368 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB07MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      200 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB07ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      475 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB07ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      510 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB08ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      877 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB08ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      510 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB08NW.dat
+-rw-r--r--   0 ben       (1000) users      (100)      913 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB08NW.res
+-rw-r--r--   0 ben       (1000) users      (100)      868 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB08NZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)      923 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB08NZ.res
+-rw-r--r--   0 ben       (1000) users      (100)      820 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      754 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      888 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      848 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09BD.res
+-rw-r--r--   0 ben       (1000) users      (100)      876 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09CD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      848 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09CD.res
+-rw-r--r--   0 ben       (1000) users      (100)      927 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09DD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      775 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09DD.res
+-rw-r--r--   0 ben       (1000) users      (100)      865 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09ED.dat
+-rw-r--r--   0 ben       (1000) users      (100)      851 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09ED.res
+-rw-r--r--   0 ben       (1000) users      (100)      815 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09FD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      769 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09FD.res
+-rw-r--r--   0 ben       (1000) users      (100)      882 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09GD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      867 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09GD.res
+-rw-r--r--   0 ben       (1000) users      (100)      882 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09HD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      880 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09HD.res
+-rw-r--r--   0 ben       (1000) users      (100)      736 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09ID.dat
+-rw-r--r--   0 ben       (1000) users      (100)      401 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09ID.res
+-rw-r--r--   0 ben       (1000) users      (100)      716 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09JD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      585 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09JD.res
+-rw-r--r--   0 ben       (1000) users      (100)      713 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09KD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      585 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09KD.res
+-rw-r--r--   0 ben       (1000) users      (100)      807 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      753 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      875 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      851 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      787 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      208 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      855 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)       77 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13BD.res
+-rw-r--r--   0 ben       (1000) users      (100)      394 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13CD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      131 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13CD.res
+-rw-r--r--   0 ben       (1000) users      (100)      436 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13DD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      131 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13DD.res
+-rw-r--r--   0 ben       (1000) users      (100)      257 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13ED.dat
+-rw-r--r--   0 ben       (1000) users      (100)      611 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13ED.res
+-rw-r--r--   0 ben       (1000) users      (100)      282 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13FD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      471 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13FD.res
+-rw-r--r--   0 ben       (1000) users      (100)     1302 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13ID.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1435 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13ID.res
+-rw-r--r--   0 ben       (1000) users      (100)      700 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)       99 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13MD.res
+-rw-r--r--   0 ben       (1000) users      (100)     1450 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AG08BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1701 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AG08BD.res
+-rw-r--r--   0 ben       (1000) users      (100)     1942 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AG08BZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1736 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AG08BZ.res
+-rw-r--r--   0 ben       (1000) users      (100)       72 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BB01AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      517 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BB01AD.res
+-rw-r--r--   0 ben       (1000) users      (100)       74 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BB02AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      499 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BB02AD.res
+-rw-r--r--   0 ben       (1000) users      (100)       52 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BB03AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      998 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BB03AD.res
+-rw-r--r--   0 ben       (1000) users      (100)       52 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BB04AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      998 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BB04AD.res
+-rw-r--r--   0 ben       (1000) users      (100)       34 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BD01AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      396 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BD01AD.res
+-rw-r--r--   0 ben       (1000) users      (100)       34 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BD02AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      377 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BD02AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      192 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DE01OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      176 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DE01OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      198 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DE01PD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      176 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DE01PD.res
+-rw-r--r--   0 ben       (1000) users      (100)      218 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DF01MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      358 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DF01MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      192 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DG01MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      315 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DG01MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      200 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DG01ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      342 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DG01ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      115 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DG01OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      294 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DG01OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      120 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DK01MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      220 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/DK01MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      550 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01QD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      338 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01QD.res
+-rw-r--r--   0 ben       (1000) users      (100)      550 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01RD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      338 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01RD.res
+-rw-r--r--   0 ben       (1000) users      (100)      636 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01SD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      384 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01SD.res
+-rw-r--r--   0 ben       (1000) users      (100)      630 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01TD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      384 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01TD.res
+-rw-r--r--   0 ben       (1000) users      (100)      612 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01VD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      430 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01VD.res
+-rw-r--r--   0 ben       (1000) users      (100)       50 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FD01AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      223 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FD01AD.res
+-rw-r--r--   0 ben       (1000) users      (100)    20108 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB01AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      230 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB01AD.res
+-rw-r--r--   0 ben       (1000) users      (100)    20119 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB01BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      796 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB01BD.res
+-rw-r--r--   0 ben       (1000) users      (100)    20125 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB01CD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      475 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB01CD.res
+-rw-r--r--   0 ben       (1000) users      (100)    34954 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB03AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      780 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB03AD.res
+-rw-r--r--   0 ben       (1000) users      (100)    34946 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB03BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      812 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB03BD.res
+-rw-r--r--   0 ben       (1000) users      (100)      334 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB01TD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      291 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB01TD.res
+-rw-r--r--   0 ben       (1000) users      (100)      161 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02CD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1076 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02CD.res
+-rw-r--r--   0 ben       (1000) users      (100)      262 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02DD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     3296 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02DD.res
+-rw-r--r--   0 ben       (1000) users      (100)      516 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02ED.dat
+-rw-r--r--   0 ben       (1000) users      (100)      233 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02ED.res
+-rw-r--r--   0 ben       (1000) users      (100)      185 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02FD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      509 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02FD.res
+-rw-r--r--   0 ben       (1000) users      (100)      165 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02GD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      452 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02GD.res
+-rw-r--r--   0 ben       (1000) users      (100)      196 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02HD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      812 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02HD.res
+-rw-r--r--   0 ben       (1000) users      (100)      522 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02ID.dat
+-rw-r--r--   0 ben       (1000) users      (100)      304 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02ID.res
+-rw-r--r--   0 ben       (1000) users      (100)      351 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02JD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1312 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02JD.res
+-rw-r--r--   0 ben       (1000) users      (100)      657 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02JX.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1728 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02JX.res
+-rw-r--r--   0 ben       (1000) users      (100)      551 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02KD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      180 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02KD.res
+-rw-r--r--   0 ben       (1000) users      (100)      287 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      227 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      307 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      776 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      190 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02QD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      220 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02QD.res
+-rw-r--r--   0 ben       (1000) users      (100)      323 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02SD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      288 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02SD.res
+-rw-r--r--   0 ben       (1000) users      (100)      262 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02VD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      243 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02VD.res
+-rw-r--r--   0 ben       (1000) users      (100)      250 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      889 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03BD.res
+-rw-r--r--   0 ben       (1000) users      (100)      925 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03BZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     2500 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03BZ.res
+-rw-r--r--   0 ben       (1000) users      (100)      515 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03FZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     2448 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03FZ.res
+-rw-r--r--   0 ben       (1000) users      (100)      254 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03KD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      880 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03KD.res
+-rw-r--r--   0 ben       (1000) users      (100)      709 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03LD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1177 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03LD.res
+-rw-r--r--   0 ben       (1000) users      (100)     1018 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03LF.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1516 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03LF.res
+-rw-r--r--   0 ben       (1000) users      (100)      410 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03LZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     2008 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03LZ.res
+-rw-r--r--   0 ben       (1000) users      (100)      114 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      298 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      107 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      259 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      242 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      153 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      242 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03PD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      155 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03PD.res
+-rw-r--r--   0 ben       (1000) users      (100)      176 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03QD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      511 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03QD.res
+-rw-r--r--   0 ben       (1000) users      (100)      283 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03QG.dat
+-rw-r--r--   0 ben       (1000) users      (100)      943 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03QG.res
+-rw-r--r--   0 ben       (1000) users      (100)      478 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03RD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1458 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03RD.res
+-rw-r--r--   0 ben       (1000) users      (100)      143 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03SD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      200 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03SD.res
+-rw-r--r--   0 ben       (1000) users      (100)      897 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03TD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1689 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03TD.res
+-rw-r--r--   0 ben       (1000) users      (100)      147 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03UD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      556 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03UD.res
+-rw-r--r--   0 ben       (1000) users      (100)      168 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03VD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      691 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03VD.res
+-rw-r--r--   0 ben       (1000) users      (100)      176 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03WD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      895 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03WD.res
+-rw-r--r--   0 ben       (1000) users      (100)     1424 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     6093 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XD.res
+-rw-r--r--   0 ben       (1000) users      (100)     1350 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XP.dat
+-rw-r--r--   0 ben       (1000) users      (100)     3194 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XP.res
+-rw-r--r--   0 ben       (1000) users      (100)      694 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     8586 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XZ.res
+-rw-r--r--   0 ben       (1000) users      (100)     3578 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03ZD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1515 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03ZD.res
+-rw-r--r--   0 ben       (1000) users      (100)     1333 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     3991 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      515 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04AZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     4121 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04AZ.res
+-rw-r--r--   0 ben       (1000) users      (100)      713 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     2623 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04BD.res
+-rw-r--r--   0 ben       (1000) users      (100)      405 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04BZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     3043 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04BZ.res
+-rw-r--r--   0 ben       (1000) users      (100)      837 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1166 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DD.res
+-rw-r--r--   0 ben       (1000) users      (100)      382 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DL.dat
+-rw-r--r--   0 ben       (1000) users      (100)      944 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DL.res
+-rw-r--r--   0 ben       (1000) users      (100)      262 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DP.dat
+-rw-r--r--   0 ben       (1000) users      (100)      780 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DP.res
+-rw-r--r--   0 ben       (1000) users      (100)      837 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DS.dat
+-rw-r--r--   0 ben       (1000) users      (100)      932 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DS.res
+-rw-r--r--   0 ben       (1000) users      (100)      187 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DY.dat
+-rw-r--r--   0 ben       (1000) users      (100)      493 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DY.res
+-rw-r--r--   0 ben       (1000) users      (100)      867 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1790 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DZ.res
+-rw-r--r--   0 ben       (1000) users      (100)     1047 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04ED.dat
+-rw-r--r--   0 ben       (1000) users      (100)     2192 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04ED.res
+-rw-r--r--   0 ben       (1000) users      (100)      776 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04FD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1600 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04FD.res
+-rw-r--r--   0 ben       (1000) users      (100)      256 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04GD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      380 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04GD.res
+-rw-r--r--   0 ben       (1000) users      (100)      141 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      295 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      202 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      328 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      598 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04PB.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1789 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04PB.res
+-rw-r--r--   0 ben       (1000) users      (100)      598 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04PU.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1789 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04PU.res
+-rw-r--r--   0 ben       (1000) users      (100)     1074 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04TB.dat
+-rw-r--r--   0 ben       (1000) users      (100)     3303 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04TB.res
+-rw-r--r--   0 ben       (1000) users      (100)     1074 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04TS.dat
+-rw-r--r--   0 ben       (1000) users      (100)     3303 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04TS.res
+-rw-r--r--   0 ben       (1000) users      (100)      224 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04UD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      457 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04UD.res
+-rw-r--r--   0 ben       (1000) users      (100)      142 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04VD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      885 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04VD.res
+-rw-r--r--   0 ben       (1000) users      (100)      313 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04XD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1129 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04XD.res
+-rw-r--r--   0 ben       (1000) users      (100)      132 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04YD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      268 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04YD.res
+-rw-r--r--   0 ben       (1000) users      (100)      117 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04ZD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      865 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04ZD.res
+-rw-r--r--   0 ben       (1000) users      (100)      142 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB05MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      715 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB05MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      208 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB05ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      554 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB05ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      105 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB05OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      320 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB05OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      382 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB4DLZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1251 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB4DLZ.res
+-rw-r--r--   0 ben       (1000) users      (100)      261 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB4DPZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)      971 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB4DPZ.res
+-rw-r--r--   0 ben       (1000) users      (100)       80 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      349 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01MD.res
+-rw-r--r--   0 ben       (1000) users      (100)       81 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      132 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01ND.res
+-rw-r--r--   0 ben       (1000) users      (100)       99 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      355 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01OD.res
+-rw-r--r--   0 ben       (1000) users      (100)       99 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01PD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      265 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01PD.res
+-rw-r--r--   0 ben       (1000) users      (100)       85 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01QD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      287 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01QD.res
+-rw-r--r--   0 ben       (1000) users      (100)      101 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01RD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      245 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01RD.res
+-rw-r--r--   0 ben       (1000) users      (100)       78 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01SD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      382 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01SD.res
+-rw-r--r--   0 ben       (1000) users      (100)       68 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01TD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      126 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01TD.res
+-rw-r--r--   0 ben       (1000) users      (100)       47 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01VD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      128 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01VD.res
+-rw-r--r--   0 ben       (1000) users      (100)       92 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01WD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      387 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01WD.res
+-rw-r--r--   0 ben       (1000) users      (100)      109 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01XD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      316 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC01XD.res
+-rw-r--r--   0 ben       (1000) users      (100)      310 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC03MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      458 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC03MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      429 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC03ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      608 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC03ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      104 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MD03AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      211 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MD03AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      137 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MD03BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      243 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MD03BD.res
+-rw-r--r--   0 ben       (1000) users      (100)      367 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB01BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      461 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB01BD.res
+-rw-r--r--   0 ben       (1000) users      (100)      274 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB01DD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      139 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB01DD.res
+-rw-r--r--   0 ben       (1000) users      (100)      202 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB01MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      118 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB01MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      142 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      113 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      173 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      153 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      185 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)       98 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      131 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02PD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      196 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02PD.res
+-rw-r--r--   0 ben       (1000) users      (100)      142 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02QD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      217 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02QD.res
+-rw-r--r--   0 ben       (1000) users      (100)      166 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02RD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      218 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02RD.res
+-rw-r--r--   0 ben       (1000) users      (100)      136 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02SD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      217 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB02SD.res
+-rw-r--r--   0 ben       (1000) users      (100)      172 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      172 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      286 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      390 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      178 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03QD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      291 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03QD.res
+-rw-r--r--   0 ben       (1000) users      (100)      178 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03SD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      291 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03SD.res
+-rw-r--r--   0 ben       (1000) users      (100)      178 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03TD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      291 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03TD.res
+-rw-r--r--   0 ben       (1000) users      (100)      178 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03UD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      291 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB03UD.res
+-rw-r--r--   0 ben       (1000) users      (100)      162 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      185 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      373 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      200 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      340 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      621 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      198 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04PD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      327 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04PD.res
+-rw-r--r--   0 ben       (1000) users      (100)      235 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04QD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      258 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04QD.res
+-rw-r--r--   0 ben       (1000) users      (100)      531 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04RD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      290 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04RD.res
+-rw-r--r--   0 ben       (1000) users      (100)      315 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB06ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      161 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB06ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      853 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08CD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1452 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08CD.res
+-rw-r--r--   0 ben       (1000) users      (100)      853 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08DD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1369 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08DD.res
+-rw-r--r--   0 ben       (1000) users      (100)      858 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08ED.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1452 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08ED.res
+-rw-r--r--   0 ben       (1000) users      (100)      858 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08FD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1369 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08FD.res
+-rw-r--r--   0 ben       (1000) users      (100)       64 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      417 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08MD.res
+-rw-r--r--   0 ben       (1000) users      (100)       57 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      365 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      190 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB09MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      264 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB09MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      729 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10DD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      913 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10DD.res
+-rw-r--r--   0 ben       (1000) users      (100)      721 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10ED.dat
+-rw-r--r--   0 ben       (1000) users      (100)      899 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10ED.res
+-rw-r--r--   0 ben       (1000) users      (100)      726 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10FD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1290 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10FD.res
+-rw-r--r--   0 ben       (1000) users      (100)      721 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10HD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      987 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10HD.res
+-rw-r--r--   0 ben       (1000) users      (100)      452 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10ID.dat
+-rw-r--r--   0 ben       (1000) users      (100)      816 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10ID.res
+-rw-r--r--   0 ben       (1000) users      (100)      389 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10KD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      860 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10KD.res
+-rw-r--r--   0 ben       (1000) users      (100)      462 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10ZD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      959 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10ZD.res
+-rw-r--r--   0 ben       (1000) users      (100)      349 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB16AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      450 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB16AD.res
+-rw-r--r--   0 ben       (1000) users      (100)     1097 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB16BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      641 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB16BD.res
+-rw-r--r--   0 ben       (1000) users      (100)     1289 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB16CD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      431 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB16CD.res
+-rw-r--r--   0 ben       (1000) users      (100)      221 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SG02AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)       98 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SG02AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      197 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SG02ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      153 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SG02ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      272 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SG03AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      199 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SG03AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      209 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SG03BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      185 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SG03BD.res
+-rw-r--r--   0 ben       (1000) users      (100)     2609 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3661 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     2876 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3191 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB04MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5048 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4743 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     5039 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4542 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5440 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5738 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05RD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3310 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB07MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2918 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB07ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     8781 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB08ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     9589 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB08NW.f
+-rw-r--r--   0 ben       (1000) users      (100)     8818 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB08NZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     3481 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3936 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4168 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3430 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4356 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09ED.f
+-rw-r--r--   0 ben       (1000) users      (100)     3655 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09FD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4046 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09GD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4278 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09HD.f
+-rw-r--r--   0 ben       (1000) users      (100)     9369 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09ID.f
+-rw-r--r--   0 ben       (1000) users      (100)     8111 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09JD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7213 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09KD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3557 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4017 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     2702 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3017 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3095 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3885 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1660 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13ED.f
+-rw-r--r--   0 ben       (1000) users      (100)     1809 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13FD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4964 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13ID.f
+-rw-r--r--   0 ben       (1000) users      (100)     2381 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17103 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAG08BD.f
+-rw-r--r--   0 ben       (1000) users      (100)    16231 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAG08BZ.f
+-rw-r--r--   0 ben       (1000) users      (100)      856 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01ID.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1520 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01ID.res
+-rw-r--r--   0 ben       (1000) users      (100)     1202 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01IZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     2874 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01IZ.res
+-rw-r--r--   0 ben       (1000) users      (100)      545 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01KD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1147 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01KD.res
+-rw-r--r--   0 ben       (1000) users      (100)      545 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01LD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1140 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01LD.res
+-rw-r--r--   0 ben       (1000) users      (100)      388 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      611 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      300 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      482 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      180 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01PD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      448 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01PD.res
+-rw-r--r--   0 ben       (1000) users      (100)      180 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01PX.dat
+-rw-r--r--   0 ben       (1000) users      (100)      513 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01PX.res
+-rw-r--r--   0 ben       (1000) users      (100)      350 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01TD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      728 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01TD.res
+-rw-r--r--   0 ben       (1000) users      (100)      193 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01UD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      687 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01UD.res
+-rw-r--r--   0 ben       (1000) users      (100)      199 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01UY.dat
+-rw-r--r--   0 ben       (1000) users      (100)      690 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01UY.res
+-rw-r--r--   0 ben       (1000) users      (100)      518 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01WD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1078 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01WD.res
+-rw-r--r--   0 ben       (1000) users      (100)      524 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01WX.dat
+-rw-r--r--   0 ben       (1000) users      (100)      914 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01WX.res
+-rw-r--r--   0 ben       (1000) users      (100)      168 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01ZD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      582 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01ZD.res
+-rw-r--r--   0 ben       (1000) users      (100)      193 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB03AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      805 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB03AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      227 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB04AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1308 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB04AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      232 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB04BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      667 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB04BD.res
+-rw-r--r--   0 ben       (1000) users      (100)      226 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB04CD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      972 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB04CD.res
+-rw-r--r--   0 ben       (1000) users      (100)      186 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB05AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      298 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB05AD.res
+-rw-r--r--   0 ben       (1000) users      (100)     6131 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBB01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6421 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBB02AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3572 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBB03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3572 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBB04AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3189 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBD01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3184 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBD02AD.f
+-rw-r--r--   0 ben       (1000) users      (100)      204 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TC01OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      513 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TC01OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      209 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TC04AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      582 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TC04AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      223 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TC05AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      153 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TC05AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      227 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TD03AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      954 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TD03AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      215 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TD04AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      673 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TD04AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      122 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TD05AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)       79 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TD05AD.res
+-rw-r--r--   0 ben       (1000) users      (100)     1626 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDE01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1656 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDE01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1865 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDF01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1453 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDG01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1796 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDG01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     1370 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDG01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1396 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDK01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)      467 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      443 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      473 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      443 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      222 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01OD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      390 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01OD.res
+-rw-r--r--   0 ben       (1000) users      (100)      222 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01PD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      390 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01PD.res
+-rw-r--r--   0 ben       (1000) users      (100)      203 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01QD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      515 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01QD.res
+-rw-r--r--   0 ben       (1000) users      (100)      213 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01RD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      350 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01RD.res
+-rw-r--r--   0 ben       (1000) users      (100)     4289 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFB01QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4324 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFB01RD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4826 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFB01SD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4921 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFB01TD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3470 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFB01VD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4073 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFD01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)      529 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01AD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1058 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01AD.res
+-rw-r--r--   0 ben       (1000) users      (100)      656 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01AZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1586 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01AZ.res
+-rw-r--r--   0 ben       (1000) users      (100)      306 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01CD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      732 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01CD.res
+-rw-r--r--   0 ben       (1000) users      (100)      304 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01DD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      728 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01DD.res
+-rw-r--r--   0 ben       (1000) users      (100)      363 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01ED.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1098 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01ED.res
+-rw-r--r--   0 ben       (1000) users      (100)      363 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01FD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1098 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01FD.res
+-rw-r--r--   0 ben       (1000) users      (100)      555 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01FZ.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1898 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01FZ.res
+-rw-r--r--   0 ben       (1000) users      (100)      395 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01GD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      571 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01GD.res
+-rw-r--r--   0 ben       (1000) users      (100)      878 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01HD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     2565 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01HD.res
+-rw-r--r--   0 ben       (1000) users      (100)      879 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01ID.dat
+-rw-r--r--   0 ben       (1000) users      (100)     2565 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01ID.res
+-rw-r--r--   0 ben       (1000) users      (100)     1280 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01JD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1589 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01JD.res
+-rw-r--r--   0 ben       (1000) users      (100)     1299 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01JY.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1511 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01JY.res
+-rw-r--r--   0 ben       (1000) users      (100)      370 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01LD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1146 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01LD.res
+-rw-r--r--   0 ben       (1000) users      (100)      364 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1298 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      370 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1295 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01ND.res
+-rw-r--r--   0 ben       (1000) users      (100)      411 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01PD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1202 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01PD.res
+-rw-r--r--   0 ben       (1000) users      (100)      387 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01QD.dat
+-rw-r--r--   0 ben       (1000) users      (100)     1305 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01QD.res
+-rw-r--r--   0 ben       (1000) users      (100)     4674 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TIB01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10136 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TIB01BD.f
+-rw-r--r--   0 ben       (1000) users      (100)    11013 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TIB01CD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10254 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TIB03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10794 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TIB03BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1597 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB01TD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3338 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6602 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3281 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02ED.f
+-rw-r--r--   0 ben       (1000) users      (100)     5862 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02FD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2407 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02GD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3214 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02HD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3747 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02ID.f
+-rw-r--r--   0 ben       (1000) users      (100)     3046 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02JD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3356 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02JX.f
+-rw-r--r--   0 ben       (1000) users      (100)     3726 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02KD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3670 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5206 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     3052 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2859 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02SD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1803 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02VD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4924 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3602 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03BZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     5398 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03FZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     7940 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03KD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4137 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03LD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4454 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03LF.f
+-rw-r--r--   0 ben       (1000) users      (100)     4535 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03LZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     2879 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2271 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     2331 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2313 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2575 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3318 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03QG.f
+-rw-r--r--   0 ben       (1000) users      (100)     2702 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03RD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2048 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03SD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3589 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03TD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2335 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03UD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4783 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03VD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6571 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03WD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8081 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03XD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4731 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03XP.f
+-rw-r--r--   0 ben       (1000) users      (100)     9814 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03XZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     6151 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03ZD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5410 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4897 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04AZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     5120 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4121 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04BZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     2309 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3255 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DL.f
+-rw-r--r--   0 ben       (1000) users      (100)     3860 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DP.f
+-rw-r--r--   0 ben       (1000) users      (100)     2310 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DS.f
+-rw-r--r--   0 ben       (1000) users      (100)     2620 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DY.f
+-rw-r--r--   0 ben       (1000) users      (100)     2322 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     4204 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04ED.f
+-rw-r--r--   0 ben       (1000) users      (100)     3923 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04FD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2546 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04GD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1553 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3012 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6984 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04PB.f
+-rw-r--r--   0 ben       (1000) users      (100)     6928 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04PU.f
+-rw-r--r--   0 ben       (1000) users      (100)    11087 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04TB.f
+-rw-r--r--   0 ben       (1000) users      (100)    10989 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04TS.f
+-rw-r--r--   0 ben       (1000) users      (100)     2615 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04UD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5407 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04VD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5537 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04XD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4693 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04YD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4008 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04ZD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2442 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB05MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1965 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB05ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     2221 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB05OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3307 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB4DLZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     3908 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB4DPZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     1519 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1429 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     1513 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1415 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2703 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2548 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01RD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1846 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01SD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2305 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01TD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1092 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01VD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1764 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01WD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2019 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01XD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4003 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC03MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3529 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC03ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     6760 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMD03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8675 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMD03BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4493 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB01BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3045 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB01DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2184 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2265 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4500 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     4522 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2725 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5322 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3755 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02RD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5709 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02SD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2570 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3826 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4112 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4113 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03SD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3841 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03TD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3891 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03UD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2489 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2351 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     4682 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3439 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2489 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2351 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04RD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3234 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB06ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     4673 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4643 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4722 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08ED.f
+-rw-r--r--   0 ben       (1000) users      (100)     4636 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08FD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2150 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2148 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     2589 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB09MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4764 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4416 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10ED.f
+-rw-r--r--   0 ben       (1000) users      (100)     6195 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10FD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4211 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10HD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3852 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10ID.f
+-rw-r--r--   0 ben       (1000) users      (100)     3888 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10KD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3936 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10ZD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5626 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB16AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4575 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB16BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4157 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB16CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4795 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSG02AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4896 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSG02ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     3023 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSG03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2804 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSG03BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2609 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01ID.f
+-rw-r--r--   0 ben       (1000) users      (100)     2616 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01IZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     3640 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01KD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3635 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01LD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2768 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2765 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     3327 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3756 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01PX.f
+-rw-r--r--   0 ben       (1000) users      (100)     3207 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01TD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4374 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01UD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4427 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01UY.f
+-rw-r--r--   0 ben       (1000) users      (100)     3329 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01WD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3138 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01WX.f
+-rw-r--r--   0 ben       (1000) users      (100)     3331 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01ZD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6546 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6189 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB04AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4337 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB04BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4345 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB04CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3851 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB05AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3124 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTC01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4364 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTC04AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3568 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTC05AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6815 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTD03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5053 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTD04AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2058 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTD05AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2997 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3068 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     2198 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2200 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3009 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2805 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01RD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5099 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5140 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01AZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     3202 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3195 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4578 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01ED.f
+-rw-r--r--   0 ben       (1000) users      (100)     4585 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01FD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4724 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01FZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     4252 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01GD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4497 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01HD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4589 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01ID.f
+-rw-r--r--   0 ben       (1000) users      (100)     3901 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01JD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4176 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01JY.f
+-rw-r--r--   0 ben       (1000) users      (100)     4555 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01LD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4870 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4884 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     5235 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5440 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1943 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TUD01BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1965 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TUD01CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1545 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TUD01DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1332 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TUD01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1962 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TUD01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)      375 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01BD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      856 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01BD.res
+-rw-r--r--   0 ben       (1000) users      (100)      114 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01CD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      856 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01CD.res
+-rw-r--r--   0 ben       (1000) users      (100)      163 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01DD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      615 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01DD.res
+-rw-r--r--   0 ben       (1000) users      (100)      161 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01MD.dat
+-rw-r--r--   0 ben       (1000) users      (100)      377 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01MD.res
+-rw-r--r--   0 ben       (1000) users      (100)      388 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01ND.dat
+-rw-r--r--   0 ben       (1000) users      (100)      853 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01ND.res
+-rw-r--r--   0 ben       (1000) users      (100)    57438 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/makefile
+-rw-r--r--   0 ben       (1000) users      (100)    55379 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/makefile_Unix
+-rw-r--r--   0 ben       (1000) users      (100)     1108 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/examples/readme
+-rw-r--r--   0 ben       (1000) users      (100)    38876 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/libindex.html
+-rw-r--r--   0 ben       (1000) users      (100)     1631 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/make.inc
+-rw-r--r--   0 ben       (1000) users      (100)     1367 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/make_Unix.inc
+-rw-r--r--   0 ben       (1000) users      (100)     1886 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/makefile
+-rw-r--r--   0 ben       (1000) users      (100)     1834 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/makefile_Unix
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:48.050601 slycot-0.5.4/slycot/src/SLICOT-Reference/src/
+-rw-r--r--   0 ben       (1000) users      (100)    13388 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    16256 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    19924 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10651 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB04MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17577 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    18119 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    12969 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05OD.f
+-rw-r--r--   0 ben       (1000) users      (100)    11939 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05PD.f
+-rw-r--r--   0 ben       (1000) users      (100)    13523 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05QD.f
+-rw-r--r--   0 ben       (1000) users      (100)    13196 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05RD.f
+-rw-r--r--   0 ben       (1000) users      (100)    11707 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05SD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6122 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB07MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     9978 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB07ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     9436 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     9597 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08MZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    18491 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    19794 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08NW.f
+-rw-r--r--   0 ben       (1000) users      (100)    15224 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08NX.f
+-rw-r--r--   0 ben       (1000) users      (100)    19969 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08NY.f
+-rw-r--r--   0 ben       (1000) users      (100)    18880 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08NZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    12486 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19246 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09AX.f
+-rw-r--r--   0 ben       (1000) users      (100)    13362 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09BD.f
+-rw-r--r--   0 ben       (1000) users      (100)    22818 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09BX.f
+-rw-r--r--   0 ben       (1000) users      (100)    13288 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09CD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19074 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09CX.f
+-rw-r--r--   0 ben       (1000) users      (100)     8214 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09DD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17903 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09ED.f
+-rw-r--r--   0 ben       (1000) users      (100)    24413 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09FD.f
+-rw-r--r--   0 ben       (1000) users      (100)    25869 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09GD.f
+-rw-r--r--   0 ben       (1000) users      (100)    25636 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09HD.f
+-rw-r--r--   0 ben       (1000) users      (100)    24665 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09HX.f
+-rw-r--r--   0 ben       (1000) users      (100)    12631 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09HY.f
+-rw-r--r--   0 ben       (1000) users      (100)    43280 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09ID.f
+-rw-r--r--   0 ben       (1000) users      (100)    24534 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09IX.f
+-rw-r--r--   0 ben       (1000) users      (100)    31554 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09IY.f
+-rw-r--r--   0 ben       (1000) users      (100)    58312 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09JD.f
+-rw-r--r--   0 ben       (1000) users      (100)    35740 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09JV.f
+-rw-r--r--   0 ben       (1000) users      (100)    36169 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09JW.f
+-rw-r--r--   0 ben       (1000) users      (100)     7640 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09JX.f
+-rw-r--r--   0 ben       (1000) users      (100)    34205 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09KD.f
+-rw-r--r--   0 ben       (1000) users      (100)    31362 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09KX.f
+-rw-r--r--   0 ben       (1000) users      (100)    16581 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17609 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    11668 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     9087 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13AX.f
+-rw-r--r--   0 ben       (1000) users      (100)    13106 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13BD.f
+-rw-r--r--   0 ben       (1000) users      (100)    18030 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13CD.f
+-rw-r--r--   0 ben       (1000) users      (100)    64623 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13DD.f
+-rw-r--r--   0 ben       (1000) users      (100)    18226 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13DX.f
+-rw-r--r--   0 ben       (1000) users      (100)    10636 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13ED.f
+-rw-r--r--   0 ben       (1000) users      (100)    12761 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13FD.f
+-rw-r--r--   0 ben       (1000) users      (100)    33585 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13ID.f
+-rw-r--r--   0 ben       (1000) users      (100)    59291 2022-05-29 11:35:56.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    15752 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB8NXZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     8517 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AG07BD.f
+-rw-r--r--   0 ben       (1000) users      (100)    21364 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AG08BD.f
+-rw-r--r--   0 ben       (1000) users      (100)    22470 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AG08BY.f
+-rw-r--r--   0 ben       (1000) users      (100)    21945 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AG08BZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    23110 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/AG8BYZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    49714 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/BB01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    37531 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/BB02AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17019 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/BB03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    16276 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/BB04AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    34360 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/BD01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19237 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/BD02AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4698 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/DE01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6053 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/DE01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7666 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/DF01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6054 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/DG01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7843 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/DG01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     2011 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/DG01NY.f
+-rw-r--r--   0 ben       (1000) users      (100)     8970 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/DG01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4200 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/DK01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    16908 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/FB01QD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19438 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/FB01RD.f
+-rw-r--r--   0 ben       (1000) users      (100)    22667 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/FB01SD.f
+-rw-r--r--   0 ben       (1000) users      (100)    24240 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/FB01TD.f
+-rw-r--r--   0 ben       (1000) users      (100)    13042 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/FB01VD.f
+-rw-r--r--   0 ben       (1000) users      (100)    12706 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/FD01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    30121 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    31877 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01BD.f
+-rw-r--r--   0 ben       (1000) users      (100)    34315 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01CD.f
+-rw-r--r--   0 ben       (1000) users      (100)    53910 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    41860 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01MY.f
+-rw-r--r--   0 ben       (1000) users      (100)    27606 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     5773 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4591 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01OY.f
+-rw-r--r--   0 ben       (1000) users      (100)    49760 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)    15760 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01PX.f
+-rw-r--r--   0 ben       (1000) users      (100)    29354 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01PY.f
+-rw-r--r--   0 ben       (1000) users      (100)    39165 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01QD.f
+-rw-r--r--   0 ben       (1000) users      (100)    26853 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01RD.f
+-rw-r--r--   0 ben       (1000) users      (100)    44357 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    45297 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB03BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2094 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3459 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA01BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3392 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA01BZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     2829 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA01CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2429 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3403 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02AZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     2871 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2924 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02BZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     2823 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2824 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02CZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     4469 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2270 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02ED.f
+-rw-r--r--   0 ben       (1000) users      (100)     2467 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02ES.f
+-rw-r--r--   0 ben       (1000) users      (100)     5565 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02EZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     2410 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02FD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4175 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02GD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4206 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02GZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     4319 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02HD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4244 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02HZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     9148 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02ID.f
+-rw-r--r--   0 ben       (1000) users      (100)    11211 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02IZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     5035 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02JD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5106 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02JZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     5458 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6061 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02MZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     5882 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02NZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     4177 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4746 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02OZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     2393 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2405 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02PZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    10622 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01KD.f
+-rw-r--r--   0 ben       (1000) users      (100)    14826 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01LD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8084 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7549 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    10606 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OC.f
+-rw-r--r--   0 ben       (1000) users      (100)    13117 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8786 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OE.f
+-rw-r--r--   0 ben       (1000) users      (100)     8790 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OH.f
+-rw-r--r--   0 ben       (1000) users      (100)     5643 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OO.f
+-rw-r--r--   0 ben       (1000) users      (100)     9428 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OS.f
+-rw-r--r--   0 ben       (1000) users      (100)     7743 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OT.f
+-rw-r--r--   0 ben       (1000) users      (100)     8089 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8842 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01QD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17110 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RB.f
+-rw-r--r--   0 ben       (1000) users      (100)    10977 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RD.f
+-rw-r--r--   0 ben       (1000) users      (100)    11083 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RH.f
+-rw-r--r--   0 ben       (1000) users      (100)     8955 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RT.f
+-rw-r--r--   0 ben       (1000) users      (100)     9024 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RU.f
+-rw-r--r--   0 ben       (1000) users      (100)     6974 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RW.f
+-rw-r--r--   0 ben       (1000) users      (100)    10594 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RX.f
+-rw-r--r--   0 ben       (1000) users      (100)    13778 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RY.f
+-rw-r--r--   0 ben       (1000) users      (100)     2910 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01SD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3817 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01SS.f
+-rw-r--r--   0 ben       (1000) users      (100)     4379 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01TD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6907 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01UD.f
+-rw-r--r--   0 ben       (1000) users      (100)    11842 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01UW.f
+-rw-r--r--   0 ben       (1000) users      (100)    11999 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01UX.f
+-rw-r--r--   0 ben       (1000) users      (100)    14764 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01UY.f
+-rw-r--r--   0 ben       (1000) users      (100)    17828 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01UZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    46653 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01VD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10509 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01WD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5901 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01XD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4971 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01XY.f
+-rw-r--r--   0 ben       (1000) users      (100)    10183 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01YD.f
+-rw-r--r--   0 ben       (1000) users      (100)    14210 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01ZD.f
+-rw-r--r--   0 ben       (1000) users      (100)    21939 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02CD.f
+-rw-r--r--   0 ben       (1000) users      (100)    36346 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02CU.f
+-rw-r--r--   0 ben       (1000) users      (100)    27075 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02CV.f
+-rw-r--r--   0 ben       (1000) users      (100)    10027 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02CX.f
+-rw-r--r--   0 ben       (1000) users      (100)    11454 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02CY.f
+-rw-r--r--   0 ben       (1000) users      (100)    21105 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02DD.f
+-rw-r--r--   0 ben       (1000) users      (100)    15867 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02ED.f
+-rw-r--r--   0 ben       (1000) users      (100)    12794 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02FD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19214 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02GD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19161 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02HD.f
+-rw-r--r--   0 ben       (1000) users      (100)    20760 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02ID.f
+-rw-r--r--   0 ben       (1000) users      (100)    20166 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02JD.f
+-rw-r--r--   0 ben       (1000) users      (100)    24476 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02JX.f
+-rw-r--r--   0 ben       (1000) users      (100)    26986 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02KD.f
+-rw-r--r--   0 ben       (1000) users      (100)    22436 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    33633 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     8480 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02NY.f
+-rw-r--r--   0 ben       (1000) users      (100)     8391 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02OD.f
+-rw-r--r--   0 ben       (1000) users      (100)    21111 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02PD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17866 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02QD.f
+-rw-r--r--   0 ben       (1000) users      (100)    11424 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02QY.f
+-rw-r--r--   0 ben       (1000) users      (100)     5068 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02RD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5800 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02RZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     3921 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02SD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4204 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02SZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     6055 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02TD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6506 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02TZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    21891 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02UD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4298 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02UU.f
+-rw-r--r--   0 ben       (1000) users      (100)     5288 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02UV.f
+-rw-r--r--   0 ben       (1000) users      (100)     9764 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02UW.f
+-rw-r--r--   0 ben       (1000) users      (100)     5427 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02VD.f
+-rw-r--r--   0 ben       (1000) users      (100)    14883 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02WD.f
+-rw-r--r--   0 ben       (1000) users      (100)    14038 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02XD.f
+-rw-r--r--   0 ben       (1000) users      (100)    11492 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02YD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8287 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AB.f
+-rw-r--r--   0 ben       (1000) users      (100)     7205 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     9318 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AE.f
+-rw-r--r--   0 ben       (1000) users      (100)    11962 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AF.f
+-rw-r--r--   0 ben       (1000) users      (100)    10070 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AG.f
+-rw-r--r--   0 ben       (1000) users      (100)     9224 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AH.f
+-rw-r--r--   0 ben       (1000) users      (100)     8238 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AI.f
+-rw-r--r--   0 ben       (1000) users      (100)     2521 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BA.f
+-rw-r--r--   0 ben       (1000) users      (100)    13821 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BB.f
+-rw-r--r--   0 ben       (1000) users      (100)    12109 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BC.f
+-rw-r--r--   0 ben       (1000) users      (100)    74389 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4537 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BE.f
+-rw-r--r--   0 ben       (1000) users      (100)     4194 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BF.f
+-rw-r--r--   0 ben       (1000) users      (100)     3982 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BG.f
+-rw-r--r--   0 ben       (1000) users      (100)    41418 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    20675 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4343 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03CZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    23535 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3354 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03DZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    12531 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03ED.f
+-rw-r--r--   0 ben       (1000) users      (100)    10235 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03FD.f
+-rw-r--r--   0 ben       (1000) users      (100)    44919 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03FZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    11486 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03GD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3617 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03GZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     9116 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03HD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2768 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03HZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    62943 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03ID.f
+-rw-r--r--   0 ben       (1000) users      (100)    24855 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03IZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    47137 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03JD.f
+-rw-r--r--   0 ben       (1000) users      (100)    68854 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03JP.f
+-rw-r--r--   0 ben       (1000) users      (100)    18233 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03JZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    23179 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03KA.f
+-rw-r--r--   0 ben       (1000) users      (100)    60190 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03KB.f
+-rw-r--r--   0 ben       (1000) users      (100)     8080 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03KC.f
+-rw-r--r--   0 ben       (1000) users      (100)    18160 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03KD.f
+-rw-r--r--   0 ben       (1000) users      (100)    28149 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03KE.f
+-rw-r--r--   0 ben       (1000) users      (100)    29739 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03LD.f
+-rw-r--r--   0 ben       (1000) users      (100)    36822 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03LF.f
+-rw-r--r--   0 ben       (1000) users      (100)    30052 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03LP.f
+-rw-r--r--   0 ben       (1000) users      (100)    34359 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03LZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    11933 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1887 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03MY.f
+-rw-r--r--   0 ben       (1000) users      (100)     6868 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     5657 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03NY.f
+-rw-r--r--   0 ben       (1000) users      (100)    11339 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03OD.f
+-rw-r--r--   0 ben       (1000) users      (100)    13160 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03OY.f
+-rw-r--r--   0 ben       (1000) users      (100)    11797 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03PD.f
+-rw-r--r--   0 ben       (1000) users      (100)    13361 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03PY.f
+-rw-r--r--   0 ben       (1000) users      (100)    11081 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QD.f
+-rw-r--r--   0 ben       (1000) users      (100)    16223 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QG.f
+-rw-r--r--   0 ben       (1000) users      (100)     3672 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QV.f
+-rw-r--r--   0 ben       (1000) users      (100)     6582 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QW.f
+-rw-r--r--   0 ben       (1000) users      (100)     2780 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QX.f
+-rw-r--r--   0 ben       (1000) users      (100)     4892 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QY.f
+-rw-r--r--   0 ben       (1000) users      (100)    21728 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03RD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7988 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03RW.f
+-rw-r--r--   0 ben       (1000) users      (100)     7566 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03RX.f
+-rw-r--r--   0 ben       (1000) users      (100)     8127 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03RY.f
+-rw-r--r--   0 ben       (1000) users      (100)    20412 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03RZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    11275 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03SD.f
+-rw-r--r--   0 ben       (1000) users      (100)    22798 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03TD.f
+-rw-r--r--   0 ben       (1000) users      (100)    26590 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03TS.f
+-rw-r--r--   0 ben       (1000) users      (100)    11053 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03UD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10269 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03VD.f
+-rw-r--r--   0 ben       (1000) users      (100)    25576 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03VW.f
+-rw-r--r--   0 ben       (1000) users      (100)     7416 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03VY.f
+-rw-r--r--   0 ben       (1000) users      (100)    19411 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03WA.f
+-rw-r--r--   0 ben       (1000) users      (100)    32750 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03WD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4415 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03WX.f
+-rw-r--r--   0 ben       (1000) users      (100)    33154 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03XD.f
+-rw-r--r--   0 ben       (1000) users      (100)    22195 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03XP.f
+-rw-r--r--   0 ben       (1000) users      (100)    16760 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03XS.f
+-rw-r--r--   0 ben       (1000) users      (100)   112885 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03XU.f
+-rw-r--r--   0 ben       (1000) users      (100)    28625 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03XZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     9976 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03YA.f
+-rw-r--r--   0 ben       (1000) users      (100)    17926 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03YD.f
+-rw-r--r--   0 ben       (1000) users      (100)     9465 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03YT.f
+-rw-r--r--   0 ben       (1000) users      (100)    56706 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03ZA.f
+-rw-r--r--   0 ben       (1000) users      (100)    41509 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03ZD.f
+-rw-r--r--   0 ben       (1000) users      (100)    58674 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    38788 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04AZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    49784 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04BD.f
+-rw-r--r--   0 ben       (1000) users      (100)    58499 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04BP.f
+-rw-r--r--   0 ben       (1000) users      (100)    34475 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04BZ.f
+-rw-r--r--   0 ben       (1000) users      (100)   143552 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6281 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DB.f
+-rw-r--r--   0 ben       (1000) users      (100)    14837 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5916 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DI.f
+-rw-r--r--   0 ben       (1000) users      (100)    28402 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DL.f
+-rw-r--r--   0 ben       (1000) users      (100)    43810 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DP.f
+-rw-r--r--   0 ben       (1000) users      (100)    15019 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DS.f
+-rw-r--r--   0 ben       (1000) users      (100)    11159 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DY.f
+-rw-r--r--   0 ben       (1000) users      (100)    15971 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    43773 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04ED.f
+-rw-r--r--   0 ben       (1000) users      (100)    38139 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04FD.f
+-rw-r--r--   0 ben       (1000) users      (100)    43589 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04FP.f
+-rw-r--r--   0 ben       (1000) users      (100)     7408 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04GD.f
+-rw-r--r--   0 ben       (1000) users      (100)   100661 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04HD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8471 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04ID.f
+-rw-r--r--   0 ben       (1000) users      (100)     9918 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04IY.f
+-rw-r--r--   0 ben       (1000) users      (100)     8689 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04IZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     7426 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04JD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6976 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04KD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6964 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04LD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7884 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8320 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    11316 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04NY.f
+-rw-r--r--   0 ben       (1000) users      (100)     8103 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8066 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04OW.f
+-rw-r--r--   0 ben       (1000) users      (100)     2680 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04OX.f
+-rw-r--r--   0 ben       (1000) users      (100)     9773 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04OY.f
+-rw-r--r--   0 ben       (1000) users      (100)    48131 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04PA.f
+-rw-r--r--   0 ben       (1000) users      (100)    11721 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04PB.f
+-rw-r--r--   0 ben       (1000) users      (100)    11802 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04PU.f
+-rw-r--r--   0 ben       (1000) users      (100)    18073 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04PY.f
+-rw-r--r--   0 ben       (1000) users      (100)    16042 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04QB.f
+-rw-r--r--   0 ben       (1000) users      (100)    40151 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04QC.f
+-rw-r--r--   0 ben       (1000) users      (100)    19849 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04QF.f
+-rw-r--r--   0 ben       (1000) users      (100)     9582 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04QS.f
+-rw-r--r--   0 ben       (1000) users      (100)    16626 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04QU.f
+-rw-r--r--   0 ben       (1000) users      (100)    12060 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04RB.f
+-rw-r--r--   0 ben       (1000) users      (100)    10865 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04RU.f
+-rw-r--r--   0 ben       (1000) users      (100)     7730 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04SU.f
+-rw-r--r--   0 ben       (1000) users      (100)    28603 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TB.f
+-rw-r--r--   0 ben       (1000) users      (100)    17849 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TS.f
+-rw-r--r--   0 ben       (1000) users      (100)    13875 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TT.f
+-rw-r--r--   0 ben       (1000) users      (100)     2000 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TU.f
+-rw-r--r--   0 ben       (1000) users      (100)     5494 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TV.f
+-rw-r--r--   0 ben       (1000) users      (100)     5856 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TW.f
+-rw-r--r--   0 ben       (1000) users      (100)    14165 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TX.f
+-rw-r--r--   0 ben       (1000) users      (100)     7949 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TY.f
+-rw-r--r--   0 ben       (1000) users      (100)    13148 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04UD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19456 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04VD.f
+-rw-r--r--   0 ben       (1000) users      (100)    13767 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04VX.f
+-rw-r--r--   0 ben       (1000) users      (100)    15537 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04WD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7221 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04WP.f
+-rw-r--r--   0 ben       (1000) users      (100)    12725 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04WR.f
+-rw-r--r--   0 ben       (1000) users      (100)    13414 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04WU.f
+-rw-r--r--   0 ben       (1000) users      (100)    24819 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04XD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8185 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04XY.f
+-rw-r--r--   0 ben       (1000) users      (100)    22848 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04YD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17365 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04YW.f
+-rw-r--r--   0 ben       (1000) users      (100)    17268 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04ZD.f
+-rw-r--r--   0 ben       (1000) users      (100)    12341 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB05MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    11110 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB05MY.f
+-rw-r--r--   0 ben       (1000) users      (100)    11292 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB05ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    17518 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB05OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4629 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB05OY.f
+-rw-r--r--   0 ben       (1000) users      (100)    26707 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB3JZP.f
+-rw-r--r--   0 ben       (1000) users      (100)    34693 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB3LZP.f
+-rw-r--r--   0 ben       (1000) users      (100)    13198 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB3OYZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    13642 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB3PYZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     6338 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB4DBZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    28572 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB4DLZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    42410 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB4DPZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     4100 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3081 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     3473 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3787 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3654 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01PY.f
+-rw-r--r--   0 ben       (1000) users      (100)     5622 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7890 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01RD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7131 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01SD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1931 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01SW.f
+-rw-r--r--   0 ben       (1000) users      (100)     1370 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01SX.f
+-rw-r--r--   0 ben       (1000) users      (100)     3260 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01SY.f
+-rw-r--r--   0 ben       (1000) users      (100)     9206 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01TD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8228 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01VD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3732 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01WD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10210 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01XD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10781 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC03MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17534 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC03ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     4126 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC03NX.f
+-rw-r--r--   0 ben       (1000) users      (100)    13886 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC03NY.f
+-rw-r--r--   0 ben       (1000) users      (100)    37710 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4762 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BA.f
+-rw-r--r--   0 ben       (1000) users      (100)     6981 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BB.f
+-rw-r--r--   0 ben       (1000) users      (100)    48883 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3164 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BF.f
+-rw-r--r--   0 ben       (1000) users      (100)     7376 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BX.f
+-rw-r--r--   0 ben       (1000) users      (100)    16092 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BY.f
+-rw-r--r--   0 ben       (1000) users      (100)     7044 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10532 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01AY.f
+-rw-r--r--   0 ben       (1000) users      (100)     3162 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BA.f
+-rw-r--r--   0 ben       (1000) users      (100)     4561 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BB.f
+-rw-r--r--   0 ben       (1000) users      (100)    13015 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3184 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BE.f
+-rw-r--r--   0 ben       (1000) users      (100)     5216 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BF.f
+-rw-r--r--   0 ben       (1000) users      (100)    23050 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BP.f
+-rw-r--r--   0 ben       (1000) users      (100)    16554 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BQ.f
+-rw-r--r--   0 ben       (1000) users      (100)    23814 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BR.f
+-rw-r--r--   0 ben       (1000) users      (100)    19648 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BS.f
+-rw-r--r--   0 ben       (1000) users      (100)    12213 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BU.f
+-rw-r--r--   0 ben       (1000) users      (100)     6865 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BV.f
+-rw-r--r--   0 ben       (1000) users      (100)     6950 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BW.f
+-rw-r--r--   0 ben       (1000) users      (100)     4484 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BX.f
+-rw-r--r--   0 ben       (1000) users      (100)     8822 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BY.f
+-rw-r--r--   0 ben       (1000) users      (100)    28040 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4214 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01BX.f
+-rw-r--r--   0 ben       (1000) users      (100)     9930 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01BY.f
+-rw-r--r--   0 ben       (1000) users      (100)    22024 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     9194 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01FY.f
+-rw-r--r--   0 ben       (1000) users      (100)    11162 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1669 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02CX.f
+-rw-r--r--   0 ben       (1000) users      (100)    20210 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1234 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MR.f
+-rw-r--r--   0 ben       (1000) users      (100)     1394 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MS.f
+-rw-r--r--   0 ben       (1000) users      (100)    21487 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MT.f
+-rw-r--r--   0 ben       (1000) users      (100)    15692 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MU.f
+-rw-r--r--   0 ben       (1000) users      (100)     1229 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MV.f
+-rw-r--r--   0 ben       (1000) users      (100)     1374 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MW.f
+-rw-r--r--   0 ben       (1000) users      (100)    25300 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MX.f
+-rw-r--r--   0 ben       (1000) users      (100)    30639 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    32249 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     1695 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OU.f
+-rw-r--r--   0 ben       (1000) users      (100)     1732 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OV.f
+-rw-r--r--   0 ben       (1000) users      (100)     1690 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OW.f
+-rw-r--r--   0 ben       (1000) users      (100)     1706 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OX.f
+-rw-r--r--   0 ben       (1000) users      (100)    25732 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OY.f
+-rw-r--r--   0 ben       (1000) users      (100)    24947 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02PD.f
+-rw-r--r--   0 ben       (1000) users      (100)    28828 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02QD.f
+-rw-r--r--   0 ben       (1000) users      (100)    45011 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02RD.f
+-rw-r--r--   0 ben       (1000) users      (100)    16519 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02RU.f
+-rw-r--r--   0 ben       (1000) users      (100)    32171 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02SD.f
+-rw-r--r--   0 ben       (1000) users      (100)    21077 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    14414 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MU.f
+-rw-r--r--   0 ben       (1000) users      (100)     8829 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MV.f
+-rw-r--r--   0 ben       (1000) users      (100)     8541 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MW.f
+-rw-r--r--   0 ben       (1000) users      (100)    25043 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MX.f
+-rw-r--r--   0 ben       (1000) users      (100)    20390 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MY.f
+-rw-r--r--   0 ben       (1000) users      (100)    32135 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OD.f
+-rw-r--r--   0 ben       (1000) users      (100)    13413 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OR.f
+-rw-r--r--   0 ben       (1000) users      (100)    19607 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OS.f
+-rw-r--r--   0 ben       (1000) users      (100)    35867 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OT.f
+-rw-r--r--   0 ben       (1000) users      (100)    15269 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OU.f
+-rw-r--r--   0 ben       (1000) users      (100)     2994 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OV.f
+-rw-r--r--   0 ben       (1000) users      (100)    23490 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OY.f
+-rw-r--r--   0 ben       (1000) users      (100)    30928 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    13488 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03PD.f
+-rw-r--r--   0 ben       (1000) users      (100)    24244 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03QD.f
+-rw-r--r--   0 ben       (1000) users      (100)    12125 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03QX.f
+-rw-r--r--   0 ben       (1000) users      (100)    13679 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03QY.f
+-rw-r--r--   0 ben       (1000) users      (100)    13267 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03RD.f
+-rw-r--r--   0 ben       (1000) users      (100)    24627 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03SD.f
+-rw-r--r--   0 ben       (1000) users      (100)    12292 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03SX.f
+-rw-r--r--   0 ben       (1000) users      (100)    13989 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03SY.f
+-rw-r--r--   0 ben       (1000) users      (100)    20057 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03TD.f
+-rw-r--r--   0 ben       (1000) users      (100)    20251 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03UD.f
+-rw-r--r--   0 ben       (1000) users      (100)    12558 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5298 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04MR.f
+-rw-r--r--   0 ben       (1000) users      (100)     4877 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04MU.f
+-rw-r--r--   0 ben       (1000) users      (100)     4564 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04MW.f
+-rw-r--r--   0 ben       (1000) users      (100)     4179 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04MY.f
+-rw-r--r--   0 ben       (1000) users      (100)    13096 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     5040 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04NV.f
+-rw-r--r--   0 ben       (1000) users      (100)     4359 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04NW.f
+-rw-r--r--   0 ben       (1000) users      (100)    10570 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04NX.f
+-rw-r--r--   0 ben       (1000) users      (100)     7719 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04NY.f
+-rw-r--r--   0 ben       (1000) users      (100)    38542 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04OD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17741 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04OW.f
+-rw-r--r--   0 ben       (1000) users      (100)    24585 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04PD.f
+-rw-r--r--   0 ben       (1000) users      (100)    14233 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04PX.f
+-rw-r--r--   0 ben       (1000) users      (100)    40219 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04PY.f
+-rw-r--r--   0 ben       (1000) users      (100)    13259 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5313 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04QR.f
+-rw-r--r--   0 ben       (1000) users      (100)     5712 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04QU.f
+-rw-r--r--   0 ben       (1000) users      (100)     4665 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04QY.f
+-rw-r--r--   0 ben       (1000) users      (100)    13047 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04RD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6565 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04RV.f
+-rw-r--r--   0 ben       (1000) users      (100)     5371 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04RW.f
+-rw-r--r--   0 ben       (1000) users      (100)    13195 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04RX.f
+-rw-r--r--   0 ben       (1000) users      (100)     7736 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04RY.f
+-rw-r--r--   0 ben       (1000) users      (100)    10670 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB06ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    12742 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08CD.f
+-rw-r--r--   0 ben       (1000) users      (100)    20654 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08DD.f
+-rw-r--r--   0 ben       (1000) users      (100)    12831 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08ED.f
+-rw-r--r--   0 ben       (1000) users      (100)    22423 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08FD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7978 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08GD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8539 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08HD.f
+-rw-r--r--   0 ben       (1000) users      (100)    14316 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     2407 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08MY.f
+-rw-r--r--   0 ben       (1000) users      (100)    12182 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     1789 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08NY.f
+-rw-r--r--   0 ben       (1000) users      (100)     7496 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB09MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    30294 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    34738 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10DD.f
+-rw-r--r--   0 ben       (1000) users      (100)    16346 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10ED.f
+-rw-r--r--   0 ben       (1000) users      (100)    16906 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10FD.f
+-rw-r--r--   0 ben       (1000) users      (100)    12718 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10HD.f
+-rw-r--r--   0 ben       (1000) users      (100)    18316 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10ID.f
+-rw-r--r--   0 ben       (1000) users      (100)    10650 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10JD.f
+-rw-r--r--   0 ben       (1000) users      (100)    20934 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10KD.f
+-rw-r--r--   0 ben       (1000) users      (100)    13819 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10LD.f
+-rw-r--r--   0 ben       (1000) users      (100)    23576 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17239 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10PD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19644 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10QD.f
+-rw-r--r--   0 ben       (1000) users      (100)    23673 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10RD.f
+-rw-r--r--   0 ben       (1000) users      (100)    20581 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10SD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10872 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10TD.f
+-rw-r--r--   0 ben       (1000) users      (100)    13495 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10UD.f
+-rw-r--r--   0 ben       (1000) users      (100)    12236 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10VD.f
+-rw-r--r--   0 ben       (1000) users      (100)     9207 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10WD.f
+-rw-r--r--   0 ben       (1000) users      (100)    21377 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10YD.f
+-rw-r--r--   0 ben       (1000) users      (100)    29986 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10ZD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10582 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10ZP.f
+-rw-r--r--   0 ben       (1000) users      (100)    28304 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB16AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    31201 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB16AY.f
+-rw-r--r--   0 ben       (1000) users      (100)    24504 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB16BD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19937 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB16CD.f
+-rw-r--r--   0 ben       (1000) users      (100)    12843 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB16CY.f
+-rw-r--r--   0 ben       (1000) users      (100)    34716 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG02AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17103 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG02CV.f
+-rw-r--r--   0 ben       (1000) users      (100)   116531 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG02CW.f
+-rw-r--r--   0 ben       (1000) users      (100)    25459 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG02CX.f
+-rw-r--r--   0 ben       (1000) users      (100)    47210 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG02ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    23750 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    21210 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03AX.f
+-rw-r--r--   0 ben       (1000) users      (100)    21191 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03AY.f
+-rw-r--r--   0 ben       (1000) users      (100)    34718 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5365 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BR.f
+-rw-r--r--   0 ben       (1000) users      (100)    22062 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BS.f
+-rw-r--r--   0 ben       (1000) users      (100)    19412 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BT.f
+-rw-r--r--   0 ben       (1000) users      (100)    25072 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BU.f
+-rw-r--r--   0 ben       (1000) users      (100)    22444 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BV.f
+-rw-r--r--   0 ben       (1000) users      (100)    13950 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BW.f
+-rw-r--r--   0 ben       (1000) users      (100)    26021 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BX.f
+-rw-r--r--   0 ben       (1000) users      (100)     2033 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BY.f
+-rw-r--r--   0 ben       (1000) users      (100)    32696 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     6189 2021-02-21 11:35:22.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SLCT_DLATZM.f
+-rw-r--r--   0 ben       (1000) users      (100)     6252 2021-02-21 11:35:22.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/SLCT_ZLATZM.f
+-rw-r--r--   0 ben       (1000) users      (100)    11518 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01ID.f
+-rw-r--r--   0 ben       (1000) users      (100)    11693 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01IZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    11816 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01KD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8224 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01KX.f
+-rw-r--r--   0 ben       (1000) users      (100)    11735 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01LD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10505 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10706 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    12198 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17370 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01PX.f
+-rw-r--r--   0 ben       (1000) users      (100)     9848 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01TD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4161 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01TY.f
+-rw-r--r--   0 ben       (1000) users      (100)    17290 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01UD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10382 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01UX.f
+-rw-r--r--   0 ben       (1000) users      (100)    22004 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01UY.f
+-rw-r--r--   0 ben       (1000) users      (100)    16941 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01VD.f
+-rw-r--r--   0 ben       (1000) users      (100)     9543 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01VY.f
+-rw-r--r--   0 ben       (1000) users      (100)     8088 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01WD.f
+-rw-r--r--   0 ben       (1000) users      (100)     9704 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01WX.f
+-rw-r--r--   0 ben       (1000) users      (100)     8006 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01XD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7878 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01XZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     4568 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01YD.f
+-rw-r--r--   0 ben       (1000) users      (100)    14799 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01ZD.f
+-rw-r--r--   0 ben       (1000) users      (100)    26079 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4777 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB03AY.f
+-rw-r--r--   0 ben       (1000) users      (100)    13925 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8158 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04AY.f
+-rw-r--r--   0 ben       (1000) users      (100)    21420 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04BD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10662 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04BV.f
+-rw-r--r--   0 ben       (1000) users      (100)     8554 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04BW.f
+-rw-r--r--   0 ben       (1000) users      (100)     6965 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04BX.f
+-rw-r--r--   0 ben       (1000) users      (100)    20498 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04CD.f
+-rw-r--r--   0 ben       (1000) users      (100)    17929 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB05AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6850 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TC01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)    16163 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TC04AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    13038 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TC05AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    21042 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TD03AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     5436 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TD03AY.f
+-rw-r--r--   0 ben       (1000) users      (100)    14731 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TD04AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8657 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TD05AD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6781 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    13198 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01MX.f
+-rw-r--r--   0 ben       (1000) users      (100)    11789 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01MY.f
+-rw-r--r--   0 ben       (1000) users      (100)     8179 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     4826 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4931 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)     7255 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01QD.f
+-rw-r--r--   0 ben       (1000) users      (100)     6435 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01RD.f
+-rw-r--r--   0 ben       (1000) users      (100)    15534 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01AD.f
+-rw-r--r--   0 ben       (1000) users      (100)    15790 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01AZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    15683 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8797 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     8968 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01DD.f
+-rw-r--r--   0 ben       (1000) users      (100)    28377 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01ED.f
+-rw-r--r--   0 ben       (1000) users      (100)    26004 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01FD.f
+-rw-r--r--   0 ben       (1000) users      (100)    26204 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01FZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    16187 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01GD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19720 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01HD.f
+-rw-r--r--   0 ben       (1000) users      (100)    29831 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01HU.f
+-rw-r--r--   0 ben       (1000) users      (100)    23696 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01HX.f
+-rw-r--r--   0 ben       (1000) users      (100)    31804 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01HY.f
+-rw-r--r--   0 ben       (1000) users      (100)    21425 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01ID.f
+-rw-r--r--   0 ben       (1000) users      (100)    23430 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01JD.f
+-rw-r--r--   0 ben       (1000) users      (100)    39681 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01JY.f
+-rw-r--r--   0 ben       (1000) users      (100)    11157 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01KD.f
+-rw-r--r--   0 ben       (1000) users      (100)    11457 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01KZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    19227 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01LD.f
+-rw-r--r--   0 ben       (1000) users      (100)    27137 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01LY.f
+-rw-r--r--   0 ben       (1000) users      (100)    16640 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19789 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)    11559 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01NX.f
+-rw-r--r--   0 ben       (1000) users      (100)     5401 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01OA.f
+-rw-r--r--   0 ben       (1000) users      (100)     5582 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01OB.f
+-rw-r--r--   0 ben       (1000) users      (100)    11395 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01OD.f
+-rw-r--r--   0 ben       (1000) users      (100)    11772 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01OZ.f
+-rw-r--r--   0 ben       (1000) users      (100)    19572 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01PD.f
+-rw-r--r--   0 ben       (1000) users      (100)    19304 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01QD.f
+-rw-r--r--   0 ben       (1000) users      (100)    10460 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01WD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3375 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01BD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4803 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01CD.f
+-rw-r--r--   0 ben       (1000) users      (100)     3066 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01DD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4214 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)     4155 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01MZ.f
+-rw-r--r--   0 ben       (1000) users      (100)     5338 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01ND.f
+-rw-r--r--   0 ben       (1000) users      (100)     8563 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/UE01MD.f
+-rw-r--r--   0 ben       (1000) users      (100)      198 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/delctg.f
+-rw-r--r--   0 ben       (1000) users      (100)     8744 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/makefile
+-rw-r--r--   0 ben       (1000) users      (100)     7580 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/makefile_Unix
+-rw-r--r--   0 ben       (1000) users      (100)      348 2021-02-07 14:11:14.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/readme
+-rw-r--r--   0 ben       (1000) users      (100)      186 2022-07-09 12:47:33.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src/select.f
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:48.054601 slycot-0.5.4/slycot/src/SLICOT-Reference/src_aux/
+-rw-r--r--   0 ben       (1000) users      (100)     6003 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src_aux/dlatzm.f
+-rw-r--r--   0 ben       (1000) users      (100)     1360 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src_aux/makefile
+-rw-r--r--   0 ben       (1000) users      (100)     1504 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src_aux/makefile_Unix
+-rw-r--r--   0 ben       (1000) users      (100)      225 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src_aux/readme
+-rw-r--r--   0 ben       (1000) users      (100)     6140 2023-04-26 07:37:27.000000 slycot-0.5.4/slycot/src/SLICOT-Reference/src_aux/zlatzm.f
+-rw-r--r--   0 ben       (1000) users      (100)      207 2021-01-22 23:20:08.000000 slycot-0.5.4/slycot/src/XERBLA.f
+-rw-r--r--   0 ben       (1000) users      (100)      335 2021-01-22 23:20:08.000000 slycot-0.5.4/slycot/src/_helper.pyf
+-rw-r--r--   0 ben       (1000) users      (100)      292 2021-01-22 23:20:08.000000 slycot-0.5.4/slycot/src/_wrapper.pyf
+-rw-r--r--   0 ben       (1000) users      (100)    23086 2022-12-19 11:28:53.000000 slycot-0.5.4/slycot/src/analysis.pyf
+-rw-r--r--   0 ben       (1000) users      (100)      252 2021-01-22 23:20:08.000000 slycot-0.5.4/slycot/src/ftruefalse.f
+-rw-r--r--   0 ben       (1000) users      (100)     6368 2022-12-19 11:28:53.000000 slycot-0.5.4/slycot/src/math.pyf
+-rw-r--r--   0 ben       (1000) users      (100)    46295 2022-07-09 14:31:14.000000 slycot-0.5.4/slycot/src/synthesis.pyf
+-rw-r--r--   0 ben       (1000) users      (100)    28949 2021-01-22 23:20:08.000000 slycot-0.5.4/slycot/src/transform.pyf
+-rw-r--r--   0 ben       (1000) users      (100)   107860 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/synthesis.py
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:48.058601 slycot-0.5.4/slycot/tests/
+-rw-r--r--   0 ben       (1000) users      (100)      359 2021-01-22 23:20:08.000000 slycot-0.5.4/slycot/tests/CMakeLists.txt
+-rw-r--r--   0 ben       (1000) users      (100)        0 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/__init__.py
+-rw-r--r--   0 ben       (1000) users      (100)     1936 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_ab01.py
+-rw-r--r--   0 ben       (1000) users      (100)     3063 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_ab08n.py
+-rw-r--r--   0 ben       (1000) users      (100)     4107 2022-05-29 11:49:04.000000 slycot-0.5.4/slycot/tests/test_ab13md.py
+-rw-r--r--   0 ben       (1000) users      (100)     4145 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_ag08bd.py
+-rw-r--r--   0 ben       (1000) users      (100)     2434 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_analysis.py
+-rw-r--r--   0 ben       (1000) users      (100)     1952 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_examples.py
+-rw-r--r--   0 ben       (1000) users      (100)     4390 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_exceptions.py
+-rw-r--r--   0 ben       (1000) users      (100)    14232 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_mb.py
+-rw-r--r--   0 ben       (1000) users      (100)     1575 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_mc.py
+-rw-r--r--   0 ben       (1000) users      (100)     8712 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_sb.py
+-rw-r--r--   0 ben       (1000) users      (100)     1531 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_sg02ad.py
+-rw-r--r--   0 ben       (1000) users      (100)     2591 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_sg03ad.py
+-rw-r--r--   0 ben       (1000) users      (100)     8898 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_tb05ad.py
+-rw-r--r--   0 ben       (1000) users      (100)     8707 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_td04ad.py
+-rw-r--r--   0 ben       (1000) users      (100)     2573 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_tg01ad.py
+-rw-r--r--   0 ben       (1000) users      (100)     4403 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_tg01fd.py
+-rw-r--r--   0 ben       (1000) users      (100)      914 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/tests/test_transform.py
+-rw-r--r--   0 ben       (1000) users      (100)    55443 2022-07-10 10:32:17.000000 slycot-0.5.4/slycot/transform.py
+-rw-r--r--   0 ben       (1000) users      (100)      160 2023-04-27 19:48:47.000000 slycot-0.5.4/slycot/version.py
+drwxr-xr-x   0 ben       (1000) users      (100)        0 2023-04-27 19:48:47.382582 slycot-0.5.4/slycot.egg-info/
+-rw-r--r--   0 ben       (1000) users      (100)    10373 2023-04-27 19:48:47.000000 slycot-0.5.4/slycot.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (100)    89591 2023-04-27 19:48:47.000000 slycot-0.5.4/slycot.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) users      (100)        1 2023-04-27 19:48:47.000000 slycot-0.5.4/slycot.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) users      (100)        6 2023-04-27 19:48:47.000000 slycot-0.5.4/slycot.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) users      (100)        7 2023-04-27 19:48:47.000000 slycot-0.5.4/slycot.egg-info/top_level.txt
```

### Comparing `slycot-0.5.3/.github/scripts/run-tests.sh` & `slycot-0.5.4/.github/scripts/run-tests.sh`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/.github/scripts/set-conda-test-matrix.py` & `slycot-0.5.4/.github/scripts/set-conda-test-matrix.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/.github/scripts/set-pip-test-matrix.py` & `slycot-0.5.4/.github/scripts/set-pip-test-matrix.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/.github/workflows/slycot-build-and-test.yml` & `slycot-0.5.4/.github/workflows/slycot-build-and-test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -279,15 +279,17 @@
       - name: Install Wheel
         run: |
           python -m pip install --upgrade pip
           pip install matplotlib scipy pytest pytest-cov pytest-timeout coverage coveralls
           pip install slycot-wheels/${{ matrix.packagekey }}/slycot*.whl
           pip show slycot
       - name: Slycot and python-control tests
-        run: bash slycot-src/.github/scripts/run-tests.sh
+        run: JOBNAME="$JOBNAME" bash slycot-src/.github/scripts/run-tests.sh
+        env:
+          JOBNAME: wheel ${{ matrix.packagekey }} ${{ matrix.blas_lib }}
       - name: report coverage
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           COVERALLS_FLAG_NAME: wheel-${{ matrix.packagekey }}-${{matrix.blas_lib}}
           COVERALLS_PARALLEL: true
         working-directory: slycot-src
         # https://github.com/TheKevJames/coveralls-python/issues/252
@@ -355,15 +357,17 @@
               echo "libblas * *mkl" >> $CONDA_PREFIX/conda-meta/pinned
               ;;
           esac
           conda index --no-progress ./slycot-conda-pkgs
           mamba install -c ./slycot-conda-pkgs slycot
           conda list
       - name: Slycot and python-control tests
-        run: bash slycot-src/.github/scripts/run-tests.sh
+        run: JOBNAME="$JOBNAME" bash slycot-src/.github/scripts/run-tests.sh
+        env:
+          JOBNAME: conda ${{ matrix.packagekey }} ${{ matrix.blas_lib }}
       - name: Report coverage
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           COVERALLS_FLAG_NAME: conda-${{ matrix.packagekey }}-${{matrix.blas_lib}}
           COVERALLS_PARALLEL: true
         working-directory: slycot-src
         # https://github.com/TheKevJames/coveralls-python/issues/252
```

### Comparing `slycot-0.5.3/CMakeLists.txt` & `slycot-0.5.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/COPYING` & `slycot-0.5.4/COPYING`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/PKG-INFO` & `slycot-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slycot
-Version: 0.5.3
+Version: 0.5.4
 Summary: A wrapper for the SLICOT control and systems library
 Author: Enrico Avventi et al.
 Maintainer-email: Slycot developers <python-control-discuss@lists.sourceforge.net>
 License: GPL-2.0 AND BSD-3-Clause
 Project-URL: homepage, https://github.com/python-control/Slycot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -23,14 +23,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: COPYING
 License-File: AUTHORS
 
 Slycot
 ======
 
 .. image:: https://img.shields.io/pypi/v/slycot.svg
    :target: https://pypi.org/project/slycot/
```

### Comparing `slycot-0.5.3/README.rst` & `slycot-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/conda-recipe/meta.yaml` & `slycot-0.5.4/conda-recipe/meta.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     # deviating from above link: we have to specifiy netlib variant, because
     # the mkl variant selected by default for older pythons on windows
     # does not provide the generic headers
     - libblas * *netlib
     - libcblas * *netlib
     - liblapack * *netlib
     - python
-    - numpy !=1.23.0
+    - numpy >=1.19,!=1.23.0
     - pip
     - scikit-build >=0.15
     - setuptools >=45
     - setuptools_scm >=7
 
   run:
     - python {{ PY_VER }}
```

### Comparing `slycot-0.5.3/gpl-2.0.txt` & `slycot-0.5.4/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/pyproject.toml` & `slycot-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/setup.py` & `slycot-0.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,13 +54,14 @@
     """ check submodules on sdist to prevent incomplete tarballs """
     def run(self):
         check_submodules()
         sdist.run(self)
 
 # These need to stay in setup.py
 # https://scikit-build.readthedocs.io/en/latest/usage.html#setuptools-options
-setup(     
+setup(
     packages=['slycot', 'slycot.tests'],
     cmdclass={'sdist': sdist_checked},
     cmake_languages=('C', 'Fortran'),
     use_scm_version = True,
+    include_package_data = False,
 )
```

### Comparing `slycot-0.5.3/slycot/CMakeLists.txt` & `slycot-0.5.4/slycot/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/__init__.py` & `slycot-0.5.4/slycot/__init__.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/analysis.py` & `slycot-0.5.4/slycot/analysis.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/examples.py` & `slycot-0.5.4/slycot/examples.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/exceptions.py` & `slycot-0.5.4/slycot/exceptions.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/math.py` & `slycot-0.5.4/slycot/math.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/Readme.md` & `slycot-0.5.4/slycot/src/Readme.md`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/Contributors.md` & `slycot-0.5.4/slycot/src/SLICOT-Reference/Contributors.md`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/LICENSE` & `slycot-0.5.4/slycot/src/SLICOT-Reference/LICENSE`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/README.md` & `slycot-0.5.4/slycot/src/SLICOT-Reference/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,17 @@
 - the contributors to the library and financial support, Contributors.md,
 
 - the license file, LICENSE, and
 
 - the main SLICOT Library documentation index, libindex.html.
 
 After software installation, this directory will also contain the library 
-file slicot.a or slicot.lib, for Unix or Windows platforms, respectively.
-The library file could then be linked in applications programs, as usual.
+files slicot.a and lpkaux.a, or slicot.lib and lpkaux.lib, for Unix or 
+Windows platforms, respectively.
+The library files could then be linked in applications programs, as usual.
 Specific examples are contained in the directory examples.
 The on-line documentation of the SLICOT user's callable routines is
 accessible via the main SLICOT Library documentation index, libindex.html.
 This file also contains a link to the documentation of the lower-level,
 support routines.
 
 The SLICOT Library is built on LAPACK (Linear Algebra PACKage) and BLAS
```

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/ReleaseNotes.md` & `slycot-0.5.4/slycot/src/SLICOT-Reference/ReleaseNotes.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,33 @@
 # SLICOT Library Release Notes
 
+## Version v5.8, Update 1
+
+**Updated Routines**
+
+**`MB01PD:`** Removed `SAVE` statement and variable `FIRST` to get a thread safe version.
+
+**`MB03VY:`**  Set `A( ILO, ILO, J )` to 1 if `IHI = ILO` in the loop labelled 20.
+ 
+**`MB04BD`**:  Changed some part of finding the number of infinite eigenvalues (replaced `DE(1,2)` by `DE(1,3)` in the line 495, and replaced `NINF = MAX( I, J )` by `NINF = MAX( I, J )/2` in the line 513).
+
+**`MB04BP`**:  Changed some part of finding the number of infinite eigenvalues (replaced `DE(1,2)` by `DE(1,3)` in the line 509, and replaced `NINF = MAX( I, J )` by `NINF = MAX( I, J )/2` in the line 527).  Called **`MB04BD`** internally, if on entry `INFO = 0` or if `INFO < 0` and `M` is sufficiently small (`M <= NX`, with parameter `NX` set to 250).  Updated the documentation file, **`MB04BP.html`**.
+
+**Updated makefile**
+
+The files **`makefile`** in the **`examples`** and **`src`** sub-directories have been updated, by alphabetically ordering the names, and adding the missing ones.
+
+**New files**
+
+Added **`make.inc`** and **`makefile`** in the **`slicot`** directory for Windows platform with Intel Fortran compilers.
+
+Added **`make_Unix.inc`** in **`slicot`** directory and **`makefile_Unix`** in **`slicot`** directory and subdirectories **`examples`** and **`src`**, for Unix-like platfoms with gfortran compiler.
+
+Added the file **`Installation.txt`** in the **`slicot`** directory.
+
 ## Version v5.8 
 
 Version v5.8 of the **SLICOT** Library includes 18 new routines and 14 routines with more or few changes in the operational part of the source code, in comparison to Version v5.7 of the library.  Moreover, the (comment) lines referring to the version number have been removed in all routines, example programs, and documentation files.
 
 **New Routines**
 
 **`MA02AZ:`** (Conjugate) transposes all or part of a two-dimensional complex matrix.
@@ -84,15 +108,15 @@
 
 **`TG01OA, TG01OB:`** Compute for a single-input single-output descriptor system, `(A, E, B, C)`, with `E` upper triangular, a transformed system, `(Q'*A*Z, Q'*E*Z, Q'*B, C*Z)`, via an orthogonal/unitary equivalence transformation, so that `Q'*B` has only the first element nonzero and `Q'*E*Z` remains upper triangular. `TG01OA` is the real version and `TG01OB` is the complex version. `A`, `B`, `C` are stored in an array as the block elements `(2,2)`, `(2,1)`, and `(1,2)`, respectively, and `Q` and `Z` are not accumulated. These are the main differences with SLICOT Library routines `TG01KD` and `TG01KZ`.
 
 **`TG01OD, TG01OZ:`** Compute for a single-input single-output descriptor system, `(A, E, B, C)`, with `E` nonsingular, a reduced system with a "sufficiently" large feedthrough variable, using `TG01OA/TG01OB`.
 
 **Updated Routines**
 
-**`AB13MD:`** Computed the correct upper bound on the structured singular value for a 1-by-1 real matrix and a real uncertainty. Replaced `DFLOAT` by `DBLE` in line `834` to avoid a trouble with an Apple Silicon  compiler.
+**`AB13MD:`** Computed the correct upper bound on the structured singular value for a 1-by-1 real matrix and a real uncertainty. Replaced `DFLOAT` by `DBLE` in line `834` to avoid a trouble with an Apple Silicon compiler.
 
 **`MA02EZ:`** A new option, `SKEW = 'G'`, has been added that allows to suitably deal with the diagonal of a general square triangular matrix. This option is needed in the new routines `MB01UZ`, `SG03BS`, and `SG03BT`. Moreover, the internal loop index `J` has been modified from `2` to `I` or `I+1`, to reduce the number of cycles to the minimum values.
 
 **`MB03RD:`** Replaced `PMAX*PMAX` by `PMAX` in the comments;  the `PMAX` value agrees to the condition number for the optimally scaled transformations used.
 
 **`MB04BD:`** Made a correction (in comments) of the indices of the `1-by-1` or `2-by-2` quadruple diagonal blocks stored in `DWORK`. Increased `I2X2` by `1` if a `2x2` quadruple of diagonal blocks is found to have real eigenvalues (in order to check them externally). These are stored as `2x2` quadruple blocks in DWORK in that case. Made two corrections of the pointers to the locations in `DWORK` storing the quadruples with unreliable eigenvalues.
```

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB01104.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB01104.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB01105.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB01105.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB01106.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB01106.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB012091.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB012091.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB012092.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB012092.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB01404.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB01404.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB02110.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB02110.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB02111.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB02111.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BB02113.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BB02113.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01104.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01104.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01105.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01105.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01106.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01106.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01107.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01107.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01108.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01108.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01109.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01109.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01110.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01110.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01203.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01203.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012053.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012053.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012054.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012054.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012055.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012055.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012056.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012056.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD012057.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD012057.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD01304.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD01304.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/benchmark_data/BD02111.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/benchmark_data/BD02111.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB01ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB01ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB01OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB01OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB04MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB04MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB05SD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB05SD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB07MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB07MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB07ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB07ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08MZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08MZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08NW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08NW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08NX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08NX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08NY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08NY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB08NZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB08NZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09AX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09AX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09BX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09BX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09CX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09CX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09DD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09DD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09ED.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09ED.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09FD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09FD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09GD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09GD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09HD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09HD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09HX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09HX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09HY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09HY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09ID.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09ID.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09IX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09IX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09IY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09IY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09JD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09JD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09JV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09JV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09JW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09JW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09JX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09JX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09KD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09KD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09KX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09KX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB09ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB09ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13AX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13AX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13DD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13DD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13DX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13DX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13ED.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13ED.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13FD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13FD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13ID.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13ID.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB13MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB13MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AB8NXZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AB8NXZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AG07BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AG07BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AG08BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AG08BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AG08BY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AG08BY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AG08BZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AG08BZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/AG8BYZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/AG8BYZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BB01AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BB01AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BB02AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BB02AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BB03AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BB03AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BB04AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BB04AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BD01AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BD01AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/BD02AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/BD02AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DAESolver.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DAESolver.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DE01OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DE01OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DE01PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DE01PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DF01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DF01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DG01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DG01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DG01ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DG01ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DG01OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DG01OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/DK01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/DK01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FB01QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FB01QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FB01RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FB01RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FB01SD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FB01SD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FB01TD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FB01TD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FB01VD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FB01VD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FD01AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FD01AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/FSQP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/FSQP.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01MY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01MY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01OY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01OY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01PX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01PX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01PY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01PY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB01RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB01RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB03AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB03AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/IB03BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/IB03BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/KINSOL.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/KINSOL.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA01AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA01AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA01BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA01BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA01BZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA01BZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA01CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA01CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02AZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02AZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02BZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02BZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02CZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02CZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02DD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02DD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02ED.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02ED.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02ES.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02ES.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02EZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02EZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02FD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02FD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02GD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02GD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02GZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02GZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02HD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02HD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02HZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02HZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02ID.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02ID.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02IZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02IZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02JD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02JD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02JZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02JZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02MZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02MZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02NZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02NZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02OZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02OZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MA02PZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MA02PZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01KD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01KD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01LD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01LD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OC.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OC.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OE.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OE.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OH.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OH.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OO.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OO.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OS.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OS.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01OT.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01OT.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RB.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RB.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RH.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RH.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RT.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RT.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01RY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01RY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01SD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01SD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01SS.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01SS.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01TD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01TD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01UD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01UD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01UW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01UW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01UX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01UX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01UY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01UY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01UZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01UZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01VD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01VD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01WD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01WD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01XD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01XD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01XY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01XY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01YD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01YD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB01ZD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB01ZD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02CU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02CU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02CV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02CV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02CX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02CX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02CY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02CY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02DD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02DD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02ED.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02ED.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02FD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02FD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02GD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02GD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02HD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02HD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02ID.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02ID.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02JD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02JD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02JX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02JX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02KD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02KD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02NY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02NY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02QY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02QY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02RZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02RZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02SD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02SD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02SZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02SZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02TD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02TD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02TZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02TZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02UD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02UD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02UU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02UU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02UV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02UV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02UW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02UW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02VD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02VD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02WD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02WD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02XD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02XD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB02YD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB02YD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AB.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AB.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AE.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AE.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AF.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AF.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AG.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AG.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AH.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AH.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03AI.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03AI.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BA.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BA.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BB.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BB.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BC.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BC.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BE.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BE.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BF.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BF.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03BZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03BZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03CZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03CZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03DD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03DD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03DZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03DZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03ED.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03ED.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03FD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03FD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03FZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03FZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03GD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03GD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03GZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03GZ.html`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,21 @@
 
          (  CO1  SI1  )         (  CO2  SI2  )
      Q = (            ) and U = (            ), respectively.
          ( -SI1' CO1  )         ( -SI2' CO2  )
 
   The notation M' denotes the conjugate transpose of the matrix M.
 
+</PRE>
+<A name="Specification"><B><FONT SIZE="+1">Specification</FONT></B></A>
+<PRE>
+      SUBROUTINE MB03GZ( Z11, Z12, Z22, H11, H12, CO1, SI1, CO2, SI2 )
+C     .. Scalar Arguments ..
+      DOUBLE PRECISION   CO1, CO2
+      COMPLEX*16         H11, H12, SI1, SI2, Z11, Z12, Z22
 
 </PRE>
 <A name="Arguments"><B><FONT SIZE="+1">Arguments</FONT></B></A>
 <P>
 
 </PRE>
 <B>Input/Output Parameters</B>
```

#### html2text {}

```diff
@@ -16,15 +16,19 @@
   The matrices Q and U are represented by
 
          (  CO1  SI1  )         (  CO2  SI2  )
      Q = (            ) and U = (            ), respectively.
          ( -SI1' CO1  )         ( -SI2' CO2  )
 
   The notation M' denotes the conjugate transpose of the matrix M.
-
+Specification
+      SUBROUTINE MB03GZ( Z11, Z12, Z22, H11, H12, CO1, SI1, CO2, SI2 )
+C     .. Scalar Arguments ..
+      DOUBLE PRECISION   CO1, CO2
+      COMPLEX*16         H11, H12, SI1, SI2, Z11, Z12, Z22
 Arguments
 Input/Output Parameters
   Z11     (input) COMPLEX*16
           Upper left element of the non-trivial factor Z in the
           factorization of S.
 
   Z12     (input) COMPLEX*16
```

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03HD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03HD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03HZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03HZ.html`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,21 @@
 
       (  CO  SI  )
   Q = (          ).
       ( -SI' CO  )
 
   The notation M' denotes the conjugate transpose of the matrix M.
 
+</PRE>
+<A name="Specification"><B><FONT SIZE="+1">Specification</FONT></B></A>
+<PRE>
+      SUBROUTINE MB03HZ( S11, S12, H11, H12, CO, SI )
+C     .. Scalar Arguments ..
+      DOUBLE PRECISION   CO
+      COMPLEX*16         H11, H12, S11, S12, SI
 
 </PRE>
 <A name="Arguments"><B><FONT SIZE="+1">Arguments</FONT></B></A>
 <P>
 
 </PRE>
 <B>Input/Output Parameters</B>
```

#### html2text {}

```diff
@@ -14,15 +14,19 @@
   eigenvalues are in reversed order. The matrix Q is represented by
 
       (  CO  SI  )
   Q = (          ).
       ( -SI' CO  )
 
   The notation M' denotes the conjugate transpose of the matrix M.
-
+Specification
+      SUBROUTINE MB03HZ( S11, S12, H11, H12, CO, SI )
+C     .. Scalar Arguments ..
+      DOUBLE PRECISION   CO
+      COMPLEX*16         H11, H12, S11, S12, SI
 Arguments
 Input/Output Parameters
   S11     (input) COMPLEX*16
           Upper left element of the skew-Hamiltonian matrix S.
 
   S12     (input) COMPLEX*16
           Upper right element of the skew-Hamiltonian matrix S.
```

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03ID.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03ID.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03IZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03IZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03JD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03JD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03JP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03JP.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03JZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03JZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03KA.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03KA.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03KB.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03KB.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03KC.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03KC.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03KD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03KD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03KE.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03KE.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03LD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03LD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03LF.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03LF.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03LP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03LP.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03LZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03LZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03NY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03NY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03OY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03OY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03PY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03PY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QG.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QG.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03QY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03QY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03RW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03RW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03RX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03RX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03RY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03RY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03RZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03RZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03SD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03SD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03TD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03TD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03TS.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03TS.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03UD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03UD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03VD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03VD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03VW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03VW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03VY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03VY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03WA.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03WA.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03WD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03WD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03WX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03WX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03XD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03XD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03XP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03XP.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03XS.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03XS.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03XU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03XU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03XZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03XZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03YA.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03YA.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03YD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03YD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03YT.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03YT.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03ZA.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03ZA.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB03ZD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB03ZD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04AZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04AZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04BP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04BP.html`

 * *Files 1% similar despite different names*

```diff
@@ -369,16 +369,17 @@
   floating point operations.
 
 </PRE>
 <A name="Comments"><B><FONT SIZE="+1">Further Comments</FONT></B></A>
 <PRE>
   For large values of N, the routine applies the transformations
   for reducing T on panels of columns. The user may specify in INFO
-  the desired number of columns. If on entry INFO &lt;= 0, then the
-  routine estimates a suitable value of this number.
+  the desired number of columns. If on entry INFO &lt; 0, then the
+  routine estimates a suitable value of this number. If INFO = 0,
+  the routine MB04BD is directly called.
 
 </PRE>
 
 <A name="Example"><B><FONT SIZE="+1">Example</FONT></B></A>
 <P>
 <B>Program Text</B>
 <PRE>
```

#### html2text {}

```diff
@@ -327,16 +327,17 @@
 Numerical Aspects
                                                             3
   The algorithm is numerically backward stable and needs O(N ) real
   floating point operations.
 Further Comments
   For large values of N, the routine applies the transformations
   for reducing T on panels of columns. The user may specify in INFO
-  the desired number of columns. If on entry INFO <= 0, then the
-  routine estimates a suitable value of this number.
+  the desired number of columns. If on entry INFO < 0, then the
+  routine estimates a suitable value of this number. If INFO = 0,
+  the routine MB04BD is directly called.
 Example
 Program Text
   None
 Program Data
   None
 Program Results
   None
```

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04BZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04BZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DB.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DB.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DI.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DI.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DL.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DL.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DP.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DS.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DS.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04DZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04DZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04ED.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04ED.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04FD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04FD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04FP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04FP.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04GD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04GD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04HD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04HD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04ID.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04ID.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04IY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04IY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04IZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04IZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04JD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04JD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04KD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04KD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04LD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04LD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04NY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04NY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04OW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04OW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04OX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04OX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04OY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04OY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04PA.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04PA.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04PB.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04PB.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04PU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04PU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04PY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04PY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04QB.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04QB.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04QC.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04QC.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04QF.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04QF.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04QS.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04QS.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04QU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04QU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04RB.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04RB.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04RU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04RU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04SU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04SU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04TB.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04TB.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04TS.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04TS.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04TU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04TU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04UD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04UD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04VD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04VD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04WD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04WD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04WP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04WP.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04WR.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04WR.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04WU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04WU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04XD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04XD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04XY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04XY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04YD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04YD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04YW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04YW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB04ZD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB04ZD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB05MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB05MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB05MY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB05MY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB05ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB05ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB05OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB05OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB05OY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB05OY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB3JZP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB3JZP.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB3LZP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB3LZP.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB3OYZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB3OYZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB3PYZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB3PYZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB4DBZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB4DBZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB4DLZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB4DLZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MB4DPZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MB4DPZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01PY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01PY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01SD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01SD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01TD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01TD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01VD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01VD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01WD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01WD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC01XD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC01XD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC03MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC03MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC03ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC03ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MC03NX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MC03NX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MD03AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MD03AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MD03BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MD03BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MD03BX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MD03BX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/MD03BY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/MD03BY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01AY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01AY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BP.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BQ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BQ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BR.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BR.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BS.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BS.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/NF01BY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/NF01BY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/ODESolver.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/ODESolver.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01BX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01BX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01BY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01BY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01DD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01DD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01FY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01FY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02MT.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02MT.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02MU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02MU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02MX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02MX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02OY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02OY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02RU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02RU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB02SD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB02SD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03MY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03MY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OR.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OR.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OS.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OS.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OT.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OT.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03OZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03OZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03QX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03QX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03QY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03QY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03SD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03SD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03SX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03SX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03SY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03SY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03TD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03TD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB03UD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB03UD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04MR.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04MR.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04MU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04MU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04MW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04MW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04MY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04MY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04NV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04NV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04NW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04NW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04NX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04NX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04NY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04NY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04OW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04OW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04PX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04PX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04PY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04PY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04QR.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04QR.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04QU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04QU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04QY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04QY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04RV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04RV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04RW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04RW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04RX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04RX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB04RY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB04RY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB06ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB06ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08DD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08DD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08ED.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08ED.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08FD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08FD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08GD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08GD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08HD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08HD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB08ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB08ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB09MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB09MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10DD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10DD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10ED.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10ED.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10FD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10FD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10HD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10HD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10ID.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10ID.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10JD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10JD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10KD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10KD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10LD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10LD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10SD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10SD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10TD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10TD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10UD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10UD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10VD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10VD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10WD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10WD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10YD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10YD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10ZD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10ZD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB10ZP.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB10ZP.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB16AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB16AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB16AY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB16AY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB16BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB16BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB16CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB16CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SB16CY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SB16CY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG02AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG02AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG02CV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG02CV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG02CW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG02CW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG02CX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG02CX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG02ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG02ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03AX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03AX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03AY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03AY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BR.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BR.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BS.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BS.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BT.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BT.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/SG03BZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/SG03BZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01ID.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01ID.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01IZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01IZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01KD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01KD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01KX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01KX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01LD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01LD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01PX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01PX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01TD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01TD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01UD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01UD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01UX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01UX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01UY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01UY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01VD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01VD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01VY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01VY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01WD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01WD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01WX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01WX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01XD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01XD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01XZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01XZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01YD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01YD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB01ZD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB01ZD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB03AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB03AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04BV.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04BV.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04BW.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04BW.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04BX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04BX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB04CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB04CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TB05AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TB05AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TC01OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TC01OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TC04AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TC04AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TC05AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TC05AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TD03AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TD03AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TD04AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TD04AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TD05AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TD05AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01MX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01MX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01MY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01MY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TF01RD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TF01RD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01AD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01AD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01AZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01AZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01DD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01DD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01ED.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01ED.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01FD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01FD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01FZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01FZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01GD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01GD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01HD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01HD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01HU.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01HU.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01HX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01HX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01HY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01HY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01ID.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01ID.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01JD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01JD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01JY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01JY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01KD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01KD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01KZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01KZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01LD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01LD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01LY.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01LY.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01NX.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01NX.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01OA.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01OA.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01OB.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01OB.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01OD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01OD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01OZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01OZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01PD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01PD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01QD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01QD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/TG01WD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/TG01WD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01BD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01BD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01CD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01CD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01DD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01DD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01MD.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01MZ.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01MZ.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UD01ND.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UD01ND.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/UE01MD.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/UE01MD.html`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 
   The default values in this version aim to give good performance on
   a wide range of computers. For optimal performance, however, the
   user is advised to modify this routine. Note that an optimized
   BLAS is a crucial prerequisite for any speed gains. For further
   details, see ILAENV.
 
+</PRE>
+<A name="Specification"><B><FONT SIZE="+1">Specification</FONT></B></A>
+<PRE>
+      INTEGER FUNCTION UE01MD( ISPEC, NAME, OPTS, N1, N2, N3 )
+C     .. Scalar Arguments ..
+      CHARACTER*( * )    NAME, OPTS
+      INTEGER            ISPEC, N1, N2, N3
 
 </PRE>
 <B><FONT SIZE="+1">Function Value</FONT></B>
 <PRE>
   UE01MD  INTEGER
           The function value set according to ISPEC.
```

#### html2text {}

```diff
@@ -7,15 +7,19 @@
   machine-specific parameters for SLICOT routines.
 
   The default values in this version aim to give good performance on
   a wide range of computers. For optimal performance, however, the
   user is advised to modify this routine. Note that an optimized
   BLAS is a crucial prerequisite for any speed gains. For further
   details, see ILAENV.
-
+Specification
+      INTEGER FUNCTION UE01MD( ISPEC, NAME, OPTS, N1, N2, N3 )
+C     .. Scalar Arguments ..
+      CHARACTER*( * )    NAME, OPTS
+      INTEGER            ISPEC, N1, N2, N3
 Function Value
   UE01MD  INTEGER
           The function value set according to ISPEC.
 Arguments
 Input/Output Parameters
   ISPEC   (input) INTEGER
           Specifies the parameter to be returned as the value of
```

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/readme` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/readme`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/doc/support.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/doc/support.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB01ND.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB01ND.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB01OD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB01OD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05MD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05MD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05ND.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05ND.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05OD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05OD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05PD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05PD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05QD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05QD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB05RD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB05RD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB08ND.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB08ND.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB08NW.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB08NW.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB08NZ.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB08NZ.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB08NZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB08NZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09AD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09AD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09BD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09BD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09BD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09BD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09CD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09CD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09CD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09CD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09DD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09DD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09DD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09DD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09ED.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09ED.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09ED.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09ED.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09FD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09FD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09FD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09FD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09GD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09GD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09GD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09GD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09HD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09HD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09HD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09HD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09ID.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09ID.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09JD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09JD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09JD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09JD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09KD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09KD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09KD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09KD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09MD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09MD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09MD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09MD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09ND.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09ND.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB09ND.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB09ND.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13AD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13AD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13BD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13BD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13ED.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13ED.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13ID.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13ID.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13ID.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13ID.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AB13MD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AB13MD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AG08BD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AG08BD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AG08BD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AG08BD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AG08BZ.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AG08BZ.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/AG08BZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/AG08BZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BB01AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BB01AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BB03AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BB03AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/BB04AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/BB04AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01QD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01QD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01RD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01RD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01SD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01SD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01TD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01TD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/FB01VD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/FB01VD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB01AD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB01AD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB01BD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB01BD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB01BD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB01BD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB01CD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB01CD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB03AD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB03AD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB03AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB03AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB03BD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB03BD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/IB03BD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/IB03BD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02CD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02CD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02DD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02DD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02ED.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02ED.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02HD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02HD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02ID.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02ID.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02JD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02JD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02JX.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02JX.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02JX.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02JX.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02KD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02KD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB02ND.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB02ND.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03BD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03BD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03BZ.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03BZ.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03BZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03BZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03FZ.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03FZ.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03FZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03FZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03KD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03KD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03LD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03LD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03LD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03LD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03LF.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03LF.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03LF.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03LF.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03LZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03LZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03QG.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03QG.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03RD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03RD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03TD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03TD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03TD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03TD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03UD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03UD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03VD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03VD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03WD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03WD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XP.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XP.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XP.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XP.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XZ.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XZ.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03XZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03XZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03ZD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03ZD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB03ZD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB03ZD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04AD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04AD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04AZ.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04AZ.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04AZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04AZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04BD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04BD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04BD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04BD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04BZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04BZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DL.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DL.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DP.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DP.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DS.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DS.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DS.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DS.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DZ.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DZ.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04DZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04DZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04ED.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04ED.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04ED.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04ED.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04FD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04FD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04FD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04FD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04PB.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04PB.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04PB.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04PB.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04PU.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04PU.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04PU.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04PU.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04TB.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04TB.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04TB.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04TB.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04TS.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04TS.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04TS.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04TS.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04VD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04VD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04XD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04XD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB04ZD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB04ZD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB05MD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB05MD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB05ND.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB05ND.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB4DLZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB4DLZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MB4DPZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MB4DPZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/MC03ND.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/MC03ND.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04OD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04OD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB04RD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB04RD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08CD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08CD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08CD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08CD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08DD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08DD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08DD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08DD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08ED.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08ED.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08ED.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08ED.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08FD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08FD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB08FD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB08FD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10DD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10DD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10DD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10DD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10ED.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10ED.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10ED.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10ED.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10FD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10FD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10FD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10FD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10HD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10HD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10HD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10HD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10ID.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10ID.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10KD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10KD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB10ZD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB10ZD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB16BD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB16BD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB16BD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB16BD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/SB16CD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/SB16CD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB04MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB04MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB05RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB05RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB07MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB07MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB07ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB07ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB08ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB08ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB08NW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB08NW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB08NZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB08NZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09GD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09GD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09JD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09JD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB09ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB09ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAB13MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAB13MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAG08BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAG08BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TAG08BZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TAG08BZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01ID.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01ID.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01ID.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01ID.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01IZ.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01IZ.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01IZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01IZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01KD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01KD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01KD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01KD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01LD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01LD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01LD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01LD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01MD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01MD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01PX.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01PX.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01TD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01TD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01UD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01UD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01UY.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01UY.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01WD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01WD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01WD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01WD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01WX.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01WX.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01WX.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01WX.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB01ZD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB01ZD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB03AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB03AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB04AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB04AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB04BD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB04BD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TB04CD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TB04CD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBB01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBB01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBB02AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBB02AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBB03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBB03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBB04AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBB04AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBD01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBD01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TBD02AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TBD02AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TC01OD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TC01OD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TC04AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TC04AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TD03AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TD03AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TD04AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TD04AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDE01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDE01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDE01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDE01PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDF01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDF01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDG01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDG01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDG01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDG01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDG01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDG01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TDK01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TDK01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TF01QD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TF01QD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFB01QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFB01QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFB01RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFB01RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFB01SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFB01SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFB01TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFB01TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFB01VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFB01VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TFD01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TFD01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01AD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01AD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01AD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01AD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01AZ.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01AZ.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01AZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01AZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01CD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01CD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01DD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01DD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01ED.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01ED.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01FD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01FD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01FZ.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01FZ.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01FZ.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01FZ.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01GD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01GD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01HD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01HD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01HD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01HD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01ID.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01ID.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01ID.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01ID.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01JD.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01JD.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01JD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01JD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01JY.dat` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01JY.dat`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01JY.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01JY.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01LD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01LD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01MD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01MD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01ND.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01ND.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01PD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01PD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TG01QD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TG01QD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TIB01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TIB01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TIB01BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TIB01BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TIB01CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TIB01CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TIB03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TIB03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TIB03BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TIB03BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB01TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB01TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02GD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02GD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02JD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02JD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02JX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02JX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB02VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB02VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03BZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03BZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03FZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03FZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03LD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03LD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03LF.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03LF.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03LZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03LZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03QG.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03QG.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03UD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03UD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03WD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03WD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03XD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03XD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03XP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03XP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03XZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03XZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB03ZD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB03ZD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04AZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04AZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04BZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04BZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DL.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DL.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04DZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04DZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04GD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04GD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04PB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04PB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04PU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04PU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04TB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04TB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04TS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04TS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04UD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04UD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04XD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04XD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04YD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04YD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB04ZD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB04ZD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB05MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB05MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB05ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB05ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB05OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB05OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB4DLZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB4DLZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMB4DPZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMB4DPZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01WD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01WD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC01XD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC01XD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC03MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC03MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMC03ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMC03ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMD03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMD03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TMD03BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TMD03BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB01BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB01BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB01DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB01DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB02SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB02SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB03UD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB03UD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB04RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB04RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB06ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB06ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB08ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB08ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB09MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB09MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB10ZD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB10ZD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB16AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB16AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB16BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB16BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSB16CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSB16CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSG02AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSG02AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSG02ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSG02ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSG03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSG03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TSG03BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TSG03BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01IZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01IZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01LD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01LD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01PX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01PX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01UD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01UD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01UY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01UY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01WD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01WD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01WX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01WX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB01ZD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB01ZD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB04AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB04AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB04BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB04BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB04CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB04CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTB05AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTB05AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTC01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTC01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTC04AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTC04AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTC05AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTC05AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTD03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTD03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTD04AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTD04AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTD05AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTD05AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTF01RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTF01RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01AZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01AZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01FZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01FZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01GD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01GD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01JD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01JD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01JY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01JY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01LD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01LD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TTG01QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TTG01QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TUD01BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TUD01BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TUD01CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TUD01CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TUD01DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TUD01DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TUD01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TUD01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/TUD01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/TUD01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01BD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01BD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01CD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01CD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01DD.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01DD.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/UD01ND.res` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/UD01ND.res`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/makefile` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 ####################################################################
 #  SLICOT examples makefile                                        #
 #  Makefile for generating and running SLICOT Library example      # 
 #  programs on Windows platforms.                                  #
-#  SLICOT, Release 4.0                 .\slicot\examples\makefile  #
-#  Vasile Sima, KU Leuven                                          #
+#  SLICOT, Release 5.8                 .\slicot\examples\makefile  #
+#  Vasile Sima                                                     #
 #  October 31, 1996.                                               #
 #  Revised December 23, 1999, ..., Oct. 4, 2001, Jan. 8 2009,      #
 #          Nov. 17, 2010, Sep. 25, 2012, Nov. 30, 2012.            #
-#          June 8, 2015, Jan. 2017.                                #
+#          June 8, 2015, Jan. 2017, Dec. 2022.                     #
 ####################################################################
 #
 #  This makefile compiles, links, and runs the example programs for 
 #  the SLICOT Library on Windows platforms.
 #
-#  The example programs can be executed for double precision only.
+#  Most example programs are written for double precision.
+#  Some example programs have COMPLEX*16 variants.
 #  To compile, link, and run the example programs, enter 'nmake'.
 #  The executable files are created in the current directory level.
 #  The files with the results have the extension .exa, and are also
 #  created in the current directory level, so they can automatically be
 #  compared with the .res files provided in this directory. Note that, 
 #  for some programs, the signs of some matrix elements could differ;
-#  this does not mean erroneous results.
+#  this does not mean erroneous results. Even the values can differ
+#  for some compilers, when rows and/or columns of the matrix results
+#  appear in a different order.
 #
 #  To remove the .exa files after the programs have been run, enter
 #       nmake clean
 #
 #  To remove the .exa files, as well as the executable programs, enter
 #       nmake cleanup
 #
@@ -32,56 +35,55 @@
 
 !include <..\make.inc>
 
 .SUFFIXES: .f .obj .exe .lib
 
 all: AB01MD.exa AB01ND.exa AB01OD.exa AB04MD.exa AB05MD.exa AB05ND.exa \
      AB05OD.exa AB05PD.exa AB05QD.exa AB05RD.exa AB07MD.exa AB07ND.exa \
-     AB08ND.exa AB09AD.exa AB09BD.exa AB09CD.exa AB09DD.exa AB09ED.exa \
-     AB09FD.exa AB09GD.exa AB09HD.exa AB09ID.exa AB09JD.exa AB09KD.exa \
-     AB09MD.exa AB09ND.exa AB13AD.exa AB13BD.exa AB13CD.exa AB13DD.exa \
-     AB13ED.exa AB13FD.exa AB13ID.exa AB13MD.exa AG08BD.exa \
+     AB08ND.exa AB08NW.exa AB08NZ.exa AB09AD.exa AB09BD.exa AB09CD.exa \
+     AB09DD.exa AB09ED.exa AB09FD.exa AB09GD.exa AB09HD.exa AB09ID.exa \
+     AB09JD.exa AB09KD.exa AB09MD.exa AB09ND.exa AB13AD.exa AB13BD.exa \
+     AB13CD.exa AB13DD.exa AB13ED.exa AB13FD.exa AB13ID.exa AB13MD.exa \
+     AG08BD.exa AG08BZ.exa \
      BB01AD.exa BB02AD.exa BB03AD.exa BB04AD.exa BD01AD.exa BD02AD.exa \
      DE01OD.exa DE01PD.exa DF01MD.exa DG01MD.exa DG01ND.exa DG01OD.exa \
      DK01MD.exa \
      FB01QD.exa FB01RD.exa FB01SD.exa FB01TD.exa FB01VD.exa FD01AD.exa \
      IB01AD.exa IB01BD.exa IB01CD.exa IB03AD.exa IB03BD.exa \
      MB01TD.exa MB02CD.exa MB02DD.exa MB02ED.exa MB02FD.exa MB02GD.exa \
      MB02HD.exa MB02ID.exa MB02JD.exa MB02JX.exa MB02KD.exa MB02MD.exa \
-     MB02ND.exa MB02QD.exa MB02SD.exa MB02VD.exa MB03MD.exa MB03ND.exa \
-     MB03OD.exa MB03PD.exa MB03QD.exa MB03RD.exa MB03SD.exa MB03UD.exa \
-     MB03VD.exa MB03WD.exa MB04DY.exa MB04GD.exa MB04MD.exa MB04OD.exa \
+     MB02ND.exa MB02QD.exa MB02SD.exa MB02VD.exa MB03BD.exa MB03BZ.exa \
+     MB03FZ.exa MB03KD.exa MB03LD.exa MB03LF.exa MB03LZ.exa MB03MD.exa \
+     MB03ND.exa MB03OD.exa MB03PD.exa MB03QD.exa MB03QG.exa MB03RD.exa \
+     MB03SD.exa MB03TD.exa MB03UD.exa MB03VD.exa MB03WD.exa MB03XD.exa \
+     MB03XP.exa MB03XZ.exa MB03ZD.exa MB04AD.exa MB04AZ.exa MB04BD.exa \
+     MB04BZ.exa MB04DD.exa MB04DL.exa MB4DLZ.exa MB04DP.exa MB4DPZ.exa \
+     MB04DS.exa MB04DY.exa MB04DZ.exa MB04ED.exa MB04FD.exa MB04GD.exa \
+     MB04MD.exa MB04OD.exa MB04PB.exa MB04PU.exa MB04TB.exa MB04TS.exa \
      MB04UD.exa MB04VD.exa MB04XD.exa MB04YD.exa MB04ZD.exa MB05MD.exa \
      MB05ND.exa MB05OD.exa MC01MD.exa MC01ND.exa MC01OD.exa MC01PD.exa \
      MC01QD.exa MC01RD.exa MC01SD.exa MC01TD.exa MC01VD.exa MC01WD.exa \
-     MC03MD.exa MC03ND.exa \
-     MD03AD.exa MD03BD.exa \
+     MC01XD.exa MC03MD.exa MC03ND.exa MD03AD.exa MD03BD.exa \
      SB01BD.exa SB01DD.exa SB01MD.exa SB02MD.exa SB02ND.exa SB02OD.exa \
      SB02PD.exa SB02QD.exa SB02RD.exa SB02SD.exa SB03MD.exa SB03OD.exa \
      SB03QD.exa SB03SD.exa SB03TD.exa SB03UD.exa SB04MD.exa SB04ND.exa \
      SB04OD.exa SB04PD.exa SB04QD.exa SB04RD.exa SB06ND.exa SB08CD.exa \
      SB08DD.exa SB08ED.exa SB08FD.exa SB08MD.exa SB08ND.exa SB09MD.exa \
      SB10DD.exa SB10ED.exa SB10FD.exa SB10HD.exa SB10ID.exa SB10KD.exa \
-     SB10ZD.exa SB16AD.exa SB16BD.exa SB16CD.exa SG02AD.exa SG03AD.exa \
-     SG03BD.exa TB01ID.exa TB01KD.exa TB01LD.exa TB01MD.exa TB01ND.exa \
-     TB01PD.exa TB01TD.exa TB01UD.exa TB01WD.exa TB01ZD.exa TB03AD.exa \
-     TB04AD.exa TB04BD.exa TB04CD.exa TB05AD.exa TC01OD.exa TC04AD.exa \
-     TC05AD.exa TD03AD.exa TD04AD.exa TD05AD.exa TF01MD.exa TF01ND.exa \
-     TF01OD.exa TF01PD.exa TF01QD.exa TF01RD.exa TG01AD.exa TG01CD.exa \
-     TG01DD.exa TG01ED.exa TG01FD.exa TG01HD.exa TG01ID.exa TG01JD.exa \
-     TG01JY.exa UD01BD.exa UD01CD.exa UD01DD.exa UD01MD.exa UD01ND.exa \
-     MB03TD.exa MB03XD.exa MB03XP.exa MB03ZD.exa MB04DD.exa MB04DP.exa \
-     MB4DPZ.exa MB04DL.exa MB4DLZ.exa MB04DS.exa MB04PB.exa MB04PU.exa \
-     MB04TB.exa MB04TS.exa AB08NZ.exa AG08BZ.exa TB01IZ.exa TG01AZ.exa \
-     TG01FZ.exa MB03BD.exa MB03KD.exa MB03LD.exa MB04AD.exa MB04BD.exa \
-     MB03BZ.exa MB03FZ.exa MB03LF.exa MB03LZ.exa MB03XZ.exa \
-     MB04AZ.exa MB04BZ.exa MB04DZ.exa MB04ED.exa MB04FD.exa \
-     MC01XD.exa SG02ND.exa \
-     AB08NW.exa MB03QG.exa TB01PX.exa TB01UY.exa TB01WX.exa TG01GD.exa \
-     TG01LD.exa TG01MD.exa TG01ND.exa TG01PD.exa TG01QD.exa
+     SB10ZD.exa SB16AD.exa SB16BD.exa SB16CD.exa SG02AD.exa SG02ND.exa \
+     SG03AD.exa SG03BD.exa \
+     TB01ID.exa TB01IZ.exa TB01KD.exa TB01LD.exa TB01MD.exa TB01ND.exa \
+     TB01PD.exa TB01PX.exa TB01TD.exa TB01UD.exa TB01UY.exa TB01WD.exa \
+     TB01WX.exa TB01ZD.exa TB03AD.exa TB04AD.exa TB04BD.exa TB04CD.exa \
+     TB05AD.exa TC01OD.exa TC04AD.exa TC05AD.exa TD03AD.exa TD04AD.exa \
+     TD05AD.exa TF01MD.exa TF01ND.exa TF01OD.exa TF01PD.exa TF01QD.exa \
+     TF01RD.exa TG01AD.exa TG01AZ.exa TG01CD.exa TG01DD.exa TG01ED.exa \
+     TG01FD.exa TG01FZ.exa TG01GD.exa TG01HD.exa TG01ID.exa TG01JD.exa \
+     TG01JY.exa TG01LD.exa TG01MD.exa TG01ND.exa TG01PD.exa TG01QD.exa \
+     UD01BD.exa UD01CD.exa UD01DD.exa UD01MD.exa UD01ND.exa
 
 AB01MD.exa: AB01MD.dat TAB01MD.exe;  TAB01MD <AB01MD.dat >AB01MD.exa
 AB01ND.exa: AB01ND.dat TAB01ND.exe;  TAB01ND <AB01ND.dat >AB01ND.exa
 AB01OD.exa: AB01OD.dat TAB01OD.exe;  TAB01OD <AB01OD.dat >AB01OD.exa
 AB04MD.exa: AB04MD.dat TAB04MD.exe;  TAB04MD <AB04MD.dat >AB04MD.exa
 AB05MD.exa: AB05MD.dat TAB05MD.exe;  TAB05MD <AB05MD.dat >AB05MD.exa
 AB05ND.exa: AB05ND.dat TAB05ND.exe;  TAB05ND <AB05ND.dat >AB05ND.exa
@@ -89,14 +91,15 @@
 AB05PD.exa: AB05PD.dat TAB05PD.exe;  TAB05PD <AB05PD.dat >AB05PD.exa
 AB05QD.exa: AB05QD.dat TAB05QD.exe;  TAB05QD <AB05QD.dat >AB05QD.exa
 AB05RD.exa: AB05RD.dat TAB05RD.exe;  TAB05RD <AB05RD.dat >AB05RD.exa
 AB07MD.exa: AB07MD.dat TAB07MD.exe;  TAB07MD <AB07MD.dat >AB07MD.exa
 AB07ND.exa: AB07ND.dat TAB07ND.exe;  TAB07ND <AB07ND.dat >AB07ND.exa
 AB08ND.exa: AB08ND.dat TAB08ND.exe;  TAB08ND <AB08ND.dat >AB08ND.exa
 AB08NW.exa: AB08NW.dat TAB08NW.exe;  TAB08NW <AB08NW.dat >AB08NW.exa
+AB08NZ.exa: AB08NZ.dat TAB08NZ.exe;  TAB08NZ <AB08NZ.dat >AB08NZ.exa
 AB09AD.exa: AB09AD.dat TAB09AD.exe;  TAB09AD <AB09AD.dat >AB09AD.exa
 AB09BD.exa: AB09BD.dat TAB09BD.exe;  TAB09BD <AB09BD.dat >AB09BD.exa
 AB09CD.exa: AB09CD.dat TAB09CD.exe;  TAB09CD <AB09CD.dat >AB09CD.exa
 AB09DD.exa: AB09DD.dat TAB09DD.exe;  TAB09DD <AB09DD.dat >AB09DD.exa
 AB09ED.exa: AB09ED.dat TAB09ED.exe;  TAB09ED <AB09ED.dat >AB09ED.exa
 AB09FD.exa: AB09FD.dat TAB09FD.exe;  TAB09FD <AB09FD.dat >AB09FD.exa
 AB09GD.exa: AB09GD.dat TAB09GD.exe;  TAB09GD <AB09GD.dat >AB09GD.exa
@@ -111,26 +114,27 @@
 AB13CD.exa: AB13CD.dat TAB13CD.exe;  TAB13CD <AB13CD.dat >AB13CD.exa
 AB13DD.exa: AB13DD.dat TAB13DD.exe;  TAB13DD <AB13DD.dat >AB13DD.exa
 AB13ED.exa: AB13ED.dat TAB13ED.exe;  TAB13ED <AB13ED.dat >AB13ED.exa
 AB13FD.exa: AB13FD.dat TAB13FD.exe;  TAB13FD <AB13FD.dat >AB13FD.exa
 AB13ID.exa: AB13ID.dat TAB13ID.exe;  TAB13ID <AB13ID.dat >AB13ID.exa
 AB13MD.exa: AB13MD.dat TAB13MD.exe;  TAB13MD <AB13MD.dat >AB13MD.exa
 AG08BD.exa: AG08BD.dat TAG08BD.exe;  TAG08BD <AG08BD.dat >AG08BD.exa
+AG08BZ.exa: AG08BZ.dat TAG08BZ.exe;  TAG08BZ <AG08BZ.dat >AG08BZ.exa
 BB01AD.exa: BB01AD.dat TBB01AD.exe;  TBB01AD <BB01AD.dat >BB01AD.exa
 BB02AD.exa: BB02AD.dat TBB02AD.exe;  TBB02AD <BB02AD.dat >BB02AD.exa
 BB03AD.exa: BB03AD.dat TBB03AD.exe;  TBB03AD <BB03AD.dat >BB03AD.exa
 BB04AD.exa: BB04AD.dat TBB04AD.exe;  TBB04AD <BB04AD.dat >BB04AD.exa
 BD01AD.exa: BD01AD.dat TBD01AD.exe;  TBD01AD <BD01AD.dat >BD01AD.exa
 BD02AD.exa: BD02AD.dat TBD02AD.exe;  TBD02AD <BD02AD.dat >BD02AD.exa
 DE01OD.exa: DE01OD.dat TDE01OD.exe;  TDE01OD <DE01OD.dat >DE01OD.exa
 DE01PD.exa: DE01PD.dat TDE01PD.exe;  TDE01PD <DE01PD.dat >DE01PD.exa
-DG01OD.exa: DG01OD.dat TDG01OD.exe;  TDG01OD <DG01OD.dat >DG01OD.exa
 DF01MD.exa: DF01MD.dat TDF01MD.exe;  TDF01MD <DF01MD.dat >DF01MD.exa
 DG01MD.exa: DG01MD.dat TDG01MD.exe;  TDG01MD <DG01MD.dat >DG01MD.exa
 DG01ND.exa: DG01ND.dat TDG01ND.exe;  TDG01ND <DG01ND.dat >DG01ND.exa
+DG01OD.exa: DG01OD.dat TDG01OD.exe;  TDG01OD <DG01OD.dat >DG01OD.exa
 DK01MD.exa: DK01MD.dat TDK01MD.exe;  TDK01MD <DK01MD.dat >DK01MD.exa
 FB01QD.exa: FB01QD.dat TFB01QD.exe;  TFB01QD <FB01QD.dat >FB01QD.exa
 FB01RD.exa: FB01RD.dat TFB01RD.exe;  TFB01RD <FB01RD.dat >FB01RD.exa
 FB01SD.exa: FB01SD.dat TFB01SD.exe;  TFB01SD <FB01SD.dat >FB01SD.exa
 FB01TD.exa: FB01TD.dat TFB01TD.exe;  TFB01TD <FB01TD.dat >FB01TD.exa
 FB01VD.exa: FB01VD.dat TFB01VD.exe;  TFB01VD <FB01VD.dat >FB01VD.exa
 FD01AD.exa: FD01AD.dat TFD01AD.exe;  TFD01AD <FD01AD.dat >FD01AD.exa
@@ -151,28 +155,58 @@
 MB02JX.exa: MB02JX.dat TMB02JX.exe;  TMB02JX <MB02JX.dat >MB02JX.exa
 MB02KD.exa: MB02KD.dat TMB02KD.exe;  TMB02KD <MB02KD.dat >MB02KD.exa
 MB02MD.exa: MB02MD.dat TMB02MD.exe;  TMB02MD <MB02MD.dat >MB02MD.exa
 MB02ND.exa: MB02ND.dat TMB02ND.exe;  TMB02ND <MB02ND.dat >MB02ND.exa
 MB02QD.exa: MB02QD.dat TMB02QD.exe;  TMB02QD <MB02QD.dat >MB02QD.exa
 MB02SD.exa: MB02SD.dat TMB02SD.exe;  TMB02SD <MB02SD.dat >MB02SD.exa
 MB02VD.exa: MB02VD.dat TMB02VD.exe;  TMB02VD <MB02VD.dat >MB02VD.exa
+MB03BD.exa: MB03BD.dat TMB03BD.exe;  TMB03BD <MB03BD.dat >MB03BD.exa
+MB03BZ.exa: MB03BZ.dat TMB03BZ.exe;  TMB03BZ <MB03BZ.dat >MB03BZ.exa
+MB03FZ.exa: MB03FZ.dat TMB03FZ.exe;  TMB03FZ <MB03FZ.dat >MB03FZ.exa
+MB03KD.exa: MB03KD.dat TMB03KD.exe;  TMB03KD <MB03KD.dat >MB03KD.exa
+MB03LD.exa: MB03LD.dat TMB03LD.exe;  TMB03LD <MB03LD.dat >MB03LD.exa
+MB03LF.exa: MB03LF.dat TMB03LF.exe;  TMB03LF <MB03LF.dat >MB03LF.exa
+MB03LZ.exa: MB03LZ.dat TMB03LZ.exe;  TMB03LZ <MB03LZ.dat >MB03LZ.exa
 MB03MD.exa: MB03MD.dat TMB03MD.exe;  TMB03MD <MB03MD.dat >MB03MD.exa
 MB03ND.exa: MB03ND.dat TMB03ND.exe;  TMB03ND <MB03ND.dat >MB03ND.exa
 MB03OD.exa: MB03OD.dat TMB03OD.exe;  TMB03OD <MB03OD.dat >MB03OD.exa
 MB03PD.exa: MB03PD.dat TMB03PD.exe;  TMB03PD <MB03PD.dat >MB03PD.exa
 MB03QD.exa: MB03QD.dat TMB03QD.exe;  TMB03QD <MB03QD.dat >MB03QD.exa
+MB03QG.exa: MB03QG.dat TMB03QG.exe;  TMB03QG <MB03QG.dat >MB03QG.exa
 MB03RD.exa: MB03RD.dat TMB03RD.exe;  TMB03RD <MB03RD.dat >MB03RD.exa
 MB03SD.exa: MB03SD.dat TMB03SD.exe;  TMB03SD <MB03SD.dat >MB03SD.exa
+MB03TD.exa: MB03TD.dat TMB03TD.exe;  TMB03TD <MB03TD.dat >MB03TD.exa
 MB03UD.exa: MB03UD.dat TMB03UD.exe;  TMB03UD <MB03UD.dat >MB03UD.exa
 MB03VD.exa: MB03VD.dat TMB03VD.exe;  TMB03VD <MB03VD.dat >MB03VD.exa
 MB03WD.exa: MB03WD.dat TMB03WD.exe;  TMB03WD <MB03WD.dat >MB03WD.exa
+MB03XD.exa: MB03XD.dat TMB03XD.exe;  TMB03XD <MB03XD.dat >MB03XD.exa
+MB03XP.exa: MB03XP.dat TMB03XP.exe;  TMB03XP <MB03XP.dat >MB03XP.exa
+MB03XZ.exa: MB03XZ.dat TMB03XZ.exe;  TMB03XZ <MB03XZ.dat >MB03XZ.exa
+MB03ZD.exa: MB03ZD.dat TMB03ZD.exe;  TMB03ZD <MB03ZD.dat >MB03ZD.exa
+MB04AD.exa: MB04AD.dat TMB04AD.exe;  TMB04AD <MB04AD.dat >MB04AD.exa
+MB04AZ.exa: MB04AZ.dat TMB04AZ.exe;  TMB04AZ <MB04AZ.dat >MB04AZ.exa
+MB04BD.exa: MB04BD.dat TMB04BD.exe;  TMB04BD <MB04BD.dat >MB04BD.exa
+MB04BZ.exa: MB04BZ.dat TMB04BZ.exe;  TMB04BZ <MB04BZ.dat >MB04BZ.exa
+MB04DD.exa: MB04DD.dat TMB04DD.exe;  TMB04DD <MB04DD.dat >MB04DD.exa
+MB04DL.exa: MB04DL.dat TMB04DL.exe;  TMB04DL <MB04DL.dat >MB04DL.exa
+MB4DLZ.exa: MB4DLZ.dat TMB4DLZ.exe;  TMB4DLZ <MB4DLZ.dat >MB4DLZ.exa
+MB04DP.exa: MB04DP.dat TMB04DP.exe;  TMB04DP <MB04DP.dat >MB04DP.exa
+MB4DPZ.exa: MB4DPZ.dat TMB4DPZ.exe;  TMB4DPZ <MB4DPZ.dat >MB4DPZ.exa
+MB04DS.exa: MB04DS.dat TMB04DS.exe;  TMB04DS <MB04DS.dat >MB04DS.exa
 MB04DY.exa: MB04DY.dat TMB04DY.exe;  TMB04DY <MB04DY.dat >MB04DY.exa
+MB04DZ.exa: MB04DZ.dat TMB04DZ.exe;  TMB04DZ <MB04DZ.dat >MB04DZ.exa
+MB04ED.exa: MB04ED.dat TMB04ED.exe;  TMB04ED <MB04ED.dat >MB04ED.exa
+MB04FD.exa: MB04FD.dat TMB04FD.exe;  TMB04FD <MB04FD.dat >MB04FD.exa
 MB04GD.exa: MB04GD.dat TMB04GD.exe;  TMB04GD <MB04GD.dat >MB04GD.exa
 MB04MD.exa: MB04MD.dat TMB04MD.exe;  TMB04MD <MB04MD.dat >MB04MD.exa
 MB04OD.exa: MB04OD.dat TMB04OD.exe;  TMB04OD <MB04OD.dat >MB04OD.exa
+MB04PB.exa: MB04PB.dat TMB04PB.exe;  TMB04PB <MB04PB.dat >MB04PB.exa
+MB04PU.exa: MB04PU.dat TMB04PU.exe;  TMB04PU <MB04PU.dat >MB04PU.exa
+MB04TB.exa: MB04TB.dat TMB04TB.exe;  TMB04TB <MB04TB.dat >MB04TB.exa
+MB04TS.exa: MB04TS.dat TMB04TS.exe;  TMB04TS <MB04TS.dat >MB04TS.exa
 MB04UD.exa: MB04UD.dat TMB04UD.exe;  TMB04UD <MB04UD.dat >MB04UD.exa
 MB04VD.exa: MB04VD.dat TMB04VD.exe;  TMB04VD <MB04VD.dat >MB04VD.exa
 MB04XD.exa: MB04XD.dat TMB04XD.exe;  TMB04XD <MB04XD.dat >MB04XD.exa
 MB04YD.exa: MB04YD.dat TMB04YD.exe;  TMB04YD <MB04YD.dat >MB04YD.exa
 MB04ZD.exa: MB04ZD.dat TMB04ZD.exe;  TMB04ZD <MB04ZD.dat >MB04ZD.exa
 MB05MD.exa: MB05MD.dat TMB05MD.exe;  TMB05MD <MB05MD.dat >MB05MD.exa
 MB05ND.exa: MB05ND.dat TMB05ND.exe;  TMB05ND <MB05ND.dat >MB05ND.exa
@@ -183,14 +217,15 @@
 MC01PD.exa: MC01PD.dat TMC01PD.exe;  TMC01PD <MC01PD.dat >MC01PD.exa
 MC01QD.exa: MC01QD.dat TMC01QD.exe;  TMC01QD <MC01QD.dat >MC01QD.exa
 MC01RD.exa: MC01RD.dat TMC01RD.exe;  TMC01RD <MC01RD.dat >MC01RD.exa
 MC01SD.exa: MC01SD.dat TMC01SD.exe;  TMC01SD <MC01SD.dat >MC01SD.exa
 MC01TD.exa: MC01TD.dat TMC01TD.exe;  TMC01TD <MC01TD.dat >MC01TD.exa
 MC01VD.exa: MC01VD.dat TMC01VD.exe;  TMC01VD <MC01VD.dat >MC01VD.exa
 MC01WD.exa: MC01WD.dat TMC01WD.exe;  TMC01WD <MC01WD.dat >MC01WD.exa
+MC01XD.exa: MC01XD.dat TMC01XD.exe;  TMC01XD <MC01XD.dat >MC01XD.exa
 MC03MD.exa: MC03MD.dat TMC03MD.exe;  TMC03MD <MC03MD.dat >MC03MD.exa
 MC03ND.exa: MC03ND.dat TMC03ND.exe;  TMC03ND <MC03ND.dat >MC03ND.exa
 MD03AD.exa: MD03AD.dat TMD03AD.exe;  TMD03AD <MD03AD.dat >MD03AD.exa
 MD03BD.exa: MD03BD.dat TMD03BD.exe;  TMD03BD <MD03BD.dat >MD03BD.exa
 SB01BD.exa: SB01BD.dat TSB01BD.exe;  TSB01BD <SB01BD.dat >SB01BD.exa
 SB01DD.exa: SB01DD.dat TSB01DD.exe;  TSB01DD <SB01DD.dat >SB01DD.exa
 SB01MD.exa: SB01MD.dat TSB01MD.exe;  TSB01MD <SB01MD.dat >SB01MD.exa
@@ -228,25 +263,30 @@
 SB10ID.exa: SB10ID.dat TSB10ID.exe;  TSB10ID <SB10ID.dat >SB10ID.exa
 SB10KD.exa: SB10KD.dat TSB10KD.exe;  TSB10KD <SB10KD.dat >SB10KD.exa
 SB10ZD.exa: SB10ZD.dat TSB10ZD.exe;  TSB10ZD <SB10ZD.dat >SB10ZD.exa
 SB16AD.exa: SB16AD.dat TSB16AD.exe;  TSB16AD <SB16AD.dat >SB16AD.exa
 SB16BD.exa: SB16BD.dat TSB16BD.exe;  TSB16BD <SB16BD.dat >SB16BD.exa
 SB16CD.exa: SB16CD.dat TSB16CD.exe;  TSB16CD <SB16CD.dat >SB16CD.exa
 SG02AD.exa: SG02AD.dat TSG02AD.exe;  TSG02AD <SG02AD.dat >SG02AD.exa
+SG02ND.exa: SG02ND.dat TSG02ND.exe;  TSG02ND <SG02ND.dat >SG02ND.exa
 SG03AD.exa: SG03AD.dat TSG03AD.exe;  TSG03AD <SG03AD.dat >SG03AD.exa
 SG03BD.exa: SG03BD.dat TSG03BD.exe;  TSG03BD <SG03BD.dat >SG03BD.exa
 TB01ID.exa: TB01ID.dat TTB01ID.exe;  TTB01ID <TB01ID.dat >TB01ID.exa
+TB01IZ.exa: TB01IZ.dat TTB01IZ.exe;  TTB01IZ <TB01IZ.dat >TB01IZ.exa
 TB01KD.exa: TB01KD.dat TTB01KD.exe;  TTB01KD <TB01KD.dat >TB01KD.exa
 TB01LD.exa: TB01LD.dat TTB01LD.exe;  TTB01LD <TB01LD.dat >TB01LD.exa
 TB01MD.exa: TB01MD.dat TTB01MD.exe;  TTB01MD <TB01MD.dat >TB01MD.exa
 TB01ND.exa: TB01ND.dat TTB01ND.exe;  TTB01ND <TB01ND.dat >TB01ND.exa
 TB01PD.exa: TB01PD.dat TTB01PD.exe;  TTB01PD <TB01PD.dat >TB01PD.exa
+TB01PX.exa: TB01PX.dat TTB01PX.exe;  TTB01PX <TB01PX.dat >TB01PX.exa
 TB01TD.exa: TB01TD.dat TTB01TD.exe;  TTB01TD <TB01TD.dat >TB01TD.exa
 TB01UD.exa: TB01UD.dat TTB01UD.exe;  TTB01UD <TB01UD.dat >TB01UD.exa
+TB01UY.exa: TB01UY.dat TTB01UY.exe;  TTB01UY <TB01UY.dat >TB01UY.exa
 TB01WD.exa: TB01WD.dat TTB01WD.exe;  TTB01WD <TB01WD.dat >TB01WD.exa
+TB01WX.exa: TB01WX.dat TTB01WX.exe;  TTB01WX <TB01WX.dat >TB01WX.exa
 TB01ZD.exa: TB01ZD.dat TTB01ZD.exe;  TTB01ZD <TB01ZD.dat >TB01ZD.exa
 TB03AD.exa: TB03AD.dat TTB03AD.exe;  TTB03AD <TB03AD.dat >TB03AD.exa
 TB04AD.exa: TB04AD.dat TTB04AD.exe;  TTB04AD <TB04AD.dat >TB04AD.exa
 TB04BD.exa: TB04BD.dat TTB04BD.exe;  TTB04BD <TB04BD.dat >TB04BD.exa
 TB04CD.exa: TB04CD.dat TTB04CD.exe;  TTB04CD <TB04CD.dat >TB04CD.exa
 TB05AD.exa: TB05AD.dat TTB05AD.exe;  TTB05AD <TB05AD.dat >TB05AD.exa
 TC01OD.exa: TC01OD.dat TTC01OD.exe;  TTC01OD <TC01OD.dat >TC01OD.exa
@@ -258,73 +298,35 @@
 TF01MD.exa: TF01MD.dat TTF01MD.exe;  TTF01MD <TF01MD.dat >TF01MD.exa
 TF01ND.exa: TF01ND.dat TTF01ND.exe;  TTF01ND <TF01ND.dat >TF01ND.exa
 TF01OD.exa: TF01OD.dat TTF01OD.exe;  TTF01OD <TF01OD.dat >TF01OD.exa
 TF01PD.exa: TF01PD.dat TTF01PD.exe;  TTF01PD <TF01PD.dat >TF01PD.exa
 TF01QD.exa: TF01QD.dat TTF01QD.exe;  TTF01QD <TF01QD.dat >TF01QD.exa
 TF01RD.exa: TF01RD.dat TTF01RD.exe;  TTF01RD <TF01RD.dat >TF01RD.exa
 TG01AD.exa: TG01AD.dat TTG01AD.exe;  TTG01AD <TG01AD.dat >TG01AD.exa
+TG01AZ.exa: TG01AZ.dat TTG01AZ.exe;  TTG01AZ <TG01AZ.dat >TG01AZ.exa
 TG01CD.exa: TG01CD.dat TTG01CD.exe;  TTG01CD <TG01CD.dat >TG01CD.exa
 TG01DD.exa: TG01DD.dat TTG01DD.exe;  TTG01DD <TG01DD.dat >TG01DD.exa
 TG01ED.exa: TG01ED.dat TTG01ED.exe;  TTG01ED <TG01ED.dat >TG01ED.exa
 TG01FD.exa: TG01FD.dat TTG01FD.exe;  TTG01FD <TG01FD.dat >TG01FD.exa
+TG01FZ.exa: TG01FZ.dat TTG01FZ.exe;  TTG01FZ <TG01FZ.dat >TG01FZ.exa
+TG01GD.exa: TG01GD.dat TTG01GD.exe;  TTG01GD <TG01GD.dat >TG01GD.exa
 TG01HD.exa: TG01HD.dat TTG01HD.exe;  TTG01HD <TG01HD.dat >TG01HD.exa
 TG01ID.exa: TG01ID.dat TTG01ID.exe;  TTG01ID <TG01ID.dat >TG01ID.exa
 TG01JD.exa: TG01JD.dat TTG01JD.exe;  TTG01JD <TG01JD.dat >TG01JD.exa
 TG01JY.exa: TG01JY.dat TTG01JY.exe;  TTG01JY <TG01JY.dat >TG01JY.exa
-UD01BD.exa: UD01BD.dat TUD01BD.exe;  TUD01BD <UD01BD.dat >UD01BD.exa
-UD01CD.exa: UD01CD.dat TUD01CD.exe;  TUD01CD <UD01CD.dat >UD01CD.exa
-UD01DD.exa: UD01DD.dat TUD01DD.exe;  TUD01DD <UD01DD.dat >UD01DD.exa
-UD01MD.exa: UD01MD.dat TUD01MD.exe;  TUD01MD <UD01MD.dat >UD01MD.exa
-UD01ND.exa: UD01ND.dat TUD01ND.exe;  TUD01ND <UD01ND.dat >UD01ND.exa
-MB03TD.exa: MB03TD.dat TMB03TD.exe;  TMB03TD <MB03TD.dat >MB03TD.exa
-MB03XD.exa: MB03XD.dat TMB03XD.exe;  TMB03XD <MB03XD.dat >MB03XD.exa
-MB03XP.exa: MB03XP.dat TMB03XP.exe;  TMB03XP <MB03XP.dat >MB03XP.exa
-MB03ZD.exa: MB03ZD.dat TMB03ZD.exe;  TMB03ZD <MB03ZD.dat >MB03ZD.exa
-MB04DD.exa: MB04DD.dat TMB04DD.exe;  TMB04DD <MB04DD.dat >MB04DD.exa
-MB04DP.exa: MB04DP.dat TMB04DP.exe;  TMB04DP <MB04DP.dat >MB04DP.exa
-MB4DPZ.exa: MB4DPZ.dat TMB4DPZ.exe;  TMB4DPZ <MB4DPZ.dat >MB4DPZ.exa
-MB04DL.exa: MB04DL.dat TMB04DL.exe;  TMB04DL <MB04DL.dat >MB04DL.exa
-MB4DLZ.exa: MB4DLZ.dat TMB4DLZ.exe;  TMB4DLZ <MB4DLZ.dat >MB4DLZ.exa
-MB04DS.exa: MB04DS.dat TMB04DS.exe;  TMB04DS <MB04DS.dat >MB04DS.exa
-MB04PB.exa: MB04PB.dat TMB04PB.exe;  TMB04PB <MB04PB.dat >MB04PB.exa
-MB04PU.exa: MB04PU.dat TMB04PU.exe;  TMB04PU <MB04PU.dat >MB04PU.exa
-MB04TB.exa: MB04TB.dat TMB04TB.exe;  TMB04TB <MB04TB.dat >MB04TB.exa
-MB04TS.exa: MB04TS.dat TMB04TS.exe;  TMB04TS <MB04TS.dat >MB04TS.exa
-AB08NZ.exa: AB08NZ.dat TAB08NZ.exe;  TAB08NZ <AB08NZ.dat >AB08NZ.exa
-AG08BZ.exa: AG08BZ.dat TAG08BZ.exe;  TAG08BZ <AG08BZ.dat >AG08BZ.exa
-TB01IZ.exa: TB01IZ.dat TTB01IZ.exe;  TTB01IZ <TB01IZ.dat >TB01IZ.exa
-TG01AZ.exa: TG01AZ.dat TTG01AZ.exe;  TTG01AZ <TG01AZ.dat >TG01AZ.exa
-TG01FZ.exa: TG01FZ.dat TTG01FZ.exe;  TTG01FZ <TG01FZ.dat >TG01FZ.exa
-MB03BD.exa: MB03BD.dat TMB03BD.exe;  TMB03BD <MB03BD.dat >MB03BD.exa
-MB03KD.exa: MB03KD.dat TMB03KD.exe;  TMB03KD <MB03KD.dat >MB03KD.exa
-MB03LD.exa: MB03LD.dat TMB03LD.exe;  TMB03LD <MB03LD.dat >MB03LD.exa
-MB04AD.exa: MB04AD.dat TMB04AD.exe;  TMB04AD <MB04AD.dat >MB04AD.exa
-MB04BD.exa: MB04BD.dat TMB04BD.exe;  TMB04BD <MB04BD.dat >MB04BD.exa
-MB03BZ.exa: MB03BZ.dat TMB03BZ.exe;  TMB03BZ <MB03BZ.dat >MB03BZ.exa
-MB03FZ.exa: MB03FZ.dat TMB03FZ.exe;  TMB03FZ <MB03FZ.dat >MB03FZ.exa
-MB03LF.exa: MB03LF.dat TMB03LF.exe;  TMB03LF <MB03LF.dat >MB03LF.exa
-MB03LZ.exa: MB03LZ.dat TMB03LZ.exe;  TMB03LZ <MB03LZ.dat >MB03LZ.exa
-MB03XZ.exa: MB03XZ.dat TMB03XZ.exe;  TMB03XZ <MB03XZ.dat >MB03XZ.exa
-MB04AZ.exa: MB04AZ.dat TMB04AZ.exe;  TMB04AZ <MB04AZ.dat >MB04AZ.exa
-MB04BZ.exa: MB04BZ.dat TMB04BZ.exe;  TMB04BZ <MB04BZ.dat >MB04BZ.exa
-MB04DZ.exa: MB04DZ.dat TMB04DZ.exe;  TMB04DZ <MB04DZ.dat >MB04DZ.exa
-MB04ED.exa: MB04ED.dat TMB04ED.exe;  TMB04ED <MB04ED.dat >MB04ED.exa
-MB04FD.exa: MB04FD.dat TMB04FD.exe;  TMB04FD <MB04FD.dat >MB04FD.exa
-MC01XD.exa: MC01XD.dat TMC01XD.exe;  TMC01XD <MC01XD.dat >MC01XD.exa
-SG02ND.exa: SG02ND.dat TSG02ND.exe;  TSG02ND <SG02ND.dat >SG02ND.exa
-MB03QG.exa: MB03QG.dat TMB03QG.exe;  TMB03QG <MB03QG.dat >MB03QG.exa
-TB01PX.exa: TB01PX.dat TTB01PX.exe;  TTB01PX <TB01PX.dat >TB01PX.exa
-TB01UY.exa: TB01UY.dat TTB01UY.exe;  TTB01UY <TB01UY.dat >TB01UY.exa
-TB01WX.exa: TB01WX.dat TTB01WX.exe;  TTB01WX <TB01WX.dat >TB01WX.exa
-TG01GD.exa: TG01GD.dat TTG01GD.exe;  TTG01GD <TG01GD.dat >TG01GD.exa
 TG01LD.exa: TG01LD.dat TTG01LD.exe;  TTG01LD <TG01LD.dat >TG01LD.exa
 TG01MD.exa: TG01MD.dat TTG01MD.exe;  TTG01MD <TG01MD.dat >TG01MD.exa
 TG01ND.exa: TG01ND.dat TTG01ND.exe;  TTG01ND <TG01ND.dat >TG01ND.exa
 TG01PD.exa: TG01PD.dat TTG01PD.exe;  TTG01PD <TG01PD.dat >TG01PD.exa
 TG01QD.exa: TG01QD.dat TTG01QD.exe;  TTG01QD <TG01QD.dat >TG01QD.exa
+UD01BD.exa: UD01BD.dat TUD01BD.exe;  TUD01BD <UD01BD.dat >UD01BD.exa
+UD01CD.exa: UD01CD.dat TUD01CD.exe;  TUD01CD <UD01CD.dat >UD01CD.exa
+UD01DD.exa: UD01DD.dat TUD01DD.exe;  TUD01DD <UD01DD.dat >UD01DD.exa
+UD01MD.exa: UD01MD.dat TUD01MD.exe;  TUD01MD <UD01MD.dat >UD01MD.exa
+UD01ND.exa: UD01ND.dat TUD01ND.exe;  TUD01ND <UD01ND.dat >UD01ND.exa
 
 TAB01MD.exe:  TAB01MD.obj ; $(LOADER) -exe:TAB01MD TAB01MD.obj $(LOADOPTS)
 TAB01ND.exe:  TAB01ND.obj ; $(LOADER) -exe:TAB01ND TAB01ND.obj $(LOADOPTS)
 TAB01OD.exe:  TAB01OD.obj ; $(LOADER) -exe:TAB01OD TAB01OD.obj $(LOADOPTS)
 TAB04MD.exe:  TAB04MD.obj ; $(LOADER) -exe:TAB04MD TAB04MD.obj $(LOADOPTS)
 TAB05MD.exe:  TAB05MD.obj ; $(LOADER) -exe:TAB05MD TAB05MD.obj $(LOADOPTS)
 TAB05ND.exe:  TAB05ND.obj ; $(LOADER) -exe:TAB05ND TAB05ND.obj $(LOADOPTS)
@@ -332,14 +334,15 @@
 TAB05PD.exe:  TAB05PD.obj ; $(LOADER) -exe:TAB05PD TAB05PD.obj $(LOADOPTS)
 TAB05QD.exe:  TAB05QD.obj ; $(LOADER) -exe:TAB05QD TAB05QD.obj $(LOADOPTS)
 TAB05RD.exe:  TAB05RD.obj ; $(LOADER) -exe:TAB05RD TAB05RD.obj $(LOADOPTS)
 TAB07MD.exe:  TAB07MD.obj ; $(LOADER) -exe:TAB07MD TAB07MD.obj $(LOADOPTS)
 TAB07ND.exe:  TAB07ND.obj ; $(LOADER) -exe:TAB07ND TAB07ND.obj $(LOADOPTS)
 TAB08ND.exe:  TAB08ND.obj ; $(LOADER) -exe:TAB08ND TAB08ND.obj $(LOADOPTS)
 TAB08NW.exe:  TAB08NW.obj ; $(LOADER) -exe:TAB08NW TAB08NW.obj $(LOADOPTS)
+TAB08NZ.exe:  TAB08NZ.obj ; $(LOADER) -exe:TAB08NZ TAB08NZ.obj $(LOADOPTS)
 TAB09AD.exe:  TAB09AD.obj ; $(LOADER) -exe:TAB09AD TAB09AD.obj $(LOADOPTS)
 TAB09BD.exe:  TAB09BD.obj ; $(LOADER) -exe:TAB09BD TAB09BD.obj $(LOADOPTS)
 TAB09CD.exe:  TAB09CD.obj ; $(LOADER) -exe:TAB09CD TAB09CD.obj $(LOADOPTS)
 TAB09DD.exe:  TAB09DD.obj ; $(LOADER) -exe:TAB09DD TAB09DD.obj $(LOADOPTS)
 TAB09ED.exe:  TAB09ED.obj ; $(LOADER) -exe:TAB09ED TAB09ED.obj $(LOADOPTS)
 TAB09FD.exe:  TAB09FD.obj ; $(LOADER) -exe:TAB09FD TAB09FD.obj $(LOADOPTS)
 TAB09GD.exe:  TAB09GD.obj ; $(LOADER) -exe:TAB09GD TAB09GD.obj $(LOADOPTS)
@@ -354,26 +357,27 @@
 TAB13CD.exe:  TAB13CD.obj ; $(LOADER) -exe:TAB13CD TAB13CD.obj $(LOADOPTS)
 TAB13DD.exe:  TAB13DD.obj ; $(LOADER) -exe:TAB13DD TAB13DD.obj $(LOADOPTS)
 TAB13ED.exe:  TAB13ED.obj ; $(LOADER) -exe:TAB13ED TAB13ED.obj $(LOADOPTS)
 TAB13FD.exe:  TAB13FD.obj ; $(LOADER) -exe:TAB13FD TAB13FD.obj $(LOADOPTS)
 TAB13ID.exe:  TAB13ID.obj ; $(LOADER) -exe:TAB13ID TAB13ID.obj $(LOADOPTS)
 TAB13MD.exe:  TAB13MD.obj ; $(LOADER) -exe:TAB13MD TAB13MD.obj $(LOADOPTS)
 TAG08BD.exe:  TAG08BD.obj ; $(LOADER) -exe:TAG08BD TAG08BD.obj $(LOADOPTS)
+TAG08BZ.exe:  TAG08BZ.obj ; $(LOADER) -exe:TAG08BZ TAG08BZ.obj $(LOADOPTS)
 TBB01AD.exe:  TBB01AD.obj ; $(LOADER) -exe:TBB01AD TBB01AD.obj $(LOADOPTS)
 TBB02AD.exe:  TBB02AD.obj ; $(LOADER) -exe:TBB02AD TBB02AD.obj $(LOADOPTS)
 TBB03AD.exe:  TBB03AD.obj ; $(LOADER) -exe:TBB03AD TBB03AD.obj $(LOADOPTS)
 TBB04AD.exe:  TBB04AD.obj ; $(LOADER) -exe:TBB04AD TBB04AD.obj $(LOADOPTS)
 TBD01AD.exe:  TBD01AD.obj ; $(LOADER) -exe:TBD01AD TBD01AD.obj $(LOADOPTS)
 TBD02AD.exe:  TBD02AD.obj ; $(LOADER) -exe:TBD02AD TBD02AD.obj $(LOADOPTS)
 TDE01OD.exe:  TDE01OD.obj ; $(LOADER) -exe:TDE01OD TDE01OD.obj $(LOADOPTS)
 TDE01PD.exe:  TDE01PD.obj ; $(LOADER) -exe:TDE01PD TDE01PD.obj $(LOADOPTS)
-TDG01OD.exe:  TDG01OD.obj ; $(LOADER) -exe:TDG01OD TDG01OD.obj $(LOADOPTS)
 TDF01MD.exe:  TDF01MD.obj ; $(LOADER) -exe:TDF01MD TDF01MD.obj $(LOADOPTS)
 TDG01MD.exe:  TDG01MD.obj ; $(LOADER) -exe:TDG01MD TDG01MD.obj $(LOADOPTS)
 TDG01ND.exe:  TDG01ND.obj ; $(LOADER) -exe:TDG01ND TDG01ND.obj $(LOADOPTS)
+TDG01OD.exe:  TDG01OD.obj ; $(LOADER) -exe:TDG01OD TDG01OD.obj $(LOADOPTS)
 TDK01MD.exe:  TDK01MD.obj ; $(LOADER) -exe:TDK01MD TDK01MD.obj $(LOADOPTS)
 TFB01QD.exe:  TFB01QD.obj ; $(LOADER) -exe:TFB01QD TFB01QD.obj $(LOADOPTS)
 TFB01RD.exe:  TFB01RD.obj ; $(LOADER) -exe:TFB01RD TFB01RD.obj $(LOADOPTS)
 TFB01SD.exe:  TFB01SD.obj ; $(LOADER) -exe:TFB01SD TFB01SD.obj $(LOADOPTS)
 TFB01TD.exe:  TFB01TD.obj ; $(LOADER) -exe:TFB01TD TFB01TD.obj $(LOADOPTS)
 TFB01VD.exe:  TFB01VD.obj ; $(LOADER) -exe:TFB01VD TFB01VD.obj $(LOADOPTS)
 TFD01AD.exe:  TFD01AD.obj ; $(LOADER) -exe:TFD01AD TFD01AD.obj $(LOADOPTS)
@@ -394,28 +398,58 @@
 TMB02JX.exe:  TMB02JX.obj ; $(LOADER) -exe:TMB02JX TMB02JX.obj $(LOADOPTS)
 TMB02KD.exe:  TMB02KD.obj ; $(LOADER) -exe:TMB02KD TMB02KD.obj $(LOADOPTS)
 TMB02MD.exe:  TMB02MD.obj ; $(LOADER) -exe:TMB02MD TMB02MD.obj $(LOADOPTS)
 TMB02ND.exe:  TMB02ND.obj ; $(LOADER) -exe:TMB02ND TMB02ND.obj $(LOADOPTS)
 TMB02QD.exe:  TMB02QD.obj ; $(LOADER) -exe:TMB02QD TMB02QD.obj $(LOADOPTS)
 TMB02SD.exe:  TMB02SD.obj ; $(LOADER) -exe:TMB02SD TMB02SD.obj $(LOADOPTS)
 TMB02VD.exe:  TMB02VD.obj ; $(LOADER) -exe:TMB02VD TMB02VD.obj $(LOADOPTS)
+TMB03BD.exe:  TMB03BD.obj ; $(LOADER) -exe:TMB03BD TMB03BD.obj $(LOADOPTS)
+TMB03BZ.exe:  TMB03BZ.obj ; $(LOADER) -exe:TMB03BZ TMB03BZ.obj $(LOADOPTS)
+TMB03FZ.exe:  TMB03FZ.obj ; $(LOADER) -exe:TMB03FZ TMB03FZ.obj $(LOADOPTS)
+TMB03KD.exe:  TMB03KD.obj ; $(LOADER) -exe:TMB03KD TMB03KD.obj $(LOADOPTS)
+TMB03LD.exe:  TMB03LD.obj ; $(LOADER) -exe:TMB03LD TMB03LD.obj $(LOADOPTS)
+TMB03LF.exe:  TMB03LF.obj ; $(LOADER) -exe:TMB03LF TMB03LF.obj $(LOADOPTS)
+TMB03LZ.exe:  TMB03LZ.obj ; $(LOADER) -exe:TMB03LZ TMB03LZ.obj $(LOADOPTS)
 TMB03MD.exe:  TMB03MD.obj ; $(LOADER) -exe:TMB03MD TMB03MD.obj $(LOADOPTS)
 TMB03ND.exe:  TMB03ND.obj ; $(LOADER) -exe:TMB03ND TMB03ND.obj $(LOADOPTS)
 TMB03OD.exe:  TMB03OD.obj ; $(LOADER) -exe:TMB03OD TMB03OD.obj $(LOADOPTS)
 TMB03PD.exe:  TMB03PD.obj ; $(LOADER) -exe:TMB03PD TMB03PD.obj $(LOADOPTS)
 TMB03QD.exe:  TMB03QD.obj ; $(LOADER) -exe:TMB03QD TMB03QD.obj $(LOADOPTS)
+TMB03QG.exe:  TMB03QG.obj ; $(LOADER) -exe:TMB03QG TMB03QG.obj $(LOADOPTS)
 TMB03RD.exe:  TMB03RD.obj ; $(LOADER) -exe:TMB03RD TMB03RD.obj $(LOADOPTS)
 TMB03SD.exe:  TMB03SD.obj ; $(LOADER) -exe:TMB03SD TMB03SD.obj $(LOADOPTS)
+TMB03TD.exe:  TMB03TD.obj ; $(LOADER) -exe:TMB03TD TMB03TD.obj $(LOADOPTS)
 TMB03UD.exe:  TMB03UD.obj ; $(LOADER) -exe:TMB03UD TMB03UD.obj $(LOADOPTS)
 TMB03VD.exe:  TMB03VD.obj ; $(LOADER) -exe:TMB03VD TMB03VD.obj $(LOADOPTS)
 TMB03WD.exe:  TMB03WD.obj ; $(LOADER) -exe:TMB03WD TMB03WD.obj $(LOADOPTS)
+TMB03XD.exe:  TMB03XD.obj ; $(LOADER) -exe:TMB03XD TMB03XD.obj $(LOADOPTS)
+TMB03XP.exe:  TMB03XP.obj ; $(LOADER) -exe:TMB03XP TMB03XP.obj $(LOADOPTS)
+TMB03XZ.exe:  TMB03XZ.obj ; $(LOADER) -exe:TMB03XZ TMB03XZ.obj $(LOADOPTS)
+TMB03ZD.exe:  TMB03ZD.obj ; $(LOADER) -exe:TMB03ZD TMB03ZD.obj $(LOADOPTS)
+TMB04AD.exe:  TMB04AD.obj ; $(LOADER) -exe:TMB04AD TMB04AD.obj $(LOADOPTS)
+TMB04AZ.exe:  TMB04AZ.obj ; $(LOADER) -exe:TMB04AZ TMB04AZ.obj $(LOADOPTS)
+TMB04BD.exe:  TMB04BD.obj ; $(LOADER) -exe:TMB04BD TMB04BD.obj $(LOADOPTS)
+TMB04BZ.exe:  TMB04BZ.obj ; $(LOADER) -exe:TMB04BZ TMB04BZ.obj $(LOADOPTS)
+TMB04DD.exe:  TMB04DD.obj ; $(LOADER) -exe:TMB04DD TMB04DD.obj $(LOADOPTS)
+TMB04DL.exe:  TMB04DL.obj ; $(LOADER) -exe:TMB04DL TMB04DL.obj $(LOADOPTS)
+TMB4DLZ.exe:  TMB4DLZ.obj ; $(LOADER) -exe:TMB4DLZ TMB4DLZ.obj $(LOADOPTS)
+TMB04DP.exe:  TMB04DP.obj ; $(LOADER) -exe:TMB04DP TMB04DP.obj $(LOADOPTS)
+TMB4DPZ.exe:  TMB4DPZ.obj ; $(LOADER) -exe:TMB4DPZ TMB4DPZ.obj $(LOADOPTS)
+TMB04DS.exe:  TMB04DS.obj ; $(LOADER) -exe:TMB04DS TMB04DS.obj $(LOADOPTS)
 TMB04DY.exe:  TMB04DY.obj ; $(LOADER) -exe:TMB04DY TMB04DY.obj $(LOADOPTS)
+TMB04DZ.exe:  TMB04DZ.obj ; $(LOADER) -exe:TMB04DZ TMB04DZ.obj $(LOADOPTS)
+TMB04ED.exe:  TMB04ED.obj ; $(LOADER) -exe:TMB04ED TMB04ED.obj $(LOADOPTS)
+TMB04FD.exe:  TMB04FD.obj ; $(LOADER) -exe:TMB04FD TMB04FD.obj $(LOADOPTS)
 TMB04GD.exe:  TMB04GD.obj ; $(LOADER) -exe:TMB04GD TMB04GD.obj $(LOADOPTS)
 TMB04MD.exe:  TMB04MD.obj ; $(LOADER) -exe:TMB04MD TMB04MD.obj $(LOADOPTS)
 TMB04OD.exe:  TMB04OD.obj ; $(LOADER) -exe:TMB04OD TMB04OD.obj $(LOADOPTS)
+TMB04PB.exe:  TMB04PB.obj ; $(LOADER) -exe:TMB04PB TMB04PB.obj $(LOADOPTS)
+TMB04PU.exe:  TMB04PU.obj ; $(LOADER) -exe:TMB04PU TMB04PU.obj $(LOADOPTS)
+TMB04TB.exe:  TMB04TB.obj ; $(LOADER) -exe:TMB04TB TMB04TB.obj $(LOADOPTS)
+TMB04TS.exe:  TMB04TS.obj ; $(LOADER) -exe:TMB04TS TMB04TS.obj $(LOADOPTS)
 TMB04UD.exe:  TMB04UD.obj ; $(LOADER) -exe:TMB04UD TMB04UD.obj $(LOADOPTS)
 TMB04VD.exe:  TMB04VD.obj ; $(LOADER) -exe:TMB04VD TMB04VD.obj $(LOADOPTS)
 TMB04XD.exe:  TMB04XD.obj ; $(LOADER) -exe:TMB04XD TMB04XD.obj $(LOADOPTS)
 TMB04YD.exe:  TMB04YD.obj ; $(LOADER) -exe:TMB04YD TMB04YD.obj $(LOADOPTS)
 TMB04ZD.exe:  TMB04ZD.obj ; $(LOADER) -exe:TMB04ZD TMB04ZD.obj $(LOADOPTS)
 TMB05MD.exe:  TMB05MD.obj ; $(LOADER) -exe:TMB05MD TMB05MD.obj $(LOADOPTS)
 TMB05ND.exe:  TMB05ND.obj ; $(LOADER) -exe:TMB05ND TMB05ND.obj $(LOADOPTS)
@@ -426,14 +460,15 @@
 TMC01PD.exe:  TMC01PD.obj ; $(LOADER) -exe:TMC01PD TMC01PD.obj $(LOADOPTS)
 TMC01QD.exe:  TMC01QD.obj ; $(LOADER) -exe:TMC01QD TMC01QD.obj $(LOADOPTS)
 TMC01RD.exe:  TMC01RD.obj ; $(LOADER) -exe:TMC01RD TMC01RD.obj $(LOADOPTS)
 TMC01SD.exe:  TMC01SD.obj ; $(LOADER) -exe:TMC01SD TMC01SD.obj $(LOADOPTS)
 TMC01TD.exe:  TMC01TD.obj ; $(LOADER) -exe:TMC01TD TMC01TD.obj $(LOADOPTS)
 TMC01VD.exe:  TMC01VD.obj ; $(LOADER) -exe:TMC01VD TMC01VD.obj $(LOADOPTS)
 TMC01WD.exe:  TMC01WD.obj ; $(LOADER) -exe:TMC01WD TMC01WD.obj $(LOADOPTS)
+TMC01XD.exe:  TMC01XD.obj ; $(LOADER) -exe:TMC01XD TMC01XD.obj $(LOADOPTS)
 TMC03MD.exe:  TMC03MD.obj ; $(LOADER) -exe:TMC03MD TMC03MD.obj $(LOADOPTS)
 TMC03ND.exe:  TMC03ND.obj ; $(LOADER) -exe:TMC03ND TMC03ND.obj $(LOADOPTS)
 TMD03AD.exe:  TMD03AD.obj ; $(LOADER) -exe:TMD03AD TMD03AD.obj $(LOADOPTS)
 TMD03BD.exe:  TMD03BD.obj ; $(LOADER) -exe:TMD03BD TMD03BD.obj $(LOADOPTS)
 TSB01BD.exe:  TSB01BD.obj ; $(LOADER) -exe:TSB01BD TSB01BD.obj $(LOADOPTS)
 TSB01DD.exe:  TSB01DD.obj ; $(LOADER) -exe:TSB01DD TSB01DD.obj $(LOADOPTS)
 TSB01MD.exe:  TSB01MD.obj ; $(LOADER) -exe:TSB01MD TSB01MD.obj $(LOADOPTS)
@@ -471,25 +506,30 @@
 TSB10ID.exe:  TSB10ID.obj ; $(LOADER) -exe:TSB10ID TSB10ID.obj $(LOADOPTS)
 TSB10KD.exe:  TSB10KD.obj ; $(LOADER) -exe:TSB10KD TSB10KD.obj $(LOADOPTS)
 TSB10ZD.exe:  TSB10ZD.obj ; $(LOADER) -exe:TSB10ZD TSB10ZD.obj $(LOADOPTS)
 TSB16AD.exe:  TSB16AD.obj ; $(LOADER) -exe:TSB16AD TSB16AD.obj $(LOADOPTS)
 TSB16BD.exe:  TSB16BD.obj ; $(LOADER) -exe:TSB16BD TSB16BD.obj $(LOADOPTS)
 TSB16CD.exe:  TSB16CD.obj ; $(LOADER) -exe:TSB16CD TSB16CD.obj $(LOADOPTS)
 TSG02AD.exe:  TSG02AD.obj ; $(LOADER) -exe:TSG02AD TSG02AD.obj $(LOADOPTS)
+TSG02ND.exe:  TSG02ND.obj ; $(LOADER) -exe:TSG02ND TSG02ND.obj $(LOADOPTS)
 TSG03AD.exe:  TSG03AD.obj ; $(LOADER) -exe:TSG03AD TSG03AD.obj $(LOADOPTS)
 TSG03BD.exe:  TSG03BD.obj ; $(LOADER) -exe:TSG03BD TSG03BD.obj $(LOADOPTS)
 TTB01ID.exe:  TTB01ID.obj ; $(LOADER) -exe:TTB01ID TTB01ID.obj $(LOADOPTS)
+TTB01IZ.exe:  TTB01IZ.obj ; $(LOADER) -exe:TTB01IZ TTB01IZ.obj $(LOADOPTS)
 TTB01KD.exe:  TTB01KD.obj ; $(LOADER) -exe:TTB01KD TTB01KD.obj $(LOADOPTS)
 TTB01LD.exe:  TTB01LD.obj ; $(LOADER) -exe:TTB01LD TTB01LD.obj $(LOADOPTS)
 TTB01MD.exe:  TTB01MD.obj ; $(LOADER) -exe:TTB01MD TTB01MD.obj $(LOADOPTS)
 TTB01ND.exe:  TTB01ND.obj ; $(LOADER) -exe:TTB01ND TTB01ND.obj $(LOADOPTS)
 TTB01PD.exe:  TTB01PD.obj ; $(LOADER) -exe:TTB01PD TTB01PD.obj $(LOADOPTS)
+TTB01PX.exe:  TTB01PX.obj ; $(LOADER) -exe:TTB01PX TTB01PX.obj $(LOADOPTS)
 TTB01TD.exe:  TTB01TD.obj ; $(LOADER) -exe:TTB01TD TTB01TD.obj $(LOADOPTS)
 TTB01UD.exe:  TTB01UD.obj ; $(LOADER) -exe:TTB01UD TTB01UD.obj $(LOADOPTS)
+TTB01UY.exe:  TTB01UY.obj ; $(LOADER) -exe:TTB01UY TTB01UY.obj $(LOADOPTS)
 TTB01WD.exe:  TTB01WD.obj ; $(LOADER) -exe:TTB01WD TTB01WD.obj $(LOADOPTS)
+TTB01WX.exe:  TTB01WX.obj ; $(LOADER) -exe:TTB01WX TTB01WX.obj $(LOADOPTS)
 TTB01ZD.exe:  TTB01ZD.obj ; $(LOADER) -exe:TTB01ZD TTB01ZD.obj $(LOADOPTS)
 TTB03AD.exe:  TTB03AD.obj ; $(LOADER) -exe:TTB03AD TTB03AD.obj $(LOADOPTS)
 TTB04AD.exe:  TTB04AD.obj ; $(LOADER) -exe:TTB04AD TTB04AD.obj $(LOADOPTS)
 TTB04BD.exe:  TTB04BD.obj ; $(LOADER) -exe:TTB04BD TTB04BD.obj $(LOADOPTS)
 TTB04CD.exe:  TTB04CD.obj ; $(LOADER) -exe:TTB04CD TTB04CD.obj $(LOADOPTS)
 TTB05AD.exe:  TTB05AD.obj ; $(LOADER) -exe:TTB05AD TTB05AD.obj $(LOADOPTS)
 TTC01OD.exe:  TTC01OD.obj ; $(LOADER) -exe:TTC01OD TTC01OD.obj $(LOADOPTS)
@@ -501,73 +541,35 @@
 TTF01MD.exe:  TTF01MD.obj ; $(LOADER) -exe:TTF01MD TTF01MD.obj $(LOADOPTS)
 TTF01ND.exe:  TTF01ND.obj ; $(LOADER) -exe:TTF01ND TTF01ND.obj $(LOADOPTS)
 TTF01OD.exe:  TTF01OD.obj ; $(LOADER) -exe:TTF01OD TTF01OD.obj $(LOADOPTS)
 TTF01PD.exe:  TTF01PD.obj ; $(LOADER) -exe:TTF01PD TTF01PD.obj $(LOADOPTS)
 TTF01QD.exe:  TTF01QD.obj ; $(LOADER) -exe:TTF01QD TTF01QD.obj $(LOADOPTS)
 TTF01RD.exe:  TTF01RD.obj ; $(LOADER) -exe:TTF01RD TTF01RD.obj $(LOADOPTS)
 TTG01AD.exe:  TTG01AD.obj ; $(LOADER) -exe:TTG01AD TTG01AD.obj $(LOADOPTS)
+TTG01AZ.exe:  TTG01AZ.obj ; $(LOADER) -exe:TTG01AZ TTG01AZ.obj $(LOADOPTS)
 TTG01CD.exe:  TTG01CD.obj ; $(LOADER) -exe:TTG01CD TTG01CD.obj $(LOADOPTS)
 TTG01DD.exe:  TTG01DD.obj ; $(LOADER) -exe:TTG01DD TTG01DD.obj $(LOADOPTS)
 TTG01ED.exe:  TTG01ED.obj ; $(LOADER) -exe:TTG01ED TTG01ED.obj $(LOADOPTS)
 TTG01FD.exe:  TTG01FD.obj ; $(LOADER) -exe:TTG01FD TTG01FD.obj $(LOADOPTS)
+TTG01FZ.exe:  TTG01FZ.obj ; $(LOADER) -exe:TTG01FZ TTG01FZ.obj $(LOADOPTS)
+TTG01GD.exe:  TTG01GD.obj ; $(LOADER) -exe:TTG01GD TTG01GD.obj $(LOADOPTS)
 TTG01HD.exe:  TTG01HD.obj ; $(LOADER) -exe:TTG01HD TTG01HD.obj $(LOADOPTS)
 TTG01ID.exe:  TTG01ID.obj ; $(LOADER) -exe:TTG01ID TTG01ID.obj $(LOADOPTS)
 TTG01JD.exe:  TTG01JD.obj ; $(LOADER) -exe:TTG01JD TTG01JD.obj $(LOADOPTS)
 TTG01JY.exe:  TTG01JY.obj ; $(LOADER) -exe:TTG01JY TTG01JY.obj $(LOADOPTS)
-TUD01BD.exe:  TUD01BD.obj ; $(LOADER) -exe:TUD01BD TUD01BD.obj $(LOADOPTS)
-TUD01CD.exe:  TUD01CD.obj ; $(LOADER) -exe:TUD01CD TUD01CD.obj $(LOADOPTS)
-TUD01DD.exe:  TUD01DD.obj ; $(LOADER) -exe:TUD01DD TUD01DD.obj $(LOADOPTS)
-TUD01MD.exe:  TUD01MD.obj ; $(LOADER) -exe:TUD01MD TUD01MD.obj $(LOADOPTS)
-TUD01ND.exe:  TUD01ND.obj ; $(LOADER) -exe:TUD01ND TUD01ND.obj $(LOADOPTS)
-TMB03TD.exe:  TMB03TD.obj ; $(LOADER) -exe:TMB03TD TMB03TD.obj $(LOADOPTS)
-TMB03XD.exe:  TMB03XD.obj ; $(LOADER) -exe:TMB03XD TMB03XD.obj $(LOADOPTS)
-TMB03XP.exe:  TMB03XP.obj ; $(LOADER) -exe:TMB03XP TMB03XP.obj $(LOADOPTS)
-TMB03ZD.exe:  TMB03ZD.obj ; $(LOADER) -exe:TMB03ZD TMB03ZD.obj $(LOADOPTS)
-TMB04DD.exe:  TMB04DD.obj ; $(LOADER) -exe:TMB04DD TMB04DD.obj $(LOADOPTS)
-TMB04DP.exe:  TMB04DP.obj ; $(LOADER) -exe:TMB04DP TMB04DP.obj $(LOADOPTS)
-TMB4DPZ.exe:  TMB4DPZ.obj ; $(LOADER) -exe:TMB4DPZ TMB4DPZ.obj $(LOADOPTS)
-TMB04DL.exe:  TMB04DL.obj ; $(LOADER) -exe:TMB04DL TMB04DL.obj $(LOADOPTS)
-TMB4DLZ.exe:  TMB4DLZ.obj ; $(LOADER) -exe:TMB4DLZ TMB4DLZ.obj $(LOADOPTS)
-TMB04DS.exe:  TMB04DS.obj ; $(LOADER) -exe:TMB04DS TMB04DS.obj $(LOADOPTS)
-TMB04PB.exe:  TMB04PB.obj ; $(LOADER) -exe:TMB04PB TMB04PB.obj $(LOADOPTS)
-TMB04PU.exe:  TMB04PU.obj ; $(LOADER) -exe:TMB04PU TMB04PU.obj $(LOADOPTS)
-TMB04TB.exe:  TMB04TB.obj ; $(LOADER) -exe:TMB04TB TMB04TB.obj $(LOADOPTS)
-TMB04TS.exe:  TMB04TS.obj ; $(LOADER) -exe:TMB04TS TMB04TS.obj $(LOADOPTS)
-TAB08NZ.exe:  TAB08NZ.obj ; $(LOADER) -exe:TAB08NZ TAB08NZ.obj $(LOADOPTS)
-TAG08BZ.exe:  TAG08BZ.obj ; $(LOADER) -exe:TAG08BZ TAG08BZ.obj $(LOADOPTS)
-TTB01IZ.exe:  TTB01IZ.obj ; $(LOADER) -exe:TTB01IZ TTB01IZ.obj $(LOADOPTS)
-TTG01AZ.exe:  TTG01AZ.obj ; $(LOADER) -exe:TTG01AZ TTG01AZ.obj $(LOADOPTS)
-TTG01FZ.exe:  TTG01FZ.obj ; $(LOADER) -exe:TTG01FZ TTG01FZ.obj $(LOADOPTS)
-TMB03BD.exe:  TMB03BD.obj ; $(LOADER) -exe:TMB03BD TMB03BD.obj $(LOADOPTS)
-TMB03KD.exe:  TMB03KD.obj ; $(LOADER) -exe:TMB03KD TMB03KD.obj $(LOADOPTS)
-TMB03LD.exe:  TMB03LD.obj ; $(LOADER) -exe:TMB03LD TMB03LD.obj $(LOADOPTS)
-TMB04AD.exe:  TMB04AD.obj ; $(LOADER) -exe:TMB04AD TMB04AD.obj $(LOADOPTS)
-TMB04BD.exe:  TMB04BD.obj ; $(LOADER) -exe:TMB04BD TMB04BD.obj $(LOADOPTS)
-TMB03BZ.exe:  TMB03BZ.obj ; $(LOADER) -exe:TMB03BZ TMB03BZ.obj $(LOADOPTS)
-TMB03FZ.exe:  TMB03FZ.obj ; $(LOADER) -exe:TMB03FZ TMB03FZ.obj $(LOADOPTS)
-TMB03LF.exe:  TMB03LF.obj ; $(LOADER) -exe:TMB03LF TMB03LF.obj $(LOADOPTS)
-TMB03LZ.exe:  TMB03LZ.obj ; $(LOADER) -exe:TMB03LZ TMB03LZ.obj $(LOADOPTS)
-TMB03XZ.exe:  TMB03XZ.obj ; $(LOADER) -exe:TMB03XZ TMB03XZ.obj $(LOADOPTS)
-TMB04AZ.exe:  TMB04AZ.obj ; $(LOADER) -exe:TMB04AZ TMB04AZ.obj $(LOADOPTS)
-TMB04BZ.exe:  TMB04BZ.obj ; $(LOADER) -exe:TMB04BZ TMB04BZ.obj $(LOADOPTS)
-TMB04DZ.exe:  TMB04DZ.obj ; $(LOADER) -exe:TMB04DZ TMB04DZ.obj $(LOADOPTS)
-TMB04ED.exe:  TMB04ED.obj ; $(LOADER) -exe:TMB04ED TMB04ED.obj $(LOADOPTS)
-TMB04FD.exe:  TMB04FD.obj ; $(LOADER) -exe:TMB04FD TMB04FD.obj $(LOADOPTS)
-TMC01XD.exe:  TMC01XD.obj ; $(LOADER) -exe:TMC01XD TMC01XD.obj $(LOADOPTS)
-TSG02ND.exe:  TSG02ND.obj ; $(LOADER) -exe:TSG02ND TSG02ND.obj $(LOADOPTS)
-TMB03QG.exe:  TMB03QG.obj ; $(LOADER) -exe:TMB03QG TMB03QG.obj $(LOADOPTS)
-TTB01PX.exe:  TTB01PX.obj ; $(LOADER) -exe:TTB01PX TTB01PX.obj $(LOADOPTS)
-TTB01UY.exe:  TTB01UY.obj ; $(LOADER) -exe:TTB01UY TTB01UY.obj $(LOADOPTS)
-TTB01WX.exe:  TTB01WX.obj ; $(LOADER) -exe:TTB01WX TTB01WX.obj $(LOADOPTS)
-TTG01GD.exe:  TTG01GD.obj ; $(LOADER) -exe:TTG01GD TTG01GD.obj $(LOADOPTS)
 TTG01LD.exe:  TTG01LD.obj ; $(LOADER) -exe:TTG01LD TTG01LD.obj $(LOADOPTS)
 TTG01MD.exe:  TTG01MD.obj ; $(LOADER) -exe:TTG01MD TTG01MD.obj $(LOADOPTS)
 TTG01ND.exe:  TTG01ND.obj ; $(LOADER) -exe:TTG01ND TTG01ND.obj $(LOADOPTS)
 TTG01PD.exe:  TTG01PD.obj ; $(LOADER) -exe:TTG01PD TTG01PD.obj $(LOADOPTS)
 TTG01QD.exe:  TTG01QD.obj ; $(LOADER) -exe:TTG01QD TTG01QD.obj $(LOADOPTS)
+TUD01BD.exe:  TUD01BD.obj ; $(LOADER) -exe:TUD01BD TUD01BD.obj $(LOADOPTS)
+TUD01CD.exe:  TUD01CD.obj ; $(LOADER) -exe:TUD01CD TUD01CD.obj $(LOADOPTS)
+TUD01DD.exe:  TUD01DD.obj ; $(LOADER) -exe:TUD01DD TUD01DD.obj $(LOADOPTS)
+TUD01MD.exe:  TUD01MD.obj ; $(LOADER) -exe:TUD01MD TUD01MD.obj $(LOADOPTS)
+TUD01ND.exe:  TUD01ND.obj ; $(LOADER) -exe:TUD01ND TUD01ND.obj $(LOADOPTS)
 
 clean:
 	del *.exa
 
 cleanup:
 	del *.ex*
 
@@ -581,14 +583,15 @@
 TAB05PD.obj: ..\src\AB05PD.f TAB05PD.f ; $(FORTRAN) $(OPTS) -c TAB05PD.f
 TAB05QD.obj: ..\src\AB05QD.f TAB05QD.f ; $(FORTRAN) $(OPTS) -c TAB05QD.f
 TAB05RD.obj: ..\src\AB05RD.f TAB05RD.f ; $(FORTRAN) $(OPTS) -c TAB05RD.f
 TAB07MD.obj: ..\src\AB07MD.f TAB07MD.f ; $(FORTRAN) $(OPTS) -c TAB07MD.f
 TAB07ND.obj: ..\src\AB07ND.f TAB07ND.f ; $(FORTRAN) $(OPTS) -c TAB07ND.f
 TAB08ND.obj: ..\src\AB08ND.f TAB08ND.f ; $(FORTRAN) $(OPTS) -c TAB08ND.f
 TAB08NW.obj: ..\src\AB08NW.f TAB08NW.f ; $(FORTRAN) $(OPTS) -c TAB08NW.f
+TAB08NZ.obj: ..\src\AB08NZ.f TAB08NZ.f ; $(FORTRAN) $(OPTS) -c TAB08NZ.f
 TAB09AD.obj: ..\src\AB09AD.f TAB09AD.f ; $(FORTRAN) $(OPTS) -c TAB09AD.f
 TAB09BD.obj: ..\src\AB09BD.f TAB09BD.f ; $(FORTRAN) $(OPTS) -c TAB09BD.f
 TAB09CD.obj: ..\src\AB09CD.f TAB09CD.f ; $(FORTRAN) $(OPTS) -c TAB09CD.f
 TAB09DD.obj: ..\src\AB09DD.f TAB09DD.f ; $(FORTRAN) $(OPTS) -c TAB09DD.f
 TAB09ED.obj: ..\src\AB09ED.f TAB09ED.f ; $(FORTRAN) $(OPTS) -c TAB09ED.f
 TAB09FD.obj: ..\src\AB09FD.f TAB09FD.f ; $(FORTRAN) $(OPTS) -c TAB09FD.f
 TAB09GD.obj: ..\src\AB09GD.f TAB09GD.f ; $(FORTRAN) $(OPTS) -c TAB09GD.f
@@ -603,24 +606,25 @@
 TAB13CD.obj: ..\src\AB13CD.f TAB13CD.f ; $(FORTRAN) $(OPTS) -c TAB13CD.f
 TAB13DD.obj: ..\src\AB13DD.f TAB13DD.f ; $(FORTRAN) $(OPTS) -c TAB13DD.f
 TAB13ED.obj: ..\src\AB13ED.f TAB13ED.f ; $(FORTRAN) $(OPTS) -c TAB13ED.f
 TAB13FD.obj: ..\src\AB13FD.f TAB13FD.f ; $(FORTRAN) $(OPTS) -c TAB13FD.f
 TAB13ID.obj: ..\src\AB13ID.f TAB13ID.f ; $(FORTRAN) $(OPTS) -c TAB13ID.f
 TAB13MD.obj: ..\src\AB13MD.f TAB13MD.f ; $(FORTRAN) $(OPTS) -c TAB13MD.f
 TAG08BD.obj: ..\src\AG08BD.f TAG08BD.f ; $(FORTRAN) $(OPTS) -c TAG08BD.f
+TAG08BZ.obj: ..\src\AG08BZ.f TAG08BZ.f ; $(FORTRAN) $(OPTS) -c TAG08BZ.f
 TBB01AD.obj: ..\src\BB01AD.f TBB01AD.f ; $(FORTRAN) $(OPTS) -c TBB01AD.f
 TBB02AD.obj: ..\src\BB02AD.f TBB02AD.f ; $(FORTRAN) $(OPTS) -c TBB02AD.f
 TBB03AD.obj: ..\src\BB03AD.f TBB03AD.f ; $(FORTRAN) $(OPTS) -c TBB03AD.f
 TBB04AD.obj: ..\src\BB04AD.f TBB04AD.f ; $(FORTRAN) $(OPTS) -c TBB04AD.f
 TBD01AD.obj: ..\src\BD01AD.f TBD01AD.f ; $(FORTRAN) $(OPTS) -c TBD01AD.f
 TBD02AD.obj: ..\src\BD02AD.f TBD02AD.f ; $(FORTRAN) $(OPTS) -c TBD02AD.f
 TDE01OD.obj: ..\src\DE01OD.f TDE01OD.f ; $(FORTRAN) $(OPTS) -c TDE01OD.f
 TDE01PD.obj: ..\src\DE01PD.f TDE01PD.f ; $(FORTRAN) $(OPTS) -c TDE01PD.f
-TDG01OD.obj: ..\src\DG01OD.f TDG01OD.f ; $(FORTRAN) $(OPTS) -c TDG01OD.f
 TDF01MD.obj: ..\src\DF01MD.f TDF01MD.f ; $(FORTRAN) $(OPTS) -c TDF01MD.f
+TDG01OD.obj: ..\src\DG01OD.f TDG01OD.f ; $(FORTRAN) $(OPTS) -c TDG01OD.f
 TDG01MD.obj: ..\src\DG01MD.f TDG01MD.f ; $(FORTRAN) $(OPTS) -c TDG01MD.f
 TDG01ND.obj: ..\src\DG01ND.f TDG01ND.f ; $(FORTRAN) $(OPTS) -c TDG01ND.f
 TDK01MD.obj: ..\src\DK01MD.f TDK01MD.f ; $(FORTRAN) $(OPTS) -c TDK01MD.f
 TFB01QD.obj: ..\src\FB01QD.f TFB01QD.f ; $(FORTRAN) $(OPTS) -c TFB01QD.f
 TFB01RD.obj: ..\src\FB01RD.f TFB01RD.f ; $(FORTRAN) $(OPTS) -c TFB01RD.f
 TFB01SD.obj: ..\src\FB01SD.f TFB01SD.f ; $(FORTRAN) $(OPTS) -c TFB01SD.f
 TFB01TD.obj: ..\src\FB01TD.f TFB01TD.f ; $(FORTRAN) $(OPTS) -c TFB01TD.f
@@ -643,28 +647,58 @@
 TMB02JX.obj: ..\src\MB02JX.f TMB02JX.f ; $(FORTRAN) $(OPTS) -c TMB02JX.f
 TMB02KD.obj: ..\src\MB02KD.f TMB02KD.f ; $(FORTRAN) $(OPTS) -c TMB02KD.f
 TMB02MD.obj: ..\src\MB02MD.f TMB02MD.f ; $(FORTRAN) $(OPTS) -c TMB02MD.f
 TMB02ND.obj: ..\src\MB02ND.f TMB02ND.f ; $(FORTRAN) $(OPTS) -c TMB02ND.f
 TMB02QD.obj: ..\src\MB02QD.f TMB02QD.f ; $(FORTRAN) $(OPTS) -c TMB02QD.f
 TMB02SD.obj: ..\src\MB02SD.f TMB02SD.f ; $(FORTRAN) $(OPTS) -c TMB02SD.f
 TMB02VD.obj: ..\src\MB02VD.f TMB02VD.f ; $(FORTRAN) $(OPTS) -c TMB02VD.f
+TMB03BD.obj: ..\src\MB03BD.f TMB03BD.f ; $(FORTRAN) $(OPTS) -c TMB03BD.f
+TMB03BZ.obj: ..\src\MB03BZ.f TMB03BZ.f ; $(FORTRAN) $(OPTS) -c TMB03BZ.f
+TMB03FZ.obj: ..\src\MB03FZ.f TMB03FZ.f ; $(FORTRAN) $(OPTS) -c TMB03FZ.f
+TMB03KD.obj: ..\src\MB03KD.f TMB03KD.f ; $(FORTRAN) $(OPTS) -c TMB03KD.f
+TMB03LD.obj: ..\src\MB03LD.f TMB03LD.f ; $(FORTRAN) $(OPTS) -c TMB03LD.f
+TMB03LF.obj: ..\src\MB03LF.f TMB03LF.f ; $(FORTRAN) $(OPTS) -c TMB03LF.f
+TMB03LZ.obj: ..\src\MB03LZ.f TMB03LZ.f ; $(FORTRAN) $(OPTS) -c TMB03LZ.f
 TMB03MD.obj: ..\src\MB03MD.f TMB03MD.f ; $(FORTRAN) $(OPTS) -c TMB03MD.f
 TMB03ND.obj: ..\src\MB03ND.f TMB03ND.f ; $(FORTRAN) $(OPTS) -c TMB03ND.f
 TMB03OD.obj: ..\src\MB03OD.f TMB03OD.f ; $(FORTRAN) $(OPTS) -c TMB03OD.f
 TMB03PD.obj: ..\src\MB03PD.f TMB03PD.f ; $(FORTRAN) $(OPTS) -c TMB03PD.f
 TMB03QD.obj: ..\src\MB03QD.f TMB03QD.f ; $(FORTRAN) $(OPTS) -c TMB03QD.f
+TMB03QG.obj: ..\src\MB03QG.f TMB03QG.f ; $(FORTRAN) $(OPTS) -c TMB03QG.f
 TMB03RD.obj: ..\src\MB03RD.f TMB03RD.f ; $(FORTRAN) $(OPTS) -c TMB03RD.f
 TMB03SD.obj: ..\src\MB03SD.f TMB03SD.f ; $(FORTRAN) $(OPTS) -c TMB03SD.f
+TMB03TD.obj: ..\src\MB03TD.f TMB03TD.f ; $(FORTRAN) $(OPTS) -c TMB03TD.f
 TMB03UD.obj: ..\src\MB03UD.f TMB03UD.f ; $(FORTRAN) $(OPTS) -c TMB03UD.f
 TMB03VD.obj: ..\src\MB03VD.f TMB03VD.f ; $(FORTRAN) $(OPTS) -c TMB03VD.f
 TMB03WD.obj: ..\src\MB03WD.f TMB03WD.f ; $(FORTRAN) $(OPTS) -c TMB03WD.f
+TMB03XD.obj: ..\src\MB03XD.f TMB03XD.f ; $(FORTRAN) $(OPTS) -c TMB03XD.f
+TMB03XP.obj: ..\src\MB03XP.f TMB03XP.f ; $(FORTRAN) $(OPTS) -c TMB03XP.f
+TMB03XZ.obj: ..\src\MB03XZ.f TMB03XZ.f ; $(FORTRAN) $(OPTS) -c TMB03XZ.f
+TMB03ZD.obj: ..\src\MB03ZD.f TMB03ZD.f ; $(FORTRAN) $(OPTS) -c TMB03ZD.f
+TMB04AD.obj: ..\src\MB04AD.f TMB04AD.f ; $(FORTRAN) $(OPTS) -c TMB04AD.f
+TMB04AZ.obj: ..\src\MB04AZ.f TMB04AZ.f ; $(FORTRAN) $(OPTS) -c TMB04AZ.f
+TMB04BD.obj: ..\src\MB04BD.f TMB04BD.f ; $(FORTRAN) $(OPTS) -c TMB04BD.f
+TMB04BZ.obj: ..\src\MB04BZ.f TMB04BZ.f ; $(FORTRAN) $(OPTS) -c TMB04BZ.f
+TMB04DD.obj: ..\src\MB04DD.f TMB04DD.f ; $(FORTRAN) $(OPTS) -c TMB04DD.f
+TMB04DL.obj: ..\src\MB04DL.f TMB04DL.f ; $(FORTRAN) $(OPTS) -c TMB04DL.f
+TMB4DLZ.obj: ..\src\MB4DLZ.f TMB4DLZ.f ; $(FORTRAN) $(OPTS) -c TMB4DLZ.f
+TMB04DP.obj: ..\src\MB04DP.f TMB04DP.f ; $(FORTRAN) $(OPTS) -c TMB04DP.f
+TMB4DPZ.obj: ..\src\MB4DPZ.f TMB4DPZ.f ; $(FORTRAN) $(OPTS) -c TMB4DPZ.f
+TMB04DS.obj: ..\src\MB04DS.f TMB04DS.f ; $(FORTRAN) $(OPTS) -c TMB04DS.f
 TMB04DY.obj: ..\src\MB04DY.f TMB04DY.f ; $(FORTRAN) $(OPTS) -c TMB04DY.f
+TMB04DZ.obj: ..\src\MB04DZ.f TMB04DZ.f ; $(FORTRAN) $(OPTS) -c TMB04DZ.f
+TMB04ED.obj: ..\src\MB04ED.f TMB04ED.f ; $(FORTRAN) $(OPTS) -c TMB04ED.f
+TMB04FD.obj: ..\src\MB04FD.f TMB04FD.f ; $(FORTRAN) $(OPTS) -c TMB04FD.f
 TMB04GD.obj: ..\src\MB04GD.f TMB04GD.f ; $(FORTRAN) $(OPTS) -c TMB04GD.f
 TMB04MD.obj: ..\src\MB04MD.f TMB04MD.f ; $(FORTRAN) $(OPTS) -c TMB04MD.f
 TMB04OD.obj: ..\src\MB04OD.f TMB04OD.f ; $(FORTRAN) $(OPTS) -c TMB04OD.f
+TMB04PB.obj: ..\src\MB04PB.f TMB04PB.f ; $(FORTRAN) $(OPTS) -c TMB04PB.f
+TMB04PU.obj: ..\src\MB04PU.f TMB04PU.f ; $(FORTRAN) $(OPTS) -c TMB04PU.f
+TMB04TB.obj: ..\src\MB04TB.f TMB04TB.f ; $(FORTRAN) $(OPTS) -c TMB04TB.f
+TMB04TS.obj: ..\src\MB04TS.f TMB04TS.f ; $(FORTRAN) $(OPTS) -c TMB04TS.f
 TMB04UD.obj: ..\src\MB04UD.f TMB04UD.f ; $(FORTRAN) $(OPTS) -c TMB04UD.f
 TMB04VD.obj: ..\src\MB04VD.f TMB04VD.f ; $(FORTRAN) $(OPTS) -c TMB04VD.f
 TMB04XD.obj: ..\src\MB04XD.f TMB04XD.f ; $(FORTRAN) $(OPTS) -c TMB04XD.f
 TMB04YD.obj: ..\src\MB04YD.f TMB04YD.f ; $(FORTRAN) $(OPTS) -c TMB04YD.f
 TMB04ZD.obj: ..\src\MB04ZD.f TMB04ZD.f ; $(FORTRAN) $(OPTS) -c TMB04ZD.f
 TMB05MD.obj: ..\src\MB05MD.f TMB05MD.f ; $(FORTRAN) $(OPTS) -c TMB05MD.f
 TMB05ND.obj: ..\src\MB05ND.f TMB05ND.f ; $(FORTRAN) $(OPTS) -c TMB05ND.f
@@ -675,14 +709,15 @@
 TMC01PD.obj: ..\src\MC01PD.f TMC01PD.f ; $(FORTRAN) $(OPTS) -c TMC01PD.f
 TMC01QD.obj: ..\src\MC01QD.f TMC01QD.f ; $(FORTRAN) $(OPTS) -c TMC01QD.f
 TMC01RD.obj: ..\src\MC01RD.f TMC01RD.f ; $(FORTRAN) $(OPTS) -c TMC01RD.f
 TMC01SD.obj: ..\src\MC01SD.f TMC01SD.f ; $(FORTRAN) $(OPTS) -c TMC01SD.f
 TMC01TD.obj: ..\src\MC01TD.f TMC01TD.f ; $(FORTRAN) $(OPTS) -c TMC01TD.f
 TMC01VD.obj: ..\src\MC01VD.f TMC01VD.f ; $(FORTRAN) $(OPTS) -c TMC01VD.f
 TMC01WD.obj: ..\src\MC01WD.f TMC01WD.f ; $(FORTRAN) $(OPTS) -c TMC01WD.f
+TMC01XD.obj: ..\src\MC01XD.f TMC01XD.f ; $(FORTRAN) $(OPTS) -c TMC01XD.f
 TMC03MD.obj: ..\src\MC03MD.f TMC03MD.f ; $(FORTRAN) $(OPTS) -c TMC03MD.f
 TMC03ND.obj: ..\src\MC03ND.f TMC03ND.f ; $(FORTRAN) $(OPTS) -c TMC03ND.f
 TMD03AD.obj: ..\src\MD03AD.f TMD03AD.f ; $(FORTRAN) $(OPTS) -c TMD03AD.f
 TMD03BD.obj: ..\src\MD03BD.f TMD03BD.f ; $(FORTRAN) $(OPTS) -c TMD03BD.f
 TSB01BD.obj: ..\src\SB01BD.f TSB01BD.f ; $(FORTRAN) $(OPTS) -c TSB01BD.f
 TSB01DD.obj: ..\src\SB01DD.f TSB01DD.f ; $(FORTRAN) $(OPTS) -c TSB01DD.f
 TSB01MD.obj: ..\src\SB01MD.f TSB01MD.f ; $(FORTRAN) $(OPTS) -c TSB01MD.f
@@ -720,25 +755,30 @@
 TSB10ID.obj: ..\src\SB10ID.f TSB10ID.f ; $(FORTRAN) $(OPTS) -c TSB10ID.f
 TSB10KD.obj: ..\src\SB10KD.f TSB10KD.f ; $(FORTRAN) $(OPTS) -c TSB10KD.f
 TSB10ZD.obj: ..\src\SB10ZD.f TSB10ZD.f ; $(FORTRAN) $(OPTS) -c TSB10ZD.f
 TSB16AD.obj: ..\src\SB16AD.f TSB16AD.f ; $(FORTRAN) $(OPTS) -c TSB16AD.f
 TSB16BD.obj: ..\src\SB16BD.f TSB16BD.f ; $(FORTRAN) $(OPTS) -c TSB16BD.f
 TSB16CD.obj: ..\src\SB16CD.f TSB16CD.f ; $(FORTRAN) $(OPTS) -c TSB16CD.f
 TSG02AD.obj: ..\src\SG02AD.f TSG02AD.f ; $(FORTRAN) $(OPTS) -c TSG02AD.f
+TSG02ND.obj: ..\src\SG02ND.f TSG02ND.f ; $(FORTRAN) $(OPTS) -c TSG02ND.f
 TSG03AD.obj: ..\src\SG03AD.f TSG03AD.f ; $(FORTRAN) $(OPTS) -c TSG03AD.f
 TSG03BD.obj: ..\src\SG03BD.f TSG03BD.f ; $(FORTRAN) $(OPTS) -c TSG03BD.f
 TTB01ID.obj: ..\src\TB01ID.f TTB01ID.f ; $(FORTRAN) $(OPTS) -c TTB01ID.f
+TTB01IZ.obj: ..\src\TB01IZ.f TTB01IZ.f ; $(FORTRAN) $(OPTS) -c TTB01IZ.f
 TTB01KD.obj: ..\src\TB01KD.f TTB01KD.f ; $(FORTRAN) $(OPTS) -c TTB01KD.f
 TTB01LD.obj: ..\src\TB01LD.f TTB01LD.f ; $(FORTRAN) $(OPTS) -c TTB01LD.f
 TTB01MD.obj: ..\src\TB01MD.f TTB01MD.f ; $(FORTRAN) $(OPTS) -c TTB01MD.f
 TTB01ND.obj: ..\src\TB01ND.f TTB01ND.f ; $(FORTRAN) $(OPTS) -c TTB01ND.f
 TTB01PD.obj: ..\src\TB01PD.f TTB01PD.f ; $(FORTRAN) $(OPTS) -c TTB01PD.f
+TTB01PX.obj: ..\src\TB01PX.f TTB01PX.f ; $(FORTRAN) $(OPTS) -c TTB01PX.f
 TTB01TD.obj: ..\src\TB01TD.f TTB01TD.f ; $(FORTRAN) $(OPTS) -c TTB01TD.f
 TTB01UD.obj: ..\src\TB01UD.f TTB01UD.f ; $(FORTRAN) $(OPTS) -c TTB01UD.f
+TTB01UY.obj: ..\src\TB01UY.f TTB01UY.f ; $(FORTRAN) $(OPTS) -c TTB01UY.f
 TTB01WD.obj: ..\src\TB01WD.f TTB01WD.f ; $(FORTRAN) $(OPTS) -c TTB01WD.f
+TTB01WX.obj: ..\src\TB01WX.f TTB01WX.f ; $(FORTRAN) $(OPTS) -c TTB01WX.f
 TTB01ZD.obj: ..\src\TB01ZD.f TTB01ZD.f ; $(FORTRAN) $(OPTS) -c TTB01ZD.f
 TTB03AD.obj: ..\src\TB03AD.f TTB03AD.f ; $(FORTRAN) $(OPTS) -c TTB03AD.f
 TTB04AD.obj: ..\src\TB04AD.f TTB04AD.f ; $(FORTRAN) $(OPTS) -c TTB04AD.f
 TTB04BD.obj: ..\src\TB04BD.f TTB04BD.f ; $(FORTRAN) $(OPTS) -c TTB04BD.f
 TTB04CD.obj: ..\src\TB04CD.f TTB04CD.f ; $(FORTRAN) $(OPTS) -c TTB04CD.f
 TTB05AD.obj: ..\src\TB05AD.f TTB05AD.f ; $(FORTRAN) $(OPTS) -c TTB05AD.f
 TTC01OD.obj: ..\src\TC01OD.f TTC01OD.f ; $(FORTRAN) $(OPTS) -c TTC01OD.f
@@ -750,68 +790,30 @@
 TTF01MD.obj: ..\src\TF01MD.f TTF01MD.f ; $(FORTRAN) $(OPTS) -c TTF01MD.f
 TTF01ND.obj: ..\src\TF01ND.f TTF01ND.f ; $(FORTRAN) $(OPTS) -c TTF01ND.f
 TTF01OD.obj: ..\src\TF01OD.f TTF01OD.f ; $(FORTRAN) $(OPTS) -c TTF01OD.f
 TTF01PD.obj: ..\src\TF01PD.f TTF01PD.f ; $(FORTRAN) $(OPTS) -c TTF01PD.f
 TTF01QD.obj: ..\src\TF01QD.f TTF01QD.f ; $(FORTRAN) $(OPTS) -c TTF01QD.f
 TTF01RD.obj: ..\src\TF01RD.f TTF01RD.f ; $(FORTRAN) $(OPTS) -c TTF01RD.f
 TTG01AD.obj: ..\src\TG01AD.f TTG01AD.f ; $(FORTRAN) $(OPTS) -c TTG01AD.f
+TTG01AZ.obj: ..\src\TG01AZ.f TTG01AZ.f ; $(FORTRAN) $(OPTS) -c TTG01AZ.f
 TTG01CD.obj: ..\src\TG01CD.f TTG01CD.f ; $(FORTRAN) $(OPTS) -c TTG01CD.f
 TTG01DD.obj: ..\src\TG01DD.f TTG01DD.f ; $(FORTRAN) $(OPTS) -c TTG01DD.f
 TTG01ED.obj: ..\src\TG01ED.f TTG01ED.f ; $(FORTRAN) $(OPTS) -c TTG01ED.f
 TTG01FD.obj: ..\src\TG01FD.f TTG01FD.f ; $(FORTRAN) $(OPTS) -c TTG01FD.f
+TTG01FZ.obj: ..\src\TG01FZ.f TTG01FZ.f ; $(FORTRAN) $(OPTS) -c TTG01FZ.f
+TTG01GD.obj: ..\src\TG01GD.f TTG01GD.f ; $(FORTRAN) $(OPTS) -c TTG01GD.f
 TTG01HD.obj: ..\src\TG01HD.f TTG01HD.f ; $(FORTRAN) $(OPTS) -c TTG01HD.f
 TTG01ID.obj: ..\src\TG01ID.f TTG01ID.f ; $(FORTRAN) $(OPTS) -c TTG01ID.f
 TTG01JD.obj: ..\src\TG01JD.f TTG01JD.f ; $(FORTRAN) $(OPTS) -c TTG01JD.f
 TTG01JY.obj: ..\src\TG01JY.f TTG01JY.f ; $(FORTRAN) $(OPTS) -c TTG01JY.f
-TUD01BD.obj: ..\src\UD01BD.f TUD01BD.f ; $(FORTRAN) $(OPTS) -c TUD01BD.f
-TUD01CD.obj: ..\src\UD01CD.f TUD01CD.f ; $(FORTRAN) $(OPTS) -c TUD01CD.f
-TUD01DD.obj: ..\src\UD01DD.f TUD01DD.f ; $(FORTRAN) $(OPTS) -c TUD01DD.f
-TUD01MD.obj: ..\src\UD01MD.f TUD01MD.f ; $(FORTRAN) $(OPTS) -c TUD01MD.f
-TUD01ND.obj: ..\src\UD01ND.f TUD01ND.f ; $(FORTRAN) $(OPTS) -c TUD01ND.f
-TMB03TD.obj: ..\src\MB03TD.f TMB03TD.f ; $(FORTRAN) $(OPTS) -c TMB03TD.f
-TMB03XD.obj: ..\src\MB03XD.f TMB03XD.f ; $(FORTRAN) $(OPTS) -c TMB03XD.f
-TMB03XP.obj: ..\src\MB03XP.f TMB03XP.f ; $(FORTRAN) $(OPTS) -c TMB03XP.f
-TMB03ZD.obj: ..\src\MB03ZD.f TMB03ZD.f ; $(FORTRAN) $(OPTS) -c TMB03ZD.f
-TMB04DD.obj: ..\src\MB04DD.f TMB04DD.f ; $(FORTRAN) $(OPTS) -c TMB04DD.f
-TMB04DP.obj: ..\src\MB04DP.f TMB04DP.f ; $(FORTRAN) $(OPTS) -c TMB04DP.f
-TMB4DPZ.obj: ..\src\MB4DPZ.f TMB4DPZ.f ; $(FORTRAN) $(OPTS) -c TMB4DPZ.f
-TMB04DL.obj: ..\src\MB04DL.f TMB04DL.f ; $(FORTRAN) $(OPTS) -c TMB04DL.f
-TMB4DLZ.obj: ..\src\MB4DLZ.f TMB4DLZ.f ; $(FORTRAN) $(OPTS) -c TMB4DLZ.f
-TMB04DS.obj: ..\src\MB04DS.f TMB04DS.f ; $(FORTRAN) $(OPTS) -c TMB04DS.f
-TMB04PB.obj: ..\src\MB04PB.f TMB04PB.f ; $(FORTRAN) $(OPTS) -c TMB04PB.f
-TMB04PU.obj: ..\src\MB04PU.f TMB04PU.f ; $(FORTRAN) $(OPTS) -c TMB04PU.f
-TMB04TB.obj: ..\src\MB04TB.f TMB04TB.f ; $(FORTRAN) $(OPTS) -c TMB04TB.f
-TMB04TS.obj: ..\src\MB04TS.f TMB04TS.f ; $(FORTRAN) $(OPTS) -c TMB04TS.f
-TAB08NZ.obj: ..\src\AB08NZ.f TAB08NZ.f ; $(FORTRAN) $(OPTS) -c TAB08NZ.f
-TAG08BZ.obj: ..\src\AG08BZ.f TAG08BZ.f ; $(FORTRAN) $(OPTS) -c TAG08BZ.f
-TTB01IZ.obj: ..\src\TB01IZ.f TTB01IZ.f ; $(FORTRAN) $(OPTS) -c TTB01IZ.f
-TTG01AZ.obj: ..\src\TG01AZ.f TTG01AZ.f ; $(FORTRAN) $(OPTS) -c TTG01AZ.f
-TTG01FZ.obj: ..\src\TG01FZ.f TTG01FZ.f ; $(FORTRAN) $(OPTS) -c TTG01FZ.f
-TMB03BD.obj: ..\src\MB03BD.f TMB03BD.f ; $(FORTRAN) $(OPTS) -c TMB03BD.f
-TMB03KD.obj: ..\src\MB03KD.f TMB03KD.f ; $(FORTRAN) $(OPTS) -c TMB03KD.f
-TMB03LD.obj: ..\src\MB03LD.f TMB03LD.f ; $(FORTRAN) $(OPTS) -c TMB03LD.f
-TMB04AD.obj: ..\src\MB04AD.f TMB04AD.f ; $(FORTRAN) $(OPTS) -c TMB04AD.f
-TMB04BD.obj: ..\src\MB04BD.f TMB04BD.f ; $(FORTRAN) $(OPTS) -c TMB04BD.f
-TMB03BZ.obj: ..\src\MB03BZ.f TMB03BZ.f ; $(FORTRAN) $(OPTS) -c TMB03BZ.f
-TMB03FZ.obj: ..\src\MB03FZ.f TMB03FZ.f ; $(FORTRAN) $(OPTS) -c TMB03FZ.f
-TMB03LF.obj: ..\src\MB03LF.f TMB03LF.f ; $(FORTRAN) $(OPTS) -c TMB03LF.f
-TMB03LZ.obj: ..\src\MB03LZ.f TMB03LZ.f ; $(FORTRAN) $(OPTS) -c TMB03LZ.f
-TMB03XZ.obj: ..\src\MB03XZ.f TMB03XZ.f ; $(FORTRAN) $(OPTS) -c TMB03XZ.f
-TMB04AZ.obj: ..\src\MB04AZ.f TMB04AZ.f ; $(FORTRAN) $(OPTS) -c TMB04AZ.f
-TMB04BZ.obj: ..\src\MB04BZ.f TMB04BZ.f ; $(FORTRAN) $(OPTS) -c TMB04BZ.f
-TMB04DZ.obj: ..\src\MB04DZ.f TMB04DZ.f ; $(FORTRAN) $(OPTS) -c TMB04DZ.f
-TMB04ED.obj: ..\src\MB04ED.f TMB04ED.f ; $(FORTRAN) $(OPTS) -c TMB04ED.f
-TMB04FD.obj: ..\src\MB04FD.f TMB04FD.f ; $(FORTRAN) $(OPTS) -c TMB04FD.f
-TMC01XD.obj: ..\src\MC01XD.f TMC01XD.f ; $(FORTRAN) $(OPTS) -c TMC01XD.f
-TSG02ND.obj: ..\src\SG02ND.f TSG02ND.f ; $(FORTRAN) $(OPTS) -c TSG02ND.f
-TMB03QG.obj: ..\src\MB03QG.f TMB03QG.f ; $(FORTRAN) $(OPTS) -c TMB03QG.f
-TTB01PX.obj: ..\src\TB01PX.f TTB01PX.f ; $(FORTRAN) $(OPTS) -c TTB01PX.f
-TTB01UY.obj: ..\src\TB01UY.f TTB01UY.f ; $(FORTRAN) $(OPTS) -c TTB01UY.f
-TTB01WX.obj: ..\src\TB01WX.f TTB01WX.f ; $(FORTRAN) $(OPTS) -c TTB01WX.f
-TTG01GD.obj: ..\src\TG01GD.f TTG01GD.f ; $(FORTRAN) $(OPTS) -c TTG01GD.f
 TTG01LD.obj: ..\src\TG01LD.f TTG01LD.f ; $(FORTRAN) $(OPTS) -c TTG01LD.f
 TTG01MD.obj: ..\src\TG01MD.f TTG01MD.f ; $(FORTRAN) $(OPTS) -c TTG01MD.f
 TTG01ND.obj: ..\src\TG01ND.f TTG01ND.f ; $(FORTRAN) $(OPTS) -c TTG01ND.f
 TTG01PD.obj: ..\src\TG01PD.f TTG01PD.f ; $(FORTRAN) $(OPTS) -c TTG01PD.f
 TTG01QD.obj: ..\src\TG01QD.f TTG01QD.f ; $(FORTRAN) $(OPTS) -c TTG01QD.f
+TUD01BD.obj: ..\src\UD01BD.f TUD01BD.f ; $(FORTRAN) $(OPTS) -c TUD01BD.f
+TUD01CD.obj: ..\src\UD01CD.f TUD01CD.f ; $(FORTRAN) $(OPTS) -c TUD01CD.f
+TUD01DD.obj: ..\src\UD01DD.f TUD01DD.f ; $(FORTRAN) $(OPTS) -c TUD01DD.f
+TUD01MD.obj: ..\src\UD01MD.f TUD01MD.f ; $(FORTRAN) $(OPTS) -c TUD01MD.f
+TUD01ND.obj: ..\src\UD01ND.f TUD01ND.f ; $(FORTRAN) $(OPTS) -c TUD01ND.f
 
 .f.obj: ; $(FORTRAN) $(OPTS) -c $<
```

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/examples/readme` & `slycot-0.5.4/slycot/src/SLICOT-Reference/examples/readme`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/libindex.html` & `slycot-0.5.4/slycot/src/SLICOT-Reference/libindex.html`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB04MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB04MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB05SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB05SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB07MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB07MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB07ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB07ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08MZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08MZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08NW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08NW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08NX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08NX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08NY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08NY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB08NZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB08NZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09AX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09AX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09BX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09BX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09CX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09CX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09GD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09GD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09HX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09HX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09HY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09HY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09IX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09IX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09IY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09IY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09JD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09JD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09JV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09JV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09JW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09JW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09JX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09JX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09KX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09KX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB09ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB09ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13AX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13AX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13DX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13DX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB13MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB13MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AB8NXZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AB8NXZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AG07BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AG07BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AG08BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AG08BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AG08BY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AG08BY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AG08BZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AG08BZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/AG8BYZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/AG8BYZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/BB01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/BB01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/BB02AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/BB02AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/BB03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/BB03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/BB04AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/BB04AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/BD01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/BD01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/BD02AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/BD02AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/DE01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/DE01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/DE01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/DE01PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/DF01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/DF01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/DG01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/DG01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/DG01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/DG01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/DG01NY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/DG01NY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/DG01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/DG01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/DK01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/DK01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/FB01QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/FB01QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/FB01RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/FB01RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/FB01SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/FB01SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/FB01TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/FB01TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/FB01VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/FB01VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/FD01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/FD01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01MY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01MY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01OY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01OY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01PX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01PX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01PY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01PY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB01RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB01RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/IB03BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/IB03BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA01BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA01BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA01BZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA01BZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA01CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA01CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02AZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02AZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02BZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02BZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02CZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02CZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02ES.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02ES.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02EZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02EZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02GD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02GD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02GZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02GZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02HZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02HZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02IZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02IZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02JD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02JD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02JZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02JZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02MZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02MZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02NZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02NZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02OZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02OZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MA02PZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MA02PZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01LD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01LD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OC.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OC.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OE.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OE.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OH.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OH.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OO.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OO.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01OT.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01OT.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01PD.f`

 * *Files 6% similar despite different names*

```diff
@@ -97,45 +97,41 @@
 C
 C     CONTRIBUTOR
 C
 C     V. Sima, Katholieke Univ. Leuven, Belgium, Nov. 1996.
 C
 C     REVISIONS
 C
-C     Oct. 2001, V. Sima, Research Institute for Informatics, Bucharest.
+C     V. Sima, Oct. 2001, June 2022.
 C
 C    ******************************************************************
 C
 C     .. Parameters ..
       DOUBLE PRECISION   ZERO, ONE
       PARAMETER          ( ZERO = 0.0D0, ONE = 1.0D0 )
 C     .. Scalar Arguments ..
       CHARACTER          SCUN, TYPE
       INTEGER            INFO, KL, KU, LDA, M, MN, N, NBL
       DOUBLE PRECISION   ANRM
 C     .. Array Arguments ..
       INTEGER            NROWS ( * )
       DOUBLE PRECISION   A( LDA, * )
 C     .. Local Scalars ..
-      LOGICAL            FIRST, LSCALE
+      LOGICAL            LSCALE
       INTEGER            I, ISUM, ITYPE
       DOUBLE PRECISION   BIGNUM, SMLNUM
 C     .. External Functions ..
       LOGICAL            LSAME
       DOUBLE PRECISION   DLAMCH
       EXTERNAL           DLAMCH, LSAME
 C     ..
 C     .. External Subroutines ..
       EXTERNAL           DLABAD, MB01QD, XERBLA
 C     .. Intrinsic Functions ..
       INTRINSIC          MAX, MIN
-C     .. Save statement ..
-      SAVE               BIGNUM, FIRST, SMLNUM
-C     .. Data statements ..
-      DATA               FIRST/.TRUE./
 C     ..
 C     .. Executable Statements ..
 C
 C     Test the input scalar arguments.
 C
       INFO = 0
       LSCALE = LSAME( SCUN, 'S' )
@@ -203,23 +199,19 @@
       END IF
 C
 C     Quick return if possible.
 C
       IF( MN.EQ.0 .OR. ANRM.EQ.ZERO )
      $   RETURN
 C
-      IF ( FIRST ) THEN
+C     Get machine parameters.
 C
-C        Get machine parameters.
-C
-         SMLNUM = DLAMCH( 'S' ) / DLAMCH( 'P' )
-         BIGNUM = ONE / SMLNUM
-         CALL DLABAD( SMLNUM, BIGNUM )
-         FIRST = .FALSE.
-      END IF
+      SMLNUM = DLAMCH( 'S' ) / DLAMCH( 'P' )
+      BIGNUM = ONE / SMLNUM
+      CALL DLABAD( SMLNUM, BIGNUM )
 C
       IF ( LSCALE ) THEN
 C
 C        Scale A, if its norm is outside range [SMLNUM,BIGNUM].
 C
          IF( ANRM.LT.SMLNUM ) THEN
 C
```

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RH.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RH.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RT.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RT.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01RY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01RY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01SS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01SS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01UD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01UD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01UW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01UW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01UX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01UX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01UY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01UY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01UZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01UZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01WD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01WD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01XD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01XD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01XY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01XY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01YD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01YD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB01ZD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB01ZD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02CU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02CU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02CV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02CV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02CX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02CX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02CY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02CY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02GD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02GD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02JD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02JD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02JX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02JX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02NY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02NY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02QY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02QY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02RZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02RZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02SZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02SZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02TZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02TZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02UD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02UD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02UU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02UU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02UV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02UV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02UW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02UW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02WD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02WD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02XD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02XD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB02YD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB02YD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AE.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AE.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AF.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AF.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AG.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AG.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AH.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AH.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03AI.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03AI.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BA.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BA.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BC.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BC.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BE.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BE.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BF.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BF.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BG.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BG.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03BZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03BZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03CZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03CZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03DZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03DZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03FZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03FZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03GD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03GD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03GZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03GZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03HZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03HZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03IZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03IZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03JD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03JD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03JP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03JP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03JZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03JZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03KA.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03KA.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03KB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03KB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03KC.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03KC.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03KE.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03KE.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03LD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03LD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03LF.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03LF.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03LP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03LP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03LZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03LZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03MY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03MY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03NY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03NY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03OY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03OY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03PY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03PY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QG.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QG.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03QY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03QY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03RW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03RW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03RX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03RX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03RY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03RY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03RZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03RZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03TS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03TS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03UD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03UD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03VW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03VW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03VY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03VY.f`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 C     German Aerospace Center, DLR Oberpfaffenhofen, February 1999.
 C     Partly based on the routine PSHTR by A. Varga
 C     (DLR Oberpfaffenhofen), November 26, 1995.
 C
 C     REVISIONS
 C
 C     V. Sima, Research Institute for Informatics, Bucharest, Feb. 2004,
-C     July 2012.
+C     July 2012, June 2022.
 C
 C     KEYWORDS
 C
 C     Hessenberg form, orthogonal transformation, periodic systems,
 C     similarity transformation, triangular form.
 C
 C     ******************************************************************
@@ -195,17 +195,20 @@
 C        Generate the orthogonal matrix Q_j.
 C        Set the first ILO-1 and the last N-IHI rows and columns of Q_j
 C        to those of the unit matrix.
 C
          CALL DLASET( 'Full', N, ILO-1, ZERO, ONE, A( 1, 1, J ), LDA1 )
          CALL DLASET( 'Full', ILO-1, NH, ZERO, ZERO, A( 1, ILO, J ),
      $                LDA1 )
-         IF ( NH.GT.1 )
-     $      CALL DORGQR( NH, NH, NH-1, A( ILO, ILO, J ), LDA1,
+         IF ( NH.GT.1 ) THEN
+            CALL DORGQR( NH, NH, NH-1, A( ILO, ILO, J ), LDA1,
      $                   TAU( ILO, J ), DWORK, LDWORK, INFO )
+         ELSE
+            A( ILO, ILO, J ) = ONE
+         END IF
          IF ( IHI.LT.N ) THEN
             CALL DLASET( 'Full', N-IHI, NH, ZERO, ZERO,
      $                   A( IHI+1, ILO, J ), LDA1 )
             CALL DLASET( 'Full', IHI, N-IHI, ZERO, ZERO,
      $                   A( 1, IHI+1, J ), LDA1 )
             CALL DLASET( 'Full', N-IHI, N-IHI, ZERO, ONE,
      $                   A( IHI+1, IHI+1, J ), LDA1 )
```

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03WA.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03WA.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03WD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03WD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03WX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03WX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03XD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03XD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03XP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03XP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03XS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03XS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03XU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03XU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03XZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03XZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03YA.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03YA.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03YD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03YD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03YT.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03YT.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03ZA.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03ZA.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB03ZD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB03ZD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04AZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04AZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04BD.f`

 * *Files 1% similar despite different names*

```diff
@@ -337,15 +337,15 @@
 C     REVISIONS
 C
 C     V. Sima, Oct. 2009 (SLICOT version of the routine DHAUTR).
 C     V. Sima, Nov. 2010, Feb. 2011, Oct. 2011.
 C     M. Voigt, Jan. 2012, July 2014.
 C     V. Sima, Oct. 2012, Jan. 2013, Feb. 2013, July 2013, Aug. 2014,
 C     Sep. 2016, Nov. 2016, Jan. 2017, Apr. 2018, Mar. 2019, Mar. 2020,
-C     Apr. 2020, Apr. 2021.
+C     Apr. 2020, Apr. 2021, July 2022.
 C
 C     KEYWORDS
 C
 C     periodic QZ algorithm, upper (quasi-)triangular matrix,
 C     skew-Hamiltonian/Hamiltonian pencil.
 C
 C     ******************************************************************
@@ -488,15 +488,15 @@
 C
       NINF = 0
       IF( M.EQ.1 ) THEN
          TEMP = ZERO
       ELSE
          TEMP = DLANTR( 'Max', 'Lower', 'No-diag', M-1, M-1, DE( 2, 1 ),
      $                  LDDE, DWORK ) +
-     $          DLANTR( 'Max', 'Upper', 'No-diag', M-1, M-1, DE( 1, 2 ),
+     $          DLANTR( 'Max', 'Upper', 'No-diag', M-1, M-1, DE( 1, 3 ),
      $                  LDDE, DWORK )
       END IF
       IF( TEMP.EQ.ZERO ) THEN
          IF( M.EQ.1 ) THEN
             IF( A( 1, 1 ).EQ.ZERO )
      $         NINF = 1
          ELSE
@@ -506,15 +506,15 @@
      $                                   LDA, DWORK ).EQ.ZERO ) THEN
                DO 10 J = 1, M
                   IF( A( J, J ).EQ.ZERO )
      $               NINF = NINF + 1
    10          CONTINUE
             ELSE
                CALL MA02PD( M, M, A, LDA, I, J )
-               NINF = MAX( I, J )
+               NINF = MAX( I, J )/2
             END IF
          END IF
       ELSE
 C
 C        Incrementing NINF below is due to even multiplicity of
 C        eigenvalues for real skew-Hamiltonian matrices.
 C
```

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04BP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04BP.f`

 * *Files 1% similar despite different names*

```diff
@@ -329,38 +329,42 @@
 C     The algorithm is numerically backward stable and needs O(N ) real
 C     floating point operations.
 C
 C     FURTHER COMMENTS
 C
 C     For large values of N, the routine applies the transformations
 C     for reducing T on panels of columns. The user may specify in INFO
-C     the desired number of columns. If on entry INFO <= 0, then the
-C     routine estimates a suitable value of this number.
+C     the desired number of columns. If on entry INFO < 0, then the
+C     routine estimates a suitable value of this number. If INFO = 0,
+C     the routine MB04BD is directly called.
 C
 C     CONTRIBUTOR
 C
 C     V. Sima, Research Institute for Informatics, Bucharest, July 2011.
 C
 C     REVISIONS
 C
 C     M. Voigt, Jan. 2012, July 2013, June 2014, July 2014.
 C     V. Sima, Oct. 2012, Jan. 2013, Feb. 2013, July 2013, July 2014,
-C     Aug. 2014, June 2015, Jan. 2017, Mar. 2020, Apr. 2020.
+C     Aug. 2014, June 2015, Jan. 2017, Mar. 2020, Apr. 2020, Sep. 2022.
 C
 C     KEYWORDS
 C
 C     periodic QZ algorithm, upper (quasi-)triangular matrix,
 C     skew-Hamiltonian/Hamiltonian pencil.
 C
 C     ******************************************************************
 C
 C     .. Parameters ..
+C     NX is the maximum value of N for which MB04BD can be called.
       DOUBLE PRECISION   ZERO, HALF, ONE, TWO, FIVE
       PARAMETER          ( ZERO = 0.0D+0, HALF = 0.5D+0, ONE = 1.0D+0,
      $                     TWO  = 2.0D+0, FIVE = 5.0D+0 )
+      INTEGER            NX
+      PARAMETER          ( NX = 250 )
 C
 C     .. Scalar Arguments ..
       CHARACTER          COMPQ1, COMPQ2, JOB
       INTEGER            INFO, LDA, LDB, LDC1, LDC2, LDDE, LDF, LDQ1,
      $                   LDQ2, LDVW, LDWORK, LIWORK, N
 C
 C     .. Array Arguments ..
@@ -392,15 +396,15 @@
       DOUBLE PRECISION   DDOT, DLAMCH, DLANTR, DLAPY2
       EXTERNAL           DDOT, DLAMCH, DLANTR, DLAPY2, LSAME, MA02OD
 C
 C     .. External Subroutines ..
       EXTERNAL           DAXPY, DCOPY, DGEMM, DGEQRF, DLACPY, DLARF,
      $                   DLARFG, DLARTG, DLASET, DROT, DSYMV, DSYR2,
      $                   MA02AD, MA02PD, MB01LD, MB01MD, MB01ND, MB03BD,
-     $                   XERBLA
+     $                   MB04BD, XERBLA
 C
 C     .. Intrinsic Functions ..
       INTRINSIC          ABS, DBLE, DCMPLX, DIMAG, INT, MAX, MIN, MOD,
      $                   SQRT
 C
 C     .. Executable Statements ..
 C
@@ -482,15 +486,21 @@
          DWORK( 4 ) = ZERO
          DWORK( 5 ) = ZERO
          RETURN
       END IF
 C
 C     A block algorithm is used for large M.
 C
-      IF( NB.LE.0 ) THEN
+      IF( NB.EQ.0 .OR. ( NB.LT.0 .AND. N.LE.NX ) ) THEN
+         CALL MB04BD( JOB, COMPQ1, COMPQ2, N, A, LDA, DE, LDDE, C1,
+     $                LDC1, VW, LDVW, Q1, LDQ1, Q2, LDQ2, B, LDB, F,
+     $                LDF, C2, LDC2, ALPHAR, ALPHAI, BETA, IWORK,
+     $                LIWORK, DWORK, LDWORK, INFO )
+         RETURN
+      ELSE IF( NB.LT.0 ) THEN
          CALL DGEQRF( M, M, A, LDA, DWORK, DWORK, -1, INFO )
          NB = MIN( MAX( INT( DWORK( 1 ) )/M1, 2 ), M )
       END IF
 C
 C     Determine machine constants.
 C
       BASE = DLAMCH( 'Base' )
@@ -502,15 +512,15 @@
 C
       NINF = 0
       IF( M.EQ.1 ) THEN
          TEMP = ZERO
       ELSE
          TEMP = DLANTR( 'Max', 'Lower', 'No-diag', M-1, M-1, DE( 2, 1 ),
      $                  LDDE, DWORK ) +
-     $          DLANTR( 'Max', 'Upper', 'No-diag', M-1, M-1, DE( 1, 2 ),
+     $          DLANTR( 'Max', 'Upper', 'No-diag', M-1, M-1, DE( 1, 3 ),
      $                  LDDE, DWORK )
       END IF
       IF( TEMP.EQ.ZERO ) THEN
          IF( M.EQ.1 ) THEN
             IF( A( 1, 1 ).EQ.ZERO )
      $         NINF = 1
          ELSE
@@ -520,15 +530,15 @@
      $                                   LDA, DWORK ).EQ.ZERO ) THEN
                DO 10 J = 1, M
                   IF( A( J, J ).EQ.ZERO )
      $               NINF = NINF + 1
    10          CONTINUE
             ELSE
                CALL MA02PD( M, M, A, LDA, I, J )
-               NINF = MAX( I, J )
+               NINF = MAX( I, J )/2
             END IF
          END IF
       ELSE
 C
 C        Incrementing NINF below is due to even multiplicity of
 C        eigenvalues for real skew-Hamiltonian matrices.
 C
```

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04BZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04BZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DI.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DI.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DL.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DL.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04DZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04DZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04FP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04FP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04GD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04GD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04IY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04IY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04IZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04IZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04JD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04JD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04LD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04LD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04NY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04NY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04OW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04OW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04OX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04OX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04OY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04OY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04PA.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04PA.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04PB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04PB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04PU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04PU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04PY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04PY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04QB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04QB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04QC.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04QC.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04QF.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04QF.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04QS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04QS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04QU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04QU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04RB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04RB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04RU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04RU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04SU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04SU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TT.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TT.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04TY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04TY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04UD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04UD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04VX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04VX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04WD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04WD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04WP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04WP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04WR.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04WR.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04WU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04WU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04XD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04XD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04XY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04XY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04YD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04YD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04YW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04YW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB04ZD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB04ZD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB05MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB05MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB05MY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB05MY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB05ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB05ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB05OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB05OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB05OY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB05OY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB3JZP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB3JZP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB3LZP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB3LZP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB3OYZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB3OYZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB3PYZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB3PYZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB4DBZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB4DBZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB4DLZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB4DLZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MB4DPZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MB4DPZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01PY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01PY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01SW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01SW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01SX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01SX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01SY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01SY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01WD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01WD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC01XD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC01XD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC03MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC03MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC03ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC03ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC03NX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC03NX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MC03NY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MC03NY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BA.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BA.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BF.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BF.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/MD03BY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/MD03BY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01AY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01AY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BA.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BA.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BE.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BE.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BF.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BF.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BQ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BQ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BR.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BR.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/NF01BY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/NF01BY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01BX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01BX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01BY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01BY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01FY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01FY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02CX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02CX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MR.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MR.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MT.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MT.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02MX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02MX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02OY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02OY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02RU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02RU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB02SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB02SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03MY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03MY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OR.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OR.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OT.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OT.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03OZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03OZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03QX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03QX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03QY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03QY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03SX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03SX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03SY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03SY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB03UD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB03UD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04MR.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04MR.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04MU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04MU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04MW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04MW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04MY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04MY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04NV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04NV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04NW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04NW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04NX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04NX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04NY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04NY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04OW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04OW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04PX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04PX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04PY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04PY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04QR.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04QR.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04QU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04QU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04QY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04QY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04RV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04RV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04RW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04RW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04RX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04RX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB04RY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB04RY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB06ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB06ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08GD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08GD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08MY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08MY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB08NY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB08NY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB09MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB09MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10JD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10JD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10LD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10LD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10SD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10SD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10UD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10UD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10WD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10WD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10YD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10YD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10ZD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10ZD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB10ZP.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB10ZP.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB16AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB16AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB16AY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB16AY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB16BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB16BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB16CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB16CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SB16CY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SB16CY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG02AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG02AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG02CV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG02CV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG02CW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG02CW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG02CX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG02CX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG02ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG02ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03AX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03AX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03AY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03AY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BR.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BR.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BS.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BS.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BT.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BT.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SG03BZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SG03BZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SLCT_DLATZM.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SLCT_DLATZM.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/SLCT_ZLATZM.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/SLCT_ZLATZM.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01IZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01IZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01KX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01KX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01LD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01LD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01PX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01PX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01TD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01TD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01TY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01TY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01UD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01UD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01UX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01UX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01UY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01UY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01VD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01VD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01VY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01VY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01WD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01WD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01WX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01WX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01XD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01XD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01XZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01XZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01YD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01YD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB01ZD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB01ZD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB03AY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB03AY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04AY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04AY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04BV.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04BV.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04BW.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04BW.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04BX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04BX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB04CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB04CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TB05AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TB05AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TC01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TC01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TC04AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TC04AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TC05AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TC05AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TD03AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TD03AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TD03AY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TD03AY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TD04AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TD04AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TD05AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TD05AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01MX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01MX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01MY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01MY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TF01RD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TF01RD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01AD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01AD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01AZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01AZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01ED.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01ED.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01FD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01FD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01FZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01FZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01GD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01GD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01HD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01HD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01HU.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01HU.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01HX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01HX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01HY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01HY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01ID.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01ID.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01JD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01JD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01JY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01JY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01KD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01KD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01KZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01KZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01LD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01LD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01LY.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01LY.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01NX.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01NX.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01OA.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01OA.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01OB.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01OB.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01OD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01OD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01OZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01OZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01PD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01PD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01QD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01QD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/TG01WD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/TG01WD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01BD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01BD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01CD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01CD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01DD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01DD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01MZ.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01MZ.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/UD01ND.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/UD01ND.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/UE01MD.f` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/UE01MD.f`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/SLICOT-Reference/src/makefile` & `slycot-0.5.4/slycot/src/SLICOT-Reference/src/makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 ####################################################################
 #  SLICOT routines makefile                                        #
 #  Makefile for creating/updating the SLICOT Library object file   # 
 #  on Windows platforms.                                           #
-#  SLICOT, Release 4.0                      .\slicot\src\makefile  #
-#  Vasile Sima, KU Leuven                                          #
+#  SLICOT, Release 5.8                      .\slicot\src\makefile  #
+#  Vasile Sima                                                     #
 #  October 31, 1996.                                               #
 #  Revised December 23, 1999, ..., Oct. 4, 2001, Aug. 25, 2003,    #
 #          Jan. 9, 2009, Nov. 17, 2010, Sep. 25, 2012,             #
-#          May 08, 2015, Jan. 2017                                 #
+#          May 08, 2015, Jan. 2017, Dec. 2022                      #
 ####################################################################
 #
 #  This is the makefile to create/update the library for SLICOT.
-#  The SLICOT Library routines are written for double precision only.
+#  Most SLICOT Library routines are written for double precision.
+#  Some routines have COMPLEX*16 variants.
 #
 #  The command
 #       nmake
 #  without any arguments creates or updates a library called
 #       slicot.lib
 #  in the next higher directory level.
 #
@@ -24,110 +25,109 @@
 #
 #######################################################################
  
 !include <..\make.inc>
 
 .SUFFIXES: .f .obj
 
-DSLSRC = \
+SLSRC = \
     AB01MD.obj AB01ND.obj AB01OD.obj AB04MD.obj AB05MD.obj AB05ND.obj AB05OD.obj \
     AB05PD.obj AB05QD.obj AB05RD.obj AB05SD.obj AB07MD.obj AB07ND.obj AB08MD.obj \
-    AB08ND.obj AB08NX.obj AB09AD.obj AB09AX.obj AB09BD.obj AB09BX.obj AB09CD.obj \
-    AB09CX.obj AB09DD.obj AB09ED.obj AB09FD.obj AB09GD.obj AB09HD.obj AB09HX.obj \
-    AB09HY.obj AB09ID.obj AB09IX.obj AB09IY.obj AB09JD.obj AB09JV.obj AB09JW.obj \
-    AB09JX.obj AB09KD.obj AB09KX.obj AB09MD.obj AB09ND.obj AB13AD.obj AB13AX.obj \
-    AB13BD.obj AB13CD.obj AB13DD.obj AB13DX.obj AB13ED.obj AB13FD.obj AB13ID.obj \
-    AB13MD.obj AG07BD.obj AG08BD.obj AG08BY.obj \
+    AB08MZ.obj AB08ND.obj AB08NW.obj AB08NX.obj AB08NY.obj AB08NZ.obj AB09AD.obj \
+    AB09AX.obj AB09BD.obj AB09BX.obj AB09CD.obj AB09CX.obj AB09DD.obj AB09ED.obj \
+    AB09FD.obj AB09GD.obj AB09HD.obj AB09HX.obj AB09HY.obj AB09ID.obj AB09IX.obj \
+    AB09IY.obj AB09JD.obj AB09JV.obj AB09JW.obj AB09JX.obj AB09KD.obj AB09KX.obj \
+    AB09MD.obj AB09ND.obj AB13AD.obj AB13AX.obj AB13BD.obj AB13CD.obj AB13DD.obj \
+    AB13DX.obj AB13ED.obj AB13FD.obj AB13ID.obj AB13MD.obj AB8NXZ.obj AG07BD.obj \
+    AG08BD.obj AG08BY.obj AG08BZ.obj AG8BYZ.obj \
     BB01AD.obj BB02AD.obj BB03AD.obj BB04AD.obj BD01AD.obj BD02AD.obj \
-    DE01OD.obj DE01PD.obj DF01MD.obj DG01MD.obj DG01ND.obj DG01NY.obj DG01OD.obj \
-    DK01MD.obj delctg.obj \
+    DE01OD.obj DE01PD.obj delctg.obj DF01MD.obj DG01MD.obj DG01ND.obj DG01NY.obj \
+    DG01OD.obj DK01MD.obj \
     FB01QD.obj FB01RD.obj FB01SD.obj FB01TD.obj FB01VD.obj FD01AD.obj \
     IB01AD.obj IB01BD.obj IB01CD.obj IB01MD.obj IB01MY.obj IB01ND.obj IB01OD.obj \
-    IB01OY.obj IB01PD.obj IB01PX.obj IB01PY.obj IB01QD.obj IB01RD.obj \
-    IB03AD.obj IB03BD.obj \
-    MA01AD.obj MA02AD.obj MA02BD.obj MA02CD.obj MA02DD.obj MA02ED.obj MA02FD.obj \
-    MA02GD.obj MB01PD.obj MB01QD.obj MB01RD.obj MB01RU.obj MB01RW.obj MB01RX.obj \
-    MB01RY.obj MB01SD.obj MB01TD.obj MB01UD.obj MB01UW.obj MB01VD.obj MB01WD.obj \
-    MB01XD.obj MB01XY.obj MB01YD.obj MB01ZD.obj MB02CD.obj MB02CU.obj MB02CV.obj \
-    MB02CX.obj MB02CY.obj MB02DD.obj MB02ED.obj MB02FD.obj MB02GD.obj MB02HD.obj \
-    MB02ID.obj MB02JD.obj MB02JX.obj MB02KD.obj MB02MD.obj MB02ND.obj MB02NY.obj \
-    MB02OD.obj MB02PD.obj MB02QD.obj MB02QY.obj MB02RD.obj MB02RZ.obj MB02SD.obj \
-    MB02SZ.obj MB02TD.obj MB02TZ.obj MB02UD.obj MB02UU.obj MB02UV.obj MB02VD.obj \
-    MB02WD.obj MB02XD.obj MB02YD.obj MB01SS.obj \
+    IB01OY.obj IB01PD.obj IB01PX.obj IB01PY.obj IB01QD.obj IB01RD.obj IB03AD.obj \
+    IB03BD.obj \
+    MA01AD.obj MA01BD.obj MA01BZ.obj MA01CD.obj MA02AD.obj MA02AZ.obj MA02BD.obj \
+    MA02BZ.obj MA02CD.obj MA02CZ.obj MA02DD.obj MA02ED.obj MA02ES.obj MA02EZ.obj \
+    MA02FD.obj MA02GD.obj MA02GZ.obj MA02HD.obj MA02HZ.obj MA02ID.obj MA02IZ.obj \
+    MA02JD.obj MA02JZ.obj MA02MD.obj MA02MZ.obj MA02NZ.obj MA02OD.obj MA02OZ.obj \
+    MA02PD.obj MA02PZ.obj MB01KD.obj MB01LD.obj MB01MD.obj MB01ND.obj MB01OC.obj \
+    MB01OD.obj MB01OE.obj MB01OH.obj MB01OO.obj MB01OS.obj MB01OT.obj MB01PD.obj \
+    MB01QD.obj MB01RB.obj MB01RD.obj MB01RH.obj MB01RT.obj MB01RU.obj MB01RW.obj \
+    MB01RX.obj MB01RY.obj MB01SD.obj MB01SS.obj MB01TD.obj MB01UD.obj MB01UW.obj \
+    MB01UX.obj MB01UY.obj MB01UZ.obj MB01VD.obj MB01WD.obj MB01XD.obj MB01XY.obj \
+    MB01YD.obj MB01ZD.obj MB02CD.obj MB02CU.obj MB02CV.obj MB02CX.obj MB02CY.obj \
+    MB02DD.obj MB02ED.obj MB02FD.obj MB02GD.obj MB02HD.obj MB02ID.obj MB02JD.obj \
+    MB02JX.obj MB02KD.obj MB02MD.obj MB02ND.obj MB02NY.obj MB02OD.obj MB02PD.obj \
+    MB02QD.obj MB02QY.obj MB02RD.obj MB02RZ.obj MB02SD.obj MB02SZ.obj MB02TD.obj \
+    MB02TZ.obj MB02UD.obj MB02UU.obj MB02UV.obj MB02UW.obj MB02VD.obj MB02WD.obj \
+    MB02XD.obj MB02YD.obj MB03AB.obj MB03AD.obj MB03AE.obj MB03AF.obj MB03AG.obj \
+    MB03AH.obj MB03AI.obj MB03BA.obj MB03BB.obj MB03BC.obj MB03BD.obj MB03BE.obj \
+    MB03BF.obj MB03BG.obj MB03BZ.obj MB03CD.obj MB03CZ.obj MB03DD.obj MB03DZ.obj \
+    MB03ED.obj MB03FD.obj MB03FZ.obj MB03GD.obj MB03GZ.obj MB03HD.obj MB03HZ.obj \
+    MB03ID.obj MB03IZ.obj MB03JD.obj MB03JP.obj MB03JZ.obj MB03KA.obj MB03KB.obj \
+    MB03KC.obj MB03KD.obj MB03KE.obj MB03LD.obj MB03LF.obj MB03LP.obj MB03LZ.obj \
     MB03MD.obj MB03MY.obj MB03ND.obj MB03NY.obj MB03OD.obj MB03OY.obj MB03PD.obj \
-    MB03PY.obj MB03QD.obj MB03QX.obj MB03QY.obj MB03RD.obj MB03RX.obj MB03RY.obj \
-    MB03SD.obj MB03UD.obj MB03VD.obj MB03VY.obj MB03WD.obj MB03WX.obj MB04DY.obj \
-    MB04GD.obj MB04ID.obj MB04IY.obj MB04JD.obj MB04KD.obj MB04LD.obj MB04MD.obj \
-    MB04ND.obj MB04NY.obj MB04OD.obj MB04OW.obj MB04OX.obj MB04OY.obj MB04PY.obj \
+    MB03PY.obj MB03QD.obj MB03QG.obj MB03QV.obj MB03QW.obj MB03QX.obj MB03QY.obj \
+    MB03RD.obj MB03RW.obj MB03RX.obj MB03RY.obj MB03RZ.obj MB03SD.obj MB03TD.obj \
+    MB03TS.obj MB03UD.obj MB03VD.obj MB03VW.obj MB03VY.obj MB03WA.obj MB03WD.obj \
+    MB03WX.obj MB03XD.obj MB03XP.obj MB03XS.obj MB03XU.obj MB03XZ.obj MB03YA.obj \
+    MB03YD.obj MB03YT.obj MB03ZA.obj MB03ZD.obj MB04AD.obj MB04AZ.obj MB04BD.obj \
+    MB04BP.obj MB04BZ.obj MB04CD.obj MB04DB.obj MB04DD.obj MB04DI.obj MB04DL.obj \
+    MB04DP.obj MB04DS.obj MB04DY.obj MB04DZ.obj MB04ED.obj MB04FD.obj MB04FP.obj \
+    MB04GD.obj MB04HD.obj MB04ID.obj MB04IY.obj MB04IZ.obj MB04JD.obj MB04KD.obj \
+    MB04LD.obj MB04MD.obj MB04ND.obj MB04NY.obj MB04OD.obj MB04OW.obj MB04OX.obj \
+    MB04OY.obj MB04PA.obj MB04PB.obj MB04PU.obj MB04PY.obj MB04QB.obj MB04QC.obj \
+    MB04QF.obj MB04QS.obj MB04QU.obj MB04RB.obj MB04RD.obj MB04RS.obj MB04RT.obj \
+    MB04RU.obj MB04RV.obj MB04RW.obj MB04RZ.obj MB04SU.obj MB04TB.obj MB04TS.obj \
     MB04TT.obj MB04TU.obj MB04TV.obj MB04TW.obj MB04TX.obj MB04TY.obj MB04UD.obj \
-    MB04VD.obj MB04VX.obj MB04XD.obj MB04XY.obj MB04YD.obj MB04YW.obj MB04ZD.obj \
-    MB05MD.obj MB05MY.obj MB05ND.obj MB05OD.obj MB05OY.obj \
-    MC01MD.obj MC01ND.obj MC01OD.obj MC01PD.obj MC01PY.obj MC01QD.obj MC01RD.obj \
-    MC01SD.obj MC01SW.obj MC01SX.obj MC01SY.obj MC01TD.obj MC01VD.obj MC01WD.obj \
-    MC03MD.obj MC03ND.obj MC03NX.obj MC03NY.obj \
+    MB04VD.obj MB04VX.obj MB04WD.obj MB04WP.obj MB04WR.obj MB04WU.obj MB04XD.obj \
+    MB04XY.obj MB04YD.obj MB04YW.obj MB04ZD.obj MB05MD.obj MB05MY.obj MB05ND.obj \
+    MB05OD.obj MB05OY.obj MB3JZP.obj MB3LZP.obj MB3OYZ.obj MB3PYZ.obj MB4DBZ.obj \
+    MB4DLZ.obj MB4DPZ.obj MC01MD.obj MC01ND.obj MC01OD.obj MC01PD.obj MC01PY.obj \
+    MC01QD.obj MC01RD.obj MC01SD.obj MC01SW.obj MC01SX.obj MC01SY.obj MC01TD.obj \
+    MC01VD.obj MC01WD.obj MC01XD.obj MC03MD.obj MC03ND.obj MC03NX.obj MC03NY.obj \
     MD03AD.obj MD03BA.obj MD03BB.obj MD03BD.obj MD03BF.obj MD03BX.obj MD03BY.obj \
     NF01AD.obj NF01AY.obj NF01BA.obj NF01BB.obj NF01BD.obj NF01BE.obj NF01BF.obj \
     NF01BP.obj NF01BQ.obj NF01BR.obj NF01BS.obj NF01BU.obj NF01BV.obj NF01BW.obj \
     NF01BX.obj NF01BY.obj \
     SB01BD.obj SB01BX.obj SB01BY.obj SB01DD.obj SB01FY.obj SB01MD.obj SB02CX.obj \
     SB02MD.obj SB02MR.obj SB02MS.obj SB02MT.obj SB02MU.obj SB02MV.obj SB02MW.obj \
-    SB02ND.obj SB02OD.obj SB02OU.obj SB02OV.obj SB02OW.obj SB02OX.obj SB02OY.obj \
-    SB02PD.obj SB02QD.obj SB02RD.obj SB02RU.obj SB02SD.obj SB03MD.obj SB03MU.obj \
-    SB03MV.obj SB03MW.obj SB03MX.obj SB03MY.obj SB03OD.obj SB03OR.obj SB03OT.obj \
-    SB03OU.obj SB03OV.obj SB03OY.obj SB03PD.obj SB03QD.obj SB03QX.obj SB03QY.obj \
-    SB03RD.obj SB03SD.obj SB03SX.obj SB03SY.obj SB03TD.obj SB03UD.obj SB04MD.obj \
-    SB04MR.obj SB04MU.obj SB04MW.obj SB04MY.obj SB04ND.obj SB04NV.obj SB04NW.obj \
-    SB04NX.obj SB04NY.obj SB04OD.obj SB04PD.obj SB04PX.obj SB04PY.obj SB04QD.obj \
-    SB04QR.obj SB04QU.obj SB04QY.obj SB04RD.obj SB04RV.obj SB04RW.obj SB04RX.obj \
-    SB04RY.obj SB06ND.obj SB08CD.obj SB08DD.obj SB08ED.obj SB08FD.obj SB08GD.obj \
-    SB08HD.obj SB08MD.obj SB08MY.obj SB08ND.obj SB08NY.obj SB09MD.obj SB10AD.obj \
-    SB10DD.obj SB10ED.obj SB10FD.obj SB10HD.obj SB10ID.obj SB10JD.obj SB10KD.obj \
-    SB10LD.obj SB10MD.obj SB10PD.obj SB10QD.obj SB10RD.obj SB10SD.obj SB10TD.obj \
-    SB10UD.obj SB10VD.obj SB10WD.obj SB10YD.obj SB10ZD.obj SB10ZP.obj SB16AD.obj \
-    SB16AY.obj SB16BD.obj SB16CD.obj SB16CY.obj SG02AD.obj SG03AD.obj SG03AX.obj \
-    SG03AY.obj SG03BD.obj SG03BU.obj SG03BV.obj SG03BW.obj SG03BX.obj SG03BY.obj \
-    TB01ID.obj TB01KD.obj TB01LD.obj TB01MD.obj TB01ND.obj TB01PD.obj TB01TD.obj \
-    TB01TY.obj TB01UD.obj TB01VD.obj TB01VY.obj TB01WD.obj TB01XD.obj TB01YD.obj \
+    SB02MX.obj SB02ND.obj SB02OD.obj SB02OU.obj SB02OV.obj SB02OW.obj SB02OX.obj \
+    SB02OY.obj SB02PD.obj SB02QD.obj SB02RD.obj SB02RU.obj SB02SD.obj SB03MD.obj \
+    SB03MU.obj SB03MV.obj SB03MW.obj SB03MX.obj SB03MY.obj SB03OD.obj SB03OR.obj \
+    SB03OS.obj SB03OT.obj SB03OU.obj SB03OV.obj SB03OY.obj SB03OZ.obj SB03PD.obj \
+    SB03QD.obj SB03QX.obj SB03QY.obj SB03RD.obj SB03SD.obj SB03SX.obj SB03SY.obj \
+    SB03TD.obj SB03UD.obj SB04MD.obj SB04MR.obj SB04MU.obj SB04MW.obj SB04MY.obj \
+    SB04ND.obj SB04NV.obj SB04NW.obj SB04NX.obj SB04NY.obj SB04OD.obj SB04OW.obj \
+    SB04PD.obj SB04PX.obj SB04PY.obj SB04QD.obj SB04QR.obj SB04QU.obj SB04QY.obj \
+    SB04RD.obj SB04RV.obj SB04RW.obj SB04RX.obj SB04RY.obj SB06ND.obj SB08CD.obj \
+    SB08DD.obj SB08ED.obj SB08FD.obj SB08GD.obj SB08HD.obj SB08MD.obj SB08MY.obj \
+    SB08ND.obj SB08NY.obj SB09MD.obj SB10AD.obj SB10DD.obj SB10ED.obj SB10FD.obj \
+    SB10HD.obj SB10ID.obj SB10JD.obj SB10KD.obj SB10LD.obj SB10MD.obj SB10PD.obj \
+    SB10QD.obj SB10RD.obj SB10SD.obj SB10TD.obj SB10UD.obj SB10VD.obj SB10WD.obj \
+    SB10YD.obj SB10ZD.obj SB10ZP.obj SB16AD.obj SB16AY.obj SB16BD.obj SB16CD.obj \
+    SB16CY.obj select.obj SG02AD.obj SG02CV.obj SG02CW.obj SG02CX.obj SG02ND.obj \
+    SG03AD.obj SG03AX.obj SG03AY.obj SG03BD.obj SG03BR.obj SG03BS.obj SG03BT.obj \
+    SG03BU.obj SG03BV.obj SG03BW.obj SG03BX.obj SG03BY.obj SG03BZ.obj \
+    TB01ID.obj TB01IZ.obj TB01KD.obj TB01KX.obj TB01LD.obj TB01MD.obj TB01ND.obj \
+    TB01PD.obj TB01PX.obj TB01TD.obj TB01TY.obj TB01UD.obj TB01UX.obj TB01UY.obj \
+    TB01VD.obj TB01VY.obj TB01WD.obj TB01WX.obj TB01XD.obj TB01XZ.obj TB01YD.obj \
     TB01ZD.obj TB03AD.obj TB03AY.obj TB04AD.obj TB04AY.obj TB04BD.obj TB04BV.obj \
     TB04BW.obj TB04BX.obj TB04CD.obj TB05AD.obj TC01OD.obj TC04AD.obj TC05AD.obj \
-    TD03AD.obj TD03AY.obj TD04AD.obj TD05AD.obj \
-    TF01MD.obj TF01MX.obj TF01MY.obj TF01ND.obj TF01OD.obj TF01PD.obj TF01QD.obj \
-    TF01RD.obj TG01AD.obj TG01CD.obj TG01DD.obj TG01ED.obj TG01FD.obj TG01HD.obj \
-    TG01HX.obj TG01HY.obj TG01ID.obj TG01JD.obj TG01JY.obj \
-    UD01BD.obj UD01CD.obj UD01DD.obj UD01MD.obj UD01ND.obj select.obj \
-    MA02HD.obj TG01BD.obj TG01WD.obj \
-    MA02ID.obj MA02JD.obj MB01MD.obj MB01ND.obj MB01UX.obj MB03TD.obj MB03TS.obj \
-    MB03WA.obj MB03XD.obj MB03XP.obj MB03XU.obj MB03YA.obj MB03YD.obj MB03YT.obj \
-    MB03ZA.obj MB03ZD.obj MB04DD.obj MB04DI.obj MB04DS.obj MB04PA.obj MB04PB.obj \
-    MB04PU.obj MB04QB.obj MB04QC.obj MB04QF.obj MB04QU.obj MB04TB.obj MB04TS.obj \
-    MB04WD.obj MB04WP.obj MB04WR.obj MB04WU.obj SB04OW.obj UE01MD.obj UD01MZ.obj \
-    AB08MZ.obj AB08NZ.obj AB8NXZ.obj AG08BZ.obj AG8BYZ.obj MA02BZ.obj MA02CZ.obj \
-    MB04IZ.obj MB3OYZ.obj MB3PYZ.obj TB01IZ.obj TB01XZ.obj TG01AZ.obj TG01FZ.obj \
-    MA01BD.obj MA01CD.obj MB01KD.obj MB01LD.obj MB02UW.obj MB03AD.obj MB03BA.obj \
-    MB03BB.obj MB03BC.obj MB03BD.obj MB03BE.obj MB03CD.obj MB03DD.obj MB03ED.obj \
-    MB03FD.obj MB03GD.obj MB03HD.obj MB03ID.obj MB03JD.obj MB03KA.obj MB03KB.obj \
-    MB03KC.obj MB03KD.obj MB03KE.obj MB03LD.obj MB04AD.obj MB04BD.obj MB04HD.obj \
-    MB04SU.obj MB04CD.obj MB04ED.obj MB04FD.obj MA01BZ.obj MA02GZ.obj MB03BZ.obj \
-    MB03CZ.obj MB03DZ.obj MB03FZ.obj MB03GZ.obj MB03HZ.obj MB03IZ.obj MB03JZ.obj \
-    MB03LF.obj MB03LZ.obj MB03XS.obj MB03XZ.obj MB04QS.obj MB04RB.obj MB04RU.obj \
-    MB04BZ.obj MA02IZ.obj MB04DZ.obj MB04FP.obj MB04AZ.obj MA02ES.obj MA02EZ.obj \
-    MA02JZ.obj MB01RB.obj MC01XD.obj SB02MX.obj SG02CW.obj SG02CX.obj SG02ND.obj \
-    MB03JP.obj MB03LP.obj MB3JZP.obj MB3LZP.obj MB04BP.obj MA02HZ.obj MA02MD.obj \
-    MB03QG.obj MB03QV.obj MB03QW.obj TB01KX.obj TB01PX.obj TB01UX.obj TB01UY.obj \
-    TB01WX.obj TG01GD.obj TG01HU.obj TG01LD.obj TG01LY.obj TG01MD.obj TG01ND.obj \
-    TG01NX.obj TG01PD.obj TG01QD.obj AB08NW.obj AB08NY.obj \
-    MA02MZ.obj MA02NZ.obj MA02OD.obj MA02OZ.obj MA02PD.obj MA02PZ.obj MB01OC.obj \
-    MB04DB.obj MB4DBZ.obj MB04DL.obj MB4DLZ.obj MB04DP.obj MB4DPZ.obj MB03AF.obj \
-    MB03AG.obj MB03BF.obj MB03BG.obj MB01OD.obj MB01OE.obj MB01OH.obj MB01OO.obj \
-    MB01OS.obj MB01OT.obj MB01RH.obj MB01RT.obj SG02CV.obj MB03AB.obj MB03AE.obj \
-    MB03AH.obj MB03AI.obj 
+    TD03AD.obj TD03AY.obj TD04AD.obj TD05AD.obj TF01MD.obj TF01MX.obj TF01MY.obj \
+    TF01ND.obj TF01OD.obj TF01PD.obj TF01QD.obj TF01RD.obj TG01AD.obj TG01AZ.obj \
+    TG01BD.obj TG01CD.obj TG01DD.obj TG01ED.obj TG01FD.obj TG01FZ.obj TG01GD.obj \
+    TG01HD.obj TG01HU.obj TG01HX.obj TG01HY.obj TG01ID.obj TG01JD.obj TG01JY.obj \
+    TG01KD.obj TG01KZ.obj TG01LD.obj TG01LY.obj TG01MD.obj TG01ND.obj TG01NX.obj \
+    TG01OA.obj TG01OB.obj TG01OD.obj TG01OZ.obj TG01PD.obj TG01QD.obj TG01WD.obj \
+    UD01BD.obj UD01CD.obj UD01DD.obj UD01MD.obj UD01MZ.obj UD01ND.obj UE01MD.obj \
+    zelctg.obj
 
-all: double
-
-double: $(DSLSRC)
-	$(ARCH) $(ARCHFLAGS):$(SLICOTLIB) $(DSLSRC)
+all: 	$(SLSRC)
+	$(ARCH) $(ARCHFLAGS):$(SLICOTLIB) $(SLSRC)
 
 clean:
 	del *.obj
 
 .f.obj:
 	$(FORTRAN) $(OPTS) -c $<
```

### Comparing `slycot-0.5.3/slycot/src/analysis.pyf` & `slycot-0.5.4/slycot/src/analysis.pyf`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/math.pyf` & `slycot-0.5.4/slycot/src/math.pyf`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/synthesis.pyf` & `slycot-0.5.4/slycot/src/synthesis.pyf`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/src/transform.pyf` & `slycot-0.5.4/slycot/src/transform.pyf`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/synthesis.py` & `slycot-0.5.4/slycot/synthesis.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_ab01.py` & `slycot-0.5.4/slycot/tests/test_ab01.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_ab08n.py` & `slycot-0.5.4/slycot/tests/test_ab08n.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_ab13md.py` & `slycot-0.5.4/slycot/tests/test_ab13md.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_ag08bd.py` & `slycot-0.5.4/slycot/tests/test_ag08bd.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_analysis.py` & `slycot-0.5.4/slycot/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_examples.py` & `slycot-0.5.4/slycot/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_exceptions.py` & `slycot-0.5.4/slycot/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_mb.py` & `slycot-0.5.4/slycot/tests/test_mb.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_mc.py` & `slycot-0.5.4/slycot/tests/test_mc.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_sb.py` & `slycot-0.5.4/slycot/tests/test_sb.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_sg02ad.py` & `slycot-0.5.4/slycot/tests/test_sg02ad.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_sg03ad.py` & `slycot-0.5.4/slycot/tests/test_sg03ad.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_tb05ad.py` & `slycot-0.5.4/slycot/tests/test_tb05ad.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_td04ad.py` & `slycot-0.5.4/slycot/tests/test_td04ad.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_tg01ad.py` & `slycot-0.5.4/slycot/tests/test_tg01ad.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_tg01fd.py` & `slycot-0.5.4/slycot/tests/test_tg01fd.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/tests/test_transform.py` & `slycot-0.5.4/slycot/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot/transform.py` & `slycot-0.5.4/slycot/transform.py`

 * *Files identical despite different names*

### Comparing `slycot-0.5.3/slycot.egg-info/PKG-INFO` & `slycot-0.5.4/slycot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slycot
-Version: 0.5.3
+Version: 0.5.4
 Summary: A wrapper for the SLICOT control and systems library
 Author: Enrico Avventi et al.
 Maintainer-email: Slycot developers <python-control-discuss@lists.sourceforge.net>
 License: GPL-2.0 AND BSD-3-Clause
 Project-URL: homepage, https://github.com/python-control/Slycot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -23,14 +23,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: COPYING
 License-File: AUTHORS
 
 Slycot
 ======
 
 .. image:: https://img.shields.io/pypi/v/slycot.svg
    :target: https://pypi.org/project/slycot/
```

### Comparing `slycot-0.5.3/slycot.egg-info/SOURCES.txt` & `slycot-0.5.4/slycot.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -39,18 +39,23 @@
 slycot/src/analysis.pyf
 slycot/src/ftruefalse.f
 slycot/src/math.pyf
 slycot/src/synthesis.pyf
 slycot/src/transform.pyf
 slycot/src/SLICOT-Reference/.git
 slycot/src/SLICOT-Reference/Contributors.md
+slycot/src/SLICOT-Reference/Installation.md
 slycot/src/SLICOT-Reference/LICENSE
 slycot/src/SLICOT-Reference/README.md
 slycot/src/SLICOT-Reference/ReleaseNotes.md
 slycot/src/SLICOT-Reference/libindex.html
+slycot/src/SLICOT-Reference/make.inc
+slycot/src/SLICOT-Reference/make_Unix.inc
+slycot/src/SLICOT-Reference/makefile
+slycot/src/SLICOT-Reference/makefile_Unix
 slycot/src/SLICOT-Reference/benchmark_data/BB01103.dat
 slycot/src/SLICOT-Reference/benchmark_data/BB01104.dat
 slycot/src/SLICOT-Reference/benchmark_data/BB01105.dat
 slycot/src/SLICOT-Reference/benchmark_data/BB01106.dat
 slycot/src/SLICOT-Reference/benchmark_data/BB012091.dat
 slycot/src/SLICOT-Reference/benchmark_data/BB012092.dat
 slycot/src/SLICOT-Reference/benchmark_data/BB01404.dat
@@ -1386,14 +1391,15 @@
 slycot/src/SLICOT-Reference/examples/UD01DD.dat
 slycot/src/SLICOT-Reference/examples/UD01DD.res
 slycot/src/SLICOT-Reference/examples/UD01MD.dat
 slycot/src/SLICOT-Reference/examples/UD01MD.res
 slycot/src/SLICOT-Reference/examples/UD01ND.dat
 slycot/src/SLICOT-Reference/examples/UD01ND.res
 slycot/src/SLICOT-Reference/examples/makefile
+slycot/src/SLICOT-Reference/examples/makefile_Unix
 slycot/src/SLICOT-Reference/examples/readme
 slycot/src/SLICOT-Reference/src/AB01MD.f
 slycot/src/SLICOT-Reference/src/AB01ND.f
 slycot/src/SLICOT-Reference/src/AB01OD.f
 slycot/src/SLICOT-Reference/src/AB04MD.f
 slycot/src/SLICOT-Reference/src/AB05MD.f
 slycot/src/SLICOT-Reference/src/AB05ND.f
@@ -1998,16 +2004,22 @@
 slycot/src/SLICOT-Reference/src/UD01DD.f
 slycot/src/SLICOT-Reference/src/UD01MD.f
 slycot/src/SLICOT-Reference/src/UD01MZ.f
 slycot/src/SLICOT-Reference/src/UD01ND.f
 slycot/src/SLICOT-Reference/src/UE01MD.f
 slycot/src/SLICOT-Reference/src/delctg.f
 slycot/src/SLICOT-Reference/src/makefile
+slycot/src/SLICOT-Reference/src/makefile_Unix
 slycot/src/SLICOT-Reference/src/readme
 slycot/src/SLICOT-Reference/src/select.f
+slycot/src/SLICOT-Reference/src_aux/dlatzm.f
+slycot/src/SLICOT-Reference/src_aux/makefile
+slycot/src/SLICOT-Reference/src_aux/makefile_Unix
+slycot/src/SLICOT-Reference/src_aux/readme
+slycot/src/SLICOT-Reference/src_aux/zlatzm.f
 slycot/tests/CMakeLists.txt
 slycot/tests/__init__.py
 slycot/tests/test_ab01.py
 slycot/tests/test_ab08n.py
 slycot/tests/test_ab13md.py
 slycot/tests/test_ag08bd.py
 slycot/tests/test_analysis.py
```


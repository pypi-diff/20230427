# Comparing `tmp/ocsmesh-1.2.1.tar.gz` & `tmp/ocsmesh-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocsmesh-1.2.1.tar", last modified: Fri Mar 24 19:47:15 2023, max compression
+gzip compressed data, was "ocsmesh-1.3.0.tar", last modified: Thu Apr 27 18:48:01 2023, max compression
```

## Comparing `ocsmesh-1.2.1.tar` & `ocsmesh-1.3.0.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.321700 ocsmesh-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.301700 ocsmesh-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.305700 ocsmesh-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/.github/workflows/functional_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/.github/workflows/functional_test_2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-03-24 19:47:15.325700 ocsmesh-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.309700 ocsmesh-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)  2851126 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/docs/noaa_33879_DS1.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.313700 ocsmesh-1.2.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/docs/source/ocsmesh.command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/docs/source/ocsmesh.geometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/docs/source/ocsmesh.mesh.rst
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/docs/source/ocsmesh.size_function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/docs/source/ocsmesh.utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.313700 ocsmesh-1.2.1/ocsmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.317700 ocsmesh-1.2.1/ocsmesh/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/cli/mesh_upgrader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/cli/remesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/cli/remesh_by_shape_factor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23104 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/cli/subset_n_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.317700 ocsmesh-1.2.1/ocsmesh/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/features/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/features/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/features/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/features/linefeature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/features/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/figures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.317700 ocsmesh-1.2.1/ocsmesh/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/geom/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25838 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/geom/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/geom/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/geom/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/geom/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/geom/shapely.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.321700 ocsmesh-1.2.1/ocsmesh/hfun/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/hfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/hfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    79425 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/hfun/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/hfun/hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/hfun/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    58065 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/hfun/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.321700 ocsmesh-1.2.1/ocsmesh/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/mesh/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    74112 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/mesh/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.321700 ocsmesh-1.2.1/ocsmesh/mesh/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/mesh/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/mesh/parsers/grd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/mesh/parsers/sms2dm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.321700 ocsmesh-1.2.1/ocsmesh/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21087 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/ops/combine_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/ops/combine_hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    64534 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    64734 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/ocsmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.317700 ocsmesh-1.2.1/ocsmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-03-24 19:47:15.000000 ocsmesh-1.2.1/ocsmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-24 19:47:15.000000 ocsmesh-1.2.1/ocsmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:47:15.000000 ocsmesh-1.2.1/ocsmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-24 19:47:15.000000 ocsmesh-1.2.1/ocsmesh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-24 19:47:15.000000 ocsmesh-1.2.1/ocsmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-24 19:47:15.000000 ocsmesh-1.2.1/ocsmesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 19:47:15.325700 ocsmesh-1.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3046 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.305700 ocsmesh-1.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.321700 ocsmesh-1.2.1/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/tests/api/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/tests/api/features.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23079 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/tests/api/hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/tests/api/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/tests/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:47:15.321700 ocsmesh-1.2.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/tests/cli/build_geom.sh
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/tests/cli/build_hfun.sh
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-24 19:46:58.000000 ocsmesh-1.2.1/tests/cli/remesh_by_dem.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.514091 ocsmesh-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.486091 ocsmesh-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.494091 ocsmesh-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/.github/workflows/functional_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/.github/workflows/functional_test_2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-27 18:48:01.514091 ocsmesh-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.494091 ocsmesh-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)  2851126 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/docs/noaa_33879_DS1.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.498091 ocsmesh-1.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/docs/source/ocsmesh.command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/docs/source/ocsmesh.geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/docs/source/ocsmesh.mesh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/docs/source/ocsmesh.size_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/docs/source/ocsmesh.utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.502091 ocsmesh-1.3.0/ocsmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.506091 ocsmesh-1.3.0/ocsmesh/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/cli/mesh_upgrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/cli/remesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/cli/remesh_by_shape_factor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23104 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/cli/subset_n_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.506091 ocsmesh-1.3.0/ocsmesh/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/features/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/features/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/features/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/features/linefeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/features/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/figures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.510091 ocsmesh-1.3.0/ocsmesh/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/geom/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/geom/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/geom/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/geom/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/geom/shapely.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.510091 ocsmesh-1.3.0/ocsmesh/hfun/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/hfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/hfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79426 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/hfun/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/hfun/hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/hfun/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58083 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/hfun/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.510091 ocsmesh-1.3.0/ocsmesh/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/mesh/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74321 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/mesh/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.510091 ocsmesh-1.3.0/ocsmesh/mesh/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/mesh/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/mesh/parsers/grd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/mesh/parsers/sms2dm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.510091 ocsmesh-1.3.0/ocsmesh/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/ops/combine_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/ops/combine_hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64799 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64881 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/ocsmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.502091 ocsmesh-1.3.0/ocsmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-27 18:48:01.000000 ocsmesh-1.3.0/ocsmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-27 18:48:01.000000 ocsmesh-1.3.0/ocsmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:48:01.000000 ocsmesh-1.3.0/ocsmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 18:48:01.000000 ocsmesh-1.3.0/ocsmesh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-27 18:48:01.000000 ocsmesh-1.3.0/ocsmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-27 18:48:01.000000 ocsmesh-1.3.0/ocsmesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 18:48:01.514091 ocsmesh-1.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3046 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.490091 ocsmesh-1.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.514091 ocsmesh-1.3.0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/tests/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/tests/api/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/tests/api/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/tests/api/geom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24061 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/tests/api/hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/tests/api/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/tests/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:48:01.514091 ocsmesh-1.3.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/tests/cli/build_geom.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/tests/cli/build_hfun.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-27 18:47:45.000000 ocsmesh-1.3.0/tests/cli/remesh_by_dem.sh
```

### Comparing `ocsmesh-1.2.1/.github/workflows/documentation.yml` & `ocsmesh-1.3.0/.github/workflows/documentation.yml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     name: Build documentation HTML
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Checkout repository
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
     - name: Setup Mamba environment for Python
       uses: mamba-org/provision-with-micromamba@main
       with:
         environment-file: ./environment.yml
         environment-name: ocsmesh-env
         extra-specs: |
           python=3.*
```

### Comparing `ocsmesh-1.2.1/.github/workflows/functional_test.yml` & `ocsmesh-1.3.0/.github/workflows/functional_test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest ]
         python-version: [ '3.8', '3.9', '3.10' ]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Setup Mamba environment for Python
       uses: mamba-org/provision-with-micromamba@main
       with:
         environment-file: ./environment.yml
         environment-name: ocsmesh-env
         extra-specs: |
```

### Comparing `ocsmesh-1.2.1/.github/workflows/functional_test_2.yml` & `ocsmesh-1.3.0/.github/workflows/functional_test_2.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,23 @@
       fail-fast: false
       matrix:
         os: [ ubuntu-latest ]
         python-version: [ '3.8', '3.9', '3.10' ]
 
     steps:
     - name: Checkout 
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
 
     - name: OS binaries
       shell: bash -l {0}
       run: |
         sudo apt install gdal-bin
 
     - name: Install Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install packages
       shell: bash -l {0}
       run: |
         pip install packaging # jigsaw dependency in its setup.py
```

### Comparing `ocsmesh-1.2.1/.github/workflows/pylint.yml` & `ocsmesh-1.3.0/.github/workflows/pylint.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   format-check:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Setup Mamba environment for Python
       uses: mamba-org/provision-with-micromamba@main
       with:
         environment-file: ./environment.yml
         environment-name: ocsmesh-env
         extra-specs: |
           python=3.*
```

### Comparing `ocsmesh-1.2.1/.github/workflows/release.yml` & `ocsmesh-1.3.0/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-latest ]
         python-version: [ '3.10' ]
     steps:
       - name: checkout repository
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: install Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: load cached Python installation
         id: cache
         uses: actions/cache@v2
         with:
           path: ${{ env.pythonLocation }}
```

### Comparing `ocsmesh-1.2.1/.gitignore` & `ocsmesh-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/.pylintrc` & `ocsmesh-1.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/LICENSE` & `ocsmesh-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/PKG-INFO` & `ocsmesh-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsmesh
-Version: 1.2.1
+Version: 1.3.0
 Summary: Package to generate computational unstructured meshes from planetary modeling.
 Author-email: Jaime R Calzada <jreniel@gmail.com>, Soroosh Mani <soroosh.mani@noaa.gov>
 Maintainer-email: Soroosh Mani <soroosh.mani@noaa.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
```

### Comparing `ocsmesh-1.2.1/README.md` & `ocsmesh-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/docs/Makefile` & `ocsmesh-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/docs/make.bat` & `ocsmesh-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/docs/noaa_33879_DS1.pdf` & `ocsmesh-1.3.0/docs/noaa_33879_DS1.pdf`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/docs/source/conf.py` & `ocsmesh-1.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/__init__.py` & `ocsmesh-1.3.0/ocsmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/__main__.py` & `ocsmesh-1.3.0/ocsmesh/__main__.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/cli/cli.py` & `ocsmesh-1.3.0/ocsmesh/cli/cli.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/cli/mesh_upgrader.py` & `ocsmesh-1.3.0/ocsmesh/cli/mesh_upgrader.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/cli/remesh.py` & `ocsmesh-1.3.0/ocsmesh/cli/remesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/cli/remesh_by_shape_factor.py` & `ocsmesh-1.3.0/ocsmesh/cli/remesh_by_shape_factor.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/cli/subset_n_combine.py` & `ocsmesh-1.3.0/ocsmesh/cli/subset_n_combine.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/cmd.py` & `ocsmesh-1.3.0/ocsmesh/cmd.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/db.py` & `ocsmesh-1.3.0/ocsmesh/db.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/driver.py` & `ocsmesh-1.3.0/ocsmesh/driver.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/features/channel.py` & `ocsmesh-1.3.0/ocsmesh/features/channel.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/features/constraint.py` & `ocsmesh-1.3.0/ocsmesh/features/constraint.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/features/contour.py` & `ocsmesh-1.3.0/ocsmesh/features/contour.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/features/linefeature.py` & `ocsmesh-1.3.0/ocsmesh/features/linefeature.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/features/patch.py` & `ocsmesh-1.3.0/ocsmesh/features/patch.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/figures.py` & `ocsmesh-1.3.0/ocsmesh/figures.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/geom/base.py` & `ocsmesh-1.3.0/ocsmesh/geom/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/geom/collector.py` & `ocsmesh-1.3.0/ocsmesh/geom/collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,16 @@
                         continue
 
                 geom = RasterGeom(in_item, **self._elev_info)
 
             elif isinstance(in_item, BaseMesh):
                 geom = MeshGeom(in_item)
 
-            elif isinstance(in_item, str):
+            elif isinstance(in_item, (Path, str)):
+                in_item = str(in_item)
                 if in_item.endswith('.tif'):
                     raster = Raster(in_item)
                     if self._base_shape:
                         clip_shape = self._base_shape
                         if not self._base_shape_crs.equals(raster.crs):
                             transformer = Transformer.from_crs(
                                 self._base_shape_crs, raster.crs, always_xy=True)
@@ -302,16 +303,18 @@
                     base_multipoly = ops.transform(
                             transformer.transform, base_multipoly)
 
             elif self._base_mesh:
                 # TODO: Make sure all calcs are in EPSG:4326
                 base_multipoly = self._base_mesh.hull.multipolygon()
 
-            feather_files.append(self._extract_global_boundary(
-                temp_path, base_multipoly))
+            raster_geom_path = self._extract_global_boundary(
+                temp_path, base_multipoly)
+            if raster_geom_path.is_file():
+                feather_files.append(raster_geom_path)
             feather_files.extend(self._extract_nonraster_boundary(
                 temp_path, base_multipoly))
             feather_files.extend(self._extract_features(
                 temp_path, base_multipoly))
 
             gdf = gpd.GeoDataFrame(columns=['geometry'], crs=epsg4326)
             for f in feather_files:
@@ -443,19 +446,20 @@
 
         Raises
         ------
         TypeError
             If the any of the inputs are not supported
         """
 
-        valid_types = (str, Raster, BaseGeom, BaseMesh)
+        valid_types = (str, Path, Raster, BaseGeom, BaseMesh)
         if not all(isinstance(item, valid_types) for item in input_list):
             raise TypeError(
-                f'Input list items must be of type {", ".join(valid_types)}'
-                f', or a derived type.')
+                f'Input list items must be of type'
+                f' {", ".join(str(i) for i in valid_types)},'
+                f' or a derived type.')
 
     def _get_raster_sources(self) -> List[Union[RasterGeom, Raster]]:
         """Get the list rasters from inputs to the object constructor
 
         Retruns
         -------
         list of RasterGeom or Raster
@@ -625,15 +629,15 @@
 
             geom_path = out_path / f'nonraster_{os.getpid()}_{e}.feather'
 
             crs = geom.crs
             multipoly = self._get_valid_multipolygon(
                     geom.get_multipolygon())
             gdf_non_raster = gpd.GeoDataFrame(
-                    {'geometry': multipoly}, crs=crs)
+                    {'geometry': multipoly.geoms}, crs=crs)
             if crs != CRS.from_user_input("EPSG:4326"):
                 gdf_non_raster = gdf_non_raster.to_crs("EPSG:4326")
 
             # TODO: Clip using base_multipoly?
 
             gdf_non_raster.to_feather(geom_path)
 
@@ -719,15 +723,15 @@
             # Pass patch shape instead of base mesh
             # See explanation in add_patch
             _logger.info("Extracting patch contours")
             combine_poly = base_multipoly
             if ptch_defn:
                 patch_mp, crs = ptch_defn.get_multipolygon()
                 gdf_patch = gpd.GeoDataFrame(
-                        {'geometry': patch_mp}, crs=crs)
+                        {'geometry': patch_mp.geoms}, crs=crs)
                 if crs != CRS.from_user_input("EPSG:4326"):
                     gdf_patch = gdf_patch.to_crs("EPSG:4326")
                 combine_poly = MultiPolygon(list(gdf_patch.geometry))
             geom_path = out_path / f'patch_{os.getpid()}_{e}.feather'
             combine_geometry(
                 patch_raster_files, geom_path, "feather",
                 None, combine_poly, True,
```

### Comparing `ocsmesh-1.2.1/ocsmesh/geom/geom.py` & `ocsmesh-1.3.0/ocsmesh/geom/geom.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/geom/mesh.py` & `ocsmesh-1.3.0/ocsmesh/geom/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/geom/raster.py` & `ocsmesh-1.3.0/ocsmesh/geom/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/geom/shapely.py` & `ocsmesh-1.3.0/ocsmesh/geom/shapely.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/hfun/base.py` & `ocsmesh-1.3.0/ocsmesh/hfun/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/hfun/collector.py` & `ocsmesh-1.3.0/ocsmesh/hfun/collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1281,15 +1281,15 @@
             patch_defn,
             expansion_rate=expansion_rate,
             target_size=target_size)
 
     def add_feature(
             self,
             shape: Union[MultiLineString, LineString, None] = None,
-            line_defn: Optional[LineString] = None,
+            line_defn: Optional[LineFeature] = None,
             shapefile: Union[None, str, Path] = None,
             expansion_rate: float = 0.01,
             target_size: Optional[float] = None,
             crs: CRS = 4326
             ) -> None:
         """Add refinement as a region of fixed size with an optional rate
```

### Comparing `ocsmesh-1.2.1/ocsmesh/hfun/hfun.py` & `ocsmesh-1.3.0/ocsmesh/hfun/hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/hfun/mesh.py` & `ocsmesh-1.3.0/ocsmesh/hfun/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/hfun/raster.py` & `ocsmesh-1.3.0/ocsmesh/hfun/raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -832,17 +832,17 @@
             raise ValueError('Argument target_size must be specified if no '
                              'global hmin has been set.')
         if target_size <= 0:
             raise ValueError("Argument target_size must be greater than zero.")
 
         # For expansion_rate
         if expansion_rate is not None:
-            exteriors = [ply.exterior for ply in multipolygon]
+            exteriors = [ply.exterior for ply in multipolygon.geoms]
             interiors = [
-                inter for ply in multipolygon for inter in ply.interiors]
+                inter for ply in multipolygon.geoms for inter in ply.interiors]
 
             features = MultiLineString([*exteriors, *interiors])
             # pylint: disable=E1123, E1125
             self.add_feature(
                 feature=features,
                 expansion_rate=expansion_rate,
                 target_size=target_size,
@@ -858,15 +858,15 @@
                 # as the hfun (we don't calculate distances in this
                 # method)
 
                 _logger.info('Creating mask from shape ...')
                 start = time()
                 try:
                     mask, _, _ = rasterio.mask.raster_geometry_mask(
-                        self.src, multipolygon,
+                        self.src, multipolygon.geoms,
                         all_touched=True, invert=True)
                     mask = mask[rasterio.windows.window_index(window)]
 
                 except ValueError:
                     # If there's no overlap between the raster and
                     # shapes then it throws ValueError, instead of
                     # checking for intersection, if there's a value
```

### Comparing `ocsmesh-1.2.1/ocsmesh/interp.py` & `ocsmesh-1.3.0/ocsmesh/interp.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/mesh/base.py` & `ocsmesh-1.3.0/ocsmesh/mesh/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/mesh/mesh.py` & `ocsmesh-1.3.0/ocsmesh/mesh/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -741,14 +741,15 @@
         """
 
         polys = utils.get_mesh_polygons(self.mesh.msh_t)
 
         data = []
         bnd_id = 0
         for poly in polys.geoms:
+            # TODO: Enforce CCW vs CW here
             data.append({
                     "geometry": poly.exterior,
                     "bnd_id": bnd_id,
                     "type": 'exterior'
                 })
             for interior in poly.interiors:
                 data.append({
@@ -1030,15 +1031,15 @@
         a single `MultiPolygon` where as `__call__` returns a
         dataframe with multiple `Polygon` entries with associated
         `bnd_id`.
         """
 
         return gpd.GeoDataFrame(
             {"geometry": MultiPolygon([polygon.geometry for polygon
-                                       in self().itertuples()])},
+                                       in self().itertuples()]).geoms},
             crs=self.mesh.crs)
 
     def multipolygon(self) -> MultiPolygon:
         """Returns mesh multi-polygons.
 
         Parameters
         ----------
@@ -1592,25 +1593,27 @@
         coords = self.mesh.msh_t.vert2['coord']
         coo_to_idx = {
             tuple(coo): idx
             for idx, coo in enumerate(coords)}
 
         ext_bdry_nodes = []
         for ring in self.mesh.hull.rings.exterior().itertuples():
+            # TODO: Enforce external rings to be ccw as https://github.com/noaa-ocs-modeling/OCSMesh/issues/65
             ext_ring_coo = ring.geometry.coords
             ext_ring = np.array([
                     (coo_to_idx[ext_ring_coo[e]],
                      coo_to_idx[ext_ring_coo[e + 1]])
                     for e, coo in enumerate(ext_ring_coo[:-1])])
 
             ext_bdry_nodes.append(ext_ring)
 
 
         int_bdry_nodes = []
         for ring in self.mesh.hull.rings.interior().itertuples():
+            # TODO: Internal rings should be cw?
             if not LinearRing(ring.geometry).is_ccw:
                 ring.geometry = ring.geometry.reverse()
             int_ring_coo = ring.geometry.coords
             int_ring = [
                     (coo_to_idx[int_ring_coo[e]],
                      coo_to_idx[int_ring_coo[e + 1]])
                     for e, coo in enumerate(int_ring_coo[:-1])]
```

### Comparing `ocsmesh-1.2.1/ocsmesh/mesh/parsers/grd.py` & `ocsmesh-1.3.0/ocsmesh/mesh/parsers/grd.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/mesh/parsers/sms2dm.py` & `ocsmesh-1.3.0/ocsmesh/mesh/parsers/sms2dm.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/ops/combine_geom.py` & `ocsmesh-1.3.0/ocsmesh/ops/combine_geom.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
                     crs=self._calc_crs
                 )
             for feather_f in poly_files_coll:
                 rasters_gdf = pd.concat(
                     [
                         rasters_gdf,
                         gpd.GeoDataFrame(
-                            {'geometry': self._read_multipolygon(feather_f)},
+                            {'geometry': self._read_multipolygon(feather_f).geoms},
                             crs=self._calc_crs
                         ),
                     ],
                     ignore_index=True
                 )
 
 
@@ -285,15 +285,15 @@
                     multipolygon)
 
         if isinstance(multipolygon, Polygon):
             # In case fix is not True, we need to make sure it's
             # a multipolygon instead of polygon for dataframe creation
             multipolygon = MultiPolygon([multipolygon])
 
-        gpd.GeoDataFrame({'geometry': multipolygon}).to_feather(path)
+        gpd.GeoDataFrame({'geometry': multipolygon.geoms}).to_feather(path)
 
 
     def _read_multipolygon(
             self,
             path: Union[str, os.PathLike],
             fix: bool = True
             ) -> MultiPolygon:
@@ -519,27 +519,27 @@
             self, out_format, out_file, multi_polygon, crs):
 
         _logger.info(f"Writing for file ({out_format}) ...")
 
         # TODO: Check for correct extension on out_file
         if out_format == "shapefile":
             gdf = gpd.GeoDataFrame(
-                    {'geometry': multi_polygon},
+                    {'geometry': multi_polygon.geoms},
                     crs=self._calc_crs
                     )
             if not crs.equals(self._calc_crs):
                 _logger.info(
                     f"Project from {self._calc_crs.to_string()} to"
                     f" {crs.to_string()} ...")
                 gdf = gdf.to_crs(crs)
             gdf.to_file(out_file)
 
         elif out_format == "feather":
             gdf = gpd.GeoDataFrame(
-                    {'geometry': multi_polygon},
+                    {'geometry': multi_polygon.geoms},
                     crs=self._calc_crs
                     )
             if not crs.equals(self._calc_crs):
                 _logger.info(
                     f"Project from {self._calc_crs.to_string()} to"
                     f" {crs.to_string()} ...")
                 gdf = gdf.to_crs(crs)
```

### Comparing `ocsmesh-1.2.1/ocsmesh/ops/combine_hfun.py` & `ocsmesh-1.3.0/ocsmesh/ops/combine_hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/ocsmesh/raster.py` & `ocsmesh-1.3.0/ocsmesh/raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,32 +574,38 @@
         if window is None:
             iter_windows = self.iter_windows(overlap=overlap)
         else:
             iter_windows = [window]
 
         for win in iter_windows:
             x, y, z = self.get_window_data(win, band=band)
-            new_mask = np.full(z.mask.shape, 0)
-            new_mask[np.where(z.mask)] = -1
-            new_mask[np.where(~z.mask)] = 1
+            if z.mask.ndim == 2:
+                new_mask = np.full(z.mask.shape, 0)
+                new_mask[np.where(z.mask)] = -1
+                new_mask[np.where(~z.mask)] = 1
+            else:
+                # If not mask available
+                # NOTE: We want dtype to be int64, not float64
+                new_mask = np.full((len(y), len(x)), 1)
 
             if zmin is not None:
                 new_mask[np.where(z < zmin)] = -1
 
             if zmax is not None:
                 new_mask[np.where(z > zmax)] = -1
 
             if np.all(new_mask == -1):  # or not new_mask.any():
                 continue
 
             fig, ax = plt.subplots()
             ax.contourf(x, y, new_mask, levels=[0, 1])
+            mpoly = utils.get_multipolygon_from_pathplot(ax)
+            if mpoly is not None:
+                polygon_collection.extend(mpoly.geoms)
             plt.close(fig)
-            polygon_collection.extend(
-                    utils.get_multipolygon_from_pathplot(ax).geoms)
 
         union_result = ops.unary_union(polygon_collection)
         if not isinstance(union_result, MultiPolygon):
             union_result = MultiPolygon([union_result])
         return union_result
 
     def get_bbox(
```

### Comparing `ocsmesh-1.2.1/ocsmesh/utils.py` & `ocsmesh-1.3.0/ocsmesh/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,16 +180,17 @@
 
             polys_gdf = gpd.GeoDataFrame(
                 {'geometry': polys, 'list_index': range(len(polys))})
 
 
             res_gdf = polys_gdf[polys_gdf.intersects(pnt)]
             if len(res_gdf) == 0:
-                # How is this possible?!
-                pnts = MultiPoint([*(pnts.geoms[:idx]), *(pnts.geoms[idx + 1:])])
+                # How is this possible for the remaining points not to
+                # intersect with the remaining polys?!
+                pnts = MultiPoint([pt for i, pt in enumerate(pnts.geoms) if i != idx])
                 if pnts.is_empty:
                     break
 
                 continue
 
             poly = res_gdf.geometry.iloc[0]
             polys.pop(res_gdf.iloc[0].list_index)
@@ -621,14 +622,15 @@
         inner_ring_coll[key] = rings['interiors']
     return inner_ring_coll
 
 
 def get_multipolygon_from_pathplot(ax):
     # extract linear_rings from plot
     linear_ring_collection = []
+    multipolygon = None
     for path_collection in ax.collections:
         for path in path_collection.get_paths():
             polygons = path.to_polygons(closed_only=True)
             for linear_ring in polygons:
                 if linear_ring.shape[0] > 3:
                     linear_ring_collection.append(
                         LinearRing(linear_ring))
@@ -647,15 +649,15 @@
                     list(enumerate(linear_ring_collection))):
                 xy = np.asarray(linear_ring.coords)[0, :]
                 if path.contains_point(xy):
                     inner_rings.append(linear_ring_collection.pop(i))
             polygon_collection.append(Polygon(outer_ring, inner_rings))
 
         multipolygon = MultiPolygon(polygon_collection)
-    else:
+    elif len(linear_ring_collection) != 0:
         multipolygon = MultiPolygon(
             [Polygon(linear_ring_collection.pop())])
     return multipolygon
 
 
 def signed_polygon_area(vertices):
     # https://code.activestate.com/recipes/578047-area-of-polygon-using-shoelace-formula/
```

### Comparing `ocsmesh-1.2.1/ocsmesh.egg-info/PKG-INFO` & `ocsmesh-1.3.0/ocsmesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsmesh
-Version: 1.2.1
+Version: 1.3.0
 Summary: Package to generate computational unstructured meshes from planetary modeling.
 Author-email: Jaime R Calzada <jreniel@gmail.com>, Soroosh Mani <soroosh.mani@noaa.gov>
 Maintainer-email: Soroosh Mani <soroosh.mani@noaa.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
```

### Comparing `ocsmesh-1.2.1/ocsmesh.egg-info/SOURCES.txt` & `ocsmesh-1.3.0/ocsmesh.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 ocsmesh/mesh/parsers/grd.py
 ocsmesh/mesh/parsers/sms2dm.py
 ocsmesh/ops/__init__.py
 ocsmesh/ops/combine_geom.py
 ocsmesh/ops/combine_hfun.py
 tests/api/__init__.py
 tests/api/common.py
+tests/api/driver.py
 tests/api/features.py
+tests/api/geom.py
 tests/api/hfun.py
 tests/api/mesh.py
 tests/api/utils.py
 tests/cli/build_geom.sh
 tests/cli/build_hfun.sh
 tests/cli/remesh_by_dem.sh
```

### Comparing `ocsmesh-1.2.1/pyproject.toml` & `ocsmesh-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 readme = "README.md"
 requires-python = '>=3.8, <3.11' # 3.11 no supported by numba
 dependencies = [
     "colored-traceback", "fiona", "geoalchemy2", "geopandas",
     "jigsawpy", "matplotlib", "netCDF4", "numba",
     "numpy>=1.21", # introduce npt.NDArray
     "pyarrow", "rtree", "pyproj>=3.0", "rasterio", "requests", "scipy",
-    "shapely>=1.8, <2", "tqdm", "typing_extensions", "utm",
+    "shapely", "tqdm", "typing_extensions", "utm",
     ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://noaa-ocs-modeling.github.io/OCSMesh/"
 Source = "https://github.com/noaa-ocs-modeling/OCSMesh/"
```

### Comparing `ocsmesh-1.2.1/setup.py` & `ocsmesh-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/tests/api/common.py` & `ocsmesh-1.3.0/tests/api/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import rasterio as rio
 import numpy as np
 from pyproj import CRS
 from jigsawpy import jigsaw_msh_t
 
+import ocsmesh
 
 def create_rectangle_mesh(nx, ny, holes, x_extent=None, y_extent=None):
     """
     Note:
         x = x-index
         y = y-index
 
@@ -117,7 +118,41 @@
         [(index, 0) for index in triangles],
         dtype=jigsaw_msh_t.TRIA3_t
         )
 
     return mesh
 
 
+def topo_2rast_1mesh(r1_path, r2_path, m1_path):
+
+        rast_xy_1 = np.mgrid[-1:0.1:0.1, -0.7:0.1:0.1]
+        rast_xy_2 = np.mgrid[0:1.1:0.1, -0.7:0.1:0.1]
+        nx_z_1, ny_z_1 = rast_xy_1[0].shape
+        rast_z_1 = np.ones_like(rast_xy_1[0]) * 100
+        rast_z_1[:, ny_z_1*1//3:ny_z_1*2//3] = 10
+        rast_z_1[:, ny_z_1*2//3:] = 0
+        rast_z_1[nx_z_1*7//16:nx_z_1*11//16, :] = -10
+        nx_z_2, ny_z_2 = rast_xy_2[0].shape
+        rast_z_2 = np.ones_like(rast_xy_2[0]) * -100
+        rast_z_2[:, :ny_z_2*1//3] = 0
+        rast_z_2[:, ny_z_2*1//3:ny_z_2*2//3] = -10
+        rast_z_2[nx_z_2*7//16:nx_z_2*11//16, :ny_z_2*2//3] = -10
+
+        raster_from_numpy(
+            r1_path, rast_z_1, rast_xy_1, 4326
+        )
+        raster_from_numpy(
+            r2_path, rast_z_2, rast_xy_2, 4326
+        )
+
+        msh_t = create_rectangle_mesh(
+            nx=17, ny=7, holes=[40, 41], x_extent=(-1, 1), y_extent=(0, 1))
+        msh_t.crs = CRS.from_epsg(4326)
+        msh_t.value[:] = 10
+
+        mesh = ocsmesh.Mesh(msh_t)
+        # NOTE: Assuming the interpolation works fine!
+        mesh.interpolate(
+            [ocsmesh.Raster(i) for i in [r1_path, r2_path]],
+            method='nearest'
+        )
+        mesh.write(str(m1_path), format='grd', overwrite=False)
```

### Comparing `ocsmesh-1.2.1/tests/api/mesh.py` & `ocsmesh-1.3.0/tests/api/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.2.1/tests/api/utils.py` & `ocsmesh-1.3.0/tests/api/utils.py`

 * *Files identical despite different names*


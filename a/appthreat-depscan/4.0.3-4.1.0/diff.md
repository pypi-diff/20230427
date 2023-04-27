# Comparing `tmp/appthreat-depscan-4.0.3.tar.gz` & `tmp/appthreat-depscan-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appthreat-depscan-4.0.3.tar", last modified: Wed Apr  5 03:03:48 2023, max compression
+gzip compressed data, was "appthreat-depscan-4.1.0.tar", last modified: Thu Apr 27 12:20:09 2023, max compression
```

## Comparing `appthreat-depscan-4.0.3.tar` & `appthreat-depscan-4.1.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:48.587876 appthreat-depscan-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-04-05 03:03:48.587876 appthreat-depscan-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:48.575876 appthreat-depscan-4.0.3/appthreat_depscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-04-05 03:03:48.000000 appthreat-depscan-4.0.3/appthreat_depscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-05 03:03:48.000000 appthreat-depscan-4.0.3/appthreat_depscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 03:03:48.000000 appthreat-depscan-4.0.3/appthreat_depscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-05 03:03:48.000000 appthreat-depscan-4.0.3/appthreat_depscan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-05 03:03:48.000000 appthreat-depscan-4.0.3/appthreat_depscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-05 03:03:48.000000 appthreat-depscan-4.0.3/appthreat_depscan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:48.575876 appthreat-depscan-4.0.3/depscan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25919 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:48.575876 appthreat-depscan-4.0.3/depscan/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30587 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/lib/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/lib/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/lib/bom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/lib/license.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/lib/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/lib/pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/lib/privado.py
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/depscan/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 03:03:48.587876 appthreat-depscan-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:48.575876 appthreat-depscan-4.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/test/test_bom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/test/test_license.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/test/test_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/test/test_pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/test/test_privado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:48.575876 appthreat-depscan-4.0.3/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:48.571876 appthreat-depscan-4.0.3/vendor/choosealicense.com/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:48.579876 appthreat-depscan-4.0.3/vendor/choosealicense.com/_data/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_data/fields.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_data/meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_data/rules.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:48.583876 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/0bsd.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/afl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35944 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/agpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/artistic-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/bsl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19759 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21474 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cc0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23872 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cecill-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/ecl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/epl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/epl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14163 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/eupl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/eupl-1.2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23969 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/gpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/gpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/isc.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27491 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19902 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/mit-0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/mit.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/mpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/ms-pl.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/ms-rl.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/ncsa.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26174 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/odbl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/ofl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/osl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/postgresql.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/upl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/vim.txt
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/wtfpl.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/zlib.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:48.571876 appthreat-depscan-4.0.3/vendor/spdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:03:48.587876 appthreat-depscan-4.0.3/vendor/spdx/json/
--rw-r--r--   0 runner    (1001) docker     (123)   224002 2023-04-05 03:03:37.000000 appthreat-depscan-4.0.3/vendor/spdx/json/licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:20:09.982984 appthreat-depscan-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-04-27 12:20:09.982984 appthreat-depscan-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:20:09.974984 appthreat-depscan-4.1.0/appthreat_depscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-04-27 12:20:09.000000 appthreat-depscan-4.1.0/appthreat_depscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-27 12:20:09.000000 appthreat-depscan-4.1.0/appthreat_depscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:20:09.000000 appthreat-depscan-4.1.0/appthreat_depscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 12:20:09.000000 appthreat-depscan-4.1.0/appthreat_depscan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 12:20:09.000000 appthreat-depscan-4.1.0/appthreat_depscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 12:20:09.000000 appthreat-depscan-4.1.0/appthreat_depscan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:20:09.974984 appthreat-depscan-4.1.0/depscan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25919 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:20:09.974984 appthreat-depscan-4.1.0/depscan/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30587 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/lib/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/lib/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/lib/bom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/lib/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/lib/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/lib/pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/lib/privado.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/depscan/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 12:20:09.982984 appthreat-depscan-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:20:09.974984 appthreat-depscan-4.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/test/test_bom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/test/test_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/test/test_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/test/test_pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/test/test_privado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:20:09.974984 appthreat-depscan-4.1.0/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:20:09.970984 appthreat-depscan-4.1.0/vendor/choosealicense.com/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:20:09.974984 appthreat-depscan-4.1.0/vendor/choosealicense.com/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_data/fields.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_data/meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_data/rules.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:20:09.978984 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/0bsd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/afl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35944 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/agpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/artistic-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/bsl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19759 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21474 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cc0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23872 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cecill-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/ecl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/epl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/epl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14163 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/eupl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/eupl-1.2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23969 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/gpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/gpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/isc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27491 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19902 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/mit-0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/mit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/mpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/ms-pl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/ms-rl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/ncsa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26174 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/odbl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/ofl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/osl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/postgresql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/upl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/vim.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/wtfpl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/zlib.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:20:09.974984 appthreat-depscan-4.1.0/vendor/spdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:20:09.982984 appthreat-depscan-4.1.0/vendor/spdx/json/
+-rw-r--r--   0 runner    (1001) docker     (123)   224002 2023-04-27 12:19:53.000000 appthreat-depscan-4.1.0/vendor/spdx/json/licenses.json
```

### Comparing `appthreat-depscan-4.0.3/LICENSE` & `appthreat-depscan-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/PKG-INFO` & `appthreat-depscan-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appthreat-depscan
-Version: 4.0.3
+Version: 4.1.0
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
 Home-page: https://github.com/appthreat/dep-scan
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `appthreat-depscan-4.0.3/README.md` & `appthreat-depscan-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/appthreat_depscan.egg-info/PKG-INFO` & `appthreat-depscan-4.1.0/appthreat_depscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appthreat-depscan
-Version: 4.0.3
+Version: 4.1.0
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
 Home-page: https://github.com/appthreat/dep-scan
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `appthreat-depscan-4.0.3/appthreat_depscan.egg-info/SOURCES.txt` & `appthreat-depscan-4.1.0/appthreat_depscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/depscan/cli.py` & `appthreat-depscan-4.1.0/depscan/cli.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/depscan/lib/analysis.py` & `appthreat-depscan-4.1.0/depscan/lib/analysis.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/depscan/lib/audit.py` & `appthreat-depscan-4.1.0/depscan/lib/audit.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/depscan/lib/bom.py` & `appthreat-depscan-4.1.0/depscan/lib/bom.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,35 +133,39 @@
     return pkg
 
 
 def get_pkg_list_json(jsonfile):
     """Method to extract packages from a bom json file"""
     pkgs = []
     with open(jsonfile) as fp:
-        bom_data = json.load(fp)
-        if bom_data and bom_data.get("components"):
-            for comp in bom_data.get("components"):
-                licenses = []
-                vendor = comp.get("group")
-                if not vendor:
-                    vendor = ""
-                if comp.get("licenses"):
-                    for lic in comp.get("licenses"):
-                        license_obj = lic
-                        # licenses has list of dict with either license or expression as key
-                        # Only license is supported for now
-                        if lic.get("license"):
-                            license_obj = lic.get("license")
-                        if license_obj.get("id"):
-                            licenses.append(license_obj.get("id"))
-                        elif license_obj.get("name"):
-                            licenses.append(
-                                cleanup_license_string(license_obj.get("name"))
-                            )
-                pkgs.append({**comp, "vendor": vendor, "licenses": licenses})
+        try:
+            bom_data = json.load(fp)
+            if bom_data and bom_data.get("components"):
+                for comp in bom_data.get("components"):
+                    licenses = []
+                    vendor = comp.get("group")
+                    if not vendor:
+                        vendor = ""
+                    if comp.get("licenses"):
+                        for lic in comp.get("licenses"):
+                            license_obj = lic
+                            # licenses has list of dict with either license or expression as key
+                            # Only license is supported for now
+                            if lic.get("license"):
+                                license_obj = lic.get("license")
+                            if license_obj.get("id"):
+                                licenses.append(license_obj.get("id"))
+                            elif license_obj.get("name"):
+                                licenses.append(
+                                    cleanup_license_string(license_obj.get("name"))
+                                )
+                    pkgs.append({**comp, "vendor": vendor, "licenses": licenses})
+        except Exception:
+            # Ignore json errors
+            pass
         return pkgs
 
 
 def get_pkg_list(xmlfile):
     """Method to parse the bom xml file and convert into packages list
 
     :param xmlfile: BOM xml file to parse
```

### Comparing `appthreat-depscan-4.0.3/depscan/lib/config.py` & `appthreat-depscan-4.1.0/depscan/lib/config.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/depscan/lib/license.py` & `appthreat-depscan-4.1.0/depscan/lib/license.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/depscan/lib/logger.py` & `appthreat-depscan-4.1.0/depscan/lib/logger.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/depscan/lib/normalize.py` & `appthreat-depscan-4.1.0/depscan/lib/normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
             if len(tmpA) > 1 and len(tmpA[1]) > 3:
                 if tmpA[1] != name:
                     vendor_aliases.add(tmpA[1])
     # Add some common vendor aliases
     if purl.startswith("pkg:composer") or purl.startswith("pkg:pypi"):
         vendor_aliases.add(name)
     if purl.startswith("pkg:golang") and not name.startswith("go"):
+        vendor_aliases.add("go")
         # Ignore third party alternatives for builtins
         if "golang" not in vendor and name not in ["net", "crypto", "http", "text"]:
             vendor_aliases.add("golang")
     if pkg_type not in config.OS_PKG_TYPES:
         name_aliases.add("package_" + name)
         if not purl.startswith("pkg:golang"):
             vendor_aliases.add("get" + name)
```

### Comparing `appthreat-depscan-4.0.3/depscan/lib/pkg_query.py` & `appthreat-depscan-4.1.0/depscan/lib/pkg_query.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/depscan/lib/privado.py` & `appthreat-depscan-4.1.0/depscan/lib/privado.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/depscan/lib/utils.py` & `appthreat-depscan-4.1.0/depscan/lib/utils.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/setup.py` & `appthreat-depscan-4.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="appthreat-depscan",
-    version="4.0.3",
+    version="4.1.0",
     author="Team AppThreat",
     author_email="cloud@appthreat.com",
     description="Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.",
     entry_points={
         "console_scripts": ["scan=depscan.cli:main", "depscan=depscan.cli:main"]
     },
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/appthreat/dep-scan",
     packages=["depscan", "depscan.lib", "vendor"],
     include_package_data=True,
     install_requires=[
-        "appthreat-vulnerability-db>=5.0.2",
+        "appthreat-vulnerability-db>=5.1.0",
         "defusedxml",
         "PyYAML",
         "rich",
         "quart",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `appthreat-depscan-4.0.3/test/test_analysis.py` & `appthreat-depscan-4.1.0/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/test/test_bom.py` & `appthreat-depscan-4.1.0/test/test_bom.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/test/test_license.py` & `appthreat-depscan-4.1.0/test/test_license.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/test/test_norm.py` & `appthreat-depscan-4.1.0/test/test_norm.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/test/test_pkg_query.py` & `appthreat-depscan-4.1.0/test/test_pkg_query.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/test/test_utils.py` & `appthreat-depscan-4.1.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_data/fields.yml` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_data/fields.yml`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_data/meta.yml` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_data/meta.yml`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_data/rules.yml` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_data/rules.yml`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/0bsd.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/0bsd.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/afl-3.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/agpl-3.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/apache-2.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/artistic-2.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/bsd-2-clause.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/bsd-3-clause.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/bsd-3-clause.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/bsd-4-clause.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/bsl-1.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cc-by-4.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cc0-1.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cecill-2.1.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/ecl-2.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/epl-1.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/epl-2.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/eupl-1.1.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/eupl-1.2.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/gfdl-1.3.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/gpl-2.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/gpl-3.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/isc.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/isc.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/lgpl-2.1.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/lgpl-3.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/lppl-1.3c.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/lppl-1.3c.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/mit-0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/mit-0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/mit.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/mit.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/mpl-2.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/mpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/ms-pl.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/ms-pl.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/ms-rl.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/ms-rl.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/ncsa.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/ncsa.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/odbl-1.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/odbl-1.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/ofl-1.1.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/ofl-1.1.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/osl-3.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/postgresql.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/postgresql.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/unlicense.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/unlicense.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/upl-1.0.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/upl-1.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/vim.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/vim.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/wtfpl.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/wtfpl.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/choosealicense.com/_licenses/zlib.txt` & `appthreat-depscan-4.1.0/vendor/choosealicense.com/_licenses/zlib.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.0.3/vendor/spdx/json/licenses.json` & `appthreat-depscan-4.1.0/vendor/spdx/json/licenses.json`

 * *Files identical despite different names*


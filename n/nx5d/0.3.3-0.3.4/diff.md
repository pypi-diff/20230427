# Comparing `tmp/nx5d-0.3.3.tar.gz` & `tmp/nx5d-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nx5d-0.3.3.tar", last modified: Mon Apr 24 10:38:35 2023, max compression
+gzip compressed data, was "nx5d-0.3.4.tar", last modified: Thu Apr 27 15:34:05 2023, max compression
```

## Comparing `nx5d-0.3.3.tar` & `nx5d-0.3.4.tar`

### file list

```diff
@@ -1,172 +1,181 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.939599 nx5d-0.3.3/
--rw-r--r--   0 florin    (1000) florin    (1000)       72 2023-04-24 10:31:16.000000 nx5d-0.3.3/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-04-24 10:31:16.000000 nx5d-0.3.3/.gitlab-ci.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-30 12:37:15.000000 nx5d-0.3.3/.readthedocs.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-30 12:37:15.000000 nx5d-0.3.3/COPYING.md
--rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-04-24 10:38:35.939599 nx5d-0.3.3/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-30 12:37:15.000000 nx5d-0.3.3/README.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.914599 nx5d-0.3.3/doc/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.916599 nx5d-0.3.3/doc/mkdocs/
--rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/about.md
--rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-24 10:31:17.000000 nx5d-0.3.3/doc/mkdocs/api.md
--rw-r--r--   0 florin    (1000) florin    (1000)    27046 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/concepts.md
--rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/frame.svg
--rw-r--r--   0 florin    (1000) florin    (1000)     2482 2023-04-24 10:31:17.000000 nx5d-0.3.3/doc/mkdocs/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/license.md
--rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/module-nx.md
--rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/scan.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/streak1.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/streak2.svg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.916599 nx5d-0.3.3/doc/mkdocs/tutorials/
--rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/tutorials/index.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.917599 nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/
--rw-r--r--   0 florin    (1000) florin    (1000)    44315 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
--rw-r--r--   0 florin    (1000) florin    (1000)    19430 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
--rw-r--r--   0 florin    (1000) florin    (1000)    25263 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
--rw-r--r--   0 florin    (1000) florin    (1000)    23184 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
--rw-r--r--   0 florin    (1000) florin    (1000)    13289 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
--rw-r--r--   0 florin    (1000) florin    (1000)    16038 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.918599 nx5d-0.3.3/doc/mkdocs/tutorials/scansource-howto/
--rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.918599 nx5d-0.3.3/doc/mkdocs/user-guide/
--rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-24 10:31:17.000000 nx5d-0.3.3/doc/mkdocs/user-guide/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-30 12:37:15.000000 nx5d-0.3.3/doc/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-30 12:37:15.000000 nx5d-0.3.3/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-30 12:37:15.000000 nx5d-0.3.3/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)     2974 2023-03-30 12:37:15.000000 nx5d-0.3.3/scratch.org
--rw-r--r--   0 florin    (1000) florin    (1000)      946 2023-04-24 10:38:35.939599 nx5d-0.3.3/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.912598 nx5d-0.3.3/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.919599 nx5d-0.3.3/src/nx5d/
--rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-04-24 10:38:35.000000 nx5d-0.3.3/src/nx5d/_version.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/edf.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.921599 nx5d-0.3.3/src/nx5d/h5like/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-24 10:31:17.000000 nx5d-0.3.3/src/nx5d/h5like/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5686 2023-04-24 10:31:17.000000 nx5d-0.3.3/src/nx5d/h5like/pypod.py
--rw-r--r--   0 florin    (1000) florin    (1000)    11246 2023-04-24 10:31:17.000000 nx5d-0.3.3/src/nx5d/h5like/tools.py
--rw-r--r--   0 florin    (1000) florin    (1000)    31529 2023-04-24 10:31:17.000000 nx5d-0.3.3/src/nx5d/h5like/xfel.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/nx.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/runlog.py
--rw-r--r--   0 florin    (1000) florin    (1000)    13662 2023-04-24 10:31:17.000000 nx5d-0.3.3/src/nx5d/scan.py
--rw-r--r--   0 florin    (1000) florin    (1000)     7572 2023-04-24 10:31:17.000000 nx5d-0.3.3/src/nx5d/streaks.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.923599 nx5d-0.3.3/src/nx5d/xrd/
--rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/xrd/ColonelSandersFinest.py
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/xrd/__init__.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/xrd/analysis.py
--rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/xrd/esrf_id09.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/xrd/experiment-xpp.yml
--rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/xrd/experiment.py
--rw-r--r--   0 florin    (1000) florin    (1000)    13272 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/xrd/kmc3.py
--rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/xrd/roi.py
--rw-r--r--   0 florin    (1000) florin    (1000)    19453 2023-04-24 10:31:17.000000 nx5d-0.3.3/src/nx5d/xrd/signal.py
--rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-04-24 10:31:17.000000 nx5d-0.3.3/src/nx5d/xrd/xfel.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/xrd/xraytest.py
--rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-30 12:37:15.000000 nx5d-0.3.3/src/nx5d/xrd/xrd_helpers.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.920599 nx5d-0.3.3/src/nx5d.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-04-24 10:38:35.000000 nx5d-0.3.3/src/nx5d.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     7583 2023-04-24 10:38:35.000000 nx5d-0.3.3/src/nx5d.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-04-24 10:38:35.000000 nx5d-0.3.3/src/nx5d.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)      157 2023-04-24 10:38:35.000000 nx5d-0.3.3/src/nx5d.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-04-24 10:38:35.000000 nx5d-0.3.3/src/nx5d.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.924599 nx5d-0.3.3/tests/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)      961 2023-04-24 10:31:17.000000 nx5d-0.3.3/tests/pabst_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1559 2023-04-24 10:31:17.000000 nx5d-0.3.3/tests/pypod_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/runlog_test.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.912598 nx5d-0.3.3/tests/test_data/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.931599 nx5d-0.3.3/tests/test_data/runfile/
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/run105.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/run105_brokendata1.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/run105_brokendata2.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/run105_brokenheader.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/run105_simple.log
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0001.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0002.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0003.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0004.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0005.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0006.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0007.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0008.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0009.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0010.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0011.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0012.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0013.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0014.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0015.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0016.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0017.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0018.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0019.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0020.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0021.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0022.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0023.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0024.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0025.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0026.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0027.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0028.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0029.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0030.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0031.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0032.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0033.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0034.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0035.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0036.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/runfile/short_run04_0037.edf
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.912598 nx5d-0.3.3/tests/test_data/spech5/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.931599 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/
--rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.913599 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.932599 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
--rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-24 10:38:35.939599 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
--rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3341 2023-04-24 10:31:17.000000 nx5d-0.3.3/tests/xfel_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1059 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/xrd_data_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      915 2023-03-30 12:37:15.000000 nx5d-0.3.3/tests/xrd_kmc3_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.648910 nx5d-0.3.4/
+-rw-r--r--   0 florin    (1000) florin    (1000)       72 2023-04-13 14:23:04.000000 nx5d-0.3.4/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-04-12 13:31:40.000000 nx5d-0.3.4/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-15 11:10:41.000000 nx5d-0.3.4/.readthedocs.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-14 11:33:48.000000 nx5d-0.3.4/COPYING.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-04-27 15:34:05.648910 nx5d-0.3.4/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-27 10:49:57.000000 nx5d-0.3.4/README.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.623910 nx5d-0.3.4/doc/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.625910 nx5d-0.3.4/doc/mkdocs/
+-rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-15 10:15:42.000000 nx5d-0.3.4/doc/mkdocs/about.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-12 12:52:07.000000 nx5d-0.3.4/doc/mkdocs/api.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    27056 2023-04-25 09:48:18.000000 nx5d-0.3.4/doc/mkdocs/concepts.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-25 14:27:00.000000 nx5d-0.3.4/doc/mkdocs/frame.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)     2483 2023-04-25 09:48:18.000000 nx5d-0.3.4/doc/mkdocs/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-15 10:32:22.000000 nx5d-0.3.4/doc/mkdocs/license.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-27 10:50:49.000000 nx5d-0.3.4/doc/mkdocs/module-nx.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-25 14:25:35.000000 nx5d-0.3.4/doc/mkdocs/scan.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-25 14:49:22.000000 nx5d-0.3.4/doc/mkdocs/streak1.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-25 14:49:37.000000 nx5d-0.3.4/doc/mkdocs/streak2.svg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.626910 nx5d-0.3.4/doc/mkdocs/tutorials/
+-rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-15 10:35:31.000000 nx5d-0.3.4/doc/mkdocs/tutorials/index.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.627910 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/
+-rw-------   0 florin    (1000) florin    (1000)    44315 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
+-rw-------   0 florin    (1000) florin    (1000)    19430 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
+-rw-------   0 florin    (1000) florin    (1000)    25263 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
+-rw-------   0 florin    (1000) florin    (1000)    23184 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
+-rw-------   0 florin    (1000) florin    (1000)    13289 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
+-rw-------   0 florin    (1000) florin    (1000)    16038 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.627910 nx5d-0.3.4/doc/mkdocs/tutorials/scansource-howto/
+-rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-14 12:31:08.000000 nx5d-0.3.4/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.627910 nx5d-0.3.4/doc/mkdocs/user-guide/
+-rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-12 12:48:11.000000 nx5d-0.3.4/doc/mkdocs/user-guide/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-15 14:06:55.000000 nx5d-0.3.4/doc/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-15 10:49:21.000000 nx5d-0.3.4/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-14 11:33:48.000000 nx5d-0.3.4/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)     2974 2022-08-02 20:02:56.000000 nx5d-0.3.4/scratch.org
+-rw-r--r--   0 florin    (1000) florin    (1000)      946 2023-04-27 15:34:05.649910 nx5d-0.3.4/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.621910 nx5d-0.3.4/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.628910 nx5d-0.3.4/src/nx5d/
+-rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d/_version.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/edf.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.629910 nx5d-0.3.4/src/nx5d/h5like/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-12 12:44:54.000000 nx5d-0.3.4/src/nx5d/h5like/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    11230 2023-04-27 15:18:39.000000 nx5d-0.3.4/src/nx5d/h5like/petra3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     5686 2023-04-17 15:45:54.000000 nx5d-0.3.4/src/nx5d/h5like/pypod.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    10119 2023-04-27 15:05:03.000000 nx5d-0.3.4/src/nx5d/h5like/spec.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    11246 2023-04-18 08:03:50.000000 nx5d-0.3.4/src/nx5d/h5like/tools.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    31529 2023-04-13 15:04:17.000000 nx5d-0.3.4/src/nx5d/h5like/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/nx.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/runlog.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    14860 2023-04-27 14:19:57.000000 nx5d-0.3.4/src/nx5d/scan.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     7572 2023-04-17 15:45:54.000000 nx5d-0.3.4/src/nx5d/streaks.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.631910 nx5d-0.3.4/src/nx5d/xrd/
+-rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/ColonelSandersFinest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/__init__.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/analysis.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/esrf_id09.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/experiment-xpp.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/experiment.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1939 2023-04-27 14:16:35.000000 nx5d-0.3.4/src/nx5d/xrd/kmc3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/roi.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    19453 2023-04-25 09:48:18.000000 nx5d-0.3.4/src/nx5d/xrd/signal.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-04-25 09:48:18.000000 nx5d-0.3.4/src/nx5d/xrd/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/xraytest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/xrd_helpers.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.629910 nx5d-0.3.4/src/nx5d.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     7794 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)      157 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.632910 nx5d-0.3.4/tests/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     1167 2023-04-27 15:21:20.000000 nx5d-0.3.4/tests/fio_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      961 2023-04-17 15:45:54.000000 nx5d-0.3.4/tests/pabst_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1559 2023-04-17 15:45:54.000000 nx5d-0.3.4/tests/pypod_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/runlog_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      915 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/spec_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.622910 nx5d-0.3.4/tests/test_data/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.632910 nx5d-0.3.4/tests/test_data/fioh5/
+-rw-r--r--   0 florin    (1000) florin    (1000)    13611 2023-04-25 09:48:18.000000 nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00342.fio
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.622910 nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00744/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.632910 nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00744/lambda/
+-rw-r--r--   0 florin    (1000) florin    (1000)   302228 2023-04-25 10:50:01.000000 nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs
+-rw-r--r--   0 florin    (1000) florin    (1000)    13952 2023-04-25 09:48:18.000000 nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00744.fio
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.637910 nx5d-0.3.4/tests/test_data/runfile/
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run105.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run105_brokendata1.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run105_brokendata2.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run105_brokenheader.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run105_simple.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0001.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0002.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0003.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0004.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0005.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0006.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0007.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0008.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0009.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0010.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0011.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0012.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0013.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0014.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0015.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0016.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0017.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0018.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0019.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0020.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0021.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0022.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0023.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0024.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0025.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0026.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0027.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0028.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0029.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0030.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0031.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0032.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0033.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0034.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0035.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0036.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0037.edf
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.622910 nx5d-0.3.4/tests/test_data/spech5/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.637910 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/
+-rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.622910 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.640910 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
+-rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.648910 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
+-rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3341 2023-04-13 14:23:04.000000 nx5d-0.3.4/tests/xfel_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1059 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/xrd_data_test.py
```

### Comparing `nx5d-0.3.3/.gitlab-ci.yml` & `nx5d-0.3.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/COPYING.md` & `nx5d-0.3.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/PKG-INFO` & `nx5d-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.3
+Version: 0.3.4
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.3/README.md` & `nx5d-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/concepts.md` & `nx5d-0.3.4/doc/mkdocs/concepts.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Core Concepts
 =============
 
 Here we explain how, to our perception, scientific data analysis generally
 takes place, what are the most challenging aspects in the typical workflow,
-and now nx5d intends to
+and how nx5d intends to
 [scratch that itch](http://www.catb.org/~esr/writings/cathedral-bazaar/cathedral-bazaar/ar01s02.html).
 
 If you're looking to dive right in, skip to the
 [Quick Start](user-guide/index.md#quick-start) page and the rest of the
 [User Guide](user-guide/index.md).
 You can return to this section at a later point if you feel inclined.
 
@@ -30,35 +30,34 @@
    environment (e. g. Python, likely inside a
    [Jupyter Lab](https://jupyterlab.readthedocs.io/en/latest/index.html) environment),
    parsing *all* the relevant data including positioners, and generating useful
    language objects (e. g. [Numpy arrays](https://numpy.org/doc/stable/))
    to interact with it.
 
 3. **Processing** -- this is the "core" of data analysis process: translating the
-   data from its machine-generated form (e. g. detector images with pixels and angles)
-   into a form closer to the actual science to be performed (e. g.
+   data from its machine-generated form (e. g. detector images with pixels and
+   associated angles) into a form closer to the actual science to be performed (e. g.
    "energy distribution map by crystal momentum coordinates").
    
 4. **Presentation** -- many activities fall into this category, for instance
-   writing a paper intended for peer-reviewed publication, designing a conference
-   poster, creating a presentation for group-itnernal review etc; but all of these
+   writing a paper intended for (peer-reviewed) publication, designing a conference
+   poster, creating a presentation for group-internal review etc; but all of these
    actually begin with the benign task of just *plotting* the data, i. e. visualising
    it, mostly still within the same processing enviroment as previous steps, with
    the help of a designated library like [Matplotlib](https://matplotlib.org/).
    
 The essential message behind this breakdown is that by the time step 4 is reached,
 the data-processing part of a scientists's job is done; and that every part of
-that job which is *specific* to a certain scientist and a certain experimental
-setup is already finished after step 1.
+that job, which is *specific* to a certain scientist and a certain experimental
+setup, is already finished after step 1.
 
-Conversely, as far as steps 2 and 3 are
-concerned -- reading and processing of experimental data -- there is a lot of
-potential for "joining forces" among scientists. Yet ironically, this is what
-swallows up a large amount of time and energy of every PhD's and postdoctoral
-researcher's time.
+Conversely, as far as steps 2 and 3 are concerned -- reading and processing of
+experimental data -- there is a lot of potential for "joining forces" among
+scientists. Yet ironically, this is what swallows up a large amount of time and
+energy of every PhD's and postdoctoral researcher's time.
 
 
 ### If Data Analysis Was a Picnic...
 
 ...at a leisurely pace, and in a programming language resembling Python code,
 the typical workflow for loading, preparing and visualising the latest
 measurement data should look similar to this:
@@ -78,41 +77,40 @@
 
 # Finally, the data can be displayed as desired.
 pyplot.plot(transformed_data)
 ```
 
 Ideally, this is all it should take to load, process and display the
 data of a particular measurement: about as many lines of code as
-can be counted on one hand.
-While it is acknowledged that IT people tend to "cheat" and hide a lot of
-processing steps behind few lines of code, which makes the example above seem
-somewhat artificial, the example above is not primarily about an upper limit
-for the ideal number of *lines of code*. What we can learn instead is that
-it is absolutely possible, and desirable, to get by with very few, highly
-specific intermediate structures:
+can be counted on one hand. While it is acknowledged that IT people tend
+to "cheat" and hide a lot of processing steps behind few lines of code,
+which makes the example above seem somewhat artificial, the example above
+is not primarily about an upper limit for the ideal number of *lines of code*.
+What we can learn instead is that it is absolutely possible, and desirable, to get
+by with very few, highly specific intermediate structures:
 
-  - `experiment_setup`, a data container which describes everything that is
+  - `experiment_setup`, a data container that describes everything that is
     required is to know about our *particular* experiment in order to
-	analyse the data -- geometry of the device, offsets	for positioners,
+	analyse the data -- geometry of the device, offsets for positioners,
 	etc.
 	
   - `raw_data`, the actual data of one particular experiment run -- the
     detector image(s), actual positioner values, accompanying parameters
 	like temperatures, flow data etc.
 	
   - `data_transformation()`, a specific analysis algorithm (ofen also a *generic*
-     algorithm with specific parameters) which depends mostly on
+     algorithm with specific parameters), which depends mostly on
      the task at hand; the exact processiong pipeline may be somewhat unique to
 	 the situation (e. g. a certain scaling or biasing parameter for data processing),
 	 but the inverse is not true: the data itself does *not* mingle with the
 	 tweaking parameters, it can truly stand on its own.
 	 
-  - `transformed_data`, the final in a physical data -- meaningful and able
+  - `transformed_data`, the final of the physical data -- meaningful and able
     to stand on its own, ready to draw conclusions from (we also include
-	intrinsic scaling, dimensions, meta information etc in this category).
+	intrinsic scaling, dimensions, meta information etc. in this category).
 
 Finally, this is what nx5d tries to achieve: unify the workflow as much
 as possible in order to allow consolidating "boilerplate" tasks: defining
 the experimental layout, reading the data and applying experiment-specific
 transformations. This will free time and energy of the ambitious researcher
 for things that actually matter: doing the *scientific* work.
 
@@ -120,15 +118,15 @@
 The "Moving Parts" of Data Analysis
 -----------------------------------
 
 ### On-Disk Data Formats
 
 The reality of experimental physics is that many formats fly around.
 Some are de-facto standards, stemming either from a commonly used
-software package (e.g. Spec, IgorPro etc), but most are "wild", unique
+software package (e.g. SPEC, IgorPro, etc.), but most are "wild", unique
 creations grown historically in a particular lab. They are utterly
 unstandardized, and we view the attempt to change that as a hopeless
 endeavour.
 
 None the less, there *are* standards worth mentioning, most prominently
 the [HDF on-disk format](https://www.hdfgroup.org/). For HDF there is
 ample tooling available for essentially any programming language of
@@ -141,25 +139,25 @@
 suffers from the want (or need) to placate too many requirements. It
 even contains details about data storage and exprimental description of
 a number of "standard" physical experiments, yet to our knowledge even
 a development groupas large as the one of the European Syncrotron Radiaon
 Facility (ESRF) hasn't, for instance, managed to model a typical X-ray
 diffraction (XRD) setup inside a Nexus file.
   
-However, the HDF/Nexus combination has its strengths. For isntance it
-defines a very well usable *API layer* on which to build. Focusing on 
-hat allows us to create modular data I/O routines with backends to the
+However, the HDF/Nexus combination has its strengths. For instance, it
+defines a very well-usable *API layer* on which to build on. Focusing on 
+that allows us to create modular data I/O routines with backends to the
 myriads of obscure and entrenched formats, while still retaining the
 upstream data post-processing abilities unchanged.
 
 This is what nx5d attempts.
 
 ### Scan, Streak, Frame
 
-With regards to data semantics we've decided to try to avoid mistakes
+With regards to data semantics, we've decided to try to avoid mistakes
 of the past by throwing away the dedication to *absoulte* generality,
 simply because the "general" is the enemy of the "specific" and -- if
 words play is permitted -- it's "specific" problems that everyone is
 trying to solve. Staying too general creates the necessity to write
 a large amount of "boilerplate code" just to deal with menial tasks.
 
 Instead we're focusing on what we perceive to be a common denominator
@@ -187,43 +185,43 @@
 	here called "image"), and possibly several additional data
 	of auxiliary devices (e.g. positioners, here called "array"
 	and "scalar").
 	
 	For the example of an X-ray diffraction pump-probe experiment,
 	the meaning could be as follows:
 	
-	- *"image"*: the X-ray detector image
+	- *"image"*: the X-ray detector image(s)
 	- *"array"*: a list of goniometer angles
 	- *"scalar"*: an additional parameter that may change from
-	  frame to frame, e.g. a pump-probe delay time, or a 
+	  frame to frame, e.g. a pump-probe delay time, or 
 	  sample temperature, etc.
 	  
-    Quite generally, a *frame* is the typical structure of the data
+    Generally speaking, a *frame* is the typical structure of the data
 	with which the experimental setup is primarily concerned.
 	  
   - **Scan**: the typical set of experimental data with which the
     scientist is concerned: they typically need more than one single
 	frame in order to perform scientific work. In the X-ray diffraction
 	case, they need several detector images, and for each image the
-	corresponding auxiliary parameters (angles etc) to evaluate the
-	physics they're intereted in.
+	corresponding auxiliary parameters (angles, distances, etc.) to
+	evaluate the physics they're intereted in.
 	
   - **Streak**: coalescing a set of *frames* into a scientifically
     useful format (e.g. a reciprocal space map of a sample, to
 	stick with the XRD example) usually involves transformation
 	of some kind -- perfomred by e.g. by something akin to the
 	`data_transform()` routine outlined above.
 	But this is typically done by breaking up the scan into smaller
 	subsets, each outlining one specific aspect of the data.
 	
 	A *streak* is therefore the typical data processing unit of
 	the algorithm employed for analysis.
 	
 In the example above, we have N+1 frames in one scan, and we can
-subdivide the scan in two families of streaks.
+subdivide the scan into two families of streaks.
 
 One would be, in the XRD example, all images taken at different
 values for the angle set "array", but all having the same
 value of "scalar" (for instance: the same pump-probe delay):
 
 ![Streak A](streak1.svg "One particular family of streaks")
 
@@ -231,15 +229,15 @@
 same value set for "array", but different for "scalar":
 
 ![Streak B](streak2.svg "An particular streak")
 
 Some data processing steps may require one particular family
 of streaks or the other, or both families for different steps
 of data processing. In the end, this is a question of that
-particular, experiment and scientist specific method of
+particular experiment and scientist-specific method of
 data conversion and analysis -- nx5d tries not to make
 further assumptions in this regard.
 We also try to not make any restricting assumptions as to the nature
 of the data (data type or dimensionality) within the individual
 sets ("image", "array", "scalar"), or to the number of such
 sets.
 
@@ -263,15 +261,15 @@
    streak -- there's nothing in nx5d that requires that 
    a scan be broken down into more than one streak.
    But if the experiment involved the same kind of measurement
    for several photon energies, e.g. for 3D mapping of the
    Fermi surface, several such streaks -- each for one
    specific photon energy -- could make up one *scan*.
 
-What nx5d wants to provide, however, is a standard API for
+What nx5d wants to provide is a standard API for
 accessing different streaks, selected by custom criteria,
 in a hassle-free manner and with as little necessity for
 "boilerplate code" as possible. It then offers a unified API
 for passing on data to experiment-specific analysis and data
 transformation code. The general internal data exchange format
 within nx5d for this is a Python `dict()`, with the set
 name as labels, and whatever data container is deemed appropriate
@@ -313,23 +311,23 @@
   "imageChannelSize": (1e-4, 1e-4),
   "imageDistance": 0.750,
   ...
 }
 ```
 
 Ideally such a structure should only be dependent on the type
-of experiment, but in reality dependent on a good code
-abstraction layer, and thus fairly dependent also on a specific
+of experiment, but in reality depends on a good code
+abstraction layer, and thus is fairly dependent also on a specific
 analysis toolkit. The example above is an excerpt of
 what the `nx5d.xrd.LazyQMap` class requires, which fits nx5d with
 the out-of-the-box ability to generate reciprocal space maps
 for X-ray diffraction experiments. `LazyQMap` in turn is
 based on the elaborate abstractions of the `xrayutilities` package.
 
-While we acknowledge that we are in quite a comfortable position
+While we acknowledge that we are in the quite comfortable position
 to reap benefits of a well thought-of experimental software, nx5d
 can use 3rd-party abstractions and data analysis modules, and can
 enhance these if they observe the principles of data formatting
 as outline above. This serves to underline the importance of such
 a software package, and the fact that scholars of every (class of)
 experimental technique should get together to build at least one.
   
@@ -337,15 +335,15 @@
 of (discipline-specific) experimental devices, and we're in the procees
 of investigating the possibilities of reading such information directly
 from the data file itself.
 
 ### Dictionary Templates
 
 The core strength of nx5d is to not only process data formatted as
-Python dictionaries, but to actually use dictionary *templates* which
+Python dictionaries, but to actually use dictionary *templates* that
 contain references to datasets within HDF files instead of actual data.
 For instance, the experimental setup description in the previous section
 could also be formulated like this:
 
 ```
 experiment = {
   "goniometerAxes": "@instrument/goniometer/axes",
@@ -377,29 +375,29 @@
 data = {
   "image": "@measurement/detector-image",
   ...
 }
 ```
 
 Nx5d offers mechanisms to flesh out such templates with real data from
-the corresponding scans, streaks, frames.
+the corresponding scans, streaks and frames.
 
 ### Data Post-Processing
 
 This is a difficult task to make an abstraction of. On one hand, it must unify
 all the components we want to separate and "tame" for the sake of reusability
 of modules: experimental data (both positioning data and "measurement payload"),
 experimental geometry information (setup), and analysis algorithms.
 On the other, it requires *flexibility* -- everyone's experiment is different,
 their science is different, and the post-processing step is what makes up this
 individuality to the largest parts.
   
 The nx5d approach is to build on what we've already seen above:
 
-  - a data model which tames discrete, senquential data (*scan, streak, frame*),
+  - a data model which tames discrete, sequential data (*scan, streak, frame*),
     and at least allows to abstract away the loops over data partitions suitable
 	for processing
 	
   - a unified interface to access data at several levels of granularity, and which
     makes simple common tasks of this category easy, while not making the difficult 
 	impossible.
 
@@ -409,15 +407,15 @@
 X-ray diffraction data). Again, we were fortunate to be able to already make use
 of a well-thought-of Python toolkit for this specific kind of work,
 [xrayutilities](https://xrayutilities.sourceforge.io/).
 
 This data analysis is ultimately where the scientist's IT effort will have to be
 spent. If the nx5d structuring and data formatting offer is accepted, it is
 an easier way to make code reusable across many similar experimental setups,
-enabling the user spend those efforts only *once* for a given discipline and kind
+enabling the user to spend those efforts only *once* for a given discipline and kind
 of research -- independently on the data source (laboratory setup? beamline?),
 or the on-disk format in which it was saved.
 
 Putting It All Together
 -----------------------
 
 ### A Typical Nx5d Analysis Example
@@ -451,50 +449,50 @@
 ```
 
 We are proud of the fact that this is strikingly close to the "perfect"
 algorithm we've formulated above, except for the part where we initialize
 the `ScanReader` class. We emphasize that this wouldn't change if we
 were to load data from a different, similar facilty, as long as the
 facility stores the data in a HDF5 format structurally compatible with
-this. If not, there nx5d provides a series of HDF5-alike APIs for reading
+this. If not, nx5d provides a series of HDF5-alike APIs for reading
 various files (e.g. `.spec` files) in the module `nx5d.h5like`.
-We are using API of the [silx library](https://www.silx.org/doc/silx/latest/),
+We are using the API of the [silx library](https://www.silx.org/doc/silx/latest/),
 so even if nx5d doesn't yet have what *you* need, examples on how to
 rapidly create a HDF5-like API for accessing *your* data are plenty.
 
 ### Integration With Other Toolsets
 
-One component that's not the merit of nx5d, but we none the less shamelessly
+One component that's not the merit of nx5d, but we nonetheless shamelessly
 take advantage of, is the [xarray library](https://docs.xarray.dev/en/stable/index.html).
 It allows to create multidimensional arrays with intrinsic scaling information.
 While the core components of nx5d don't care about that, all data analysis
 and transformation templates, examples and productive code make heavy use
 of that feature. For instance in the example above, integrating along "qx"
 leaves the *qy/qz* 2D plane resolved, which is what in many XRD experiments
 is desireable.
 
 But this is totally left up to the user :-)
 
 For instance: different calculations, integrating along two axes and then
-peparing all signals to be added up all signals according to their remaining
+peparing all signals to be added up according to their remaining
 *qz* value would also be just a one-liner:
 ```
 qdata = [q.sum("qx").sum("qy") for q in qimages]
 ```
 
 We feel that now, once the "boilerplate code" required to load data and transform
-it into a forman useful to actually do *physics* has been scaled down to a minimum,
-a solid foundation on which to build, more complex, highly specific data analysis
+it into a for man useful form  to actually do *physics* has been scaled down to a minimum,
+a solid foundation on which to build more complex, highly specific data analysis
 emerges.
 
 Notable Mentions and Ideas
 --------------------------
 
 Beyond what was described, there are a number of concepts still lingering
-or shinig through, of which some proof-of-concept code may exist within
+or shining through, of which some proof-of-concept code may exist within
 nx5d, but which didn't quite make it to "full analysis concepts" in their
 own right.
 
 Here we give a brief description, as well as an outlook on what may
 become of them.
 
 ### Data Assembly
@@ -522,15 +520,15 @@
 The question of how complex data slicing for the purpose of building
 streaks is not yet fully settled. The initial idea of defining either
 "chunks", i.e. data sets of a fixed length, or "strides", i.e. data
 sets with a fixed stepping) covers a large part of use cases.
 But there are more sophisticated cases where the streaking is dynamic,
 for instance depending on the structure of the data acquisition, e.g.
 as given by a sequence of heterogenous pulses, or otherwise subsequent
-scans have a non-trivially chaning meaning attached to them (e.g.
+scans have a non-trivially changing meaning attached to them (e.g.
 "real" data vs. "reference" data).
 
 We are still working to determine a more general approach to this
 without sacrificing simplicity.
 
 ### Advanced Signal Manipulation
 
@@ -551,15 +549,15 @@
 
 The previous idea -- advanced signal manipulation -- shows that
 there might be a necessity for a pipeline-like data processing
 facilty. This would allow modularization and abstraction of common
 data processing steps in a building-stone like way.
 
 For this, we are currently acquiring ideas, and are intrigued by
-the [EWOKS system](https://streamline.esrf.fr/non-classe/ewoks-the-esrf-workflow-system/),
+the [EWOKS system](https://gitlab.esrf.fr/workflow/ewoks/ewoks/),
 a workflow library developed at ESRF.
 
 ### Data Exporting
 
 Once data has been analized, saving finished data might be a good
 idea.
 
@@ -573,31 +571,31 @@
 than a finished, readily processed dataset ever can.
 
 However, we don't discard that there *still are* legitimate use cases
 for saving finished data, or at least data that has passed specific
 intermedaite processing steps. One such example is presented in the
 `nx5d.h5like.xfel` module: the "original" data format of
 [XFEL](https://www.xfel.eu/facility/overview/desy/index_eng.html)
-is prohibitively cumbersome and large, and actually impossible to
+is prohibitively cumbersome and large. It is actually impossible to
 analyze data from outside the context of the XFEL processing systems
 themselves. Yet one intermediate result, namely the one where all the
-origianl XFEL data has at least been merged into "regular X-ray
+original XFEL data has at least been merged into "regular X-ray
 detector images" and "regular goniometer positioners", is a perfect
 candidate for retaining and distribution in a more accessible
 format.
 
 Such intermediate formats might also be stepping stones for further
 processing. In the XFEL case, for example, we are using a stacked
 system of `ScanReader` layers, which would be impossible without
 an intermediate re-transformation of the data into an easily
 storeable format.
 
 ### Graphical User Interfacing
 
-We are very reluctant with this one. Nx5d is primarily developed
-to help with rapid data analysis "from scratch", and by its very
-nature this will always require minor adjustments in Python code.
+We are very reluctant with this one. nx5d is primarily developed
+to help with rapid data analysis "from scratch" and by its very
+nature, this will always require minor adjustments in Python code.
 However, given a sufficiently abstract pipelining platform (like
 EWOKS), a graphical user interface to actually *help* the user
 without further restricting processing capabilities might be
 conceivable. We are at least open to the possibility.
```

### Comparing `nx5d-0.3.3/doc/mkdocs/frame.svg` & `nx5d-0.3.4/doc/mkdocs/frame.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/index.md` & `nx5d-0.3.4/doc/mkdocs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Nx5d -- A Rapid Data Analys Framework
+# Nx5d -- A Rapid Data Analysis Framework
 
 Nx5d is a Python framework for rapid data processing and analysis workflows
 in scienfic enviroments. It is aimed to be the first thing a physicist
-imports and uses in his or her Jupyter Lab notebook for on-line analysis,
+imports and uses in his or her Jupyter Lab notebook for on-line analysis
 during data acquisition.
 
 This is all it should take to visualize your X-ray diffraction data in 
 reciprocal space:
 
 ```
 import nx5d, h5py, json
@@ -69,15 +69,15 @@
   - Improving code, e.g. by writing unit tests, developing data
     analysis methods, adding HDF5-like interfaces for new data
 	formats or experimental setups
 	
   - ...or diving straight in and contributing to the concepts and
     core part of the code :-)
 	
-So pick your fight! And aemember that [if you break it, you get to keep both pieces.](https://english.stackexchange.com/questions/118717/how-is-the-phrase-when-your-program-breaks-you-get-to-keep-both-pieces-commo) :-)
+So pick your fight! And remember that [if you break it, you get to keep both pieces.](https://english.stackexchange.com/questions/118717/how-is-the-phrase-when-your-program-breaks-you-get-to-keep-both-pieces-commo) :-)
 
 The main repository around which nx5d development happens is
 [over at GitLab](https://gitlab.com/codedump2/nx5d). If enough
 interest prevails, we're pondering setting up a mailing list
 and a dedicated website.
```

### Comparing `nx5d-0.3.3/doc/mkdocs/license.md` & `nx5d-0.3.4/doc/mkdocs/license.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/module-nx.md` & `nx5d-0.3.4/doc/mkdocs/module-nx.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/scan.svg` & `nx5d-0.3.4/doc/mkdocs/scan.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/streak1.svg` & `nx5d-0.3.4/doc/mkdocs/streak1.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/streak2.svg` & `nx5d-0.3.4/doc/mkdocs/streak2.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/tutorials/index.md` & `nx5d-0.3.4/doc/mkdocs/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md` & `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png` & `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png` & `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png` & `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png` & `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png` & `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md` & `nx5d-0.3.4/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/doc/mkdocs.yml` & `nx5d-0.3.4/doc/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/scratch.org` & `nx5d-0.3.4/scratch.org`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/setup.cfg` & `nx5d-0.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/edf.py` & `nx5d-0.3.4/src/nx5d/edf.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/h5like/pypod.py` & `nx5d-0.3.4/src/nx5d/h5like/pypod.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/h5like/tools.py` & `nx5d-0.3.4/src/nx5d/h5like/tools.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/h5like/xfel.py` & `nx5d-0.3.4/src/nx5d/h5like/xfel.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/nx.py` & `nx5d-0.3.4/src/nx5d/nx.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/runlog.py` & `nx5d-0.3.4/src/nx5d/runlog.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/scan.py` & `nx5d-0.3.4/src/nx5d/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,45 @@
 from numpy import array as np_array
 
 import logging
 
 from nx5d.h5like.tools import *
 
 __all__ = [ "ScanReader" ]
+
+'''
+The Scan-Streak-Frame concept uses the following HDF5 API elements
+to implement sophisticated iteration and slicing helpers:
+
+  - Accessing of data using slicers and the indexing operator (`__getitem__`).
+
+  - `__getitem__` access works both for selecting paths / subpaths, or selecting
+    data containers within paths, or slicing parts of the data container itself,
+    i.e. sub-access to limited parts of the images (i.e. only specific
+    region-of-interests) via slicing. Examples:
+    ```
+      data["detector"] -> directory containing the "acme" subdirectory
+
+      data["detector/acme"] -> directory, containing the "images" dataset
+      data["detector"]["acme"] -> same as above
+
+      data["detector/acme/images"] -> the dataset itself
+      data["detector"]["acme"]["images"] -> same as above
+
+      data["detector/acme/images"][3] -> image no. 3 from the dataset
+
+      data["detector/acme/images"][3][60:160,60:160] -> a 100x100 pixel area centered
+                                                        around pixel 110x110 of image no. 3
+
+    ```
+
+  - The HDF5 taxonomy (i.e. the '.attrs' dictionary
+
+  - We're not using any HDF5 specific properties or Python attributes.
+'''
     
 class ScanReader:
     '''
     Loads data from one X-ray diffraction (XRD) scan run and offers
     convesion of images to Q space for further analysis.
     
     The idea is to open/initialize metadata (experimental parameters,
```

### Comparing `nx5d-0.3.3/src/nx5d/streaks.py` & `nx5d-0.3.4/src/nx5d/streaks.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/xrd/ColonelSandersFinest.py` & `nx5d-0.3.4/src/nx5d/xrd/ColonelSandersFinest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/xrd/analysis.py` & `nx5d-0.3.4/src/nx5d/xrd/analysis.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/xrd/esrf_id09.py` & `nx5d-0.3.4/src/nx5d/xrd/esrf_id09.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/xrd/experiment-xpp.yml` & `nx5d-0.3.4/src/nx5d/xrd/experiment-xpp.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/xrd/experiment.py` & `nx5d-0.3.4/src/nx5d/xrd/experiment.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/xrd/roi.py` & `nx5d-0.3.4/src/nx5d/xrd/roi.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/xrd/signal.py` & `nx5d-0.3.4/src/nx5d/xrd/signal.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/xrd/xfel.py` & `nx5d-0.3.4/src/nx5d/xrd/xfel.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/xrd/xraytest.py` & `nx5d-0.3.4/src/nx5d/xrd/xraytest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d/xrd/xrd_helpers.py` & `nx5d-0.3.4/src/nx5d/xrd/xrd_helpers.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/src/nx5d.egg-info/PKG-INFO` & `nx5d-0.3.4/src/nx5d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.3
+Version: 0.3.4
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.3/src/nx5d.egg-info/SOURCES.txt` & `nx5d-0.3.4/src/nx5d.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 src/nx5d/streaks.py
 src/nx5d.egg-info/PKG-INFO
 src/nx5d.egg-info/SOURCES.txt
 src/nx5d.egg-info/dependency_links.txt
 src/nx5d.egg-info/requires.txt
 src/nx5d.egg-info/top_level.txt
 src/nx5d/h5like/__init__.py
+src/nx5d/h5like/petra3.py
 src/nx5d/h5like/pypod.py
+src/nx5d/h5like/spec.py
 src/nx5d/h5like/tools.py
 src/nx5d/h5like/xfel.py
 src/nx5d/xrd/ColonelSandersFinest.py
 src/nx5d/xrd/__init__.py
 src/nx5d/xrd/analysis.py
 src/nx5d/xrd/esrf_id09.py
 src/nx5d/xrd/experiment-xpp.yml
@@ -52,20 +54,24 @@
 src/nx5d/xrd/kmc3.py
 src/nx5d/xrd/roi.py
 src/nx5d/xrd/signal.py
 src/nx5d/xrd/xfel.py
 src/nx5d/xrd/xraytest.py
 src/nx5d/xrd/xrd_helpers.py
 tests/.gitignore
+tests/fio_test.py
 tests/pabst_test.py
 tests/pypod_test.py
 tests/runlog_test.py
+tests/spec_test.py
 tests/xfel_test.py
 tests/xrd_data_test.py
-tests/xrd_kmc3_test.py
+tests/test_data/fioh5/m3_2507_00342.fio
+tests/test_data/fioh5/m3_2507_00744.fio
+tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs
 tests/test_data/runfile/run04.log
 tests/test_data/runfile/run105.log
 tests/test_data/runfile/run105_brokendata1.log
 tests/test_data/runfile/run105_brokendata2.log
 tests/test_data/runfile/run105_brokenheader.log
 tests/test_data/runfile/run105_simple.log
 tests/test_data/runfile/short_run04.log
```

### Comparing `nx5d-0.3.3/tests/pabst_test.py` & `nx5d-0.3.4/tests/pabst_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/pypod_test.py` & `nx5d-0.3.4/tests/pypod_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/runlog_test.py` & `nx5d-0.3.4/tests/runlog_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/run04.log` & `nx5d-0.3.4/tests/test_data/runfile/run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/run105.log` & `nx5d-0.3.4/tests/test_data/runfile/run105.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/run105_brokendata1.log` & `nx5d-0.3.4/tests/test_data/runfile/run105_brokendata1.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/run105_brokendata2.log` & `nx5d-0.3.4/tests/test_data/runfile/run105_brokendata2.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/run105_brokenheader.log` & `nx5d-0.3.4/tests/test_data/runfile/run105_brokenheader.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/run105_simple.log` & `nx5d-0.3.4/tests/test_data/runfile/run105_simple.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04.log` & `nx5d-0.3.4/tests/test_data/runfile/short_run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0001.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0001.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0002.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0002.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0003.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0003.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0004.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0004.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0005.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0005.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0006.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0006.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0007.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0007.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0008.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0008.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0009.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0009.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0010.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0010.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0011.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0011.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0012.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0012.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0013.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0013.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0014.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0014.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0015.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0015.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0016.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0016.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0017.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0017.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0018.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0018.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0019.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0019.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0020.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0020.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0021.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0021.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0022.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0022.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0023.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0023.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0024.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0024.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0025.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0025.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0026.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0026.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0027.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0027.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0028.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0028.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0029.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0029.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0030.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0030.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0031.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0031.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0032.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0032.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0033.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0033.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0034.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0034.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0035.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0035.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0036.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0036.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/runfile/short_run04_0037.edf` & `nx5d-0.3.4/tests/test_data/runfile/short_run04_0037.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif` & `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/xfel_test.py` & `nx5d-0.3.4/tests/xfel_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/xrd_data_test.py` & `nx5d-0.3.4/tests/xrd_data_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.3/tests/xrd_kmc3_test.py` & `nx5d-0.3.4/tests/spec_test.py`

 * *Files identical despite different names*


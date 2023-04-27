# Comparing `tmp/ecl-data-io-3.0.0b0.tar.gz` & `tmp/ecl-data-io-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecl-data-io-3.0.0b0.tar", last modified: Sat Jul 30 13:38:17 2022, max compression
+gzip compressed data, was "ecl-data-io-3.0.0b1.tar", last modified: Thu Apr 27 09:57:52 2023, max compression
```

## Comparing `ecl-data-io-3.0.0b0.tar` & `ecl-data-io-3.0.0b1.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:17.416910 ecl-data-io-3.0.0b0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:17.404910 ecl-data-io-3.0.0b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:17.408910 ecl-data-io-3.0.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7653 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-07-30 13:38:17.416910 ecl-data-io-3.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:17.404910 ecl-data-io-3.0.0b0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:17.408910 ecl-data-io-3.0.0b0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/docs/source/api_doc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/docs/source/developer_guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/docs/source/error_handling.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3197 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/docs/source/example_usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/docs/source/the_file_format.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-07-30 13:38:17.416910 ecl-data-io-3.0.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:17.404910 ecl-data-io-3.0.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:17.408910 ecl-data-io-3.0.0b0/src/ecl_data_io/
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:17.412910 ecl-data-io-3.0.0b0/src/ecl_data_io/_formatted/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/_formatted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/_formatted/read.py
--rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/_formatted/write.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:17.412910 ecl-data-io-3.0.0b0/src/ecl_data_io/_unformatted/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/_unformatted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/_unformatted/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     5689 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/_unformatted/read.py
--rw-r--r--   0 runner    (1001) docker     (121)     4267 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/_unformatted/write.py
--rw-r--r--   0 runner    (1001) docker     (121)     3053 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/array_entry.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/format.py
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/read.py
--rw-r--r--   0 runner    (1001) docker     (121)     3856 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/src/ecl_data_io/write.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:17.408910 ecl-data-io-3.0.0b0/src/ecl_data_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-07-30 13:38:17.000000 ecl-data-io-3.0.0b0/src/ecl_data_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-07-30 13:38:17.000000 ecl-data-io-3.0.0b0/src/ecl_data_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 13:38:17.000000 ecl-data-io-3.0.0b0/src/ecl_data_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-07-30 13:38:17.000000 ecl-data-io-3.0.0b0/src/ecl_data_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-30 13:38:17.000000 ecl-data-io-3.0.0b0/src/ecl_data_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:17.416910 ecl-data-io-3.0.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/generators.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/test_formatted_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/test_formatted_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/test_formatted_read_write.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/test_formatted_write.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/test_read_write.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8974 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/test_unformatted_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/test_unformatted_read_write.py
--rw-r--r--   0 runner    (1001) docker     (121)     3830 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/test_unformatted_write.py
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-07-30 13:38:06.000000 ecl-data-io-3.0.0b0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.981689 ecl-data-io-3.0.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.973688 ecl-data-io-3.0.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.973688 ecl-data-io-3.0.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-27 09:57:52.981689 ecl-data-io-3.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.973688 ecl-data-io-3.0.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.977689 ecl-data-io-3.0.0b1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/api_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/developer_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/error_handling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/example_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/the_file_format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-27 09:57:52.981689 ecl-data-io-3.0.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.973688 ecl-data-io-3.0.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.977689 ecl-data-io-3.0.0b1/src/ecl_data_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.977689 ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.977689 ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/array_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.977689 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-27 09:57:52.000000 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-27 09:57:52.000000 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:57:52.000000 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 09:57:52.000000 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 09:57:52.000000 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.981689 ecl-data-io-3.0.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_formatted_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_formatted_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_formatted_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_formatted_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_type_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_unformatted_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_unformatted_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_unformatted_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tox.ini
```

### Comparing `ecl-data-io-3.0.0b0/.github/workflows/publish_to_pypi.yml` & `ecl-data-io-3.0.0b1/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/.github/workflows/testing.yml` & `ecl-data-io-3.0.0b1/.github/workflows/testing.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   tests:
     name: "Python ${{ matrix.python-version }}"
     runs-on: "ubuntu-latest"
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10"]
 
     steps:
       - uses: actions/checkout@v1
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `ecl-data-io-3.0.0b0/LICENSE.md` & `ecl-data-io-3.0.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/PKG-INFO` & `ecl-data-io-3.0.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: ecl-data-io
-Version: 3.0.0b0
+Version: 3.0.0b1
 Summary: A (lazy) parser and writer for the ecl output format.
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>
 License: LGPL-3.0
 Project-URL: Homepage, https://github.com/equinor/ecl-data-io
 Project-URL: Repository, https://github.com/equinor/ecl-data-io
 Project-URL: Documentation, https://ecl-data-io.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/equinor/ecl-data-io/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE.md
```

### Comparing `ecl-data-io-3.0.0b0/README.md` & `ecl-data-io-3.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/docs/source/developer_guide.rst` & `ecl-data-io-3.0.0b1/docs/source/developer_guide.rst`

 * *Files 22% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 ecl-data-io is set up to use tox which can simplify development,
 but all that is necessary in order to get started is git, pip and python:
 
 First, install ecl-data-io in editable mode:
 
 .. code-block:: console
 
-git clone git@github.com:equinor/ecl-data-io.git
-cd ecl-data-io
-pip install -e .
+    git clone git@github.com:equinor/ecl-data-io.git
+    cd ecl-data-io
+    pip install -e .
 
 Second, install the dev-requirements.txt, which contains the packages ecl-data-io
 require in order to run tests:
 
 .. code-block:: console
 
-pip install -r dev-requirements.txt
+    pip install -r dev-requirements.txt
 
 At last, you can use pytest to run the tests
 
 .. code-block:: console
 
-pytest tests
+    pytest tests
```

### Comparing `ecl-data-io-3.0.0b0/docs/source/error_handling.rst` & `ecl-data-io-3.0.0b1/docs/source/error_handling.rst`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/docs/source/example_usage.rst` & `ecl-data-io-3.0.0b1/docs/source/example_usage.rst`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/docs/source/index.rst` & `ecl-data-io-3.0.0b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/docs/source/the_file_format.rst` & `ecl-data-io-3.0.0b1/docs/source/the_file_format.rst`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/pyproject.toml` & `ecl-data-io-3.0.0b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 name = "ecl-data-io"
 description="A (lazy) parser and writer for the ecl output format."
 readme = "README.md"
 classifiers=[
     "Development Status :: 1 - Planning",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = ["numpy"]
 dynamic=["version"]
```

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io/_formatted/read.py` & `ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/read.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io/_formatted/write.py` & `ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io/_unformatted/common.py` & `ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/common.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io/_unformatted/read.py` & `ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/read.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io/_unformatted/write.py` & `ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io/array_entry.py` & `ecl-data-io-3.0.0b1/src/ecl_data_io/array_entry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Optional, Union
+
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike
+
+    from .types import ArrayValue
 
 
 class EclArray(ABC):
     """
     An array entry in a ecl file.
 
     This class is not ment to be constructed directly, but rather
@@ -31,53 +37,57 @@
         at the end of the file, in which case its keyword
         and array is None.
         """
         if self._keyword is None:
             self._read()
         return self._is_eof
 
-    def read_keyword(self):
+    def read_keyword(self) -> str:
         """
         Read the keyword from the ecl file.
 
         :returns: The keyword as a 8 character string.
         """
         if self._keyword is None:
             self._read()
-        return self._keyword
+        return self._keyword  # type: ignore
 
-    def read_length(self):
+    def read_length(self) -> int:
         """
         Read the length from the ecl file.
 
         :returns: The length of the array in number of entries.
         """
         if self._length is None:
             self._read()
-        return self._length
+        return self._length  # type: ignore
 
     @abstractmethod
-    def read_array(self):
+    def read_array(self) -> "ArrayValue":
         """
         Read the array from the unformatted ecl file.
 
         :returns: numpy array of values.
         """
         pass
 
-    def read_type(self):
+    def read_type(self) -> Union[str, bytes]:
         """
-        The type given in the header of the array
+        The type given in the header of the array.
+        In case of unformatted file this will be bytes, for
+        unformatted files it is str.
         """
         if self._type is None:
             self._read()
-        return self._type
+        return self._type  # type: ignore
 
     @abstractmethod
-    def update(self, *, keyword=None, array=None):
+    def update(
+        self, *, keyword: Optional[str] = None, array: Optional["ArrayLike"] = None
+    ):
         """
         Updates the entry with the given new data.
 
         :param new_keyword: The new keyword, must be 8 characters, defaults to no change.
         :param new_array: The new array, must be of same type and size
             as existing array, defaults to no change.
```

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io/format.py` & `ecl-data-io-3.0.0b1/src/ecl_data_io/format.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     filelike.seek(goback)
     if isinstance(bytes_or_str, bytes):
         return Format.UNFORMATTED
     else:
         return Format.FORMATTED
 
 
-def get_stream(filepath, fileformat, mode="r"):
+def get_stream(filepath, fileformat: Format, mode: str = "r"):
     """
     Openes the given file with the correct mode (text or binary)
     based on fileformat.
     :param filepath: Either a filename or pathlib.Path
     :param fileformat: A ecl_data_io.Format.
     :returns: The opened file.
     """
@@ -54,15 +54,15 @@
             return open(filepath, mode + "t"), True
         else:
             return open(filepath, mode + "b"), True
     else:
         return filepath, False
 
 
-def check_correct_mode(stream, fileformat):
+def check_correct_mode(stream, fileformat: Format):
     """
     Checks that the stream is the correct mode (text or binary) for the given
     fileformat.
     """
     if isinstance(stream, io.TextIOBase) and fileformat == Format.UNFORMATTED:
         raise ValueError(
             "Formatted file was opened in byte reading mode, should be text mode"
```

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io/read.py` & `ecl-data-io-3.0.0b1/src/ecl_data_io/read.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-from pathlib import Path
+from typing import TYPE_CHECKING, Iterator, List, Optional, Tuple
 
 from ecl_data_io._formatted.read import FormattedEclArray
 from ecl_data_io._unformatted.read import UnformattedEclArray
+from ecl_data_io.array_entry import EclArray
 from ecl_data_io.format import Format, check_correct_mode, get_stream, guess_format
 
+if TYPE_CHECKING:
+    from .types import ArrayValue
 
-def read(*args, **kwargs):
+
+def read(*args, **kwargs) -> List[Tuple[str, "ArrayValue"]]:
     """
     Read the contents of a ecl file and return a list of
     tuples (keyword, array). Takes the same parameters as
     lazy_read, but differs in return type
     """
     return [
         (arr.read_keyword(), arr.read_array()) for arr in lazy_read(*args, **kwargs)
     ]
 
 
-def lazy_read(filelike, fileformat=None):
+def lazy_read(filelike, fileformat: Optional[Format] = None) -> Iterator[EclArray]:
     """
     Reads the contents of an ecl file and generates the entries
     of that file. Each entry has a entry.read_keyword() and
     entry.read_array() method which will return the corresponding
     data, but only upon request. This requires the user to
     pay attention to when values are read as it should happen
     before the file is closed.
```

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io/types.py` & `ecl-data-io-3.0.0b1/src/ecl_data_io/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 
 ecl_data_io converts ecl types to corresponding numpy dtypes
 and back. Some numpy dtypes will give a loss of precision and
 that results in a warning.
 
 """
 import warnings
+from typing import Union
 
 import numpy as np
+from numpy.typing import ArrayLike
 
 # np dtype for ecl types with fixed width
 static_dtypes = {
     b"INTE": np.dtype(np.int32).newbyteorder(">"),
     b"REAL": np.dtype(np.float32).newbyteorder(">"),
     b"LOGI": np.dtype(np.int32).newbyteorder(">"),
     b"DOUB": np.dtype(np.float64).newbyteorder(">"),
@@ -41,14 +43,17 @@
     The MESS value is a sentinell object used to signal that the type of the
     array that is to be written should be an empty array of type MESS.
     """
 
     pass
 
 
+ArrayValue = Union[ArrayLike, MESS]
+
+
 def to_np_type(type_keyword):
     """
     :param type_keyword: A bytestring of a ecl type.
     :returns: A np dtype corresponding to the given
         ecl type.
     """
     if type_keyword[0:2] == b"C0":
```

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io/write.py` & `ecl-data-io-3.0.0b1/src/ecl_data_io/write.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-from pathlib import Path
+from typing import Dict, Sequence, Tuple, Union
 
 from ecl_data_io._formatted.write import formatted_write
 from ecl_data_io._unformatted.write import unformatted_write
 from ecl_data_io.format import Format, check_correct_mode, get_stream
 
+from .types import ArrayValue
 
-def write(filelike, contents, fileformat=Format.UNFORMATTED):
+
+def write(
+    filelike,
+    contents: Union[Sequence[Tuple[str, ArrayValue]], Dict[str, ArrayValue]],
+    fileformat: Format = Format.UNFORMATTED,
+):
     """
     Write the given contents to the given file in ecl format.
 
     :param filelike: Either filename, pathlib.Path or stream
         to write file to. For fileformat=Format.UNFORMATTED the
         stream must be in binary mode and for fileformat=Format.FORMATTED
         in text mode.
```

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io.egg-info/PKG-INFO` & `ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: ecl-data-io
-Version: 3.0.0b0
+Version: 3.0.0b1
 Summary: A (lazy) parser and writer for the ecl output format.
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>
 License: LGPL-3.0
 Project-URL: Homepage, https://github.com/equinor/ecl-data-io
 Project-URL: Repository, https://github.com/equinor/ecl-data-io
 Project-URL: Documentation, https://ecl-data-io.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/equinor/ecl-data-io/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE.md
```

### Comparing `ecl-data-io-3.0.0b0/src/ecl_data_io.egg-info/SOURCES.txt` & `ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 conftest.py
 pyproject.toml
 setup.cfg
 tox.ini
 .github/workflows/lint.yml
 .github/workflows/publish_to_pypi.yml
 .github/workflows/testing.yml
+docs/requirements.txt
 docs/source/api_doc.rst
 docs/source/conf.py
 docs/source/developer_guide.rst
 docs/source/error_handling.rst
 docs/source/example_usage.rst
 docs/source/index.rst
 docs/source/the_file_format.rst
@@ -41,12 +42,13 @@
 tests/generators.py
 tests/test_error_handling.py
 tests/test_formatted_common.py
 tests/test_formatted_read.py
 tests/test_formatted_read_write.py
 tests/test_formatted_write.py
 tests/test_read_write.py
+tests/test_type_resolution.py
 tests/test_types.py
 tests/test_unformatted_read.py
 tests/test_unformatted_read_write.py
 tests/test_unformatted_write.py
 tests/test_update.py
```

### Comparing `ecl-data-io-3.0.0b0/tests/generators.py` & `ecl-data-io-3.0.0b1/tests/generators.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/tests/test_error_handling.py` & `ecl-data-io-3.0.0b1/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/tests/test_formatted_common.py` & `ecl-data-io-3.0.0b1/tests/test_formatted_common.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/tests/test_formatted_read.py` & `ecl-data-io-3.0.0b1/tests/test_formatted_read.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/tests/test_formatted_read_write.py` & `ecl-data-io-3.0.0b1/tests/test_formatted_read_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
             ("KEYWORDS", np.array(["HELLO WORLD"], dtype="|S")),
             ("KEYWORDU", np.array(["HELLO WORLD"], dtype="|U")),
             ("KEYWORDU", np.array(["HELLO WORLD"], dtype="|U11")),
         ],
     ],
 )
 def test_formatted_write(container, data, tmp_path):
-
     with (tmp_path / "test.data").open("wt") as fh:
         formatted_write(fh, container(data))
 
     with (tmp_path / "test.data").open("rt") as fh:
         out_records = list(FormattedEclArray.parse(fh))
         out_keywords = [r.read_keyword() for r in out_records]
         out_arrays = [r.read_array() for r in out_records]
```

### Comparing `ecl-data-io-3.0.0b0/tests/test_formatted_write.py` & `ecl-data-io-3.0.0b1/tests/test_formatted_write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/tests/test_read_write.py` & `ecl-data-io-3.0.0b1/tests/test_read_write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/tests/test_types.py` & `ecl-data-io-3.0.0b1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/tests/test_unformatted_read.py` & `ecl-data-io-3.0.0b1/tests/test_unformatted_read.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/tests/test_unformatted_read_write.py` & `ecl-data-io-3.0.0b1/tests/test_unformatted_read_write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/tests/test_unformatted_write.py` & `ecl-data-io-3.0.0b1/tests/test_unformatted_write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b0/tests/test_update.py` & `ecl-data-io-3.0.0b1/tests/test_update.py`

 * *Files identical despite different names*


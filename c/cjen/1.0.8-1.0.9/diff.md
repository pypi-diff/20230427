# Comparing `tmp/cjen-1.0.8.tar.gz` & `tmp/cjen-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjen-1.0.8.tar", last modified: Fri Dec  2 11:52:08 2022, max compression
+gzip compressed data, was "cjen-1.0.9.tar", last modified: Thu Apr 27 01:58:17 2023, max compression
```

## Comparing `cjen-1.0.8.tar` & `cjen-1.0.9.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.523958 cjen-1.0.8/
--rw-rw-rw-   0        0        0     1073 2022-02-04 16:23:58.000000 cjen-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     2814 2022-12-02 11:52:08.523958 cjen-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2338 2022-12-02 11:47:07.000000 cjen-1.0.8/README.md
--rw-rw-rw-   0        0        0      103 2022-02-04 17:03:06.000000 cjen-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      802 2022-12-02 11:52:08.528943 cjen-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.229842 cjen-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.273283 cjen-1.0.8/src/cjen/
--rw-rw-rw-   0        0        0      668 2022-06-22 09:52:42.000000 cjen-1.0.8/src/cjen/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.324082 cjen-1.0.8/src/cjen/aiai/
--rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.8/src/cjen/aiai/__init__.py
--rw-rw-rw-   0        0        0      734 2022-05-10 04:49:20.000000 cjen-1.0.8/src/cjen/aiai/context.py
--rw-rw-rw-   0        0        0     9324 2022-02-28 05:46:09.000000 cjen-1.0.8/src/cjen/aiai/file-content-type.yaml
--rw-rw-rw-   0        0        0     3736 2022-05-10 04:49:20.000000 cjen-1.0.8/src/cjen/aiai/headers.py
--rw-rw-rw-   0        0        0    13357 2022-06-30 09:10:44.000000 cjen-1.0.8/src/cjen/aiai/http.py
--rw-rw-rw-   0        0        0     1585 2022-05-10 04:49:20.000000 cjen-1.0.8/src/cjen/aiai/jwt.py
--rw-rw-rw-   0        0        0     2953 2022-06-24 09:46:06.000000 cjen-1.0.8/src/cjen/bigtangerine.py
--rw-rw-rw-   0        0        0     1041 2022-02-07 09:57:47.000000 cjen-1.0.8/src/cjen/commons.py
--rw-rw-rw-   0        0        0      740 2022-02-16 02:40:53.000000 cjen-1.0.8/src/cjen/context.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.332059 cjen-1.0.8/src/cjen/dada/
--rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.8/src/cjen/dada/__init__.py
--rw-rw-rw-   0        0        0     2451 2022-05-10 04:49:20.000000 cjen-1.0.8/src/cjen/dada/smile.py
--rw-rw-rw-   0        0        0     3580 2022-02-25 02:06:00.000000 cjen-1.0.8/src/cjen/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.339041 cjen-1.0.8/src/cjen/mama/
--rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.8/src/cjen/mama/__init__.py
--rw-rw-rw-   0        0        0      865 2022-05-10 04:49:20.000000 cjen-1.0.8/src/cjen/mama/meta_data.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.368961 cjen-1.0.8/src/cjen/mama/operate/
--rw-rw-rw-   0        0        0      150 2022-02-07 09:57:47.000000 cjen-1.0.8/src/cjen/mama/operate/__init__.py
--rw-rw-rw-   0        0        0     5555 2022-02-17 05:59:22.000000 cjen-1.0.8/src/cjen/mama/operate/asserts.py
--rw-rw-rw-   0        0        0     1216 2022-05-10 04:49:20.000000 cjen-1.0.8/src/cjen/mama/operate/common.py
--rw-rw-rw-   0        0        0     4653 2022-08-03 06:42:53.000000 cjen-1.0.8/src/cjen/mama/operate/json.py
--rw-rw-rw-   0        0        0     5528 2022-12-02 11:51:18.000000 cjen-1.0.8/src/cjen/mama/operate/mysql.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.394133 cjen-1.0.8/src/cjen/nene/
--rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.8/src/cjen/nene/__init__.py
--rw-rw-rw-   0        0        0      636 2022-08-03 06:42:53.000000 cjen-1.0.8/src/cjen/nene/caculate_utils.py
--rw-rw-rw-   0        0        0      850 2022-02-07 09:57:47.000000 cjen-1.0.8/src/cjen/nene/database_pool.py
--rw-rw-rw-   0        0        0      937 2022-02-16 02:40:53.000000 cjen-1.0.8/src/cjen/nene/helper.py
--rw-rw-rw-   0        0        0      801 2022-08-03 06:42:53.000000 cjen-1.0.8/src/cjen/nene/time_utils.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.418266 cjen-1.0.8/src/cjen/sco/
--rw-rw-rw-   0        0        0        0 2022-06-02 08:29:55.000000 cjen-1.0.8/src/cjen/sco/__init__.py
--rw-rw-rw-   0        0        0     1971 2022-08-04 06:46:30.000000 cjen-1.0.8/src/cjen/sco/scenario.py
--rw-rw-rw-   0        0        0     1615 2022-08-04 06:55:09.000000 cjen-1.0.8/src/cjen/sco/standard_step.py
--rw-rw-rw-   0        0        0      382 2022-06-22 09:52:42.000000 cjen-1.0.8/src/cjen/sco/step.py
--rw-rw-rw-   0        0        0      174 2022-06-02 08:29:55.000000 cjen-1.0.8/src/cjen/sco/step_definitions.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.435250 cjen-1.0.8/src/cjen/tests/
--rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.8/src/cjen/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.466796 cjen-1.0.8/src/cjen/tests/aiai/
--rw-rw-rw-   0        0        0        0 2022-02-16 02:40:53.000000 cjen-1.0.8/src/cjen/tests/aiai/__init__.py
--rw-rw-rw-   0        0        0      358 2022-02-16 02:40:53.000000 cjen-1.0.8/src/cjen/tests/aiai/conftest.py
--rw-rw-rw-   0        0        0     2283 2022-05-10 04:49:20.000000 cjen-1.0.8/src/cjen/tests/aiai/test_header.py
--rw-rw-rw-   0        0        0     5091 2022-06-24 10:23:08.000000 cjen-1.0.8/src/cjen/tests/aiai/test_http.py
--rw-rw-rw-   0        0        0     2608 2022-05-10 04:49:20.000000 cjen-1.0.8/src/cjen/tests/aiai/test_jwt.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.475149 cjen-1.0.8/src/cjen/tests/common/
--rw-rw-rw-   0        0        0        0 2022-02-16 02:40:53.000000 cjen-1.0.8/src/cjen/tests/common/__init__.py
--rw-rw-rw-   0        0        0     1043 2022-02-16 02:40:53.000000 cjen-1.0.8/src/cjen/tests/common/test_context_manager.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.495103 cjen-1.0.8/src/cjen/tests/dada/
--rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.8/src/cjen/tests/dada/__init__.py
--rw-rw-rw-   0        0        0      275 2022-02-07 09:57:47.000000 cjen-1.0.8/src/cjen/tests/dada/test_delay.py
--rw-rw-rw-   0        0        0     2080 2022-05-10 04:49:20.000000 cjen-1.0.8/src/cjen/tests/dada/test_smile_parallel1.py
--rw-rw-rw-   0        0        0     2055 2022-05-10 04:49:20.000000 cjen-1.0.8/src/cjen/tests/dada/test_smile_parallel2.py
--rw-rw-rw-   0        0        0      139 2022-02-22 10:41:46.000000 cjen-1.0.8/src/cjen/tests/main_app.py
--rw-rw-rw-   0        0        0     6457 2022-06-22 09:52:42.000000 cjen-1.0.8/src/cjen/tests/mock_service.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.521962 cjen-1.0.8/src/cjen/tests/step/
--rw-rw-rw-   0        0        0        0 2022-06-22 09:52:42.000000 cjen-1.0.8/src/cjen/tests/step/__init__.py
--rw-rw-rw-   0        0        0      358 2022-06-22 09:52:42.000000 cjen-1.0.8/src/cjen/tests/step/conftest.py
--rw-rw-rw-   0        0        0      299 2022-06-22 09:52:42.000000 cjen-1.0.8/src/cjen/tests/step/ok_response.py
--rw-rw-rw-   0        0        0      496 2022-06-24 09:46:06.000000 cjen-1.0.8/src/cjen/tests/step/ok_step.py
--rw-rw-rw-   0        0        0      500 2022-06-24 09:46:06.000000 cjen-1.0.8/src/cjen/tests/step/other_step.py
--rw-rw-rw-   0        0        0     1731 2022-06-24 10:23:08.000000 cjen-1.0.8/src/cjen/tests/step/test_step.py
-drwxrwxrwx   0        0        0        0 2022-12-02 11:52:08.285182 cjen-1.0.8/src/cjen.egg-info/
--rw-rw-rw-   0        0        0     2814 2022-12-02 11:52:08.000000 cjen-1.0.8/src/cjen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1683 2022-12-02 11:52:08.000000 cjen-1.0.8/src/cjen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-02 11:52:08.000000 cjen-1.0.8/src/cjen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2022-12-02 11:52:08.000000 cjen-1.0.8/src/cjen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-12-02 11:52:08.000000 cjen-1.0.8/src/cjen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.464698 cjen-1.0.9/
+-rw-rw-rw-   0        0        0     1073 2022-02-04 16:23:58.000000 cjen-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2881 2023-04-27 01:58:17.464698 cjen-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2405 2023-04-27 01:46:47.000000 cjen-1.0.9/README.md
+-rw-rw-rw-   0        0        0      103 2022-02-04 17:03:06.000000 cjen-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      813 2023-04-27 01:58:17.467689 cjen-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.104660 cjen-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.148543 cjen-1.0.9/src/cjen/
+-rw-rw-rw-   0        0        0      668 2022-06-22 09:52:42.000000 cjen-1.0.9/src/cjen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.209379 cjen-1.0.9/src/cjen/aiai/
+-rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.9/src/cjen/aiai/__init__.py
+-rw-rw-rw-   0        0        0      734 2022-05-10 04:49:20.000000 cjen-1.0.9/src/cjen/aiai/context.py
+-rw-rw-rw-   0        0        0     9324 2022-02-28 05:46:09.000000 cjen-1.0.9/src/cjen/aiai/file-content-type.yaml
+-rw-rw-rw-   0        0        0     3736 2022-05-10 04:49:20.000000 cjen-1.0.9/src/cjen/aiai/headers.py
+-rw-rw-rw-   0        0        0    13357 2022-06-30 09:10:44.000000 cjen-1.0.9/src/cjen/aiai/http.py
+-rw-rw-rw-   0        0        0     1585 2022-05-10 04:49:20.000000 cjen-1.0.9/src/cjen/aiai/jwt.py
+-rw-rw-rw-   0        0        0     2953 2022-06-24 09:46:06.000000 cjen-1.0.9/src/cjen/bigtangerine.py
+-rw-rw-rw-   0        0        0     1041 2022-02-07 09:57:47.000000 cjen-1.0.9/src/cjen/commons.py
+-rw-rw-rw-   0        0        0      740 2022-02-16 02:40:53.000000 cjen-1.0.9/src/cjen/context.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.218355 cjen-1.0.9/src/cjen/dada/
+-rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.9/src/cjen/dada/__init__.py
+-rw-rw-rw-   0        0        0     2451 2022-05-10 04:49:20.000000 cjen-1.0.9/src/cjen/dada/smile.py
+-rw-rw-rw-   0        0        0     3580 2022-02-25 02:06:00.000000 cjen-1.0.9/src/cjen/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.225336 cjen-1.0.9/src/cjen/mama/
+-rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.9/src/cjen/mama/__init__.py
+-rw-rw-rw-   0        0        0      865 2022-05-10 04:49:20.000000 cjen-1.0.9/src/cjen/mama/meta_data.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.261241 cjen-1.0.9/src/cjen/mama/operate/
+-rw-rw-rw-   0        0        0      186 2023-04-27 01:40:41.000000 cjen-1.0.9/src/cjen/mama/operate/__init__.py
+-rw-rw-rw-   0        0        0     5555 2022-02-17 05:59:22.000000 cjen-1.0.9/src/cjen/mama/operate/asserts.py
+-rw-rw-rw-   0        0        0     1216 2022-05-10 04:49:20.000000 cjen-1.0.9/src/cjen/mama/operate/common.py
+-rw-rw-rw-   0        0        0     4653 2022-08-03 06:42:53.000000 cjen-1.0.9/src/cjen/mama/operate/json.py
+-rw-rw-rw-   0        0        0     5528 2022-12-02 11:51:18.000000 cjen-1.0.9/src/cjen/mama/operate/mysql.py
+-rw-rw-rw-   0        0        0     2372 2023-04-27 01:40:41.000000 cjen-1.0.9/src/cjen/mama/operate/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.295150 cjen-1.0.9/src/cjen/nene/
+-rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.9/src/cjen/nene/__init__.py
+-rw-rw-rw-   0        0        0      636 2022-08-03 06:42:53.000000 cjen-1.0.9/src/cjen/nene/caculate_utils.py
+-rw-rw-rw-   0        0        0      623 2023-04-27 01:40:41.000000 cjen-1.0.9/src/cjen/nene/collection_utils.py
+-rw-rw-rw-   0        0        0      850 2022-02-07 09:57:47.000000 cjen-1.0.9/src/cjen/nene/database_pool.py
+-rw-rw-rw-   0        0        0      937 2022-02-16 02:40:53.000000 cjen-1.0.9/src/cjen/nene/helper.py
+-rw-rw-rw-   0        0        0      801 2022-08-03 06:42:53.000000 cjen-1.0.9/src/cjen/nene/time_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.330057 cjen-1.0.9/src/cjen/sco/
+-rw-rw-rw-   0        0        0        0 2022-06-02 08:29:55.000000 cjen-1.0.9/src/cjen/sco/__init__.py
+-rw-rw-rw-   0        0        0     1971 2022-08-04 06:46:30.000000 cjen-1.0.9/src/cjen/sco/scenario.py
+-rw-rw-rw-   0        0        0     1615 2022-08-04 06:55:09.000000 cjen-1.0.9/src/cjen/sco/standard_step.py
+-rw-rw-rw-   0        0        0      382 2022-06-22 09:52:42.000000 cjen-1.0.9/src/cjen/sco/step.py
+-rw-rw-rw-   0        0        0      174 2022-06-02 08:29:55.000000 cjen-1.0.9/src/cjen/sco/step_definitions.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.351000 cjen-1.0.9/src/cjen/tests/
+-rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.9/src/cjen/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.389897 cjen-1.0.9/src/cjen/tests/aiai/
+-rw-rw-rw-   0        0        0        0 2022-02-16 02:40:53.000000 cjen-1.0.9/src/cjen/tests/aiai/__init__.py
+-rw-rw-rw-   0        0        0      358 2022-02-16 02:40:53.000000 cjen-1.0.9/src/cjen/tests/aiai/conftest.py
+-rw-rw-rw-   0        0        0     2283 2022-05-10 04:49:20.000000 cjen-1.0.9/src/cjen/tests/aiai/test_header.py
+-rw-rw-rw-   0        0        0     5091 2022-06-24 10:23:08.000000 cjen-1.0.9/src/cjen/tests/aiai/test_http.py
+-rw-rw-rw-   0        0        0     2608 2022-05-10 04:49:20.000000 cjen-1.0.9/src/cjen/tests/aiai/test_jwt.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.397877 cjen-1.0.9/src/cjen/tests/common/
+-rw-rw-rw-   0        0        0        0 2022-02-16 02:40:53.000000 cjen-1.0.9/src/cjen/tests/common/__init__.py
+-rw-rw-rw-   0        0        0     1043 2022-02-16 02:40:53.000000 cjen-1.0.9/src/cjen/tests/common/test_context_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.423807 cjen-1.0.9/src/cjen/tests/dada/
+-rw-rw-rw-   0        0        0        0 2022-02-07 09:57:47.000000 cjen-1.0.9/src/cjen/tests/dada/__init__.py
+-rw-rw-rw-   0        0        0      275 2022-02-07 09:57:47.000000 cjen-1.0.9/src/cjen/tests/dada/test_delay.py
+-rw-rw-rw-   0        0        0     2080 2022-05-10 04:49:20.000000 cjen-1.0.9/src/cjen/tests/dada/test_smile_parallel1.py
+-rw-rw-rw-   0        0        0     2055 2022-05-10 04:49:20.000000 cjen-1.0.9/src/cjen/tests/dada/test_smile_parallel2.py
+-rw-rw-rw-   0        0        0      139 2022-02-22 10:41:46.000000 cjen-1.0.9/src/cjen/tests/main_app.py
+-rw-rw-rw-   0        0        0     6457 2022-06-22 09:52:42.000000 cjen-1.0.9/src/cjen/tests/mock_service.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.463700 cjen-1.0.9/src/cjen/tests/step/
+-rw-rw-rw-   0        0        0        0 2022-06-22 09:52:42.000000 cjen-1.0.9/src/cjen/tests/step/__init__.py
+-rw-rw-rw-   0        0        0      358 2022-06-22 09:52:42.000000 cjen-1.0.9/src/cjen/tests/step/conftest.py
+-rw-rw-rw-   0        0        0      299 2022-06-22 09:52:42.000000 cjen-1.0.9/src/cjen/tests/step/ok_response.py
+-rw-rw-rw-   0        0        0      496 2022-06-24 09:46:06.000000 cjen-1.0.9/src/cjen/tests/step/ok_step.py
+-rw-rw-rw-   0        0        0      500 2022-06-24 09:46:06.000000 cjen-1.0.9/src/cjen/tests/step/other_step.py
+-rw-rw-rw-   0        0        0     1731 2022-06-24 10:23:08.000000 cjen-1.0.9/src/cjen/tests/step/test_step.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:58:17.169487 cjen-1.0.9/src/cjen.egg-info/
+-rw-rw-rw-   0        0        0     2881 2023-04-27 01:58:17.000000 cjen-1.0.9/src/cjen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1747 2023-04-27 01:58:17.000000 cjen-1.0.9/src/cjen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 01:58:17.000000 cjen-1.0.9/src/cjen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-04-27 01:58:17.000000 cjen-1.0.9/src/cjen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 01:58:17.000000 cjen-1.0.9/src/cjen.egg-info/top_level.txt
```

### Comparing `cjen-1.0.8/LICENSE` & `cjen-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/PKG-INFO` & `cjen-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjen
-Version: 1.0.8
+Version: 1.0.9
 Summary: automation test helper
 Home-page: https://github.com/thcpc/cjen
 Author: thcpc
 Author-email: redcpc@163.com
 Project-URL: Bug Tracker, https://github.com/thcpc/cjen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -86,7 +86,10 @@
 - 1. 修复一些低级错误
 
 # Release 1.0.7
 - 1 . 针对 mysql 增加可通过函数参数传递查询参数，而不是一定需要通过上下文传递
 
 # Release 1.0.7
 - 1 . 修改查询参数为空时，设置查询参数为
+# Release 1.0.9
+- 1 . xlsx读取装饰器
+- 2 . list_eql 函数
```

### Comparing `cjen-1.0.8/README.md` & `cjen-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,8 +70,11 @@
 # Release 1.0.6.2
 - 1. 修复一些低级错误
 
 # Release 1.0.7
 - 1 . 针对 mysql 增加可通过函数参数传递查询参数，而不是一定需要通过上下文传递
 
 # Release 1.0.7
-- 1 . 修改查询参数为空时，设置查询参数为
+- 1 . 修改查询参数为空时，设置查询参数为
+# Release 1.0.9
+- 1 . xlsx读取装饰器
+- 2 . list_eql 函数
```

### Comparing `cjen-1.0.8/setup.cfg` & `cjen-1.0.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6a65 6e0d 0a76 6572 7369 6f6e   = cjen..version
-00000020: 203d 2031 2e30 2e38 0d0a 6175 7468 6f72   = 1.0.8..author
+00000020: 203d 2031 2e30 2e39 0d0a 6175 7468 6f72   = 1.0.9..author
 00000030: 203d 2074 6863 7063 0d0a 6175 7468 6f72   = thcpc..author
 00000040: 5f65 6d61 696c 203d 2072 6564 6370 6340  _email = redcpc@
 00000050: 3136 332e 636f 6d0d 0a64 6573 6372 6970  163.com..descrip
 00000060: 7469 6f6e 203d 2061 7574 6f6d 6174 696f  tion = automatio
 00000070: 6e20 7465 7374 2068 656c 7065 720d 0a6c  n test helper..l
 00000080: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000090: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
@@ -34,18 +34,18 @@
 00000210: 6378 0d0a 096a 736f 6e70 6174 680d 0a09  cx...jsonpath...
 00000220: 5079 4d79 5351 4c0d 0a09 7079 7465 7374  PyMySQL...pytest
 00000230: 0d0a 0950 7959 414d 4c0d 0a09 7265 7175  ...PyYAML...requ
 00000240: 6573 7473 0d0a 0972 6571 7565 7374 732d  ests...requests-
 00000250: 746f 6f6c 6265 6c74 0d0a 0972 7561 6d65  toolbelt...ruame
 00000260: 6c2e 7961 6d6c 0d0a 0972 7561 6d65 6c2e  l.yaml...ruamel.
 00000270: 7961 6d6c 2e63 6c69 620d 0a09 4442 5574  yaml.clib...DBUt
-00000280: 696c 730d 0a09 6368 6172 6465 740d 0a70  ils...chardet..p
-00000290: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-000002a0: 203e 3d33 2e39 0d0a 0d0a 5b6f 7074 696f   >=3.9....[optio
-000002b0: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
-000002c0: 0d0a 2a20 3d20 2a2e 7961 6d6c 0d0a 0d0a  ..* = *.yaml....
-000002d0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-000002e0: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-000002f0: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
-00000300: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000310: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000320: 0d0a                                     ..
+00000280: 696c 730d 0a09 6368 6172 6465 740d 0a09  ils...chardet...
+00000290: 6f70 656e 7079 786c 0d0a 7079 7468 6f6e  openpyxl..python
+000002a0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+000002b0: 390d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  9....[options.pa
+000002c0: 636b 6167 655f 6461 7461 5d0d 0a2a 203d  ckage_data]..* =
+000002d0: 202a 2e79 616d 6c0d 0a0d 0a5b 6f70 7469   *.yaml....[opti
+000002e0: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+000002f0: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+00000300: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000310: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000320: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `cjen-1.0.8/src/cjen/__init__.py` & `cjen-1.0.9/src/cjen/__init__.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/aiai/context.py` & `cjen-1.0.9/src/cjen/aiai/context.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/aiai/file-content-type.yaml` & `cjen-1.0.9/src/cjen/aiai/file-content-type.yaml`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/aiai/headers.py` & `cjen-1.0.9/src/cjen/aiai/headers.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/aiai/http.py` & `cjen-1.0.9/src/cjen/aiai/http.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/aiai/jwt.py` & `cjen-1.0.9/src/cjen/aiai/jwt.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/bigtangerine.py` & `cjen-1.0.9/src/cjen/bigtangerine.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/commons.py` & `cjen-1.0.9/src/cjen/commons.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/context.py` & `cjen-1.0.9/src/cjen/context.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/dada/smile.py` & `cjen-1.0.9/src/cjen/dada/smile.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/exceptions.py` & `cjen-1.0.9/src/cjen/exceptions.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/mama/meta_data.py` & `cjen-1.0.9/src/cjen/mama/meta_data.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/mama/operate/asserts.py` & `cjen-1.0.9/src/cjen/mama/operate/asserts.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/mama/operate/common.py` & `cjen-1.0.9/src/cjen/mama/operate/common.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/mama/operate/json.py` & `cjen-1.0.9/src/cjen/mama/operate/json.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/mama/operate/mysql.py` & `cjen-1.0.9/src/cjen/mama/operate/mysql.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/nene/caculate_utils.py` & `cjen-1.0.9/src/cjen/nene/caculate_utils.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/nene/database_pool.py` & `cjen-1.0.9/src/cjen/nene/database_pool.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/nene/helper.py` & `cjen-1.0.9/src/cjen/nene/helper.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/nene/time_utils.py` & `cjen-1.0.9/src/cjen/nene/time_utils.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/sco/scenario.py` & `cjen-1.0.9/src/cjen/sco/scenario.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/sco/standard_step.py` & `cjen-1.0.9/src/cjen/sco/standard_step.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/tests/aiai/test_header.py` & `cjen-1.0.9/src/cjen/tests/aiai/test_header.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/tests/aiai/test_http.py` & `cjen-1.0.9/src/cjen/tests/aiai/test_http.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/tests/aiai/test_jwt.py` & `cjen-1.0.9/src/cjen/tests/aiai/test_jwt.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/tests/common/test_context_manager.py` & `cjen-1.0.9/src/cjen/tests/common/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/tests/dada/test_smile_parallel1.py` & `cjen-1.0.9/src/cjen/tests/dada/test_smile_parallel1.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/tests/dada/test_smile_parallel2.py` & `cjen-1.0.9/src/cjen/tests/dada/test_smile_parallel2.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/tests/mock_service.py` & `cjen-1.0.9/src/cjen/tests/mock_service.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen/tests/step/test_step.py` & `cjen-1.0.9/src/cjen/tests/step/test_step.py`

 * *Files identical despite different names*

### Comparing `cjen-1.0.8/src/cjen.egg-info/PKG-INFO` & `cjen-1.0.9/src/cjen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjen
-Version: 1.0.8
+Version: 1.0.9
 Summary: automation test helper
 Home-page: https://github.com/thcpc/cjen
 Author: thcpc
 Author-email: redcpc@163.com
 Project-URL: Bug Tracker, https://github.com/thcpc/cjen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -86,7 +86,10 @@
 - 1. 修复一些低级错误
 
 # Release 1.0.7
 - 1 . 针对 mysql 增加可通过函数参数传递查询参数，而不是一定需要通过上下文传递
 
 # Release 1.0.7
 - 1 . 修改查询参数为空时，设置查询参数为
+# Release 1.0.9
+- 1 . xlsx读取装饰器
+- 2 . list_eql 函数
```

### Comparing `cjen-1.0.8/src/cjen.egg-info/SOURCES.txt` & `cjen-1.0.9/src/cjen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 src/cjen/mama/__init__.py
 src/cjen/mama/meta_data.py
 src/cjen/mama/operate/__init__.py
 src/cjen/mama/operate/asserts.py
 src/cjen/mama/operate/common.py
 src/cjen/mama/operate/json.py
 src/cjen/mama/operate/mysql.py
+src/cjen/mama/operate/xlsx.py
 src/cjen/nene/__init__.py
 src/cjen/nene/caculate_utils.py
+src/cjen/nene/collection_utils.py
 src/cjen/nene/database_pool.py
 src/cjen/nene/helper.py
 src/cjen/nene/time_utils.py
 src/cjen/sco/__init__.py
 src/cjen/sco/scenario.py
 src/cjen/sco/standard_step.py
 src/cjen/sco/step.py
```


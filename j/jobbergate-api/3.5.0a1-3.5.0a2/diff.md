# Comparing `tmp/jobbergate-api-3.5.0a1.tar.gz` & `tmp/jobbergate-api-3.5.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate-api-3.5.0a1.tar", max compression
+gzip compressed data, was "jobbergate-api-3.5.0a2.tar", max compression
```

## Comparing `jobbergate-api-3.5.0a1.tar` & `jobbergate-api-3.5.0a2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1082 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/LICENSE
--rw-r--r--   0        0        0      738 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/README.rst
--rw-r--r--   0        0        0      169 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0       41 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/__init__.py
--rw-r--r--   0        0        0     5655 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/application_files.py
--rw-r--r--   0        0        0      234 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/constants.py
--rw-r--r--   0        0        0     9408 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/file_validation.py
--rw-r--r--   0        0        0     1404 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/models.py
--rw-r--r--   0        0        0    13548 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/routers.py
--rw-r--r--   0        0        0     7239 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/schemas.py
--rw-r--r--   0        0        0       40 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0    12157 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/job_script_files.py
--rw-r--r--   0        0        0     1185 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    11747 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     3890 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0       44 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0      529 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     1910 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    12331 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/properties_parser.py
--rw-r--r--   0        0        0    18431 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0    14894 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0      554 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     3621 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/config.py
--rw-r--r--   0        0        0     2466 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     3268 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/main.py
--rw-r--r--   0        0        0     3433 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0       96 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/metadata.py
--rw-r--r--   0        0        0     3470 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/pagination.py
--rw-r--r--   0        0        0     2284 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/s3_manager.py
--rw-r--r--   0        0        0     2166 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/security.py
--rw-r--r--   0        0        0     5580 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/storage.py
--rw-r--r--   0        0        0       40 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/__init__.py
--rw-r--r--   0        0        0       44 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/__init__.py
--rw-r--r--   0        0        0    10634 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_application_files.py
--rw-r--r--   0        0        0     1967 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_file_validation.py
--rw-r--r--   0        0        0    41708 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_routers.py
--rw-r--r--   0        0        0     5180 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_schemas.py
--rw-r--r--   0        0        0     2756 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/conftest.py
--rw-r--r--   0        0        0       42 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     1376 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/conftest.py
--rw-r--r--   0        0        0    11518 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
--rw-r--r--   0        0        0    42583 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/test_routers.py
--rw-r--r--   0        0        0       46 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0    23970 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
--rw-r--r--   0        0        0    78149 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_submissions/test_routers.py
--rw-r--r--   0        0        0      511 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/test_main.py
--rw-r--r--   0        0        0     8900 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/conftest.py
--rw-r--r--   0        0        0     4503 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
--rw-r--r--   0        0        0     3215 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_config.py
--rw-r--r--   0        0        0     4974 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_email_notification.py
--rw-r--r--   0        0        0     3177 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_meta_mapper.py
--rw-r--r--   0        0        0     3959 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_pagination.py
--rw-r--r--   0        0        0     1146 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_s3_manager.py
--rw-r--r--   0        0        0     2718 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_security.py
--rw-r--r--   0        0        0     4512 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_storage.py
--rw-r--r--   0        0        0     2777 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_version.py
--rw-r--r--   0        0        0     1102 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/version.py
--rw-r--r--   0        0        0     2904 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/pyproject.toml
--rw-r--r--   0        0        0     2488 2023-04-14 17:46:54.497939 jobbergate-api-3.5.0a1/setup.py
--rw-r--r--   0        0        0     2657 2023-04-14 17:46:54.498371 jobbergate-api-3.5.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/LICENSE
+-rw-r--r--   0        0        0      738 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/README.rst
+-rw-r--r--   0        0        0      169 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0       41 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/__init__.py
+-rw-r--r--   0        0        0     5655 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/application_files.py
+-rw-r--r--   0        0        0      234 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/constants.py
+-rw-r--r--   0        0        0     9408 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/file_validation.py
+-rw-r--r--   0        0        0     1404 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/models.py
+-rw-r--r--   0        0        0    13548 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/routers.py
+-rw-r--r--   0        0        0     7239 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/schemas.py
+-rw-r--r--   0        0        0       40 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    12157 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/job_script_files.py
+-rw-r--r--   0        0        0     1185 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    11747 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     3890 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0       44 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0      529 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     1910 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    12331 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/properties_parser.py
+-rw-r--r--   0        0        0    18431 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0    14894 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0      554 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     3621 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2466 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     3268 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3433 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0       96 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/metadata.py
+-rw-r--r--   0        0        0     3470 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/pagination.py
+-rw-r--r--   0        0        0     2284 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/s3_manager.py
+-rw-r--r--   0        0        0     2166 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/security.py
+-rw-r--r--   0        0        0     5580 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/storage.py
+-rw-r--r--   0        0        0       40 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/__init__.py
+-rw-r--r--   0        0        0    10634 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_application_files.py
+-rw-r--r--   0        0        0     1967 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_file_validation.py
+-rw-r--r--   0        0        0    41708 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_routers.py
+-rw-r--r--   0        0        0     5180 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_schemas.py
+-rw-r--r--   0        0        0     2756 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/conftest.py
+-rw-r--r--   0        0        0       42 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     1376 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/conftest.py
+-rw-r--r--   0        0        0    11518 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
+-rw-r--r--   0        0        0    42583 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/test_routers.py
+-rw-r--r--   0        0        0       46 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0    23970 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
+-rw-r--r--   0        0        0    78149 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_submissions/test_routers.py
+-rw-r--r--   0        0        0      511 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/test_main.py
+-rw-r--r--   0        0        0     8900 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/conftest.py
+-rw-r--r--   0        0        0     4503 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
+-rw-r--r--   0        0        0     3215 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_config.py
+-rw-r--r--   0        0        0     4974 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_email_notification.py
+-rw-r--r--   0        0        0     3177 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_meta_mapper.py
+-rw-r--r--   0        0        0     3959 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_pagination.py
+-rw-r--r--   0        0        0     1146 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_s3_manager.py
+-rw-r--r--   0        0        0     2718 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_security.py
+-rw-r--r--   0        0        0     4512 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_storage.py
+-rw-r--r--   0        0        0     2777 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_version.py
+-rw-r--r--   0        0        0     1102 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/version.py
+-rw-r--r--   0        0        0     2904 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2488 2023-04-27 21:34:22.967130 jobbergate-api-3.5.0a2/setup.py
+-rw-r--r--   0        0        0     2657 2023-04-27 21:34:22.967521 jobbergate-api-3.5.0a2/PKG-INFO
```

### Comparing `jobbergate-api-3.5.0a1/LICENSE` & `jobbergate-api-3.5.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/README.rst` & `jobbergate-api-3.5.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/application_files.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/file_validation.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/models.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/routers.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/schemas.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/job_script_files.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/models.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/routers.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/models.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/properties_parser.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/properties_parser.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/apps/permissions.py` & `jobbergate-api-3.5.0a2/jobbergate_api/apps/permissions.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/config.py` & `jobbergate-api-3.5.0a2/jobbergate_api/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/email_notification.py` & `jobbergate-api-3.5.0a2/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/main.py` & `jobbergate-api-3.5.0a2/jobbergate_api/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/meta_mapper.py` & `jobbergate-api-3.5.0a2/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/pagination.py` & `jobbergate-api-3.5.0a2/jobbergate_api/pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/s3_manager.py` & `jobbergate-api-3.5.0a2/jobbergate_api/s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/security.py` & `jobbergate-api-3.5.0a2/jobbergate_api/security.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/storage.py` & `jobbergate-api-3.5.0a2/jobbergate_api/storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_application_files.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_file_validation.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_routers.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_schemas.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/conftest.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/conftest.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/test_routers.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/test_routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_submissions/test_routers.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_submissions/test_routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/conftest.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_config.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_email_notification.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_meta_mapper.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_pagination.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_s3_manager.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_security.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_storage.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_version.py` & `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/jobbergate_api/version.py` & `jobbergate-api-3.5.0a2/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a1/pyproject.toml` & `jobbergate-api-3.5.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "3.5.0-alpha.1"
+version = "3.5.0-alpha.2"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate-api-3.5.0a1/setup.py` & `jobbergate-api-3.5.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
  'yarl>=1.7.2,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['dev-tools = dev_tools:app']}
 
 setup_kwargs = {
     'name': 'jobbergate-api',
-    'version': '3.5.0a1',
+    'version': '3.5.0a2',
     'description': 'Jobbergate API',
     'long_description': '================\n Jobbergate API\n================\n\n\nThe Jobbergate API provides a RESTful interface over the Jobbergate data and is used\nby both the ``jobbergate-agent`` and the ``jobbergate-cli`` to view and manage the\nJobbergate resources.\n\nJobbergate API is a Python project implemented with\n`FastAPI <https://fastapi.tiangolo.com/>`_. Its dependencies and environment are\nmanaged by `Poetry <https://python-poetry.org/>`_.\n\nIt integrates with an OIDC server to provide identity and auth for its endpoints.\n\nSee also:\n\n* `jobbergate-cli <https://github.com/omnivector-solutions/jobbergate/jobbergate-cli>`_\n\nLicense\n-------\n* `MIT <LICENSE>`_\n\n\nCopyright\n---------\n* Copyright (c) 2020 OmniVector Solutions <info@omnivector.solutions>\n',
     'author': 'Omnivector Solutions',
     'author_email': 'info@omnivector.solutions',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/omnivector-solutions/jobbergate',
```

### Comparing `jobbergate-api-3.5.0a1/PKG-INFO` & `jobbergate-api-3.5.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 3.5.0a1
+Version: 3.5.0a2
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


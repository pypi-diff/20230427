# Comparing `tmp/astro_provider_databricks-0.1.2.tar.gz` & `tmp/astro_provider_databricks-0.1.3.tar.gz`

## Comparing `astro_provider_databricks-0.1.2.tar` & `astro_provider_databricks-0.1.3.tar`

### file list

```diff
@@ -1,72 +1,65 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/.deepsource.toml
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/CHANGELOG.rst
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/Tiltfile
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/codecov.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/mlc-config.json
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/noxfile.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/yamllint-config.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/.github/ci-test-connections.yaml
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/.github/scripts/verify_tag_and_version.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/.github/workflows/astro-deploy.yml
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/.github/workflows/mlc_config.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/dev/.dockerignore
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/dev/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/dev/Dockerfile
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/dev/docker-compose.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/dev/packages.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/dev/requirements.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/dev/.astro/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/dev/dags/.airflowignore
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/dev/dags/basic_notebooks.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/dev/dags/task_group_example.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/Makefile
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/conf.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/contributing.rst
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/make.bat
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/requirements.txt
--rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/_static/banner.png
--rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/_static/dbt_dag.png
--rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/_static/dbt_task_group.png
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/_static/logo-dark.png
--rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/_static/logo-light.png
--rw-r--r--   0        0        0    80206 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/_static/connections_doc/bigquery_airflow_connection.png
--rw-r--r--   0        0        0    82236 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/_static/connections_doc/databricks_airflow_connection.png
--rw-r--r--   0        0        0    72389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/_static/connections_doc/postgres_airflow_connection.png
--rw-r--r--   0        0        0    75178 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/_static/connections_doc/redshift_airflow_connection.png
--rw-r--r--   0        0        0   108877 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/_static/connections_doc/snowflake_airflow_connection.png
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/_static/css/custom.css
--rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/assets/images/dbutils-notebook-success.png
--rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/assets/images/repair-all-failed.png
--rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/docs/assets/images/repair-single-failed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/example_dags/.airflowignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/example_dags/__init__.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/example_dags/example_databricks_notebook.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/example_dags/example_databricks_workflow.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/astro_databricks/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/astro_databricks/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/astro_databricks/operators/__init__.py
--rw-r--r--   0        0        0    11715 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/astro_databricks/operators/notebook.py
--rw-r--r--   0        0        0    15983 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/astro_databricks/operators/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/astro_databricks/plugins/__init__.py
--rw-r--r--   0        0        0    17286 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/astro_databricks/plugins/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/tests/pytest.ini
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/tests/test_example_dags.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/tests/databricks/__init__.py
--rw-r--r--   0        0        0    14857 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/tests/databricks/test_notebook.py
--rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/tests/databricks/test_plugin.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/tests/databricks/test_workflow.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/LICENSE
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/README.md
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.deepsource.toml
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/CHANGELOG.rst
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/Tiltfile
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/codecov.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/mlc-config.json
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/noxfile.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/yamllint-config.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/ci-test-connections.yaml
+-rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/scripts/verify_tag_and_version.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/workflows/astro-deploy.yml
+-rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/workflows/mlc_config.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/.dockerignore
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/Dockerfile
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/docker-compose.yaml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/packages.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/requirements.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/.astro/config.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/Makefile
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/conf.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/contributing.rst
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/make.bat
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/requirements.txt
+-rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/banner.png
+-rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/dbt_dag.png
+-rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/dbt_task_group.png
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/logo-dark.png
+-rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/logo-light.png
+-rw-r--r--   0        0        0    80206 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/connections_doc/bigquery_airflow_connection.png
+-rw-r--r--   0        0        0    82236 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/connections_doc/databricks_airflow_connection.png
+-rw-r--r--   0        0        0    72389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/connections_doc/postgres_airflow_connection.png
+-rw-r--r--   0        0        0    75178 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/connections_doc/redshift_airflow_connection.png
+-rw-r--r--   0        0        0   108877 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/connections_doc/snowflake_airflow_connection.png
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/assets/images/dbutils-notebook-success.png
+-rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/assets/images/repair-all-failed.png
+-rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/assets/images/repair-single-failed.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/operators/__init__.py
+-rw-r--r--   0        0        0    12957 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/operators/notebook.py
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/operators/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/plugins/__init__.py
+-rw-r--r--   0        0        0    17286 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/plugins/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/pytest.ini
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/test_example_dags.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/databricks/__init__.py
+-rw-r--r--   0        0        0    14882 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/databricks/test_notebook.py
+-rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/databricks/test_plugin.py
+-rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/databricks/test_workflow.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/LICENSE
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/README.md
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/PKG-INFO
```

### Comparing `astro_provider_databricks-0.1.2/.pre-commit-config.yaml` & `astro_provider_databricks-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/CODE_OF_CONDUCT.md` & `astro_provider_databricks-0.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/Tiltfile` & `astro_provider_databricks-0.1.3/Tiltfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/noxfile.py` & `astro_provider_databricks-0.1.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/.github/scripts/verify_tag_and_version.py` & `astro_provider_databricks-0.1.3/.github/scripts/verify_tag_and_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 version_file = path_of_init_file.read_text()
 git_ref = os.getenv("GITHUB_REF", "")
 git_tag = git_ref.replace("refs/tags/", "")
 version = re.findall('__version__ = "(.*)"', version_file)[0]
 
 if git_tag is not None:
     if version != git_tag:
-        raise SystemExit(f"The version in {path_of_init_file} ({version}) does not match the Git Tag ({git_tag}).")
+        raise SystemExit(
+            f"The version in {path_of_init_file} ({version}) does not match the Git Tag ({git_tag})."
+        )
```

### Comparing `astro_provider_databricks-0.1.2/.github/workflows/astro-deploy.yml` & `astro_provider_databricks-0.1.3/.github/workflows/astro-deploy.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/.github/workflows/ci.yml` & `astro_provider_databricks-0.1.3/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -200,8 +200,7 @@
           coverage xml
       - name: Upload coverage
         uses: codecov/codecov-action@v2
         with:
           fail_ci_if_error: true
           token: ${{ secrets.CODECOV_TOKEN }}
           files: ./coverage.xml
-
```

### Comparing `astro_provider_databricks-0.1.2/.github/workflows/deploy.yml` & `astro_provider_databricks-0.1.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/.github/workflows/docs.yml` & `astro_provider_databricks-0.1.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/dev/Dockerfile` & `astro_provider_databricks-0.1.3/dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/dev/docker-compose.yaml` & `astro_provider_databricks-0.1.3/dev/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/Makefile` & `astro_provider_databricks-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/conf.py` & `astro_provider_databricks-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/contributing.rst` & `astro_provider_databricks-0.1.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/index.rst` & `astro_provider_databricks-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/make.bat` & `astro_provider_databricks-0.1.3/docs/make.bat`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=sphinx-build
-)
-set SOURCEDIR=.
-set BUILDDIR=_build
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.https://www.sphinx-doc.org/
-	exit /b 1
-)
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+    set SPHINXBUILD=sphinx-build
+)
+set SOURCEDIR=.
+set BUILDDIR=_build
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+    echo.
+    echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+    echo.installed, then set the SPHINXBUILD environment variable to point
+    echo.to the full path of the 'sphinx-build' executable. Alternatively you
+    echo.may add the Sphinx directory to PATH.
+    echo.
+    echo.If you don't have Sphinx installed, grab it from
+    echo.https://www.sphinx-doc.org/
+    exit /b 1
+)
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+
+:end
+popd
```

### Comparing `astro_provider_databricks-0.1.2/docs/_static/banner.png` & `astro_provider_databricks-0.1.3/docs/_static/banner.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/_static/dbt_dag.png` & `astro_provider_databricks-0.1.3/docs/_static/dbt_dag.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/_static/dbt_task_group.png` & `astro_provider_databricks-0.1.3/docs/_static/dbt_task_group.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/_static/logo-dark.png` & `astro_provider_databricks-0.1.3/docs/_static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/_static/logo-light.png` & `astro_provider_databricks-0.1.3/docs/_static/logo-light.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/_static/connections_doc/bigquery_airflow_connection.png` & `astro_provider_databricks-0.1.3/docs/_static/connections_doc/bigquery_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/_static/connections_doc/databricks_airflow_connection.png` & `astro_provider_databricks-0.1.3/docs/_static/connections_doc/databricks_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/_static/connections_doc/postgres_airflow_connection.png` & `astro_provider_databricks-0.1.3/docs/_static/connections_doc/postgres_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/_static/connections_doc/redshift_airflow_connection.png` & `astro_provider_databricks-0.1.3/docs/_static/connections_doc/redshift_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/_static/connections_doc/snowflake_airflow_connection.png` & `astro_provider_databricks-0.1.3/docs/_static/connections_doc/snowflake_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/assets/images/dbutils-notebook-success.png` & `astro_provider_databricks-0.1.3/docs/assets/images/dbutils-notebook-success.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/assets/images/repair-all-failed.png` & `astro_provider_databricks-0.1.3/docs/assets/images/repair-all-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/docs/assets/images/repair-single-failed.png` & `astro_provider_databricks-0.1.3/docs/assets/images/repair-single-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/astro_databricks/operators/notebook.py` & `astro_provider_databricks-0.1.3/astro_databricks/operators/notebook.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 from airflow.models import BaseOperator
 from airflow.providers.databricks.hooks.databricks import DatabricksHook
 from airflow.utils.context import Context
 from databricks_cli.runs.api import RunsApi
 from databricks_cli.sdk.api_client import ApiClient
 
 from astro_databricks.constants import JOBS_API_VERSION
-from astro_databricks.operators.workflow import DatabricksMetaData, DatabricksWorkflowTaskGroup
+from astro_databricks.operators.workflow import (
+    DatabricksMetaData,
+    DatabricksWorkflowTaskGroup,
+)
 from astro_databricks.plugins.plugin import (
     DatabricksJobRepairSingleFailedLink,
     DatabricksJobRunLink,
 )
 
 
 class DatabricksNotebookOperator(BaseOperator):
@@ -33,15 +36,15 @@
     .. code-block: python
 
         with dag:
             task_group = DatabricksWorkflowTaskGroup(
                 group_id="test_workflow",
                 databricks_conn_id="databricks_conn",
                 job_clusters=job_cluster_spec,
-                notebook_params=[],
+                notebook_params={},
             )
             with task_group:
                 notebook_1 = DatabricksNotebookOperator(
                     task_id="notebook_1",
                     databricks_conn_id="databricks_conn",
                     notebook_path="/Users/daniel@astronomer.io/Test workflow",
                     source="WORKSPACE",
@@ -70,15 +73,18 @@
         :param notebook_params: the parameters to pass to the notebook
     """
 
     operator_extra_links = (
         DatabricksJobRunLink(),
         DatabricksJobRepairSingleFailedLink(),
     )
-    template_fields = ("databricks_metadata",)
+    template_fields = (
+        "databricks_metadata",
+        "notebook_params",
+    )
 
     def __init__(
         self,
         notebook_path: str,
         source: str,
         databricks_conn_id: str,
         notebook_params: dict | None = None,
@@ -120,21 +126,41 @@
                 "source": self.source,
                 "base_parameters": self.notebook_params,
             },
             "libraries": self.notebook_packages,
         }
 
     def convert_to_databricks_workflow_task(
-        self, relevant_upstreams: list[BaseOperator]
+        self, relevant_upstreams: list[BaseOperator], context: Context | None = None
     ):
         """
         Convert the operator to a Databricks workflow task that can be a task in a workflow
         """
-        if self.databricks_task_group and (self.databricks_task_group, "notebook_packages"):
+        if self.databricks_task_group and hasattr(
+            self.databricks_task_group,
+            "notebook_packages",
+        ):
             self.notebook_packages.extend(self.databricks_task_group.notebook_packages)
+
+        if self.databricks_task_group and hasattr(
+            self.databricks_task_group,
+            "notebook_params",
+        ):
+            self.notebook_params = {
+                **self.notebook_params,
+                **self.databricks_task_group.notebook_params,
+            }
+        if context:
+            # The following exception currently only happens on Airflow 2.3, with the following error:
+            # airflow.exceptions.AirflowException: XComArg result from test_workflow.launch at example_databricks_workflow with key="return_value" is not found!
+            try:
+                self.render_template_fields(context)
+            except AirflowException:
+                self.log.exception("Unable to process template fields")
+
         base_task_json = self._get_task_base_json()
         result = {
             "task_key": self._get_databricks_task_id(self.task_id),
             "depends_on": [
                 {"task_key": self._get_databricks_task_id(t)}
                 for t in self.upstream_task_ids
                 if t in relevant_upstreams
@@ -149,15 +175,17 @@
         return self.dag_id + "__" + task_id.replace(".", "__")
 
     def monitor_databricks_job(self):
         """Monitor the Databricks job until it completes. Raises Airflow exception if the job fails."""
         api_client = self._get_api_client()
         runs_api = RunsApi(api_client)
         current_task = self._get_current_databricks_task(runs_api)
-        url = runs_api.get_run(self.databricks_run_id, version=JOBS_API_VERSION)['run_page_url']
+        url = runs_api.get_run(self.databricks_run_id, version=JOBS_API_VERSION)[
+            "run_page_url"
+        ]
         self.log.info(f"Check the job run in Databricks: {url}")
         self._wait_for_pending_task(current_task, runs_api)
         self._wait_for_running_task(current_task, runs_api)
         self._wait_for_terminating_task(current_task, runs_api)
         final_state = runs_api.get_run(
             current_task["run_id"], version=JOBS_API_VERSION
         )["state"]
@@ -242,15 +270,22 @@
         DatabricksWorkflowTaskGroup, it assumes the notebook is already launched
         and proceeds to monitor the running notebook.
 
         :param context:
         :return:
         """
         if self.databricks_task_group:
-            # if we are in a workflow, we assume there is a metadata from the launch task
+            # if we are in a workflow, we assume there is an upstream launch task
+            if not self.databricks_metadata:
+                launch_task_id = [
+                    task for task in self.upstream_task_ids if task.endswith(".launch")
+                ][0]
+                self.databricks_metadata = context["ti"].xcom_pull(
+                    task_ids=launch_task_id
+                )
             databricks_metadata = DatabricksMetaData(**self.databricks_metadata)
             self.databricks_run_id = databricks_metadata.databricks_run_id
             self.databricks_conn_id = databricks_metadata.databricks_conn_id
         else:
             self.launch_notebook_job()
 
         self.monitor_databricks_job()
@@ -260,15 +295,17 @@
         """
         Traverses up parent TaskGroups until the `is_databricks` flag is found.
         If found, returns the task group. Otherwise, returns None.
         """
         parent_tg = self.task_group
 
         while parent_tg:
-            if hasattr(parent_tg, "is_databricks") and getattr(parent_tg, "is_databricks"):
+            if hasattr(parent_tg, "is_databricks") and getattr(
+                parent_tg, "is_databricks"
+            ):
                 return parent_tg
 
             # here, we rely on the fact that Airflow sets the task_group property on tasks/task groups
             # if that ever changes, we will need to update this
             if hasattr(parent_tg, "task_group") and getattr(parent_tg, "task_group"):
                 parent_tg = parent_tg.task_group
             else:
```

### Comparing `astro_provider_databricks-0.1.2/astro_databricks/operators/workflow.py` & `astro_provider_databricks-0.1.3/astro_databricks/operators/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,24 +43,26 @@
     jobs = jobs_api.list_jobs().get("jobs", [])
     for job in jobs:
         if job.get("settings", {}).get("name") == job_name:
             return job
     return None
 
 
-def flatten_node(node: TaskGroup | BaseOperator, tasks: list[BaseOperator] = []) -> list[BaseOperator]:
+def flatten_node(
+    node: TaskGroup | BaseOperator, tasks: list[BaseOperator] = []
+) -> list[BaseOperator]:
     """
     Flattens a node (either a TaskGroup or Operator) to a list of nodes
     """
     if isinstance(node, BaseOperator):
         return [node]
 
     if isinstance(node, TaskGroup):
         new_tasks = []
-        for id, child in node.children.items():
+        for id_, child in node.children.items():
             new_tasks += flatten_node(child, tasks)
 
         return tasks + new_tasks
 
     return tasks
 
 
@@ -72,41 +74,47 @@
     :param job_clusters: A list of job clusters to use in the workflow
     :param existing_clusters: A list of existing clusters to use in the workflow
     :param max_concurrent_runs: The maximum number of concurrent runs
     :param tasks_to_convert: A list of tasks to convert to a workflow. This list can also
     be populated after initialization by calling add_task.
     :param extra_job_params: A dictionary containing properties which will override the
     default Databricks Workflow Job definitions.
+    :param notebook_params:  A dictionary of notebook parameters to pass to the workflow.These parameters will be passed to
+    all notebook tasks in the workflow.
     """
 
+    template_fields = ("notebook_params",)
+
     operator_extra_links = (DatabricksJobRunLink(), DatabricksJobRepairAllFailedLink())
     databricks_conn_id: str
     databricks_run_id: str
     databricks_job_id: str
 
     def __init__(
         self,
         task_id,
         databricks_conn_id,
         job_clusters: list[dict[str, object]] = None,
         existing_clusters: list[str] = None,
         max_concurrent_runs: int = 1,
         tasks_to_convert: list[BaseOperator] = None,
         extra_job_params: dict[str, Any] = None,
+        notebook_params: dict | None = None,
         **kwargs,
     ):
         self.existing_clusters = existing_clusters or []
         self.job_clusters = job_clusters or []
         self.job_cluster_dict = {j["job_cluster_key"]: j for j in self.job_clusters}
         self.tasks_to_convert = tasks_to_convert or []
         self.relevant_upstreams = [task_id]
         self.databricks_conn_id = databricks_conn_id
         self.databricks_run_id = None
         self.max_concurrent_runs = max_concurrent_runs
         self.extra_job_params = extra_job_params or {}
+        self.notebook_params = notebook_params or {}
         super().__init__(task_id=task_id, **kwargs)
 
         # For Airflow versions <2.3, the `task_group` attribute is unassociated, and hence we need to add that.
         if not hasattr(self, "task_group"):
             from airflow.utils.task_group import TaskGroupContext
 
             self.task_group = TaskGroupContext.get_current_task_group(self.dag)
@@ -116,22 +124,22 @@
         Add a task to the list of tasks to convert to a workflow.
 
         :param task:
         :return:
         """
         self.tasks_to_convert.append(task)
 
-    def create_workflow_json(self) -> dict[str, object]:
+    def create_workflow_json(self, context: Context | None = None) -> dict[str, object]:
         """Create a workflow json that can be submitted to databricks.
 
         :return: A workflow json
         """
         task_json = [
             task.convert_to_databricks_workflow_task(
-                relevant_upstreams=self.relevant_upstreams
+                relevant_upstreams=self.relevant_upstreams, context=context
             )
             for task in self.tasks_to_convert
         ]
         default_json = {
             "name": self.databricks_job_name,
             "email_notifications": {"no_alert_for_skipped_runs": False},
             "timeout_seconds": 0,
@@ -153,48 +161,56 @@
         api_client = ApiClient(
             token=databricks_conn.password, host=databricks_conn.host
         )
         jobs_api = JobsApi(api_client)
         job = _get_job_by_name(self.databricks_job_name, jobs_api)
 
         job_id = job["job_id"] if job else None
-        current_job_spec = self.create_workflow_json()
+        current_job_spec = self.create_workflow_json(context)
         if not isinstance(self.task_group, DatabricksWorkflowTaskGroup):
-            raise AirflowException(
-                "Task group must be a DatabricksWorkflowTaskGroup")
+            raise AirflowException("Task group must be a DatabricksWorkflowTaskGroup")
         if job_id:
             self.log.info(
                 "Updating existing job with spec %s",
                 json.dumps(current_job_spec, indent=4),
             )
 
             jobs_api.reset_job(
                 json={"job_id": job_id, "new_settings": current_job_spec}
             )
         else:
             self.log.info(
-                "Creating new job with spec %s", json.dumps(
-                    current_job_spec, indent=4)
+                "Creating new job with spec %s", json.dumps(current_job_spec, indent=4)
             )
             job_id = jobs_api.create_job(json=current_job_spec)["job_id"]
 
         run_id = jobs_api.run_now(
             job_id=job_id,
             jar_params=self.task_group.jar_params,
-            notebook_params=self.task_group.notebook_params,
+            notebook_params=self.notebook_params,
             python_params=self.task_group.python_params,
             spark_submit_params=self.task_group.spark_submit_params,
         )["run_id"]
+        self.databricks_run_id = run_id
+
         runs_api = RunsApi(api_client)
         url = runs_api.get_run(run_id).get("run_page_url")
         self.log.info(f"Check the job run in Databricks: {url}")
-        while runs_api.get_run(run_id)["state"]["life_cycle_state"] == "PENDING":
-            print("job pending")
+        state = runs_api.get_run(run_id)["state"]["life_cycle_state"]
+        self.log.info(f"Job state: {state}")
+
+        if state not in ("PENDING", "BLOCKED", "RUNNING"):
+            raise AirflowException(
+                f"Could not start the workflow job, it had state {state}"
+            )
+
+        while state in ("PENDING", "BLOCKED"):
+            self.log.info(f"Job {state}")
             time.sleep(5)
-        self.databricks_run_id = run_id
+            state = runs_api.get_run(run_id)["state"]["life_cycle_state"]
 
         return {
             "databricks_conn_id": self.databricks_conn_id,
             "databricks_job_id": job_id,
             "databricks_run_id": run_id,
         }
 
@@ -236,15 +252,15 @@
         ]
 
     with dag:
         task_group = DatabricksWorkflowTaskGroup(
             group_id="test_workflow",
             databricks_conn_id="databricks_conn",
             job_clusters=job_cluster_spec,
-            notebook_params=[],
+            notebook_params={},
             notebook_packages=[
                 {
                     "pypi": {
                         "package": "simplejson"
                     }
                 },
             ]
@@ -285,15 +301,15 @@
     ``DatabricksWorkflowTaskGroup`` and not in the ``DatabricksNotebookOperator`` whenever possible.
         This is because tasks in the
     ``DatabricksWorkflowTaskGroup`` are passed in at the job trigger time and do not modify the job definition
 
     :param group_id: The name of the task group
     :param databricks_conn_id: The name of the databricks connection to use
     :param job_clusters: A list of job clusters to use for this workflow.
-    :param notebook_params: A list of notebook parameters to pass to the workflow.These parameters will be passed to
+    :param notebook_params: A dictionary of notebook parameters to pass to the workflow. These parameters will be passed to
     all notebook tasks in the workflow.
     :param notebook_packages: A list of dictionary of Python packages to be installed. Packages defined at the
     workflow task group level are installed for each of the notebook tasks under it. And packages defined at the
     notebook task level are installed specific for the notebook task.
     :param jar_params: A list of jar parameters to pass to the workflow. These parameters will be passed to all jar
         tasks
     in the workflow.
@@ -317,48 +333,48 @@
 
     def __init__(
         self,
         databricks_conn_id,
         existing_clusters=None,
         job_clusters=None,
         jar_params: dict = None,
-        notebook_params: list = None,
+        notebook_params: dict | None = None,
         notebook_packages: list[dict[str, Any]] = None,
         python_params: list = None,
         spark_submit_params: list = None,
         max_concurrent_runs: int = 1,
         extra_job_params: dict[str, Any] = None,
         **kwargs,
     ):
         """
         Create a new DatabricksWorkflowTaskGroup.
 
         :param group_id: The name of the task group
         :param databricks_conn_id: The name of the databricks connection to use
         :param job_clusters: A list of job clusters to use for this workflow.
-        :param notebook_params: A list of notebook parameters to pass to the workflow.These parameters will be passed to
+        :param notebook_params: A dictionary of notebook parameters to pass to the workflow.These parameters will be passed to
         all notebook tasks in the workflow.
         :param notebook_packages: A list of dictionary of Python packages to be installed. These packages will be passed
          to all notebook tasks in the workflow.
         :param jar_params: A list of jar parameters to pass to the workflow.
          These parameters will be passed to all jar tasks
         in the workflow.
-        :param python_params: A list of python parameters to pass to the workflow.
+        :param python_params: A dictionary of python parameters to pass to the workflow.
          These parameters will be passed to all python tasks
         in the workflow.
         :param spark_submit_params: A list of spark submit parameters to pass to the workflow.
          These parameters will be passed to all spark submit tasks
         :param max_concurrent_runs: The maximum number of concurrent runs for this workflow.
         :param extra_job_params: A dictionary containing properties which will override the default Databricks
         Workflow Job definitions.
         """
         self.databricks_conn_id = databricks_conn_id
         self.existing_clusters = existing_clusters or []
         self.job_clusters = job_clusters or []
-        self.notebook_params = notebook_params or []
+        self.notebook_params = notebook_params or {}
         self.notebook_packages = notebook_packages or []
         self.python_params = python_params or []
         self.spark_submit_params = spark_submit_params or []
         self.jar_params = jar_params or []
         self.max_concurrent_runs = max_concurrent_runs
         self.extra_job_params = extra_job_params or {}
         super().__init__(**kwargs)
@@ -378,26 +394,27 @@
             dag=self.dag,
             task_group=self,
             task_id="launch",
             databricks_conn_id=self.databricks_conn_id,
             job_clusters=self.job_clusters,
             existing_clusters=self.existing_clusters,
             extra_job_params=self.extra_job_params,
+            notebook_params=self.notebook_params,
         )
 
         for task in tasks:
             if not (
                 hasattr(task, "convert_to_databricks_workflow_task")
                 and callable(task.convert_to_databricks_workflow_task)
             ):
                 raise AirflowException(
                     f"Task {task.task_id} does not support conversion to databricks workflow task."
                 )
 
+            task.databricks_metadata = create_databricks_workflow_task.output
             create_databricks_workflow_task.relevant_upstreams.append(task.task_id)
             create_databricks_workflow_task.add_task(task)
-            task.databricks_metadata = create_databricks_workflow_task.output
 
         for root_task in roots:
             root_task.set_upstream(create_databricks_workflow_task)
 
         super().__exit__(_type, _value, _tb)
```

### Comparing `astro_provider_databricks-0.1.2/astro_databricks/plugins/plugin.py` & `astro_provider_databricks-0.1.3/astro_databricks/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/tests/conftest.py` & `astro_provider_databricks-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/tests/test_example_dags.py` & `astro_provider_databricks-0.1.3/tests/test_example_dags.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/tests/utils.py` & `astro_provider_databricks-0.1.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/tests/databricks/test_notebook.py` & `astro_provider_databricks-0.1.3/tests/databricks/test_notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,15 +353,15 @@
 )
 def test_monitor_databricks_job_success(
     mock_get_databricks_task_id,
     mock_get_api_client,
     mock_runs_api,
     mock_databricks_hook,
     databricks_notebook_operator,
-    caplog
+    caplog,
 ):
     mock_get_databricks_task_id.return_value = "1"
     # Define the expected response
     response = {
         "run_page_url": "https://databricks-instance-xyz.cloud.databricks.com/#job/1234/run/1",
         "state": {
             "life_cycle_state": "TERMINATED",
@@ -378,15 +378,18 @@
     mock_runs_api.return_value.get_run.return_value = response
 
     databricks_notebook_operator.databricks_run_id = "1"
     databricks_notebook_operator.monitor_databricks_job()
     mock_runs_api.return_value.get_run.assert_called_with(
         databricks_notebook_operator.databricks_run_id, version="2.1"
     )
-    assert 'Check the job run in Databricks: https://databricks-instance-xyz.cloud.databricks.com/#job/1234/run/1' in caplog.messages
+    assert (
+        "Check the job run in Databricks: https://databricks-instance-xyz.cloud.databricks.com/#job/1234/run/1"
+        in caplog.messages
+    )
 
 
 @mock.patch("astro_databricks.operators.notebook.DatabricksHook")
 @mock.patch("astro_databricks.operators.notebook.RunsApi")
 @mock.patch(
     "astro_databricks.operators.notebook.DatabricksNotebookOperator._get_api_client"
 )
```

### Comparing `astro_provider_databricks-0.1.2/tests/databricks/test_plugin.py` & `astro_provider_databricks-0.1.3/tests/databricks/test_plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/tests/databricks/test_workflow.py` & `astro_provider_databricks-0.1.3/tests/databricks/test_workflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+from __future__ import annotations
+
+import logging
 from unittest import mock
 
+import pytest
+from airflow.exceptions import AirflowException
 from astro_databricks.operators.notebook import DatabricksNotebookOperator
 from astro_databricks.operators.workflow import DatabricksWorkflowTaskGroup
 
 expected_workflow_json = {
     "name": "unit_test_dag.test_workflow",
     "email_notifications": {"no_alert_for_skipped_runs": False},
     "format": "MULTI_TASK",
@@ -15,52 +20,56 @@
             "email_notifications": {},
             "job_cluster_key": "foo",
             "libraries": [
                 {"nb_index": {"package": "nb_package"}},
                 {"tg_index": {"package": "tg_package"}},
             ],
             "notebook_task": {
-                "base_parameters": {},
+                "base_parameters": {"notebook_path": "/foo/bar"},
                 "notebook_path": "/foo/bar",
                 "source": "WORKSPACE",
             },
             "task_key": "unit_test_dag__test_workflow__notebook_1",
             "timeout_seconds": 0,
         },
         {
             "depends_on": [{"task_key": "unit_test_dag__test_workflow__notebook_1"}],
             "email_notifications": {},
             "job_cluster_key": "foo",
             "libraries": [{"tg_index": {"package": "tg_package"}}],
             "notebook_task": {
-                "base_parameters": {"foo": "bar"},
+                "base_parameters": {"foo": "bar", "notebook_path": "/foo/bar"},
                 "notebook_path": "/foo/bar",
                 "source": "WORKSPACE",
             },
             "task_key": "unit_test_dag__test_workflow__notebook_2",
             "timeout_seconds": 0,
         },
     ],
     "timeout_seconds": 0,
 }
 
 
 @mock.patch("astro_databricks.operators.workflow.DatabricksHook")
 @mock.patch("astro_databricks.operators.workflow.ApiClient")
 @mock.patch("astro_databricks.operators.workflow.JobsApi")
-def test_create_workflow_from_notebooks_with_create(
-    mock_jobs_api, mock_api, mock_hook, dag
+@mock.patch(
+    "astro_databricks.operators.workflow.RunsApi.get_run",
+    return_value={"state": {"life_cycle_state": "SKIPPED"}},
+)
+def test_create_workflow_from_notebooks_raises_exception_due_to_job_being_skipped(
+    mock_run_api, mock_jobs_api, mock_api, mock_hook, dag
 ):
     mock_jobs_api.return_value.create_job.return_value = {"job_id": 1}
     with dag:
         task_group = DatabricksWorkflowTaskGroup(
             group_id="test_workflow",
             databricks_conn_id="foo",
             job_clusters=[{"job_cluster_key": "foo"}],
-            notebook_params=[{"notebook_path": "/foo/bar"}],
+            notebook_params={"notebook_path": "/foo/bar"},
             notebook_packages=[{"tg_index": {"package": "tg_package"}}],
         )
         with task_group:
             notebook_1 = DatabricksNotebookOperator(
                 task_id="notebook_1",
                 databricks_conn_id="foo",
                 notebook_path="/foo/bar",
@@ -77,41 +86,38 @@
                 notebook_params={
                     "foo": "bar",
                 },
             )
             notebook_1 >> notebook_2
 
     assert len(task_group.children) == 3
-    task_group.children["test_workflow.launch"].execute(context={})
-    mock_jobs_api.return_value.create_job.assert_called_once_with(
-        json=expected_workflow_json,
-    )
-    mock_jobs_api.return_value.run_now.assert_called_once_with(
-        job_id=1,
-        jar_params=[],
-        notebook_params=[{"notebook_path": "/foo/bar"}],
-        python_params=[],
-        spark_submit_params=[],
+    with pytest.raises(AirflowException) as exc_info:
+        task_group.children["test_workflow.launch"].execute(context={})
+    assert (
+        str(exc_info.value) == "Could not start the workflow job, it had state SKIPPED"
     )
 
 
 @mock.patch("astro_databricks.operators.workflow.DatabricksHook")
 @mock.patch("astro_databricks.operators.workflow.ApiClient")
 @mock.patch("astro_databricks.operators.workflow.JobsApi")
-@mock.patch("astro_databricks.operators.workflow._get_job_by_name")
-def test_create_workflow_from_notebooks_existing_job(
-    mock_get_jobs, mock_jobs_api, mock_api, mock_hook, dag
+@mock.patch(
+    "astro_databricks.operators.workflow.RunsApi.get_run",
+    return_value={"state": {"life_cycle_state": "RUNNING"}},
+)
+def test_create_workflow_from_notebooks_with_create(
+    mock_run_api, mock_jobs_api, mock_api, mock_hook, dag
 ):
-    mock_get_jobs.return_value = {"job_id": 1}
+    mock_jobs_api.return_value.create_job.return_value = {"job_id": 1}
     with dag:
         task_group = DatabricksWorkflowTaskGroup(
             group_id="test_workflow",
             databricks_conn_id="foo",
             job_clusters=[{"job_cluster_key": "foo"}],
-            notebook_params=[{"notebook_path": "/foo/bar"}],
+            notebook_params={"notebook_path": "/foo/bar"},
             notebook_packages=[{"tg_index": {"package": "tg_package"}}],
         )
         with task_group:
             notebook_1 = DatabricksNotebookOperator(
                 task_id="notebook_1",
                 databricks_conn_id="foo",
                 notebook_path="/foo/bar",
@@ -129,32 +135,100 @@
                     "foo": "bar",
                 },
             )
             notebook_1 >> notebook_2
 
     assert len(task_group.children) == 3
     task_group.children["test_workflow.launch"].execute(context={})
-    mock_jobs_api.return_value.reset_job.assert_called_once_with(
-        json={"job_id": 1, "new_settings": expected_workflow_json},
+    mock_jobs_api.return_value.create_job.assert_called_once_with(
+        json=expected_workflow_json,
     )
     mock_jobs_api.return_value.run_now.assert_called_once_with(
         job_id=1,
         jar_params=[],
-        notebook_params=[{"notebook_path": "/foo/bar"}],
+        notebook_params={"notebook_path": "/foo/bar"},
         python_params=[],
         spark_submit_params=[],
     )
 
 
 @mock.patch("astro_databricks.operators.workflow.DatabricksHook")
 @mock.patch("astro_databricks.operators.workflow.ApiClient")
+@mock.patch("astro_databricks.operators.workflow._get_job_by_name")
+@mock.patch(
+    "astro_databricks.operators.workflow.RunsApi.get_run",
+    side_effect=[
+        {"state": {"life_cycle_state": "BLOCKED"}},
+        {"state": {"life_cycle_state": "BLOCKED"}},
+        {"state": {"life_cycle_state": "RUNNING"}},
+    ],
+)
+@mock.patch("astro_databricks.operators.workflow.JobsApi.run_now")
+@mock.patch("astro_databricks.operators.workflow.JobsApi.create_job")
+def test_create_workflow_from_notebooks_job_templates_notebook_jobs(
+    mock_create_job,
+    mock_run_now,
+    mock_get_run,
+    mock_get_jobs,
+    mock_api,
+    mock_hook,
+    dag,
+    caplog,
+):
+    mock_get_jobs.return_value = {"job_id": None}
+    caplog.set_level(logging.INFO)
+    with dag:
+        task_group = DatabricksWorkflowTaskGroup(
+            group_id="test_workflow",
+            databricks_conn_id="foo",
+            job_clusters=[{"job_cluster_key": "foo"}],
+            notebook_params={"notebook_path": "/foo/bar", "ts": "{{ ts }}"},
+            notebook_packages=[{"tg_index": {"package": "tg_package"}}],
+        )
+        with task_group:
+            notebook_1 = DatabricksNotebookOperator(
+                task_id="notebook_1",
+                databricks_conn_id="foo",
+                notebook_path="/foo/bar",
+                notebook_packages=[{"nb_index": {"package": "nb_package"}}],
+                notebook_params={"ds": "{{ ds }}"},
+                source="WORKSPACE",
+                job_cluster_key="foo",
+            )
+
+            notebook_1
+
+    assert len(task_group.children) == 2
+    context = {
+        "ds": "yyyy-mm-dd",
+        "ts": "hh:mm",
+        "ti": mock.MagicMock(),
+        "expanded_ti_count": 0,
+    }
+    task_group.children["test_workflow.launch"].execute(context=context)
+    assert mock_get_run.call_count == 3
+    assert "Job state: BLOCKED" in caplog.messages
+
+    notebook_job_parameters = mock_create_job.call_args.kwargs["json"]["tasks"][0][
+        "notebook_task"
+    ]["base_parameters"]
+    assert notebook_job_parameters["ds"] == "yyyy-mm-dd"
+    assert notebook_job_parameters["ts"] == "hh:mm"
+
+
+@mock.patch("astro_databricks.operators.workflow.DatabricksHook")
+@mock.patch("astro_databricks.operators.workflow.ApiClient")
 @mock.patch("astro_databricks.operators.workflow.JobsApi")
 @mock.patch("astro_databricks.operators.workflow._get_job_by_name")
+@mock.patch(
+    "astro_databricks.operators.workflow.RunsApi.get_run",
+    return_value={"state": {"life_cycle_state": "RUNNING"}},
+)
 def test_create_workflow_with_arbitrary_extra_job_params(
-    mock_get_jobs, mock_jobs_api, mock_api, mock_hook, dag
+    mock_run_api, mock_get_jobs, mock_jobs_api, mock_api, mock_hook, dag
 ):
     mock_get_jobs.return_value = {"job_id": 862519602273592}
 
     extra_job_params = {
         "timeout_seconds": 10,  # default: 0
         "webhook_notifications": {
             "on_failure": [{"id": "b0aea8ab-ea8c-4a45-a2e9-9a26753fd702"}],
@@ -170,15 +244,15 @@
         },
     }
     with dag:
         task_group = DatabricksWorkflowTaskGroup(
             group_id="test_workflow",
             databricks_conn_id="foo",
             job_clusters=[{"job_cluster_key": "foo"}],
-            notebook_params=[{"notebook_path": "/foo/bar"}],
+            notebook_params={"notebook_path": "/foo/bar"},
             extra_job_params=extra_job_params,
         )
         with task_group:
             notebook_with_extra = DatabricksNotebookOperator(
                 task_id="notebook_with_extra",
                 databricks_conn_id="foo",
                 notebook_path="/foo/bar",
```

### Comparing `astro_provider_databricks-0.1.2/.gitignore` & `astro_provider_databricks-0.1.3/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -139,7 +139,17 @@
 .DS_Store
 
 # dbt
 logs/
 
 # Airflow connections file
 test-connections.yaml
+
+# Airflow standalone
+airflow.cfg
+airflow.db
+dags
+standalone_admin_password.txt
+webserver_config.py
+
+# VIM
+*.sw[a-z]
```

### Comparing `astro_provider_databricks-0.1.2/LICENSE` & `astro_provider_databricks-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/README.md` & `astro_provider_databricks-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.2/pyproject.toml` & `astro_provider_databricks-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "astro-provider-databricks"
-version = "0.1.2"
+dynamic = ["version"]
 description = "Affordable Databricks Workflows in Apache Airflow"
 readme = "README.md"
 license = "Apache-2.0"
 requires-python = ">=3.7"
 packages = [{include = "astro_databricks", from = "src"}]
 
 authors = [
```

### Comparing `astro_provider_databricks-0.1.2/PKG-INFO` & `astro_provider_databricks-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-provider-databricks
-Version: 0.1.2
+Version: 0.1.3
 Summary: Affordable Databricks Workflows in Apache Airflow
 Project-URL: Homepage, https://github.com/astronomer/astro-provider-databricks/
 Project-URL: Documentation, https://github.com/astronomer/astro-provider-databricks/
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags
```


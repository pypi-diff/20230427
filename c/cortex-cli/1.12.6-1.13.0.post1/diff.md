# Comparing `tmp/cortex_cli-1.12.6.tar.gz` & `tmp/cortex_cli-1.13.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_cli-1.12.6.tar", last modified: Fri Apr 21 19:48:48 2023, max compression
+gzip compressed data, was "cortex_cli-1.13.0.post1.tar", last modified: Thu Apr 27 21:05:55 2023, max compression
```

## Comparing `cortex_cli-1.12.6.tar` & `cortex_cli-1.13.0.post1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5185 2023-04-06 19:56:17.000000 cortex_cli-1.12.6/README.md
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-04-20 17:50:53.000000 cortex_cli-1.12.6/cortex_cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.12.6/cortex_cli/cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/cli/api/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/cli/api/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3990 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/cli/api/github_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/cli/api/http_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.12.6/cortex_cli/cli/cli_api_base.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.12.6/cortex_cli/cli/cli_api_base_config.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/cli/clients.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      880 2023-04-07 17:56:26.000000 cortex_cli-1.12.6/cortex_cli/cli/configure.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.12.6/cortex_cli/cli/cortex_cli.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.12.6/cortex_cli/cli/generic_get.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/cli/inferences.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24183 2023-04-21 19:48:42.000000 cortex_cli-1.12.6/cortex_cli/cli/models.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.12.6/cortex_cli/cli/pipelines.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/core/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/core/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/core/cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/core/drift_checks.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/core/ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/core/mlflow/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/core/mlflow/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/core/mlflow/mlflow_cortex.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/core/models/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/core/models/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-04-20 17:50:53.000000 cortex_cli-1.12.6/cortex_cli/core/models/cortex_model.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-04-21 19:32:17.000000 cortex_cli-1.12.6/cortex_cli/core/secrets_manager.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-20 19:24:15.000000 cortex_cli-1.12.6/cortex_cli/model_templates/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-04-20 19:25:56.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.537815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-04-20 19:27:56.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-04-20 17:50:53.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/tests/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/tests/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/tests/test_cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/tests/test_ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli.egg-info/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3123 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/requires.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.12.6/pyproject.toml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/setup.cfg
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1076 2023-04-20 19:25:09.000000 cortex_cli-1.12.6/setup.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5185 2023-04-06 19:56:17.000000 cortex_cli-1.13.0.post1/README.md
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       25 2023-04-26 17:25:59.000000 cortex_cli-1.13.0.post1/cortex_cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/cli/api/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/api/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-04-25 18:51:50.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/api/github_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/api/http_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/cli_api_base.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/cli_api_base_config.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/clients.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2001 2023-04-26 16:12:30.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/configure.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/cortex_cli.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/generic_get.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/inferences.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24439 2023-04-26 15:26:09.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/models.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/pipelines.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/core/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/core/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-17 18:14:34.000000 cortex_cli-1.13.0.post1/cortex_cli/core/cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/core/drift_checks.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-17 18:14:34.000000 cortex_cli-1.13.0.post1/cortex_cli/core/ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/core/mlflow/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/core/mlflow/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/core/mlflow/mlflow_cortex.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/core/models/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/core/models/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-04-20 17:50:53.000000 cortex_cli-1.13.0.post1/cortex_cli/core/models/cortex_model.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/core/secrets_manager.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/tests/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/tests/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/tests/test_cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/tests/test_ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli.egg-info/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3123 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.13.0.post1/pyproject.toml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/setup.cfg
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1076 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/setup.py
```

### Comparing `cortex_cli-1.12.6/README.md` & `cortex_cli-1.13.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/cli/api/github_api.py` & `cortex_cli-1.13.0.post1/cortex_cli/cli/api/github_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -158,8 +158,8 @@
             '-C',
             self._path,
             'show-ref',
             '--head',
             '--hash',
             'head'
         )
-        return hash.replace('\n', '')
+        return hash.replace('\n', '')
```

### Comparing `cortex_cli-1.12.6/cortex_cli/cli/api/http_api.py` & `cortex_cli-1.13.0.post1/cortex_cli/cli/api/http_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/cli/cli_api_base.py` & `cortex_cli-1.13.0.post1/cortex_cli/cli/cli_api_base.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/cli/cli_api_base_config.py` & `cortex_cli-1.13.0.post1/cortex_cli/cli/cli_api_base_config.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/cli/cortex_cli.py` & `cortex_cli-1.13.0.post1/cortex_cli/cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/cli/generic_get.py` & `cortex_cli-1.13.0.post1/cortex_cli/cli/generic_get.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/cli/inferences.py` & `cortex_cli-1.13.0.post1/cortex_cli/cli/inferences.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/cli/models.py` & `cortex_cli-1.13.0.post1/cortex_cli/cli/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,16 @@
     def _register_model(self):
         if self._register:
             response = requests.post(
                 url=self._endpoint,
                 headers=self._headers,
                 json={
                     'name': self._name,
-                    'repo': self._repo
+                    'repo': self._repo,
+                    'githubEnabled': True if self._token else False
                 }
             )
 
             self._handle_api_response(
                 response, f'Registered the model repository {response.json()["_id"]}')
 
 
@@ -218,15 +219,16 @@
 
     def _register_model(self):
         return self._handle_api_response(requests.post(
             url=self._endpoint,
             headers=self._headers,
             json={
                 'name': self._name,
-                'repo': self._repo
+                'repo': self._repo,
+                'githubEnabled': True if gh.Repo().hash else False
             }
         ))
 
 
 @ModelsCli.subcommand('run')
 class RunModelPipeline(CliApiBase):
     _path = plumbum.cli.SwitchAttr(
@@ -325,15 +327,15 @@
             self._model_json = self._get_model()
             # Step 1 - Get live model data
             if self._tracking:
                 self._mlflow_client = self._setup_mlflow()
                 self._setup_pipeline()
 
             # Step 2 - Load the Model Class
-            self.model = self._instantiate_model(self._config)
+            self.model = self._instantiate_model()
 
             # Step 3 - Initialize the pipeline steps
             self._initialize_steps()
 
             # Step 4 - Run the pipeline
             if self._tracking:
                 self._pipeline_json = self._run_pipeline()
@@ -514,16 +516,15 @@
     def _create_pipeline(self, model_id, git_branch, git_hash):
         response = requests.post(
             url=f'{self._api_url}/pipelines',
             headers=self._headers,
             json={
                 'modelId':   model_id,
                 'gitBranch': git_branch,
-                'gitHash':   git_hash,
-                'local':     True
+                'gitHash':   git_hash
             }
         ).json()
         
         return response
 
 
     def _run_pipeline(self):
@@ -579,26 +580,29 @@
             if self._tracking:
                 self._complete_step(step, 'Failed', str(e), '')
             self._error_message = f'{step["name"]} completed with an error.\n{traceback.format_exc()}'
             raise Exception
 
 
     def _setup_pipeline(self):
+        pipeline_response = None
+
         # Get the local branch
         git_branch = gh.Repo().branch
         git_hash = gh.Repo().hash
 
-        if git_hash is None or git_hash == '':
-            self._fail('Could not get git commit hash. Please initialize the git repository and commit your code before running the pipeline.')
-
-        # Look for an existing 'Pending' pipeline for this branch
-        pipeline_response = self._get_pipeline(
-            git_branch,
-            self._model_id
-        )
+        if (self._model_json['githubEnabled']):
+            if git_hash is None or git_hash == '':
+                self._fail('Could not get git commit hash. Please initialize the git repository and commit your code before running the pipeline.')
+
+            # Look for an existing 'Pending' pipeline for this branch
+            pipeline_response = self._get_pipeline(
+                git_branch,
+                self._model_id
+            )
 
         if pipeline_response:
             self._pipeline_json = self._handle_api_response(pipeline_response)
             return
 
         # If not found, create the locally sourced pipeline
         self._pipeline_json = self._create_pipeline(
@@ -609,30 +613,30 @@
 
         self._pass(f'Pipeline {self._pipeline_json["currentStage"]} with id: {self._pipeline_id}')
 
 # -------------------------------------------------------------------------------
 
     def _get_model(self):
         query = {
-            'repo': gh.Repo().repo
+            'repo': self._config['model_repo']
         }
 
         response = requests.get(
             url=self._endpoint,
             params=query,
             headers=self._headers
         )
 
         if response.status_code != 200 or 'documents' not in response.json() or len(response.json()['documents']) != 1:
             raise Exception('Error! This model could not be found')
         
         model = response.json()['documents']
 
         self._pass(
-            f'Found the model {gh.Repo().repo}')
+            f'Found the model {self._config["model_repo"]}')
 
         return model[0]
 
 
     def _complete_callback(self, status, error_message=None):
         body = {
             'modelId':      self._model_id,
@@ -718,25 +722,25 @@
                     upload_urls[i],
                     data=f
                 )
         
         return f'Uploaded the pipeline artifacts to Cortex'
 
 
-    def _instantiate_model(self, config):
+    def _instantiate_model(self):
         # LOAD DEPENDENCY MODULES (except model)
         for path, module in self._modules.items():
             self._load_module(path, module)
 
         # LOAD MODEL MODULE
         model_module = self._load_module(
-            '{}/{}.py'.format(config['module_path'], config['model_module']),
-            config['model_module']
+            '{}/{}.py'.format(self._config['module_path'], self._config['model_module']),
+            self._config['model_module']
         )
 
-        model_params = dict(ChainMap(*config['params'])) if config['params'] else {}
-        return getattr(model_module, config['model_class'])(model_params, self._model_id, self._api_url, self._headers)
+        model_params = dict(ChainMap(*self._config['params'])) if self._config['params'] else {}
+        return getattr(model_module, self._config['model_class'])(model_params, self._model_id, self._api_url, self._headers)
 
 
     def _setup_mlflow(self):
         # Create a client to make API calls to the tracking server
         return mlflow.tracking.MlflowClient()
```

### Comparing `cortex_cli-1.12.6/cortex_cli/cli/pipelines.py` & `cortex_cli-1.13.0.post1/cortex_cli/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/core/cortex_data.py` & `cortex_cli-1.13.0.post1/cortex_cli/core/cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/core/drift_checks.py` & `cortex_cli-1.13.0.post1/cortex_cli/core/drift_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/core/ethics_checks.py` & `cortex_cli-1.13.0.post1/cortex_cli/core/ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/core/mlflow/mlflow_cortex.py` & `cortex_cli-1.13.0.post1/cortex_cli/core/mlflow/mlflow_cortex.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/core/models/cortex_model.py` & `cortex_cli-1.13.0.post1/cortex_cli/core/models/cortex_model.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/core/secrets_manager.py` & `cortex_cli-1.13.0.post1/cortex_cli/core/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/.gitignore` & `cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/README.md` & `cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/.gitignore` & `cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/README.md` & `cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/tests/test_cortex_data.py` & `cortex_cli-1.13.0.post1/cortex_cli/tests/test_cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli/tests/test_ethics_checks.py` & `cortex_cli-1.13.0.post1/cortex_cli/tests/test_ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/cortex_cli.egg-info/SOURCES.txt` & `cortex_cli-1.13.0.post1/cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.6/setup.py` & `cortex_cli-1.13.0.post1/setup.py`

 * *Files identical despite different names*


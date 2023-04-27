# Comparing `tmp/rockingester-1.1.1.tar.gz` & `tmp/rockingester-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockingester-1.1.1.tar", last modified: Wed Apr 26 08:00:05 2023, max compression
+gzip compressed data, was "rockingester-2.0.0.tar", last modified: Thu Apr 27 05:48:01 2023, max compression
```

## Comparing `rockingester-1.1.1.tar` & `rockingester-2.0.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.814047 rockingester-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.806048 rockingester-1.1.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-26 07:59:56.000000 rockingester-1.1.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.806048 rockingester-1.1.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-26 07:59:56.000000 rockingester-1.1.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-26 07:59:56.000000 rockingester-1.1.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-26 07:59:56.000000 rockingester-1.1.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-26 07:59:56.000000 rockingester-1.1.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-26 07:59:56.000000 rockingester-1.1.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 07:59:56.000000 rockingester-1.1.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 07:59:56.000000 rockingester-1.1.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 07:59:56.000000 rockingester-1.1.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.806048 rockingester-1.1.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-26 07:59:56.000000 rockingester-1.1.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-26 07:59:56.000000 rockingester-1.1.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.806048 rockingester-1.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-26 07:59:56.000000 rockingester-1.1.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.802048 rockingester-1.1.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.806048 rockingester-1.1.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-26 07:59:56.000000 rockingester-1.1.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-26 07:59:56.000000 rockingester-1.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.806048 rockingester-1.1.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-26 07:59:56.000000 rockingester-1.1.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-26 07:59:56.000000 rockingester-1.1.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-26 07:59:56.000000 rockingester-1.1.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-26 07:59:56.000000 rockingester-1.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-26 07:59:56.000000 rockingester-1.1.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-26 07:59:56.000000 rockingester-1.1.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-26 07:59:56.000000 rockingester-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-26 07:59:56.000000 rockingester-1.1.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 07:59:56.000000 rockingester-1.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-26 07:59:56.000000 rockingester-1.1.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-26 07:59:56.000000 rockingester-1.1.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 07:59:56.000000 rockingester-1.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-26 07:59:56.000000 rockingester-1.1.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 07:59:56.000000 rockingester-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-04-26 08:00:05.814047 rockingester-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-26 07:59:56.000000 rockingester-1.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-26 07:59:56.000000 rockingester-1.1.1/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.806048 rockingester-1.1.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 07:59:56.000000 rockingester-1.1.1/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-26 07:59:56.000000 rockingester-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:00:05.814047 rockingester-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.806048 rockingester-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/src/rockingester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-04-26 08:00:05.000000 rockingester-1.1.1/src/rockingester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-26 08:00:05.000000 rockingester-1.1.1/src/rockingester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:00:05.000000 rockingester-1.1.1/src/rockingester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 08:00:05.000000 rockingester-1.1.1/src/rockingester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-26 08:00:05.000000 rockingester-1.1.1/src/rockingester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 08:00:05.000000 rockingester-1.1.1/src/rockingester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.810047 rockingester-1.1.1/src/rockingester_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.814047 rockingester-1.1.1/src/rockingester_api/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_api/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_api/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_api/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_api/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.814047 rockingester-1.1.1/src/rockingester_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.814047 rockingester-1.1.1/src/rockingester_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.814047 rockingester-1.1.1/src/rockingester_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 08:00:05.000000 rockingester-1.1.1/src/rockingester_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.814047 rockingester-1.1.1/src/rockingester_lib/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/collectors/direct_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.814047 rockingester-1.1.1/src/rockingester_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-26 07:59:56.000000 rockingester-1.1.1/src/rockingester_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.814047 rockingester-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:59:56.000000 rockingester-1.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-26 07:59:56.000000 rockingester-1.1.1/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:05.814047 rockingester-1.1.1/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-26 07:59:56.000000 rockingester-1.1.1/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-26 07:59:56.000000 rockingester-1.1.1/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-26 07:59:56.000000 rockingester-1.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13851 2023-04-26 07:59:56.000000 rockingester-1.1.1/tests/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.230316 rockingester-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-27 05:47:51.000000 rockingester-2.0.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-27 05:47:51.000000 rockingester-2.0.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.214316 rockingester-2.0.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-27 05:47:51.000000 rockingester-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-27 05:47:51.000000 rockingester-2.0.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-27 05:47:51.000000 rockingester-2.0.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-27 05:47:51.000000 rockingester-2.0.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-27 05:47:51.000000 rockingester-2.0.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-27 05:47:51.000000 rockingester-2.0.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 05:47:51.000000 rockingester-2.0.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 05:47:51.000000 rockingester-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-04-27 05:48:01.230316 rockingester-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-27 05:47:51.000000 rockingester-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-27 05:47:51.000000 rockingester-2.0.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-27 05:47:51.000000 rockingester-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 05:48:01.230316 rockingester-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester_api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.230316 rockingester-2.0.0/src/rockingester_lib/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/direct_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.230316 rockingester-2.0.0/src/rockingester_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.230316 rockingester-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.230316 rockingester-2.0.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/configurations/direct_poll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/test_collector.py
```

### Comparing `rockingester-1.1.1/.dae-devops/Makefile` & `rockingester-2.0.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.dae-devops/docs/conventions.rst` & `rockingester-2.0.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.dae-devops/docs/developing.rst` & `rockingester-2.0.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.dae-devops/docs/devops.rst` & `rockingester-2.0.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.dae-devops/docs/docs_structure.rst` & `rockingester-2.0.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.dae-devops/docs/installing.rst` & `rockingester-2.0.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.dae-devops/docs/testing.rst` & `rockingester-2.0.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.dae-devops/project.yaml` & `rockingester-2.0.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.devcontainer/Dockerfile` & `rockingester-2.0.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.devcontainer/devcontainer.json` & `rockingester-2.0.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.github/CONTRIBUTING.rst` & `rockingester-2.0.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.github/actions/install_requirements/action.yml` & `rockingester-2.0.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.github/dependabot.yml` & `rockingester-2.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.github/pages/make_switcher.py` & `rockingester-2.0.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.github/workflows/code.yml` & `rockingester-2.0.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.github/workflows/docs.yml` & `rockingester-2.0.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.github/workflows/docs_clean.yml` & `rockingester-2.0.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.github/workflows/linkcheck.yml` & `rockingester-2.0.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.gitignore` & `rockingester-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.gitlab-ci.yml` & `rockingester-2.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/.vscode/launch.json` & `rockingester-2.0.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/LICENSE` & `rockingester-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/PKG-INFO` & `rockingester-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 1.1.1
+Version: 2.0.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -262,23 +262,23 @@
 
 Algorithm
 -----------------------------------------------------------------------
 Looks in SubwellImages directory.
 
 Uses first 4 letters of each subdirectory as "barcode".
 
-If barcode is NOT in the plates mined from the formulatrix, then moves subdirectory to SubwellImages_nobarcode.
+If barcode is NOT in the plates mined from the formulatrix, then it is ignored.
 
 Otherrwise, if name of plate is a valid visit name, and the visit directory exists, then copies the images to the visit directory and inserts them into the database.
 
 Otherwise ignores the subdirectory.
 
 We have to leave all plate directories in SubwellImages since this is where Texrank expects them.
 
-After we don't need Texrank, then we can move the non-visit directories into SubwellImages_novisit, and move (instead of copy) them for good visits.  This will keep SubwellImages clean and more efficient to poll.
+After we don't need Texrank, then we can move the non-visit directories into something like SubwellImages_novisit, and move (instead of copy) them for good visits.  This will keep SubwellImages clean and more efficient to poll.
 
 Documentation
 -----------------------------------------------------------------------
 
 See https://www.cs.diamond.ac.uk/rockingester for more detailed documentation.
 
 Building and viewing the documents locally::
```

### Comparing `rockingester-1.1.1/README.rst` & `rockingester-2.0.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -43,23 +43,23 @@
 
 Algorithm
 -----------------------------------------------------------------------
 Looks in SubwellImages directory.
 
 Uses first 4 letters of each subdirectory as "barcode".
 
-If barcode is NOT in the plates mined from the formulatrix, then moves subdirectory to SubwellImages_nobarcode.
+If barcode is NOT in the plates mined from the formulatrix, then it is ignored.
 
 Otherrwise, if name of plate is a valid visit name, and the visit directory exists, then copies the images to the visit directory and inserts them into the database.
 
 Otherwise ignores the subdirectory.
 
 We have to leave all plate directories in SubwellImages since this is where Texrank expects them.
 
-After we don't need Texrank, then we can move the non-visit directories into SubwellImages_novisit, and move (instead of copy) them for good visits.  This will keep SubwellImages clean and more efficient to poll.
+After we don't need Texrank, then we can move the non-visit directories into something like SubwellImages_novisit, and move (instead of copy) them for good visits.  This will keep SubwellImages clean and more efficient to poll.
 
 Documentation
 -----------------------------------------------------------------------
 
 See https://www.cs.diamond.ac.uk/rockingester for more detailed documentation.
 
 Building and viewing the documents locally::
```

### Comparing `rockingester-1.1.1/configurations/development.yaml` & `rockingester-2.0.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/docs/conf.py` & `rockingester-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/docs/images/dls-favicon.ico` & `rockingester-2.0.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/docs/images/dls-logo.svg` & `rockingester-2.0.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/docs/index.rst` & `rockingester-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/docs/user/explanations/25-docs-structure.rst` & `rockingester-2.0.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/docs/user/index.rst` & `rockingester-2.0.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/pyproject.toml` & `rockingester-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester.egg-info/PKG-INFO` & `rockingester-2.0.0/src/rockingester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 1.1.1
+Version: 2.0.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -262,23 +262,23 @@
 
 Algorithm
 -----------------------------------------------------------------------
 Looks in SubwellImages directory.
 
 Uses first 4 letters of each subdirectory as "barcode".
 
-If barcode is NOT in the plates mined from the formulatrix, then moves subdirectory to SubwellImages_nobarcode.
+If barcode is NOT in the plates mined from the formulatrix, then it is ignored.
 
 Otherrwise, if name of plate is a valid visit name, and the visit directory exists, then copies the images to the visit directory and inserts them into the database.
 
 Otherwise ignores the subdirectory.
 
 We have to leave all plate directories in SubwellImages since this is where Texrank expects them.
 
-After we don't need Texrank, then we can move the non-visit directories into SubwellImages_novisit, and move (instead of copy) them for good visits.  This will keep SubwellImages clean and more efficient to poll.
+After we don't need Texrank, then we can move the non-visit directories into something like SubwellImages_novisit, and move (instead of copy) them for good visits.  This will keep SubwellImages clean and more efficient to poll.
 
 Documentation
 -----------------------------------------------------------------------
 
 See https://www.cs.diamond.ac.uk/rockingester for more detailed documentation.
 
 Building and viewing the documents locally::
```

### Comparing `rockingester-1.1.1/src/rockingester.egg-info/SOURCES.txt` & `rockingester-2.0.0/src/rockingester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_api/collectors/aiohttp.py` & `rockingester-2.0.0/src/rockingester_api/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_api/collectors/collectors.py` & `rockingester-2.0.0/src/rockingester_api/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_api/collectors/context.py` & `rockingester-2.0.0/src/rockingester_api/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_api/context_base.py` & `rockingester-2.0.0/src/rockingester_api/context_base.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_api/exceptions.py` & `rockingester-2.0.0/src/rockingester_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_api/thing.py` & `rockingester-2.0.0/src/rockingester_api/thing.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_api/things.py` & `rockingester-2.0.0/src/rockingester_api/things.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_cli/main.py` & `rockingester-2.0.0/src/rockingester_cli/main.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_cli/subcommands/base.py` & `rockingester-2.0.0/src/rockingester_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_cli/subcommands/service.py` & `rockingester-2.0.0/src/rockingester_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_cli/version.py` & `rockingester-2.0.0/src/rockingester_cli/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_lib/__main__.py` & `rockingester-2.0.0/src/rockingester_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_lib/collectors/aiohttp.py` & `rockingester-2.0.0/src/rockingester_lib/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_lib/collectors/base.py` & `rockingester-2.0.0/src/rockingester_lib/collectors/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_lib/collectors/collectors.py` & `rockingester-2.0.0/src/rockingester_lib/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_lib/collectors/context.py` & `rockingester-2.0.0/src/rockingester_lib/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_lib/collectors/direct_poll.py` & `rockingester-2.0.0/src/rockingester_lib/collectors/direct_poll.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,79 +29,69 @@
 thing_type = "rockingester_lib.collectors.direct_poll"
 
 
 # ------------------------------------------------------------------------------------------
 class DirectPoll(CollectorBase):
     """
     Object representing an image collector.
-    The behavior is to start a coro task to waken every few seconds and scan for incoming files.
-    Files are pushed to xchembku.
+    The behavior is to start a coro task to waken every few seconds and scan for newly created plate directories.
+    Image files are pushed to xchembku.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification, predefined_uuid=None):
         CollectorBase.__init__(
             self, thing_type, specification, predefined_uuid=predefined_uuid
         )
 
         s = f"{callsign(self)} specification", self.specification()
 
         type_specific_tbd = require(s, self.specification(), "type_specific_tbd")
+
+        # The sources for the collecting.
         self.__plates_directories = require(s, type_specific_tbd, "plates_directories")
+
+        # The root directory of all visits.
         self.__visits_directory = Path(
             require(s, type_specific_tbd, "visits_directory")
         )
+
+        # The subdirectory under a visit where to put subwell images that are collected.
         self.__visit_plates_subdirectory = Path(
             require(s, type_specific_tbd, "visit_plates_subdirectory")
         )
-        self.__novisit_directory = Path(
-            require(s, type_specific_tbd, "novisit_directory")
-        )
-        self.__nobarcode_directory = Path(
-            require(s, type_specific_tbd, "nobarcode_directory")
-        )
 
+        # Explicit list of barcodes to process (used when testing a deployment).
         self.__ingest_only_barcodes = type_specific_tbd.get("ingest_only_barcodes")
 
         # Database where we will get plate barcodes and add new wells.
         self.__xchembku_client_context = None
         self.__xchembku = None
 
         # This flag will stop the ticking async task.
         self.__keep_ticking = True
         self.__tick_future = None
 
+        # This is the last formulatrix plate we have ingested, used to avoid re-handling the same plate.
         self.__latest_formulatrix__plate__id = 0
 
         # This is the list of plates indexed by their barcode.
         self.__crystal_plate_models_by_barcode: Dict[CrystalPlateModel] = {}
 
-        # The plate names which we have already finished handling.
+        # The plate names which we have already finished handling within the current instance.
         self.__handled_plate_names = []
 
     # ----------------------------------------------------------------------------------------
     async def activate(self) -> None:
         """
         Activate the object.
 
         Then it starts the coro task to awaken every few seconds to scrape the directories.
         """
 
-        # Make sure the novisit_directory is created.
-        try:
-            self.__novisit_directory.mkdir(parents=True)
-        except FileExistsError:
-            pass
-
-        # Make sure the nobarcode_directory is created.
-        try:
-            self.__nobarcode_directory.mkdir(parents=True)
-        except FileExistsError:
-            pass
-
         # Make the xchembku client context.
         s = require(
             f"{callsign(self)} specification",
             self.specification(),
             "type_specific_tbd",
         )
         s = require(
@@ -233,164 +223,109 @@
                     continue
 
             # Get the matching plate record from the database.
             crystal_plate_model = self.__crystal_plate_models_by_barcode.get(
                 plate_barcode
             )
 
-            # This plate is in the database?
-            if crystal_plate_model is not None:
-                visit_directory = None
-                try:
-                    visit_directory = Path(
-                        get_xchem_directory(
-                            self.__visits_directory, crystal_plate_model.visit
-                        )
-                    )
-                except ValueError:
-                    pass
-                except VisitNotFound:
-                    pass
-
-                if visit_directory is not None:
-                    await self.scrape_plate_directory(
-                        plates_directory / plate_name,
-                        crystal_plate_model,
-                        visit_directory,
+            # This plate is not in the database?
+            if crystal_plate_model is None:
+                continue
+
+            try:
+                visit_directory = Path(
+                    get_xchem_directory(
+                        self.__visits_directory, crystal_plate_model.visit
                     )
-                # This barcode is in the database, but the visit name
-                # is not properly formatted or the visit directory doesn't exist.
-                else:
-                    # For now, don't move these out of SubwellImages since Texrank expects them here.
-                    # TODO: Find out how to disable Texrank jobs from running at all.
-                    # await self.__move_without_ingesting(
-                    #     plates_directory / plate_name,
-                    #     self.__novisit_directory,
-                    # )
-
-                    # Remember we "handled" this one.
-                    self.__handled_plate_names.append(plate_name)
-
-            # Not in the formulatrix's database?
-            else:
-                # Move the plate directory somewhere else.
-                await self.__move_without_ingesting(
-                    plates_directory / plate_name,
-                    self.__nobarcode_directory,
                 )
+            # This is an improperly formatted visit name?
+            except ValueError:
+                continue
+            # This visit is not found on disk?
+            except VisitNotFound:
+                continue
 
-    # ----------------------------------------------------------------------------------------
-    async def __move_without_ingesting(
-        self,
-        plate_directory: Path,
-        target_directory: Path,
-    ) -> None:
-        """
-        Move a plate directory's well images to the given target without ingesting it.
-
-        Then remove the plate directory.
-        """
-
-        target = target_directory / plate_directory.name
-        try:
-            target.mkdir(parents=True)
-        except FileExistsError:
-            pass
-
-        # Get all the well images in the plate directory.
-        well_names = [
-            entry.name for entry in os.scandir(plate_directory) if entry.is_file()
-        ]
-
-        for well_name in well_names:
-            # Move to target, replacing what might already be there.
-            # TODO: Protect against moving an image file which is currently being written by Luigi.
-            shutil.move(
-                plate_directory / well_name,
-                target / well_name,
+            # Scrape the directory when all image files have arrived.
+            await self.scrape_plate_directory_when_complete(
+                plates_directory / plate_name,
+                crystal_plate_model,
+                visit_directory,
             )
 
-        # Remove the source directory, which should now be empty.
-        # TODO: Protect against removing an plate directory which is currently being written by Luigi.
-        try:
-            plate_directory.rmdir()
-        except OSError:
-            pass
-
-        logger.info(f"moved plate {plate_directory.name} to {target_directory}")
-
     # ----------------------------------------------------------------------------------------
-    async def scrape_plate_directory(
+    async def scrape_plate_directory_when_complete(
         self,
         plate_directory: Path,
         crystal_plate_model: CrystalPlateModel,
         visit_directory: Path,
     ) -> None:
         """
         Scrape a single directory looking for new files.
 
         Adds discovered files to internal list which gets pushed when it reaches a configurable size.
         """
 
-        # Update the path stem in the crystal plate record.
-        # TODO: Consider if important to report/record same barcodes on different rockmaker directories.
+        # Name of the destination directory where we will permanently store ingested well image files.
+        target = (
+            visit_directory / self.__visit_plates_subdirectory / plate_directory.name
+        )
+
+        # We have already put this plate directory into the visit directory and presumably also the database?
+        if target.is_dir():
+            # Remember we "handled" this one.
+            self.__handled_plate_names.append(plate_directory.stem)
+            return
+
+        # This is the first time we have scraped a directory for this plate?
         if crystal_plate_model.rockminer_collected_stem is None:
+            # Update the path stem in the crystal plate record.
+            # TODO: Consider if important to report/record same barcodes on different rockmaker directories.
             crystal_plate_model.rockminer_collected_stem = plate_directory.stem
             await self.__xchembku.upsert_crystal_plates(
                 [crystal_plate_model], "update rockminer_collected_stem"
             )
 
         # Get all the well images in the plate directory.
         well_names = [
             entry.name for entry in os.scandir(plate_directory) if entry.is_file()
         ]
 
         # Don't handle the plate directory until all images have arrived.
         if len(well_names) < 288:
             return
 
-        # Name of the destination directory where we will permanently store ingested well image files.
-        target = (
-            visit_directory / self.__visit_plates_subdirectory / plate_directory.name
-        )
-
-        # We have already put this plate directory into the visit directory?
-        # And presumable the database?
-        if target.is_dir():
-            # Remember we "handled" this one.
-            self.__handled_plate_names.append(plate_directory.stem)
-            return
-
-        # Sort so that tests are deterministic.
+        # Sort wells by name so that tests are deterministic.
         well_names.sort()
 
         crystal_well_models: List[CrystalWellModel] = []
         for well_name in well_names:
-            # Process well's image file.
-            # TODO: Improve safety by ignoring wrongly formatted and non-jpg well filenames.
-            crystal_well_models.append(
-                await self.ingest_well(
-                    plate_directory,
-                    well_name,
-                    crystal_plate_model,
-                    target,
-                )
+            # Make the well model, including image width/height.
+            crystal_well_model = await self.ingest_well(
+                plate_directory,
+                well_name,
+                crystal_plate_model,
+                target,
             )
 
+            # Append well model to the list of all wells on the plate.
+            crystal_well_models.append(crystal_well_model)
+
         # Here we create or update the crystal well records into xchembku.
-        # TODO: Handle case where we upsert the crystal_well record bit the image object store fails to accept image binary.
         await self.__xchembku.upsert_crystal_wells(crystal_well_models)
 
         # Copy scraped directory to visit, replacing what might already be there.
+        # TODO: Handle case where we upsert the crystal_well record but then unable to copy image file.
         shutil.copytree(
             plate_directory,
             target,
         )
 
-        logger.info(f"copied well images from plate {plate_directory.name} to {target}")
+        logger.info(
+            f"copied {len(well_names)} well images from plate {plate_directory.name} to {target}"
+        )
 
         # Remember we "handled" this one.
         self.__handled_plate_names.append(plate_directory.stem)
 
     # ----------------------------------------------------------------------------------------
     async def ingest_well(
         self,
@@ -405,14 +340,15 @@
         Move the well image file to the ingested area.
         """
 
         input_well_filename = plate_directory / well_name
         ingested_well_filename = target / well_name
 
         # Stems are like "9acx_01A_1".
+        # TODO: Improve safety by ignoring wrongly formatted and non-jpg well filenames.
         parts = Path(well_name).stem.split("_")
         if len(parts) > 1:
             # Strip off the leading 4-letter barcode and underscore.
             position = "".join(parts[1:])
         else:
             position = parts[0]
```

### Comparing `rockingester-1.1.1/src/rockingester_lib/contexts/base.py` & `rockingester-2.0.0/src/rockingester_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_lib/exceptions.py` & `rockingester-2.0.0/src/rockingester_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/src/rockingester_lib/version.py` & `rockingester-2.0.0/src/rockingester_lib/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/tests/base.py` & `rockingester-2.0.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/tests/configurations/direct_poll.yaml` & `rockingester-2.0.0/tests/configurations/direct_poll.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -6,27 +6,23 @@
     database:
         type: "xchembku_lib.xchembku_databases.normsql"
         filename: "${output_directory}/xchembku.sqlite"
         log_level: "WARNING"
 
 visits_directory: &VISITS_DIRECTORY "${output_directory}/visits"
 visit_plates_subdirectory: &VISIT_PLATES_SUBDIRECTORY "processing/rockingester"
-novisit_directory: &NONVISIT_DIRECTORY "${output_directory}/SubwellImages_novisit"
-nobarcode_directory: &NOBARCODE_DIRECTORY "${output_directory}/SubwellImages_nobarcode"
 
 # The rockingester direct access.
 rockingester_collector_specification:
     type: "rockingester_lib.collectors.direct_poll"
     type_specific_tbd:
         plates_directories:
             - "${output_directory}/SubwellImages"
         visits_directory: *VISITS_DIRECTORY
         visit_plates_subdirectory: *VISIT_PLATES_SUBDIRECTORY
-        novisit_directory: *NONVISIT_DIRECTORY
-        nobarcode_directory: *NOBARCODE_DIRECTORY
         xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION
         ingest_only_barcodes:
             - 98ab
             - 98ac
             - 98ad
     context:
         start_as: direct
```

### Comparing `rockingester-1.1.1/tests/configurations/service.yaml` & `rockingester-2.0.0/tests/configurations/service.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -23,28 +23,24 @@
     database:
         type: "xchembku_lib.xchembku_databases.normsql"
         filename: "${output_directory}/xchembku.sqlite"
         log_level: "WARNING"
 
 visits_directory: &VISITS_DIRECTORY "${output_directory}/visits"
 visit_plates_subdirectory: &VISIT_PLATES_SUBDIRECTORY "processing/rockingester"
-novisit_directory: &NONVISIT_DIRECTORY "${output_directory}/SubwellImages_novisit"
-nobarcode_directory: &NOBARCODE_DIRECTORY "${output_directory}/SubwellImages_nobarcode"
 
 # The rockingester direct access.
 rockingester_collector_specification_direct_poll:
     &ROCKINGESTER_COLLECTOR_SPECIFICATION_DIRECT_POLL
     type: "rockingester_lib.collectors.direct_poll"
     type_specific_tbd:
         plates_directories:
             - "${output_directory}/SubwellImages"
         visits_directory: *VISITS_DIRECTORY
         visit_plates_subdirectory: *VISIT_PLATES_SUBDIRECTORY
-        novisit_directory: *NONVISIT_DIRECTORY
-        nobarcode_directory: *NOBARCODE_DIRECTORY
         xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION
         ingest_only_barcodes:
             - 98ab
             - 98ac
             - 98ad
 
 # The rockingester client/server composite.
```

### Comparing `rockingester-1.1.1/tests/conftest.py` & `rockingester-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.1.1/tests/test_collector.py` & `rockingester-2.0.0/tests/test_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,16 +65,17 @@
         First it starts the xchembku and collector and loads a single plate barcode into the database.
 
         Then, while the collector thread is running, it creates some scrapable images.
 
         The test then waits a while for the scraping to be done, and verifies the outputs.
 
         These are in 3 barcodes.  The first matches the barcode in the database, so it gets scraped.
-        The second matches no barcode in the database, so it is moved to the nobarcode area and not added to the database.
-        The third barcode is not scraped because it is not configured in the ingest_only_barcodes list.
+        The second matches no barcode in the database, so it is ignored.
+        The third matches a barcode, but the visit is improperly formatted, so it is ignored.
+        The fourth barcode is not scraped because it is not configured in the ingest_only_barcodes list.
         """
 
         # Get the multiconf from the testing configuration yaml.
         multiconf = self.get_multiconf()
 
         # Load the multiconf into a dict.
         multiconf_dict = await multiconf.load()
@@ -97,16 +98,14 @@
         collector_client_context = CollectorClientContext(collector_specification)
 
         # Remember the collector specification so we can assert some things later.
         self.__visits_directory = Path(multiconf_dict["visits_directory"])
         self.__visit_plates_subdirectory = Path(
             multiconf_dict["visit_plates_subdirectory"]
         )
-        self.__nobarcode_directory = Path(multiconf_dict["nobarcode_directory"])
-        self.__novisit_directory = Path(multiconf_dict["novisit_directory"])
 
         scrapable_image_count = 288
 
         # Start the client context for the direct access to the xchembku.
         async with xchembku_client_context:
             # Start the collector client context.
             async with collector_client_context:
@@ -180,27 +179,27 @@
         plate_directory1.mkdir(parents=True)
         for i in range(10, 10 + scrapable_image_count):
             filename = plate_directory1 / ("98ab_%03dA_1.jpg" % (i))
             with open(filename, "w") as stream:
                 stream.write("")
 
         # Make another scrapable directory with a different barcode.
-        # This one gets moved into nobarcode since it doesn't match any plate.
+        # This one gets ignored since it doesn't match any plate's barcode.
         plate_directory2 = (
             plates_directory / f"{nobarcode_barcode}_2023-04-06_RI1000-0276-3drop"
         )
         plate_directory2.mkdir(parents=True)
         nobarcode_image_count = 3
         for i in range(10, 10 + nobarcode_image_count):
             filename = plate_directory2 / ("%s_%03dA_1.jpg" % (nobarcode_barcode, i))
             with open(filename, "w") as stream:
                 stream.write("")
 
         # Make yet another scrapable directory with a different barcode.
-        # This one gets moved into novisit since it matches a plate with a bad visit name.
+        # This one gets ignored since it matches a plate with a bad visit name.
         plate_directory3 = (
             plates_directory / f"{novisit_barcode}_2023-04-06_RI1000-0276-3drop"
         )
         plate_directory3.mkdir(parents=True)
         novisit_image_count = 6
         for i in range(10, 10 + novisit_image_count):
             filename = plate_directory3 / ("%s_%03dA_1.jpg" % (novisit_barcode, i))
@@ -259,22 +258,22 @@
             assert crystal_well_model.position == "%03dA1" % (i)
             i += 1
 
         # The first "scrapable" plate directory should still exist.
         count = sum(1 for _ in plate_directory1.glob("*") if _.is_file())
         assert count == scrapable_image_count, "first (scrapable) plate_directory"
 
-        # The second "nobarcode" plate directory should no longer exist.
+        # The second "nobarcode" plate directory should still exist.
         count = sum(1 for _ in plate_directory2.glob("*") if _.is_file())
-        assert count == 0, "second plate_directory"
+        assert count == nobarcode_image_count, "nobarcode plate_directory"
 
         # The third plate directory (novisit) is left intact.
         # We keep "novisit" plate directories for now, since Texrank still needs them.
         count = sum(1 for _ in plate_directory3.glob("*") if _.is_file())
-        assert count == novisit_image_count, "third plate_directory"
+        assert count == novisit_image_count, "novisit plate_directory"
 
         # The fourth plate directory is left intact.
         count = sum(1 for _ in plate_directory4.glob("*") if _.is_file())
         assert count == excluded_image_count, "fourth plate_directory"
 
         # We should have ingested the first barcode.
         count = sum(1 for _ in rockingester_directory.glob("*") if _.is_dir())
@@ -284,36 +283,14 @@
             for _ in (rockingester_directory / plate_directory1.name).glob("*")
             if _.is_file()
         )
         assert (
             count == scrapable_image_count
         ), f"ingested_directory images {str(rockingester_directory)}"
 
-        # We should have sent the second barcode to the nobarcode area.
-        count = sum(1 for _ in self.__nobarcode_directory.glob("*") if _.is_dir())
-        assert count == 1, f"nobarcode_directory {str(self.__nobarcode_directory)}"
-        count = sum(
-            1
-            for _ in (self.__nobarcode_directory / plate_directory2.name).glob("*")
-            if _.is_file()
-        )
-        assert (
-            count == nobarcode_image_count
-        ), f"nobarcode_directory images {str(self.__nobarcode_directory)}"
-
-        # We should NOT have sent the third (novisit) barcode to the novisit area.
-        count = sum(1 for _ in self.__novisit_directory.glob("*") if _.is_dir())
-        assert count == 0, f"novisit_directory {str(self.__novisit_directory)}"
-        count = sum(
-            1
-            for _ in (self.__novisit_directory / plate_directory3.name).glob("*")
-            if _.is_file()
-        )
-        assert count == 0, f"novisit_directory images {str(self.__novisit_directory)}"
-
     # ----------------------------------------------------------------------------------------
 
     async def __run_part2(self, scrapable_image_count, constants, output_directory):
         """ """
         # Reference the xchembku object which the context has set up as the default.
         xchembku = xchembku_datafaces_get_default()
```


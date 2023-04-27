# Comparing `tmp/django_spinproject-2.4.0.tar.gz` & `tmp/django_spinproject-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_spinproject-2.4.0.tar", max compression
+gzip compressed data, was "django_spinproject-2.5.0.tar", max compression
```

## Comparing `django_spinproject-2.4.0.tar` & `django_spinproject-2.5.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0     1076 2022-12-22 06:56:55.784266 django_spinproject-2.4.0/LICENSE
--rw-r--r--   0        0        0     3789 2023-02-02 14:08:15.681510 django_spinproject-2.4.0/README.md
--rwxr-xr-x   0        0        0     1028 2022-12-22 06:56:55.784266 django_spinproject-2.4.0/django_spinproject/bin/enhance-dockerfile.py
--rwxr-xr-x   0        0        0      640 2022-12-22 06:56:55.784266 django_spinproject-2.4.0/django_spinproject/bin/enhance-dockerignore.py
--rwxr-xr-x   0        0        0     7094 2022-12-22 06:56:55.784266 django_spinproject-2.4.0/django_spinproject/bin/enhance-gitignore.py
--rwxr-xr-x   0        0        0     2831 2022-12-22 06:56:55.784266 django_spinproject-2.4.0/django_spinproject/bin/enhance-gitlab-ci.py
--rwxr-xr-x   0        0        0      668 2022-12-22 06:56:55.784266 django_spinproject-2.4.0/django_spinproject/bin/enhance-makefile.py
--rwxr-xr-x   0        0        0      672 2022-12-22 06:56:55.784266 django_spinproject-2.4.0/django_spinproject/bin/enhance-pg-readonly.py
--rwxr-xr-x   0        0        0      902 2022-12-22 06:56:55.784266 django_spinproject-2.4.0/django_spinproject/bin/enhance-pytest.py
--rwxr-xr-x   0        0        0     5800 2022-12-22 06:56:55.784266 django_spinproject-2.4.0/django_spinproject/bin/enhance-settings.py
--rwxr-xr-x   0        0        0     1946 2022-12-22 06:56:55.784266 django_spinproject-2.4.0/django_spinproject/bin/enhance-srta.py
--rwxr-xr-x   0        0        0     1759 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/bin/spinproject.py
--rw-r--r--   0        0        0     1832 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/cli.py
--rw-r--r--   0        0        0       22 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/constants.py
--rw-r--r--   0        0        0        0 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/generic/__init__.py
--rw-r--r--   0        0        0      318 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/generic/compatibility_trait.py
--rw-r--r--   0        0        0      544 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/generic/dicts_merging.py
--rw-r--r--   0        0        0      803 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/generic/directory_cleaning.py
--rw-r--r--   0        0        0      106 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/generic/exit.py
--rw-r--r--   0        0        0      712 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/generic/extended_jinja_environment.py
--rw-r--r--   0        0        0     1898 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/generic/file_upgrade.py
--rw-r--r--   0        0        0      730 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/generic/hash.py
--rw-r--r--   0        0        0      389 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/generic/serializable_obj.py
--rw-r--r--   0        0        0      726 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/__init__.py
--rw-r--r--   0        0        0     2830 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/_base.py
--rw-r--r--   0        0        0      617 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/_mixins.py
--rw-r--r--   0        0        0      747 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/docker_scripts.py
--rw-r--r--   0        0        0      205 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/docker_scripts_data/__init__.py
--rw-r--r--   0        0        0      292 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/docker_scripts_data/v1.py
--rw-r--r--   0        0        0      497 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/dockerfile.py
--rw-r--r--   0        0        0      307 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/dockerfile_data/__init__.py
--rw-r--r--   0        0        0      793 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/dockerfile_data/v1.py
--rw-r--r--   0        0        0      868 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/dockerfile_data/v2.py
--rw-r--r--   0        0        0      236 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/dockerignore.py
--rw-r--r--   0        0        0      409 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/dockerignore_data/__init__.py
--rw-r--r--   0        0        0      345 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/dockerignore_data/v1.py
--rw-r--r--   0        0        0      356 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/dockerignore_data/v2.py
--rw-r--r--   0        0        0      385 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/dockerignore_data/v3.py
--rw-r--r--   0        0        0      242 2023-02-08 12:12:58.924356 django_spinproject-2.4.0/django_spinproject/modules/gitignore.py
--rw-r--r--   0        0        0      511 2023-02-08 12:12:58.924356 django_spinproject-2.4.0/django_spinproject/modules/gitignore_data/__init__.py
--rw-r--r--   0        0        0     6801 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/gitignore_data/v1.py
--rw-r--r--   0        0        0     6809 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/gitignore_data/v2.py
--rw-r--r--   0        0        0     6818 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/gitignore_data/v3.py
--rw-r--r--   0        0        0     6819 2023-02-08 12:12:58.924356 django_spinproject-2.4.0/django_spinproject/modules/gitignore_data/v4.py
--rw-r--r--   0        0        0      535 2023-02-03 06:25:59.487960 django_spinproject-2.4.0/django_spinproject/modules/gitlab_ci.py
--rw-r--r--   0        0        0      409 2023-02-03 06:25:59.491960 django_spinproject-2.4.0/django_spinproject/modules/gitlab_ci_data/__init__.py
--rw-r--r--   0        0        0     2529 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/gitlab_ci_data/v1.py
--rw-r--r--   0        0        0     2545 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/gitlab_ci_data/v2.py
--rw-r--r--   0        0        0     2926 2023-02-03 06:25:59.491960 django_spinproject-2.4.0/django_spinproject/modules/gitlab_ci_data/v3.py
--rw-r--r--   0        0        0      465 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/pg_readonly.py
--rw-r--r--   0        0        0      205 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/pg_readonly_data/__init__.py
--rw-r--r--   0        0        0      288 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/pg_readonly_data/v1.py
--rw-r--r--   0        0        0      519 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/pytest.py
--rw-r--r--   0        0        0      205 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/pytest_data/__init__.py
--rw-r--r--   0        0        0      374 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/pytest_data/v1.py
--rw-r--r--   0        0        0     1988 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/settings.py
--rw-r--r--   0        0        0      307 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/settings_data/__init__.py
--rw-r--r--   0        0        0     4861 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/settings_data/v1.py
--rw-r--r--   0        0        0     5019 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/settings_data/v2.py
--rw-r--r--   0        0        0     1723 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/srta.py
--rw-r--r--   0        0        0      361 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/srta_data/__init__.py
--rw-r--r--   0        0        0     1738 2023-02-02 13:47:45.971755 django_spinproject-2.4.0/django_spinproject/modules/srta_data/v1.py
--rw-r--r--   0        0        0     1745 2023-02-02 13:47:45.975756 django_spinproject-2.4.0/django_spinproject/modules/srta_data/v2.py
--rw-r--r--   0        0        0        0 2023-02-02 13:47:45.975756 django_spinproject-2.4.0/django_spinproject/project_manager/__init__.py
--rw-r--r--   0        0        0     3962 2023-02-02 13:47:45.975756 django_spinproject-2.4.0/django_spinproject/project_manager/project_info.py
--rw-r--r--   0        0        0     5094 2023-02-02 13:47:45.975756 django_spinproject-2.4.0/django_spinproject/project_manager/project_info_manager.py
--rw-r--r--   0        0        0      982 2023-02-08 12:12:58.924356 django_spinproject-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     5406 1970-01-01 00:00:00.000000 django_spinproject-2.4.0/setup.py
--rw-r--r--   0        0        0     4918 1970-01-01 00:00:00.000000 django_spinproject-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-12-22 06:56:55.784266 django_spinproject-2.5.0/LICENSE
+-rw-r--r--   0        0        0     3789 2023-02-02 14:08:15.681510 django_spinproject-2.5.0/README.md
+-rwxr-xr-x   0        0        0     1028 2022-12-22 06:56:55.784266 django_spinproject-2.5.0/django_spinproject/bin/enhance-dockerfile.py
+-rwxr-xr-x   0        0        0      640 2022-12-22 06:56:55.784266 django_spinproject-2.5.0/django_spinproject/bin/enhance-dockerignore.py
+-rwxr-xr-x   0        0        0     7094 2022-12-22 06:56:55.784266 django_spinproject-2.5.0/django_spinproject/bin/enhance-gitignore.py
+-rwxr-xr-x   0        0        0     2831 2022-12-22 06:56:55.784266 django_spinproject-2.5.0/django_spinproject/bin/enhance-gitlab-ci.py
+-rwxr-xr-x   0        0        0      668 2022-12-22 06:56:55.784266 django_spinproject-2.5.0/django_spinproject/bin/enhance-makefile.py
+-rwxr-xr-x   0        0        0      672 2022-12-22 06:56:55.784266 django_spinproject-2.5.0/django_spinproject/bin/enhance-pg-readonly.py
+-rwxr-xr-x   0        0        0      902 2022-12-22 06:56:55.784266 django_spinproject-2.5.0/django_spinproject/bin/enhance-pytest.py
+-rwxr-xr-x   0        0        0     5800 2022-12-22 06:56:55.784266 django_spinproject-2.5.0/django_spinproject/bin/enhance-settings.py
+-rwxr-xr-x   0        0        0     1946 2022-12-22 06:56:55.784266 django_spinproject-2.5.0/django_spinproject/bin/enhance-srta.py
+-rwxr-xr-x   0        0        0     1812 2023-04-27 08:48:57.155641 django_spinproject-2.5.0/django_spinproject/bin/spinproject.py
+-rw-r--r--   0        0        0     1966 2023-04-27 08:48:57.155641 django_spinproject-2.5.0/django_spinproject/cli.py
+-rw-r--r--   0        0        0       22 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/constants.py
+-rw-r--r--   0        0        0        0 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/generic/__init__.py
+-rw-r--r--   0        0        0      318 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/generic/compatibility_trait.py
+-rw-r--r--   0        0        0      544 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/generic/dicts_merging.py
+-rw-r--r--   0        0        0      803 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/generic/directory_cleaning.py
+-rw-r--r--   0        0        0      106 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/generic/exit.py
+-rw-r--r--   0        0        0      712 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/generic/extended_jinja_environment.py
+-rw-r--r--   0        0        0     1900 2023-04-27 08:48:57.155641 django_spinproject-2.5.0/django_spinproject/generic/file_upgrade.py
+-rw-r--r--   0        0        0      730 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/generic/hash.py
+-rw-r--r--   0        0        0     1428 2023-04-27 08:48:57.155641 django_spinproject-2.5.0/django_spinproject/generic/package.py
+-rw-r--r--   0        0        0      389 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/generic/serializable_obj.py
+-rw-r--r--   0        0        0      726 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/__init__.py
+-rw-r--r--   0        0        0     2830 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/_base.py
+-rw-r--r--   0        0        0      617 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/_mixins.py
+-rw-r--r--   0        0        0      747 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/docker_scripts.py
+-rw-r--r--   0        0        0      205 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/docker_scripts_data/__init__.py
+-rw-r--r--   0        0        0      292 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/docker_scripts_data/v1.py
+-rw-r--r--   0        0        0      497 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/dockerfile.py
+-rw-r--r--   0        0        0      307 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/dockerfile_data/__init__.py
+-rw-r--r--   0        0        0      793 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/dockerfile_data/v1.py
+-rw-r--r--   0        0        0      868 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/dockerfile_data/v2.py
+-rw-r--r--   0        0        0      236 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/dockerignore.py
+-rw-r--r--   0        0        0      409 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/dockerignore_data/__init__.py
+-rw-r--r--   0        0        0      345 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/dockerignore_data/v1.py
+-rw-r--r--   0        0        0      356 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/dockerignore_data/v2.py
+-rw-r--r--   0        0        0      385 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/dockerignore_data/v3.py
+-rw-r--r--   0        0        0      242 2023-02-08 12:12:58.924356 django_spinproject-2.5.0/django_spinproject/modules/gitignore.py
+-rw-r--r--   0        0        0      511 2023-02-08 12:12:58.924356 django_spinproject-2.5.0/django_spinproject/modules/gitignore_data/__init__.py
+-rw-r--r--   0        0        0     6801 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/gitignore_data/v1.py
+-rw-r--r--   0        0        0     6809 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/gitignore_data/v2.py
+-rw-r--r--   0        0        0     6818 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/gitignore_data/v3.py
+-rw-r--r--   0        0        0     6819 2023-02-08 12:12:58.924356 django_spinproject-2.5.0/django_spinproject/modules/gitignore_data/v4.py
+-rw-r--r--   0        0        0      535 2023-02-03 06:25:59.487960 django_spinproject-2.5.0/django_spinproject/modules/gitlab_ci.py
+-rw-r--r--   0        0        0      409 2023-02-03 06:25:59.491960 django_spinproject-2.5.0/django_spinproject/modules/gitlab_ci_data/__init__.py
+-rw-r--r--   0        0        0     2529 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/gitlab_ci_data/v1.py
+-rw-r--r--   0        0        0     2545 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/gitlab_ci_data/v2.py
+-rw-r--r--   0        0        0     2926 2023-02-03 06:25:59.491960 django_spinproject-2.5.0/django_spinproject/modules/gitlab_ci_data/v3.py
+-rw-r--r--   0        0        0      465 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/pg_readonly.py
+-rw-r--r--   0        0        0      205 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/pg_readonly_data/__init__.py
+-rw-r--r--   0        0        0      288 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/pg_readonly_data/v1.py
+-rw-r--r--   0        0        0      519 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/pytest.py
+-rw-r--r--   0        0        0      205 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/pytest_data/__init__.py
+-rw-r--r--   0        0        0      374 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/pytest_data/v1.py
+-rw-r--r--   0        0        0     1988 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/settings.py
+-rw-r--r--   0        0        0      307 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/settings_data/__init__.py
+-rw-r--r--   0        0        0     4861 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/settings_data/v1.py
+-rw-r--r--   0        0        0     5019 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/settings_data/v2.py
+-rw-r--r--   0        0        0     1723 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/srta.py
+-rw-r--r--   0        0        0      361 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/srta_data/__init__.py
+-rw-r--r--   0        0        0     1738 2023-02-02 13:47:45.971755 django_spinproject-2.5.0/django_spinproject/modules/srta_data/v1.py
+-rw-r--r--   0        0        0     1745 2023-02-02 13:47:45.975756 django_spinproject-2.5.0/django_spinproject/modules/srta_data/v2.py
+-rw-r--r--   0        0        0        0 2023-02-02 13:47:45.975756 django_spinproject-2.5.0/django_spinproject/project_manager/__init__.py
+-rw-r--r--   0        0        0     3962 2023-02-02 13:47:45.975756 django_spinproject-2.5.0/django_spinproject/project_manager/project_info.py
+-rw-r--r--   0        0        0     5100 2023-04-27 08:48:57.159641 django_spinproject-2.5.0/django_spinproject/project_manager/project_info_manager.py
+-rw-r--r--   0        0        0      982 2023-04-27 08:50:17.259028 django_spinproject-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5406 1970-01-01 00:00:00.000000 django_spinproject-2.5.0/setup.py
+-rw-r--r--   0        0        0     4918 1970-01-01 00:00:00.000000 django_spinproject-2.5.0/PKG-INFO
```

### Comparing `django_spinproject-2.4.0/LICENSE` & `django_spinproject-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/README.md` & `django_spinproject-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/bin/enhance-dockerfile.py` & `django_spinproject-2.5.0/django_spinproject/bin/enhance-dockerfile.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/bin/enhance-dockerignore.py` & `django_spinproject-2.5.0/django_spinproject/bin/enhance-dockerignore.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/bin/enhance-gitignore.py` & `django_spinproject-2.5.0/django_spinproject/bin/enhance-gitignore.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/bin/enhance-gitlab-ci.py` & `django_spinproject-2.5.0/django_spinproject/bin/enhance-gitlab-ci.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/bin/enhance-makefile.py` & `django_spinproject-2.5.0/django_spinproject/bin/enhance-makefile.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/bin/enhance-pg-readonly.py` & `django_spinproject-2.5.0/django_spinproject/bin/enhance-pg-readonly.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/bin/enhance-pytest.py` & `django_spinproject-2.5.0/django_spinproject/bin/enhance-pytest.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/bin/enhance-settings.py` & `django_spinproject-2.5.0/django_spinproject/bin/enhance-settings.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/bin/enhance-srta.py` & `django_spinproject-2.5.0/django_spinproject/bin/enhance-srta.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/bin/spinproject.py` & `django_spinproject-2.5.0/django_spinproject/bin/spinproject.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,10 +56,14 @@
 
 	elif args.module_to_disable is not None:
 		ProjectInfoManager.disable_module(args.module_to_disable[0])
 
 	elif args.modules_to_upgrade is not None:
 		ProjectInfoManager.upgrade_modules(*args.modules_to_upgrade)
 
+	else:
+		argparser.print_help()
+		argparser.exit(1)
+
 
 if __name__ == '__main__':
 	main()
```

### Comparing `django_spinproject-2.4.0/django_spinproject/cli.py` & `django_spinproject-2.5.0/django_spinproject/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .modules import MODULES
+from .generic.package import Distribution
 
 import argparse
 import textwrap
 
 
 DESCRIPTION = """Opinionated version of django-admin startproject
 that intends to go further and do things that startproject can't do
@@ -67,9 +68,10 @@
 		metavar='MODULE_TO_UPGRADE',
 		help="upgrade all or specified modules. if modules are not specified, then all modules will be upgraded.",
 		action='store',
 		nargs='*',
 		type=str,
 		choices=MODULES.keys(),
 	)
+	parser.add_argument('--version', action='version', version=str(Distribution(parser.prog)))
 
 	return parser
```

### Comparing `django_spinproject-2.4.0/django_spinproject/generic/dicts_merging.py` & `django_spinproject-2.5.0/django_spinproject/generic/dicts_merging.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/generic/directory_cleaning.py` & `django_spinproject-2.5.0/django_spinproject/generic/directory_cleaning.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/generic/extended_jinja_environment.py` & `django_spinproject-2.5.0/django_spinproject/generic/extended_jinja_environment.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/generic/file_upgrade.py` & `django_spinproject-2.5.0/django_spinproject/generic/file_upgrade.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 
 def upgrade_files_content(files_dir: str, expected_content: Dict[str, Sequence[str]], new_content: Dict[str, str]):
 	"""
 	Upgrades content in specified files.
 
 	Args:
-		files_dir: Path to directory where the files should be updated.
+		files_dir: Path to directory where the files should be upgraded.
 		expected_content: Dictionary of expected content in existing files.
 		new_content: Dictionary of new content in all files.
 
 	Raises:
 		ValueError: If at least one file is modified.
 
 	Notes:
-		If the file does not exist during the update, it will be added with the new content.
+		If the file does not exist during the upgrade, it will be added with the new content.
 	"""
 	check_existed_files(files_dir, expected_content)
 
 	if not os.path.exists(files_dir):
 		os.mkdir(files_dir)
 
 	for filename in new_content:
```

### Comparing `django_spinproject-2.4.0/django_spinproject/generic/hash.py` & `django_spinproject-2.5.0/django_spinproject/generic/hash.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/__init__.py` & `django_spinproject-2.5.0/django_spinproject/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/_base.py` & `django_spinproject-2.5.0/django_spinproject/modules/_base.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/_mixins.py` & `django_spinproject-2.5.0/django_spinproject/modules/_mixins.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/docker_scripts.py` & `django_spinproject-2.5.0/django_spinproject/modules/docker_scripts.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/dockerfile_data/v1.py` & `django_spinproject-2.5.0/django_spinproject/modules/dockerfile_data/v1.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/dockerfile_data/v2.py` & `django_spinproject-2.5.0/django_spinproject/modules/dockerfile_data/v2.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/gitignore_data/v1.py` & `django_spinproject-2.5.0/django_spinproject/modules/gitignore_data/v1.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/gitignore_data/v2.py` & `django_spinproject-2.5.0/django_spinproject/modules/gitignore_data/v2.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/gitignore_data/v3.py` & `django_spinproject-2.5.0/django_spinproject/modules/gitignore_data/v3.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/gitignore_data/v4.py` & `django_spinproject-2.5.0/django_spinproject/modules/gitignore_data/v4.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/gitlab_ci.py` & `django_spinproject-2.5.0/django_spinproject/modules/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/gitlab_ci_data/v1.py` & `django_spinproject-2.5.0/django_spinproject/modules/gitlab_ci_data/v1.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/gitlab_ci_data/v2.py` & `django_spinproject-2.5.0/django_spinproject/modules/gitlab_ci_data/v2.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/gitlab_ci_data/v3.py` & `django_spinproject-2.5.0/django_spinproject/modules/gitlab_ci_data/v3.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/pytest.py` & `django_spinproject-2.5.0/django_spinproject/modules/pytest.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/settings.py` & `django_spinproject-2.5.0/django_spinproject/modules/settings.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/settings_data/v1.py` & `django_spinproject-2.5.0/django_spinproject/modules/settings_data/v1.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/settings_data/v2.py` & `django_spinproject-2.5.0/django_spinproject/modules/settings_data/v2.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/srta.py` & `django_spinproject-2.5.0/django_spinproject/modules/srta.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/srta_data/v1.py` & `django_spinproject-2.5.0/django_spinproject/modules/srta_data/v1.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/modules/srta_data/v2.py` & `django_spinproject-2.5.0/django_spinproject/modules/srta_data/v2.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/project_manager/project_info.py` & `django_spinproject-2.5.0/django_spinproject/project_manager/project_info.py`

 * *Files identical despite different names*

### Comparing `django_spinproject-2.4.0/django_spinproject/project_manager/project_info_manager.py` & `django_spinproject-2.5.0/django_spinproject/project_manager/project_info_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,39 +142,39 @@
 		else:
 			modules_to_upgrade = set(modules_to_upgrade)
 			module_names_intersection = set(project_info.modules) & modules_to_upgrade
 			not_enabled_modules = modules_to_upgrade - set(module_names_intersection)
 
 			if not_enabled_modules:
 				exit_with_output(
-					"Some modules are not enabled or don't exist and therefore cannot be updated\n"
+					"Some modules are not enabled or don't exist and therefore cannot be upgraded\n"
 					f"Modules: {','.join(not_enabled_modules)}",
 					1,
 				)
 
 			modules_to_upgrade = module_names_intersection
 
 		for module_name in modules_to_upgrade:
-			_module_version_before_update = project_info.migration_state[module_name]
-			current_module_version = _module_version_before_update
+			_module_version_before_upgrade = project_info.migration_state[module_name]
+			current_module_version = _module_version_before_upgrade
 			module = MODULES[module_name]
 			module_last_version = module.last_version()
 
 			while current_module_version < module_last_version:
 				try:
 					module.upgrade_step(current_module_version, project_info)
 					current_module_version += 1
 					project_info.migration_state[module_name] = current_module_version
 					project_info.save()
 
 				except ValueError as e:
-					exit_with_output(f"Failed to update the module {module_name}. {e}", 1)
+					exit_with_output(f"Failed to upgrade the module {module_name}. {e}", 1)
 
-			if _module_version_before_update != module_last_version:
-				print(f"Successfully upgraded {module_name}: {_module_version_before_update} -> {module_last_version}")
+			if _module_version_before_upgrade != module_last_version:
+				print(f"Successfully upgraded {module_name}: {_module_version_before_upgrade} -> {module_last_version}")
 
 
 ENABLE_MODULE_MESSAGE_TEMPLATE = """Successfully enabled modules: {modules_as_list}
 
 The modules was added to config, but migrations
 were not run. Run them with:
     django-spinproject --upgrade {modules_as_args}"""
```

### Comparing `django_spinproject-2.4.0/pyproject.toml` & `django_spinproject-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-spinproject"
-version = "2.4.0"
+version = "2.5.0"
 description = "Opinionated version of `startproject` with some popular third-party packages. Starter pack includes: whitenoise, django-environ, logging, GitHub Scripts to Rule Them All, basic Dockerfile and Makefile."
 authors = ["m1kc (Max Musatov) <m1kc@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/m1kc/django-spinproject"
 repository = "https://github.com/m1kc/django-spinproject.git"
 documentation = "https://github.com/m1kc/django-spinproject"
```

### Comparing `django_spinproject-2.4.0/setup.py` & `django_spinproject-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 entry_points = \
 {'console_scripts': ['django-spinproject = '
                      'django_spinproject.bin.spinproject:main']}
 
 setup_kwargs = {
     'name': 'django-spinproject',
-    'version': '2.4.0',
+    'version': '2.5.0',
     'description': 'Opinionated version of `startproject` with some popular third-party packages. Starter pack includes: whitenoise, django-environ, logging, GitHub Scripts to Rule Them All, basic Dockerfile and Makefile.',
     'long_description': "# django-spinproject\n\nOpinionated version of `django-admin startproject` that intends to go further and do things that startproject can't do but most people will do anyway. Here's what you get:\n\n* ⚛️ **Whitenoise**: usually you don't need that during local development but one day you're going to deploy your project and find out that it ignores the `static/` folder when running under gunicorn — which is sorta fine because big applications usually serve static files separately via nginx. Smaller apps with small number of assets, however, usually serve them within the same process, which is what whitenoise is for.\n* 🔧 **settings.py**: it's slightly modified to also understand environment variables and `.env` files. This functionality requires the `django-environ` package. Also, app logger is mostly pre-configured for you.\n* 🔒 **Support for marking PostgreSQL databases as read-only**.\n* 🧰 `script/bootstrap` and other [scripts to rule them all](https://github.blog/2015-06-30-scripts-to-rule-them-all/) so your fellow developers and maintainers don't ask you how to run this thing. Current versions of these scripts optimized for use with [poetry](https://python-poetry.org/), but you can easily adapt them for any Python package manager.\n* 🏗️ **Dockerfile and .dockerignore**: one day your app will go to production, and we've got you covered.\n* 🏛️ **Gitlab CI config**: CI is a good thing.\n* ⚕️ **Pre-configured linter** so you can find some common problems automagically.\n* 🏃 **Pre-configured pytest** because you are going to need unit tests one day.\n* 🗃️ **Auto-checks if you forgot to create migrations** whenever you run tests or CI.\n* *️⃣ **.gitignore**: well, you know why.\n\n## Requirements\n\n* \\*nix system;\n* `django-admin` installed and available from `$PATH`.\n\nGenerated files will work fine in Django >= 2.0, not tested in earlier versions.\n\n## How to use\n\n* Install the package: `pip install django-spinproject`\n* Create a new project: `django-spinproject --create <path>`\n* OR initialize spinproject in your existing project's folder: `django-spinproject --init`\n\nYou're all set. Now you can take a look at the list of available modules: `django-spinproject --help`\n\nUse `django-spinproject --enable` to enable a module, `django-spinproject --upgrade` to apply changes.\n\n## Other commands\n\n* `--create PATH`: create django project in specified path \n* `--init`: create spinproject.json file\n* `--enable MODULE_TO_ENABLE [MODULE_TO_ENABLE ...]`: enable specified module(s). use 'all' to enable all modules\n* `--disable MODULE_TO_DISABLE`: disable specified module\n* `--upgrade [MODULE_TO_UPGRADE [MODULE_TO_UPGRADE ...]]`: upgrade (specified or all) enabled modules\n\n## Available modules\n\n* `gitignore` — Creates `.gitignore` file suitable for most Django projects.\n* `srta` — Creates [Scripts to Rule Them All](https://github.blog/2015-06-30-scripts-to-rule-them-all/) (simplifies life a lot, you should check it out).\n* `pytest` — Creates `pytest.ini` and `.coveragerc` files.\n* `dockerfile` — Creates a Dockerfile.\n* `dockerignore` — Creates `.dockerignore` (you should totally do that).\n* `docker-scripts` — Creates additional SRTA scripts for building and pushing your Docker image.\n* `gitlab-ci` — Creates GitLab CI config, `.gitlab-ci.yml`.\n* `pg-readonly` — Creates a DatabaseWrapper class for readonly connection to PostgreSQL.\n* `settings` — Improves the default `settings.py`, adding support for envvars and `.env` files. Also enables Whitenoise and CLI logger.\n\n## Planned features\n\n(for requests, create an issue or drop me a line at m1kc@yandex.ru)\n\n* login page template (see `experimental` branch)\n\n## Changelog\n\nSee the [Releases](https://github.com/m1kc/django-spinproject/releases) page.\n",
     'author': 'm1kc (Max Musatov)',
     'author_email': 'm1kc@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/m1kc/django-spinproject',
```

### Comparing `django_spinproject-2.4.0/PKG-INFO` & `django_spinproject-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-spinproject
-Version: 2.4.0
+Version: 2.5.0
 Summary: Opinionated version of `startproject` with some popular third-party packages. Starter pack includes: whitenoise, django-environ, logging, GitHub Scripts to Rule Them All, basic Dockerfile and Makefile.
 Home-page: https://github.com/m1kc/django-spinproject
 License: MIT
 Keywords: django,django-admin,startproject,template,whitenoise,django-environ,SRTA
 Author: m1kc (Max Musatov)
 Author-email: m1kc@yandex.ru
 Requires-Python: >=3.7,<4.0
```


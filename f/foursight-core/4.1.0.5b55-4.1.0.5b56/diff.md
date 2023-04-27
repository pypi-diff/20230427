# Comparing `tmp/foursight_core-4.1.0.5b55.tar.gz` & `tmp/foursight_core-4.1.0.5b56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.1.0.5b55.tar", max compression
+gzip compressed data, was "foursight_core-4.1.0.5b56.tar", max compression
```

## Comparing `foursight_core-4.1.0.5b55.tar` & `foursight_core-4.1.0.5b56.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-04-27 03:08:07.496060 foursight_core-4.1.0.5b55/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/app.py
--rw-r--r--   0        0        0   105729 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4452 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5146 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-04-27 03:08:07.504060 foursight_core-4.1.0.5b55/foursight_core/package.py
--rw-r--r--   0        0        0    17191 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     7608 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    23203 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6315 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28316 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20652 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4876 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3257 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9524 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5164 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    79112 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11353 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    32676 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4861 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-04-27 03:08:07.508060 foursight_core-4.1.0.5b55/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1927376 2023-04-27 03:08:07.516060 foursight_core-4.1.0.5b55/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-04-27 03:08:07.516060 foursight_core-4.1.0.5b55/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1613 2023-04-27 03:08:07.520060 foursight_core-4.1.0.5b55/pyproject.toml
--rw-r--r--   0        0        0     1199 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b55/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-27 12:43:29.950014 foursight_core-4.1.0.5b56/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-04-27 12:43:29.954014 foursight_core-4.1.0.5b56/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-04-27 12:43:29.954014 foursight_core-4.1.0.5b56/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-04-27 12:43:29.954014 foursight_core-4.1.0.5b56/foursight_core/app.py
+-rw-r--r--   0        0        0   105729 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4452 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5146 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/package.py
+-rw-r--r--   0        0        0    17191 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     7608 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    23203 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6315 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28316 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20652 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4876 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3257 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9524 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5164 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    79112 2023-04-27 12:43:29.958014 foursight_core-4.1.0.5b56/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11353 2023-04-27 12:43:29.962014 foursight_core-4.1.0.5b56/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-04-27 12:43:29.962014 foursight_core-4.1.0.5b56/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    32676 2023-04-27 12:43:29.962014 foursight_core-4.1.0.5b56/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4861 2023-04-27 12:43:29.962014 foursight_core-4.1.0.5b56/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-04-27 12:43:29.962014 foursight_core-4.1.0.5b56/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-04-27 12:43:29.962014 foursight_core-4.1.0.5b56/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-04-27 12:43:29.962014 foursight_core-4.1.0.5b56/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-04-27 12:43:29.962014 foursight_core-4.1.0.5b56/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-04-27 12:43:29.962014 foursight_core-4.1.0.5b56/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1927376 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1613 2023-04-27 12:43:29.974014 foursight_core-4.1.0.5b56/pyproject.toml
+-rw-r--r--   0        0        0     1199 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b56/PKG-INFO
```

### Comparing `foursight_core-4.1.0.5b55/LICENSE.txt` & `foursight_core-4.1.0.5b56/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/abstract_connection.py` & `foursight_core-4.1.0.5b56/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/app_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/buckets.py` & `foursight_core-4.1.0.5b56/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/check_schema.py` & `foursight_core-4.1.0.5b56/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/check_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.1.0.5b56/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.1.0.5b56/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/checks/ecs_checks.py` & `foursight_core-4.1.0.5b56/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.1.0.5b56/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/checks/scaling_checks.py` & `foursight_core-4.1.0.5b56/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/checks/test_checks.py` & `foursight_core-4.1.0.5b56/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/decorators.py` & `foursight_core-4.1.0.5b56/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/deploy.py` & `foursight_core-4.1.0.5b56/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/environment.py` & `foursight_core-4.1.0.5b56/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/es_connection.py` & `foursight_core-4.1.0.5b56/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/exceptions.py` & `foursight_core-4.1.0.5b56/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/fs_connection.py` & `foursight_core-4.1.0.5b56/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/identity.py` & `foursight_core-4.1.0.5b56/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/mapping.json` & `foursight_core-4.1.0.5b56/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/package.py` & `foursight_core-4.1.0.5b56/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/auth.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/auth0_config.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/aws_network.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/aws_s3.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/checks.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/cognito.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/encryption.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/envs.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/gac.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/misc_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/react_api.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/react_api.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/react_api_base.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/react_routes.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/react_ui.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/ui/index.html` & `foursight_core-4.1.0.5b56/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.1.0.5b56/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.1.0.5b56/foursight_core/react/ui/static/js/main.js`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/route_prefixes.py` & `foursight_core-4.1.0.5b56/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/routes.py` & `foursight_core-4.1.0.5b56/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/run_result.py` & `foursight_core-4.1.0.5b56/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/s3_connection.py` & `foursight_core-4.1.0.5b56/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/schedule_decorator.py` & `foursight_core-4.1.0.5b56/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.1.0.5b56/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.1.0.5b56/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/sqs_utils.py` & `foursight_core-4.1.0.5b56/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/stage.py` & `foursight_core-4.1.0.5b56/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/templates/base.html` & `foursight_core-4.1.0.5b56/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/templates/header.html` & `foursight_core-4.1.0.5b56/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/templates/history.html` & `foursight_core-4.1.0.5b56/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/templates/info.html` & `foursight_core-4.1.0.5b56/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/templates/unused.html` & `foursight_core-4.1.0.5b56/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/templates/user.html` & `foursight_core-4.1.0.5b56/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/templates/users.html` & `foursight_core-4.1.0.5b56/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/templates/view_checks.html` & `foursight_core-4.1.0.5b56/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/foursight_core/templates/view_groups.html` & `foursight_core-4.1.0.5b56/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b55/pyproject.toml` & `foursight_core-4.1.0.5b56/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.1.0.5b55"
+version = "4.1.0.5b56"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.10"
 click = "^7.1.2"
 cron-descriptor = "^1.2.31"
 cryptography = "39.0.2" # Required for AWS Cognito JWT decode (PyJWKClient)
-dcicutils = "7.3.0.1b39"
+dcicutils = "7.3.0.1b41"
 elasticsearch = "7.13.4"
 elasticsearch-dsl = "^7.0.0"
 geocoder = "1.38.1"
 gitpython = "^3.1.2"
 google = "^3.0.0"
 google-auth-oauthlib = "^0.7.0"
 google-api-python-client = "^1.12.5"
```

### Comparing `foursight_core-4.1.0.5b55/PKG-INFO` & `foursight_core-4.1.0.5b56/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.1.0.5b55
+Version: 4.1.0.5b56
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: cron-descriptor (>=1.2.31,<2.0.0)
 Requires-Dist: cryptography (==39.0.2)
-Requires-Dist: dcicutils (==7.3.0.1b39)
+Requires-Dist: dcicutils (==7.3.0.1b41)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: google-auth-oauthlib (>=0.7.0,<0.8.0)
```


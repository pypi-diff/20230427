# Comparing `tmp/foursight_core-4.1.0.5b51.tar.gz` & `tmp/foursight_core-4.1.0.5b54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.1.0.5b51.tar", max compression
+gzip compressed data, was "foursight_core-4.1.0.5b54.tar", max compression
```

## Comparing `foursight_core-4.1.0.5b51.tar` & `foursight_core-4.1.0.5b54.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-04-26 14:15:59.652887 foursight_core-4.1.0.5b51/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/app.py
--rw-r--r--   0        0        0   105729 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4452 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5146 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/package.py
--rw-r--r--   0        0        0    17191 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     7608 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    23203 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6315 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28316 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20652 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3456 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4876 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3257 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9524 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5200 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    78139 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11353 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    32676 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4861 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1927239 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1609 2023-04-26 14:15:59.676888 foursight_core-4.1.0.5b51/pyproject.toml
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b51/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-27 02:47:39.057521 foursight_core-4.1.0.5b54/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/app.py
+-rw-r--r--   0        0        0   105729 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4452 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5146 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/package.py
+-rw-r--r--   0        0        0    17191 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     7608 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    23203 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6315 2023-04-27 02:47:39.065521 foursight_core-4.1.0.5b54/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28316 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20652 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4876 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3257 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9524 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5164 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    79112 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11353 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    32676 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4861 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-04-27 02:47:39.069521 foursight_core-4.1.0.5b54/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1927376 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1613 2023-04-27 02:47:39.081521 foursight_core-4.1.0.5b54/pyproject.toml
+-rw-r--r--   0        0        0     1199 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b54/PKG-INFO
```

### Comparing `foursight_core-4.1.0.5b51/LICENSE.txt` & `foursight_core-4.1.0.5b54/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/abstract_connection.py` & `foursight_core-4.1.0.5b54/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/app_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/buckets.py` & `foursight_core-4.1.0.5b54/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/check_schema.py` & `foursight_core-4.1.0.5b54/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/check_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.1.0.5b54/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.1.0.5b54/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/checks/ecs_checks.py` & `foursight_core-4.1.0.5b54/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.1.0.5b54/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/checks/scaling_checks.py` & `foursight_core-4.1.0.5b54/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/checks/test_checks.py` & `foursight_core-4.1.0.5b54/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/decorators.py` & `foursight_core-4.1.0.5b54/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/deploy.py` & `foursight_core-4.1.0.5b54/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/environment.py` & `foursight_core-4.1.0.5b54/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/es_connection.py` & `foursight_core-4.1.0.5b54/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/exceptions.py` & `foursight_core-4.1.0.5b54/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/fs_connection.py` & `foursight_core-4.1.0.5b54/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/identity.py` & `foursight_core-4.1.0.5b54/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/mapping.json` & `foursight_core-4.1.0.5b54/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/package.py` & `foursight_core-4.1.0.5b54/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/auth.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/auth0_config.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/aws_network.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/aws_s3.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/checks.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/cognito.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/cookie_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,18 +19,29 @@
         return ""
     simple_cookies = _read_cookies(request)
     cookie_morsel = simple_cookies.get(cookie_name) if simple_cookies else None
     return cookie_morsel.value if cookie_morsel else None
 
 
 def read_cookie_bool(request: dict, cookie_name: str) -> bool:
-    return str_to_bool(read_cookie(request, cookie_name))
+    """
+    Returns the value of the cookie of the given name from within the given request,
+    as a bool (per dcicutils.str_to_bool), or False if the cookie does not exist
+    or is not a value True specifier.
+    """
+    result = str_to_bool(read_cookie(request, cookie_name))
+    return True if result else False
 
 
 def read_cookie_int(request: dict, cookie_name: str, default: int = 0) -> int:
+    """
+    Returns the value of the cookie of the given name from within the given request,
+    as an integer, or the given default value (which defaults to 0) if the cookie
+    does not exist or is not a value a valid integer.
+    """
     value = read_cookie(request, cookie_name)
     if not value:
         return default
     if value.startswith("-"):
         value = value[1:]
         multiplier = -1
     else:
```

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/encryption.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/envs.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/gac.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/misc_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/portal_access_key_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,18 +19,18 @@
     try:
         now = datetime.now(pytz.utc)
         connection = app.core.init_connection(env)
         connection_keys = connection.ff_keys
         key = connection_keys.get("key")
         if key and not logged_in:
             # This logged_in flag is passed from caller (react_api.reactapi_portal_access_key)
-            # and is False iff the user is NOT logged in; so if logged in then we do NOT obfuscate
-            # the access key (ID) but if we ARE not logged in we just see the first letter of it.
-            # And of course we do not return a value for any part of the secret at all, ever.
-            key = key[0] + "*******"
+            # and is False iff the user is NOT logged in; so if logged in then we do NOT
+            # obfuscate the access key (ID) but if we are NOT logged in we do obfuscate it.
+            # And of course we do not return any part of the secret at all, ever.
+            key = "********"
         server = connection_keys.get("server")
         access_key_info = {"key": key, "secret": "********", "server": server, "logged_in": logged_in}
         access_key_create_date, access_key_expires_date, access_key_expires_exception = \
             _get_portal_access_key_expires_date(connection_keys)
         if access_key_expires_date:
             access_key_info["created_at"] = access_key_create_date.strftime("%Y-%m-%d %H:%M:%S")
             if access_key_expires_date == datetime.max:
```

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/react_api.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/react_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,14 +379,34 @@
                 "global_env_bucket": os.environ.get("GLOBAL_ENV_BUCKET", os.environ.get("GLOBAL_BUCKET_ENV", None)),
                 "encrypt_key_id": os.environ.get("S3_ENCRYPT_KEY_ID", None)
             }
         }
         return response
 
     def reactapi_certificates(self, request: dict, args: Optional[dict] = None) -> Response:
+        """
+        Called from react_routes for endpoint: GET /certificates
+        Called from react_routes for endpoint: GET /{env}/certificates
+        Note that this in an UNPROTECTED route.
+
+        Returns a dictionary with pertinent publicly available information about the
+        SSL certificate for this Foursight instance and the associated Portal instance.
+        Of, if a hostname (or hostnames) URL argument is given, then instead returns
+        SSL certificate info for the specified (comma-separated) list of hostnames.
+
+        Here are the data points (properties) of the returned dictionary:
+
+        active_at    issuer           owner_country
+        exception    issuer_city      owner_entity
+        expired      issuer_country   owner_state
+        expires_at   issuer_entity    pem
+        hostname     issuer_state     public_key_pem
+        hostnames    owner            serial_number
+        inactive     owner_city       invalid
+        """
         hostnames = args.get("hostname", args.get("hostnames", None))
         response = []
         if hostnames and hostnames.lower() != "null":
             for hostname in hostnames.split(","):
                 certificate = get_ssl_certificate_info(hostname.strip())
                 if certificate:
                     response.append(certificate)
```

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/react_api_base.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/react_routes.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/react_ui.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/ui/index.html` & `foursight_core-4.1.0.5b54/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.1.0.5b54/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.1.0.5b54/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.faf78e31.js.LICENSE.txt */
+/*! For license information please see main.59afd838.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             4189: function(e, t) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -49298,23 +49298,32 @@
                                 })]
                             }), (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: s,
                                     children: "Access Key:"
                                 }), (0, Kr.jsxs)("td", {
                                     style: i,
-                                    children: [r.key, Br.IsLoggedIn(n) && (0, Kr.jsxs)(Kr.Fragment, {
-                                        children: ["\xa0\xa0", Fr.RightArrow, "\xa0\xa0", (0, Kr.jsx)("a", {
+                                    children: [r.key, "\xa0\xa0", Fr.RightArrow, "\xa0\xa0", Br.IsLoggedIn(n) ? (0, Kr.jsx)(Kr.Fragment, {
+                                        children: (0, Kr.jsx)("a", {
                                             href: "".concat(r.server, "/access-keys/").concat(r.key, "/"),
                                             style: {
                                                 color: o
                                             },
                                             target: "_blank",
                                             children: "View"
-                                        })]
+                                        })
+                                    }) : (0, Kr.jsx)(Kr.Fragment, {
+                                        children: (0, Kr.jsx)("a", {
+                                            href: "".concat(r.server, "/access-keys"),
+                                            style: {
+                                                color: o
+                                            },
+                                            target: "_blank",
+                                            children: "View"
+                                        })
                                     })]
                                 })]
                             }), (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: s,
                                     children: "Creation Date:"
                                 }), (0, Kr.jsxs)("td", {
```

### Comparing `foursight_core-4.1.0.5b51/foursight_core/route_prefixes.py` & `foursight_core-4.1.0.5b54/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/routes.py` & `foursight_core-4.1.0.5b54/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/run_result.py` & `foursight_core-4.1.0.5b54/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/s3_connection.py` & `foursight_core-4.1.0.5b54/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/schedule_decorator.py` & `foursight_core-4.1.0.5b54/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.1.0.5b54/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.1.0.5b54/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/sqs_utils.py` & `foursight_core-4.1.0.5b54/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/stage.py` & `foursight_core-4.1.0.5b54/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/templates/base.html` & `foursight_core-4.1.0.5b54/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/templates/header.html` & `foursight_core-4.1.0.5b54/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/templates/history.html` & `foursight_core-4.1.0.5b54/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/templates/info.html` & `foursight_core-4.1.0.5b54/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/templates/unused.html` & `foursight_core-4.1.0.5b54/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/templates/user.html` & `foursight_core-4.1.0.5b54/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/templates/users.html` & `foursight_core-4.1.0.5b54/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/templates/view_checks.html` & `foursight_core-4.1.0.5b54/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/foursight_core/templates/view_groups.html` & `foursight_core-4.1.0.5b54/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b51/pyproject.toml` & `foursight_core-4.1.0.5b54/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.1.0.5b51"
+version = "4.1.0.5b54"
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
-dcicutils = "7.3.0.1b36"
+dcicutils = "7.3.0.1b38"
 elasticsearch = "7.13.4"
 elasticsearch-dsl = "^7.0.0"
 geocoder = "1.38.1"
 gitpython = "^3.1.2"
 google = "^3.0.0"
 google-auth-oauthlib = "^0.7.0"
 google-api-python-client = "^1.12.5"
@@ -29,15 +29,15 @@
 # TODO: I think this can update to ">=1.1.1,<3" so that it can move to version 2.x.
 #       Doing so will mean adjusting the Jinja2 constraint as well. -kmp 23-Feb-2023
 MarkupSafe = "1.1.1"
 pyDes = "^2.0.1"
 PyJWT = "^2.5.0"
 pytz = ">=2020.1"
 redis = "^4.5.1"
-toml = "^0.10.2"
+toml = ">=0.10.2,<1"
 
 [tool.poetry.dev-dependencies]
 chalice = "^1.21.4"
 flake8 = ">=3.9.2"
 flaky = "3.6.1"
 pytest = "5.1.2"
 pytest-cov = "2.7.1"
```

### Comparing `foursight_core-4.1.0.5b51/PKG-INFO` & `foursight_core-4.1.0.5b54/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.1.0.5b51
+Version: 4.1.0.5b54
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,19 +13,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: cron-descriptor (>=1.2.31,<2.0.0)
 Requires-Dist: cryptography (==39.0.2)
-Requires-Dist: dcicutils (==7.3.0.1b36)
+Requires-Dist: dcicutils (==7.3.0.1b38)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: google-auth-oauthlib (>=0.7.0,<0.8.0)
 Requires-Dist: pyDes (>=2.0.1,<3.0.0)
 Requires-Dist: pytz (>=2020.1)
 Requires-Dist: redis (>=4.5.1,<5.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: toml (>=0.10.2,<1)
```


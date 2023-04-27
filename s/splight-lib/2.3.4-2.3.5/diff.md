# Comparing `tmp/splight-lib-2.3.4.tar.gz` & `tmp/splight-lib-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-2.3.4.tar", last modified: Tue Apr 25 15:01:42 2023, max compression
+gzip compressed data, was "splight-lib-2.3.5.tar", last modified: Thu Apr 27 17:25:12 2023, max compression
```

## Comparing `splight-lib-2.3.4.tar` & `splight-lib-2.3.5.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.327626 splight-lib-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:41.000000 splight-lib-2.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-25 15:01:42.327626 splight-lib-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-25 15:01:41.000000 splight-lib-2.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.315625 splight-lib-2.3.4/remote_splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.315625 splight-lib-2.3.4/remote_splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.315625 splight-lib-2.3.4/remote_splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/communication/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.315625 splight-lib-2.3.4/remote_splight_lib/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/database/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.315625 splight-lib-2.3.4/remote_splight_lib/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/datalake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/remote_splight_lib/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:01:42.327626 splight-lib-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-25 15:01:41.000000 splight-lib-2.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/auth/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/cache/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/client/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/client/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/client/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/communication/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/database/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/database/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/datalake/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/deployment/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/hub/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/notification/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/notification/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/remote/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/storage/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26067 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.327626 splight-lib-2.3.4/splight_models/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.327626 splight-lib-2.3.4/splight_models/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/communication/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/communication/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/datalake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/setpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.077466 splight-lib-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:10.000000 splight-lib-2.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-27 17:25:12.077466 splight-lib-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 17:25:10.000000 splight-lib-2.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.069466 splight-lib-2.3.5/remote_splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.069466 splight-lib-2.3.5/remote_splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/remote_splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/communication/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/remote_splight_lib/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/database/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/remote_splight_lib/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/datalake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/remote_splight_lib/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-27 17:25:10.000000 splight-lib-2.3.5/remote_splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:25:12.077466 splight-lib-2.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-27 17:25:10.000000 splight-lib-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/auth/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/cache/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/client/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/client/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/communication/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/database/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/datalake/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/deployment/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/hub/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/notification/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/remote/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_abstract/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_abstract/storage/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.077466 splight-lib-2.3.5/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.077466 splight-lib-2.3.5/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/client/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.077466 splight-lib-2.3.5/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27556 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.077466 splight-lib-2.3.5/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.077466 splight-lib-2.3.5/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.073466 splight-lib-2.3.5/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-27 17:25:12.000000 splight-lib-2.3.5/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-27 17:25:12.000000 splight-lib-2.3.5/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:25:12.000000 splight-lib-2.3.5/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:25:12.000000 splight-lib-2.3.5/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-27 17:25:12.000000 splight-lib-2.3.5/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 17:25:12.000000 splight-lib-2.3.5/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.077466 splight-lib-2.3.5/splight_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:25:12.077466 splight-lib-2.3.5/splight_models/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/communication/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/communication/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/datalake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/setpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-27 17:25:10.000000 splight-lib-2.3.5/splight_models/webhook.py
```

### Comparing `splight-lib-2.3.4/PKG-INFO` & `splight-lib-2.3.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.3.4
+Version: 2.3.5
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-2.3.4/remote_splight_lib/communication/client.py` & `splight-lib-2.3.5/remote_splight_lib/communication/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/remote_splight_lib/database/classmap.py` & `splight-lib-2.3.5/remote_splight_lib/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/remote_splight_lib/database/client.py` & `splight-lib-2.3.5/remote_splight_lib/database/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/remote_splight_lib/datalake/client.py` & `splight-lib-2.3.5/remote_splight_lib/datalake/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/remote_splight_lib/hub/client.py` & `splight-lib-2.3.5/remote_splight_lib/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/remote_splight_lib/settings.py` & `splight-lib-2.3.5/remote_splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/setup.py` & `splight-lib-2.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="2.3.4",
+    version="2.3.5",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-2.3.4/splight_abstract/auth/abstract.py` & `splight-lib-2.3.5/splight_abstract/auth/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/auth/exceptions.py` & `splight-lib-2.3.5/splight_abstract/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/cache/abstract.py` & `splight-lib-2.3.5/splight_abstract/cache/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/client/abstract.py` & `splight-lib-2.3.5/splight_abstract/client/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/client/filter.py` & `splight-lib-2.3.5/splight_abstract/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/client/hooks.py` & `splight-lib-2.3.5/splight_abstract/client/hooks.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/communication/abstract.py` & `splight-lib-2.3.5/splight_abstract/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/database/abstract.py` & `splight-lib-2.3.5/splight_abstract/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/datalake/abstract.py` & `splight-lib-2.3.5/splight_abstract/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/deployment/abstract.py` & `splight-lib-2.3.5/splight_abstract/deployment/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/endpoints/__init__.py` & `splight-lib-2.3.5/splight_abstract/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/hub/abstract.py` & `splight-lib-2.3.5/splight_abstract/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_abstract/storage/abstract.py` & `splight-lib-2.3.5/splight_abstract/storage/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/auth/mac_auth.py` & `splight-lib-2.3.5/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/client/database/classmap.py` & `splight-lib-2.3.5/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/client/database/local_client.py` & `splight-lib-2.3.5/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/client/database/remote_client.py` & `splight-lib-2.3.5/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/client/datalake/local_client.py` & `splight-lib-2.3.5/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/client/datalake/remote_client.py` & `splight-lib-2.3.5/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/client/exceptions.py` & `splight-lib-2.3.5/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/client/file_handler.py` & `splight-lib-2.3.5/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/client/filter.py` & `splight-lib-2.3.5/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/client/settings.py` & `splight-lib-2.3.5/splight_lib/client/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/component/abstract.py` & `splight-lib-2.3.5/splight_lib/component/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 import uuid
 from abc import abstractmethod
 from collections import defaultdict
 from functools import cached_property, partial
 from tempfile import NamedTemporaryFile
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
+from retry import retry
 
 import splight_models as spmodels
 from mergedeep import Strategy as mergeStrategy
 from mergedeep import merge
 from pydantic import BaseModel, main
 from splight_lib.execution import ExecutionClient, Thread
 from splight_lib.logging._internal import LogTags, get_splight_logger
@@ -42,16 +43,25 @@
 from splight_models.setpoint import (
     SetPoint,
     SetPointCreateEvent,
     SetPointResponse,
     SetPointResponseStatus,
     SetPointUpdateEvent,
 )
+from remote_splight_lib.auth import SplightAuthToken
+from splight_lib.restclient import (
+    ConnectError,
+    HTTPError,
+    SplightRestClient,
+    Timeout,
+)
+from remote_splight_lib.settings import settings as remote_settings
 
 logger = get_splight_logger()
+REQUEST_EXCEPTIONS = (HTTPError, Timeout, ConnectError)
 
 
 class SecretValueParser:
     def __init__(self, utils, *args, **kwargs):
         self.utils = utils
 
     def get_value(self, name: str) -> Any:
@@ -636,14 +646,18 @@
                     [self._transform_parameters(val) for val in value]
                     if multiple
                     else self._transform_parameters(value)
                 )
         return parameters_dict
 
 
+class DuplicatedComponentException(Exception):
+    pass
+
+
 class AbstractComponent(
     RunnableMixin,
     HooksMixin,
     IndexMixin,
     BindingsMixin,
     ParametersMixin,
     VariableValueMixin,
@@ -668,14 +682,15 @@
 
         self.namespace = self._setup.settings.NAMESPACE
         self.instance_type = Component
         self.instance_id = component_id if component_id else str(uuid.uuid4())
         self.deployment_id = run_spec.pop("id", None)
 
         self._spec: Deployment = Deployment(id=self.instance_id, **run_spec)
+        self._check_duplicated_component()
         self._load_instance_kwargs_for_clients()
         self._load_clients(
             database_config=kwargs.get("database_config", {}),
             datalake_config=kwargs.get("datalake_config", {}),
         )
         self._load_spec_models()
         self._load_input_model()
@@ -721,7 +736,31 @@
         self.datalake_client = self.setup.DATALAKE_CLIENT(
             namespace=self.namespace, **datalake_config
         )
         self.communication_client = self.setup.COMMUNICATION_CLIENT(
             namespace=self.namespace, **self.communication_client_kwargs
         )
         self.execution_client = ExecutionClient(namespace=self.namespace)
+
+    @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
+    def _check_duplicated_component(self):
+        """
+            Validates that there are no other connections to communication client
+        """
+        token = SplightAuthToken(
+            access_key=remote_settings.SPLIGHT_ACCESS_ID,
+            secret_key=remote_settings.SPLIGHT_SECRET_KEY,
+        )
+        rest_client = SplightRestClient()
+        rest_client.update_headers(token.header)
+        api_url = f"{remote_settings.SPLIGHT_PLATFORM_API_HOST}/v2/engine/component/components/{self.instance_id}/connections/"
+        response = rest_client.get(api_url)
+        if response.status_code == 200:
+            connections = response.json()['subscription_count']
+            if int(connections) > 0:
+                raise DuplicatedComponentException(
+                    f"Component with id {self.instance_id} is already running."
+                )
+        else:
+            raise Exception(
+                f"Error checking if component is already running. Status: {response.status_code}"
+            )
```

### Comparing `splight-lib-2.3.4/splight_lib/encryption.py` & `splight-lib-2.3.5/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/execution.py` & `splight-lib-2.3.5/splight_lib/execution.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/logging/_internal.py` & `splight-lib-2.3.5/splight_lib/logging/_internal.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/logging/component.py` & `splight-lib-2.3.5/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/logging/logging.py` & `splight-lib-2.3.5/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/restclient/client.py` & `splight-lib-2.3.5/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/restclient/exceptions.py` & `splight-lib-2.3.5/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/restclient/types.py` & `splight-lib-2.3.5/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/settings.py` & `splight-lib-2.3.5/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib/webhook.py` & `splight-lib-2.3.5/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_lib.egg-info/PKG-INFO` & `splight-lib-2.3.5/splight_lib.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.3.4
+Version: 2.3.5
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-2.3.4/splight_lib.egg-info/SOURCES.txt` & `splight-lib-2.3.5/splight_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/__init__.py` & `splight-lib-2.3.5/splight_models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/alert.py` & `splight-lib-2.3.5/splight_models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/asset.py` & `splight-lib-2.3.5/splight_models/asset.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     external_id: Optional[str]
     latitude: Optional[float]
     longitude: Optional[float]
     tags: List[str] = []
     attributes: List[Attribute] = []
     verified: bool = False
     geometry: Optional[GeometryCollection]
-    centroid_coordinates: Optional[Tuple[float]]
+    centroid_coordinates: Optional[Tuple[float, float]]
```

### Comparing `splight-lib-2.3.4/splight_models/base.py` & `splight-lib-2.3.5/splight_models/base.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/blockchain.py` & `splight-lib-2.3.5/splight_models/blockchain.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/communication/context.py` & `splight-lib-2.3.5/splight_models/communication/context.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/communication/events.py` & `splight-lib-2.3.5/splight_models/communication/events.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/component.py` & `splight-lib-2.3.5/splight_models/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/constants.py` & `splight-lib-2.3.5/splight_models/constants.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/datalake.py` & `splight-lib-2.3.5/splight_models/datalake.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/deployment.py` & `splight-lib-2.3.5/splight_models/deployment.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/exception.py` & `splight-lib-2.3.5/splight_models/exception.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/file.py` & `splight-lib-2.3.5/splight_models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/hub.py` & `splight-lib-2.3.5/splight_models/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/notification.py` & `splight-lib-2.3.5/splight_models/notification.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/query.py` & `splight-lib-2.3.5/splight_models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/setpoint.py` & `splight-lib-2.3.5/splight_models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/user.py` & `splight-lib-2.3.5/splight_models/user.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/variable.py` & `splight-lib-2.3.5/splight_models/variable.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.4/splight_models/webhook.py` & `splight-lib-2.3.5/splight_models/webhook.py`

 * *Files identical despite different names*


# Comparing `tmp/dapr-dev-1.9.0rc1.dev1489.tar.gz` & `tmp/dapr-dev-1.9.0rc1.dev1502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-dev-1.9.0rc1.dev1489.tar", last modified: Thu Apr 20 19:54:18 2023, max compression
+gzip compressed data, was "dist/dapr-dev-1.9.0rc1.dev1502.tar", last modified: Thu Apr 27 19:57:46 2023, max compression
```

## Comparing `dapr-dev-1.9.0rc1.dev1489.tar` & `dapr-dev-1.9.0rc1.dev1502.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/actor_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/client/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/client/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_call_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_method_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_reminder_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_state_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_timer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_type_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/method_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/reentrancy_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/remindable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/state_change.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/state_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/_asynchelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    48922 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    30396 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    48045 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/dapr_actor_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/dapr_invocation_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/conf/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/appcallback_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/appcallback_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    71113 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/dapr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    57502 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/dapr_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/serializers/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/version/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/version/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-20 19:54:17.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:54:17.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:54:17.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 19:54:17.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 19:54:17.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/actor_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/client/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_call_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_method_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_reminder_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_state_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_timer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_type_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/method_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/reentrancy_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/remindable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/state_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/state_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/aio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/aio/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/aio/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/aio/clients/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/aio/clients/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/aio/clients/grpc/_asynchelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48453 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/aio/clients/grpc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30396 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47653 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/http/dapr_actor_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/clients/http/dapr_invocation_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/conf/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/common/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/common/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/common/v1/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/common/v1/common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/v1/appcallback_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/v1/appcallback_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86347 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/v1/dapr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81978 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/v1/dapr_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/serializers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr/version/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/dapr/version/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-27 19:57:45.000000 dapr-dev-1.9.0rc1.dev1502/dapr_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/dapr_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:57:45.000000 dapr-dev-1.9.0rc1.dev1502/dapr_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:57:45.000000 dapr-dev-1.9.0rc1.dev1502/dapr_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 19:57:45.000000 dapr-dev-1.9.0rc1.dev1502/dapr_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 19:57:45.000000 dapr-dev-1.9.0rc1.dev1502/dapr_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-27 19:57:46.000000 dapr-dev-1.9.0rc1.dev1502/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-27 19:57:28.000000 dapr-dev-1.9.0rc1.dev1502/setup.py
```

### Comparing `dapr-dev-1.9.0rc1.dev1489/LICENSE` & `dapr-dev-1.9.0rc1.dev1502/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/PKG-INFO` & `dapr-dev-1.9.0rc1.dev1502/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-dev
-Version: 1.9.0rc1.dev1489
+Version: 1.9.0rc1.dev1502
 Summary: The developmental release for Dapr Python SDK.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-dev-1.9.0rc1.dev1489/README.md` & `dapr-dev-1.9.0rc1.dev1502/README.md`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/actor_interface.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/actor_interface.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/client/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/client/proxy.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/client/proxy.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/id.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/id.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_call_type.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_call_type.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_method_context.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_method_context.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_reminder_data.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_reminder_data.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_state_provider.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_state_provider.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_timer_data.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_timer_data.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_type_information.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_type_information.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_type_utils.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/_type_utils.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/actor.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/actor.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/config.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/config.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/context.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/context.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/manager.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/manager.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/method_dispatcher.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/method_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/reentrancy_context.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/reentrancy_context.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/remindable.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/remindable.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/runtime.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/state_change.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/state_change.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/state_manager.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/actor/runtime/state_manager.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/aio/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/aio/clients/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/_asynchelpers.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/aio/clients/grpc/_asynchelpers.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/client.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/aio/clients/grpc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,17 +144,14 @@
         self._stub = api_service_v1.DaprStub(self._channel)
 
     async def close(self):
         """Closes Dapr runtime gRPC channel."""
         if self._channel:
             self._channel.close()
 
-    async def __del__(self):
-        await self.close()
-
     async def __aenter__(self) -> Self:  # type: ignore
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
         await self.close()
 
     def _get_http_extension(
@@ -921,42 +918,40 @@
             headers=await call.initial_metadata())
 
     async def get_configuration(
             self,
             store_name: str,
             keys: List[str],
             config_metadata: Optional[Dict[str, str]] = dict()) -> ConfigurationResponse:
-        """Gets value from a config store with a key
+        """Gets values from a config store with keys
 
         The example gets value from a config store:
             from dapr.aio.clients import DaprClient
             async with DaprClient() as d:
                 resp = await d.get_configuration(
                     store_name='state_store'
                     keys=['key_1'],
                     config_metadata={"metakey": "metavalue"}
                 )
 
         Args:
             store_name (str): the state store name to get from
-            keys (str): the keys of the key-value pairs to be gotten
+            keys (List[str]): the keys of the key-value pairs to be gotten
             config_metadata (Dict[str, str], optional): Dapr metadata for configuration
 
         Returns:
             :class:`ConfigurationResponse` gRPC metadata returned from callee
             and value obtained from the config store
         """
-        warn('The Get Configuration API is an Alpha version and is subject to change.',
-             UserWarning, stacklevel=2)
-
         if not store_name or len(store_name) == 0 or len(store_name.strip()) == 0:
             raise ValueError("Config store name cannot be empty to get the configuration")
+
         req = api_v1.GetConfigurationRequest(
             store_name=store_name, keys=keys, metadata=config_metadata)
-        call = self._stub.GetConfigurationAlpha1(req)
+        call = self._stub.GetConfiguration(req)
         response = await call
         return ConfigurationResponse(
             items=response.items,
             headers=await call.initial_metadata())
 
     async def subscribe_configuration(
             self,
@@ -965,35 +960,33 @@
             handler: Callable[[Text, ConfigurationResponse], None],
             config_metadata: Optional[Dict[str, str]] = dict()) -> Text:
         """Gets changed value from a config store with a key
 
         The example gets value from a config store:
             from dapr.aio.clients import DaprClient
             async with DaprClient() as d:
-                resp = await d.subscribe_config(
+                resp = await d.subscribe_configuration(
                     store_name='state_store'
-                    key='key_1',
+                    keys=['key_1'],
                     handler=handler,
                     config_metadata={"metakey": "metavalue"}
                 )
 
         Args:
             store_name (str): the state store name to get from
             keys (str array): the keys of the key-value pairs to be gotten
             handler(func (key, ConfigurationResponse)): the callback function to be called
             config_metadata (Dict[str, str], optional): Dapr metadata for configuration
 
         Returns:
             id (str): subscription id, which can be used to unsubscribe later
         """
-        warn('The Subscribe Configuration API is an Alpha version and is subject to change.',
-             UserWarning, stacklevel=2)
-
         if not store_name or len(store_name) == 0 or len(store_name.strip()) == 0:
             raise ValueError("Config store name cannot be empty to get the configuration")
+
         configWatcher = ConfigurationWatcher()
         id = configWatcher.watch_configuration(self._stub, store_name, keys,
                                                handler, config_metadata)
         return id
 
     async def unsubscribe_configuration(
             self,
@@ -1004,19 +997,16 @@
             Args:
                 store_name (str): the state store name to unsubscribe from
                 id (str): the subscription id to unsubscribe
 
             Returns:
                 bool: True if unsubscribed successfully, False otherwise
         """
-        warn('The Unsubscribe Configuration API is an Alpha version and is subject to change.',
-             UserWarning, stacklevel=2)
         req = api_v1.UnsubscribeConfigurationRequest(store_name=store_name, id=id)
-        call = self._stub.UnsubscribeConfigurationAlpha1(req)
-        response: UnsubscribeConfigurationResponse = await call
+        response: UnsubscribeConfigurationResponse = await self._stub.UnsubscribeConfiguration(req)
         return response.ok
 
     async def try_lock(
             self,
             store_name: str,
             resource_id: str,
             lock_owner: str,
@@ -1062,15 +1052,15 @@
         if not expiry_in_seconds or expiry_in_seconds < 1:
             raise ValueError("expiry_in_seconds must be a positive number")
         # Actual tryLock invocation
         req = api_v1.TryLockRequest(
             store_name=store_name,
             resource_id=resource_id,
             lock_owner=lock_owner,
-            expiryInSeconds=expiry_in_seconds)
+            expiry_in_seconds=expiry_in_seconds)
         call = self._stub.TryLockAlpha1(req)
         response = await call
         return TryLockResponse(
             success=response.success,
             client=self,
             store_name=store_name,
             resource_id=resource_id,
```

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/base.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/base.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/exceptions.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_helpers.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/_helpers.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_request.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/_request.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_response.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/_response.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_state.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/_state.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/client.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/grpc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -919,29 +919,26 @@
                     store_name='state_store'
                     keys=['key_1'],
                     config_metadata={"metakey": "metavalue"}
                 )
 
         Args:
             store_name (str): the state store name to get from
-            keys (str): the keys of the key-value pairs to be gotten
+            keys (List[str]): the keys of the key-value pairs to be gotten
             config_metadata (Dict[str, str], optional): Dapr metadata for configuration
 
         Returns:
             :class:`ConfigurationResponse` gRPC metadata returned from callee
             and value obtained from the config store
         """
-        warn('The Get Configuration API is an Alpha version and is subject to change.',
-             UserWarning, stacklevel=2)
-
         if not store_name or len(store_name) == 0 or len(store_name.strip()) == 0:
             raise ValueError("Config store name cannot be empty to get the configuration")
         req = api_v1.GetConfigurationRequest(
             store_name=store_name, keys=keys, metadata=config_metadata)
-        response, call = self._stub.GetConfigurationAlpha1.with_call(req)
+        response, call = self._stub.GetConfiguration.with_call(req)
         return ConfigurationResponse(
             items=response.items,
             headers=call.initial_metadata())
 
     def subscribe_configuration(
             self,
             store_name: str,
@@ -949,35 +946,34 @@
             handler: Callable[[Text, ConfigurationResponse], None],
             config_metadata: Optional[Dict[str, str]] = dict()) -> Text:
         """Gets changed value from a config store with a key
 
         The example gets value from a config store:
             from dapr.clients import DaprClient
             with DaprClient() as d:
-                resp = d.subscribe_config(
+                resp = d.subscribe_configuration(
                     store_name='state_store'
-                    key='key_1',
+                    keys=['key_1'],
                     handler=handler,
                     config_metadata={"metakey": "metavalue"}
                 )
 
         Args:
             store_name (str): the state store name to get from
             keys (str array): the keys of the key-value pairs to be gotten
             handler(func (key, ConfigurationResponse)): the callback function to be called
             config_metadata (Dict[str, str], optional): Dapr metadata for configuration
 
         Returns:
             id (str): subscription id, which can be used to unsubscribe later
         """
-        warn('The Subscribe Configuration API is an Alpha version and is subject to change.',
-             UserWarning, stacklevel=2)
 
         if not store_name or len(store_name) == 0 or len(store_name.strip()) == 0:
             raise ValueError("Config store name cannot be empty to get the configuration")
+
         configWatcher = ConfigurationWatcher()
         id = configWatcher.watch_configuration(self._stub, store_name, keys,
                                                handler, config_metadata)
         return id
 
     def unsubscribe_configuration(
             self,
@@ -988,18 +984,16 @@
             Args:
                 store_name (str): the state store name to unsubscribe from
                 id (str): the subscription id to unsubscribe
 
             Returns:
                 bool: True if unsubscribed successfully, False otherwise
         """
-        warn('The Unsubscribe Configuration API is an Alpha version and is subject to change.',
-             UserWarning, stacklevel=2)
         req = api_v1.UnsubscribeConfigurationRequest(store_name=store_name, id=id)
-        response: UnsubscribeConfigurationResponse = self._stub.UnsubscribeConfigurationAlpha1(req)
+        response: UnsubscribeConfigurationResponse = self._stub.UnsubscribeConfiguration(req)
         return response.ok
 
     def try_lock(
             self,
             store_name: str,
             resource_id: str,
             lock_owner: str,
@@ -1045,15 +1039,15 @@
         if not expiry_in_seconds or expiry_in_seconds < 1:
             raise ValueError("expiry_in_seconds must be a positive number")
         # Actual tryLock invocation
         req = api_v1.TryLockRequest(
             store_name=store_name,
             resource_id=resource_id,
             lock_owner=lock_owner,
-            expiryInSeconds=expiry_in_seconds)
+            expiry_in_seconds=expiry_in_seconds)
         response, call = self._stub.TryLockAlpha1.with_call(req)
         return TryLockResponse(
             success=response.success,
             client=self,
             store_name=store_name,
             resource_id=resource_id,
             lock_owner=lock_owner,
```

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/http/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/client.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/http/client.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/dapr_actor_http_client.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/http/dapr_actor_http_client.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/dapr_invocation_http_client.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/clients/http/dapr_invocation_http_client.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/conf/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/conf/global_settings.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/proto/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/proto/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/proto/common/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/common_pb2.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/proto/common/v1/common_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!dapr/proto/common/v1/common.proto\x12\x14\x64\x61pr.proto.common.v1\x1a\x19google/protobuf/any.proto\"\xd0\x01\n\rHTTPExtension\x12\x36\n\x04verb\x18\x01 \x01(\x0e\x32(.dapr.proto.common.v1.HTTPExtension.Verb\x12\x13\n\x0bquerystring\x18\x02 \x01(\t\"r\n\x04Verb\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03GET\x10\x01\x12\x08\n\x04HEAD\x10\x02\x12\x08\n\x04POST\x10\x03\x12\x07\n\x03PUT\x10\x04\x12\n\n\x06\x44\x45LETE\x10\x05\x12\x0b\n\x07\x43ONNECT\x10\x06\x12\x0b\n\x07OPTIONS\x10\x07\x12\t\n\x05TRACE\x10\x08\x12\t\n\x05PATCH\x10\t\"\x96\x01\n\rInvokeRequest\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\"\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x14\n\x0c\x63ontent_type\x18\x03 \x01(\t\x12;\n\x0ehttp_extension\x18\x04 \x01(\x0b\x32#.dapr.proto.common.v1.HTTPExtension\"J\n\x0eInvokeResponse\x12\"\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x14\n\x0c\x63ontent_type\x18\x02 \x01(\t\"\xf8\x01\n\tStateItem\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12(\n\x04\x65tag\x18\x03 \x01(\x0b\x32\x1a.dapr.proto.common.v1.Etag\x12?\n\x08metadata\x18\x04 \x03(\x0b\x32-.dapr.proto.common.v1.StateItem.MetadataEntry\x12\x33\n\x07options\x18\x05 \x01(\x0b\x32\".dapr.proto.common.v1.StateOptions\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x15\n\x04\x45tag\x12\r\n\x05value\x18\x01 \x01(\t\"\xef\x02\n\x0cStateOptions\x12H\n\x0b\x63oncurrency\x18\x01 \x01(\x0e\x32\x33.dapr.proto.common.v1.StateOptions.StateConcurrency\x12H\n\x0b\x63onsistency\x18\x02 \x01(\x0e\x32\x33.dapr.proto.common.v1.StateOptions.StateConsistency\"h\n\x10StateConcurrency\x12\x1b\n\x17\x43ONCURRENCY_UNSPECIFIED\x10\x00\x12\x1b\n\x17\x43ONCURRENCY_FIRST_WRITE\x10\x01\x12\x1a\n\x16\x43ONCURRENCY_LAST_WRITE\x10\x02\"a\n\x10StateConsistency\x12\x1b\n\x17\x43ONSISTENCY_UNSPECIFIED\x10\x00\x12\x18\n\x14\x43ONSISTENCY_EVENTUAL\x10\x01\x12\x16\n\x12\x43ONSISTENCY_STRONG\x10\x02\"\xad\x01\n\x11\x43onfigurationItem\x12\r\n\x05value\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12G\n\x08metadata\x18\x03 \x03(\x0b\x32\x35.dapr.proto.common.v1.ConfigurationItem.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42i\n\nio.dapr.v1B\x0c\x43ommonProtosZ/github.com/dapr/dapr/pkg/proto/common/v1;common\xaa\x02\x1b\x44\x61pr.Client.Autogen.Grpc.v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!dapr/proto/common/v1/common.proto\x12\x14\x64\x61pr.proto.common.v1\x1a\x19google/protobuf/any.proto\"\xd0\x01\n\rHTTPExtension\x12\x36\n\x04verb\x18\x01 \x01(\x0e\x32(.dapr.proto.common.v1.HTTPExtension.Verb\x12\x13\n\x0bquerystring\x18\x02 \x01(\t\"r\n\x04Verb\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03GET\x10\x01\x12\x08\n\x04HEAD\x10\x02\x12\x08\n\x04POST\x10\x03\x12\x07\n\x03PUT\x10\x04\x12\n\n\x06\x44\x45LETE\x10\x05\x12\x0b\n\x07\x43ONNECT\x10\x06\x12\x0b\n\x07OPTIONS\x10\x07\x12\t\n\x05TRACE\x10\x08\x12\t\n\x05PATCH\x10\t\"\x96\x01\n\rInvokeRequest\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\"\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x14\n\x0c\x63ontent_type\x18\x03 \x01(\t\x12;\n\x0ehttp_extension\x18\x04 \x01(\x0b\x32#.dapr.proto.common.v1.HTTPExtension\"J\n\x0eInvokeResponse\x12\"\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x14\n\x0c\x63ontent_type\x18\x02 \x01(\t\"*\n\rStreamPayload\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0b\n\x03seq\x18\x02 \x01(\x04\"\xf8\x01\n\tStateItem\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12(\n\x04\x65tag\x18\x03 \x01(\x0b\x32\x1a.dapr.proto.common.v1.Etag\x12?\n\x08metadata\x18\x04 \x03(\x0b\x32-.dapr.proto.common.v1.StateItem.MetadataEntry\x12\x33\n\x07options\x18\x05 \x01(\x0b\x32\".dapr.proto.common.v1.StateOptions\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x15\n\x04\x45tag\x12\r\n\x05value\x18\x01 \x01(\t\"\xef\x02\n\x0cStateOptions\x12H\n\x0b\x63oncurrency\x18\x01 \x01(\x0e\x32\x33.dapr.proto.common.v1.StateOptions.StateConcurrency\x12H\n\x0b\x63onsistency\x18\x02 \x01(\x0e\x32\x33.dapr.proto.common.v1.StateOptions.StateConsistency\"h\n\x10StateConcurrency\x12\x1b\n\x17\x43ONCURRENCY_UNSPECIFIED\x10\x00\x12\x1b\n\x17\x43ONCURRENCY_FIRST_WRITE\x10\x01\x12\x1a\n\x16\x43ONCURRENCY_LAST_WRITE\x10\x02\"a\n\x10StateConsistency\x12\x1b\n\x17\x43ONSISTENCY_UNSPECIFIED\x10\x00\x12\x18\n\x14\x43ONSISTENCY_EVENTUAL\x10\x01\x12\x16\n\x12\x43ONSISTENCY_STRONG\x10\x02\"\xad\x01\n\x11\x43onfigurationItem\x12\r\n\x05value\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12G\n\x08metadata\x18\x03 \x03(\x0b\x32\x35.dapr.proto.common.v1.ConfigurationItem.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42i\n\nio.dapr.v1B\x0c\x43ommonProtosZ/github.com/dapr/dapr/pkg/proto/common/v1;common\xaa\x02\x1b\x44\x61pr.Client.Autogen.Grpc.v1b\x06proto3')
 
 
 
 _HTTPEXTENSION = DESCRIPTOR.message_types_by_name['HTTPExtension']
 _INVOKEREQUEST = DESCRIPTOR.message_types_by_name['InvokeRequest']
 _INVOKERESPONSE = DESCRIPTOR.message_types_by_name['InvokeResponse']
+_STREAMPAYLOAD = DESCRIPTOR.message_types_by_name['StreamPayload']
 _STATEITEM = DESCRIPTOR.message_types_by_name['StateItem']
 _STATEITEM_METADATAENTRY = _STATEITEM.nested_types_by_name['MetadataEntry']
 _ETAG = DESCRIPTOR.message_types_by_name['Etag']
 _STATEOPTIONS = DESCRIPTOR.message_types_by_name['StateOptions']
 _CONFIGURATIONITEM = DESCRIPTOR.message_types_by_name['ConfigurationItem']
 _CONFIGURATIONITEM_METADATAENTRY = _CONFIGURATIONITEM.nested_types_by_name['MetadataEntry']
 _HTTPEXTENSION_VERB = _HTTPEXTENSION.enum_types_by_name['Verb']
@@ -48,14 +49,21 @@
 InvokeResponse = _reflection.GeneratedProtocolMessageType('InvokeResponse', (_message.Message,), {
   'DESCRIPTOR' : _INVOKERESPONSE,
   '__module__' : 'dapr.proto.common.v1.common_pb2'
   # @@protoc_insertion_point(class_scope:dapr.proto.common.v1.InvokeResponse)
   })
 _sym_db.RegisterMessage(InvokeResponse)
 
+StreamPayload = _reflection.GeneratedProtocolMessageType('StreamPayload', (_message.Message,), {
+  'DESCRIPTOR' : _STREAMPAYLOAD,
+  '__module__' : 'dapr.proto.common.v1.common_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.common.v1.StreamPayload)
+  })
+_sym_db.RegisterMessage(StreamPayload)
+
 StateItem = _reflection.GeneratedProtocolMessageType('StateItem', (_message.Message,), {
 
   'MetadataEntry' : _reflection.GeneratedProtocolMessageType('MetadataEntry', (_message.Message,), {
     'DESCRIPTOR' : _STATEITEM_METADATAENTRY,
     '__module__' : 'dapr.proto.common.v1.common_pb2'
     # @@protoc_insertion_point(class_scope:dapr.proto.common.v1.StateItem.MetadataEntry)
     })
@@ -108,24 +116,26 @@
   _HTTPEXTENSION._serialized_end=295
   _HTTPEXTENSION_VERB._serialized_start=181
   _HTTPEXTENSION_VERB._serialized_end=295
   _INVOKEREQUEST._serialized_start=298
   _INVOKEREQUEST._serialized_end=448
   _INVOKERESPONSE._serialized_start=450
   _INVOKERESPONSE._serialized_end=524
-  _STATEITEM._serialized_start=527
-  _STATEITEM._serialized_end=775
-  _STATEITEM_METADATAENTRY._serialized_start=728
-  _STATEITEM_METADATAENTRY._serialized_end=775
-  _ETAG._serialized_start=777
-  _ETAG._serialized_end=798
-  _STATEOPTIONS._serialized_start=801
-  _STATEOPTIONS._serialized_end=1168
-  _STATEOPTIONS_STATECONCURRENCY._serialized_start=965
-  _STATEOPTIONS_STATECONCURRENCY._serialized_end=1069
-  _STATEOPTIONS_STATECONSISTENCY._serialized_start=1071
-  _STATEOPTIONS_STATECONSISTENCY._serialized_end=1168
-  _CONFIGURATIONITEM._serialized_start=1171
-  _CONFIGURATIONITEM._serialized_end=1344
-  _CONFIGURATIONITEM_METADATAENTRY._serialized_start=728
-  _CONFIGURATIONITEM_METADATAENTRY._serialized_end=775
+  _STREAMPAYLOAD._serialized_start=526
+  _STREAMPAYLOAD._serialized_end=568
+  _STATEITEM._serialized_start=571
+  _STATEITEM._serialized_end=819
+  _STATEITEM_METADATAENTRY._serialized_start=772
+  _STATEITEM_METADATAENTRY._serialized_end=819
+  _ETAG._serialized_start=821
+  _ETAG._serialized_end=842
+  _STATEOPTIONS._serialized_start=845
+  _STATEOPTIONS._serialized_end=1212
+  _STATEOPTIONS_STATECONCURRENCY._serialized_start=1009
+  _STATEOPTIONS_STATECONCURRENCY._serialized_end=1113
+  _STATEOPTIONS_STATECONSISTENCY._serialized_start=1115
+  _STATEOPTIONS_STATECONSISTENCY._serialized_end=1212
+  _CONFIGURATIONITEM._serialized_start=1215
+  _CONFIGURATIONITEM._serialized_end=1388
+  _CONFIGURATIONITEM_METADATAENTRY._serialized_start=772
+  _CONFIGURATIONITEM_METADATAENTRY._serialized_end=819
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/appcallback_pb2.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/v1/appcallback_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from dapr.proto.common.v1 import common_pb2 as dapr_dot_proto_dot_common_dot_v1_dot_common__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'dapr/proto/runtime/v1/appcallback.proto\x12\x15\x64\x61pr.proto.runtime.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a!dapr/proto/common/v1/common.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xdb\x01\n\x11TopicEventRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x14\n\x0cspec_version\x18\x04 \x01(\t\x12\x19\n\x11\x64\x61ta_content_type\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\x0c\x12\r\n\x05topic\x18\x06 \x01(\t\x12\x13\n\x0bpubsub_name\x18\x08 \x01(\t\x12\x0c\n\x04path\x18\t \x01(\t\x12+\n\nextensions\x18\n \x01(\x0b\x32\x17.google.protobuf.Struct\"\xa6\x01\n\x12TopicEventResponse\x12R\n\x06status\x18\x01 \x01(\x0e\x32\x42.dapr.proto.runtime.v1.TopicEventResponse.TopicEventResponseStatus\"<\n\x18TopicEventResponseStatus\x12\x0b\n\x07SUCCESS\x10\x00\x12\t\n\x05RETRY\x10\x01\x12\x08\n\x04\x44ROP\x10\x02\"\xab\x01\n\x13TopicEventCERequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x14\n\x0cspec_version\x18\x04 \x01(\t\x12\x19\n\x11\x64\x61ta_content_type\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12+\n\nextensions\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xa5\x02\n\x1aTopicEventBulkRequestEntry\x12\x10\n\x08\x65ntry_id\x18\x01 \x01(\t\x12\x0f\n\x05\x62ytes\x18\x02 \x01(\x0cH\x00\x12\x41\n\x0b\x63loud_event\x18\x03 \x01(\x0b\x32*.dapr.proto.runtime.v1.TopicEventCERequestH\x00\x12\x14\n\x0c\x63ontent_type\x18\x04 \x01(\t\x12Q\n\x08metadata\x18\x05 \x03(\x0b\x32?.dapr.proto.runtime.v1.TopicEventBulkRequestEntry.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x07\n\x05\x65vent\"\xa6\x02\n\x15TopicEventBulkRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x42\n\x07\x65ntries\x18\x02 \x03(\x0b\x32\x31.dapr.proto.runtime.v1.TopicEventBulkRequestEntry\x12L\n\x08metadata\x18\x03 \x03(\x0b\x32:.dapr.proto.runtime.v1.TopicEventBulkRequest.MetadataEntry\x12\r\n\x05topic\x18\x04 \x01(\t\x12\x13\n\x0bpubsub_name\x18\x05 \x01(\t\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x0c\n\x04path\x18\x07 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x01\n\x1bTopicEventBulkResponseEntry\x12\x10\n\x08\x65ntry_id\x18\x01 \x01(\t\x12R\n\x06status\x18\x02 \x01(\x0e\x32\x42.dapr.proto.runtime.v1.TopicEventResponse.TopicEventResponseStatus\"^\n\x16TopicEventBulkResponse\x12\x44\n\x08statuses\x18\x01 \x03(\x0b\x32\x32.dapr.proto.runtime.v1.TopicEventBulkResponseEntry\"\xae\x01\n\x13\x42indingEventRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12J\n\x08metadata\x18\x03 \x03(\x0b\x32\x38.dapr.proto.runtime.v1.BindingEventRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x02\n\x14\x42indingEventResponse\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12/\n\x06states\x18\x02 \x03(\x0b\x32\x1f.dapr.proto.common.v1.StateItem\x12\n\n\x02to\x18\x03 \x03(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12X\n\x0b\x63oncurrency\x18\x05 \x01(\x0e\x32\x43.dapr.proto.runtime.v1.BindingEventResponse.BindingEventConcurrency\"7\n\x17\x42indingEventConcurrency\x12\x0e\n\nSEQUENTIAL\x10\x00\x12\x0c\n\x08PARALLEL\x10\x01\"a\n\x1eListTopicSubscriptionsResponse\x12?\n\rsubscriptions\x18\x01 \x03(\x0b\x32(.dapr.proto.runtime.v1.TopicSubscription\"\x81\x02\n\x11TopicSubscription\x12\x13\n\x0bpubsub_name\x18\x01 \x01(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12H\n\x08metadata\x18\x03 \x03(\x0b\x32\x36.dapr.proto.runtime.v1.TopicSubscription.MetadataEntry\x12\x32\n\x06routes\x18\x05 \x01(\x0b\x32\".dapr.proto.runtime.v1.TopicRoutes\x12\x19\n\x11\x64\x65\x61\x64_letter_topic\x18\x06 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"O\n\x0bTopicRoutes\x12/\n\x05rules\x18\x01 \x03(\x0b\x32 .dapr.proto.runtime.v1.TopicRule\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x02 \x01(\t\"(\n\tTopicRule\x12\r\n\x05match\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"-\n\x19ListInputBindingsResponse\x12\x10\n\x08\x62indings\x18\x01 \x03(\t\"\x15\n\x13HealthCheckResponse2\x86\x04\n\x0b\x41ppCallback\x12W\n\x08OnInvoke\x12#.dapr.proto.common.v1.InvokeRequest\x1a$.dapr.proto.common.v1.InvokeResponse\"\x00\x12i\n\x16ListTopicSubscriptions\x12\x16.google.protobuf.Empty\x1a\x35.dapr.proto.runtime.v1.ListTopicSubscriptionsResponse\"\x00\x12\x65\n\x0cOnTopicEvent\x12(.dapr.proto.runtime.v1.TopicEventRequest\x1a).dapr.proto.runtime.v1.TopicEventResponse\"\x00\x12_\n\x11ListInputBindings\x12\x16.google.protobuf.Empty\x1a\x30.dapr.proto.runtime.v1.ListInputBindingsResponse\"\x00\x12k\n\x0eOnBindingEvent\x12*.dapr.proto.runtime.v1.BindingEventRequest\x1a+.dapr.proto.runtime.v1.BindingEventResponse\"\x00\x32m\n\x16\x41ppCallbackHealthCheck\x12S\n\x0bHealthCheck\x12\x16.google.protobuf.Empty\x1a*.dapr.proto.runtime.v1.HealthCheckResponse\"\x00\x32\x8b\x01\n\x10\x41ppCallbackAlpha\x12w\n\x16OnBulkTopicEventAlpha1\x12,.dapr.proto.runtime.v1.TopicEventBulkRequest\x1a-.dapr.proto.runtime.v1.TopicEventBulkResponse\"\x00\x42y\n\nio.dapr.v1B\x15\x44\x61prAppCallbackProtosZ1github.com/dapr/dapr/pkg/proto/runtime/v1;runtime\xaa\x02 Dapr.AppCallback.Autogen.Grpc.v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'dapr/proto/runtime/v1/appcallback.proto\x12\x15\x64\x61pr.proto.runtime.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a!dapr/proto/common/v1/common.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xdb\x01\n\x11TopicEventRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x14\n\x0cspec_version\x18\x04 \x01(\t\x12\x19\n\x11\x64\x61ta_content_type\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\x0c\x12\r\n\x05topic\x18\x06 \x01(\t\x12\x13\n\x0bpubsub_name\x18\x08 \x01(\t\x12\x0c\n\x04path\x18\t \x01(\t\x12+\n\nextensions\x18\n \x01(\x0b\x32\x17.google.protobuf.Struct\"\xa6\x01\n\x12TopicEventResponse\x12R\n\x06status\x18\x01 \x01(\x0e\x32\x42.dapr.proto.runtime.v1.TopicEventResponse.TopicEventResponseStatus\"<\n\x18TopicEventResponseStatus\x12\x0b\n\x07SUCCESS\x10\x00\x12\t\n\x05RETRY\x10\x01\x12\x08\n\x04\x44ROP\x10\x02\"\xab\x01\n\x13TopicEventCERequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x14\n\x0cspec_version\x18\x04 \x01(\t\x12\x19\n\x11\x64\x61ta_content_type\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12+\n\nextensions\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xa5\x02\n\x1aTopicEventBulkRequestEntry\x12\x10\n\x08\x65ntry_id\x18\x01 \x01(\t\x12\x0f\n\x05\x62ytes\x18\x02 \x01(\x0cH\x00\x12\x41\n\x0b\x63loud_event\x18\x03 \x01(\x0b\x32*.dapr.proto.runtime.v1.TopicEventCERequestH\x00\x12\x14\n\x0c\x63ontent_type\x18\x04 \x01(\t\x12Q\n\x08metadata\x18\x05 \x03(\x0b\x32?.dapr.proto.runtime.v1.TopicEventBulkRequestEntry.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x07\n\x05\x65vent\"\xa6\x02\n\x15TopicEventBulkRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x42\n\x07\x65ntries\x18\x02 \x03(\x0b\x32\x31.dapr.proto.runtime.v1.TopicEventBulkRequestEntry\x12L\n\x08metadata\x18\x03 \x03(\x0b\x32:.dapr.proto.runtime.v1.TopicEventBulkRequest.MetadataEntry\x12\r\n\x05topic\x18\x04 \x01(\t\x12\x13\n\x0bpubsub_name\x18\x05 \x01(\t\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x0c\n\x04path\x18\x07 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x01\n\x1bTopicEventBulkResponseEntry\x12\x10\n\x08\x65ntry_id\x18\x01 \x01(\t\x12R\n\x06status\x18\x02 \x01(\x0e\x32\x42.dapr.proto.runtime.v1.TopicEventResponse.TopicEventResponseStatus\"^\n\x16TopicEventBulkResponse\x12\x44\n\x08statuses\x18\x01 \x03(\x0b\x32\x32.dapr.proto.runtime.v1.TopicEventBulkResponseEntry\"\xae\x01\n\x13\x42indingEventRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12J\n\x08metadata\x18\x03 \x03(\x0b\x32\x38.dapr.proto.runtime.v1.BindingEventRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x02\n\x14\x42indingEventResponse\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12/\n\x06states\x18\x02 \x03(\x0b\x32\x1f.dapr.proto.common.v1.StateItem\x12\n\n\x02to\x18\x03 \x03(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12X\n\x0b\x63oncurrency\x18\x05 \x01(\x0e\x32\x43.dapr.proto.runtime.v1.BindingEventResponse.BindingEventConcurrency\"7\n\x17\x42indingEventConcurrency\x12\x0e\n\nSEQUENTIAL\x10\x00\x12\x0c\n\x08PARALLEL\x10\x01\"a\n\x1eListTopicSubscriptionsResponse\x12?\n\rsubscriptions\x18\x01 \x03(\x0b\x32(.dapr.proto.runtime.v1.TopicSubscription\"\xc5\x02\n\x11TopicSubscription\x12\x13\n\x0bpubsub_name\x18\x01 \x01(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12H\n\x08metadata\x18\x03 \x03(\x0b\x32\x36.dapr.proto.runtime.v1.TopicSubscription.MetadataEntry\x12\x32\n\x06routes\x18\x05 \x01(\x0b\x32\".dapr.proto.runtime.v1.TopicRoutes\x12\x19\n\x11\x64\x65\x61\x64_letter_topic\x18\x06 \x01(\t\x12\x42\n\x0e\x62ulk_subscribe\x18\x07 \x01(\x0b\x32*.dapr.proto.runtime.v1.BulkSubscribeConfig\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"O\n\x0bTopicRoutes\x12/\n\x05rules\x18\x01 \x03(\x0b\x32 .dapr.proto.runtime.v1.TopicRule\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x02 \x01(\t\"(\n\tTopicRule\x12\r\n\x05match\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"a\n\x13\x42ulkSubscribeConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12max_messages_count\x18\x02 \x01(\x05\x12\x1d\n\x15max_await_duration_ms\x18\x03 \x01(\x05\"-\n\x19ListInputBindingsResponse\x12\x10\n\x08\x62indings\x18\x01 \x03(\t\"\x15\n\x13HealthCheckResponse2\x86\x04\n\x0b\x41ppCallback\x12W\n\x08OnInvoke\x12#.dapr.proto.common.v1.InvokeRequest\x1a$.dapr.proto.common.v1.InvokeResponse\"\x00\x12i\n\x16ListTopicSubscriptions\x12\x16.google.protobuf.Empty\x1a\x35.dapr.proto.runtime.v1.ListTopicSubscriptionsResponse\"\x00\x12\x65\n\x0cOnTopicEvent\x12(.dapr.proto.runtime.v1.TopicEventRequest\x1a).dapr.proto.runtime.v1.TopicEventResponse\"\x00\x12_\n\x11ListInputBindings\x12\x16.google.protobuf.Empty\x1a\x30.dapr.proto.runtime.v1.ListInputBindingsResponse\"\x00\x12k\n\x0eOnBindingEvent\x12*.dapr.proto.runtime.v1.BindingEventRequest\x1a+.dapr.proto.runtime.v1.BindingEventResponse\"\x00\x32m\n\x16\x41ppCallbackHealthCheck\x12S\n\x0bHealthCheck\x12\x16.google.protobuf.Empty\x1a*.dapr.proto.runtime.v1.HealthCheckResponse\"\x00\x32\x8b\x01\n\x10\x41ppCallbackAlpha\x12w\n\x16OnBulkTopicEventAlpha1\x12,.dapr.proto.runtime.v1.TopicEventBulkRequest\x1a-.dapr.proto.runtime.v1.TopicEventBulkResponse\"\x00\x42y\n\nio.dapr.v1B\x15\x44\x61prAppCallbackProtosZ1github.com/dapr/dapr/pkg/proto/runtime/v1;runtime\xaa\x02 Dapr.AppCallback.Autogen.Grpc.v1b\x06proto3')
 
 
 
 _TOPICEVENTREQUEST = DESCRIPTOR.message_types_by_name['TopicEventRequest']
 _TOPICEVENTRESPONSE = DESCRIPTOR.message_types_by_name['TopicEventResponse']
 _TOPICEVENTCEREQUEST = DESCRIPTOR.message_types_by_name['TopicEventCERequest']
 _TOPICEVENTBULKREQUESTENTRY = DESCRIPTOR.message_types_by_name['TopicEventBulkRequestEntry']
@@ -34,14 +34,15 @@
 _BINDINGEVENTREQUEST_METADATAENTRY = _BINDINGEVENTREQUEST.nested_types_by_name['MetadataEntry']
 _BINDINGEVENTRESPONSE = DESCRIPTOR.message_types_by_name['BindingEventResponse']
 _LISTTOPICSUBSCRIPTIONSRESPONSE = DESCRIPTOR.message_types_by_name['ListTopicSubscriptionsResponse']
 _TOPICSUBSCRIPTION = DESCRIPTOR.message_types_by_name['TopicSubscription']
 _TOPICSUBSCRIPTION_METADATAENTRY = _TOPICSUBSCRIPTION.nested_types_by_name['MetadataEntry']
 _TOPICROUTES = DESCRIPTOR.message_types_by_name['TopicRoutes']
 _TOPICRULE = DESCRIPTOR.message_types_by_name['TopicRule']
+_BULKSUBSCRIBECONFIG = DESCRIPTOR.message_types_by_name['BulkSubscribeConfig']
 _LISTINPUTBINDINGSRESPONSE = DESCRIPTOR.message_types_by_name['ListInputBindingsResponse']
 _HEALTHCHECKRESPONSE = DESCRIPTOR.message_types_by_name['HealthCheckResponse']
 _TOPICEVENTRESPONSE_TOPICEVENTRESPONSESTATUS = _TOPICEVENTRESPONSE.enum_types_by_name['TopicEventResponseStatus']
 _BINDINGEVENTRESPONSE_BINDINGEVENTCONCURRENCY = _BINDINGEVENTRESPONSE.enum_types_by_name['BindingEventConcurrency']
 TopicEventRequest = _reflection.GeneratedProtocolMessageType('TopicEventRequest', (_message.Message,), {
   'DESCRIPTOR' : _TOPICEVENTREQUEST,
   '__module__' : 'dapr.proto.runtime.v1.appcallback_pb2'
@@ -161,14 +162,21 @@
 TopicRule = _reflection.GeneratedProtocolMessageType('TopicRule', (_message.Message,), {
   'DESCRIPTOR' : _TOPICRULE,
   '__module__' : 'dapr.proto.runtime.v1.appcallback_pb2'
   # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.TopicRule)
   })
 _sym_db.RegisterMessage(TopicRule)
 
+BulkSubscribeConfig = _reflection.GeneratedProtocolMessageType('BulkSubscribeConfig', (_message.Message,), {
+  'DESCRIPTOR' : _BULKSUBSCRIBECONFIG,
+  '__module__' : 'dapr.proto.runtime.v1.appcallback_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.BulkSubscribeConfig)
+  })
+_sym_db.RegisterMessage(BulkSubscribeConfig)
+
 ListInputBindingsResponse = _reflection.GeneratedProtocolMessageType('ListInputBindingsResponse', (_message.Message,), {
   'DESCRIPTOR' : _LISTINPUTBINDINGSRESPONSE,
   '__module__' : 'dapr.proto.runtime.v1.appcallback_pb2'
   # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.ListInputBindingsResponse)
   })
 _sym_db.RegisterMessage(ListInputBindingsResponse)
 
@@ -221,25 +229,27 @@
   _BINDINGEVENTRESPONSE._serialized_start=1726
   _BINDINGEVENTRESPONSE._serialized_end=1990
   _BINDINGEVENTRESPONSE_BINDINGEVENTCONCURRENCY._serialized_start=1935
   _BINDINGEVENTRESPONSE_BINDINGEVENTCONCURRENCY._serialized_end=1990
   _LISTTOPICSUBSCRIPTIONSRESPONSE._serialized_start=1992
   _LISTTOPICSUBSCRIPTIONSRESPONSE._serialized_end=2089
   _TOPICSUBSCRIPTION._serialized_start=2092
-  _TOPICSUBSCRIPTION._serialized_end=2349
+  _TOPICSUBSCRIPTION._serialized_end=2417
   _TOPICSUBSCRIPTION_METADATAENTRY._serialized_start=963
   _TOPICSUBSCRIPTION_METADATAENTRY._serialized_end=1010
-  _TOPICROUTES._serialized_start=2351
-  _TOPICROUTES._serialized_end=2430
-  _TOPICRULE._serialized_start=2432
-  _TOPICRULE._serialized_end=2472
-  _LISTINPUTBINDINGSRESPONSE._serialized_start=2474
-  _LISTINPUTBINDINGSRESPONSE._serialized_end=2519
-  _HEALTHCHECKRESPONSE._serialized_start=2521
-  _HEALTHCHECKRESPONSE._serialized_end=2542
-  _APPCALLBACK._serialized_start=2545
-  _APPCALLBACK._serialized_end=3063
-  _APPCALLBACKHEALTHCHECK._serialized_start=3065
-  _APPCALLBACKHEALTHCHECK._serialized_end=3174
-  _APPCALLBACKALPHA._serialized_start=3177
-  _APPCALLBACKALPHA._serialized_end=3316
+  _TOPICROUTES._serialized_start=2419
+  _TOPICROUTES._serialized_end=2498
+  _TOPICRULE._serialized_start=2500
+  _TOPICRULE._serialized_end=2540
+  _BULKSUBSCRIBECONFIG._serialized_start=2542
+  _BULKSUBSCRIBECONFIG._serialized_end=2639
+  _LISTINPUTBINDINGSRESPONSE._serialized_start=2641
+  _LISTINPUTBINDINGSRESPONSE._serialized_end=2686
+  _HEALTHCHECKRESPONSE._serialized_start=2688
+  _HEALTHCHECKRESPONSE._serialized_end=2709
+  _APPCALLBACK._serialized_start=2712
+  _APPCALLBACK._serialized_end=3230
+  _APPCALLBACKHEALTHCHECK._serialized_start=3232
+  _APPCALLBACKHEALTHCHECK._serialized_end=3341
+  _APPCALLBACKALPHA._serialized_start=3344
+  _APPCALLBACKALPHA._serialized_end=3483
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/appcallback_pb2_grpc.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/v1/appcallback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/dapr_pb2.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/v1/dapr_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from dapr.proto.common.v1 import common_pb2 as dapr_dot_proto_dot_common_dot_v1_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n dapr/proto/runtime/v1/dapr.proto\x12\x15\x64\x61pr.proto.runtime.v1\x1a\x19google/protobuf/any.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a!dapr/proto/common/v1/common.proto\"X\n\x14InvokeServiceRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x34\n\x07message\x18\x03 \x01(\x0b\x32#.dapr.proto.common.v1.InvokeRequest\"\xf5\x01\n\x0fGetStateRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12H\n\x0b\x63onsistency\x18\x03 \x01(\x0e\x32\x33.dapr.proto.common.v1.StateOptions.StateConsistency\x12\x46\n\x08metadata\x18\x04 \x03(\x0b\x32\x34.dapr.proto.runtime.v1.GetStateRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc9\x01\n\x13GetBulkStateRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12\x13\n\x0bparallelism\x18\x03 \x01(\x05\x12J\n\x08metadata\x18\x04 \x03(\x0b\x32\x38.dapr.proto.runtime.v1.GetBulkStateRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"K\n\x14GetBulkStateResponse\x12\x33\n\x05items\x18\x01 \x03(\x0b\x32$.dapr.proto.runtime.v1.BulkStateItem\"\xbe\x01\n\rBulkStateItem\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x0c\n\x04\x65tag\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\x12\x44\n\x08metadata\x18\x05 \x03(\x0b\x32\x32.dapr.proto.runtime.v1.BulkStateItem.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa8\x01\n\x10GetStateResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0c\n\x04\x65tag\x18\x02 \x01(\t\x12G\n\x08metadata\x18\x03 \x03(\x0b\x32\x35.dapr.proto.runtime.v1.GetStateResponse.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x90\x02\n\x12\x44\x65leteStateRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12(\n\x04\x65tag\x18\x03 \x01(\x0b\x32\x1a.dapr.proto.common.v1.Etag\x12\x33\n\x07options\x18\x04 \x01(\x0b\x32\".dapr.proto.common.v1.StateOptions\x12I\n\x08metadata\x18\x05 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.DeleteStateRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"]\n\x16\x44\x65leteBulkStateRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12/\n\x06states\x18\x02 \x03(\x0b\x32\x1f.dapr.proto.common.v1.StateItem\"W\n\x10SaveStateRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12/\n\x06states\x18\x02 \x03(\x0b\x32\x1f.dapr.proto.common.v1.StateItem\"\xb1\x01\n\x11QueryStateRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\r\n\x05query\x18\x02 \x01(\t\x12H\n\x08metadata\x18\x03 \x03(\x0b\x32\x36.dapr.proto.runtime.v1.QueryStateRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"H\n\x0eQueryStateItem\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x0c\n\x04\x65tag\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"\xd7\x01\n\x12QueryStateResponse\x12\x36\n\x07results\x18\x01 \x03(\x0b\x32%.dapr.proto.runtime.v1.QueryStateItem\x12\r\n\x05token\x18\x02 \x01(\t\x12I\n\x08metadata\x18\x03 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.QueryStateResponse.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xdf\x01\n\x13PublishEventRequest\x12\x13\n\x0bpubsub_name\x18\x01 \x01(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\x12\x19\n\x11\x64\x61ta_content_type\x18\x04 \x01(\t\x12J\n\x08metadata\x18\x05 \x03(\x0b\x32\x38.dapr.proto.runtime.v1.PublishEventRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xf5\x01\n\x12\x42ulkPublishRequest\x12\x13\n\x0bpubsub_name\x18\x01 \x01(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12?\n\x07\x65ntries\x18\x03 \x03(\x0b\x32..dapr.proto.runtime.v1.BulkPublishRequestEntry\x12I\n\x08metadata\x18\x04 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.BulkPublishRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xd1\x01\n\x17\x42ulkPublishRequestEntry\x12\x10\n\x08\x65ntry_id\x18\x01 \x01(\t\x12\r\n\x05\x65vent\x18\x02 \x01(\x0c\x12\x14\n\x0c\x63ontent_type\x18\x03 \x01(\t\x12N\n\x08metadata\x18\x04 \x03(\x0b\x32<.dapr.proto.runtime.v1.BulkPublishRequestEntry.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"X\n\x13\x42ulkPublishResponse\x12\x41\n\x08statuses\x18\x01 \x03(\x0b\x32/.dapr.proto.runtime.v1.BulkPublishResponseEntry\"\xa6\x01\n\x18\x42ulkPublishResponseEntry\x12\x10\n\x08\x65ntry_id\x18\x01 \x01(\t\x12\x46\n\x06status\x18\x02 \x01(\x0e\x32\x36.dapr.proto.runtime.v1.BulkPublishResponseEntry.Status\x12\r\n\x05\x65rror\x18\x03 \x01(\t\"!\n\x06Status\x12\x0b\n\x07SUCCESS\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\"\xc3\x01\n\x14InvokeBindingRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12K\n\x08metadata\x18\x03 \x03(\x0b\x32\x39.dapr.proto.runtime.v1.InvokeBindingRequest.MetadataEntry\x12\x11\n\toperation\x18\x04 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa4\x01\n\x15InvokeBindingResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12L\n\x08metadata\x18\x02 \x03(\x0b\x32:.dapr.proto.runtime.v1.InvokeBindingResponse.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xad\x01\n\x10GetSecretRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12G\n\x08metadata\x18\x03 \x03(\x0b\x32\x35.dapr.proto.runtime.v1.GetSecretRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x82\x01\n\x11GetSecretResponse\x12@\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x32.dapr.proto.runtime.v1.GetSecretResponse.DataEntry\x1a+\n\tDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa8\x01\n\x14GetBulkSecretRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12K\n\x08metadata\x18\x02 \x03(\x0b\x32\x39.dapr.proto.runtime.v1.GetBulkSecretRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x85\x01\n\x0eSecretResponse\x12\x43\n\x07secrets\x18\x01 \x03(\x0b\x32\x32.dapr.proto.runtime.v1.SecretResponse.SecretsEntry\x1a.\n\x0cSecretsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb1\x01\n\x15GetBulkSecretResponse\x12\x44\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x36.dapr.proto.runtime.v1.GetBulkSecretResponse.DataEntry\x1aR\n\tDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.dapr.proto.runtime.v1.SecretResponse:\x02\x38\x01\"f\n\x1bTransactionalStateOperation\x12\x15\n\roperationType\x18\x01 \x01(\t\x12\x30\n\x07request\x18\x02 \x01(\x0b\x32\x1f.dapr.proto.common.v1.StateItem\"\x83\x02\n\x1e\x45xecuteStateTransactionRequest\x12\x11\n\tstoreName\x18\x01 \x01(\t\x12\x46\n\noperations\x18\x02 \x03(\x0b\x32\x32.dapr.proto.runtime.v1.TransactionalStateOperation\x12U\n\x08metadata\x18\x03 \x03(\x0b\x32\x43.dapr.proto.runtime.v1.ExecuteStateTransactionRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9e\x01\n\x19RegisterActorTimerRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08\x64ue_time\x18\x04 \x01(\t\x12\x0e\n\x06period\x18\x05 \x01(\t\x12\x10\n\x08\x63\x61llback\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\x0c\x12\x0b\n\x03ttl\x18\x08 \x01(\t\"Q\n\x1bUnregisterActorTimerRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"\x8f\x01\n\x1cRegisterActorReminderRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08\x64ue_time\x18\x04 \x01(\t\x12\x0e\n\x06period\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12\x0b\n\x03ttl\x18\x07 \x01(\t\"T\n\x1eUnregisterActorReminderRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"f\n\x1aRenameActorReminderRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x10\n\x08old_name\x18\x03 \x01(\t\x12\x10\n\x08new_name\x18\x04 \x01(\t\"I\n\x14GetActorStateRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\"%\n\x15GetActorStateResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\x98\x01\n#ExecuteActorStateTransactionRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12K\n\noperations\x18\x03 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.TransactionalActorStateOperation\"k\n TransactionalActorStateOperation\x12\x15\n\roperationType\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12#\n\x05value\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\"\xd4\x01\n\x12InvokeActorRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0e\n\x06method\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12I\n\x08metadata\x18\x05 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.InvokeActorRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"#\n\x13InvokeActorResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\x8c\x03\n\x13GetMetadataResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x45\n\x13\x61\x63tive_actors_count\x18\x02 \x03(\x0b\x32(.dapr.proto.runtime.v1.ActiveActorsCount\x12J\n\x15registered_components\x18\x03 \x03(\x0b\x32+.dapr.proto.runtime.v1.RegisteredComponents\x12[\n\x11\x65xtended_metadata\x18\x04 \x03(\x0b\x32@.dapr.proto.runtime.v1.GetMetadataResponse.ExtendedMetadataEntry\x12@\n\rsubscriptions\x18\x05 \x03(\x0b\x32).dapr.proto.runtime.v1.PubsubSubscription\x1a\x37\n\x15\x45xtendedMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"0\n\x11\x41\x63tiveActorsCount\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\"Y\n\x14RegisteredComponents\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x14\n\x0c\x63\x61pabilities\x18\x04 \x03(\t\"\x8e\x02\n\x12PubsubSubscription\x12\x13\n\x0bpubsub_name\x18\x01 \x01(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12I\n\x08metadata\x18\x03 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.PubsubSubscription.MetadataEntry\x12=\n\x05rules\x18\x04 \x01(\x0b\x32..dapr.proto.runtime.v1.PubsubSubscriptionRules\x12\x19\n\x11\x64\x65\x61\x64_letter_topic\x18\x05 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"W\n\x17PubsubSubscriptionRules\x12<\n\x05rules\x18\x01 \x03(\x0b\x32-.dapr.proto.runtime.v1.PubsubSubscriptionRule\"5\n\x16PubsubSubscriptionRule\x12\r\n\x05match\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"0\n\x12SetMetadataRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xbc\x01\n\x17GetConfigurationRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12N\n\x08metadata\x18\x03 \x03(\x0b\x32<.dapr.proto.runtime.v1.GetConfigurationRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xbc\x01\n\x18GetConfigurationResponse\x12I\n\x05items\x18\x01 \x03(\x0b\x32:.dapr.proto.runtime.v1.GetConfigurationResponse.ItemsEntry\x1aU\n\nItemsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.dapr.proto.common.v1.ConfigurationItem:\x02\x38\x01\"\xc8\x01\n\x1dSubscribeConfigurationRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12T\n\x08metadata\x18\x03 \x03(\x0b\x32\x42.dapr.proto.runtime.v1.SubscribeConfigurationRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"A\n\x1fUnsubscribeConfigurationRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"\xd4\x01\n\x1eSubscribeConfigurationResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.dapr.proto.runtime.v1.SubscribeConfigurationResponse.ItemsEntry\x1aU\n\nItemsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.dapr.proto.common.v1.ConfigurationItem:\x02\x38\x01\"?\n UnsubscribeConfigurationResponse\x12\n\n\x02ok\x18\x01 \x01(\x08\x12\x0f\n\x07message\x18\x02 \x01(\t\"f\n\x0eTryLockRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\x12\x12\n\nlock_owner\x18\x03 \x01(\t\x12\x17\n\x0f\x65xpiryInSeconds\x18\x04 \x01(\x05\"\"\n\x0fTryLockResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"L\n\rUnlockRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\x12\x12\n\nlock_owner\x18\x03 \x01(\t\"\xae\x01\n\x0eUnlockResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.dapr.proto.runtime.v1.UnlockResponse.Status\"^\n\x06Status\x12\x0b\n\x07SUCCESS\x10\x00\x12\x17\n\x13LOCK_DOES_NOT_EXIST\x10\x01\x12\x1a\n\x16LOCK_BELONGS_TO_OTHERS\x10\x02\x12\x12\n\x0eINTERNAL_ERROR\x10\x03\"(\n\x11WorkflowReference\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\"\\\n\x12GetWorkflowRequest\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12\x15\n\rworkflow_type\x18\x02 \x01(\t\x12\x1a\n\x12workflow_component\x18\x03 \x01(\t\"\xbb\x01\n\x13GetWorkflowResponse\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12\x12\n\nstart_time\x18\x02 \x01(\x03\x12J\n\x08metadata\x18\x03 \x03(\x0b\x32\x38.dapr.proto.runtime.v1.GetWorkflowResponse.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xfe\x01\n\x14StartWorkflowRequest\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12\x1a\n\x12workflow_component\x18\x02 \x01(\t\x12\x15\n\rworkflow_name\x18\x03 \x01(\t\x12I\n\x07options\x18\x04 \x03(\x0b\x32\x38.dapr.proto.runtime.v1.StartWorkflowRequest.OptionsEntry\x12#\n\x05input\x18\x05 \x01(\x0b\x32\x14.google.protobuf.Any\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"K\n\x18TerminateWorkflowRequest\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12\x1a\n\x12workflow_component\x18\x02 \x01(\t\"\x1b\n\x19TerminateWorkflowResponse2\x8b\x1a\n\x04\x44\x61pr\x12\x64\n\rInvokeService\x12+.dapr.proto.runtime.v1.InvokeServiceRequest\x1a$.dapr.proto.common.v1.InvokeResponse\"\x00\x12]\n\x08GetState\x12&.dapr.proto.runtime.v1.GetStateRequest\x1a\'.dapr.proto.runtime.v1.GetStateResponse\"\x00\x12i\n\x0cGetBulkState\x12*.dapr.proto.runtime.v1.GetBulkStateRequest\x1a+.dapr.proto.runtime.v1.GetBulkStateResponse\"\x00\x12N\n\tSaveState\x12\'.dapr.proto.runtime.v1.SaveStateRequest\x1a\x16.google.protobuf.Empty\"\x00\x12i\n\x10QueryStateAlpha1\x12(.dapr.proto.runtime.v1.QueryStateRequest\x1a).dapr.proto.runtime.v1.QueryStateResponse\"\x00\x12R\n\x0b\x44\x65leteState\x12).dapr.proto.runtime.v1.DeleteStateRequest\x1a\x16.google.protobuf.Empty\"\x00\x12Z\n\x0f\x44\x65leteBulkState\x12-.dapr.proto.runtime.v1.DeleteBulkStateRequest\x1a\x16.google.protobuf.Empty\"\x00\x12j\n\x17\x45xecuteStateTransaction\x12\x35.dapr.proto.runtime.v1.ExecuteStateTransactionRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x0cPublishEvent\x12*.dapr.proto.runtime.v1.PublishEventRequest\x1a\x16.google.protobuf.Empty\"\x00\x12q\n\x16\x42ulkPublishEventAlpha1\x12).dapr.proto.runtime.v1.BulkPublishRequest\x1a*.dapr.proto.runtime.v1.BulkPublishResponse\"\x00\x12l\n\rInvokeBinding\x12+.dapr.proto.runtime.v1.InvokeBindingRequest\x1a,.dapr.proto.runtime.v1.InvokeBindingResponse\"\x00\x12`\n\tGetSecret\x12\'.dapr.proto.runtime.v1.GetSecretRequest\x1a(.dapr.proto.runtime.v1.GetSecretResponse\"\x00\x12l\n\rGetBulkSecret\x12+.dapr.proto.runtime.v1.GetBulkSecretRequest\x1a,.dapr.proto.runtime.v1.GetBulkSecretResponse\"\x00\x12`\n\x12RegisterActorTimer\x12\x30.dapr.proto.runtime.v1.RegisterActorTimerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x64\n\x14UnregisterActorTimer\x12\x32.dapr.proto.runtime.v1.UnregisterActorTimerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x66\n\x15RegisterActorReminder\x12\x33.dapr.proto.runtime.v1.RegisterActorReminderRequest\x1a\x16.google.protobuf.Empty\"\x00\x12j\n\x17UnregisterActorReminder\x12\x35.dapr.proto.runtime.v1.UnregisterActorReminderRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x62\n\x13RenameActorReminder\x12\x31.dapr.proto.runtime.v1.RenameActorReminderRequest\x1a\x16.google.protobuf.Empty\"\x00\x12l\n\rGetActorState\x12+.dapr.proto.runtime.v1.GetActorStateRequest\x1a,.dapr.proto.runtime.v1.GetActorStateResponse\"\x00\x12t\n\x1c\x45xecuteActorStateTransaction\x12:.dapr.proto.runtime.v1.ExecuteActorStateTransactionRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x66\n\x0bInvokeActor\x12).dapr.proto.runtime.v1.InvokeActorRequest\x1a*.dapr.proto.runtime.v1.InvokeActorResponse\"\x00\x12{\n\x16GetConfigurationAlpha1\x12..dapr.proto.runtime.v1.GetConfigurationRequest\x1a/.dapr.proto.runtime.v1.GetConfigurationResponse\"\x00\x12\x8f\x01\n\x1cSubscribeConfigurationAlpha1\x12\x34.dapr.proto.runtime.v1.SubscribeConfigurationRequest\x1a\x35.dapr.proto.runtime.v1.SubscribeConfigurationResponse\"\x00\x30\x01\x12\x93\x01\n\x1eUnsubscribeConfigurationAlpha1\x12\x36.dapr.proto.runtime.v1.UnsubscribeConfigurationRequest\x1a\x37.dapr.proto.runtime.v1.UnsubscribeConfigurationResponse\"\x00\x12`\n\rTryLockAlpha1\x12%.dapr.proto.runtime.v1.TryLockRequest\x1a&.dapr.proto.runtime.v1.TryLockResponse\"\x00\x12]\n\x0cUnlockAlpha1\x12$.dapr.proto.runtime.v1.UnlockRequest\x1a%.dapr.proto.runtime.v1.UnlockResponse\"\x00\x12S\n\x0bGetMetadata\x12\x16.google.protobuf.Empty\x1a*.dapr.proto.runtime.v1.GetMetadataResponse\"\x00\x12R\n\x0bSetMetadata\x12).dapr.proto.runtime.v1.SetMetadataRequest\x1a\x16.google.protobuf.Empty\"\x00\x12n\n\x13StartWorkflowAlpha1\x12+.dapr.proto.runtime.v1.StartWorkflowRequest\x1a(.dapr.proto.runtime.v1.WorkflowReference\"\x00\x12l\n\x11GetWorkflowAlpha1\x12).dapr.proto.runtime.v1.GetWorkflowRequest\x1a*.dapr.proto.runtime.v1.GetWorkflowResponse\"\x00\x12~\n\x17TerminateWorkflowAlpha1\x12/.dapr.proto.runtime.v1.TerminateWorkflowRequest\x1a\x30.dapr.proto.runtime.v1.TerminateWorkflowResponse\"\x00\x12<\n\x08Shutdown\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x42i\n\nio.dapr.v1B\nDaprProtosZ1github.com/dapr/dapr/pkg/proto/runtime/v1;runtime\xaa\x02\x1b\x44\x61pr.Client.Autogen.Grpc.v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n dapr/proto/runtime/v1/dapr.proto\x12\x15\x64\x61pr.proto.runtime.v1\x1a\x19google/protobuf/any.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a!dapr/proto/common/v1/common.proto\"X\n\x14InvokeServiceRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x34\n\x07message\x18\x03 \x01(\x0b\x32#.dapr.proto.common.v1.InvokeRequest\"\xf5\x01\n\x0fGetStateRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12H\n\x0b\x63onsistency\x18\x03 \x01(\x0e\x32\x33.dapr.proto.common.v1.StateOptions.StateConsistency\x12\x46\n\x08metadata\x18\x04 \x03(\x0b\x32\x34.dapr.proto.runtime.v1.GetStateRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc9\x01\n\x13GetBulkStateRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12\x13\n\x0bparallelism\x18\x03 \x01(\x05\x12J\n\x08metadata\x18\x04 \x03(\x0b\x32\x38.dapr.proto.runtime.v1.GetBulkStateRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"K\n\x14GetBulkStateResponse\x12\x33\n\x05items\x18\x01 \x03(\x0b\x32$.dapr.proto.runtime.v1.BulkStateItem\"\xbe\x01\n\rBulkStateItem\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x0c\n\x04\x65tag\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\x12\x44\n\x08metadata\x18\x05 \x03(\x0b\x32\x32.dapr.proto.runtime.v1.BulkStateItem.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa8\x01\n\x10GetStateResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0c\n\x04\x65tag\x18\x02 \x01(\t\x12G\n\x08metadata\x18\x03 \x03(\x0b\x32\x35.dapr.proto.runtime.v1.GetStateResponse.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x90\x02\n\x12\x44\x65leteStateRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12(\n\x04\x65tag\x18\x03 \x01(\x0b\x32\x1a.dapr.proto.common.v1.Etag\x12\x33\n\x07options\x18\x04 \x01(\x0b\x32\".dapr.proto.common.v1.StateOptions\x12I\n\x08metadata\x18\x05 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.DeleteStateRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"]\n\x16\x44\x65leteBulkStateRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12/\n\x06states\x18\x02 \x03(\x0b\x32\x1f.dapr.proto.common.v1.StateItem\"W\n\x10SaveStateRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12/\n\x06states\x18\x02 \x03(\x0b\x32\x1f.dapr.proto.common.v1.StateItem\"\xbc\x01\n\x11QueryStateRequest\x12\x1d\n\nstore_name\x18\x01 \x01(\tR\tstoreName\x12\r\n\x05query\x18\x02 \x01(\t\x12H\n\x08metadata\x18\x03 \x03(\x0b\x32\x36.dapr.proto.runtime.v1.QueryStateRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"H\n\x0eQueryStateItem\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x0c\n\x04\x65tag\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"\xd7\x01\n\x12QueryStateResponse\x12\x36\n\x07results\x18\x01 \x03(\x0b\x32%.dapr.proto.runtime.v1.QueryStateItem\x12\r\n\x05token\x18\x02 \x01(\t\x12I\n\x08metadata\x18\x03 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.QueryStateResponse.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xdf\x01\n\x13PublishEventRequest\x12\x13\n\x0bpubsub_name\x18\x01 \x01(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\x12\x19\n\x11\x64\x61ta_content_type\x18\x04 \x01(\t\x12J\n\x08metadata\x18\x05 \x03(\x0b\x32\x38.dapr.proto.runtime.v1.PublishEventRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xf5\x01\n\x12\x42ulkPublishRequest\x12\x13\n\x0bpubsub_name\x18\x01 \x01(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12?\n\x07\x65ntries\x18\x03 \x03(\x0b\x32..dapr.proto.runtime.v1.BulkPublishRequestEntry\x12I\n\x08metadata\x18\x04 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.BulkPublishRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xd1\x01\n\x17\x42ulkPublishRequestEntry\x12\x10\n\x08\x65ntry_id\x18\x01 \x01(\t\x12\r\n\x05\x65vent\x18\x02 \x01(\x0c\x12\x14\n\x0c\x63ontent_type\x18\x03 \x01(\t\x12N\n\x08metadata\x18\x04 \x03(\x0b\x32<.dapr.proto.runtime.v1.BulkPublishRequestEntry.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"c\n\x13\x42ulkPublishResponse\x12L\n\rfailedEntries\x18\x01 \x03(\x0b\x32\x35.dapr.proto.runtime.v1.BulkPublishResponseFailedEntry\"A\n\x1e\x42ulkPublishResponseFailedEntry\x12\x10\n\x08\x65ntry_id\x18\x01 \x01(\t\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"\xc3\x01\n\x14InvokeBindingRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12K\n\x08metadata\x18\x03 \x03(\x0b\x32\x39.dapr.proto.runtime.v1.InvokeBindingRequest.MetadataEntry\x12\x11\n\toperation\x18\x04 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa4\x01\n\x15InvokeBindingResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12L\n\x08metadata\x18\x02 \x03(\x0b\x32:.dapr.proto.runtime.v1.InvokeBindingResponse.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb8\x01\n\x10GetSecretRequest\x12\x1d\n\nstore_name\x18\x01 \x01(\tR\tstoreName\x12\x0b\n\x03key\x18\x02 \x01(\t\x12G\n\x08metadata\x18\x03 \x03(\x0b\x32\x35.dapr.proto.runtime.v1.GetSecretRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x82\x01\n\x11GetSecretResponse\x12@\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x32.dapr.proto.runtime.v1.GetSecretResponse.DataEntry\x1a+\n\tDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb3\x01\n\x14GetBulkSecretRequest\x12\x1d\n\nstore_name\x18\x01 \x01(\tR\tstoreName\x12K\n\x08metadata\x18\x02 \x03(\x0b\x32\x39.dapr.proto.runtime.v1.GetBulkSecretRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x85\x01\n\x0eSecretResponse\x12\x43\n\x07secrets\x18\x01 \x03(\x0b\x32\x32.dapr.proto.runtime.v1.SecretResponse.SecretsEntry\x1a.\n\x0cSecretsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb1\x01\n\x15GetBulkSecretResponse\x12\x44\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x36.dapr.proto.runtime.v1.GetBulkSecretResponse.DataEntry\x1aR\n\tDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.dapr.proto.runtime.v1.SecretResponse:\x02\x38\x01\"f\n\x1bTransactionalStateOperation\x12\x15\n\roperationType\x18\x01 \x01(\t\x12\x30\n\x07request\x18\x02 \x01(\x0b\x32\x1f.dapr.proto.common.v1.StateItem\"\x83\x02\n\x1e\x45xecuteStateTransactionRequest\x12\x11\n\tstoreName\x18\x01 \x01(\t\x12\x46\n\noperations\x18\x02 \x03(\x0b\x32\x32.dapr.proto.runtime.v1.TransactionalStateOperation\x12U\n\x08metadata\x18\x03 \x03(\x0b\x32\x43.dapr.proto.runtime.v1.ExecuteStateTransactionRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9e\x01\n\x19RegisterActorTimerRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08\x64ue_time\x18\x04 \x01(\t\x12\x0e\n\x06period\x18\x05 \x01(\t\x12\x10\n\x08\x63\x61llback\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\x0c\x12\x0b\n\x03ttl\x18\x08 \x01(\t\"Q\n\x1bUnregisterActorTimerRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"\x8f\x01\n\x1cRegisterActorReminderRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08\x64ue_time\x18\x04 \x01(\t\x12\x0e\n\x06period\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12\x0b\n\x03ttl\x18\x07 \x01(\t\"T\n\x1eUnregisterActorReminderRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"f\n\x1aRenameActorReminderRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x10\n\x08old_name\x18\x03 \x01(\t\x12\x10\n\x08new_name\x18\x04 \x01(\t\"I\n\x14GetActorStateRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\"%\n\x15GetActorStateResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\x98\x01\n#ExecuteActorStateTransactionRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12K\n\noperations\x18\x03 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.TransactionalActorStateOperation\"\xf5\x01\n TransactionalActorStateOperation\x12\x15\n\roperationType\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12#\n\x05value\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12W\n\x08metadata\x18\x04 \x03(\x0b\x32\x45.dapr.proto.runtime.v1.TransactionalActorStateOperation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xd4\x01\n\x12InvokeActorRequest\x12\x12\n\nactor_type\x18\x01 \x01(\t\x12\x10\n\x08\x61\x63tor_id\x18\x02 \x01(\t\x12\x0e\n\x06method\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12I\n\x08metadata\x18\x05 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.InvokeActorRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"#\n\x13InvokeActorResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\x8c\x03\n\x13GetMetadataResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x45\n\x13\x61\x63tive_actors_count\x18\x02 \x03(\x0b\x32(.dapr.proto.runtime.v1.ActiveActorsCount\x12J\n\x15registered_components\x18\x03 \x03(\x0b\x32+.dapr.proto.runtime.v1.RegisteredComponents\x12[\n\x11\x65xtended_metadata\x18\x04 \x03(\x0b\x32@.dapr.proto.runtime.v1.GetMetadataResponse.ExtendedMetadataEntry\x12@\n\rsubscriptions\x18\x05 \x03(\x0b\x32).dapr.proto.runtime.v1.PubsubSubscription\x1a\x37\n\x15\x45xtendedMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"0\n\x11\x41\x63tiveActorsCount\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\"Y\n\x14RegisteredComponents\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x14\n\x0c\x63\x61pabilities\x18\x04 \x03(\t\"\x8e\x02\n\x12PubsubSubscription\x12\x13\n\x0bpubsub_name\x18\x01 \x01(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12I\n\x08metadata\x18\x03 \x03(\x0b\x32\x37.dapr.proto.runtime.v1.PubsubSubscription.MetadataEntry\x12=\n\x05rules\x18\x04 \x01(\x0b\x32..dapr.proto.runtime.v1.PubsubSubscriptionRules\x12\x19\n\x11\x64\x65\x61\x64_letter_topic\x18\x05 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"W\n\x17PubsubSubscriptionRules\x12<\n\x05rules\x18\x01 \x03(\x0b\x32-.dapr.proto.runtime.v1.PubsubSubscriptionRule\"5\n\x16PubsubSubscriptionRule\x12\r\n\x05match\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"0\n\x12SetMetadataRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xbc\x01\n\x17GetConfigurationRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12N\n\x08metadata\x18\x03 \x03(\x0b\x32<.dapr.proto.runtime.v1.GetConfigurationRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xbc\x01\n\x18GetConfigurationResponse\x12I\n\x05items\x18\x01 \x03(\x0b\x32:.dapr.proto.runtime.v1.GetConfigurationResponse.ItemsEntry\x1aU\n\nItemsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.dapr.proto.common.v1.ConfigurationItem:\x02\x38\x01\"\xc8\x01\n\x1dSubscribeConfigurationRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12T\n\x08metadata\x18\x03 \x03(\x0b\x32\x42.dapr.proto.runtime.v1.SubscribeConfigurationRequest.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"A\n\x1fUnsubscribeConfigurationRequest\x12\x12\n\nstore_name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"\xd4\x01\n\x1eSubscribeConfigurationResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.dapr.proto.runtime.v1.SubscribeConfigurationResponse.ItemsEntry\x1aU\n\nItemsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.dapr.proto.common.v1.ConfigurationItem:\x02\x38\x01\"?\n UnsubscribeConfigurationResponse\x12\n\n\x02ok\x18\x01 \x01(\x08\x12\x0f\n\x07message\x18\x02 \x01(\t\"\x9b\x01\n\x0eTryLockRequest\x12\x1d\n\nstore_name\x18\x01 \x01(\tR\tstoreName\x12\x1f\n\x0bresource_id\x18\x02 \x01(\tR\nresourceId\x12\x1d\n\nlock_owner\x18\x03 \x01(\tR\tlockOwner\x12*\n\x11\x65xpiry_in_seconds\x18\x04 \x01(\x05R\x0f\x65xpiryInSeconds\"\"\n\x0fTryLockResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"n\n\rUnlockRequest\x12\x1d\n\nstore_name\x18\x01 \x01(\tR\tstoreName\x12\x1f\n\x0bresource_id\x18\x02 \x01(\tR\nresourceId\x12\x1d\n\nlock_owner\x18\x03 \x01(\tR\tlockOwner\"\xae\x01\n\x0eUnlockResponse\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.dapr.proto.runtime.v1.UnlockResponse.Status\"^\n\x06Status\x12\x0b\n\x07SUCCESS\x10\x00\x12\x17\n\x13LOCK_DOES_NOT_EXIST\x10\x01\x12\x1a\n\x16LOCK_BELONGS_TO_OTHERS\x10\x02\x12\x12\n\x0eINTERNAL_ERROR\x10\x03\"\xbc\x01\n\x19SubtleGetKeyAlpha1Request\x12%\n\x0e\x63omponent_name\x18\x01 \x01(\tR\rcomponentName\x12\x0c\n\x04name\x18\x02 \x01(\t\x12J\n\x06\x66ormat\x18\x03 \x01(\x0e\x32:.dapr.proto.runtime.v1.SubtleGetKeyAlpha1Request.KeyFormat\"\x1e\n\tKeyFormat\x12\x07\n\x03PEM\x10\x00\x12\x08\n\x04JSON\x10\x01\"I\n\x1aSubtleGetKeyAlpha1Response\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\npublic_key\x18\x02 \x01(\tR\tpublicKey\"\xbc\x01\n\x1aSubtleEncryptAlpha1Request\x12%\n\x0e\x63omponent_name\x18\x01 \x01(\tR\rcomponentName\x12\x11\n\tplaintext\x18\x02 \x01(\x0c\x12\x11\n\talgorithm\x18\x03 \x01(\t\x12\x19\n\x08key_name\x18\x04 \x01(\tR\x07keyName\x12\r\n\x05nonce\x18\x05 \x01(\x0c\x12\'\n\x0f\x61ssociated_data\x18\x06 \x01(\x0cR\x0e\x61ssociatedData\">\n\x1bSubtleEncryptAlpha1Response\x12\x12\n\nciphertext\x18\x01 \x01(\x0c\x12\x0b\n\x03tag\x18\x02 \x01(\x0c\"\xca\x01\n\x1aSubtleDecryptAlpha1Request\x12%\n\x0e\x63omponent_name\x18\x01 \x01(\tR\rcomponentName\x12\x12\n\nciphertext\x18\x02 \x01(\x0c\x12\x11\n\talgorithm\x18\x03 \x01(\t\x12\x19\n\x08key_name\x18\x04 \x01(\tR\x07keyName\x12\r\n\x05nonce\x18\x05 \x01(\x0c\x12\x0b\n\x03tag\x18\x06 \x01(\x0c\x12\'\n\x0f\x61ssociated_data\x18\x07 \x01(\x0cR\x0e\x61ssociatedData\"0\n\x1bSubtleDecryptAlpha1Response\x12\x11\n\tplaintext\x18\x01 \x01(\x0c\"\xce\x01\n\x1aSubtleWrapKeyAlpha1Request\x12%\n\x0e\x63omponent_name\x18\x01 \x01(\tR\rcomponentName\x12#\n\rplaintext_key\x18\x02 \x01(\x0cR\x0cplaintextKey\x12\x11\n\talgorithm\x18\x03 \x01(\t\x12\x19\n\x08key_name\x18\x04 \x01(\tR\x07keyName\x12\r\n\x05nonce\x18\x05 \x01(\x0c\x12\'\n\x0f\x61ssociated_data\x18\x06 \x01(\x0cR\x0e\x61ssociatedData\"K\n\x1bSubtleWrapKeyAlpha1Response\x12\x1f\n\x0bwrapped_key\x18\x01 \x01(\x0cR\nwrappedKey\x12\x0b\n\x03tag\x18\x02 \x01(\x0c\"\xd9\x01\n\x1cSubtleUnwrapKeyAlpha1Request\x12%\n\x0e\x63omponent_name\x18\x01 \x01(\tR\rcomponentName\x12\x1f\n\x0bwrapped_key\x18\x02 \x01(\x0cR\nwrappedKey\x12\x11\n\talgorithm\x18\x03 \x01(\t\x12\x19\n\x08key_name\x18\x04 \x01(\tR\x07keyName\x12\r\n\x05nonce\x18\x05 \x01(\x0c\x12\x0b\n\x03tag\x18\x06 \x01(\x0c\x12\'\n\x0f\x61ssociated_data\x18\x07 \x01(\x0cR\x0e\x61ssociatedData\"D\n\x1dSubtleUnwrapKeyAlpha1Response\x12#\n\rplaintext_key\x18\x01 \x01(\x0cR\x0cplaintextKey\"~\n\x17SubtleSignAlpha1Request\x12%\n\x0e\x63omponent_name\x18\x01 \x01(\tR\rcomponentName\x12\x0e\n\x06\x64igest\x18\x02 \x01(\x0c\x12\x11\n\talgorithm\x18\x03 \x01(\t\x12\x19\n\x08key_name\x18\x04 \x01(\tR\x07keyName\"-\n\x18SubtleSignAlpha1Response\x12\x11\n\tsignature\x18\x01 \x01(\x0c\"\x93\x01\n\x19SubtleVerifyAlpha1Request\x12%\n\x0e\x63omponent_name\x18\x01 \x01(\tR\rcomponentName\x12\x0e\n\x06\x64igest\x18\x02 \x01(\x0c\x12\x11\n\talgorithm\x18\x03 \x01(\t\x12\x19\n\x08key_name\x18\x04 \x01(\tR\x07keyName\x12\x11\n\tsignature\x18\x05 \x01(\x0c\"+\n\x1aSubtleVerifyAlpha1Response\x12\r\n\x05valid\x18\x01 \x01(\x08\"4\n\x11WorkflowReference\x12\x1f\n\x0binstance_id\x18\x01 \x01(\tR\ninstanceId\"\x89\x01\n\x12GetWorkflowRequest\x12\x1f\n\x0binstance_id\x18\x01 \x01(\tR\ninstanceId\x12-\n\x12workflow_component\x18\x02 \x01(\tR\x11workflowComponent\x12#\n\rworkflow_name\x18\x03 \x01(\tR\x0cworkflowName\"\xbb\x01\n\x13GetWorkflowResponse\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12\x12\n\nstart_time\x18\x02 \x01(\x03\x12J\n\x08metadata\x18\x03 \x03(\x0b\x32\x38.dapr.proto.runtime.v1.GetWorkflowResponse.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x95\x02\n\x14StartWorkflowRequest\x12\x1f\n\x0binstance_id\x18\x01 \x01(\tR\ninstanceId\x12-\n\x12workflow_component\x18\x02 \x01(\tR\x11workflowComponent\x12#\n\rworkflow_name\x18\x03 \x01(\tR\x0cworkflowName\x12I\n\x07options\x18\x04 \x03(\x0b\x32\x38.dapr.proto.runtime.v1.StartWorkflowRequest.OptionsEntry\x12\r\n\x05input\x18\x05 \x01(\x0c\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"i\n\x17WorkflowActivityRequest\x12\x1f\n\x0binstance_id\x18\x01 \x01(\tR\ninstanceId\x12-\n\x12workflow_component\x18\x02 \x01(\tR\x11workflowComponent\"\x1a\n\x18WorkflowActivityResponse\"\x99\x01\n\x19RaiseEventWorkflowRequest\x12\x1f\n\x0binstance_id\x18\x01 \x01(\tR\ninstanceId\x12-\n\x12workflow_component\x18\x02 \x01(\tR\x11workflowComponent\x12\x1d\n\nevent_name\x18\x03 \x01(\tR\teventName\x12\r\n\x05input\x18\x04 \x01(\x0c\"\x1c\n\x1aRaiseEventWorkflowResponse2\xff&\n\x04\x44\x61pr\x12\x64\n\rInvokeService\x12+.dapr.proto.runtime.v1.InvokeServiceRequest\x1a$.dapr.proto.common.v1.InvokeResponse\"\x00\x12]\n\x08GetState\x12&.dapr.proto.runtime.v1.GetStateRequest\x1a\'.dapr.proto.runtime.v1.GetStateResponse\"\x00\x12i\n\x0cGetBulkState\x12*.dapr.proto.runtime.v1.GetBulkStateRequest\x1a+.dapr.proto.runtime.v1.GetBulkStateResponse\"\x00\x12N\n\tSaveState\x12\'.dapr.proto.runtime.v1.SaveStateRequest\x1a\x16.google.protobuf.Empty\"\x00\x12i\n\x10QueryStateAlpha1\x12(.dapr.proto.runtime.v1.QueryStateRequest\x1a).dapr.proto.runtime.v1.QueryStateResponse\"\x00\x12R\n\x0b\x44\x65leteState\x12).dapr.proto.runtime.v1.DeleteStateRequest\x1a\x16.google.protobuf.Empty\"\x00\x12Z\n\x0f\x44\x65leteBulkState\x12-.dapr.proto.runtime.v1.DeleteBulkStateRequest\x1a\x16.google.protobuf.Empty\"\x00\x12j\n\x17\x45xecuteStateTransaction\x12\x35.dapr.proto.runtime.v1.ExecuteStateTransactionRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x0cPublishEvent\x12*.dapr.proto.runtime.v1.PublishEventRequest\x1a\x16.google.protobuf.Empty\"\x00\x12q\n\x16\x42ulkPublishEventAlpha1\x12).dapr.proto.runtime.v1.BulkPublishRequest\x1a*.dapr.proto.runtime.v1.BulkPublishResponse\"\x00\x12l\n\rInvokeBinding\x12+.dapr.proto.runtime.v1.InvokeBindingRequest\x1a,.dapr.proto.runtime.v1.InvokeBindingResponse\"\x00\x12`\n\tGetSecret\x12\'.dapr.proto.runtime.v1.GetSecretRequest\x1a(.dapr.proto.runtime.v1.GetSecretResponse\"\x00\x12l\n\rGetBulkSecret\x12+.dapr.proto.runtime.v1.GetBulkSecretRequest\x1a,.dapr.proto.runtime.v1.GetBulkSecretResponse\"\x00\x12`\n\x12RegisterActorTimer\x12\x30.dapr.proto.runtime.v1.RegisterActorTimerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x64\n\x14UnregisterActorTimer\x12\x32.dapr.proto.runtime.v1.UnregisterActorTimerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x66\n\x15RegisterActorReminder\x12\x33.dapr.proto.runtime.v1.RegisterActorReminderRequest\x1a\x16.google.protobuf.Empty\"\x00\x12j\n\x17UnregisterActorReminder\x12\x35.dapr.proto.runtime.v1.UnregisterActorReminderRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x62\n\x13RenameActorReminder\x12\x31.dapr.proto.runtime.v1.RenameActorReminderRequest\x1a\x16.google.protobuf.Empty\"\x00\x12l\n\rGetActorState\x12+.dapr.proto.runtime.v1.GetActorStateRequest\x1a,.dapr.proto.runtime.v1.GetActorStateResponse\"\x00\x12t\n\x1c\x45xecuteActorStateTransaction\x12:.dapr.proto.runtime.v1.ExecuteActorStateTransactionRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x66\n\x0bInvokeActor\x12).dapr.proto.runtime.v1.InvokeActorRequest\x1a*.dapr.proto.runtime.v1.InvokeActorResponse\"\x00\x12{\n\x16GetConfigurationAlpha1\x12..dapr.proto.runtime.v1.GetConfigurationRequest\x1a/.dapr.proto.runtime.v1.GetConfigurationResponse\"\x00\x12u\n\x10GetConfiguration\x12..dapr.proto.runtime.v1.GetConfigurationRequest\x1a/.dapr.proto.runtime.v1.GetConfigurationResponse\"\x00\x12\x8f\x01\n\x1cSubscribeConfigurationAlpha1\x12\x34.dapr.proto.runtime.v1.SubscribeConfigurationRequest\x1a\x35.dapr.proto.runtime.v1.SubscribeConfigurationResponse\"\x00\x30\x01\x12\x89\x01\n\x16SubscribeConfiguration\x12\x34.dapr.proto.runtime.v1.SubscribeConfigurationRequest\x1a\x35.dapr.proto.runtime.v1.SubscribeConfigurationResponse\"\x00\x30\x01\x12\x93\x01\n\x1eUnsubscribeConfigurationAlpha1\x12\x36.dapr.proto.runtime.v1.UnsubscribeConfigurationRequest\x1a\x37.dapr.proto.runtime.v1.UnsubscribeConfigurationResponse\"\x00\x12\x8d\x01\n\x18UnsubscribeConfiguration\x12\x36.dapr.proto.runtime.v1.UnsubscribeConfigurationRequest\x1a\x37.dapr.proto.runtime.v1.UnsubscribeConfigurationResponse\"\x00\x12`\n\rTryLockAlpha1\x12%.dapr.proto.runtime.v1.TryLockRequest\x1a&.dapr.proto.runtime.v1.TryLockResponse\"\x00\x12]\n\x0cUnlockAlpha1\x12$.dapr.proto.runtime.v1.UnlockRequest\x1a%.dapr.proto.runtime.v1.UnlockResponse\"\x00\x12S\n\x0bGetMetadata\x12\x16.google.protobuf.Empty\x1a*.dapr.proto.runtime.v1.GetMetadataResponse\"\x00\x12R\n\x0bSetMetadata\x12).dapr.proto.runtime.v1.SetMetadataRequest\x1a\x16.google.protobuf.Empty\"\x00\x12y\n\x12SubtleGetKeyAlpha1\x12\x30.dapr.proto.runtime.v1.SubtleGetKeyAlpha1Request\x1a\x31.dapr.proto.runtime.v1.SubtleGetKeyAlpha1Response\x12|\n\x13SubtleEncryptAlpha1\x12\x31.dapr.proto.runtime.v1.SubtleEncryptAlpha1Request\x1a\x32.dapr.proto.runtime.v1.SubtleEncryptAlpha1Response\x12|\n\x13SubtleDecryptAlpha1\x12\x31.dapr.proto.runtime.v1.SubtleDecryptAlpha1Request\x1a\x32.dapr.proto.runtime.v1.SubtleDecryptAlpha1Response\x12|\n\x13SubtleWrapKeyAlpha1\x12\x31.dapr.proto.runtime.v1.SubtleWrapKeyAlpha1Request\x1a\x32.dapr.proto.runtime.v1.SubtleWrapKeyAlpha1Response\x12\x82\x01\n\x15SubtleUnwrapKeyAlpha1\x12\x33.dapr.proto.runtime.v1.SubtleUnwrapKeyAlpha1Request\x1a\x34.dapr.proto.runtime.v1.SubtleUnwrapKeyAlpha1Response\x12s\n\x10SubtleSignAlpha1\x12..dapr.proto.runtime.v1.SubtleSignAlpha1Request\x1a/.dapr.proto.runtime.v1.SubtleSignAlpha1Response\x12y\n\x12SubtleVerifyAlpha1\x12\x30.dapr.proto.runtime.v1.SubtleVerifyAlpha1Request\x1a\x31.dapr.proto.runtime.v1.SubtleVerifyAlpha1Response\x12n\n\x13StartWorkflowAlpha1\x12+.dapr.proto.runtime.v1.StartWorkflowRequest\x1a(.dapr.proto.runtime.v1.WorkflowReference\"\x00\x12l\n\x11GetWorkflowAlpha1\x12).dapr.proto.runtime.v1.GetWorkflowRequest\x1a*.dapr.proto.runtime.v1.GetWorkflowResponse\"\x00\x12|\n\x17TerminateWorkflowAlpha1\x12..dapr.proto.runtime.v1.WorkflowActivityRequest\x1a/.dapr.proto.runtime.v1.WorkflowActivityResponse\"\x00\x12x\n\x13PauseWorkflowAlpha1\x12..dapr.proto.runtime.v1.WorkflowActivityRequest\x1a/.dapr.proto.runtime.v1.WorkflowActivityResponse\"\x00\x12y\n\x14ResumeWorkflowAlpha1\x12..dapr.proto.runtime.v1.WorkflowActivityRequest\x1a/.dapr.proto.runtime.v1.WorkflowActivityResponse\"\x00\x12\x81\x01\n\x18RaiseEventWorkflowAlpha1\x12\x30.dapr.proto.runtime.v1.RaiseEventWorkflowRequest\x1a\x31.dapr.proto.runtime.v1.RaiseEventWorkflowResponse\"\x00\x12<\n\x08Shutdown\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x42i\n\nio.dapr.v1B\nDaprProtosZ1github.com/dapr/dapr/pkg/proto/runtime/v1;runtime\xaa\x02\x1b\x44\x61pr.Client.Autogen.Grpc.v1b\x06proto3')
 
 
 
 _INVOKESERVICEREQUEST = DESCRIPTOR.message_types_by_name['InvokeServiceRequest']
 _GETSTATEREQUEST = DESCRIPTOR.message_types_by_name['GetStateRequest']
 _GETSTATEREQUEST_METADATAENTRY = _GETSTATEREQUEST.nested_types_by_name['MetadataEntry']
 _GETBULKSTATEREQUEST = DESCRIPTOR.message_types_by_name['GetBulkStateRequest']
@@ -44,15 +43,15 @@
 _PUBLISHEVENTREQUEST = DESCRIPTOR.message_types_by_name['PublishEventRequest']
 _PUBLISHEVENTREQUEST_METADATAENTRY = _PUBLISHEVENTREQUEST.nested_types_by_name['MetadataEntry']
 _BULKPUBLISHREQUEST = DESCRIPTOR.message_types_by_name['BulkPublishRequest']
 _BULKPUBLISHREQUEST_METADATAENTRY = _BULKPUBLISHREQUEST.nested_types_by_name['MetadataEntry']
 _BULKPUBLISHREQUESTENTRY = DESCRIPTOR.message_types_by_name['BulkPublishRequestEntry']
 _BULKPUBLISHREQUESTENTRY_METADATAENTRY = _BULKPUBLISHREQUESTENTRY.nested_types_by_name['MetadataEntry']
 _BULKPUBLISHRESPONSE = DESCRIPTOR.message_types_by_name['BulkPublishResponse']
-_BULKPUBLISHRESPONSEENTRY = DESCRIPTOR.message_types_by_name['BulkPublishResponseEntry']
+_BULKPUBLISHRESPONSEFAILEDENTRY = DESCRIPTOR.message_types_by_name['BulkPublishResponseFailedEntry']
 _INVOKEBINDINGREQUEST = DESCRIPTOR.message_types_by_name['InvokeBindingRequest']
 _INVOKEBINDINGREQUEST_METADATAENTRY = _INVOKEBINDINGREQUEST.nested_types_by_name['MetadataEntry']
 _INVOKEBINDINGRESPONSE = DESCRIPTOR.message_types_by_name['InvokeBindingResponse']
 _INVOKEBINDINGRESPONSE_METADATAENTRY = _INVOKEBINDINGRESPONSE.nested_types_by_name['MetadataEntry']
 _GETSECRETREQUEST = DESCRIPTOR.message_types_by_name['GetSecretRequest']
 _GETSECRETREQUEST_METADATAENTRY = _GETSECRETREQUEST.nested_types_by_name['MetadataEntry']
 _GETSECRETRESPONSE = DESCRIPTOR.message_types_by_name['GetSecretResponse']
@@ -71,14 +70,15 @@
 _REGISTERACTORREMINDERREQUEST = DESCRIPTOR.message_types_by_name['RegisterActorReminderRequest']
 _UNREGISTERACTORREMINDERREQUEST = DESCRIPTOR.message_types_by_name['UnregisterActorReminderRequest']
 _RENAMEACTORREMINDERREQUEST = DESCRIPTOR.message_types_by_name['RenameActorReminderRequest']
 _GETACTORSTATEREQUEST = DESCRIPTOR.message_types_by_name['GetActorStateRequest']
 _GETACTORSTATERESPONSE = DESCRIPTOR.message_types_by_name['GetActorStateResponse']
 _EXECUTEACTORSTATETRANSACTIONREQUEST = DESCRIPTOR.message_types_by_name['ExecuteActorStateTransactionRequest']
 _TRANSACTIONALACTORSTATEOPERATION = DESCRIPTOR.message_types_by_name['TransactionalActorStateOperation']
+_TRANSACTIONALACTORSTATEOPERATION_METADATAENTRY = _TRANSACTIONALACTORSTATEOPERATION.nested_types_by_name['MetadataEntry']
 _INVOKEACTORREQUEST = DESCRIPTOR.message_types_by_name['InvokeActorRequest']
 _INVOKEACTORREQUEST_METADATAENTRY = _INVOKEACTORREQUEST.nested_types_by_name['MetadataEntry']
 _INVOKEACTORRESPONSE = DESCRIPTOR.message_types_by_name['InvokeActorResponse']
 _GETMETADATARESPONSE = DESCRIPTOR.message_types_by_name['GetMetadataResponse']
 _GETMETADATARESPONSE_EXTENDEDMETADATAENTRY = _GETMETADATARESPONSE.nested_types_by_name['ExtendedMetadataEntry']
 _ACTIVEACTORSCOUNT = DESCRIPTOR.message_types_by_name['ActiveActorsCount']
 _REGISTEREDCOMPONENTS = DESCRIPTOR.message_types_by_name['RegisteredComponents']
@@ -97,24 +97,40 @@
 _SUBSCRIBECONFIGURATIONRESPONSE = DESCRIPTOR.message_types_by_name['SubscribeConfigurationResponse']
 _SUBSCRIBECONFIGURATIONRESPONSE_ITEMSENTRY = _SUBSCRIBECONFIGURATIONRESPONSE.nested_types_by_name['ItemsEntry']
 _UNSUBSCRIBECONFIGURATIONRESPONSE = DESCRIPTOR.message_types_by_name['UnsubscribeConfigurationResponse']
 _TRYLOCKREQUEST = DESCRIPTOR.message_types_by_name['TryLockRequest']
 _TRYLOCKRESPONSE = DESCRIPTOR.message_types_by_name['TryLockResponse']
 _UNLOCKREQUEST = DESCRIPTOR.message_types_by_name['UnlockRequest']
 _UNLOCKRESPONSE = DESCRIPTOR.message_types_by_name['UnlockResponse']
+_SUBTLEGETKEYALPHA1REQUEST = DESCRIPTOR.message_types_by_name['SubtleGetKeyAlpha1Request']
+_SUBTLEGETKEYALPHA1RESPONSE = DESCRIPTOR.message_types_by_name['SubtleGetKeyAlpha1Response']
+_SUBTLEENCRYPTALPHA1REQUEST = DESCRIPTOR.message_types_by_name['SubtleEncryptAlpha1Request']
+_SUBTLEENCRYPTALPHA1RESPONSE = DESCRIPTOR.message_types_by_name['SubtleEncryptAlpha1Response']
+_SUBTLEDECRYPTALPHA1REQUEST = DESCRIPTOR.message_types_by_name['SubtleDecryptAlpha1Request']
+_SUBTLEDECRYPTALPHA1RESPONSE = DESCRIPTOR.message_types_by_name['SubtleDecryptAlpha1Response']
+_SUBTLEWRAPKEYALPHA1REQUEST = DESCRIPTOR.message_types_by_name['SubtleWrapKeyAlpha1Request']
+_SUBTLEWRAPKEYALPHA1RESPONSE = DESCRIPTOR.message_types_by_name['SubtleWrapKeyAlpha1Response']
+_SUBTLEUNWRAPKEYALPHA1REQUEST = DESCRIPTOR.message_types_by_name['SubtleUnwrapKeyAlpha1Request']
+_SUBTLEUNWRAPKEYALPHA1RESPONSE = DESCRIPTOR.message_types_by_name['SubtleUnwrapKeyAlpha1Response']
+_SUBTLESIGNALPHA1REQUEST = DESCRIPTOR.message_types_by_name['SubtleSignAlpha1Request']
+_SUBTLESIGNALPHA1RESPONSE = DESCRIPTOR.message_types_by_name['SubtleSignAlpha1Response']
+_SUBTLEVERIFYALPHA1REQUEST = DESCRIPTOR.message_types_by_name['SubtleVerifyAlpha1Request']
+_SUBTLEVERIFYALPHA1RESPONSE = DESCRIPTOR.message_types_by_name['SubtleVerifyAlpha1Response']
 _WORKFLOWREFERENCE = DESCRIPTOR.message_types_by_name['WorkflowReference']
 _GETWORKFLOWREQUEST = DESCRIPTOR.message_types_by_name['GetWorkflowRequest']
 _GETWORKFLOWRESPONSE = DESCRIPTOR.message_types_by_name['GetWorkflowResponse']
 _GETWORKFLOWRESPONSE_METADATAENTRY = _GETWORKFLOWRESPONSE.nested_types_by_name['MetadataEntry']
 _STARTWORKFLOWREQUEST = DESCRIPTOR.message_types_by_name['StartWorkflowRequest']
 _STARTWORKFLOWREQUEST_OPTIONSENTRY = _STARTWORKFLOWREQUEST.nested_types_by_name['OptionsEntry']
-_TERMINATEWORKFLOWREQUEST = DESCRIPTOR.message_types_by_name['TerminateWorkflowRequest']
-_TERMINATEWORKFLOWRESPONSE = DESCRIPTOR.message_types_by_name['TerminateWorkflowResponse']
-_BULKPUBLISHRESPONSEENTRY_STATUS = _BULKPUBLISHRESPONSEENTRY.enum_types_by_name['Status']
+_WORKFLOWACTIVITYREQUEST = DESCRIPTOR.message_types_by_name['WorkflowActivityRequest']
+_WORKFLOWACTIVITYRESPONSE = DESCRIPTOR.message_types_by_name['WorkflowActivityResponse']
+_RAISEEVENTWORKFLOWREQUEST = DESCRIPTOR.message_types_by_name['RaiseEventWorkflowRequest']
+_RAISEEVENTWORKFLOWRESPONSE = DESCRIPTOR.message_types_by_name['RaiseEventWorkflowResponse']
 _UNLOCKRESPONSE_STATUS = _UNLOCKRESPONSE.enum_types_by_name['Status']
+_SUBTLEGETKEYALPHA1REQUEST_KEYFORMAT = _SUBTLEGETKEYALPHA1REQUEST.enum_types_by_name['KeyFormat']
 InvokeServiceRequest = _reflection.GeneratedProtocolMessageType('InvokeServiceRequest', (_message.Message,), {
   'DESCRIPTOR' : _INVOKESERVICEREQUEST,
   '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
   # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.InvokeServiceRequest)
   })
 _sym_db.RegisterMessage(InvokeServiceRequest)
 
@@ -299,20 +315,20 @@
 BulkPublishResponse = _reflection.GeneratedProtocolMessageType('BulkPublishResponse', (_message.Message,), {
   'DESCRIPTOR' : _BULKPUBLISHRESPONSE,
   '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
   # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.BulkPublishResponse)
   })
 _sym_db.RegisterMessage(BulkPublishResponse)
 
-BulkPublishResponseEntry = _reflection.GeneratedProtocolMessageType('BulkPublishResponseEntry', (_message.Message,), {
-  'DESCRIPTOR' : _BULKPUBLISHRESPONSEENTRY,
+BulkPublishResponseFailedEntry = _reflection.GeneratedProtocolMessageType('BulkPublishResponseFailedEntry', (_message.Message,), {
+  'DESCRIPTOR' : _BULKPUBLISHRESPONSEFAILEDENTRY,
   '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
-  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.BulkPublishResponseEntry)
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.BulkPublishResponseFailedEntry)
   })
-_sym_db.RegisterMessage(BulkPublishResponseEntry)
+_sym_db.RegisterMessage(BulkPublishResponseFailedEntry)
 
 InvokeBindingRequest = _reflection.GeneratedProtocolMessageType('InvokeBindingRequest', (_message.Message,), {
 
   'MetadataEntry' : _reflection.GeneratedProtocolMessageType('MetadataEntry', (_message.Message,), {
     'DESCRIPTOR' : _INVOKEBINDINGREQUEST_METADATAENTRY,
     '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
     # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.InvokeBindingRequest.MetadataEntry)
@@ -490,19 +506,27 @@
   'DESCRIPTOR' : _EXECUTEACTORSTATETRANSACTIONREQUEST,
   '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
   # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.ExecuteActorStateTransactionRequest)
   })
 _sym_db.RegisterMessage(ExecuteActorStateTransactionRequest)
 
 TransactionalActorStateOperation = _reflection.GeneratedProtocolMessageType('TransactionalActorStateOperation', (_message.Message,), {
+
+  'MetadataEntry' : _reflection.GeneratedProtocolMessageType('MetadataEntry', (_message.Message,), {
+    'DESCRIPTOR' : _TRANSACTIONALACTORSTATEOPERATION_METADATAENTRY,
+    '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+    # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.TransactionalActorStateOperation.MetadataEntry)
+    })
+  ,
   'DESCRIPTOR' : _TRANSACTIONALACTORSTATEOPERATION,
   '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
   # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.TransactionalActorStateOperation)
   })
 _sym_db.RegisterMessage(TransactionalActorStateOperation)
+_sym_db.RegisterMessage(TransactionalActorStateOperation.MetadataEntry)
 
 InvokeActorRequest = _reflection.GeneratedProtocolMessageType('InvokeActorRequest', (_message.Message,), {
 
   'MetadataEntry' : _reflection.GeneratedProtocolMessageType('MetadataEntry', (_message.Message,), {
     'DESCRIPTOR' : _INVOKEACTORREQUEST_METADATAENTRY,
     '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
     # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.InvokeActorRequest.MetadataEntry)
@@ -685,14 +709,112 @@
 UnlockResponse = _reflection.GeneratedProtocolMessageType('UnlockResponse', (_message.Message,), {
   'DESCRIPTOR' : _UNLOCKRESPONSE,
   '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
   # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.UnlockResponse)
   })
 _sym_db.RegisterMessage(UnlockResponse)
 
+SubtleGetKeyAlpha1Request = _reflection.GeneratedProtocolMessageType('SubtleGetKeyAlpha1Request', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEGETKEYALPHA1REQUEST,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleGetKeyAlpha1Request)
+  })
+_sym_db.RegisterMessage(SubtleGetKeyAlpha1Request)
+
+SubtleGetKeyAlpha1Response = _reflection.GeneratedProtocolMessageType('SubtleGetKeyAlpha1Response', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEGETKEYALPHA1RESPONSE,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleGetKeyAlpha1Response)
+  })
+_sym_db.RegisterMessage(SubtleGetKeyAlpha1Response)
+
+SubtleEncryptAlpha1Request = _reflection.GeneratedProtocolMessageType('SubtleEncryptAlpha1Request', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEENCRYPTALPHA1REQUEST,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleEncryptAlpha1Request)
+  })
+_sym_db.RegisterMessage(SubtleEncryptAlpha1Request)
+
+SubtleEncryptAlpha1Response = _reflection.GeneratedProtocolMessageType('SubtleEncryptAlpha1Response', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEENCRYPTALPHA1RESPONSE,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleEncryptAlpha1Response)
+  })
+_sym_db.RegisterMessage(SubtleEncryptAlpha1Response)
+
+SubtleDecryptAlpha1Request = _reflection.GeneratedProtocolMessageType('SubtleDecryptAlpha1Request', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEDECRYPTALPHA1REQUEST,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleDecryptAlpha1Request)
+  })
+_sym_db.RegisterMessage(SubtleDecryptAlpha1Request)
+
+SubtleDecryptAlpha1Response = _reflection.GeneratedProtocolMessageType('SubtleDecryptAlpha1Response', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEDECRYPTALPHA1RESPONSE,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleDecryptAlpha1Response)
+  })
+_sym_db.RegisterMessage(SubtleDecryptAlpha1Response)
+
+SubtleWrapKeyAlpha1Request = _reflection.GeneratedProtocolMessageType('SubtleWrapKeyAlpha1Request', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEWRAPKEYALPHA1REQUEST,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleWrapKeyAlpha1Request)
+  })
+_sym_db.RegisterMessage(SubtleWrapKeyAlpha1Request)
+
+SubtleWrapKeyAlpha1Response = _reflection.GeneratedProtocolMessageType('SubtleWrapKeyAlpha1Response', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEWRAPKEYALPHA1RESPONSE,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleWrapKeyAlpha1Response)
+  })
+_sym_db.RegisterMessage(SubtleWrapKeyAlpha1Response)
+
+SubtleUnwrapKeyAlpha1Request = _reflection.GeneratedProtocolMessageType('SubtleUnwrapKeyAlpha1Request', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEUNWRAPKEYALPHA1REQUEST,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleUnwrapKeyAlpha1Request)
+  })
+_sym_db.RegisterMessage(SubtleUnwrapKeyAlpha1Request)
+
+SubtleUnwrapKeyAlpha1Response = _reflection.GeneratedProtocolMessageType('SubtleUnwrapKeyAlpha1Response', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEUNWRAPKEYALPHA1RESPONSE,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleUnwrapKeyAlpha1Response)
+  })
+_sym_db.RegisterMessage(SubtleUnwrapKeyAlpha1Response)
+
+SubtleSignAlpha1Request = _reflection.GeneratedProtocolMessageType('SubtleSignAlpha1Request', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLESIGNALPHA1REQUEST,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleSignAlpha1Request)
+  })
+_sym_db.RegisterMessage(SubtleSignAlpha1Request)
+
+SubtleSignAlpha1Response = _reflection.GeneratedProtocolMessageType('SubtleSignAlpha1Response', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLESIGNALPHA1RESPONSE,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleSignAlpha1Response)
+  })
+_sym_db.RegisterMessage(SubtleSignAlpha1Response)
+
+SubtleVerifyAlpha1Request = _reflection.GeneratedProtocolMessageType('SubtleVerifyAlpha1Request', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEVERIFYALPHA1REQUEST,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleVerifyAlpha1Request)
+  })
+_sym_db.RegisterMessage(SubtleVerifyAlpha1Request)
+
+SubtleVerifyAlpha1Response = _reflection.GeneratedProtocolMessageType('SubtleVerifyAlpha1Response', (_message.Message,), {
+  'DESCRIPTOR' : _SUBTLEVERIFYALPHA1RESPONSE,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.SubtleVerifyAlpha1Response)
+  })
+_sym_db.RegisterMessage(SubtleVerifyAlpha1Response)
+
 WorkflowReference = _reflection.GeneratedProtocolMessageType('WorkflowReference', (_message.Message,), {
   'DESCRIPTOR' : _WORKFLOWREFERENCE,
   '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
   # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.WorkflowReference)
   })
 _sym_db.RegisterMessage(WorkflowReference)
 
@@ -729,27 +851,41 @@
   'DESCRIPTOR' : _STARTWORKFLOWREQUEST,
   '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
   # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.StartWorkflowRequest)
   })
 _sym_db.RegisterMessage(StartWorkflowRequest)
 _sym_db.RegisterMessage(StartWorkflowRequest.OptionsEntry)
 
-TerminateWorkflowRequest = _reflection.GeneratedProtocolMessageType('TerminateWorkflowRequest', (_message.Message,), {
-  'DESCRIPTOR' : _TERMINATEWORKFLOWREQUEST,
+WorkflowActivityRequest = _reflection.GeneratedProtocolMessageType('WorkflowActivityRequest', (_message.Message,), {
+  'DESCRIPTOR' : _WORKFLOWACTIVITYREQUEST,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.WorkflowActivityRequest)
+  })
+_sym_db.RegisterMessage(WorkflowActivityRequest)
+
+WorkflowActivityResponse = _reflection.GeneratedProtocolMessageType('WorkflowActivityResponse', (_message.Message,), {
+  'DESCRIPTOR' : _WORKFLOWACTIVITYRESPONSE,
+  '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.WorkflowActivityResponse)
+  })
+_sym_db.RegisterMessage(WorkflowActivityResponse)
+
+RaiseEventWorkflowRequest = _reflection.GeneratedProtocolMessageType('RaiseEventWorkflowRequest', (_message.Message,), {
+  'DESCRIPTOR' : _RAISEEVENTWORKFLOWREQUEST,
   '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
-  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.TerminateWorkflowRequest)
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.RaiseEventWorkflowRequest)
   })
-_sym_db.RegisterMessage(TerminateWorkflowRequest)
+_sym_db.RegisterMessage(RaiseEventWorkflowRequest)
 
-TerminateWorkflowResponse = _reflection.GeneratedProtocolMessageType('TerminateWorkflowResponse', (_message.Message,), {
-  'DESCRIPTOR' : _TERMINATEWORKFLOWRESPONSE,
+RaiseEventWorkflowResponse = _reflection.GeneratedProtocolMessageType('RaiseEventWorkflowResponse', (_message.Message,), {
+  'DESCRIPTOR' : _RAISEEVENTWORKFLOWRESPONSE,
   '__module__' : 'dapr.proto.runtime.v1.dapr_pb2'
-  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.TerminateWorkflowResponse)
+  # @@protoc_insertion_point(class_scope:dapr.proto.runtime.v1.RaiseEventWorkflowResponse)
   })
-_sym_db.RegisterMessage(TerminateWorkflowResponse)
+_sym_db.RegisterMessage(RaiseEventWorkflowResponse)
 
 _DAPR = DESCRIPTOR.services_by_name['Dapr']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\nio.dapr.v1B\nDaprProtosZ1github.com/dapr/dapr/pkg/proto/runtime/v1;runtime\252\002\033Dapr.Client.Autogen.Grpc.v1'
   _GETSTATEREQUEST_METADATAENTRY._options = None
@@ -784,14 +920,16 @@
   _GETBULKSECRETREQUEST_METADATAENTRY._serialized_options = b'8\001'
   _SECRETRESPONSE_SECRETSENTRY._options = None
   _SECRETRESPONSE_SECRETSENTRY._serialized_options = b'8\001'
   _GETBULKSECRETRESPONSE_DATAENTRY._options = None
   _GETBULKSECRETRESPONSE_DATAENTRY._serialized_options = b'8\001'
   _EXECUTESTATETRANSACTIONREQUEST_METADATAENTRY._options = None
   _EXECUTESTATETRANSACTIONREQUEST_METADATAENTRY._serialized_options = b'8\001'
+  _TRANSACTIONALACTORSTATEOPERATION_METADATAENTRY._options = None
+  _TRANSACTIONALACTORSTATEOPERATION_METADATAENTRY._serialized_options = b'8\001'
   _INVOKEACTORREQUEST_METADATAENTRY._options = None
   _INVOKEACTORREQUEST_METADATAENTRY._serialized_options = b'8\001'
   _GETMETADATARESPONSE_EXTENDEDMETADATAENTRY._options = None
   _GETMETADATARESPONSE_EXTENDEDMETADATAENTRY._serialized_options = b'8\001'
   _PUBSUBSUBSCRIPTION_METADATAENTRY._options = None
   _PUBSUBSUBSCRIPTION_METADATAENTRY._serialized_options = b'8\001'
   _GETCONFIGURATIONREQUEST_METADATAENTRY._options = None
@@ -802,188 +940,222 @@
   _SUBSCRIBECONFIGURATIONREQUEST_METADATAENTRY._serialized_options = b'8\001'
   _SUBSCRIBECONFIGURATIONRESPONSE_ITEMSENTRY._options = None
   _SUBSCRIBECONFIGURATIONRESPONSE_ITEMSENTRY._serialized_options = b'8\001'
   _GETWORKFLOWRESPONSE_METADATAENTRY._options = None
   _GETWORKFLOWRESPONSE_METADATAENTRY._serialized_options = b'8\001'
   _STARTWORKFLOWREQUEST_OPTIONSENTRY._options = None
   _STARTWORKFLOWREQUEST_OPTIONSENTRY._serialized_options = b'8\001'
-  _INVOKESERVICEREQUEST._serialized_start=183
-  _INVOKESERVICEREQUEST._serialized_end=271
-  _GETSTATEREQUEST._serialized_start=274
-  _GETSTATEREQUEST._serialized_end=519
-  _GETSTATEREQUEST_METADATAENTRY._serialized_start=472
-  _GETSTATEREQUEST_METADATAENTRY._serialized_end=519
-  _GETBULKSTATEREQUEST._serialized_start=522
-  _GETBULKSTATEREQUEST._serialized_end=723
-  _GETBULKSTATEREQUEST_METADATAENTRY._serialized_start=472
-  _GETBULKSTATEREQUEST_METADATAENTRY._serialized_end=519
-  _GETBULKSTATERESPONSE._serialized_start=725
-  _GETBULKSTATERESPONSE._serialized_end=800
-  _BULKSTATEITEM._serialized_start=803
-  _BULKSTATEITEM._serialized_end=993
-  _BULKSTATEITEM_METADATAENTRY._serialized_start=472
-  _BULKSTATEITEM_METADATAENTRY._serialized_end=519
-  _GETSTATERESPONSE._serialized_start=996
-  _GETSTATERESPONSE._serialized_end=1164
-  _GETSTATERESPONSE_METADATAENTRY._serialized_start=472
-  _GETSTATERESPONSE_METADATAENTRY._serialized_end=519
-  _DELETESTATEREQUEST._serialized_start=1167
-  _DELETESTATEREQUEST._serialized_end=1439
-  _DELETESTATEREQUEST_METADATAENTRY._serialized_start=472
-  _DELETESTATEREQUEST_METADATAENTRY._serialized_end=519
-  _DELETEBULKSTATEREQUEST._serialized_start=1441
-  _DELETEBULKSTATEREQUEST._serialized_end=1534
-  _SAVESTATEREQUEST._serialized_start=1536
-  _SAVESTATEREQUEST._serialized_end=1623
-  _QUERYSTATEREQUEST._serialized_start=1626
-  _QUERYSTATEREQUEST._serialized_end=1803
-  _QUERYSTATEREQUEST_METADATAENTRY._serialized_start=472
-  _QUERYSTATEREQUEST_METADATAENTRY._serialized_end=519
-  _QUERYSTATEITEM._serialized_start=1805
-  _QUERYSTATEITEM._serialized_end=1877
-  _QUERYSTATERESPONSE._serialized_start=1880
-  _QUERYSTATERESPONSE._serialized_end=2095
-  _QUERYSTATERESPONSE_METADATAENTRY._serialized_start=472
-  _QUERYSTATERESPONSE_METADATAENTRY._serialized_end=519
-  _PUBLISHEVENTREQUEST._serialized_start=2098
-  _PUBLISHEVENTREQUEST._serialized_end=2321
-  _PUBLISHEVENTREQUEST_METADATAENTRY._serialized_start=472
-  _PUBLISHEVENTREQUEST_METADATAENTRY._serialized_end=519
-  _BULKPUBLISHREQUEST._serialized_start=2324
-  _BULKPUBLISHREQUEST._serialized_end=2569
-  _BULKPUBLISHREQUEST_METADATAENTRY._serialized_start=472
-  _BULKPUBLISHREQUEST_METADATAENTRY._serialized_end=519
-  _BULKPUBLISHREQUESTENTRY._serialized_start=2572
-  _BULKPUBLISHREQUESTENTRY._serialized_end=2781
-  _BULKPUBLISHREQUESTENTRY_METADATAENTRY._serialized_start=472
-  _BULKPUBLISHREQUESTENTRY_METADATAENTRY._serialized_end=519
-  _BULKPUBLISHRESPONSE._serialized_start=2783
-  _BULKPUBLISHRESPONSE._serialized_end=2871
-  _BULKPUBLISHRESPONSEENTRY._serialized_start=2874
-  _BULKPUBLISHRESPONSEENTRY._serialized_end=3040
-  _BULKPUBLISHRESPONSEENTRY_STATUS._serialized_start=3007
-  _BULKPUBLISHRESPONSEENTRY_STATUS._serialized_end=3040
-  _INVOKEBINDINGREQUEST._serialized_start=3043
-  _INVOKEBINDINGREQUEST._serialized_end=3238
-  _INVOKEBINDINGREQUEST_METADATAENTRY._serialized_start=472
-  _INVOKEBINDINGREQUEST_METADATAENTRY._serialized_end=519
-  _INVOKEBINDINGRESPONSE._serialized_start=3241
-  _INVOKEBINDINGRESPONSE._serialized_end=3405
-  _INVOKEBINDINGRESPONSE_METADATAENTRY._serialized_start=472
-  _INVOKEBINDINGRESPONSE_METADATAENTRY._serialized_end=519
-  _GETSECRETREQUEST._serialized_start=3408
-  _GETSECRETREQUEST._serialized_end=3581
-  _GETSECRETREQUEST_METADATAENTRY._serialized_start=472
-  _GETSECRETREQUEST_METADATAENTRY._serialized_end=519
-  _GETSECRETRESPONSE._serialized_start=3584
-  _GETSECRETRESPONSE._serialized_end=3714
-  _GETSECRETRESPONSE_DATAENTRY._serialized_start=3671
-  _GETSECRETRESPONSE_DATAENTRY._serialized_end=3714
-  _GETBULKSECRETREQUEST._serialized_start=3717
-  _GETBULKSECRETREQUEST._serialized_end=3885
-  _GETBULKSECRETREQUEST_METADATAENTRY._serialized_start=472
-  _GETBULKSECRETREQUEST_METADATAENTRY._serialized_end=519
-  _SECRETRESPONSE._serialized_start=3888
-  _SECRETRESPONSE._serialized_end=4021
-  _SECRETRESPONSE_SECRETSENTRY._serialized_start=3975
-  _SECRETRESPONSE_SECRETSENTRY._serialized_end=4021
-  _GETBULKSECRETRESPONSE._serialized_start=4024
-  _GETBULKSECRETRESPONSE._serialized_end=4201
-  _GETBULKSECRETRESPONSE_DATAENTRY._serialized_start=4119
-  _GETBULKSECRETRESPONSE_DATAENTRY._serialized_end=4201
-  _TRANSACTIONALSTATEOPERATION._serialized_start=4203
-  _TRANSACTIONALSTATEOPERATION._serialized_end=4305
-  _EXECUTESTATETRANSACTIONREQUEST._serialized_start=4308
-  _EXECUTESTATETRANSACTIONREQUEST._serialized_end=4567
-  _EXECUTESTATETRANSACTIONREQUEST_METADATAENTRY._serialized_start=472
-  _EXECUTESTATETRANSACTIONREQUEST_METADATAENTRY._serialized_end=519
-  _REGISTERACTORTIMERREQUEST._serialized_start=4570
-  _REGISTERACTORTIMERREQUEST._serialized_end=4728
-  _UNREGISTERACTORTIMERREQUEST._serialized_start=4730
-  _UNREGISTERACTORTIMERREQUEST._serialized_end=4811
-  _REGISTERACTORREMINDERREQUEST._serialized_start=4814
-  _REGISTERACTORREMINDERREQUEST._serialized_end=4957
-  _UNREGISTERACTORREMINDERREQUEST._serialized_start=4959
-  _UNREGISTERACTORREMINDERREQUEST._serialized_end=5043
-  _RENAMEACTORREMINDERREQUEST._serialized_start=5045
-  _RENAMEACTORREMINDERREQUEST._serialized_end=5147
-  _GETACTORSTATEREQUEST._serialized_start=5149
-  _GETACTORSTATEREQUEST._serialized_end=5222
-  _GETACTORSTATERESPONSE._serialized_start=5224
-  _GETACTORSTATERESPONSE._serialized_end=5261
-  _EXECUTEACTORSTATETRANSACTIONREQUEST._serialized_start=5264
-  _EXECUTEACTORSTATETRANSACTIONREQUEST._serialized_end=5416
-  _TRANSACTIONALACTORSTATEOPERATION._serialized_start=5418
-  _TRANSACTIONALACTORSTATEOPERATION._serialized_end=5525
-  _INVOKEACTORREQUEST._serialized_start=5528
-  _INVOKEACTORREQUEST._serialized_end=5740
-  _INVOKEACTORREQUEST_METADATAENTRY._serialized_start=472
-  _INVOKEACTORREQUEST_METADATAENTRY._serialized_end=519
-  _INVOKEACTORRESPONSE._serialized_start=5742
-  _INVOKEACTORRESPONSE._serialized_end=5777
-  _GETMETADATARESPONSE._serialized_start=5780
-  _GETMETADATARESPONSE._serialized_end=6176
-  _GETMETADATARESPONSE_EXTENDEDMETADATAENTRY._serialized_start=6121
-  _GETMETADATARESPONSE_EXTENDEDMETADATAENTRY._serialized_end=6176
-  _ACTIVEACTORSCOUNT._serialized_start=6178
-  _ACTIVEACTORSCOUNT._serialized_end=6226
-  _REGISTEREDCOMPONENTS._serialized_start=6228
-  _REGISTEREDCOMPONENTS._serialized_end=6317
-  _PUBSUBSUBSCRIPTION._serialized_start=6320
-  _PUBSUBSUBSCRIPTION._serialized_end=6590
-  _PUBSUBSUBSCRIPTION_METADATAENTRY._serialized_start=472
-  _PUBSUBSUBSCRIPTION_METADATAENTRY._serialized_end=519
-  _PUBSUBSUBSCRIPTIONRULES._serialized_start=6592
-  _PUBSUBSUBSCRIPTIONRULES._serialized_end=6679
-  _PUBSUBSUBSCRIPTIONRULE._serialized_start=6681
-  _PUBSUBSUBSCRIPTIONRULE._serialized_end=6734
-  _SETMETADATAREQUEST._serialized_start=6736
-  _SETMETADATAREQUEST._serialized_end=6784
-  _GETCONFIGURATIONREQUEST._serialized_start=6787
-  _GETCONFIGURATIONREQUEST._serialized_end=6975
-  _GETCONFIGURATIONREQUEST_METADATAENTRY._serialized_start=472
-  _GETCONFIGURATIONREQUEST_METADATAENTRY._serialized_end=519
-  _GETCONFIGURATIONRESPONSE._serialized_start=6978
-  _GETCONFIGURATIONRESPONSE._serialized_end=7166
-  _GETCONFIGURATIONRESPONSE_ITEMSENTRY._serialized_start=7081
-  _GETCONFIGURATIONRESPONSE_ITEMSENTRY._serialized_end=7166
-  _SUBSCRIBECONFIGURATIONREQUEST._serialized_start=7169
-  _SUBSCRIBECONFIGURATIONREQUEST._serialized_end=7369
-  _SUBSCRIBECONFIGURATIONREQUEST_METADATAENTRY._serialized_start=472
-  _SUBSCRIBECONFIGURATIONREQUEST_METADATAENTRY._serialized_end=519
-  _UNSUBSCRIBECONFIGURATIONREQUEST._serialized_start=7371
-  _UNSUBSCRIBECONFIGURATIONREQUEST._serialized_end=7436
-  _SUBSCRIBECONFIGURATIONRESPONSE._serialized_start=7439
-  _SUBSCRIBECONFIGURATIONRESPONSE._serialized_end=7651
-  _SUBSCRIBECONFIGURATIONRESPONSE_ITEMSENTRY._serialized_start=7081
-  _SUBSCRIBECONFIGURATIONRESPONSE_ITEMSENTRY._serialized_end=7166
-  _UNSUBSCRIBECONFIGURATIONRESPONSE._serialized_start=7653
-  _UNSUBSCRIBECONFIGURATIONRESPONSE._serialized_end=7716
-  _TRYLOCKREQUEST._serialized_start=7718
-  _TRYLOCKREQUEST._serialized_end=7820
-  _TRYLOCKRESPONSE._serialized_start=7822
-  _TRYLOCKRESPONSE._serialized_end=7856
-  _UNLOCKREQUEST._serialized_start=7858
-  _UNLOCKREQUEST._serialized_end=7934
-  _UNLOCKRESPONSE._serialized_start=7937
-  _UNLOCKRESPONSE._serialized_end=8111
-  _UNLOCKRESPONSE_STATUS._serialized_start=8017
-  _UNLOCKRESPONSE_STATUS._serialized_end=8111
-  _WORKFLOWREFERENCE._serialized_start=8113
-  _WORKFLOWREFERENCE._serialized_end=8153
-  _GETWORKFLOWREQUEST._serialized_start=8155
-  _GETWORKFLOWREQUEST._serialized_end=8247
-  _GETWORKFLOWRESPONSE._serialized_start=8250
-  _GETWORKFLOWRESPONSE._serialized_end=8437
-  _GETWORKFLOWRESPONSE_METADATAENTRY._serialized_start=472
-  _GETWORKFLOWRESPONSE_METADATAENTRY._serialized_end=519
-  _STARTWORKFLOWREQUEST._serialized_start=8440
-  _STARTWORKFLOWREQUEST._serialized_end=8694
-  _STARTWORKFLOWREQUEST_OPTIONSENTRY._serialized_start=8648
-  _STARTWORKFLOWREQUEST_OPTIONSENTRY._serialized_end=8694
-  _TERMINATEWORKFLOWREQUEST._serialized_start=8696
-  _TERMINATEWORKFLOWREQUEST._serialized_end=8771
-  _TERMINATEWORKFLOWRESPONSE._serialized_start=8773
-  _TERMINATEWORKFLOWRESPONSE._serialized_end=8800
-  _DAPR._serialized_start=8803
-  _DAPR._serialized_end=12142
+  _INVOKESERVICEREQUEST._serialized_start=150
+  _INVOKESERVICEREQUEST._serialized_end=238
+  _GETSTATEREQUEST._serialized_start=241
+  _GETSTATEREQUEST._serialized_end=486
+  _GETSTATEREQUEST_METADATAENTRY._serialized_start=439
+  _GETSTATEREQUEST_METADATAENTRY._serialized_end=486
+  _GETBULKSTATEREQUEST._serialized_start=489
+  _GETBULKSTATEREQUEST._serialized_end=690
+  _GETBULKSTATEREQUEST_METADATAENTRY._serialized_start=439
+  _GETBULKSTATEREQUEST_METADATAENTRY._serialized_end=486
+  _GETBULKSTATERESPONSE._serialized_start=692
+  _GETBULKSTATERESPONSE._serialized_end=767
+  _BULKSTATEITEM._serialized_start=770
+  _BULKSTATEITEM._serialized_end=960
+  _BULKSTATEITEM_METADATAENTRY._serialized_start=439
+  _BULKSTATEITEM_METADATAENTRY._serialized_end=486
+  _GETSTATERESPONSE._serialized_start=963
+  _GETSTATERESPONSE._serialized_end=1131
+  _GETSTATERESPONSE_METADATAENTRY._serialized_start=439
+  _GETSTATERESPONSE_METADATAENTRY._serialized_end=486
+  _DELETESTATEREQUEST._serialized_start=1134
+  _DELETESTATEREQUEST._serialized_end=1406
+  _DELETESTATEREQUEST_METADATAENTRY._serialized_start=439
+  _DELETESTATEREQUEST_METADATAENTRY._serialized_end=486
+  _DELETEBULKSTATEREQUEST._serialized_start=1408
+  _DELETEBULKSTATEREQUEST._serialized_end=1501
+  _SAVESTATEREQUEST._serialized_start=1503
+  _SAVESTATEREQUEST._serialized_end=1590
+  _QUERYSTATEREQUEST._serialized_start=1593
+  _QUERYSTATEREQUEST._serialized_end=1781
+  _QUERYSTATEREQUEST_METADATAENTRY._serialized_start=439
+  _QUERYSTATEREQUEST_METADATAENTRY._serialized_end=486
+  _QUERYSTATEITEM._serialized_start=1783
+  _QUERYSTATEITEM._serialized_end=1855
+  _QUERYSTATERESPONSE._serialized_start=1858
+  _QUERYSTATERESPONSE._serialized_end=2073
+  _QUERYSTATERESPONSE_METADATAENTRY._serialized_start=439
+  _QUERYSTATERESPONSE_METADATAENTRY._serialized_end=486
+  _PUBLISHEVENTREQUEST._serialized_start=2076
+  _PUBLISHEVENTREQUEST._serialized_end=2299
+  _PUBLISHEVENTREQUEST_METADATAENTRY._serialized_start=439
+  _PUBLISHEVENTREQUEST_METADATAENTRY._serialized_end=486
+  _BULKPUBLISHREQUEST._serialized_start=2302
+  _BULKPUBLISHREQUEST._serialized_end=2547
+  _BULKPUBLISHREQUEST_METADATAENTRY._serialized_start=439
+  _BULKPUBLISHREQUEST_METADATAENTRY._serialized_end=486
+  _BULKPUBLISHREQUESTENTRY._serialized_start=2550
+  _BULKPUBLISHREQUESTENTRY._serialized_end=2759
+  _BULKPUBLISHREQUESTENTRY_METADATAENTRY._serialized_start=439
+  _BULKPUBLISHREQUESTENTRY_METADATAENTRY._serialized_end=486
+  _BULKPUBLISHRESPONSE._serialized_start=2761
+  _BULKPUBLISHRESPONSE._serialized_end=2860
+  _BULKPUBLISHRESPONSEFAILEDENTRY._serialized_start=2862
+  _BULKPUBLISHRESPONSEFAILEDENTRY._serialized_end=2927
+  _INVOKEBINDINGREQUEST._serialized_start=2930
+  _INVOKEBINDINGREQUEST._serialized_end=3125
+  _INVOKEBINDINGREQUEST_METADATAENTRY._serialized_start=439
+  _INVOKEBINDINGREQUEST_METADATAENTRY._serialized_end=486
+  _INVOKEBINDINGRESPONSE._serialized_start=3128
+  _INVOKEBINDINGRESPONSE._serialized_end=3292
+  _INVOKEBINDINGRESPONSE_METADATAENTRY._serialized_start=439
+  _INVOKEBINDINGRESPONSE_METADATAENTRY._serialized_end=486
+  _GETSECRETREQUEST._serialized_start=3295
+  _GETSECRETREQUEST._serialized_end=3479
+  _GETSECRETREQUEST_METADATAENTRY._serialized_start=439
+  _GETSECRETREQUEST_METADATAENTRY._serialized_end=486
+  _GETSECRETRESPONSE._serialized_start=3482
+  _GETSECRETRESPONSE._serialized_end=3612
+  _GETSECRETRESPONSE_DATAENTRY._serialized_start=3569
+  _GETSECRETRESPONSE_DATAENTRY._serialized_end=3612
+  _GETBULKSECRETREQUEST._serialized_start=3615
+  _GETBULKSECRETREQUEST._serialized_end=3794
+  _GETBULKSECRETREQUEST_METADATAENTRY._serialized_start=439
+  _GETBULKSECRETREQUEST_METADATAENTRY._serialized_end=486
+  _SECRETRESPONSE._serialized_start=3797
+  _SECRETRESPONSE._serialized_end=3930
+  _SECRETRESPONSE_SECRETSENTRY._serialized_start=3884
+  _SECRETRESPONSE_SECRETSENTRY._serialized_end=3930
+  _GETBULKSECRETRESPONSE._serialized_start=3933
+  _GETBULKSECRETRESPONSE._serialized_end=4110
+  _GETBULKSECRETRESPONSE_DATAENTRY._serialized_start=4028
+  _GETBULKSECRETRESPONSE_DATAENTRY._serialized_end=4110
+  _TRANSACTIONALSTATEOPERATION._serialized_start=4112
+  _TRANSACTIONALSTATEOPERATION._serialized_end=4214
+  _EXECUTESTATETRANSACTIONREQUEST._serialized_start=4217
+  _EXECUTESTATETRANSACTIONREQUEST._serialized_end=4476
+  _EXECUTESTATETRANSACTIONREQUEST_METADATAENTRY._serialized_start=439
+  _EXECUTESTATETRANSACTIONREQUEST_METADATAENTRY._serialized_end=486
+  _REGISTERACTORTIMERREQUEST._serialized_start=4479
+  _REGISTERACTORTIMERREQUEST._serialized_end=4637
+  _UNREGISTERACTORTIMERREQUEST._serialized_start=4639
+  _UNREGISTERACTORTIMERREQUEST._serialized_end=4720
+  _REGISTERACTORREMINDERREQUEST._serialized_start=4723
+  _REGISTERACTORREMINDERREQUEST._serialized_end=4866
+  _UNREGISTERACTORREMINDERREQUEST._serialized_start=4868
+  _UNREGISTERACTORREMINDERREQUEST._serialized_end=4952
+  _RENAMEACTORREMINDERREQUEST._serialized_start=4954
+  _RENAMEACTORREMINDERREQUEST._serialized_end=5056
+  _GETACTORSTATEREQUEST._serialized_start=5058
+  _GETACTORSTATEREQUEST._serialized_end=5131
+  _GETACTORSTATERESPONSE._serialized_start=5133
+  _GETACTORSTATERESPONSE._serialized_end=5170
+  _EXECUTEACTORSTATETRANSACTIONREQUEST._serialized_start=5173
+  _EXECUTEACTORSTATETRANSACTIONREQUEST._serialized_end=5325
+  _TRANSACTIONALACTORSTATEOPERATION._serialized_start=5328
+  _TRANSACTIONALACTORSTATEOPERATION._serialized_end=5573
+  _TRANSACTIONALACTORSTATEOPERATION_METADATAENTRY._serialized_start=439
+  _TRANSACTIONALACTORSTATEOPERATION_METADATAENTRY._serialized_end=486
+  _INVOKEACTORREQUEST._serialized_start=5576
+  _INVOKEACTORREQUEST._serialized_end=5788
+  _INVOKEACTORREQUEST_METADATAENTRY._serialized_start=439
+  _INVOKEACTORREQUEST_METADATAENTRY._serialized_end=486
+  _INVOKEACTORRESPONSE._serialized_start=5790
+  _INVOKEACTORRESPONSE._serialized_end=5825
+  _GETMETADATARESPONSE._serialized_start=5828
+  _GETMETADATARESPONSE._serialized_end=6224
+  _GETMETADATARESPONSE_EXTENDEDMETADATAENTRY._serialized_start=6169
+  _GETMETADATARESPONSE_EXTENDEDMETADATAENTRY._serialized_end=6224
+  _ACTIVEACTORSCOUNT._serialized_start=6226
+  _ACTIVEACTORSCOUNT._serialized_end=6274
+  _REGISTEREDCOMPONENTS._serialized_start=6276
+  _REGISTEREDCOMPONENTS._serialized_end=6365
+  _PUBSUBSUBSCRIPTION._serialized_start=6368
+  _PUBSUBSUBSCRIPTION._serialized_end=6638
+  _PUBSUBSUBSCRIPTION_METADATAENTRY._serialized_start=439
+  _PUBSUBSUBSCRIPTION_METADATAENTRY._serialized_end=486
+  _PUBSUBSUBSCRIPTIONRULES._serialized_start=6640
+  _PUBSUBSUBSCRIPTIONRULES._serialized_end=6727
+  _PUBSUBSUBSCRIPTIONRULE._serialized_start=6729
+  _PUBSUBSUBSCRIPTIONRULE._serialized_end=6782
+  _SETMETADATAREQUEST._serialized_start=6784
+  _SETMETADATAREQUEST._serialized_end=6832
+  _GETCONFIGURATIONREQUEST._serialized_start=6835
+  _GETCONFIGURATIONREQUEST._serialized_end=7023
+  _GETCONFIGURATIONREQUEST_METADATAENTRY._serialized_start=439
+  _GETCONFIGURATIONREQUEST_METADATAENTRY._serialized_end=486
+  _GETCONFIGURATIONRESPONSE._serialized_start=7026
+  _GETCONFIGURATIONRESPONSE._serialized_end=7214
+  _GETCONFIGURATIONRESPONSE_ITEMSENTRY._serialized_start=7129
+  _GETCONFIGURATIONRESPONSE_ITEMSENTRY._serialized_end=7214
+  _SUBSCRIBECONFIGURATIONREQUEST._serialized_start=7217
+  _SUBSCRIBECONFIGURATIONREQUEST._serialized_end=7417
+  _SUBSCRIBECONFIGURATIONREQUEST_METADATAENTRY._serialized_start=439
+  _SUBSCRIBECONFIGURATIONREQUEST_METADATAENTRY._serialized_end=486
+  _UNSUBSCRIBECONFIGURATIONREQUEST._serialized_start=7419
+  _UNSUBSCRIBECONFIGURATIONREQUEST._serialized_end=7484
+  _SUBSCRIBECONFIGURATIONRESPONSE._serialized_start=7487
+  _SUBSCRIBECONFIGURATIONRESPONSE._serialized_end=7699
+  _SUBSCRIBECONFIGURATIONRESPONSE_ITEMSENTRY._serialized_start=7129
+  _SUBSCRIBECONFIGURATIONRESPONSE_ITEMSENTRY._serialized_end=7214
+  _UNSUBSCRIBECONFIGURATIONRESPONSE._serialized_start=7701
+  _UNSUBSCRIBECONFIGURATIONRESPONSE._serialized_end=7764
+  _TRYLOCKREQUEST._serialized_start=7767
+  _TRYLOCKREQUEST._serialized_end=7922
+  _TRYLOCKRESPONSE._serialized_start=7924
+  _TRYLOCKRESPONSE._serialized_end=7958
+  _UNLOCKREQUEST._serialized_start=7960
+  _UNLOCKREQUEST._serialized_end=8070
+  _UNLOCKRESPONSE._serialized_start=8073
+  _UNLOCKRESPONSE._serialized_end=8247
+  _UNLOCKRESPONSE_STATUS._serialized_start=8153
+  _UNLOCKRESPONSE_STATUS._serialized_end=8247
+  _SUBTLEGETKEYALPHA1REQUEST._serialized_start=8250
+  _SUBTLEGETKEYALPHA1REQUEST._serialized_end=8438
+  _SUBTLEGETKEYALPHA1REQUEST_KEYFORMAT._serialized_start=8408
+  _SUBTLEGETKEYALPHA1REQUEST_KEYFORMAT._serialized_end=8438
+  _SUBTLEGETKEYALPHA1RESPONSE._serialized_start=8440
+  _SUBTLEGETKEYALPHA1RESPONSE._serialized_end=8513
+  _SUBTLEENCRYPTALPHA1REQUEST._serialized_start=8516
+  _SUBTLEENCRYPTALPHA1REQUEST._serialized_end=8704
+  _SUBTLEENCRYPTALPHA1RESPONSE._serialized_start=8706
+  _SUBTLEENCRYPTALPHA1RESPONSE._serialized_end=8768
+  _SUBTLEDECRYPTALPHA1REQUEST._serialized_start=8771
+  _SUBTLEDECRYPTALPHA1REQUEST._serialized_end=8973
+  _SUBTLEDECRYPTALPHA1RESPONSE._serialized_start=8975
+  _SUBTLEDECRYPTALPHA1RESPONSE._serialized_end=9023
+  _SUBTLEWRAPKEYALPHA1REQUEST._serialized_start=9026
+  _SUBTLEWRAPKEYALPHA1REQUEST._serialized_end=9232
+  _SUBTLEWRAPKEYALPHA1RESPONSE._serialized_start=9234
+  _SUBTLEWRAPKEYALPHA1RESPONSE._serialized_end=9309
+  _SUBTLEUNWRAPKEYALPHA1REQUEST._serialized_start=9312
+  _SUBTLEUNWRAPKEYALPHA1REQUEST._serialized_end=9529
+  _SUBTLEUNWRAPKEYALPHA1RESPONSE._serialized_start=9531
+  _SUBTLEUNWRAPKEYALPHA1RESPONSE._serialized_end=9599
+  _SUBTLESIGNALPHA1REQUEST._serialized_start=9601
+  _SUBTLESIGNALPHA1REQUEST._serialized_end=9727
+  _SUBTLESIGNALPHA1RESPONSE._serialized_start=9729
+  _SUBTLESIGNALPHA1RESPONSE._serialized_end=9774
+  _SUBTLEVERIFYALPHA1REQUEST._serialized_start=9777
+  _SUBTLEVERIFYALPHA1REQUEST._serialized_end=9924
+  _SUBTLEVERIFYALPHA1RESPONSE._serialized_start=9926
+  _SUBTLEVERIFYALPHA1RESPONSE._serialized_end=9969
+  _WORKFLOWREFERENCE._serialized_start=9971
+  _WORKFLOWREFERENCE._serialized_end=10023
+  _GETWORKFLOWREQUEST._serialized_start=10026
+  _GETWORKFLOWREQUEST._serialized_end=10163
+  _GETWORKFLOWRESPONSE._serialized_start=10166
+  _GETWORKFLOWRESPONSE._serialized_end=10353
+  _GETWORKFLOWRESPONSE_METADATAENTRY._serialized_start=439
+  _GETWORKFLOWRESPONSE_METADATAENTRY._serialized_end=486
+  _STARTWORKFLOWREQUEST._serialized_start=10356
+  _STARTWORKFLOWREQUEST._serialized_end=10633
+  _STARTWORKFLOWREQUEST_OPTIONSENTRY._serialized_start=10587
+  _STARTWORKFLOWREQUEST_OPTIONSENTRY._serialized_end=10633
+  _WORKFLOWACTIVITYREQUEST._serialized_start=10635
+  _WORKFLOWACTIVITYREQUEST._serialized_end=10740
+  _WORKFLOWACTIVITYRESPONSE._serialized_start=10742
+  _WORKFLOWACTIVITYRESPONSE._serialized_end=10768
+  _RAISEEVENTWORKFLOWREQUEST._serialized_start=10771
+  _RAISEEVENTWORKFLOWREQUEST._serialized_end=10924
+  _RAISEEVENTWORKFLOWRESPONSE._serialized_start=10926
+  _RAISEEVENTWORKFLOWRESPONSE._serialized_end=10954
+  _DAPR._serialized_start=10957
+  _DAPR._serialized_end=15948
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/dapr_pb2_grpc.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/proto/runtime/v1/dapr_pb2_grpc.py`

 * *Files 18% similar despite different names*

```diff
@@ -123,24 +123,39 @@
                 response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.InvokeActorResponse.FromString,
                 )
         self.GetConfigurationAlpha1 = channel.unary_unary(
                 '/dapr.proto.runtime.v1.Dapr/GetConfigurationAlpha1',
                 request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationRequest.SerializeToString,
                 response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationResponse.FromString,
                 )
+        self.GetConfiguration = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/GetConfiguration',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationRequest.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationResponse.FromString,
+                )
         self.SubscribeConfigurationAlpha1 = channel.unary_stream(
                 '/dapr.proto.runtime.v1.Dapr/SubscribeConfigurationAlpha1',
                 request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationRequest.SerializeToString,
                 response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationResponse.FromString,
                 )
+        self.SubscribeConfiguration = channel.unary_stream(
+                '/dapr.proto.runtime.v1.Dapr/SubscribeConfiguration',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationRequest.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationResponse.FromString,
+                )
         self.UnsubscribeConfigurationAlpha1 = channel.unary_unary(
                 '/dapr.proto.runtime.v1.Dapr/UnsubscribeConfigurationAlpha1',
                 request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationRequest.SerializeToString,
                 response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationResponse.FromString,
                 )
+        self.UnsubscribeConfiguration = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/UnsubscribeConfiguration',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationRequest.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationResponse.FromString,
+                )
         self.TryLockAlpha1 = channel.unary_unary(
                 '/dapr.proto.runtime.v1.Dapr/TryLockAlpha1',
                 request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.TryLockRequest.SerializeToString,
                 response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.TryLockResponse.FromString,
                 )
         self.UnlockAlpha1 = channel.unary_unary(
                 '/dapr.proto.runtime.v1.Dapr/UnlockAlpha1',
@@ -153,42 +168,93 @@
                 response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetMetadataResponse.FromString,
                 )
         self.SetMetadata = channel.unary_unary(
                 '/dapr.proto.runtime.v1.Dapr/SetMetadata',
                 request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SetMetadataRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
+        self.SubtleGetKeyAlpha1 = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/SubtleGetKeyAlpha1',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleGetKeyAlpha1Request.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleGetKeyAlpha1Response.FromString,
+                )
+        self.SubtleEncryptAlpha1 = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/SubtleEncryptAlpha1',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleEncryptAlpha1Request.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleEncryptAlpha1Response.FromString,
+                )
+        self.SubtleDecryptAlpha1 = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/SubtleDecryptAlpha1',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleDecryptAlpha1Request.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleDecryptAlpha1Response.FromString,
+                )
+        self.SubtleWrapKeyAlpha1 = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/SubtleWrapKeyAlpha1',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleWrapKeyAlpha1Request.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleWrapKeyAlpha1Response.FromString,
+                )
+        self.SubtleUnwrapKeyAlpha1 = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/SubtleUnwrapKeyAlpha1',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleUnwrapKeyAlpha1Request.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleUnwrapKeyAlpha1Response.FromString,
+                )
+        self.SubtleSignAlpha1 = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/SubtleSignAlpha1',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleSignAlpha1Request.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleSignAlpha1Response.FromString,
+                )
+        self.SubtleVerifyAlpha1 = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/SubtleVerifyAlpha1',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleVerifyAlpha1Request.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleVerifyAlpha1Response.FromString,
+                )
         self.StartWorkflowAlpha1 = channel.unary_unary(
                 '/dapr.proto.runtime.v1.Dapr/StartWorkflowAlpha1',
                 request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.StartWorkflowRequest.SerializeToString,
                 response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowReference.FromString,
                 )
         self.GetWorkflowAlpha1 = channel.unary_unary(
                 '/dapr.proto.runtime.v1.Dapr/GetWorkflowAlpha1',
                 request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetWorkflowRequest.SerializeToString,
                 response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetWorkflowResponse.FromString,
                 )
         self.TerminateWorkflowAlpha1 = channel.unary_unary(
                 '/dapr.proto.runtime.v1.Dapr/TerminateWorkflowAlpha1',
-                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.TerminateWorkflowRequest.SerializeToString,
-                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.TerminateWorkflowResponse.FromString,
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityRequest.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityResponse.FromString,
+                )
+        self.PauseWorkflowAlpha1 = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/PauseWorkflowAlpha1',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityRequest.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityResponse.FromString,
+                )
+        self.ResumeWorkflowAlpha1 = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/ResumeWorkflowAlpha1',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityRequest.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityResponse.FromString,
+                )
+        self.RaiseEventWorkflowAlpha1 = channel.unary_unary(
+                '/dapr.proto.runtime.v1.Dapr/RaiseEventWorkflowAlpha1',
+                request_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.RaiseEventWorkflowRequest.SerializeToString,
+                response_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.RaiseEventWorkflowResponse.FromString,
                 )
         self.Shutdown = channel.unary_unary(
                 '/dapr.proto.runtime.v1.Dapr/Shutdown',
                 request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
 
 
 class DaprServicer(object):
     """Dapr service provides APIs to user application to access Dapr building blocks.
     """
 
     def InvokeService(self, request, context):
         """Invokes a method on a remote Dapr app.
+        Deprecated: Use proxy mode service invocation instead.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetState(self, request, context):
         """Gets the state for a specific key.
@@ -333,28 +399,49 @@
     def GetConfigurationAlpha1(self, request, context):
         """GetConfiguration gets configuration from configuration store.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetConfiguration(self, request, context):
+        """GetConfiguration gets configuration from configuration store.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def SubscribeConfigurationAlpha1(self, request, context):
         """SubscribeConfiguration gets configuration from configuration store and subscribe the updates event by grpc stream
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SubscribeConfiguration(self, request, context):
+        """SubscribeConfiguration gets configuration from configuration store and subscribe the updates event by grpc stream
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def UnsubscribeConfigurationAlpha1(self, request, context):
         """UnSubscribeConfiguration unsubscribe the subscription of configuration
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def UnsubscribeConfiguration(self, request, context):
+        """UnSubscribeConfiguration unsubscribe the subscription of configuration
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def TryLockAlpha1(self, request, context):
         """TryLockAlpha1 tries to get a lock with an expiry.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -375,14 +462,63 @@
     def SetMetadata(self, request, context):
         """Sets value in extended metadata of the sidecar
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SubtleGetKeyAlpha1(self, request, context):
+        """SubtleGetKeyAlpha1 returns the public part of an asymmetric key stored in the vault.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubtleEncryptAlpha1(self, request, context):
+        """SubtleEncryptAlpha1 encrypts a small message using a key stored in the vault.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubtleDecryptAlpha1(self, request, context):
+        """SubtleDecryptAlpha1 decrypts a small message using a key stored in the vault.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubtleWrapKeyAlpha1(self, request, context):
+        """SubtleWrapKeyAlpha1 wraps a key using a key stored in the vault.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubtleUnwrapKeyAlpha1(self, request, context):
+        """SubtleUnwrapKeyAlpha1 unwraps a key using a key stored in the vault.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubtleSignAlpha1(self, request, context):
+        """SubtleSignAlpha1 signs a message using a key stored in the vault.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubtleVerifyAlpha1(self, request, context):
+        """SubtleVerifyAlpha1 verifies the signature of a message using a key stored in the vault.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def StartWorkflowAlpha1(self, request, context):
         """Start Workflow
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -396,14 +532,35 @@
     def TerminateWorkflowAlpha1(self, request, context):
         """Terminate Workflow
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def PauseWorkflowAlpha1(self, request, context):
+        """Pause Workflow
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ResumeWorkflowAlpha1(self, request, context):
+        """Resume Workflow
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def RaiseEventWorkflowAlpha1(self, request, context):
+        """Raise Event for a Workflow
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def Shutdown(self, request, context):
         """Shutdown the sidecar
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -516,24 +673,39 @@
                     response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.InvokeActorResponse.SerializeToString,
             ),
             'GetConfigurationAlpha1': grpc.unary_unary_rpc_method_handler(
                     servicer.GetConfigurationAlpha1,
                     request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationRequest.FromString,
                     response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationResponse.SerializeToString,
             ),
+            'GetConfiguration': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetConfiguration,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationRequest.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationResponse.SerializeToString,
+            ),
             'SubscribeConfigurationAlpha1': grpc.unary_stream_rpc_method_handler(
                     servicer.SubscribeConfigurationAlpha1,
                     request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationRequest.FromString,
                     response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationResponse.SerializeToString,
             ),
+            'SubscribeConfiguration': grpc.unary_stream_rpc_method_handler(
+                    servicer.SubscribeConfiguration,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationRequest.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationResponse.SerializeToString,
+            ),
             'UnsubscribeConfigurationAlpha1': grpc.unary_unary_rpc_method_handler(
                     servicer.UnsubscribeConfigurationAlpha1,
                     request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationRequest.FromString,
                     response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationResponse.SerializeToString,
             ),
+            'UnsubscribeConfiguration': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnsubscribeConfiguration,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationRequest.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationResponse.SerializeToString,
+            ),
             'TryLockAlpha1': grpc.unary_unary_rpc_method_handler(
                     servicer.TryLockAlpha1,
                     request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.TryLockRequest.FromString,
                     response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.TryLockResponse.SerializeToString,
             ),
             'UnlockAlpha1': grpc.unary_unary_rpc_method_handler(
                     servicer.UnlockAlpha1,
@@ -546,28 +718,78 @@
                     response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetMetadataResponse.SerializeToString,
             ),
             'SetMetadata': grpc.unary_unary_rpc_method_handler(
                     servicer.SetMetadata,
                     request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SetMetadataRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
+            'SubtleGetKeyAlpha1': grpc.unary_unary_rpc_method_handler(
+                    servicer.SubtleGetKeyAlpha1,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleGetKeyAlpha1Request.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleGetKeyAlpha1Response.SerializeToString,
+            ),
+            'SubtleEncryptAlpha1': grpc.unary_unary_rpc_method_handler(
+                    servicer.SubtleEncryptAlpha1,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleEncryptAlpha1Request.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleEncryptAlpha1Response.SerializeToString,
+            ),
+            'SubtleDecryptAlpha1': grpc.unary_unary_rpc_method_handler(
+                    servicer.SubtleDecryptAlpha1,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleDecryptAlpha1Request.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleDecryptAlpha1Response.SerializeToString,
+            ),
+            'SubtleWrapKeyAlpha1': grpc.unary_unary_rpc_method_handler(
+                    servicer.SubtleWrapKeyAlpha1,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleWrapKeyAlpha1Request.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleWrapKeyAlpha1Response.SerializeToString,
+            ),
+            'SubtleUnwrapKeyAlpha1': grpc.unary_unary_rpc_method_handler(
+                    servicer.SubtleUnwrapKeyAlpha1,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleUnwrapKeyAlpha1Request.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleUnwrapKeyAlpha1Response.SerializeToString,
+            ),
+            'SubtleSignAlpha1': grpc.unary_unary_rpc_method_handler(
+                    servicer.SubtleSignAlpha1,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleSignAlpha1Request.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleSignAlpha1Response.SerializeToString,
+            ),
+            'SubtleVerifyAlpha1': grpc.unary_unary_rpc_method_handler(
+                    servicer.SubtleVerifyAlpha1,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleVerifyAlpha1Request.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleVerifyAlpha1Response.SerializeToString,
+            ),
             'StartWorkflowAlpha1': grpc.unary_unary_rpc_method_handler(
                     servicer.StartWorkflowAlpha1,
                     request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.StartWorkflowRequest.FromString,
                     response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowReference.SerializeToString,
             ),
             'GetWorkflowAlpha1': grpc.unary_unary_rpc_method_handler(
                     servicer.GetWorkflowAlpha1,
                     request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetWorkflowRequest.FromString,
                     response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetWorkflowResponse.SerializeToString,
             ),
             'TerminateWorkflowAlpha1': grpc.unary_unary_rpc_method_handler(
                     servicer.TerminateWorkflowAlpha1,
-                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.TerminateWorkflowRequest.FromString,
-                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.TerminateWorkflowResponse.SerializeToString,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityRequest.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityResponse.SerializeToString,
+            ),
+            'PauseWorkflowAlpha1': grpc.unary_unary_rpc_method_handler(
+                    servicer.PauseWorkflowAlpha1,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityRequest.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityResponse.SerializeToString,
+            ),
+            'ResumeWorkflowAlpha1': grpc.unary_unary_rpc_method_handler(
+                    servicer.ResumeWorkflowAlpha1,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityRequest.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityResponse.SerializeToString,
+            ),
+            'RaiseEventWorkflowAlpha1': grpc.unary_unary_rpc_method_handler(
+                    servicer.RaiseEventWorkflowAlpha1,
+                    request_deserializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.RaiseEventWorkflowRequest.FromString,
+                    response_serializer=dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.RaiseEventWorkflowResponse.SerializeToString,
             ),
             'Shutdown': grpc.unary_unary_rpc_method_handler(
                     servicer.Shutdown,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
     }
@@ -952,14 +1174,31 @@
         return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/GetConfigurationAlpha1',
             dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationRequest.SerializeToString,
             dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetConfiguration(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/GetConfiguration',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationRequest.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.GetConfigurationResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def SubscribeConfigurationAlpha1(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -969,14 +1208,31 @@
         return grpc.experimental.unary_stream(request, target, '/dapr.proto.runtime.v1.Dapr/SubscribeConfigurationAlpha1',
             dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationRequest.SerializeToString,
             dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def SubscribeConfiguration(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/dapr.proto.runtime.v1.Dapr/SubscribeConfiguration',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationRequest.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubscribeConfigurationResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def UnsubscribeConfigurationAlpha1(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -986,14 +1242,31 @@
         return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/UnsubscribeConfigurationAlpha1',
             dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationRequest.SerializeToString,
             dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def UnsubscribeConfiguration(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/UnsubscribeConfiguration',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationRequest.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.UnsubscribeConfigurationResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def TryLockAlpha1(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1054,14 +1327,133 @@
         return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/SetMetadata',
             dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SetMetadataRequest.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def SubtleGetKeyAlpha1(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/SubtleGetKeyAlpha1',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleGetKeyAlpha1Request.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleGetKeyAlpha1Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubtleEncryptAlpha1(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/SubtleEncryptAlpha1',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleEncryptAlpha1Request.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleEncryptAlpha1Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubtleDecryptAlpha1(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/SubtleDecryptAlpha1',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleDecryptAlpha1Request.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleDecryptAlpha1Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubtleWrapKeyAlpha1(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/SubtleWrapKeyAlpha1',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleWrapKeyAlpha1Request.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleWrapKeyAlpha1Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubtleUnwrapKeyAlpha1(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/SubtleUnwrapKeyAlpha1',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleUnwrapKeyAlpha1Request.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleUnwrapKeyAlpha1Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubtleSignAlpha1(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/SubtleSignAlpha1',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleSignAlpha1Request.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleSignAlpha1Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubtleVerifyAlpha1(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/SubtleVerifyAlpha1',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleVerifyAlpha1Request.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.SubtleVerifyAlpha1Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def StartWorkflowAlpha1(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1099,16 +1491,67 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/TerminateWorkflowAlpha1',
-            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.TerminateWorkflowRequest.SerializeToString,
-            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.TerminateWorkflowResponse.FromString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityRequest.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def PauseWorkflowAlpha1(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/PauseWorkflowAlpha1',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityRequest.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ResumeWorkflowAlpha1(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/ResumeWorkflowAlpha1',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityRequest.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.WorkflowActivityResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def RaiseEventWorkflowAlpha1(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/dapr.proto.runtime.v1.Dapr/RaiseEventWorkflowAlpha1',
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.RaiseEventWorkflowRequest.SerializeToString,
+            dapr_dot_proto_dot_runtime_dot_v1_dot_dapr__pb2.RaiseEventWorkflowResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Shutdown(request,
             target,
             options=(),
```

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/serializers/__init__.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/serializers/base.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/serializers/base.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/serializers/json.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/serializers/json.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/serializers/util.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/serializers/util.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr/version/version.py` & `dapr-dev-1.9.0rc1.dev1502/dapr/version/version.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/PKG-INFO` & `dapr-dev-1.9.0rc1.dev1502/dapr_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-dev
-Version: 1.9.0rc1.dev1489
+Version: 1.9.0rc1.dev1502
 Summary: The developmental release for Dapr Python SDK.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/SOURCES.txt` & `dapr-dev-1.9.0rc1.dev1502/dapr_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/setup.cfg` & `dapr-dev-1.9.0rc1.dev1502/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1489/setup.py` & `dapr-dev-1.9.0rc1.dev1502/setup.py`

 * *Files identical despite different names*


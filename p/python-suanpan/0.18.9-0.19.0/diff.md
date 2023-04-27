# Comparing `tmp/python-suanpan-0.18.9.tar.gz` & `tmp/python-suanpan-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-suanpan-0.18.9.tar", last modified: Sat Oct  8 06:15:57 2022, max compression
+gzip compressed data, was "dist/python-suanpan-0.19.0.tar", last modified: Wed Apr 26 05:55:53 2023, max compression
```

## Comparing `python-suanpan-0.18.9.tar` & `python-suanpan-0.19.0.tar`

### file list

```diff
@@ -1,213 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/__suanpan__/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/__suanpan__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/__suanpan__/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/__suanpan__/tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/python_suanpan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/python_suanpan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4391 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/python_suanpan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/python_suanpan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/python_suanpan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/python_suanpan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/python_suanpan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/api/
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/component.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/api/hardware/
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/hardware/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/hardware/suanpan.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/oss.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/api/requests/
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/requests/affinity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/requests/host.py
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/api/sio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/app/
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/loops.py
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/message_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/app/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/modules/front.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/modules/images.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/modules/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/modules/params.py
--rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/modules/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/spark.py
--rw-r--r--   0 runner    (1001) docker     (121)     7895 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/app/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/arguments/
--rw-r--r--   0 runner    (1001) docker     (121)     7626 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/arguments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/arguments/auto.py
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)     7247 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/components.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/debug/
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/debug/ab.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/device/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/device/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/device/zmq.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/docker/
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/docker/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/dw/
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/dw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/dw/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)     5554 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/dw/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5090 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/dw/hive.py
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/dw/mock.py
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/dw/mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/dw/odps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/dw/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/error/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/component.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/device.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/imports.py
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/model.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/mq.py
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/mstorage.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/node.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/spark.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/state.py
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/error/tool.py
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/g.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/graph/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/graph/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/helper/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/helper/init_project.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/helper/sio_send.py
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)    11939 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/interfaces/optional.py
--rw-r--r--   0 runner    (1001) docker     (121)     4165 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/lazy_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/model/
--rw-r--r--   0 runner    (1001) docker     (121)     4537 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/model/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/mq/
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/mq/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)    14104 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/mq/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/mstorage/
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/mstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/mstorage/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/mstorage/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5182 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/mstorage/redis.py
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/mstorage/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/node/
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/node/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)     6539 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/node/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/node/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/node/spark.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/node/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     5667 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/path.py
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     4124 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/screenshots/
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/screenshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2567 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/screenshots/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/sfile/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/sfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/sfile/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/simple_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/spark/
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6325 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/spark/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)     3462 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/spark/db.py
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/spark/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     7660 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/spark/odpsops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/state/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1911 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/state/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/state/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/storage/
--rw-r--r--   0 runner    (1001) docker     (121)     2409 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8611 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/storage/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)    11166 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4701 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/storage/local.py
--rw-r--r--   0 runner    (1001) docker     (121)    19842 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/storage/minio.py
--rw-r--r--   0 runner    (1001) docker     (121)    24941 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/storage/oss.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/stream/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stream/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)    22784 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stream/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8463 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stream/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     3416 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stream/loops.py
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stream/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     7549 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stream/sio.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stream/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/stypes/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4568 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stypes/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stypes/argument.py
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stypes/node.py
--rw-r--r--   0 runner    (1001) docker     (121)    10361 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stypes/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/stypes/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/tools/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/tools/app/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/tools/app/graph/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/app/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/app/graph/download.py
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/app/graph/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/tools/dw/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/dw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/dw/download.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/dw/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/npy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/tools/storage/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/storage/copy.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/storage/download.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/storage/remove.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/tools/storage/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/excel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/npy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/pbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/pickle.py
--rw-r--r--   0 runner    (1001) docker     (121)     6462 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/port.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:15:57.000000 python-suanpan-0.18.9/suanpan/utils/term/
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/term/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14965 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/term/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/utils/text.py
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-10-08 06:15:52.000000 python-suanpan-0.18.9/suanpan/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/__suanpan__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/__suanpan__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/__suanpan__/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/__suanpan__/tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/python_suanpan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/python_suanpan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/python_suanpan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/python_suanpan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/python_suanpan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/python_suanpan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/python_suanpan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/python_suanpan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/api/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/hardware/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/hardware/suanpan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/oss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/api/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/requests/affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/requests/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/api/sio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/message_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/app/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/modules/front.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/modules/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/modules/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/modules/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/modules/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/app/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/arguments/
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/arguments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/arguments/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/debug/ab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/device/zmq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/docker/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/dw/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/dw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/dw/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/dw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/dw/hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/dw/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/dw/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/dw/odps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/dw/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/mq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/mstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/error/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/g.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/graph/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/helper/init_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/helper/sio_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/interfaces/optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/lazy_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/model/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/mq/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/mq/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/mq/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/mstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/mstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/mstorage/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/mstorage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/mstorage/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/mstorage/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/node/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/node/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/node/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/node/spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/node/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/node_badge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/screenshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/screenshots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/service_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/sfile/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/sfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/sfile/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/simple_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/spark/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/spark/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/spark/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/spark/odpsops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/state/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/state/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/state/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/storage/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/storage/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20047 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/storage/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25133 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/storage/oss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stream/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stream/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stream/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stream/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stream/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stream/sio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stream/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/stypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stypes/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stypes/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stypes/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stypes/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/stypes/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/tools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/tools/app/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/app/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/app/graph/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/app/graph/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/tools/dw/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/dw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/dw/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/dw/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/npy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/tools/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/storage/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/storage/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/storage/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/tools/storage/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/npy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/pbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:55:53.000000 python-suanpan-0.19.0/suanpan/utils/term/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/term/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/term/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-26 05:55:49.000000 python-suanpan-0.19.0/suanpan/version.py
```

### Comparing `python-suanpan-0.18.9/PKG-INFO` & `python-suanpan-0.19.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-suanpan
-Version: 0.18.9
+Version: 0.19.0
 Summary: Suanpan SDK
 Home-page: UNKNOWN
 Author: yanqinghao
 Author-email: woshiyanqinghao@gmail.com
 License: See License
 Description: # AiLab
         
@@ -15,9 +15,9 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `python-suanpan-0.18.9/__suanpan__/tensorflow.py` & `python-suanpan-0.19.0/__suanpan__/tensorflow.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/python_suanpan.egg-info/PKG-INFO` & `python-suanpan-0.19.0/python_suanpan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-suanpan
-Version: 0.18.9
+Version: 0.19.0
 Summary: Suanpan SDK
 Home-page: UNKNOWN
 Author: yanqinghao
 Author-email: woshiyanqinghao@gmail.com
 License: See License
 Description: # AiLab
         
@@ -15,9 +15,9 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `python-suanpan-0.18.9/python_suanpan.egg-info/SOURCES.txt` & `python-suanpan-0.19.0/python_suanpan.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 setup.py
 __suanpan__/__init__.py
 __suanpan__/asyncio.py
 __suanpan__/tensorflow.py
 python_suanpan.egg-info/PKG-INFO
 python_suanpan.egg-info/SOURCES.txt
 python_suanpan.egg-info/dependency_links.txt
+python_suanpan.egg-info/entry_points.txt
 python_suanpan.egg-info/not-zip-safe
 python_suanpan.egg-info/requires.txt
 python_suanpan.egg-info/top_level.txt
 suanpan/__init__.py
 suanpan/asyncio.py
 suanpan/components.py
 suanpan/g.py
 suanpan/imports.py
 suanpan/lazy_import.py
 suanpan/log.py
+suanpan/node_badge.py
 suanpan/notebook.py
 suanpan/objects.py
 suanpan/path.py
 suanpan/proxy.py
 suanpan/run.py
 suanpan/runtime.py
+suanpan/service_registry.py
 suanpan/simple_run.py
 suanpan/version.py
 suanpan/api/__init__.py
 suanpan/api/app.py
 suanpan/api/auth.py
 suanpan/api/component.py
 suanpan/api/oss.py
```

### Comparing `python-suanpan-0.18.9/python_suanpan.egg-info/requires.txt` & `python-suanpan-0.19.0/python_suanpan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/setup.py` & `python-suanpan-0.19.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,25 +77,31 @@
 packages = find_packages(exclude=["tests"])
 packages.extend(fix_packages)
 
 setup(
     name="python-suanpan",
     version=VERSION,
     packages=packages,
+    package_data={"suanpan": ["helper/example/*/*", "stream/*.so"]},
     license="See License",
     author="yanqinghao",
     author_email="woshiyanqinghao@gmail.com",
     description="Suanpan SDK",
     long_description=read_file(README),
     long_description_content_type="text/markdown",
     zip_safe=False,
     include_package_data=True,
     platforms="any",
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=INSTALL_REQUIRES,
+    entry_points={
+        'console_scripts': [
+            'suanpan = suanpan:helper',
+        ],
+    },
     classifiers=[
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

### Comparing `python-suanpan-0.18.9/suanpan/api/app.py` & `python-suanpan-0.19.0/suanpan/api/app.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/api/auth.py` & `python-suanpan-0.19.0/suanpan/api/auth.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/api/component.py` & `python-suanpan-0.19.0/suanpan/api/component.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/api/hardware/__init__.py` & `python-suanpan-0.19.0/suanpan/api/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/api/hardware/suanpan.py` & `python-suanpan-0.19.0/suanpan/api/hardware/suanpan.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/api/requests/__init__.py` & `python-suanpan-0.19.0/suanpan/api/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/api/requests/affinity.py` & `python-suanpan-0.19.0/suanpan/api/requests/affinity.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/api/requests/host.py` & `python-suanpan-0.19.0/suanpan/api/requests/host.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/app/__init__.py` & `python-suanpan-0.19.0/suanpan/app/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/app/arguments.py` & `python-suanpan-0.19.0/suanpan/app/arguments.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/app/base.py` & `python-suanpan-0.19.0/suanpan/app/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 from suanpan.log import logger
 from suanpan.objects import HasName
 from suanpan.app import MessageHandler
 from suanpan.node import node
 
 
 class BaseApp(HasName):
+    def __init__(self):
+        self._auto_in = None
+        self._auto_out = None
+        self._auto_param = None
+
     def __call__(self, *args, **kwargs):
         raise NotImplementedError("Method not implemented!")
 
     def start(self, *args, **kwargs):  # pylint: disable=unused-argument
         logger.info(f"Suanpan component {self.name} start...")
 
     def use(self, handlerClass):
@@ -38,28 +43,44 @@
         self.afterInit(handler.afterInit)
         self.beforeCall(handler.beforeCall)
         self.afterCall(handler.afterCall)
 
         self(handler.run)
         handler.initialize()
 
-    def loadNodeArgs(self, funcOrApp=None):
+    def loadNodeArgs(self, funcOrApp=None, *, autoIn=True, autoOut=True, autoParam=True):
+        self._auto_in = autoIn
+        self._auto_out = autoOut
+        self._auto_param = autoParam
         self.beforeInit(self._load_node_info)
-        if funcOrApp:
+
+        def decorator(func2):
+            # func2 is main message loop function
+            self(func2)
+            return self
+
+        if funcOrApp is not None:
+            # loadNodeArgs with no args
             self(funcOrApp)
-        return self
+            return self
+        else:
+            # loadNodeArgs with args
+            return decorator
 
     def _load_node_info(self):
         logger.debug('auto load node args and params')
-        for inarg in node.inargs:
-            self.input(inarg)
-        for outarg in node.outargs:
-            self.output(outarg)
-        for paramarg in node.paramargs:
-            self.param(paramarg)
+        if self._auto_in:
+            for inarg in node.inargs:
+                self.input(inarg)
+        if self._auto_out:
+            for outarg in node.outargs:
+                self.output(outarg)
+        if self._auto_param:
+            for paramarg in node.paramargs:
+                self.param(paramarg)
 
     @property
     def trigger(self):
         raise NotImplementedError(f"{self.name} not support trigger")
 
     def input(self, argument):
         raise NotImplementedError("Method not implemented!")
```

### Comparing `python-suanpan-0.18.9/suanpan/app/docker.py` & `python-suanpan-0.19.0/suanpan/app/docker.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/app/message_handler.py` & `python-suanpan-0.19.0/suanpan/app/message_handler.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/app/modules/__init__.py` & `python-suanpan-0.19.0/suanpan/app/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/app/modules/base.py` & `python-suanpan-0.19.0/suanpan/app/modules/base.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/app/modules/images.py` & `python-suanpan-0.19.0/suanpan/app/modules/images.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/app/modules/params.py` & `python-suanpan-0.19.0/suanpan/app/modules/params.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/app/modules/storage.py` & `python-suanpan-0.19.0/suanpan/app/modules/storage.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/app/spark.py` & `python-suanpan-0.19.0/suanpan/app/spark.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/app/stream.py` & `python-suanpan-0.19.0/suanpan/app/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,18 @@
         raise NotImplementedError("Method not implemented!")
 
     @functional.lazyproperty
     def _loop(self):
         raise NotImplementedError("Method not implemented!")
 
     @functional.lazyproperty
+    def _ergo_loop(self):
+        raise NotImplementedError("Method not implemented!")
+
+    @functional.lazyproperty
     def _handler(self):
         return self._loop.getHandler()
 
     def bootstrap(self):
         self.modules.info()
 
     @property
@@ -93,14 +97,17 @@
 
     def load(self, *args, **kwargs):
         return self._handler.load(*args, **kwargs)
 
     def send(self, *args, **kwargs):
         return self._loop.send(*args, **kwargs)
 
+    def ergo_send(self, *args, **kwargs):
+        return self._ergo_loop.ergo_send(*args, **kwargs)
+
     def save(self, *args, **kwargs):
         return self.send(*args, **kwargs)
 
     def publish(self, topic: str, payload: dict):
         data = json.dumps(payload)
         self._stream.pubsubLoop.send(topic, data)
 
@@ -120,14 +127,18 @@
     def _stream(self):
         return Stream()
 
     @functional.lazyproperty
     def _loop(self):
         return self._stream.callLoop
 
+    @functional.lazyproperty
+    def _ergo_loop(self):
+        return self._stream.ergoLoop
+
     @property
     def args(self):
         return self._stream.args
 
     @property
     def vars(self):
         return self._stream.vars
```

### Comparing `python-suanpan-0.18.9/suanpan/arguments/__init__.py` & `python-suanpan-0.19.0/suanpan/arguments/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # coding=utf-8
 from __future__ import absolute_import, print_function
-
-import os
-
 from suanpan import error, utils
 from suanpan.log import logger
 from suanpan.objects import HasName
 from suanpan.utils import env, json
 
 DEFAULT_MAX_VALUE_LENGTH = 120
 
@@ -19,14 +16,15 @@
         self.alias = kwargs.pop("alias", None)
         self.label = kwargs.pop("label", None)
         self.required = kwargs.pop("required", False)
         self.default = kwargs.pop("default", None)
         self.choices = kwargs.pop("choices", [])
         self.type = kwargs.pop("type", str)
         self.value = None
+        self.use_argo = False
 
         self.kwargs = self.cleanParams(kwargs)
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     @property
     def preprocess(self):
@@ -55,16 +53,27 @@
             raise error.ArgumentRequiredError(f"{self.key} is required")
         return self
 
     def format(self):
         if self.value is None:
             self.value = self.default
         else:
+            from suanpan.storage.arguments import StorageArg
+
+            bytes_transform = False
+            if isinstance(self.value, bytes):
+                if issubclass(self.__class__, StorageArg):
+                    bytes_transform = True
+                else:
+                    self.value = self.value.decode("utf8")
             try:
-                self.value = self.transform(self.value)
+                if bytes_transform:
+                    self.value = self.bytes_transform(self.value)
+                else:
+                    self.value = self.transform(self.value)
                 if getattr(self, "preprocess", None):
                     self.value = self.preprocess(self.value)
             except Exception as e:
                 raise error.ArgumentTypeError(
                     f"({self.name}) {self.key}: {utils.shorten(self.value, maxlen=self.MAX_VALUE_LENGTH)}"
                 ) from e
         if self.choices and self.value not in self.choices.values():
@@ -73,14 +82,17 @@
             )
         self.logLoaded(self.value)
         return self
 
     def transform(self, value):
         return self.type(value)
 
+    def bytes_transform(self, value):
+        raise NotImplementedError
+
     def clean(self):  # pylint: disable=unused-argument
         return self
 
     def save(self, result):  # pylint: disable=unused-argument
         self.logSaved(result.value)
         return result.value
```

### Comparing `python-suanpan-0.18.9/suanpan/asyncio.py` & `python-suanpan-0.19.0/suanpan/asyncio.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/components.py` & `python-suanpan-0.19.0/suanpan/components.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/debug/__init__.py` & `python-suanpan-0.19.0/suanpan/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/debug/ab.py` & `python-suanpan-0.19.0/suanpan/debug/ab.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/device/base.py` & `python-suanpan-0.19.0/suanpan/device/base.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/device/zmq.py` & `python-suanpan-0.19.0/suanpan/device/zmq.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/docker/__init__.py` & `python-suanpan-0.19.0/suanpan/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/docker/arguments.py` & `python-suanpan-0.19.0/suanpan/docker/arguments.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/dw/__init__.py` & `python-suanpan-0.19.0/suanpan/dw/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/dw/arguments.py` & `python-suanpan-0.19.0/suanpan/dw/arguments.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/dw/base.py` & `python-suanpan-0.19.0/suanpan/dw/base.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/dw/hive.py` & `python-suanpan-0.19.0/suanpan/dw/hive.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/dw/mysql.py` & `python-suanpan-0.19.0/suanpan/dw/mysql.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/dw/odps.py` & `python-suanpan-0.19.0/suanpan/dw/odps.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/dw/postgres.py` & `python-suanpan-0.19.0/suanpan/dw/postgres.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/error/__init__.py` & `python-suanpan-0.19.0/suanpan/error/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/error/mstorage.py` & `python-suanpan-0.19.0/suanpan/error/mstorage.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/error/stream.py` & `python-suanpan-0.19.0/suanpan/error/stream.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/g.py` & `python-suanpan-0.19.0/suanpan/g.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,8 +48,9 @@
     desktopHome=env.lazyget("SP_DESKTOP_HOME", default=""),
     backendPort=env.lazyget("SP_PORT", type=env.Int, default=7000),
     portStart=env.lazyget("SP_PORT_START", type=env.Int, default=10000),
     portEnd=env.lazyget("SP_PORT_END", type=env.Int, default=20000),
     # service disable
     serviceSioDisable=env.lazyget("SP_SERVICE_SIO_DISABLE", type=env.Bool, default=False),
     serviceHttpDisable=env.lazyget("SP_SERVICE_HTTP_DISABLE", type=env.Bool, default=False),
+    serviceErgoEnable=env.lazyget("SP_SERVICE_ERGO_ENABLE", type=env.Bool, default=False),
 )
```

### Comparing `python-suanpan-0.18.9/suanpan/graph/base.py` & `python-suanpan-0.19.0/suanpan/graph/base.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/helper/init_project.py` & `python-suanpan-0.19.0/suanpan/helper/init_project.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/helper/sio_send.py` & `python-suanpan-0.19.0/suanpan/helper/sio_send.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,21 @@
             data = json.load(f)
     else:
         data = json.loads(data_string)
 
     sio = socketio.Client()
     sio.connect('http://localhost:8888')
 
-    def callback(resp):
+    def callback(*args):
+        if len(args) == 0:
+            print('invalid event')
+            sio.disconnect()
+            return
+
+        resp = args[0]
         print('=' * 32)
         print('Response:')
         print(json.dumps(resp, indent=2))
         sio.disconnect()
 
     print('Send Request:')
     print(json.dumps(data, indent=2))
```

### Comparing `python-suanpan-0.18.9/suanpan/imports.py` & `python-suanpan-0.19.0/suanpan/imports.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/interfaces/__init__.py` & `python-suanpan-0.19.0/suanpan/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/interfaces/optional.py` & `python-suanpan-0.19.0/suanpan/interfaces/optional.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/lazy_import.py` & `python-suanpan-0.19.0/suanpan/lazy_import.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/log.py` & `python-suanpan-0.19.0/suanpan/log.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/model/__init__.py` & `python-suanpan-0.19.0/suanpan/model/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/model/arguments.py` & `python-suanpan-0.19.0/suanpan/model/arguments.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/mq/__init__.py` & `python-suanpan-0.19.0/suanpan/mq/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/mq/redis.py` & `python-suanpan-0.19.0/suanpan/mq/redis.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/mstorage/__init__.py` & `python-suanpan-0.19.0/suanpan/mstorage/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/mstorage/arguments.py` & `python-suanpan-0.19.0/suanpan/mstorage/arguments.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/mstorage/base.py` & `python-suanpan-0.19.0/suanpan/mstorage/base.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/mstorage/redis.py` & `python-suanpan-0.19.0/suanpan/mstorage/redis.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/mstorage/vars.py` & `python-suanpan-0.19.0/suanpan/mstorage/vars.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/node/arguments.py` & `python-suanpan-0.19.0/suanpan/node/arguments.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/node/base.py` & `python-suanpan-0.19.0/suanpan/node/base.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/notebook.py` & `python-suanpan-0.19.0/suanpan/notebook.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/objects.py` & `python-suanpan-0.19.0/suanpan/objects.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/path.py` & `python-suanpan-0.19.0/suanpan/path.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/proxy.py` & `python-suanpan-0.19.0/suanpan/proxy.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/run.py` & `python-suanpan-0.19.0/suanpan/run.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/runtime.py` & `python-suanpan-0.19.0/suanpan/runtime.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/screenshots/__init__.py` & `python-suanpan-0.19.0/suanpan/screenshots/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/screenshots/base.py` & `python-suanpan-0.19.0/suanpan/screenshots/base.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/sfile/settings.py` & `python-suanpan-0.19.0/suanpan/sfile/settings.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/simple_run.py` & `python-suanpan-0.19.0/suanpan/simple_run.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/spark/__init__.py` & `python-suanpan-0.19.0/suanpan/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/spark/arguments.py` & `python-suanpan-0.19.0/suanpan/spark/arguments.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/spark/db.py` & `python-suanpan-0.19.0/suanpan/spark/db.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/spark/io.py` & `python-suanpan-0.19.0/suanpan/spark/io.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/spark/odpsops.py` & `python-suanpan-0.19.0/suanpan/spark/odpsops.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/state/base.py` & `python-suanpan-0.19.0/suanpan/state/base.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/state/storage.py` & `python-suanpan-0.19.0/suanpan/state/storage.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/storage/__init__.py` & `python-suanpan-0.19.0/suanpan/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/storage/arguments.py` & `python-suanpan-0.19.0/suanpan/storage/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from suanpan.utils import csv, excel, image, json, npy, text
 
 
 class StorageArg(Arg):
     def getOutputTmpValue(self, *args):
         return storage.delimiter.join(args)
 
+    def bytes_transform(self, value):
+        raise NotImplementedError
+
 
 class NameFile(StorageArg):
     def __init__(self, key, **kwargs):
         self.objectPrefix = None  # oss path to save file
         self.filePath = None
         super().__init__(key, **kwargs)
 
@@ -72,43 +75,58 @@
     @property
     def isSet(self):
         return True
 
     def load(self, args):
         super().load(args)
         if self.value:
-            self.value = self.value.replace('{{userId}}', g.userId).replace('{{appId}}', g.appId)
-            self.objectPrefix = self.value
-            self.objectName = storage.storagePathJoin(self.objectPrefix, self.fileName)
-            self.filePath = storage.getPathInTempStore(self.objectName)
-            self.value = self.filePath
+            if isinstance(self.value, bytes):
+                self.filePath = storage.getPathInNodeTmpStore(self.fileName)
+            else:
+                self.value = self.value.replace('{{userId}}', g.userId).replace('{{appId}}', g.appId)
+                self.objectPrefix = self.value
+                self.objectName = storage.storagePathJoin(self.objectPrefix, self.fileName)
+                self.filePath = storage.getPathInTempStore(self.objectName)
+                self.value = self.filePath
         return self
 
     def transform(self, value):
         if self.filePath:
             _download = (
                 storage.download if self.required else runtime.saferun(storage.download)
             )
             _download(self.objectName, self.filePath)
         return self.filePath
 
+    def bytes_transform(self, value):
+        if self.filePath:
+            path.mkdirs(self.filePath, parent=True)
+            with open(self.filePath, 'wb') as f:
+                f.write(value)
+        return self.filePath
+
     def clean(self):
         if self.filePath:
             path.remove(self.filePath)
             logger.debug("clean folder from {} to {}".format(self.filePath, storage.tempStore))
             path.removeEmptyFoldersTo(os.path.dirname(self.filePath), storage.tempStore)
         return self
 
     def save(self, result):
         filePath = result.value
-        storage.upload(self.objectName, filePath)
-        if filePath != self.filePath:
-            path.remove(filePath)
-        self.logSaved(self.objectName)
-        return self.objectPrefix
+        if self.use_argo:
+            with open(filePath, 'rb') as f:
+                data = f.read()
+            return data
+        else:
+            storage.upload(self.objectName, filePath)
+            if filePath != self.filePath:
+                path.remove(filePath)
+            self.logSaved(self.objectName)
+            return self.objectPrefix
 
 
 class Folder(StorageArg):
     def __init__(self, key, **kwargs):
         super().__init__(key, **kwargs)
         self.folderName = None
         self.folderPath = None
@@ -288,14 +306,21 @@
     def transform(self, value):
         filePath = super().transform(value)
         if not filePath:
             return None
         _read = image.read if self.required else runtime.saferun(image.read)
         return _read(filePath)
 
+    def bytes_transform(self, value):
+        filePath = super().bytes_transform(value)
+        if not filePath:
+            return None
+        _read = image.read if self.required else runtime.saferun(image.read)
+        return _read(filePath)
+
     def save(self, result):
         image.save(self.filePath, result.value)
         return super().save(Result.froms(value=self.filePath))
 
 
 class Screenshots(Image):
     FILENAME = "screenshots"
```

### Comparing `python-suanpan-0.18.9/suanpan/storage/base.py` & `python-suanpan-0.19.0/suanpan/storage/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import absolute_import, print_function
 
 import abc
 import os
 import tempfile
 import zipfile
 import pathlib
-
+from datetime import datetime, timezone
 from suanpan import g
 from suanpan import path as spath
 from suanpan.log import logger
 from suanpan.objects import HasName
 from suanpan.utils import functional
 
 
@@ -20,19 +20,19 @@
     DEFAULT_TEMP_DATA_STORE = tempfile.gettempdir()
     DEFAULT_GLOBAL_DATA_STORE = "/global"
     DEFAULT_IGNORE_KEYWORDS = ("__MACOSX", ".DS_Store")
     CONTENT_MD5 = "Content-MD5"
     PBAR_FORMAT = "{l_bar}{bar}"
 
     def __init__(
-        self,
-        delimiter=os.sep,
-        tempStore=DEFAULT_TEMP_DATA_STORE,
-        globalStore=DEFAULT_GLOBAL_DATA_STORE,
-        **kwargs,
+            self,
+            delimiter=os.sep,
+            tempStore=DEFAULT_TEMP_DATA_STORE,
+            globalStore=DEFAULT_GLOBAL_DATA_STORE,
+            **kwargs,
     ):  # pylint: disable=unused-argument
         self.delimiter = delimiter
         self.tempStore = tempStore
         self.globalStore = globalStore
 
     @abc.abstractmethod
     def download(self, name, path, progress=None, **kwargs):
@@ -157,14 +157,17 @@
     def nodeLogsStoreKey(self):
         return self.storagePathJoin("studio", g.userId, "logs", g.appId, g.nodeId)
 
     @functional.lazyproperty
     def componentsStoreKey(self):
         return self.storagePathJoin("studio", g.userId, "component")
 
+    def getKeyInGlobalStore(self, *paths):
+        return self.storagePathJoin("studio", "global", *paths)
+
     def getKeyInAppStore(self, *paths):
         return self.storagePathJoin(self.appStoreKey, *paths)
 
     def getKeyInAppDataStore(self, *paths):
         return self.storagePathJoin(self.appDataStoreKey, *paths)
 
     def getKeyInAppConfigsStore(self, *paths):
@@ -262,15 +265,15 @@
 
     def storageRelativePath(self, path, base, delimiter=None):
         delimiter = delimiter or self.delimiter
         return self._relativePath(path, base, delimiter=delimiter)
 
     def _relativePath(self, path, base, delimiter):
         base = base if base.endswith(delimiter) else base + delimiter
-        return path[len(base) :] if path.startswith(base) else path
+        return path[len(base):] if path.startswith(base) else path
 
     @abc.abstractmethod
     def getStorageMd5(self, name, **kwargs):
         pass
 
     def getLocalMd5(self, path, **kwargs):  # pylint: disable=unused-argument
         return spath.md5(path) if os.path.isfile(path) else None
@@ -312,7 +315,22 @@
         return path.split(delimiter)
 
     def pathSplitExt(self, path, extDelimiter="."):
         return path.rsplit(extDelimiter, 1)
 
     def basename(self, path, delimiter=None):
         return self.pathSplit(path, delimiter=delimiter)[-1]
+
+
+class ObjectStat(object):
+    def __init__(self, obj, typ='minio'):
+        self.content_type = obj.content_type
+        self.etag = obj.etag
+
+        if typ == 'minio':
+            self.last_modified = obj.last_modified
+            self.size = obj.size
+            self.version_id = obj.version_id
+        else:
+            self.last_modified = datetime.fromtimestamp(obj.last_modified, timezone.utc)
+            self.size = obj.content_length
+            self.version_id = obj.versionid
```

### Comparing `python-suanpan-0.18.9/suanpan/storage/local.py` & `python-suanpan-0.19.0/suanpan/storage/local.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/storage/minio.py` & `python-suanpan-0.19.0/suanpan/storage/minio.py`

 * *Files 1% similar despite different names*

```diff
@@ -537,14 +537,19 @@
                 return None
             raise e
 
     def getStorageSize(self, key, bucket=None):
         bucket = bucket or self.bucket
         return self.autoRefreshToken(self.client.stat_object)(bucket, key).size
 
+    def statObject(self, key, bucket=None):
+        bucket = bucket or self.bucket
+        stat = self.autoRefreshToken(self.client.stat_object)(bucket, key)
+        return base.ObjectStat(stat, 'minio')
+
     def storageUrl(self, key, bucket=None):
         bucket = bucket or self.bucket
         return "minio:///" + self.storagePathJoin(bucket, key)
 
     def _getObjectNames(self, objects):
         return (
             [obj.object_name for obj in objects]
```

### Comparing `python-suanpan-0.18.9/suanpan/storage/oss.py` & `python-suanpan-0.19.0/suanpan/storage/oss.py`

 * *Files 1% similar despite different names*

```diff
@@ -728,7 +728,12 @@
 
     def _getObjectNames(self, objects):
         return (
             [obj.key for obj in objects]
             if isinstance(objects, (tuple, list))
             else objects.key
         )
+
+    def statObject(self, key, bucketOrBucketName=None):
+        bucket = self.getBucket(bucketOrBucketName)
+        stat = bucket.head_object(key)
+        return base.ObjectStat(stat, 'oss')
```

### Comparing `python-suanpan-0.18.9/suanpan/stream/arguments.py` & `python-suanpan-0.19.0/suanpan/stream/arguments.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/stream/base.py` & `python-suanpan-0.19.0/suanpan/stream/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 from __future__ import absolute_import, print_function
 
 import abc
 import os
 import sys
 import traceback
 import uuid
-import gc
 import logging
 import gevent
 import gevent.pywsgi
 import gevent.util
+import copy
 import socketio
 from engineio import static_files
-from gevent._greenlet_primitives import get_reachable_greenlets
-
 from suanpan import asyncio, error, g, runtime, utils
 from suanpan.arguments import Bool, BoolOrInt, Float, Int, String
 from suanpan.components import Arguments
 from suanpan.interfaces import HasDevMode, HasExitHooks, HasInitHooks, HasLogger, HasEventHooks
 from suanpan.interfaces.optional import HasBaseServices
 from suanpan.log import logger
 from suanpan.mq import mq
@@ -26,14 +24,15 @@
 from suanpan.storage import storage
 from suanpan.stream import handlers, loops
 from suanpan.stream.interfaces import HasHandlers
 from suanpan.stream.objects import Context
 from suanpan.stream.sio import StreamServer, WebSocketHandler
 from suanpan.utils import functional, json, port
 from suanpan.path import rootDir
+from suanpan.objects import Context
 
 
 class Stream(
     HasBaseServices, HasLogger, HasDevMode, HasInitHooks, HasExitHooks, HasHandlers, HasEventHooks
 ):
     STREAM_ARGUMENTS = [
         String("stream-recv-queue", default=f"mq-{g.nodeId}"),
@@ -48,14 +47,15 @@
         String("stream-send-queue", default="mq-master"),
         Int("stream-send-queue-max-length", default=1000),
         Bool("stream-send-queue-trim-immediately", default=False),
         String("stream-sio-static-folder", default="/web"),
         String("stream-sio-static-url-prefix", default="/"),
         String("stream-app-event-hub", default=f"app-event-hub-{g.appId}"),
         Int("stream-app-event-hub-max-length", default=1000),
+        Bool("stream-enable-ergo", default=False),
     ]
     STREAM_PARAMS_FILE = "params.json"
 
     def __init__(self):
         super().__init__()
         self.title = ""
         self.argsDict = {}
@@ -64,18 +64,19 @@
         self._exit_code = 0
 
         self.callLoop = StreamCallLoop(self)
         self.triggerLoop = StreamTriggerLoop(self)
         self.sioLoop = StreamSIOLoop(self)
         self.httpLoop = StreamHTTPLoop(self)
         self.pubsubLoop = StreamPubsubLoop(self)
+        self.ergoLoop = StreamErgoLoop(self)
 
     @property
     def loops(self):
-        return [self.callLoop, self.triggerLoop, self.sioLoop, self.httpLoop, self.pubsubLoop]
+        return [self.callLoop, self.triggerLoop, self.sioLoop, self.httpLoop, self.pubsubLoop, self.ergoLoop]
 
     def beforeInit(self):
         logger.logDebugInfo()
         logger.debug(f"Stream {self.name} starting...")
 
     def init(self, *args, **kwargs):
         self.argsDict = self.getArgsDict(*args, **kwargs)
@@ -667,7 +668,64 @@
         )
         return mq.sendEvent(
             self.stream.options["stream-app-event-hub"],
             data,
             maxlen=self.stream.options["stream-app-event-hub-max-length"],
             trimImmediately=self.stream.options["stream-send-queue-trim-immediately"],
         )
+
+
+class StreamErgoLoop(StreamMQBaseLoop):
+    DEFAULT_HANDLER_KEY = "call"
+    DEFAULT_HANDLER_CLASS = handlers.CallHandler
+
+    def __init__(self, stream):
+        super().__init__(stream)
+
+    @property
+    def ready(self):
+        try:
+            from . import ergo
+        except ImportError:
+            logger.warning("failed to import the ergo.so")
+            return False
+        return self.stream.options["stream-enable-ergo"] or g.serviceErgoEnable
+
+    def close(self):
+        from . import ergo
+        logger.debug("Stream Ergo Loop Closing...")
+        ergo.close()
+        logger.debug("Stream Ergo Loop Closed")
+
+    def getHandler(self):
+        return self.stream.callLoop.getHandler()
+
+    def _ergo_send(self, result, message_id, output):
+        from . import ergo
+        logger.debug(utils.shorten(f"Send to ergo {output}: {result}", self.DEFAULT_LOGGER_MAX_LENGTH))
+        if isinstance(result, str):
+            result = result.encode('utf8')
+        ergo.send(result, message_id, output)
+
+    def ergo_send(self, results, message=None, args=None, **_):
+        if not self.ready:
+            raise Exception('ergo is not enabled')
+
+        message = message or self.generateMessage()
+        if not args:
+            args = copy.deepcopy(self.getHandler().getArguments(include="outputs"))
+        for arg in args:
+            arg.use_argo = True
+        outputs = self.getHandler().save(results, args=args, message=message)
+        for key, value in outputs.items():
+            self._ergo_send(value, message["id"], key)
+
+    @runtime.globalrun
+    def start(self):
+        from . import ergo
+
+        ergo.init()
+        logger.debug("Stream Ergo Loop Starting...")
+        while True:
+            msg, msg_id, in_port = ergo.recv()
+            message = {'id': msg_id, in_port: msg}
+            self.handle(message)
```

### Comparing `python-suanpan-0.18.9/suanpan/stream/handlers.py` & `python-suanpan-0.19.0/suanpan/stream/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,23 @@
     def formatAsOuts(self, args, results):
         return {
             f"out{i + 1}": self.getArgumentValueFromDict(results, arg)
             for i, arg in enumerate(args)
         }
 
     def stringifyOuts(self, outs):
-        return {k: str(v) for k, v in outs.items() if v is not None}
+        o = {}
+        for k, v in outs.items():
+            if v is None:
+                continue
+            if isinstance(v, bytes):
+                o[k] = v
+            else:
+                o[k] = str(v)
+        return o
 
     def shortenRequestID(self, requestID):
         return requestID.replace("-", "")
 
     def clean(self):
         super(CallHandler, self).clean()
         for argument in self._input_arguments:
```

### Comparing `python-suanpan-0.18.9/suanpan/stream/interfaces.py` & `python-suanpan-0.19.0/suanpan/stream/interfaces.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/stream/loops.py` & `python-suanpan-0.19.0/suanpan/stream/loops.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/stream/sio.py` & `python-suanpan-0.19.0/suanpan/stream/sio.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/stream/vars.py` & `python-suanpan-0.19.0/suanpan/stream/vars.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/stypes/app.py` & `python-suanpan-0.19.0/suanpan/stypes/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,22 @@
     @property
     @abc.abstractmethod
     def trigger(self) -> 'TriggerT':
         """Get a trigger instance that can run task at periodic intervals."""
         ...
 
     @abc.abstractmethod
-    def loadNodeArgs(self, funcOrApp=None):
+    def loadNodeArgs(self, funcOrApp=None, *, autoIn=True, autoOut=True, autoParam=True):
         """Decorate a function to run with autoload node args.
 
         Arguments:
             funcOrApp: The function to decorate.
+            autoIn: autoload node input args
+            autoOut: autoload node output args
+            autoParam: autoload node params
 
         Example:
             >>> @app.loadNodeArgs
             >>> def example(context):
             ...     args = context.args
         """
         ...
```

### Comparing `python-suanpan-0.18.9/suanpan/stypes/argument.py` & `python-suanpan-0.19.0/suanpan/stypes/argument.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/stypes/node.py` & `python-suanpan-0.19.0/suanpan/stypes/node.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/stypes/storage.py` & `python-suanpan-0.19.0/suanpan/stypes/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,18 @@
         Arguments:
             key: Object name in the bucket.
             data: A string object.
             bucket: Name of the bucket.
         """
         ...
 
+    @abc.abstractmethod
+    def statObject(self, key, bucket=None):
+        ...
+
     @property
     def appStoreKey(self):
         return self.storagePathJoin("studio", g.userId, g.appId)
 
     @property
     def appDataStoreKey(self):
         return self.storagePathJoin("studio", g.userId, "share", g.appId)
@@ -181,14 +185,17 @@
     def nodeLogsStoreKey(self):
         return self.storagePathJoin("studio", g.userId, "logs", g.appId, g.nodeId)
 
     @property
     def componentsStoreKey(self):
         return self.storagePathJoin("studio", g.userId, "component")
 
+    def getKeyInGlobalStore(self, *paths):
+        return self.storagePathJoin("studio", "global", *paths)
+
     def getKeyInAppStore(self, *paths):
         return self.storagePathJoin(self.appStoreKey, *paths)
 
     def getKeyInAppDataStore(self, *paths):
         return self.storagePathJoin(self.appDataStoreKey, *paths)
 
     def getKeyInAppConfigsStore(self, *paths):
```

### Comparing `python-suanpan-0.18.9/suanpan/stypes/trigger.py` & `python-suanpan-0.19.0/suanpan/stypes/trigger.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/tools/app/graph/download.py` & `python-suanpan-0.19.0/suanpan/tools/app/graph/download.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/tools/app/graph/upload.py` & `python-suanpan-0.19.0/suanpan/tools/app/graph/upload.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/tools/npy.py` & `python-suanpan-0.19.0/suanpan/tools/npy.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/__init__.py` & `python-suanpan-0.19.0/suanpan/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/convert.py` & `python-suanpan-0.19.0/suanpan/utils/convert.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/csv.py` & `python-suanpan-0.19.0/suanpan/utils/csv.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/env.py` & `python-suanpan-0.19.0/suanpan/utils/env.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/excel.py` & `python-suanpan-0.19.0/suanpan/utils/excel.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/functional.py` & `python-suanpan-0.19.0/suanpan/utils/functional.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/image.py` & `python-suanpan-0.19.0/suanpan/utils/image.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/json.py` & `python-suanpan-0.19.0/suanpan/utils/json.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/npy.py` & `python-suanpan-0.19.0/suanpan/utils/npy.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/pbar.py` & `python-suanpan-0.19.0/suanpan/utils/pbar.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/pickle.py` & `python-suanpan-0.19.0/suanpan/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/port.py` & `python-suanpan-0.19.0/suanpan/utils/port.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/term/__init__.py` & `python-suanpan-0.19.0/suanpan/utils/term/__init__.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/term/graph.py` & `python-suanpan-0.19.0/suanpan/utils/term/graph.py`

 * *Files identical despite different names*

### Comparing `python-suanpan-0.18.9/suanpan/utils/text.py` & `python-suanpan-0.19.0/suanpan/utils/text.py`

 * *Files identical despite different names*


# Comparing `tmp/covfee-0.0.8.tar.gz` & `tmp/covfee-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covfee-0.0.8.tar", last modified: Mon Dec  6 23:17:56 2021, max compression
+gzip compressed data, was "covfee-0.0.9.tar", last modified: Mon Dec  6 23:21:28 2021, max compression
```

## Comparing `covfee-0.0.8.tar` & `covfee-0.0.9.tar`

### file list

```diff
@@ -1,77 +1,82 @@
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:56.221640 covfee-0.0.8/
--rw-r--r--   0 jose      (1000) jose      (1000)     1068 2021-12-06 23:09:57.000000 covfee-0.0.8/LICENSE
--rw-r--r--   0 jose      (1000) jose      (1000)      202 2021-12-06 23:16:37.000000 covfee-0.0.8/MANIFEST.in
--rw-r--r--   0 jose      (1000) jose      (1000)     1469 2021-12-06 23:17:56.220132 covfee-0.0.8/PKG-INFO
--rwxrwxrwx   0 jose      (1000) jose      (1000)     1185 2021-12-05 20:07:12.000000 covfee-0.0.8/README.md
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:55.471134 covfee-0.0.8/covfee/
--rw-r--r--   0 jose      (1000) jose      (1000)     2440 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/__init__.py
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:55.555636 covfee-0.0.8/covfee/cli/
--rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/cli/__init__.py
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:55.600631 covfee-0.0.8/covfee/cli/commands/
--rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/cli/commands/__init__.py
--rw-r--r--   0 jose      (1000) jose      (1000)     1097 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/cli/commands/dev.py
--rw-r--r--   0 jose      (1000) jose      (1000)     6462 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/cli/commands/launch.py
--rw-r--r--   0 jose      (1000) jose      (1000)      665 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/cli/utils.py
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:55.375138 covfee-0.0.8/covfee/client/
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:55.682632 covfee-0.0.8/covfee/client/bundles/
--rw-r--r--   0 jose      (1000) jose      (1000)  1371074 2021-12-06 18:38:37.000000 covfee-0.0.8/covfee/client/bundles/admin.js
--rw-r--r--   0 jose      (1000) jose      (1000)     1160 2021-12-06 18:38:37.000000 covfee-0.0.8/covfee/client/bundles/admin.js.LICENSE.txt
--rw-r--r--   0 jose      (1000) jose      (1000)  1999983 2021-12-06 18:38:37.000000 covfee-0.0.8/covfee/client/bundles/main.js
--rw-r--r--   0 jose      (1000) jose      (1000)     4475 2021-12-06 18:38:37.000000 covfee-0.0.8/covfee/client/bundles/main.js.LICENSE.txt
--rw-r--r--   0 jose      (1000) jose      (1000)     7659 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/covfee_folder.py
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:55.733155 covfee-0.0.8/covfee/server/
--rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/__init__.py
--rw-r--r--   0 jose      (1000) jose      (1000)     1698 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/config.py
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:55.819133 covfee-0.0.8/covfee/server/orm/
--rw-r--r--   0 jose      (1000) jose      (1000)     3016 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/orm/__init__.py
--rw-r--r--   0 jose      (1000) jose      (1000)      129 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/orm/db.py
--rw-r--r--   0 jose      (1000) jose      (1000)    10723 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/orm/hit.py
--rw-r--r--   0 jose      (1000) jose      (1000)     3274 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/orm/project.py
--rw-r--r--   0 jose      (1000) jose      (1000)    13355 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/orm/task.py
--rw-r--r--   0 jose      (1000) jose      (1000)     1261 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/orm/user.py
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:55.864641 covfee-0.0.8/covfee/server/rest_api/
--rw-r--r--   0 jose      (1000) jose      (1000)       40 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/rest_api/__init__.py
--rw-r--r--   0 jose      (1000) jose      (1000)    11665 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/rest_api/api.py
--rw-r--r--   0 jose      (1000) jose      (1000)     5762 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/rest_api/auth.py
--rw-r--r--   0 jose      (1000) jose      (1000)       95 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/rtstore.py
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:55.908132 covfee-0.0.8/covfee/server/socketio/
--rw-r--r--   0 jose      (1000) jose      (1000)       30 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/socketio/__init__.py
--rw-r--r--   0 jose      (1000) jose      (1000)     2307 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/socketio/redux_store.py
--rw-r--r--   0 jose      (1000) jose      (1000)     2420 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/socketio/socketio.py
--rw-r--r--   0 jose      (1000) jose      (1000)     2112 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/start.py
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:56.000586 covfee-0.0.8/covfee/server/tasks/
--rw-r--r--   0 jose      (1000) jose      (1000)       87 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/tasks/__init__.py
--rw-r--r--   0 jose      (1000) jose      (1000)     3451 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/tasks/base.py
--rw-r--r--   0 jose      (1000) jose      (1000)      328 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/tasks/continous_keypoint.py
--rw-r--r--   0 jose      (1000) jose      (1000)      204 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/tasks/continuous_1d.py
--rw-r--r--   0 jose      (1000) jose      (1000)      201 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/tasks/video_recall.py
--rw-r--r--   0 jose      (1000) jose      (1000)     1961 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/tasks/videocall.py
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:56.073625 covfee-0.0.8/covfee/server/templates/
--rw-r--r--   0 jose      (1000) jose      (1000)      243 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/templates/404.html
--rw-r--r--   0 jose      (1000) jose      (1000)     2190 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/templates/admin.html
--rw-r--r--   0 jose      (1000) jose      (1000)     2177 2021-12-06 23:09:57.000000 covfee-0.0.8/covfee/server/templates/app.html
--rw-r--r--   0 jose      (1000) jose      (1000)      462 2021-12-06 23:09:58.000000 covfee-0.0.8/covfee/server/templates/externals.html
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:56.105616 covfee-0.0.8/covfee/server/utils/
--rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:09:58.000000 covfee-0.0.8/covfee/server/utils/__init__.py
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:56.153132 covfee-0.0.8/covfee/server/utils/agora/
--rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:09:58.000000 covfee-0.0.8/covfee/server/utils/agora/__init__.py
--rw-r--r--   0 jose      (1000) jose      (1000)     4564 2021-12-06 23:09:58.000000 covfee-0.0.8/covfee/server/utils/agora/access_token.py
--rw-r--r--   0 jose      (1000) jose      (1000)     3046 2021-12-06 23:09:58.000000 covfee-0.0.8/covfee/server/utils/agora/rtc_token_builder.py
--rw-r--r--   0 jose      (1000) jose      (1000)      775 2021-12-06 23:09:58.000000 covfee-0.0.8/covfee/server/utils/packer.py
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:56.167638 covfee-0.0.8/covfee/shared/
--rw-r--r--   0 jose      (1000) jose      (1000)    83704 2021-12-06 23:03:05.000000 covfee-0.0.8/covfee/shared/schemata.json
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:56.207634 covfee-0.0.8/covfee/shared/validator/
--rw-r--r--   0 jose      (1000) jose      (1000)       27 2021-12-06 23:09:58.000000 covfee-0.0.8/covfee/shared/validator/index.js
--rw-r--r--   0 jose      (1000) jose      (1000)     1393 2021-12-06 23:09:58.000000 covfee-0.0.8/covfee/shared/validator/validator.js
--rw-r--r--   0 jose      (1000) jose      (1000)     1021 2021-12-06 23:09:58.000000 covfee-0.0.8/covfee/shared/validator/validator_service.js
-drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:17:55.533635 covfee-0.0.8/covfee.egg-info/
--rw-r--r--   0 jose      (1000) jose      (1000)     1469 2021-12-06 23:17:55.000000 covfee-0.0.8/covfee.egg-info/PKG-INFO
--rw-r--r--   0 jose      (1000) jose      (1000)     1727 2021-12-06 23:17:55.000000 covfee-0.0.8/covfee.egg-info/SOURCES.txt
--rw-r--r--   0 jose      (1000) jose      (1000)        1 2021-12-06 23:17:55.000000 covfee-0.0.8/covfee.egg-info/dependency_links.txt
--rw-r--r--   0 jose      (1000) jose      (1000)      118 2021-12-06 23:17:55.000000 covfee-0.0.8/covfee.egg-info/entry_points.txt
--rw-r--r--   0 jose      (1000) jose      (1000)        1 2021-12-06 23:17:55.000000 covfee-0.0.8/covfee.egg-info/not-zip-safe
--rw-r--r--   0 jose      (1000) jose      (1000)      275 2021-12-06 23:17:55.000000 covfee-0.0.8/covfee.egg-info/requires.txt
--rw-r--r--   0 jose      (1000) jose      (1000)        7 2021-12-06 23:17:55.000000 covfee-0.0.8/covfee.egg-info/top_level.txt
--rw-r--r--   0 jose      (1000) jose      (1000)      103 2021-12-06 23:09:58.000000 covfee-0.0.8/pyproject.toml
--rw-r--r--   0 jose      (1000) jose      (1000)       38 2021-12-06 23:17:56.222133 covfee-0.0.8/setup.cfg
--rw-r--r--   0 jose      (1000) jose      (1000)     1259 2021-12-06 23:17:19.000000 covfee-0.0.8/setup.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:29.002313 covfee-0.0.9/
+-rw-r--r--   0 jose      (1000) jose      (1000)     1068 2021-12-06 23:09:57.000000 covfee-0.0.9/LICENSE
+-rw-r--r--   0 jose      (1000) jose      (1000)      202 2021-12-06 23:16:37.000000 covfee-0.0.9/MANIFEST.in
+-rw-r--r--   0 jose      (1000) jose      (1000)     1469 2021-12-06 23:21:29.000312 covfee-0.0.9/PKG-INFO
+-rwxrwxrwx   0 jose      (1000) jose      (1000)     1185 2021-12-05 20:07:12.000000 covfee-0.0.9/README.md
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.223812 covfee-0.0.9/covfee/
+-rw-r--r--   0 jose      (1000) jose      (1000)     2440 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/__init__.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.307312 covfee-0.0.9/covfee/cli/
+-rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/cli/__init__.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.347312 covfee-0.0.9/covfee/cli/commands/
+-rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/cli/commands/__init__.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     1097 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/cli/commands/dev.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     6462 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/cli/commands/launch.py
+-rw-r--r--   0 jose      (1000) jose      (1000)      665 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/cli/utils.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.139815 covfee-0.0.9/covfee/client/
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.428813 covfee-0.0.9/covfee/client/bundles/
+-rw-r--r--   0 jose      (1000) jose      (1000)  1371074 2021-12-06 18:38:37.000000 covfee-0.0.9/covfee/client/bundles/admin.js
+-rw-r--r--   0 jose      (1000) jose      (1000)     1160 2021-12-06 18:38:37.000000 covfee-0.0.9/covfee/client/bundles/admin.js.LICENSE.txt
+-rw-r--r--   0 jose      (1000) jose      (1000)  1999983 2021-12-06 18:38:37.000000 covfee-0.0.9/covfee/client/bundles/main.js
+-rw-r--r--   0 jose      (1000) jose      (1000)     4475 2021-12-06 18:38:37.000000 covfee-0.0.9/covfee/client/bundles/main.js.LICENSE.txt
+-rw-r--r--   0 jose      (1000) jose      (1000)     7659 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/covfee_folder.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.479312 covfee-0.0.9/covfee/server/
+-rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/__init__.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     1698 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/config.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.568814 covfee-0.0.9/covfee/server/orm/
+-rw-r--r--   0 jose      (1000) jose      (1000)     3016 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/orm/__init__.py
+-rw-r--r--   0 jose      (1000) jose      (1000)      129 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/orm/db.py
+-rw-r--r--   0 jose      (1000) jose      (1000)    10723 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/orm/hit.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     3274 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/orm/project.py
+-rw-r--r--   0 jose      (1000) jose      (1000)    13355 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/orm/task.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     1261 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/orm/user.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.613312 covfee-0.0.9/covfee/server/rest_api/
+-rw-r--r--   0 jose      (1000) jose      (1000)       40 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/rest_api/__init__.py
+-rw-r--r--   0 jose      (1000) jose      (1000)    11665 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/rest_api/api.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     5762 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/rest_api/auth.py
+-rw-r--r--   0 jose      (1000) jose      (1000)       95 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/rtstore.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.658812 covfee-0.0.9/covfee/server/socketio/
+-rw-r--r--   0 jose      (1000) jose      (1000)       30 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/socketio/__init__.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     2307 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/socketio/redux_store.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     2420 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/socketio/socketio.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     2112 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/start.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.748313 covfee-0.0.9/covfee/server/tasks/
+-rw-r--r--   0 jose      (1000) jose      (1000)       87 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/tasks/__init__.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     3451 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/tasks/base.py
+-rw-r--r--   0 jose      (1000) jose      (1000)      328 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/tasks/continous_keypoint.py
+-rw-r--r--   0 jose      (1000) jose      (1000)      204 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/tasks/continuous_1d.py
+-rw-r--r--   0 jose      (1000) jose      (1000)      201 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/tasks/video_recall.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     1961 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/tasks/videocall.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.806812 covfee-0.0.9/covfee/server/templates/
+-rw-r--r--   0 jose      (1000) jose      (1000)      243 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/templates/404.html
+-rw-r--r--   0 jose      (1000) jose      (1000)     2190 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/templates/admin.html
+-rw-r--r--   0 jose      (1000) jose      (1000)     2177 2021-12-06 23:09:57.000000 covfee-0.0.9/covfee/server/templates/app.html
+-rw-r--r--   0 jose      (1000) jose      (1000)      462 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/server/templates/externals.html
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.834313 covfee-0.0.9/covfee/server/utils/
+-rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/server/utils/__init__.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.884311 covfee-0.0.9/covfee/server/utils/agora/
+-rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/server/utils/agora/__init__.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     4564 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/server/utils/agora/access_token.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     3046 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/server/utils/agora/rtc_token_builder.py
+-rw-r--r--   0 jose      (1000) jose      (1000)      775 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/server/utils/packer.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.917313 covfee-0.0.9/covfee/shared/
+-rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:06.000000 covfee-0.0.9/covfee/shared/__init__.py
+-rw-r--r--   0 jose      (1000) jose      (1000)    83704 2021-12-06 23:03:05.000000 covfee-0.0.9/covfee/shared/schemata.json
+-rw-r--r--   0 jose      (1000) jose      (1000)     5894 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/shared/schemata.py
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.989312 covfee-0.0.9/covfee/shared/validator/
+-rw-r--r--   0 jose      (1000) jose      (1000)        0 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/shared/validator/__init__.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     2095 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/shared/validator/ajv_validator.py
+-rw-r--r--   0 jose      (1000) jose      (1000)       27 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/shared/validator/index.js
+-rw-r--r--   0 jose      (1000) jose      (1000)     3208 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/shared/validator/validation_errors.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     1393 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/shared/validator/validator.js
+-rw-r--r--   0 jose      (1000) jose      (1000)     1021 2021-12-06 23:09:58.000000 covfee-0.0.9/covfee/shared/validator/validator_service.js
+drwxr-xr-x   0 jose      (1000) jose      (1000)        0 2021-12-06 23:21:28.285313 covfee-0.0.9/covfee.egg-info/
+-rw-r--r--   0 jose      (1000) jose      (1000)     1469 2021-12-06 23:21:27.000000 covfee-0.0.9/covfee.egg-info/PKG-INFO
+-rw-r--r--   0 jose      (1000) jose      (1000)     1901 2021-12-06 23:21:28.000000 covfee-0.0.9/covfee.egg-info/SOURCES.txt
+-rw-r--r--   0 jose      (1000) jose      (1000)        1 2021-12-06 23:21:27.000000 covfee-0.0.9/covfee.egg-info/dependency_links.txt
+-rw-r--r--   0 jose      (1000) jose      (1000)      118 2021-12-06 23:21:27.000000 covfee-0.0.9/covfee.egg-info/entry_points.txt
+-rw-r--r--   0 jose      (1000) jose      (1000)        1 2021-12-06 23:21:27.000000 covfee-0.0.9/covfee.egg-info/not-zip-safe
+-rw-r--r--   0 jose      (1000) jose      (1000)      275 2021-12-06 23:21:27.000000 covfee-0.0.9/covfee.egg-info/requires.txt
+-rw-r--r--   0 jose      (1000) jose      (1000)        7 2021-12-06 23:21:27.000000 covfee-0.0.9/covfee.egg-info/top_level.txt
+-rw-r--r--   0 jose      (1000) jose      (1000)      103 2021-12-06 23:09:58.000000 covfee-0.0.9/pyproject.toml
+-rw-r--r--   0 jose      (1000) jose      (1000)       38 2021-12-06 23:21:29.002815 covfee-0.0.9/setup.cfg
+-rw-r--r--   0 jose      (1000) jose      (1000)     1259 2021-12-06 23:21:26.000000 covfee-0.0.9/setup.py
```

### Comparing `covfee-0.0.8/LICENSE` & `covfee-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/PKG-INFO` & `covfee-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covfee
-Version: 0.0.8
+Version: 0.0.9
 Summary: Continuous video feedback tool
 Home-page: UNKNOWN
 Author: Jose Vargas
 Author-email: josedvq@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `covfee-0.0.8/README.md` & `covfee-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/__init__.py` & `covfee-0.0.9/covfee/__init__.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/cli/commands/dev.py` & `covfee-0.0.9/covfee/cli/commands/dev.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/cli/commands/launch.py` & `covfee-0.0.9/covfee/cli/commands/launch.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/cli/utils.py` & `covfee-0.0.9/covfee/cli/utils.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/client/bundles/admin.js` & `covfee-0.0.9/covfee/client/bundles/admin.js`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/client/bundles/admin.js.LICENSE.txt` & `covfee-0.0.9/covfee/client/bundles/admin.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/client/bundles/main.js` & `covfee-0.0.9/covfee/client/bundles/main.js`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/client/bundles/main.js.LICENSE.txt` & `covfee-0.0.9/covfee/client/bundles/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/covfee_folder.py` & `covfee-0.0.9/covfee/covfee_folder.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/config.py` & `covfee-0.0.9/covfee/server/config.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/orm/__init__.py` & `covfee-0.0.9/covfee/server/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/orm/hit.py` & `covfee-0.0.9/covfee/server/orm/hit.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/orm/project.py` & `covfee-0.0.9/covfee/server/orm/project.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/orm/task.py` & `covfee-0.0.9/covfee/server/orm/task.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/orm/user.py` & `covfee-0.0.9/covfee/server/orm/user.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/rest_api/api.py` & `covfee-0.0.9/covfee/server/rest_api/api.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/rest_api/auth.py` & `covfee-0.0.9/covfee/server/rest_api/auth.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/socketio/redux_store.py` & `covfee-0.0.9/covfee/server/socketio/redux_store.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/socketio/socketio.py` & `covfee-0.0.9/covfee/server/socketio/socketio.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/start.py` & `covfee-0.0.9/covfee/server/start.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/tasks/base.py` & `covfee-0.0.9/covfee/server/tasks/base.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/tasks/videocall.py` & `covfee-0.0.9/covfee/server/tasks/videocall.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/templates/admin.html` & `covfee-0.0.9/covfee/server/templates/admin.html`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/templates/app.html` & `covfee-0.0.9/covfee/server/templates/app.html`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/utils/agora/access_token.py` & `covfee-0.0.9/covfee/server/utils/agora/access_token.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/utils/agora/rtc_token_builder.py` & `covfee-0.0.9/covfee/server/utils/agora/rtc_token_builder.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/server/utils/packer.py` & `covfee-0.0.9/covfee/server/utils/packer.py`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/shared/schemata.json` & `covfee-0.0.9/covfee/shared/schemata.json`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/shared/validator/validator.js` & `covfee-0.0.9/covfee/shared/validator/validator.js`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee/shared/validator/validator_service.js` & `covfee-0.0.9/covfee/shared/validator/validator_service.js`

 * *Files identical despite different names*

### Comparing `covfee-0.0.8/covfee.egg-info/PKG-INFO` & `covfee-0.0.9/covfee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covfee
-Version: 0.0.8
+Version: 0.0.9
 Summary: Continuous video feedback tool
 Home-page: UNKNOWN
 Author: Jose Vargas
 Author-email: josedvq@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `covfee-0.0.8/covfee.egg-info/SOURCES.txt` & `covfee-0.0.9/covfee.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -48,11 +48,16 @@
 covfee/server/templates/app.html
 covfee/server/templates/externals.html
 covfee/server/utils/__init__.py
 covfee/server/utils/packer.py
 covfee/server/utils/agora/__init__.py
 covfee/server/utils/agora/access_token.py
 covfee/server/utils/agora/rtc_token_builder.py
+covfee/shared/__init__.py
 covfee/shared/schemata.json
+covfee/shared/schemata.py
+covfee/shared/validator/__init__.py
+covfee/shared/validator/ajv_validator.py
 covfee/shared/validator/index.js
+covfee/shared/validator/validation_errors.py
 covfee/shared/validator/validator.js
 covfee/shared/validator/validator_service.js
```

### Comparing `covfee-0.0.8/setup.py` & `covfee-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='covfee',
-    version='0.0.8',
+    version='0.0.9',
     author="Jose Vargas",
     author_email="josedvq@gmail.com",
     description="Continuous video feedback tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```


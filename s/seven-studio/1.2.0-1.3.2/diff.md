# Comparing `tmp/seven_studio-1.2.0.tar.gz` & `tmp/seven_studio-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seven_studio-1.2.0.tar", last modified: Mon Apr 10 07:25:52 2023, max compression
+gzip compressed data, was "dist/seven_studio-1.3.2.tar", last modified: Thu Apr 27 11:20:01 2023, max compression
```

## Comparing `seven_studio-1.2.0.tar` & `seven_studio-1.3.2.tar`

### file list

```diff
@@ -1,83 +1,82 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.657166 seven_studio-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     2868 2023-04-10 07:25:52.657166 seven_studio-1.2.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1449 2023-04-10 07:25:27.000000 seven_studio-1.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 07:25:52.657166 seven_studio-1.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1265 2023-04-10 07:25:27.000000 seven_studio-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.629154 seven_studio-1.2.0/seven_studio/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.632155 seven_studio-1.2.0/seven_studio/handlers/
--rwxrwxrwx   0 root         (0) root         (0)      132 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1626 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/monitor.py
--rwxrwxrwx   0 root         (0) root         (0)    24916 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/studio_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.635156 seven_studio-1.2.0/seven_studio/handlers/system/
--rwxrwxrwx   0 root         (0) root         (0)      224 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8880 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/core.py
--rwxrwxrwx   0 root         (0) root         (0)    22072 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/file.py
--rwxrwxrwx   0 root         (0) root         (0)    17591 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/menu.py
--rwxrwxrwx   0 root         (0) root         (0)    31748 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/power.py
--rwxrwxrwx   0 root         (0) root         (0)     6606 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/product.py
--rwxrwxrwx   0 root         (0) root         (0)     2582 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/handlers/system/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.636157 seven_studio-1.2.0/seven_studio/libs/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.639158 seven_studio-1.2.0/seven_studio/libs/file/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8612 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/bos.py
--rwxrwxrwx   0 root         (0) root         (0)     8613 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/cos.py
--rwxrwxrwx   0 root         (0) root         (0)    19074 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/ks3.py
--rwxrwxrwx   0 root         (0) root         (0)     9588 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/oss2.py
--rwxrwxrwx   0 root         (0) root         (0)     8593 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/s3.py
--rwxrwxrwx   0 root         (0) root         (0)    14037 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/file/upload.py
--rwxrwxrwx   0 root         (0) root         (0)     6306 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/libs/geetest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.641159 seven_studio-1.2.0/seven_studio/models/
--rwxrwxrwx   0 root         (0) root         (0)      180 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.641159 seven_studio-1.2.0/seven_studio/models/db_models/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.645161 seven_studio-1.2.0/seven_studio/models/db_models/file/
--rwxrwxrwx   0 root         (0) root         (0)      308 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1492 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_history_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1131 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_resource_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2433 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_restrict_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1578 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_restrict_pic_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1451 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_storage_path_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1011 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/file/file_water_image_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.645161 seven_studio-1.2.0/seven_studio/models/db_models/log/
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/log/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1298 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/log/log_action_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.647162 seven_studio-1.2.0/seven_studio/models/db_models/menu/
--rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/menu/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1583 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_cote_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2174 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)    19404 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_info_model_ex.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.649163 seven_studio-1.2.0/seven_studio/models/db_models/product/
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/product/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1689 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/product/product_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)      983 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/product/product_user_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.651164 seven_studio-1.2.0/seven_studio/models/db_models/role/
--rwxrwxrwx   0 root         (0) root         (0)       87 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/role/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1148 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/role/role_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1014 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/role/role_power_model.py
--rwxrwxrwx   0 root         (0) root         (0)      952 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/role/role_power_model_ex.py
--rwxrwxrwx   0 root         (0) root         (0)     1036 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/role/role_user_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.652164 seven_studio-1.2.0/seven_studio/models/db_models/settings/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/settings/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1152 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/settings/settings_base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.654165 seven_studio-1.2.0/seven_studio/models/db_models/user/
--rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/user/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2025 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/user/user_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1125 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/user/user_info_model_ex.py
--rwxrwxrwx   0 root         (0) root         (0)     1035 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/db_models/user/user_login_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/dto_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2419 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/enum.py
--rwxrwxrwx   0 root         (0) root         (0)    37518 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/power_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2689 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/models/seven_model.py
--rwxrwxrwx   0 root         (0) root         (0)     4391 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/route.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.656166 seven_studio-1.2.0/seven_studio/utils/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1959 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/utils/dict.py
--rwxrwxrwx   0 root         (0) root         (0)      637 2023-04-10 07:25:27.000000 seven_studio-1.2.0/seven_studio/utils/random.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:25:52.631154 seven_studio-1.2.0/seven_studio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2868 2023-04-10 07:25:52.000000 seven_studio-1.2.0/seven_studio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2669 2023-04-10 07:25:52.000000 seven_studio-1.2.0/seven_studio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 07:25:52.000000 seven_studio-1.2.0/seven_studio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-10 07:25:52.000000 seven_studio-1.2.0/seven_studio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 07:25:52.000000 seven_studio-1.2.0/seven_studio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.711851 seven_studio-1.3.2/
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-04-27 11:20:01.710851 seven_studio-1.3.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1494 2023-04-27 11:19:10.000000 seven_studio-1.3.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 11:20:01.711851 seven_studio-1.3.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1265 2023-04-27 11:19:10.000000 seven_studio-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.645852 seven_studio-1.3.2/seven_studio/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.652852 seven_studio-1.3.2/seven_studio/handlers/
+-rwxrwxrwx   0 root         (0) root         (0)      132 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    25307 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/studio_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.657852 seven_studio-1.3.2/seven_studio/handlers/system/
+-rwxrwxrwx   0 root         (0) root         (0)      224 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9186 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    22072 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/file.py
+-rwxrwxrwx   0 root         (0) root         (0)    17591 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/menu.py
+-rwxrwxrwx   0 root         (0) root         (0)    31748 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/power.py
+-rwxrwxrwx   0 root         (0) root         (0)     6606 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/product.py
+-rwxrwxrwx   0 root         (0) root         (0)     2582 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.659852 seven_studio-1.3.2/seven_studio/libs/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.670852 seven_studio-1.3.2/seven_studio/libs/file/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8612 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/bos.py
+-rwxrwxrwx   0 root         (0) root         (0)     8613 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/cos.py
+-rwxrwxrwx   0 root         (0) root         (0)    19074 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/ks3.py
+-rwxrwxrwx   0 root         (0) root         (0)     9588 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/oss2.py
+-rwxrwxrwx   0 root         (0) root         (0)     8593 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/s3.py
+-rwxrwxrwx   0 root         (0) root         (0)    14037 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/upload.py
+-rwxrwxrwx   0 root         (0) root         (0)     6306 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/geetest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.679852 seven_studio-1.3.2/seven_studio/models/
+-rwxrwxrwx   0 root         (0) root         (0)      180 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.679852 seven_studio-1.3.2/seven_studio/models/db_models/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.686852 seven_studio-1.3.2/seven_studio/models/db_models/file/
+-rwxrwxrwx   0 root         (0) root         (0)      308 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1492 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_history_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1131 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_resource_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2433 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_restrict_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1578 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_restrict_pic_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1451 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_storage_path_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1011 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_water_image_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.690852 seven_studio-1.3.2/seven_studio/models/db_models/log/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/log/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1298 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/log/log_action_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.692852 seven_studio-1.3.2/seven_studio/models/db_models/menu/
+-rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/menu/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1583 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_cote_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2174 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    19404 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_info_model_ex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.695851 seven_studio-1.3.2/seven_studio/models/db_models/product/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/product/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1689 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/product/product_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)      983 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/product/product_user_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.700852 seven_studio-1.3.2/seven_studio/models/db_models/role/
+-rwxrwxrwx   0 root         (0) root         (0)       87 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/role/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1148 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/role/role_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1014 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/role/role_power_model.py
+-rwxrwxrwx   0 root         (0) root         (0)      952 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/role/role_power_model_ex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1036 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/role/role_user_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.704851 seven_studio-1.3.2/seven_studio/models/db_models/settings/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/settings/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1152 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/settings/settings_base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.706851 seven_studio-1.3.2/seven_studio/models/db_models/user/
+-rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/user/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2025 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/user/user_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1125 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/user/user_info_model_ex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1035 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/user/user_login_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/dto_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2419 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/enum.py
+-rwxrwxrwx   0 root         (0) root         (0)    37518 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/power_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2689 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/seven_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     4391 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/route.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.709851 seven_studio-1.3.2/seven_studio/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1959 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/utils/dict.py
+-rwxrwxrwx   0 root         (0) root         (0)      637 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/utils/random.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.649852 seven_studio-1.3.2/seven_studio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-04-27 11:20:01.000000 seven_studio-1.3.2/seven_studio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-04-27 11:20:01.000000 seven_studio-1.3.2/seven_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:20:01.000000 seven_studio-1.3.2/seven_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-27 11:20:01.000000 seven_studio-1.3.2/seven_studio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 11:20:01.000000 seven_studio-1.3.2/seven_studio.egg-info/top_level.txt
```

### Comparing `seven_studio-1.2.0/PKG-INFO` & `seven_studio-1.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven_studio
-Version: 1.2.0
+Version: 1.3.2
 Summary: seven studio
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_studio
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: 
         
@@ -15,14 +15,17 @@
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         # seven_studio
         
         ## 天志互联Python公共基础后台管理平台
         
+        ### 1.3.2 更新内容
+        * 登录问题修改
+        
         ### 1.2.0 更新内容
         * GetUserInfoHandler增加字段返回
         
         ### 1.1.9 更新内容
         * 基础配置更新
         * 用户登录过期处理
```

### Comparing `seven_studio-1.2.0/README.md` & `seven_studio-1.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
  * @LastEditors: ChenXiaolei
  * @Description: 
 -->
 # seven_studio
 
 ## 天志互联Python公共基础后台管理平台
 
+### 1.3.2 更新内容
+* 登录问题修改
+
 ### 1.2.0 更新内容
 * GetUserInfoHandler增加字段返回
 
 ### 1.1.9 更新内容
 * 基础配置更新
 * 用户登录过期处理
```

### Comparing `seven_studio-1.2.0/setup.py` & `seven_studio-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="seven_studio",
-    version="1.2.0",
+    version="1.3.2",
     author="seven",
     author_email="tech@gao7.com",
     description="seven studio",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="http://gitlab.tdtech.gao7.com/python/seven_studio",
```

### Comparing `seven_studio-1.2.0/seven_studio/handlers/studio_base.py` & `seven_studio-1.3.2/seven_studio/handlers/studio_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: ChenXiaolei
 :Date: 2020-03-24 10:42:34
-:LastEditTime: 2023-02-07 09:17:25
+:LastEditTime: 2023-04-27 18:19:33
 :LastEditors: HuangJingCan
 :Description: StudioBaseHandler
 """
 
 from seven_framework.web_tornado.base_handler.base_cookie_handler import *
 from seven_framework.redis import *
 
@@ -412,38 +412,22 @@
         if map_dict:
             field_list = s_model.get_field_list()
             for filed in field_list:
                 if filed in map_dict:
                     setattr(s_model, filed, map_dict[filed])
         return s_model
 
-    def login_filter(self, is_need_login, optional_params):
-        # sourcery skip: class-extract-method
+    def check_login_user(self, user_id, user_token, is_need_login=True):
         """
-        :description: 登录过滤器
-        :param is_need_login: 是否需要登录（true需要false不需要）
-        :param optional_params: 其他参数
-        :return: InvokeResult
+        :description: 登录用户检查
+        :param user_id：用户id
+        :param user_token：用户user_token
+        :return: 
         """
         invoke_result = InvokeResult()
-        base_manage_context_key = config.get_value("base_manage_context_key")
-        # 获取头部信息
-        header_token = self.request_header_token()
-        user_id = header_token["UserID"] if header_token.__contains__("UserID") else ""
-        user_token = header_token["UserToken"] if header_token.__contains__("UserToken") else ""
-        user_id_md5 = header_token["UserIDMD5"] if header_token.__contains__("UserIDMD5") else ""
-        if user_id.strip() == "" or user_token.strip() == "" or user_id_md5.strip() == "":
-            invoke_result.ResultCode = "error"
-            invoke_result.ResultMessage = "操作失败，用户未登录"
-            return invoke_result
-        if is_need_login and CryptoHelper.md5_encrypt(user_id, config.get_value("login_encrypt_key")) != user_id_md5:
-            invoke_result.ResultCode = "error"
-            invoke_result.ResultMessage = "操作失败，用户未登录"
-            return invoke_result
-
         # 登陆日志判断，Redis还是MySQL
         if config.get_value("login_type") == "redis":
             redis_user_login = self.redis_init().hget(config.get_value("redis_provider_name_user_login"), user_id)
             user_login = json.loads(redis_user_login) if redis_user_login else {}
             if not user_login or TimeHelper.format_time_to_datetime(user_login["ExpireTime"]) < TimeHelper.get_now_datetime():
                 if not is_need_login:
                     return invoke_result
@@ -464,14 +448,17 @@
                 invoke_result.ResultCode = "login_expire"
                 invoke_result.ResultMessage = "用户已被锁，请联系管理员"
                 return invoke_result
 
             user_login["ExpireTime"] = TimeHelper.add_hours_by_format_time(hour=config.get_value("login_expire"))
             self.redis_init().hset(config.get_value("redis_provider_name_user_login"), user_id, self.json_dumps(user_login))
         else:
+            base_manage_context_key = config.get_value("base_manage_context_key")
+            manage_context_key = self.get_manage_context_key()
+
             user_login_model = UserLoginModel(base_manage_context_key)
             user_login = user_login_model.get_entity_by_id(user_id)
 
             if not user_login or TimeHelper.format_time_to_datetime(user_login.ExpireTime) < TimeHelper.get_now_datetime():
                 if not is_need_login:
                     return invoke_result
                 self.clear_user_cookie()
@@ -482,16 +469,14 @@
                 if not is_need_login:
                     return invoke_result
                 self.clear_user_cookie()
                 invoke_result.ResultCode = "login_expire"
                 invoke_result.ResultMessage = "用户在其他终端登录，请重新登录"
                 return invoke_result
 
-            manage_context_key = self.get_manage_context_key()
-
             curr_user_info = UserInfoModel(manage_context_key).get_entity_by_id(user_id)
             if not curr_user_info:
                 invoke_result.ResultCode = "login_expire"
                 invoke_result.ResultMessage = "用户已过期，请重新登录"
                 return invoke_result
             if curr_user_info.IsLock == 1:
                 invoke_result.ResultCode = "login_expire"
@@ -510,14 +495,41 @@
                     return invoke_result
 
             user_login.ExpireTime = TimeHelper.add_hours_by_format_time(hour=config.get_value("login_expire"))
             user_login_model.update_table(f"ExpireTime='{user_login.ExpireTime}'", "UserID=%s", user_login.UserID)
 
         return invoke_result
 
+    def login_filter(self, is_need_login, optional_params):
+        # sourcery skip: class-extract-method
+        """
+        :description: 登录过滤器
+        :param is_need_login: 是否需要登录（true需要false不需要）
+        :param optional_params: 其他参数
+        :return: InvokeResult
+        """
+        invoke_result = InvokeResult()
+        # 获取头部信息
+        header_token = self.request_header_token()
+        user_id = header_token["UserID"] if header_token.__contains__("UserID") else ""
+        user_token = header_token["UserToken"] if header_token.__contains__("UserToken") else ""
+        user_id_md5 = header_token["UserIDMD5"] if header_token.__contains__("UserIDMD5") else ""
+        if user_id.strip() == "" or user_token.strip() == "" or user_id_md5.strip() == "":
+            invoke_result.ResultCode = "error"
+            invoke_result.ResultMessage = "操作失败，用户未登录"
+            return invoke_result
+        if is_need_login and CryptoHelper.md5_encrypt(user_id, config.get_value("login_encrypt_key")) != user_id_md5:
+            invoke_result.ResultCode = "error"
+            invoke_result.ResultMessage = "操作失败，用户未登录"
+            return invoke_result
+
+        invoke_result = self.check_login_user(user_id, user_token, is_need_login)
+
+        return invoke_result
+
     def power_filter(self, is_check_power, optional_params):
         """
         :description: 权限过滤器
         :param is_check_power: 是否需要验证权限（true需要false不需要）
         :param optional_params: 其他参数
         :return: InvokeResult
         """
```

### Comparing `seven_studio-1.2.0/seven_studio/handlers/system/core.py` & `seven_studio-1.3.2/seven_studio/handlers/system/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: HuangJingCan
 :Date: 2020-03-24 19:48:05
-:LastEditTime: 2023-02-06 16:29:03
+:LastEditTime: 2023-04-27 18:13:33
 :LastEditors: HuangJingCan
 :Description: 
 """
 from seven_studio.handlers.studio_base import *
 from seven_studio.libs.geetest import *
 
 from seven_studio.models.db_models.user.user_info_model_ex import *
@@ -63,15 +63,22 @@
             if challenge == "" or validate == "" or seccode == "":
                 return self.response_common("CaptchaError", "对不起，请先校验验证码")
 
             result = self.check_code(challenge, validate, seccode)
             if not result:
                 return self.response_common("CaptchaError", "对不起，验证码验证失败")
 
-        return self.response_custom(self.login(account, password, True))
+        invoke_result = self.login(account, password, True)
+
+        if invoke_result.ResultCode == "0":
+            invoke_result_user = self.check_login_user(invoke_result.Data['UserID'], invoke_result.Data['UserToken'])
+            if invoke_result_user.ResultCode != "0":
+                invoke_result = invoke_result_user
+
+        return self.response_custom(invoke_result)
 
     def check_code(self, challenge="", validate="", seccode=""):
         """
         :description: 验证码校验
         :param challenge：极验证参数challenge
         :param validate：极验证参数validate
         :param seccode：极验证参数seccode
```

### Comparing `seven_studio-1.2.0/seven_studio/handlers/system/file.py` & `seven_studio-1.3.2/seven_studio/handlers/system/file.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/handlers/system/menu.py` & `seven_studio-1.3.2/seven_studio/handlers/system/menu.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/handlers/system/power.py` & `seven_studio-1.3.2/seven_studio/handlers/system/power.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/handlers/system/product.py` & `seven_studio-1.3.2/seven_studio/handlers/system/product.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/handlers/system/settings.py` & `seven_studio-1.3.2/seven_studio/handlers/system/settings.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/libs/file/bos.py` & `seven_studio-1.3.2/seven_studio/libs/file/bos.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/libs/file/cos.py` & `seven_studio-1.3.2/seven_studio/libs/file/cos.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/libs/file/ks3.py` & `seven_studio-1.3.2/seven_studio/libs/file/ks3.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/libs/file/oss2.py` & `seven_studio-1.3.2/seven_studio/libs/file/oss2.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/libs/file/s3.py` & `seven_studio-1.3.2/seven_studio/libs/file/s3.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/libs/file/upload.py` & `seven_studio-1.3.2/seven_studio/libs/file/upload.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/libs/geetest.py` & `seven_studio-1.3.2/seven_studio/libs/geetest.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/file/file_history_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/file/file_history_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/file/file_resource_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/file/file_resource_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/file/file_restrict_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/file/file_restrict_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/file/file_restrict_pic_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/file/file_restrict_pic_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/file/file_storage_path_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/file/file_storage_path_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/file/file_water_image_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/file/file_water_image_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/log/log_action_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/log/log_action_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_cote_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_cote_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_info_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/menu/menu_info_model_ex.py` & `seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_info_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/product/product_info_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/product/product_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/product/product_user_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/product/product_user_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/role/role_info_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/role/role_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/role/role_power_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/role/role_power_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/role/role_power_model_ex.py` & `seven_studio-1.3.2/seven_studio/models/db_models/role/role_power_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/role/role_user_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/role/role_user_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/settings/settings_base_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/settings/settings_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/user/user_info_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/user/user_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/user/user_info_model_ex.py` & `seven_studio-1.3.2/seven_studio/models/db_models/user/user_info_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/db_models/user/user_login_model.py` & `seven_studio-1.3.2/seven_studio/models/db_models/user/user_login_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/dto_model.py` & `seven_studio-1.3.2/seven_studio/models/dto_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/enum.py` & `seven_studio-1.3.2/seven_studio/models/enum.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/power_model.py` & `seven_studio-1.3.2/seven_studio/models/power_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/models/seven_model.py` & `seven_studio-1.3.2/seven_studio/models/seven_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/route.py` & `seven_studio-1.3.2/seven_studio/route.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/utils/dict.py` & `seven_studio-1.3.2/seven_studio/utils/dict.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio/utils/random.py` & `seven_studio-1.3.2/seven_studio/utils/random.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.2.0/seven_studio.egg-info/PKG-INFO` & `seven_studio-1.3.2/seven_studio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven-studio
-Version: 1.2.0
+Version: 1.3.2
 Summary: seven studio
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_studio
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: 
         
@@ -15,14 +15,17 @@
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         # seven_studio
         
         ## 天志互联Python公共基础后台管理平台
         
+        ### 1.3.2 更新内容
+        * 登录问题修改
+        
         ### 1.2.0 更新内容
         * GetUserInfoHandler增加字段返回
         
         ### 1.1.9 更新内容
         * 基础配置更新
         * 用户登录过期处理
```

### Comparing `seven_studio-1.2.0/seven_studio.egg-info/SOURCES.txt` & `seven_studio-1.3.2/seven_studio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 seven_studio/route.py
 seven_studio.egg-info/PKG-INFO
 seven_studio.egg-info/SOURCES.txt
 seven_studio.egg-info/dependency_links.txt
 seven_studio.egg-info/requires.txt
 seven_studio.egg-info/top_level.txt
 seven_studio/handlers/__init__.py
-seven_studio/handlers/monitor.py
 seven_studio/handlers/studio_base.py
 seven_studio/handlers/system/__init__.py
 seven_studio/handlers/system/core.py
 seven_studio/handlers/system/file.py
 seven_studio/handlers/system/menu.py
 seven_studio/handlers/system/power.py
 seven_studio/handlers/system/product.py
```


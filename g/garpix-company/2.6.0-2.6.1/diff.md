# Comparing `tmp/garpix_company-2.6.0.tar.gz` & `tmp/garpix_company-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_company-2.6.0.tar", last modified: Tue Feb 14 14:46:31 2023, max compression
+gzip compressed data, was "garpix_company-2.6.1.tar", last modified: Thu Apr 27 15:15:25 2023, max compression
```

## Comparing `garpix_company-2.6.0.tar` & `garpix_company-2.6.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.232354 garpix_company-2.6.0/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-02-14 14:46:31.000000 garpix_company-2.6.0/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3807 2023-02-14 14:46:31.232213 garpix_company-2.6.0/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.227996 garpix_company-2.6.0/garpix_company/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2252 2023-02-14 14:39:39.000000 garpix_company-2.6.0/garpix_company/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3237 2023-01-24 14:45:59.000000 garpix_company-2.6.0/garpix_company/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.229059 garpix_company-2.6.0/garpix_company/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      352 2023-01-30 05:54:06.000000 garpix_company-2.6.0/garpix_company/admin/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.6.0/garpix_company/admin/company_invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/helpers.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.229377 garpix_company-2.6.0/garpix_company/managers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/managers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/managers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/managers/invite.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.229491 garpix_company-2.6.0/garpix_company/migrations/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/migrations/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.229586 garpix_company-2.6.0/garpix_company/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.229776 garpix_company-2.6.0/garpix_company/mixins/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/mixins/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.6.0/garpix_company/mixins/views/company_mixin.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.230303 garpix_company-2.6.0/garpix_company/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      177 2022-12-09 15:26:30.000000 garpix_company-2.6.0/garpix_company/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5711 2023-02-10 15:45:53.000000 garpix_company-2.6.0/garpix_company/models/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4306 2023-02-14 14:37:52.000000 garpix_company-2.6.0/garpix_company/models/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3371 2023-02-10 15:45:53.000000 garpix_company-2.6.0/garpix_company/models/user_company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.6.0/garpix_company/models/user_role.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.230820 garpix_company-2.6.0/garpix_company/permissions/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.6.0/garpix_company/permissions/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      985 2023-02-10 15:45:53.000000 garpix_company-2.6.0/garpix_company/permissions/company_admin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      656 2023-02-02 07:34:38.000000 garpix_company-2.6.0/garpix_company/permissions/company_owner.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      441 2023-02-10 15:45:53.000000 garpix_company-2.6.0/garpix_company/permissions/company_user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      420 2022-12-09 14:51:29.000000 garpix_company-2.6.0/garpix_company/permissions/invite_receiver.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.231448 garpix_company-2.6.0/garpix_company/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.6.0/garpix_company/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3341 2023-02-10 15:45:53.000000 garpix_company-2.6.0/garpix_company/serializers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5420 2023-02-10 15:45:53.000000 garpix_company-2.6.0/garpix_company/serializers/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.6.0/garpix_company/serializers/role.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.6.0/garpix_company/serializers/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      801 2023-02-10 15:21:14.000000 garpix_company-2.6.0/garpix_company/serializers/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.231641 garpix_company-2.6.0/garpix_company/services/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.6.0/garpix_company/services/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      609 2023-01-30 05:54:06.000000 garpix_company-2.6.0/garpix_company/services/role_service.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.6.0/garpix_company/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-02-14 14:39:39.000000 garpix_company-2.6.0/garpix_company/setup.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.6.0/garpix_company/tests.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.6.0/garpix_company/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.232052 garpix_company-2.6.0/garpix_company/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.6.0/garpix_company/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5459 2023-02-10 15:45:53.000000 garpix_company-2.6.0/garpix_company/views/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2127 2023-02-06 10:05:38.000000 garpix_company-2.6.0/garpix_company/views/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3536 2023-02-06 08:24:58.000000 garpix_company-2.6.0/garpix_company/views/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-14 14:46:31.228698 garpix_company-2.6.0/garpix_company.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3807 2023-02-14 14:46:31.000000 garpix_company-2.6.0/garpix_company.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-02-14 14:46:31.000000 garpix_company-2.6.0/garpix_company.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-02-14 14:46:31.000000 garpix_company-2.6.0/garpix_company.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-02-14 14:46:31.000000 garpix_company-2.6.0/garpix_company.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-02-14 14:46:31.000000 garpix_company-2.6.0/garpix_company.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-02-14 14:46:31.000000 garpix_company-2.6.0/garpix_company.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-02-14 14:46:31.232390 garpix_company-2.6.0/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-02-14 14:46:31.000000 garpix_company-2.6.0/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.439727 garpix_company-2.6.1/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-04-27 15:15:25.000000 garpix_company-2.6.1/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3807 2023-04-27 15:15:25.439570 garpix_company-2.6.1/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.434204 garpix_company-2.6.1/garpix_company/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2301 2023-04-27 15:15:01.000000 garpix_company-2.6.1/garpix_company/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3237 2023-01-24 14:45:59.000000 garpix_company-2.6.1/garpix_company/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.435221 garpix_company-2.6.1/garpix_company/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      352 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/admin/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.6.1/garpix_company/admin/company_invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/helpers.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.435527 garpix_company-2.6.1/garpix_company/managers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/managers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/managers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/managers/invite.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.435643 garpix_company-2.6.1/garpix_company/migrations/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/migrations/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.435736 garpix_company-2.6.1/garpix_company/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.435953 garpix_company-2.6.1/garpix_company/mixins/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/mixins/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.6.1/garpix_company/mixins/views/company_mixin.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.436602 garpix_company-2.6.1/garpix_company/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      177 2022-12-09 15:26:30.000000 garpix_company-2.6.1/garpix_company/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5711 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/models/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4306 2023-02-14 14:37:52.000000 garpix_company-2.6.1/garpix_company/models/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3371 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/models/user_company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/models/user_role.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.437480 garpix_company-2.6.1/garpix_company/permissions/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/permissions/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      985 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/permissions/company_admin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      656 2023-02-02 07:34:38.000000 garpix_company-2.6.1/garpix_company/permissions/company_owner.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      441 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/permissions/company_user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      420 2022-12-09 14:51:29.000000 garpix_company-2.6.1/garpix_company/permissions/invite_receiver.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.438384 garpix_company-2.6.1/garpix_company/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2841 2023-04-27 15:14:15.000000 garpix_company-2.6.1/garpix_company/serializers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5570 2023-04-27 15:13:08.000000 garpix_company-2.6.1/garpix_company/serializers/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/serializers/role.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.6.1/garpix_company/serializers/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      801 2023-02-10 15:21:14.000000 garpix_company-2.6.1/garpix_company/serializers/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.438696 garpix_company-2.6.1/garpix_company/services/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/services/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      609 2023-01-30 05:54:06.000000 garpix_company-2.6.1/garpix_company/services/role_service.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.6.1/garpix_company/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-04-27 15:15:01.000000 garpix_company-2.6.1/garpix_company/setup.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.6.1/garpix_company/tests.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.439368 garpix_company-2.6.1/garpix_company/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.6.1/garpix_company/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5459 2023-02-10 15:45:53.000000 garpix_company-2.6.1/garpix_company/views/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2127 2023-02-06 10:05:38.000000 garpix_company-2.6.1/garpix_company/views/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3536 2023-02-06 08:24:58.000000 garpix_company-2.6.1/garpix_company/views/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-27 15:15:25.434874 garpix_company-2.6.1/garpix_company.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3807 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-04-27 15:15:25.000000 garpix_company-2.6.1/garpix_company.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-04-27 15:15:25.439777 garpix_company-2.6.1/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-04-27 15:15:25.000000 garpix_company-2.6.1/setup.py
```

### Comparing `garpix_company-2.6.0/PKG-INFO` & `garpix_company-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_company
-Version: 2.6.0
+Version: 2.6.1
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_company-2.6.0/garpix_company/CHANGELOG.md` & `garpix_company-2.6.1/garpix_company/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+### 2.6.1 (27.04.2023)
+
+- Invite user bug fixed
+
 ### 2.6.0 (14.02.2023)
 
 - Decline previous invites for the invite to same person
 
 ### 2.5.0 (10.02.2023)
 
 - `is_admin` field removed from `company` views
```

### Comparing `garpix_company-2.6.0/garpix_company/CONTRIBUTING.md` & `garpix_company-2.6.1/garpix_company/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/README.md` & `garpix_company-2.6.1/garpix_company/README.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/helpers.py` & `garpix_company-2.6.1/garpix_company/helpers.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/models/company.py` & `garpix_company-2.6.1/garpix_company/models/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/models/invite.py` & `garpix_company-2.6.1/garpix_company/models/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/models/user_company.py` & `garpix_company-2.6.1/garpix_company/models/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/models/user_role.py` & `garpix_company-2.6.1/garpix_company/models/user_role.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/permissions/company_admin.py` & `garpix_company-2.6.1/garpix_company/permissions/company_admin.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/permissions/company_owner.py` & `garpix_company-2.6.1/garpix_company/permissions/company_owner.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/serializers/company.py` & `garpix_company-2.6.1/garpix_company/serializers/company.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,54 +9,40 @@
 from garpix_company.models.user_role import get_company_role_model
 from garpix_company.services.role_service import UserCompanyRoleService
 
 Company = get_company_model()
 CompanyRole = get_company_role_model()
 
 
-class AdminCompanySerializerMixin(serializers.Serializer):
-    is_admin = serializers.SerializerMethodField(read_only=True)
-
-    def get_is_admin(self, obj):
-        company_role_service = UserCompanyRoleService()
-
-        request = self.context.get("request")
-        if request and hasattr(request, "user"):
-            user = request.user
-            if user.is_authenticated:
-                user_company = UserCompany.objects.filter(user=user, company=obj).first()
-                if user_company is not None:
-                    return user_company.role == company_role_service.get_admin_role()
-        return False
+class ExtraFieldsCompanySerializerMixin(serializers.Serializer):
 
     def get_field_names(self, declared_fields, info):
         expanded_fields = super().get_field_names(declared_fields, info)
 
         if getattr(self.Meta, 'extra_fields', None):
             return expanded_fields + self.Meta.extra_fields
         else:
             return expanded_fields
 
 
-class CompanySerializer(serializers.ModelSerializer):
+class CompanySerializer(ExtraFieldsCompanySerializerMixin, serializers.ModelSerializer):
 
     class Meta:
         model = Company
         exclude = ('participants',)
-        extra_fields = ['is_admin']
 
 
-class CreateCompanySerializer(serializers.ModelSerializer):
+class CreateCompanySerializer(ExtraFieldsCompanySerializerMixin, serializers.ModelSerializer):
 
     user_by = serializers.HiddenField(default=serializers.CurrentUserDefault())
 
     class Meta:
         model = Company
         exclude = ('participants',)
-        extra_fields = ['is_admin', 'user_by']
+        extra_fields = ['user_by']
         extra_kwargs = {
             'created_at': {'read_only': True},
             'updated_at': {'read_only': True}
         }
 
     def validate_user_by(self, value):
         Company = get_company_model()
@@ -80,15 +66,15 @@
             )
             obj.save()
             user_company = UserCompany(user=user, company=obj, role=company_role_service.get_owner_role())
             user_company.save()
         return obj
 
 
-class UpdateCompanySerializer(serializers.ModelSerializer):
+class UpdateCompanySerializer(ExtraFieldsCompanySerializerMixin, serializers.ModelSerializer):
     class Meta:
         model = Company
         fields = (
             'title', 'full_title', 'inn', 'ogrn', 'kpp', 'bank_title',
             'bic', 'schet', 'korschet', 'ur_address', 'fact_address'
         )
```

### Comparing `garpix_company-2.6.0/garpix_company/serializers/invite.py` & `garpix_company-2.6.1/garpix_company/serializers/invite.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,29 +24,31 @@
         extra_kwargs = {
             'role': {'required': True},
         }
 
     def validate_email(self, value):
         User = get_user_model()
         Company = get_company_model()
+        company_id = self.context.get("company_id")
         try:
             user = User.objects.get(email=value)
             if not Company.check_user_companies_limit(user):
                 raise ValidationError(_('У пользователя с указанным email превышен лимит количества компаний'))
-            if UserCompany.active_objects.filter(user=user).exists():
+            if UserCompany.active_objects.filter(user=user, company_id=company_id).exists():
                 raise ValidationError(_('Указанный пользователь уже является сотрудником компании'))
         except User.DoesNotExist:
             raise ValidationError(_('Пользователь с указанным email не зарегистрирован'))
         return value
 
     def validate_user(self, value):
         Company = get_company_model()
+        company_id = self.context.get("company_id")
         if not Company.check_user_companies_limit(value):
             raise ValidationError(_('У пользователя с указанным id превышен лимит количества компаний'))
-        if UserCompany.active_objects.filter(user=value).exists():
+        if UserCompany.active_objects.filter(user=value, company_id=company_id).exists():
             raise ValidationError(_('Указанный пользователь уже является сотрудником компании'))
         return value
 
     def validate(self, data):
         validated_data = super().validate(data)
         user = validated_data.get('user', None)
         email = validated_data.get('email', None)
```

### Comparing `garpix_company-2.6.0/garpix_company/serializers/user_company.py` & `garpix_company-2.6.1/garpix_company/serializers/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/services/role_service.py` & `garpix_company-2.6.1/garpix_company/services/role_service.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/settings.py` & `garpix_company-2.6.1/garpix_company/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/setup.py` & `garpix_company-2.6.1/garpix_company/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.6.0',
+    version='2.6.1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_company-2.6.0/garpix_company/urls.py` & `garpix_company-2.6.1/garpix_company/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/views/company.py` & `garpix_company-2.6.1/garpix_company/views/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/views/invite.py` & `garpix_company-2.6.1/garpix_company/views/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company/views/user_company.py` & `garpix_company-2.6.1/garpix_company/views/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/garpix_company.egg-info/PKG-INFO` & `garpix_company-2.6.1/garpix_company.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-company
-Version: 2.6.0
+Version: 2.6.1
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_company-2.6.0/garpix_company.egg-info/SOURCES.txt` & `garpix_company-2.6.1/garpix_company.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_company-2.6.0/setup.py` & `garpix_company-2.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.6.0',
+    version='2.6.1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```


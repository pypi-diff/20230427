# Comparing `tmp/djangorestframework-stubs-1.9.1.tar.gz` & `tmp/djangorestframework-stubs-3.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-stubs-1.9.1.tar", last modified: Thu Feb 23 12:13:13 2023, max compression
+gzip compressed data, was "djangorestframework-stubs-3.14.0.tar", last modified: Thu Apr 27 14:18:07 2023, max compression
```

## Comparing `djangorestframework-stubs-1.9.1.tar` & `djangorestframework-stubs-3.14.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:13.377945 djangorestframework-stubs-1.9.1/
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1075 2019-12-19 16:09:51.000000 djangorestframework-stubs-1.9.1/LICENSE.txt
--rw-r--r--   0 marti.raudsepp   (502) 630137818     2493 2023-02-23 12:13:13.378159 djangorestframework-stubs-1.9.1/PKG-INFO
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1495 2023-02-09 11:45:29.000000 djangorestframework-stubs-1.9.1/README.md
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:12.975474 djangorestframework-stubs-1.9.1/djangorestframework_stubs.egg-info/
--rw-r--r--   0 marti.raudsepp   (502) 630137818     2493 2023-02-23 12:13:12.000000 djangorestframework-stubs-1.9.1/djangorestframework_stubs.egg-info/PKG-INFO
--rw-r--r--   0 marti.raudsepp   (502) 630137818     3237 2023-02-23 12:13:12.000000 djangorestframework-stubs-1.9.1/djangorestframework_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 marti.raudsepp   (502) 630137818        1 2023-02-23 12:13:12.000000 djangorestframework-stubs-1.9.1/djangorestframework_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 marti.raudsepp   (502) 630137818      212 2023-02-23 12:13:12.000000 djangorestframework-stubs-1.9.1/djangorestframework_stubs.egg-info/requires.txt
--rw-r--r--   0 marti.raudsepp   (502) 630137818       37 2023-02-23 12:13:12.000000 djangorestframework-stubs-1.9.1/djangorestframework_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:12.977544 djangorestframework-stubs-1.9.1/mypy_drf_plugin/
--rw-r--r--   0 marti.raudsepp   (502) 630137818        0 2019-12-19 16:09:51.000000 djangorestframework-stubs-1.9.1/mypy_drf_plugin/__init__.py
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:12.991715 djangorestframework-stubs-1.9.1/mypy_drf_plugin/lib/
--rw-r--r--   0 marti.raudsepp   (502) 630137818        0 2019-12-19 16:09:51.000000 djangorestframework-stubs-1.9.1/mypy_drf_plugin/lib/__init__.py
--rw-r--r--   0 marti.raudsepp   (502) 630137818     2714 2020-11-23 10:59:14.000000 djangorestframework-stubs-1.9.1/mypy_drf_plugin/lib/fullnames.py
--rw-r--r--   0 marti.raudsepp   (502) 630137818      167 2020-11-23 10:59:14.000000 djangorestframework-stubs-1.9.1/mypy_drf_plugin/lib/helpers.py
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1880 2023-02-23 11:29:15.000000 djangorestframework-stubs-1.9.1/mypy_drf_plugin/main.py
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:12.998174 djangorestframework-stubs-1.9.1/mypy_drf_plugin/transformers/
--rw-r--r--   0 marti.raudsepp   (502) 630137818        0 2019-12-19 16:09:51.000000 djangorestframework-stubs-1.9.1/mypy_drf_plugin/transformers/__init__.py
--rw-r--r--   0 marti.raudsepp   (502) 630137818      355 2019-12-19 16:09:51.000000 djangorestframework-stubs-1.9.1/mypy_drf_plugin/transformers/serializers.py
--rw-r--r--   0 marti.raudsepp   (502) 630137818      207 2022-11-16 14:21:32.000000 djangorestframework-stubs-1.9.1/pyproject.toml
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:13.217166 djangorestframework-stubs-1.9.1/rest_framework-stubs/
--rw-r--r--   0 marti.raudsepp   (502) 630137818      193 2020-11-23 10:59:14.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/__init__.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818       77 2019-12-19 16:09:51.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/apps.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1115 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/authentication.pyi
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:13.250395 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/
--rw-r--r--   0 marti.raudsepp   (502) 630137818       24 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/__init__.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818       74 2019-12-19 16:09:51.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/admin.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818       73 2019-12-19 16:09:51.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/apps.pyi
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:13.251638 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/management/
--rw-r--r--   0 marti.raudsepp   (502) 630137818        0 2020-11-23 10:59:14.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/management/__init__.pyi
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:13.257571 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/management/commands/
--rw-r--r--   0 marti.raudsepp   (502) 630137818        0 2020-11-23 10:59:14.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/management/commands/__init__.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      394 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/management/commands/drf_create_token.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      296 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/models.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      196 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/serializers.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      417 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/authtoken/views.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      103 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/checks.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1985 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/compat.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     3265 2023-02-09 11:45:29.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/decorators.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1560 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/documentation.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     2146 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/exceptions.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818    23612 2023-02-09 11:45:29.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/fields.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1988 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/filters.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     4415 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/generics.pyi
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:13.258671 djangorestframework-stubs-1.9.1/rest_framework-stubs/management/
--rw-r--r--   0 marti.raudsepp   (502) 630137818        0 2022-05-24 09:49:48.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/management/__init__.pyi
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:13.265456 djangorestframework-stubs-1.9.1/rest_framework-stubs/management/commands/
--rw-r--r--   0 marti.raudsepp   (502) 630137818        0 2022-05-24 09:49:48.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/management/commands/__init__.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      384 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/management/commands/generateschema.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      737 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/metadata.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1260 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/mixins.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      739 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/negotiation.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     4964 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/pagination.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1794 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/parsers.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     3062 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/permissions.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     6893 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/relations.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     4382 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/renderers.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     3302 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/request.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1128 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/response.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      671 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/reverse.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     2564 2023-02-22 13:00:57.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/routers.pyi
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:13.302754 djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/
--rw-r--r--   0 marti.raudsepp   (502) 630137818      973 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/__init__.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     2814 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/coreapi.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     2044 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/generators.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      528 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/inspectors.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     3250 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/openapi.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      261 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/utils.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      218 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/views.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818    12294 2023-02-09 11:45:29.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/serializers.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     4150 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/settings.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     2642 2021-05-13 08:26:11.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/status.pyi
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:13.314114 djangorestframework-stubs-1.9.1/rest_framework-stubs/templatetags/
--rw-r--r--   0 marti.raudsepp   (502) 630137818        0 2020-11-23 10:59:14.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/templatetags/__init__.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1658 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/templatetags/rest_framework.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     5571 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/test.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1126 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/throttling.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      565 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/urlpatterns.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818       89 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/urls.pyi
-drwxr-xr-x   0 marti.raudsepp   (502) 630137818        0 2023-02-23 12:13:13.377107 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/
--rw-r--r--   0 marti.raudsepp   (502) 630137818        0 2019-12-19 16:09:51.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/__init__.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818       86 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/breadcrumbs.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818       54 2019-12-19 16:09:51.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/encoders.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      918 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/field_mapping.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      404 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/formatting.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      213 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/html.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      183 2022-11-18 08:18:27.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/humanize_datetime.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      274 2019-12-19 16:09:51.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/json.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      293 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/mediatypes.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      703 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/model_meta.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      280 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/representation.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1824 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/serializer_helpers.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      145 2020-11-23 10:59:14.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/urls.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     2975 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/validators.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1169 2023-02-09 09:31:40.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/versioning.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     4716 2023-02-09 11:45:29.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/views.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818     1835 2023-02-22 12:47:19.000000 djangorestframework-stubs-1.9.1/rest_framework-stubs/viewsets.pyi
--rw-r--r--   0 marti.raudsepp   (502) 630137818      434 2023-02-23 12:13:13.384370 djangorestframework-stubs-1.9.1/setup.cfg
--rw-r--r--   0 marti.raudsepp   (502) 630137818     2088 2023-02-23 12:11:09.000000 djangorestframework-stubs-1.9.1/setup.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.141746 djangorestframework-stubs-3.14.0/
+-rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/LICENSE.txt
+-rw-r--r--   0 marti     (1000) marti      (121)     2494 2023-04-27 14:18:07.141746 djangorestframework-stubs-3.14.0/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)     1495 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/README.md
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.125080 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/
+-rw-r--r--   0 marti     (1000) marti      (121)     2494 2023-04-27 14:18:07.000000 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)     3237 2023-04-27 14:18:07.000000 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti      (121)        1 2023-04-27 14:18:07.000000 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti      (121)      214 2023-04-27 14:18:07.000000 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       37 2023-04-27 14:18:07.000000 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.125080 djangorestframework-stubs-3.14.0/mypy_drf_plugin/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/__init__.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.128413 djangorestframework-stubs-3.14.0/mypy_drf_plugin/lib/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/lib/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2714 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/lib/fullnames.py
+-rw-r--r--   0 marti     (1000) marti      (121)      167 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/lib/helpers.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1880 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/main.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.128413 djangorestframework-stubs-3.14.0/mypy_drf_plugin/transformers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/transformers/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)      355 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/transformers/serializers.py
+-rw-r--r--   0 marti     (1000) marti      (121)      207 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/pyproject.toml
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/
+-rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       77 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1115 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authentication.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/
+-rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       74 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       73 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      394 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/management/commands/drf_create_token.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/views.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1985 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/compat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3265 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1560 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/documentation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3052 2023-04-27 14:17:42.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    23612 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2002 2023-04-27 14:17:42.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/filters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4415 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/generics.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      384 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/management/commands/generateschema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      737 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/metadata.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1260 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/negotiation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4964 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/pagination.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1794 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/parsers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3062 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/permissions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6893 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/relations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4382 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/renderers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3302 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/request.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1128 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/response.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      671 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/reverse.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/routers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.138413 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/
+-rw-r--r--   0 marti     (1000) marti      (121)      973 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2814 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/coreapi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2044 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/generators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      528 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/inspectors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3250 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/openapi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      261 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/views.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    12294 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4150 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/settings.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2642 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/status.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.138413 djangorestframework-stubs-3.14.0/rest_framework-stubs/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1658 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/templatetags/rest_framework.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5592 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/test.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1126 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/throttling.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      565 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/urlpatterns.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       89 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/urls.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.141746 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/breadcrumbs.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       54 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/encoders.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      918 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/field_mapping.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      404 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/formatting.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/html.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      183 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/humanize_datetime.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/json.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/mediatypes.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      703 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/model_meta.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/representation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1824 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/serializer_helpers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      145 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/validators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1169 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/versioning.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4716 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/views.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1835 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/viewsets.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      434 2023-04-27 14:18:07.141746 djangorestframework-stubs-3.14.0/setup.cfg
+-rw-r--r--   0 marti     (1000) marti      (121)     2091 2023-04-27 14:17:42.000000 djangorestframework-stubs-3.14.0/setup.py
```

### Comparing `djangorestframework-stubs-1.9.1/LICENSE.txt` & `djangorestframework-stubs-3.14.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/PKG-INFO` & `djangorestframework-stubs-3.14.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-stubs
-Version: 1.9.1
+Version: 3.14.0
 Summary: PEP-484 stubs for django-rest-framework
 Home-page: https://github.com/typeddjango/djangorestframework-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
```

### Comparing `djangorestframework-stubs-1.9.1/README.md` & `djangorestframework-stubs-3.14.0/README.md`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/djangorestframework_stubs.egg-info/PKG-INFO` & `djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-stubs
-Version: 1.9.1
+Version: 3.14.0
 Summary: PEP-484 stubs for django-rest-framework
 Home-page: https://github.com/typeddjango/djangorestframework-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
```

### Comparing `djangorestframework-stubs-1.9.1/djangorestframework_stubs.egg-info/SOURCES.txt` & `djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/mypy_drf_plugin/lib/fullnames.py` & `djangorestframework-stubs-3.14.0/mypy_drf_plugin/lib/fullnames.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/mypy_drf_plugin/main.py` & `djangorestframework-stubs-3.14.0/mypy_drf_plugin/main.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/authentication.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/authentication.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/compat.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/decorators.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/decorators.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/documentation.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/documentation.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/exceptions.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/exceptions.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,74 @@
-from collections.abc import Sequence
+from collections.abc import Mapping, Sequence
 from typing import Any
 
 from django.http import HttpRequest, JsonResponse
 from django_stubs_ext import StrOrPromise
 from rest_framework.renderers import BaseRenderer
 from rest_framework.request import Request
-from typing_extensions import TypeAlias
-
-def _get_error_details(data: Any, default_code: str | None = ...) -> Any: ...
-def _get_codes(detail: Any) -> Any: ...
-def _get_full_details(detail: Any) -> Any: ...
+from typing_extensions import TypeAlias, TypedDict
 
 class ErrorDetail(str):
     code: str | None
     def __new__(cls, string: str, code: str | None = ...): ...
 
-_Detail: TypeAlias = StrOrPromise | list[Any] | dict[str, Any]
+_Detail: TypeAlias = ErrorDetail | list[ErrorDetail] | dict[str, ErrorDetail]
+# NB! _APIExceptionInput doesn't technically handle Sequence/Mapping, but only list/tuple/dict.
+# But since list/tuple are non-covariant types, we run into issues with union type compatibility for input params.
+# So use the more relaxed Sequence/Mapping for now.
+_APIExceptionInput: TypeAlias = (
+    _Detail | StrOrPromise | Sequence[_APIExceptionInput] | Mapping[str, _APIExceptionInput] | None
+)
+_ErrorCodes: TypeAlias = str | None | list[_ErrorCodes] | dict[str, _ErrorCodes]
+
+class _FullDetailDict(TypedDict):
+    message: ErrorDetail
+    code: str | None
+
+_ErrorFullDetails: TypeAlias = _FullDetailDict | list[_FullDetailDict] | dict[str, _FullDetailDict]
+
+def _get_error_details(data: _APIExceptionInput, default_code: str | None = ...) -> _Detail: ...
+def _get_codes(detail: _Detail) -> _ErrorCodes: ...
+def _get_full_details(detail: _Detail) -> _ErrorFullDetails: ...
 
 class APIException(Exception):
     status_code: int
-    default_detail: _Detail
+    default_detail: _APIExceptionInput
     default_code: str
 
     detail: _Detail
-    def __init__(self, detail: _Detail | None = ..., code: str | None = ...) -> None: ...
-    def get_codes(self) -> Any: ...
-    def get_full_details(self) -> Any: ...
+    def __init__(self, detail: _APIExceptionInput = ..., code: str | None = ...) -> None: ...
+    def get_codes(self) -> _ErrorCodes: ...
+    def get_full_details(self) -> _ErrorFullDetails: ...
+
+class ValidationError(APIException):
+    # ValidationError always wraps `detail` in a list.
+    detail: list[ErrorDetail] | dict[str, ErrorDetail]
 
-class ValidationError(APIException): ...
 class ParseError(APIException): ...
 class AuthenticationFailed(APIException): ...
 class NotAuthenticated(APIException): ...
 class PermissionDenied(APIException): ...
 class NotFound(APIException): ...
 
 class MethodNotAllowed(APIException):
-    def __init__(self, method: str, detail: _Detail | None = ..., code: str | None = ...) -> None: ...
+    def __init__(self, method: str, detail: _APIExceptionInput = ..., code: str | None = ...) -> None: ...
 
 class NotAcceptable(APIException):
     available_renderers: Sequence[BaseRenderer] | None
     def __init__(
         self,
-        detail: _Detail | None = ...,
+        detail: _APIExceptionInput = ...,
         code: str | None = ...,
         available_renderers: Sequence[BaseRenderer] | None = ...,
     ) -> None: ...
 
 class UnsupportedMediaType(APIException):
-    def __init__(self, media_type: str, detail: _Detail | None = ..., code: str | None = ...) -> None: ...
+    def __init__(self, media_type: str, detail: _APIExceptionInput = ..., code: str | None = ...) -> None: ...
 
 class Throttled(APIException):
     extra_detail_singular: str
     extra_detail_plural: str
-    def __init__(self, wait: float | None = ..., detail: _Detail | None = ..., code: str | None = ...): ...
+    def __init__(self, wait: float | None = ..., detail: _APIExceptionInput = ..., code: str | None = ...): ...
 
 def server_error(request: HttpRequest | Request, *args: Any, **kwargs: Any) -> JsonResponse: ...
 def bad_request(request: HttpRequest | Request, exception: Exception, *args: Any, **kwargs: Any) -> JsonResponse: ...
```

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/fields.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/fields.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/filters.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/filters.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 class OrderingFilter(BaseFilterBackend):
     ordering_param: str
     ordering_fields: Sequence[str] | None
     ordering_title: str
     ordering_description: str
     template: str
-    def get_ordering(self, request: Request, queryset: QuerySet, view: APIView) -> Sequence[str]: ...
-    def get_default_ordering(self, view: APIView) -> Sequence[str]: ...
+    def get_ordering(self, request: Request, queryset: QuerySet, view: APIView) -> Sequence[str] | None: ...
+    def get_default_ordering(self, view: APIView) -> Sequence[str] | None: ...
     def get_default_valid_fields(
         self, queryset: QuerySet, view, context: Mapping[str, Any] = ...
     ) -> list[tuple[str, str]]: ...
     def get_valid_fields(self, queryset: QuerySet, view, context: Mapping[str, Any] = ...) -> list[tuple[str, str]]: ...
     def remove_invalid_fields(self, queryset: QuerySet, fields: Iterable[str], view, request: Request) -> list[str]: ...
     def get_template_context(self, request: Request, queryset: QuerySet, view: APIView) -> dict[str, Any]: ...
     def to_html(self, request: Request, queryset: QuerySet, view: APIView) -> str: ...
```

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/generics.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/generics.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/metadata.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/metadata.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/mixins.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/mixins.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/negotiation.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/negotiation.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/pagination.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/pagination.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/parsers.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/permissions.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/permissions.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/relations.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/relations.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/renderers.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/renderers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/request.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/request.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/response.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/reverse.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/reverse.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/routers.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/routers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/__init__.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/coreapi.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/coreapi.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/generators.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/generators.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/inspectors.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/inspectors.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/schemas/openapi.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/openapi.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/serializers.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/serializers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/settings.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/settings.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/status.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/status.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/templatetags/rest_framework.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/templatetags/rest_framework.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/test.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/test.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,17 @@
 
 class ForceAuthClientHandler(ClientHandler):
     def __init__(self, *args: Any, **kwargs: Any): ...
     def get_response(self, request: Request) -> _MonkeyPatchedResponse: ...  # type: ignore[override]
 
 class APIClient(APIRequestFactory, DjangoClient):
     def credentials(self, **kwargs: Any): ...
-    def force_authenticate(self, user: AnonymousUser | AbstractBaseUser = ..., token: Token | None = ...) -> None: ...
+    def force_authenticate(
+        self, user: AnonymousUser | AbstractBaseUser | None = ..., token: Token | None = ...
+    ) -> None: ...
     def request(self, **kwargs: Any) -> _MonkeyPatchedResponse: ...  # type: ignore[override]
     def get(self, path: str, data: _GetDataType = ..., follow: bool = ..., **extra: Any) -> _MonkeyPatchedResponse: ...  # type: ignore[override]
     def post(self, path: str, data: Any | None = ..., format: str | None = ..., content_type: str | None = ..., follow: bool = ..., **extra: Any) -> _MonkeyPatchedResponse: ...  # type: ignore[override]
     def put(self, path: str, data: Any | None = ..., format: str | None = ..., content_type: str | None = ..., follow: bool = ..., **extra: Any) -> _MonkeyPatchedResponse: ...  # type: ignore[override]
     def patch(self, path: str, data: Any | None = ..., format: str | None = ..., content_type: str | None = ..., follow: bool = ..., **extra: Any) -> _MonkeyPatchedResponse: ...  # type: ignore[override]
     def delete(self, path: str, data: Any | None = ..., format: str | None = ..., content_type: str | None = ..., follow: bool = ..., **extra: Any) -> _MonkeyPatchedResponse: ...  # type: ignore[override]
     def options(self, path: str, data: dict[str, str] | str = ..., format: str | None = ..., content_type: Any | None = ..., follow: bool = ..., **extra: Any) -> _MonkeyPatchedResponse: ...  # type: ignore[override]
```

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/throttling.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/throttling.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/urlpatterns.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/urlpatterns.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/field_mapping.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/field_mapping.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/model_meta.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/model_meta.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/utils/serializer_helpers.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/serializer_helpers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/validators.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/validators.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/versioning.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/versioning.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/views.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/views.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/rest_framework-stubs/viewsets.pyi` & `djangorestframework-stubs-3.14.0/rest_framework-stubs/viewsets.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-1.9.1/setup.py` & `djangorestframework-stubs-3.14.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,31 +16,31 @@
     return result
 
 
 with open("README.md") as f:
     readme = f.read()
 
 dependencies = [
-    "mypy>=0.980",
+    "mypy>=0.991",
     "django-stubs>=1.13.0",
     "typing-extensions>=3.10.0",
     "requests>=2.0.0",
     "types-requests>=0.1.12",
     "types-PyYAML>=5.4.3",
 ]
 
 extras_require = {
-    "compatible-mypy": ["mypy>=1.0,<1.1"],
+    "compatible-mypy": ["mypy>=1.2.0,<1.3"],
     "coreapi": ["coreapi>=2.0.0"],
     "markdown": ["types-Markdown>=0.1.5"],
 }
 
 setup(
     name="djangorestframework-stubs",
-    version="1.9.1",
+    version="3.14.0",
     description="PEP-484 stubs for django-rest-framework",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/typeddjango/djangorestframework-stubs",
     author="Maksim Kurnikov",
     author_email="maxim.kurnikov@gmail.com",
     maintainer="Marti Raudsepp",
```


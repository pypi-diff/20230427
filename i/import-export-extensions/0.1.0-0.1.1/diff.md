# Comparing `tmp/import_export_extensions-0.1.0.tar.gz` & `tmp/import_export_extensions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "import_export_extensions-0.1.0.tar", last modified: Tue Apr 25 15:06:35 2023, max compression
+gzip compressed data, was "import_export_extensions-0.1.1.tar", last modified: Thu Apr 27 11:21:02 2023, max compression
```

## Comparing `import_export_extensions-0.1.0.tar` & `import_export_extensions-0.1.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.583753 import_export_extensions-0.1.0/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      176 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/AUTHORS.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3236 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)       89 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/HISTORY.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1066 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/LICENSE
--rw-r--r--   0 yalef     (1000) yalef     (1000)      282 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/MANIFEST.in
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2948 2023-04-25 15:06:35.583753 import_export_extensions-0.1.0/PKG-INFO
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1922 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/README.rst
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.567087 import_export_extensions-0.1.0/docs/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      625 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/docs/Makefile
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.553753 import_export_extensions-0.1.0/docs/_build/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.553753 import_export_extensions-0.1.0/docs/_build/html/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.567087 import_export_extensions-0.1.0/docs/_build/html/_static/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      286 2023-04-05 15:45:06.000000 import_export_extensions-0.1.0/docs/_build/html/_static/file.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 import_export_extensions-0.1.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 import_export_extensions-0.1.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/docs/authors.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     4476 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/docs/conf.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)       33 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/docs/contributing.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/docs/history.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)      334 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/docs/index.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2754 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/docs/installation.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)      822 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/docs/make.bat
--rw-r--r--   0 yalef     (1000) yalef     (1000)       27 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/docs/readme.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3447 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/docs/usage.rst
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.567087 import_export_extensions-0.1.0/import_export_extensions/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      144 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.570420 import_export_extensions-0.1.0/import_export_extensions/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      166 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.570420 import_export_extensions-0.1.0/import_export_extensions/admin/forms/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      100 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/forms/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      997 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/forms/export_admin_form.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1177 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/forms/import_admin_form.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.570420 import_export_extensions-0.1.0/import_export_extensions/admin/mixins/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      155 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/mixins/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      797 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/mixins/base.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    10885 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/mixins/export_mixin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      340 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/mixins/import_export_mixin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    12731 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/mixins/import_mixin.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.573753 import_export_extensions-0.1.0/import_export_extensions/admin/model_admins/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/model_admins/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5715 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/model_admins/export_job_admin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     7018 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/model_admins/import_job_admin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3817 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/model_admins/mixins.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1394 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/admin/widgets.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.573753 import_export_extensions-0.1.0/import_export_extensions/api/
--rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/api/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.573753 import_export_extensions-0.1.0/import_export_extensions/api/serializers/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      156 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/api/serializers/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3566 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/api/serializers/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3158 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/api/serializers/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      378 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/api/serializers/progress.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.573753 import_export_extensions-0.1.0/import_export_extensions/api/views/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       82 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/api/views/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     4418 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/api/views/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     6243 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/api/views/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      716 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/apps.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     7233 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/fields.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1315 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/forms.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.573753 import_export_extensions-0.1.0/import_export_extensions/migrations/
--rw-r--r--   0 yalef     (1000) yalef     (1000)    12282 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/migrations/0001_initial.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/migrations/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.577087 import_export_extensions-0.1.0/import_export_extensions/models/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       68 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/models/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1267 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/models/core.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    10445 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/models/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    17389 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/models/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      752 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/models/tools.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     8148 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/resources.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.557087 import_export_extensions-0.1.0/import_export_extensions/static/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.560420 import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.560420 import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/css/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.577087 import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/css/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       67 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/css/admin/admin.css
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.577087 import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/css/widgets/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      626 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.560420 import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/js/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.577087 import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/js/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      768 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/js/admin/admin.js
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.577087 import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/js/widgets/
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1712 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js
--rw-r--r--   0 yalef     (1000) yalef     (1000)      537 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/tasks.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.560420 import_export_extensions-0.1.0/import_export_extensions/templates/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.580420 import_export_extensions-0.1.0/import_export_extensions/templates/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       37 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/base.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1081 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1482 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_export_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2440 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_export_status.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1215 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_import.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5062 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_import_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2413 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_import_status.html
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.583753 import_export_extensions-0.1.0/import_export_extensions/templates/admin/change_list/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      391 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/change_list/change_list.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/change_list/change_list_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/change_list/change_list_export_item.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/change_list/change_list_import.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      248 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/change_list/change_list_import_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/change_list/change_list_import_item.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2571 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/templates/admin/import_job_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5135 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/utils.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    10744 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/import_export_extensions/widgets.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-25 15:06:35.570420 import_export_extensions-0.1.0/import_export_extensions.egg-info/
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2948 2023-04-25 15:06:35.000000 import_export_extensions-0.1.0/import_export_extensions.egg-info/PKG-INFO
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3724 2023-04-25 15:06:35.000000 import_export_extensions-0.1.0/import_export_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-04-25 15:06:35.000000 import_export_extensions-0.1.0/import_export_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)       79 2023-04-25 15:06:35.000000 import_export_extensions-0.1.0/import_export_extensions.egg-info/entry_points.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-04-25 15:06:35.000000 import_export_extensions-0.1.0/import_export_extensions.egg-info/not-zip-safe
--rw-r--r--   0 yalef     (1000) yalef     (1000)      126 2023-04-25 15:06:35.000000 import_export_extensions-0.1.0/import_export_extensions.egg-info/requires.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)       25 2023-04-25 15:06:35.000000 import_export_extensions-0.1.0/import_export_extensions.egg-info/top_level.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1791 2023-04-25 15:06:35.583753 import_export_extensions-0.1.0/setup.cfg
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2481 2023-04-18 11:22:55.000000 import_export_extensions-0.1.0/setup.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.721572 import_export_extensions-0.1.1/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      176 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/AUTHORS.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3236 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      206 2023-04-27 11:07:57.000000 import_export_extensions-0.1.1/HISTORY.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1066 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/LICENSE
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      282 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/MANIFEST.in
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3228 2023-04-27 11:21:02.721572 import_export_extensions-0.1.1/PKG-INFO
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2072 2023-04-27 10:39:21.000000 import_export_extensions-0.1.1/README.rst
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.678239 import_export_extensions-0.1.1/docs/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      625 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/docs/Makefile
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.664905 import_export_extensions-0.1.1/docs/_build/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.664905 import_export_extensions-0.1.1/docs/_build/html/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.678239 import_export_extensions-0.1.1/docs/_build/html/_static/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      286 2023-04-05 15:45:06.000000 import_export_extensions-0.1.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 import_export_extensions-0.1.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 import_export_extensions-0.1.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/docs/authors.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4476 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/docs/conf.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       33 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/docs/contributing.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/docs/history.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      334 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/docs/index.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2754 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/docs/installation.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      822 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/docs/make.bat
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       27 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/docs/readme.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3447 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/docs/usage.rst
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.681572 import_export_extensions-0.1.1/import_export_extensions/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      144 2023-04-27 11:03:10.000000 import_export_extensions-0.1.1/import_export_extensions/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.684905 import_export_extensions-0.1.1/import_export_extensions/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      166 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.684905 import_export_extensions-0.1.1/import_export_extensions/admin/forms/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      100 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/forms/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      997 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/forms/export_admin_form.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1177 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/forms/import_admin_form.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.688239 import_export_extensions-0.1.1/import_export_extensions/admin/mixins/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      155 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/mixins/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      797 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/mixins/base.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    10885 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/mixins/export_mixin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      340 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/mixins/import_export_mixin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    12731 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/mixins/import_mixin.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.701572 import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5715 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/export_job_admin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     7018 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/import_job_admin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3817 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/mixins.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1394 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/admin/widgets.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.701572 import_export_extensions-0.1.1/import_export_extensions/api/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/api/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.704905 import_export_extensions-0.1.1/import_export_extensions/api/serializers/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      156 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/api/serializers/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3566 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/api/serializers/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3158 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/api/serializers/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      378 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/api/serializers/progress.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.708239 import_export_extensions-0.1.1/import_export_extensions/api/views/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       82 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/api/views/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4418 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/api/views/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     6243 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/api/views/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      716 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/apps.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     7233 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/fields.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1315 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/forms.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.708239 import_export_extensions-0.1.1/import_export_extensions/migrations/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    12282 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/migrations/0001_initial.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/migrations/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.711572 import_export_extensions-0.1.1/import_export_extensions/models/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       68 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/models/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1267 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/models/core.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    10445 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/models/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    17389 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/models/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      752 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/models/tools.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     8148 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/resources.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.671572 import_export_extensions-0.1.1/import_export_extensions/static/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.671572 import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.671572 import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.711572 import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       67 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/admin/admin.css
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.711572 import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/widgets/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      626 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.671572 import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.711572 import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      768 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/admin/admin.js
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.714905 import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/widgets/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1712 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      537 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/tasks.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.671572 import_export_extensions-0.1.1/import_export_extensions/templates/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.718239 import_export_extensions-0.1.1/import_export_extensions/templates/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       37 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/base.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1081 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1482 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2440 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export_status.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1215 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5062 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2413 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import_status.html
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.721572 import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      391 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list_export_item.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list_import.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      248 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list_import_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/change_list/change_list_import_item.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2571 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/templates/admin/import_job_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5135 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/utils.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    10744 2023-04-18 11:22:55.000000 import_export_extensions-0.1.1/import_export_extensions/widgets.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-04-27 11:21:02.684905 import_export_extensions-0.1.1/import_export_extensions.egg-info/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3228 2023-04-27 11:21:02.000000 import_export_extensions-0.1.1/import_export_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3724 2023-04-27 11:21:02.000000 import_export_extensions-0.1.1/import_export_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-04-27 11:21:02.000000 import_export_extensions-0.1.1/import_export_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       79 2023-04-27 11:21:02.000000 import_export_extensions-0.1.1/import_export_extensions.egg-info/entry_points.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-04-27 11:21:02.000000 import_export_extensions-0.1.1/import_export_extensions.egg-info/not-zip-safe
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      126 2023-04-27 11:21:02.000000 import_export_extensions-0.1.1/import_export_extensions.egg-info/requires.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       25 2023-04-27 11:21:02.000000 import_export_extensions-0.1.1/import_export_extensions.egg-info/top_level.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1791 2023-04-27 11:21:02.721572 import_export_extensions-0.1.1/setup.cfg
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2472 2023-04-27 11:03:24.000000 import_export_extensions-0.1.1/setup.py
```

### Comparing `import_export_extensions-0.1.0/CONTRIBUTING.rst` & `import_export_extensions-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/LICENSE` & `import_export_extensions-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/PKG-INFO` & `import_export_extensions-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: import_export_extensions
-Version: 0.1.0
-Summary: TODO: There should be description
+Version: 0.1.1
+Summary: Extend functionality of `django-import-export`
 Home-page: https://github.com/saritasa-nest/django-import-export-extensions
 Author: Saritasa
 Author-email: pypi@saritasa.com
 License: MIT license
 Keywords: import_export_extensions
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -29,21 +29,24 @@
 ===============================
 
 .. image:: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml/badge.svg
         :target: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml
         :alt: Build status on Github
 
 .. image:: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
-        :target: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
+        :target: https://pypi.org/project/import-export-extensions/
         :alt: Supported python versions
 
 .. image:: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
-        :target: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
+        :target: https://pypi.org/project/import-export-extensions/
         :alt: Supported django versions
 
+.. image:: https://readthedocs.org/projects/django-import-export-extensions/badge/?version=latest
+    :target: https://django-import-export-extensions.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
 
 Description
 -----------
 `django-import-export-extensions` extends the functionality of
 `django-import-export <https://github.com/django-import-export/django-import-export/>`_
 adding the following features:
 
@@ -71,11 +74,17 @@
 * Documentation: https://django-import-export-extensions.readthedocs.io.
 
 
 =======
 History
 =======
 
+0.1.1 (2023-04-27)
+------------------
+
+* Add package description
+* Add configuration file for read-the-docs service
+
 0.1.0 (2023-04-01)
 ------------------
 
 * First release on PyPI.
```

### Comparing `import_export_extensions-0.1.0/README.rst` & `import_export_extensions-0.1.1/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 ===============================
 
 .. image:: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml/badge.svg
         :target: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml
         :alt: Build status on Github
 
 .. image:: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
-        :target: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
+        :target: https://pypi.org/project/import-export-extensions/
         :alt: Supported python versions
 
 .. image:: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
-        :target: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
+        :target: https://pypi.org/project/import-export-extensions/
         :alt: Supported django versions
 
+.. image:: https://readthedocs.org/projects/django-import-export-extensions/badge/?version=latest
+    :target: https://django-import-export-extensions.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
 
 Description
 -----------
 `django-import-export-extensions` extends the functionality of
 `django-import-export <https://github.com/django-import-export/django-import-export/>`_
 adding the following features:
```

### Comparing `import_export_extensions-0.1.0/docs/Makefile` & `import_export_extensions-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/docs/conf.py` & `import_export_extensions-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/docs/installation.rst` & `import_export_extensions-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/docs/make.bat` & `import_export_extensions-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/docs/usage.rst` & `import_export_extensions-0.1.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/admin/forms/export_admin_form.py` & `import_export_extensions-0.1.1/import_export_extensions/admin/forms/export_admin_form.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/admin/forms/import_admin_form.py` & `import_export_extensions-0.1.1/import_export_extensions/admin/forms/import_admin_form.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/admin/mixins/base.py` & `import_export_extensions-0.1.1/import_export_extensions/admin/mixins/base.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/admin/mixins/export_mixin.py` & `import_export_extensions-0.1.1/import_export_extensions/admin/mixins/export_mixin.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/admin/mixins/import_mixin.py` & `import_export_extensions-0.1.1/import_export_extensions/admin/mixins/import_mixin.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/admin/model_admins/export_job_admin.py` & `import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/export_job_admin.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/admin/model_admins/import_job_admin.py` & `import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/import_job_admin.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/admin/model_admins/mixins.py` & `import_export_extensions-0.1.1/import_export_extensions/admin/model_admins/mixins.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/admin/widgets.py` & `import_export_extensions-0.1.1/import_export_extensions/admin/widgets.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/api/serializers/export_job.py` & `import_export_extensions-0.1.1/import_export_extensions/api/serializers/export_job.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/api/serializers/import_job.py` & `import_export_extensions-0.1.1/import_export_extensions/api/serializers/import_job.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/api/views/export_job.py` & `import_export_extensions-0.1.1/import_export_extensions/api/views/export_job.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/api/views/import_job.py` & `import_export_extensions-0.1.1/import_export_extensions/api/views/import_job.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/apps.py` & `import_export_extensions-0.1.1/import_export_extensions/apps.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/fields.py` & `import_export_extensions-0.1.1/import_export_extensions/fields.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/forms.py` & `import_export_extensions-0.1.1/import_export_extensions/forms.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/migrations/0001_initial.py` & `import_export_extensions-0.1.1/import_export_extensions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/models/core.py` & `import_export_extensions-0.1.1/import_export_extensions/models/core.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/models/export_job.py` & `import_export_extensions-0.1.1/import_export_extensions/models/export_job.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/models/import_job.py` & `import_export_extensions-0.1.1/import_export_extensions/models/import_job.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/models/tools.py` & `import_export_extensions-0.1.1/import_export_extensions/models/tools.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/resources.py` & `import_export_extensions-0.1.1/import_export_extensions/resources.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css` & `import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/js/admin/admin.js` & `import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/admin/admin.js`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js` & `import_export_extensions-0.1.1/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/tasks.py` & `import_export_extensions-0.1.1/import_export_extensions/tasks.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_export.html` & `import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export.html`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_export_results.html` & `import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export_results.html`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_export_status.html` & `import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_export_status.html`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_import.html` & `import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import.html`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_import_results.html` & `import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import_results.html`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/templates/admin/celery_import_status.html` & `import_export_extensions-0.1.1/import_export_extensions/templates/admin/celery_import_status.html`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/templates/admin/import_job_results.html` & `import_export_extensions-0.1.1/import_export_extensions/templates/admin/import_job_results.html`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/utils.py` & `import_export_extensions-0.1.1/import_export_extensions/utils.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions/widgets.py` & `import_export_extensions-0.1.1/import_export_extensions/widgets.py`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/import_export_extensions.egg-info/PKG-INFO` & `import_export_extensions-0.1.1/import_export_extensions.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: import-export-extensions
-Version: 0.1.0
-Summary: TODO: There should be description
+Version: 0.1.1
+Summary: Extend functionality of `django-import-export`
 Home-page: https://github.com/saritasa-nest/django-import-export-extensions
 Author: Saritasa
 Author-email: pypi@saritasa.com
 License: MIT license
 Keywords: import_export_extensions
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -29,21 +29,24 @@
 ===============================
 
 .. image:: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml/badge.svg
         :target: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml
         :alt: Build status on Github
 
 .. image:: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
-        :target: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
+        :target: https://pypi.org/project/import-export-extensions/
         :alt: Supported python versions
 
 .. image:: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
-        :target: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
+        :target: https://pypi.org/project/import-export-extensions/
         :alt: Supported django versions
 
+.. image:: https://readthedocs.org/projects/django-import-export-extensions/badge/?version=latest
+    :target: https://django-import-export-extensions.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
 
 Description
 -----------
 `django-import-export-extensions` extends the functionality of
 `django-import-export <https://github.com/django-import-export/django-import-export/>`_
 adding the following features:
 
@@ -71,11 +74,17 @@
 * Documentation: https://django-import-export-extensions.readthedocs.io.
 
 
 =======
 History
 =======
 
+0.1.1 (2023-04-27)
+------------------
+
+* Add package description
+* Add configuration file for read-the-docs service
+
 0.1.0 (2023-04-01)
 ------------------
 
 * First release on PyPI.
```

### Comparing `import_export_extensions-0.1.0/import_export_extensions.egg-info/SOURCES.txt` & `import_export_extensions-0.1.1/import_export_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `import_export_extensions-0.1.0/setup.cfg` & `import_export_extensions-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.1.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `import_export_extensions-0.1.0/setup.py` & `import_export_extensions-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    description="TODO: There should be description\nTODO: Rename project",
+    description="Extend functionality of `django-import-export`",
     entry_points={
         "console_scripts": [
             "import_export_extensions=import_export_extensions.cli:main",
         ],
     },
     install_requires=reqs("production.txt"),
     license="MIT license",
@@ -72,10 +72,10 @@
     include_package_data=True,
     keywords="import_export_extensions",
     name="import_export_extensions",
     packages=find_packages(include=["import_export_extensions", "import_export_extensions.*"]),
     test_suite="tests",
     tests_require=reqs("development.txt"),
     url="https://github.com/saritasa-nest/django-import-export-extensions",
-    version="0.1.0",
+    version="0.1.1",
     zip_safe=False,
 )
```


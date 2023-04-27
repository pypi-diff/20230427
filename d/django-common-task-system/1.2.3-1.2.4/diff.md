# Comparing `tmp/django-common-task-system-1.2.3.tar.gz` & `tmp/django-common-task-system-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.2.3.tar", last modified: Sun Apr 23 03:20:20 2023, max compression
+gzip compressed data, was "dist\django-common-task-system-1.2.4.tar", last modified: Thu Apr 27 05:43:22 2023, max compression
```

## Comparing `django-common-task-system-1.2.3.tar` & `django-common-task-system-1.2.4.tar`

### file list

```diff
@@ -1,98 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.083304 django-common-task-system-1.2.3/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.2.3/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-04-23 03:20:20.083304 django-common-task-system-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.037069 django-common-task-system-1.2.3/django_common_task_system/
--rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.2.3/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0    11370 2023-04-21 09:44:38.000000 django-common-task-system-1.2.3/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.2.3/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.2.3/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.2.3/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    15985 2023-04-21 09:40:54.000000 django-common-task-system-1.2.3/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.050304 django-common-task-system-1.2.3/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0006_consumerpermission.py
--rw-rw-rw-   0        0        0     1275 2023-04-21 07:23:00.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.2.3/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.2.3/django_common_task_system/mixin.py
--rw-rw-rw-   0        0        0    36762 2023-04-23 03:16:06.000000 django-common-task-system-1.2.3/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.2.3/django_common_task_system/permissions.py
--rw-rw-rw-   0        0        0     2272 2023-04-21 08:20:32.000000 django-common-task-system-1.2.3/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.023551 django-common-task-system-1.2.3/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.024551 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.051308 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.053307 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.061304 django-common-task-system-1.2.3/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     5166 2023-04-21 07:14:23.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     4130 2023-04-19 09:42:02.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.066307 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
--rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
--rw-rw-rw-   0        0        0     1062 2023-04-21 07:23:00.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0    14945 2023-04-21 07:09:25.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/queue.py
--rw-rw-rw-   0        0        0     1679 2023-04-21 07:11:39.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/serializers.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      846 2023-04-21 07:22:44.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     5505 2023-04-21 07:22:44.000000 django-common-task-system-1.2.3/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.067306 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.069307 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     3100 2023-04-21 07:40:43.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.073310 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.026547 django-common-task-system-1.2.3/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.025546 django-common-task-system-1.2.3/django_common_task_system/templates/admin/
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.074309 django-common-task-system-1.2.3/django_common_task_system/templates/admin/system_schedule/
--rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.2.3/django_common_task_system/templates/admin/system_schedule/change_list.html
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.078307 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.2.3/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0     1060 2023-04-21 07:22:44.000000 django-common-task-system-1.2.3/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.082304 django-common-task-system-1.2.3/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.2.3/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.2.3/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.2.3/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.2.3/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.2.3/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0    11880 2023-04-23 03:18:23.000000 django-common-task-system-1.2.3/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.043308 django-common-task-system-1.2.3/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-04-23 03:20:20.000000 django-common-task-system-1.2.3/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4423 2023-04-23 03:20:20.000000 django-common-task-system-1.2.3/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 03:20:20.000000 django-common-task-system-1.2.3/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-04-23 03:20:20.000000 django-common-task-system-1.2.3/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-23 03:20:20.000000 django-common-task-system-1.2.3/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 03:20:20.084304 django-common-task-system-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-04-23 03:13:16.000000 django-common-task-system-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:20.082304 django-common-task-system-1.2.3/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.2.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/
+-rw-rw-rw-   0        0        0      249 2023-04-27 05:43:08.000000 django-common-task-system-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      289 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-04-27 05:43:08.000000 django-common-task-system-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:21.000000 django-common-task-system-1.2.4/django_common_task_system/
+-rw-rw-rw-   0        0        0     3014 2023-04-27 05:43:08.000000 django-common-task-system-1.2.4/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0    11370 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0     1596 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    15985 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0     3283 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      495 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1560 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/migrations/0006_consumerpermission.py
+-rw-rw-rw-   0        0        0     1275 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/mixin.py
+-rw-rw-rw-   0        0        0    36866 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     1010 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/permissions.py
+-rw-rw-rw-   0        0        0     2272 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:21.000000 django-common-task-system-1.2.4/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:21.000000 django-common-task-system-1.2.4/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     5166 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      629 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     4130 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10614 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0     2209 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+-rw-rw-rw-   0        0        0     1007 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      467 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1540 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+-rw-rw-rw-   0        0        0     1062 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    14945 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1132 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0     2237 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/queue.py
+-rw-rw-rw-   0        0        0     1679 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      846 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     5505 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1674 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     3100 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     3708 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      832 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1110 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      375 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:21.000000 django-common-task-system-1.2.4/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:21.000000 django-common-task-system-1.2.4/django_common_task_system/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/django_common_task_system/templates/admin/system_schedule/
+-rw-rw-rw-   0        0        0     8452 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/templates/admin/system_schedule/change_list.html
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0     1060 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0    12335 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:21.000000 django-common-task-system-1.2.4/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-04-27 05:43:21.000000 django-common-task-system-1.2.4/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4415 2023-04-27 05:43:21.000000 django-common-task-system-1.2.4/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 05:43:21.000000 django-common-task-system-1.2.4/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-27 05:43:21.000000 django-common-task-system-1.2.4/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-27 05:43:21.000000 django-common-task-system-1.2.4/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:43:22.000000 django-common-task-system-1.2.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:43:09.000000 django-common-task-system-1.2.4/tests/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `django-common-task-system-1.2.3/django_common_task_system/__init__.py` & `django-common-task-system-1.2.4/django_common_task_system/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/admin.py` & `django-common-task-system-1.2.4/django_common_task_system/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/choices.py` & `django-common-task-system-1.2.4/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/fields.py` & `django-common-task-system-1.2.4/django_common_task_system/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/forms.py` & `django-common-task-system-1.2.4/django_common_task_system/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.2.4/django_common_task_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.2.4/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py` & `django-common-task-system-1.2.4/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/migrations/0006_consumerpermission.py` & `django-common-task-system-1.2.4/django_common_task_system/migrations/0006_consumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py` & `django-common-task-system-1.2.4/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/mixin.py` & `django-common-task-system-1.2.4/django_common_task_system/mixin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/models.py` & `django-common-task-system-1.2.4/django_common_task_system/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,14 +371,15 @@
             next_time = get_next_cron_time(type_config['crontab'], last_time)
         elif schedule_type == TaskScheduleType.TIMINGS:
             timing_type = type_config['type']
             hour, minute, second = type_config['time'].split(':')
             hour, minute, second = int(hour), int(minute), int(second)
             timing_config = type_config[timing_type]
             timing_period = timing_config.get('period', 1)
+            next_time = datetime(next_time.year, next_time.month, next_time.day, hour, minute, second)
             if timing_type == ScheduleTimingType.DAY:
                 while next_time <= last_time:
                     next_time += timedelta(days=timing_period)
             elif timing_type == ScheduleTimingType.WEEKDAY:
                 weekdays = timing_config['weekday']
                 weekday = last_time.isoweekday()
                 for i in weekdays:
```

### Comparing `django-common-task-system-1.2.3/django_common_task_system/permissions.py` & `django-common-task-system-1.2.4/django_common_task_system/permissions.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/serializers.py` & `django-common-task-system-1.2.4/django_common_task_system/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.2.4/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.2.4/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.2.4/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/choices.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/models.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/models.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/process.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/process.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/queue.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/queue.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/serializers.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task/views.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task_execution/main.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,35 +44,43 @@
             select queue, schedule_id, schedule_time, count(*) as times, max(create_time) as lastest_time 
             from %s where create_time > CURDATE() and status != 'S' 
             GROUP BY queue, schedule_id, schedule_time order by queue, schedule_id, schedule_time
             ) a where a.times < %s and a.lastest_time > '%s' limit %s
         ''' % (self.schedule_log_model._meta.db_table, max_retry_times, last_schedule_time, max_fetch_num,)
         with connection.cursor() as cursor:
             cursor.execute(command)
-            rows = cursor.fetchall()
-        if rows:
+            rows = list(cursor.fetchall())
+        batch_num = 1000
+        i = 0
+        batch = rows[:batch_num]
+        result = {}
+        error = None
+        while batch:
             path = reverse(self.handle_url)
             ids, queues, times = [], [], []
-            for q, i, t, *_ in rows:
+            for q, i, t, *_ in batch:
                 if i == self.schedule_id:
                     continue
                 ids.append(str(i))
                 queues.append(q)
                 times.append(t.strftime('%Y-%m-%d %H:%M:%S'))
-            if ids:
-                url = settings.HOST + path
-                result = requests.get(url, params={
-                    'i': ','.join(ids),
-                    'q': ','.join(queues),
-                    't': ','.join(times)
-                }).json()
-                if 'error' in result:
-                    raise Exception(result['error'])
-                return result
-        return "no schedule need to retry"
+            url = settings.HOST + path
+            batch_result = requests.get(url, params={
+                'i': ','.join(ids),
+                'q': ','.join(queues),
+                't': ','.join(times)
+            }).json()
+            result[i] = batch_result
+            if 'error' in batch_result:
+                error = batch_result['error']
+            i += 1
+            batch = rows[i * batch_num: (i + 1) * batch_num]
+        if error:
+            raise Exception(error)
+        return result
 
 
 class ScheduleExceptionExecutor(SystemExceptionExecutor):
     name = builtins.tasks.task_exception_handling.name
     schedule_model = TaskSchedule
     schedule_id = builtins.schedules.task_exception_handling.id
     schedule_log_model = TaskScheduleLog
```

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.2.4/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/templates/admin/system_schedule/change_list.html` & `django-common-task-system-1.2.4/django_common_task_system/templates/admin/system_schedule/change_list.html`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,210 +1,210 @@
-{% extends "admin/base_site.html" %}
-{% load i18n admin_urls static admin_list %}
-
-{% block extrastyle %}
-  {{ block.super }}
-  <link rel="stylesheet" href="{% static "admin/css/changelists.css" %}">
-  {% if cl.formset %}
-    <link rel="stylesheet" href="{% static "admin/css/forms.css" %}">
-  {% endif %}
-  {% if cl.formset or action_form %}
-    <script src="{% url 'admin:jsi18n' %}"></script>
-  {% endif %}
-  {{ media.css }}
-  {% if not actions_on_top and not actions_on_bottom %}
-    <style>
-      #changelist table thead th:first-child {width: inherit}
-    </style>
-  {% endif %}
-{% endblock %}
-
-
-{% block extrahead %}
-{{ block.super }}
-<script type="text/javascript">window.__admin_media_prefix__ = "{% filter escapejs %}{% static 'admin/' %}{% endfilter %}";</script>
-{{ media.js }}
-<script src="{% static 'admin/js/filters.js' %}" defer></script>
-{% endblock %}
-
-{% block bodyclass %}{{ block.super }} app-{{ opts.app_label }} model-{{ opts.model_name }} change-list{% endblock %}
-
-{% if not is_popup %}
-{% block breadcrumbs %}
-<div class="breadcrumbs">
-<a href="{% url 'admin:index' %}">{% translate 'Home' %}</a>
-&rsaquo; <a href="{% url 'admin:app_list' app_label=cl.opts.app_label %}">{{ cl.opts.app_config.verbose_name }}</a>
-&rsaquo; {{ cl.opts.verbose_name_plural|capfirst }}
-</div>
-{% endblock %}
-{% endif %}
-
-{% block coltype %}{% endblock %}
-
-{% block content %}
-  <div id="option-msg" style="text-align: center; color: red"></div>
-  <div id="content-main">
-    {% block object-tools %}
-        <ul class="object-tools">
-          {% block object-tools-items %}
-            {% change_list_object_tools %}
-          {% endblock %}
-        </ul>
-    {% endblock %}
-    {% if cl.formset and cl.formset.errors %}
-        <p class="errornote">
-        {% if cl.formset.total_error_count == 1 %}{% translate "Please correct the error below." %}{% else %}{% translate "Please correct the errors below." %}{% endif %}
-        </p>
-        {{ cl.formset.non_form_errors }}
-    {% endif %}
-    <div class="module{% if cl.has_filters %} filtered{% endif %}" id="changelist">
-      <div class="changelist-form-container">
-        {% block search %}{% search_form cl %}{% endblock %}
-        {% block date_hierarchy %}{% if cl.date_hierarchy %}{% date_hierarchy cl %}{% endif %}{% endblock %}
-
-        <form id="changelist-form" method="post"{% if cl.formset and cl.formset.is_multipart %} enctype="multipart/form-data"{% endif %} novalidate>{% csrf_token %}
-        {% if cl.formset %}
-          <div>{{ cl.formset.management_form }}</div>
-        {% endif %}
-
-        {% block result_list %}
-          {% if action_form and actions_on_top and cl.show_admin_actions %}{% admin_actions %}{% endif %}
-          {% result_list cl %}
-          {% if action_form and actions_on_bottom and cl.show_admin_actions %}{% admin_actions %}{% endif %}
-        {% endblock %}
-        {% block pagination %}{% pagination cl %}{% endblock %}
-        </form>
-      </div>
-      {% block filters %}
-        {% if cl.has_filters %}
-          <div id="changelist-filter">
-            <h2>{% translate 'Filter' %}</h2>
-            {% if cl.has_active_filters %}<h3 id="changelist-filter-clear">
-              <a href="{{ cl.clear_all_filters_qs }}">&#10006; {% translate "Clear all filters" %}</a>
-            </h3>{% endif %}
-            {% for spec in cl.filter_specs %}{% admin_list_filter cl spec %}{% endfor %}
-          </div>
-        {% endif %}
-      {% endblock %}
-    </div>
-  </div>
-
-    <script>
-        function put_schedule(base_url, schedule_id){
-            const schedule_box = $('#schedule_box_' + schedule_id);
-            let date = schedule_box.find('input[class="vDateField"]').val();
-            let time = schedule_box.find('input[class="vTimeField"]').val();
-            if(date === ""){
-                date = new Date().toLocaleDateString();
-            }
-            if (time === ""){
-                time = new Date().toLocaleTimeString();
-            }
-            if(time.split(':').length === 2){
-                time = time + ':00'
-            }
-            const url = base_url + '&t=' + date.replaceAll('/', '-') + ' ' + time;
-            $.ajax({
-                url: url,
-                dataType: 'json',
-                contentType: 'application/json; charset=utf-8',
-                success: function(data){
-                    $('#option-msg').text("加入成功");
-                    $(document).trigger('mouseup');
-                    setTimeout(function(){
-                        $('#option-msg').text("");
-                    }, 1000);
-                },
-                error: function(data){
-                    console.debug(data);
-                    alert(JSON.stringify(JSON.parse(data.responseText)));
-                }}
-            );
-        }
-
-        (function ($) {
-            $.fn.popmenu = function (options) {
-                var settings = $.extend({
-                    'controller': true,
-                    'width': '300px',
-                    'background': '#34495e',
-                    'focusColor': '#1abc9c',
-                    'borderRadius': '10px',
-                    'top': '50',
-                    'left': '0',
-                    'iconSize': '100px',
-                    'color': '#fff',
-                    'border': '0px'
-                }, options);
-                if (settings.controller === true) {
-                    var temp_display = 'none';
-                } else {
-                    var temp_display = 'block';
-                }
-                var tar = $(this);
-                var tar_body = tar.children('ul');
-                var tar_list = tar_body.children('li');
-                var tar_a = tar_list.children('a');
-                var tar_ctrl = tar.children('.pop_ctrl');
-
-                function setIt() {
-                    tar_body.css({
-                        'display': temp_display,
-                        'position': 'absolute',
-                        'margin-top': -settings.top,
-                        'margin-left': -settings.left,
-                        'background': settings.background,
-                        'padding': '0',
-                        'border-radius': settings.borderRadius,
-                        'border': settings.border
-                    });
-                    tar_list.css({
-                        'padding': '10px',
-                        'display': 'block',
-                        'color': settings.color,
-                        'border-radius': settings.borderRadius
-                    });
-                    tar_a.css({
-                        'text-decoration': 'none',
-                        'color': settings.color
-                    });
-                    tar_ctrl.hover(
-                        function () {
-                            tar_ctrl.css('cursor', 'pointer');
-                        },
-                        function () {
-                            tar_ctrl.css('cursor', 'default')
-                        }
-                    );
-                    tar_ctrl.click(function (e) {
-                        e.preventDefault();
-                        tar_body.show('fast');
-                        $(document).mouseup(function (e) {
-                            var _con = tar_body;
-                            if (!_con.is(e.target) && _con.has(e.target).length === 0) {
-                                _con.hide();
-                            }
-                            //_con.hide(); some functions you want
-                        });
-                    });
-                    tar_list.hover(function () {
-                        $(this).css({
-                            'background': settings.focusColor,
-                            'cursor': 'pointer'
-                        });
-                    }, function () {
-                        $(this).css({
-                            'background': settings.background,
-                            'cursor': 'default'
-                        });
-                    });
-                }
-                return setIt();
-
-            };
-        }(jQuery));
-        $('.schedule_box').each(function () {
-            $(this).popmenu({background: '#79aec8', color: 'black'});
-        });
-    </script>
-{% endblock %}
-
+{% extends "admin/base_site.html" %}
+{% load i18n admin_urls static admin_list %}
+
+{% block extrastyle %}
+  {{ block.super }}
+  <link rel="stylesheet" href="{% static "admin/css/changelists.css" %}">
+  {% if cl.formset %}
+    <link rel="stylesheet" href="{% static "admin/css/forms.css" %}">
+  {% endif %}
+  {% if cl.formset or action_form %}
+    <script src="{% url 'admin:jsi18n' %}"></script>
+  {% endif %}
+  {{ media.css }}
+  {% if not actions_on_top and not actions_on_bottom %}
+    <style>
+      #changelist table thead th:first-child {width: inherit}
+    </style>
+  {% endif %}
+{% endblock %}
+
+
+{% block extrahead %}
+{{ block.super }}
+<script type="text/javascript">window.__admin_media_prefix__ = "{% filter escapejs %}{% static 'admin/' %}{% endfilter %}";</script>
+{{ media.js }}
+<script src="{% static 'admin/js/filters.js' %}" defer></script>
+{% endblock %}
+
+{% block bodyclass %}{{ block.super }} app-{{ opts.app_label }} model-{{ opts.model_name }} change-list{% endblock %}
+
+{% if not is_popup %}
+{% block breadcrumbs %}
+<div class="breadcrumbs">
+<a href="{% url 'admin:index' %}">{% translate 'Home' %}</a>
+&rsaquo; <a href="{% url 'admin:app_list' app_label=cl.opts.app_label %}">{{ cl.opts.app_config.verbose_name }}</a>
+&rsaquo; {{ cl.opts.verbose_name_plural|capfirst }}
+</div>
+{% endblock %}
+{% endif %}
+
+{% block coltype %}{% endblock %}
+
+{% block content %}
+  <div id="option-msg" style="text-align: center; color: red"></div>
+  <div id="content-main">
+    {% block object-tools %}
+        <ul class="object-tools">
+          {% block object-tools-items %}
+            {% change_list_object_tools %}
+          {% endblock %}
+        </ul>
+    {% endblock %}
+    {% if cl.formset and cl.formset.errors %}
+        <p class="errornote">
+        {% if cl.formset.total_error_count == 1 %}{% translate "Please correct the error below." %}{% else %}{% translate "Please correct the errors below." %}{% endif %}
+        </p>
+        {{ cl.formset.non_form_errors }}
+    {% endif %}
+    <div class="module{% if cl.has_filters %} filtered{% endif %}" id="changelist">
+      <div class="changelist-form-container">
+        {% block search %}{% search_form cl %}{% endblock %}
+        {% block date_hierarchy %}{% if cl.date_hierarchy %}{% date_hierarchy cl %}{% endif %}{% endblock %}
+
+        <form id="changelist-form" method="post"{% if cl.formset and cl.formset.is_multipart %} enctype="multipart/form-data"{% endif %} novalidate>{% csrf_token %}
+        {% if cl.formset %}
+          <div>{{ cl.formset.management_form }}</div>
+        {% endif %}
+
+        {% block result_list %}
+          {% if action_form and actions_on_top and cl.show_admin_actions %}{% admin_actions %}{% endif %}
+          {% result_list cl %}
+          {% if action_form and actions_on_bottom and cl.show_admin_actions %}{% admin_actions %}{% endif %}
+        {% endblock %}
+        {% block pagination %}{% pagination cl %}{% endblock %}
+        </form>
+      </div>
+      {% block filters %}
+        {% if cl.has_filters %}
+          <div id="changelist-filter">
+            <h2>{% translate 'Filter' %}</h2>
+            {% if cl.has_active_filters %}<h3 id="changelist-filter-clear">
+              <a href="{{ cl.clear_all_filters_qs }}">&#10006; {% translate "Clear all filters" %}</a>
+            </h3>{% endif %}
+            {% for spec in cl.filter_specs %}{% admin_list_filter cl spec %}{% endfor %}
+          </div>
+        {% endif %}
+      {% endblock %}
+    </div>
+  </div>
+
+    <script>
+        function put_schedule(base_url, schedule_id){
+            const schedule_box = $('#schedule_box_' + schedule_id);
+            let date = schedule_box.find('input[class="vDateField"]').val();
+            let time = schedule_box.find('input[class="vTimeField"]').val();
+            if(date === ""){
+                date = new Date().toLocaleDateString();
+            }
+            if (time === ""){
+                time = new Date().toLocaleTimeString();
+            }
+            if(time.split(':').length === 2){
+                time = time + ':00'
+            }
+            const url = base_url + '&t=' + date.replaceAll('/', '-') + ' ' + time;
+            $.ajax({
+                url: url,
+                dataType: 'json',
+                contentType: 'application/json; charset=utf-8',
+                success: function(data){
+                    $('#option-msg').text("加入成功");
+                    $(document).trigger('mouseup');
+                    setTimeout(function(){
+                        $('#option-msg').text("");
+                    }, 1000);
+                },
+                error: function(data){
+                    console.debug(data);
+                    alert(JSON.stringify(JSON.parse(data.responseText)));
+                }}
+            );
+        }
+
+        (function ($) {
+            $.fn.popmenu = function (options) {
+                var settings = $.extend({
+                    'controller': true,
+                    'width': '300px',
+                    'background': '#34495e',
+                    'focusColor': '#1abc9c',
+                    'borderRadius': '10px',
+                    'top': '50',
+                    'left': '0',
+                    'iconSize': '100px',
+                    'color': '#fff',
+                    'border': '0px'
+                }, options);
+                if (settings.controller === true) {
+                    var temp_display = 'none';
+                } else {
+                    var temp_display = 'block';
+                }
+                var tar = $(this);
+                var tar_body = tar.children('ul');
+                var tar_list = tar_body.children('li');
+                var tar_a = tar_list.children('a');
+                var tar_ctrl = tar.children('.pop_ctrl');
+
+                function setIt() {
+                    tar_body.css({
+                        'display': temp_display,
+                        'position': 'absolute',
+                        'margin-top': -settings.top,
+                        'margin-left': -settings.left,
+                        'background': settings.background,
+                        'padding': '0',
+                        'border-radius': settings.borderRadius,
+                        'border': settings.border
+                    });
+                    tar_list.css({
+                        'padding': '10px',
+                        'display': 'block',
+                        'color': settings.color,
+                        'border-radius': settings.borderRadius
+                    });
+                    tar_a.css({
+                        'text-decoration': 'none',
+                        'color': settings.color
+                    });
+                    tar_ctrl.hover(
+                        function () {
+                            tar_ctrl.css('cursor', 'pointer');
+                        },
+                        function () {
+                            tar_ctrl.css('cursor', 'default')
+                        }
+                    );
+                    tar_ctrl.click(function (e) {
+                        e.preventDefault();
+                        tar_body.show('fast');
+                        $(document).mouseup(function (e) {
+                            var _con = tar_body;
+                            if (!_con.is(e.target) && _con.has(e.target).length === 0) {
+                                _con.hide();
+                            }
+                            //_con.hide(); some functions you want
+                        });
+                    });
+                    tar_list.hover(function () {
+                        $(this).css({
+                            'background': settings.focusColor,
+                            'cursor': 'pointer'
+                        });
+                    }, function () {
+                        $(this).css({
+                            'background': settings.background,
+                            'cursor': 'default'
+                        });
+                    });
+                }
+                return setIt();
+
+            };
+        }(jQuery));
+        $('.schedule_box').each(function () {
+            $(this).popmenu({background: '#79aec8', color: 'black'});
+        });
+    </script>
+{% endblock %}
+
```

### Comparing `django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.2.4/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.2.4/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.2.4/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.2.4/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/urls.py` & `django-common-task-system-1.2.4/django_common_task_system/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.2.4/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.2.4/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.2.4/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.3/django_common_task_system/views.py` & `django-common-task-system-1.2.4/django_common_task_system/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         if not schedule_ids or not queues or not schedule_times:
             return JsonResponse({'error': 'schedule_ids(i)、queues(q)、schedule_times(t)不能为空'},
                                 status=status.HTTP_400_BAD_REQUEST)
         try:
             schedule_ids = [int(i) for i in schedule_ids.split(',')]
             queues = [i.strip() for i in queues.split(',')]
             schedule_times = [datetime.strptime(i, '%Y-%m-%d %H:%M:%S') for i in schedule_times.split(',')]
-            assert len(schedule_ids) < 1000, '不能超过1000个'
+            assert len(schedule_ids) <= 1000, '不能超过1000个'
             if len(queues) == 1:
                 queue_mapping = {x: queues[0] for x in schedule_ids}
             elif len(queues) == len(schedule_ids):
                 queue_mapping = dict(zip(schedule_ids, queues))
             else:
                 raise Exception('ids和queues长度不一致')
             if len(schedule_times) == 1:
@@ -224,26 +224,35 @@
             elif len(schedule_times) == len(schedule_ids):
                 schedule_time_mapping = dict(zip(schedule_ids, schedule_times))
             else:
                 raise Exception('ids和schedule_times长度不一致')
         except Exception as e:
             return JsonResponse({'error': 'ids参数错误: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
         try:
-            schedules = cls.schedule_model.objects.filter(id__in=schedule_ids)
-            result = {x: 'no such schedule' for x in schedule_ids}
-            for schedule in schedules:
-                queue = cls.queues.get(queue_mapping[schedule.id], None)
+            schedules = cls.schedule_model.objects.filter(id__in=set(schedule_ids))
+            schedule_mapping = {x.id: x for x in schedules}
+            result = {}
+            for schedule_id in schedule_ids:
+                queue_name = queue_mapping[schedule_id]
+                queue = cls.queues.get(queue_name, None)
                 if queue is None:
-                    result[schedule.id] = 'no such queue: %s' % queue_mapping[schedule.id]
-                else:
-                    schedule.next_schedule_time = schedule_time_mapping[schedule.id]
-                    data = cls.serializer(schedule).data
-                    data['queue'] = queue_mapping[schedule.id]
-                    queue.queue.put(data)
-                    result[schedule.id] = queue_mapping[schedule.id]
+                    result[queue_name] = 'no such queue: %s' % queue_name
+                    continue
+                schedule_time = schedule_time_mapping[schedule_id].strftime('%Y-%m-%d %H:%M:%S')
+                queue_result = result.setdefault(queue_name, {})
+                schedule = schedule_mapping.get(schedule_id, None)
+                if schedule is None:
+                    queue_result[schedule_id] = 'no such schedule: %s' % schedule_id
+                    continue
+                schedule_result = queue_result.setdefault(schedule_id, [])
+                schedule.next_schedule_time = schedule_time
+                data = cls.serializer(schedule).data
+                data['queue'] = queue.code
+                queue.queue.put(data)
+                schedule_result.append(schedule_time)
             return JsonResponse(result)
         except Exception as e:
             return JsonResponse({'error': '添加到队列失败: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
 
     @staticmethod
     @api_view(['GET'])
     def status(request):
```

### Comparing `django-common-task-system-1.2.3/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.2.4/django_common_task_system.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 MANIFEST.in
 README.md
 setup.py
 django_common_task_system/__init__.py
 django_common_task_system/admin.py
 django_common_task_system/apps.py
 django_common_task_system/choices.py
```

### Comparing `django-common-task-system-1.2.3/setup.py` & `django-common-task-system-1.2.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests']),
-    version='1.2.3',
+    version='1.2.4',
     install_requires=[
         "django-common-objects>=1.0.5",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
```


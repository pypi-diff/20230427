# Comparing `tmp/elementary-data-0.7.7.tar.gz` & `tmp/elementary-data-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-jrikyhh6/elementary-data-0.7.7.tar", last modified: Tue Apr 11 12:53:07 2023, max compression
+gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-en32z20k/elementary-data-0.7.8.tar", last modified: Thu Apr 27 12:29:21 2023, max compression
```

## Comparing `elementary-data-0.7.7.tar` & `elementary-data-0.7.8.tar`

### file list

```diff
@@ -1,277 +1,289 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-04-11 12:52:52.000000 elementary-data-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-11 12:52:52.000000 elementary-data-0.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14153 2023-04-11 12:53:07.000000 elementary-data-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13274 2023-04-11 12:52:52.000000 elementary-data-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/cli/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/dbt/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/dbt/base_dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     7958 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/dbt/dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     5188 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/dbt/slim_dbt_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/fetcher/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/fetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/fetcher/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/gcs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/gcs/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/s3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/s3/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/clients/slack/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7387 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/slack/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/slack/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5552 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/clients/slack/slack_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4116 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)    12920 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/group_of_alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/malformed.py
--rw-r--r--   0 runner    (1001) docker     (122)     7697 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/alerts/schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/schema/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/schema/alert_group_component.py
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/schema/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/source_freshness.py
--rw-r--r--   0 runner    (1001) docker     (122)    15821 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/alerts/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4854 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/alerts/alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     7762 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/alerts/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4067 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/filters/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8094 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6692 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/report/report.py
--rw-r--r--   0 runner    (1001) docker     (122)      602 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/report/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/sidebar/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/sidebar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/sidebar/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/sidebar/sidebar.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    19501 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/api/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)    19322 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6175 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/data_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    10127 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/data_monitoring_alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11666 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/report/data_monitoring_report.py
--rw-r--r--   0 runner    (1001) docker     (122)  1674955 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/report/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     4191 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/data_monitoring/selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)     7646 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/base_queries/
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_exposures.sql
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_models_runs.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_sources.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     5345 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_results.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/test_conn.sql
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/packages.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/dbt_project_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     5125 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/alerts/normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/base_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/monitor/fetchers/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/monitor/fetchers/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/operations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/operations/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/operations/upload_source_freshness.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/tracking/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6159 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/tracking/anonymous_tracking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/tracking/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/tracking/tracking_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/bucket_path.py
--rw-r--r--   0 runner    (1001) docker     (122)      934 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/ordered_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-04-11 12:52:52.000000 elementary-data-0.7.7/elementary/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14153 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9291 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-11 12:53:07.000000 elementary-data-0.7.7/elementary_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 12:53:07.000000 elementary-data-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-04-11 12:52:52.000000 elementary-data-0.7.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/integration/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/integration/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/integration/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/integration/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/integration/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/anonymous_tracking_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/mocks/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/api/alerts_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/api/invocations_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/api/tests_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/dbt_runner_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/mocks/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/fetchers/alerts_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/fetchers/invocations_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/fetchers/selector_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/mocks/fetchers/tests_fetcher_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12236 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/test_malformed_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7565 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/test_normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7348 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/alerts/test_alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1919 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/alerts/test_alerts_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8825 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/data_monitoring/test_selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:53:07.000000 elementary-data-0.7.7/tests/unit/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-04-11 12:52:52.000000 elementary-data-0.7.7/tests/unit/monitor/fetchers/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-04-27 12:29:03.000000 elementary-data-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-27 12:29:03.000000 elementary-data-0.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14291 2023-04-27 12:29:21.000000 elementary-data-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-04-27 12:29:03.000000 elementary-data-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/cli/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/api/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/dbt/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/dbt/base_dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7958 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/dbt/dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5188 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/dbt/slim_dbt_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/fetcher/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/fetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/fetcher/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/gcs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/gcs/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/s3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/s3/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/slack/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7387 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/slack/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/slack/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5552 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/slack/slack_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4116 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12986 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/group_of_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/malformed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7697 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/alerts/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/schema/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/schema/alert_group_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/schema/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/source_freshness.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15821 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4854 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/alerts/alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7770 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/alerts/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4067 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/filters/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8094 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6692 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (122)      602 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/report/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/sidebar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/sidebar/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/sidebar/sidebar.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/test_management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/test_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/test_management/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/test_management/test_management.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19501 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19321 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6175 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/data_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10139 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/data_monitoring_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11666 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/report/data_monitoring_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)  1674955 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/report/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4191 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     7646 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/owners.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     2471 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/resources.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/tags.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/tests.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_exposures.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_models_runs.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_sources.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     5345 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_results.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/test_conn.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/packages.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5125 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/alerts/normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/base_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2362 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/test_management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/test_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/test_management/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6135 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/test_management/test_management.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/operations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/operations/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/operations/upload_source_freshness.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/tracking/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6159 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/tracking/anonymous_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/tracking/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/tracking/tracking_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/bucket_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)      934 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/ordered_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14291 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9870 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-27 12:29:21.000000 elementary-data-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-04-27 12:29:03.000000 elementary-data-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/integration/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/integration/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/integration/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/integration/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/anonymous_tracking_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/mocks/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/api/alerts_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/api/invocations_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/api/tests_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/dbt_runner_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/mocks/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/fetchers/alerts_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/fetchers/invocations_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/fetchers/selector_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/fetchers/tests_fetcher_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12236 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/test_malformed_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7565 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/test_normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7348 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/alerts/test_alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1919 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/alerts/test_alerts_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/test_selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/fetchers/test_alerts_fetcher.py
```

### Comparing `elementary-data-0.7.7/LICENSE` & `elementary-data-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/PKG-INFO` & `elementary-data-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.7.7
+Version: 0.7.8
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -198,12 +198,13 @@
 <a href="https://github.com/andreqaugusto"><img src="https://avatars.githubusercontent.com/u/68784205?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/tc-chrisbui"><img src="https://avatars.githubusercontent.com/u/115048867?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vishaalkk"><img src="https://avatars.githubusercontent.com/u/13641827?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/sadahry"><img src="https://avatars.githubusercontent.com/u/28292300?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/dimoschi"><img src="https://avatars.githubusercontent.com/u/13113025?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.7.7 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.7.8 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `elementary-data-0.7.7/README.md` & `elementary-data-0.7.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -172,12 +172,13 @@
 <a href="https://github.com/andreqaugusto"><img src="https://avatars.githubusercontent.com/u/68784205?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/tc-chrisbui"><img src="https://avatars.githubusercontent.com/u/115048867?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vishaalkk"><img src="https://avatars.githubusercontent.com/u/13641827?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/sadahry"><img src="https://avatars.githubusercontent.com/u/28292300?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/dimoschi"><img src="https://avatars.githubusercontent.com/u/13113025?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `elementary-data-0.7.7/elementary/cli/cli.py` & `elementary-data-0.7.8/elementary/cli/cli.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/cli/upgrade.py` & `elementary-data-0.7.8/elementary/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/clients/dbt/base_dbt_runner.py` & `elementary-data-0.7.8/elementary/clients/dbt/base_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/clients/dbt/dbt_runner.py` & `elementary-data-0.7.8/elementary/clients/dbt/dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/clients/dbt/slim_dbt_runner.py` & `elementary-data-0.7.8/elementary/clients/dbt/slim_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/clients/gcs/client.py` & `elementary-data-0.7.8/elementary/clients/gcs/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/clients/s3/client.py` & `elementary-data-0.7.8/elementary/clients/s3/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/clients/slack/client.py` & `elementary-data-0.7.8/elementary/clients/slack/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/clients/slack/schema.py` & `elementary-data-0.7.8/elementary/clients/slack/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/clients/slack/slack_message_builder.py` & `elementary-data-0.7.8/elementary/clients/slack/slack_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/config/config.py` & `elementary-data-0.7.8/elementary/config/config.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/exceptions/exceptions.py` & `elementary-data-0.7.8/elementary/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/alerts/alert.py` & `elementary-data-0.7.8/elementary/monitor/alerts/alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/alerts/alerts.py` & `elementary-data-0.7.8/elementary/monitor/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/alerts/group_of_alerts.py` & `elementary-data-0.7.8/elementary/monitor/alerts/group_of_alerts.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,15 +320,15 @@
             self.channel_destination = self.alerts[0].slack_channel
         else:
             self.channel_destination = default_channel
 
     def to_slack(self):
         return self.alerts[0].to_slack()
 
-    def set_owners(self, owners):
-        self.alerts[0].owners = owners
+    def set_owners(self, owners: List[str]):
+        self.alerts[0].owners = ", ".join(owners)
 
-    def set_subscribers(self, subscribers):
-        self.alerts[0].subscribers = subscribers
+    def set_subscribers(self, subscribers: List[str]):
+        self.alerts[0].subscribers = ", ".join(subscribers)
 
-    def set_tags(self, tags):
-        self.alerts[0].tags = tags
+    def set_tags(self, tags: List[str]):
+        self.alerts[0].tags = ", ".join(tags)
```

### Comparing `elementary-data-0.7.7/elementary/monitor/alerts/malformed.py` & `elementary-data-0.7.8/elementary/monitor/alerts/malformed.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/alerts/model.py` & `elementary-data-0.7.8/elementary/monitor/alerts/model.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/alerts/source_freshness.py` & `elementary-data-0.7.8/elementary/monitor/alerts/source_freshness.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/alerts/test.py` & `elementary-data-0.7.8/elementary/monitor/alerts/test.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/alerts/alert_filters.py` & `elementary-data-0.7.8/elementary/monitor/api/alerts/alert_filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/alerts/alerts.py` & `elementary-data-0.7.8/elementary/monitor/api/alerts/alerts.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             suppression_interval = alert.alert_suppression_interval
             last_sent_time = (
                 datetime.fromisoformat(last_alert_sent_times.get(alert_class_id))
                 if last_alert_sent_times.get(alert_class_id)
                 else None
             )
             is_alert_in_suppression = (
-                (current_time_utc - last_sent_time).seconds / 3600
+                (current_time_utc - last_sent_time).total_seconds() / 3600
                 <= suppression_interval
                 if last_sent_time
                 else False
             )
             if is_alert_in_suppression:
                 suppressed_alerts.append(alert.id)
```

### Comparing `elementary-data-0.7.7/elementary/monitor/api/filters/filters.py` & `elementary-data-0.7.8/elementary/monitor/api/filters/filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/filters/schema.py` & `elementary-data-0.7.8/elementary/monitor/api/filters/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/invocations/invocations.py` & `elementary-data-0.7.8/elementary/monitor/api/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/lineage/lineage.py` & `elementary-data-0.7.8/elementary/monitor/api/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/lineage/schema.py` & `elementary-data-0.7.8/elementary/monitor/api/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/models/models.py` & `elementary-data-0.7.8/elementary/monitor/api/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/models/schema.py` & `elementary-data-0.7.8/elementary/monitor/api/models/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/report/report.py` & `elementary-data-0.7.8/elementary/monitor/api/report/report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/report/schema.py` & `elementary-data-0.7.8/elementary/monitor/api/report/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/selector/selector.py` & `elementary-data-0.7.8/elementary/monitor/api/selector/selector.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/sidebar/sidebar.py` & `elementary-data-0.7.8/elementary/monitor/api/sidebar/sidebar.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/tests/schema.py` & `elementary-data-0.7.8/elementary/monitor/api/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/api/tests/tests.py` & `elementary-data-0.7.8/elementary/monitor/api/tests/tests.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/cli.py` & `elementary-data-0.7.8/elementary/monitor/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         )(func)
         func = click.option(
             "--profile-target",
             "-t",
             type=str,
             default=None,
             help="Which target to load for the given profile. "
-            "If specified, the target will be used for both the 'elementary' profile and your dbt project."
+            "If specified, the target will be used for both the 'elementary' profile and your dbt project. "
             "Else, the default target will be used.",
         )(func)
         func = click.option(
             "--profiles-dir",
             "-p",
             type=click.Path(exists=True),
             default=None,
@@ -129,15 +129,15 @@
             help="Which directory to look in for the dbt_project.yml file. Default is the current working directory.",
         )(func)
         func = click.option(
             "--project-profile-target",
             type=str,
             default=None,
             help="Which target to load for the given profile. "
-            "If specified, the target will be used for your dbt project."
+            "If specified, the target will be used for your dbt project. "
             "Else, the --profile-target will be used.",
         )(func)
         func = click.option(
             "--select",
             type=str,
             default=None,
             help="Filter the report by last_invocation / invocation_id:<INVOCATION_ID> / invocation_time:<INVOCATION_TIME>."
@@ -213,15 +213,15 @@
     type=bool,
     default=False,
     help="Whether to send a test message in case there are no alerts.",
 )
 @click.option(
     "--group-by",
     type=click.Choice(["alert", "table"]),
-    default="alert",
+    default=None,
     help="Whether to group alerts by 'alert' or by 'table'",
 )
 @click.pass_context
 def monitor(
     ctx,
     days_back,
     slack_webhook,
```

### Comparing `elementary-data-0.7.7/elementary/monitor/data_monitoring/data_monitoring.py` & `elementary-data-0.7.8/elementary/monitor/data_monitoring/data_monitoring.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/data_monitoring/data_monitoring_alerts.py` & `elementary-data-0.7.8/elementary/monitor/data_monitoring/data_monitoring_alerts.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,16 +84,16 @@
             alert.owners = self._parse_emails_to_ids(alert.owners)
             alert.subscribers = self._parse_emails_to_ids(alert.subscribers)
         all_owners = set([])
         all_subscribers = set([])
         for alert in group_alert.alerts:
             all_owners.update(alert.owners)
             all_subscribers.update(alert.subscribers)
-        group_alert.set_owners(all_owners)
-        group_alert.set_subscribers(all_subscribers)
+        group_alert.set_owners(list(all_owners))
+        group_alert.set_subscribers(list(all_subscribers))
 
     def _group_alerts_per_config(self, alerts: List[Alert]) -> List[GroupOfAlerts]:
         """
         reads self.config and alerts' config, and groups alerts in a smart way
         1. split by grouping type
         2. split Table grouped-by, by the Table
         3. concat
```

### Comparing `elementary-data-0.7.7/elementary/monitor/data_monitoring/report/data_monitoring_report.py` & `elementary-data-0.7.8/elementary/monitor/data_monitoring/report/data_monitoring_report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/data_monitoring/report/index.html` & `elementary-data-0.7.8/elementary/monitor/data_monitoring/report/index.html`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py` & `elementary-data-0.7.8/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,69 +17,42 @@
         test_results: List[TestResultSummarySchema],
         env: str,
         days_back: int,
         bucket_website_url: Optional[str] = None,
         filter: SelectorFilterSchema = SelectorFilterSchema(),
         include_description: bool = False,
     ) -> SlackMessageSchema:
-        self._add_title_to_slack_alert(
-            test_results=test_results,
-            bucket_website_url=bucket_website_url,
+        self._add_title_to_slack_alert(env=env)
+        self._add_preview_to_slack_alert(
+            test_results,
             days_back=days_back,
-            env=env,
+            bucket_website_url=bucket_website_url,
             filter=filter,
         )
-        self._add_preview_to_slack_alert(test_results)
         self._add_details_to_slack_alert(
             test_results=test_results,
             include_description=include_description,
             bucket_website_url=bucket_website_url,
         )
         return super().get_slack_message()
 
     def _add_title_to_slack_alert(
         self,
-        test_results: List[TestResultSummarySchema],
         env: str,
-        days_back: int,
-        bucket_website_url: Optional[str] = None,
-        filter: SelectorFilterSchema = SelectorFilterSchema(),
     ):
         env_text = (
             ":construction: Development"
             if env == "dev"
             else ":large_green_circle: Production"
         )
-        summary_filter_text = self._get_summary_filter_text(days_back, filter)
-        totals = self._get_test_results_totals(test_results)
 
         title_blocks = [
             self.create_header_block(f":mag: Monitoring summary ({env_text})"),
-            self.create_text_section_block(summary_filter_text),
+            self.create_divider_block(),
         ]
-
-        if bucket_website_url:
-            title_blocks.append(
-                self.create_text_section_block(
-                    f"<{bucket_website_url}|View full report> :arrow_upper_right:"
-                )
-            )
-
-        title_blocks.append(
-            self.create_fields_section_block(
-                [
-                    f":white_check_mark: Passed: {totals.get('passed', 0)}",
-                    f":small_red_triangle: Failed: {totals.get('failed', 0)}",
-                    f":exclamation: Errors: {totals.get('error', 0)}",
-                    f":Warning: Warning: {totals.get('warning', 0)}",
-                ]
-            )
-        )
-
-        title_blocks.append(self.create_divider_block())
         self._add_always_displayed_blocks(title_blocks)
 
     @staticmethod
     def _get_summary_filter_text(
         days_back: int,
         filter: SelectorFilterSchema = SelectorFilterSchema(),
     ) -> str:
@@ -92,45 +65,50 @@
             selector_text = f"owner: {filter.owner}"
         days_back_text = (
             f"timeframe: {days_back} day{'s' if days_back > 1 else ''} back"
         )
 
         return f"_This summary was generated with the following filters - {days_back_text}{f', {selector_text}' if selector_text else ''}_"
 
-    def _add_preview_to_slack_alert(self, test_results: List[TestResultSummarySchema]):
-        owners = []
-        tags = []
-        subscribers = []
-        for test in test_results:
-            if test.status != "pass":
-                formatted_tags = [
-                    tag if tag.startswith(TAG_PREFIX) else f"{TAG_PREFIX}{tag}"
-                    for tag in test.tags
+    def _add_preview_to_slack_alert(
+        self,
+        test_results: List[TestResultSummarySchema],
+        days_back: int,
+        filter: SelectorFilterSchema = SelectorFilterSchema(),
+        bucket_website_url: Optional[str] = None,
+    ):
+        preview_blocks = []
+
+        summary_filter_text = self._get_summary_filter_text(days_back, filter)
+        preview_blocks.append(self.create_text_section_block(summary_filter_text))
+
+        if bucket_website_url:
+            preview_blocks.append(
+                self.create_text_section_block(
+                    f"<{bucket_website_url}|View full report> :arrow_upper_right:"
+                )
+            )
+
+        totals = self._get_test_results_totals(test_results)
+        preview_blocks.append(
+            self.create_fields_section_block(
+                [
+                    f":white_check_mark: Passed: {totals.get('passed', 0)}",
+                    f":small_red_triangle: Failed: {totals.get('failed', 0)}",
+                    f":exclamation: Errors: {totals.get('error', 0)}",
+                    f":Warning: Warning: {totals.get('warning', 0)}",
                 ]
-                owners.extend(test.owners)
-                tags.extend(formatted_tags)
-                subscribers.extend(test.subscribers)
-
-        tags_text = self.prettify_and_dedup_list(tags) if tags else "_No tags_"
-        owners_text = self.prettify_and_dedup_list(owners) if owners else "_No owners_"
-        subscribers_text = (
-            self.prettify_and_dedup_list(subscribers)
-            if subscribers
-            else "_No subscribers_"
-        )
-
-        preview_blocks = [
-            self.create_text_section_block(":mega: *Attention required* :mega:"),
-            self.create_text_section_block(f"*Tags:* {tags_text}"),
-            self.create_text_section_block(f"*Owners:* {owners_text}"),
-            self.create_text_section_block(f"*Subscribers:* {subscribers_text}"),
-            self.create_empty_section_block(),
-        ]
-        if preview_blocks:
-            self._add_blocks_as_attachments(preview_blocks)
+            )
+        )
+
+        preview_blocks_filler = [self.create_empty_section_block()] * (
+            self._MAX_ALERT_PREVIEW_BLOCKS - len(preview_blocks)
+        )
+        preview_blocks.extend(preview_blocks_filler)
+        self._add_blocks_as_attachments(preview_blocks)
 
     def _add_details_to_slack_alert(
         self,
         test_results: List[TestResultSummarySchema],
         include_description: bool = False,
         bucket_website_url: Optional[str] = None,
     ):
```

### Comparing `elementary-data-0.7.7/elementary/monitor/data_monitoring/schema.py` & `elementary-data-0.7.8/elementary/monitor/data_monitoring/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/data_monitoring/selector_filter.py` & `elementary-data-0.7.8/elementary/monitor/data_monitoring/selector_filter.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/README.md` & `elementary-data-0.7.8/elementary/monitor/dbt_project/README.md`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/dbt_project.yml` & `elementary-data-0.7.8/elementary/monitor/dbt_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_exposures.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_exposures.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_latest_invocation.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_latest_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_models.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_models_runs.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_models_runs.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_sources.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_sources.sql`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     {% set dbt_sources_relation = ref('elementary', 'dbt_sources') %}
     {%- if elementary.relation_exists(dbt_sources_relation) -%}
         --{# TODO: should we group by #}
         {% set get_sources_query %}
             with dbt_artifacts_sources as (
                 select
                   name,
+                  source_name,
                   unique_id,
                   database_name,
                   schema_name,
                   identifier as table_name,
                   owner as owners,
                   tags,
                   package_name,
```

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_results.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_results.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/materializations/incremental.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/macros/materializations/table.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts_models.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql` & `elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/dbt_project_utils.py` & `elementary-data-0.7.8/elementary/monitor/dbt_project_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/debug.py` & `elementary-data-0.7.8/elementary/monitor/debug.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/fetchers/alerts/alerts.py` & `elementary-data-0.7.8/elementary/monitor/fetchers/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/fetchers/alerts/normalized_alert.py` & `elementary-data-0.7.8/elementary/monitor/fetchers/alerts/normalized_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/fetchers/invocations/invocations.py` & `elementary-data-0.7.8/elementary/monitor/fetchers/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/fetchers/invocations/schema.py` & `elementary-data-0.7.8/elementary/monitor/fetchers/invocations/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/fetchers/lineage/lineage.py` & `elementary-data-0.7.8/elementary/monitor/fetchers/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/fetchers/lineage/schema.py` & `elementary-data-0.7.8/elementary/monitor/fetchers/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/fetchers/models/models.py` & `elementary-data-0.7.8/elementary/monitor/fetchers/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/fetchers/models/schema.py` & `elementary-data-0.7.8/elementary/monitor/fetchers/models/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import posixpath
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 
 from pydantic import Field, validator
 
 from elementary.utils.schema import ExtendedBaseModel
 from elementary.utils.time import convert_partial_iso_format_to_full_iso_format
 
 
@@ -28,14 +28,15 @@
     name: Optional[str] = None
     unique_id: Optional[str] = None
     owners: Optional[List[str]] = None
     tags: Optional[List[str]] = None
     package_name: Optional[str] = None
     description: Optional[str] = None
     full_path: Optional[str] = None
+    meta: Optional[Dict[str, Any]] = None
 
     @validator("tags", pre=True)
     def load_tags(cls, tags):
         return cls._load_var_to_list(tags)
 
     @validator("owners", pre=True)
     def load_owners(cls, owners):
@@ -46,29 +47,40 @@
         return posixpath.sep.join(full_path.split(os.path.sep))
 
 
 class ModelSchema(ArtifactSchema):
     database_name: Optional[str] = None
     schema_name: str
     table_name: str
-    ref_function: str = "ref"
+
+    def ref(self):
+        return f"ref('{self.name}')"
 
 
 class SourceSchema(ArtifactSchema):
+    source_name: Optional[str] = None
     database_name: Optional[str] = None
     schema_name: str
     table_name: str
-    ref_function: str = "source"
+
+    def ref(self):
+        return f"source('{self.source_name}', '{self.table_name}')"
+
+
+class OwnerSchema(ExtendedBaseModel):
+    name: Optional[str] = None
+    email: Optional[str] = None
 
 
 class ExposureSchema(ArtifactSchema):
+    label: Optional[str] = None
     url: Optional[str] = None
     type: Optional[str] = None
     maturity: Optional[str] = None
-    owner_email: Optional[str] = None
     depends_on: Optional[List[str]] = None
+    owner: Optional[OwnerSchema] = None
 
 
 class ModelTestCoverage(ExtendedBaseModel):
     model_unique_id: Optional[str] = None
     column_tests: int = 0
     table_tests: int = 0
```

### Comparing `elementary-data-0.7.7/elementary/monitor/fetchers/tests/schema.py` & `elementary-data-0.7.8/elementary/monitor/fetchers/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/monitor/fetchers/tests/tests.py` & `elementary-data-0.7.8/elementary/monitor/fetchers/tests/tests.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/operations/cli.py` & `elementary-data-0.7.8/elementary/operations/cli.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/operations/upload_source_freshness.py` & `elementary-data-0.7.8/elementary/operations/upload_source_freshness.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/tracking/anonymous_tracking.py` & `elementary-data-0.7.8/elementary/tracking/anonymous_tracking.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/tracking/runner.py` & `elementary-data-0.7.8/elementary/tracking/runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/tracking/tracking_interface.py` & `elementary-data-0.7.8/elementary/tracking/tracking_interface.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/utils/cli_utils.py` & `elementary-data-0.7.8/elementary/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/utils/json_utils.py` & `elementary-data-0.7.8/elementary/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/utils/log.py` & `elementary-data-0.7.8/elementary/utils/log.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/utils/ordered_yaml.py` & `elementary-data-0.7.8/elementary/utils/ordered_yaml.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/utils/package.py` & `elementary-data-0.7.8/elementary/utils/package.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/utils/schema.py` & `elementary-data-0.7.8/elementary/utils/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary/utils/time.py` & `elementary-data-0.7.8/elementary/utils/time.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/elementary_data.egg-info/PKG-INFO` & `elementary-data-0.7.8/elementary_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.7.7
+Version: 0.7.8
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -198,12 +198,13 @@
 <a href="https://github.com/andreqaugusto"><img src="https://avatars.githubusercontent.com/u/68784205?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/tc-chrisbui"><img src="https://avatars.githubusercontent.com/u/115048867?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vishaalkk"><img src="https://avatars.githubusercontent.com/u/13641827?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/sadahry"><img src="https://avatars.githubusercontent.com/u/28292300?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/dimoschi"><img src="https://avatars.githubusercontent.com/u/13113025?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.7.7 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.7.8 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `elementary-data-0.7.7/elementary_data.egg-info/SOURCES.txt` & `elementary-data-0.7.8/elementary_data.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 elementary/monitor/api/report/schema.py
 elementary/monitor/api/selector/__init__.py
 elementary/monitor/api/selector/schema.py
 elementary/monitor/api/selector/selector.py
 elementary/monitor/api/sidebar/__init__.py
 elementary/monitor/api/sidebar/schema.py
 elementary/monitor/api/sidebar/sidebar.py
+elementary/monitor/api/test_management/__init__.py
+elementary/monitor/api/test_management/schema.py
+elementary/monitor/api/test_management/test_management.py
 elementary/monitor/api/tests/__init__.py
 elementary/monitor/api/tests/schema.py
 elementary/monitor/api/tests/tests.py
 elementary/monitor/data_monitoring/__init__.py
 elementary/monitor/data_monitoring/data_monitoring.py
 elementary/monitor/data_monitoring/data_monitoring_alerts.py
 elementary/monitor/data_monitoring/schema.py
@@ -107,14 +110,18 @@
 elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
 elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
 elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
 elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
 elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
 elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
 elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
+elementary/monitor/dbt_project/macros/base_queries/owners.sql
+elementary/monitor/dbt_project/macros/base_queries/resources.sql
+elementary/monitor/dbt_project/macros/base_queries/tags.sql
+elementary/monitor/dbt_project/macros/base_queries/tests.sql
 elementary/monitor/dbt_project/macros/materializations/incremental.sql
 elementary/monitor/dbt_project/macros/materializations/table.sql
 elementary/monitor/dbt_project/models/alerts/alerts.sql
 elementary/monitor/dbt_project/models/alerts/alerts_models.sql
 elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
 elementary/monitor/dbt_project/snapshots/.gitkeep
 elementary/monitor/dbt_project/tests/.gitkeep
@@ -131,14 +138,17 @@
 elementary/monitor/fetchers/lineage/schema.py
 elementary/monitor/fetchers/models/__init__.py
 elementary/monitor/fetchers/models/models.py
 elementary/monitor/fetchers/models/schema.py
 elementary/monitor/fetchers/selector/__init__.py
 elementary/monitor/fetchers/selector/schema.py
 elementary/monitor/fetchers/selector/selector.py
+elementary/monitor/fetchers/test_management/__init__.py
+elementary/monitor/fetchers/test_management/schema.py
+elementary/monitor/fetchers/test_management/test_management.py
 elementary/monitor/fetchers/tests/__init__.py
 elementary/monitor/fetchers/tests/schema.py
 elementary/monitor/fetchers/tests/tests.py
 elementary/operations/__init__.py
 elementary/operations/cli.py
 elementary/operations/upload_source_freshness.py
 elementary/tracking/__init__.py
```

### Comparing `elementary-data-0.7.7/elementary_data.egg-info/requires.txt` & `elementary-data-0.7.8/elementary_data.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/setup.py` & `elementary-data-0.7.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "spark": ["dbt-spark>=0.20,<2.0.0", "dbt-spark[PyHive]>=0.20,<2.0.0"],
 }
 
 
 setup(
     name="elementary-data",
     description="Data monitoring and lineage",
-    version="0.7.7",
+    version="0.7.8",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6.2",
     entry_points="""
         [console_scripts]
         edr=elementary.cli.cli:cli
     """,
```

### Comparing `elementary-data-0.7.7/tests/integration/monitor/api/alerts/test_alerts_fetcher.py` & `elementary-data-0.7.8/tests/integration/monitor/api/alerts/test_alerts_fetcher.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/integration/monitor/api/tests/test_tests_api.py` & `elementary-data-0.7.8/tests/integration/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/mocks/api/alerts_api_mock.py` & `elementary-data-0.7.8/tests/mocks/api/alerts_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/mocks/api/tests_api_mock.py` & `elementary-data-0.7.8/tests/mocks/api/tests_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/mocks/fetchers/alerts_fetcher_mock.py` & `elementary-data-0.7.8/tests/mocks/fetchers/alerts_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/mocks/fetchers/tests_fetcher_mock.py` & `elementary-data-0.7.8/tests/mocks/fetchers/tests_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py` & `elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py` & `elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py` & `elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/alerts/group_alerts_by_table/utils.py` & `elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/alerts/test_malformed_alert.py` & `elementary-data-0.7.8/tests/unit/monitor/alerts/test_malformed_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/alerts/test_normalized_alert.py` & `elementary-data-0.7.8/tests/unit/monitor/alerts/test_normalized_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/alerts/test_slack_alert_message_builder.py` & `elementary-data-0.7.8/tests/unit/monitor/alerts/test_slack_alert_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/api/alerts/test_alert_filters.py` & `elementary-data-0.7.8/tests/unit/monitor/api/alerts/test_alert_filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/api/alerts/test_alerts_api.py` & `elementary-data-0.7.8/tests/unit/monitor/api/alerts/test_alerts_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/api/tests/test_tests_api.py` & `elementary-data-0.7.8/tests/unit/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py` & `elementary-data-0.7.8/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,43 +48,20 @@
     )
     attachments_as_string = json.dumps(
         message_builder.slack_message.get("attachments")[0].get("blocks")
     )
     assert "The amount of results exceeded Slack" in attachments_as_string
 
 
-def test_owners_tags_and_subscribers_of_passed_tests_are_filtered_out(
-    test_results_summary,
-):
-    # Within attachments limitation
-    message_builder = SlackReportSummaryMessageBuilder()
-    message_builder._add_preview_to_slack_alert(test_results_summary)
-    attachments_as_string = json.dumps(
-        message_builder.slack_message.get("attachments")[0].get("blocks")
-    )
-    assert "Jeff" in attachments_as_string
-    assert "Joe" in attachments_as_string
-    assert "Ron" in attachments_as_string
-    assert "subscriber1" in attachments_as_string
-    assert "subscriber2" in attachments_as_string
-    assert "production" in attachments_as_string
-    assert "dev" in attachments_as_string
-
-    assert "Jack" not in attachments_as_string
-    assert "subscriber22" not in attachments_as_string
-    assert "staging" not in attachments_as_string
-
-
 def test_passed_tests_filtered_out_of_details_view(
     test_results_summary,
 ):
     # Within attachments limitation
     message_builder = SlackReportSummaryMessageBuilder()
     passed_tests_from_fixture = [x for x in test_results_summary if x.status == "pass"]
-    message_builder._add_preview_to_slack_alert(passed_tests_from_fixture)
     message_builder._add_details_to_slack_alert(passed_tests_from_fixture)
     attachments_as_string = json.dumps(
         message_builder.slack_message.get("attachments")[0].get("blocks")
     )
     assert "Warning" not in attachments_as_string
     assert "*table_3* | first_test" not in attachments_as_string
```

### Comparing `elementary-data-0.7.7/tests/unit/monitor/data_monitoring/test_selector_filter.py` & `elementary-data-0.7.8/tests/unit/monitor/data_monitoring/test_selector_filter.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.7/tests/unit/monitor/fetchers/test_alerts_fetcher.py` & `elementary-data-0.7.8/tests/unit/monitor/fetchers/test_alerts_fetcher.py`

 * *Files identical despite different names*


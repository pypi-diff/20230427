# Comparing `tmp/bemserver-ui-0.5.0.tar.gz` & `tmp/bemserver-ui-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bemserver-ui-0.5.0.tar", last modified: Thu Mar 30 12:26:35 2023, max compression
+gzip compressed data, was "bemserver-ui-0.5.1.tar", last modified: Thu Apr 27 15:02:13 2023, max compression
```

## Comparing `bemserver-ui-0.5.0.tar` & `bemserver-ui-0.5.1.tar`

### file list

```diff
@@ -1,301 +1,312 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.636454 bemserver-ui-0.5.0/bemserver_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.640455 bemserver-ui-0.5.0/bemserver_ui/common/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/common/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/common/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/common/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.640455 bemserver-ui-0.5.0/bemserver_ui/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/campaign_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/flask_es6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/jinja_custom_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/partners.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.640455 bemserver-ui-0.5.0/bemserver_ui/extensions/timezones/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/timezones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66289 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/timezones/timezones-areas.json
--rw-r--r--   0 runner    (1001) docker     (123)   224723 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/timezones/timezones-full.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/timezones/timezones-regions.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/extensions/timezones/timezones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.640455 bemserver-ui-0.5.0/bemserver_ui/internal_api/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.640455 bemserver-ui-0.5.0/bemserver_ui/internal_api/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/analysis/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/analysis/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/campaign_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.640455 bemserver-ui-0.5.0/bemserver_ui/internal_api/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.640455 bemserver-ui-0.5.0/bemserver_ui/internal_api/semantics/energy/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/semantics/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/semantics/energy/consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/semantics/energy/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/semantics/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.640455 bemserver-ui-0.5.0/bemserver_ui/internal_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/services/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/services/missing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/services/outlier_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/structural_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.644455 bemserver-ui-0.5.0/bemserver_ui/internal_api/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/timeseries/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/timeseries/datastates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/timeseries/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/internal_api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.636454 bemserver-ui-0.5.0/bemserver_ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.644455 bemserver-ui-0.5.0/bemserver_ui/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/images/bemserver-ico.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/images/bemserver-min.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/images/bemserver.ico
--rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/images/bemserver.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.644455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.644455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.644455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/accordionList.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.644455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
--rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/dropZone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/eventLevel.js
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/filterSelect.js
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/flash.js
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/itemsCount.js
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/modalConfirm.js
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/pagination.js
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/spinner.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.644455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/structuralElements/
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.644455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/time/
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/time/tzPicker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.644455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
--rw-r--r--   0 runner    (1001) docker     (123)    32394 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/timeseries/selector.js
--rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/tree.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/userGroup/
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/flashTimer.js
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/formController.js
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/notifications.js
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/sidebar.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/array.js
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/dict.js
--rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/fetcher.js
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/flaskES6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/parser.js
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/time.js
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/uuid.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.636454 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/campaignScopes/
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/campaigns/selector.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/events/
--rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/events/edit.js
--rw-r--r--   0 runner    (1001) docker     (123)    45177 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/events/list.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)    66390 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/notifications/explore.js
--rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/notifications/setup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/missingData/
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/missingData/list.js
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/outlierData/
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/structuralElements/
--rw-r--r--   0 runner    (1001) docker     (123)    26818 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.648455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js
--rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/delete.js
--rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/list.js
--rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js
--rw-r--r--   0 runner    (1001) docker     (123)    52668 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.652455 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/users/list.js
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/users/manageGroups.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.652455 bemserver-ui-0.5.0/bemserver_ui/static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/styles/app.css
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/styles/dragndrop.css
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/styles/main.css
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/styles/signin.css
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/static/styles/tree.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.636454 bemserver-ui-0.5.0/bemserver_ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.652455 bemserver-ui-0.5.0/bemserver_ui/templates/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.652455 bemserver-ui-0.5.0/bemserver_ui/templates/components/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/campaigns/selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.652455 bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_admin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_services.html
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.652455 bemserver-ui-0.5.0/bemserver_ui/templates/components/user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/user_groups/group_for_campaign.html
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/user_groups/user_group_available.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.652455 bemserver-ui-0.5.0/bemserver_ui/templates/components/users/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/users/user_available.html
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/components/users/user_for_group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.652455 bemserver-ui-0.5.0/bemserver_ui/templates/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.652455 bemserver-ui-0.5.0/bemserver_ui/templates/macros/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/macros/components/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/macros/components/structural_element_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/macros/components/ts_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/macros/flash.html
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/macros/partners.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.652455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/about.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.652455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/analysis/energy_consumption.html
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaign_scopes/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaign_scopes/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaign_scopes/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaign_scopes/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaign_scopes/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaigns/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaigns/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaigns/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaigns/manage_groups.html
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaigns/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/categories/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/categories/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/categories/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/categories/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/create.html
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/home.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/notifications/explore.html
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/notifications/setup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.636454 bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/cleanup/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/cleanup/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/missing_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/missing_data/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/missing_data/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/outlier_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/outlier_data/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/outlier_data/manage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/signin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/skeleton.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/create.html
--rw-r--r--   0 runner    (1001) docker     (123)    14988 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/explore.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/properties/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/properties/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/properties/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/create.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/data/completeness.html
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/data/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/data/explore.html
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/data/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/datastates/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/datastates/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/datastates/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/datastates/list.html
--rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    15642 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.656455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/properties/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/properties/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/properties/list.html
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/semantic_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/manage.html
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/manage_campaigns.html
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/bemserver_ui/templates/pages/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/users/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/users/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/users/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/templates/pages/users/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/bemserver_ui/views/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/bemserver_ui/views/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/analysis/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/campaign_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/campaigns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/bemserver_ui/views/events/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/events/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/bemserver_ui/views/services/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/services/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/services/missing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/services/outlier_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/bemserver_ui/views/structural_elements/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/structural_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/structural_elements/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/structural_elements/structural_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/bemserver_ui/views/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/timeseries/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/timeseries/datastates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/timeseries/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/timeseries/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/bemserver_ui/views/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.636454 bemserver-ui-0.5.0/bemserver_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-30 12:26:35.000000 bemserver-ui-0.5.0/bemserver_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-03-30 12:26:35.000000 bemserver-ui-0.5.0/bemserver_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 12:26:35.000000 bemserver-ui-0.5.0/bemserver_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-30 12:26:35.000000 bemserver-ui-0.5.0/bemserver_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-30 12:26:35.000000 bemserver-ui-0.5.0/bemserver_ui.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/requirements/install.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-30 12:26:35.660455 bemserver-ui-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-30 12:26:22.000000 bemserver-ui-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.574422 bemserver-ui-0.5.1/bemserver_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.574422 bemserver-ui-0.5.1/bemserver_ui/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.574422 bemserver-ui-0.5.1/bemserver_ui/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/campaign_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/flask_es6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/jinja_custom_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/partners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66289 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones-areas.json
+-rw-r--r--   0 runner    (1001) docker     (123)   224723 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones-full.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones-regions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/degree_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/campaign_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/outlier_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/weather_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/structural_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/datastates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.570421 bemserver-ui-0.5.1/bemserver_ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver-ico.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver-min.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/accordionList.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/dropZone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/eventLevel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/filterSelect.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/flash.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/itemsCount.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/modalConfirm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/pagination.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/spinner.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/structuralElements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/time/tzPicker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32394 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/timeseries/selector.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/tree.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/userGroup/
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/flashTimer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/formController.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/notifications.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/sidebar.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/array.js
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/dict.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/fetcher.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/flaskES6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/parser.js
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/time.js
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/uuid.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.570421 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaignScopes/
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaigns/selector.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/events/
+-rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/events/edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)    45177 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/events/list.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    66390 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/notifications/explore.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/notifications/setup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/missingData/
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/missingData/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/outlierData/
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/weatherData/
+-rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/structuralElements/
+-rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/delete.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25263 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52668 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/users/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/users/manageGroups.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/styles/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/styles/dragndrop.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/styles/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/styles/signin.css
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/styles/tree.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.570421 bemserver-ui-0.5.1/bemserver_ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/templates/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/templates/components/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/campaigns/selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_admin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_services.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/group_for_campaign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/user_group_available.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/templates/components/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/users/user_available.html
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/users/user_for_group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/structural_element_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/ts_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/macros/flash.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/macros/partners.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/about.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/analysis/degree_days.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/analysis/energy_consumption.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/manage_groups.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/home.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/notifications/explore.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/notifications/setup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.574422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/cleanup/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/cleanup/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/missing_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/missing_data/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/missing_data/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/outlier_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/outlier_data/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/outlier_data/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/weather_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/weather_data/manage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/skeleton.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/explore.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/create.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/completeness.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/explore.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/semantic_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/manage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/manage_campaigns.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/views/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/analysis/degree_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/analysis/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/campaign_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/campaigns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/bemserver_ui/views/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/events/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/bemserver_ui/views/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/services/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/services/missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/services/outlier_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/services/weather_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/structural_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/datastates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.574422 bemserver-ui-0.5.1/bemserver_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-27 15:02:13.000000 bemserver-ui-0.5.1/bemserver_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-27 15:02:13.000000 bemserver-ui-0.5.1/bemserver_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:02:13.000000 bemserver-ui-0.5.1/bemserver_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-27 15:02:13.000000 bemserver-ui-0.5.1/bemserver_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 15:02:13.000000 bemserver-ui-0.5.1/bemserver_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/tox.ini
```

### Comparing `bemserver-ui-0.5.0/LICENSE` & `bemserver-ui-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/PKG-INFO` & `bemserver-ui-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: bemserver-ui
-Version: 0.5.0
+Version: 0.5.1
 Summary: BEMServer web interface
 Home-page: https://github.com/BEMServer/bemserver-ui
 Author: NOBATEK/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
-Provides-Extra: lint
 Provides-Extra: dev
+Provides-Extra: lint
 License-File: LICENSE
 
 ============
 BEMServer UI
 ============
 
 .. image:: https://img.shields.io/pypi/v/bemserver-ui.svg
@@ -85,7 +86,9 @@
                         "text": "The Python micro framework for building web applications."
                     }
                 }
             ]
 
     *(optional)* **BEMSERVER_UI_PLUGINS = None**
         List of absolute folder paths that locate the ``__init__.py`` file from each UI plugin package to load
+
+
```

### Comparing `bemserver-ui-0.5.0/README.rst` & `bemserver-ui-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/__init__.py` & `bemserver-ui-0.5.1/bemserver_ui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import flask
 
 from . import extensions
 from . import internal_api
 from . import views
 
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 def create_app(config_override=None):
     """Create application"""
     app = flask.Flask(__name__)
     app.config.from_object("bemserver_ui.settings.Config")
     app.config.from_envvar("BEMSERVER_UI_SETTINGS_FILE", silent=True)
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/common/tree.py` & `bemserver-ui-0.5.1/bemserver_ui/common/tree.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/__init__.py` & `bemserver-ui-0.5.1/bemserver_ui/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/api_client.py` & `bemserver-ui-0.5.1/bemserver_ui/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/auth.py` & `bemserver-ui-0.5.1/bemserver_ui/extensions/auth.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/campaign_context.py` & `bemserver-ui-0.5.1/bemserver_ui/extensions/campaign_context.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/error_handlers.py` & `bemserver-ui-0.5.1/bemserver_ui/extensions/error_handlers.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/flask_es6.py` & `bemserver-ui-0.5.1/bemserver_ui/extensions/flask_es6.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/jinja_custom_filters.py` & `bemserver-ui-0.5.1/bemserver_ui/extensions/jinja_custom_filters.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/partners.py` & `bemserver-ui-0.5.1/bemserver_ui/extensions/partners.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/plugins.py` & `bemserver-ui-0.5.1/bemserver_ui/extensions/plugins.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/timezones/__init__.py` & `bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/timezones/timezones-areas.json` & `bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones-areas.json`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/timezones/timezones-full.json` & `bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones-full.json`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/extensions/timezones/timezones.py` & `bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/__init__.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/analysis/completeness.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/completeness.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/analysis/energy_consumption.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/energy_consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/campaign_scopes.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/campaign_scopes.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/campaigns.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/events.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/notifications.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/semantics/energy/__init__.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/semantics/energy/consumption.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/semantics/energy/production.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/production.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/semantics/weather.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/weather.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/services/cleanup.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/services/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/services/missing_data.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/services/missing_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/services/outlier_data.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/services/outlier_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/structural_elements.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/structural_elements.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Structural elements internal API"""
+import zoneinfo
 import flask
 
-from bemserver_ui.extensions import auth, ensure_campaign_context
+from bemserver_ui.extensions import auth, ensure_campaign_context, Roles
 from bemserver_ui.common.const import (
     STRUCTURAL_ELEMENT_TYPES,
     FULL_STRUCTURAL_ELEMENT_TYPES,
 )
 from bemserver_ui.common.tree import build_tree
+from bemserver_ui.common.time import convert_html_form_datetime
+from bemserver_ui.common.exceptions import BEMServerUICommonInvalidDatetimeError
 
 
 blp = flask.Blueprint(
     "structural_elements", __name__, url_prefix="/structural_elements"
 )
 
 
@@ -114,14 +117,45 @@
         {
             "type": type,
             "properties": properties,
         }
     )
 
 
+@blp.route("/site/<int:id>/fetch_weather_data", methods=["PUT"])
+@auth.signin_required(roles=[Roles.admin])
+@ensure_campaign_context
+def fetch_weather_data(id):
+    tz = zoneinfo.ZoneInfo(flask.g.campaign_ctxt.tz_name)
+    try:
+        dt_start = convert_html_form_datetime(
+            flask.request.json["start_date"],
+            flask.request.json["start_time"],
+            tz=tz,
+        )
+    except BEMServerUICommonInvalidDatetimeError:
+        flask.abort(422, description="Invalid start datetime!")
+    try:
+        dt_end = convert_html_form_datetime(
+            flask.request.json["end_date"],
+            flask.request.json["end_time"],
+            tz=tz,
+        )
+    except BEMServerUICommonInvalidDatetimeError:
+        flask.abort(422, description="Invalid end datetime!")
+
+    flask.g.api_client.sites.download_weather_data(
+        id,
+        dt_start.isoformat(),
+        dt_end.isoformat(),
+    )
+
+    return flask.jsonify({"success": True})
+
+
 @blp.route("/tree/sites")
 @auth.signin_required
 @ensure_campaign_context
 def retrieve_tree_sites():
     kwargs = {}
     if "draggable" in flask.request.args:
         kwargs["is_draggable"] = flask.request.args["draggable"]
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/timeseries/data.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from io import StringIO
 import csv
 import zoneinfo
 import flask
 
 from bemserver_api_client.enums import DataFormat, Aggregation, BucketWidthUnit
 from bemserver_ui.extensions import auth, ensure_campaign_context
-from bemserver_ui.common.time import convert_html_form_datetime
+from bemserver_ui.common.time import (
+    convert_html_form_datetime,
+    convert_from_iso,
+    strfdelta,
+)
 from bemserver_ui.common.exceptions import BEMServerUICommonInvalidDatetimeError
 
 
 blp = flask.Blueprint("data", __name__, url_prefix="/data")
 
 
 @blp.route("/<int:id>/retrieve_data")
@@ -197,7 +201,36 @@
         dt_start.isoformat(),
         dt_end.isoformat(),
         flask.request.json["data_state"],
         flask.request.json["timeseries_ids"],
     )
 
     return flask.jsonify({"success": True})
+
+
+@blp.route("/stats")
+@auth.signin_required
+@ensure_campaign_context
+def retrieve_stats():
+    ts_ids = [int(x) for x in flask.request.args["timeseries"].split(",")]
+    data_state_id = flask.request.args["data_state"]
+    tz_name = flask.request.args.get("timezone") or flask.g.campaign_ctxt.tz_name
+
+    ts_data_stats_resp = flask.g.api_client.timeseries_data.get_stats(
+        data_state_id,
+        ts_ids,
+        timezone=tz_name,
+    )
+
+    data_stats = ts_data_stats_resp.data["stats"]
+
+    tz = zoneinfo.ZoneInfo(tz_name)
+    for ts_stats in data_stats.values():
+        try:
+            dt_first = convert_from_iso(ts_stats["first_timestamp"], tz=tz)
+            dt_last = convert_from_iso(ts_stats["last_timestamp"], tz=tz)
+            ts_stats["elapsed_time"] = strfdelta(dt_last - dt_first)
+        except BEMServerUICommonInvalidDatetimeError:
+            # Exception raised if timestamps are None.
+            ts_stats["elapsed_time"] = None
+
+    return flask.jsonify(data_stats)
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/timeseries/timeseries.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/user_groups.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/user_groups.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/internal_api/users.py` & `bemserver-ui-0.5.1/bemserver_ui/internal_api/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/images/bemserver-ico.svg` & `bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver-ico.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/images/bemserver-min.svg` & `bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver-min.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/images/bemserver.ico` & `bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver.ico`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/images/bemserver.svg` & `bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/app.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/app.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/accordionList.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/accordionList.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/dropZone.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/dropZone.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/eventLevel.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/eventLevel.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/filterSelect.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/filterSelect.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/flash.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/flash.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/itemsCount.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/itemsCount.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/modalConfirm.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/modalConfirm.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/pagination.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/pagination.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/spinner.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/spinner.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -255,20 +255,27 @@
         this.#updateDateAndTime();
         this.#updateTzInfo();
         this.#updateStyle();
 
         this.#initEventListeners();
     }
 
-    reset() {
-        this.#date = null;
-        this.#time = null;
-        this.#dateMin = null;
-        this.#dateMax = null;
-        this.#updateDateBounds();
+    reset(options = {
+        ignoreDate: false,
+        ignoreTime: false
+    }) {
+        if (!options.ignoreDate) {
+            this.#date = null;
+            this.#dateMin = null;
+            this.#dateMax = null;
+            this.#updateDateBounds();
+        }
+        if (!options.ignoreTime) {
+            this.#time = null;
+        }
         this.#updateDateAndTime();
         this.#updateStyle();
     }
 }
 
 
 if (window.customElements.get("app-datetime-picker") == null) {
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/time/tzPicker.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/time/tzPicker.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/timeseries/selector.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/timeseries/selector.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/tree.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/tree.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/flashTimer.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/flashTimer.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/formController.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/formController.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -12,31 +12,31 @@
     constructor() {
         this.#cacheDOM();
     }
 
     #cacheDOM() {
         this.#confirmFormElmts = [].slice.call(document.querySelectorAll(`form[data-modal-confirm-message]`));
         this.#requiredInputElmts = [].slice.call(document.querySelectorAll(`input:required, select:required, div[is^="app-"][required]`));
-        this.#minMaxInputElmts = [].slice.call(document.querySelectorAll(`input[minlength], input[maxlength], textarea[minlength], textarea[maxlength]`));
+        this.#minMaxInputElmts = [].slice.call(document.querySelectorAll(`input[minlength], input[maxlength], textarea[minlength], textarea[maxlength], input[min], input[max]`));
     }
 
     #getRequiredLabelElmt() {
         let requiredLabelElmt = document.createElement("small");
         requiredLabelElmt.classList.add("fst-italic", "text-danger", "ms-2", "fade-in");
         requiredLabelElmt.textContent = "* (required)";
         return requiredLabelElmt;
     }
 
-    #getMinMaxLabelElmt(minLength, maxLength) {
+    #getMinMaxLabelElmt(minLength, maxLength, isNumber = false) {
         let texts = new Array();
         if (minLength != null) {
-            texts.push(`min. ${minLength} character${minLength > 1 ? "s" : ""}`);
+            texts.push(`min. ${minLength}${!isNumber ? ` character${minLength > 1 ? "s" : ""}` : ""}`);
         }
         if (maxLength != null) {
-            texts.push(`max. ${maxLength} character${maxLength > 1 ? "s": ""}`);
+            texts.push(`max. ${maxLength}${!isNumber ? ` character${maxLength > 1 ? "s" : ""}` : ""}`);
         }
 
         let minMaxText = ``;
         if (texts.length > 0) {
             minMaxText = `(${texts.join(", ")})`;
         }
 
@@ -70,11 +70,17 @@
             requiredInputLabelElmt?.appendChild(this.#getRequiredLabelElmt());
         }
 
         // Add min/max length of inputs.
         for (let minMaxInputElmt of this.#minMaxInputElmts) {
             let minLength = minMaxInputElmt.getAttribute("minlength");
             let maxLength = minMaxInputElmt.getAttribute("maxlength");
-            minMaxInputElmt.parentElement.appendChild(this.#getMinMaxLabelElmt(minLength, maxLength));
+            if (minLength != null || maxLength != null) {
+                minMaxInputElmt.parentElement.appendChild(this.#getMinMaxLabelElmt(minLength, maxLength));
+            } else {
+                let min = minMaxInputElmt.getAttribute("min");
+                let max = minMaxInputElmt.getAttribute("max");
+                minMaxInputElmt.parentElement.appendChild(this.#getMinMaxLabelElmt(min, max, true));
+            }
         }
     }
 }
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/notifications.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/notifications.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/sidebar.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/sidebar.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/array.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/array.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/fetcher.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/fetcher.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/flaskES6.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/flaskES6.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/parser.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/parser.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/time.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/time.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/tools/uuid.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/uuid.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/campaigns/selector.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaigns/selector.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/events/edit.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/events/edit.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/events/list.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/events/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/notifications/explore.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/notifications/explore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/notifications/setup.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/notifications/setup.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/missingData/list.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/missingData/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -281,28 +281,43 @@
                 this.#messagesElmt.appendChild(flashMsgElmt);
             }
         }
         return ``;
     }
 
     #getGeneralHTML(data, path) {
-        return `<div class="d-flex justify-content-between align-items-start gap-3 mb-3">
+        let htmlContent = `<div class="d-flex justify-content-between align-items-start gap-3 mb-3">
     <div>
         <h5 class="text-break">${data.structural_element.name}</h5>
         <h6 class="text-break">${path}</h6>
     </div>
     ${this.#getEditBtnHTML(data.type, data.structural_element.id)}
 </div>
 <p class="fst-italic text-muted text-break">${data.structural_element.description}</p>
 <div class="row">
     <dl class="col">
         <dt>IFC ID</dt>
         <dd>${(data.structural_element.ifc_id != null && data.structural_element.ifc_id != "") ? data.structural_element.ifc_id : "-"}</dd>
     </dl>
 </div>`;
+
+        if (data.type == "site") {
+            htmlContent += `<div class="row">
+    <dl class="col">
+        <dt>Latitude <small class="text-muted">[°]</small></dt>
+        <dd>${data.structural_element.latitude != null ? data.structural_element.latitude : "-"}</dd>
+    </dl>
+    <dl class="col">
+        <dt>Longitude <small class="text-muted">[°]</small></dt>
+        <dd>${data.structural_element.longitude != null ? data.structural_element.longitude : "-"}</dd>
+    </dl>
+</div>`;
+        }
+
+        return htmlContent;
     }
 
     #getItemHelpHTML(itemDescription, withSpace = true) {
         let ret = ``;
         if (itemDescription?.length > 0) {
             let abbrElmt = document.createElement("abbr");
             abbrElmt.title = itemDescription != null ? itemDescription : "";
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/delete.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/delete.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/list.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/list.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -29,14 +29,15 @@
 
 
 export class TimeseriesListView {
 
     #internalAPIRequester = null;
     #getStructElmtsReqID = null;
     #getPropDataReqID = null;
+    #getStatsReqID = {};
     #getEventsReqID = null;
     #sitesTreeReqID = null;
     #zonesTreeReqID = null;
 
     #tzName = "UTC";
 
     #messagesElmt = null;
@@ -113,14 +114,15 @@
         }
 
         for (let accordionTimeseriesBtnElmt of this.#accordionTimeseriesBtnElmts) {
             accordionTimeseriesBtnElmt.addEventListener("show.bs.collapse", (event) => {
                 let tsId = event.target.getAttribute("data-ts-id");
                 this.#renderProperties(tsId);
                 this.#renderStructuralElements(tsId);
+                this.#renderStats(tsId);
                 this.#renderEvents(tsId);
             });
         }
 
         this.#siteSelector.addEventListener("treeNodeSelect", (event) => {
             if (event.detail.type == "space") {
                 this.#structuralElementRecursiveSwitchElmt.checked = false;
@@ -260,14 +262,67 @@
         }
 
         return `<div class="mb-3">
     ${contentHTML}
 </div>`;
     }
 
+    #populateStats(tsDataStats, statsContainerElmt) {
+        statsContainerElmt.innerHTML = "";
+
+        let createListGroupItemElmt = (title, value) => {
+            let listGroupItemElmt = document.createElement("li");
+            listGroupItemElmt.classList.add("list-group-item", "d-flex", "align-items-center", "justify-content-between", "gap-2");
+            timestampsBoundsListElmt.appendChild(listGroupItemElmt);
+            let listGroupItemTitleElmt = document.createElement("h6");
+            listGroupItemTitleElmt.classList.add("fw-bold", "text-muted", "mb-0");
+            listGroupItemTitleElmt.innerText = title;
+            listGroupItemElmt.appendChild(listGroupItemTitleElmt);
+            let listGroupItemValueElmt = document.createElement("small");
+            listGroupItemValueElmt.classList.add("text-nowrap");
+            listGroupItemValueElmt.innerText = value;
+            listGroupItemElmt.appendChild(listGroupItemValueElmt);
+            return listGroupItemElmt;
+        };
+
+        let timestampsCardElmt = document.createElement("div");
+        timestampsCardElmt.classList.add("card", "mb-auto");
+        statsContainerElmt.appendChild(timestampsCardElmt);
+        let timestampsCardHeaderElmt = document.createElement("div");
+        timestampsCardHeaderElmt.classList.add("card-header", "fw-bold");
+        timestampsCardHeaderElmt.innerText = "Timestamp bounds";
+        timestampsCardElmt.appendChild(timestampsCardHeaderElmt);
+        let timestampsBoundsListElmt = document.createElement("ul");
+        timestampsBoundsListElmt.classList.add("list-group", "list-group-flush");
+        timestampsCardElmt.appendChild(timestampsBoundsListElmt);
+        timestampsBoundsListElmt.appendChild(createListGroupItemElmt("First", tsDataStats["first_timestamp"] != null ? TimeDisplay.toLocaleString(new Date(tsDataStats["first_timestamp"]), {
+            timezone: this.#tzName
+        }) : "-"));
+        timestampsBoundsListElmt.appendChild(createListGroupItemElmt("Last", tsDataStats["last_timestamp"] != null ? TimeDisplay.toLocaleString(new Date(tsDataStats["last_timestamp"]), {
+            timezone: this.#tzName
+        }) : "-"));
+        timestampsBoundsListElmt.appendChild(createListGroupItemElmt("Elapsed", tsDataStats["elapsed_time"] || "-"));
+
+        let statsCardElmt = document.createElement("div");
+        statsCardElmt.classList.add("card", "mb-auto");
+        statsContainerElmt.appendChild(statsCardElmt);
+        let statsCardHeaderElmt = document.createElement("div");
+        statsCardHeaderElmt.classList.add("card-header", "fw-bold");
+        statsCardHeaderElmt.innerText = "Values statistics";
+        statsCardElmt.appendChild(statsCardHeaderElmt);
+        let statsListElmt = document.createElement("ul");
+        statsListElmt.classList.add("list-group", "list-group-flush");
+        statsCardElmt.appendChild(statsListElmt);
+        statsListElmt.appendChild(createListGroupItemElmt("Count", Parser.parseIntOrDefault(tsDataStats["count"])));
+        statsListElmt.appendChild(createListGroupItemElmt("Minimum", Parser.parseFloatOrDefault(tsDataStats["min"], Number.NaN, 2)));
+        statsListElmt.appendChild(createListGroupItemElmt("Maximum", Parser.parseFloatOrDefault(tsDataStats["max"], Number.NaN, 2)));
+        statsListElmt.appendChild(createListGroupItemElmt("Average", Parser.parseFloatOrDefault(tsDataStats["avg"], Number.NaN, 2)));
+        statsListElmt.appendChild(createListGroupItemElmt("Standard deviation", Parser.parseFloatOrDefault(tsDataStats["stddev"], Number.NaN, 2)));
+    }
+
     #populateEventList(eventsList, eventsContainerElmt) {
         eventsContainerElmt.innerHTML = "";
         if (eventsList.length > 0) {
             for (let eventData of eventsList) {
                 let eventElmt = document.createElement("div");
                 eventElmt.classList.add("list-group-item");
 
@@ -373,14 +428,48 @@
                 (error) => {
                     timeseriesStructuralElementsElmt.innerHTML = this.#getErrorHTML(error.message);
                 },
             );
         }
     }
 
+    #renderStats(tsId) {
+        let tsDataStatsStatesElmt = document.getElementById(`tsDataStatsStates-${tsId}`);
+        let tsDataStatsContainerElmt = document.getElementById(`tsDataStats-${tsId}`);
+        let alreadyLoaded = JSON.parse(tsDataStatsContainerElmt.getAttribute("data-ts-loaded"));
+
+        if (!alreadyLoaded) {
+            tsDataStatsContainerElmt.innerHTML = "";
+            tsDataStatsContainerElmt.appendChild(new Spinner());
+
+            if (this.#getStatsReqID[tsId] != null) {
+                this.#internalAPIRequester.abort(this.#getStatsReqID[tsId]);
+                this.#getStatsReqID[tsId] = null;
+            }
+            this.#getStatsReqID[tsId] = this.#internalAPIRequester.get(
+                flaskES6.urlFor(`api.timeseries.data.retrieve_stats`, {
+                    data_state: tsDataStatsStatesElmt.value,
+                    timeseries: [tsId]
+                }),
+                (data) => {
+                    this.#populateStats(data[tsId.toString()], tsDataStatsContainerElmt);
+                    tsDataStatsContainerElmt.setAttribute("data-ts-loaded", true);
+                },
+                (error) => {
+                    tsDataStatsContainerElmt.innerHTML = this.#getErrorHTML(error);
+                },
+            );
+
+            tsDataStatsStatesElmt.addEventListener("change", () => {
+                tsDataStatsContainerElmt.setAttribute("data-ts-loaded", false);
+                this.#renderStats(tsId);
+            });
+        }
+    }
+
     #renderEvents(tsId) {
         let tsEventsPageSizeElmt = document.getElementById(`tsEventsPageSize-${tsId}`);
         let tsEventsItemsCountElmt = document.getElementById(`tsEventsItemsCount-${tsId}`);
         let tsEventsPaginationElmt = document.getElementById(`tsEventsPagination-${tsId}`);
         let tsEventsContainerElmt = document.getElementById(`tsEvents-${tsId}`);
         let alreadyLoaded = JSON.parse(tsEventsContainerElmt.getAttribute("data-ts-loaded"));
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/users/list.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/users/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/scripts/modules/views/users/manageGroups.js` & `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/users/manageGroups.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/styles/app.css` & `bemserver-ui-0.5.1/bemserver_ui/static/styles/app.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/styles/main.css` & `bemserver-ui-0.5.1/bemserver_ui/static/styles/main.css`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 h1 {
     color: var(--app-gray);
 }
 h2 {
     color: var(--app-green);
 }
 
+input:invalid:not(:focus) {
+    border-color: var(--bs-danger);
+    border-left-width: 8px;
+    background-color: rgba(var(--bs-danger-rgb), 0.05);
+}
+
 .vr {
     color: var(--app-gray) !important;
 }
 
 .badge.bg-primary {
     background-color: rgba(var(--app-blue-rgb), var(--bs-bg-opacity)) !important;
 }
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/styles/signin.css` & `bemserver-ui-0.5.1/bemserver_ui/static/styles/signin.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/static/styles/tree.css` & `bemserver-ui-0.5.1/bemserver_ui/static/styles/tree.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/campaigns/selector.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/campaigns/selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/header.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/header.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_admin.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_admin.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_services.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_services.html`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
             <div class="accordion-body px-0 py-2">
                 <ul class="nav nav-pills flex-column gap-1">
                     {% filter indent(width=20, first=True) %}
                     {% if g.campaign_ctxt.has_campaign %}
                     {{- mac_sidebar.render_nav_item("Cleanup", url_for("services.cleanup.state"), "Cleanup service", ["bi", "bi-magic"]) -}}
                     {{- mac_sidebar.render_nav_item("Check missing data", url_for("services.missing_data.campaign_context_state"), "Check missing data service", ["bi", "bi-journal-x"]) -}}
                     {{- mac_sidebar.render_nav_item("Check outlier data", url_for("services.outlier_data.campaign_context_state"), "Check outlier data service", ["bi", "bi-layout-wtf"]) -}}
+                    {{- mac_sidebar.render_nav_item("Weather data", url_for("services.weather_data.manage"), "Weather data service", ["bi", "bi-cloud-sun"]) -}}
                     {% endif %}
                     {% for sidebar_section_plugin in sidebar_section_plugins %}
                     {{- mac_sidebar.render_nav_item_from_plugin(sidebar_section_plugin) -}}
                     {% endfor %}
                     {% endfilter %}
                 </ul>
             </div>
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/user_groups/group_for_campaign.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/group_for_campaign.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/user_groups/user_group_available.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/user_group_available.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/users/user_available.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/users/user_available.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/components/users/user_for_group.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/components/users/user_for_group.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/macros/components/sidebar.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/sidebar.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/macros/components/structural_element_selector.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/structural_element_selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/macros/components/ts_selector.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/ts_selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/macros/flash.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/macros/flash.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/macros/partners.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/macros/partners.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/about.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/about.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/analysis/energy_consumption.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/analysis/energy_consumption.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/base.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/base.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaign_scopes/create.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaign_scopes/edit.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaign_scopes/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaign_scopes/view.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaigns/create.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaigns/edit.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaigns/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaigns/manage_groups.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/manage_groups.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/campaigns/view.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/categories/create.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/categories/edit.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/categories/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/create.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/edit.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/events/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/home.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/home.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/notifications/explore.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/notifications/explore.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/notifications/setup.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/notifications/setup.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/cleanup/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/cleanup/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/cleanup/manage.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/cleanup/manage.html`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             {% endif %}
             {% endif %}
         </div>
     </div>
     <div class="row mb-3">
         <div class="col"> 
             <div class="d-flex justify-content-between align-items-center">
-                <form id="formFiltersElmt" class="d-lg-flex d-grid gap-2" action="{{ url_for(request.endpoint) }}" method="POST">
+                <form id="formFiltersElmt" class="d-lg-flex d-grid gap-2" action="{{ url_for(request.endpoint, **request.view_args) }}" method="POST">
                     <input type="hidden" name="sort" id="sort" value="{{ sort }}">
                     <label class="form-label text-nowrap text-muted mb-0" for="sort">Sort by</label>
                     <input type="radio" class="btn-check" name="sort" id="sort-timeseries_name-asc" autocomplete="off" {% if sort == "+timeseries_name" %} checked{% endif %}>
                     <label class="btn btn-sm btn-outline-info" for="sort-timeseries_name-asc" title="Name alphabetical order"><i class="bi bi-sort-alpha-down"></i> Name</label>
                     <input type="radio" class="btn-check" name="sort" id="sort-timeseries_name-desc" autocomplete="off" {% if sort == "-timeseries_name" %} checked{% endif %}>
                     <label class="btn btn-sm btn-outline-info" for="sort-timeseries_name-desc" title="Name reverse alphabetical order"><i class="bi bi-sort-alpha-up"></i> Name</label>
                     <input type="radio" class="btn-check" name="sort" id="sort-last_timestamp-asc" autocomplete="off"{% if sort == "+last_timestamp" %} checked{% endif %}>
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/missing_data/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/missing_data/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/missing_data/manage.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/missing_data/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/outlier_data/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/outlier_data/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/services/outlier_data/manage.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/outlier_data/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/signin.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/signin.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/skeleton.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/skeleton.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/create.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/create.html`

 * *Files 14% similar despite different names*

```diff
@@ -40,14 +40,24 @@
                         <label class="form-label" for="description">Description</label>
                         <textarea class="form-control" id="description" name="description" maxlength="500" rows="3"></textarea>
                     </div>
                     <div class="mb-3">
                         <label class="form-label" for="ifc_id">IFC ID</label>
                         <input type="text" class="form-control" id="ifc_id" name="ifc_id" maxlength="22">
                     </div>
+                    {% if type == 'site' %}
+                    <div class="mb-3">
+                        <label class="form-label" for="latitude">Latitude <span class="fst-italic text-muted">[°]</span></label>
+                        <input type="number" class="form-control" id="latitude" name="latitude" min="-90" max="90" step="0.00001">
+                    </div>
+                    <div class="mb-3">
+                        <label class="form-label" for="longitude">Longitude <span class="fst-italic text-muted">[°]</span></label>
+                        <input type="number" class="form-control" id="longitude" name="longitude" min="-180" max="180" step="0.00001">
+                    </div>
+                    {% endif %}
                 </fieldset>
                 <div class="d-flex justify-content-end gap-2">
                     <a href="{{ url_for('structural_elements.explore') }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
                     <button type="submit" class="btn btn-sm btn-primary text-break" title="Save"{% if has_no_parents %} disabled{% endif %}><i class="bi bi-save"></i> Save</button>
                 </div>
             </form>
         </div>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -9,10 +9,14 @@
 informations {% if parent_type is not none and parents|length > 0 %}
 {% for x in parents %}
 {{ x.name }}
 {% endfor %}
 {% endif %}
 Name [name                ]
 IFC ID [ifc_id              ]
+{% if type == 'site' %}
+Latitude [Â°] [Unknown INPUT type]
+Longitude [Â°] [Unknown INPUT type]
+{% endif %}
 Cancel
 % if has_no_parents %} disabled{% endif %}> Save
 {% endblock main_content %}
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/edit.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/edit.html`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,24 @@
                             <label class="form-label" for="description">Description</label>
                             <textarea form="editForm" class="form-control" id="description" name="description" maxlength="500" rows="3">{{ structural_element.description }}</textarea>
                         </div>
                         <div class="mb-3">
                             <label class="form-label" for="ifc_id">IFC ID</label>
                             <input type="text" form="editForm" class="form-control" id="ifc_id" name="ifc_id" value="{{ structural_element.ifc_id }}" maxlength="22">
                         </div>
+                        {% if type == "site" %}
+                        <div class="mb-3">
+                            <label class="form-label" for="latitude">Latitude <span class="fst-italic text-muted">[°]</span></label>
+                            <input type="number" form="editForm" class="form-control" id="latitude" name="latitude" min="-90" max="90" step="0.00001" value="{{ structural_element.latitude }}">
+                        </div>
+                        <div class="mb-3">
+                            <label class="form-label" for="longitude">Longitude <span class="fst-italic text-muted">[°]</span></label>
+                            <input type="number" form="editForm" class="form-control" id="longitude" name="longitude" min="-180" max="180" step="0.00001" value="{{ structural_element.longitude }}">
+                        </div>
+                        {% endif %}
                     </fieldset>
                 </div>
                 <div class="tab-pane fade{% if tab == 'properties' %} show active{% endif %} p-3" id="properties-tabcontent" role="tabpanel" aria-labelledby="properties-tab">
                     <fieldset>
                         <legend class="invisible d-none">{{ type|capitalize }} properties</legend>
                         {% for property_id, property_data in properties.items() %}
                         <div class="mb-3">
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/explore.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/explore.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/properties/create.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/properties/edit.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/properties/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/structural_elements/upload.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/create.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/data/completeness.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/completeness.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/data/delete.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/delete.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/data/explore.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/explore.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/data/upload.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/datastates/create.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/datastates/edit.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/datastates/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/edit.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/list.html`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,17 @@
                                 <li class="nav-item" role="presentation">
                                     <button class="nav-link" id="properties-tab-{{ x.id }}" data-bs-toggle="tab" data-bs-target="#properties-tabcontent-{{ x.id }}" type="button" role="tab" aria-controls="properties-tabcontent-{{ x.id }}">Properties</button>
                                 </li>
                                 <li class="nav-item" role="presentation">
                                     <button class="nav-link" id="locations-tab-{{ x.id }}" data-bs-toggle="tab" data-bs-target="#locations-tabcontent-{{ x.id }}" type="button" role="tab" aria-controls="locations-tabcontent-{{ x.id }}">Locations</button>
                                 </li>
                                 <li class="nav-item" role="presentation">
+                                    <button class="nav-link" id="stats-tab-{{ x.id }}" data-bs-toggle="tab" data-bs-target="#stats-tabcontent-{{ x.id }}" type="button" role="tab" aria-controls="stats-tabcontent-{{ x.id }}">Data statistics</button>
+                                </li>
+                                <li class="nav-item" role="presentation">
                                     <button class="nav-link" id="events-tab-{{ x.id }}" data-bs-toggle="tab" data-bs-target="#events-tabcontent-{{ x.id }}" type="button" role="tab" aria-controls="events-tabcontent-{{ x.id }}">Events</button>
                                 </li>
                             </ul>
                             <div class="tab-content overflow-auto border border-top-0 bg-white mb-3">
                                 <div class="tab-pane fade show active p-3" id="general-tabcontent-{{ x.id }}" role="tabpanel" aria-labelledby="general-tab-{{ x.id }}">
                                     <div class="d-flex justify-content-between align-items-start gap-3 mb-2">
                                         <small>{{ x.description }}</small>
@@ -151,14 +154,29 @@
                                 </div>
                                 <div class="tab-pane fade p-3" id="properties-tabcontent-{{ x.id }}" role="tabpanel" aria-labelledby="properties-tab-{{ x.id }}">
                                     <div id="timeseriesProperties-{{ x.id }}" data-ts-loaded="false"></div>
                                 </div>
                                 <div class="tab-pane fade p-3" id="locations-tabcontent-{{ x.id }}" role="tabpanel" aria-labelledby="locations-tab-{{ x.id }}">
                                     <div id="timeseriesStructuralElements-{{ x.id }}" data-ts-loaded="false"></div>
                                 </div>
+                                <div class="tab-pane fade p-3" id="stats-tabcontent-{{ x.id }}" role="tabpanel" aria-labelledby="tats-tab-{{ x.id }}">
+                                    <div class="row mb-2 gap-3">
+                                        <div class="col-auto">
+                                            <div class="input-group input-group-sm">
+                                                <span class="input-group-text">Timeseries data state</span>
+                                                <select id="tsDataStatsStates-{{ x.id }}" class="form-select form-select-sm">
+                                                    {% for ts_datastate in ts_data_states %}
+                                                    <option value="{{ ts_datastate.id }}"{% if loop.first %} selected{% endif %}>{{ ts_datastate.name }}</option>
+                                                    {% endfor %}
+                                                </select>
+                                            </div>
+                                        </div>
+                                        <div id="tsDataStats-{{ x.id }}" class="col d-flex flex-wrap gap-3" data-ts-loaded="false"></div>
+                                    </div>
+                                </div>
                                 <div class="tab-pane fade p-3" id="events-tabcontent-{{ x.id }}" role="tabpanel" aria-labelledby="events-tab-{{ x.id }}">
                                     <nav class="row mb-2" aria-label="Events pagination">
                                         <div class="col-auto align-self-center py-1">
                                             <div is="app-pagesize-selector" id="tsEventsPageSize-{{ x.id }}" current="5"></div>
                                         </div>
                                         <div class="col d-flex flex-wrap justify-content-end align-items-center gap-2">
                                             <small class="text-nowrap text-muted"><app-items-count id="tsEventsItemsCount-{{ x.id }}"></app-items-count></small>
```

#### html2text {}

```diff
@@ -55,18 +55,22 @@
 {% if timeseries|length > 0 %}
 {% for x in timeseries %}
  {{ x.name }} {% if x.unit_symbol %} [{{ x.unit_symbol }}] {% endif %}
 {{ x.campaign_scope_name }}
     * General
     * Properties
     * Locations
+    * Data statistics
     * Events
 {{ x.description }} {% if signed_user.is_admin %}
  Edit
  {% endif %}
+{% for ts_datastate in ts_data_states %}
+% if loop.first %} selected{% endif %}>{{ ts_datastate.name }}
+{% endfor %}
 {% endfor %}
 {% else %}
 No data
 {% endif %}
 {% endblock main_content %} {% block body_scripts %} {{ super() -}} {% filter
 indent(width=8, first=True) %}
  {% endfilter %} {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/properties/create.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/properties/edit.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/properties/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/semantic_setup.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/semantic_setup.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/timeseries/upload.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/create.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/edit.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/manage.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/manage_campaigns.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/manage_campaigns.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/user_groups/view.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/users/create.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/users/edit.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/users/list.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/templates/pages/users/view.html` & `bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/__init__.py` & `bemserver-ui-0.5.1/bemserver_ui/views/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/auth.py` & `bemserver-ui-0.5.1/bemserver_ui/views/auth.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/campaign_scopes.py` & `bemserver-ui-0.5.1/bemserver_ui/views/campaign_scopes.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/campaigns.py` & `bemserver-ui-0.5.1/bemserver_ui/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/events/categories.py` & `bemserver-ui-0.5.1/bemserver_ui/views/events/categories.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/events/events.py` & `bemserver-ui-0.5.1/bemserver_ui/views/events/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/main.py` & `bemserver-ui-0.5.1/bemserver_ui/views/main.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/notifications.py` & `bemserver-ui-0.5.1/bemserver_ui/views/notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/services/cleanup.py` & `bemserver-ui-0.5.1/bemserver_ui/views/services/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/services/missing_data.py` & `bemserver-ui-0.5.1/bemserver_ui/views/services/missing_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/services/outlier_data.py` & `bemserver-ui-0.5.1/bemserver_ui/views/services/outlier_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/structural_elements/properties.py` & `bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/properties.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/structural_elements/structural_elements.py` & `bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/structural_elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,17 @@
         payload = {
             "name": flask.request.form["name"],
             "description": flask.request.form["description"],
             "ifc_id": flask.request.form["ifc_id"],
         }
 
         if type in ("site", "zone"):
+            if type == "site":
+                payload["latitude"] = flask.request.form["latitude"]
+                payload["longitude"] = flask.request.form["longitude"]
             payload["campaign_id"] = flask.g.campaign_ctxt.id
         elif type == "building":
             payload["site_id"] = flask.request.form["site"]
         elif type == "storey":
             payload["building_id"] = flask.request.form["building"]
         elif type == "space":
             payload["storey_id"] = flask.request.form["storey"]
@@ -111,15 +114,18 @@
         ret_resp = api_resource.getone(id)
 
     elif flask.request.method == "POST":
         payload = {
             "name": flask.request.form["name"],
             "description": flask.request.form["description"],
             "ifc_id": flask.request.form["ifc_id"],
+            "latitude": flask.request.form["latitude"],
+            "longitude": flask.request.form["longitude"],
         }
+
         ret_resp = api_resource.update(id, payload, etag=flask.request.form["editEtag"])
         flask.flash(f"{type} updated: {ret_resp.data['name']}", "success")
 
         # Update property values, only if value has changed.
         for prop_id, prop_data in properties.items():
             # Flask form is special with checkboxes, it sets:
             #  - "on" if a checkbox input is checked
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/timeseries/data.py` & `bemserver-ui-0.5.1/bemserver_ui/views/timeseries/data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/timeseries/datastates.py` & `bemserver-ui-0.5.1/bemserver_ui/views/timeseries/datastates.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/timeseries/properties.py` & `bemserver-ui-0.5.1/bemserver_ui/views/timeseries/properties.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/timeseries/timeseries.py` & `bemserver-ui-0.5.1/bemserver_ui/views/timeseries/timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,21 +119,25 @@
 
     timeseries_data = deepcopy(timeseries_resp.data)
     for ts_data in timeseries_data:
         ts_data["campaign_scope_name"] = campaign_scopes_by_id[
             ts_data["campaign_scope_id"]
         ]["name"]
 
+    # Get timeseries data states for stats.
+    ts_data_states_resp = flask.g.api_client.timeseries_datastates.getall()
+
     return flask.render_template(
         "pages/timeseries/list.html",
         timeseries=timeseries_data,
         campaign_scopes=campaign_scopes_resp.data,
         filters={**filters, **ui_filters},
         is_filtered=is_filtered,
         pagination=prepare_pagination(timeseries_resp.pagination),
+        ts_data_states=ts_data_states_resp.data,
     )
 
 
 @blp.route("/create", methods=["GET", "POST"])
 @auth.signin_required(roles=[Roles.admin])
 @ensure_campaign_context
 def create():
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/user_groups.py` & `bemserver-ui-0.5.1/bemserver_ui/views/user_groups.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui/views/users.py` & `bemserver-ui-0.5.1/bemserver_ui/views/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.0/bemserver_ui.egg-info/PKG-INFO` & `bemserver-ui-0.5.1/bemserver_ui.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: bemserver-ui
-Version: 0.5.0
+Version: 0.5.1
 Summary: BEMServer web interface
 Home-page: https://github.com/BEMServer/bemserver-ui
 Author: NOBATEK/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
-Provides-Extra: lint
 Provides-Extra: dev
+Provides-Extra: lint
 License-File: LICENSE
 
 ============
 BEMServer UI
 ============
 
 .. image:: https://img.shields.io/pypi/v/bemserver-ui.svg
@@ -85,7 +86,9 @@
                         "text": "The Python micro framework for building web applications."
                     }
                 }
             ]
 
     *(optional)* **BEMSERVER_UI_PLUGINS = None**
         List of absolute folder paths that locate the ``__init__.py`` file from each UI plugin package to load
+
+
```

### Comparing `bemserver-ui-0.5.0/bemserver_ui.egg-info/SOURCES.txt` & `bemserver-ui-0.5.1/bemserver_ui.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -37,24 +37,26 @@
 bemserver_ui/internal_api/events.py
 bemserver_ui/internal_api/notifications.py
 bemserver_ui/internal_api/structural_elements.py
 bemserver_ui/internal_api/user_groups.py
 bemserver_ui/internal_api/users.py
 bemserver_ui/internal_api/analysis/__init__.py
 bemserver_ui/internal_api/analysis/completeness.py
+bemserver_ui/internal_api/analysis/degree_days.py
 bemserver_ui/internal_api/analysis/energy_consumption.py
 bemserver_ui/internal_api/semantics/__init__.py
 bemserver_ui/internal_api/semantics/weather.py
 bemserver_ui/internal_api/semantics/energy/__init__.py
 bemserver_ui/internal_api/semantics/energy/consumption.py
 bemserver_ui/internal_api/semantics/energy/production.py
 bemserver_ui/internal_api/services/__init__.py
 bemserver_ui/internal_api/services/cleanup.py
 bemserver_ui/internal_api/services/missing_data.py
 bemserver_ui/internal_api/services/outlier_data.py
+bemserver_ui/internal_api/services/weather_data.py
 bemserver_ui/internal_api/timeseries/__init__.py
 bemserver_ui/internal_api/timeseries/data.py
 bemserver_ui/internal_api/timeseries/datastates.py
 bemserver_ui/internal_api/timeseries/timeseries.py
 bemserver_ui/static/images/bemserver-ico.svg
 bemserver_ui/static/images/bemserver-min.svg
 bemserver_ui/static/images/bemserver.ico
@@ -71,14 +73,15 @@
 bemserver_ui/static/scripts/modules/components/flash.js
 bemserver_ui/static/scripts/modules/components/itemsCount.js
 bemserver_ui/static/scripts/modules/components/modalConfirm.js
 bemserver_ui/static/scripts/modules/components/pagination.js
 bemserver_ui/static/scripts/modules/components/spinner.js
 bemserver_ui/static/scripts/modules/components/tree.js
 bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
+bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js
 bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
 bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
 bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
 bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
 bemserver_ui/static/scripts/modules/components/time/tzPicker.js
 bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
 bemserver_ui/static/scripts/modules/components/timeseries/selector.js
@@ -86,26 +89,28 @@
 bemserver_ui/static/scripts/modules/tools/array.js
 bemserver_ui/static/scripts/modules/tools/dict.js
 bemserver_ui/static/scripts/modules/tools/fetcher.js
 bemserver_ui/static/scripts/modules/tools/flaskES6.js
 bemserver_ui/static/scripts/modules/tools/parser.js
 bemserver_ui/static/scripts/modules/tools/time.js
 bemserver_ui/static/scripts/modules/tools/uuid.js
+bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
 bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
 bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
 bemserver_ui/static/scripts/modules/views/campaigns/selector.js
 bemserver_ui/static/scripts/modules/views/events/edit.js
 bemserver_ui/static/scripts/modules/views/events/list.js
 bemserver_ui/static/scripts/modules/views/notifications/explore.js
 bemserver_ui/static/scripts/modules/views/notifications/setup.js
 bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
 bemserver_ui/static/scripts/modules/views/services/missingData/list.js
 bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
 bemserver_ui/static/scripts/modules/views/services/outlierData/list.js
 bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js
+bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js
 bemserver_ui/static/scripts/modules/views/structuralElements/explore.js
 bemserver_ui/static/scripts/modules/views/timeseries/delete.js
 bemserver_ui/static/scripts/modules/views/timeseries/list.js
 bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js
 bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js
 bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js
 bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js
@@ -137,14 +142,15 @@
 bemserver_ui/templates/macros/components/structural_element_selector.html
 bemserver_ui/templates/macros/components/ts_selector.html
 bemserver_ui/templates/pages/about.html
 bemserver_ui/templates/pages/base.html
 bemserver_ui/templates/pages/home.html
 bemserver_ui/templates/pages/signin.html
 bemserver_ui/templates/pages/skeleton.html
+bemserver_ui/templates/pages/analysis/degree_days.html
 bemserver_ui/templates/pages/analysis/energy_consumption.html
 bemserver_ui/templates/pages/campaign_scopes/create.html
 bemserver_ui/templates/pages/campaign_scopes/edit.html
 bemserver_ui/templates/pages/campaign_scopes/list.html
 bemserver_ui/templates/pages/campaign_scopes/view.html
 bemserver_ui/templates/pages/campaigns/create.html
 bemserver_ui/templates/pages/campaigns/edit.html
@@ -161,14 +167,15 @@
 bemserver_ui/templates/pages/notifications/setup.html
 bemserver_ui/templates/pages/services/cleanup/list.html
 bemserver_ui/templates/pages/services/cleanup/manage.html
 bemserver_ui/templates/pages/services/missing_data/list.html
 bemserver_ui/templates/pages/services/missing_data/manage.html
 bemserver_ui/templates/pages/services/outlier_data/list.html
 bemserver_ui/templates/pages/services/outlier_data/manage.html
+bemserver_ui/templates/pages/services/weather_data/manage.html
 bemserver_ui/templates/pages/structural_elements/create.html
 bemserver_ui/templates/pages/structural_elements/edit.html
 bemserver_ui/templates/pages/structural_elements/explore.html
 bemserver_ui/templates/pages/structural_elements/upload.html
 bemserver_ui/templates/pages/structural_elements/properties/create.html
 bemserver_ui/templates/pages/structural_elements/properties/edit.html
 bemserver_ui/templates/pages/structural_elements/properties/list.html
@@ -204,22 +211,24 @@
 bemserver_ui/views/campaign_scopes.py
 bemserver_ui/views/campaigns.py
 bemserver_ui/views/main.py
 bemserver_ui/views/notifications.py
 bemserver_ui/views/user_groups.py
 bemserver_ui/views/users.py
 bemserver_ui/views/analysis/__init__.py
+bemserver_ui/views/analysis/degree_days.py
 bemserver_ui/views/analysis/energy_consumption.py
 bemserver_ui/views/events/__init__.py
 bemserver_ui/views/events/categories.py
 bemserver_ui/views/events/events.py
 bemserver_ui/views/services/__init__.py
 bemserver_ui/views/services/cleanup.py
 bemserver_ui/views/services/missing_data.py
 bemserver_ui/views/services/outlier_data.py
+bemserver_ui/views/services/weather_data.py
 bemserver_ui/views/structural_elements/__init__.py
 bemserver_ui/views/structural_elements/properties.py
 bemserver_ui/views/structural_elements/structural_elements.py
 bemserver_ui/views/timeseries/__init__.py
 bemserver_ui/views/timeseries/data.py
 bemserver_ui/views/timeseries/datastates.py
 bemserver_ui/views/timeseries/properties.py
```

### Comparing `bemserver-ui-0.5.0/requirements/dev.txt` & `bemserver-ui-0.5.1/requirements/dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # via virtualenv
 identify==2.5.0
     # via pre-commit
 nodeenv==1.6.0
     # via pre-commit
 platformdirs==2.5.2
     # via virtualenv
-pre-commit==3.2.1
+pre-commit==3.2.2
     # via -r requirements/dev.in
 pyyaml==6.0
     # via pre-commit
 six==1.16.0
     # via virtualenv
 virtualenv==20.14.1
     # via pre-commit
```

### Comparing `bemserver-ui-0.5.0/requirements/install.txt` & `bemserver-ui-0.5.1/requirements/install.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --output-file=requirements/install.txt --resolver=backtracking setup.py
 #
-bemserver-api-client==0.16.0
+bemserver-api-client==0.18.0
     # via bemserver-ui (setup.py)
 certifi==2021.10.8
     # via requests
 charset-normalizer==2.0.12
     # via requests
 click==8.1.3
     # via flask
```

### Comparing `bemserver-ui-0.5.0/setup.py` & `bemserver-ui-0.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Get the long description from the README file
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="bemserver-ui",
-    version="0.5.0",
+    version="0.5.1",
     description="BEMServer web interface",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/BEMServer/bemserver-ui",
     author="NOBATEK/INEF4",
     author_email="dfrederique@nobatek.inef4.com",
     license="AGPLv3+",
@@ -44,13 +44,13 @@
             "GNU Affero General Public License v3 or later (AGPLv3+)"
         ),
     ],
     python_requires=">=3.9",
     install_requires=[
         "flask>=2.2.3,<3.0.0",
         "python-dotenv>=1.0.0,<2.0.0",
-        "bemserver-api-client>=0.16.0,<0.17.0",
+        "bemserver-api-client>=0.18.0,<0.19.0",
     ],
     extras_require=EXTRAS_REQUIRE,
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
 )
```


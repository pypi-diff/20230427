# Comparing `tmp/auterion-cli-1.0.6.tar.gz` & `tmp/auterion-cli-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.0.6.tar", last modified: Tue Apr 25 12:58:48 2023, max compression
+gzip compressed data, was "auterion-cli-1.0.7.tar", last modified: Thu Apr 27 11:42:00 2023, max compression
```

## Comparing `auterion-cli-1.0.6.tar` & `auterion-cli-1.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 12:58:47.000000 auterion-cli-1.0.6/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app-yml-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.956484 auterion-cli-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 11:42:00.952484 auterion-cli-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 11:41:59.000000 auterion-cli-1.0.7/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.948484 auterion-cli-1.0.7/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.952484 auterion-cli-1.0.7/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.952484 auterion-cli-1.0.7/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.952484 auterion-cli-1.0.7/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.952484 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app-yml-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-27 11:41:50.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-27 11:41:50.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 11:42:00.956484 auterion-cli-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/setup.py
```

### Comparing `auterion-cli-1.0.6/README.md` & `auterion-cli-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.0.7/auterion_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/app_command.py` & `auterion-cli-1.0.7/auterioncli/commands/app_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,30 +178,43 @@
         apps = requests.get(f'{self._apps_api_endpoint}/apps')
         if apps:
             return apps.json()
         else:
             error(f"Failed to get apps")
 
     def _print_apps(self, apps):
-        headers = ["Name", "Version", "Status", "Enable", "Services", "Status", "Enable"]
-        matrix = []
+        rows = []
         for app in apps:
-            row = [app.get('name', 'unknown'), app.get('version', 'unknown'), app.get('status', 'unknown'), app.get('enable', 'unknown')]
-            if len(app['services']) > 0:
-                row.append(app['services'][0].get("name", 'unknown'))
-                row.append(app['services'][0].get("status", 'unknown'))
-                row.append(app['services'][0].get("enable", 'unknown'))
-            else:
-                row.append("")
-                row.append("")
-                row.append("")
-            matrix.append(row)
-            for s in app['services'][1:]:
-                matrix.append(["", "", "", "", s.get("name", 'unknown'), s.get("status", 'unknown'), s.get("enable", 'unknown')])
-        print(tabulate(matrix, headers=headers))
+            rows.append({
+                'App name': app.get('name', 'unknown'),
+                'Version': app.get('version', 'unknown'),
+                'App status': app.get('status', 'unknown'),
+                'App enable (autostart)': app.get('enable', 'unknown'),
+            })
+
+            for i, s in enumerate(app['services']):
+                row = {
+                    'Service name': s.get('name', 'unknown'),
+                    'Service status': s.get('status', 'unknown'),
+                    'Service enable (autostart)': s.get('enable', 'unknown')
+                }
+                if 'ssh' in s:
+                    row['SSH port'] = s['ssh']
+                
+                # add the first service to the row with the app name
+                if i == 0:
+                    rows[-1].update(row)
+                else:
+                    if i != len(app['services']) - 1:
+                        row['App name'] = '├─'
+                    else:
+                        row['App name'] = '└─'
+                    rows.append(row)
+
+        print(tabulate(rows, headers='keys'))
 
     def _print_app_result(self, data, app, success_message):
         try:
             body = data.json()
         except:
             body = {}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `auterion-cli-1.0.6/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json` & `auterion-cli-1.0.7/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json` & `auterion-cli-1.0.7/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.0.7/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.0.7/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_install_command.py` & `auterion-cli-1.0.7/auterioncli/commands/app_sdk/app_install_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/app_sdk/environment.py` & `auterion-cli-1.0.7/auterioncli/commands/app_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.0.7/auterioncli/commands/app_sdk/slimify.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.0.7/auterioncli/commands/app_sdk/update.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/container_command.py` & `auterion-cli-1.0.7/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/device_command.py` & `auterion-cli-1.0.7/auterioncli/commands/device_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/info_command.py` & `auterion-cli-1.0.7/auterioncli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/report_command.py` & `auterion-cli-1.0.7/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/commands/utils.py` & `auterion-cli-1.0.7/auterioncli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/main.py` & `auterion-cli-1.0.7/auterioncli/main.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/auterioncli/meta_util.py` & `auterion-cli-1.0.7/auterioncli/meta_util.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.6/setup.py` & `auterion-cli-1.0.7/setup.py`

 * *Files identical despite different names*


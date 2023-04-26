# Comparing `tmp/jaaql-monitor-1.2.12.tar.gz` & `tmp/jaaql-monitor-1.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.12.tar", last modified: Wed Apr 26 22:39:29 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.13.tar", last modified: Wed Apr 26 22:43:20 2023, max compression
```

## Comparing `jaaql-monitor-1.2.12.tar` & `jaaql-monitor-1.2.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 22:39:29.956722 jaaql-monitor-1.2.12/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.12/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-04-26 22:39:29.956722 jaaql-monitor-1.2.12/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.12/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 22:39:29.950720 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-04-26 22:39:29.000000 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-04-26 22:39:29.000000 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 22:39:29.000000 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-26 22:39:29.000000 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 22:39:29.000000 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 22:39:29.954721 jaaql-monitor-1.2.12/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.12/monitor/__init__.py
--rw-rw-rw-   0        0        0    20901 2023-04-26 22:39:12.000000 jaaql-monitor-1.2.12/monitor/main.py
--rw-rw-rw-   0        0        0       42 2023-04-26 22:39:29.957718 jaaql-monitor-1.2.12/setup.cfg
--rw-rw-rw-   0        0        0      828 2023-04-25 20:11:36.000000 jaaql-monitor-1.2.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 22:43:20.474217 jaaql-monitor-1.2.13/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.13/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-04-26 22:43:20.473219 jaaql-monitor-1.2.13/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.13/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 22:43:20.435119 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-04-26 22:43:20.000000 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-04-26 22:43:20.000000 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 22:43:20.000000 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-26 22:43:20.000000 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 22:43:20.000000 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 22:43:20.472219 jaaql-monitor-1.2.13/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.13/monitor/__init__.py
+-rw-rw-rw-   0        0        0    20907 2023-04-26 22:43:04.000000 jaaql-monitor-1.2.13/monitor/main.py
+-rw-rw-rw-   0        0        0       42 2023-04-26 22:43:20.474217 jaaql-monitor-1.2.13/setup.cfg
+-rw-rw-rw-   0        0        0      828 2023-04-25 20:11:36.000000 jaaql-monitor-1.2.13/setup.py
```

### Comparing `jaaql-monitor-1.2.12/LICENSE.txt` & `jaaql-monitor-1.2.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.12/PKG-INFO` & `jaaql-monitor-1.2.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.12
+Version: 1.2.13
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.12/README.md` & `jaaql-monitor-1.2.13/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.12/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.13/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.12
+Version: 1.2.13
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.12/monitor/main.py` & `jaaql-monitor-1.2.13/monitor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
 
             state.connections[configuration_name] = candidate_file_name
 
     deal_with_input(state)
 
 
 def initialise(file_name: str, configs: list[[str, str]]):
-    args = ["-f", file_name]
+    args = ["-f", file_name, "-s"]
 
     for config in configs:
         args.append("-c")
         args.append(config[0])
         args.append(config[1])
 
     initialise_from_args(args)
```

### Comparing `jaaql-monitor-1.2.12/setup.py` & `jaaql-monitor-1.2.13/setup.py`

 * *Files identical despite different names*


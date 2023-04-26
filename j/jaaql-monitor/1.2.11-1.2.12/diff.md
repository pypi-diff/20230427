# Comparing `tmp/jaaql-monitor-1.2.11.tar.gz` & `tmp/jaaql-monitor-1.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.11.tar", last modified: Tue Apr 25 21:13:35 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.12.tar", last modified: Wed Apr 26 22:39:29 2023, max compression
```

## Comparing `jaaql-monitor-1.2.11.tar` & `jaaql-monitor-1.2.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 21:13:35.551519 jaaql-monitor-1.2.11/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.11/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-04-25 21:13:35.551519 jaaql-monitor-1.2.11/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 21:13:35.545519 jaaql-monitor-1.2.11/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-04-25 21:13:35.000000 jaaql-monitor-1.2.11/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-04-25 21:13:35.000000 jaaql-monitor-1.2.11/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 21:13:35.000000 jaaql-monitor-1.2.11/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-25 21:13:35.000000 jaaql-monitor-1.2.11/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 21:13:35.000000 jaaql-monitor-1.2.11/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 21:13:35.548518 jaaql-monitor-1.2.11/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.11/monitor/__init__.py
--rw-rw-rw-   0        0        0    20672 2023-04-18 15:38:10.000000 jaaql-monitor-1.2.11/monitor/main.py
--rw-rw-rw-   0        0        0       42 2023-04-25 21:13:35.552521 jaaql-monitor-1.2.11/setup.cfg
--rw-rw-rw-   0        0        0      828 2023-04-25 20:11:36.000000 jaaql-monitor-1.2.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 22:39:29.956722 jaaql-monitor-1.2.12/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.12/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-04-26 22:39:29.956722 jaaql-monitor-1.2.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.12/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 22:39:29.950720 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-04-26 22:39:29.000000 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-04-26 22:39:29.000000 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 22:39:29.000000 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-26 22:39:29.000000 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 22:39:29.000000 jaaql-monitor-1.2.12/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 22:39:29.954721 jaaql-monitor-1.2.12/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.12/monitor/__init__.py
+-rw-rw-rw-   0        0        0    20901 2023-04-26 22:39:12.000000 jaaql-monitor-1.2.12/monitor/main.py
+-rw-rw-rw-   0        0        0       42 2023-04-26 22:39:29.957718 jaaql-monitor-1.2.12/setup.cfg
+-rw-rw-rw-   0        0        0      828 2023-04-25 20:11:36.000000 jaaql-monitor-1.2.12/setup.py
```

### Comparing `jaaql-monitor-1.2.11/LICENSE.txt` & `jaaql-monitor-1.2.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.11/PKG-INFO` & `jaaql-monitor-1.2.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.11
+Version: 1.2.12
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.11/README.md` & `jaaql-monitor-1.2.12/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.11/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.12/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.11
+Version: 1.2.12
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.11/monitor/main.py` & `jaaql-monitor-1.2.12/monitor/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,19 +459,17 @@
     if len(state.fetched_query) != 0:
         if state.single_query:
             on_go(state)
         else:
             print_error(state, "Attempting to quit with non-empty buffer. Please submit with \\g or clear with \\r")
 
 
-def initialise_from_args():
+def initialise_from_args(args):
     state = State()
 
-    args = sys.argv[1:]
-
     file_name = [idx for arg, idx in zip(args, range(len(args))) if arg in ['-f', '--file']]
     if len(file_name) != 0:
         state.file_name = args[file_name[0] + 1]
 
     state.is_verbose = len([arg for arg in args if arg in ['-v', '--verbose']]) != 0
     state.is_debugging = len([arg for arg in args if arg in ['-d', '--debugging']]) != 0
     state.single_query = len([arg for arg in args if arg in ['-s', '--single-query']]) != 0
@@ -500,9 +498,20 @@
                 print_error(state, "The configuration with name '" + configuration_name + "' already exists")
 
             state.connections[configuration_name] = candidate_file_name
 
     deal_with_input(state)
 
 
+def initialise(file_name: str, configs: list[[str, str]]):
+    args = ["-f", file_name]
+
+    for config in configs:
+        args.append("-c")
+        args.append(config[0])
+        args.append(config[1])
+
+    initialise_from_args(args)
+
+
 if __name__ == "__main__":
-    initialise_from_args()
+    initialise_from_args(sys.argv[1:])
```

### Comparing `jaaql-monitor-1.2.11/setup.py` & `jaaql-monitor-1.2.12/setup.py`

 * *Files identical despite different names*


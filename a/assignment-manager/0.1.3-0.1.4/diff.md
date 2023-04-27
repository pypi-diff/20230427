# Comparing `tmp/assignment-manager-0.1.3.tar.gz` & `tmp/assignment-manager-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assignment-manager-0.1.3.tar", last modified: Wed Apr 26 06:47:06 2023, max compression
+gzip compressed data, was "assignment-manager-0.1.4.tar", last modified: Thu Apr 27 05:46:31 2023, max compression
```

## Comparing `assignment-manager-0.1.3.tar` & `assignment-manager-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-26 06:47:06.773841 assignment-manager-0.1.3/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.3/LICENSE
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-26 06:47:06.773841 assignment-manager-0.1.3/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       21 2023-04-23 16:24:52.000000 assignment-manager-0.1.3/README.md
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       98 2023-04-23 16:36:52.000000 assignment-manager-0.1.3/pyproject.toml
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-04-26 06:47:06.773841 assignment-manager-0.1.3/setup.cfg
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-04-25 18:46:18.000000 assignment-manager-0.1.3/setup.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-26 06:47:06.769841 assignment-manager-0.1.3/src/
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-26 06:47:06.773841 assignment-manager-0.1.3/src/assignment_manager/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.3/src/assignment_manager/__init__.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     3684 2023-04-25 18:43:44.000000 assignment-manager-0.1.3/src/assignment_manager/assignments.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1811 2023-04-25 18:23:27.000000 assignment-manager-0.1.3/src/assignment_manager/data.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2390 2023-04-25 18:39:29.000000 assignment-manager-0.1.3/src/assignment_manager/io.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      989 2023-04-25 18:44:19.000000 assignment-manager-0.1.3/src/assignment_manager/main.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-26 06:47:06.773841 assignment-manager-0.1.3/src/assignment_manager.egg-info/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      493 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/entry_points.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/requires.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/top_level.txt
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.4/LICENSE
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       21 2023-04-23 16:24:52.000000 assignment-manager-0.1.4/README.md
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      129 2023-04-26 20:40:07.000000 assignment-manager-0.1.4/pyproject.toml
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/setup.cfg
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-04-27 05:45:44.000000 assignment-manager-0.1.4/setup.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/src/
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/src/assignment_manager/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.4/src/assignment_manager/__init__.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     3954 2023-04-26 20:45:44.000000 assignment-manager-0.1.4/src/assignment_manager/assignments.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1811 2023-04-25 18:23:27.000000 assignment-manager-0.1.4/src/assignment_manager/data.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2440 2023-04-26 20:40:11.000000 assignment-manager-0.1.4/src/assignment_manager/io.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      989 2023-04-25 18:44:19.000000 assignment-manager-0.1.4/src/assignment_manager/main.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/src/assignment_manager.egg-info/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      493 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/requires.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/top_level.txt
```

### Comparing `assignment-manager-0.1.3/LICENSE` & `assignment-manager-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.3/PKG-INFO` & `assignment-manager-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assignment-manager
-Version: 0.1.3
+Version: 0.1.4
 Summary: Manage reoccuring assignments and tasks.
 Home-page: https://github.com/PraxTube/assignment-manager
 Author: Prax
 Project-URL: Bug Reports, https://github.com/PraxTube/assignment-manager/issues
 Project-URL: Source, https://github.com/PraxTube/assignment-manager
 Keywords: manager,task,assignment,task-manager,assignment-manager
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `assignment-manager-0.1.3/setup.py` & `assignment-manager-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="assignment-manager",
-    version="0.1.3",
+    version="0.1.4",
     description=("Manage reoccuring assignments and tasks."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PraxTube/assignment-manager",
     author="Prax",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `assignment-manager-0.1.3/src/assignment_manager/assignments.py` & `assignment-manager-0.1.4/src/assignment_manager/assignments.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,42 @@
 
 def show_all_assignments():
     data = load_data()
     table_headers = ["Name", "Start", "Deadline", "Progress"]
     table_rows = []
     for key in data:
         cycle = _find_next_deadline(data[key])
+        deadline = "{} ({})".format(
+            data[key][cycle][1],
+            (
+                datetime.strptime(data[key][cycle][1], "%d.%m.%Y")
+                - datetime.today()
+            ).days,
+        )
         table_rows.append(
             [
                 key,
                 data[key][cycle][0],
-                data[key][cycle][1],
+                deadline,
                 Progress(data[key][cycle][2]).name,
             ]
         )
     io.print_table(table_headers, table_rows)
 
 
 def show_specific_assignment():
     data = load_data()
     name = io.course_response(data.keys())
 
     table_headers = ["Start", "Deadline", "Progress"]
     table_rows = []
     for data_entry in data[name]:
-        table_rows.append([data_entry[0], data_entry[1], Progress(data_entry[2]).name])
+        table_rows.append(
+            [data_entry[0], data_entry[1], Progress(data_entry[2]).name]
+        )
     io.print_table(table_headers, table_rows)
 
 
 def generate_dates(start_date, deadline, torus, number_of_assignments):
     start = datetime.strptime(start_date, "%d.%m.%Y")
     end = datetime.strptime(deadline, "%d.%m.%Y")
 
@@ -80,15 +89,17 @@
 
 def update_assignment():
     data = load_data()
     name = io.course_response(data.keys())
 
     cycle_choices = [d for d in data[name]]
     progress_choices = [p.name for p in Progress]
-    cycle, progress = io.update_assignment_response(cycle_choices, progress_choices)
+    cycle, progress = io.update_assignment_response(
+        cycle_choices, progress_choices
+    )
 
     data[name][cycle][2] = progress
     write_data(data)
 
 
 def rename_assignment():
     data = load_data()
@@ -102,30 +113,33 @@
     write_data(data)
 
 
 def remove_assignment():
     data = load_data()
     name = io.course_response(data.keys())
 
-    confirmation_msg = "This will delete [bold]ALL[/bold] data for the course: [bold]{}[/bold]\n".format(
-        name
+    confirmation_msg = (
+        "This will delete [bold]ALL[/bold] data for "
+        "the course: [bold]{}[/bold]\n".format(name)
     )
 
     if not io.confirmation_prompt(confirmation_msg):
         return
 
     data.pop(name)
     write_data(data)
 
 
 def copy_backup():
     if data_file_empty():
         raise ValueError("The data file is empty. No backup will be made.")
 
-    confirmation_msg = "This will OVERWRITE the old BACKUP file if there is one."
+    confirmation_msg = (
+        "This will OVERWRITE the old BACKUP file if there is one."
+    )
 
     if not io.confirmation_prompt(confirmation_msg):
         return
 
     data_copy_backup()
```

### Comparing `assignment-manager-0.1.3/src/assignment_manager/data.py` & `assignment-manager-0.1.4/src/assignment_manager/data.py`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.3/src/assignment_manager/io.py` & `assignment-manager-0.1.4/src/assignment_manager/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from rich.table import Table as RichTable
 import inquirer
 
 
 def print_table(table_headers, table_rows):
     if len(table_headers) != len(table_rows[0]):
         raise ValueError(
-            "The length of the given lists must match", table_headers, table_rows
+            "The length of the given lists must match",
+            table_headers,
+            table_rows,
         )
 
     table = RichTable(*table_headers)
     for row in table_rows:
         table.add_row(*row)
     print(table)
 
@@ -62,15 +64,17 @@
     ]
     return inquirer.prompt(question_course)["name"]
 
 
 def update_assignment_response(cycle_choices, progress_choices):
     questions = [
         inquirer.List(
-            "cycle", message="Which cycle do you want to update?", choices=cycle_choices
+            "cycle",
+            message="Which cycle do you want to update?",
+            choices=cycle_choices,
         ),
         inquirer.List(
             "progress", message="New progress status", choices=progress_choices
         ),
     ]
     answers = inquirer.prompt(questions)
     cycle = cycle_choices.index(answers["cycle"])
```

### Comparing `assignment-manager-0.1.3/src/assignment_manager/main.py` & `assignment-manager-0.1.4/src/assignment_manager/main.py`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.3/src/assignment_manager.egg-info/PKG-INFO` & `assignment-manager-0.1.4/src/assignment_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assignment-manager
-Version: 0.1.3
+Version: 0.1.4
 Summary: Manage reoccuring assignments and tasks.
 Home-page: https://github.com/PraxTube/assignment-manager
 Author: Prax
 Project-URL: Bug Reports, https://github.com/PraxTube/assignment-manager/issues
 Project-URL: Source, https://github.com/PraxTube/assignment-manager
 Keywords: manager,task,assignment,task-manager,assignment-manager
 Classifier: Development Status :: 3 - Alpha
```


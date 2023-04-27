# Comparing `tmp/vinset-4.0.0.tar.gz` & `tmp/vinset-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vinset-4.0.0.tar", last modified: Wed Apr 19 03:12:48 2023, max compression
+gzip compressed data, was "vinset-4.0.1.tar", last modified: Thu Apr 27 06:08:15 2023, max compression
```

## Comparing `vinset-4.0.0.tar` & `vinset-4.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 03:12:48.343947 vinset-4.0.0/
--rw-rw-rw-   0        0        0    11558 2023-03-26 20:05:51.000000 vinset-4.0.0/LICENSE
--rw-rw-rw-   0        0        0      560 2023-04-19 03:12:48.343947 vinset-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6863 2023-03-26 20:05:51.000000 vinset-4.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 03:12:48.343947 vinset-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0      983 2023-04-17 21:29:38.000000 vinset-4.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 03:12:48.329933 vinset-4.0.0/vinset/
--rw-rw-rw-   0        0        0        0 2023-03-26 20:05:52.000000 vinset-4.0.0/vinset/__init__.py
--rw-rw-rw-   0        0        0    54148 2023-04-19 03:09:32.000000 vinset-4.0.0/vinset/vin.py
-drwxrwxrwx   0        0        0        0 2023-04-19 03:12:48.329933 vinset-4.0.0/vinset.egg-info/
--rw-rw-rw-   0        0        0      560 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-19 03:11:11.000000 vinset-4.0.0/vinset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 03:12:48.000000 vinset-4.0.0/vinset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 06:08:15.871229 vinset-4.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-02-15 23:27:28.000000 vinset-4.0.1/LICENSE
+-rw-rw-rw-   0        0        0      581 2023-04-27 06:08:15.870231 vinset-4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9583 2023-04-27 05:44:25.000000 vinset-4.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 06:08:15.871229 vinset-4.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      983 2023-04-27 05:56:07.000000 vinset-4.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 06:08:15.857266 vinset-4.0.1/vinset/
+-rw-rw-rw-   0        0        0        0 2023-02-15 23:27:29.000000 vinset-4.0.1/vinset/__init__.py
+-rw-rw-rw-   0        0        0    55697 2023-04-27 05:56:07.000000 vinset-4.0.1/vinset/vin.py
+drwxrwxrwx   0        0        0        0 2023-04-27 06:08:15.869234 vinset-4.0.1/vinset.egg-info/
+-rw-rw-rw-   0        0        0      581 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-27 06:07:44.000000 vinset-4.0.1/vinset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 06:08:15.000000 vinset-4.0.1/vinset.egg-info/top_level.txt
```

### Comparing `vinset-4.0.0/LICENSE` & `vinset-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vinset-4.0.0/PKG-INFO` & `vinset-4.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: vinset
-Version: 4.0.0
+Version: 4.0.1
 Summary: gaze visualisation program
 Home-page: https://github.com/jtur044/vinset
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: gaze visualisation program vinset
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Command line program to draw the graph from video and csv files.
+
```

### Comparing `vinset-4.0.0/setup.py` & `vinset-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to draw the graph from video and csv files.'
 
 setup(
     name='vinset',
-    version='4.0.0',
+    version='4.0.1',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/vinset',
     description='gaze visualisation program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

### Comparing `vinset-4.0.0/vinset/vin.py` & `vinset-4.0.1/vinset/vin.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,30 +151,44 @@
 
 
 # This function is to create the data array in order to draw lines in graph
 def get_data_array(csv_data_input, t_data_input, y_data_input, offset_input,
                    filter_input=False, filter_by_input=None):
     if filter_input:
         if "=" in filter_by_input:
-            filter_name, filter_value = str(filter_by_input).split("=")
-            filter_value = int(filter_value)
+            filter_name, filter_value, filter_value_type = get_filter_value(filter_by_input)
             data_array_output = []
+
             with open(csv_data_input, "r") as csv_file:
                 csv_reader = (csv.reader(csv_file, delimiter=','))
                 header_array = next(csv_reader)
                 t_pos = get_position(t_data_input, header_array)
                 y_pos = get_position(y_data_input, header_array)
                 f_pos = get_position(filter_name, header_array)
-
-                for row in csv_reader:
-                    filter_check = int(row[f_pos])
-                    if filter_check == filter_value:
-                        time_value = (float(row[t_pos]) + offset_input) * 1000
-                        y_value = float(row[y_pos])
-                        data_array_output.append([time_value, y_value])
+                if filter_value_type == "float":
+                    for row in csv_reader:
+                        filter_check = float(row[f_pos])
+                        if filter_check == filter_value:
+                            time_value = (float(row[t_pos]) + offset_input) * 1000
+                            y_value = float(row[y_pos])
+                            data_array_output.append([time_value, y_value])
+                elif filter_value_type == "int":
+                    for row in csv_reader:
+                        filter_check = int(row[f_pos])
+                        if filter_check == filter_value:
+                            time_value = (float(row[t_pos]) + offset_input) * 1000
+                            y_value = float(row[y_pos])
+                            data_array_output.append([time_value, y_value])
+                else:
+                    for row in csv_reader:
+                        filter_check = str(row[f_pos])
+                        if filter_check == filter_value:
+                            time_value = (float(row[t_pos]) + offset_input) * 1000
+                            y_value = float(row[y_pos])
+                            data_array_output.append([time_value, y_value])
 
             return data_array_output
 
         elif "event" in filter_by_input:
             data_array_output = []
             experience_data = False
             first_value_record = False
@@ -215,14 +229,35 @@
                 time_value = (float(row[t_pos]) + offset_input) * 1000
                 y_value = float(row[y_pos])
                 data_array_output.append([time_value, y_value])
 
         return data_array_output
 
 
+# This function is to get filter by value
+def get_filter_value(string_input):
+    filter_name, filter_value = str(string_input).split("=")
+    if "." in filter_value:
+        try:
+            filter_value = float(filter_value)
+            filter_value_type = "float"
+        except ValueError:
+            filter_value = str(filter_value)
+            filter_value_type = "str"
+    else:
+        try:
+            filter_value = int(filter_value)
+            filter_value_type = "int"
+        except ValueError:
+            filter_value = str(filter_value)
+            filter_value_type = "str"
+
+    return filter_name, filter_value, filter_value_type
+
+
 # This function is to change the given number to scaled value
 def number_to_scale(lower_limit_input, upper_limit_input, box_height_input, number_input):
     total_limit = upper_limit_input - lower_limit_input
     number_in_total = number_input - lower_limit_input
     number_output = int(box_height_input * (number_in_total / total_limit))
 
     return number_output
@@ -975,15 +1010,15 @@
         if float(string_input) == 0:
             string_input = "0.0"
     return string_input
 
 
 def main():
     parser = argparse.ArgumentParser(prog='vinset', description='VINSET package.')
-    parser.add_argument('--version', action='version', version='4.0.0'),
+    parser.add_argument('--version', action='version', version='4.0.1'),
     parser.add_argument("-i", dest="input_filename", required=True, type=argparse.FileType('r'), default=sys.stdin,
                         help="input mp4 file", metavar="filename.mp4")
     parser.add_argument("-d", dest="input_data_filename", required=False, type=argparse.FileType('r'),
                         default=sys.stdin,
                         help="input csv data file", metavar="filename.csv")
     parser.add_argument("-o", dest="output_filename", required=True, type=argparse.FileType('w'), default=sys.stdout,
                         help="output mp4 file", metavar="filename.mp4")
```

### Comparing `vinset-4.0.0/vinset.egg-info/PKG-INFO` & `vinset-4.0.1/vinset.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: vinset
-Version: 4.0.0
+Version: 4.0.1
 Summary: gaze visualisation program
 Home-page: https://github.com/jtur044/vinset
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: gaze visualisation program vinset
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Command line program to draw the graph from video and csv files.
+
```


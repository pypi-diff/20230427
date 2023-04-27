# Comparing `tmp/nyaa-timer-1.2.2.tar.gz` & `tmp/nyaa-timer-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nyaa-timer-1.2.2.tar", last modified: Thu Apr 27 13:17:00 2023, max compression
+gzip compressed data, was "nyaa-timer-1.2.3.tar", last modified: Thu Apr 27 13:18:13 2023, max compression
```

## Comparing `nyaa-timer-1.2.2.tar` & `nyaa-timer-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 13:17:00.693504 nyaa-timer-1.2.2/
--rw-rw-rw-   0        0        0     1620 2023-04-27 13:17:00.693504 nyaa-timer-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1380 2023-04-27 13:16:45.000000 nyaa-timer-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 13:17:00.685503 nyaa-timer-1.2.2/nyaa_timer.egg-info/
--rw-rw-rw-   0        0        0     1620 2023-04-27 13:17:00.000000 nyaa-timer-1.2.2/nyaa_timer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-04-27 13:17:00.000000 nyaa-timer-1.2.2/nyaa_timer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 13:17:00.000000 nyaa-timer-1.2.2/nyaa_timer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 13:17:00.000000 nyaa-timer-1.2.2/nyaa_timer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-27 13:17:00.000000 nyaa-timer-1.2.2/nyaa_timer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 13:17:00.693504 nyaa-timer-1.2.2/nyaatimer/
--rw-rw-rw-   0        0        0        0 2023-04-27 13:13:22.000000 nyaa-timer-1.2.2/nyaatimer/__init__.py
--rw-rw-rw-   0        0        0      530 2023-04-27 12:28:16.000000 nyaa-timer-1.2.2/nyaatimer/nyaatimer.py
--rw-rw-rw-   0        0        0       42 2023-04-27 13:17:00.693504 nyaa-timer-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-04-27 13:16:52.000000 nyaa-timer-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:18:13.891892 nyaa-timer-1.2.3/
+-rw-rw-rw-   0        0        0     1620 2023-04-27 13:18:13.891892 nyaa-timer-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1380 2023-04-27 13:17:40.000000 nyaa-timer-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 13:18:13.883841 nyaa-timer-1.2.3/nyaa_timer.egg-info/
+-rw-rw-rw-   0        0        0     1620 2023-04-27 13:18:13.000000 nyaa-timer-1.2.3/nyaa_timer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-04-27 13:18:13.000000 nyaa-timer-1.2.3/nyaa_timer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:18:13.000000 nyaa-timer-1.2.3/nyaa_timer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 13:18:13.000000 nyaa-timer-1.2.3/nyaa_timer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-27 13:18:13.000000 nyaa-timer-1.2.3/nyaa_timer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 13:18:13.891892 nyaa-timer-1.2.3/nyaatimer/
+-rw-rw-rw-   0        0        0        0 2023-04-27 13:13:22.000000 nyaa-timer-1.2.3/nyaatimer/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-04-27 13:17:59.000000 nyaa-timer-1.2.3/nyaatimer/nyaatimer.py
+-rw-rw-rw-   0        0        0       42 2023-04-27 13:18:13.891892 nyaa-timer-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-04-27 13:17:50.000000 nyaa-timer-1.2.3/setup.py
```

### Comparing `nyaa-timer-1.2.2/PKG-INFO` & `nyaa-timer-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyaa-timer
-Version: 1.2.2
+Version: 1.2.3
 Summary: A simple nyaa_timer decorator to calculate the elapsed time of a function
 Author: Praveen Senpai
 Author-email: pvnt20@gmail.com
 Description-Content-Type: text/markdown
 
 Title: Nyaatimer - A Simple Python Timer Decorator with Rich Output
 
@@ -26,15 +26,17 @@
 ```
 from nyaatimer import nyaatimer
 
 
 @nyaatimer
 def example_function(a, b):
     return a + b
-    result = example_function(1, 2)
+
+
+result = example_function(1, 2)
 ```
 
 This will output the execution time and function details in a visually appealing format:
 
 `Function example_function took 0.00012345 seconds Args=(1, 2), Kwargs={}`
 
 Installation:
```

### Comparing `nyaa-timer-1.2.2/README.md` & `nyaa-timer-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 ```
 from nyaatimer import nyaatimer
 
 
 @nyaatimer
 def example_function(a, b):
     return a + b
-    result = example_function(1, 2)
+
+
+result = example_function(1, 2)
 ```
 
 This will output the execution time and function details in a visually appealing format:
 
 `Function example_function took 0.00012345 seconds Args=(1, 2), Kwargs={}`
 
 Installation:
```

### Comparing `nyaa-timer-1.2.2/nyaa_timer.egg-info/PKG-INFO` & `nyaa-timer-1.2.3/nyaa_timer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyaa-timer
-Version: 1.2.2
+Version: 1.2.3
 Summary: A simple nyaa_timer decorator to calculate the elapsed time of a function
 Author: Praveen Senpai
 Author-email: pvnt20@gmail.com
 Description-Content-Type: text/markdown
 
 Title: Nyaatimer - A Simple Python Timer Decorator with Rich Output
 
@@ -26,15 +26,17 @@
 ```
 from nyaatimer import nyaatimer
 
 
 @nyaatimer
 def example_function(a, b):
     return a + b
-    result = example_function(1, 2)
+
+
+result = example_function(1, 2)
 ```
 
 This will output the execution time and function details in a visually appealing format:
 
 `Function example_function took 0.00012345 seconds Args=(1, 2), Kwargs={}`
 
 Installation:
```

### Comparing `nyaa-timer-1.2.2/setup.py` & `nyaa-timer-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="nyaa-timer",
-    version="1.2.2",
+    version="1.2.3",
     packages=find_packages(),
     install_requires=["rich"],
     author="Praveen Senpai",
     author_email="pvnt20@gmail.com",
     description="A simple nyaa_timer decorator to calculate the elapsed time of a function",
     long_description=long_description,
     long_description_content_type="text/markdown",
```


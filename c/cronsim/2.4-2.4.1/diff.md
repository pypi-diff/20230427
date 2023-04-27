# Comparing `tmp/cronsim-2.4.tar.gz` & `tmp/cronsim-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cronsim-2.4.tar", last modified: Wed Apr 26 15:06:37 2023, max compression
+gzip compressed data, was "cronsim-2.4.1.tar", last modified: Thu Apr 27 15:49:44 2023, max compression
```

## Comparing `cronsim-2.4.tar` & `cronsim-2.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-26 15:06:37.631533 cronsim-2.4/
--rw-r--r--   0 cepe      (1000) cepe      (1000)     1484 2021-05-16 16:31:36.000000 cronsim-2.4/LICENSE
--rw-rw-r--   0 cepe      (1000) cepe      (1000)       24 2022-09-28 14:26:08.000000 cronsim-2.4/MANIFEST.in
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     5497 2023-04-26 15:06:37.631533 cronsim-2.4/PKG-INFO
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     4704 2023-04-26 13:47:00.000000 cronsim-2.4/README.md
-drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-26 15:06:37.631533 cronsim-2.4/cronsim/
--rw-rw-r--   0 cepe      (1000) cepe      (1000)       70 2022-09-28 11:52:58.000000 cronsim-2.4/cronsim/__init__.py
--rw-rw-r--   0 cepe      (1000) cepe      (1000)    10693 2023-04-24 10:56:48.000000 cronsim-2.4/cronsim/cronsim.py
--rw-rw-r--   0 cepe      (1000) cepe      (1000)    19156 2023-04-26 13:19:47.000000 cronsim-2.4/cronsim/explain.py
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        0 2022-09-28 07:26:47.000000 cronsim-2.4/cronsim/py.typed
-drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-26 15:06:37.631533 cronsim-2.4/cronsim.egg-info/
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     5497 2023-04-26 15:06:37.000000 cronsim-2.4/cronsim.egg-info/PKG-INFO
--rw-rw-r--   0 cepe      (1000) cepe      (1000)      267 2023-04-26 15:06:37.000000 cronsim-2.4/cronsim.egg-info/SOURCES.txt
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2023-04-26 15:06:37.000000 cronsim-2.4/cronsim.egg-info/dependency_links.txt
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2022-09-28 14:37:53.000000 cronsim-2.4/cronsim.egg-info/not-zip-safe
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        8 2023-04-26 15:06:37.000000 cronsim-2.4/cronsim.egg-info/top_level.txt
--rw-rw-r--   0 cepe      (1000) cepe      (1000)       38 2023-04-26 15:06:37.631533 cronsim-2.4/setup.cfg
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     1447 2023-04-26 14:46:27.000000 cronsim-2.4/setup.py
+drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-27 15:49:44.206700 cronsim-2.4.1/
+-rw-r--r--   0 cepe      (1000) cepe      (1000)     1484 2021-05-16 16:31:36.000000 cronsim-2.4.1/LICENSE
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)       24 2022-09-28 14:26:08.000000 cronsim-2.4.1/MANIFEST.in
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     5502 2023-04-27 15:49:44.206700 cronsim-2.4.1/PKG-INFO
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     4707 2023-04-27 15:47:03.000000 cronsim-2.4.1/README.md
+drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-27 15:49:44.206700 cronsim-2.4.1/cronsim/
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)       70 2022-09-28 11:52:58.000000 cronsim-2.4.1/cronsim/__init__.py
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)    10693 2023-04-24 10:56:48.000000 cronsim-2.4.1/cronsim/cronsim.py
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)    19130 2023-04-27 15:47:50.000000 cronsim-2.4.1/cronsim/explain.py
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        0 2022-09-28 07:26:47.000000 cronsim-2.4.1/cronsim/py.typed
+drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-27 15:49:44.206700 cronsim-2.4.1/cronsim.egg-info/
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     5502 2023-04-27 15:49:44.000000 cronsim-2.4.1/cronsim.egg-info/PKG-INFO
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)      267 2023-04-27 15:49:44.000000 cronsim-2.4.1/cronsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2023-04-27 15:49:44.000000 cronsim-2.4.1/cronsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2022-09-28 14:37:53.000000 cronsim-2.4.1/cronsim.egg-info/not-zip-safe
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        8 2023-04-27 15:49:44.000000 cronsim-2.4.1/cronsim.egg-info/top_level.txt
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)       38 2023-04-27 15:49:44.206700 cronsim-2.4.1/setup.cfg
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     1449 2023-04-27 15:46:20.000000 cronsim-2.4.1/setup.py
```

### Comparing `cronsim-2.4/LICENSE` & `cronsim-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cronsim-2.4/PKG-INFO` & `cronsim-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cronsim
-Version: 2.4
+Version: 2.4.1
 Summary: Cron expression parser and evaluator
 Home-page: https://github.com/cuu508/cronsim
 Author: Pēteris Caune
 Author-email: cuu508@gmail.com
 License: BSD
 Project-URL: Changelog, https://github.com/cuu508/cronsim/blob/main/CHANGELOG.md
 Keywords: cron,cronjob,crontab,schedule
@@ -154,15 +154,15 @@
 expr = CronSim("*/5 9-17 * * *", datetime.now())
 print(expr.explain())
 ```
 
 Outputs:
 
 ```
-Every 5th minute from 9:00 through 17:59
+Every fifth minute from 09:00 through 17:59
 ```
 
 The text descriptions are available in English only. The text descriptions
 use the 24-hour time format ("23:00" instead of "11:00 PM").
 
 For examples of generated descriptions see `tests/test_explain.py`.
```

### Comparing `cronsim-2.4/README.md` & `cronsim-2.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,14 @@
 expr = CronSim("*/5 9-17 * * *", datetime.now())
 print(expr.explain())
 ```
 
 Outputs:
 
 ```
-Every 5th minute from 9:00 through 17:59
+Every fifth minute from 09:00 through 17:59
 ```
 
 The text descriptions are available in English only. The text descriptions
 use the 24-hour time format ("23:00" instead of "11:00 PM").
 
 For examples of generated descriptions see `tests/test_explain.py`.
```

### Comparing `cronsim-2.4/cronsim/cronsim.py` & `cronsim-2.4.1/cronsim/cronsim.py`

 * *Files identical despite different names*

### Comparing `cronsim-2.4/cronsim/explain.py` & `cronsim-2.4.1/cronsim/explain.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,43 +36,47 @@
     if len(l) == 2:
         return f"{l[0]} and {l[1]}"
 
     head = ", ".join(l[:-1])
     return f"{head}, and {l[-1]}"
 
 
+ORDINALS = {
+    1: "first",
+    2: "second",
+    3: "third",
+    4: "fourth",
+    5: "fifth",
+    6: "sixth",
+    7: "seventh",
+    8: "eighth",
+    9: "ninth",
+}
+
+
 def ordinal(x: int) -> str:
     """Format integer as an ordinal number.
 
     >>> ordinal(1)
-    '1st'
+    'first'
     >>> ordinal(15)
     '15th'
     """
-    if x == 1:
-        return "1st"
-    if x == 2:
-        return "2nd"
-    if x == 3:
-        return "3rd"
-    return f"{x}th"
+    return ORDINALS.get(x, f"{x}th")
 
 
 def format_time(h: int, m: int) -> str:
-    """Format hours and minutes as a 24-hour time.
+    """Format hours and minutes as HH:MM.
 
     >>> format_time(0, 0)
     '00:00'
     >>> format_time(1, 23)
-    '1:23'
+    '01:23'
     """
-    if h == 0:
-        return f"00:{m:02d}"
-
-    return f"{h}:{m:02d}"
+    return f"{h:02d}:{m:02d}"
 
 
 class Field(object):
     name = "FIXME"
     symbolic: list[str] = []
     min_value = 0
     max_value = 0
@@ -502,16 +506,15 @@
         If no special optimizations apply, return None.
         """
 
         if self.dow.star:
             if self.day.single_value == -1:
                 return f"on the last day of {self.month.format()}"
             if self.month.single_value and self.day.single_value:
-                date_ord = ordinal(self.day.single_value)
-                return f"on {self.month.format()} {date_ord}"
+                return f"on {self.month.format()} {self.day.single_value}"
             if self.day.single_value:
                 date_ord = ordinal(self.day.single_value)
                 return f"on the {date_ord} day of {self.month.format()}"
 
         return None
 
     def translate_time(self) -> tuple[str, bool]:
@@ -565,15 +568,15 @@
         return result[0].upper() + result[1:]
 
 
 def explain(expr: str) -> str:
     """Convert the given cron expression to human-friendly description.
 
     >>> explain("0 0 15 JAN-FEB *")
-    'At 00:00 on the 15th day of month in January and February'
+    'At 00:00 on the 15th day of January and February'
     """
     parts = expr.upper().split()
     return Expression(parts).explain()
 
 
 # For quick testing, you can run this script from shell like so:
 # python explain.py "0 0 15 JAN-FEB *"
```

### Comparing `cronsim-2.4/cronsim.egg-info/PKG-INFO` & `cronsim-2.4.1/cronsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cronsim
-Version: 2.4
+Version: 2.4.1
 Summary: Cron expression parser and evaluator
 Home-page: https://github.com/cuu508/cronsim
 Author: Pēteris Caune
 Author-email: cuu508@gmail.com
 License: BSD
 Project-URL: Changelog, https://github.com/cuu508/cronsim/blob/main/CHANGELOG.md
 Keywords: cron,cronjob,crontab,schedule
@@ -154,15 +154,15 @@
 expr = CronSim("*/5 9-17 * * *", datetime.now())
 print(expr.explain())
 ```
 
 Outputs:
 
 ```
-Every 5th minute from 9:00 through 17:59
+Every fifth minute from 09:00 through 17:59
 ```
 
 The text descriptions are available in English only. The text descriptions
 use the 24-hour time format ("23:00" instead of "11:00 PM").
 
 For examples of generated descriptions see `tests/test_explain.py`.
```

### Comparing `cronsim-2.4/setup.py` & `cronsim-2.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from setuptools import find_packages, setup
 
 setup(
     name="cronsim",
-    version="2.4",
+    version="2.4.1",
     url="https://github.com/cuu508/cronsim",
     license="BSD",
     author="Pēteris Caune",
     author_email="cuu508@gmail.com",
     description="Cron expression parser and evaluator",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```


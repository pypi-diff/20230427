# Comparing `tmp/resource_monitoring_bon-1.0.0.4-py3-none-any.whl.zip` & `tmp/resource_monitoring_bon-1.0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9318 bytes, number of entries: 11
+Zip file size: 9321 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      107 b- defN 23-Apr-26 11:57 monitoring/__init__.py
 -rw-rw-rw-  2.0 fat       61 b- defN 23-Apr-17 06:42 monitoring/resource_monitoring.bat
 -rw-rw-rw-  2.0 fat    10052 b- defN 23-Apr-26 12:04 monitoring/resource_monitoring.py
 -rw-rw-rw-  2.0 fat      747 b- defN 23-Apr-27 05:10 monitoring/resource_monitoring_runner.py
 -rw-rw-rw-  2.0 fat      985 b- defN 23-Apr-27 05:01 monitoring/resource_monitoring_runner.spec
 -rw-rw-rw-  2.0 fat     4621 b- defN 23-Apr-20 03:15 monitoring/swagger_manager.py
 -rw-rw-rw-  2.0 fat     3050 b- defN 23-Apr-26 11:39 monitoring/task_scheduler_script.py
--rw-rw-rw-  2.0 fat      919 b- defN 23-Apr-27 05:26 resource_monitoring_bon-1.0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 05:26 resource_monitoring_bon-1.0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       96 b- defN 23-Apr-27 05:26 resource_monitoring_bon-1.0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      999 b- defN 23-Apr-27 05:26 resource_monitoring_bon-1.0.0.4.dist-info/RECORD
-11 files, 21729 bytes uncompressed, 7590 bytes compressed:  65.1%
+-rw-rw-rw-  2.0 fat      919 b- defN 23-Apr-27 09:36 resource_monitoring_bon-1.0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 09:36 resource_monitoring_bon-1.0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       96 b- defN 23-Apr-27 09:36 resource_monitoring_bon-1.0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      999 b- defN 23-Apr-27 09:36 resource_monitoring_bon-1.0.0.5.dist-info/RECORD
+11 files, 21729 bytes uncompressed, 7593 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: monitoring/swagger_manager.py
 Comment: 
 
 Filename: monitoring/task_scheduler_script.py
 Comment: 
 
-Filename: resource_monitoring_bon-1.0.0.4.dist-info/METADATA
+Filename: resource_monitoring_bon-1.0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: resource_monitoring_bon-1.0.0.4.dist-info/WHEEL
+Filename: resource_monitoring_bon-1.0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: resource_monitoring_bon-1.0.0.4.dist-info/top_level.txt
+Filename: resource_monitoring_bon-1.0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: resource_monitoring_bon-1.0.0.4.dist-info/RECORD
+Filename: resource_monitoring_bon-1.0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `resource_monitoring_bon-1.0.0.4.dist-info/METADATA` & `resource_monitoring_bon-1.0.0.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resource-monitoring-bon
-Version: 1.0.0.4
+Version: 1.0.0.5
 Summary: Resource Monitoring Package
 Home-page: 
 Author: bon
 Author-email: kbsrnqhstjr@naver.com
 License: MIT
 Requires-Python: >=3
 Requires-Dist: certifi (==2022.12.7)
```

## Comparing `resource_monitoring_bon-1.0.0.4.dist-info/RECORD` & `resource_monitoring_bon-1.0.0.5.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 monitoring/__init__.py,sha256=JNX5vTedCM-KdZonnC80WwGSpE5ipLi9RHyJnOCoYYs,107
 monitoring/resource_monitoring.bat,sha256=A18QYQl7GlLrNn2JR9sLAmdcqCwGfm8SLtgk2GEmkHM,61
 monitoring/resource_monitoring.py,sha256=ZZnhIwudaNV3p_Op5s64BV21nDB9R9Lv8H2SnZEiOIw,10052
 monitoring/resource_monitoring_runner.py,sha256=WY_NgoMgymtAvV379bazrb54pg8nNGWEP5Gj7EuY0SU,747
 monitoring/resource_monitoring_runner.spec,sha256=MSGbCYs0ssOqtbcFaWgMk9nrYeT0xHCVkY3Px9VxKBE,985
 monitoring/swagger_manager.py,sha256=Y-rxP6kJxYmchW0hHzeu4ZriXrTWIsv824xIR9ZHf3c,4621
 monitoring/task_scheduler_script.py,sha256=y6iQvcXwEEn_6CJ5lAZt_shoBfyd4FeissYV0lEcX9M,3050
-resource_monitoring_bon-1.0.0.4.dist-info/METADATA,sha256=sldfi6lyfa9G_jd0MOj-A0IHEO8FCrGfglT9-aZOgsE,919
-resource_monitoring_bon-1.0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-resource_monitoring_bon-1.0.0.4.dist-info/top_level.txt,sha256=xNf34vcXyWOohixxmhapFhNNJmiihgcHDc0In_7npys,96
-resource_monitoring_bon-1.0.0.4.dist-info/RECORD,,
+resource_monitoring_bon-1.0.0.5.dist-info/METADATA,sha256=14064QjZGsCoPWoc9SDMr5vsoLpdUlpk7moeAA4AtsI,919
+resource_monitoring_bon-1.0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+resource_monitoring_bon-1.0.0.5.dist-info/top_level.txt,sha256=xNf34vcXyWOohixxmhapFhNNJmiihgcHDc0In_7npys,96
+resource_monitoring_bon-1.0.0.5.dist-info/RECORD,,
```


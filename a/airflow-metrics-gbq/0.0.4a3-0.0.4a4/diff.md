# Comparing `tmp/airflow_metrics_gbq-0.0.4a3.tar.gz` & `tmp/airflow_metrics_gbq-0.0.4a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_metrics_gbq-0.0.4a3.tar", max compression
+gzip compressed data, was "airflow_metrics_gbq-0.0.4a4.tar", max compression
```

## Comparing `airflow_metrics_gbq-0.0.4a3.tar` & `airflow_metrics_gbq-0.0.4a4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1296 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/LICENSE
--rw-r--r--   0        0        0     2549 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/README.md
--rw-r--r--   0        0        0        0 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/__init__.py
--rw-r--r--   0        0        0       94 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/exceptions.py
--rw-r--r--   0        0        0    10631 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/metrics.py
--rw-r--r--   0        0        0      700 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/utils/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/utils/gbq_connector.py
--rw-r--r--   0        0        0     1320 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/pyproject.toml
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.4a3/PKG-INFO
+-rw-r--r--   0        0        0     1296 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/LICENSE
+-rw-r--r--   0        0        0     2549 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/__init__.py
+-rw-r--r--   0        0        0       94 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/exceptions.py
+-rw-r--r--   0        0        0    10649 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/metrics.py
+-rw-r--r--   0        0        0      700 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/utils/__init__.py
+-rw-r--r--   0        0        0     1674 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/utils/gbq_connector.py
+-rw-r--r--   0        0        0     1320 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/pyproject.toml
+-rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.4a4/PKG-INFO
```

### Comparing `airflow_metrics_gbq-0.0.4a3/LICENSE` & `airflow_metrics_gbq-0.0.4a4/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a3/README.md` & `airflow_metrics_gbq-0.0.4a4/README.md`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/metrics.py` & `airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,30 +216,30 @@
         """Get dataframes to upload"""
         measure_dict = self._part_types(metrics)
 
         df_counts, df_last, df_timer = pd.DataFrame(), pd.DataFrame(), pd.DataFrame()
 
         if len(measure_dict[Measure.COUNT]) > 0:
             df_counts = (
-                pd.DataFrame([record.__dict__ for record in measure_dict["count"]])
+                pd.DataFrame([record.__dict__ for record in measure_dict[Measure.COUNT]])
                 .groupby(["app", "domain", "check", "name"], dropna=False)
                 .aggregate({"value": "sum", "timestamp": "last"})
                 .reset_index(drop=False)
             )
 
         if len(measure_dict[Measure.LAST]) > 0:
             df_last = (
-                pd.DataFrame([record.__dict__ for record in measure_dict["last"]])
+                pd.DataFrame([record.__dict__ for record in measure_dict[Measure.LAST]])
                 .groupby(["app", "domain", "check", "name"], dropna=False)
                 .aggregate({"value": "last", "timestamp": "last"})
                 .reset_index(drop=False)
             )
 
         if len(measure_dict[Measure.TIMER]) > 0:
-            df_timer = pd.DataFrame([record.__dict__ for record in measure_dict["timer"]])
+            df_timer = pd.DataFrame([record.__dict__ for record in measure_dict[Measure.TIMER]])
             df_timer = df_timer[
                 (df_timer["domain"].isin(["dag", "collect_db_dags"]))
                 | (
                     df_timer["domain"].isin(["dagrun"])
                     & df_timer["name"].apply(lambda x: x.startswith("success") or x.startswith("failed") if x is not None else False)
                 )
             ]
```

### Comparing `airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/utils/__init__.py` & `airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/utils/gbq_connector.py` & `airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/utils/gbq_connector.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a3/pyproject.toml` & `airflow_metrics_gbq-0.0.4a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-metrics-gbq"
-version = "0.0.4a3"
+version = "0.0.4a4"
 description = "Airflow metrics to Google BigQuery"
 authors = ["Shaurya Rawat <rawatshaurya1994@gmail.com>"]
 license = "BSD2"
 readme = "README.md"
 homepage="https://github.com/abyssnlp/airflow-metrics-gbq"
 repository="https://github.com/abyssnlp/airflow-metrics-gbq"
 include=[
```

### Comparing `airflow_metrics_gbq-0.0.4a3/PKG-INFO` & `airflow_metrics_gbq-0.0.4a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-metrics-gbq
-Version: 0.0.4a3
+Version: 0.0.4a4
 Summary: Airflow metrics to Google BigQuery
 Home-page: https://github.com/abyssnlp/airflow-metrics-gbq
 License: BSD2
 Author: Shaurya Rawat
 Author-email: rawatshaurya1994@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```


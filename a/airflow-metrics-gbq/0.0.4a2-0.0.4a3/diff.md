# Comparing `tmp/airflow_metrics_gbq-0.0.4a2.tar.gz` & `tmp/airflow_metrics_gbq-0.0.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_metrics_gbq-0.0.4a2.tar", max compression
+gzip compressed data, was "airflow_metrics_gbq-0.0.4a3.tar", max compression
```

## Comparing `airflow_metrics_gbq-0.0.4a2.tar` & `airflow_metrics_gbq-0.0.4a3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1296 2023-04-26 17:54:29.802426 airflow_metrics_gbq-0.0.4a2/LICENSE
--rw-r--r--   0        0        0     2549 2023-04-26 17:54:29.802426 airflow_metrics_gbq-0.0.4a2/README.md
--rw-r--r--   0        0        0        0 2023-04-26 17:54:29.802426 airflow_metrics_gbq-0.0.4a2/airflow_metrics_gbq/__init__.py
--rw-r--r--   0        0        0       94 2023-04-26 17:54:29.802426 airflow_metrics_gbq-0.0.4a2/airflow_metrics_gbq/exceptions.py
--rw-r--r--   0        0        0    10632 2023-04-26 17:54:29.802426 airflow_metrics_gbq-0.0.4a2/airflow_metrics_gbq/metrics.py
--rw-r--r--   0        0        0      700 2023-04-26 17:54:29.802426 airflow_metrics_gbq-0.0.4a2/airflow_metrics_gbq/utils/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-26 17:54:29.802426 airflow_metrics_gbq-0.0.4a2/airflow_metrics_gbq/utils/gbq_connector.py
--rw-r--r--   0        0        0     1320 2023-04-26 17:54:29.802426 airflow_metrics_gbq-0.0.4a2/pyproject.toml
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.4a2/PKG-INFO
+-rw-r--r--   0        0        0     1296 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/LICENSE
+-rw-r--r--   0        0        0     2549 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/__init__.py
+-rw-r--r--   0        0        0       94 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/exceptions.py
+-rw-r--r--   0        0        0    10631 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/metrics.py
+-rw-r--r--   0        0        0      700 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/utils/__init__.py
+-rw-r--r--   0        0        0     1674 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/utils/gbq_connector.py
+-rw-r--r--   0        0        0     1320 2023-04-26 21:57:28.834967 airflow_metrics_gbq-0.0.4a3/pyproject.toml
+-rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.4a3/PKG-INFO
```

### Comparing `airflow_metrics_gbq-0.0.4a2/LICENSE` & `airflow_metrics_gbq-0.0.4a3/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a2/README.md` & `airflow_metrics_gbq-0.0.4a3/README.md`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a2/airflow_metrics_gbq/metrics.py` & `airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,27 +125,26 @@
         self._last_flush = time.time()
         # buffer
         self.pool = ThreadPoolExecutor(max_workers=num_threads)
         self._metrics = []
         self._buffer = Queue(maxsize=self.CAPACITY + 50)
         self.monitor_batch = threading.Event()
         self.monitor_batch.set()
-        self.pool.submit(self.monitor).add_done_callback(self.callback)
 
         # Flush running
         self.is_flush_running = threading.Event()
         self.is_flush_running.clear()
 
-        # Fetch into queue from socket
-        self.pool.submit(self._fetch).add_done_callback(self.callback)
-
         # Metrics connection
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self._sock.bind((host, port))
 
+        # Fetch into queue from socket
+        self.pool.submit(self._fetch).add_done_callback(self.callback)
+        self.pool.submit(self.monitor).add_done_callback(self.callback)
         atexit.register(self.close)
 
     def monitor(self):
         """Monitor batch time for flushing metrics"""
         while self.monitor_batch.is_set():
             if not self.is_flush_running.is_set():
                 self.is_flush_running.set()
```

### Comparing `airflow_metrics_gbq-0.0.4a2/airflow_metrics_gbq/utils/__init__.py` & `airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a2/airflow_metrics_gbq/utils/gbq_connector.py` & `airflow_metrics_gbq-0.0.4a3/airflow_metrics_gbq/utils/gbq_connector.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a2/pyproject.toml` & `airflow_metrics_gbq-0.0.4a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-metrics-gbq"
-version = "0.0.4a2"
+version = "0.0.4a3"
 description = "Airflow metrics to Google BigQuery"
 authors = ["Shaurya Rawat <rawatshaurya1994@gmail.com>"]
 license = "BSD2"
 readme = "README.md"
 homepage="https://github.com/abyssnlp/airflow-metrics-gbq"
 repository="https://github.com/abyssnlp/airflow-metrics-gbq"
 include=[
```

### Comparing `airflow_metrics_gbq-0.0.4a2/PKG-INFO` & `airflow_metrics_gbq-0.0.4a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-metrics-gbq
-Version: 0.0.4a2
+Version: 0.0.4a3
 Summary: Airflow metrics to Google BigQuery
 Home-page: https://github.com/abyssnlp/airflow-metrics-gbq
 License: BSD2
 Author: Shaurya Rawat
 Author-email: rawatshaurya1994@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```


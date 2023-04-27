# Comparing `tmp/datadog_lambda-4.71.0.tar.gz` & `tmp/datadog_lambda-4.72.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog_lambda-4.71.0.tar", max compression
+gzip compressed data, was "datadog_lambda-4.72.0.tar", max compression
```

## Comparing `datadog_lambda-4.71.0.tar` & `datadog_lambda-4.72.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11379 2022-08-04 20:47:28.483033 datadog_lambda-4.71.0/LICENSE
--rw-r--r--   0        0        0      394 2023-02-13 18:56:36.618770 datadog_lambda-4.71.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0     3422 2023-04-17 18:27:24.481065 datadog_lambda-4.71.0/README.md
--rw-r--r--   0        0        0      538 2023-02-17 16:21:55.265937 datadog_lambda-4.71.0/datadog_lambda/__init__.py
--rw-r--r--   0        0        0     3653 2023-02-13 18:56:36.619460 datadog_lambda-4.71.0/datadog_lambda/api.py
--rw-r--r--   0        0        0     7232 2023-04-12 18:23:27.980925 datadog_lambda-4.71.0/datadog_lambda/cold_start.py
--rw-r--r--   0        0        0     1669 2023-02-13 18:56:36.620125 datadog_lambda-4.71.0/datadog_lambda/constants.py
--rw-r--r--   0        0        0     4769 2023-02-13 18:56:36.620241 datadog_lambda-4.71.0/datadog_lambda/dogstatsd.py
--rw-r--r--   0        0        0     1199 2023-02-13 18:56:36.620396 datadog_lambda-4.71.0/datadog_lambda/extension.py
--rw-r--r--   0        0        0      994 2022-08-04 20:47:28.483885 datadog_lambda-4.71.0/datadog_lambda/handler.py
--rw-r--r--   0        0        0     4707 2023-03-15 15:25:33.105333 datadog_lambda-4.71.0/datadog_lambda/metric.py
--rw-r--r--   0        0        0      139 2023-02-13 18:56:36.620660 datadog_lambda-4.71.0/datadog_lambda/module_name.py
--rw-r--r--   0        0        0     4641 2023-02-13 18:56:36.620808 datadog_lambda-4.71.0/datadog_lambda/patch.py
--rw-r--r--   0        0        0      243 2023-02-13 18:56:36.620890 datadog_lambda-4.71.0/datadog_lambda/stats_writer.py
--rw-r--r--   0        0        0      403 2023-02-13 18:56:36.620968 datadog_lambda-4.71.0/datadog_lambda/statsd_writer.py
--rw-r--r--   0        0        0     1751 2023-02-13 18:56:36.621061 datadog_lambda-4.71.0/datadog_lambda/tag_object.py
--rw-r--r--   0        0        0     3240 2023-02-13 18:56:36.621201 datadog_lambda-4.71.0/datadog_lambda/tags.py
--rw-r--r--   0        0        0     2522 2023-02-13 18:56:36.621290 datadog_lambda-4.71.0/datadog_lambda/thread_stats_writer.py
--rw-r--r--   0        0        0    45292 2023-04-12 18:23:27.981500 datadog_lambda-4.71.0/datadog_lambda/tracing.py
--rw-r--r--   0        0        0    12082 2023-04-12 18:23:27.981977 datadog_lambda-4.71.0/datadog_lambda/trigger.py
--rw-r--r--   0        0        0    13237 2023-04-17 15:01:22.537628 datadog_lambda-4.71.0/datadog_lambda/wrapper.py
--rw-r--r--   0        0        0     3449 2023-04-12 15:37:46.255654 datadog_lambda-4.71.0/datadog_lambda/xray.py
--rw-r--r--   0        0        0     1251 2023-04-17 19:45:09.828867 datadog_lambda-4.71.0/pyproject.toml
--rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 datadog_lambda-4.71.0/setup.py
--rw-r--r--   0        0        0     4969 1970-01-01 00:00:00.000000 datadog_lambda-4.71.0/PKG-INFO
+-rw-r--r--   0        0        0    11379 2022-08-04 20:47:28.483033 datadog_lambda-4.72.0/LICENSE
+-rw-r--r--   0        0        0      394 2023-02-13 18:56:36.618770 datadog_lambda-4.72.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0     3422 2023-04-21 16:54:22.800300 datadog_lambda-4.72.0/README.md
+-rw-r--r--   0        0        0      538 2023-02-17 16:21:55.265937 datadog_lambda-4.72.0/datadog_lambda/__init__.py
+-rw-r--r--   0        0        0     3653 2023-02-13 18:56:36.619460 datadog_lambda-4.72.0/datadog_lambda/api.py
+-rw-r--r--   0        0        0     7232 2023-04-21 16:53:43.883638 datadog_lambda-4.72.0/datadog_lambda/cold_start.py
+-rw-r--r--   0        0        0     1669 2023-02-13 18:56:36.620125 datadog_lambda-4.72.0/datadog_lambda/constants.py
+-rw-r--r--   0        0        0     4769 2023-02-13 18:56:36.620241 datadog_lambda-4.72.0/datadog_lambda/dogstatsd.py
+-rw-r--r--   0        0        0     1199 2023-02-13 18:56:36.620396 datadog_lambda-4.72.0/datadog_lambda/extension.py
+-rw-r--r--   0        0        0      994 2022-08-04 20:47:28.483885 datadog_lambda-4.72.0/datadog_lambda/handler.py
+-rw-r--r--   0        0        0     4707 2023-03-15 15:25:33.105333 datadog_lambda-4.72.0/datadog_lambda/metric.py
+-rw-r--r--   0        0        0      139 2023-02-13 18:56:36.620660 datadog_lambda-4.72.0/datadog_lambda/module_name.py
+-rw-r--r--   0        0        0     4641 2023-02-13 18:56:36.620808 datadog_lambda-4.72.0/datadog_lambda/patch.py
+-rw-r--r--   0        0        0      243 2023-02-13 18:56:36.620890 datadog_lambda-4.72.0/datadog_lambda/stats_writer.py
+-rw-r--r--   0        0        0      403 2023-02-13 18:56:36.620968 datadog_lambda-4.72.0/datadog_lambda/statsd_writer.py
+-rw-r--r--   0        0        0     1751 2023-02-13 18:56:36.621061 datadog_lambda-4.72.0/datadog_lambda/tag_object.py
+-rw-r--r--   0        0        0     3240 2023-02-13 18:56:36.621201 datadog_lambda-4.72.0/datadog_lambda/tags.py
+-rw-r--r--   0        0        0     2522 2023-02-13 18:56:36.621290 datadog_lambda-4.72.0/datadog_lambda/thread_stats_writer.py
+-rw-r--r--   0        0        0    45292 2023-04-12 18:23:27.981500 datadog_lambda-4.72.0/datadog_lambda/tracing.py
+-rw-r--r--   0        0        0    12082 2023-04-12 18:23:27.981977 datadog_lambda-4.72.0/datadog_lambda/trigger.py
+-rw-r--r--   0        0        0    14126 2023-04-25 15:31:19.068502 datadog_lambda-4.72.0/datadog_lambda/wrapper.py
+-rw-r--r--   0        0        0     3449 2023-04-24 17:49:26.625012 datadog_lambda-4.72.0/datadog_lambda/xray.py
+-rw-r--r--   0        0        0     1251 2023-04-27 18:36:42.931504 datadog_lambda-4.72.0/pyproject.toml
+-rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 datadog_lambda-4.72.0/setup.py
+-rw-r--r--   0        0        0     4969 1970-01-01 00:00:00.000000 datadog_lambda-4.72.0/PKG-INFO
```

### Comparing `datadog_lambda-4.71.0/LICENSE` & `datadog_lambda-4.72.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/README.md` & `datadog_lambda-4.72.0/README.md`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/__init__.py` & `datadog_lambda-4.72.0/datadog_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/api.py` & `datadog_lambda-4.72.0/datadog_lambda/api.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/cold_start.py` & `datadog_lambda-4.72.0/datadog_lambda/cold_start.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/constants.py` & `datadog_lambda-4.72.0/datadog_lambda/constants.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/dogstatsd.py` & `datadog_lambda-4.72.0/datadog_lambda/dogstatsd.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/extension.py` & `datadog_lambda-4.72.0/datadog_lambda/extension.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/handler.py` & `datadog_lambda-4.72.0/datadog_lambda/handler.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/metric.py` & `datadog_lambda-4.72.0/datadog_lambda/metric.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/patch.py` & `datadog_lambda-4.72.0/datadog_lambda/patch.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/tag_object.py` & `datadog_lambda-4.72.0/datadog_lambda/tag_object.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/tags.py` & `datadog_lambda-4.72.0/datadog_lambda/tags.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/thread_stats_writer.py` & `datadog_lambda-4.72.0/datadog_lambda/thread_stats_writer.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/tracing.py` & `datadog_lambda-4.72.0/datadog_lambda/tracing.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/trigger.py` & `datadog_lambda-4.72.0/datadog_lambda/trigger.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/datadog_lambda/wrapper.py` & `datadog_lambda-4.72.0/datadog_lambda/wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,28 @@
 
 dd_capture_lambda_payload_enabled = (
     os.environ.get("DD_CAPTURE_LAMBDA_PAYLOAD", "false").lower() == "true"
 )
 service_env_var = os.environ.get("DD_SERVICE", "DefaultServiceName")
 env_env_var = os.environ.get("DD_ENV", None)
 
+DD_FLUSH_TO_LOG = "DD_FLUSH_TO_LOG"
+DD_LOGS_INJECTION = "DD_LOGS_INJECTION"
+DD_MERGE_XRAY_TRACES = "DD_MERGE_XRAY_TRACES"
+AWS_LAMBDA_FUNCTION_NAME = "AWS_LAMBDA_FUNCTION_NAME"
+DD_TRACE_EXTRACTOR = "DD_TRACE_EXTRACTOR"
+DD_TRACE_MANAGED_SERVICES = "DD_TRACE_MANAGED_SERVICES"
+DD_ENCODE_AUTHORIZER_CONTEXT = "DD_ENCODE_AUTHORIZER_CONTEXT"
+DD_DECODE_AUTHORIZER_CONTEXT = "DD_DECODE_AUTHORIZER_CONTEXT"
+DD_COLD_START_TRACING = "DD_COLD_START_TRACING"
+DD_MIN_COLD_START_DURATION = "DD_MIN_COLD_START_DURATION"
+DD_COLD_START_TRACE_SKIP_LIB = "DD_COLD_START_TRACE_SKIP_LIB"
+DD_REQUESTS_SERVICE_NAME = "DD_REQUESTS_SERVICE_NAME"
+DD_SERVICE = "DD_SERVICE"
+
 """
 Usage:
 
 import requests
 from datadog_lambda.wrapper import datadog_lambda_wrapper
 from datadog_lambda.metric import lambda_metric
 
@@ -106,57 +120,60 @@
             traceback.print_exc()
             return func
 
     def __init__(self, func):
         """Executes when the wrapped function gets wrapped"""
         try:
             self.func = func
-            self.flush_to_log = os.environ.get("DD_FLUSH_TO_LOG", "").lower() == "true"
+            self.flush_to_log = os.environ.get(DD_FLUSH_TO_LOG, "").lower() == "true"
             self.logs_injection = (
-                os.environ.get("DD_LOGS_INJECTION", "true").lower() == "true"
+                os.environ.get(DD_LOGS_INJECTION, "true").lower() == "true"
             )
             self.merge_xray_traces = (
-                os.environ.get("DD_MERGE_XRAY_TRACES", "false").lower() == "true"
+                os.environ.get(DD_MERGE_XRAY_TRACES, "false").lower() == "true"
             )
-            self.function_name = os.environ.get("AWS_LAMBDA_FUNCTION_NAME", "function")
-            self.extractor_env = os.environ.get("DD_TRACE_EXTRACTOR", None)
+            self.function_name = os.environ.get(AWS_LAMBDA_FUNCTION_NAME, "function")
+            self.extractor_env = os.environ.get(DD_TRACE_EXTRACTOR, None)
             self.trace_extractor = None
             self.span = None
             self.inferred_span = None
-            self.make_inferred_span = (
-                os.environ.get("DD_TRACE_MANAGED_SERVICES", "true").lower() == "true"
+            depends_on_dd_tracing_enabled = (
+                lambda original_boolean: dd_tracing_enabled and original_boolean
+            )
+            self.make_inferred_span = depends_on_dd_tracing_enabled(
+                os.environ.get(DD_TRACE_MANAGED_SERVICES, "true").lower() == "true"
             )
-            self.encode_authorizer_context = (
-                os.environ.get("DD_ENCODE_AUTHORIZER_CONTEXT", "true").lower() == "true"
+            self.encode_authorizer_context = depends_on_dd_tracing_enabled(
+                os.environ.get(DD_ENCODE_AUTHORIZER_CONTEXT, "true").lower() == "true"
             )
-            self.decode_authorizer_context = (
-                os.environ.get("DD_DECODE_AUTHORIZER_CONTEXT", "true").lower() == "true"
+            self.decode_authorizer_context = depends_on_dd_tracing_enabled(
+                os.environ.get(DD_DECODE_AUTHORIZER_CONTEXT, "true").lower() == "true"
             )
-            self.cold_start_tracing = (
-                os.environ.get("DD_COLD_START_TRACING", "true").lower() == "true"
+            self.cold_start_tracing = depends_on_dd_tracing_enabled(
+                os.environ.get(DD_COLD_START_TRACING, "true").lower() == "true"
             )
             self.min_cold_start_trace_duration = 3
-            if "DD_MIN_COLD_START_DURATION" in os.environ:
+            if DD_MIN_COLD_START_DURATION in os.environ:
                 try:
                     self.min_cold_start_trace_duration = int(
-                        os.environ["DD_MIN_COLD_START_DURATION"]
+                        os.environ[DD_MIN_COLD_START_DURATION]
                     )
                 except Exception:
-                    logger.debug("Malformatted env DD_MIN_COLD_START_DURATION")
+                    logger.debug(f"Malformatted env {DD_MIN_COLD_START_DURATION}")
             self.cold_start_trace_skip_lib = [
                 "ddtrace.internal.compat",
                 "ddtrace.filters",
             ]
-            if "DD_COLD_START_TRACE_SKIP_LIB" in os.environ:
+            if DD_COLD_START_TRACE_SKIP_LIB in os.environ:
                 try:
                     self.cold_start_trace_skip_lib = os.environ[
-                        "DD_COLD_START_TRACE_SKIP_LIB"
+                        DD_COLD_START_TRACE_SKIP_LIB
                     ].split(",")
                 except Exception:
-                    logger.debug("Malformatted for env DD_COLD_START_TRACE_SKIP_LIB")
+                    logger.debug(f"Malformatted for env {DD_COLD_START_TRACE_SKIP_LIB}")
             self.response = None
             if profiling_env_var:
                 self.prof = profiler.Profiler(env=env_env_var, service=service_env_var)
             if self.extractor_env:
                 extractor_parts = self.extractor_env.rsplit(".", 1)
                 if len(extractor_parts) == 2:
                     (mod_name, extractor_name) = extractor_parts
@@ -166,16 +183,16 @@
 
             # Inject trace correlation ids to logs
             if self.logs_injection:
                 inject_correlation_ids()
 
             # This prevents a breaking change in ddtrace v0.49 regarding the service name
             # in requests-related spans
-            os.environ["DD_REQUESTS_SERVICE_NAME"] = os.environ.get(
-                "DD_SERVICE", "aws.lambda"
+            os.environ[DD_REQUESTS_SERVICE_NAME] = os.environ.get(
+                DD_SERVICE, "aws.lambda"
             )
             # Patch third-party libraries for tracing
             patch_all()
 
             logger.debug("datadog_lambda_wrapper initialized")
         except Exception:
             traceback.print_exc()
@@ -215,15 +232,15 @@
         if sampling_priority is not None:
             injected_headers[TraceHeader.SAMPLING_PRIORITY] = str(
                 span_context.sampling_priority
             )
         injected_headers[Headers.Parent_Span_Finish_Time] = finish_time_ns
         if request_id is not None:
             injected_headers[Headers.Authorizing_Request_Id] = request_id
-        datadog_data = base64.b64encode(json.dumps(injected_headers).encode())
+        datadog_data = base64.b64encode(json.dumps(injected_headers).encode()).decode()
         self.response.setdefault("context", {})
         self.response["context"]["_datadog"] = datadog_data
 
     def _before(self, event, context):
         try:
             self.response = None
             set_cold_start()
```

### Comparing `datadog_lambda-4.71.0/datadog_lambda/xray.py` & `datadog_lambda-4.72.0/datadog_lambda/xray.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.71.0/pyproject.toml` & `datadog_lambda-4.72.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datadog_lambda"
-version = "4.71.0"
+version = "4.72.0"
 description = "The Datadog AWS Lambda Library"
 authors = ["Datadog, Inc. <dev@datadoghq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/DataDog/datadog-lambda-python"
 keywords = [
     "datadog",
```

### Comparing `datadog_lambda-4.71.0/setup.py` & `datadog_lambda-4.72.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
          'requests>=2.22.0,<3.0.0',
          'nose2>=0.9.1,<0.10.0',
          'flake8>=3.7.9,<4.0.0',
          'httpretty>=0.9.7,<0.10.0']}
 
 setup_kwargs = {
     'name': 'datadog-lambda',
-    'version': '4.71.0',
+    'version': '4.72.0',
     'description': 'The Datadog AWS Lambda Library',
     'long_description': "# datadog-lambda-python\n\n![build](https://github.com/DataDog/datadog-lambda-python/workflows/build/badge.svg)\n[![PyPI](https://img.shields.io/pypi/v/datadog-lambda)](https://pypi.org/project/datadog-lambda/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datadog-lambda)\n[![Slack](https://chat.datadoghq.com/badge.svg?bg=632CA6)](https://chat.datadoghq.com/)\n[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-lambda-python/blob/main/LICENSE)\n\nDatadog Lambda Library for Python (3.7, 3.8, 3.9, and 3.10) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.\n\n## Installation\n\nFollow the [installation instructions](https://docs.datadoghq.com/serverless/installation/python/), and view your function's enhanced metrics, traces and logs in Datadog.\n\n## Configuration\n\nFollow the [configuration instructions](https://docs.datadoghq.com/serverless/configuration) to tag your telemetry, capture request/response payloads, filter or scrub sensitive information from logs or traces, and more.\n\n## Opening Issues\n\nIf you encounter a bug with this package, we want to hear about it. Before opening a new issue, search the existing issues to avoid duplicates.\n\nWhen opening an issue, include the Datadog Lambda Library version, Python version, and stack trace if available. In addition, include the steps to reproduce when appropriate.\n\nYou can also open an issue for a feature request.\n\n## Lambda Profiling Beta\n\nDatadog's [Continuous Profiler](https://www.datadoghq.com/product/code-profiling/) is now available in beta for Python in version 4.62.0 and layer version 62 and above. This optional feature is enabled by setting the `DD_PROFILING_ENABLED` environment variable to `true`. During the beta period, profiling is available at no additional cost.\n\nThe Continuous Profiler works by spawning a thread which periodically wakes up and takes a snapshot of the CPU and Heap of all running python code. This can include the profiler itself. If you want the Profiler to ignore itself, set `DD_PROFILING_IGNORE_PROFILER` to `true`.\n\n## Major Version Notes\n\n### 4.x / Layer version 61+\n\n- Python3.6 support has been [deprecated](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html) by AWS, and support removed from this library.\n- `dd-trace` upgraded from 0.61 to 1.4, full release notes are available [here](https://ddtrace.readthedocs.io/en/stable/release_notes.html#v1-0-0)\n  - `get_correlation_ids()` has been changed to `get_log_correlation_context()`, which now returns a dictionary containing the active `span_id`, `trace_id`, as well as `service` and `env`.\n\n## Contributing\n\nIf you find an issue with this package and have a fix, please feel free to open a pull request following the [procedures](CONTRIBUTING.md).\n\n## Community\n\nFor product feedback and questions, join the `#serverless` channel in the [Datadog community on Slack](https://chat.datadoghq.com/).\n\n## License\n\nUnless explicitly stated otherwise all files in this repository are licensed under the Apache License Version 2.0.\n\nThis product includes software developed at Datadog (https://www.datadoghq.com/). Copyright 2019 Datadog, Inc.\n",
     'author': 'Datadog, Inc.',
     'author_email': 'dev@datadoghq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DataDog/datadog-lambda-python',
```

### Comparing `datadog_lambda-4.71.0/PKG-INFO` & `datadog_lambda-4.72.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-lambda
-Version: 4.71.0
+Version: 4.72.0
 Summary: The Datadog AWS Lambda Library
 Home-page: https://github.com/DataDog/datadog-lambda-python
 License: Apache-2.0
 Keywords: datadog,aws,lambda,layer
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 Requires-Python: >=3.7.0,<4
```


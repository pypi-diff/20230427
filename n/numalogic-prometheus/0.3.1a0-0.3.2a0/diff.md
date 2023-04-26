# Comparing `tmp/numalogic_prometheus-0.3.1a0.tar.gz` & `tmp/numalogic_prometheus-0.3.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic_prometheus-0.3.1a0.tar", max compression
+gzip compressed data, was "numalogic_prometheus-0.3.2a0.tar", max compression
```

## Comparing `numalogic_prometheus-0.3.1a0.tar` & `numalogic_prometheus-0.3.2a0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-04-24 22:45:22.427111 numalogic_prometheus-0.3.1a0/LICENSE
--rw-r--r--   0        0        0      847 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/__init__.py
--rw-r--r--   0        0        0      974 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/_config.py
--rw-r--r--   0        0        0      756 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/_constants.py
--rw-r--r--   0        0        0        0 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/clients/__init__.py
--rw-r--r--   0        0        0     3565 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/clients/prometheus.py
--rw-r--r--   0        0        0     1316 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/clients/redis.py
--rw-r--r--   0        0        0     1367 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/clients/sentinel.py
--rw-r--r--   0        0        0     2145 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/configs/config.yaml
--rw-r--r--   0        0        0     1841 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/default-configs/config.yaml
--rw-r--r--   0        0        0      337 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/default-configs/numalogic_config.yaml
--rw-r--r--   0        0        0     4447 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/entities.py
--rw-r--r--   0        0        0      954 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/factory.py
--rw-r--r--   0        0        0     8854 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/tools.py
--rw-r--r--   0        0        0      366 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/__init__.py
--rw-r--r--   0        0        0      741 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/filter.py
--rw-r--r--   0        0        0     3628 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/inference.py
--rw-r--r--   0        0        0     7014 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/postprocess.py
--rw-r--r--   0        0        0     1889 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/preprocess.py
--rw-r--r--   0        0        0     3476 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/threshold.py
--rw-r--r--   0        0        0     4321 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/window.py
--rw-r--r--   0        0        0      134 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udsink/__init__.py
--rw-r--r--   0        0        0     5608 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udsink/train.py
--rw-r--r--   0        0        0     7795 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udsink/train_rollout.py
--rw-r--r--   0        0        0     5026 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/watcher.py
--rw-r--r--   0        0        0     1542 2023-04-24 22:45:22.435111 numalogic_prometheus-0.3.1a0/pyproject.toml
--rw-r--r--   0        0        0     1063 1970-01-01 00:00:00.000000 numalogic_prometheus-0.3.1a0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-26 22:19:51.663205 numalogic_prometheus-0.3.2a0/LICENSE
+-rw-r--r--   0        0        0      839 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/__init__.py
+-rw-r--r--   0        0        0     1395 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/_config.py
+-rw-r--r--   0        0        0      561 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/_constants.py
+-rw-r--r--   0        0        0        0 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/__init__.py
+-rw-r--r--   0        0        0     3565 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/prometheus.py
+-rw-r--r--   0        0        0     1316 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/redis.py
+-rw-r--r--   0        0        0     1342 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/sentinel.py
+-rw-r--r--   0        0        0     2145 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/configs/config.yaml
+-rw-r--r--   0        0        0     1841 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/default-configs/config.yaml
+-rw-r--r--   0        0        0      337 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/default-configs/numalogic_config.yaml
+-rw-r--r--   0        0        0      382 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/default-configs/pipeline_config.yaml
+-rw-r--r--   0        0        0     4483 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/entities.py
+-rw-r--r--   0        0        0      954 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/factory.py
+-rw-r--r--   0        0        0     8855 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/tools.py
+-rw-r--r--   0        0        0      366 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/__init__.py
+-rw-r--r--   0        0        0      741 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/filter.py
+-rw-r--r--   0        0        0     4148 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/inference.py
+-rw-r--r--   0        0        0     6982 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/postprocess.py
+-rw-r--r--   0        0        0     1887 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/preprocess.py
+-rw-r--r--   0        0        0     3431 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/threshold.py
+-rw-r--r--   0        0        0     4321 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/window.py
+-rw-r--r--   0        0        0      134 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udsink/__init__.py
+-rw-r--r--   0        0        0     5616 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udsink/train.py
+-rw-r--r--   0        0        0     7808 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udsink/train_rollout.py
+-rw-r--r--   0        0        0     5935 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/watcher.py
+-rw-r--r--   0        0        0     1542 2023-04-26 22:19:51.671205 numalogic_prometheus-0.3.2a0/pyproject.toml
+-rw-r--r--   0        0        0     1063 1970-01-01 00:00:00.000000 numalogic_prometheus-0.3.2a0/PKG-INFO
```

### Comparing `numalogic_prometheus-0.3.1a0/LICENSE` & `numalogic_prometheus-0.3.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/__init__.py` & `numalogic_prometheus-0.3.2a0/numaprom/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 
-from numaprom._config import UnifiedConf, MetricConf, AppConf, NumapromConf
+from numaprom._config import UnifiedConf, MetricConf, AppConf, DataConf
 
 
 def get_logger(name):
     formatter = logging.Formatter("%(asctime)s-%(levelname)s-%(message)s")
     logger = logging.getLogger(name)
     stream_handler = logging.StreamHandler()
     if os.getenv("DEBUG", False):
@@ -21,8 +21,8 @@
     pl_logger = logging.getLogger("pytorch_lightning")
     pl_logger.propagate = False
     pl_logger.setLevel(logging.ERROR)
     pl_logger.addHandler(stream_handler)
     return logger
 
 
-__all__ = ["UnifiedConf", "MetricConf", "AppConf", "NumapromConf", "get_logger"]
+__all__ = ["UnifiedConf", "MetricConf", "AppConf", "DataConf", "get_logger"]
```

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/clients/prometheus.py` & `numalogic_prometheus-0.3.2a0/numaprom/clients/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/clients/redis.py` & `numalogic_prometheus-0.3.2a0/numaprom/clients/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/clients/sentinel.py` & `numalogic_prometheus-0.3.2a0/numaprom/clients/sentinel.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,14 +35,11 @@
         ),
     )
     sentinel_args = {"sentinels": [(host, port)], "socket_timeout": 0.1, "decode_responses": True}
 
     _LOGGER.info("Sentinel redis params: %s", sentinel_args)
 
     sentinel = Sentinel(
-        **sentinel_args,
-        sentinel_kwargs=dict(password=password),
-        password=password,
-        retry=retry,
+        **sentinel_args, sentinel_kwargs=dict(password=password), password=password, retry=retry
     )
     SENTINEL_MASTER_CLIENT = sentinel.master_for(mastername)
     return SENTINEL_MASTER_CLIENT
```

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/configs/config.yaml` & `numalogic_prometheus-0.3.2a0/numaprom/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/default-configs/config.yaml` & `numalogic_prometheus-0.3.2a0/numaprom/default-configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/entities.py` & `numalogic_prometheus-0.3.2a0/numaprom/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     EXTRACTED = "extracted"
     PRE_PROCESSED = "pre_processed"
     INFERRED = "inferred"
     THRESHOLD = "threshold_complete"
     POST_PROCESSED = "post_processed"
     ARTIFACT_NOT_FOUND = "artifact_not_found"
     ARTIFACT_STALE = "artifact_is_stale"
+    RUNTIME_ERROR = "runtime_error"
 
 
 class Header(str, Enum):
     STATIC_INFERENCE = "static_threshold"
     MODEL_INFERENCE = "model_inference"
     TRAIN_REQUEST = "request_training"
     MODEL_STALE = "model_stale"
```

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/factory.py` & `numalogic_prometheus-0.3.2a0/numaprom/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/tools.py` & `numalogic_prometheus-0.3.2a0/numaprom/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import socket
 import time
 from collections import OrderedDict
 from datetime import timedelta, datetime
 from functools import wraps
 from json import JSONDecodeError
 from typing import Optional, Sequence, List
@@ -16,20 +15,17 @@
 from mlflow.exceptions import RestException
 from numalogic.config import PostprocessFactory
 from numalogic.models.threshold import SigmoidThreshold
 from numalogic.registry import MLflowRegistry, ArtifactData
 from pynumaflow.function import Messages, Message
 
 from numaprom import get_logger, MetricConf
-from numaprom._constants import (
-    DEFAULT_TRACKING_URI,
-    DEFAULT_PROMETHEUS_SERVER,
-)
 from numaprom.entities import TrainerPayload, StreamPayload
 from numaprom.clients.prometheus import Prometheus
+from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 
 def catch_exception(func):
     @wraps(func)
     def inner_function(*args, **kwargs):
@@ -126,46 +122,53 @@
 
 
 def load_model(
     skeys: Sequence[str], dkeys: Sequence[str], artifact_type: str = "pytorch"
 ) -> Optional[ArtifactData]:
     set_aws_session()
     try:
-        tracking_uri = os.getenv("TRACKING_URI", DEFAULT_TRACKING_URI)
-        ml_registry = MLflowRegistry(tracking_uri=tracking_uri, artifact_type=artifact_type)
+        registry_conf = ConfigManager.get_registry_config()
+        ml_registry = MLflowRegistry(
+            tracking_uri=registry_conf.tracking_uri, artifact_type=artifact_type
+        )
         return ml_registry.load(skeys=skeys, dkeys=dkeys)
     except RestException as warn:
         if warn.error_code == 404:
             return None
         _LOGGER.warning("Non 404 error from mlflow: %r", warn)
     except Exception as ex:
         _LOGGER.error("Unexpected error while loading model from MLflow database: %r", ex)
         return None
 
 
 def save_model(
     skeys: Sequence[str], dkeys: Sequence[str], model, artifact_type="pytorch", **metadata
 ) -> Optional[ModelVersion]:
     set_aws_session()
-    tracking_uri = os.getenv("TRACKING_URI", DEFAULT_TRACKING_URI)
-    ml_registry = MLflowRegistry(tracking_uri=tracking_uri, artifact_type=artifact_type)
+    registry_conf = ConfigManager.get_registry_config()
+    ml_registry = MLflowRegistry(
+        tracking_uri=registry_conf.tracking_uri, artifact_type=artifact_type
+    )
     version = ml_registry.save(skeys=skeys, dkeys=dkeys, artifact=model, **metadata)
     return version
 
 
 def fetch_data(
-    payload: TrainerPayload, metric_config: MetricConf, labels: dict, return_labels=None
+    payload: TrainerPayload,
+    metric_config: MetricConf,
+    labels: dict,
+    return_labels=None,
+    hours: int = 36,
 ) -> pd.DataFrame:
     _start_time = time.time()
-
-    prometheus_server = os.getenv("PROMETHEUS_SERVER", DEFAULT_PROMETHEUS_SERVER)
-    datafetcher = Prometheus(prometheus_server)
+    prometheus_conf = ConfigManager.get_prometheus_config()
+    datafetcher = Prometheus(prometheus_conf.server)
 
     end_dt = datetime.now(pytz.utc)
-    start_dt = end_dt - timedelta(hours=36)
+    start_dt = end_dt - timedelta(hours=hours)
 
     df = datafetcher.query_metric(
         metric_name=payload.composite_keys["name"],
         labels_map=labels,
         return_labels=return_labels,
         start=start_dt.timestamp(),
         end=end_dt.timestamp(),
```

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/udf/filter.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/filter.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/udf/inference.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/inference.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 from orjson import orjson
 from pynumaflow.function import Datum
 from torch.utils.data import DataLoader
 
 from numaprom import get_logger, MetricConf
 from numaprom.entities import PayloadFactory
 from numaprom.entities import Status, StreamPayload, Header
-from numaprom.tools import (
-    load_model,
-    msg_forward,
-)
+from numaprom.tools import load_model, msg_forward
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 
 def _run_inference(
     payload: StreamPayload, artifact_data: ArtifactData, numalogic_conf: NumalogicConf
 ) -> StreamPayload:
     model = artifact_data.artifact
     stream_data = payload.get_stream_array()
     stream_loader = DataLoader(StreamingDataset(stream_data, numalogic_conf.model.conf["seq_len"]))
 
     trainer = AutoencoderTrainer()
-    recon_err = trainer.predict(model, dataloaders=stream_loader)
+    try:
+        recon_err = trainer.predict(model, dataloaders=stream_loader)
+    except Exception as err:
+        _LOGGER.exception("%s - Runtime error while performing inference: %r", payload.uuid, err)
+        raise RuntimeError("Failed to infer") from err
 
     _LOGGER.info("%s - Successfully inferred", payload.uuid)
 
     payload.set_win_arr(recon_err.numpy())
     payload.set_status(Status.INFERRED)
     payload.set_metadata("version", artifact_data.extras.get("version"))
     return payload
@@ -41,19 +42,15 @@
 
 def _is_model_stale(
     payload: StreamPayload, artifact_data: ArtifactData, metric_config: MetricConf
 ) -> bool:
     date_updated = artifact_data.extras["last_updated_timestamp"] / 1000
     stale_date = (datetime.now() - timedelta(hours=int(metric_config.retrain_freq_hr))).timestamp()
     if date_updated < stale_date:
-        _LOGGER.info(
-            "%s - Model found is stale for %s",
-            payload.uuid,
-            payload.composite_keys,
-        )
+        _LOGGER.info("%s - Model found is stale for %s", payload.uuid, payload.composite_keys)
         return True
     return False
 
 
 @msg_forward
 def inference(_: str, datum: Datum) -> bytes:
     _start_time = time.perf_counter()
@@ -69,15 +66,15 @@
             "%s - Models not found in the previous steps, forwarding for static thresholding. Keys: %s",
             payload.uuid,
             payload.composite_keys,
         )
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
     # Load config
-    metric_config = ConfigManager().get_metric_config(payload.composite_keys)
+    metric_config = ConfigManager.get_metric_config(payload.composite_keys)
     numalogic_conf = metric_config.numalogic_conf
 
     # Load inference model
     artifact_data = load_model(
         skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
         dkeys=[numalogic_conf.model.name],
     )
@@ -92,14 +89,24 @@
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
     # Check if current model is stale
     if _is_model_stale(payload, artifact_data, metric_config):
         payload.set_header(Header.MODEL_STALE)
 
     # Generate predictions
-    payload = _run_inference(payload, artifact_data, numalogic_conf)
+    try:
+        payload = _run_inference(payload, artifact_data, numalogic_conf)
+    except RuntimeError:
+        _LOGGER.info(
+            "%s - Failed to infer, forwarding for static thresholding. Keys: %s",
+            payload.uuid,
+            payload.composite_keys,
+        )
+        payload.set_header(Header.STATIC_INFERENCE)
+        payload.set_status(Status.RUNTIME_ERROR)
+        return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
     _LOGGER.info("%s - Sending Payload: %s ", payload.uuid, payload)
     _LOGGER.debug(
         "%s - Time taken in inference: %.4f sec", payload.uuid, time.perf_counter() - _start_time
     )
     return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
```

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/udf/postprocess.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/postprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,32 +7,33 @@
 
 from pynumaflow.function import Datum
 from redis.sentinel import MasterNotFoundError
 
 from numaprom import get_logger, UnifiedConf
 from numaprom.entities import Status, PrometheusPayload, StreamPayload, Header
 from numaprom.clients.sentinel import get_redis_client
-from numaprom.tools import (
-    msgs_forward,
-    WindowScorer,
-)
+from numaprom.tools import msgs_forward, WindowScorer
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
-HOST = os.getenv("REDIS_HOST")
-PORT = int(os.getenv("REDIS_PORT", 6379))
 AUTH = os.getenv("REDIS_AUTH")
-MASTERNAME = os.getenv("REDIS_MASTERNAME")
 
 
 def __save_to_redis(
     payload: StreamPayload, final_score: float, recreate: bool, unified_config: UnifiedConf
 ):
-    r = get_redis_client(HOST, PORT, password=AUTH, mastername=MASTERNAME, recreate=recreate)
+    redis_conf = ConfigManager.get_redis_config()
+    r = get_redis_client(
+        redis_conf.host,
+        redis_conf.port,
+        password=AUTH,
+        mastername=redis_conf.master_name,
+        recreate=recreate,
+    )
 
     metric_name = payload.composite_keys["name"]
 
     r_keys = payload.composite_keys
     r_keys.pop("name")
     r_key = f"{':'.join(r_keys.values())}:{payload.end_ts}"
 
@@ -83,17 +84,15 @@
 
 def __construct_publisher_payload(
     stream_payload: StreamPayload, final_score: float
 ) -> PrometheusPayload:
     metric_name = stream_payload.composite_keys["name"]
     namespace = stream_payload.composite_keys["namespace"]
 
-    labels = {
-        "model_version": str(stream_payload.get_metadata("version")),
-    }
+    labels = {"model_version": str(stream_payload.get_metadata("version"))}
 
     for key in stream_payload.composite_keys:
         if key != "name":
             labels[key] = stream_payload.composite_keys[key]
 
     return PrometheusPayload(
         timestamp_ms=int(stream_payload.end_ts),
@@ -107,17 +106,15 @@
 
 
 def __construct_unified_payload(
     stream_payload: StreamPayload, max_anomaly: float, unified_config: UnifiedConf
 ) -> PrometheusPayload:
     namespace = stream_payload.composite_keys["namespace"]
 
-    labels = {
-        "model_version": str(stream_payload.get_metadata("version")),
-    }
+    labels = {"model_version": str(stream_payload.get_metadata("version"))}
 
     for key in stream_payload.composite_keys:
         if key != "name":
             labels[key] = stream_payload.composite_keys[key]
 
     return PrometheusPayload(
         timestamp_ms=int(stream_payload.end_ts),
@@ -127,15 +124,15 @@
         type="Gauge",
         value=max_anomaly,
         labels=labels,
     )
 
 
 def _publish(final_score: float, payload: StreamPayload) -> List[bytes]:
-    unified_config = ConfigManager().get_unified_config(payload.composite_keys)
+    unified_config = ConfigManager.get_unified_config(payload.composite_keys)
 
     publisher_json = __construct_publisher_payload(payload, final_score).as_json()
     _LOGGER.info("%s - Payload sent to publisher: %s", payload.uuid, publisher_json)
 
     if not unified_config:
         _LOGGER.debug(
             "%s - Using default config, cannot generate a unified anomaly score", payload.uuid
@@ -176,15 +173,15 @@
     """
     _start_time = time.perf_counter()
 
     _in_msg = datum.value.decode("utf-8")
     payload = StreamPayload(**orjson.loads(_in_msg))
 
     # Load config
-    metric_config = ConfigManager().get_metric_config(payload.composite_keys)
+    metric_config = ConfigManager.get_metric_config(payload.composite_keys)
 
     _LOGGER.debug("%s - Received Payload: %r ", payload.uuid, payload)
 
     winscorer = WindowScorer(metric_config)
 
     # Use only using static thresholding
     if payload.header == Header.STATIC_INFERENCE:
```

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/udf/preprocess.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     _start_time = time.perf_counter()
     _in_msg = datum.value.decode("utf-8")
 
     payload = StreamPayload(**orjson.loads(_in_msg))
     _LOGGER.info("%s - Received Payload: %r ", payload.uuid, payload)
 
     # Load config
-    metric_config = ConfigManager().get_metric_config(payload.composite_keys)
+    metric_config = ConfigManager.get_metric_config(payload.composite_keys)
     preprocess_cfgs = metric_config.numalogic_conf.preprocess
 
     # Load preprocess artifact
     preproc_artifact = load_model(
         skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
         dkeys=[_conf.name for _conf in preprocess_cfgs],
         artifact_type="sklearn",
```

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/udf/threshold.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/threshold.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,15 @@
 
 from orjson import orjson
 from pynumaflow.function import Datum
 
 from numaprom import get_logger
 from numaprom._constants import TRAIN_VTX_KEY, POSTPROC_VTX_KEY
 from numaprom.entities import Status, TrainerPayload, PayloadFactory, Header
-from numaprom.tools import (
-    conditional_forward,
-    calculate_static_thresh,
-    load_model,
-)
+from numaprom.tools import conditional_forward, calculate_static_thresh, load_model
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 
 def _get_static_thresh_payload(payload, metric_config) -> bytes:
     """
@@ -40,22 +36,21 @@
     # Construct payload objects
     payload = PayloadFactory.from_json(_in_msg)
     train_payload = TrainerPayload(
         uuid=payload.uuid, composite_keys=OrderedDict(payload.composite_keys)
     )
 
     # Load config
-    cm = ConfigManager()
-    metric_config = cm.get_metric_config(payload.composite_keys)
+    metric_config = ConfigManager.get_metric_config(payload.composite_keys)
     thresh_cfg = metric_config.numalogic_conf.threshold
 
     # Check if payload needs static inference
     if payload.header == Header.STATIC_INFERENCE:
-        _LOGGER.debug(
-            "%s - Models not found in the previous steps, performing static thresholding. Keys: %s",
+        _LOGGER.info(
+            "%s - Sending to trainer and performing static thresholding. Keys: %s",
             payload.uuid,
             payload.composite_keys,
         )
         return [
             (TRAIN_VTX_KEY, orjson.dumps(train_payload)),
             (POSTPROC_VTX_KEY, _get_static_thresh_payload(payload, metric_config)),
         ]
@@ -91,10 +86,10 @@
     # Prepare payload for forwarding
     payload.set_win_arr(y_score)
     payload.set_status(Status.THRESHOLD)
     messages.append((POSTPROC_VTX_KEY, orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)))
 
     _LOGGER.info("%s - Sending Payload: %r ", payload.uuid, payload)
     _LOGGER.debug(
-        "%s - Time taken in threshold: %.4f", payload.uuid, time.perf_counter() - _start_time
+        "%s - Time taken in threshold: %.4f sec", payload.uuid, time.perf_counter() - _start_time
     )
     return messages
```

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/udf/window.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 from numaprom.entities import StreamPayload, Status, Header
 from numaprom.clients.sentinel import get_redis_client
 from numaprom.tools import msg_forward, create_composite_keys
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
-HOST = os.getenv("REDIS_HOST")
-PORT = int(os.getenv("REDIS_PORT", 6379))
 AUTH = os.getenv("REDIS_AUTH")
-MASTERNAME = os.getenv("REDIS_MASTERNAME")
 
 
 # TODO get the replacement value from config
 def _clean_arr(
     id_: str,
     ckeys: dict,
     arr: npt.NDArray[float],
@@ -43,17 +40,23 @@
 ) -> list[tuple[float, float]]:
     """
     Adds an element to the sliding window using a redis sorted set.
 
     Returns an empty list if adding the element does not create a new entry
     to the set.
     """
+    redis_conf = ConfigManager.get_redis_config()
     redis_client = get_redis_client(
-        HOST, PORT, password=AUTH, mastername=MASTERNAME, recreate=recreate
+        redis_conf.host,
+        redis_conf.port,
+        password=AUTH,
+        mastername=redis_conf.master_name,
+        recreate=recreate,
     )
+
     with redis_client.pipeline() as pl:
         pl.zadd(key, {f"{value}::{ts}": ts})
         pl.zremrangebyrank(key, -(buff_size + 10), -buff_size)
         pl.zrange(key, -win_size, -1, withscores=True, score_cast_func=int)
         out = pl.execute()
     _is_new, _, _window = out
     if not _is_new:
@@ -68,15 +71,15 @@
     UDF to construct windowing of the streaming input data, required by ML models.
     """
     _LOGGER.debug("Received Msg: %s ", datum.value)
 
     _start_time = time.perf_counter()
     msg = orjson.loads(datum.value)
 
-    metric_config = ConfigManager().get_metric_config(
+    metric_config = ConfigManager.get_metric_config(
         {"name": msg["name"], "namespace": msg["labels"]["namespace"]}
     )
     win_size = metric_config.numalogic_conf.model.conf["seq_len"]
     buff_size = int(os.getenv("BUFF_SIZE", 10 * win_size))
 
     if buff_size < win_size:
         raise ValueError(
```

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/udsink/train.py` & `numalogic_prometheus-0.3.2a0/numaprom/udsink/train.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,20 +16,15 @@
 from numaprom.entities import TrainerPayload
 from numaprom.clients.sentinel import get_redis_client
 from numaprom.tools import save_model, fetch_data
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
-HOST = os.getenv("REDIS_HOST")
-PORT = int(os.getenv("REDIS_PORT", 6379))
 AUTH = os.getenv("REDIS_AUTH")
-MASTERNAME = os.getenv("REDIS_MASTERNAME")
-EXPIRY = int(os.getenv("REDIS_EXPIRY", 300))
-MIN_TRAIN_SIZE = int(os.getenv("MIN_TRAIN_SIZE", 2000))
 
 
 def clean_data(df: pd.DataFrame, limit=12) -> pd.DataFrame:
     df.replace([np.inf, -np.inf], np.nan, inplace=True)
     df = df.fillna(method="ffill", limit=limit)
     df = df.fillna(method="bfill", limit=limit)
     if df.columns[df.isna().any()].tolist():
@@ -73,25 +68,31 @@
     thresh_factory = ThresholdFactory()
     thresh_clf = thresh_factory.get_instance(thresh_cfg)
     thresh_clf.fit(x_reconerr)
     return thresh_clf
 
 
 def _is_new_request(payload: TrainerPayload) -> bool:
+    redis_conf = ConfigManager.get_redis_config()
     redis_client = get_redis_client(
-        HOST, PORT, password=AUTH, mastername=MASTERNAME, recreate=False
+        redis_conf.host,
+        redis_conf.port,
+        password=AUTH,
+        mastername=redis_conf.master_name,
+        recreate=False,
     )
+
     _ckeys = ":".join([payload.composite_keys["namespace"], payload.composite_keys["name"]])
     r_key = f"train::{_ckeys}"
 
     value = redis_client.get(r_key)
     if value:
         return False
 
-    redis_client.setex(r_key, time=EXPIRY, value=1)
+    redis_client.setex(r_key, time=redis_conf.expiry, value=1)
     return True
 
 
 def train(datums: List[Datum]) -> Responses:
     responses = Responses()
 
     for _datum in datums:
@@ -103,27 +104,30 @@
         if not is_new:
             _LOGGER.debug(
                 "%s - Skipping train request with keys: %s", payload.uuid, payload.composite_keys
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
-        metric_config = ConfigManager().get_metric_config(payload.composite_keys)
+        metric_config = ConfigManager.get_metric_config(payload.composite_keys)
         model_cfg = metric_config.numalogic_conf.model
 
         train_df = fetch_data(
-            payload, metric_config, {"namespace": payload.composite_keys["namespace"]}
+            payload,
+            metric_config,
+            {"namespace": payload.composite_keys["namespace"]},
+            hours=metric_config.train_hours,
         )
         train_df = clean_data(train_df)
 
-        if len(train_df) < MIN_TRAIN_SIZE:
+        if len(train_df) < metric_config.min_train_size:
             _LOGGER.warning(
                 "%s - Skipping training, train data less than minimum required: %s, df shape: %s",
                 payload.uuid,
-                MIN_TRAIN_SIZE,
+                metric_config.min_train_size,
                 train_df.shape,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
         preproc_cfg = metric_config.numalogic_conf.preprocess
         x_train, preproc_clf = _preprocess(train_df.to_numpy(), preproc_cfg)
```

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/udsink/train_rollout.py` & `numalogic_prometheus-0.3.2a0/numaprom/udsink/train_rollout.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,20 +16,15 @@
 from numaprom.entities import TrainerPayload
 from numaprom.clients.sentinel import get_redis_client
 from numaprom.tools import save_model, fetch_data
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
-HOST = os.getenv("REDIS_HOST")
-PORT = int(os.getenv("REDIS_PORT", 6379))
 AUTH = os.getenv("REDIS_AUTH")
-MASTERNAME = os.getenv("REDIS_MASTERNAME")
-EXPIRY = int(os.getenv("REDIS_EXPIRY", 360))
-MIN_TRAIN_SIZE = int(os.getenv("MIN_TRAIN_SIZE", 2000))
 
 
 # TODO: extract all good hashes, including when there are 2 hashes at a time
 # TODO avoid filling inf with nan, or at least throw warning
 def clean_data(df: pd.DataFrame, hash_col: str, limit=12) -> pd.DataFrame:
     df.replace([np.inf, -np.inf], np.nan, inplace=True)
     df = df.fillna(method="ffill", limit=limit)
@@ -86,22 +81,30 @@
     thresh_factory = ThresholdFactory()
     thresh_clf = thresh_factory.get_instance(thresh_cfg)
     thresh_clf.fit(x_reconerr)
     return thresh_clf
 
 
 def _is_new_request(payload: TrainerPayload) -> bool:
-    redis_client = get_redis_client(HOST, PORT, password=AUTH, mastername=MASTERNAME)
+    redis_conf = ConfigManager.get_redis_config()
+    redis_client = get_redis_client(
+        redis_conf.host,
+        redis_conf.port,
+        password=AUTH,
+        mastername=redis_conf.master_name,
+        recreate=False,
+    )
+
     _ckeys = ":".join([payload.composite_keys["namespace"], payload.composite_keys["name"]])
     r_key = f"trainrollout::{_ckeys}"
     value = redis_client.get(r_key)
     if value:
         return False
 
-    redis_client.setex(r_key, time=EXPIRY, value=1)
+    redis_client.setex(r_key, time=redis_conf.expiry, value=1)
     return True
 
 
 def train_rollout(datums: Iterator[Datum]) -> Responses:
     responses = Responses()
 
     for _datum in datums:
@@ -115,43 +118,44 @@
                 "%s - Skipping rollouts train request with keys: %s",
                 payload.uuid,
                 payload.composite_keys,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
-        metric_config = ConfigManager().get_metric_config(payload.composite_keys)
+        metric_config = ConfigManager.get_metric_config(payload.composite_keys)
         model_cfg = metric_config.numalogic_conf.model
 
         # ToDo: standardize the label name
         if "rollouts_pod_template_hash" in payload.composite_keys:
             hash_label = "rollouts_pod_template_hash"
         else:
             hash_label = "hash_id"
 
         train_df = fetch_data(
             payload,
             metric_config,
             {"namespace": payload.composite_keys["namespace"]},
             return_labels=[hash_label],
+            hours=metric_config.train_hours,
         )
         try:
             train_df = clean_data(train_df, hash_label)
         except KeyError:
             _LOGGER.error(
                 "%s - KeyError while data cleaning for train payload: %s", payload.uuid, payload
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
-        if len(train_df) < MIN_TRAIN_SIZE:
+        if len(train_df) < metric_config.min_train_size:
             _LOGGER.warning(
                 "%s - Skipping training, train data less than minimum required: %s, df shape: %s",
                 payload.uuid,
-                MIN_TRAIN_SIZE,
+                metric_config.min_train_size,
                 train_df.shape,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
         preproc_cfgs = metric_config.numalogic_conf.preprocess
         x_train, preproc_clf = _preprocess(train_df.to_numpy(), preproc_cfgs)
```

### Comparing `numalogic_prometheus-0.3.1a0/numaprom/watcher.py` & `numalogic_prometheus-0.3.2a0/numaprom/watcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,49 +4,55 @@
 from typing import Optional
 
 from omegaconf import OmegaConf
 from watchdog.observers import Observer
 from numalogic.config import NumalogicConf
 from watchdog.events import FileSystemEventHandler
 
+from numaprom._config import PipelineConf, RedisConf, PrometheusConf, RegistryConf
 from numaprom._constants import CONFIG_DIR, DEFAULT_CONFIG_DIR
-from numaprom import NumapromConf, get_logger, AppConf, MetricConf, UnifiedConf
+from numaprom import DataConf, get_logger, AppConf, MetricConf, UnifiedConf
 
 _LOGGER = get_logger(__name__)
 
 
 class ConfigManager:
     config = {}
 
     @staticmethod
     def load_configs():
-        schema: NumapromConf = OmegaConf.structured(NumapromConf)
+        schema: DataConf = OmegaConf.structured(DataConf)
 
         conf = OmegaConf.load(os.path.join(CONFIG_DIR, "config.yaml"))
         app_configs = OmegaConf.merge(schema, conf).configs
 
         conf = OmegaConf.load(os.path.join(DEFAULT_CONFIG_DIR, "config.yaml"))
         default_configs = OmegaConf.merge(schema, conf).configs
 
         conf = OmegaConf.load(os.path.join(DEFAULT_CONFIG_DIR, "numalogic_config.yaml"))
         schema: NumalogicConf = OmegaConf.structured(NumalogicConf)
         default_numalogic = OmegaConf.merge(schema, conf)
 
-        return app_configs, default_configs, default_numalogic
+        conf = OmegaConf.load(os.path.join(DEFAULT_CONFIG_DIR, "pipeline_config.yaml"))
+        schema: PipelineConf = OmegaConf.structured(PipelineConf)
+        pipeline_config = OmegaConf.merge(schema, conf)
+
+        return app_configs, default_configs, default_numalogic, pipeline_config
 
     @classmethod
     def update_configs(cls):
-        app_configs, default_configs, default_numalogic = cls.load_configs()
+        app_configs, default_configs, default_numalogic, pipeline_config = cls.load_configs()
 
         cls.config["app_configs"] = dict()
         for _config in app_configs:
             cls.config["app_configs"][_config.namespace] = _config
 
         cls.config["default_configs"] = dict(map(lambda c: (c.namespace, c), default_configs))
         cls.config["default_numalogic"] = default_numalogic
+        cls.config["pipeline_config"] = pipeline_config
 
         _LOGGER.info("Successfully updated configs - %s", cls.config)
         return cls.config
 
     @classmethod
     @lru_cache(maxsize=100)
     def get_app_config(cls, metric: str, namespace: str) -> Optional[AppConf]:
@@ -100,18 +106,36 @@
                 app_config.unified_configs,
             )
         )
         if not unified_config:
             return None
         return unified_config[0]
 
+    @classmethod
+    def get_pipeline_config(cls) -> PipelineConf:
+        if not cls.config:
+            cls.update_configs()
+        return cls.config["pipeline_config"]
+
+    @classmethod
+    def get_redis_config(cls) -> RedisConf:
+        return cls.get_pipeline_config().redis_conf
+
+    @classmethod
+    def get_prometheus_config(cls) -> PrometheusConf:
+        return cls.get_pipeline_config().prometheus_conf
+
+    @classmethod
+    def get_registry_config(cls) -> RegistryConf:
+        return cls.get_pipeline_config().registry_conf
+
 
 class ConfigHandler(FileSystemEventHandler):
     def ___init__(self):
-        self.config_manger = ConfigManager()
+        self.config_manger = ConfigManager
 
     def on_any_event(self, event):
         if event.event_type == "created" or event.event_type == "modified":
             _file = os.path.basename(event.src_path)
             _dir = os.path.basename(os.path.dirname(event.src_path))
 
             _LOGGER.info("Watchdog received %s event - %s/%s", event.event_type, _dir, _file)
```

### Comparing `numalogic_prometheus-0.3.1a0/pyproject.toml` & `numalogic_prometheus-0.3.2a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic-prometheus"
-version = "0.3.1a0"
+version = "0.3.2a0"
 description = "ML inference on numaflow using numalogic on Prometheus metrics"
 authors = ["Numalogic developers"]
 packages = [{ include = "numaprom" }]
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Nandita Koppisetty <nandita.iitkgp@gmail.com>",
 ]
```

### Comparing `numalogic_prometheus-0.3.1a0/PKG-INFO` & `numalogic_prometheus-0.3.2a0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic-prometheus
-Version: 0.3.1a0
+Version: 0.3.2a0
 Summary: ML inference on numaflow using numalogic on Prometheus metrics
 Home-page: https://github.com/numaproj/numalogic-prometheus
 Author: Numalogic developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
```


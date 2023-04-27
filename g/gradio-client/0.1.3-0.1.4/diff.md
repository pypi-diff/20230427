# Comparing `tmp/gradio_client-0.1.3.tar.gz` & `tmp/gradio_client-0.1.4.tar.gz`

## Comparing `gradio_client-0.1.3.tar` & `gradio_client-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.1.3/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.1.3/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.1.3/gradio_client/__init__.py
--rw-r--r--   0        0        0    45304 2020-02-02 00:00:00.000000 gradio_client-0.1.3/gradio_client/client.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.1.3/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 gradio_client-0.1.3/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.1.3/gradio_client/media_data.py
--rw-r--r--   0        0        0    20110 2020-02-02 00:00:00.000000 gradio_client-0.1.3/gradio_client/serializing.py
--rw-r--r--   0        0        0    13725 2020-02-02 00:00:00.000000 gradio_client-0.1.3/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.1.3/gradio_client/version.txt
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.1.3/.gitignore
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.1.4/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/__init__.py
+-rw-r--r--   0        0        0    46264 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/client.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/media_data.py
+-rw-r--r--   0        0        0    20110 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/serializing.py
+-rw-r--r--   0        0        0    14633 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/version.txt
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.1.4/PKG-INFO
```

### Comparing `gradio_client-0.1.3/README.md` & `gradio_client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.3/gradio_client/client.py` & `gradio_client-0.1.4/gradio_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from gradio_client.documentation import document, set_documentation_group
 from gradio_client.serializing import Serializable
 from gradio_client.utils import Communicator, JobStatus, Status, StatusUpdate
 
 set_documentation_group("py-client")
 
 
-@document("predict", "submit", "view_api")
+@document("predict", "submit", "view_api", "duplicate")
 class Client:
     """
     The main Client class for the Python client. This class is used to connect to a remote Gradio app and call its API endpoints.
 
     Example:
         from gradio_client import Client
 
@@ -47,15 +47,14 @@
         client.predict("test.mp4", api_name="/predict")
         >> What a nice recording! # returns the result of the remote API call
 
         client = Client("https://bec81a83-5b5c-471e.gradio.live")  # connecting to a temporary Gradio share URL
         job = client.submit("hello", api_name="/predict")  # runs the prediction in a background thread
         job.result()
         >> 49 # returns the result of the remote API call (blocking call)
-
     """
 
     def __init__(
         self,
         src: str,
         hf_token: str | None = None,
         max_workers: int = 40,
@@ -156,14 +155,21 @@
             hf_token: The Hugging Face token to use to access private Spaces. Automatically fetched if you are logged in via the Hugging Face Hub CLI. Obtain from: https://huggingface.co/settings/token
             private: Whether the new Space should be private (True) or public (False). Defaults to True.
             hardware: The hardware tier to use for the new Space. Defaults to the same hardware tier as the original Space. Options include "cpu-basic", "cpu-upgrade", "t4-small", "t4-medium", "a10g-small", "a10g-large", "a100-large", subject to availability.
             secrets: A dictionary of (secret key, secret value) to pass to the new Space. Defaults to None. Secrets are only used when the Space is duplicated for the first time, and are not updated if the duplicated Space already exists.
             sleep_timeout: The number of minutes after which the duplicate Space will be puased if no requests are made to it (to minimize billing charges). Defaults to 5 minutes.
             max_workers: The maximum number of thread workers that can be used to make requests to the remote Gradio app simultaneously.
             verbose: Whether the client should print statements to the console.
+        Example:
+            import os
+            from gradio_client import Client
+            HF_TOKEN = os.environ.get("HF_TOKEN")
+            client = Client.duplicate("abidlabs/whisper", hf_token=HF_TOKEN)
+            client.predict("audio_sample.wav")
+            >> "This is a test of the whisper speech recognition model."
         """
         try:
             original_info = huggingface_hub.get_space_runtime(from_id, token=hf_token)
         except RepositoryNotFoundError:
             raise ValueError(
                 f"Could not find Space: {from_id}. If it is a private Space, please provide an `hf_token`."
             )
@@ -405,30 +411,31 @@
                 utils.SPACE_FETCHER_URL,
                 json={"serialize": self.serialize, "config": json.dumps(self.config)},
             )
             if fetch.ok:
                 info = fetch.json()["api"]
             else:
                 raise ValueError(f"Could not fetch api info for {self.src}")
-
         num_named_endpoints = len(info["named_endpoints"])
         num_unnamed_endpoints = len(info["unnamed_endpoints"])
         if num_named_endpoints == 0 and all_endpoints is None:
             all_endpoints = True
 
         human_info = "Client.predict() Usage Info\n---------------------------\n"
         human_info += f"Named API endpoints: {num_named_endpoints}\n"
 
         for api_name, endpoint_info in info["named_endpoints"].items():
             human_info += self._render_endpoints_info(api_name, endpoint_info)
 
         if all_endpoints:
             human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}\n"
             for fn_index, endpoint_info in info["unnamed_endpoints"].items():
-                human_info += self._render_endpoints_info(fn_index, endpoint_info)
+                # When loading from json, the fn_indices are read as strings
+                # because json keys can only be strings
+                human_info += self._render_endpoints_info(int(fn_index), endpoint_info)
         else:
             if num_unnamed_endpoints > 0:
                 human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}, to view, run Client.view_api(`all_endpoints=True`)\n"
 
         if print_info:
             print(human_info)
         if return_format == "str":
@@ -939,15 +946,19 @@
         else:
             with self.communicator.lock:
                 return self.communicator.job.outputs
 
     def status(self) -> StatusUpdate:
         """
         Returns the latest status update from the Job in the form of a StatusUpdate
-        object, which contains the following fields: code, rank, queue_size, success, time, eta.
+        object, which contains the following fields: code, rank, queue_size, success, time, eta, and progress_data.
+
+        progress_data is a list of updates emitted by the gr.Progress() tracker of the event handler. Each element
+        of the list has the following fields: index, length, unit, progress, desc. If the event handler does not have
+        a gr.Progress() tracker, the progress_data field will be None.
 
         Example:
             from gradio_client import Client
             client = Client(src="gradio/calculator")
             job = client.submit(5, "add", 4, api_name="/predict")
             job.status()
             >> <Status.STARTING: 'STARTING'>
@@ -963,43 +974,47 @@
             return StatusUpdate(
                 code=Status.CANCELLED,
                 rank=0,
                 queue_size=None,
                 success=False,
                 time=time,
                 eta=None,
+                progress_data=None,
             )
         if self.done():
             if not self.future._exception:  # type: ignore
                 return StatusUpdate(
                     code=Status.FINISHED,
                     rank=0,
                     queue_size=None,
                     success=True,
                     time=time,
                     eta=None,
+                    progress_data=None,
                 )
             else:
                 return StatusUpdate(
                     code=Status.FINISHED,
                     rank=0,
                     queue_size=None,
                     success=False,
                     time=time,
                     eta=None,
+                    progress_data=None,
                 )
         else:
             if not self.communicator:
                 return StatusUpdate(
                     code=Status.PROCESSING,
                     rank=0,
                     queue_size=None,
                     success=None,
                     time=time,
                     eta=None,
+                    progress_data=None,
                 )
             else:
                 with self.communicator.lock:
                     eta = self.communicator.job.latest_status.eta
                     if self.verbose and self.space_id and eta and eta > 30:
                         print(
                             f"Due to heavy traffic on this app, the prediction will take approximately {int(eta)} seconds."
```

### Comparing `gradio_client-0.1.3/gradio_client/documentation.py` & `gradio_client-0.1.4/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.3/gradio_client/media_data.py` & `gradio_client-0.1.4/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.3/gradio_client/serializing.py` & `gradio_client-0.1.4/gradio_client/serializing.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.3/gradio_client/utils.py` & `gradio_client-0.1.4/gradio_client/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import tempfile
 from concurrent.futures import CancelledError
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from threading import Lock
-from typing import Any, Callable, Dict, List, Tuple
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import fsspec.asyn
 import httpx
 import huggingface_hub
 import requests
 from huggingface_hub import SpaceStage
 from websockets.legacy.protocol import WebSocketCommonProtocol
@@ -73,29 +73,31 @@
     """Status codes presented to client users."""
 
     STARTING = "STARTING"
     JOINING_QUEUE = "JOINING_QUEUE"
     QUEUE_FULL = "QUEUE_FULL"
     IN_QUEUE = "IN_QUEUE"
     SENDING_DATA = "SENDING_DATA"
-    PROCESSING = "PROCESSSING"
+    PROCESSING = "PROCESSING"
     ITERATING = "ITERATING"
+    PROGRESS = "PROGRESS"
     FINISHED = "FINISHED"
     CANCELLED = "CANCELLED"
 
     @staticmethod
     def ordering(status: "Status") -> int:
         """Order of messages. Helpful for testing."""
         order = [
             Status.STARTING,
             Status.JOINING_QUEUE,
             Status.QUEUE_FULL,
             Status.IN_QUEUE,
             Status.SENDING_DATA,
             Status.PROCESSING,
+            Status.PROGRESS,
             Status.ITERATING,
             Status.FINISHED,
             Status.CANCELLED,
         ]
         return order.index(status)
 
     def __lt__(self, other: "Status"):
@@ -108,37 +110,62 @@
             "send_hash": Status.JOINING_QUEUE,
             "queue_full": Status.QUEUE_FULL,
             "estimation": Status.IN_QUEUE,
             "send_data": Status.SENDING_DATA,
             "process_starts": Status.PROCESSING,
             "process_generating": Status.ITERATING,
             "process_completed": Status.FINISHED,
+            "progress": Status.PROGRESS,
         }[msg]
 
 
 @dataclass
+class ProgressUnit:
+    index: Optional[int]
+    length: Optional[int]
+    unit: Optional[str]
+    progress: Optional[float]
+    desc: Optional[str]
+
+    @classmethod
+    def from_ws_msg(cls, data: List[Dict]) -> List["ProgressUnit"]:
+        return [
+            cls(
+                index=d.get("index"),
+                length=d.get("length"),
+                unit=d.get("unit"),
+                progress=d.get("progress"),
+                desc=d.get("desc"),
+            )
+            for d in data
+        ]
+
+
+@dataclass
 class StatusUpdate:
     """Update message sent from the worker thread to the Job on the main thread."""
 
     code: Status
     rank: int | None
     queue_size: int | None
     eta: float | None
     success: bool | None
     time: datetime | None
+    progress_data: List[ProgressUnit] | None
 
 
 def create_initial_status_update():
     return StatusUpdate(
         code=Status.STARTING,
         rank=None,
         queue_size=None,
         eta=None,
         success=None,
         time=datetime.now(),
+        progress_data=None,
     )
 
 
 @dataclass
 class JobStatus:
     """The job status.
 
@@ -205,21 +232,25 @@
                         raise CancelledError()
             # Need to suspend this coroutine so that task actually runs
             await asyncio.sleep(0.01)
         msg = task.result()
         resp = json.loads(msg)
         if helper:
             with helper.lock:
+                has_progress = "progress_data" in resp
                 status_update = StatusUpdate(
                     code=Status.msg_to_status(resp["msg"]),
                     queue_size=resp.get("queue_size"),
                     rank=resp.get("rank", None),
                     success=resp.get("success"),
                     time=datetime.now(),
                     eta=resp.get("rank_eta"),
+                    progress_data=ProgressUnit.from_ws_msg(resp["progress_data"])
+                    if has_progress
+                    else None,
                 )
                 output = resp.get("output", {}).get("data", [])
                 if output and status_update.code != Status.FINISHED:
                     try:
                         result = helper.deserialize(*output)
                     except Exception as e:
                         result = [e]
```

### Comparing `gradio_client-0.1.3/.gitignore` & `gradio_client-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.3/pyproject.toml` & `gradio_client-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.3/PKG-INFO` & `gradio_client-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Requires-Python: >=3.7
 Requires-Dist: fsspec
```


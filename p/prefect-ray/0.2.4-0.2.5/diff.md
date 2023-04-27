# Comparing `tmp/prefect-ray-0.2.4.tar.gz` & `tmp/prefect-ray-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-ray/prefect-ray/dist/.tmp-er_knrc8/prefect-ray-0.2.4.tar", last modified: Tue Feb 21 20:23:08 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-ray/prefect-ray/dist/.tmp-w999k4n4/prefect-ray-0.2.5.tar", last modified: Thu Apr 27 17:10:46 2023, max compression
```

## Comparing `prefect-ray-0.2.4.tar` & `prefect-ray-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/prefect_ray/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/prefect_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/prefect_ray/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/prefect_ray/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/prefect_ray/task_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/prefect_ray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/prefect_ray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/prefect_ray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/prefect_ray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/prefect_ray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/prefect_ray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:23:08.000000 prefect-ray-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/tests/test_task_runners.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-02-21 20:20:55.000000 prefect-ray-0.2.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/prefect_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/prefect_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/prefect_ray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/prefect_ray/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/prefect_ray/task_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/prefect_ray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/prefect_ray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/prefect_ray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/prefect_ray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/prefect_ray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/prefect_ray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:10:46.000000 prefect-ray-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/tests/test_task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-27 17:08:55.000000 prefect-ray-0.2.5/versioneer.py
```

### Comparing `prefect-ray-0.2.4/LICENSE` & `prefect-ray-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-ray-0.2.4/PKG-INFO` & `prefect-ray-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-ray
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations with the Ray execution framework.
 Home-page: https://github.com/PrefectHQ/prefect-ray
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-ray-0.2.4/README.md` & `prefect-ray-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prefect-ray-0.2.4/prefect_ray/context.py` & `prefect-ray-0.2.5/prefect_ray/context.py`

 * *Files identical despite different names*

### Comparing `prefect-ray-0.2.4/prefect_ray/task_runners.py` & `prefect-ray-0.2.5/prefect_ray/task_runners.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,80 +120,108 @@
         init_kwargs: dict = None,
     ):
         # Store settings
         self.address = address
         self.init_kwargs = init_kwargs.copy() if init_kwargs else {}
 
         self.init_kwargs.setdefault("namespace", "prefect")
-        self.init_kwargs
 
         # Runtime attributes
         self._ray_refs: Dict[str, "ray.ObjectRef"] = {}
 
         super().__init__()
 
+    def duplicate(self):
+        """
+        Return a new instance of with the same settings as this one.
+        """
+        return type(self)(address=self.address, init_kwargs=self.init_kwargs)
+
+    def __eq__(self, other: object) -> bool:
+        """
+        Check if an instance has the same settings as this task runner.
+        """
+        if type(self) == type(other):
+            return (
+                self.address == other.address and self.init_kwargs == other.init_kwargs
+            )
+        else:
+            return NotImplemented
+
     @property
     def concurrency_type(self) -> TaskConcurrencyType:
         return TaskConcurrencyType.PARALLEL
 
     async def submit(
         self,
         key: UUID,
         call: Callable[..., Awaitable[State[R]]],
     ) -> None:
         if not self._started:
             raise RuntimeError(
                 "The task runner must be started before submitting work."
             )
 
-        call_kwargs = self._exchange_prefect_for_ray_futures(call.keywords)
+        call_kwargs, upstream_ray_obj_refs = self._exchange_prefect_for_ray_futures(
+            call.keywords
+        )
 
         remote_options = RemoteOptionsContext.get().current_remote_options
         # Ray does not support the submission of async functions and we must create a
         # sync entrypoint
         if remote_options:
             ray_decorator = ray.remote(**remote_options)
         else:
             ray_decorator = ray.remote
+
         self._ray_refs[key] = ray_decorator(self._run_prefect_task).remote(
-            sync_compatible(call.func), **call_kwargs
+            sync_compatible(call.func), *upstream_ray_obj_refs, **call_kwargs
         )
 
     def _exchange_prefect_for_ray_futures(self, kwargs_prefect_futures):
         """Exchanges Prefect futures for Ray futures."""
 
+        upstream_ray_obj_refs = []
+
         def exchange_prefect_for_ray_future(expr):
             """Exchanges Prefect future for Ray future."""
             if isinstance(expr, PrefectFuture):
                 ray_future = self._ray_refs.get(expr.key)
                 if ray_future is not None:
+                    upstream_ray_obj_refs.append(ray_future)
                     return ray_future
             return expr
 
         kwargs_ray_futures = visit_collection(
             kwargs_prefect_futures,
             visit_fn=exchange_prefect_for_ray_future,
             return_data=True,
         )
 
-        return kwargs_ray_futures
+        return kwargs_ray_futures, upstream_ray_obj_refs
 
     @staticmethod
-    def _run_prefect_task(func, *args, **kwargs):
-        """Resolves Ray futures before calling the actual Prefect task function."""
+    def _run_prefect_task(func, *upstream_ray_obj_refs, **kwargs):
+        """Resolves Ray futures before calling the actual Prefect task function.
+
+        Passing upstream_ray_obj_refs directly as args enables Ray to wait for
+        upstream tasks before running this remote function.
+        This variable is otherwise unused as the ray object refs are also
+        contained in kwargs.
+        """
 
         def resolve_ray_future(expr):
             """Resolves Ray future."""
             if isinstance(expr, ray.ObjectRef):
                 return ray.get(expr)
             return expr
 
         kwargs = visit_collection(kwargs, visit_fn=resolve_ray_future, return_data=True)
 
-        return func(*args, **kwargs)
+        return func(**kwargs)
 
     async def wait(self, key: UUID, timeout: float = None) -> Optional[State]:
         ref = self._get_ray_ref(key)
 
         result = None
 
         with anyio.move_on_after(timeout):
```

### Comparing `prefect-ray-0.2.4/prefect_ray.egg-info/PKG-INFO` & `prefect-ray-0.2.5/prefect_ray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-ray
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations with the Ray execution framework.
 Home-page: https://github.com/PrefectHQ/prefect-ray
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-ray-0.2.4/setup.cfg` & `prefect-ray-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-ray-0.2.4/setup.py` & `prefect-ray-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-ray-0.2.4/tests/test_block_standards.py` & `prefect-ray-0.2.5/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-ray-0.2.4/tests/test_context.py` & `prefect-ray-0.2.5/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `prefect-ray-0.2.4/tests/test_task_runners.py` & `prefect-ray-0.2.5/tests/test_task_runners.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 import prefect
 import prefect.engine
 import pytest
 import ray
 import ray.cluster_utils
 from prefect import flow, get_run_logger, task
 from prefect.states import State
-from prefect.testing.fixtures import hosted_orion_api, use_hosted_orion  # noqa: F401
+from prefect.testing.fixtures import (  # noqa: F401
+    hosted_api_server,
+    use_hosted_api_server,
+)
 from prefect.testing.standard_test_suites import TaskRunnerStandardTestSuite
 from prefect.testing.utilities import exceptions_equal
 from ray.exceptions import TaskCancelledError
 
 import tests
 from prefect_ray import RayTaskRunner
 from prefect_ray.context import remote_options
@@ -66,15 +69,15 @@
 @pytest.fixture(scope="module")
 def machine_ray_instance():
     """
     Starts a ray instance for the current machine
     """
     subprocess.check_call(
         ["ray", "start", "--head", "--include-dashboard", "False"],
-        cwd=str(prefect.__root_path__),
+        cwd=str(prefect.__development_base_path__),
     )
     try:
         yield "ray://127.0.0.1:10001"
     finally:
         subprocess.run(["ray", "stop"])
 
 
@@ -87,15 +90,15 @@
         warnings.simplefilter("ignore", ResourceWarning)
 
         yield RayTaskRunner()
 
 
 @pytest.fixture
 def ray_task_runner_with_existing_cluster(
-    machine_ray_instance, use_hosted_orion, hosted_orion_api  # noqa: F811
+    machine_ray_instance, use_hosted_api_server, hosted_api_server  # noqa: F811
 ):
     """
     Generate a ray task runner that's connected to a ray instance running in a separate
     process.
 
     This tests connection via `ray://` which is a client-based connection.
     """
@@ -122,15 +125,15 @@
         yield cluster
     finally:
         cluster.shutdown()
 
 
 @pytest.fixture
 def ray_task_runner_with_inprocess_cluster(
-    inprocess_ray_cluster, use_hosted_orion, hosted_orion_api  # noqa: F811
+    inprocess_ray_cluster, use_hosted_api_server, hosted_api_server  # noqa: F811
 ):
     """
     Generate a ray task runner that's connected to an in-process cluster.
 
     This tests connection via 'localhost' which is not a client-based connection.
     """
 
@@ -144,15 +147,15 @@
             }
         },
     )
 
 
 @pytest.fixture
 def ray_task_runner_with_temporary_cluster(
-    use_hosted_orion, hosted_orion_api  # noqa: F811
+    use_hosted_api_server, hosted_api_server  # noqa: F811
 ):
     """
     Generate a ray task runner that creates a temporary cluster.
 
     This tests connection via 'localhost' which is not a client-based connection.
     """
 
@@ -221,15 +224,14 @@
             (KeyboardInterrupt(), TaskCancelledError),
             (ValueError("test"), ValueError),
         ],
     )
     async def test_exception_to_crashed_state_in_flow_run(
         self, exceptions, task_runner, monkeypatch
     ):
-
         (raised_exception, state_exception_type) = exceptions
 
         async def throws_exception_before_task_begins(
             task, task_run, parameters, wait_for, result_factory, settings, **kwds
         ):
             """
             Simulates an exception occurring while a remote task runner is attempting
```

### Comparing `prefect-ray-0.2.4/versioneer.py` & `prefect-ray-0.2.5/versioneer.py`

 * *Files identical despite different names*


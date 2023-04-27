# Comparing `tmp/pyroscope-io-0.8.1.tar.gz` & `tmp/pyroscope-io-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscope-io-0.8.1.tar", last modified: Fri Jan 20 04:37:57 2023, max compression
+gzip compressed data, was "pyroscope-io-0.8.2.tar", last modified: Thu Apr 27 07:29:02 2023, max compression
```

## Comparing `pyroscope-io-0.8.1.tar` & `pyroscope-io-0.8.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 04:37:57.617043 pyroscope-io-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-01-20 04:37:57.617043 pyroscope-io-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 04:37:57.613043 pyroscope-io-0.8.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 04:37:57.613043 pyroscope-io-0.8.1/lib/.cargo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/lib/.cargo/config
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/lib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/lib/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/lib/cbindgen.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 04:37:57.613043 pyroscope-io-0.8.1/lib/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/lib/include/pyroscope_ffi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 04:37:57.613043 pyroscope-io-0.8.1/lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 04:37:57.613043 pyroscope-io-0.8.1/pyroscope/
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/pyroscope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 04:37:57.613043 pyroscope-io-0.8.1/pyroscope_io/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/pyroscope_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 04:37:57.613043 pyroscope-io-0.8.1/pyroscope_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-01-20 04:37:57.000000 pyroscope-io-0.8.1/pyroscope_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-01-20 04:37:57.000000 pyroscope-io-0.8.1/pyroscope_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 04:37:57.000000 pyroscope-io-0.8.1/pyroscope_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 04:37:57.000000 pyroscope-io-0.8.1/pyroscope_io.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-20 04:37:57.000000 pyroscope-io-0.8.1/pyroscope_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-20 04:37:57.000000 pyroscope-io-0.8.1/pyroscope_io.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-20 04:37:57.617043 pyroscope-io-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-01-20 04:37:49.000000 pyroscope-io-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.107032 pyroscope-io-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-27 07:29:02.107032 pyroscope-io-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/lib/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/.cargo/config
+-rw-r--r--   0 runner    (1001) docker     (123)    63646 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/cbindgen.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/lib/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/include/pyroscope_ffi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/pyroscope/
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/pyroscope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/pyroscope_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/pyroscope_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.107032 pyroscope-io-0.8.2/pyroscope_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-27 07:29:02.107032 pyroscope-io-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/setup.py
```

### Comparing `pyroscope-io-0.8.1/LICENSE` & `pyroscope-io-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.1/PKG-INFO` & `pyroscope-io-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscope-io
-Version: 0.8.1
+Version: 0.8.2
 Summary: Pyroscope Python integration
 Home-page: https://pyroscope.io
 Maintainer: Abid Omar
 Maintainer-email: contact@pyroscope.io
 License: Apache 2.0
 Project-URL: Documentation, https://pyroscope.io
 Project-URL: Bug Tracker, https://pyroscope.io
@@ -91,9 +91,7 @@
 with pyroscope.tag_wrapper({ "controller": "slow_controller_i_want_to_profile" }):
   slow_code()
 ```
 
 ### Example
 
 Check out this [example python project in our repository](https://github.com/pyroscope-io/pyroscope/tree/main/examples/python) for examples of how you can use these features.
-
-
```

### Comparing `pyroscope-io-0.8.1/README.md` & `pyroscope-io-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.1/lib/cbindgen.toml` & `pyroscope-io-0.8.2/lib/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.1/lib/src/lib.rs` & `pyroscope-io-0.8.2/lib/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -3,48 +3,63 @@
 use pyroscope::PyroscopeAgent;
 use pyroscope_pyspy::{pyspy_backend, PyspyConfig};
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::CStr;
 use std::hash::Hasher;
 use std::os::raw::c_char;
 
+const LOG_TAG: &str = "Pyroscope::pyspy::ffi";
+
 #[no_mangle]
 pub extern "C" fn initialize_logging(logging_level: u32) -> bool {
     // Force rustc to display the log messages in the console.
     match logging_level {
         50 => {
-            std::env::set_var("RUST_LOG", "error");
+            std::env::set_var("RUST_LOG", "off");
         }
         40 => {
-            std::env::set_var("RUST_LOG", "warn");
+            std::env::set_var("RUST_LOG", "error");
         }
         30 => {
-            std::env::set_var("RUST_LOG", "info");
+            std::env::set_var("RUST_LOG", "warn");
         }
         20 => {
-            std::env::set_var("RUST_LOG", "debug");
+            std::env::set_var("RUST_LOG", "info");
         }
         10 => {
-            std::env::set_var("RUST_LOG", "trace");
+            std::env::set_var("RUST_LOG", "debug");
         }
         _ => {
             std::env::set_var("RUST_LOG", "debug");
         }
     }
 
     // Initialize the logger.
     pretty_env_logger::init_timed();
     true
 }
 
 #[no_mangle]
 pub extern "C" fn initialize_agent(
-    application_name: *const c_char, server_address: *const c_char, auth_token: *const c_char,
-    sample_rate: u32, detect_subprocesses: bool, oncpu: bool, native: bool, gil_only: bool,
-    report_pid: bool, report_thread_id: bool, report_thread_name: bool, tags: *const c_char,
+    application_name: *const c_char,
+    server_address: *const c_char,
+    auth_token: *const c_char,
+    basic_auth_username: *const c_char,
+    basic_auth_password: *const c_char,
+    sample_rate: u32,
+    detect_subprocesses: bool,
+    oncpu: bool,
+    native: bool,
+    gil_only: bool,
+    report_pid: bool,
+    report_thread_id: bool,
+    report_thread_name: bool,
+    tags: *const c_char,
+    scope_org_id: *const c_char,
+    http_headers_json: *const c_char,
 ) -> bool {
     // Initialize FFIKit
     let recv = ffikit::initialize_ffi().unwrap();
 
     // application_name
     let application_name = unsafe { CStr::from_ptr(application_name) }
         .to_str()
@@ -53,26 +68,45 @@
 
     // server_address
     let server_address = unsafe { CStr::from_ptr(server_address) }
         .to_str()
         .unwrap()
         .to_string();
 
-    // auth_token
     let auth_token = unsafe { CStr::from_ptr(auth_token) }
         .to_str()
         .unwrap()
         .to_string();
 
+    let basic_auth_username = unsafe { CStr::from_ptr(basic_auth_username) }
+        .to_str()
+        .unwrap()
+        .to_string();
+
+    let basic_auth_password = unsafe { CStr::from_ptr(basic_auth_password) }
+        .to_str()
+        .unwrap()
+        .to_string();
+
     // tags
     let tags_string = unsafe { CStr::from_ptr(tags) }
         .to_str()
         .unwrap()
         .to_string();
 
+    let scope_org_id = unsafe { CStr::from_ptr(scope_org_id) }
+        .to_str()
+        .unwrap()
+        .to_string();
+
+    let http_headers_json = unsafe { CStr::from_ptr(http_headers_json) }
+        .to_str()
+        .unwrap()
+        .to_string();
+
     let pid = std::process::id();
 
     // Configure the Pyspy Backend.
     let mut pyspy_config = PyspyConfig::new(pid.try_into().unwrap())
         .sample_rate(sample_rate)
         .lock_process(false)
         .detect_subprocesses(detect_subprocesses)
@@ -106,14 +140,37 @@
     let mut agent_builder = PyroscopeAgent::builder(server_address, application_name)
         .backend(pyspy)
         .tags(tags);
 
     // Add the auth token if it is not empty.
     if auth_token != "" {
         agent_builder = agent_builder.auth_token(auth_token);
+    } else if basic_auth_username != "" && basic_auth_password != "" {
+        agent_builder = agent_builder.basic_auth(basic_auth_username, basic_auth_password);
+    }
+    if scope_org_id != "" {
+        agent_builder = agent_builder.scope_org_id(scope_org_id);
+    }
+
+    let http_headers = pyroscope::pyroscope::parse_http_headers_json(http_headers_json);
+    match http_headers {
+        Ok(http_headers) => {
+            agent_builder = agent_builder.http_headers(http_headers);
+        }
+        Err(e) => {
+            match e {
+                pyroscope::PyroscopeError::Json(e) => {
+                    log::error!(target: LOG_TAG, "parse_http_headers_json error {}", e);
+                }
+                pyroscope::PyroscopeError::AdHoc(e) => {
+                    log::error!(target: LOG_TAG, "parse_http_headers_json {}", e);
+                }
+                _ => {}
+            }
+        }
     }
 
     // Build the agent.
     let agent = agent_builder.build().unwrap();
 
     // Start the agent.
     let agent_running = agent.start().unwrap();
```

### Comparing `pyroscope-io-0.8.1/pyroscope/__init__.py` & `pyroscope-io-0.8.2/pyroscope/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,64 @@
 import threading
 import warnings
 import logging
+import json
 from collections import namedtuple
 from pyroscope._native import ffi, lib
 from contextlib import contextmanager 
 
 
-Config = namedtuple('Config', ('app_name', 'application_name',
-    'server_address', 'auth_token', 'enable_logging', 'sample_rate', 'detect_subprocesses','oncpu', 'native', 'gil_only'))
+def configure(
+        app_name=None,
+        application_name=None,
+        server_address="http://localhost:4040",
+        auth_token="",
+        basic_auth_username="",
+        basic_auth_password="",
+        enable_logging=False,
+        sample_rate=100,
+        detect_subprocesses=False,
+        oncpu=True,
+        native=False,
+        gil_only=True,
+        report_pid=False,
+        report_thread_id=False,
+        report_thread_name=False,
+        tags=None,
+        scope_org_id="",
+        http_headers=None,
+):
 
-def configure(app_name=None, application_name=None, server_address="http://localhost:4040",
-        auth_token="", enable_logging=False, sample_rate=100, detect_subprocesses=False,
-        oncpu=True, native=False, gil_only=True, report_pid=False, report_thread_id=False,
-        report_thread_name=False, tags=None): 
-
-    # app_name deprecation warning
     if app_name is not None:
         warnings.warn("app_name is deprecated, use application_name", DeprecationWarning)
         application_name = app_name
 
-    # Determine Logging level
-    #   Python Logging levels
-    #   CRITICAL = 50
-    #   ERROR = 40
-    #   WARNING = 30
-    #   INFO = 20
-    #   DEBUG = 10
-    #   NOTSET = 0
     if enable_logging:
         logger = logging.getLogger()
         log_level = logger.getEffectiveLevel()
         lib.initialize_logging(log_level)
 
-    # Initialize Pyroscope Agent
-    lib.initialize_agent(application_name.encode("UTF-8"),
-            server_address.encode("UTF-8"), auth_token.encode("UTF-8"), sample_rate, detect_subprocesses,
-            oncpu, native, gil_only, report_pid, report_thread_id,
-            report_thread_name,
-            tags_to_string(tags).encode("UTF-8"))
+    lib.initialize_agent(
+        application_name.encode("UTF-8"),
+        server_address.encode("UTF-8"),
+        auth_token.encode("UTF-8"),
+        basic_auth_username.encode("UTF-8"),
+        basic_auth_password.encode("UTF-8"),
+        sample_rate,
+        detect_subprocesses,
+        oncpu,
+        native,
+        gil_only,
+        report_pid,
+        report_thread_id,
+        report_thread_name,
+        tags_to_string(tags).encode("UTF-8"),
+        (scope_org_id or "").encode("UTF-8"),
+        http_headers_to_json(http_headers).encode("UTF-8"),
+)
 
 def shutdown():
     drop = lib.drop_agent()
 
     if drop:
         logging.info("Pyroscope Agent successfully shutdown")
     else:
@@ -55,20 +72,24 @@
 
 def add_global_tag(thread_id, key, value):
     lib.add_global_tag(key.encode("UTF-8"), value.encode("UTF-8"))
 
 def remove_global_tag(key, value):
     lib.remove_global_tag(key.encode("UTF-8"), value.encode("UTF-8"))
 
-# Convert a struct of tags to a string
 def tags_to_string(tags):
     if tags is None:
         return ""
     return ",".join(["{}={}".format(key, value) for key, value in tags.items()])
 
+def http_headers_to_json(headers):
+    if headers is None:
+        return "{}"
+    return json.dumps(headers)
+
 @contextmanager
 def tag_wrapper(tags):
     for key, value in tags.items():
         lib.add_thread_tag(threading.get_ident(), key.encode("UTF-8"), value.encode("UTF-8"))
     try:
         yield
     finally:
```

### Comparing `pyroscope-io-0.8.1/pyroscope_io.egg-info/PKG-INFO` & `pyroscope-io-0.8.2/pyroscope_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscope-io
-Version: 0.8.1
+Version: 0.8.2
 Summary: Pyroscope Python integration
 Home-page: https://pyroscope.io
 Maintainer: Abid Omar
 Maintainer-email: contact@pyroscope.io
 License: Apache 2.0
 Project-URL: Documentation, https://pyroscope.io
 Project-URL: Bug Tracker, https://pyroscope.io
@@ -91,9 +91,7 @@
 with pyroscope.tag_wrapper({ "controller": "slow_controller_i_want_to_profile" }):
   slow_code()
 ```
 
 ### Example
 
 Check out this [example python project in our repository](https://github.com/pyroscope-io/pyroscope/tree/main/examples/python) for examples of how you can use these features.
-
-
```

### Comparing `pyroscope-io-0.8.1/setup.cfg` & `pyroscope-io-0.8.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyroscope-io
-version = 0.8.1
+version = 0.8.2
 description = Pyroscope Python integration
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pyroscope.io
 maintainer = Abid Omar
 maintainer_email = contact@pyroscope.io
 license = Apache 2.0
```

### Comparing `pyroscope-io-0.8.1/setup.py` & `pyroscope-io-0.8.2/setup.py`

 * *Files identical despite different names*


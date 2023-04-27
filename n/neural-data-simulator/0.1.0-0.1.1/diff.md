# Comparing `tmp/neural_data_simulator-0.1.0.tar.gz` & `tmp/neural_data_simulator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_data_simulator-0.1.0.tar", max compression
+gzip compressed data, was "neural_data_simulator-0.1.1.tar", max compression
```

## Comparing `neural_data_simulator-0.1.0.tar` & `neural_data_simulator-0.1.1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0    11339 2023-04-24 15:46:30.520844 neural_data_simulator-0.1.0/LICENSE
--rw-r--r--   0        0        0     2539 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      970 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/decoder/__init__.py
--rw-r--r--   0        0        0      999 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/decoder/config/settings_decoder.yaml
--rw-r--r--   0        0        0     7509 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/decoder/decoders.py
--rw-r--r--   0        0        0     4772 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/decoder/run_decoder.py
--rw-r--r--   0        0        0     2117 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/__init__.py
--rw-r--r--   0        0        0      607 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/config/lsl.config
--rw-r--r--   0        0        0     5069 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/config/settings.yaml
--rw-r--r--   0        0        0     1297 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/config/settings_streamer.yaml
--rw-r--r--   0        0        0     3797 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/encoder.py
--rw-r--r--   0        0        0    27831 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/ephys_generator.py
--rw-r--r--   0        0        0     9464 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/filters.py
--rw-r--r--   0        0        0     2573 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/health_checker.py
--rw-r--r--   0        0        0    11751 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/inputs.py
--rw-r--r--   0        0        0     1686 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/models.py
--rw-r--r--   0        0        0    13854 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/outputs.py
--rw-r--r--   0        0        0     3129 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/runner.py
--rw-r--r--   0        0        0     4198 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/samples.py
--rw-r--r--   0        0        0       65 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/scripts/__init__.py
--rw-r--r--   0        0        0      103 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/scripts/errors.py
--rw-r--r--   0        0        0     4579 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/scripts/post_install_config.py
--rw-r--r--   0        0        0     9483 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/scripts/run_encoder.py
--rw-r--r--   0        0        0     8718 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/scripts/run_ephys_generator.py
--rw-r--r--   0        0        0    11758 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/scripts/run_streamer.py
--rw-r--r--   0        0        0     6979 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/settings.py
--rw-r--r--   0        0        0     5498 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/streamers.py
--rw-r--r--   0        0        0     2739 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/timing.py
--rw-r--r--   0        0        0       56 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/util/__init__.py
--rw-r--r--   0        0        0     3775 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/util/buffer.py
--rw-r--r--   0        0        0      961 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/util/circular_dequeue.py
--rw-r--r--   0        0        0     2992 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/util/runtime.py
--rw-r--r--   0        0        0     1255 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/nds/util/settings_loader.py
--rw-r--r--   0        0        0       48 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/plugins/__init__.py
--rw-r--r--   0        0        0      964 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/plugins/examples/gamepad_preprocessor.py
--rw-r--r--   0        0        0     5190 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/plugins/examples/model.py
--rw-r--r--   0        0        0      536 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/plugins/examples/postprocessor.py
--rw-r--r--   0        0        0      462 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/plugins/examples/preprocessor.py
--rw-r--r--   0        0        0     3987 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/plugins/examples/tests/test_model.py
--rw-r--r--   0        0        0      288 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/recorder/__init__.py
--rw-r--r--   0        0        0     3183 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/recorder/run_recorder.py
--rw-r--r--   0        0        0      251 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/tasks/__init__.py
--rw-r--r--   0        0        0      872 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/tasks/center_out_reach/__init__.py
--rw-r--r--   0        0        0     2125 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/tasks/center_out_reach/buttons.py
--rw-r--r--   0        0        0     2734 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/tasks/center_out_reach/input_events.py
--rw-r--r--   0        0        0     1628 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/tasks/center_out_reach/joystick.py
--rw-r--r--   0        0        0     9783 2023-04-24 15:46:30.608844 neural_data_simulator-0.1.0/src/tasks/center_out_reach/metrics.py
--rw-r--r--   0        0        0     4049 2023-04-24 15:46:30.612844 neural_data_simulator-0.1.0/src/tasks/center_out_reach/scalers.py
--rw-r--r--   0        0        0     1583 2023-04-24 15:46:30.612844 neural_data_simulator-0.1.0/src/tasks/center_out_reach/screen_info.py
--rw-r--r--   0        0        0     2778 2023-04-24 15:46:30.612844 neural_data_simulator-0.1.0/src/tasks/center_out_reach/sprites.py
--rw-r--r--   0        0        0     6382 2023-04-24 15:46:30.612844 neural_data_simulator-0.1.0/src/tasks/center_out_reach/task_runner.py
--rw-r--r--   0        0        0    11351 2023-04-24 15:46:30.612844 neural_data_simulator-0.1.0/src/tasks/center_out_reach/task_state.py
--rw-r--r--   0        0        0    13007 2023-04-24 15:46:30.612844 neural_data_simulator-0.1.0/src/tasks/center_out_reach/task_window.py
--rw-r--r--   0        0        0     1593 2023-04-24 15:46:30.612844 neural_data_simulator-0.1.0/src/tasks/config/settings_center_out_reach.yaml
--rw-r--r--   0        0        0    11494 2023-04-24 15:46:30.612844 neural_data_simulator-0.1.0/src/tasks/run_center_out_reach.py
--rw-r--r--   0        0        0      837 2023-04-24 15:46:30.612844 neural_data_simulator-0.1.0/src/tasks/run_closed_loop.py
--rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 neural_data_simulator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-26 05:17:41.403203 neural_data_simulator-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1726 2023-04-26 05:17:41.403203 neural_data_simulator-0.1.1/README.md
+-rw-r--r--   0        0        0     3169 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      970 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/decoder/__init__.py
+-rw-r--r--   0        0        0      999 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/decoder/config/settings_decoder.yaml
+-rw-r--r--   0        0        0     7509 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/decoder/decoders.py
+-rw-r--r--   0        0        0     4772 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/decoder/run_decoder.py
+-rw-r--r--   0        0        0     2117 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/__init__.py
+-rw-r--r--   0        0        0      607 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/config/lsl.config
+-rw-r--r--   0        0        0     5069 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/config/settings.yaml
+-rw-r--r--   0        0        0     1297 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/config/settings_streamer.yaml
+-rw-r--r--   0        0        0     3797 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/encoder.py
+-rw-r--r--   0        0        0    27831 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/ephys_generator.py
+-rw-r--r--   0        0        0     9464 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/filters.py
+-rw-r--r--   0        0        0     2573 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/health_checker.py
+-rw-r--r--   0        0        0    11751 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/inputs.py
+-rw-r--r--   0        0        0     1686 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/models.py
+-rw-r--r--   0        0        0    13854 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/outputs.py
+-rw-r--r--   0        0        0     3129 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/runner.py
+-rw-r--r--   0        0        0     4198 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/samples.py
+-rw-r--r--   0        0        0       65 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/scripts/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/scripts/errors.py
+-rw-r--r--   0        0        0     4579 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/scripts/post_install_config.py
+-rw-r--r--   0        0        0     9483 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/scripts/run_encoder.py
+-rw-r--r--   0        0        0     8718 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/scripts/run_ephys_generator.py
+-rw-r--r--   0        0        0    11758 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/scripts/run_streamer.py
+-rw-r--r--   0        0        0     6979 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/settings.py
+-rw-r--r--   0        0        0     5498 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/streamers.py
+-rw-r--r--   0        0        0     2739 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/timing.py
+-rw-r--r--   0        0        0       56 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/util/__init__.py
+-rw-r--r--   0        0        0     3775 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/util/buffer.py
+-rw-r--r--   0        0        0      961 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/util/circular_dequeue.py
+-rw-r--r--   0        0        0     2992 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/util/runtime.py
+-rw-r--r--   0        0        0     1255 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/nds/util/settings_loader.py
+-rw-r--r--   0        0        0       48 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/plugins/__init__.py
+-rw-r--r--   0        0        0      964 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/plugins/examples/gamepad_preprocessor.py
+-rw-r--r--   0        0        0     5190 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/plugins/examples/model.py
+-rw-r--r--   0        0        0      536 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/plugins/examples/postprocessor.py
+-rw-r--r--   0        0        0      462 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/plugins/examples/preprocessor.py
+-rw-r--r--   0        0        0     3987 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/plugins/examples/tests/test_model.py
+-rw-r--r--   0        0        0      288 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/recorder/__init__.py
+-rw-r--r--   0        0        0     3183 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/recorder/run_recorder.py
+-rw-r--r--   0        0        0      251 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/__init__.py
+-rw-r--r--   0        0        0      872 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/center_out_reach/__init__.py
+-rw-r--r--   0        0        0     2125 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/center_out_reach/buttons.py
+-rw-r--r--   0        0        0     2734 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/center_out_reach/input_events.py
+-rw-r--r--   0        0        0     1628 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/center_out_reach/joystick.py
+-rw-r--r--   0        0        0     9783 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/center_out_reach/metrics.py
+-rw-r--r--   0        0        0     4049 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/center_out_reach/scalers.py
+-rw-r--r--   0        0        0     1583 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/center_out_reach/screen_info.py
+-rw-r--r--   0        0        0     2778 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/center_out_reach/sprites.py
+-rw-r--r--   0        0        0     6382 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/center_out_reach/task_runner.py
+-rw-r--r--   0        0        0    11351 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/center_out_reach/task_state.py
+-rw-r--r--   0        0        0    13007 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/center_out_reach/task_window.py
+-rw-r--r--   0        0        0     1593 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/config/settings_center_out_reach.yaml
+-rw-r--r--   0        0        0    11494 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/run_center_out_reach.py
+-rw-r--r--   0        0        0      837 2023-04-26 05:17:41.483204 neural_data_simulator-0.1.1/src/tasks/run_closed_loop.py
+-rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 neural_data_simulator-0.1.1/PKG-INFO
```

### Comparing `neural_data_simulator-0.1.0/LICENSE` & `neural_data_simulator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/pyproject.toml` & `neural_data_simulator-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 [tool.poetry]
 name = "neural-data-simulator"
-version = "0.1.0"
+version = "0.1.1"
 description = "Electrophysiology simulator data for developing Brain-Computer Interfaces"
-authors = ["AE Studio, Chadwick Boulay"]
+authors = ["AE Studio <bci@ae.studio>", "Chadwick Boulay <chadwick.boulay@gmail.com>"]
+maintainers = ["Chadwick Boulay <chadwick.boulay@gmail.com>", "AE Studio <bci@ae.studio>"]
 packages = [
     {include = "nds", from = "src"},
     {include = "decoder", from = "src"},
     {include = "recorder", from = "src"},
     {include = "tasks", from = "src"},
     {include = "plugins", from = "src"},
 ]
+readme = "README.md"
+license = "Apache-2.0"
+classifiers = [
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: MacOS",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/agencyenterprise/neural-data-simulator"
+"Documentation" = "https://agencyenterprise.github.io/neural-data-simulator/"
+"Bug Tracker" = "https://github.com/agencyenterprise/neural-data-simulator/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 numpy = "^1.22.4"
 pydantic = "^1.9.1"
 pylsl = "^1.16.1"
 colorednoise = "^2.1.0"
```

### Comparing `neural_data_simulator-0.1.0/src/decoder/__init__.py` & `neural_data_simulator-0.1.1/src/decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/decoder/config/settings_decoder.yaml` & `neural_data_simulator-0.1.1/src/decoder/config/settings_decoder.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/decoder/decoders.py` & `neural_data_simulator-0.1.1/src/decoder/decoders.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/decoder/run_decoder.py` & `neural_data_simulator-0.1.1/src/decoder/run_decoder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/__init__.py` & `neural_data_simulator-0.1.1/src/nds/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/config/lsl.config` & `neural_data_simulator-0.1.1/src/nds/config/lsl.config`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/config/settings.yaml` & `neural_data_simulator-0.1.1/src/nds/config/settings.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/config/settings_streamer.yaml` & `neural_data_simulator-0.1.1/src/nds/config/settings_streamer.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/encoder.py` & `neural_data_simulator-0.1.1/src/nds/encoder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/ephys_generator.py` & `neural_data_simulator-0.1.1/src/nds/ephys_generator.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/filters.py` & `neural_data_simulator-0.1.1/src/nds/filters.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/health_checker.py` & `neural_data_simulator-0.1.1/src/nds/health_checker.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/inputs.py` & `neural_data_simulator-0.1.1/src/nds/inputs.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/models.py` & `neural_data_simulator-0.1.1/src/nds/models.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/outputs.py` & `neural_data_simulator-0.1.1/src/nds/outputs.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/runner.py` & `neural_data_simulator-0.1.1/src/nds/runner.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/samples.py` & `neural_data_simulator-0.1.1/src/nds/samples.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/scripts/post_install_config.py` & `neural_data_simulator-0.1.1/src/nds/scripts/post_install_config.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/scripts/run_encoder.py` & `neural_data_simulator-0.1.1/src/nds/scripts/run_encoder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/scripts/run_ephys_generator.py` & `neural_data_simulator-0.1.1/src/nds/scripts/run_ephys_generator.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/scripts/run_streamer.py` & `neural_data_simulator-0.1.1/src/nds/scripts/run_streamer.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/settings.py` & `neural_data_simulator-0.1.1/src/nds/settings.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/streamers.py` & `neural_data_simulator-0.1.1/src/nds/streamers.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/timing.py` & `neural_data_simulator-0.1.1/src/nds/timing.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/util/buffer.py` & `neural_data_simulator-0.1.1/src/nds/util/buffer.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/util/circular_dequeue.py` & `neural_data_simulator-0.1.1/src/nds/util/circular_dequeue.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/util/runtime.py` & `neural_data_simulator-0.1.1/src/nds/util/runtime.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/nds/util/settings_loader.py` & `neural_data_simulator-0.1.1/src/nds/util/settings_loader.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/plugins/examples/gamepad_preprocessor.py` & `neural_data_simulator-0.1.1/src/plugins/examples/gamepad_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/plugins/examples/model.py` & `neural_data_simulator-0.1.1/src/plugins/examples/model.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/plugins/examples/postprocessor.py` & `neural_data_simulator-0.1.1/src/plugins/examples/postprocessor.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/plugins/examples/tests/test_model.py` & `neural_data_simulator-0.1.1/src/plugins/examples/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/recorder/run_recorder.py` & `neural_data_simulator-0.1.1/src/recorder/run_recorder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/center_out_reach/__init__.py` & `neural_data_simulator-0.1.1/src/tasks/center_out_reach/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/center_out_reach/buttons.py` & `neural_data_simulator-0.1.1/src/tasks/center_out_reach/buttons.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/center_out_reach/input_events.py` & `neural_data_simulator-0.1.1/src/tasks/center_out_reach/input_events.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/center_out_reach/joystick.py` & `neural_data_simulator-0.1.1/src/tasks/center_out_reach/joystick.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/center_out_reach/metrics.py` & `neural_data_simulator-0.1.1/src/tasks/center_out_reach/metrics.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/center_out_reach/scalers.py` & `neural_data_simulator-0.1.1/src/tasks/center_out_reach/scalers.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/center_out_reach/screen_info.py` & `neural_data_simulator-0.1.1/src/tasks/center_out_reach/screen_info.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/center_out_reach/sprites.py` & `neural_data_simulator-0.1.1/src/tasks/center_out_reach/sprites.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/center_out_reach/task_runner.py` & `neural_data_simulator-0.1.1/src/tasks/center_out_reach/task_runner.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/center_out_reach/task_state.py` & `neural_data_simulator-0.1.1/src/tasks/center_out_reach/task_state.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/center_out_reach/task_window.py` & `neural_data_simulator-0.1.1/src/tasks/center_out_reach/task_window.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/config/settings_center_out_reach.yaml` & `neural_data_simulator-0.1.1/src/tasks/config/settings_center_out_reach.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/run_center_out_reach.py` & `neural_data_simulator-0.1.1/src/tasks/run_center_out_reach.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.0/src/tasks/run_closed_loop.py` & `neural_data_simulator-0.1.1/src/tasks/run_closed_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         import screeninfo  # noqa: F401
     except ImportError:
         print(
             "Not running closed loop because neural-data-simulator "
             "extras couldn't be imported"
         )
         print("Please reinstall neural-data-simulator with extras by running:")
-        print("pip install 'neural-data-simulator[extras]'")
+        print('pip install "neural-data-simulator[extras]"')
         return
 
     encoder = subprocess.Popen(["encoder"])
     ephys = subprocess.Popen(["ephys_generator"])
     decoder = subprocess.Popen(["decoder"])
     center_out_reach = subprocess.Popen(["center_out_reach"])
```


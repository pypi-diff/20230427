# Comparing `tmp/neural_data_simulator-0.1.2.tar.gz` & `tmp/neural_data_simulator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_data_simulator-0.1.2.tar", max compression
+gzip compressed data, was "neural_data_simulator-0.2.0.tar", max compression
```

## Comparing `neural_data_simulator-0.1.2.tar` & `neural_data_simulator-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    11339 2023-04-27 03:36:56.590837 neural_data_simulator-0.1.2/LICENSE
--rw-r--r--   0        0        0     1736 2023-04-27 03:36:56.590837 neural_data_simulator-0.1.2/README.md
--rw-r--r--   0        0        0     3173 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      970 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/decoder/__init__.py
--rw-r--r--   0        0        0      999 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/decoder/config/settings_decoder.yaml
--rw-r--r--   0        0        0     7509 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/decoder/decoders.py
--rw-r--r--   0        0        0     4772 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/decoder/run_decoder.py
--rw-r--r--   0        0        0     2117 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/__init__.py
--rw-r--r--   0        0        0      607 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/config/lsl.config
--rw-r--r--   0        0        0     5069 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/config/settings.yaml
--rw-r--r--   0        0        0     1297 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/config/settings_streamer.yaml
--rw-r--r--   0        0        0     3797 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/encoder.py
--rw-r--r--   0        0        0    27831 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/ephys_generator.py
--rw-r--r--   0        0        0     9464 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/filters.py
--rw-r--r--   0        0        0     2573 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/health_checker.py
--rw-r--r--   0        0        0    11751 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/inputs.py
--rw-r--r--   0        0        0     1686 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/models.py
--rw-r--r--   0        0        0    13854 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/outputs.py
--rw-r--r--   0        0        0     3129 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/runner.py
--rw-r--r--   0        0        0     4198 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/samples.py
--rw-r--r--   0        0        0       65 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/scripts/__init__.py
--rw-r--r--   0        0        0      103 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/scripts/errors.py
--rw-r--r--   0        0        0     4579 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/scripts/post_install_config.py
--rw-r--r--   0        0        0     9483 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/scripts/run_encoder.py
--rw-r--r--   0        0        0     8718 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/scripts/run_ephys_generator.py
--rw-r--r--   0        0        0    11758 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/scripts/run_streamer.py
--rw-r--r--   0        0        0     6979 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/settings.py
--rw-r--r--   0        0        0     5498 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/streamers.py
--rw-r--r--   0        0        0     2739 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/timing.py
--rw-r--r--   0        0        0       56 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/util/__init__.py
--rw-r--r--   0        0        0     3775 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/util/buffer.py
--rw-r--r--   0        0        0      961 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/util/circular_dequeue.py
--rw-r--r--   0        0        0     2992 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/util/runtime.py
--rw-r--r--   0        0        0     1255 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/nds/util/settings_loader.py
--rw-r--r--   0        0        0       48 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/plugins/__init__.py
--rw-r--r--   0        0        0      964 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/plugins/examples/gamepad_preprocessor.py
--rw-r--r--   0        0        0     5190 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/plugins/examples/model.py
--rw-r--r--   0        0        0      536 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/plugins/examples/postprocessor.py
--rw-r--r--   0        0        0      462 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/plugins/examples/preprocessor.py
--rw-r--r--   0        0        0     3987 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/plugins/examples/tests/test_model.py
--rw-r--r--   0        0        0      288 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/recorder/__init__.py
--rw-r--r--   0        0        0     3183 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/recorder/run_recorder.py
--rw-r--r--   0        0        0      251 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/__init__.py
--rw-r--r--   0        0        0      872 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/center_out_reach/__init__.py
--rw-r--r--   0        0        0     2125 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/center_out_reach/buttons.py
--rw-r--r--   0        0        0     2734 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/center_out_reach/input_events.py
--rw-r--r--   0        0        0     1628 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/center_out_reach/joystick.py
--rw-r--r--   0        0        0     9783 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/center_out_reach/metrics.py
--rw-r--r--   0        0        0     4049 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/center_out_reach/scalers.py
--rw-r--r--   0        0        0     1583 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/center_out_reach/screen_info.py
--rw-r--r--   0        0        0     2778 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/center_out_reach/sprites.py
--rw-r--r--   0        0        0     6382 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/center_out_reach/task_runner.py
--rw-r--r--   0        0        0    11351 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/center_out_reach/task_state.py
--rw-r--r--   0        0        0    13007 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/center_out_reach/task_window.py
--rw-r--r--   0        0        0     1593 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/config/settings_center_out_reach.yaml
--rw-r--r--   0        0        0    11494 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/run_center_out_reach.py
--rw-r--r--   0        0        0      837 2023-04-27 03:36:56.646839 neural_data_simulator-0.1.2/src/tasks/run_closed_loop.py
--rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 neural_data_simulator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-27 10:26:04.608077 neural_data_simulator-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1736 2023-04-27 10:26:04.608077 neural_data_simulator-0.2.0/README.md
+-rw-r--r--   0        0        0     3281 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      970 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/decoder/__init__.py
+-rw-r--r--   0        0        0      999 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/decoder/config/settings_decoder.yaml
+-rw-r--r--   0        0        0     7657 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/decoder/decoders.py
+-rw-r--r--   0        0        0     4988 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/decoder/run_decoder.py
+-rw-r--r--   0        0        0     2487 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/__init__.py
+-rw-r--r--   0        0        0      607 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/config/lsl.config
+-rw-r--r--   0        0        0     5069 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/config/settings.yaml
+-rw-r--r--   0        0        0     1297 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/config/settings_streamer.yaml
+-rw-r--r--   0        0        0     3887 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/encoder.py
+-rw-r--r--   0        0        0    27939 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/ephys_generator.py
+-rw-r--r--   0        0        0     9464 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/filters.py
+-rw-r--r--   0        0        0     2591 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/health_checker.py
+-rw-r--r--   0        0        0    11823 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/inputs.py
+-rw-r--r--   0        0        0     1792 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/models.py
+-rw-r--r--   0        0        0    14019 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/outputs.py
+-rw-r--r--   0        0        0     3129 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/runner.py
+-rw-r--r--   0        0        0     4198 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/samples.py
+-rw-r--r--   0        0        0       65 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/errors.py
+-rw-r--r--   0        0        0     4723 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/post_install_config.py
+-rw-r--r--   0        0        0     9843 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/run_encoder.py
+-rw-r--r--   0        0        0     9060 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/run_ephys_generator.py
+-rw-r--r--   0        0        0    11992 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/run_streamer.py
+-rw-r--r--   0        0        0     6979 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/settings.py
+-rw-r--r--   0        0        0     5574 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/streamers.py
+-rw-r--r--   0        0        0     2765 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/timing.py
+-rw-r--r--   0        0        0       56 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/util/__init__.py
+-rw-r--r--   0        0        0     3775 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/util/buffer.py
+-rw-r--r--   0        0        0      961 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/util/circular_dequeue.py
+-rw-r--r--   0        0        0     3046 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/util/runtime.py
+-rw-r--r--   0        0        0     1291 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/neural_data_simulator/util/settings_loader.py
+-rw-r--r--   0        0        0       48 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/plugins/__init__.py
+-rw-r--r--   0        0        0     1000 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/plugins/examples/gamepad_preprocessor.py
+-rw-r--r--   0        0        0     5294 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/plugins/examples/model.py
+-rw-r--r--   0        0        0      572 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/plugins/examples/postprocessor.py
+-rw-r--r--   0        0        0      498 2023-04-27 10:26:04.668079 neural_data_simulator-0.2.0/src/plugins/examples/preprocessor.py
+-rw-r--r--   0        0        0     4005 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/plugins/examples/tests/test_model.py
+-rw-r--r--   0        0        0      288 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/recorder/__init__.py
+-rw-r--r--   0        0        0     3201 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/recorder/run_recorder.py
+-rw-r--r--   0        0        0      251 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/__init__.py
+-rw-r--r--   0        0        0      872 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/__init__.py
+-rw-r--r--   0        0        0     2125 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/buttons.py
+-rw-r--r--   0        0        0     2734 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/input_events.py
+-rw-r--r--   0        0        0     1628 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/joystick.py
+-rw-r--r--   0        0        0     9783 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/metrics.py
+-rw-r--r--   0        0        0     4049 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/scalers.py
+-rw-r--r--   0        0        0     1583 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/screen_info.py
+-rw-r--r--   0        0        0     2778 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/sprites.py
+-rw-r--r--   0        0        0     6472 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_runner.py
+-rw-r--r--   0        0        0    11351 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_state.py
+-rw-r--r--   0        0        0    13007 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_window.py
+-rw-r--r--   0        0        0     1593 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/config/settings_center_out_reach.yaml
+-rw-r--r--   0        0        0    11674 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/run_center_out_reach.py
+-rw-r--r--   0        0        0      837 2023-04-27 10:26:04.672078 neural_data_simulator-0.2.0/src/tasks/run_closed_loop.py
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 neural_data_simulator-0.2.0/PKG-INFO
```

### Comparing `neural_data_simulator-0.1.2/LICENSE` & `neural_data_simulator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/README.md` & `neural_data_simulator-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/pyproject.toml` & `neural_data_simulator-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "neural-data-simulator"
-version = "0.1.2"
+version = "0.2.0"
 description = "Electrophysiology simulator data for developing Brain-Computer Interfaces"
 authors = ["AE Studio <bci@ae.studio>", "Chadwick Boulay <chadwick.boulay@gmail.com>"]
 maintainers = ["Chadwick Boulay <chadwick.boulay@gmail.com>", "AE Studio <bci@ae.studio>"]
 packages = [
-    {include = "nds", from = "src"},
+    {include = "neural_data_simulator", from = "src"},
     {include = "decoder", from = "src"},
     {include = "recorder", from = "src"},
     {include = "tasks", from = "src"},
     {include = "plugins", from = "src"},
 ]
 readme = "README.md"
 license = "Apache-2.0"
@@ -68,18 +68,18 @@
 types-requests = "^2.28.11.8"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-nds_post_install_config = "nds.scripts.post_install_config:run"
-encoder = "nds.scripts.run_encoder:run"
-streamer = "nds.scripts.run_streamer:run"
-ephys_generator = "nds.scripts.run_ephys_generator:run"
+nds_post_install_config = "neural_data_simulator.scripts.post_install_config:run"
+encoder = "neural_data_simulator.scripts.run_encoder:run"
+streamer = "neural_data_simulator.scripts.run_streamer:run"
+ephys_generator = "neural_data_simulator.scripts.run_ephys_generator:run"
 decoder = "decoder.run_decoder:run"
 recorder = "recorder.run_recorder:run"
 center_out_reach = "tasks.run_center_out_reach:run"
 run_closed_loop = "tasks.run_closed_loop:run"
 
 [tool.pytest.ini_options]
 # note: not overriding 'norecursedirs' here in order to keep the default value
@@ -96,15 +96,15 @@
 extend-exclude = """(
     docs
 )"""
 
 [tool.isort]
 profile = "google"
 src_paths = "."
-known_first_party = "nds"
+known_first_party = "neural_data_simulator"
 line_length = 88
 multi_line_output = 3
 include_trailing_comma = true
 
 [tool.pyright]
 include = ["src"]
```

### Comparing `neural_data_simulator-0.1.2/src/decoder/__init__.py` & `neural_data_simulator-0.2.0/src/decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/decoder/config/settings_decoder.yaml` & `neural_data_simulator-0.2.0/src/decoder/config/settings_decoder.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/decoder/decoders.py` & `neural_data_simulator-0.2.0/src/decoder/decoders.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 import time
 from typing import Protocol
 
 import joblib
 from numpy import ndarray
 import numpy as np
 
-from nds.filters import BandpassFilter
-from nds.filters import GaussianFilter
-from nds.filters import LowpassFilter
-from nds.samples import Samples
-from nds.util.buffer import RingBuffer
+from neural_data_simulator.filters import BandpassFilter
+from neural_data_simulator.filters import GaussianFilter
+from neural_data_simulator.filters import LowpassFilter
+from neural_data_simulator.samples import Samples
+from neural_data_simulator.util.buffer import RingBuffer
 
 logger = logging.getLogger(__name__)
 
 
 class DecoderModel(Protocol):
     """Protocol for a `Decoder` model.
 
     A `Decoder model` predicts behavior data from spike rate data.
 
-    The Decoder processes data in chunks represented as :class:`nds.samples.Samples`.
+    The Decoder processes data in chunks represented as
+    :class:`neural_data_simulator.samples.Samples`.
     One chunk may contain several spike rate data points (n_samples) across multiple
     units (n_units). The :meth:`predict` method is called for each chunk in order to
     transform the spike rate data into behavior data (n_samples) across multiple axes
     (n_axes).
 
     A python protocol (`PEP-544 <https://peps.python.org/pep-0544/>`_) works in
     a similar way to an abstract class.
@@ -34,19 +35,19 @@
     may be defined in a concrete implementation of this protocol if needed.
     """
 
     def predict(self, data: ndarray) -> ndarray:
         """Predict behavior from spike rate input.
 
         Args:
-            data: Spike rate data as :class:`nds.samples.Samples` with shape
-                (n_samples, n_units).
+            data: Spike rate data as :class:`neural_data_simulator.samples.Samples`
+                with shape (n_samples, n_units).
 
         Returns:
-            Behavior data as :class:`nds.samples.Samples` with shape
+            Behavior data as :class:`neural_data_simulator.samples.Samples` with shape
             (n_samples, n_axes). For example, in case of modeling velocities in a
             horizontal and vertical direction (2 axes), the returned data is a 2D
             array with shape (n_samples, 2).
         """
         ...
```

### Comparing `neural_data_simulator-0.1.2/src/decoder/run_decoder.py` & `neural_data_simulator-0.2.0/src/decoder/run_decoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from typing import cast
 
 from decoder.decoders import Decoder
 from decoder.decoders import PersistedFileDecoderModel
 from pydantic import BaseModel
 from pydantic_yaml import VersionedYamlModel
 
-from nds import inputs
-from nds import outputs
-from nds import timing
-from nds.outputs import StreamConfig
-from nds.settings import LogLevel
-from nds.settings import LSLInputModel
-from nds.settings import LSLOutputModel
-from nds.settings import TimerModel
-from nds.util.runtime import configure_logger
-from nds.util.runtime import get_abs_path
-from nds.util.runtime import open_connection
-from nds.util.settings_loader import get_script_settings
+from neural_data_simulator import inputs
+from neural_data_simulator import outputs
+from neural_data_simulator import timing
+from neural_data_simulator.outputs import StreamConfig
+from neural_data_simulator.settings import LogLevel
+from neural_data_simulator.settings import LSLInputModel
+from neural_data_simulator.settings import LSLOutputModel
+from neural_data_simulator.settings import TimerModel
+from neural_data_simulator.util.runtime import configure_logger
+from neural_data_simulator.util.runtime import get_abs_path
+from neural_data_simulator.util.runtime import open_connection
+from neural_data_simulator.util.settings_loader import get_script_settings
 
 logger = logging.getLogger(__name__)
 
 
 class _Settings(VersionedYamlModel):
     """Decoder settings."""
```

### Comparing `neural_data_simulator-0.1.2/src/nds/config/lsl.config` & `neural_data_simulator-0.2.0/src/neural_data_simulator/config/lsl.config`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/nds/config/settings.yaml` & `neural_data_simulator-0.2.0/src/neural_data_simulator/config/settings.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/nds/config/settings_streamer.yaml` & `neural_data_simulator-0.2.0/src/neural_data_simulator/config/settings_streamer.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/nds/encoder.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """This module contains the `Encoder` implementation."""
 import contextlib
 import logging
 from typing import Iterator, Optional, Protocol, runtime_checkable
 
-from nds.inputs import Input
-from nds.models import EncoderModel
-from nds.outputs import Output
-from nds.samples import Samples
-from nds.util.runtime import open_connection
+from neural_data_simulator.inputs import Input
+from neural_data_simulator.models import EncoderModel
+from neural_data_simulator.outputs import Output
+from neural_data_simulator.samples import Samples
+from neural_data_simulator.util.runtime import open_connection
 
 
 @runtime_checkable
 class Processor(Protocol):
     """Protocol for an encoder Processor class.
 
     A processor can be used to transform data, usually for the purpose of
```

### Comparing `neural_data_simulator-0.1.2/src/nds/ephys_generator.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/ephys_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from typing import Dict, List, NamedTuple, Optional, Protocol, Tuple
 
 import colorednoise
 from numpy import ndarray
 import numpy as np
 import pylsl
 
-from nds.filters import LowpassFilter
-from nds.health_checker import HealthChecker
-from nds.inputs import LSLInput
-from nds.outputs import LSLOutputDevice
-from nds.timing import Timer
-from nds.util.buffer import RingBuffer
+from neural_data_simulator.filters import LowpassFilter
+from neural_data_simulator.health_checker import HealthChecker
+from neural_data_simulator.inputs import LSLInput
+from neural_data_simulator.outputs import LSLOutputDevice
+from neural_data_simulator.timing import Timer
+from neural_data_simulator.util.buffer import RingBuffer
 
 
 class SpikeRateInput(Protocol):
     """An abstract input that can be used to read spike rates.
 
     A python protocol (`PEP-544 <https://peps.python.org/pep-0544/>`_) works in
     a similar way to an abstract class.
```

### Comparing `neural_data_simulator-0.1.2/src/nds/filters.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/filters.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/nds/health_checker.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/health_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Health checker for NDS components."""
 import logging
 import time
 
 import numpy as np
 
-from nds.util.circular_dequeue import CircularDeque
+from neural_data_simulator.util.circular_dequeue import CircularDeque
 
 logger = logging.getLogger(__name__)
 
 
 class HealthChecker:
     """Class to monitor the processing time consistency.
```

### Comparing `neural_data_simulator-0.1.2/src/nds/inputs.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import math
 import time
 from typing import List, Optional, Union
 
 import numpy as np
 import pylsl
 
-from nds.samples import Samples
+from neural_data_simulator.samples import Samples
 
 
 class Input(abc.ABC):
     """Represents an input that can be used to consume data from.
 
     This can be an interface for a joystick, a behavior data generator, a data
     streamer that loads data from disk, etc.
@@ -34,15 +34,15 @@
 
     def disconnect(self) -> None:
         """Disconnect from input. The default implementation does nothing."""
         pass
 
 
 class SamplesInput(Input):
-    """An input object based on a :class:`nds.samples.Samples` dataclass.
+    """An input object based on a :class:`neural_data_simulator.samples.Samples` dataclass.
 
     The underlying samples dataclass will have its timestamps modified to be
     in reference to when the first read was made from this class, simulating the
     appearance of data being collected in real-time. Alternatively, the function
     `set_reference_time_to_now` can be called prior to the first `read` of the data to
     use that as a reference time.
 
@@ -75,16 +75,16 @@
         """Get new samples from the time of last read.
 
         If first call to `read` samples will be read since the call to
         `set_reference_time_to_now`.
         If `set_reference_time_to_now` was not previously called, it will be called.
 
         Returns:
-            :class:`nds.samples.Samples` dataclass with timestamps and data available
-            since last `read` call.
+            :class:`neural_data_simulator.samples.Samples` dataclass with timestamps and
+            data available since last `read` call.
         """
         if not self._has_reference_time:
             self._logger.warning(
                 "Reference time not calculated before first read call."
                 " Calculating now."
             )
             self.set_reference_time_to_now()
@@ -230,17 +230,17 @@
                 "LSL StreamInlet is not connected, ensure you run connect before read."
             )
 
     def read(self) -> Samples:
         """Read available data from the inlet as a samples.
 
         Returns:
-            :class:`nds.samples.Samples` dataclass with timestamps and data read from
-            the LSL StreamInlet. If no data is available, an empty Samples is
-            returned.
+            :class:`neural_data_simulator.samples.Samples` dataclass with timestamps and
+            data read from the LSL StreamInlet. If no data is available, an empty
+            Samples is returned.
 
         Raises:
             ValueError: LSL StreamInlet is not connected. `connect` should be called
               before `read`.
         """
         self._check_connection()
         assert self._inlet is not None
```

### Comparing `neural_data_simulator-0.1.2/src/nds/models.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Classes that implement a model for encoding neural data from behavior data."""
 from typing import Protocol, runtime_checkable
 
-from nds.samples import Samples
+from neural_data_simulator.samples import Samples
 
 
 @runtime_checkable
 class EncoderModel(Protocol):
     """Protocol for an `Encoder` model.
 
     Classes that conform to this protocol can be used by the
-    :class:`nds.encoder.Encoder` to convert behavioral input data into
+    :class:`neural_data_simulator.encoder.Encoder` to convert behavioral input data into
     spiking rate data.
 
-    The Encoder processes data in chunks represented as :class:`nds.samples.Samples`.
+    The Encoder processes data in chunks represented as
+    :class:`neural_data_simulator.samples.Samples`.
     One chunk may contain several behavioral data points (n_samples) across
     multiple axes (n_axes). The Encoder calls the EncoderModel's :meth:`encode` method
     for each chunk in order to transform the behavioral data into spiking rates
     (n_samples) across multiple units (n_units).
 
     A python protocol (`PEP-544 <https://peps.python.org/pep-0544/>`_) works in
     a similar way to an abstract class.
@@ -25,16 +26,17 @@
     may be defined in a concrete implementation of this protocol if needed.
     """
 
     def encode(self, data: Samples) -> Samples:
         """Encode behavior into spiking rates.
 
         Args:
-            data: Behavioral data as :class:`nds.samples.Samples`.
+            data: Behavioral data as :class:`neural_data_simulator.samples.Samples`.
               For example, in case of modeling velocities in a horizontal and vertical
               direction (2 axes), the data is a 2D array with shape (n_samples, 2).
 
         Returns:
-            Spiking rates as :class:`nds.samples.Samples`. The spiking rates are
-            represented as a 2D array with shape (n_samples, n_units).
+            Spiking rates as :class:`neural_data_simulator.samples.Samples`.
+            The spiking rates are represented as a 2D array with shape
+            (n_samples, n_units).
         """
         ...
```

### Comparing `neural_data_simulator-0.1.2/src/nds/outputs.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/outputs.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import logging
 from typing import Any, Callable, IO, List, Optional, Union
 
 from numpy import ndarray
 import numpy as np
 import pylsl
 
-from nds.samples import Samples
-from nds.settings import LSLOutputModel
+from neural_data_simulator.samples import Samples
+from neural_data_simulator.settings import LSLOutputModel
 
 
 class Output(abc.ABC):
     """Represents an abstract output that can be used to send samples."""
 
     @property
     @abc.abstractmethod
@@ -98,15 +98,16 @@
         """
         return self._channel_count
 
     def _send(self, samples: Samples) -> None:
         """Send data to a file without index or header.
 
         Args:
-            samples: :class:`nds.samples.Samples` dataclass with timestamps and data.
+            samples: :class:`neural_data_simulator.samples.Samples` dataclass with
+              timestamps and data.
         """
         timestamps_and_data = np.column_stack((samples.timestamps, samples.data))
         print(np.array2string(timestamps_and_data))
 
     def connect(self) -> None:
         """Connect to the device within a context.
 
@@ -140,15 +141,15 @@
         """
         return self._channel_count
 
     def _send(self, samples: Samples) -> None:
         """Write the samples into the file.
 
         Args:
-            samples: :class:`nds.samples.Samples` dataclass.
+            samples: :class:`neural_data_simulator.samples.Samples` dataclass.
         """
         if self.file is not None:
             timestamps_and_data = np.column_stack((samples.timestamps, samples.data))
             np.savetxt(self.file, timestamps_and_data, delimiter=",", fmt="%f")
 
     def connect(self) -> None:
         """Open the output file."""
@@ -190,18 +191,19 @@
     @classmethod
     def from_lsl_settings(
         cls,
         lsl_settings: LSLOutputModel,
         sampling_rate: Union[float, Callable],
         n_channels: int,
     ):
-        """Create a StreamConfig from an :class:`nds.settings.LSLOutputModel`.
+        """Create a StreamConfig from an :class:`neural_data_simulator.settings.LSLOutputModel`.
 
         Args:
-            lsl_settings: :class:`nds.settings.LSLOutputModel` instance.
+            lsl_settings: :class:`neural_data_simulator.settings.LSLOutputModel`
+              instance.
             sampling_rate: Sampling rate in Hz.
             n_channels: Number of channels.
         """
         acquisition = {
             "manufacturer": lsl_settings.instrument.manufacturer,
             "model": lsl_settings.instrument.model,
             "instrument_id": lsl_settings.instrument.id,
@@ -218,18 +220,18 @@
         )
 
 
 class LSLOutputDevice(Output):
     """An output device that can be used to stream data via LSL."""
 
     def __init__(self, stream_config: StreamConfig):
-        """Initialize the LSL Output Device from a :class:`nds.outputs.StreamConfig`.
+        """Initialize the LSL Output Device from a StreamConfig.
 
         Args:
-            stream_config: :class:`nds.outputs.StreamConfig` instance.
+            stream_config: :class:`neural_data_simulator.outputs.StreamConfig` instance.
         """
         self.logger = logging.getLogger(__name__)
         self._stream_config = stream_config
         self._outlet: Optional[pylsl.StreamOutlet] = None
         self._stream_info: Optional[pylsl.StreamInfo] = None
         self._stream_configured = False
 
@@ -285,15 +287,16 @@
                 "LSL StreamOutlet is not connected, ensure you run connect before send."
             )
 
     def _send(self, samples: Samples):
         """Push the data to the LSL outlet.
 
         Args:
-            samples: :class:`nds.samples.Samples` dataclass with timestamps and data.
+            samples: :class:`neural_data_simulator.samples.Samples` dataclass with
+              timestamps and data.
 
         Raises:
             ValueError: LSL StreamOutlet is not connected. `connect` should be called
               before `send`.
         """
         for timestamp, data_point in zip(samples.timestamps, samples.data):
             self.send_as_sample(data_point, timestamp)
```

### Comparing `neural_data_simulator-0.1.2/src/nds/runner.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/runner.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/nds/samples.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/samples.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/nds/scripts/post_install_config.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/post_install_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,36 +14,36 @@
 from urllib.parse import urljoin
 
 import decoder
 import plugins
 import pooch
 import tasks
 
-import nds
-from nds.util.runtime import get_abs_path
-from nds.util.runtime import get_configs_dir
-from nds.util.runtime import get_plugins_dir
-from nds.util.runtime import get_sample_data_dir
+import neural_data_simulator
+from neural_data_simulator.util.runtime import get_abs_path
+from neural_data_simulator.util.runtime import get_configs_dir
+from neural_data_simulator.util.runtime import get_plugins_dir
+from neural_data_simulator.util.runtime import get_sample_data_dir
 
 plugin_files = [
     ("model.py", plugins.__file__),
     ("preprocessor.py", plugins.__file__),
     ("postprocessor.py", plugins.__file__),
     ("gamepad_preprocessor.py", plugins.__file__),
 ]
 
 plugin_test_files = [
     ("test_model.py", os.path.join(os.path.dirname(plugins.__file__), "examples"))
 ]
 
 
 core_configs = [
-    ("settings.yaml", nds.__file__),
-    ("settings_streamer.yaml", nds.__file__),
-    ("lsl.config", nds.__file__),
+    ("settings.yaml", neural_data_simulator.__file__),
+    ("settings_streamer.yaml", neural_data_simulator.__file__),
+    ("lsl.config", neural_data_simulator.__file__),
 ]
 
 extras_configs = [
     ("settings_decoder.yaml", decoder.__file__),
     ("settings_center_out_reach.yaml", tasks.__file__),
 ]
```

### Comparing `neural_data_simulator-0.1.2/src/nds/scripts/run_encoder.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/run_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 r"""Script that starts the encoder.
 
 The encoder default configuration is located in `NDS_HOME/settings.yaml`
-(see :mod:`nds.scripts.post_install_config`). The script can use different
-config file specified via the `\--settings-path` argument.
+(see :mod:`neural_data_simulator.scripts.post_install_config`). The script can use
+different config file specified via the `\--settings-path` argument.
 
 The config file has an `encoder` section where the settings for the model,
 input and output can be adjusted. By default, the encoder expects to read
 data from an LSL stream and output to an LSL outlet. In absence of the
 input stream, the encoder will not be able to start.
 """
 import argparse
@@ -16,32 +16,32 @@
 from pathlib import Path
 import sys
 from types import ModuleType
 from typing import Callable, cast, Optional, Union
 
 import numpy as np
 
-from nds import encoder
-from nds import inputs
-from nds import models
-from nds import outputs
-from nds import runner
-from nds import timing
-from nds.outputs import LSLOutputDevice
-from nds.outputs import StreamConfig
-from nds.samples import Samples
-from nds.scripts.errors import InvalidPluginError
-from nds.settings import EncoderEndpointType
-from nds.settings import EncoderSettings
-from nds.settings import LSLOutputModel
-from nds.settings import Settings
-from nds.util.runtime import configure_logger
-from nds.util.runtime import get_abs_path
-from nds.util.runtime import unwrap
-from nds.util.settings_loader import get_script_settings
+from neural_data_simulator import encoder
+from neural_data_simulator import inputs
+from neural_data_simulator import models
+from neural_data_simulator import outputs
+from neural_data_simulator import runner
+from neural_data_simulator import timing
+from neural_data_simulator.outputs import LSLOutputDevice
+from neural_data_simulator.outputs import StreamConfig
+from neural_data_simulator.samples import Samples
+from neural_data_simulator.scripts.errors import InvalidPluginError
+from neural_data_simulator.settings import EncoderEndpointType
+from neural_data_simulator.settings import EncoderSettings
+from neural_data_simulator.settings import LSLOutputModel
+from neural_data_simulator.settings import Settings
+from neural_data_simulator.util.runtime import configure_logger
+from neural_data_simulator.util.runtime import get_abs_path
+from neural_data_simulator.util.runtime import unwrap
+from neural_data_simulator.util.settings_loader import get_script_settings
 
 logger = logging.getLogger(__name__)
 
 
 def _setup_npz_input(
     behavior_file: str, timestamps_array_name: str, data_array_name: str
 ) -> inputs.SamplesInput:
@@ -163,15 +163,15 @@
 def _setup_model(encoder_settings: EncoderSettings) -> models.EncoderModel:
     """Instantiate the model to be used in the encoder.
 
     Args:
         encoder_settings: The encoder settings with the model path.
 
     Returns:
-        An instance of an :class:`nds.models.EncoderModel`.
+        An instance of an :class:`neural_data_simulator.models.EncoderModel`.
     """
     return _load_plugin_model(encoder_settings.model)
 
 
 def _setup_file_output(output_file: str, channel_count: int) -> outputs.FileOutput:
     """Set up the file output.
```

### Comparing `neural_data_simulator-0.1.2/src/nds/scripts/run_streamer.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/scripts/run_streamer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 r"""Script that starts the streamer.
 
 The streamer default configuration is located in `NDS_HOME/settings_streamer.yaml`
-(see :mod:`nds.scripts.post_install_config`). The script can use different
-config file specified via the `\--settings-path` argument.
+(see :mod:`neural_data_simulator.scripts.post_install_config`). The script can use
+different config file specified via the `\--settings-path` argument.
 
 Upon start, the streamer expects to read data from a file and output to an LSL
 outlet. By default, a sample behavior data file will be downloaded by the
-:mod:`nds.scripts.post_install_config` script, so the streamer should be able
-to run without any additional configuration. If the input file cannot be found,
+:mod:`neural_data_simulator.scripts.post_install_config` script, so the streamer should
+be able to run without any additional configuration. If the input file cannot be found,
 the streamer will not be able to start.
 """
 import argparse
 import contextlib
 import logging
 from pathlib import Path
 from typing import cast, Dict, Iterator, List, Optional, Tuple
@@ -19,25 +19,25 @@
 from neo.rawio.blackrockrawio import BlackrockRawIO
 import numpy as np
 from pydantic import BaseModel
 from pydantic import validator
 from pydantic_yaml import VersionedYamlModel
 from pydantic_yaml import YamlStrEnum
 
-from nds import outputs
-from nds import streamers
-from nds.outputs import StreamConfig
-from nds.samples import Samples
-from nds.settings import LogLevel
-from nds.settings import LSLChannelFormatType
-from nds.settings import LSLOutputModel
-from nds.util.runtime import configure_logger
-from nds.util.runtime import get_abs_path
-from nds.util.runtime import unwrap
-from nds.util.settings_loader import get_script_settings
+from neural_data_simulator import outputs
+from neural_data_simulator import streamers
+from neural_data_simulator.outputs import StreamConfig
+from neural_data_simulator.samples import Samples
+from neural_data_simulator.settings import LogLevel
+from neural_data_simulator.settings import LSLChannelFormatType
+from neural_data_simulator.settings import LSLOutputModel
+from neural_data_simulator.util.runtime import configure_logger
+from neural_data_simulator.util.runtime import get_abs_path
+from neural_data_simulator.util.runtime import unwrap
+from neural_data_simulator.util.settings_loader import get_script_settings
 
 logger = logging.getLogger(__name__)
 
 
 class StreamerInputType(YamlStrEnum):
     """Possible types for the streamer input."""
```

### Comparing `neural_data_simulator-0.1.2/src/nds/settings.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/settings.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/nds/streamers.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/streamers.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from dataclasses import dataclass
 import logging
 from typing import List
 
 import numpy as np
 import pylsl
 
-from nds.outputs import LSLOutputDevice
-from nds.samples import Samples
-from nds.timing import Timer
+from neural_data_simulator.outputs import LSLOutputDevice
+from neural_data_simulator.samples import Samples
+from neural_data_simulator.timing import Timer
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Stream:
     """Stream information."""
@@ -38,17 +38,18 @@
         """
         return len(self.samples)
 
 
 class LSLStreamer:
     """Streamer class that can be used to send samples through an LSL stream.
 
-    A streamer class that takes a :class:`nds.samples.Samples` dataclass with timestamps
-    and behavior data and stream it through LSL. Following the timestamps provided, the
-    data is streamed to simulate a real-time data acquisition.
+    A streamer class that takes a :class:`neural_data_simulator.samples.Samples`
+    dataclass with timestamps and behavior data and stream it through LSL.
+    Following the timestamps provided, the data is streamed to simulate a
+    real-time data acquisition.
     """
 
     def __init__(
         self,
         outputs: List[LSLOutputDevice],
         samples: List[Samples],
         lsl_chunk_frequency: float,
```

### Comparing `neural_data_simulator-0.1.2/src/nds/timing.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/timing.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,10 +69,11 @@
     Args:
         loop_time: expected time between returns from the wait function (in seconds).
         max_cpu_buffer: Maximum time to stay in cpu bound loop (i.e. a while loop
           that does nothing) waiting for correct time to return from a `wait`
           call (in seconds). Defaults to 0.005.
 
     Returns:
-        An instance of the :class:`nds.timing.Timer` class based on input parameters.
+        An instance of the :class:`neural_data_simulator.timing.Timer` class based on
+        input parameters.
     """
     return Timer(loop_time, max_cpu_buffer)
```

### Comparing `neural_data_simulator-0.1.2/src/nds/util/buffer.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/util/buffer.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/nds/util/circular_dequeue.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/util/circular_dequeue.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/nds/util/runtime.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/util/runtime.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Functions commonly used by scripts."""
 import contextlib
 import logging
 import os
 from pathlib import Path
 from typing import Any, Optional, Union
 
-from nds.inputs import Input
-from nds.outputs import Output
-from nds.settings import LogLevel
+from neural_data_simulator.inputs import Input
+from neural_data_simulator.outputs import Output
+from neural_data_simulator.settings import LogLevel
 
 logger = logging.getLogger(__name__)
 
 NDS_HOME = os.path.join(os.path.expanduser("~"), ".nds")
 
 
 def configure_logger(script_name: str, log_level: LogLevel):
```

### Comparing `neural_data_simulator-0.1.2/src/nds/util/settings_loader.py` & `neural_data_simulator-0.2.0/src/neural_data_simulator/util/settings_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import errno
 import logging
 from pathlib import Path
 from typing import Optional, Type
 
 from pydantic_yaml import VersionedYamlModel
 
-from nds.util.runtime import get_abs_path
-from nds.util.runtime import NDS_HOME
+from neural_data_simulator.util.runtime import get_abs_path
+from neural_data_simulator.util.runtime import NDS_HOME
 
 logger = logging.getLogger(__name__)
 
 
 def get_script_settings(
     settings_file: Optional[Path],
     filename: str,
```

### Comparing `neural_data_simulator-0.1.2/src/plugins/examples/gamepad_preprocessor.py` & `neural_data_simulator-0.2.0/src/plugins/examples/gamepad_preprocessor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Preprocessor for LSL Gamepad app for velocity tuning model."""
-from nds.encoder import Processor
-from nds.samples import Samples
+from neural_data_simulator.encoder import Processor
+from neural_data_simulator.samples import Samples
 
 
 class GamepadPreprocessor(Processor):
     """Custom Preprocessor implementation."""
 
     def execute(self, data: Samples) -> Samples:
         """Process the data and return the transformation."""
```

### Comparing `neural_data_simulator-0.1.2/src/plugins/examples/model.py` & `neural_data_simulator-0.2.0/src/plugins/examples/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Example of a custom EncoderModel."""
 import logging
 from typing import Union
 
 from numpy import ndarray
 import numpy as np
 
-from nds.models import EncoderModel
-from nds.samples import Samples
-from nds.util.runtime import get_abs_path
+from neural_data_simulator.models import EncoderModel
+from neural_data_simulator.samples import Samples
+from neural_data_simulator.util.runtime import get_abs_path
 
 
 class VelocityTuningCurvesModel(EncoderModel):
     r"""Two-dimensional tuning curve model.
 
     A two-dimensional tuning curve model that takes into account both preferred
     direction and magnitude of the velocity, following the equation from `decoding arm
@@ -50,25 +50,26 @@
         r"""Encode 2D behavior data into spiking data.
 
         Calculate spiking rates from the equation:
         :math:`spike rate = b_0 + m * |v| * cos(\theta - \theta_{pd}) + b_s*|v|`
         with v = velocity, theta = velocity direction.
 
         Args:
-            X: :class:`nds.samples.Samples` dataclass with timestamps and data points
-              for velocity data (x and y direction, respectively) in the same unit as
-              parameters were fit for. Each element of samples timestamps has 1 column
-              where the acquisition time of the data point is stored. Each element of
-              samples data has 2 columns, one for each velocity direction. Each row of
-              samples corresponds to a data point acquisition.
+            X: :class:`neural_data_simulator.samples.Samples` dataclass with timestamps
+              and data points for velocity data (x and y direction, respectively) in
+              the same unit as parameters were fit for. Each element of samples
+              timestamps has 1 column where the acquisition time of the data point
+              is stored. Each element of samples data has 2 columns, one for each
+              velocity direction. Each row of samples corresponds to a data point
+              acquisition.
 
         Returns:
-            :class:`nds.samples.Samples` with the same timestamps as input, but data
-            matching the size of the model parameters (which represent the units
-            spikes are generated for).
+            :class:`neural_data_simulator.samples.Samples` with the same timestamps as
+            input, but data matching the size of the model parameters (which represent
+            the units spikes are generated for).
         """
         velocities = X.data
         magnitudes = VelocityTuningCurvesModel._get_magnitude(velocities)
         angles = VelocityTuningCurvesModel._get_angle(velocities)
 
         spike_rates = self._encode(magnitudes, angles)
         return Samples(timestamps=X.timestamps, data=spike_rates)
```

### Comparing `neural_data_simulator-0.1.2/src/plugins/examples/postprocessor.py` & `neural_data_simulator-0.2.0/src/plugins/examples/postprocessor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Example of a custom Postprocessor implementation."""
 import numpy as np
 
-from nds.encoder import Processor
-from nds.samples import Samples
+from neural_data_simulator.encoder import Processor
+from neural_data_simulator.samples import Samples
 
 
 class PassThroughPostprocessor(Processor):
     """Custom Postprocessor implementation."""
 
     def execute(self, data: Samples) -> Samples:
         """Process the data and return the transformation."""
```

### Comparing `neural_data_simulator-0.1.2/src/plugins/examples/tests/test_model.py` & `neural_data_simulator-0.2.0/src/plugins/examples/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests for models.py module."""
 
 import numpy as np
 from plugins.examples.model import VelocityTuningCurvesModel
 import pytest
 
-from nds.samples import Samples
+from neural_data_simulator.samples import Samples
 
 
 def _create_model_weights_file(tmp_path, b0, m, pd, bs):
     filepath = tmp_path / "weights"
     np.savez(str(filepath), b0=b0, m=m, pd=pd, bs=bs)
     return str(filepath) + ".npz"
```

### Comparing `neural_data_simulator-0.1.2/src/recorder/run_recorder.py` & `neural_data_simulator-0.2.0/src/recorder/run_recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import argparse
 import signal
 import sys
 import time
 
 import numpy as np
 
-from nds import inputs
+from neural_data_simulator import inputs
 
 
 class LSLStreamRecorder:
     """Helper class for collecting data from an LSL stream."""
 
     def __init__(self, stream_name):
         """Initialize the LSLStreamRecorder class.
```

### Comparing `neural_data_simulator-0.1.2/src/tasks/center_out_reach/__init__.py` & `neural_data_simulator-0.2.0/src/tasks/center_out_reach/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/tasks/center_out_reach/buttons.py` & `neural_data_simulator-0.2.0/src/tasks/center_out_reach/buttons.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/tasks/center_out_reach/input_events.py` & `neural_data_simulator-0.2.0/src/tasks/center_out_reach/input_events.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/tasks/center_out_reach/joystick.py` & `neural_data_simulator-0.2.0/src/tasks/center_out_reach/joystick.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/tasks/center_out_reach/metrics.py` & `neural_data_simulator-0.2.0/src/tasks/center_out_reach/metrics.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/tasks/center_out_reach/scalers.py` & `neural_data_simulator-0.2.0/src/tasks/center_out_reach/scalers.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/tasks/center_out_reach/screen_info.py` & `neural_data_simulator-0.2.0/src/tasks/center_out_reach/screen_info.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/tasks/center_out_reach/sprites.py` & `neural_data_simulator-0.2.0/src/tasks/center_out_reach/sprites.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/tasks/center_out_reach/task_runner.py` & `neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 import numpy as np
 import pylsl
 from tasks.center_out_reach.input_events import InputEvent
 from tasks.center_out_reach.input_events import InputHandler
 from tasks.center_out_reach.metrics import MetricsCollector
 from tasks.center_out_reach.task_state import TaskState
 
-from nds import inputs
-from nds import outputs
-from nds.filters import LowpassFilter
-from nds.samples import Samples
-from nds.timing import Timer
+from neural_data_simulator import inputs
+from neural_data_simulator import outputs
+from neural_data_simulator.filters import LowpassFilter
+from neural_data_simulator.samples import Samples
+from neural_data_simulator.timing import Timer
 
 
 class VelocityScaler(Protocol):
     """Scales the cursor velocity.
 
     A python protocol (`PEP-544 <https://peps.python.org/pep-0544/>`_) works in
     a similar way to an abstract class.
```

### Comparing `neural_data_simulator-0.1.2/src/tasks/center_out_reach/task_state.py` & `neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_state.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/tasks/center_out_reach/task_window.py` & `neural_data_simulator-0.2.0/src/tasks/center_out_reach/task_window.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/tasks/config/settings_center_out_reach.yaml` & `neural_data_simulator-0.2.0/src/tasks/config/settings_center_out_reach.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/src/tasks/run_center_out_reach.py` & `neural_data_simulator-0.2.0/src/tasks/run_center_out_reach.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 from tasks.center_out_reach.scalers import PixelsToMetersConverter
 from tasks.center_out_reach.scalers import StandardVelocityScaler
 from tasks.center_out_reach.task_runner import TaskRunner
 from tasks.center_out_reach.task_state import StateParams
 from tasks.center_out_reach.task_state import TaskState
 from tasks.center_out_reach.task_window import TaskWindow
 
-from nds import inputs
-from nds import outputs
-from nds.outputs import StreamConfig
-from nds.settings import LogLevel
-from nds.settings import LSLInputModel
-from nds.settings import LSLOutputModel
-from nds.util.runtime import configure_logger
-from nds.util.runtime import open_connection
-from nds.util.runtime import unwrap
-from nds.util.settings_loader import get_script_settings
+from neural_data_simulator import inputs
+from neural_data_simulator import outputs
+from neural_data_simulator.outputs import StreamConfig
+from neural_data_simulator.settings import LogLevel
+from neural_data_simulator.settings import LSLInputModel
+from neural_data_simulator.settings import LSLOutputModel
+from neural_data_simulator.util.runtime import configure_logger
+from neural_data_simulator.util.runtime import open_connection
+from neural_data_simulator.util.runtime import unwrap
+from neural_data_simulator.util.settings_loader import get_script_settings
 
 logger = logging.getLogger(__name__)
 
 
 class _Settings(VersionedYamlModel):
     """Center-out reach settings."""
```

### Comparing `neural_data_simulator-0.1.2/src/tasks/run_closed_loop.py` & `neural_data_simulator-0.2.0/src/tasks/run_closed_loop.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.1.2/PKG-INFO` & `neural_data_simulator-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-data-simulator
-Version: 0.1.2
+Version: 0.2.0
 Summary: Electrophysiology simulator data for developing Brain-Computer Interfaces
 License: Apache-2.0
 Author: AE Studio
 Author-email: bci@ae.studio
 Maintainer: Chadwick Boulay
 Maintainer-email: chadwick.boulay@gmail.com
 Requires-Python: >=3.9,<3.12
```


# Comparing `tmp/lightning-graphcore-0.1.0.dev0.tar.gz` & `tmp/lightning-graphcore-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-graphcore-0.1.0.dev0.tar", last modified: Fri Apr 21 22:21:15 2023, max compression
+gzip compressed data, was "lightning-graphcore-0.1.0rc0.tar", last modified: Thu Apr 27 14:17:44 2023, max compression
```

## Comparing `lightning-graphcore-0.1.0.dev0.tar` & `lightning-graphcore-0.1.0rc0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:21:15.832266 lightning-graphcore-0.1.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-21 22:21:15.832266 lightning-graphcore-0.1.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 22:21:15.832266 lightning-graphcore-0.1.0.dev0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:21:15.828266 lightning-graphcore-0.1.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:21:15.832266 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:21:15.832266 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/top_level.txt
```

### Comparing `lightning-graphcore-0.1.0.dev0/LICENSE` & `lightning-graphcore-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0.dev0/MANIFEST.in` & `lightning-graphcore-0.1.0rc0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0.dev0/PKG-INFO` & `lightning-graphcore-0.1.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-graphcore
-Version: 0.1.0.dev0
+Version: 0.1.0rc0
 Summary: Lightning support for GraphCore accelerators
 Home-page: https://github.com/Lightning-AI/lightning-graphcore
 Download-URL: https://github.com/Lightning-AI/lightning-graphcore
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-graphcore/issues
```

### Comparing `lightning-graphcore-0.1.0.dev0/README.md` & `lightning-graphcore-0.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0.dev0/setup.py` & `lightning-graphcore-0.1.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/accelerator.py` & `lightning-graphcore-0.1.0rc0/src/lightning_graphcore/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/precision.py` & `lightning-graphcore-0.1.0rc0/src/lightning_graphcore/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/strategy.py` & `lightning-graphcore-0.1.0rc0/src/lightning_graphcore/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import json
 import os
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
-import pytorch_lightning as pl
 import torch
 from lightning_utilities.core.apply_func import apply_to_collection
 from lightning_utilities.core.imports import package_available
 from torch import Tensor
 from torch.utils.data import DataLoader, Sampler
 
 if package_available("lightning"):
+    import lightning.pytorch as pl
     from lightning.fabric.plugins import CheckpointIO, ClusterEnvironment
     from lightning.fabric.utilities.cloud_io import get_filesystem
     from lightning.pytorch import Trainer
     from lightning.pytorch.accelerators import Accelerator
     from lightning.pytorch.overrides.base import _LightningModuleWrapperBase
     from lightning.pytorch.plugins.precision import PrecisionPlugin
     from lightning.pytorch.strategies.parallel import ParallelStrategy
@@ -35,14 +35,15 @@
     from lightning.pytorch.trainer.states import RunningStage, TrainerFn
     from lightning.pytorch.utilities import rank_zero_warn
     from lightning.pytorch.utilities.data import _get_dataloader_init_args_and_kwargs, _reinstantiate_wrapped_cls
     from lightning.pytorch.utilities.exceptions import MisconfigurationException
     from lightning.pytorch.utilities.model_helpers import is_overridden
     from lightning.pytorch.utilities.types import STEP_OUTPUT
 elif package_available("pytorch_lightning"):
+    import pytorch_lightning as pl
     from lightning_fabric.plugins import CheckpointIO, ClusterEnvironment
     from lightning_fabric.utilities.cloud_io import get_filesystem
     from pytorch_lightning import Trainer
     from pytorch_lightning.accelerators import Accelerator
     from pytorch_lightning.overrides.base import _LightningModuleWrapperBase
     from pytorch_lightning.plugins.precision import PrecisionPlugin
     from pytorch_lightning.strategies.parallel import ParallelStrategy
```

### Comparing `lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/PKG-INFO` & `lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-graphcore
-Version: 0.1.0.dev0
+Version: 0.1.0rc0
 Summary: Lightning support for GraphCore accelerators
 Home-page: https://github.com/Lightning-AI/lightning-graphcore
 Download-URL: https://github.com/Lightning-AI/lightning-graphcore
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-graphcore/issues
```

### Comparing `lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/SOURCES.txt` & `lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*


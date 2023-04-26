# Comparing `tmp/torchchronos-0.0.2.tar.gz` & `tmp/torchchronos-0.0.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchchronos-0.0.2.tar", max compression
+gzip compressed data, was "torchchronos-0.0.3.post1.tar", max compression
```

## Comparing `torchchronos-0.0.2.tar` & `torchchronos-0.0.3.post1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1088 2023-04-20 08:07:10.115949 torchchronos-0.0.2/LICENSE
--rw-r--r--   0        0        0     3767 2023-04-20 08:07:10.115949 torchchronos-0.0.2/README.md
--rw-r--r--   0        0        0      605 2023-04-20 08:07:10.115949 torchchronos-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       19 2023-04-20 08:07:09.667947 torchchronos-0.0.2/torchchronos/__init__.py
--rw-r--r--   0        0        0      131 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/datasets/__init__.py
--rw-r--r--   0        0        0     3557 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/datasets/tfc_pretrain.py
--rw-r--r--   0        0        0     1841 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/datasets/ucr_uea.py
--rw-r--r--   0        0        0     1860 2023-04-20 08:07:09.667947 torchchronos-0.0.2/torchchronos/datasets/ucr_uea_dataset.py
--rw-r--r--   0        0        0     1765 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/download.py
--rw-r--r--   0        0        0      143 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/lightning/__init__.py
--rw-r--r--   0        0        0     2320 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/lightning/tfc_pretrain.py
--rw-r--r--   0        0        0     3348 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/lightning/ucr_uea.py
--rw-r--r--   0        0        0     3397 2023-04-20 08:07:09.667947 torchchronos-0.0.2/torchchronos/lightning/ucr_uea_module.py
--rw-r--r--   0        0        0      135 2023-04-20 08:06:54.531840 torchchronos-0.0.2/torchchronos/transforms/__init__.py
--rw-r--r--   0        0        0      868 2023-04-20 08:06:54.531840 torchchronos-0.0.2/torchchronos/transforms/base.py
--rw-r--r--   0        0        0      635 2023-04-20 08:06:54.531840 torchchronos-0.0.2/torchchronos/transforms/padding.py
--rw-r--r--   0        0        0      202 2023-04-20 08:07:10.115949 torchchronos-0.0.2/torchchronos/typing.py
--rw-r--r--   0        0        0     1338 2023-04-20 08:06:54.531840 torchchronos-0.0.2/torchchronos/utils.py
--rw-r--r--   0        0        0     4483 1970-01-01 00:00:00.000000 torchchronos-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/LICENSE
+-rw-r--r--   0        0        0     4121 2023-04-26 23:13:27.917850 torchchronos-0.0.3.post1/README.md
+-rw-r--r--   0        0        0      687 2023-04-26 23:13:27.917850 torchchronos-0.0.3.post1/pyproject.toml
+-rw-r--r--   0        0        0       19 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/datasets/__init__.py
+-rw-r--r--   0        0        0     3557 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/datasets/tfc_pretrain.py
+-rw-r--r--   0        0        0     3963 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/datasets/ucr_uea.py
+-rw-r--r--   0        0        0     2896 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/download.py
+-rw-r--r--   0        0        0      166 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/errors.py
+-rw-r--r--   0        0        0      143 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/lightning/__init__.py
+-rw-r--r--   0        0        0     2320 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/lightning/tfc_pretrain.py
+-rw-r--r--   0        0        0     6281 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/lightning/ucr_uea.py
+-rw-r--r--   0        0        0      135 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/transforms/__init__.py
+-rw-r--r--   0        0        0      868 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/transforms/base.py
+-rw-r--r--   0        0        0      635 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/transforms/padding.py
+-rw-r--r--   0        0        0      202 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/typing.py
+-rw-r--r--   0        0        0     1494 2023-04-26 23:13:13.373840 torchchronos-0.0.3.post1/torchchronos/utils.py
+-rw-r--r--   0        0        0     4939 1970-01-01 00:00:00.000000 torchchronos-0.0.3.post1/PKG-INFO
```

### Comparing `torchchronos-0.0.2/LICENSE` & `torchchronos-0.0.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchchronos-0.0.2/README.md` & `torchchronos-0.0.3.post1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # torchchronos
 
 [![PyPI version](https://img.shields.io/pypi/v/torchchronos.svg?color=blue)](https://pypi.org/project/torchchronos)
-[![license](https://img.shields.io/pypi/l/torchchronos.svg?color=blue)](https://github.com/felixdivo/torchchronos/blob/main/LICENSE)
+[![license](https://img.shields.io/pypi/l/torchchronos.svg?color=blue)](https://github.com/mauricekraus/torchchronos/blob/main/LICENSE)
 [![python version](https://img.shields.io/badge/python-3.10+-blue)](https://devguide.python.org/versions/)
 
 [![test](https://github.com/mauricekraus/torchchronos/actions/workflows/main.yml/badge.svg)](https://github.com/mauricekraus/torchchronos/actions/workflows/main.yml)
 [![code style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 *torchchronos* is an experimental [PyTorch](https://pytorch.org/) and [Lightning](https://lightning.ai/pytorch-lightning/) compatible library that provides easy and flexible access to various time-series datasets for classification and regression tasks. It also provides a simple and extensible transform API to preprocess data.
 It is inspired by the much more complicated [torchtime](https://github.com/philipdarke/torchtime).
@@ -25,15 +25,15 @@
 To use a dataset, you can simply import the corresponding dataset class and create an instance:
 
 ```python
 from torchchronos.datasets import UCRUEADataset
 from torchchronos.transforms import PadFront
 from torchchronos.download import download_uea_ucr
 
-download_uea_ucr(Path(".cache/data"), "ECG5000")
+download_uea_ucr("ECG5000",Path(".cache/data"))
 dataset = UCRUEADataset('ECG5000', path=Path(".cache") / "data", transforms=PadFront(10))
 ```
 
 ### Data Modules
 torchchronos also provides [Lightning compatible `DataModules`](https://lightning.ai/docs/pytorch/stable/data/datamodule.html) to make it easy to load and preprocess data. They support common use cases like (multi-)GPU training and train/test/val-splitting out of the box. For example:
 
 ```python
@@ -63,14 +63,19 @@
         self.mean = data.mean()
         self.std = data.std()
 
     def __call__(self, data):
         return (data - self.mean) / self.std
 ```
 
+## Known issues
+- The dataset [SpokenArabicDigits](https://www.timeseriesclassification.com/description.php?Dataset=SpokenArabicDigits) does not seem to work due to a missmatch of TRAIN and TEST size
+- The dataset [UrbanSound](https://www.timeseriesclassification.com/description.php?Dataset=UrbanSound) does not seem to work due to missing ts files
+
+
 ## Roadmap
 The following features are planned for future releases of torchchronos:
 
 - Support for additional time-series datasets, including:
     - Energy consumption dataset
     - Traffic dataset
     - PhysioNet Challenge 2012 (in-hospital mortality)
```

### Comparing `torchchronos-0.0.2/pyproject.toml` & `torchchronos-0.0.3.post1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "torchchronos"
-version = "0.0.2"
+version = "0.0.3-post1"
 authors = ["Maurice Kraus <dev@mkraus.io>"]
 readme = "README.md"
 description = "PyTorch and Lightning compatible library that provides easy and flexible access to various time-series datasets for classification and regression tasks"
 license = "MIT"
+homepage = "https://github.com/mauricekraus/torchchronos"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 sktime = "^0.16.1"
 torch = "^2.0.0"
 lightning = "^2.0.0"
 fastapi = { version = "^0.88.0" }
+uplink = "^0.9.7"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `torchchronos-0.0.2/torchchronos/datasets/tfc_pretrain.py` & `torchchronos-0.0.3.post1/torchchronos/datasets/tfc_pretrain.py`

 * *Files identical despite different names*

### Comparing `torchchronos-0.0.2/torchchronos/lightning/tfc_pretrain.py` & `torchchronos-0.0.3.post1/torchchronos/lightning/tfc_pretrain.py`

 * *Files identical despite different names*

### Comparing `torchchronos-0.0.2/torchchronos/transforms/base.py` & `torchchronos-0.0.3.post1/torchchronos/transforms/base.py`

 * *Files identical despite different names*

### Comparing `torchchronos-0.0.2/torchchronos/transforms/padding.py` & `torchchronos-0.0.3.post1/torchchronos/transforms/padding.py`

 * *Files identical despite different names*

### Comparing `torchchronos-0.0.2/torchchronos/utils.py` & `torchchronos-0.0.3.post1/torchchronos/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,35 +16,41 @@
 @dataclass
 class TSInfo:
     num_classes: int
     series_length: int
     equal_length: bool
     dimensions: int
     univariate: bool
+    missing: bool
 
 
 def parse_ts(path: Path):
     num_classes = 0
     series_length = -1
     equal_length = False
     dimensions = -1
     univariate = False
+    missing = False
 
     with path.open("r") as f:
         for line in f:
             if "@data" in line:
                 break
 
             split = line.strip().split(" ")
             if split[0] == "@classLabel":
                 if split[1] == "true":
                     num_classes = len(split[2:])
             elif split[0] == "@seriesLength" and split[1].isdigit():
                 series_length = int(split[1])
             elif split[0] == "@equalLength" and split[1] == "true":
                 equal_length = True
+            elif split[0] == "@missing" and split[1] == "true":
+                missing = True
             elif split[0] == "@dimensions" and split[1].isdigit():
                 dimensions = int(split[1])
             elif split[0] == "@univariate" and split[1] == "true":
                 univariate = True
                 dimensions = 1
-    return TSInfo(num_classes, series_length, equal_length, dimensions, univariate)
+    return TSInfo(
+        num_classes, series_length, equal_length, dimensions, univariate, missing
+    )
```

### Comparing `torchchronos-0.0.2/PKG-INFO` & `torchchronos-0.0.3.post1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: torchchronos
-Version: 0.0.2
+Version: 0.0.3.post1
 Summary: PyTorch and Lightning compatible library that provides easy and flexible access to various time-series datasets for classification and regression tasks
+Home-page: https://github.com/mauricekraus/torchchronos
 License: MIT
 Author: Maurice Kraus
 Author-email: dev@mkraus.io
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.88.0,<0.89.0)
 Requires-Dist: lightning (>=2.0.0,<3.0.0)
 Requires-Dist: sktime (>=0.16.1,<0.17.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
+Requires-Dist: uplink (>=0.9.7,<0.10.0)
 Description-Content-Type: text/markdown
 
 # torchchronos
 
 [![PyPI version](https://img.shields.io/pypi/v/torchchronos.svg?color=blue)](https://pypi.org/project/torchchronos)
-[![license](https://img.shields.io/pypi/l/torchchronos.svg?color=blue)](https://github.com/felixdivo/torchchronos/blob/main/LICENSE)
+[![license](https://img.shields.io/pypi/l/torchchronos.svg?color=blue)](https://github.com/mauricekraus/torchchronos/blob/main/LICENSE)
 [![python version](https://img.shields.io/badge/python-3.10+-blue)](https://devguide.python.org/versions/)
 
 [![test](https://github.com/mauricekraus/torchchronos/actions/workflows/main.yml/badge.svg)](https://github.com/mauricekraus/torchchronos/actions/workflows/main.yml)
 [![code style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 *torchchronos* is an experimental [PyTorch](https://pytorch.org/) and [Lightning](https://lightning.ai/pytorch-lightning/) compatible library that provides easy and flexible access to various time-series datasets for classification and regression tasks. It also provides a simple and extensible transform API to preprocess data.
 It is inspired by the much more complicated [torchtime](https://github.com/philipdarke/torchtime).
@@ -43,15 +45,15 @@
 To use a dataset, you can simply import the corresponding dataset class and create an instance:
 
 ```python
 from torchchronos.datasets import UCRUEADataset
 from torchchronos.transforms import PadFront
 from torchchronos.download import download_uea_ucr
 
-download_uea_ucr(Path(".cache/data"), "ECG5000")
+download_uea_ucr("ECG5000",Path(".cache/data"))
 dataset = UCRUEADataset('ECG5000', path=Path(".cache") / "data", transforms=PadFront(10))
 ```
 
 ### Data Modules
 torchchronos also provides [Lightning compatible `DataModules`](https://lightning.ai/docs/pytorch/stable/data/datamodule.html) to make it easy to load and preprocess data. They support common use cases like (multi-)GPU training and train/test/val-splitting out of the box. For example:
 
 ```python
@@ -81,14 +83,19 @@
         self.mean = data.mean()
         self.std = data.std()
 
     def __call__(self, data):
         return (data - self.mean) / self.std
 ```
 
+## Known issues
+- The dataset [SpokenArabicDigits](https://www.timeseriesclassification.com/description.php?Dataset=SpokenArabicDigits) does not seem to work due to a missmatch of TRAIN and TEST size
+- The dataset [UrbanSound](https://www.timeseriesclassification.com/description.php?Dataset=UrbanSound) does not seem to work due to missing ts files
+
+
 ## Roadmap
 The following features are planned for future releases of torchchronos:
 
 - Support for additional time-series datasets, including:
     - Energy consumption dataset
     - Traffic dataset
     - PhysioNet Challenge 2012 (in-hospital mortality)
```


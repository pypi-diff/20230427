# Comparing `tmp/quantuloop_simulator-2023.4.tar.gz` & `tmp/quantuloop_simulator-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantuloop_simulator-2023.4.tar", max compression
+gzip compressed data, was "quantuloop_simulator-2023.4.1.tar", max compression
```

## Comparing `quantuloop_simulator-2023.4.tar` & `quantuloop_simulator-2023.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11546 2023-02-17 18:11:32.487403 quantuloop_simulator-2023.4/LICENSE
--rw-r--r--   0        0        0     3480 2023-04-03 18:35:19.192945 quantuloop_simulator-2023.4/README.md
--rw-r--r--   0        0        0      670 2023-04-03 18:27:14.865405 quantuloop_simulator-2023.4/pyproject.toml
--rw-r--r--   0        0        0     3901 2023-04-03 18:32:51.323253 quantuloop_simulator-2023.4/src/quantuloop_simulator/__init__.py
--rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 quantuloop_simulator-2023.4/setup.py
--rw-r--r--   0        0        0     4155 1970-01-01 00:00:00.000000 quantuloop_simulator-2023.4/PKG-INFO
+-rw-r--r--   0        0        0    11546 2023-04-27 20:18:00.209120 quantuloop_simulator-2023.4.1/LICENSE
+-rw-r--r--   0        0        0     3480 2023-04-27 20:18:00.209120 quantuloop_simulator-2023.4.1/README.md
+-rw-r--r--   0        0        0      674 2023-04-27 20:19:37.082320 quantuloop_simulator-2023.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3848 2023-04-27 20:24:23.873873 quantuloop_simulator-2023.4.1/src/quantuloop_simulator/__init__.py
+-rw-r--r--   0        0        0     4340 1970-01-01 00:00:00.000000 quantuloop_simulator-2023.4.1/setup.py
+-rw-r--r--   0        0        0     4161 1970-01-01 00:00:00.000000 quantuloop_simulator-2023.4.1/PKG-INFO
```

### Comparing `quantuloop_simulator-2023.4/LICENSE` & `quantuloop_simulator-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quantuloop_simulator-2023.4/README.md` & `quantuloop_simulator-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `quantuloop_simulator-2023.4/pyproject.toml` & `quantuloop_simulator-2023.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "quantuloop-simulator"
-version = "2023.04"
+version = "2023.04.1"
 description = "Quantuloop Quantum Simulator Suite for HPC"
 authors = ["Quantuloop <dev@quantuloop.com>"]
 readme = "README.md"
 packages = [{include = "quantuloop_simulator", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-quantuloop-quest = "^0.2"
+quantuloop-quest = "^0.2.1"
 quantuloop-dense = "^0.2"
 quantuloop-sparse = "^0.2"
 
 
 [[tool.poetry.source]]
 name = "quantuloop"
 url = "https://gitlab.com/api/v4/projects/43029789/packages/pypi/simple"
```

### Comparing `quantuloop_simulator-2023.4/src/quantuloop_simulator/__init__.py` & `quantuloop_simulator-2023.4.1/src/quantuloop_simulator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 import quantuloop_sparse
 import quantuloop_quest
 
 
 def set_simulator(simulator: Literal['Dense', 'Sparse', 'QuEST'] | None = None, *,
                   token: str | None = None,
                   token_file: PathLike | None = None,
-                  seed: int | None = None,
-                  dump_type: str | None = None,
+                  seed: any | None = None,
+                  dump_type: Literal['vector',
+                                     'probability', 'shots'] | None = None,
                   shots: int | None = None,
                   gpu_count: int | None = None,
-                  precision: int | None = None):
+                  precision: Literal[1, 2] | None = None):
     """Set a Quantuloop simulator as the quantum execution target
 
     Args:
         token: A Quantuloop Access Token. This token is used to authenticate access to the
             simulator. If you do not provide a token, the simulator will not work.
         token_file: A file containing the Quantuloop Access Token. The file must contain a
             single line with the access token. If you specify both a token and a token file,
@@ -50,19 +51,14 @@
 
     if token_file is not None:
         with open(token_file, 'r') as file:
             token = file.read()
     if token is not None:
         environ['QULOOP_TOKEN'] = str(token)
 
-    if seed is not None:
-        if seed < 0:
-            raise ValueError('parameter "seed" must be greater than zero')
-        environ['QULOOP_SEED'] = str(seed)
-
     if dump_type:
         if dump_type not in ["vector", "probability", "shots"]:
             raise ValueError(
                 'parameter "dump_type" must be "vector", "probability", or "shots"')
         environ['QULOOP_DUMP_TYPE'] = dump_type
 
     if shots:
@@ -81,12 +77,12 @@
     if simulator is not None:
         simulator = str(simulator).lower()
         if simulator not in ["dense", "sparse", "quest"]:
             raise ValueError(
                 'parameter "simulator" must be "dense", "sparse", "quest"')
 
         if simulator == "dense":
-            quantuloop_dense.set_simulator()
+            quantuloop_dense.set_simulator(seed=seed)
         elif simulator == "sparse":
-            quantuloop_sparse.set_simulator()
+            quantuloop_sparse.set_simulator(seed=seed)
         elif simulator == "quest":
-            quantuloop_quest.set_simulator()
+            quantuloop_quest.set_simulator(seed=seed)
```

### Comparing `quantuloop_simulator-2023.4/setup.py` & `quantuloop_simulator-2023.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 ['quantuloop_simulator']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['quantuloop-dense>=0.2,<0.3',
- 'quantuloop-quest>=0.2,<0.3',
+ 'quantuloop-quest>=0.2.1,<0.3.0',
  'quantuloop-sparse>=0.2,<0.3']
 
 setup_kwargs = {
     'name': 'quantuloop-simulator',
-    'version': '2023.4',
+    'version': '2023.4.1',
     'description': 'Quantuloop Quantum Simulator Suite for HPC',
     'long_description': '# Quantuloop Quantum Simulator Suite for HPC\n\nThe **Quantuloop Quantum Simulator Suite for HPC** is a collection of high-performance quantum computer simulators for the **Ket language**. Since quantum algorithms explore distinct aspects of quantum computation to extract advantages, there is no silver bullet for the simulation of a quantum computer. The Quantuloop Quantum Simulator Suite for HPC offers three quantum simulators today, with new ones coming in the future. The simulators available today are:\n\n* **Quantuloop Sparse**, which brings the Bitwise Representation (implemented in the KBW Sparse) for HPC. This is the only simulator that implements this simulation algorithm and it provides many benefits:\n  * Ready for multi-GPU systems, allowing you to scale up simulations as needed.\n  * Efficient execution time with the amount of superposition, providing faster simulations.\n  * Exact simulation of more than 100 qubits [depending on the algorithm](https://repositorio.ufsc.br/handle/123456789/231060), making it ideal for larger simulations.\n* **Quantuloop Dense** is a state vector simulator built with the NVIDIA cuQuantum SDK cuStateVec. It provides several advantages:\n  * Great scalability in multi-GPU systems, enabling large simulations to be run with ease.\n  * The perfect fit for most quantum algorithms, allowing you to simulate many different types of quantum circuits.\n* **Quantuloop QuEST**, which is an interface for the open-source simulator QuEST. It provides many benefits, including:\n  * Excellent performance for single GPU systems, allowing you to run simulations even if you don\'t have access to multiple GPUs.\n\nBy using the Quantuloop Quantum Simulator Suite for HPC, you can enjoy the following benefits:\n\n* Faster simulation times, as the simulators are optimized for GPU-based computing.\n* Higher scalability, as multi-GPU systems, can be used to run large simulations.\n* Access to unique simulation algorithms, such as the Parallel Bitwise implemented in the Quantuloop Sparse simulator.\n* Ability to simulate a wide range of quantum algorithms and circuits, allowing you to explore the potential of quantum computing.\n\nThe use of this simulator is exclusively for Quantuloop\'s customers and partners. Contact your institution to get your access token or visit <https://quantuloop.com>.\n\n## Installation  \n\nInstalling using pip:\n\n```shell\npip install --index-url https://gitlab.com/api/v4/projects/43029789/packages/pypi/simple quantuloop-simulator\n```\n\nAdd in poetry:\n\n```shell\npoetry source add quantuloop https://gitlab.com/api/v4/projects/43029789/packages/pypi/simple --secondary\npoetry add quantuloop-simulator\n```\n\n## Usage\n\n```py\nimport quantuloop_simulator as ql\n\nql.set_simulator(\n    "Sparse", # or "Dense" or "QuEST"\n    token="YOR.ACCESS.TOKEN", # Quantuloop Access Token is required to use the simulators \n    precision=2, # optional, default 1\n    gpu_count=4, # optional, default use all GPUs\n)\n```\n\n## Compatibility\n\nThe following system requirements are necessary to run the Quantuloop Dense simulator:\n\n* CUDA 11.2 or newer with compatible NVIDIA driver\n* Linux x86_64 with glibc 2.17 or newer\n  * Ubuntu 18.04 or newer.\n  * Red Hat Enterprise Linux 7 or newer.\n* Python 3.7 or newer\n* Ket 0.5.x\n\nQuantuloop Dense is compatible only with CUDA architecture 70, 75, 80, and 86.\n\n----\n\nBy installing or using this package, you agree to the Quantuloop Quantum Simulator Suite EULA.\n\nAll rights reserved (C) 2023 Quantuloop\n',
     'author': 'Quantuloop',
     'author_email': 'dev@quantuloop.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `quantuloop_simulator-2023.4/PKG-INFO` & `quantuloop_simulator-2023.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: quantuloop-simulator
-Version: 2023.4
+Version: 2023.4.1
 Summary: Quantuloop Quantum Simulator Suite for HPC
 Author: Quantuloop
 Author-email: dev@quantuloop.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: quantuloop-dense (>=0.2,<0.3)
-Requires-Dist: quantuloop-quest (>=0.2,<0.3)
+Requires-Dist: quantuloop-quest (>=0.2.1,<0.3.0)
 Requires-Dist: quantuloop-sparse (>=0.2,<0.3)
 Description-Content-Type: text/markdown
 
 # Quantuloop Quantum Simulator Suite for HPC
 
 The **Quantuloop Quantum Simulator Suite for HPC** is a collection of high-performance quantum computer simulators for the **Ket language**. Since quantum algorithms explore distinct aspects of quantum computation to extract advantages, there is no silver bullet for the simulation of a quantum computer. The Quantuloop Quantum Simulator Suite for HPC offers three quantum simulators today, with new ones coming in the future. The simulators available today are:
```


# Comparing `tmp/phlearn-1.0.0.tar.gz` & `tmp/phlearn-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phlearn-1.0.0.tar", last modified: Wed Jan 18 14:30:23 2023, max compression
+gzip compressed data, was "phlearn-1.1.0.tar", last modified: Thu Apr 27 14:10:25 2023, max compression
```

## Comparing `phlearn-1.0.0.tar` & `phlearn-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,54 @@
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-01-18 14:30:23.443200 phlearn-1.0.0/
--rw-r--r--   0 eeb        (501) staff       (20)     1075 2023-01-18 13:51:50.000000 phlearn-1.0.0/LICENSE.txt
--rw-r--r--   0 eeb        (501) staff       (20)      996 2023-01-18 14:30:23.442700 phlearn-1.0.0/PKG-INFO
--rw-r--r--   0 eeb        (501) staff       (20)      513 2023-01-18 13:51:50.000000 phlearn-1.0.0/README.md
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-01-18 14:30:23.426081 phlearn-1.0.0/phlearn/
--rw-r--r--   0 eeb        (501) staff       (20)      517 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/__init__.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-01-18 14:30:23.433029 phlearn-1.0.0/phlearn/control/
--rw-r--r--   0 eeb        (501) staff       (20)      740 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/control/__init__.py
--rw-r--r--   0 eeb        (501) staff       (20)     3818 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/control/casadiNN.py
--rw-r--r--   0 eeb        (501) staff       (20)     1238 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/control/casadiPH.py
--rw-r--r--   0 eeb        (501) staff       (20)    15443 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/control/mpc.py
--rw-r--r--   0 eeb        (501) staff       (20)     3017 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/control/phcontroller.py
--rw-r--r--   0 eeb        (501) staff       (20)     4708 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/control/pid.py
--rw-r--r--   0 eeb        (501) staff       (20)     2554 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/control/reference.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-01-18 14:30:23.436718 phlearn-1.0.0/phlearn/phnns/
--rw-r--r--   0 eeb        (501) staff       (20)     1900 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/phnns/__init__.py
--rw-r--r--   0 eeb        (501) staff       (20)    10785 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/phnns/dynamic_system_neural_network.py
--rw-r--r--   0 eeb        (501) staff       (20)    19199 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/phnns/models.py
--rw-r--r--   0 eeb        (501) staff       (20)    16585 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/phnns/pseudo_hamiltonian_neural_network.py
--rw-r--r--   0 eeb        (501) staff       (20)    18488 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/phnns/train_utils.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-01-18 14:30:23.439755 phlearn-1.0.0/phlearn/phsystems/
--rw-r--r--   0 eeb        (501) staff       (20)     1003 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/phsystems/__init__.py
--rw-r--r--   0 eeb        (501) staff       (20)     2443 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/phsystems/msd_system.py
--rw-r--r--   0 eeb        (501) staff       (20)     9600 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/phsystems/pseudo_Hamiltonian_system.py
--rw-r--r--   0 eeb        (501) staff       (20)     7134 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/phsystems/tank_system.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-01-18 14:30:23.441841 phlearn-1.0.0/phlearn/utils/
--rw-r--r--   0 eeb        (501) staff       (20)      433 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/utils/__init__.py
--rw-r--r--   0 eeb        (501) staff       (20)     2830 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/utils/derivatives.py
--rw-r--r--   0 eeb        (501) staff       (20)      566 2023-01-18 13:51:50.000000 phlearn-1.0.0/phlearn/utils/utils.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-01-18 14:30:23.428142 phlearn-1.0.0/phlearn.egg-info/
--rw-r--r--   0 eeb        (501) staff       (20)      996 2023-01-18 14:30:23.000000 phlearn-1.0.0/phlearn.egg-info/PKG-INFO
--rw-r--r--   0 eeb        (501) staff       (20)      792 2023-01-18 14:30:23.000000 phlearn-1.0.0/phlearn.egg-info/SOURCES.txt
--rw-r--r--   0 eeb        (501) staff       (20)        1 2023-01-18 14:30:23.000000 phlearn-1.0.0/phlearn.egg-info/dependency_links.txt
--rw-r--r--   0 eeb        (501) staff       (20)       64 2023-01-18 14:30:23.000000 phlearn-1.0.0/phlearn.egg-info/requires.txt
--rw-r--r--   0 eeb        (501) staff       (20)        8 2023-01-18 14:30:23.000000 phlearn-1.0.0/phlearn.egg-info/top_level.txt
--rw-r--r--   0 eeb        (501) staff       (20)       38 2023-01-18 14:30:23.443394 phlearn-1.0.0/setup.cfg
--rw-r--r--   0 eeb        (501) staff       (20)      927 2023-01-18 14:24:59.000000 phlearn-1.0.0/setup.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.136832 phlearn-1.1.0/
+-rw-r--r--   0 eeb        (501) staff       (20)     1075 2023-04-27 14:08:31.000000 phlearn-1.1.0/LICENSE.txt
+-rw-r--r--   0 eeb        (501) staff       (20)     1020 2023-04-27 14:10:25.136383 phlearn-1.1.0/PKG-INFO
+-rw-r--r--   0 eeb        (501) staff       (20)      513 2023-04-27 14:08:31.000000 phlearn-1.1.0/README.md
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.107239 phlearn-1.1.0/phlearn/
+-rw-r--r--   0 eeb        (501) staff       (20)      640 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/__init__.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.116982 phlearn-1.1.0/phlearn/control/
+-rw-r--r--   0 eeb        (501) staff       (20)      740 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/__init__.py
+-rw-r--r--   0 eeb        (501) staff       (20)     3971 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/casadiNN.py
+-rw-r--r--   0 eeb        (501) staff       (20)     1386 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/casadiPH.py
+-rw-r--r--   0 eeb        (501) staff       (20)    15597 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/mpc.py
+-rw-r--r--   0 eeb        (501) staff       (20)     3017 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/phcontroller.py
+-rw-r--r--   0 eeb        (501) staff       (20)     4708 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/pid.py
+-rw-r--r--   0 eeb        (501) staff       (20)     2554 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/reference.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.122729 phlearn-1.1.0/phlearn/phnns/
+-rw-r--r--   0 eeb        (501) staff       (20)     2075 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/__init__.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)    22515 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/conservative_dissipative_neural_network.py
+-rw-r--r--   0 eeb        (501) staff       (20)    12511 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/dynamic_system_neural_network.py
+-rw-r--r--   0 eeb        (501) staff       (20)    32704 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/models.py
+-rw-r--r--   0 eeb        (501) staff       (20)    17459 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/pseudo_hamiltonian_neural_network.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.123666 phlearn-1.1.0/phlearn/phnns/tests/
+-rw-r--r--   0 eeb        (501) staff       (20)        0 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/tests/__init__.py
+-rw-r--r--   0 eeb        (501) staff       (20)     2113 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/tests/test_phnns.py
+-rw-r--r--   0 eeb        (501) staff       (20)    23204 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/train_utils.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.131787 phlearn-1.1.0/phlearn/phsystems/
+-rw-r--r--   0 eeb        (501) staff       (20)     1957 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/__init__.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)     2867 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/allen_cahn_system.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)     3281 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/bbm_system.py
+-rw-r--r--   0 eeb        (501) staff       (20)     4345 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/burgers_system.py
+-rw-r--r--   0 eeb        (501) staff       (20)     3001 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/cahn_hilliard_system.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)    13517 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/conservative_dissipative_system.py
+-rw-r--r--   0 eeb        (501) staff       (20)     3790 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/fvm.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)     3063 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/heat_system.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)     2983 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/kdv_system.py
+-rw-r--r--   0 eeb        (501) staff       (20)     2443 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/msd_system.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)     3322 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/perona_malik_system.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)     3318 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/phase_system.py
+-rw-r--r--   0 eeb        (501) staff       (20)    10873 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/pseudo_Hamiltonian_system.py
+-rw-r--r--   0 eeb        (501) staff       (20)     7230 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/tank_system.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.133056 phlearn-1.1.0/phlearn/phsystems/tests/
+-rw-r--r--   0 eeb        (501) staff       (20)        0 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/tests/__init__.py
+-rw-r--r--   0 eeb        (501) staff       (20)     3051 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/tests/test_phsystems.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.135517 phlearn-1.1.0/phlearn/utils/
+-rw-r--r--   0 eeb        (501) staff       (20)      433 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/utils/__init__.py
+-rw-r--r--   0 eeb        (501) staff       (20)     4481 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/utils/derivatives.py
+-rw-r--r--   0 eeb        (501) staff       (20)     4293 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/utils/utils.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.110180 phlearn-1.1.0/phlearn.egg-info/
+-rw-r--r--   0 eeb        (501) staff       (20)     1020 2023-04-27 14:10:25.000000 phlearn-1.1.0/phlearn.egg-info/PKG-INFO
+-rw-r--r--   0 eeb        (501) staff       (20)     1360 2023-04-27 14:10:25.000000 phlearn-1.1.0/phlearn.egg-info/SOURCES.txt
+-rw-r--r--   0 eeb        (501) staff       (20)        1 2023-04-27 14:10:25.000000 phlearn-1.1.0/phlearn.egg-info/dependency_links.txt
+-rw-r--r--   0 eeb        (501) staff       (20)      146 2023-04-27 14:10:25.000000 phlearn-1.1.0/phlearn.egg-info/requires.txt
+-rw-r--r--   0 eeb        (501) staff       (20)        8 2023-04-27 14:10:25.000000 phlearn-1.1.0/phlearn.egg-info/top_level.txt
+-rw-r--r--   0 eeb        (501) staff       (20)       38 2023-04-27 14:10:25.136998 phlearn-1.1.0/setup.cfg
+-rw-r--r--   0 eeb        (501) staff       (20)     1072 2023-04-27 14:08:31.000000 phlearn-1.1.0/setup.py
```

### Comparing `phlearn-1.0.0/LICENSE.txt` & `phlearn-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phlearn-1.0.0/PKG-INFO` & `phlearn-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: phlearn
-Version: 1.0.0
+Version: 1.1.0
 Summary: A package for simulating and learning pseudo-Hamiltonian systems. For further details, see https://arxiv.org/pdf/2206.02660.pdf
 Home-page: https://gitlab.sintef.no/hybrid-machine-learning/pseudo-Hamiltonian-neural-networks
 Author: Sølve Eidnes
 Author-email: solve.eidnes@sintef.no
 License: MIT
 Keywords: pseudo-Hamiltonian neural networks
 Classifier: Development Status :: 5 - Production/Stable
+Provides-Extra: control
 License-File: LICENSE.txt
 
 # phlearn
 Package for modelling pseudo-Hamiltonian systems with neural networks as described in [(Eidnes et al. 2022)](https://arxiv.org/pdf/2206.02660.pdf).
 
 [Documentation available here](https://pseudo-Hamiltonian-neural-networks.readthedocs.io/en/latest/)
```

### Comparing `phlearn-1.0.0/README.md` & `phlearn-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `phlearn-1.0.0/phlearn/__init__.py` & `phlearn-1.1.0/phlearn/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,16 @@
   pseudo-Hamiltonian neural networks
 
 - :py:mod:`~.control` for control functionality
 
 - :py:mod:`~.utils` for convenience functions.
 
 """
-
-from . import control
+try:
+  from . import control
+except ModuleNotFoundError:
+  # from warnings import warn
+  # warn("Loading phlearn without control module")
+  pass 
 from . import phnns
 from . import phsystems
 from . import utils
```

### Comparing `phlearn-1.0.0/phlearn/control/__init__.py` & `phlearn-1.1.0/phlearn/control/__init__.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.0.0/phlearn/control/casadiNN.py` & `phlearn-1.1.0/phlearn/control/casadiNN.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-from casadi import *
-import casadi.tools
+try:
+    from casadi import *
+    import casadi.tools
+except ModuleNotFoundError:
+    raise ModuleNotFoundError("To use the phlearn.control module install via 'pip install phlearn[control]' ")
+
 
 
 class CasadiFCNN:
     """
     Casadi-implementation of a fully-connected neural network. The class
     takes in a specification of a neural network
     model and implements the specification as a Casadi function.
```

### Comparing `phlearn-1.0.0/phlearn/control/casadiPH.py` & `phlearn-1.1.0/phlearn/control/casadiPH.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from casadi import *
+try:
+    from casadi import *
+except ModuleNotFoundError:
+    raise ModuleNotFoundError("To use the phlearn.control module install via 'pip install phlearn[control]' ")
 
 
 class CasadiPseudoHamiltonianSystem:
     """
     Casadi implementation of the pseudo-Hamiltonian framework, modeling a
     system of the form::
```

### Comparing `phlearn-1.0.0/phlearn/control/mpc.py` & `phlearn-1.1.0/phlearn/control/mpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from .phcontroller import PseudoHamiltonianController
 from ..phnns.models import R_estimator
 from .casadiPH import CasadiPseudoHamiltonianSystem
 from .casadiNN import CasadiFCNN, get_pytorch_model_parameters, get_pytorch_model_architecture
-import do_mpc
 import numpy as np
-import casadi
 import torch
 
+try:
+    import do_mpc
+    import casadi
+except ModuleNotFoundError:
+    raise ModuleNotFoundError("To use the phlearn.control module install via 'pip install phlearn[control]' ")
+
+
 __all__ = ['PseudoHamiltonianMPC']
 
 
 class PseudoHamiltonianMPC(PseudoHamiltonianController):
     """
     This class implements a model predictive controller (MPC) that
     solves an optimal control problem to decide control inputs,
```

### Comparing `phlearn-1.0.0/phlearn/control/phcontroller.py` & `phlearn-1.1.0/phlearn/control/phcontroller.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.0.0/phlearn/control/pid.py` & `phlearn-1.1.0/phlearn/control/pid.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.0.0/phlearn/control/reference.py` & `phlearn-1.1.0/phlearn/control/reference.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.0.0/phlearn/phnns/__init__.py` & `phlearn-1.1.0/phlearn/phnns/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -58,16 +58,19 @@
 
 """
 
 from . import dynamic_system_neural_network
 from .dynamic_system_neural_network import *
 from . import pseudo_hamiltonian_neural_network
 from .pseudo_hamiltonian_neural_network import *
+from . import conservative_dissipative_neural_network
+from .conservative_dissipative_neural_network import *
 from . import models
 from .models import *
 from . import train_utils
 from .train_utils import *
 
 __all__ = dynamic_system_neural_network.__all__.copy()
 __all__ += pseudo_hamiltonian_neural_network.__all__.copy()
+__all__ += conservative_dissipative_neural_network.__all__.copy()
 __all__ += models.__all__.copy()
 __all__ += train_utils.__all__.copy()
```

### Comparing `phlearn-1.0.0/phlearn/phnns/dynamic_system_neural_network.py` & `phlearn-1.1.0/phlearn/phnns/dynamic_system_neural_network.py`

 * *Files 13% similar despite different names*

```diff
@@ -84,28 +84,30 @@
     def time_derivative(self, integrator, *args, **kwargs):
         """
         See :py:meth:~`utils.derivatives.time_derivative`
         """
 
         return time_derivative(integrator, self.x_dot, *args, **kwargs)
 
+
     def simulate_trajectory(self, integrator, t_sample, x0=None,
-                            noise_std=0., reference=None):
+                            xspatial=None, noise_std=0., reference=None):
         """
         Simulate a trajectory using the rhs_model and sample at times
         *t_sample*.
 
         Parameters
         ----------
         integrator : str or False
             Specifies which solver to use during simulation. If False,
-            the problem is left to scipy's solve_ivp. If 'euler', the system
-            is simulated with the forward Euler method.
-            If 'midpoint', 'rk4' or 'srk4' the system is simulated with
-            the classic Runge-Kutta-4 method.
+            the problem is left to scipy's solve_ivp. If 'euler',
+            'midpoint', 'rk4' or 'srk4' the system is simulated with
+            the forward euler method, the implicit midpoint method,
+            the explicit Runge-Kutta 4 method or a symmetric fourth
+            order Runge-Kutta method, respectively.
         t_sample : (T, 1) tensor or ndarray
             Times at which the trajectory is sampled.
         x0 : (N,) tensor or ndarray, default None
             Initial condition. If None, an initial condition is sampled
             with the internal sampler.
         noise_std : number, default 0.
             Standard deviation of Gaussian white noise added to the
@@ -122,35 +124,45 @@
         """
 
         x0 = to_tensor(x0)
         if x0 is None:
             x0 = self._initial_condition_sampler(1)
 
         if not integrator and self.controller is None:
-            x_dot = lambda t, x: self.x_dot(
-                        torch.tensor(x.reshape(1, x.shape[-1]),
-                                     dtype=self.ttype),
-                        torch.tensor(np.array(t).reshape((1, 1)),
-                                     dtype=self.ttype)
-                        ).detach().numpy().flatten()
+            if xspatial is not None:
+                x_dot = lambda t, x: self._x_dot(
+                            torch.tensor(x.reshape(1, x.shape[-1]),
+                                        dtype=self.ttype),
+                            torch.tensor(np.array(t).reshape((1, 1)),
+                                        dtype=self.ttype),
+                            xspatial=torch.tensor(np.array(xspatial).reshape(1, xspatial.shape[-1]),
+                                        dtype=self.ttype)
+                            ).detach().numpy().flatten()
+            else:
+                x_dot = lambda t, x: self._x_dot(
+                            torch.tensor(x.reshape(1, x.shape[-1]),
+                                        dtype=self.ttype),
+                            torch.tensor(np.array(t).reshape((1, 1)),
+                                        dtype=self.ttype)
+                            ).detach().numpy().flatten()
             out_ivp = solve_ivp(fun=x_dot, t_span=(t_sample[0], t_sample[-1]),
                                 y0=x0.detach().numpy().flatten(),
                                 t_eval=t_sample, rtol=1e-10)
             xs = out_ivp['y'].T
             us = None
         else:
             t_sample = to_tensor(t_sample, self.ttype)
             if not integrator and self.controller is not None:
                 integrator = 'rk4'
                 print('Warning: Since the system contains a controller, '
                       'the rk4 integrator is used to simulate the trajectory '
                       'instead of solve_ivp.')
             elif integrator.lower() not in ['euler', 'rk4']:
                 print('Warning: Only explicit integrators euler and rk4 or no '
-                      'integrator (False) allowed for simulation. Ignoring '
+                      'integrator (False) allowed for inference. Ignoring '
                       f'integrator {integrator} and using rk4.')
                 integrator = 'rk4'
 
             if self.controller is not None:
                 self.controller.reset()
                 if reference is not None:
                     self.controller.set_reference(reference)
@@ -158,32 +170,47 @@
             x0 = x0.reshape(1, x0.shape[-1])
             xs = torch.zeros([nsteps, x0.shape[-1]])
             xs[0, :] = x0
 
             u = None
             us = torch.zeros([nsteps - 1, x0.shape[-1]])
 
-            for i, t_step in enumerate(t_sample[:-1]):
-                t_step = torch.squeeze(t_step).reshape(-1, 1)
-                if self.controller is not None:
-                    u = to_tensor(self.controller(xs[i, :], t_step),
-                                  self.ttype)
-                    us[i, :] = u
-                dt = t_sample[i + 1] - t_step
-                xs[i + 1, :] = xs[i, :] + dt*self.time_derivative(
-                    integrator, xs[i:i+1, :], xs[i:i+1, :],
-                    t_step, t_step, dt, u)
+            if xspatial is not None:
+                for i, t_step in enumerate(t_sample[:-1]):
+                    t_step = torch.squeeze(t_step).reshape(-1, 1)
+                    if self.controller is not None:
+                        u = to_tensor(self.controller(xs[i, :], t_step),
+                                    self.ttype)
+                        us[i, :] = u
+                    dt = t_sample[i + 1] - t_step
+                    xs[i + 1, :] = xs[i, :] + dt*self.time_derivative(
+                        integrator, xs[i:i+1, :], xs[i:i+1, :],
+                        t_step, t_step, dt, u, xspatial=torch.tensor(
+                                np.array(xspatial).reshape(1, xspatial.shape[-1]),
+                                dtype=self.ttype))
+            else:
+                for i, t_step in enumerate(t_sample[:-1]):
+                    t_step = torch.squeeze(t_step).reshape(-1, 1)
+                    if self.controller is not None:
+                        u = to_tensor(self.controller(xs[i, :], t_step),
+                                    self.ttype)
+                        us[i, :] = u
+                    dt = t_sample[i + 1] - t_step
+                    xs[i + 1, :] = xs[i, :] + dt*self.time_derivative(
+                        integrator, xs[i:i+1, :], xs[i:i+1, :],
+                        t_step, t_step, dt, u)
             xs = xs.detach().numpy()
             if self.controller is not None:
                 us = us.detach().numpy()
             else:
                 us = None
 
         return xs, us
 
+
     def simulate_trajectories(self, ntrajectories, integrator, t_sample,
                               x0=None, noise_std=0, references=None):
         """
         Calls :py:meth:`~DynamicSystemNN.simulate_trajectory`
         *ntrajectories* times.
 
         Parameters
@@ -267,19 +294,26 @@
     def set_controller(self, controller):
         """
         Set controller.
         """
 
         self.controller = controller
 
-    def _x_dot(self, x, t, u=None):
+    def lhs(self, dxdt):
+        return dxdt
+
+    def _x_dot(self, x, t, u=None, xspatial=None):
         x = to_tensor(x, self.ttype)
         t = to_tensor(t, self.ttype)
         u = to_tensor(u, self.ttype)
 
-        dynamics = self.rhs_model(x, t)
+        if xspatial is not None:
+            xspatial = to_tensor(xspatial, self.ttype)
+            dynamics = self.rhs_model(x, t, xspatial)
+        else:
+            dynamics = self.rhs_model(x, t)
         if u is not None:
             dynamics += u
         return dynamics
 
     def _initial_condition_sampler(self, nsamples=1):
         return 2*torch.rand((nsamples, self.nstates), dtype=self.ttype) - 1
```

### Comparing `phlearn-1.0.0/phlearn/phnns/pseudo_hamiltonian_neural_network.py` & `phlearn-1.1.0/phlearn/phnns/pseudo_hamiltonian_neural_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 import torch
+import numpy as np
 
 from .dynamic_system_neural_network import DynamicSystemNN
 from .models import HamiltonianNN, ExternalForcesNN, R_NN, R_estimator
 from ..utils.utils import to_tensor
 
 __all__ = ['PseudoHamiltonianNN', 'load_phnn_model', 'store_phnn_model']
 
@@ -84,38 +85,54 @@
             (nsamples, nstates) as input, returning a tensor of shape
             (nsamples, nstates).
 
     """
 
     def __init__(self,
                  nstates,
-                 structure_matrix,
+                 structure_matrix=None,
                  hamiltonian_true=None,
                  grad_hamiltonian_true=None,
                  dissipation_true=None,
                  external_forces_true=None,
                  hamiltonian_est=None,
                  dissipation_est=None,
                  external_forces_est=None,
                  **kwargs):
         super().__init__(nstates, **kwargs)
+        
+        if structure_matrix is None:
+            if nstates % 2 == 1:
+                raise Exception(
+                    "nstates must be even when structure_matrix not provided"
+                )
+            npos = nstates // 2
+            structure_matrix = np.block(
+                [
+                    [np.zeros([npos, npos]), np.eye(npos)],
+                    [-np.eye(npos), np.zeros([npos, npos])],
+                ]
+            )
+            
         self.S = None
         self.hamiltonian = None
         self.external_forces = None
         self.R = None
         self.hamiltonian_provided = False
         self.grad_hamiltonian_provided = False
         self.external_forces_provided = False
         self.dissipation_provided = False
+        self.nstates = nstates
         self.structure_matrix = structure_matrix
         self.hamiltonian_true = hamiltonian_true
         self.grad_hamiltonian_true = grad_hamiltonian_true
         self.dissipation_true = dissipation_true
         self.external_forces_true = external_forces_true
 
+        
         if not callable(structure_matrix):
             self.S = self._structure_matrix
         else:
             self.S = structure_matrix
 
         if dissipation_true is not None:
             self.dissipation_provided = True
@@ -135,20 +152,25 @@
                 self.dH = self._grad_hamiltonian_true
                 self.grad_hamiltonian_provided = True
             self.hamiltonian_provided = True
         elif grad_hamiltonian_true is not None:
             self.dH = self._grad_hamiltonian_true
             self.grad_hamiltonian_provided = True
         else:
-            self.hamiltonian = hamiltonian_est
+            if hamiltonian_est is not None:
+                self.hamiltonian = hamiltonian_est
+            else:
+                self.hamiltonian = HamiltonianNN(self.nstates)
             self.dH = self._dH_hamiltonian_est
 
         if external_forces_true is not None:
             self.external_forces = self._external_forces_true
             self.external_forces_provided = True
+        elif external_forces_true is None and external_forces_est is None:
+            self.external_forces = lambda x,t: 0
         else:
             self.external_forces = external_forces_est
 
     def _structure_matrix(self, x):
         return to_tensor(self.structure_matrix, self.ttype)
 
     def _hamiltonian_true(self, x):
@@ -174,22 +196,23 @@
 
     def _dH_hamiltonian_true(self, x):
         x = x.detach().requires_grad_()
         return torch.autograd.grad(self.hamiltonian(x).sum(), x,
                                    retain_graph=False,
                                    create_graph=False)[0].detach()
 
-    def _x_dot(self, x, t, u=None):
+    def _x_dot(self, x, t, u=None, xspatial=None):
         x = to_tensor(x, self.ttype)
         t = to_tensor(t, self.ttype)
         u = to_tensor(u, self.ttype)
 
         S = self.S(x)
         R = self.R(x)
         dH = self.dH(x)
+        
         if (len(S.shape) == 3) or (len(R.shape) == 3):
             dynamics = (torch.matmul(S - R, torch.atleast_3d(dH)
                                      ).reshape(x.shape)
                         + self.external_forces(x, t))
         else:
             dynamics = dH@(S.T - R.T) + self.external_forces(x, t)
         if u is not None:
@@ -317,21 +340,23 @@
 
     """
 
     metadict = {}
     metadict['nstates'] = model.nstates
     metadict['structure_matrix'] = model.structure_matrix
     metadict['hamiltonian_provided'] = model.hamiltonian_provided
-    metadict['grad_hamiltonian_provided'] = model.hamiltonian_provided
+    metadict['grad_hamiltonian_provided'] = model.grad_hamiltonian_provided
     metadict['external_forces_provided'] = model.external_forces_provided
     metadict['dissipation_provided'] = model.dissipation_provided
     metadict['init_sampler'] = model._initial_condition_sampler
     metadict['controller'] = model.controller
     metadict['ttype'] = model.ttype
 
+    metadict = {att.__name__ : att for att in model.__attr__}
+
     metadict['traininginfo'] = {}
     metadict['traininginfo']['optimizer_state_dict'] = optimizer.state_dict()
     for key, value in kwargs.items():
         metadict['traininginfo'][key] = value
 
     metadict['hamiltonian'] = {}
     metadict['grad_hamiltonian'] = {}
```

### Comparing `phlearn-1.0.0/phlearn/phnns/train_utils.py` & `phlearn-1.1.0/phlearn/phnns/train_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,57 @@
-
 import copy
 import datetime
 import os
 
 import numpy as np
 import torch
 import torch.nn as nn
+from tqdm import tqdm
+from tqdm import trange
 
-from .pseudo_hamiltonian_neural_network import (PseudoHamiltonianNN,
-                                              load_phnn_model,
-                                              store_phnn_model)
+from .pseudo_hamiltonian_neural_network import (
+    PseudoHamiltonianNN,
+    load_phnn_model,
+    store_phnn_model,
+)
+from .conservative_dissipative_neural_network import (
+    ConservativeDissipativeNN,
+    load_cdnn_model,
+    store_cdnn_model
+)
+from ..phsystems.pseudo_Hamiltonian_system import PseudoHamiltonianSystem
+from ..phsystems.conservative_dissipative_system import ConservativeDissipativeSystem
 from .models import load_baseline_model, store_baseline_model
 
-__all__ = ['generate_dataset', 'train', 'compute_validation_loss',
-           'batch_data', 'train_one_epoch', 'l1_loss_pHnn',
-           'npoints_to_ntrajectories_tsample', 'EarlyStopping',
-           'load_dynamic_system_model', 'store_dynamic_system_model']
-
-
-def generate_dataset(pH_system, ntrajectories, t_sample,
-                     true_derivatives=False, nsamples=None, seed=None,
-                     noise_std=0., references=None, ttype=torch.float32):
+__all__ = [
+    "generate_dataset",
+    "train",
+    "compute_validation_loss",
+    "batch_data",
+    "train_one_epoch",
+    "l1_loss_pHnn",
+    "npoints_to_ntrajectories_tsample",
+    "EarlyStopping",
+    "load_dynamic_system_model",
+    "store_dynamic_system_model",
+]
+
+
+def generate_dataset(
+    pH_system,
+    ntrajectories,
+    t_sample,
+    true_derivatives=False,
+    nsamples=None,
+    seed=None,
+    noise_std=0.0,
+    references=None,
+    xspatial=None,
+    ttype=torch.float32,
+):
     """
     Generate a dataset consisting of simulated data.
 
     Parameters
     ----------
     pH_system : phlearn.phsystems.PseudoHamiltonianSystem
     ntrajectories : int
@@ -42,26 +69,34 @@
     noise_std : number, default 0.
         Standard deviation of Gaussian white noise added to the
         samples of the trajectory.
     references : list of phlearn.control.Reference, default
         None
             If the *pH_system* has a controller, a list of ntrajectories
             reference objects may be passed.
+    xspatial : (1, M) ndarray
+        If *pH_system* is a discretized PDE system, this should be the
+        spatial points at which the system is discretized.
     ttype : torch type, default torch.float32
 
     Returns
     -------
 
-    (x_start, x_end, t_start, t_end, dt, u) : tuple
+    If the system is an ODE:
+        (x_start, x_end, t_start, t_end, dt, u) : tuple
+    If the system is a PDE:
+        (x_start, x_end, t_start, t_end, dt, u, xspatial) : tuple
+    with
         x_start : (ntrajectories * (T-1), N) or (nsamples, N) tensor
         x_end : (ntrajectories * (T-1), N) or (nsamples, N) tensor
         t_start : (ntrajectories * (T-1), 1) or (nsamples, 1) tensor
         t_end : (ntrajectories * (T-1), 1) or (nsamples, 1) tensor
         dt : (ntrajectories * (T-1), 1) or (nsamples, 1) tensor
         u : (ntrajectories * (T-1), N) or (nsamples, N) tensor
+        xspatial : (1, M) ndarray, same as input
     dxdt : (ntrajectories * (T-1), N) or (nsamples, N) tensor
 
     """
 
     if ntrajectories == 0:
         return None
     pH_system.seed(seed)
@@ -72,47 +107,84 @@
     t = np.zeros((ntrajectories, traj_length))
     u = np.zeros((ntrajectories, traj_length - 1, nstates))
     if references is None:
         references = [None] * ntrajectories
 
     for i in range(ntrajectories):
         x[i], dxdt[i], t[i], u[i] = pH_system.sample_trajectory(
-            t_sample, noise_std=noise_std, reference=references[i])
+            t_sample, noise_std=noise_std, reference=references[i]
+                                                                )
 
     dt = torch.tensor([t[0, 1] - t[0, 0]], dtype=ttype)
 
-    x_start = torch.tensor(x[:, :-1], dtype=ttype).reshape(-1, nstates)
-    x_end = torch.tensor(x[:, 1:], dtype=ttype).reshape(-1, nstates)
-    t_start = torch.tensor(t[:, :-1], dtype=ttype).reshape(-1, 1)
-    t_end = torch.tensor(t[:, 1:], dtype=ttype).reshape(-1, 1)
-    dt = dt*torch.ones_like(t_start, dtype=ttype)
-    if pH_system.controller is None:
+    if isinstance(pH_system, PseudoHamiltonianSystem):
+        x_start = torch.tensor(x[:, :-1], dtype=ttype).reshape(-1, nstates)
+        x_end = torch.tensor(x[:, 1:], dtype=ttype).reshape(-1, nstates)
+        t_start = torch.tensor(t[:, :-1], dtype=ttype).reshape(-1, 1)
+        t_end = torch.tensor(t[:, 1:], dtype=ttype).reshape(-1, 1)
+        dt = dt * torch.ones_like(t_start, dtype=ttype)
+        if pH_system.controller is None:
+            u = torch.zeros_like(x_start, dtype=ttype)
+        else:
+            u = torch.tensor(u[:, :-1], dtype=ttype).reshape(-1, nstates)
+        if true_derivatives:
+            dxdt = torch.tensor(dxdt[:, :-1], dtype=ttype).reshape(-1, nstates)
+        else:
+            dxdt = (x_end - x_start).clone().detach() / dt[0, 0]
+    elif isinstance(pH_system, ConservativeDissipativeSystem):
+        x_start = torch.tensor(x[:, :-1], dtype=ttype).reshape(-1, 1, nstates)
+        x_end = torch.tensor(x[:, 1:], dtype=ttype).reshape(-1, 1, nstates)
+        t_start = torch.tensor(t[:, :-1], dtype=ttype).reshape(-1, 1, 1)
+        t_end = torch.tensor(t[:, 1:], dtype=ttype).reshape(-1, 1, 1)
+        dt = dt * torch.ones_like(t_start, dtype=ttype)
         u = torch.zeros_like(x_start, dtype=ttype)
+        if true_derivatives:
+            dxdt = torch.tensor(
+                dxdt[:, :-1], dtype=ttype).reshape(-1, 1, nstates)
+        else:
+            dxdt = (x_end - x_start).clone().detach() / dt[0, 0]
+        xspatial = torch.tensor(np.repeat(xspatial.reshape(1, 1, -1), dxdt.shape[0], axis=0),
+                                dtype=ttype).reshape(dxdt.shape[0], 1, -1)
     else:
-        u = torch.tensor(u[:, :-1], dtype=ttype).reshape(-1, nstates)
-
-    if true_derivatives:
-        dxdt = torch.tensor(dxdt[:, :-1], dtype=ttype).reshape(-1, nstates)
-    else:
-        dxdt = (x_end - x_start).clone().detach() / dt[0, 0]
+        print('Unknown system')
+        return
 
     if nsamples is not None:
         x_start, x_end = x_start[:nsamples], x_end[:nsamples]
         t_start, t_end = t_start[:nsamples], t_end[:nsamples]
         dxdt = dxdt[:nsamples]
 
-    return (x_start, x_end, t_start, t_end, dt, u), dxdt
-
-
-def train(model, integrator, traindata, optimizer, valdata=None, epochs=1,
-          batch_size=1, shuffle=False, l1_param_forces=0.0,
-          l1_param_dissipation=0.0, loss_fn=torch.nn.MSELoss(),
-          batch_size_val=None, verbose=False, early_stopping_patience=None,
-          early_stopping_delta=0., return_best=False, store_best=False,
-          store_best_dir=None, modelname=None, trainingdetails={}):
+    if isinstance(pH_system, PseudoHamiltonianSystem):
+        return (x_start, x_end, t_start, t_end, dt, u), dxdt
+    elif isinstance(pH_system, ConservativeDissipativeSystem):
+        return (x_start, x_end, t_start, t_end, dt, u, xspatial), dxdt
+
+
+def train(
+    model,
+    integrator,
+    traindata,
+    optimizer=None,
+    valdata=None,
+    epochs=1,
+    batch_size=1,
+    shuffle=True,
+    l1_param_forces=0.0,
+    l1_param_dissipation=0.0,
+    loss_fn=torch.nn.MSELoss(),
+    batch_size_val=None,
+    verbose=True,
+    early_stopping_patience=None,
+    early_stopping_delta=0.0,
+    return_best=False,
+    store_best=False,
+    store_best_dir=None,
+    modelname=None,
+    trainingdetails={},
+):
     """
     Train a :py:meth:~`DynamicSystemNN`.
 
     Parameters
     ----------
     model : DynamicSystemNN
     integrator : str or False
@@ -170,101 +242,136 @@
 
     traindata_batched = batch_data(traindata, batch_size, shuffle)
     if batch_size_val is not None:
         valdata_batched = batch_data(traindata, batch_size, False)
     else:
         valdata_batched = None
 
+    if optimizer is None:
+        optimizer = torch.optim.Adam(
+            model.parameters(), lr=1e-3, weight_decay=1e-4)
+
     vloss = None
     vloss_best = np.inf
     newbest = True
     early_stopping = None
 
     if early_stopping_patience is not None:
-        early_stopping = EarlyStopping(patience=early_stopping_patience,
-                                       min_delta=early_stopping_delta)
+        early_stopping = EarlyStopping(
+            patience=early_stopping_patience, min_delta=early_stopping_delta
+        )
     if store_best:
         if store_best_dir is None:
-            store_best_dir = 'models/' + str(datetime.datetime.now()).replace(
-                '.', '').replace('-', '').replace(':', '').replace(' ', '')
+            store_best_dir = "models/" + str(datetime.datetime.now()).replace(
+                ".", ""
+            ).replace("-", "").replace(":", "").replace(" ", "")
         if not os.path.exists(store_best_dir):
             os.makedirs(store_best_dir)
         best_path = None
 
     best_model = model
     for epoch in range(epochs):
         if shuffle:
             traindata_batched = batch_data(traindata, batch_size, shuffle)
         model.train(True)
         start = datetime.datetime.now()
-        avg_loss = train_one_epoch(model, traindata_batched, loss_fn,
-                                   optimizer, integrator, l1_param_forces,
-                                   l1_param_dissipation)
+        avg_loss = train_one_epoch(
+            model,
+            traindata_batched,
+            loss_fn,
+            optimizer,
+            integrator,
+            l1_param_forces,
+            l1_param_dissipation,
+        )
         end = datetime.datetime.now()
         model.train(False)
 
         if verbose:
-            print(f'\nEpoch {epoch+1}')
-            print(f'Training loss: {np.format_float_scientific(avg_loss, 2)}')
-            delta = end - start
-            print('Epoch training time:'
-                  f' {delta.seconds:d}.{int(delta.microseconds / 1e4):d}'
-                  'seconds')
+            if epoch % 1 == 0:
+                print(f"\nEpoch {epoch+1}")
+                print(
+                    f"Training loss: {np.format_float_scientific(avg_loss, 2)}")
+                delta = end - start
+                print(
+                    "Epoch training time:"
+                    f" {delta.seconds:d}.{int(delta.microseconds / 1e4):d}"
+                    "seconds"
+                )
 
         if valdata is not None:
             start = datetime.datetime.now()
-            vloss = compute_validation_loss(model, integrator, valdata,
-                                            valdata_batched, loss_fn)
+            vloss = compute_validation_loss(
+                model, integrator, valdata, valdata_batched, loss_fn
+            )
             end = datetime.datetime.now()
             if verbose:
-                print('Validation loss: '
-                      f'{np.format_float_scientific(vloss, 2)}')
+                print(
+                    "Validation loss: " f"{np.format_float_scientific(vloss, 2)}")
                 delta = end - start
-                print('Validation loss computed in'
-                      f' {delta.seconds:d}.{int(delta.microseconds / 1e4):d}'
-                      'seconds')
+                print(
+                    "Validation loss computed in"
+                    f" {delta.seconds:d}.{int(delta.microseconds / 1e4):d}"
+                    "seconds"
+                )
             if vloss <= vloss_best:
                 newbest = True
                 if verbose:
-                    print('New best validation loss')
+                    print("New best validation loss")
                 vloss_best = vloss
                 if return_best:
                     best_model = copy.deepcopy(model)
 
             if early_stopping is not None:
                 if early_stopping(vloss):
                     if verbose:
-                        print(f'Early stopping at epoch {epoch+1}/{epochs}')
+                        print(f"Early stopping at epoch {epoch+1}/{epochs}")
                     break
         else:
             newbest = True
         if store_best and newbest:
             if best_path is not None:
-                os.remove(best_path)
+                try:
+                    os.remove(best_path)
+                except:
+                    print("The best model is gone.")
             if modelname is None:
                 best_path = os.path.join(
-                    store_best_dir, str(datetime.datetime.now()).replace(
-                        '.', '').replace('-', '').replace(':', '').replace(
-                        ' ', '') + '.model')
+                    store_best_dir,
+                    str(datetime.datetime.now())
+                    .replace(".", "")
+                    .replace("-", "")
+                    .replace(":", "")
+                    .replace(" ", "")
+                    + ".model",
+                )
             else:
                 best_path = os.path.join(store_best_dir, modelname)
-            trainingdetails['epochs'] = epoch+1
-            trainingdetails['val_loss'] = vloss
-            trainingdetails['train_loss'] = avg_loss
-            store_dynamic_system_model(best_path, model, optimizer,
-                                       **trainingdetails)
+            trainingdetails["epochs"] = epoch + 1
+            trainingdetails["val_loss"] = vloss
+            trainingdetails["train_loss"] = avg_loss
+            store_dynamic_system_model(
+                best_path, model, optimizer, **trainingdetails)
             if verbose:
-                print(f'Stored new best model {best_path}')
+                print(f"Stored new best model {best_path}")
             newbest = False
 
+    if isinstance(best_model, ConservativeDissipativeNN) and best_model.external_forces is not None:
+        best_model.dV_correction()
+        best_model.external_forces_correction()
+        if store_best:
+            store_dynamic_system_model(
+                best_path, best_model, optimizer, **trainingdetails)
+    
     return best_model, vloss
 
 
-def compute_validation_loss(model, integrator, valdata=None,
-                            valdata_batched=None, loss_fn=torch.nn.MSELoss()):
+def compute_validation_loss(
+    model, integrator, valdata=None, valdata_batched=None, loss_fn=torch.nn.MSELoss()
+):
     """
     Compute the validation loss of *model*.
 
     Parameters
     ----------
     model : DynamicSystemNN
     integrator : str or False
@@ -288,21 +395,31 @@
     -------
     vloss : float
 
     """
 
     vloss = 0
     if valdata_batched is not None:
-        for (input_tuple, dxdt) in valdata_batched:
-            dxdt_hat = model.time_derivative(integrator, *input_tuple)
-            vloss += loss_fn(dxdt_hat, dxdt)
+        for input_tuple, dxdt in valdata_batched:
+            if isinstance(model, ConservativeDissipativeNN):
+                lhs_hat = model.time_derivative(integrator, *input_tuple)
+                lhs = model.lhs(dxdt)
+                vloss += loss_fn(lhs_hat, lhs)
+            else:
+                dxdt_hat = model.time_derivative(integrator, *input_tuple)
+                vloss += loss_fn(dxdt_hat, dxdt)
         vloss = vloss / len(valdata_batched)
     else:
-        dxdt_hat = model.time_derivative(integrator, *valdata[0])
-        vloss = loss_fn(dxdt_hat, valdata[1])
+        if isinstance(model, ConservativeDissipativeNN):
+            lhs_hat = model.time_derivative(integrator, *valdata[0])
+            lhs = model.lhs(valdata[1])
+            vloss += loss_fn(lhs_hat, lhs)
+        else:
+            dxdt_hat = model.time_derivative(integrator, *valdata[0])
+            vloss = loss_fn(dxdt_hat, valdata[1])
     return float(vloss.detach().numpy())
 
 
 def batch_data(data, batch_size, shuffle):
     """
     Partition *data* into batches of *batch_size*.
 
@@ -321,25 +438,32 @@
 
     nsamples = data[1].shape[0]
     if shuffle:
         permutation = torch.randperm(nsamples)
     else:
         permutation = torch.arange(nsamples)
     nbatches = np.ceil(nsamples / batch_size).astype(int)
-    batched = [(None, None)]*nbatches
+    batched = [(None, None)] * nbatches
     for i in range(0, nbatches):
-        indices = permutation[i*batch_size:(i+1)*batch_size]
+        indices = permutation[i * batch_size: (i + 1) * batch_size]
         input_tuple = [data[0][j][indices] for j in range(len(data[0]))]
         dxdt = data[1][indices]
         batched[i] = (input_tuple, dxdt)
     return batched
 
 
-def train_one_epoch(model, traindata_batched, loss_fn, optimizer, integrator,
-                    l1_param_forces, l1_param_dissipation):
+def train_one_epoch(
+    model,
+    traindata_batched,
+    loss_fn,
+    optimizer,
+    integrator,
+    l1_param_forces,
+    l1_param_dissipation,
+):
     """
     Train *model* for one epoch.
 
     Parameters
     ----------
     model : DynamicSystemNN
     traindata_batched : list of tuples
@@ -358,35 +482,46 @@
 
     Returns
     -------
     training_loss : number
 
     """
 
-    running_loss = 0.
+    running_loss = 0.0
     optimizer.zero_grad()
-    for (input_tuple, dxdt) in traindata_batched:
+    for input_tuple, dxdt in traindata_batched:
         with torch.cuda.amp.autocast():
-            dxdt_hat = model.time_derivative(integrator, *input_tuple)
-            loss = loss_fn(dxdt_hat, dxdt)
-            if (isinstance(model, PseudoHamiltonianNN)
-                    and ((l1_param_forces > 0) or (l1_param_dissipation > 0))):
+            if isinstance(model, ConservativeDissipativeNN):
+                lhs_hat = model.time_derivative(integrator, *input_tuple)
+                lhs = model.lhs(dxdt)
+                loss = loss_fn(lhs_hat, lhs)
+            else:
+                dxdt_hat = model.time_derivative(integrator, *input_tuple)
+                loss = loss_fn(dxdt_hat, dxdt)
+            if (isinstance(model, PseudoHamiltonianNN) or
+                isinstance(model, ConservativeDissipativeNN)) and (
+                (l1_param_forces > 0) or (l1_param_dissipation > 0)
+            ):
                 loss += l1_loss_pHnn(
-                    model, l1_param_forces, l1_param_dissipation,
-                    input_tuple[0], input_tuple[2])
-
+                    model,
+                    l1_param_forces,
+                    l1_param_dissipation,
+                    input_tuple[0],
+                    input_tuple[2],
+                    input_tuple[6] if isinstance(model, ConservativeDissipativeNN) else None
+                )
         loss.backward()
         optimizer.step()
         optimizer.zero_grad()
         running_loss += loss.item()
 
     return running_loss / len(traindata_batched)
 
 
-def l1_loss_pHnn(pHnn_model, l1_param_forces, l1_param_dissipation, x, t=None):
+def l1_loss_pHnn(pHnn_model, l1_param_forces, l1_param_dissipation, x, t=None, xspatial=None):
     """
     Compute L1 penalty loss of external force and dissipation terms::
 
         L1 = l1_param_forces * | f(x, t) | + l1_param_dissipation * | R(x) |
 
     Parameters
     ----------
@@ -398,22 +533,44 @@
 
     Returns
     -------
     penalty : number
 
     """
     penalty = 0
-    if (isinstance(pHnn_model.external_forces, nn.Module) and (l1_param_forces > 0)
-            and (not pHnn_model.external_forces_provided)):
-        penalty += l1_param_forces*torch.abs(
-            pHnn_model.external_forces(x, t)).mean()
-    if (isinstance(pHnn_model.R, nn.Module) and (l1_param_dissipation > 0)
-            and (not pHnn_model.R_provided)):
-        penalty += l1_param_dissipation*torch.abs(pHnn_model.R(x)).mean()
-
+    if (
+        isinstance(pHnn_model.external_forces, nn.Module)
+        and (l1_param_forces > 0)
+        and (not pHnn_model.external_forces_provided)
+    ):
+        penalty += l1_param_forces * \
+            torch.abs(pHnn_model.external_forces(x, t)).mean()
+    if (
+        isinstance(pHnn_model, PseudoHamiltonianNN)
+        and isinstance(pHnn_model.R, nn.Module)
+        and (l1_param_dissipation > 0)
+        and (not pHnn_model.R_provided)
+    ):
+        penalty += l1_param_dissipation * torch.abs(pHnn_model.R(x)).mean()
+    if (
+        isinstance(pHnn_model, ConservativeDissipativeNN)
+        and (l1_param_forces > 0)
+        and (not pHnn_model.external_forces_provided)
+        and (pHnn_model.kernel_sizes[3] > 0)
+    ):
+        penalty += l1_param_forces * \
+            torch.abs(pHnn_model.external_forces(x, t, xspatial)-pHnn_model.external_forces(torch.zeros_like(x), t, xspatial)).mean()
+    if (
+        isinstance(pHnn_model, ConservativeDissipativeNN)
+        and (l1_param_dissipation > 0)
+        and ((pHnn_model.kernel_sizes[0] > 1) or (pHnn_model.kernel_sizes[2] > 1))
+    ):
+        penalty += l1_param_dissipation * \
+            (torch.abs(pHnn_model.D_flat().sum()-1.).mean()+torch.abs(pHnn_model.P().sum()-1.).mean())
+    
     return penalty
 
 
 def npoints_to_ntrajectories_tsample(npoints, tmax, dt):
     """
     Compute number of trajectories and the necessary sample time to
     achieve *npoints* samples from trajectories lasting *tmax* time with
@@ -430,31 +587,31 @@
     int
     (npoints, ) ndarray
 
     """
 
     points_per_trajectory = round(tmax / dt)
     t_sample = np.linspace(0, tmax, points_per_trajectory + 1)
-    return int(np.ceil(npoints / points_per_trajectory)), t_sample[:npoints+1]
+    return int(np.ceil(npoints / points_per_trajectory)), t_sample[: npoints + 1]
 
 
-class EarlyStopping():
+class EarlyStopping:
     """
     Keeps track of whether the validation loss has decreased by at least
     *min_delta* for the last *patience* calls.
 
     Parameters
     ----------
     patience : int, default None
         If None, patience is infinite
     min_delta : number, default 0.
 
     """
 
-    def __init__(self, patience=None, min_delta=0.):
+    def __init__(self, patience=None, min_delta=0.0):
         if patience is None:
             self.patience = np.inf
         else:
             self.patience = patience
         self.min_delta = min_delta
         self.counter = 0
         self.best_loss = np.inf
@@ -492,25 +649,28 @@
     """
     Loads a DynamicSystemNN from disk. See
     :py:meth:~`pseudo_hamiltonian_neural_network.load_phnn_model` and
     :py:meth:~`model.load_baseline_model`.
     """
 
     metadict = torch.load(modelpath)
-    if 'structure_matrix' in metadict.keys():
+    if 'dissipation_provided' in metadict.keys():
         return load_phnn_model(modelpath)
+    elif 'symmetric_matrix' in metadict.keys():  # fix
+        return load_cdnn_model(modelpath)
     else:
         return load_baseline_model(modelpath)
 
 
 def store_dynamic_system_model(storepath, model, optimizer, **kwargs):
     """
     Stores a DynamicSystemNN to disk. See
-    :py:meth:~`pseudo_hamiltonian_neural_network.store_phnn_model` and
+    :py:meth:~`port_hamiltonian_neural_network.store_phnn_model` and
     :py:meth:~`model.store_baseline_model`.
     """
 
     if isinstance(model, PseudoHamiltonianNN):
         store_phnn_model(storepath, model, optimizer, **kwargs)
+    elif isinstance(model, ConservativeDissipativeNN):
+        store_cdnn_model(storepath, model, optimizer, **kwargs)
     else:
         store_baseline_model(storepath, model, optimizer, **kwargs)
-
```

### Comparing `phlearn-1.0.0/phlearn/phsystems/msd_system.py` & `phlearn-1.1.0/phlearn/phsystems/msd_system.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.0.0/phlearn/phsystems/pseudo_Hamiltonian_system.py` & `phlearn-1.1.0/phlearn/phsystems/pseudo_Hamiltonian_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-
 import numpy as np
 from scipy.integrate import solve_ivp
 import torch
 
 from ..utils.derivatives import time_derivative
 
-__all__ = ['PseudoHamiltonianSystem', 'zero_force']
+__all__ = ["PseudoHamiltonianSystem", "zero_force"]
 
 
-class PseudoHamiltonianSystem():
+class PseudoHamiltonianSystem:
     """
     Implements a pseudo-Hamiltonian system of the form::
 
         dx/dt = (S(x) - R(x))*grad[H(x)] + F(x, t)
 
     where x is the system state, S is the skew-synnetric interconnection
     matrix, R is the positive semi-definite dissipation matrix, H is the
@@ -25,15 +24,15 @@
 
         structure_matrix : (N, N) ndarray or callable, default None
             Corresponds to the S matrix. Must either be an
             ndarray, or callable taking an ndarray
             input of shape (nsamples, nstates) and returning an ndarray
             of shape (nsamples, nstates, nstates). If None,
             the system is assumed to be canonical, and the
-            S matrix is set to be [[0, I_n], [-I_n, 0]].
+            S matrix is set to be [[0, I_N], [-I_N, 0]].
 
         dissipation_matrix : (N, N) ndarray or callable, default None
             Corresponds to the R matrix. Must either be an
             ndarray, or callable taking an ndarray input of shape
             (nsamples, nstates) and returning an ndarray of shape
             (nsamples, nstates, nstates). If None, the R matrix is set
             to be the zero matrix of shape (N, N).
@@ -53,15 +52,15 @@
             returning a torch tensor of shape (nsamples, nstates).
             If this is not provided, the hamiltonian must be provided.
 
         external_forces : callable, default None
             The external forces affecting system. Callable taking two
             ndarrays as input, x and t, of shape (nsamples, nstates),
             (nsamples, 1), respectively and returning an ndarray of
-            shape (nasamples, nstates).
+            shape (nsamples, nstates).
 
         controller : phlearn.control.PseudoHamiltonianController,
         default None
             Additional external forces set by a controller. Callable
             taking an ndarray x of shape (nstates,) and a scalar t as
             input and returning an ndarray of shape (nstates,). Note
             that this function should not take batch inputs, and that
@@ -75,26 +74,52 @@
             of shape (nstates,) with inital conditions for the system.
             This sampler is used when calling
             PseudoHamiltonianSystem.sample_trajectory if no initial
             condition is provided.
 
     """
 
-    def __init__(self, nstates, structure_matrix=None,
-                 dissipation_matrix=None, hamiltonian=None,
-                 grad_hamiltonian=None, external_forces=None,
-                 controller=None, init_sampler=None):
-
+    def __init__(
+        self,
+        nstates,
+        structure_matrix=None,
+        dissipation_matrix=None,
+        hamiltonian=None,
+        grad_hamiltonian=None,
+        external_forces=None,
+        controller=None,
+        init_sampler=None,
+    ):
         self.nstates = nstates
 
+        if (
+            structure_matrix is not None
+            and not callable(structure_matrix)
+            and not np.allclose(structure_matrix, -structure_matrix.T, atol=1e-15)
+        ):
+            raise Exception("structure_matrix must be skew-symmetric")
+
+        if hamiltonian is None and grad_hamiltonian is None:
+            raise Exception(
+                "Either one of hamiltonian or grad_hamiltonian must be provided"
+            )
+
         if structure_matrix is None:
+            if nstates % 2 == 1:
+                raise Exception(
+                    "nstates must be even when structure_matrix not provided"
+                )
+
             npos = nstates // 2
             structure_matrix = np.block(
-                [[np.zeros([npos, npos]), np.eye(npos)],
-                 [-np.eye(npos), np.zeros([npos, npos])]])
+                [
+                    [np.zeros([npos, npos]), np.eye(npos)],
+                    [-np.eye(npos), np.zeros([npos, npos])],
+                ]
+            )
 
         if not callable(structure_matrix):
             self.structure_matrix = structure_matrix
             self.S = lambda x: structure_matrix
         else:
             self.structure_matrix = None
             self.S = structure_matrix
@@ -160,22 +185,35 @@
         -------
         (..., N) ndarray
 
         """
 
         S = self.S(x)
         R = self.R(x)
-        dH = self.dH(x)
+        dH = self.dH(x.T).T
+        
         if (len(S.shape) == 3) or (len(R.shape) == 3):
-            dynamics = (np.matmul(S - R, np.atleast_3d(dH)).reshape(x.shape)
-                        + self.external_forces(x, t))
+            dynamics = np.matmul(S - R, np.atleast_3d(dH)).reshape(
+                x.shape
+            ) + self.external_forces(x, t)
         else:
-            dynamics = dH@(S.T - R.T) + self.external_forces(x, t)
+            def F(x, t):
+                """Temporary wrapper function for external force to allow user defined
+                force that takes x of shape (nstates, 1) and t as a float.
+                Putting this here as I don't know how this would affect the
+                above logical block. TODO this is creating a ragged array from
+                list of lists and needs fixed."""
+                return np.array([Fxy for Fxy in map(self.external_forces, x, t)])
+            
+            dynamics = dH @ (S.T - R.T) + F(x, t)
+            # dynamics = dH @ (S.T - R.T) + self.external_forces(x, t)
+            
         if u is not None:
             dynamics += u
+
         return dynamics
 
     def sample_trajectory(self, t, x0=None, noise_std=0, reference=None):
         """
         Samples a trajectory of the system at times *t*.
 
         Parameters
@@ -200,19 +238,21 @@
 
         """
 
         if x0 is None:
             x0 = self._initial_condition_sampler(self.rng)
 
         if self.controller is None:
-            x_dot = lambda t, x: self.x_dot(x.reshape(1, x.shape[-1]),
-                                            np.array(t).reshape((1, 1)))
-            out_ivp = solve_ivp(fun=x_dot, t_span=(t[0], t[-1]), y0=x0,
-                                t_eval=t, rtol=1e-10)
-            x, t = out_ivp['y'].T, out_ivp['t'].T
+            x_dot = lambda t, x: self.x_dot(
+                x.reshape(1, x.shape[-1]), np.array(t).reshape((1, 1))
+            )
+            out_ivp = solve_ivp(
+                fun=x_dot, t_span=(t[0], t[-1]), y0=x0, t_eval=t, rtol=1e-10
+            )
+            x, t = out_ivp["y"].T, out_ivp["t"].T
             dxdt = self.x_dot(x, t)
             us = None
         else:
             # Use RK4 integrator instead of solve_ivp when controller
             # is provided
             self.controller.reset()
             if reference is not None:
@@ -220,43 +260,52 @@
             x = np.zeros([t.shape[0], x0.shape[-1]])
             dxdt = np.zeros_like(x)
             us = np.zeros([t.shape[0] - 1, x0.shape[-1]])
             x[0, :] = x0
             for i, t_step in enumerate(t[:-1]):
                 dt = t[i + 1] - t[i]
                 us[i, :] = self.controller(x[i, :], t_step)
-                dxdt[i, :] = self.time_derivative('rk4', x[i:i+1, :],
-                                                  x[i:i+1, :],
-                                                  np.array([t_step]),
-                                                  np.array([t_step]),
-                                                  dt, u=us[i:i+1, :])
-                x[i + 1, :] = x[i, :] + dt*dxdt[i, :]
+                dxdt[i, :] = self.time_derivative(
+                    "rk4",
+                    x[i : i + 1, :],
+                    x[i : i + 1, :],
+                    np.array([t_step]),
+                    np.array([t_step]),
+                    dt,
+                    u=us[i : i + 1, :],
+                )
+                x[i + 1, :] = x[i, :] + dt * dxdt[i, :]
 
         # Add noise:
-        x += self.rng.normal(size=x.shape)*noise_std
-        dxdt += self.rng.normal(size=dxdt.shape)*noise_std
+        x += self.rng.normal(size=x.shape) * noise_std
+        dxdt += self.rng.normal(size=dxdt.shape) * noise_std
 
         return x, dxdt, t, us
 
     def set_controller(self, controller):
         """
         Set system controller.
         """
         self.controller = controller
 
     def _dH(self, x):
         x = torch.tensor(x, requires_grad=True)
-        return torch.autograd.grad(self.H(x).sum(), x, retain_graph=False,
-                                   create_graph=False)[0].detach().numpy()
+        return (
+            torch.autograd.grad(
+                self.H(x).sum(), x, retain_graph=False, create_graph=False
+            )[0]
+            .detach()
+            .numpy()
+        )
 
     def _initial_condition_sampler(self, rng=None):
         if rng is None:
             assert self.rng is not None
             rng = self.rng
-        return rng.uniform(low=-1., high=1.0, size=self.nstates)
+        return rng.uniform(low=-1.0, high=1.0, size=self.nstates)
 
 
 def zero_force(x, t=None):
     """
     A force term that is always zero.
 
     Parameters
```

### Comparing `phlearn-1.0.0/phlearn/phsystems/tank_system.py` & `phlearn-1.1.0/phlearn/phsystems/tank_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,18 +113,20 @@
 
         if isinstance(J, numbers.Number):
             J = J*np.ones(self.npipes)
         if isinstance(A, numbers.Number):
             A = A*np.ones(self.ntanks)
 
         self.Hvec = np.concatenate((1/J, rho*g / A))
-        super().__init__(nstates, structure_matrix=structure_matrix,
-                         dissipation_matrix=dissipation, **kwargs)
-        self.H = self.H_tanksystem
-        self.dH = self.dH_tanksystem
+        super().__init__(nstates,
+                         hamiltonian=self.H_tanksystem,
+                         grad_hamiltonian=self.dH_tanksystem,
+                         structure_matrix=structure_matrix,
+                         dissipation_matrix=dissipation,
+                         **kwargs)
 
     def H_tanksystem(self, x, t=None):
         return x**2 @ self.Hvec / 2
 
     def dH_tanksystem(self, x, t=None):
         return x * self.Hvec
```

### Comparing `phlearn-1.0.0/phlearn.egg-info/PKG-INFO` & `phlearn-1.1.0/phlearn.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: phlearn
-Version: 1.0.0
+Version: 1.1.0
 Summary: A package for simulating and learning pseudo-Hamiltonian systems. For further details, see https://arxiv.org/pdf/2206.02660.pdf
 Home-page: https://gitlab.sintef.no/hybrid-machine-learning/pseudo-Hamiltonian-neural-networks
 Author: Sølve Eidnes
 Author-email: solve.eidnes@sintef.no
 License: MIT
 Keywords: pseudo-Hamiltonian neural networks
 Classifier: Development Status :: 5 - Production/Stable
+Provides-Extra: control
 License-File: LICENSE.txt
 
 # phlearn
 Package for modelling pseudo-Hamiltonian systems with neural networks as described in [(Eidnes et al. 2022)](https://arxiv.org/pdf/2206.02660.pdf).
 
 [Documentation available here](https://pseudo-Hamiltonian-neural-networks.readthedocs.io/en/latest/)
```

### Comparing `phlearn-1.0.0/setup.py` & `phlearn-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,31 +4,35 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setuptools.setup(
     name='phlearn',
-    version='1.0.0',
+    version='1.1.0',
     author='Sølve Eidnes',
     author_email='solve.eidnes@sintef.no',
     description=('A package for simulating and learning pseudo-Hamiltonian systems.'
                  ' For further details, see https://arxiv.org/pdf/2206.02660.pdf'),
     keywords='pseudo-Hamiltonian neural networks',
     url="https://gitlab.sintef.no/hybrid-machine-learning/pseudo-Hamiltonian-neural-networks",
     packages=setuptools.find_packages(),
     long_description=read('README.md'),
     classifiers=[
         'Development Status :: 5 - Production/Stable'
     ],
     license='MIT',
     install_requires=[
-        'networkx',
-        'numpy',
+        'networkx==2.7.1',
+        'numpy==1.22.3',
+        'torchvision==0.11.3',
+        'scipy==1.8.0',
         'torch',
         'torchaudio',
-        'torchvision',
-        'scipy',
-        'casadi',
-        'do_mpc'
+        'matplotlib',
+        'imageio',
+        'tqdm',
+        'autograd',
+        'IPython',
     ],
+    extras_require={'control': ['casadi', 'do_mpc']},
 )
```


# Comparing `tmp/cssfinder_backend_numpy-0.3.0.tar.gz` & `tmp/cssfinder_backend_numpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cssfinder_backend_numpy-0.3.0.tar", max compression
+gzip compressed data, was "cssfinder_backend_numpy-0.4.0.tar", max compression
```

## Comparing `cssfinder_backend_numpy-0.3.0.tar` & `cssfinder_backend_numpy-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,22 @@
--rw-r--r--   0        0        0     6342 2023-03-21 21:41:00.278146 cssfinder_backend_numpy-0.3.0/README.md
--rw-r--r--   0        0        0     1104 2023-03-21 21:41:00.278146 cssfinder_backend_numpy-0.3.0/build.py
--rw-r--r--   0        0        0     2557 2023-03-21 21:41:00.278146 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/__init__.py
--rw-r--r--   0        0        0     1241 2023-03-21 21:41:00.278146 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/_cython/__init__.py
--rw-r--r--   0        0        0   602260 2023-03-21 21:41:00.278146 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/_cython/_complex128.cpp
--rw-r--r--   0        0        0    13410 2023-03-21 21:41:00.278146 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/_cython/_complex128.py
--rw-r--r--   0        0        0   604739 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/_cython/_complex64.cpp
--rw-r--r--   0        0        0    13450 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/_cython/_complex64.py
--rw-r--r--   0        0        0    10137 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/base.py
--rw-r--r--   0        0        0     3517 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/complex128.py
--rw-r--r--   0        0        0     3482 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/complex64.py
--rw-r--r--   0        0        0     1241 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/cython/__init__.py
--rw-r--r--   0        0        0     8266 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/impl.py
--rw-r--r--   0        0        0     1241 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy/__init__.py
--rw-r--r--   0        0        0    13410 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy/_complex128.py
--rw-r--r--   0        0        0    13450 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy/_complex64.py
--rw-r--r--   0        0        0     1241 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_debug/__init__.py
--rw-r--r--   0        0        0    17006 2023-03-21 21:41:00.282147 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_debug/_complex128.py
--rw-r--r--   0        0        0    16982 2023-03-21 21:41:00.286146 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_debug/_complex64.py
--rw-r--r--   0        0        0     1241 2023-03-21 21:41:00.286146 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_jit/__init__.py
--rw-r--r--   0        0        0    14320 2023-03-21 21:41:00.286146 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_jit/_complex128.py
--rw-r--r--   0        0        0    14360 2023-03-21 21:41:00.286146 cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_jit/_complex64.py
--rw-r--r--   0        0        0    16952 2023-03-21 21:41:00.286146 cssfinder_backend_numpy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7171 1970-01-01 00:00:00.000000 cssfinder_backend_numpy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6342 2023-04-27 17:47:58.937753 cssfinder_backend_numpy-0.4.0/README.md
+-rw-r--r--   0        0        0     1104 2023-04-27 17:47:58.937753 cssfinder_backend_numpy-0.4.0/build.py
+-rw-r--r--   0        0        0     2557 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/__init__.py
+-rw-r--r--   0        0        0     1241 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/__init__.py
+-rw-r--r--   0        0        0    13392 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/_complex128.py
+-rw-r--r--   0        0        0    13432 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/_complex64.py
+-rw-r--r--   0        0        0    11378 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/base.py
+-rw-r--r--   0        0        0     3534 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/complex128.py
+-rw-r--r--   0        0        0     3499 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/complex64.py
+-rw-r--r--   0        0        0     1241 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/cython/__init__.py
+-rw-r--r--   0        0        0     8266 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/impl.py
+-rw-r--r--   0        0        0     1241 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/__init__.py
+-rw-r--r--   0        0        0    13392 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/_complex128.py
+-rw-r--r--   0        0        0    13432 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/_complex64.py
+-rw-r--r--   0        0        0     1241 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/__init__.py
+-rw-r--r--   0        0        0    16988 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/_complex128.py
+-rw-r--r--   0        0        0    16964 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/_complex64.py
+-rw-r--r--   0        0        0     1241 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/__init__.py
+-rw-r--r--   0        0        0    14359 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/_complex128.py
+-rw-r--r--   0        0        0    14399 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/_complex64.py
+-rw-r--r--   0        0        0    16962 2023-04-27 17:47:58.945753 cssfinder_backend_numpy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7171 1970-01-01 00:00:00.000000 cssfinder_backend_numpy-0.4.0/PKG-INFO
```

### Comparing `cssfinder_backend_numpy-0.3.0/README.md` & `cssfinder_backend_numpy-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,36 +67,36 @@
 
 ```
 poe build
 ```
 
 ![poe_build](https://user-images.githubusercontent.com/56170852/223251363-61fc4d00-68ad-429c-9fbb-8ab7f4712451.png)
 
-This will create `dist/` directory with `cssfinder_backend_numpy-0.3.0` or
+This will create `dist/` directory with `cssfinder_backend_numpy-0.4.0` or
 alike inside.
 
 Wheel file can be installed with
 
 ```
-pip install ./dist/cssfinder_backend_numpy-0.3.0
+pip install ./dist/cssfinder_backend_numpy-0.4.0
 ```
 
 What you expect is
 
 ```
-Successfully installed cssfinder_backend_numpy-0.3.0
+Successfully installed cssfinder_backend_numpy-0.4.0
 ```
 
 or rather something like
 
 ```
-Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder_backend_numpy-0.3.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
+Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder_backend_numpy-0.4.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
 ```
 
-But `cssfinder_backend_numpy-0.3.0` should be included in this list.
+But `cssfinder_backend_numpy-0.4.0` should be included in this list.
 
 ## Code quality
 
 To ensure that all code follow same style guidelines and code quality rules,
 multiple static analysis tools are used. For simplicity, all of them are
 configured as `pre-commit` ([learn about pre-commit](https://pre-commit.com/))
 hooks. Most of them however are listed as development dependencies.
```

### Comparing `cssfinder_backend_numpy-0.3.0/build.py` & `cssfinder_backend_numpy-0.4.0/build.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/__init__.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from cssfinder_backend_numpy.complex64 import NumPyC64, NumPyC64Debug, NumPyC64Jit
 from cssfinder_backend_numpy.complex128 import HAS_CYTHON as HAS_CYTHON_128
 from cssfinder_backend_numpy.complex128 import NumPyC128, NumPyC128Debug, NumPyC128Jit
 
 if TYPE_CHECKING:
     from cssfinder.algorithm.backend import BackendBase
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 
 def export_backend() -> dict[tuple[str, Precision], BackendBase]:
     """Export mapping of available backends in this package."""
     backends = {
         ("numpy_jit", Precision.SINGLE): NumPyC64Jit,
         ("numpy_jit", Precision.DOUBLE): NumPyC128Jit,
```

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/_cython/__init__.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/_cython/_complex128.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/_complex128.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,16 @@
 
     rho2a = np.dot(unitary, rho2a)  # matmul replaced with dot
 
     return rho2a  # type: ignore[no-any-return]
 
 
 def apply_symmetries(
-    rho: npt.NDArray[np.complex128], symmetries: list[list[npt.NDArray[np.complex128]]]
+    rho: npt.NDArray[np.complex128],
+    symmetries: list[list[npt.NDArray[np.complex128]]],
 ) -> npt.NDArray[np.complex128]:
     """Apply symmetries to density matrix.
 
     Parameters
     ----------
     rho : npt.NDArray[np.complex128]
         Density matrix to which we want to apply symmetries.
@@ -200,16 +201,16 @@
 
         product_rot2_3 = product(rotated_2, visibility_state)
 
         if product_2_3 > product_rot2_3:
             unitary = unitary.conj().T
             rotated_2 = rotate(new_state, unitary)
 
-        while (new_product_2_3 := product_rot2_3) > product_2_3:
-            product_2_3 = new_product_2_3
+        while product_rot2_3 > product_2_3:
+            product_2_3 = product_rot2_3
             rotated_2 = rotate(rotated_2, unitary)
 
             product_rot2_3 = product(rotated_2, visibility_state)
 
     return rotated_2.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
 
 
@@ -237,15 +238,15 @@
 
 
 def random_d_fs(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Random n quDit state."""
     rand_vectors = get_random_haar_2d(depth, quantity)
     vector = normalize(rand_vectors[0])
 
-    for i in range(quantity - 1):
+    for i in range(1, quantity):
         idx_vector = normalize(rand_vectors[i])
 
         vector = np.outer(vector, idx_vector).flatten()
 
     vector = project(vector)
 
     return vector  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/_cython/_complex64.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/_complex64.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,16 @@
 
     rho2a = np.dot(unitary, rho2a)  # matmul replaced with dot
 
     return rho2a  # type: ignore[no-any-return]
 
 
 def apply_symmetries(
-    rho: npt.NDArray[np.complex64], symmetries: list[list[npt.NDArray[np.complex64]]]
+    rho: npt.NDArray[np.complex64],
+    symmetries: list[list[npt.NDArray[np.complex64]]],
 ) -> npt.NDArray[np.complex64]:
     """Apply symmetries to density matrix.
 
     Parameters
     ----------
     rho : npt.NDArray[np.complex64]
         Density matrix to which we want to apply symmetries.
@@ -204,16 +205,16 @@
 
         product_rot2_3 = product(rotated_2, visibility_state)
 
         if product_2_3 > product_rot2_3:
             unitary = unitary.conj().T
             rotated_2 = rotate(new_state, unitary)
 
-        while (new_product_2_3 := product_rot2_3) > product_2_3:
-            product_2_3 = new_product_2_3
+        while product_rot2_3 > product_2_3:
+            product_2_3 = product_rot2_3
             rotated_2 = rotate(rotated_2, unitary)
 
             product_rot2_3 = product(rotated_2, visibility_state)
 
     return rotated_2.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
 
 
@@ -241,15 +242,15 @@
 
 
 def random_d_fs(depth: int, quantity: int) -> npt.NDArray[np.complex64]:
     """Random n quDit state."""
     rand_vectors = get_random_haar_2d(depth, quantity)
     vector = normalize(rand_vectors[0])
 
-    for i in range(quantity - 1):
+    for i in range(1, quantity):
         idx_vector = normalize(rand_vectors[i])
 
         vector = np.outer(vector, idx_vector).flatten()
 
     vector = project(vector)
 
     return vector  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/base.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from types import MethodType
 from typing import TYPE_CHECKING, Callable, Generic, Optional, TypeVar, cast
 
 import numpy as np
 import numpy.typing as npt
 from cssfinder.algorithm.backend.base import BackendBase
 from cssfinder.cssfproject import AlgoMode
-from numba import jit
+from numba import jit, typed  # type: ignore[attr-defined]
 
 if TYPE_CHECKING:
     from cssfinder.algorithm.backend.numpy.impl import Implementation
 
 PRIMARY = TypeVar("PRIMARY", np.complex128, np.complex64)
 SECONDARY_co = TypeVar("SECONDARY_co", np.float64, np.float32, covariant=True)
 
@@ -101,17 +101,14 @@
         )
 
         if self.mode == AlgoMode.FSnQd:
             self.optimize_callback = self.impl.optimize_d_fs
         elif self.mode == AlgoMode.SBiPa:
             self.optimize_callback = self.impl.optimize_bs
 
-        if not self.is_debug:
-            self.jit()
-
     def _create_visibility_matrix(self) -> npt.NDArray[PRIMARY]:
         vis_state = self.visibility * self.initial
         inv_vis_ident = (1 - self.visibility) * np.identity(
             len(self.initial),
             dtype=np.complex128,
         )
         return (  # type: ignore[no-any-return]
@@ -171,32 +168,14 @@
         """Return list of all corrections found during optimization."""
         return self._corrections.copy()
 
     def get_corrections_count(self) -> int:
         """Return number of all corrections found during optimization."""
         return len(self._corrections)
 
-    def jit(self) -> None:
-        """JIT compile performance critical parts of backend with numba."""
-        _update_state = jit(  # type: ignore[assignment]
-            forceobj=True,
-            cache=True,
-            looplift=False,
-        )(
-            self.__class__._update_state,  # noqa: SLF001
-        )
-
-        self._update_state = MethodType(_update_state, self)  # type: ignore[assignment]
-
-        run_epoch = jit(forceobj=True, cache=True, looplift=False)(
-            self.__class__.run_epoch,
-        )
-
-        self.run_epoch = MethodType(run_epoch, self)  # type: ignore[assignment]
-
     def run_epoch(self, iterations: int, epoch_index: int) -> None:
         """Run sequence of iterations without stopping to check any stop conditions."""
         depth = self.depth
         quantity = self.quantity
         epochs = 20 * depth * depth * quantity
 
         for iteration_index in range(iterations):
@@ -273,7 +252,66 @@
                         self.impl.product(
                             self._visibility_reduced,
                             self._visibility_reduced,
                         ),
                     ),
                 ),
             )
+
+
+class NumPyJitBase(NumPyBase[PRIMARY, SECONDARY_co]):
+    """Base class for JIT compiled numpy backends."""
+
+    def __init__(  # noqa: PLR0913
+        self,
+        initial: npt.NDArray[np.complex128],
+        depth: int,
+        quantity: int,
+        mode: AlgoMode,
+        visibility: float,
+        *,
+        is_debug: bool = False,
+    ) -> None:
+        super().__init__(initial, depth, quantity, mode, visibility, is_debug=is_debug)
+        if not self.is_debug:
+            self.jit()
+
+    def set_symmetries(
+        self, symmetries: list[list[npt.NDArray[np.complex128]]]
+    ) -> None:
+        """Set symmetries to use during calculations.
+
+        This operation may involve type conversion and copying of symmetries, therefore
+        if may be slow and should should be done only once.
+
+        Parameters
+        ----------
+        symmetries : list[list[npt.NDArray[np.complex64]]]
+            Array of symmetries.
+
+        """
+        self._symmetries = typed.List(
+            typed.List(cell.astype(self.primary_t) for cell in row)
+            for row in symmetries
+        )
+        if self._symmetries:
+            self._intermediate = self.impl.apply_symmetries(
+                self._intermediate, self._symmetries
+            )
+
+    def jit(self) -> None:
+        """JIT compile performance critical parts of backend with numba."""
+        _update_state = jit(  # type: ignore[assignment]
+            forceobj=True,
+            cache=True,
+            looplift=False,
+        )(
+            self.__class__._update_state,  # noqa: SLF001
+        )
+
+        self._update_state = MethodType(_update_state, self)  # type: ignore[assignment]
+
+        run_epoch = jit(forceobj=True, cache=True, looplift=False)(
+            self.__class__.run_epoch,
+        )
+
+        self.run_epoch = MethodType(run_epoch, self)  # type: ignore[assignment]
```

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/complex128.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/complex128.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from __future__ import annotations
 
 import logging
 from typing import cast
 
 import numpy as np
 
-from cssfinder_backend_numpy.base import NumPyBase
+from cssfinder_backend_numpy.base import NumPyBase, NumPyJitBase
 from cssfinder_backend_numpy.impl import Implementation
 from cssfinder_backend_numpy.numpy import _complex128
 from cssfinder_backend_numpy.numpy_debug import _complex128 as _complex128_debug
 from cssfinder_backend_numpy.numpy_jit import _complex128 as _complex128_jit
 
 try:
     from cssfinder_backend_numpy.cython import (  # type: ignore[attr-defined] # noqa: E501 I001 RUF100
@@ -53,15 +53,15 @@
         Implementation[np.complex128, np.float64],
         _complex128,
     )
     primary_t: type[np.complex128] = np.complex128
     secondary_t: type[np.float64] = np.float64
 
 
-class NumPyC128Jit(NumPyBase[np.complex128, np.float64]):
+class NumPyC128Jit(NumPyJitBase[np.complex128, np.float64]):
     """Concrete numpy based backend for Gilbert algorithm using complex128 type."""
 
     impl: Implementation[np.complex128, np.float64] = cast(
         Implementation[np.complex128, np.float64],
         _complex128_jit,
     )
     primary_t: type[np.complex128] = np.complex128
```

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/complex64.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/complex64.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from __future__ import annotations
 
 import logging
 from typing import cast
 
 import numpy as np
 
-from cssfinder_backend_numpy.base import NumPyBase
+from cssfinder_backend_numpy.base import NumPyBase, NumPyJitBase
 from cssfinder_backend_numpy.impl import Implementation
 from cssfinder_backend_numpy.numpy import _complex64
 from cssfinder_backend_numpy.numpy_debug import _complex64 as _complex64_debug
 from cssfinder_backend_numpy.numpy_jit import _complex64 as _complex64_jit
 
 try:
     from cssfinder_backend_numpy.cython import (  # type: ignore[attr-defined] # noqa: E501 I001 RUF100
@@ -53,15 +53,15 @@
         Implementation[np.complex64, np.float32],
         _complex64,
     )
     primary_t: type[np.complex64] = np.complex64
     secondary_t: type[np.float32] = np.float32
 
 
-class NumPyC64Jit(NumPyBase[np.complex64, np.float32]):
+class NumPyC64Jit(NumPyJitBase[np.complex64, np.float32]):
     """Concrete numpy based backend for Gilbert algorithm using complex128 type."""
 
     impl: Implementation[np.complex64, np.float32] = cast(
         Implementation[np.complex64, np.float32],
         _complex64_jit,
     )
     primary_t: type[np.complex64] = np.complex64
```

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/cython/__init__.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/cython/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/impl.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/impl.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy/__init__.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy/_complex128.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/_complex128.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,16 @@
 
     rho2a = np.dot(unitary, rho2a)  # matmul replaced with dot
 
     return rho2a  # type: ignore[no-any-return]
 
 
 def apply_symmetries(
-    rho: npt.NDArray[np.complex128], symmetries: list[list[npt.NDArray[np.complex128]]]
+    rho: npt.NDArray[np.complex128],
+    symmetries: list[list[npt.NDArray[np.complex128]]],
 ) -> npt.NDArray[np.complex128]:
     """Apply symmetries to density matrix.
 
     Parameters
     ----------
     rho : npt.NDArray[np.complex128]
         Density matrix to which we want to apply symmetries.
@@ -200,16 +201,16 @@
 
         product_rot2_3 = product(rotated_2, visibility_state)
 
         if product_2_3 > product_rot2_3:
             unitary = unitary.conj().T
             rotated_2 = rotate(new_state, unitary)
 
-        while (new_product_2_3 := product_rot2_3) > product_2_3:
-            product_2_3 = new_product_2_3
+        while product_rot2_3 > product_2_3:
+            product_2_3 = product_rot2_3
             rotated_2 = rotate(rotated_2, unitary)
 
             product_rot2_3 = product(rotated_2, visibility_state)
 
     return rotated_2.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
 
 
@@ -237,15 +238,15 @@
 
 
 def random_d_fs(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Random n quDit state."""
     rand_vectors = get_random_haar_2d(depth, quantity)
     vector = normalize(rand_vectors[0])
 
-    for i in range(quantity - 1):
+    for i in range(1, quantity):
         idx_vector = normalize(rand_vectors[i])
 
         vector = np.outer(vector, idx_vector).flatten()
 
     vector = project(vector)
 
     return vector  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy/_complex64.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/_complex64.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,16 @@
 
     rho2a = np.dot(unitary, rho2a)  # matmul replaced with dot
 
     return rho2a  # type: ignore[no-any-return]
 
 
 def apply_symmetries(
-    rho: npt.NDArray[np.complex64], symmetries: list[list[npt.NDArray[np.complex64]]]
+    rho: npt.NDArray[np.complex64],
+    symmetries: list[list[npt.NDArray[np.complex64]]],
 ) -> npt.NDArray[np.complex64]:
     """Apply symmetries to density matrix.
 
     Parameters
     ----------
     rho : npt.NDArray[np.complex64]
         Density matrix to which we want to apply symmetries.
@@ -204,16 +205,16 @@
 
         product_rot2_3 = product(rotated_2, visibility_state)
 
         if product_2_3 > product_rot2_3:
             unitary = unitary.conj().T
             rotated_2 = rotate(new_state, unitary)
 
-        while (new_product_2_3 := product_rot2_3) > product_2_3:
-            product_2_3 = new_product_2_3
+        while product_rot2_3 > product_2_3:
+            product_2_3 = product_rot2_3
             rotated_2 = rotate(rotated_2, unitary)
 
             product_rot2_3 = product(rotated_2, visibility_state)
 
     return rotated_2.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
 
 
@@ -241,15 +242,15 @@
 
 
 def random_d_fs(depth: int, quantity: int) -> npt.NDArray[np.complex64]:
     """Random n quDit state."""
     rand_vectors = get_random_haar_2d(depth, quantity)
     vector = normalize(rand_vectors[0])
 
-    for i in range(quantity - 1):
+    for i in range(1, quantity):
         idx_vector = normalize(rand_vectors[i])
 
         vector = np.outer(vector, idx_vector).flatten()
 
     vector = project(vector)
 
     return vector  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_debug/__init__.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_debug/_complex128.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/_complex128.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,16 @@
     rho2a = np.dot(unitary, rho2a)  # matmul replaced with dot
     assert_dtype(rho2a, np.complex128)
 
     return rho2a  # type: ignore[no-any-return]
 
 
 def apply_symmetries(
-    rho: npt.NDArray[np.complex128], symmetries: list[list[npt.NDArray[np.complex128]]]
+    rho: npt.NDArray[np.complex128],
+    symmetries: list[list[npt.NDArray[np.complex128]]],
 ) -> npt.NDArray[np.complex128]:
     """Apply symmetries to density matrix.
 
     Parameters
     ----------
     rho : npt.NDArray[np.complex128]
         Density matrix to which we want to apply symmetries.
@@ -254,16 +255,16 @@
         product_rot2_3 = product(rotated_2, visibility_state)
 
         if product_2_3 > product_rot2_3:
             unitary = unitary.conj().T
             rotated_2 = rotate(new_state, unitary)
             assert_dtype(rotated_2, np.complex128)
 
-        while (new_product_2_3 := product_rot2_3) > product_2_3:
-            product_2_3 = new_product_2_3
+        while product_rot2_3 > product_2_3:
+            product_2_3 = product_rot2_3
             rotated_2 = rotate(rotated_2, unitary)
             assert_dtype(rotated_2, np.complex128)
 
             product_rot2_3 = product(rotated_2, visibility_state)
 
     return rotated_2.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
 
@@ -298,15 +299,15 @@
 
 def random_d_fs(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Random n quDit state."""
     rand_vectors = get_random_haar_2d(depth, quantity)
     vector = normalize(rand_vectors[0])
     assert_dtype(vector, np.complex128)
 
-    for i in range(quantity - 1):
+    for i in range(1, quantity):
         idx_vector = normalize(rand_vectors[i])
         assert_dtype(idx_vector, np.complex128)
 
         vector = np.outer(vector, idx_vector).flatten()
         assert_dtype(vector, np.complex128)
 
     vector = project(vector)
```

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_debug/_complex64.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/_complex64.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,16 @@
     rho2a = np.dot(unitary, rho2a)  # matmul replaced with dot
     assert_dtype(rho2a, np.complex64)
 
     return rho2a  # type: ignore[no-any-return]
 
 
 def apply_symmetries(
-    rho: npt.NDArray[np.complex64], symmetries: list[list[npt.NDArray[np.complex64]]]
+    rho: npt.NDArray[np.complex64],
+    symmetries: list[list[npt.NDArray[np.complex64]]],
 ) -> npt.NDArray[np.complex64]:
     """Apply symmetries to density matrix.
 
     Parameters
     ----------
     rho : npt.NDArray[np.complex64]
         Density matrix to which we want to apply symmetries.
@@ -258,16 +259,16 @@
         product_rot2_3 = product(rotated_2, visibility_state)
 
         if product_2_3 > product_rot2_3:
             unitary = unitary.conj().T
             rotated_2 = rotate(new_state, unitary)
             assert_dtype(rotated_2, np.complex64)
 
-        while (new_product_2_3 := product_rot2_3) > product_2_3:
-            product_2_3 = new_product_2_3
+        while product_rot2_3 > product_2_3:
+            product_2_3 = product_rot2_3
             rotated_2 = rotate(rotated_2, unitary)
             assert_dtype(rotated_2, np.complex64)
 
             product_rot2_3 = product(rotated_2, visibility_state)
 
     return rotated_2.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
 
@@ -302,15 +303,15 @@
 
 def random_d_fs(depth: int, quantity: int) -> npt.NDArray[np.complex64]:
     """Random n quDit state."""
     rand_vectors = get_random_haar_2d(depth, quantity)
     vector = normalize(rand_vectors[0])
     assert_dtype(vector, np.complex64)
 
-    for i in range(quantity - 1):
+    for i in range(1, quantity):
         idx_vector = normalize(rand_vectors[i])
         assert_dtype(idx_vector, np.complex64)
 
         vector = np.outer(vector, idx_vector).flatten()
         assert_dtype(vector, np.complex64)
 
     vector = project(vector)
```

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_jit/__init__.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_jit/_complex128.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/_complex128.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
-from numba import jit
+from numba import jit, types  # type: ignore[attr-defined]
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
 
 #    █████  ██████  ███    ███ ███    ███  ██████  ███    ██
 #   ██     ██    ██ ████  ████ ████  ████ ██    ██ ████   ██
@@ -141,15 +141,16 @@
     rho2a = np.dot(unitary, rho2a)  # matmul replaced with dot
 
     return rho2a  # type: ignore[no-any-return]
 
 
 @jit(nopython=True, nogil=True, cache=True)
 def apply_symmetries(
-    rho: npt.NDArray[np.complex128], symmetries: list[list[npt.NDArray[np.complex128]]]
+    rho: npt.NDArray[np.complex128],
+    symmetries: types.ListType[types.ListType[npt.NDArray[np.complex128]]],
 ) -> npt.NDArray[np.complex128]:
     """Apply symmetries to density matrix.
 
     Parameters
     ----------
     rho : npt.NDArray[np.complex128]
         Density matrix to which we want to apply symmetries.
@@ -210,16 +211,16 @@
 
         product_rot2_3 = product(rotated_2, visibility_state)
 
         if product_2_3 > product_rot2_3:
             unitary = unitary.conj().T
             rotated_2 = rotate(new_state, unitary)
 
-        while (new_product_2_3 := product_rot2_3) > product_2_3:
-            product_2_3 = new_product_2_3
+        while product_rot2_3 > product_2_3:
+            product_2_3 = product_rot2_3
             rotated_2 = rotate(rotated_2, unitary)
 
             product_rot2_3 = product(rotated_2, visibility_state)
 
     return rotated_2.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
 
 
@@ -250,15 +251,15 @@
 
 @jit(nopython=True, nogil=True, cache=True)
 def random_d_fs(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Random n quDit state."""
     rand_vectors = get_random_haar_2d(depth, quantity)
     vector = normalize(rand_vectors[0])
 
-    for i in range(quantity - 1):
+    for i in range(1, quantity):
         idx_vector = normalize(rand_vectors[i])
 
         vector = np.outer(vector, idx_vector).flatten()
 
     vector = project(vector)
 
     return vector  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.3.0/cssfinder_backend_numpy/numpy_jit/_complex64.py` & `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/_complex64.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
-from numba import jit
+from numba import jit, types  # type: ignore[attr-defined]
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
 
 #    █████  ██████  ███    ███ ███    ███  ██████  ███    ██
 #   ██     ██    ██ ████  ████ ████  ████ ██    ██ ████   ██
@@ -145,15 +145,16 @@
     rho2a = np.dot(unitary, rho2a)  # matmul replaced with dot
 
     return rho2a  # type: ignore[no-any-return]
 
 
 @jit(nopython=True, nogil=True, cache=True)
 def apply_symmetries(
-    rho: npt.NDArray[np.complex64], symmetries: list[list[npt.NDArray[np.complex64]]]
+    rho: npt.NDArray[np.complex64],
+    symmetries: types.ListType[types.ListType[npt.NDArray[np.complex64]]],
 ) -> npt.NDArray[np.complex64]:
     """Apply symmetries to density matrix.
 
     Parameters
     ----------
     rho : npt.NDArray[np.complex64]
         Density matrix to which we want to apply symmetries.
@@ -214,16 +215,16 @@
 
         product_rot2_3 = product(rotated_2, visibility_state)
 
         if product_2_3 > product_rot2_3:
             unitary = unitary.conj().T
             rotated_2 = rotate(new_state, unitary)
 
-        while (new_product_2_3 := product_rot2_3) > product_2_3:
-            product_2_3 = new_product_2_3
+        while product_rot2_3 > product_2_3:
+            product_2_3 = product_rot2_3
             rotated_2 = rotate(rotated_2, unitary)
 
             product_rot2_3 = product(rotated_2, visibility_state)
 
     return rotated_2.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
 
 
@@ -254,15 +255,15 @@
 
 @jit(nopython=True, nogil=True, cache=True)
 def random_d_fs(depth: int, quantity: int) -> npt.NDArray[np.complex64]:
     """Random n quDit state."""
     rand_vectors = get_random_haar_2d(depth, quantity)
     vector = normalize(rand_vectors[0])
 
-    for i in range(quantity - 1):
+    for i in range(1, quantity):
         idx_vector = normalize(rand_vectors[i])
 
         vector = np.outer(vector, idx_vector).flatten()
 
     vector = project(vector)
 
     return vector  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.3.0/pyproject.toml` & `cssfinder_backend_numpy-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry] # ANCHOR: tool.poetry
 name = "cssfinder_backend_numpy"
-version = "0.3.0"
+version = "0.4.0"
 description = "Implementation of CSSFinder backend using NumPy library."
 authors = [
     "Krzysztof Wiśniewski <argmaster.world@gmail.com>",
     "Marcin Wieśniak <marcin.wiesniak@ug.edu.pl>",
 ]
 repository = "https://github.com/argmaster/cssfinder_backend_numpy"
 readme = "README.md"
@@ -32,15 +32,15 @@
 mypy = "^1.0.1"
 ptpython = "^3.0.22"
 typing-extensions = "^4.4.0"
 snakeviz = "^2.1.1"
 poethepoet = "^0.18.1"
 poetry = "^1.3.2"
 jinja2 = "^3.1.2"
-ruff = "^0.0.257"
+ruff = ">=0.0.257,<0.0.263"
 ipykernel = "^6.21.3"
 cython = "3.0.0b1"
 
 [tool.poetry.scripts]
 cssfinder_backend_numpy = "cssfinder_backend_numpy.__main__:main"
 
 [tool.poe.tasks]
```

### Comparing `cssfinder_backend_numpy-0.3.0/PKG-INFO` & `cssfinder_backend_numpy-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cssfinder-backend-numpy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Implementation of CSSFinder backend using NumPy library.
 Home-page: https://github.com/argmaster/cssfinder_backend_numpy
 Author: Krzysztof Wiśniewski
 Author-email: argmaster.world@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -87,36 +87,36 @@
 
 ```
 poe build
 ```
 
 ![poe_build](https://user-images.githubusercontent.com/56170852/223251363-61fc4d00-68ad-429c-9fbb-8ab7f4712451.png)
 
-This will create `dist/` directory with `cssfinder_backend_numpy-0.3.0` or
+This will create `dist/` directory with `cssfinder_backend_numpy-0.4.0` or
 alike inside.
 
 Wheel file can be installed with
 
 ```
-pip install ./dist/cssfinder_backend_numpy-0.3.0
+pip install ./dist/cssfinder_backend_numpy-0.4.0
 ```
 
 What you expect is
 
 ```
-Successfully installed cssfinder_backend_numpy-0.3.0
+Successfully installed cssfinder_backend_numpy-0.4.0
 ```
 
 or rather something like
 
 ```
-Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder_backend_numpy-0.3.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
+Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder_backend_numpy-0.4.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
 ```
 
-But `cssfinder_backend_numpy-0.3.0` should be included in this list.
+But `cssfinder_backend_numpy-0.4.0` should be included in this list.
 
 ## Code quality
 
 To ensure that all code follow same style guidelines and code quality rules,
 multiple static analysis tools are used. For simplicity, all of them are
 configured as `pre-commit` ([learn about pre-commit](https://pre-commit.com/))
 hooks. Most of them however are listed as development dependencies.
```


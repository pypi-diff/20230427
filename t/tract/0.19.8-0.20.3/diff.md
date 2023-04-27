# Comparing `tmp/tract-0.19.8.tar.gz` & `tmp/tract-0.20.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tract-0.19.8.tar", last modified: Mon Mar 27 13:41:16 2023, max compression
+gzip compressed data, was "tract-0.20.3.tar", last modified: Wed Apr 26 10:01:29 2023, max compression
```

## Comparing `tract-0.19.8.tar` & `tract-0.20.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:41:16.459127 tract-0.19.8/
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-03-27 13:41:16.459127 tract-0.19.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-27 13:41:03.000000 tract-0.19.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 13:41:16.459127 tract-0.19.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-27 13:41:03.000000 tract-0.19.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:41:16.459127 tract-0.19.8/tract/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-27 13:41:03.000000 tract-0.19.8/tract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-27 13:41:03.000000 tract-0.19.8/tract/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-27 13:41:03.000000 tract-0.19.8/tract/fact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-03-27 13:41:03.000000 tract-0.19.8/tract/inference_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-03-27 13:41:03.000000 tract-0.19.8/tract/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-03-27 13:41:03.000000 tract-0.19.8/tract/nnef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-27 13:41:03.000000 tract-0.19.8/tract/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-27 13:41:03.000000 tract-0.19.8/tract/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-27 13:41:03.000000 tract-0.19.8/tract/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:41:16.459127 tract-0.19.8/tract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:01:29.375778 tract-0.20.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-26 10:01:29.375778 tract-0.20.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-26 10:01:21.000000 tract-0.20.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:01:29.375778 tract-0.20.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-26 10:01:21.000000 tract-0.20.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:01:29.375778 tract-0.20.3/tract/
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-26 10:01:21.000000 tract-0.20.3/tract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-26 10:01:21.000000 tract-0.20.3/tract/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-26 10:01:21.000000 tract-0.20.3/tract/fact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-26 10:01:21.000000 tract-0.20.3/tract/inference_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-26 10:01:21.000000 tract-0.20.3/tract/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-26 10:01:21.000000 tract-0.20.3/tract/nnef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-26 10:01:21.000000 tract-0.20.3/tract/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-26 10:01:21.000000 tract-0.20.3/tract/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-26 10:01:21.000000 tract-0.20.3/tract/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:01:29.375778 tract-0.20.3/tract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-26 10:01:29.000000 tract-0.20.3/tract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 10:01:29.000000 tract-0.20.3/tract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:01:29.000000 tract-0.20.3/tract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:01:29.000000 tract-0.20.3/tract.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 10:01:29.000000 tract-0.20.3/tract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 10:01:29.000000 tract-0.20.3/tract.egg-info/top_level.txt
```

### Comparing `tract-0.19.8/pyproject.toml` & `tract-0.20.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tract-0.19.8/setup.py` & `tract-0.20.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 import toml
 import re
 
 version = toml.load("../Cargo.toml")["package"]["version"]
 version = re.sub("\-alpha\.", "a", version)
 version = re.sub("\-.*", ".dev", version)
 
-with open('../../README.md', 'r') as file:
+with open('docs/index.md', 'r') as file:
     readme = file.read()
 
-
 setup(
         name="tract",
         author="Mathieu Poumeyrol, Sonos, and tract contributors",
         author_email="mathieu@poumeyrol.fr",
         keywords="onnx tensorflow nnef runtime neural network",
         version=version,
         description="Python bindings for tract, a neural network inference engine",
```

### Comparing `tract-0.19.8/tract/__init__.py` & `tract-0.20.3/tract/__init__.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.8/tract/bindings.py` & `tract-0.20.3/tract/bindings.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.8/tract/fact.py` & `tract-0.20.3/tract/fact.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from ctypes import *
 from tract.bindings import check, lib
 
 class InferenceFact:
+    """
+    Tract inference fact, to be used with InferenceModel.
+
+    It can represent partial type and shape information of a Tensor during model analysis.
+    """
     def __init__(self, ptr):
         self.ptr = ptr
 
     def __del__(self):
         if self.ptr:
             check(lib.tract_inference_fact_destroy(byref(self.ptr)))
 
@@ -21,14 +26,20 @@
         cstring = c_char_p();
         check(lib.tract_inference_fact_dump(self.ptr, byref(cstring)))
         result = str(cstring.value, "utf-8")
         lib.tract_free_cstring(cstring)
         return result
 
 class Fact:
+    """
+    Tract-core fact, to be used with Model.
+
+    It always contains the full shape (sometimes using symbolic dimensions) and item type.
+    In some situation it can also contain the constant value of the associated tensor.
+    """
     def __init__(self, ptr):
         self.ptr = ptr
 
     def __del__(self):
         if self.ptr:
             check(lib.tract_fact_destroy(byref(self.ptr)))
```

### Comparing `tract-0.19.8/tract/inference_model.py` & `tract-0.20.3/tract/inference_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,14 +93,25 @@
         if isinstance(fact, str):
             fact = self.fact(fact)
         if fact == None:
             check(lib.tract_inference_model_set_input_fact(self.ptr, input_id, None))
         else:
             check(lib.tract_inference_model_set_input_fact(self.ptr, input_id, fact.ptr))
 
+    def set_output_names(self, names: List[str]):
+        """Change the output nodes of the model"""
+        self._valid()
+        nb = len(names)
+        names_str = []
+        names_ptr = (c_char_p * nb)()
+        for ix, n in enumerate(names):
+            names_str.append(str(n).encode("utf-8"))
+            names_ptr[ix] = names_str[ix]
+        check(lib.tract_inference_model_set_output_names(self.ptr, nb, names_ptr))
+
     def output_name(self, output_id: int) -> str:
         """Return the name of the `output_id`th output."""
         self._valid()
         cstring = c_char_p()
         check(lib.tract_inference_model_output_name(self.ptr, output_id, byref(cstring)))
         result = str(cstring.value, "utf-8")
         lib.tract_free_cstring(cstring)
```

### Comparing `tract-0.19.8/tract/model.py` & `tract-0.20.3/tract/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,178 +4,214 @@
 from .bindings import check, lib
 from .fact import Fact
 from .value import Value
 from .runnable import Runnable
 
 class Model:
     """
-    Main model object
+    # Main model object
 
     ## Central focus point of the model transformation pipeline
-
+ 
     The Model is the central point of tract model loading and "model cooking". ONNX and NNEF 
     serialized models are converted to Model (more or less directly) before we can do anything
     of value with them. Model can be dumped to NNEF (or tract-opl which is NNEF plus tract
     proprietary extensions).
-   
+    
     A Model can be `optimize()`, substituing the "high level" operators in tract-core operator set by
     the best implementation available for the current system. From there it can be transformed into a 
     Runnable object that we will use to run.
-
+ 
     ## Model cooking
-
-    But some model transformations can be peformed on the Model class:
-     * declutter (getting rid of training artefacts)
-     * "pulsification" (transforming a batch-oriented model into a streaming model)
-     * symbol substitution (make N or Batch a fixed number, unlocking potential optimisation later on)
-     * static cost evalation and dynamic profiling
-     * ...
-
+ 
+    But some model transformations can be performed on the Model class:
+ 
+    - declutter (getting rid of training artefacts)
+    - "pulsification" (transforming a batch-oriented model into a streaming model)
+    - symbol substitution (make N or Batch a fixed number, unlocking potential optimisation later on)
+    - static cost evalation and dynamic profiling
+    - ...
+ 
     In some situation, these operation are done "on-the-fly" when a ONNX or NNEF model is loaded,
     at start-up time. In other situation, when start-up time becomes an issue, it may be beneficial
     to "pre-cook" the model: apply the transformations one time, serialize the model as NNEF (with
     tract-opl extension if needed). At start-up this model can be significantly less expensive to
     "cook" for inference.
-
-    # Model and TypedModel
+ 
+    ## Model and TypedModel
 
     This class is actually a wrapper around the "TypedModel" in Rust codebase. The "Typed"
     bit means than all shapes and element types in all input, output and temporary values must
     known. There is support in tract for symbols in dimensions, with some limited computation
     capabilities on symbolic expression. For instance, it is relatively frequent to work with
     a Model where all tensors shapes start with the `N` or `Batch`.
     """
+
     def __init__(self, ptr):
         self.ptr = ptr
 
     def __del__(self):
         if self.ptr:
             check(lib.tract_model_destroy(byref(self.ptr)))
 
     def _valid(self):
         if self.ptr == None:
             raise TractError("invalid model (maybe already consumed ?)")
 
-    """Return the number of inputs of the model"""
     def input_count(self) -> int:
+        """Return the number of inputs of the model"""
         self._valid()
         i = c_size_t()
         check(lib.tract_model_nbio(self.ptr, byref(i), None))
         return i.value
 
-    """Return the number of outputs of the model"""
     def output_count(self) -> int:
+        """Return the number of outputs of the model"""
         self._valid()
         i = c_size_t()
         check(lib.tract_model_nbio(self.ptr, None, byref(i)))
         return i.value
 
-    """Return the name of the input_id-th input"""
     def input_name(self, input_id: int) -> str:
+        """Return the name of the input_id-th input"""
         self._valid()
         cstring = c_char_p()
         check(lib.tract_model_input_name(self.ptr, input_id, byref(cstring)))
         result = str(cstring.value, "utf-8")
         lib.tract_free_cstring(cstring)
         return result
 
-    """Return the fact of the input_id-th input"""
     def input_fact(self, input_id: int) -> Fact:
+        """Return the fact of the input_id-th input"""
         self._valid()
         fact = c_void_p()
         check(lib.tract_model_input_fact(self.ptr, input_id, byref(fact)))
         return Fact(fact)
 
-    """Return the name of the output_id-th output"""
+    def set_output_names(self, names: List[str]):
+        """Change the output nodes of the model"""
+        self._valid()
+        nb = len(names)
+        names_str = []
+        names_ptr = (c_char_p * nb)()
+        for ix, n in enumerate(names):
+            names_str.append(str(n).encode("utf-8"))
+            names_ptr[ix] = names_str[ix]
+        check(lib.tract_model_set_output_names(self.ptr, nb, names_ptr))
+
     def output_name(self, output_id: int) -> str:
+        """Return the name of the output_id-th output"""
         self._valid()
         cstring = c_char_p()
         check(lib.tract_model_output_name(self.ptr, output_id, byref(cstring)))
         result = str(cstring.value, "utf-8")
         lib.tract_free_cstring(cstring)
         return result
 
-    """Return the fact of the output_id-th output"""
     def output_fact(self, input_id: int) -> Fact:
+        """Return the fact of the output_id-th output"""
         self._valid()
         fact = c_void_p()
         check(lib.tract_model_output_fact(self.ptr, input_id, byref(fact)))
         return Fact(fact)
 
-    """Substitute symbols by a value
+    def concretize_symbols(self, values: Dict[str, int]) -> None:
+        """Substitute symbols by a value
 
-    Replace all occurencies of the symbols in the dictionary, in all the Model facts shapes.
+        Replace all occurencies of the symbols in the dictionary, in all the Model facts shapes.
 
-    While this is not strictly necesary, the optimizing steps may make better choices if the model
-    is informed of some specific symbol values.
-    """
-    def concretize_symbols(self, values: Dict[str, int]) -> None:
+        While this is not strictly necesary, the optimizing steps may make better choices if the model
+        is informed of some specific symbol values.
+        """
         self._valid()
         nb = len(values)
         names_str = []
         names = (c_char_p * nb)()
         values_list = (c_int64 * nb)()
         for ix, (k, v) in enumerate(values.items()):
             names_str.append(str(k).encode("utf-8"))
             names[ix] = names_str[ix]
             values_list[ix] = v
         check(lib.tract_model_concretize_symbols(self.ptr, c_size_t(nb), names, values_list))
 
-    """Pulsify a model.
-
-    `pulse` is typically a one-length dictionary mapping the time dimension symbol to a pulse len.
-    """
     def pulse(self, symbol: str, pulse: Union[str, int]) -> None:
+        """Pulsify a model.
+
+        `pulse` is typically a one-length dictionary mapping the time dimension symbol to a pulse len.
+        """
         self._valid()
         check(lib.tract_model_pulse_simple(byref(self.ptr), symbol.encode("utf-8"), str(pulse).encode("utf-8")))
 
+    def half(self) -> None:
+        """Convert the model to hald precision
+        """
+        self._valid()
+        check(lib.tract_model_half(byref(self.ptr)))
+
     def declutter(self) -> None:
+        """Declutter a model.
+
+        Perform the first "half" of optimisation phases, consisting or removing training artefacts and converge
+        on tract-core canonical form.
+        """
         self._valid()
         check(lib.tract_model_declutter(self.ptr))
 
     def optimize(self) -> None:
+        """Optimize a model.
+
+        Perform the second "half" of optimisation phases, consisting of translating the tract-core canonical
+        form to the best runtime for the current architecture.
+        """
         self._valid()
         check(lib.tract_model_optimize(self.ptr))
 
-    """Convenience method performing `declutter()` and returning the model"""
     def into_decluttered(self) -> "Model":
+        """Convenience method performing `declutter()` and returning the model"""
         self.declutter();
         return self
 
-    """Convenience method performing `optimize()` and returning the model"""
     def into_optimized(self) -> "Model":
+        """Convenience method performing `optimize()` and returning the model"""
         self.optimize()
         return self
 
     def into_runnable(self) -> Runnable:
+        """Transform the model into a ready to be used Runnable model"""
         self._valid()
         runnable = c_void_p()
         check(lib.tract_model_into_runnable(byref(self.ptr), byref(runnable)))
         return Runnable(runnable)
 
     def property_keys(self) -> List[str]:
+        """Query the list of properties names of the model."""
         self._valid()
         count = c_size_t()
         check(lib.tract_model_property_count(self.ptr, byref(count)))
         count = count.value
         cstrings = (POINTER(c_char) * count)()
         check(lib.tract_model_property_names(self.ptr, cstrings))
         names = []
         for i in range(0, count):
             names.append(str(cast(cstrings[i], c_char_p).value, "utf-8"))
             lib.tract_free_cstring(cstrings[i])
         return names
 
     def property(self, name: str) -> Value:
+        """Query a property by name"""
         self._valid()
         value = c_void_p()
         check(lib.tract_model_property(self.ptr, str(name).encode("utf-8"), byref(value)))
         return Value(value)
 
     def profile_json(self, inputs: Union[None, List[Union[Value, numpy.ndarray]]]) -> str:
+        """Profile the model. Also compute the static costs of operators.
+
+        Returns is a json buffer.
+        """
         self._valid()
         cstring = c_char_p()
         input_values = []
         input_ptrs = None
         if inputs != None:
             for v in inputs:
                 if isinstance(v, Value):
```

### Comparing `tract-0.19.8/tract/nnef.py` & `tract-0.20.3/tract/nnef.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.8/tract/onnx.py` & `tract-0.20.3/tract/onnx.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.8/tract/value.py` & `tract-0.20.3/tract/value.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,14 +33,20 @@
         return 0x30 + dt.itemsize
     if dt.kind == 'c':
         return 0x50 + dt.itemsize / 2
     raise TractError("Unsupported Numpy dtype: " + dt)
 
 
 class Value:
+    """
+    Represents a tensor suitable for manipulation by tract.
+
+    On the Python side, the main way to access tensor data is to
+    convert the value to a numpy array.
+    """
     def __init__(self, ptr):
         self.ptr = ptr
 
     def __del__(self):
         if self.ptr:
             check(lib.tract_value_destroy(byref(self.ptr)))
 
@@ -59,23 +65,25 @@
         for ix in range(0, array.ndim):
             shape[ix] = array.shape[ix]
         dt = dt_numpy_to_tract(array.dtype)
         check(lib.tract_value_create(dt, c_size_t(array.ndim), shape, data, byref(ptr)))
         return Value(ptr)
 
     def to_numpy(self) -> numpy.array:
+        """Builds a numpy array equivalent to the data in this value."""
         self._valid()
         rank = c_size_t();
         shape = POINTER(c_size_t)()
         dt = c_float
         data = POINTER(dt)()
         check(lib.tract_value_inspect(self.ptr, None, byref(rank), byref(shape), byref(data)))
         rank = rank.value
         shape = [ int(shape[ix]) for ix in range(0, rank) ]
         array = numpy.ctypeslib.as_array(data, shape).copy()
         return array
 
     def into_numpy(self) -> numpy.array:
+        """Same as to_numpy(), but drop the value content once the numpy array is built."""
         result = self.to_numpy()
         check(lib.tract_value_destroy(byref(self.ptr)))
         return result
```


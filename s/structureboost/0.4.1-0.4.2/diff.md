# Comparing `tmp/structureboost-0.4.1.tar.gz` & `tmp/structureboost-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structureboost-0.4.1.tar", last modified: Wed Apr 19 15:53:20 2023, max compression
+gzip compressed data, was "structureboost-0.4.2.tar", last modified: Thu Apr 27 21:51:57 2023, max compression
```

## Comparing `structureboost-0.4.1.tar` & `structureboost-0.4.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-04-19 15:53:20.631988 structureboost-0.4.1/
--rw-r--r--   0 brianlucena   (501) staff       (20)     1069 2020-02-12 23:26:49.000000 structureboost-0.4.1/LICENSE
--rw-r--r--   0 brianlucena   (501) staff       (20)     2269 2023-04-19 15:53:20.631583 structureboost-0.4.1/PKG-INFO
--rw-r--r--   0 brianlucena   (501) staff       (20)     1379 2020-07-30 21:19:11.000000 structureboost-0.4.1/README.md
--rw-r--r--   0 brianlucena   (501) staff       (20)      216 2020-03-27 21:03:03.000000 structureboost-0.4.1/README.rst
--rw-r--r--   0 brianlucena   (501) staff       (20)       68 2022-05-16 23:30:25.000000 structureboost-0.4.1/pyproject.toml
--rw-r--r--   0 brianlucena   (501) staff       (20)       38 2023-04-19 15:53:20.632258 structureboost-0.4.1/setup.cfg
--rw-r--r--   0 brianlucena   (501) staff       (20)     3745 2023-04-19 15:49:55.000000 structureboost-0.4.1/setup.py
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-04-19 15:53:20.627601 structureboost-0.4.1/structureboost/
--rw-r--r--   0 brianlucena   (501) staff       (20)      771 2023-04-19 15:52:35.000000 structureboost-0.4.1/structureboost/__init__.py
--rw-r--r--   0 brianlucena   (501) staff       (20)  1291598 2023-04-18 22:17:55.000000 structureboost-0.4.1/structureboost/coarsage.c
--rw-r--r--   0 brianlucena   (501) staff       (20)  1627393 2023-04-18 22:17:56.000000 structureboost-0.4.1/structureboost/graphs.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   768847 2023-04-18 22:17:56.000000 structureboost-0.4.1/structureboost/pdf_discrete.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   685166 2023-04-18 22:17:56.000000 structureboost-0.4.1/structureboost/pdf_group.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   369766 2023-04-18 22:17:57.000000 structureboost-0.4.1/structureboost/pdf_set.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   331763 2023-04-18 22:17:57.000000 structureboost-0.4.1/structureboost/prob_regr_unit.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   791318 2023-04-18 22:17:57.000000 structureboost-0.4.1/structureboost/prob_regressor.c
--rw-r--r--   0 brianlucena   (501) staff       (20)  2549702 2023-04-18 22:18:00.000000 structureboost-0.4.1/structureboost/structure_dt.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   690000 2023-04-18 22:18:00.000000 structureboost-0.4.1/structureboost/structure_dt_multi.c
--rw-r--r--   0 brianlucena   (501) staff       (20)  2191823 2023-04-18 22:18:03.000000 structureboost-0.4.1/structureboost/structure_gb.c
--rw-r--r--   0 brianlucena   (501) staff       (20)  1662473 2023-04-18 22:18:05.000000 structureboost-0.4.1/structureboost/structure_gb_multi.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   802064 2023-04-18 22:18:06.000000 structureboost-0.4.1/structureboost/structure_rf.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   754981 2023-04-18 22:18:06.000000 structureboost-0.4.1/structureboost/structure_rfdt.c
--rw-r--r--   0 brianlucena   (501) staff       (20)     9676 2022-10-26 21:11:48.000000 structureboost-0.4.1/structureboost/utils.py
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-04-19 15:53:20.631096 structureboost-0.4.1/structureboost.egg-info/
--rw-r--r--   0 brianlucena   (501) staff       (20)     2269 2023-04-19 15:53:20.000000 structureboost-0.4.1/structureboost.egg-info/PKG-INFO
--rw-r--r--   0 brianlucena   (501) staff       (20)      719 2023-04-19 15:53:20.000000 structureboost-0.4.1/structureboost.egg-info/SOURCES.txt
--rw-r--r--   0 brianlucena   (501) staff       (20)        1 2023-04-19 15:53:20.000000 structureboost-0.4.1/structureboost.egg-info/dependency_links.txt
--rw-r--r--   0 brianlucena   (501) staff       (20)        1 2022-02-04 23:34:24.000000 structureboost-0.4.1/structureboost.egg-info/not-zip-safe
--rw-r--r--   0 brianlucena   (501) staff       (20)       85 2023-04-19 15:53:20.000000 structureboost-0.4.1/structureboost.egg-info/requires.txt
--rw-r--r--   0 brianlucena   (501) staff       (20)      176 2023-04-19 15:53:20.000000 structureboost-0.4.1/structureboost.egg-info/top_level.txt
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-04-27 21:51:57.303902 structureboost-0.4.2/
+-rw-r--r--   0 brianlucena   (501) staff       (20)     1069 2020-02-12 23:26:49.000000 structureboost-0.4.2/LICENSE
+-rw-r--r--   0 brianlucena   (501) staff       (20)     2269 2023-04-27 21:51:57.303463 structureboost-0.4.2/PKG-INFO
+-rw-r--r--   0 brianlucena   (501) staff       (20)     1379 2020-07-30 21:19:11.000000 structureboost-0.4.2/README.md
+-rw-r--r--   0 brianlucena   (501) staff       (20)      216 2020-03-27 21:03:03.000000 structureboost-0.4.2/README.rst
+-rw-r--r--   0 brianlucena   (501) staff       (20)       68 2022-05-16 23:30:25.000000 structureboost-0.4.2/pyproject.toml
+-rw-r--r--   0 brianlucena   (501) staff       (20)       38 2023-04-27 21:51:57.304016 structureboost-0.4.2/setup.cfg
+-rw-r--r--   0 brianlucena   (501) staff       (20)     3745 2023-04-27 21:29:17.000000 structureboost-0.4.2/setup.py
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-04-27 21:51:57.296860 structureboost-0.4.2/structureboost/
+-rw-r--r--   0 brianlucena   (501) staff       (20)      771 2023-04-27 21:29:07.000000 structureboost-0.4.2/structureboost/__init__.py
+-rw-r--r--   0 brianlucena   (501) staff       (20)  1292117 2023-04-27 21:30:02.000000 structureboost-0.4.2/structureboost/coarsage.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)  1627393 2023-04-27 21:30:03.000000 structureboost-0.4.2/structureboost/graphs.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   768847 2023-04-27 21:30:03.000000 structureboost-0.4.2/structureboost/pdf_discrete.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   685166 2023-04-27 21:30:04.000000 structureboost-0.4.2/structureboost/pdf_group.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   369766 2023-04-27 21:30:04.000000 structureboost-0.4.2/structureboost/pdf_set.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   331763 2023-04-27 21:30:04.000000 structureboost-0.4.2/structureboost/prob_regr_unit.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   791318 2023-04-27 21:30:04.000000 structureboost-0.4.2/structureboost/prob_regressor.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)  2549702 2023-04-27 21:30:07.000000 structureboost-0.4.2/structureboost/structure_dt.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   690000 2023-04-27 21:30:08.000000 structureboost-0.4.2/structureboost/structure_dt_multi.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)  2191823 2023-04-27 21:30:10.000000 structureboost-0.4.2/structureboost/structure_gb.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)  1662806 2023-04-27 21:30:13.000000 structureboost-0.4.2/structureboost/structure_gb_multi.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   802064 2023-04-27 21:30:13.000000 structureboost-0.4.2/structureboost/structure_rf.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   754981 2023-04-27 21:30:14.000000 structureboost-0.4.2/structureboost/structure_rfdt.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)     9676 2022-10-26 21:11:48.000000 structureboost-0.4.2/structureboost/utils.py
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-04-27 21:51:57.303012 structureboost-0.4.2/structureboost.egg-info/
+-rw-r--r--   0 brianlucena   (501) staff       (20)     2269 2023-04-27 21:51:57.000000 structureboost-0.4.2/structureboost.egg-info/PKG-INFO
+-rw-r--r--   0 brianlucena   (501) staff       (20)      719 2023-04-27 21:51:57.000000 structureboost-0.4.2/structureboost.egg-info/SOURCES.txt
+-rw-r--r--   0 brianlucena   (501) staff       (20)        1 2023-04-27 21:51:57.000000 structureboost-0.4.2/structureboost.egg-info/dependency_links.txt
+-rw-r--r--   0 brianlucena   (501) staff       (20)        1 2022-02-04 23:34:24.000000 structureboost-0.4.2/structureboost.egg-info/not-zip-safe
+-rw-r--r--   0 brianlucena   (501) staff       (20)       85 2023-04-27 21:51:57.000000 structureboost-0.4.2/structureboost.egg-info/requires.txt
+-rw-r--r--   0 brianlucena   (501) staff       (20)      176 2023-04-27 21:51:57.000000 structureboost-0.4.2/structureboost.egg-info/top_level.txt
```

### Comparing `structureboost-0.4.1/LICENSE` & `structureboost-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/PKG-INFO` & `structureboost-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structureboost
-Version: 0.4.1
+Version: 0.4.2
 Summary: StructureBoost is a Python package for gradient boosting using categorical structure.  See documentation at: https://structureboost.readthedocs.io/
 Home-page: https://github.com/numeristical/structureboost
 Author: Brian Lucena
 Author-email: brianlucena@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `structureboost-0.4.1/README.md` & `structureboost-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/setup.py` & `structureboost-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     author="Brian Lucena",
     author_email="brianlucena@gmail.com",
     name='structureboost',
     license="MIT",
     license_files=['LICENSE'],
     description="StructureBoost is a Python package for gradient boosting using categorical structure.  See documentation at: https://structureboost.readthedocs.io/",
-    version='0.4.1',
+    version='0.4.2',
     long_description=README,
     zip_safe=False,
     url='https://github.com/numeristical/structureboost',
     packages=['structureboost'],
     package_dir={'structureboost':
                  'structureboost'},
     python_requires=">=3.5",
```

### Comparing `structureboost-0.4.1/structureboost/__init__.py` & `structureboost-0.4.2/structureboost/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from prob_regr_unit import ProbRegressorUnit
 from prob_regressor import PrestoBoost
 from coarsage import Coarsage
 from pdf_discrete import PdfDiscrete, average_densities
 from pdf_group import PdfGroup, log_loss_pdf, test_between_quantiles_pdf, test_in_pred_regions
 from .utils import get_basic_config, apply_defaults, default_config_dict, ice_plot, log_loss
 
-__version__ = '0.4.1'
+__version__ = '0.4.2'
```

### Comparing `structureboost-0.4.1/structureboost/coarsage.c` & `structureboost-0.4.2/structureboost/coarsage.c`

 * *Files 1% similar despite different names*

```diff
@@ -2378,15 +2378,15 @@
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'libc.math' */
 
 /* Module declarations from 'structureboost.coarsage' */
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_long = { "long", NULL, sizeof(long), { 0 }, 0, IS_UNSIGNED(long) ? 'U' : 'I', IS_UNSIGNED(long), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int_t = { "int_t", NULL, sizeof(__pyx_t_5numpy_int_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int_t), 0 };
 #define __Pyx_MODULE_NAME "structureboost.coarsage"
 extern int __pyx_module_is_main_structureboost__coarsage;
 int __pyx_module_is_main_structureboost__coarsage = 0;
 
 /* Implementation of 'structureboost.coarsage' */
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_range;
@@ -17167,15 +17167,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/coarsage.pyx":628
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_8coarsage_9predict_with_tensor_c_mc(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_14structureboost_8coarsage_8predict_with_tensor_c_mc[] = "This is the same as the structure_gb_multi version except for num_classes.\n\n    Specifically, this permits that different trees may have a different \n    number of classes.";
 static PyMethodDef __pyx_mdef_14structureboost_8coarsage_9predict_with_tensor_c_mc = {"predict_with_tensor_c_mc", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_8coarsage_9predict_with_tensor_c_mc, METH_VARARGS|METH_KEYWORDS, __pyx_doc_14structureboost_8coarsage_8predict_with_tensor_c_mc};
@@ -17334,14 +17334,15 @@
   Py_ssize_t __pyx_t_18;
   long __pyx_t_19;
   long __pyx_t_20;
   long __pyx_t_21;
   Py_ssize_t __pyx_t_22;
   Py_ssize_t __pyx_t_23;
   Py_ssize_t __pyx_t_24;
+  __pyx_t_5numpy_int_t __pyx_t_25;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__34)
   __Pyx_RefNannySetupContext("predict_with_tensor_c_mc", 0);
   __Pyx_TraceCall("predict_with_tensor_c_mc", __pyx_f[0], 628, 0, __PYX_ERR(0, 628, __pyx_L1_error));
   __pyx_pybuffer_res_tens.pybuffer.buf = NULL;
@@ -17371,25 +17372,25 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm_float.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm_float, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm_float.diminfo[0].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm_float.diminfo[0].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm_float.diminfo[1].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm_float.diminfo[1].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm_float.diminfo[2].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm_float.diminfo[2].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm.diminfo[0].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm.diminfo[0].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm.diminfo[1].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm.diminfo[1].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm.diminfo[2].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm.diminfo[2].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feat_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_feat_array, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
   }
   __pyx_pybuffernd_feat_array.diminfo[0].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feat_array.diminfo[0].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_feat_array.diminfo[1].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_feat_array.diminfo[1].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[1];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer, (PyObject*)__pyx_v_num_classes_arr, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer, (PyObject*)__pyx_v_num_classes_arr, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
   }
   __pyx_pybuffernd_num_classes_arr.diminfo[0].strides = __pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_num_classes_arr.diminfo[0].shape = __pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/coarsage.pyx":637
  *     number of classes."""
  *     cdef long cat_vals_end
  *     cdef long max_num_classes = np.max(num_classes_arr)             # <<<<<<<<<<<<<<
@@ -17494,15 +17495,15 @@
   __pyx_t_8 = 0;
   __pyx_v_res_tens = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "structureboost/coarsage.pyx":644
  *     cdef double curr_val, ind_doub
  *     cdef bint at_leaf, found_val
- *     cdef np.ndarray[long, ndim=2] isnan_array = np.isnan(feat_array).astype(int)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.int_t, ndim=2] isnan_array = np.isnan(feat_array).astype(int)             # <<<<<<<<<<<<<<
  * 
  *     # These are in dtm_float
  */
   __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_isnan); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
@@ -17540,15 +17541,15 @@
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 644, __pyx_L1_error)
   __pyx_t_9 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_isnan_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_isnan_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_isnan_array = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 644, __pyx_L1_error)
     } else {__pyx_pybuffernd_isnan_array.diminfo[0].strides = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_isnan_array.diminfo[0].shape = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_isnan_array.diminfo[1].strides = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_isnan_array.diminfo[1].shape = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_9 = 0;
   __pyx_v_isnan_array = ((PyArrayObject *)__pyx_t_1);
@@ -17687,15 +17688,15 @@
  * 
  *     for k in range(dtm.shape[0]):
  *         num_classes=num_classes_arr[k]             # <<<<<<<<<<<<<<
  *         for ri in range(feat_array.shape[0]):
  *             cn = 0
  */
     __pyx_t_12 = __pyx_v_k;
-    __pyx_v_num_classes = (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_num_classes_arr.diminfo[0].strides));
+    __pyx_v_num_classes = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_num_classes_arr.diminfo[0].strides));
 
     /* "structureboost/coarsage.pyx":668
  *     for k in range(dtm.shape[0]):
  *         num_classes=num_classes_arr[k]
  *         for ri in range(feat_array.shape[0]):             # <<<<<<<<<<<<<<
  *             cn = 0
  *             at_leaf = 0
@@ -17740,15 +17741,15 @@
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:             # <<<<<<<<<<<<<<
  *                     at_leaf = 1
  *                     for q in range(num_classes):
  */
         __pyx_t_12 = __pyx_v_k;
         __pyx_t_17 = __pyx_v_cn;
         __pyx_t_18 = __pyx_v_NODE_TYPE;
-        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
+        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
         if (__pyx_t_16) {
 
           /* "structureboost/coarsage.pyx":674
  *                 cn = int(cn)
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:
  *                     at_leaf = 1             # <<<<<<<<<<<<<<
  *                     for q in range(num_classes):
@@ -17800,63 +17801,63 @@
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:             # <<<<<<<<<<<<<<
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:
  */
         __pyx_t_12 = __pyx_v_k;
         __pyx_t_17 = __pyx_v_cn;
         __pyx_t_18 = __pyx_v_NODE_TYPE;
-        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
+        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
         if (__pyx_t_16) {
 
           /* "structureboost/coarsage.pyx":678
  *                         res_tens[ri,k,q] = dtm_float[k,cn,NODE_VALUE_START+q]
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]             # <<<<<<<<<<<<<<
  *                     if isnan_array[ri,ind]:
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  */
           __pyx_t_18 = __pyx_v_k;
           __pyx_t_17 = __pyx_v_cn;
           __pyx_t_12 = __pyx_v_FEATURE_COL;
-          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides));
 
           /* "structureboost/coarsage.pyx":679
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  *                     else:
  */
           __pyx_t_12 = __pyx_v_ri;
           __pyx_t_17 = __pyx_v_ind;
-          __pyx_t_16 = ((*__Pyx_BufPtrStrided2d(long *, __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_isnan_array.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_isnan_array.diminfo[1].strides)) != 0);
+          __pyx_t_16 = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_isnan_array.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_isnan_array.diminfo[1].strides)) != 0);
           if (__pyx_t_16) {
 
             /* "structureboost/coarsage.pyx":680
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]             # <<<<<<<<<<<<<<
  *                     else:
  *                         curr_val = feat_array[ri,ind]
  */
             __pyx_t_17 = __pyx_v_k;
             __pyx_t_12 = __pyx_v_cn;
             __pyx_t_18 = __pyx_v_NA_LEFT;
-            if (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
+            if (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
               __pyx_t_24 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_22 = __pyx_v_LEFT_CHILD;
-              __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_22 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_24 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
-            __pyx_v_cn = __pyx_t_19;
+            __pyx_v_cn = __pyx_t_25;
 
             /* "structureboost/coarsage.pyx":679
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  *                     else:
@@ -17886,22 +17887,22 @@
             __pyx_t_12 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_THRESH;
             if (((__pyx_v_curr_val < (*__Pyx_BufPtrStrided3d(double *, __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm_float.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm_float.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm_float.diminfo[2].strides))) != 0)) {
               __pyx_t_24 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_22 = __pyx_v_LEFT_CHILD;
-              __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_22 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_24 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
-            __pyx_v_cn = __pyx_t_19;
+            __pyx_v_cn = __pyx_t_25;
           }
           __pyx_L12:;
 
           /* "structureboost/coarsage.pyx":677
  *                     for q in range(num_classes):
  *                         res_tens[ri,k,q] = dtm_float[k,cn,NODE_VALUE_START+q]
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:             # <<<<<<<<<<<<<<
@@ -17917,29 +17918,29 @@
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0
  */
         __pyx_t_17 = __pyx_v_k;
         __pyx_t_18 = __pyx_v_cn;
         __pyx_t_12 = __pyx_v_NODE_TYPE;
-        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
+        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
         if (__pyx_t_16) {
 
           /* "structureboost/coarsage.pyx":685
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]             # <<<<<<<<<<<<<<
  *                     found_val = 0
  *                     j = CAT_VALS_START
  */
           __pyx_t_12 = __pyx_v_k;
           __pyx_t_18 = __pyx_v_cn;
           __pyx_t_17 = __pyx_v_FEATURE_COL;
           __pyx_t_24 = __pyx_v_ri;
-          __pyx_t_23 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_t_23 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
           __pyx_v_curr_val = (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_feat_array.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_feat_array.diminfo[1].strides));
 
           /* "structureboost/coarsage.pyx":686
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0             # <<<<<<<<<<<<<<
  *                     j = CAT_VALS_START
@@ -17962,15 +17963,15 @@
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]             # <<<<<<<<<<<<<<
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  */
           __pyx_t_17 = __pyx_v_k;
           __pyx_t_18 = __pyx_v_cn;
           __pyx_t_12 = __pyx_v_NUM_CAT_VALS;
-          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides)));
+          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides)));
 
           /* "structureboost/coarsage.pyx":689
  *                     j = CAT_VALS_START
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]
  *                     while ((not found_val) & (j<cat_vals_end)):             # <<<<<<<<<<<<<<
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1
@@ -17985,15 +17986,15 @@
  *                         if curr_val==dtm[k,cn, j]:             # <<<<<<<<<<<<<<
  *                             found_val=1
  *                         else:
  */
             __pyx_t_12 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_j;
-            __pyx_t_16 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
+            __pyx_t_16 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
             if (__pyx_t_16) {
 
               /* "structureboost/coarsage.pyx":691
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1             # <<<<<<<<<<<<<<
  *                         else:
@@ -18031,22 +18032,22 @@
  *     return(res_tens)
  * 
  */
           if ((__pyx_v_found_val != 0)) {
             __pyx_t_17 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_12 = __pyx_v_LEFT_CHILD;
-            __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides));
           } else {
             __pyx_t_12 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_RIGHT_CHILD;
-            __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
           }
-          __pyx_v_cn = __pyx_t_19;
+          __pyx_v_cn = __pyx_t_25;
 
           /* "structureboost/coarsage.pyx":684
  *                         curr_val = feat_array[ri,ind]
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0
@@ -18069,15 +18070,15 @@
   __pyx_r = ((PyObject *)__pyx_v_res_tens);
   goto __pyx_L0;
 
   /* "structureboost/coarsage.pyx":628
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -18895,15 +18896,15 @@
   __pyx_v_num_fi = ((__pyx_v_fine_binpts->dimensions[0]) - 1);
 
   /* "structureboost/coarsage.pyx":738
  *     cdef long nt = coarse_pred.shape[1]
  *     cdef long num_fi = fine_binpts.shape[0]-1
  *     cdef np.ndarray[double, ndim=2] outmat = np.zeros((num_rows,num_fi))             # <<<<<<<<<<<<<<
  *     cdef long fi_ptr = 0
- *     cdef np.ndarray[long] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)
+ *     cdef np.ndarray[np.int_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_num_rows); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 738, __pyx_L1_error)
@@ -18948,23 +18949,23 @@
   __pyx_v_outmat = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "structureboost/coarsage.pyx":739
  *     cdef long num_fi = fine_binpts.shape[0]-1
  *     cdef np.ndarray[double, ndim=2] outmat = np.zeros((num_rows,num_fi))
  *     cdef long fi_ptr = 0             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[long] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)
+ *     cdef np.ndarray[np.int_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)
  *     cdef long row_ptr = 0
  */
   __pyx_v_fi_ptr = 0;
 
   /* "structureboost/coarsage.pyx":740
  *     cdef np.ndarray[double, ndim=2] outmat = np.zeros((num_rows,num_fi))
  *     cdef long fi_ptr = 0
- *     cdef np.ndarray[long] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.int_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)             # <<<<<<<<<<<<<<
  *     cdef long row_ptr = 0
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 740, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 740, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
@@ -18990,27 +18991,27 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 740, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_coarse_ptr_arr = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 740, __pyx_L1_error)
     } else {__pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides = __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].shape = __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_coarse_ptr_arr = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "structureboost/coarsage.pyx":741
  *     cdef long fi_ptr = 0
- *     cdef np.ndarray[long] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)
+ *     cdef np.ndarray[np.int_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)
  *     cdef long row_ptr = 0             # <<<<<<<<<<<<<<
  * 
  *     for fi_ptr in range(num_fi):
  */
   __pyx_v_row_ptr = 0;
 
   /* "structureboost/coarsage.pyx":743
@@ -19055,15 +19056,15 @@
  *                 outmat[row_ptr, fi_ptr] += coarse_pred[row_ptr, i, coarse_ptr_arr[i]] * lr             # <<<<<<<<<<<<<<
  *             if fine_binpts[fi_ptr+1] >= bv_mat[i,coarse_ptr_arr[i]+1]:
  *                 coarse_ptr_arr[i]+=1
  */
         __pyx_t_17 = __pyx_v_i;
         __pyx_t_18 = __pyx_v_row_ptr;
         __pyx_t_19 = __pyx_v_i;
-        __pyx_t_20 = (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides));
+        __pyx_t_20 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides));
         __pyx_t_21 = __pyx_v_row_ptr;
         __pyx_t_22 = __pyx_v_fi_ptr;
         *__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_outmat.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_outmat.diminfo[0].strides, __pyx_t_22, __pyx_pybuffernd_outmat.diminfo[1].strides) += ((*__Pyx_BufPtrStrided3d(double *, __pyx_pybuffernd_coarse_pred.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_coarse_pred.diminfo[0].strides, __pyx_t_19, __pyx_pybuffernd_coarse_pred.diminfo[1].strides, __pyx_t_20, __pyx_pybuffernd_coarse_pred.diminfo[2].strides)) * __pyx_v_lr);
       }
 
       /* "structureboost/coarsage.pyx":747
  *             for row_ptr in range(num_rows):
@@ -19071,27 +19072,27 @@
  *             if fine_binpts[fi_ptr+1] >= bv_mat[i,coarse_ptr_arr[i]+1]:             # <<<<<<<<<<<<<<
  *                 coarse_ptr_arr[i]+=1
  *     return(outmat)
  */
       __pyx_t_17 = (__pyx_v_fi_ptr + 1);
       __pyx_t_20 = __pyx_v_i;
       __pyx_t_19 = __pyx_v_i;
-      __pyx_t_18 = ((*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides)) + 1);
+      __pyx_t_18 = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides)) + 1);
       __pyx_t_23 = (((*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_fine_binpts.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_fine_binpts.diminfo[0].strides)) >= (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_bv_mat.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_bv_mat.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_bv_mat.diminfo[1].strides))) != 0);
       if (__pyx_t_23) {
 
         /* "structureboost/coarsage.pyx":748
  *                 outmat[row_ptr, fi_ptr] += coarse_pred[row_ptr, i, coarse_ptr_arr[i]] * lr
  *             if fine_binpts[fi_ptr+1] >= bv_mat[i,coarse_ptr_arr[i]+1]:
  *                 coarse_ptr_arr[i]+=1             # <<<<<<<<<<<<<<
  *     return(outmat)
  * 
  */
         __pyx_t_20 = __pyx_v_i;
-        *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides) += 1;
+        *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides) += 1;
 
         /* "structureboost/coarsage.pyx":747
  *             for row_ptr in range(num_rows):
  *                 outmat[row_ptr, fi_ptr] += coarse_pred[row_ptr, i, coarse_ptr_arr[i]] * lr
  *             if fine_binpts[fi_ptr+1] >= bv_mat[i,coarse_ptr_arr[i]+1]:             # <<<<<<<<<<<<<<
  *                 coarse_ptr_arr[i]+=1
  *     return(outmat)
@@ -21138,15 +21139,15 @@
   __Pyx_GIVEREF(__pyx_tuple__67);
   __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(7, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_coarsage_pyx, __pyx_n_s_expand_result_mat, 609, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 609, __pyx_L1_error)
 
   /* "structureboost/coarsage.pyx":628
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
   __pyx_tuple__68 = PyTuple_Pack(32, __pyx_n_s_dtm_float, __pyx_n_s_dtm, __pyx_n_s_feat_array, __pyx_n_s_num_classes_arr, __pyx_n_s_cat_vals_end, __pyx_n_s_max_num_classes, __pyx_n_s_num_classes, __pyx_n_s_res_tens, __pyx_n_s_cn, __pyx_n_s_ri, __pyx_n_s_ind, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_q, __pyx_n_s_curr_val, __pyx_n_s_ind_doub, __pyx_n_s_at_leaf, __pyx_n_s_found_val, __pyx_n_s_isnan_array, __pyx_n_s_THRESH, __pyx_n_s_NODE_WEIGHT, __pyx_n_s_NODE_VALUE_START, __pyx_n_s_NODE_TYPE, __pyx_n_s_FEATURE_COL, __pyx_n_s_LEFT_CHILD, __pyx_n_s_RIGHT_CHILD, __pyx_n_s_NA_LEFT, __pyx_n_s_NUM_CAT_VALS, __pyx_n_s_CAT_VALS_START, __pyx_n_s_LEAF, __pyx_n_s_NUMER, __pyx_n_s_CATEG); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__68);
   __Pyx_GIVEREF(__pyx_tuple__68);
   __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(4, 0, 32, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_coarsage_pyx, __pyx_n_s_predict_with_tensor_c_mc, 628, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 628, __pyx_L1_error)
 
@@ -22086,15 +22087,15 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_expand_result_mat, __pyx_t_2) < 0) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "structureboost/coarsage.pyx":628
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_8coarsage_9predict_with_tensor_c_mc, NULL, __pyx_n_s_structureboost_coarsage); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_predict_with_tensor_c_mc, __pyx_t_2) < 0) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
```

### Comparing `structureboost-0.4.1/structureboost/graphs.c` & `structureboost-0.4.2/structureboost/graphs.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost/pdf_discrete.c` & `structureboost-0.4.2/structureboost/pdf_discrete.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost/pdf_group.c` & `structureboost-0.4.2/structureboost/pdf_group.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost/pdf_set.c` & `structureboost-0.4.2/structureboost/pdf_set.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost/prob_regr_unit.c` & `structureboost-0.4.2/structureboost/prob_regr_unit.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost/prob_regressor.c` & `structureboost-0.4.2/structureboost/prob_regressor.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost/structure_dt.c` & `structureboost-0.4.2/structureboost/structure_dt.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost/structure_dt_multi.c` & `structureboost-0.4.2/structureboost/structure_dt_multi.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost/structure_gb.c` & `structureboost-0.4.2/structureboost/structure_gb.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost/structure_gb_multi.c` & `structureboost-0.4.2/structureboost/structure_gb_multi.c`

 * *Files 0% similar despite different names*

```diff
@@ -2723,16 +2723,16 @@
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_long = { "long", NULL, sizeof(long), { 0 }, 0, IS_UNSIGNED(long) ? 'U' : 'I', IS_UNSIGNED(long), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int_t = { "int_t", NULL, sizeof(__pyx_t_5numpy_int_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_long = { "long", NULL, sizeof(long), { 0 }, 0, IS_UNSIGNED(long) ? 'U' : 'I', IS_UNSIGNED(long), 0 };
 #define __Pyx_MODULE_NAME "structureboost.structure_gb_multi"
 extern int __pyx_module_is_main_structureboost__structure_gb_multi;
 int __pyx_module_is_main_structureboost__structure_gb_multi = 0;
 
 /* Implementation of 'structureboost.structure_gb_multi' */
 static PyObject *__pyx_builtin_super;
 static PyObject *__pyx_builtin_print;
@@ -12679,15 +12679,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_gb_multi.pyx":476
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_18structure_gb_multi_1predict_with_tensor_c_mc(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_18structure_gb_multi_1predict_with_tensor_c_mc = {"predict_with_tensor_c_mc", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_18structure_gb_multi_1predict_with_tensor_c_mc, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_18structure_gb_multi_1predict_with_tensor_c_mc(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -12840,14 +12840,15 @@
   Py_ssize_t __pyx_t_18;
   long __pyx_t_19;
   long __pyx_t_20;
   long __pyx_t_21;
   Py_ssize_t __pyx_t_22;
   Py_ssize_t __pyx_t_23;
   Py_ssize_t __pyx_t_24;
+  __pyx_t_5numpy_int_t __pyx_t_25;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__29)
   __Pyx_RefNannySetupContext("predict_with_tensor_c_mc", 0);
   __Pyx_TraceCall("predict_with_tensor_c_mc", __pyx_f[0], 476, 0, __PYX_ERR(0, 476, __pyx_L1_error));
   __pyx_pybuffer_res_tens.pybuffer.buf = NULL;
@@ -12873,15 +12874,15 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm_float.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm_float, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 476, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm_float.diminfo[0].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm_float.diminfo[0].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm_float.diminfo[1].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm_float.diminfo[1].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm_float.diminfo[2].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm_float.diminfo[2].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 476, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 476, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm.diminfo[0].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm.diminfo[0].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm.diminfo[1].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm.diminfo[1].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm.diminfo[2].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm.diminfo[2].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feat_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_feat_array, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 476, __pyx_L1_error)
   }
   __pyx_pybuffernd_feat_array.diminfo[0].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feat_array.diminfo[0].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_feat_array.diminfo[1].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_feat_array.diminfo[1].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[1];
@@ -12960,15 +12961,15 @@
   __pyx_t_7 = 0;
   __pyx_v_res_tens = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":487
  *     cdef double curr_val, ind_doub
  *     cdef bint at_leaf, found_val
- *     cdef np.ndarray[long, ndim=2] isnan_array = np.isnan(feat_array).astype(int)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.int_t, ndim=2] isnan_array = np.isnan(feat_array).astype(int)             # <<<<<<<<<<<<<<
  * 
  *     # These are in dtm_float
  */
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_isnan); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
@@ -13006,15 +13007,15 @@
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 487, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_isnan_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_isnan_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_isnan_array = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 487, __pyx_L1_error)
     } else {__pyx_pybuffernd_isnan_array.diminfo[0].strides = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_isnan_array.diminfo[0].shape = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_isnan_array.diminfo[1].strides = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_isnan_array.diminfo[1].shape = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_isnan_array = ((PyArrayObject *)__pyx_t_1);
@@ -13196,15 +13197,15 @@
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:             # <<<<<<<<<<<<<<
  *                     at_leaf = 1
  *                     for q in range(num_classes):
  */
         __pyx_t_16 = __pyx_v_k;
         __pyx_t_17 = __pyx_v_cn;
         __pyx_t_18 = __pyx_v_NODE_TYPE;
-        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
+        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
         if (__pyx_t_15) {
 
           /* "structureboost/structure_gb_multi.pyx":515
  *                 cn = int(cn)
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:
  *                     at_leaf = 1             # <<<<<<<<<<<<<<
  *                     for q in range(num_classes):
@@ -13256,63 +13257,63 @@
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:             # <<<<<<<<<<<<<<
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:
  */
         __pyx_t_16 = __pyx_v_k;
         __pyx_t_17 = __pyx_v_cn;
         __pyx_t_18 = __pyx_v_NODE_TYPE;
-        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
+        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
         if (__pyx_t_15) {
 
           /* "structureboost/structure_gb_multi.pyx":519
  *                         res_tens[ri,k,q] = dtm_float[k,cn,NODE_VALUE_START+q]
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]             # <<<<<<<<<<<<<<
  *                     if isnan_array[ri,ind]:
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  */
           __pyx_t_18 = __pyx_v_k;
           __pyx_t_17 = __pyx_v_cn;
           __pyx_t_16 = __pyx_v_FEATURE_COL;
-          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
 
           /* "structureboost/structure_gb_multi.pyx":520
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  *                     else:
  */
           __pyx_t_16 = __pyx_v_ri;
           __pyx_t_17 = __pyx_v_ind;
-          __pyx_t_15 = ((*__Pyx_BufPtrStrided2d(long *, __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_isnan_array.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_isnan_array.diminfo[1].strides)) != 0);
+          __pyx_t_15 = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_isnan_array.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_isnan_array.diminfo[1].strides)) != 0);
           if (__pyx_t_15) {
 
             /* "structureboost/structure_gb_multi.pyx":521
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]             # <<<<<<<<<<<<<<
  *                     else:
  *                         curr_val = feat_array[ri,ind]
  */
             __pyx_t_17 = __pyx_v_k;
             __pyx_t_16 = __pyx_v_cn;
             __pyx_t_18 = __pyx_v_NA_LEFT;
-            if (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
+            if (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
               __pyx_t_24 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_22 = __pyx_v_LEFT_CHILD;
-              __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_22 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_24 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
-            __pyx_v_cn = __pyx_t_19;
+            __pyx_v_cn = __pyx_t_25;
 
             /* "structureboost/structure_gb_multi.pyx":520
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  *                     else:
@@ -13342,22 +13343,22 @@
             __pyx_t_16 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_THRESH;
             if (((__pyx_v_curr_val < (*__Pyx_BufPtrStrided3d(double *, __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm_float.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm_float.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm_float.diminfo[2].strides))) != 0)) {
               __pyx_t_24 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_22 = __pyx_v_LEFT_CHILD;
-              __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_22 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_24 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
-            __pyx_v_cn = __pyx_t_19;
+            __pyx_v_cn = __pyx_t_25;
           }
           __pyx_L12:;
 
           /* "structureboost/structure_gb_multi.pyx":518
  *                     for q in range(num_classes):
  *                         res_tens[ri,k,q] = dtm_float[k,cn,NODE_VALUE_START+q]
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:             # <<<<<<<<<<<<<<
@@ -13373,29 +13374,29 @@
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0
  */
         __pyx_t_17 = __pyx_v_k;
         __pyx_t_18 = __pyx_v_cn;
         __pyx_t_16 = __pyx_v_NODE_TYPE;
-        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
+        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
         if (__pyx_t_15) {
 
           /* "structureboost/structure_gb_multi.pyx":526
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]             # <<<<<<<<<<<<<<
  *                     found_val = 0
  *                     j = CAT_VALS_START
  */
           __pyx_t_16 = __pyx_v_k;
           __pyx_t_18 = __pyx_v_cn;
           __pyx_t_17 = __pyx_v_FEATURE_COL;
           __pyx_t_24 = __pyx_v_ri;
-          __pyx_t_23 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_t_23 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
           __pyx_v_curr_val = (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_feat_array.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_feat_array.diminfo[1].strides));
 
           /* "structureboost/structure_gb_multi.pyx":527
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0             # <<<<<<<<<<<<<<
  *                     j = CAT_VALS_START
@@ -13418,15 +13419,15 @@
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]             # <<<<<<<<<<<<<<
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  */
           __pyx_t_17 = __pyx_v_k;
           __pyx_t_18 = __pyx_v_cn;
           __pyx_t_16 = __pyx_v_NUM_CAT_VALS;
-          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides)));
+          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides)));
 
           /* "structureboost/structure_gb_multi.pyx":530
  *                     j = CAT_VALS_START
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]
  *                     while ((not found_val) & (j<cat_vals_end)):             # <<<<<<<<<<<<<<
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1
@@ -13441,15 +13442,15 @@
  *                         if curr_val==dtm[k,cn, j]:             # <<<<<<<<<<<<<<
  *                             found_val=1
  *                         else:
  */
             __pyx_t_16 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_j;
-            __pyx_t_15 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
+            __pyx_t_15 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
             if (__pyx_t_15) {
 
               /* "structureboost/structure_gb_multi.pyx":532
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1             # <<<<<<<<<<<<<<
  *                         else:
@@ -13487,22 +13488,22 @@
  *     return(res_tens)
  * 
  */
           if ((__pyx_v_found_val != 0)) {
             __pyx_t_17 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_16 = __pyx_v_LEFT_CHILD;
-            __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
           } else {
             __pyx_t_16 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_RIGHT_CHILD;
-            __pyx_t_19 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
           }
-          __pyx_v_cn = __pyx_t_19;
+          __pyx_v_cn = __pyx_t_25;
 
           /* "structureboost/structure_gb_multi.pyx":525
  *                         curr_val = feat_array[ri,ind]
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0
@@ -13525,15 +13526,15 @@
   __pyx_r = ((PyObject *)__pyx_v_res_tens);
   goto __pyx_L0;
 
   /* "structureboost/structure_gb_multi.pyx":476
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -32245,15 +32246,15 @@
   __Pyx_GIVEREF(__pyx_tuple__79);
   __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__79, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_multi_pyx, __pyx_n_s_convert_subtree, 451, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 451, __pyx_L1_error)
 
   /* "structureboost/structure_gb_multi.pyx":476
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
   __pyx_tuple__80 = PyTuple_Pack(30, __pyx_n_s_dtm_float, __pyx_n_s_dtm, __pyx_n_s_feat_array, __pyx_n_s_num_classes, __pyx_n_s_cat_vals_end, __pyx_n_s_res_tens, __pyx_n_s_cn, __pyx_n_s_ri, __pyx_n_s_ind, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_q, __pyx_n_s_curr_val, __pyx_n_s_ind_doub, __pyx_n_s_at_leaf, __pyx_n_s_found_val, __pyx_n_s_isnan_array, __pyx_n_s_THRESH, __pyx_n_s_NODE_WEIGHT, __pyx_n_s_NODE_VALUE_START, __pyx_n_s_NODE_TYPE, __pyx_n_s_FEATURE_COL, __pyx_n_s_LEFT_CHILD, __pyx_n_s_RIGHT_CHILD, __pyx_n_s_NA_LEFT, __pyx_n_s_NUM_CAT_VALS, __pyx_n_s_CAT_VALS_START, __pyx_n_s_LEAF, __pyx_n_s_NUMER, __pyx_n_s_CATEG); if (unlikely(!__pyx_tuple__80)) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__80);
   __Pyx_GIVEREF(__pyx_tuple__80);
   __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(4, 0, 30, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__80, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_multi_pyx, __pyx_n_s_predict_with_tensor_c_mc, 476, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 476, __pyx_L1_error)
 
@@ -33277,15 +33278,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":476
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_18structure_gb_multi_1predict_with_tensor_c_mc, NULL, __pyx_n_s_structureboost_structure_gb_mult); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_predict_with_tensor_c_mc, __pyx_t_1) < 0) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `structureboost-0.4.1/structureboost/structure_rf.c` & `structureboost-0.4.2/structureboost/structure_rf.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost/structure_rfdt.c` & `structureboost-0.4.2/structureboost/structure_rfdt.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost/utils.py` & `structureboost-0.4.2/structureboost/utils.py`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.1/structureboost.egg-info/PKG-INFO` & `structureboost-0.4.2/structureboost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structureboost
-Version: 0.4.1
+Version: 0.4.2
 Summary: StructureBoost is a Python package for gradient boosting using categorical structure.  See documentation at: https://structureboost.readthedocs.io/
 Home-page: https://github.com/numeristical/structureboost
 Author: Brian Lucena
 Author-email: brianlucena@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `structureboost-0.4.1/structureboost.egg-info/SOURCES.txt` & `structureboost-0.4.2/structureboost.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/dummy_kinematics-0.0.6.tar.gz` & `tmp/dummy_kinematics-0.0.7a0.tar.gz`

## Comparing `dummy_kinematics-0.0.6.tar` & `dummy_kinematics-0.0.7a0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/test2.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/__about__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/__init__.py
--rw-r--r--   0        0        0    19633 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/chart_element.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/config.py
--rw-r--r--   0        0        0    10322 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/data_converter.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/descriptors.py
--rw-r--r--   0        0        0    54622 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/dummy_iso_config.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/json_file_helper.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/logger_helper.py
--rw-r--r--   0        0        0    21226 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/ppt_factory.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/ppt_insert_helper.py
--rw-r--r--   0        0        0    14366 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/unitils.py
--rw-r--r--   0        0        0   111915 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/dummy_kinematics/default/default_template.pptx
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/README.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/PKG-INFO
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/test2.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/__about__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/__init__.py
+-rw-r--r--   0        0        0    19633 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/chart_element.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/config.py
+-rw-r--r--   0        0        0    10322 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/data_converter.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/descriptors.py
+-rw-r--r--   0        0        0    54622 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/dummy_iso_config.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/json_file_helper.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/logger_helper.py
+-rw-r--r--   0        0        0    21226 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/ppt_factory.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/ppt_insert_helper.py
+-rw-r--r--   0        0        0    15270 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/unitils.py
+-rw-r--r--   0        0        0   111915 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/dummy_kinematics/default/default_template.pptx
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/tests/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/LICENSE.txt
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/README.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/pyproject.toml
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.7a0/PKG-INFO
```

### Comparing `dummy_kinematics-0.0.6/test2.py` & `dummy_kinematics-0.0.7a0/test2.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.6/dummy_kinematics/chart_element.py` & `dummy_kinematics-0.0.7a0/dummy_kinematics/chart_element.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.6/dummy_kinematics/data_converter.py` & `dummy_kinematics-0.0.7a0/dummy_kinematics/data_converter.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.6/dummy_kinematics/descriptors.py` & `dummy_kinematics-0.0.7a0/dummy_kinematics/descriptors.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.6/dummy_kinematics/dummy_iso_config.py` & `dummy_kinematics-0.0.7a0/dummy_kinematics/dummy_iso_config.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.6/dummy_kinematics/logger_helper.py` & `dummy_kinematics-0.0.7a0/dummy_kinematics/logger_helper.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.6/dummy_kinematics/ppt_factory.py` & `dummy_kinematics-0.0.7a0/dummy_kinematics/ppt_factory.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.6/dummy_kinematics/ppt_insert_helper.py` & `dummy_kinematics-0.0.7a0/dummy_kinematics/ppt_insert_helper.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.6/dummy_kinematics/unitils.py` & `dummy_kinematics-0.0.7a0/dummy_kinematics/unitils.py`

 * *Files 3% similar despite different names*

```diff
@@ -439,7 +439,30 @@
     low_score, low_index = low_score_index
     if x < high_index:
         return high_score
     if x > low_index:
         return low_score
     k = (high_score - low_score) / (high_index - low_index)
     return high_score + k * (x - high_index)
+
+
+def cal_rttf(acc_g: NDArray,
+             speed_kph: float,
+             start_ms: float = 0,
+             end_ms: float = 200,
+             step_ms: float = 0.1) -> tuple[float, float]:
+    """根据三英寸，五英寸-30ms 计算RTTF"""
+    df = pd.DataFrame({"acc_g": acc_g})
+    df["dummy_g"] = 0
+    df['svel_abs'] = g_to_s(acc_g, step_ms, speed_kph, 0, True)
+    df['sd_abs'] = g_to_s(df['dummy_g'].values, step_ms, speed_kph, 0)
+    df['sd_relative'] = df['sd_abs'] - df['svel_abs']
+    timeseries = np.arange(start_ms, end_ms + step_ms, step_ms)
+    inch3 = 76
+    inch5 = 127
+    index, number = index_number(df['sd_relative'], inch3)
+    rttf_min = timeseries[index] - 30
+    rttf_min = round(rttf_min, 2)
+    index, number = index_number(df['sd_relative'], inch5)
+    rttf_max = timeseries[index] - 30
+    rttf_max = round(rttf_max, 2)
+    return rttf_min, rttf_max
```

### Comparing `dummy_kinematics-0.0.6/dummy_kinematics/default/default_template.pptx` & `dummy_kinematics-0.0.7a0/dummy_kinematics/default/default_template.pptx`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.6/README.md` & `dummy_kinematics-0.0.7a0/README.md`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.6/pyproject.toml` & `dummy_kinematics-0.0.7a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.6/PKG-INFO` & `dummy_kinematics-0.0.7a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummy-kinematics
-Version: 0.0.6
+Version: 0.0.7a0
 Project-URL: Documentation, https://github.com/unknown/dummy-kinematics#readme
 Project-URL: Issues, https://github.com/unknown/dummy-kinematics/issues
 Project-URL: Source, https://github.com/unknown/dummy-kinematics
 Author-email: xiaochai <1219295581@qq.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```


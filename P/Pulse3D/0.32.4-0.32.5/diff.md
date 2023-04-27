# Comparing `tmp/Pulse3D-0.32.4.tar.gz` & `tmp/Pulse3D-0.32.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.32.4.tar", last modified: Fri Apr 21 20:31:18 2023, max compression
+gzip compressed data, was "Pulse3D-0.32.5.tar", last modified: Thu Apr 27 01:50:44 2023, max compression
```

## Comparing `Pulse3D-0.32.4.tar` & `Pulse3D-0.32.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-21 20:30:15.000000 Pulse3D-0.32.4/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 20:30:15.000000 Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-21 20:30:15.000000 Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-21 20:30:15.000000 Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-21 20:30:15.000000 Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-21 20:31:18.000000 Pulse3D-0.32.4/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-21 20:31:18.000000 Pulse3D-0.32.4/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:31:03.000000 Pulse3D-0.32.4/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 20:30:44.000000 Pulse3D-0.32.4/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-21 20:30:44.000000 Pulse3D-0.32.4/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-21 20:30:44.000000 Pulse3D-0.32.4/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-21 20:30:44.000000 Pulse3D-0.32.4/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    45242 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34501 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19450 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-27 01:49:39.000000 Pulse3D-0.32.5/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.598796 Pulse3D-0.32.5/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 01:49:39.000000 Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-27 01:49:39.000000 Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-27 01:49:39.000000 Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-27 01:49:39.000000 Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-27 01:50:44.606796 Pulse3D-0.32.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-27 01:50:44.000000 Pulse3D-0.32.5/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-27 01:50:44.000000 Pulse3D-0.32.5/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 01:50:29.000000 Pulse3D-0.32.5/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 01:50:08.000000 Pulse3D-0.32.5/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-27 01:50:08.000000 Pulse3D-0.32.5/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-27 01:50:08.000000 Pulse3D-0.32.5/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-27 01:50:08.000000 Pulse3D-0.32.5/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:50:44.602796 Pulse3D-0.32.5/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45167 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34501 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-27 01:49:36.000000 Pulse3D-0.32.5/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.32.4/LICENSE` & `Pulse3D-0.32.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/PKG-INFO` & `Pulse3D-0.32.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.32.4
+Version: 0.32.5
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.32.4/mantarray-magnet-finding/setup.py` & `Pulse3D-0.32.5/mantarray-magnet-finding/setup.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.32.5/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/setup.py` & `Pulse3D-0.32.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.32.4",
+    version="0.32.5",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.32.4/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.32.5/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.32.4
+Version: 0.32.5
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.32.4/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.32.5/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.32.5/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.32.5/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.32.5/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/src/pulse3D/constants.py` & `Pulse3D-0.32.5/src/pulse3D/constants.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/src/pulse3D/excel_writer.py` & `Pulse3D-0.32.5/src/pulse3D/excel_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,18 +120,15 @@
     well_row = well_index * num_per_twitch_metrics
     last_column = xl_col_to_name(num_data_points)
 
     force_frequency_chart.add_series(
         {
             "categories": f"='{PER_TWITCH_METRICS_SHEET_NAME}'!$B${well_row + 7}:${last_column}${well_row + 7}",
             "values": f"='{PER_TWITCH_METRICS_SHEET_NAME}'!$B${well_row + 5}:${last_column}${well_row + 5}",
-            "marker": {
-                "type": "diamond",
-                "size": 7,
-            },
+            "marker": {"type": "diamond", "size": 7},
             "line": {"none": True},
         }
     )
 
     force_frequency_chart.set_legend({"none": True})
     x_axis_label = CALCULATED_METRIC_DISPLAY_NAMES[TWITCH_FREQUENCY_UUID]
 
@@ -657,19 +654,15 @@
             num_data_points = len(well_metrics[0])
 
             force_freq_chart = wb.add_chart({"type": "scatter", "subtype": "straight"})
             freq_vs_time_chart = wb.add_chart({"type": "scatter", "subtype": "straight"})
 
             log.info(f"Creating frequency vs time chart for well {well_info['well_name']}")
             create_frequency_vs_time_charts(
-                freq_vs_time_sheet,
-                freq_vs_time_chart,
-                well_info,
-                num_data_points,
-                num_metrics,
+                freq_vs_time_sheet, freq_vs_time_chart, well_info, num_data_points, num_metrics
             )
 
             log.info(f"Creating force frequency relationship chart for well {well_info['well_name']}")
             create_force_frequency_relationship_charts(
                 force_freq_sheet,
                 force_freq_chart,
                 well_info["well_index"],
@@ -763,20 +756,20 @@
     stim_plotting_info,
 ):
     well_idx = well_info["well_index"]
     well_name = well_info["well_name"]
 
     # maximum snapshot size is 10 seconds
     snapshot_lower_x_bound = well_info["tissue_data"][0, 0]
-    snapshot_upper_x_bound = min(well_info["tissue_data"][0, -1], CHART_MAXIMUM_SNAPSHOT_LENGTH_SECS)
-
+    snapshot_upper_x_bound = min(
+        well_info["tissue_data"][0, -1], snapshot_lower_x_bound + CHART_MAXIMUM_SNAPSHOT_LENGTH_SECS
+    )
     df_column = continuous_waveforms_df.columns.get_loc(f"{well_name} - Active Twitch Force (μN)")
 
     well_column = xl_col_to_name(df_column)
-
     # plot snapshot of waveform
     snapshot_plot_params = plotting_parameters(snapshot_upper_x_bound - snapshot_lower_x_bound)
 
     snapshot_chart = wb.add_chart({"type": "scatter", "subtype": "straight"})
 
     snapshot_chart.set_x_axis(
         {"name": "Time (seconds)", "min": snapshot_lower_x_bound, "max": snapshot_upper_x_bound}
```

### Comparing `Pulse3D-0.32.4/src/pulse3D/exceptions.py` & `Pulse3D-0.32.5/src/pulse3D/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/src/pulse3D/magnet_finding.py` & `Pulse3D-0.32.5/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/src/pulse3D/metrics.py` & `Pulse3D-0.32.5/src/pulse3D/metrics.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/src/pulse3D/peak_detection.py` & `Pulse3D-0.32.5/src/pulse3D/peak_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     windowed_signal = filtered_magnetic_signal[:, window_indices]
 
     # interpolated data points are required, meaning that the time steps should all be the same, so using the first one
     sampling_period_us = windowed_signal[0, 1] - windowed_signal[0, 0]
 
     max_possible_twitch_freq = 7
     min_required_samples_between_twitches = int(
-        round((1 / max_possible_twitch_freq) * MICRO_TO_BASE_CONVERSION / sampling_period_us, 0),
+        round((1 / max_possible_twitch_freq) * MICRO_TO_BASE_CONVERSION / sampling_period_us, 0)
     )
 
     magnetic_signal = windowed_signal[1, :]
     # find required height of peaks
     max_prominence = abs(np.max(magnetic_signal) - np.min(magnetic_signal))
 
     # find peaks and valleys
@@ -120,15 +120,15 @@
         expected_prominences = (factors, factors)
     else:
         expected_prominences = factors if len(factors) == 2 else (factors[0], factors[0])
     return expected_prominences
 
 
 def find_twitch_indices(
-    peak_and_valley_indices: Tuple[NDArray[int], NDArray[int]],
+    peak_and_valley_indices: Tuple[NDArray[int], NDArray[int]]
 ) -> Dict[int, Dict[UUID, Optional[int]]]:
     """Find twitches that can be analyzed.
 
     Sometimes the first and last peak in a trace can't be analyzed as a full twitch because not
     enough information is present.
     In order to be analyzable, a twitch needs to have a valley prior to it and another peak after it.
```

### Comparing `Pulse3D-0.32.4/src/pulse3D/plate_recording.py` & `Pulse3D-0.32.5/src/pulse3D/plate_recording.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/src/pulse3D/plotting.py` & `Pulse3D-0.32.5/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/src/pulse3D/stimulation.py` & `Pulse3D-0.32.5/src/pulse3D/stimulation.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.4/src/pulse3D/transforms.py` & `Pulse3D-0.32.5/src/pulse3D/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,34 +24,22 @@
 from .constants import RAW_TO_SIGNED_CONVERSION_VALUE
 from .constants import REFERENCE_VOLTAGE
 from .exceptions import FilterCreationNotImplementedError
 from .exceptions import UnrecognizedFilterUuidError
 
 
 FILTER_CHARACTERISTICS: Dict[uuid.UUID, Dict[str, Union[str, float, int]]] = {
-    BESSEL_BANDPASS_UUID: {
-        "filter_type": "bessel",
-        "order": 4,
-        "high_pass_hz": 0.1,
-        "low_pass_hz": 10,
-    },
+    BESSEL_BANDPASS_UUID: {"filter_type": "bessel", "order": 4, "high_pass_hz": 0.1, "low_pass_hz": 10},
     BESSEL_LOWPASS_10_UUID: {"filter_type": "bessel", "order": 4, "low_pass_hz": 10},
     BESSEL_LOWPASS_30_UUID: {"filter_type": "bessel", "order": 4, "low_pass_hz": 30},
-    BUTTERWORTH_LOWPASS_30_UUID: {
-        "filter_type": "butterworth",
-        "order": 4,
-        "low_pass_hz": 30,
-    },
+    BUTTERWORTH_LOWPASS_30_UUID: {"filter_type": "butterworth", "order": 4, "low_pass_hz": 30},
 }
 
 
-def create_filter(
-    filter_uuid: uuid.UUID,
-    sample_period_microseconds: int,
-) -> NDArray[(Any, Any), float]:
+def create_filter(filter_uuid: uuid.UUID, sample_period_microseconds: int) -> NDArray[(Any, Any), float]:
     """Create a filter to apply to data streams.
 
     Args:
         filter_uuid: a UUID of an already accepted and approved filter
         sample_period_microseconds: the sampling period for the data stream you want to apply the filter to
 
     Returns:
@@ -130,33 +118,30 @@
 
     Returns:
         A single 2D array of time vs GMR reading.
     """
     return tissue_gmr_reading
 
 
-def apply_empty_plate_calibration(
-    noise_cancelled_gmr: NDArray[(2, Any), int],
-) -> NDArray[(2, Any), int]:
+def apply_empty_plate_calibration(noise_cancelled_gmr: NDArray[(2, Any), int]) -> NDArray[(2, Any), int]:
     """Apply the result of an empty plate calibration.
 
     Actual empty plate calibration will be performed once information obtained from Jason.
 
     Args:
         noise_cancelled_gmr: an 2D array of Time and GMR readings after combining reference and tissue sensor readings.
 
     Returns:
         A 2D array of the Time and GMR readings after empty plate calibration. Data will be rounded to integers if calibration results in slight decimal behavior.
     """
     return noise_cancelled_gmr
 
 
 def apply_noise_filtering(
-    fully_calibrated_gmr: NDArray[(2, Any), int],
-    scipy_filter_sos_coefficients: NDArray[(Any, Any), float],
+    fully_calibrated_gmr: NDArray[(2, Any), int], scipy_filter_sos_coefficients: NDArray[(Any, Any), float]
 ) -> NDArray[(2, Any), int]:
     """Apply the result of an empty plate calibration.
 
     Actual empty plate calibration will be performed once information obtained from Jason.
 
     Args:
         fully_calibrated_gmr: an 2D array of Time and GMR readings after applying the Empty Plate calibration.
@@ -195,15 +180,15 @@
     millivolts_per_lsb = 1000 * reference_voltage / RAW_TO_SIGNED_CONVERSION_VALUE
     sample_in_millivolts = gmr_data[1, :].astype(np.float64) * millivolts_per_lsb * (1 / adc_gain)
     sample_in_volts = sample_in_millivolts / MILLI_TO_BASE_CONVERSION
     return np.vstack((gmr_data[0, :].astype(np.float64), sample_in_volts))
 
 
 def calculate_displacement_from_voltage(
-    voltage_data: NDArray[(2, Any), np.float64],
+    voltage_data: NDArray[(2, Any), np.float64]
 ) -> NDArray[(2, Any), np.float64]:
     """Convert voltage to displacement.
 
     Conversion values were obtained 03/09/2021 by Kevin Gray
 
     Args:
         voltage_data: time and Voltage numpy array. Typically coming from calculate_voltage_from_gmr
```

### Comparing `Pulse3D-0.32.4/src/pulse3D/utils.py` & `Pulse3D-0.32.5/src/pulse3D/utils.py`

 * *Files identical despite different names*


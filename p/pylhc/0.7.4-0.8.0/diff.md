# Comparing `tmp/pylhc-0.7.4.tar.gz` & `tmp/pylhc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PyLHC/PyLHC/dist/tmpmmmux25f/pylhc-0.7.4.tar", last modified: Wed Oct 19 16:11:53 2022, max compression
+gzip compressed data, was "pylhc-0.8.0.tar", last modified: Thu Apr 27 16:04:49 2023, max compression
```

## Comparing `pylhc-0.7.4.tar` & `pylhc-0.8.0.tar`

### file list

```diff
@@ -1,39 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:11:53.000000 pylhc-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-19 16:11:30.000000 pylhc-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4164 2022-10-19 16:11:53.000000 pylhc-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-10-19 16:11:30.000000 pylhc-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:11:53.000000 pylhc-0.7.4/pylhc/
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3590 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/bpm_calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)    15453 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/bsrt_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     3403 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/bsrt_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:11:53.000000 pylhc-0.7.4/pylhc/calibration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9146 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/calibration/beta.py
--rw-r--r--   0 runner    (1001) docker     (121)     8262 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/calibration/dispersion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:11:53.000000 pylhc-0.7.4/pylhc/constants/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/constants/calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4185 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/constants/forced_da_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/constants/general.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/constants/kickgroups.py
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/constants/machine_settings_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:11:53.000000 pylhc-0.7.4/pylhc/data_extract/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/data_extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15161 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/data_extract/lsa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/data_extract/timber.py
--rw-r--r--   0 runner    (1001) docker     (121)    51012 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/forced_da_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    15979 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/kickgroups.py
--rw-r--r--   0 runner    (1001) docker     (121)    15642 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/lsa_to_madx.py
--rw-r--r--   0 runner    (1001) docker     (121)    19285 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/machine_settings_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:11:53.000000 pylhc-0.7.4/pylhc/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-10-19 16:11:30.000000 pylhc-0.7.4/pylhc/utils/tfs_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:11:53.000000 pylhc-0.7.4/pylhc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4164 2022-10-19 16:11:53.000000 pylhc-0.7.4/pylhc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-19 16:11:53.000000 pylhc-0.7.4/pylhc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 16:11:53.000000 pylhc-0.7.4/pylhc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-10-19 16:11:53.000000 pylhc-0.7.4/pylhc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-19 16:11:53.000000 pylhc-0.7.4/pylhc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-10-19 16:11:53.000000 pylhc-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2878 2022-10-19 16:11:30.000000 pylhc-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:04:49.230069 pylhc-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 16:04:24.000000 pylhc-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-04-27 16:04:49.230069 pylhc-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-27 16:04:24.000000 pylhc-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:04:49.226069 pylhc-0.8.0/pylhc/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/bpm_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/bsrt_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/bsrt_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:04:49.230069 pylhc-0.8.0/pylhc/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/calibration/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/calibration/dispersion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:04:49.230069 pylhc-0.8.0/pylhc/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/constants/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/constants/forced_da_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/constants/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/constants/kickgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/constants/machine_settings_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:04:49.230069 pylhc-0.8.0/pylhc/data_extract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/data_extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15236 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/data_extract/lsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/data_extract/timber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51234 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/forced_da_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15979 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/kickgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15642 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/lsa_to_madx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-04-27 16:04:24.000000 pylhc-0.8.0/pylhc/machine_settings_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:04:49.230069 pylhc-0.8.0/pylhc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-04-27 16:04:49.000000 pylhc-0.8.0/pylhc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-27 16:04:49.000000 pylhc-0.8.0/pylhc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:04:49.000000 pylhc-0.8.0/pylhc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-27 16:04:49.000000 pylhc-0.8.0/pylhc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 16:04:49.000000 pylhc-0.8.0/pylhc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-27 16:04:49.230069 pylhc-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-27 16:04:24.000000 pylhc-0.8.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pylhc-0.7.4/LICENSE` & `pylhc-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/PKG-INFO` & `pylhc-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylhc
-Version: 0.7.4
+Version: 0.8.0
 Summary: An accelerator physics script collection for the OMC team at CERN.
 Home-page: https://github.com/pylhc/pylhc
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylhc-0.7.4/README.md` & `pylhc-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/pylhc/bpm_calibration.py` & `pylhc-0.8.0/pylhc/bpm_calibration.py`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/pylhc/bsrt_analysis.py` & `pylhc-0.8.0/pylhc/bsrt_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import parse
 import pytz
+
 import tfs
 from generic_parser import EntryPointParameters, entrypoint
 from omc3.utils import logging_tools, time_tools
-
 from pylhc.constants.general import TFS_SUFFIX, TIME_COLUMN
+from pylhc.forced_da_analysis import get_approximate_index
 
 LOG = logging_tools.get_logger(__name__)
 PLOT_FILE_SUFFIX = ".pdf"
 BSRT_FESA_TIME_FORMAT = "%Y/%m/%d %H:%M:%S.%f"
 OLD_FILENAMING_CONV = "{}-{}-{}-{}-{}-{}.{}"
 NEW_FILENAMING_CONV = "{}_{}_{}@{}_{}_{}_{}"
 
@@ -146,15 +147,15 @@
         assert opt["endtime"] >= opt["starttime"]
 
     indices = []
     for time, fct in zip(
         [opt["starttime"], opt["endtime"]], ["first_valid_index", "last_valid_index"]
     ):
         indices.append(
-            _get_closest_index(files_df, time if time is not None else getattr(files_df, fct)())
+            get_approximate_index(files_df, time if time is not None else getattr(files_df, fct)())
         )
 
     return files_df.iloc[indices[0] : indices[1] + 1]
 
 
 def _load_files_in_df(opt):
     files_df = pd.DataFrame(
@@ -174,18 +175,14 @@
     )
     files_df = files_df.assign(TIME=[f.timestamp() for f in files_df["TIMESTAMP"]])
 
     files_df = files_df.sort_values(by=["TIME"]).reset_index(drop=True).set_index("TIME")
     return files_df
 
 
-def _get_closest_index(df, time):
-    return df.index.get_loc(time, method="nearest")
-
-
 def _get_timestamp_from_name(name, formatstring):
     year, month, day, hour, minute, second, microsecond = map(int, parse.parse(formatstring, name))
     return datetime.datetime(
         year, month, day, hour, minute, second, microsecond, tzinfo=pytz.timezone("UTC")
     )
 
 
@@ -199,20 +196,19 @@
     return entry
 
 
 def _load_pickled_data(opt, files_df):
     merged_df = pd.DataFrame()
     for bsrtfile in files_df["FILES"]:
         data = pickle.load(gzip.open(bsrtfile, "rb"))
-        for entry in data:
-            entry = _check_and_fix_entries(entry)
-            merged_df = merged_df.append(entry, ignore_index=True)
+        new_df = pd.DataFrame.from_records([_check_and_fix_entries(entry) for entry in data])
+        merged_df = pd.concat([merged_df, new_df], axis="index", ignore_index=True)
 
     merged_df = merged_df.set_index(
-        pd.to_datetime(merged_df["acqTime"], format=BSRT_FESA_TIME_FORMAT)
+        pd.to_datetime(merged_df["acqTime"], format=BSRT_FESA_TIME_FORMAT, utc=True)
     )
     merged_df.index.name = "TimeIndex"
     merged_df = merged_df.drop_duplicates(subset=["acqCounter", "acqTime"])
     if opt.outputdir is not None:
         merged_df.to_csv(Path(opt.outputdir, _get_bsrt_tfs_fname(opt.beam)))
 
     return merged_df
@@ -359,15 +355,15 @@
 
 def plot_crosssection_for_timesteps(opt, bsrt_df):
     kick_df = opt["kick_df"]
     figlist = []
     for idx, _ in kick_df.iterrows():
         timestamp = pd.to_datetime(time_tools.cern_utc_string_to_utc(idx))
 
-        data_row = bsrt_df.iloc[_get_closest_index(bsrt_df, timestamp)]
+        data_row = bsrt_df.iloc[get_approximate_index(bsrt_df, timestamp)]
         fig, ax = plt.subplots(nrows=1, ncols=3, figsize=(18, 9), constrained_layout=True)
 
         fig.suptitle(f"Timestamp: {timestamp}")
 
         ax[0].imshow(_reshaped_imageset(data_row), cmap="hot", interpolation="nearest")
         ax[0].set_title(f"2D Pixel count")
```

### Comparing `pylhc-0.7.4/pylhc/bsrt_logger.py` & `pylhc-0.8.0/pylhc/bsrt_logger.py`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/pylhc/calibration/beta.py` & `pylhc-0.8.0/pylhc/calibration/beta.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
         # Get the factors and put them all together to have all ips in one
         # Series
         c_fit = _get_factors_from_phase(beta_phase_fit, beta_amp_tfs.reindex(BPMS[ip][beam]), plane)
         if calibration_phase_fit is None:
             calibration_phase_fit = c_fit
         else:
-            calibration_phase_fit = calibration_phase_fit.append(c_fit)
+            calibration_phase_fit = pd.concat([calibration_phase_fit, c_fit], axis="index")
 
     # Change the colum names for _fit
     calibration_phase_fit.columns = (LABELS[3], LABELS[4])
 
     return calibration_phase_fit
```

### Comparing `pylhc-0.7.4/pylhc/calibration/dispersion.py` & `pylhc-0.8.0/pylhc/calibration/dispersion.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,10 +218,10 @@
         )
         factors_for_ip.columns = LABELS
         factors_for_ip.index.name = TFS_INDEX
 
         if "X" not in calibration_factors.keys():
             calibration_factors = {"X": factors_for_ip}
         else:
-            calibration_factors["X"] = calibration_factors["X"].append(factors_for_ip)
+            calibration_factors["X"] = pd.concat([calibration_factors["X"], factors_for_ip], axis="index")
 
     return calibration_factors
```

### Comparing `pylhc-0.7.4/pylhc/constants/calibration.py` & `pylhc-0.8.0/pylhc/constants/calibration.py`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/pylhc/constants/forced_da_analysis.py` & `pylhc-0.8.0/pylhc/constants/forced_da_analysis.py`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/pylhc/constants/general.py` & `pylhc-0.8.0/pylhc/constants/general.py`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/pylhc/constants/kickgroups.py` & `pylhc-0.8.0/pylhc/constants/kickgroups.py`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/pylhc/constants/machine_settings_info.py` & `pylhc-0.8.0/pylhc/constants/machine_settings_info.py`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/pylhc/data_extract/lsa.py` & `pylhc-0.8.0/pylhc/data_extract/lsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,17 @@
             # In the past this happened, when a knob was not defined, but
             # this should have been caught by the filter_existing_knobs above
             raise ValueError(f"Something went wrong when extracting trims for the knobs: {knobs}") from e
 
         LOG.debug(f"{len(trims)} trims extracted.")
         trims_not_found = [k for k in knobs if k not in trims.keys()]
         if len(trims_not_found):
-            LOG.warning(f"The following knobs were not found in '{beamprocess}': {trims_not_found}")
+            LOG.warning(
+                f"The following knobs were not found in '{beamprocess}' "
+                f"or had no trims during the given time: {trims_not_found}")
         return trims
 
     def get_beamprocess_info(self, beamprocess: Union[str, object]) -> Dict:
         """
         Get context info of the given beamprocess.
 
         Args:
```

### Comparing `pylhc-0.7.4/pylhc/data_extract/timber.py` & `pylhc-0.8.0/pylhc/data_extract/timber.py`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/pylhc/forced_da_analysis.py` & `pylhc-0.8.0/pylhc/forced_da_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -865,15 +865,15 @@
     col_nemittance = column_norm_emittance(plane)
     cols_emitt = [mean_col(col_nemittance), err_col(mean_col(col_nemittance))]
     cols_kick = [col_nemittance, err_col(col_nemittance)]
 
     kick_df = kick_df.reindex(columns=kick_df.columns.tolist() + cols_kick)
     idx_emitt = [emittance_df.columns.get_loc(c) for c in cols_emitt]
     for time in kick_df.index:
-        idx_kick = emittance_df.index.get_loc(time, method="nearest")
+        idx_kick = get_approximate_index(emittance_df, time)
         kick_df.loc[time, cols_kick] = emittance_df.iloc[idx_kick, idx_emitt].values
 
     # add de-normalized emittance
     normalization = get_proton_gamma(energy) * get_proton_beta(
         energy
     )  # norm emittance to emittance
     col_emittance = column_emittance(plane)
@@ -1048,16 +1048,18 @@
     fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(16.80, 7.68))
 
     x_span = (kick_df.index.max() - kick_df.index.min()).seconds * np.array(
         [0.03, 0.09]
     )  # defines x-limits
 
     # convert to % relative to before first kick
-    idx_before = intensity_df.index.get_loc(
-        kick_df.index.min() - pd.Timedelta(seconds=x_span[0]), method="ffill"
+    idx_before = get_approximate_index(
+        intensity_df,
+        kick_df.index.min() - pd.Timedelta(seconds=x_span[0]),
+        method="ffill"
     )
     idx_intensity = intensity_df.columns.get_loc(INTENSITY)  # for iloc
     intensity_start = intensity_df.iloc[idx_before, idx_intensity]
     norm = intensity_start / 100.0
 
     # plot intensity
     ax.plot(
@@ -1354,14 +1356,19 @@
     fit_min = fit_fun(da - da_err, data) * multiplier
     fit_max = fit_fun(da + da_err, data) * multiplier
     return fit_mean, fit_min, fit_max
 
 
 # Helper ---
 
+def get_approximate_index(df, item, method="nearest"):
+    """ Emulates the `get_loc` from pandas<2.0, i.e.
+    single index input and output. """
+    return df.index.get_indexer([item], method=method)[0]
+
 
 def _plot_kicks_and_scale_x(ax, kick_times, pad=20):
     lines.plot_vertical_lines_fast(
         ax, kick_times, color="grey", linestyle="--", alpha=0.8, marker="", label="Kicks"
     )
 
     first_kick, last_kick = kick_times.min(), kick_times.max()
```

### Comparing `pylhc-0.7.4/pylhc/kickgroups.py` & `pylhc-0.8.0/pylhc/kickgroups.py`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/pylhc/lsa_to_madx.py` & `pylhc-0.8.0/pylhc/lsa_to_madx.py`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/pylhc/machine_settings_info.py` & `pylhc-0.8.0/pylhc/machine_settings_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,36 +13,40 @@
 This data is also not logged.
 
 Can be run from command line, parameters as given in :meth:`pylhc.machine_settings_info.get_info`.
 All gathered data is returned, if this function is called from python.
 
 .. code-block:: none
 
-    usage: machine_settings_info.py [-h] [--time TIME] [--start_time START_TIME]
-                                    [--knobs KNOBS [KNOBS ...]] [--accel ACCEL]
-                                    [--output_dir OUTPUT_DIR] [--knob_definitions]
-                                    [--source SOURCE] [--log]
-
-    optional arguments:
-    -h, --help            show this help message and exit
-    --time TIME           UTC Time as 'Y-m-d H:M:S.f' format or ISO.
-                          Acts as point in time or end time
-                         (if ``start_time`` is given).
-    --start_time START_TIME
-                            UTC Time as 'Y-m-d H:M:S.f' format.
-                            Defines the beginning of the time-range.
-    --knobs KNOBS [KNOBS ...]
-                            List of knobnames.
-    --accel ACCEL         Accelerator name.
-    --output_dir OUTPUT_DIR
-                            Output directory.
-    --knob_definitions    Set to extract knob definitions.
-    --source SOURCE       Source to extract data from.
-    --log                 Write summary into log
-                          (automatically done if no output path is given).
+   usage: machine_settings_info.py [-h] [--time TIME] [--start_time START_TIME]
+                                   [--knobs KNOBS [KNOBS ...]] [--accel ACCEL]
+                                   [--beamprocess BEAMPROCESS] [--output_dir OUTPUT_DIR]
+                                   [--knob_definitions] [--source SOURCE] [--log]
+
+  optional arguments:
+  -h, --help            show this help message and exit
+  --time TIME           UTC Time as 'Y-m-d H:M:S.f' or ISO format or AccDatetime object.
+                        Acts as point in time or end time (if ``start_time`` is given).
+  --start_time START_TIME
+                        UTC Time as 'Y-m-d H:M:S.f' or ISO format or AccDatetime object.
+                        Defines the beginning of the time-range.
+  --knobs KNOBS [KNOBS ...]
+                        List of knobnames. If `None` (or omitted) no knobs will be extracted.
+                        If it is just the string ``'all'``, all knobs will be extracted
+                        (can be slow). Use the string ``'default'`` for pre-defined knobs
+                        of interest.
+  --accel ACCEL         Accelerator name.
+  --beamprocess BEAMPROCESS
+                        Manual override for the Beamprocess
+                        (otherwise taken at the given ``time``)
+  --output_dir OUTPUT_DIR
+                        Output directory.
+  --knob_definitions    Set to extract knob definitions.
+  --source SOURCE       Source to extract data from.
+  --log                 Write summary into log (automatically done if no output path is given).
 
 
 :author: jdilly
 """
 from collections import OrderedDict, namedtuple
 
 import tfs
@@ -90,21 +94,26 @@
         knobs=dict(
             default=None,
             nargs="+",
             type=str,
             help="List of knobnames. "
                  "If `None` (or omitted) no knobs will be extracted. "
                  "If it is just the string ``'all'``, "
-                 "all knobs will be extracted (can be slow)."
-                 "Use the string ``'default'`` the main knobs of interest."
+                 "all knobs will be extracted (can be slow). "
+                 "Use the string ``'default'`` for pre-defined knobs of interest."
         ),
         accel=dict(
             default='lhc',
             type=str,
             help="Accelerator name."),
+        beamprocess=dict(
+            type=str,
+            help=("Manual override for the Beamprocess "
+                 "(otherwise taken at the given ``time``)")
+        ),
         output_dir=dict(
             default=None,
             type=PathOrStr,
             help="Output directory."),
         knob_definitions=dict(
             action="store_true",
             help="Set to extract knob definitions."),
@@ -121,107 +130,120 @@
 @entrypoint(_get_params(), strict=True)
 def get_info(opt) -> Dict[str, object]:
     """
     Get info about **Beamprocess**, **Optics** and **Knobs** at given time.
 
     Keyword Args:
 
-       *--Optional--*
+   *--Optional--*
+
+    - **accel** *(str)*:
+
+        Accelerator name.
+
+        default: ``lhc``
+
 
-        - **accel** *(str)*:
+    - **beamprocess** *(str)*:
 
-            Accelerator name.
+        Manual override for the Beamprocess
+        (otherwise taken at the given ``time``)
 
-            default: ``lhc``
+        default: ``None``
 
 
-        - **knob_definitions**:
+    - **knob_definitions**:
 
-            Set to extract knob definitions.
+        Set to extract knob definitions.
 
-            action: ``store_true``
+        action: ``store_true``
 
 
-        - **knobs** *(str)*:
+    - **knobs** *(str)*:
 
-            List of knobnames.
-            If `None` (or omitted) no knobs will be extracted.
-            If it is just the string ``'all'``,
-            all knobs will be extracted (can be slow).
-            Use the string ``'default'`` the main knobs of interest.
-            If this is called from python, the strings need
-            to be put as single items into a list.
+        List of knobnames.
+        If `None` (or omitted) no knobs will be extracted.
+        If it is just the string ``'all'``,
+        all knobs will be extracted (can be slow).
+        Use the string ``'default'`` for pre-defined knobs of interest.
+        If this is called from python, the strings need
+        to be put as single items into a list.
 
-            default: ``None``
+        default: ``None``
 
 
-        - **log**:
+    - **log**:
 
-            Write summary into log (automatically done if no output path is
-            given).
+        Write summary into log (automatically done if no output path is
+        given).
 
-            action: ``store_true``
+        action: ``store_true``
 
 
-        - **output_dir** *(PathOrStr)*:
+    - **output_dir** *(PathOrStr)*:
 
-            Output directory.
+        Output directory.
 
-            default: ``None``
+        default: ``None``
 
 
-        - **source** *(str)*:
+    - **source** *(str)*:
 
-            Source to extract data from.
+        Source to extract data from.
 
-            default: ``nxcals``
+        default: ``nxcals``
 
 
-        - **start_time** *(AccDatetime, str)*:
+    - **start_time** *(AccDatetime, str)*:
 
-            UTC Time as 'Y-m-d H:M:S.f' format or AccDatetime object.
-            Defines the beginning of the time-range.
+        UTC Time as 'Y-m-d H:M:S.f' format or AccDatetime object.
+        Defines the beginning of the time-range.
 
-            default: ``None``
+        default: ``None``
 
 
-        - **time** *(AccDatetime, str)*:
+    - **time** *(AccDatetime, str)*:
 
-            UTC Time as 'Y-m-d H:M:S.f' format or AccDatetime object.
-            Acts as point in time or end time (if ``start_time`` is given).
+        UTC Time as 'Y-m-d H:M:S.f' format or AccDatetime object.
+        Acts as point in time or end time (if ``start_time`` is given).
 
-            default: ``None``
+        default: ``None``
 
     Returns:
         dict: Dictionary containing the given ``time`` and ``start_time``,
         the extracted ``beamprocess``-info and ``optics``-info, the
         ``trim_histories`` and current (i.e. at given ``time``) ``trims``
         and the ``knob_definitions``, if extracted.
 
     """
     if opt.output_dir is None:
         opt.log = True
 
     acc_time, acc_start_time = _get_times(opt.time, opt.start_time, opt.accel)
-    beamprocess_info = _get_beamprocess(acc_time, opt.accel, opt.source)
+    beamprocess_info = _get_beamprocess(acc_time, opt.accel, opt.source, opt.beamprocess)
 
     optics_info, knob_definitions, trim_histories, trims = None, None, None, None
     try:
         optics_info = _get_optics(acc_time, beamprocess_info.Name, beamprocess_info.StartTime)
     except ValueError as e:
         LOG.error(str(e))
     else:
         if opt.knobs is not None:
             if len(opt.knobs) == 1 and opt.knobs[0].lower() == 'all':
                 opt.knobs = []  # will extract all knobs in get_trim_history
             if len(opt.knobs) == 1 and opt.knobs[0].lower() == 'default':
                 opt.knobs = [name2lsa(knob) for category in KNOB_CATEGORIES.values()
                              for knob in category]
 
-            trim_histories = LSA.get_trim_history(beamprocess_info.Object, opt.knobs, start_time=acc_start_time, end_time=acc_time, accelerator=opt.accel)
+            trim_histories = LSA.get_trim_history(
+                beamprocess_info.Object, opt.knobs,
+                start_time=acc_start_time,
+                end_time=acc_time,
+                accelerator=opt.accel
+            )
             trims = _get_last_trim(trim_histories)
 
         if opt.knob_definitions:
             if trim_histories:  # this now works with 'all'/`default`. Might create a lot of files
                 knob_definitions = _get_knob_definitions(trim_histories.keys(), optics_info.Name)
             else:
                 LOG.error("Writing out knob definitions requested, but no knobs extracted.")
@@ -328,25 +350,25 @@
     """Write Knob definitions into a **tfs** file."""
     for knob, definition in definitions.items():
         path = output_path / f"{knob.replace('/', '_')}{const.knobdef_suffix}"
         tfs.write(path, definition, save_index=LSA_COLUMN_NAME)
 
 
 def write_trim_histories(
-    output_path: Path, trim_hisotries: Dict[str, namedtuple], accel: str,
+    output_path: Path, trim_histories: Dict[str, namedtuple], accel: str,
     acc_time: AccDatetime = None, acc_start_time: AccDatetime = None, 
     bp_info: DotDict = None, optics_info: DotDict = None
 ):
     """ Write the trim histories into tfs files.
     There are two time columns, one with timestamps as they are usually easier to handle
-    and one with the UTC-string, as they are more human readable.
+    and one with the UTC-string, as they are more human-readable.
 
     Args:
         output_path (Path): Folder to write output file into
-        trim_hisotries (dict): trims histories as extracted via LSA.get_trim_history()
+        trim_histories (dict): trims histories as extracted via LSA.get_trim_history()
         accel (str): Name of the accelerator
         acc_time (AccDatetime): User given (End)Time
         acc_start_time (AccDatetime): User given Start Time
         bp_info (DotDict): BeamProcess Info Dictionary
         optics_info (DotDict): Optics Info Dictionary
     """
     AccDT = AcceleratorDatetime[accel]
@@ -368,15 +390,15 @@
             const.head_fill: bp_info.Fill,
         })
 
     if optics_info:
         headers.update({const.head_optics: optics_info.Name})
 
     # Write trim history per knob ----
-    for knob, trim_history in trim_hisotries.items():
+    for knob, trim_history in trim_histories.items():
         trims_tfs = tfs.TfsDataFrame(headers=headers, columns=[const.column_time, const.column_timestamp, const.column_value])
         for timestamp, value in zip(trim_history.time, trim_history.data):
             time = AccDT.from_timestamp(timestamp).cern_utc_string()
             try:
                 len(value)
             except TypeError:
                 # single value (as it should be)
@@ -390,27 +412,32 @@
         path = output_path / f"{knob.replace('/', '_')}{const.trimhistory_suffix}"
         tfs.write(path, trims_tfs)
 
 
 # Beamprocess ##################################################################
 
 
-def _get_beamprocess(acc_time: AccDatetime, accel: str, source: str) -> DotDict:
-    """Get the info about the active beamprocess at ``acc_time``."""
-    fill_no, fill_bps = LSA.find_last_fill(acc_time, accel, source)
-    beamprocess = LSA.find_active_beamprocess_at_time(acc_time)
+def _get_beamprocess(acc_time: AccDatetime, accel: str, source: str, beamprocess: str = None) -> DotDict:
+    """Get the info about the active beamprocess at ``acc_time`` or the given one."""
+    if beamprocess is None:
+        beamprocess = LSA.find_active_beamprocess_at_time(acc_time, accelerator=accel)
+    bp_info = LSA.get_beamprocess_info(beamprocess)
+    bp_info = DotDict(bp_info)
+
+    fill_no, fill_bps = LSA.find_last_fill(acc_time, accelerator=accel, source=source)
+    bp_info.Fill = fill_no
+
     try:
-        start_time = _get_beamprocess_start(fill_bps, acc_time, str(beamprocess))
+        start_time = _get_beamprocess_start(fill_bps, acc_time, bp_info.Name)
     except ValueError as e:
         raise ValueError(f"In fill {fill_no} the {str(e)}") from e
-    bp_info = LSA.get_beamprocess_info(beamprocess)
-    bp_info.update({"Fill": fill_no, "StartTime": start_time})
+    bp_info.StartTime = start_time
+
     LOG.debug(
-        f"Beamprocess {bp_info['Name']} in fill {fill_no}"
-        f" extracted at time {start_time}."
+        f"Beamprocess {bp_info.Name} in fill {bp_info.Fill} started at time {bp_info.StartTime}."
     )
     return DotDict(bp_info)
 
 
 def _get_beamprocess_start(beamprocesses: Iterable[Tuple[float, str]], acc_time: AccDatetime, bp_name: str) -> AccDatetime:
     """
     Get the last beamprocess in the list of beamprocesses before dt_utc.
```

### Comparing `pylhc-0.7.4/pylhc.egg-info/PKG-INFO` & `pylhc-0.8.0/pylhc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylhc
-Version: 0.7.4
+Version: 0.8.0
 Summary: An accelerator physics script collection for the OMC team at CERN.
 Home-page: https://github.com/pylhc/pylhc
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylhc-0.7.4/pylhc.egg-info/SOURCES.txt` & `pylhc-0.8.0/pylhc.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -22,10 +22,8 @@
 pylhc/constants/calibration.py
 pylhc/constants/forced_da_analysis.py
 pylhc/constants/general.py
 pylhc/constants/kickgroups.py
 pylhc/constants/machine_settings_info.py
 pylhc/data_extract/__init__.py
 pylhc/data_extract/lsa.py
-pylhc/data_extract/timber.py
-pylhc/utils/__init__.py
-pylhc/utils/tfs_tools.py
+pylhc/data_extract/timber.py
```

### Comparing `pylhc-0.7.4/pylhc.egg-info/requires.txt` & `pylhc-0.8.0/pylhc.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pylhc-0.7.4/setup.py` & `pylhc-0.8.0/setup.py`

 * *Files identical despite different names*


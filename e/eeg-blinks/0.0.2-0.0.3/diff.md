# Comparing `tmp/eeg_blinks-0.0.2.tar.gz` & `tmp/eeg_blinks-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eeg_blinks-0.0.2.tar", last modified: Sat Feb 18 14:36:20 2023, max compression
+gzip compressed data, was "eeg_blinks-0.0.3.tar", last modified: Thu Apr 27 08:53:08 2023, max compression
```

## Comparing `eeg_blinks-0.0.2.tar` & `eeg_blinks-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-02-18 14:36:20.407451 eeg_blinks-0.0.2/
--rw-rw-rw-   0        0        0      134 2023-02-18 14:36:20.404430 eeg_blinks-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-02-02 14:26:36.000000 eeg_blinks-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-18 14:36:20.387462 eeg_blinks-0.0.2/eeg_blinks/
--rw-rw-rw-   0        0        0      100 2023-02-02 14:26:36.000000 eeg_blinks-0.0.2/eeg_blinks/__init__.py
--rw-rw-rw-   0        0        0      131 2023-02-02 14:26:36.000000 eeg_blinks-0.0.2/eeg_blinks/_version.py
--rw-rw-rw-   0        0        0     1228 2023-02-02 14:26:36.000000 eeg_blinks-0.0.2/eeg_blinks/default_setting.py
--rw-rw-rw-   0        0        0     3332 2023-02-04 03:21:16.000000 eeg_blinks-0.0.2/eeg_blinks/pyblinker.py
-drwxrwxrwx   0        0        0        0 2023-02-18 14:36:20.404430 eeg_blinks-0.0.2/eeg_blinks/utilities/
--rw-rw-rw-   0        0        0       17 2023-02-02 14:26:36.000000 eeg_blinks-0.0.2/eeg_blinks/utilities/__init__.py
--rw-rw-rw-   0        0        0    11489 2023-02-04 02:49:53.000000 eeg_blinks-0.0.2/eeg_blinks/utilities/extractBlinkProperties.py
--rw-rw-rw-   0        0        0     3019 2023-02-03 16:46:39.000000 eeg_blinks-0.0.2/eeg_blinks/utilities/fit_blink.py
--rw-rw-rw-   0        0        0     5969 2023-02-04 02:11:07.000000 eeg_blinks-0.0.2/eeg_blinks/utilities/getCandidateSignal.py
--rw-rw-rw-   0        0        0     1573 2023-02-02 14:26:36.000000 eeg_blinks-0.0.2/eeg_blinks/utilities/misc.py
--rw-rw-rw-   0        0        0    19452 2023-02-04 03:19:30.000000 eeg_blinks-0.0.2/eeg_blinks/utilities/zero_crossing.py
-drwxrwxrwx   0        0        0        0 2023-02-18 14:36:20.395887 eeg_blinks-0.0.2/eeg_blinks.egg-info/
--rw-rw-rw-   0        0        0      134 2023-02-18 14:36:20.000000 eeg_blinks-0.0.2/eeg_blinks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-02-18 14:36:20.000000 eeg_blinks-0.0.2/eeg_blinks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-18 14:36:20.000000 eeg_blinks-0.0.2/eeg_blinks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-02-18 14:36:20.000000 eeg_blinks-0.0.2/eeg_blinks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-18 14:36:20.407451 eeg_blinks-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      266 2023-02-18 14:32:24.000000 eeg_blinks-0.0.2/setup.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      127 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/PKG-INFO
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      540 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/README.md
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/eeg_blinks/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       94 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      125 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/_version.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     1196 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/default_setting.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     3252 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/pyblinker.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/eeg_blinks/utilities/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       16 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)    11250 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/extractBlinkProperties.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2976 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/fit_blink.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     5828 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/getCandidateSignal.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     1526 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/misc.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)    18968 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/zero_crossing.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/eeg_blinks/vislab/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/vislab/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      916 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/vislab/base_left_right.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2590 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/vislab/blink_posi_vislab.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2677 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/vislab/getBlinkPositions_vislab.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/eeg_blinks/viz/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/viz/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2932 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/viz/viz_pd.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     3580 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/viz/viz_sanity.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/eeg_blinks.egg-info/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      127 2023-04-27 08:53:08.000000 eeg_blinks-0.0.3/eeg_blinks.egg-info/PKG-INFO
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      744 2023-04-27 08:53:08.000000 eeg_blinks-0.0.3/eeg_blinks.egg-info/SOURCES.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        1 2023-04-27 08:53:08.000000 eeg_blinks-0.0.3/eeg_blinks.egg-info/dependency_links.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        8 2023-04-27 08:53:08.000000 eeg_blinks-0.0.3/eeg_blinks.egg-info/requires.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       11 2023-04-27 08:53:08.000000 eeg_blinks-0.0.3/eeg_blinks.egg-info/top_level.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       38 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/setup.cfg
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      349 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/setup.py
```

### Comparing `eeg_blinks-0.0.2/README.md` & `eeg_blinks-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# pyblinker
-Tools for analyzing eye blinks from EEG data. This is Python alternative to the EEG-Blinks Matlab version that has been maintained by Vislab (https://github.com/VisLab/EEG-Blinks).
-
-The package documentation is accessable at: http://vislab.github.io/EEG-Blinks/.
-
-Due deligent has been made to ensure the EEG-Blinks-Python output similar result as the EEG-Blinks Matlab version.
-
-In future version, this package is expected to able to handle both continous and epoch EEG signal.
-
-# Installation
-
-pip install eeg-blinks==0.0.1
-
-
+# pyblinker
+Tools for analyzing eye blinks from EEG data. This is Python alternative to the EEG-Blinks Matlab version that has been maintained by Vislab (https://github.com/VisLab/EEG-Blinks).
+
+The package documentation is accessable at: http://vislab.github.io/EEG-Blinks/.
+
+Due deligent has been made to ensure the EEG-Blinks-Python output similar result as the EEG-Blinks Matlab version.
+
+In future version, this package is expected to able to handle both continous and epoch EEG signal.
+
+# Installation
+
+pip install eeg-blinks==0.0.1
+
+
```

### Comparing `eeg_blinks-0.0.2/eeg_blinks/default_setting.py` & `eeg_blinks-0.0.3/eeg_blinks/default_setting.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import numpy as np
-
-params = {'stdThreshold': 1.50,
-          'minEventLen': 0.05,
-          'minEventSep': 0.05,
-          'correlationThresholdTop': 0.980,
-          'correlationThresholdBottom': 0.90,
-          'params_blinkAmpRange_1': 0,
-          'params_blinkAmpRange_2': 4,
-          'params_goodRatioThreshold': 0.7,
-          'params_minGoodBlinks': 10,
-          'params_keepSignals': 0,
-          'correlationThreshold': 0.98}
-
-
-
-# def getHeader ():
-#     header = ['mean', 'median', 'std',
-#               'mad', 'goodMean', 'goodMedian',
-#               'goodStd', 'goodMad']
-#     return dict ( zip ( header, [np.nan] * len ( header ) ) )
-#
-#
-# def getStatisticsStructure ():
-#     list_detail = ['subjectID', 'task', 'uniqueName',
-#                    'srate', 'startTime', 'usedNumber',
-#                    'usedLabel', 'status', 'seconds',
-#                    'numberBlinks','numberGoodBlinks',
-#                    'goodRatio', 'header', 'pAVRZ',
-#                    'nAVRZ', 'durationZ', 'durationB',
-#                    'durationT', 'durationHZ',
-#                    'durationHB', 'blinksPerMin']
+import numpy as np
+
+params = {'stdThreshold': 1.50,
+          'minEventLen': 0.05,
+          'minEventSep': 0.05,
+          'correlationThresholdTop': 0.980,
+          'correlationThresholdBottom': 0.90,
+          'params_blinkAmpRange_1': 0,
+          'params_blinkAmpRange_2': 4,
+          'params_goodRatioThreshold': 0.7,
+          'params_minGoodBlinks': 10,
+          'params_keepSignals': 0,
+          'correlationThreshold': 0.98}
+
+
+
+# def getHeader ():
+#     header = ['mean', 'median', 'std',
+#               'mad', 'goodMean', 'goodMedian',
+#               'goodStd', 'goodMad']
+#     return dict ( zip ( header, [np.nan] * len ( header ) ) )
+#
+#
+# def getStatisticsStructure ():
+#     list_detail = ['subjectID', 'task', 'uniqueName',
+#                    'srate', 'startTime', 'usedNumber',
+#                    'usedLabel', 'status', 'seconds',
+#                    'numberBlinks','numberGoodBlinks',
+#                    'goodRatio', 'header', 'pAVRZ',
+#                    'nAVRZ', 'durationZ', 'durationB',
+#                    'durationT', 'durationHZ',
+#                    'durationHB', 'blinksPerMin']
 #     return dict ( zip ( list_detail, [np.nan] * len ( list_detail ) ) )
```

### Comparing `eeg_blinks-0.0.2/eeg_blinks/pyblinker.py` & `eeg_blinks-0.0.3/eeg_blinks/pyblinker.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import logging
-
-import pandas as pd
-
-from eeg_blinks import default_setting
-from eeg_blinks.vislab.blink_posi_vislab import BlinkFrameValley
-from eeg_blinks.utilities.extractBlinkProperties import BlinkProperties
-from eeg_blinks.utilities.fit_blink import FitBlinks
-from eeg_blinks.utilities.getCandidateSignal import PrepareSelection,ChannelSelection
-from eeg_blinks.utilities.misc import create_annotation
-from eeg_blinks.viz.viz_pd import viz_complete_blink_prop
-
-logging.getLogger().setLevel(logging.INFO)
-
-
-class BlinkDetector:
-    def __init__(self, raw_data, visualize=False, annot_label=None,filter_bad=False):
-        self.filter_bad=filter_bad
-        self.raw_data = raw_data
-        self.viz_data = visualize
-        self.annot_label = annot_label
-        self.sfreq = self.raw_data.info['sfreq']
-        self.params = default_setting.params
-        self.channel_list = self.raw_data.ch_names
-        self.all_data_info = []
-        self.all_data = []
-
-    def prepare_raw_signal(self):
-        self.raw_data.pick_types(eeg=True)
-        self.raw_data.filter(0.5, 20.5, fir_design='firwin')
-        self.raw_data.resample(100)
-        return self.raw_data
-
-    def process_channel_data(self, channel):
-
-        df = BlinkFrameValley(self.raw_data.get_data(picks=channel)[0], self.sfreq, self.params, channel, self.sfreq).blink_frame
-        df = FitBlinks(data=self.raw_data.get_data(picks=channel)[0], df=df).frame_blinks
-        # df = extracBlinkProperties(self.raw_data.get_data(picks=channel)[0], df, self.sfreq)
-        df=BlinkProperties(self.raw_data.get_data(picks=channel)[0], df, self.sfreq).df_res
-        d = PrepareSelection(signal=self.raw_data.get_data(picks=channel)[0], df=df, params=self.params, ch=channel).get_param_for_selection()
-        self.all_data_info.append(dict(df=df, ch=channel))
-        self.all_data.append(d)
-
-    @staticmethod
-    def filter_point(ch,all_data_info):
-        return list(filter(lambda all_data_info: all_data_info['ch'] == ch, all_data_info))[0]
-
-
-    def filter_bad_blink(self,df):
-        # filter_bad = False
-        if self.filter_bad:
-            df = df[df['blink_quality'] == 'Good']
-        return df
-
-
-    def generate_viz(self,data,df):
-        fig_data = [viz_complete_blink_prop(data, row, self.sfreq) for index, row in df.iterrows()]
-
-        return fig_data
-    def get_blink_stat(self):
-        for channel in self.channel_list:
-            self.process_channel_data(channel)
-
-        ch_blink_stat = pd.DataFrame(self.all_data)
-        ch_selected = ChannelSelection(df=ch_blink_stat, params=self.params).df
-        ch = ch_selected.loc[0, 'ch']
-        nGoodBlinks = ch_selected.loc[0, 'numberGoodBlinks']
-        data = self.raw_data.get_data(picks=ch)[0]
-        rep_blink_channel = self.filter_point(ch,self.all_data_info)
-        df = rep_blink_channel['df']
-
-        df=self.filter_bad_blink(df)
-        # df.to_pickle('unit_test_1.pkl')
-
-        annot_description = self.annot_label if self.annot_label else 'eye_blink'
-        annot = create_annotation(df, self.sfreq, annot_description)
-        if self.viz_data:
-            fig_data=self.generate_viz(self,data,df)
-            return annot, ch, nGoodBlinks, fig_data, df
-
+import logging
+
+import pandas as pd
+
+from eeg_blinks import default_setting
+from eeg_blinks.vislab.blink_posi_vislab import BlinkFrameValley
+from eeg_blinks.utilities.extractBlinkProperties import BlinkProperties
+from eeg_blinks.utilities.fit_blink import FitBlinks
+from eeg_blinks.utilities.getCandidateSignal import PrepareSelection,ChannelSelection
+from eeg_blinks.utilities.misc import create_annotation
+from eeg_blinks.viz.viz_pd import viz_complete_blink_prop
+
+logging.getLogger().setLevel(logging.INFO)
+
+
+class BlinkDetector:
+    def __init__(self, raw_data, visualize=False, annot_label=None,filter_bad=False):
+        self.filter_bad=filter_bad
+        self.raw_data = raw_data
+        self.viz_data = visualize
+        self.annot_label = annot_label
+        self.sfreq = self.raw_data.info['sfreq']
+        self.params = default_setting.params
+        self.channel_list = self.raw_data.ch_names
+        self.all_data_info = []
+        self.all_data = []
+
+    def prepare_raw_signal(self):
+        self.raw_data.pick_types(eeg=True)
+        self.raw_data.filter(0.5, 20.5, fir_design='firwin')
+        self.raw_data.resample(100)
+        return self.raw_data
+
+    def process_channel_data(self, channel):
+
+        df = BlinkFrameValley(self.raw_data.get_data(picks=channel)[0], self.sfreq, self.params, channel, self.sfreq).blink_frame
+        df = FitBlinks(data=self.raw_data.get_data(picks=channel)[0], df=df).frame_blinks
+        # df = extracBlinkProperties(self.raw_data.get_data(picks=channel)[0], df, self.sfreq)
+        df=BlinkProperties(self.raw_data.get_data(picks=channel)[0], df, self.sfreq).df_res
+        d = PrepareSelection(signal=self.raw_data.get_data(picks=channel)[0], df=df, params=self.params, ch=channel).get_param_for_selection()
+        self.all_data_info.append(dict(df=df, ch=channel))
+        self.all_data.append(d)
+
+    @staticmethod
+    def filter_point(ch,all_data_info):
+        return list(filter(lambda all_data_info: all_data_info['ch'] == ch, all_data_info))[0]
+
+
+    def filter_bad_blink(self,df):
+        # filter_bad = False
+        if self.filter_bad:
+            df = df[df['blink_quality'] == 'Good']
+        return df
+
+
+    def generate_viz(self,data,df):
+        fig_data = [viz_complete_blink_prop(data, row, self.sfreq) for index, row in df.iterrows()]
+
+        return fig_data
+    def get_blink_stat(self):
+        for channel in self.channel_list:
+            self.process_channel_data(channel)
+
+        ch_blink_stat = pd.DataFrame(self.all_data)
+        ch_selected = ChannelSelection(df=ch_blink_stat, params=self.params).df
+        ch = ch_selected.loc[0, 'ch']
+        nGoodBlinks = ch_selected.loc[0, 'numberGoodBlinks']
+        data = self.raw_data.get_data(picks=ch)[0]
+        rep_blink_channel = self.filter_point(ch,self.all_data_info)
+        df = rep_blink_channel['df']
+
+        df=self.filter_bad_blink(df)
+        # df.to_pickle('unit_test_1.pkl')
+
+        annot_description = self.annot_label if self.annot_label else 'eye_blink'
+        annot = create_annotation(df, self.sfreq, annot_description)
+        if self.viz_data:
+            fig_data=self.generate_viz(self,data,df)
+            return annot, ch, nGoodBlinks, fig_data, df
+
         return annot, ch, nGoodBlinks,df
```

### Comparing `eeg_blinks-0.0.2/eeg_blinks/utilities/extractBlinkProperties.py` & `eeg_blinks-0.0.3/eeg_blinks/utilities/extractBlinkProperties.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,239 +1,239 @@
-import logging
-
-import numpy as np
-import pandas as pd
-
-from eeg_blinks.utilities.misc import mad_matlab
-
-logging.getLogger().setLevel(logging.INFO)
-
-
-def _goodblink_based_corr_median_std(df, correlationThreshold):
-    R2 = df['leftR2'] >= correlationThreshold
-    R3 = df['rightR2'] >= correlationThreshold
-
-    # Now calculate the cutoff ratios -- use default for the values
-    good_data = df.loc[R2.values & R3.values, :]
-    bestValues = good_data['maxValues'].array
-
-    specifiedMedian = np.nanmedian(bestValues)
-    specifiedStd = 1.4826 * mad_matlab(bestValues)
-
-    return R2, R3, specifiedMedian, specifiedStd
-
-
-def get_mask_optimise(df, indicesNaN, correlationThreshold, zScoreThreshold):
-    """
-    "used Feb 02 2023"
-    The calculation of bestmedian,worst median, worrst rbobustst
-    is from https://github.com/VisLab/EEG-Blinks/blob/16b6ea04101ecfa74fb1c9cbceb037324572687e/blinker/utilities/extractBlinks.m#L97
-
-    :param df:
-    :param indicesNaN:
-    :param correlationThreshold:
-    :param zScoreThreshold:
-    :return:
-    """
-    R1 = ~indicesNaN
-    R2, R3, specifiedMedian, specifiedStd = _goodblink_based_corr_median_std(df, correlationThreshold)
-
-    R4 = df['maxValues'] >= max(0, specifiedMedian - zScoreThreshold * specifiedStd)
-    R5 = df['maxValues'] <= specifiedMedian + zScoreThreshold * specifiedStd
-    bool_test = R1.values & R2.values & R3.values & R4.values & R5.values
-
-    return bool_test, specifiedMedian, specifiedStd
-
-
-def getGoodBlinkMask(df, zThresholds):
-    "used Feb 02 2023"
-    ## These is the default value
-    correlationThreshold_s1, correlationThreshold_s2, zScoreThreshold_s1, zScoreThreshold_s2 = zThresholds
-
-    df['rightR2'] = df['rightR2'].abs()
-    df_data = df[['leftR2', 'rightR2', 'maxValues']]
-
-    indicesNaN = df_data.isnull().any(1)
-
-    ### GET MASK OPTIMISE
-
-    goodMaskTop_bool, bestMedian, bestRobustStd = get_mask_optimise(df_data, indicesNaN, correlationThreshold_s1,
-                                                                    zScoreThreshold_s1)
-
-    df_s2_bool, worstMedian, worstRobustStd = get_mask_optimise(df_data, indicesNaN, correlationThreshold_s2,
-                                                                zScoreThreshold_s2)
-
-    goodBlinkMask = np.reshape(goodMaskTop_bool | df_s2_bool, (-1, 1))  # Get any TRUE
-    df['blink_quality'] = 'Good'
-    df[['blink_quality']] = df[['blink_quality']].where(goodBlinkMask, other='Reject')
-    return df, bestMedian, bestRobustStd
-
-
-
-
-class BlinkProperties:
-    '''
-    Return a structure with blink shapes and properties for individual blinks
-    '''
-    def __init__(self, data, df, srate):
-        self.data = data
-        self.df = df
-        self.srate = srate
-        self.shutAmpFraction = 0.9
-        self.pAVRThreshold = 3
-        self.zThresholds = (0.90, 0.98, 2, 5)
-        self.df_res=[]
-        self.reset_index()
-        self.get_good_blink_mask()
-        self.set_blink_velocity()
-        self.set_blink_duration()
-        self.set_blink_amp_velocity_ratio_zero_to_max()
-        self.amplitude_velocity_ratio_base()
-        self.amplitude_velocity_ratio_tent()
-        self.time_zero_shut()
-        self.time_base_shut()
-        self.extract_other_times()
-
-    def reset_index(self):
-        self.df.reset_index(drop=True, inplace=True)
-
-    def get_good_blink_mask(self):
-        self.df, self.bestMedian, self.bestRobustStd = getGoodBlinkMask(self.df, self.zThresholds)
-
-    def set_blink_velocity(self):
-        self.signal_l = self.data.shape[0]
-        self.blinkVelocity = np.diff(self.data)
-
-    def set_blink_duration(self):
-        cols_int = ['rightBase']
-        self.df[cols_int] = self.df[cols_int].astype(int)
-        self.df['durationBase'] = (self.df['rightBase'] - self.df['leftBase']) / self.srate
-        self.df['durationTent'] = (self.df['rightXIntercept'] - self.df['leftXIntercept']) / self.srate
-        self.df['durationZero'] = (self.df['rightZero'] - self.df['leftZero']) / self.srate
-        self.df['durationHalfBase'] = (self.df['rightBaseHalfHeight'] - self.df['leftBaseHalfHeight'] + 1) / self.srate
-        self.df['durationHalfZero'] = (self.df['rightZeroHalfHeight'] - self.df['leftZeroHalfHeight'] + 1) / self.srate
-
-    def set_blink_amp_velocity_ratio_zero_to_max(self):
-        self.df[['leftZero', 'rightZero']] = self.df[['leftZero', 'rightZero']].astype(int)
-        self.df['peaksPosVelZero'] = self.df.apply(lambda x: x['leftZero'] + np.argmax(self.blinkVelocity[x['leftZero']:x['maxFrames'] + 1]), axis=1)
-        self.df['RRC'] = self.data[self.df['maxFrames'] - 1] / self.blinkVelocity[self.df['peaksPosVelZero']]
-        self.df['posAmpVelRatioZero'] = (100 * abs(self.df['RRC'])) / self.srate
-        self.df['downStrokevelFrame_del'] = self.df.apply(lambda x: x['maxFrames'] + np.argmin(self.blinkVelocity[x['maxFrames']:x['rightZero'] + 1]), axis=1)
-        self.df['TTT'] = self.data[self.df['maxFrames'] - 1] / self.blinkVelocity[self.df['downStrokevelFrame_del']]
-        self.df['negAmpVelRatioZero'] = (100 * abs(self.df['TTT'])) / self.srate
-
-    def amplitude_velocity_ratio_base(self):
-        self.df['peaksPosVelBase'] = self.df.apply(
-            lambda x: x['leftBase'] + np.argmax(self.blinkVelocity[x['leftBase']:x['maxFrames'] + 1]), axis=1)
-        self.df['KKK'] = self.data[self.df['maxFrames'] - 1] / self.blinkVelocity[self.df['peaksPosVelBase']]
-        self.df['posAmpVelRatioBase'] = (100 * abs(self.df['KKK'])) / self.srate
-
-        self.df['downStroke_del'] = self.df.apply(
-            lambda x: x['maxFrames'] + np.argmin(self.blinkVelocity[x['maxFrames']:x['rightBase'] + 1]), axis=1)
-        self.df['KKK'] = self.data[self.df['maxFrames'] - 1] / self.blinkVelocity[self.df['downStroke_del']]
-        self.df['negAmpVelRatioBase'] = (100 * abs(self.df['KKK'])) / self.srate
-
-    def amplitude_velocity_ratio_tent(self):
-        self.df['pop'] = self.data[self.df['maxFrames'] - 1] / self.df['averRightVelocity']
-        self.df['negAmpVelRatioTent'] = (100 * abs(self.df['pop'])) / self.srate
-
-        self.df['opi'] = self.data[self.df['maxFrames'] - 1] / self.df['averLeftVelocity']
-        self.df['WE'] = (100 * abs(self.df['opi']))
-        self.df['posAmpVelRatioTent'] = self.df['WE'] / self.srate
-
-    def time_zero_shut(self):
-        self.df['closingTimeZero'] = (self.df['maxFrames'] - self.df['leftZero']) / self.srate
-        self.df['reopeningTimeZero'] = (self.df['rightZero'] - self.df['maxFrames']) / self.srate
-
-        self.df['ampThreshhold'] = self.shutAmpFraction * self.df['maxValues']
-        self.df['start_shut_tzs'] = self.df.apply(
-            lambda x: np.argmax(self.data[x['leftZero']:x['rightZero'] + 1] >= x['ampThreshhold']), axis=1)
-
-        self.df['endShut_tzs'] = self.df.apply(
-            lambda x: np.argmax(self.data[x['leftZero']:x['rightZero'] + 1][x['start_shut_tzs'] + 1:-1] <
-                                self.shutAmpFraction * x['maxValues']), axis=1)
-
-        ## PLease expect error here, some value maybe zero or lead to empty cell
-        self.df['endShut_tzs'] = self.df['endShut_tzs'] + 1  ## temporary  to delete
-        self.df['timeShutZero'] = self.df.apply(
-            lambda x: 0 if x['endShut_tzs'] == np.isnan else x['endShut_tzs'] / self.srate, axis=1)
-    def time_base_shut(self):
-        self.df['ampThreshhold_tbs'] = self.shutAmpFraction * self.df['maxValues']
-        self.df['start_shut_tbs'] = self.df.apply(
-            lambda x: np.argmax(self.data[x['leftBase']:x['rightBase'] + 1] >= x['ampThreshhold_tbs']), axis=1)
-
-        self.df['endShut_tbs'] = self.df.apply(
-            lambda x: np.argmax(self.data[x['leftBase']:x['rightBase'] + 1][x['start_shut_tbs']:-1] <
-                                self.shutAmpFraction * x['maxValues']), axis=1)
-
-        self.df['timeShutBase'] = self.df.apply(
-            lambda x: 0 if x['endShut_tbs'] == np.isnan else (x['endShut_tbs'] / self.srate), axis=1)
-
-        ## Time shut tent
-        self.df['closingTimeTent'] = (self.df['xIntersect'] - self.df['leftXIntercept']) / self.srate
-        self.df['reopeningTimeTent'] = (self.df['rightXIntercept'] - self.df['xIntersect']) / self.srate
-
-        self.df['ampThreshhold_tst'] = self.shutAmpFraction * self.df['maxValues']
-
-        self.df[['leftXIntercept_int', 'rightXIntercept_int']] = self.df[['leftXIntercept', 'rightXIntercept']].astype(
-            int)
-
-
-        # warnings.warn('New upgrade')
-        self.df=self.df[self.df.leftXIntercept_int<self.df.rightXIntercept_int]
-        self.df.reset_index(drop=True,inplace=True)
-        self.df['start_shut_tst'] = self.df.apply(
-            lambda x: np.argmax(self.data[x['leftXIntercept_int']:x['rightXIntercept_int'] + 1] >= x['ampThreshhold']), axis=1)
-
-        self.df['endShut_tst'] = self.df.apply(
-            lambda x: np.argmax(self.data[x['leftXIntercept_int']:x['rightXIntercept_int'] + 1][x['start_shut_tst']:-1] <
-                                self.shutAmpFraction * x['maxValues']), axis=1)
-        ### Just in case got other issue, use this back, do not delete
-        ## Since we already remove imblanace left_right intercept, maybe dah xperlu kot bawah ni
-        # df['start_shut_tst'] = df.apply(
-        #     lambda x: _start_shut(data, x['leftXIntercept_int'], x['rightXIntercept_int'], x['ampThreshhold']), axis=1)
-        #
-        #
-        #
-        # df['endShut_tst'] = df.apply(
-        #     lambda x: _end_shut(data, x['leftXIntercept_int'], x['rightXIntercept_int'], x['start_shut_tst'],
-        #                         x['maxValues'], shutAmpFraction), axis=1)
-
-        self.df['timeShutTent'] = self.df.apply(
-            lambda x: 0 if x['endShut_tst'] == np.isnan else (x['endShut_tst'] / self.srate), axis=1)
-
-    def extract_other_times(self):
-        ## Other times
-        self.df['peakMaxBlink '] = self.df['maxValues']
-        self.df['peakMaxTent'] = self.df['yIntersect']
-        self.df['peakTimeTent'] = self.df['xIntersect'] / self.srate
-        self.df['peakTimeBlink'] = self.df['maxFrames'] / self.srate
-
-        dfcal = self.df[['maxFrames', 'peaksPosVelBase', 'peaksPosVelZero']]
-
-        df_t = pd.DataFrame.from_records([[self.signal_l] * 3], columns=['maxFrames', 'peaksPosVelBase', 'peaksPosVelZero'])
-
-        dfcal = pd.concat([dfcal, df_t]).reset_index(drop=True)
-
-        dfcal['ibmx'] = dfcal.maxFrames.diff().shift(-1)
-
-        dfcal['interBlinkMaxAmp'] = dfcal['ibmx'] / self.srate
-
-        dfcal['ibmvb'] = 1 - dfcal['peaksPosVelBase']
-        dfcal['interBlinkMaxVelBase'] = dfcal['ibmvb'] / self.srate  # peaksPosVelBase == velFrame
-
-        dfcal['ibmvz'] = 1 - dfcal['peaksPosVelZero']
-        dfcal['interBlinkMaxVelZero'] = dfcal['ibmvz'] / self.srate
-
-        dfcal.drop(dfcal.tail(1).index, inplace=True)  # drop last n rows# peaksPosVelZero == velFrame
-        dfnew = self.df[['maxValues', 'posAmpVelRatioZero']]
-
-        R1 = dfnew['posAmpVelRatioZero'] < self.pAVRThreshold
-
-        th_bm_brs = self.bestMedian - self.bestRobustStd
-        R2 = dfnew['maxValues'] < th_bm_brs
-        pMask = pd.concat([R1, R2], axis=1)
-        pMasks = pMask.all(1)
-        df_res = pd.merge(self.df, dfcal, on=['maxFrames'])
-        self.df_res = df_res[~pMasks].reset_index(drop=True)
-        # return df_res
-
+import logging
+
+import numpy as np
+import pandas as pd
+
+from eeg_blinks.utilities.misc import mad_matlab
+
+logging.getLogger().setLevel(logging.INFO)
+
+
+def _goodblink_based_corr_median_std(df, correlationThreshold):
+    R2 = df['leftR2'] >= correlationThreshold
+    R3 = df['rightR2'] >= correlationThreshold
+
+    # Now calculate the cutoff ratios -- use default for the values
+    good_data = df.loc[R2.values & R3.values, :]
+    bestValues = good_data['maxValues'].array
+
+    specifiedMedian = np.nanmedian(bestValues)
+    specifiedStd = 1.4826 * mad_matlab(bestValues)
+
+    return R2, R3, specifiedMedian, specifiedStd
+
+
+def get_mask_optimise(df, indicesNaN, correlationThreshold, zScoreThreshold):
+    """
+    "used Feb 02 2023"
+    The calculation of bestmedian,worst median, worrst rbobustst
+    is from https://github.com/VisLab/EEG-Blinks/blob/16b6ea04101ecfa74fb1c9cbceb037324572687e/blinker/utilities/extractBlinks.m#L97
+
+    :param df:
+    :param indicesNaN:
+    :param correlationThreshold:
+    :param zScoreThreshold:
+    :return:
+    """
+    R1 = ~indicesNaN
+    R2, R3, specifiedMedian, specifiedStd = _goodblink_based_corr_median_std(df, correlationThreshold)
+
+    R4 = df['maxValues'] >= max(0, specifiedMedian - zScoreThreshold * specifiedStd)
+    R5 = df['maxValues'] <= specifiedMedian + zScoreThreshold * specifiedStd
+    bool_test = R1.values & R2.values & R3.values & R4.values & R5.values
+
+    return bool_test, specifiedMedian, specifiedStd
+
+
+def getGoodBlinkMask(df, zThresholds):
+    "used Feb 02 2023"
+    ## These is the default value
+    correlationThreshold_s1, correlationThreshold_s2, zScoreThreshold_s1, zScoreThreshold_s2 = zThresholds
+
+    df['rightR2'] = df['rightR2'].abs()
+    df_data = df[['leftR2', 'rightR2', 'maxValues']]
+
+    indicesNaN = df_data.isnull().any(1)
+
+    ### GET MASK OPTIMISE
+
+    goodMaskTop_bool, bestMedian, bestRobustStd = get_mask_optimise(df_data, indicesNaN, correlationThreshold_s1,
+                                                                    zScoreThreshold_s1)
+
+    df_s2_bool, worstMedian, worstRobustStd = get_mask_optimise(df_data, indicesNaN, correlationThreshold_s2,
+                                                                zScoreThreshold_s2)
+
+    goodBlinkMask = np.reshape(goodMaskTop_bool | df_s2_bool, (-1, 1))  # Get any TRUE
+    df['blink_quality'] = 'Good'
+    df[['blink_quality']] = df[['blink_quality']].where(goodBlinkMask, other='Reject')
+    return df, bestMedian, bestRobustStd
+
+
+
+
+class BlinkProperties:
+    '''
+    Return a structure with blink shapes and properties for individual blinks
+    '''
+    def __init__(self, data, df, srate):
+        self.data = data
+        self.df = df
+        self.srate = srate
+        self.shutAmpFraction = 0.9
+        self.pAVRThreshold = 3
+        self.zThresholds = (0.90, 0.98, 2, 5)
+        self.df_res=[]
+        self.reset_index()
+        self.get_good_blink_mask()
+        self.set_blink_velocity()
+        self.set_blink_duration()
+        self.set_blink_amp_velocity_ratio_zero_to_max()
+        self.amplitude_velocity_ratio_base()
+        self.amplitude_velocity_ratio_tent()
+        self.time_zero_shut()
+        self.time_base_shut()
+        self.extract_other_times()
+
+    def reset_index(self):
+        self.df.reset_index(drop=True, inplace=True)
+
+    def get_good_blink_mask(self):
+        self.df, self.bestMedian, self.bestRobustStd = getGoodBlinkMask(self.df, self.zThresholds)
+
+    def set_blink_velocity(self):
+        self.signal_l = self.data.shape[0]
+        self.blinkVelocity = np.diff(self.data)
+
+    def set_blink_duration(self):
+        cols_int = ['rightBase']
+        self.df[cols_int] = self.df[cols_int].astype(int)
+        self.df['durationBase'] = (self.df['rightBase'] - self.df['leftBase']) / self.srate
+        self.df['durationTent'] = (self.df['rightXIntercept'] - self.df['leftXIntercept']) / self.srate
+        self.df['durationZero'] = (self.df['rightZero'] - self.df['leftZero']) / self.srate
+        self.df['durationHalfBase'] = (self.df['rightBaseHalfHeight'] - self.df['leftBaseHalfHeight'] + 1) / self.srate
+        self.df['durationHalfZero'] = (self.df['rightZeroHalfHeight'] - self.df['leftZeroHalfHeight'] + 1) / self.srate
+
+    def set_blink_amp_velocity_ratio_zero_to_max(self):
+        self.df[['leftZero', 'rightZero']] = self.df[['leftZero', 'rightZero']].astype(int)
+        self.df['peaksPosVelZero'] = self.df.apply(lambda x: x['leftZero'] + np.argmax(self.blinkVelocity[x['leftZero']:x['maxFrames'] + 1]), axis=1)
+        self.df['RRC'] = self.data[self.df['maxFrames'] - 1] / self.blinkVelocity[self.df['peaksPosVelZero']]
+        self.df['posAmpVelRatioZero'] = (100 * abs(self.df['RRC'])) / self.srate
+        self.df['downStrokevelFrame_del'] = self.df.apply(lambda x: x['maxFrames'] + np.argmin(self.blinkVelocity[x['maxFrames']:x['rightZero'] + 1]), axis=1)
+        self.df['TTT'] = self.data[self.df['maxFrames'] - 1] / self.blinkVelocity[self.df['downStrokevelFrame_del']]
+        self.df['negAmpVelRatioZero'] = (100 * abs(self.df['TTT'])) / self.srate
+
+    def amplitude_velocity_ratio_base(self):
+        self.df['peaksPosVelBase'] = self.df.apply(
+            lambda x: x['leftBase'] + np.argmax(self.blinkVelocity[x['leftBase']:x['maxFrames'] + 1]), axis=1)
+        self.df['KKK'] = self.data[self.df['maxFrames'] - 1] / self.blinkVelocity[self.df['peaksPosVelBase']]
+        self.df['posAmpVelRatioBase'] = (100 * abs(self.df['KKK'])) / self.srate
+
+        self.df['downStroke_del'] = self.df.apply(
+            lambda x: x['maxFrames'] + np.argmin(self.blinkVelocity[x['maxFrames']:x['rightBase'] + 1]), axis=1)
+        self.df['KKK'] = self.data[self.df['maxFrames'] - 1] / self.blinkVelocity[self.df['downStroke_del']]
+        self.df['negAmpVelRatioBase'] = (100 * abs(self.df['KKK'])) / self.srate
+
+    def amplitude_velocity_ratio_tent(self):
+        self.df['pop'] = self.data[self.df['maxFrames'] - 1] / self.df['averRightVelocity']
+        self.df['negAmpVelRatioTent'] = (100 * abs(self.df['pop'])) / self.srate
+
+        self.df['opi'] = self.data[self.df['maxFrames'] - 1] / self.df['averLeftVelocity']
+        self.df['WE'] = (100 * abs(self.df['opi']))
+        self.df['posAmpVelRatioTent'] = self.df['WE'] / self.srate
+
+    def time_zero_shut(self):
+        self.df['closingTimeZero'] = (self.df['maxFrames'] - self.df['leftZero']) / self.srate
+        self.df['reopeningTimeZero'] = (self.df['rightZero'] - self.df['maxFrames']) / self.srate
+
+        self.df['ampThreshhold'] = self.shutAmpFraction * self.df['maxValues']
+        self.df['start_shut_tzs'] = self.df.apply(
+            lambda x: np.argmax(self.data[x['leftZero']:x['rightZero'] + 1] >= x['ampThreshhold']), axis=1)
+
+        self.df['endShut_tzs'] = self.df.apply(
+            lambda x: np.argmax(self.data[x['leftZero']:x['rightZero'] + 1][x['start_shut_tzs'] + 1:-1] <
+                                self.shutAmpFraction * x['maxValues']), axis=1)
+
+        ## PLease expect error here, some value maybe zero or lead to empty cell
+        self.df['endShut_tzs'] = self.df['endShut_tzs'] + 1  ## temporary  to delete
+        self.df['timeShutZero'] = self.df.apply(
+            lambda x: 0 if x['endShut_tzs'] == np.isnan else x['endShut_tzs'] / self.srate, axis=1)
+    def time_base_shut(self):
+        self.df['ampThreshhold_tbs'] = self.shutAmpFraction * self.df['maxValues']
+        self.df['start_shut_tbs'] = self.df.apply(
+            lambda x: np.argmax(self.data[x['leftBase']:x['rightBase'] + 1] >= x['ampThreshhold_tbs']), axis=1)
+
+        self.df['endShut_tbs'] = self.df.apply(
+            lambda x: np.argmax(self.data[x['leftBase']:x['rightBase'] + 1][x['start_shut_tbs']:-1] <
+                                self.shutAmpFraction * x['maxValues']), axis=1)
+
+        self.df['timeShutBase'] = self.df.apply(
+            lambda x: 0 if x['endShut_tbs'] == np.isnan else (x['endShut_tbs'] / self.srate), axis=1)
+
+        ## Time shut tent
+        self.df['closingTimeTent'] = (self.df['xIntersect'] - self.df['leftXIntercept']) / self.srate
+        self.df['reopeningTimeTent'] = (self.df['rightXIntercept'] - self.df['xIntersect']) / self.srate
+
+        self.df['ampThreshhold_tst'] = self.shutAmpFraction * self.df['maxValues']
+
+        self.df[['leftXIntercept_int', 'rightXIntercept_int']] = self.df[['leftXIntercept', 'rightXIntercept']].astype(
+            int)
+
+
+        # warnings.warn('New upgrade')
+        self.df=self.df[self.df.leftXIntercept_int<self.df.rightXIntercept_int]
+        self.df.reset_index(drop=True,inplace=True)
+        self.df['start_shut_tst'] = self.df.apply(
+            lambda x: np.argmax(self.data[x['leftXIntercept_int']:x['rightXIntercept_int'] + 1] >= x['ampThreshhold']), axis=1)
+
+        self.df['endShut_tst'] = self.df.apply(
+            lambda x: np.argmax(self.data[x['leftXIntercept_int']:x['rightXIntercept_int'] + 1][x['start_shut_tst']:-1] <
+                                self.shutAmpFraction * x['maxValues']), axis=1)
+        ### Just in case got other issue, use this back, do not delete
+        ## Since we already remove imblanace left_right intercept, maybe dah xperlu kot bawah ni
+        # df['start_shut_tst'] = df.apply(
+        #     lambda x: _start_shut(data, x['leftXIntercept_int'], x['rightXIntercept_int'], x['ampThreshhold']), axis=1)
+        #
+        #
+        #
+        # df['endShut_tst'] = df.apply(
+        #     lambda x: _end_shut(data, x['leftXIntercept_int'], x['rightXIntercept_int'], x['start_shut_tst'],
+        #                         x['maxValues'], shutAmpFraction), axis=1)
+
+        self.df['timeShutTent'] = self.df.apply(
+            lambda x: 0 if x['endShut_tst'] == np.isnan else (x['endShut_tst'] / self.srate), axis=1)
+
+    def extract_other_times(self):
+        ## Other times
+        self.df['peakMaxBlink '] = self.df['maxValues']
+        self.df['peakMaxTent'] = self.df['yIntersect']
+        self.df['peakTimeTent'] = self.df['xIntersect'] / self.srate
+        self.df['peakTimeBlink'] = self.df['maxFrames'] / self.srate
+
+        dfcal = self.df[['maxFrames', 'peaksPosVelBase', 'peaksPosVelZero']]
+
+        df_t = pd.DataFrame.from_records([[self.signal_l] * 3], columns=['maxFrames', 'peaksPosVelBase', 'peaksPosVelZero'])
+
+        dfcal = pd.concat([dfcal, df_t]).reset_index(drop=True)
+
+        dfcal['ibmx'] = dfcal.maxFrames.diff().shift(-1)
+
+        dfcal['interBlinkMaxAmp'] = dfcal['ibmx'] / self.srate
+
+        dfcal['ibmvb'] = 1 - dfcal['peaksPosVelBase']
+        dfcal['interBlinkMaxVelBase'] = dfcal['ibmvb'] / self.srate  # peaksPosVelBase == velFrame
+
+        dfcal['ibmvz'] = 1 - dfcal['peaksPosVelZero']
+        dfcal['interBlinkMaxVelZero'] = dfcal['ibmvz'] / self.srate
+
+        dfcal.drop(dfcal.tail(1).index, inplace=True)  # drop last n rows# peaksPosVelZero == velFrame
+        dfnew = self.df[['maxValues', 'posAmpVelRatioZero']]
+
+        R1 = dfnew['posAmpVelRatioZero'] < self.pAVRThreshold
+
+        th_bm_brs = self.bestMedian - self.bestRobustStd
+        R2 = dfnew['maxValues'] < th_bm_brs
+        pMask = pd.concat([R1, R2], axis=1)
+        pMasks = pMask.all(1)
+        df_res = pd.merge(self.df, dfcal, on=['maxFrames'])
+        self.df_res = df_res[~pMasks].reset_index(drop=True)
+        # return df_res
+
```

### Comparing `eeg_blinks-0.0.2/eeg_blinks/utilities/getCandidateSignal.py` & `eeg_blinks-0.0.3/eeg_blinks/utilities/getCandidateSignal.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-import warnings
-
-import numpy as np
-
-from eeg_blinks.utilities.extractBlinkProperties import _goodblink_based_corr_median_std
-
-
-class PrepareSelection:
-    def __init__(self, signal=None, df=None, params=None, ch=None):
-        self.signal = signal
-        self.df = df
-        self.params = params
-        self.ch = ch
-
-
-
-    def get_param_for_selection(self):
-        self.df['rightR2'] = self.df['rightR2'].abs()
-        blink_mask = np.zeros(self.signal.size, dtype=bool)
-
-        for left_zero_y, right_zero_x in zip(self.df['leftZero'] - 1, self.df['rightZero']):
-            blink_mask[int(left_zero_y):int(right_zero_x)] = True
-
-        outside_blink = np.logical_and(self.signal > 0, ~blink_mask)
-        inside_blink = np.logical_and(self.signal > 0, blink_mask)
-
-        blink_amp_ratio = np.mean(self.signal[inside_blink]) / np.mean(self.signal[outside_blink])
-
-
-
-        R2_top, R3_top, best_median, best_robust_std = _goodblink_based_corr_median_std(self.df, self.params['correlationThresholdTop'])
-        R2_bot, R3_bot, worst_median, worst_robust_std = _goodblink_based_corr_median_std(self.df,self.params['correlationThresholdBottom'])
-        true_top = R2_top.values & R3_top.values
-        true_bot = R2_bot.values & R3_bot.values
-        good_values = self.df.loc[true_bot, 'maxValues']
-
-        all_values = self.df['maxValues']
-        cutoff = (best_median * worst_robust_std + worst_median * best_robust_std) / (best_robust_std + worst_robust_std)
-
-
-        mask = np.logical_and(all_values <= best_median + 2 * best_robust_std, all_values >= best_median - 2 * best_robust_std)
-        all_X = np.count_nonzero(mask)
-
-        if all_X != 0:
-            good_ratio = np.sum(np.logical_and(good_values <= best_median + 2 * best_robust_std, good_values >= best_median - 2 * best_robust_std)) / all_X
-        else:
-            good_ratio = np.nan
-
-        number_good_blinks = true_bot.sum().item()
-        all_data = [self.ch, blink_amp_ratio, best_median, best_robust_std, cutoff, good_ratio, number_good_blinks, self.df]
-        header_eb_label = ['ch', 'blinkAmpRatio', 'bestMedian', 'bestRobustStd', 'cutoff', 'goodRatio',
-                           'numberGoodBlinks']
-        data_blink = dict(zip(header_eb_label, all_data))
-        return data_blink
-
-
-
-
-class ChannelSelection:
-    '''
-
-    Reduce the number of candidate signals based on these steps
-    1) Reduce the number of candidate signals based on the blink amp ratios:
-        -params ['params_blinkAmpRange_1'],params ['params_blinkAmpRange_2']
-    2) Find the ones that meet the minimum good blink threshold
-        -params ['params_goodRatioThreshold']
-    3) See if any candidates meet the good blink ratio criteria
-
-    4) Pick the one with the maximum number of good blinks
-
-    '''
-    def __init__(self, df, params):
-        self.df = df
-        self.params = params
-        self.nbest = 5
-        self.nbest_force = 2
-        self.params_blinkAmpRange_1 = params['params_blinkAmpRange_1']
-        self.params_blinkAmpRange_2 = params['params_blinkAmpRange_2']
-        self.params_goodRatioThreshold = params['params_goodRatioThreshold']
-        self.params_minGoodBlinks = params['params_minGoodBlinks']
-        self.reduce_candidate_signals()
-        self.pick_best_channel()
-        self.df.reset_index(drop=True, inplace=True)
-
-    def reduce_candidate_signals(self):
-        self.df['con_blinkAmpRange'] = np.where((self.df.blinkAmpRatio >= self.params_blinkAmpRange_1) &
-                                                (self.df.blinkAmpRatio <= self.params_blinkAmpRange_2),
-                                                True, False)
-
-        self.df['con_GoodBlinks'] = np.where((self.df.numberGoodBlinks > self.params_minGoodBlinks),
-                                             True, False)
-
-        self.df['con_GoodRatio'] = np.where((self.df.goodRatio > self.params_goodRatioThreshold),
-                                            True, False)
-        self.df.sort_values(['goodRatio', 'numberGoodBlinks'], ascending=[False, False], inplace=True)
-
-    def pick_best_channel(self):
-
-        # step 1
-        nblinkAmpRange = self.df['con_blinkAmpRange'].sum()
-        ncon_GoodRatio = self.df['con_GoodRatio'].sum()
-
-        if nblinkAmpRange == 0:
-            warnings.warn(f'Blink amplitude ratio too low than the predeterimined therehold-- may be noise.')
-            if ncon_GoodRatio != 0:
-                self.df = self.df[self.df['con_GoodRatio'] == True]
-                self.df = self.df.head(self.nbest_force)
-            else:
-                self.df = self.df.head(self.nbest_force)
-            return self.df
-
-        # Step 2
-        # Now see if any candidates meet the good blink ratio criteria
-
-        if ncon_GoodRatio == 0:
-            if nblinkAmpRange != 0:
-                self.df = self.df[self.df['con_blinkAmpRange'] == True]
-                self.df = self.df.head(self.nbest_force)
-                return self.df
-            else:
-                return self.df.head(self.nbest_force)
-
-        # If we fulfill the con_GoodRatio,ncon_GoodRatio
-        df1 = self.df[(self.df['con_GoodRatio'] == True) & (self.df['con_blinkAmpRange'] == True)]
-        if df1.empty:
-            """
-            Most probably we have
-            con_blinkAmpRange   con_goodBLinks  con_GoodRatio
-            FALSE               TRUE            TRUE
-            TRUE                TRUE            FALSE
-            """
-            self.df = self.df[(self.df['con_GoodRatio'] == True) & (self.df['con_GoodBlinks'] == True)]
-            return self.df
-        else:
-            """
-            Ideal case
-            """
-            self.df = self.df[(self.df['con_GoodRatio'] == True) & (self.df['con_blinkAmpRange'] == True) & (self.df['con_GoodBlinks'] == True)]
-
-            return self.df.head(self.nbest)
-
+import warnings
+
+import numpy as np
+
+from eeg_blinks.utilities.extractBlinkProperties import _goodblink_based_corr_median_std
+
+
+class PrepareSelection:
+    def __init__(self, signal=None, df=None, params=None, ch=None):
+        self.signal = signal
+        self.df = df
+        self.params = params
+        self.ch = ch
+
+
+
+    def get_param_for_selection(self):
+        self.df['rightR2'] = self.df['rightR2'].abs()
+        blink_mask = np.zeros(self.signal.size, dtype=bool)
+
+        for left_zero_y, right_zero_x in zip(self.df['leftZero'] - 1, self.df['rightZero']):
+            blink_mask[int(left_zero_y):int(right_zero_x)] = True
+
+        outside_blink = np.logical_and(self.signal > 0, ~blink_mask)
+        inside_blink = np.logical_and(self.signal > 0, blink_mask)
+
+        blink_amp_ratio = np.mean(self.signal[inside_blink]) / np.mean(self.signal[outside_blink])
+
+
+
+        R2_top, R3_top, best_median, best_robust_std = _goodblink_based_corr_median_std(self.df, self.params['correlationThresholdTop'])
+        R2_bot, R3_bot, worst_median, worst_robust_std = _goodblink_based_corr_median_std(self.df,self.params['correlationThresholdBottom'])
+        true_top = R2_top.values & R3_top.values
+        true_bot = R2_bot.values & R3_bot.values
+        good_values = self.df.loc[true_bot, 'maxValues']
+
+        all_values = self.df['maxValues']
+        cutoff = (best_median * worst_robust_std + worst_median * best_robust_std) / (best_robust_std + worst_robust_std)
+
+
+        mask = np.logical_and(all_values <= best_median + 2 * best_robust_std, all_values >= best_median - 2 * best_robust_std)
+        all_X = np.count_nonzero(mask)
+
+        if all_X != 0:
+            good_ratio = np.sum(np.logical_and(good_values <= best_median + 2 * best_robust_std, good_values >= best_median - 2 * best_robust_std)) / all_X
+        else:
+            good_ratio = np.nan
+
+        number_good_blinks = true_bot.sum().item()
+        all_data = [self.ch, blink_amp_ratio, best_median, best_robust_std, cutoff, good_ratio, number_good_blinks, self.df]
+        header_eb_label = ['ch', 'blinkAmpRatio', 'bestMedian', 'bestRobustStd', 'cutoff', 'goodRatio',
+                           'numberGoodBlinks']
+        data_blink = dict(zip(header_eb_label, all_data))
+        return data_blink
+
+
+
+
+class ChannelSelection:
+    '''
+
+    Reduce the number of candidate signals based on these steps
+    1) Reduce the number of candidate signals based on the blink amp ratios:
+        -params ['params_blinkAmpRange_1'],params ['params_blinkAmpRange_2']
+    2) Find the ones that meet the minimum good blink threshold
+        -params ['params_goodRatioThreshold']
+    3) See if any candidates meet the good blink ratio criteria
+
+    4) Pick the one with the maximum number of good blinks
+
+    '''
+    def __init__(self, df, params):
+        self.df = df
+        self.params = params
+        self.nbest = 5
+        self.nbest_force = 2
+        self.params_blinkAmpRange_1 = params['params_blinkAmpRange_1']
+        self.params_blinkAmpRange_2 = params['params_blinkAmpRange_2']
+        self.params_goodRatioThreshold = params['params_goodRatioThreshold']
+        self.params_minGoodBlinks = params['params_minGoodBlinks']
+        self.reduce_candidate_signals()
+        self.pick_best_channel()
+        self.df.reset_index(drop=True, inplace=True)
+
+    def reduce_candidate_signals(self):
+        self.df['con_blinkAmpRange'] = np.where((self.df.blinkAmpRatio >= self.params_blinkAmpRange_1) &
+                                                (self.df.blinkAmpRatio <= self.params_blinkAmpRange_2),
+                                                True, False)
+
+        self.df['con_GoodBlinks'] = np.where((self.df.numberGoodBlinks > self.params_minGoodBlinks),
+                                             True, False)
+
+        self.df['con_GoodRatio'] = np.where((self.df.goodRatio > self.params_goodRatioThreshold),
+                                            True, False)
+        self.df.sort_values(['goodRatio', 'numberGoodBlinks'], ascending=[False, False], inplace=True)
+
+    def pick_best_channel(self):
+
+        # step 1
+        nblinkAmpRange = self.df['con_blinkAmpRange'].sum()
+        ncon_GoodRatio = self.df['con_GoodRatio'].sum()
+
+        if nblinkAmpRange == 0:
+            warnings.warn(f'Blink amplitude ratio too low than the predeterimined therehold-- may be noise.')
+            if ncon_GoodRatio != 0:
+                self.df = self.df[self.df['con_GoodRatio'] == True]
+                self.df = self.df.head(self.nbest_force)
+            else:
+                self.df = self.df.head(self.nbest_force)
+            return self.df
+
+        # Step 2
+        # Now see if any candidates meet the good blink ratio criteria
+
+        if ncon_GoodRatio == 0:
+            if nblinkAmpRange != 0:
+                self.df = self.df[self.df['con_blinkAmpRange'] == True]
+                self.df = self.df.head(self.nbest_force)
+                return self.df
+            else:
+                return self.df.head(self.nbest_force)
+
+        # If we fulfill the con_GoodRatio,ncon_GoodRatio
+        df1 = self.df[(self.df['con_GoodRatio'] == True) & (self.df['con_blinkAmpRange'] == True)]
+        if df1.empty:
+            """
+            Most probably we have
+            con_blinkAmpRange   con_goodBLinks  con_GoodRatio
+            FALSE               TRUE            TRUE
+            TRUE                TRUE            FALSE
+            """
+            self.df = self.df[(self.df['con_GoodRatio'] == True) & (self.df['con_GoodBlinks'] == True)]
+            return self.df
+        else:
+            """
+            Ideal case
+            """
+            self.df = self.df[(self.df['con_GoodRatio'] == True) & (self.df['con_blinkAmpRange'] == True) & (self.df['con_GoodBlinks'] == True)]
+
+            return self.df.head(self.nbest)
+
```

### Comparing `eeg_blinks-0.0.2/eeg_blinks/utilities/misc.py` & `eeg_blinks-0.0.3/eeg_blinks/utilities/misc.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-
-import numpy as np
-import mne
-import os
-import re
-import shutil
-import pandas as pd
-def mad_matlab(arr, axis=None, keepdims=True):
-    median = np.median(arr, axis=axis, keepdims=True)
-    mad = np.median(np.abs(arr - median), axis=axis, keepdims=keepdims)[0]
-    return mad
-
-def check_make_folder(path, remove=False):
-    if not remove:
-        if not os.path.exists(path):
-            os.makedirs(path, exist_ok=True)
-    else:
-        '''
-        Some time I want the folder to be emptied
-        '''
-        if os.path.exists(path):
-            shutil.rmtree(path)
-            os.makedirs(path, exist_ok=True)
-        else:
-            os.makedirs(path, exist_ok=True)
-
-
-def create_annotation(sblink, sfreq, label):
-    st_blink = 'leftZero'
-    blink_en = 'rightZero'
-    # st_blink='startBlinks'
-    # blink_en='endBlinks'
-    if not isinstance(sblink, pd.DataFrame):
-        raise ValueError('No appropriate channel. sorry. Try to use large channel selection')
-
-    # d_s = ((sblink[blink_en] - sblink[st_blink]) / sfreq).tolist()
-    # d_s = ((sblink[blink_en] - sblink[st_blink]) / sfreq).tolist()
-    # onset_s = (sblink[st_blink] / sfreq).tolist()
-    # d_s = ((sblink[blink_en] - sblink[st_blink]) / sfreq).tolist()
-    onset_s = (sblink['maxFrames'] / sfreq).tolist()
-    des_s = [label] * len(onset_s)
-    d_s=[0]* len(onset_s)
-
-    annot = mne.Annotations(onset=onset_s,  # in seconds
-                            duration=d_s,  # in seconds, too
-                            description=des_s)
-
+
+import numpy as np
+import mne
+import os
+import re
+import shutil
+import pandas as pd
+def mad_matlab(arr, axis=None, keepdims=True):
+    median = np.median(arr, axis=axis, keepdims=True)
+    mad = np.median(np.abs(arr - median), axis=axis, keepdims=keepdims)[0]
+    return mad
+
+def check_make_folder(path, remove=False):
+    if not remove:
+        if not os.path.exists(path):
+            os.makedirs(path, exist_ok=True)
+    else:
+        '''
+        Some time I want the folder to be emptied
+        '''
+        if os.path.exists(path):
+            shutil.rmtree(path)
+            os.makedirs(path, exist_ok=True)
+        else:
+            os.makedirs(path, exist_ok=True)
+
+
+def create_annotation(sblink, sfreq, label):
+    st_blink = 'leftZero'
+    blink_en = 'rightZero'
+    # st_blink='startBlinks'
+    # blink_en='endBlinks'
+    if not isinstance(sblink, pd.DataFrame):
+        raise ValueError('No appropriate channel. sorry. Try to use large channel selection')
+
+    # d_s = ((sblink[blink_en] - sblink[st_blink]) / sfreq).tolist()
+    # d_s = ((sblink[blink_en] - sblink[st_blink]) / sfreq).tolist()
+    # onset_s = (sblink[st_blink] / sfreq).tolist()
+    # d_s = ((sblink[blink_en] - sblink[st_blink]) / sfreq).tolist()
+    onset_s = (sblink['maxFrames'] / sfreq).tolist()
+    des_s = [label] * len(onset_s)
+    d_s=[0]* len(onset_s)
+
+    annot = mne.Annotations(onset=onset_s,  # in seconds
+                            duration=d_s,  # in seconds, too
+                            description=des_s)
+
     return annot
```


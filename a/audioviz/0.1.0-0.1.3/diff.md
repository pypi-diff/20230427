# Comparing `tmp/audioviz-0.1.0.tar.gz` & `tmp/audioviz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioviz-0.1.0.tar", last modified: Sun Apr 23 04:17:53 2023, max compression
+gzip compressed data, was "audioviz-0.1.3.tar", last modified: Thu Apr 27 03:19:27 2023, max compression
```

## Comparing `audioviz-0.1.0.tar` & `audioviz-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-23 04:17:53.479748 audioviz-0.1.0/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      695 2023-04-23 04:17:53.479748 audioviz-0.1.0/PKG-INFO
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-23 04:17:53.479748 audioviz-0.1.0/audioviz/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8447 2023-04-23 03:57:05.000000 audioviz-0.1.0/audioviz/BeatAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9467 2023-04-23 03:57:05.000000 audioviz-0.1.0/audioviz/ChordAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     3211 2023-04-23 03:57:05.000000 audioviz-0.1.0/audioviz/GeneralAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.0/audioviz/PitchAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14040 2023-04-23 03:57:05.000000 audioviz-0.1.0/audioviz/StructureAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.0/audioviz/TimbreAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      238 2023-04-23 03:57:05.000000 audioviz-0.1.0/audioviz/__init__.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1580 2023-04-23 03:57:05.000000 audioviz-0.1.0/audioviz/colabInterface.py
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-23 04:17:53.479748 audioviz-0.1.0/audioviz.egg-info/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      695 2023-04-23 04:17:53.000000 audioviz-0.1.0/audioviz.egg-info/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      418 2023-04-23 04:17:53.000000 audioviz-0.1.0/audioviz.egg-info/SOURCES.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-23 04:17:53.000000 audioviz-0.1.0/audioviz.egg-info/dependency_links.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-23 04:00:31.000000 audioviz-0.1.0/audioviz.egg-info/not-zip-safe
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       51 2023-04-23 04:17:53.000000 audioviz-0.1.0/audioviz.egg-info/requires.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-04-23 04:17:53.000000 audioviz-0.1.0/audioviz.egg-info/top_level.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-04-23 04:17:53.479748 audioviz-0.1.0/setup.cfg
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1133 2023-04-23 04:17:16.000000 audioviz-0.1.0/setup.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-27 03:19:27.951593 audioviz-0.1.3/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      684 2023-04-27 03:19:27.951593 audioviz-0.1.3/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1258 2023-04-25 05:51:15.000000 audioviz-0.1.3/README.md
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-27 03:19:27.951593 audioviz-0.1.3/audioviz/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.3/audioviz/BeatAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9467 2023-04-23 03:57:05.000000 audioviz-0.1.3/audioviz/ChordAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     3211 2023-04-23 03:57:05.000000 audioviz-0.1.3/audioviz/GeneralAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.3/audioviz/PitchAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.3/audioviz/StructureAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.3/audioviz/TimbreAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      238 2023-04-23 03:57:05.000000 audioviz-0.1.3/audioviz/__init__.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.3/audioviz/colabInterface.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-27 03:19:27.951593 audioviz-0.1.3/audioviz.egg-info/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      684 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      428 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/not-zip-safe
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       51 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/requires.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/top_level.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-04-27 03:19:27.951593 audioviz-0.1.3/setup.cfg
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1122 2023-04-27 03:18:14.000000 audioviz-0.1.3/setup.py
```

### Comparing `audioviz-0.1.0/PKG-INFO` & `audioviz-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.0
+Version: 0.1.3
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
-Home-page: https://github.com/TrangDuLam/NTHU_Music_AI_Tools
+Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
```

### Comparing `audioviz-0.1.0/audioviz/BeatAnalysis.py` & `audioviz-0.1.3/audioviz/BeatAnalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from matplotlib import pyplot as plt
 import plotly.express as px
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 import scipy
 
 from numpy import typing as npt
+import IPython.display as ipd
 
 from .colabInterface import *
 
 def onsets_detection(y: npt.ArrayLike, sr: int, write_to_wav: bool = False) -> None :
 
     '''
     To show onsets of the input signal with time axis and modify the .wav with onset click sounds
@@ -33,14 +34,15 @@
 
     # Save onset-to-time info
     result = np.round(times[onset_frames].T, 3)
     save_and_downloader('beats.csv', np.array(['Time']), result)
 
     # Save the processed audio
     y_onset_clicks = librosa.clicks(frames=onset_frames, sr=sr, length=len(y))
+    ipd.Audio(y_onset_clicks, rate=sr)
     audio_save_and_downloader('onset_click.wav', y_onset_clicks, sr)
 
 
 def plot_onset_strength(y: npt.ArrayLike, sr:int, standard: bool = True, custom_mel: bool = False, cqt: bool = False) :
 
     '''
     To plot the onset strength of the input signal with time-axis
@@ -116,14 +118,15 @@
 
     # Save beat-to-time info
     result = np.round(times[beats].T, 3)
     save_and_downloader('beats.csv', np.array(['Time']), result)
 
     # Save processed audio
     y_beats = librosa.clicks(frames=beats, sr=sr, length=len(y))
+    ipd.Audio(y_beats, rate=sr)
     audio_save_and_downloader('beat_click.wav', y_beats, sr)
 
 
 def predominant_local_pulses(y: npt.ArrayLike, sr:int) -> None :
 
     '''
     To plot the predominant local pulses of the input signal with time-axis
```

### Comparing `audioviz-0.1.0/audioviz/ChordAnalysis.py` & `audioviz-0.1.3/audioviz/ChordAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.0/audioviz/GeneralAnalysis.py` & `audioviz-0.1.3/audioviz/GeneralAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.0/audioviz/PitchAnalysis.py` & `audioviz-0.1.3/audioviz/PitchAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.0/audioviz/StructureAnalysis.py` & `audioviz-0.1.3/audioviz/StructureAnalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 from scipy import signal
 from matplotlib import pyplot as plt
 import matplotlib.gridspec as gridspec
 import IPython.display as ipd
 import pandas as pd
 from numba import jit
 
-import ipywidgets as widgets
-from IPython.display import display
-import functools
-
 import libfmp.b
 import libfmp.c2
 import libfmp.c3
 import libfmp.c4
 import libfmp.c6
 import libfmp
 from libfmp.b import FloatingBox
 
+import ipywidgets as widgets
+from IPython.display import display
+import functools
+from google.colab import files
+
 from numpy import typing as npt
 
 @jit(nopython=True)
 def compute_sm_dot(X, Y):
     """Computes similarty matrix from feature sequences using dot (inner) product
 
     Notebook: C4/C4S2_SSM.ipynb
@@ -222,14 +223,16 @@
     
     header_row = ['Time', 'Novelty']
     result_array = np.round(np.hstack((timeIndices, novSelected)), 3)
     with open('Novelty_SSM.csv', 'w') as out :
             print(*header_row, sep=',', file=out)
             for row in result_array :
                 print(*row, sep=',', file=out)
+                
+    files.download('Novelty_SSM.csv')
 
 def cancel_button_eventhandler(arg):
     print("Cancel")
 
 def SSM_Novelty(wav_filename:str, anno_csv: str) -> None :
 
     '''
```

### Comparing `audioviz-0.1.0/audioviz/TimbreAnalysis.py` & `audioviz-0.1.3/audioviz/TimbreAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.0/audioviz/colabInterface.py` & `audioviz-0.1.3/audioviz/colabInterface.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     files.download(filename)
 
 def noMsg(arg):
     print("No")
 
 def save_and_downloader(filename: str, header_of_file: npt.ArrayLike, result_array: npt.ArrayLike) :
 
-    buttonDownload = widgets.Button(description = 'Download & Save')
+    buttonDownload = widgets.Button(description = '.csv Download & Save')
     buttonCancel =  widgets.Button(description = 'Cancel') 
     buttonDownload.on_click(functools.partial(core_download_and_save, filename, header_of_file, result_array))
     buttonCancel.on_click(noMsg)
 
     display(buttonDownload)
     display(buttonCancel)
 
@@ -37,14 +37,14 @@
     
     sf.write(filename, audio_array, sr, subtype='PCM_24')
     files.download(filename)
 
 
 def audio_save_and_downloader(filename: str, audio_array: npt.ArrayLike, sr: int) :
 
-    buttonDownload = widgets.Button(description = 'Download & Save')
+    buttonDownload = widgets.Button(description = 'Audio Download & Save')
     buttonCancel =  widgets.Button(description = 'Cancel') 
     buttonDownload.on_click(functools.partial(core_audio_download_and_save, filename, audio_array, sr))
     buttonCancel.on_click(noMsg)
 
     display(buttonDownload)
     display(buttonCancel)
```

### Comparing `audioviz-0.1.0/audioviz.egg-info/PKG-INFO` & `audioviz-0.1.3/audioviz.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.0
+Version: 0.1.3
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
-Home-page: https://github.com/TrangDuLam/NTHU_Music_AI_Tools
+Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
```

### Comparing `audioviz-0.1.0/setup.py` & `audioviz-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='audioviz',
     packages=['audioviz'],
-    version='0.1.0',
+    version='0.1.3',
     description='An user-friendly music information retrieval tools interfacing with Google Colab',
 
-    url='https://github.com/TrangDuLam/NTHU_Music_AI_Tools',
+    url='https://github.com/TrangDuLam/audioviz',
     author='ayTrang',
     author_email='andrew.chuang@gapp.nthu.edu.tw',
     license='MIT',
     zip_safe=False,
     keywords=['Music Information Retrieval', "Academia Sinica", "NTHU"],
 
     install_requires = ["numpy",
```


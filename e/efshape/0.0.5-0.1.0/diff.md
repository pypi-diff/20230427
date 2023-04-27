# Comparing `tmp/efshape-0.0.5.tar.gz` & `tmp/efshape-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/efshape-0.0.5.tar", last modified: Fri Apr  3 12:52:29 2020, max compression
+gzip compressed data, was "efshape-0.1.0.tar", last modified: Thu Apr 27 10:52:50 2023, max compression
```

## Comparing `efshape-0.0.5.tar` & `efshape-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fukudasoujirou   (501) staff       (20)        0 2020-04-03 12:52:29.000000 efshape-0.0.5/
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)       52 2020-02-23 01:48:52.000000 efshape-0.0.5/MANIFEST.in
-drwxr-xr-x   0 fukudasoujirou   (501) staff       (20)        0 2020-04-03 12:52:29.000000 efshape-0.0.5/Main/
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)        6 2020-03-20 09:37:35.000000 efshape-0.0.5/Main/__init__.py
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)     1767 2020-04-03 12:52:29.000000 efshape-0.0.5/PKG-INFO
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)     1171 2020-04-03 11:59:11.000000 efshape-0.0.5/README.md
-drwxr-xr-x   0 fukudasoujirou   (501) staff       (20)        0 2020-04-03 12:52:29.000000 efshape-0.0.5/efshape/
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)       31 2020-04-03 12:50:12.000000 efshape-0.0.5/efshape/__init__.py
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)    33005 2020-04-03 12:39:27.000000 efshape-0.0.5/efshape/efa.py
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)    88659 2020-04-03 12:39:09.000000 efshape-0.0.5/efshape/efgui.py
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)    80240 2020-03-20 09:37:35.000000 efshape-0.0.5/efshape/fgui.py
-drwxr-xr-x   0 fukudasoujirou   (501) staff       (20)        0 2020-04-03 12:52:29.000000 efshape-0.0.5/efshape.egg-info/
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)     1767 2020-04-03 12:52:29.000000 efshape-0.0.5/efshape.egg-info/PKG-INFO
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)      303 2020-04-03 12:52:29.000000 efshape-0.0.5/efshape.egg-info/SOURCES.txt
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)        1 2020-04-03 12:52:29.000000 efshape-0.0.5/efshape.egg-info/dependency_links.txt
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)      107 2020-04-03 12:52:29.000000 efshape-0.0.5/efshape.egg-info/entry_points.txt
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)      133 2020-04-03 12:52:29.000000 efshape-0.0.5/efshape.egg-info/requires.txt
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)       13 2020-04-03 12:52:29.000000 efshape-0.0.5/efshape.egg-info/top_level.txt
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)       38 2020-04-03 12:52:29.000000 efshape-0.0.5/setup.cfg
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)     1687 2020-04-03 12:51:33.000000 efshape-0.0.5/setup.py
+drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:52:50.149411 efshape-0.1.0/
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       52 2023-04-22 02:05:01.000000 efshape-0.1.0/MANIFEST.in
+drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:52:50.149411 efshape-0.1.0/Main/
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)        6 2023-04-22 02:05:01.000000 efshape-0.1.0/Main/__init__.py
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1652 2023-04-27 10:52:50.149411 efshape-0.1.0/PKG-INFO
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1171 2023-04-22 02:05:01.000000 efshape-0.1.0/README.md
+drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:52:50.149411 efshape-0.1.0/efshape/
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       31 2023-04-22 02:05:01.000000 efshape-0.1.0/efshape/__init__.py
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)    33057 2023-04-23 15:21:35.000000 efshape-0.1.0/efshape/efa.py
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)    88190 2023-04-27 10:31:20.000000 efshape-0.1.0/efshape/efgui.py
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)    85967 2023-04-27 10:36:23.000000 efshape-0.1.0/efshape/fgui.py
+drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:52:50.149411 efshape-0.1.0/efshape.egg-info/
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1652 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/PKG-INFO
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      303 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/SOURCES.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)        1 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/dependency_links.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      107 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/entry_points.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      133 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/requires.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       13 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/top_level.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       38 2023-04-27 10:52:50.149411 efshape-0.1.0/setup.cfg
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1687 2023-04-27 10:47:25.000000 efshape-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `efshape-0.0.5/PKG-INFO` & `efshape-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: efshape
-Version: 0.0.5
+Version: 0.1.0
 Summary: Package Dependency: Validates package requirements
 Home-page: https://github.com/SojiroFukuda/efshape
 Author: SojiroFukuda
 Author-email: S.Fukuda-2018@hull.ac.uk
 Maintainer: SojiroFukuda
 Maintainer-email: S.Fukuda-2018@hull.ac.uk
 License: SojiroFukuda
-Description: # ef-shape
-        
-        efshape is a python package for shape analysis of 2D image.
-        The method is based on the combination between 'Elliptic Fourier Analysis (EFA)' and 'Principal Component Analysis (PCA)' and called EF-PCA method.
-        The basic idea is to convert the 2D closed contour into a numeric dataset by EFA and then, using multivariate analysis (PCA) , detect the major shape variation of the dataset. 
-        EFA enables you to describe the complicated shape complehensively as a number of dataset called elliptic Fourire descriptors.
-        One of the merits of this method is that you can easily reconstruct the shape from the descriptors, which also make it easier to interpret the shape variation of detected principal component axes.
-        
-        In this package, you can choose three different types of EF-PCA methods: one of which, EFD-based EF-PCA, is suitable for directional object like bio-forms and the others, Amplitude- and FPS-based EF-PCA, are suitable for non-directional object such as sedimentary grain.
-        This package provides you both CUI- and GUI-based package.
-        
-        # About license
-        © 2019 Sojiro Fukuda All Rightss Reserved.
-        Free to modify and redistribute by your own responsibility.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
+
+# ef-shape
+
+efshape is a python package for shape analysis of 2D image.
+The method is based on the combination between 'Elliptic Fourier Analysis (EFA)' and 'Principal Component Analysis (PCA)' and called EF-PCA method.
+The basic idea is to convert the 2D closed contour into a numeric dataset by EFA and then, using multivariate analysis (PCA) , detect the major shape variation of the dataset. 
+EFA enables you to describe the complicated shape complehensively as a number of dataset called elliptic Fourire descriptors.
+One of the merits of this method is that you can easily reconstruct the shape from the descriptors, which also make it easier to interpret the shape variation of detected principal component axes.
+
+In this package, you can choose three different types of EF-PCA methods: one of which, EFD-based EF-PCA, is suitable for directional object like bio-forms and the others, Amplitude- and FPS-based EF-PCA, are suitable for non-directional object such as sedimentary grain.
+This package provides you both CUI- and GUI-based package.
+
+# About license
+© 2019 Sojiro Fukuda All Rightss Reserved.
+Free to modify and redistribute by your own responsibility.
+
```

### Comparing `efshape-0.0.5/README.md` & `efshape-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `efshape-0.0.5/efshape/efa.py` & `efshape-0.1.0/efshape/efa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import cv2
 import numpy as np
 from scipy.optimize import curve_fit
 from scipy.interpolate import interp1d
 
 import pandas as pd
+import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.patches import Circle, Polygon, Rectangle
 from matplotlib.colors import LinearSegmentedColormap
-
+# matplotlib.use("agg")
 import os
 import sklearn
 from sklearn.decomposition import PCA
 import random
 import scipy.stats as st
 
 # print("OpenCV: " + cv2.__version__)
@@ -264,15 +265,15 @@
         contours.pop(scale_index)
     elif SCALE == 2:
         unit_conv = (SCALE_VALUE/scale_width)*(SCALE_VALUE/scale_width)
         contours.pop(scale_index)
     elif SCALE == 3:
         unit_conv = (SCALE_VALUE/scale_height)*(SCALE_VALUE/scale_height)
         contours.pop(scale_index)
-    draw_contours(gray,contours,file,save_dir)
+    # draw_contours(gray,contours,file,save_dir)  ## test
     Photo = im_path.split(os.sep)[-1].split(os.extsep)[0]
     len_contours = len(contours)
     INDEX_PIXEL = 0
     INDEX_AREA = 1
     INDEX_PHI = 2
     INDEX_PSI = 3
     INDEX_PERIM = 4
```

### Comparing `efshape-0.0.5/efshape/efgui.py` & `efshape-0.1.0/efshape/efgui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,54 @@
 import sys
-from PyQt5 import QtCore as Qc, QtGui as Qg, QtWidgets as Qw   
-from PyQt5.QtCore import Qt, QThread, pyqtSignal
+from PyQt6 import QtCore as Qc, QtGui as Qg, QtWidgets as Qw   
+from PyQt6.QtCore import Qt, QThread, pyqtSignal
 import matplotlib
-matplotlib.use("Qt5Agg")
+matplotlib.use("agg")
 import os
 import re
 import glob
 import numpy as np
 from . import efa as ef
+# import efa as ef
 import pandas as pd
-import random
-import time
-from . import fgui as fpsGui                            
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
+from . import fgui as fpsGui 
+# import fgui as fpsGui                           
+# from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
+from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg as FigureCanvas
+
 from matplotlib.figure import Figure
 from pathlib import Path
-from PyQt5.Qt import PYQT_VERSION_STR
+# from PyQt6.Qt import PYQT_VERSION_STR
 from datetime import datetime
 import matplotlib.animation as animation
 
 
-
-# print("Python: " + sys.version)
-# print("pandas ver. " + pd.__version__)
-# print("matplotlib ver. " + matplotlib.__version__)
-# print("numpy ver. " + np.__version__)
-# print("PyQt5 ver. " + PYQT_VERSION_STR)
-
 # Display pandas dataframe at QTableWidget
 class PandasModel(Qc.QAbstractTableModel): 
     def __init__(self, df = pd.DataFrame(), parent=None): 
         Qc.QAbstractTableModel.__init__(self, parent=parent)
         self._df = df
 
-    def headerData(self, section, orientation, role=Qt.DisplayRole):
-        if role != Qt.DisplayRole:
+    def headerData(self, section, orientation, role=Qt.ItemDataRole.DisplayRole):
+        if role != Qt.ItemDataRole.DisplayRole:
             return Qc.QVariant()
 
-        if orientation == Qt.Horizontal:
+        if orientation == Qt.Orientation.Horizontal:
             try:
                 return self._df.columns.tolist()[section]
             except (IndexError, ):
                 return Qc.QVariant()
-        elif orientation == Qt.Vertical:
+        elif orientation == Qt.Orientation.Vertical:
             try:
                 return self._df.index.tolist()[section]
             except (IndexError, ):
                 return Qc.QVariant()
 
-    def data(self, index, role=Qt.DisplayRole):
-        if role != Qt.DisplayRole:
+    def data(self, index, role=Qt.ItemDataRole.DisplayRole):
+        if role != Qt.ItemDataRole.DisplayRole:
             return Qc.QVariant()
 
         if not index.isValid():
             return Qc.QVariant()
 
         return Qc.QVariant(str(self._df.iloc[index.row(), index.column()])) 
 
@@ -85,14 +80,15 @@
         self.layoutChanged.emit()
 
 # Conduct FPS with an independent thread
 class FourierAnalyzer(QThread):
     countChanged = pyqtSignal(int)
     stringChanged = pyqtSignal(str)
     stringChangedPCA = pyqtSignal(str)
+    FourierDone = pyqtSignal(str)
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.w = Qw.QDialog(parent)
         self.parent = parent
 
     def run(self):
@@ -132,16 +128,23 @@
                 # -------------------
                 PROGRESS_VALUE = PROGRESS_VALUE + 1
                 self.countChanged.emit(PROGRESS_VALUE)
                 TOTAL_CLAST = TOTAL_CLAST + total_num
         # Log #--------------
         self.stringChanged.emit("\n"+"------------------ end."+"\n"+"In total "+str(TOTAL_CLAST)+" grains were detected"+"\n")
         # -------------------
-        self.parent.ui.textbox_fpsPath.setText(self.parent.SAVE_PATH)
-        self.parent.FPS_PATH = self.parent.SAVE_PATH
+        #######################################################
+        ###########   CHECK THIS ##############################
+        ######## Causative of segmentation error ##############
+        self.FourierDone.emit(self.parent.SAVE_PATH)
+        # self.parent.ui.textbox_fpsPath.setText(self.parent.SAVE_PATH) 
+        # self.parent.FPS_PATH = self.parent.SAVE_PATH
+        #######################################################
+        ######################################################
+        
         # self.parent.SAVE_PCA = self.parent.SAVE_PATH
         # self.parent.ui.textbox_pcaSave.setText(self.parent.SAVE_PCA)
 # Conduct FPS with an independent thread
 class GraphAnimation(QThread):
     graphRenew = pyqtSignal(int)
 
     def __init__(self, parent=None):
@@ -292,34 +295,79 @@
         self.delt = 0.001 # The inverse number of point along the contour
         self.N = 30 # Maximum number of harmonics
         self.MIN_PIXEL_SIZE = 200
         self.SCALE_TYPE = 0 # 0: None 1:Area 2: X-Length 3: Y-Length
         self.SCALE_UNIT = ""
         self.SCALE_VALUE = 1
         self.SCALE_POSITION = 0  #0: Top 1: Bottom 2: right 3: left
+        
+        # EFA threading
         self.fa = FourierAnalyzer(self)
         self.fa.countChanged.connect(self.onCountChanged)
         self.fa.stringChanged.connect(self.onStringChanged)
         self.fa.stringChangedPCA.connect(self.onStringChangedPCA)
+        self.fa.FourierDone.connect(self.onFourierDone)
+        
+        self.ui.cmb_format.currentIndexChanged.connect(self.setFormat) # type: ignore
+        self.ui.button_folda.clicked.connect(self.setFoldaPath) # type: ignore
+        self.ui.button_save.clicked.connect(self.setSavePath) # type: ignore
+        self.ui.cmb_sampleType.currentIndexChanged.connect(self.setBGC) # type: ignore
+        self.ui.spb_N.valueChanged.connect(self.setN) # type: ignore
+        self.ui.spb_mpxa.valueChanged.connect(self.setMPA) # type: ignore
+        self.ui.button_FPS.clicked.connect(self.startEFA) # type: ignore
+        self.ui.cmb_scaleType.currentIndexChanged.connect(self.setScaleType) # type: ignore
+        self.ui.textBox_scaleU.textEdited.connect(self.setScaleUnit) # type: ignore
+        self.ui.spb_scaleSize.valueChanged.connect(self.setScaleValue) # type: ignore
+        self.ui.cmb_scalePos.currentIndexChanged.connect(self.setScalePosition) # type: ignore
+        self.ui.button_header.clicked.connect(self.setHeaderName) # type: ignore
+        self.ui.button_FPSpath.clicked.connect(self.setFPSPath) # type: ignore
+        self.ui.button_savePCApath.clicked.connect(self.setSavePCAPath) # type: ignore
+        self.ui.cmb_matrixPCA.currentIndexChanged.connect(self.setPCAmatrix) # type: ignore
+        self.ui.button_PCA.clicked.connect(self.startPCA) # type: ignore
+        self.ui.cmb_x.currentIndexChanged.connect(self.setXaxis) # type: ignore
+        self.ui.cmb_y.currentIndexChanged.connect(self.setYaxis) # type: ignore
+        self.ui.cmb_color.currentIndexChanged.connect(self.setColor) # type: ignore
+        self.ui.pushButton.clicked.connect(self.graphDraw) # type: ignore
+        self.ui.pushButton_2.clicked.connect(self.savePCFig) # type: ignore
+        self.ui.cmb_sort.currentIndexChanged.connect(self.setSort) # type: ignore
+        self.ui.cmb_plot.currentIndexChanged.connect(self.setPlotType) # type: ignore
+        self.ui.cmb_recType.currentIndexChanged.connect(self.setReconstMode) # type: ignore
+        self.ui.cmb_sumDev.currentIndexChanged.connect(self.setSumDev) # type: ignore
+        self.ui.cmb_IP.currentIndexChanged.connect(self.setIPCaxis) # type: ignore
+        self.ui.cmb_IIP.currentIndexChanged.connect(self.setIIPCaxis) # type: ignore
+        self.ui.cmb_IIIP.currentIndexChanged.connect(self.setIIIPCaxis) # type: ignore
+        self.ui.dsb_Id.valueChanged.connect(self.setIdev) # type: ignore
+        self.ui.dsb_IId.valueChanged.connect(self.setIIdev) # type: ignore
+        self.ui.dsb_IIId.valueChanged.connect(self.setIIIdev) # type: ignore
+        self.ui.button_generate.clicked.connect(self.reconstGraph) # type: ignore
+        self.ui.button_saveReconst.clicked.connect(self.saveReconstGraph) # type: ignore
+        self.ui.cmb_FPS.currentIndexChanged.connect(self.setFPSorEFD) # type: ignore
+        self.ui.cmb_subcolor.currentIndexChanged.connect(self.setSubColor) # type: ignore
+        self.ui.cmb_subsort.currentIndexChanged.connect(self.setSubSort) # type: ignore
+        self.ui.cmb_subsubcolor.currentIndexChanged.connect(self.setSubsubColor) # type: ignore
+        self.ui.cmb_subsubsort.currentIndexChanged.connect(self.setSubsubSort) # type: ignore
+        self.ui.rb_none.toggled.connect(self.setCategorize) # type: ignore
+        self.ui.rb_subfolda.toggled.connect(self.setCategorize) # type: ignore
+        self.ui.rb_filename.toggled.connect(self.setCategorize) # type: ignore
+        self.ui.button_sample.clicked.connect(self.setSampleImage) # type: ignore
+        self.ui.button_startsample.clicked.connect(self.startPlayground) # type: ignore
+        self.ui.button_save_sample.clicked.connect(self.saveSample) # type: ignore
         self.setWindowTitle('Grain Shape analyzer')
         #PCA PAGE
         self.PCA_METHOD = ["Fourier Power Spectra","Amplitudes of X and Y ellipses","Elliptic Fourier Descriptors"]
         self.isFPS = 0 # 0:FPS 1:amplitude 2:EFD
         self.FPS_PATH = ""
         self.SAVE_PCA = ""
         self.isCorrelationMatrix = True
         #PC Graph
-        self.isAlreadyGraph = False
+        # self.isAlreadyGraph = False
         self.fig = Figure()
         self.ax1 = self.fig.add_subplot(111)
-        # self.ax1.set_xlabel("X")
-        # self.ax1.set_ylabel("Y")
-        # self.ax1 = self.fig.add_subplot(111)
         self.canv = FigureCanvas(self.fig)
-        self.canv.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding)
+        self.canv.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding)
         self.canv.updateGeometry()
         self.layout = Qw.QGridLayout(self.ui.canvas)
         self.layout.addWidget(self.canv)
         #Reconst shape
         self.isPCAdone = False
         self.isSummaryMODE = True
         self.sumdev = 1.0
@@ -345,17 +393,17 @@
         self.ax31.tick_params(labelleft=False,left=False); self.ax32.tick_params(labelleft=False,left=False); self.ax33.tick_params(labelleft=False,left=False);
         self.ax11.set_xticklabels([]); self.ax12.set_xticklabels([]); self.ax13.set_xticklabels([]); 
         self.ax21.set_xticklabels([]); self.ax22.set_xticklabels([]); self.ax23.set_xticklabels([]); 
         self.ax31.set_xticklabels([]); self.ax32.set_xticklabels([]); self.ax33.set_xticklabels([]); 
         self.canv11 = FigureCanvas(self.fig11); self.canv12 = FigureCanvas(self.fig12); self.canv13 = FigureCanvas(self.fig13);
         self.canv21 = FigureCanvas(self.fig21); self.canv22 = FigureCanvas(self.fig22); self.canv23 = FigureCanvas(self.fig23);
         self.canv31 = FigureCanvas(self.fig31); self.canv32 = FigureCanvas(self.fig32); self.canv33 = FigureCanvas(self.fig33);
-        self.canv11.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding); self.canv12.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding); self.canv13.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding); 
-        self.canv21.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding); self.canv22.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding); self.canv23.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding); 
-        self.canv31.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding); self.canv32.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding); self.canv33.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding); 
+        self.canv11.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding); self.canv12.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding); self.canv13.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding); 
+        self.canv21.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding); self.canv22.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding); self.canv23.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding); 
+        self.canv31.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding); self.canv32.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding); self.canv33.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding); 
         self.canv11.updateGeometry(); self.canv12.updateGeometry(); self.canv13.updateGeometry();
         self.canv21.updateGeometry(); self.canv22.updateGeometry(); self.canv23.updateGeometry();
         self.canv31.updateGeometry(); self.canv32.updateGeometry(); self.canv33.updateGeometry();
         # Add figures to parent view
         self.layout11.addWidget(self.canv11,0,0); self.layout11.addWidget(self.canv12,0,1); self.layout11.addWidget(self.canv13,0,2); 
         self.layout11.addWidget(self.canv21,1,0); self.layout11.addWidget(self.canv22,1,1); self.layout11.addWidget(self.canv23,1,2); 
         self.layout11.addWidget(self.canv31,2,0); self.layout11.addWidget(self.canv32,2,1); self.layout11.addWidget(self.canv33,2,2); 
@@ -375,86 +423,86 @@
         self.figss = Figure();
         self.figss.subplots_adjust(left=0,right=1,bottom=0,top=1)
         self.axss = self.figss.add_subplot(111);
         self.axss.tick_params(labelbottom=False,bottom=False);
         self.axss.tick_params(labelleft=False,left=False);
         self.axss.set_xticklabels([]);self.axss.set_yticklabels([]);
         self.canvss = FigureCanvas(self.figss);
-        self.canvss.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding);
+        self.canvss.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding);
         self.canvss.updateGeometry();
         self.layout_ss.addWidget(self.canvss,0,0);
 
         #-- Projection gif -----------------
         self.layout_px = Qw.QGridLayout(self.ui.f_proj_x);
         self.figpx = Figure();
         self.figpx.subplots_adjust(left=0,right=1,bottom=0,top=1)
         self.ax_px = self.figpx.add_subplot(111);
         self.ax_px.tick_params(labelbottom=False,bottom=False);
         self.ax_px.tick_params(labelleft=False,left=False);
         self.ax_px.set_xticklabels([]);self.ax_px.set_yticklabels([]);
         self.canvpx = FigureCanvas(self.figpx);
-        self.canvpx.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding);
+        self.canvpx.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding);
         self.canvpx.updateGeometry();
         self.layout_px.addWidget(self.canvpx,0,0);
 
         self.layout_py = Qw.QGridLayout(self.ui.f_proj_y);
         self.figpy = Figure();
         self.figpy.subplots_adjust(left=0,right=1,bottom=0,top=1)
         self.ax_py = self.figpy.add_subplot(111);
         self.ax_py.tick_params(labelbottom=False,bottom=False);
         self.ax_py.tick_params(labelleft=False,left=False);
         self.ax_py.set_xticklabels([]);self.ax_py.set_yticklabels([]);
         self.canvpy = FigureCanvas(self.figpy);
-        self.canvpy.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding);
+        self.canvpy.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding);
         self.canvpy.updateGeometry();
         self.layout_py.addWidget(self.canvpy,0,0);
 
         #-- X, Y, approximation view -------
         self.layout_x = Qw.QGridLayout(self.ui.f_x_sample);
         self.figx = Figure();
         self.ax_x = self.figx.add_subplot(111);
         self.canvx = FigureCanvas(self.figx);
-        self.canvx.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding);
+        self.canvx.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding);
         self.canvx.updateGeometry();
         self.layout_x.addWidget(self.canvx,0,0);
 
         self.layout_y = Qw.QGridLayout(self.ui.f_y_sample);
         self.figy = Figure();
         self.ax_y = self.figy.add_subplot(111);
         self.canvy = FigureCanvas(self.figy);
-        self.canvy.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding);
+        self.canvy.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding);
         self.canvy.updateGeometry();
         self.layout_y.addWidget(self.canvy,0,0);
 
         #-- Reconst -----
         self.layout_rre = Qw.QGridLayout(self.ui.f_r_recon);
         self.fig_rre = Figure();
         self.fig_rre.subplots_adjust(left=0,right=1,bottom=0)
         self.fig_rre.patch.set_visible(False)
         self.ax_rre = self.fig_rre.add_subplot(111);
         self.ax_rre.tick_params(labelbottom=False,bottom=False);
         self.ax_rre.tick_params(labelleft=False,left=False);
         # self.ax_rre.axis('off')
         self.ax_rre.set_xticklabels([]);self.ax_rre.set_yticklabels([]);
         self.canv_rre = FigureCanvas(self.fig_rre);
-        self.canv_rre.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding);
+        self.canv_rre.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding);
         self.canv_rre.updateGeometry();
         self.layout_rre.addWidget(self.canv_rre,0,0);
 
         self.layout_rcom = Qw.QGridLayout(self.ui.f_r_comp);
         self.fig_rcom = Figure();
         self.fig_rcom.subplots_adjust(left=0,right=1,bottom=0)
         self.fig_rcom.patch.set_visible(False)
         self.ax_rcom = self.fig_rcom.add_subplot(111);
         self.ax_rcom.tick_params(labelbottom=False,bottom=False);
         self.ax_rcom.tick_params(labelleft=False,left=False);
         # self.ax_rcom.axis('off')
         self.ax_rcom.set_xticklabels([]);self.ax_rcom.set_yticklabels([]);
         self.canv_rcom = FigureCanvas(self.fig_rcom);
-        self.canv_rcom.setSizePolicy(Qw.QSizePolicy.Expanding, Qw.QSizePolicy.Expanding);
+        self.canv_rcom.setSizePolicy(Qw.QSizePolicy.Policy.Expanding, Qw.QSizePolicy.Policy.Expanding);
         self.canv_rcom.updateGeometry();
         self.layout_rcom.addWidget(self.canv_rcom,0,0);
         self.ui.tabWidget_2.setCurrentIndex(1);
 
 
     def setSampleImage(self):
         path = self.openImageFile()
@@ -591,17 +639,14 @@
         self.ax_py.clear()
         self.ax_px.clear()
         self.ax_rre.clear()
         if self.ui.tabWidget_2.currentIndex() == 1:
             self.ga.start()
         elif self.ui.tabWidget_2.currentIndex() == 3:
             self.gah.start()
-        
-    
-    
     
     def projection(self,frame):
         self.figpx.canvas.draw_idle();
         self.figpy.canvas.draw_idle(); 
         
     def projection_h(self,frame):
         self.fig_rre.canvas.draw_idle();
@@ -659,46 +704,63 @@
             fig,ax_seq= matplotlib.pyplot.subplots()
             ax_seq.set_aspect('equal', 'datalim');
             ax_seq.plot(self.N_list[i][0],self.N_list[i][1],linewidth=0.1,color='black')
             ax_seq.fill(self.N_list[i][0],self.N_list[i][1],color='black',alpha=0.5)
             ax_seq.set_title(r"${\it N}\ =\ $"+num)
             fig.savefig(sequence_name+"seq_"+num+".pdf")
             matplotlib.pyplot.close()
-            # figc,bx_seq= matplotlib.pyplot.subplots()
-            # bx_seq.set_aspect('equal', 'datalim');
-            # bx_seq.plot(self.x_pa_ori,self.y_pa_ori,color='black',alpha=1.0)
-            # bx_seq.fill(self.x_pa_ori,self.y_pa_ori,color='black',alpha=0.5)
-            # x_Na,y_Na = ef.adjustXYCoord(self.N_list[i][0],self.N_list[i][1])
-            # bx_seq.plot(x_Na,-y_Na,color='red',alpha=0.7)
-            # bx_seq.set_title(r"${\it N}\ =\ $"+num)
-            # figc.savefig(sequence_name+"comp"+os.sep+"seq_"+num+"_c.png")
-            
-    #### Set image format PNG, BMP, JPEG
-    def setFormat(self):
-        
-        self.FILE_FORMAT = self.FORMAT_LIST[self.ui.cmb_format.currentIndex()]
-        self.FILE_LIST = [] # Initiate image file list for analysis
-
+    
+    def getImagesFromFolder(self):
+        self.FILE_LIST = []
+        # Log #--------------
+        File_log_str = "Folda Path: " + self.FOLDA_DIR +"\n"
+        # -------------------
         if self.FOLDA_DIR=="":
+            return
+        else:
             # Log #--------------
-            self.onStringChanged("Format: "+self.FILE_FORMAT+"\n"+"Select the Folda Directory"+"\n")
+            File_log_str += "#------------------" + "\n" + "Selected Files" + "\n" + "#------------------" + "\n"
             # -------------------
-        else:
-            files = os.listdir(self.FOLDA_DIR) # All File in selected directory 
-            File_log_str = ""
-            for file in files:
-                index = re.search(self.FILE_FORMAT,file) # Search the image files with the selected format
+            for file in glob.glob(self.FOLDA_DIR+os.sep+"**",recursive=True):
+                index = re.search(self.FILE_FORMAT,file)
+                # iscontdir = re.search('contdir',file)
                 if index:
-                    self.FILE_LIST.append(file[0:-1*len(self.FILE_FORMAT)]) # add image to analyze
+                    self.FILE_LIST.append(file[len(self.FOLDA_DIR)+1:-1*len(self.FILE_FORMAT)])
                     # Log #--------------
-                    File_log_str += "          • " + file[0:-1*len(self.FILE_FORMAT)] + "\n"
+                    File_log_str += "          • " + file[len(self.FOLDA_DIR)+1:-1*len(self.FILE_FORMAT)] + "\n"
                     # -------------------
             # Log #--------------
-            self.onStringChanged("#------------------"+"\n"+"Selected Files"+"\n"+"#------------------"+"\n"+File_log_str+"In total: " + str(len(self.FILE_LIST)) +" " + self.FILE_FORMAT + " files" + "\n")
+            File_log_str += "In total: " + str(len(self.FILE_LIST)) +" " + self.FILE_FORMAT + " files" + "\n"
+            self.onStringChanged(File_log_str)
             # -------------------
+    
+    #### Set image format PNG, BMP, JPEG
+    def setFormat(self):
+        
+        self.FILE_FORMAT = self.FORMAT_LIST[self.ui.cmb_format.currentIndex()]
+        self.getImagesFromFolder()
+        # self.FILE_LIST = [] # Initiate image file list for analysis
+
+        # if self.FOLDA_DIR=="":
+        #     # Log #--------------
+        #     self.onStringChanged("Format: "+self.FILE_FORMAT+"\n"+"Select the Folda Directory"+"\n")
+        #     # -------------------
+        # else:
+        #     files = os.listdir(self.FOLDA_DIR) # All File in selected directory 
+        #     File_log_str = ""
+        #     for file in files:
+        #         index = re.search(self.FILE_FORMAT,file) # Search the image files with the selected format
+        #         if index:
+        #             self.FILE_LIST.append(file[0:-1*len(self.FILE_FORMAT)]) # add image to analyze
+        #             # Log #--------------
+        #             File_log_str += "          • " + file[0:-1*len(self.FILE_FORMAT)] + "\n"
+        #             # -------------------
+        #     # Log #--------------
+        #     self.onStringChanged("#------------------"+"\n"+"Selected Files"+"\n"+"#------------------"+"\n"+File_log_str+"In total: " + str(len(self.FILE_LIST)) +" " + self.FILE_FORMAT + " files" + "\n")
+        #     # -------------------
 
     #### Set categorization method #####
     def setCategorize(self):
         cgnone = self.ui.rb_none.isChecked()
         cgsubfolda = self.ui.rb_subfolda.isChecked()
         cgfilename = self.ui.rb_filename.isChecked()
         if cgnone:
@@ -711,67 +773,42 @@
             self.categorization = 1
         elif cgfilename:
             self.ui.line_header.setEnabled(True)
             self.ui.button_header.setEnabled(True)
             self.categorization = 2
 
     def setFoldaPath(self):
-        self.FILE_LIST = []
+        # self.FILE_LIST = []
         # select Folda
         rootpath = os.path.abspath(os.path.dirname("__file__"))
         self.FOLDA_DIR = Qw.QFileDialog.getExistingDirectory(None,"rootpath",rootpath)
-        # Log #--------------
-        File_log_str = "Folda Path: " + self.FOLDA_DIR +"\n"
-        # -------------------
+        # # Log #--------------
+        # File_log_str = "Folda Path: " + self.FOLDA_DIR +"\n"
+        # # -------------------
         self.ui.line_folda.setText(self.FOLDA_DIR)
-        if self.FOLDA_DIR=="":
-            return
-        else:
-            # Log #--------------
-            File_log_str += "#------------------" + "\n" + "Selected Files" + "\n" + "#------------------" + "\n"
-            # -------------------
-            for file in glob.glob(self.FOLDA_DIR+os.sep+"**",recursive=True):
-                index = re.search(self.FILE_FORMAT,file)
-                # iscontdir = re.search('contdir',file)
-                if index:
-                    self.FILE_LIST.append(file[len(self.FOLDA_DIR)+1:-1*len(self.FILE_FORMAT)])
-                    # Log #--------------
-                    File_log_str += "          • " + file[len(self.FOLDA_DIR)+1:-1*len(self.FILE_FORMAT)] + "\n"
-                    # -------------------
-            # Log #--------------
-            File_log_str += "In total: " + str(len(self.FILE_LIST)) +" " + self.FILE_FORMAT + " files" + "\n"
-            self.onStringChanged(File_log_str)
-            # -------------------
-    #### Set image format PNG, BMP, JPEG
-    # def setFoldaPath(self):
-    #     self.FILE_LIST = []
-    #     rootpath = os.path.abspath(os.path.dirname("__file__"))
-    #     self.FOLDA_DIR = Qw.QFileDialog.getExistingDirectory(None,"rootpath",rootpath)
-    #     # Log #--------------
-    #     File_log_str = "Folda Path: " + self.FOLDA_DIR +"\n"
-    #     # -------------------
-    #     self.ui.line_folda.setText(self.FOLDA_DIR)
-    #     if self.FOLDA_DIR=="":
-    #         return
-    #     else:
-    #         files = os.listdir(self.FOLDA_DIR)
-    #         # Log #--------------
-    #         File_log_str += "#------------------" + "\n" + "Selected Files" + "\n" + "#------------------" + "\n"
-    #         # -------------------
-    #         for file in files:
-    #             index = re.search(self.FILE_FORMAT,file)
-    #             if index:
-    #                 self.FILE_LIST.append(file[0:-1*len(self.FILE_FORMAT)])
-    #                 # Log #--------------
-    #                 File_log_str += "          • " + file[0:-1*len(self.FILE_FORMAT)] + "\n"
-    #                 # -------------------
-    #         # Log #--------------
-    #         File_log_str += "In total: " + str(len(self.FILE_LIST)) +" " + self.FILE_FORMAT + " files" + "\n"
-    #         self.onStringChanged(File_log_str)
-    #         # -------------------
+        self.getImagesFromFolder()
+        # if self.FOLDA_DIR=="":
+        #     return
+        # else:
+        #     # Log #--------------
+        #     File_log_str += "#------------------" + "\n" + "Selected Files" + "\n" + "#------------------" + "\n"
+        #     # -------------------
+        #     for file in glob.glob(self.FOLDA_DIR+os.sep+"**",recursive=True):
+        #         index = re.search(self.FILE_FORMAT,file)
+        #         # iscontdir = re.search('contdir',file)
+        #         if index:
+        #             self.FILE_LIST.append(file[len(self.FOLDA_DIR)+1:-1*len(self.FILE_FORMAT)])
+        #             # Log #--------------
+        #             File_log_str += "          • " + file[len(self.FOLDA_DIR)+1:-1*len(self.FILE_FORMAT)] + "\n"
+        #             # -------------------
+        #     # Log #--------------
+        #     File_log_str += "In total: " + str(len(self.FILE_LIST)) +" " + self.FILE_FORMAT + " files" + "\n"
+        #     self.onStringChanged(File_log_str)
+        #     # -------------------
+  
 
     def setHeaderName(self):
         headername = self.ui.line_header.text()
         # File_log_str = ""
         File_log_str = "<span style=\" font-size:13pt; font-weight:600; color:#FF2219;\" >"
         File_log_str_error = ""
 
@@ -807,49 +844,14 @@
                 File_log_str += "</span>" + "\n"
                 self.onStringChanged(File_log_str)
                 # -------------------
             else:
                 File_log_str += "ERROR: check following file name" + "\n" + File_log_str_error + "\n"
                 File_log_str += "</span>" + "\n"
                 self.onStringChanged(File_log_str)
-
-    # def setHeaderName(self):
-    #     headername = self.ui.line_header.text()
-    #     File_log_str = ""
-    #     File_log_str_error = ""
-    #     if headername == "":
-    #         # Log #--------------
-    #         File_log_str += "Please enter the header name" +"\n"
-    #         self.onStringChanged(File_log_str)
-    #         # -------------------
-    #     elif len(self.FILE_LIST) == 0:
-    #         # Log #--------------
-    #         File_log_str += "Please select file directory first" + "\n"
-    #         self.onStringChanged(File_log_str)
-    #         # -------------------
-    #     else:
-    #         Header_cand = headername.split('_')
-    #         gnum = len(Header_cand) 
-    #         file_contens = True
-    #         for file in self.FILE_LIST:
-    #             if len(file.split('_')) != gnum:
-    #                 file_contens = False
-    #                 # Log #--------------
-    #                 File_log_str_error += str(file) + "\n"
-    #                 # -------------------
-    #         if file_contens:
-    #             self.HEADER_LIST = headername.split('_')
-    #             # Log #--------------
-    #             File_log_str += "Header is assigned." + "\n"
-    #             self.onStringChanged(File_log_str)
-    #             # -------------------
-    #         else:
-    #             File_log_str += "ERROR: check following file name" + "\n" + File_log_str_error + "\n"
-    #             self.onStringChanged(File_log_str)
-
             
     def setSavePath(self):
         rootpath = os.path.abspath(os.path.dirname("__file__"))
         self.SAVE_DIR = Qw.QFileDialog.getExistingDirectory(None,"rootpath",rootpath)
         self.SAVE_PATH = self.SAVE_DIR + os.sep + self.SAVE_FILE_NAME
         self.ui.line_save.setText(self.SAVE_PATH)
         # Log #--------------
@@ -943,27 +945,32 @@
     def onStringChanged(self,value):
         # Log #--------------
         date_log = "<span style=\" font-size:13pt; font-weight:600; color:#8178FF;\" >"
         date_log += datetime.now().strftime("%Y/%m/%d %H:%M:%S")
         date_log += "</span>" + "\n"
         self.ui.logbox.append(date_log)
         self.ui.logbox.append(str(value))
-        self.ui.logbox.moveCursor(Qg.QTextCursor.End)
+        self.ui.logbox.moveCursor(Qg.QTextCursor.MoveOperation.End)
+        # self.ui.logbox.moveCursor(self.ui.logbox.textCursor().End)
         #-------------------
 
     def onStringChangedPCA(self,value):
         # Log #--------------
         date_log = "<span style=\" font-size:13pt; font-weight:600; color:#8178FF;\" >"
         date_log += datetime.now().strftime("%Y/%m/%d %H:%M:%S")
         date_log += "</span>" + "\n"
         self.ui.logbox_pca.append(date_log)
         self.ui.logbox_pca.append(str(value))
-        self.ui.logbox_pca.moveCursor(Qg.QTextCursor.End)
+        self.ui.logbox_pca.moveCursor(Qg.QTextCursor.MoveOperation.End)
         #-------------------
 
+    def onFourierDone(self,path):
+        self.ui.textbox_fpsPath.setText(path) 
+        self.FPS_PATH = path
+    
     def startEFA(self):
         #INITIAL SETTING
         self.FOLDA_DIR = self.ui.line_folda.text()
         self.SAVE_PATH = self.ui.line_save.text()
         #Exception handling
         if self.checkEFASetting():
             return
@@ -975,27 +982,20 @@
             File_log_str += "No File is found" + "\n" +"------------------ end." + "\n"
             self.onStringChanged(File_log_str)
             # -------------------
         else:
             self.ui.progressBar.setMaximum(len(self.FILE_LIST))
             self.update()
             self.onStringChanged(File_log_str)
-            # self.fa.countChanged.connect(self.onCountChanged)
-            # self.fa.stringChanged.connect(self.onStringChanged)
-            # self.fa.stringChangedPCA.connect(self.onStringChangedPCA)
             self.fa.start()
 
     # PCA methods ########################
     def setFPSorEFD(self):
         self.isFPS = self.ui.cmb_FPS.currentIndex()
-        # print(self.ui.cmb_FPS.currentIndex())
-        # if  == 0:
-        #     self.isFPS = 0
-        # elif:
-        #     self.isFPS = False
+        
 
     def setFPSPath(self):
         path = self.openCSVFile()
         if path == '':
             return
         # rootpath = os.path.abspath(os.path.dirname("__file__"))
         # FPS_FOLDA = Qw.QFileDialog.getExistingDirectory(None,"rootpath",rootpath)
@@ -1511,23 +1511,14 @@
             self.ax33.set_aspect('equal', 'datalim')
             self.ax33.set_xlim([-1.5,1.5])
             self.ax33.set_ylim([-1.0,1.0])
 
 
             for i in range(20):
                 if self.isFPS !=2: # FPS or AMp
-                    # pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps1,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps1,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=[[random.random(),random.random(),random.random()]], ax=self.ax11)#,s=0.5)
-                    # pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps2,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps2,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=[[random.random(),random.random(),random.random()]], ax=self.ax12)#,s=0.5)
-                    # pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps3,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps3,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=[[random.random(),random.random(),random.random()]], ax=self.ax13)#,s=0.5)
-                    # pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps4,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps4,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=[[random.random(),random.random(),random.random()]], ax=self.ax21)#,s=0.5)
-                    # pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps5,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps5,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=[[random.random(),random.random(),random.random()]], ax=self.ax22)#,s=0.5)
-                    # pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps6,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps6,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=[[random.random(),random.random(),random.random()]], ax=self.ax23)#,s=0.5)
-                    # pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps7,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps7,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=[[random.random(),random.random(),random.random()]], ax=self.ax31)#,s=0.5)
-                    # pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps8,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps8,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=[[random.random(),random.random(),random.random()]], ax=self.ax32)#,s=0.5)
-                    # pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps9,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps9,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=[[random.random(),random.random(),random.random()]], ax=self.ax33)#,s=0.5)
                     pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps1,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps1,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=np.random.rand(3,), ax=self.ax11)#,s=0.5)
                     pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps2,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps2,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=np.random.rand(3,), ax=self.ax12)#,s=0.5)
                     pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps3,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps3,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=np.random.rand(3,), ax=self.ax13)#,s=0.5)
                     pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps4,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps4,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=np.random.rand(3,), ax=self.ax21)#,s=0.5)
                     pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps5,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps5,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=np.random.rand(3,), ax=self.ax22)#,s=0.5)
                     pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps6,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps6,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=np.random.rand(3,), ax=self.ax23)#,s=0.5)
                     pd.DataFrame({"x":ef.reconstContourCoord(self.N,fps7,self.isFPS)[0],"y":ef.reconstContourCoord(self.N,fps7,self.isFPS)[1]}).plot(kind="line",x="x", y="y",c=np.random.rand(3,), ax=self.ax31)#,s=0.5)
@@ -1617,18 +1608,14 @@
         self.fig21.savefig(file_name+"fig_21.pdf",bbox_inches='tight')
         self.fig22.savefig(file_name+"fig_22.pdf",bbox_inches='tight')
         self.fig23.savefig(file_name+"fig_23.pdf",bbox_inches='tight')
         self.fig31.savefig(file_name+"fig_31.pdf",bbox_inches='tight')
         self.fig32.savefig(file_name+"fig_32.pdf",bbox_inches='tight')
         self.fig33.savefig(file_name+"fig_33.pdf",bbox_inches='tight')
    
-def buildGUI(argv=sys.argv[1:]):
-    print("Python: " + sys.version)
-    print("pandas ver. " + pd.__version__)
-    print("matplotlib ver. " + matplotlib.__version__)
-    print("numpy ver. " + np.__version__)
-    print("PyQt5 ver. " + PYQT_VERSION_STR)
+def buildGUI():
     app = Qw.QApplication(sys.argv)         
     wmain = MyForm()                        
     wmain.show()                            
-    sys.exit(app.exec_())
+    sys.exit(app.exec())
 
+buildGUI()
```

### Comparing `efshape-0.0.5/efshape/fgui.py` & `efshape-0.1.0/efshape/fgui.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,5015 +1,5373 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 0a23 2046 6f72 6d20  f-8 -*-..# Form 
-00000020: 696d 706c 656d 656e 7461 7469 6f6e 2067  implementation g
-00000030: 656e 6572 6174 6564 2066 726f 6d20 7265  enerated from re
-00000040: 6164 696e 6720 7569 2066 696c 6520 2747  ading ui file 'G
-00000050: 7261 696e 416e 616c 797a 6572 2e75 6927  rainAnalyzer.ui'
-00000060: 0a23 0a23 2043 7265 6174 6564 2062 793a  .#.# Created by:
-00000070: 2050 7951 7435 2055 4920 636f 6465 2067   PyQt5 UI code g
-00000080: 656e 6572 6174 6f72 2035 2e31 332e 300a  enerator 5.13.0.
-00000090: 230a 2320 5741 524e 494e 4721 2041 6c6c  #.# WARNING! All
-000000a0: 2063 6861 6e67 6573 206d 6164 6520 696e   changes made in
-000000b0: 2074 6869 7320 6669 6c65 2077 696c 6c20   this file will 
-000000c0: 6265 206c 6f73 7421 0a0a 0a66 726f 6d20  be lost!...from 
-000000d0: 5079 5174 3520 696d 706f 7274 2051 7443  PyQt5 import QtC
-000000e0: 6f72 652c 2051 7447 7569 2c20 5174 5769  ore, QtGui, QtWi
-000000f0: 6467 6574 730a 0a0a 636c 6173 7320 5569  dgets...class Ui
-00000100: 5f4d 6169 6e57 696e 646f 7728 6f62 6a65  _MainWindow(obje
-00000110: 6374 293a 0a20 2020 2064 6566 2073 6574  ct):.    def set
-00000120: 7570 5569 2873 656c 662c 204d 6169 6e57  upUi(self, MainW
-00000130: 696e 646f 7729 3a0a 2020 2020 2020 2020  indow):.        
-00000140: 4d61 696e 5769 6e64 6f77 2e73 6574 4f62  MainWindow.setOb
-00000150: 6a65 6374 4e61 6d65 2822 4d61 696e 5769  jectName("MainWi
-00000160: 6e64 6f77 2229 0a20 2020 2020 2020 204d  ndow").        M
-00000170: 6169 6e57 696e 646f 772e 7265 7369 7a65  ainWindow.resize
-00000180: 2838 3130 2c20 3733 3929 0a20 2020 2020  (810, 739).     
-00000190: 2020 2073 656c 662e 6365 6e74 7261 6c77     self.centralw
-000001a0: 6964 6765 7420 3d20 5174 5769 6467 6574  idget = QtWidget
-000001b0: 732e 5157 6964 6765 7428 4d61 696e 5769  s.QWidget(MainWi
-000001c0: 6e64 6f77 290a 2020 2020 2020 2020 7365  ndow).        se
-000001d0: 6c66 2e63 656e 7472 616c 7769 6467 6574  lf.centralwidget
-000001e0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-000001f0: 6365 6e74 7261 6c77 6964 6765 7422 290a  centralwidget").
-00000200: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
-00000210: 644c 6179 6f75 745f 3720 3d20 5174 5769  dLayout_7 = QtWi
-00000220: 6467 6574 732e 5147 7269 644c 6179 6f75  dgets.QGridLayou
-00000230: 7428 7365 6c66 2e63 656e 7472 616c 7769  t(self.centralwi
-00000240: 6467 6574 290a 2020 2020 2020 2020 7365  dget).        se
-00000250: 6c66 2e67 7269 644c 6179 6f75 745f 372e  lf.gridLayout_7.
-00000260: 7365 744f 626a 6563 744e 616d 6528 2267  setObjectName("g
-00000270: 7269 644c 6179 6f75 745f 3722 290a 2020  ridLayout_7").  
-00000280: 2020 2020 2020 7365 6c66 2e74 6162 5769        self.tabWi
-00000290: 6467 6574 203d 2051 7457 6964 6765 7473  dget = QtWidgets
-000002a0: 2e51 5461 6257 6964 6765 7428 7365 6c66  .QTabWidget(self
-000002b0: 2e63 656e 7472 616c 7769 6467 6574 290a  .centralwidget).
-000002c0: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
-000002d0: 6379 203d 2051 7457 6964 6765 7473 2e51  cy = QtWidgets.Q
-000002e0: 5369 7a65 506f 6c69 6379 2851 7457 6964  SizePolicy(QtWid
-000002f0: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
-00000300: 2e45 7870 616e 6469 6e67 2c20 5174 5769  .Expanding, QtWi
-00000310: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
-00000320: 792e 4578 7061 6e64 696e 6729 0a20 2020  y.Expanding).   
-00000330: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
-00000340: 7365 7448 6f72 697a 6f6e 7461 6c53 7472  setHorizontalStr
-00000350: 6574 6368 2830 290a 2020 2020 2020 2020  etch(0).        
-00000360: 7369 7a65 506f 6c69 6379 2e73 6574 5665  sizePolicy.setVe
-00000370: 7274 6963 616c 5374 7265 7463 6828 3029  rticalStretch(0)
-00000380: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
-00000390: 6963 792e 7365 7448 6569 6768 7446 6f72  icy.setHeightFor
-000003a0: 5769 6474 6828 7365 6c66 2e74 6162 5769  Width(self.tabWi
-000003b0: 6467 6574 2e73 697a 6550 6f6c 6963 7928  dget.sizePolicy(
-000003c0: 292e 6861 7348 6569 6768 7446 6f72 5769  ).hasHeightForWi
-000003d0: 6474 6828 2929 0a20 2020 2020 2020 2073  dth()).        s
-000003e0: 656c 662e 7461 6257 6964 6765 742e 7365  elf.tabWidget.se
-000003f0: 7453 697a 6550 6f6c 6963 7928 7369 7a65  tSizePolicy(size
-00000400: 506f 6c69 6379 290a 2020 2020 2020 2020  Policy).        
-00000410: 7365 6c66 2e74 6162 5769 6467 6574 2e73  self.tabWidget.s
-00000420: 6574 4d69 6e69 6d75 6d53 697a 6528 5174  etMinimumSize(Qt
-00000430: 436f 7265 2e51 5369 7a65 2836 3431 2c20  Core.QSize(641, 
-00000440: 3430 3929 290a 2020 2020 2020 2020 7365  409)).        se
-00000450: 6c66 2e74 6162 5769 6467 6574 2e73 6574  lf.tabWidget.set
-00000460: 5573 6573 5363 726f 6c6c 4275 7474 6f6e  UsesScrollButton
-00000470: 7328 4661 6c73 6529 0a20 2020 2020 2020  s(False).       
-00000480: 2073 656c 662e 7461 6257 6964 6765 742e   self.tabWidget.
-00000490: 7365 744f 626a 6563 744e 616d 6528 2274  setObjectName("t
-000004a0: 6162 5769 6467 6574 2229 0a20 2020 2020  abWidget").     
-000004b0: 2020 2073 656c 662e 7461 625f 3520 3d20     self.tab_5 = 
-000004c0: 5174 5769 6467 6574 732e 5157 6964 6765  QtWidgets.QWidge
-000004d0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-000004e0: 2e74 6162 5f35 2e73 6574 4f62 6a65 6374  .tab_5.setObject
-000004f0: 4e61 6d65 2822 7461 625f 3522 290a 2020  Name("tab_5").  
-00000500: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
-00000510: 6179 6f75 745f 3133 203d 2051 7457 6964  ayout_13 = QtWid
-00000520: 6765 7473 2e51 4772 6964 4c61 796f 7574  gets.QGridLayout
-00000530: 2873 656c 662e 7461 625f 3529 0a20 2020  (self.tab_5).   
-00000540: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
-00000550: 796f 7574 5f31 332e 7365 744f 626a 6563  yout_13.setObjec
-00000560: 744e 616d 6528 2267 7269 644c 6179 6f75  tName("gridLayou
-00000570: 745f 3133 2229 0a20 2020 2020 2020 2073  t_13").        s
-00000580: 656c 662e 7461 6257 6964 6765 745f 3220  elf.tabWidget_2 
-00000590: 3d20 5174 5769 6467 6574 732e 5154 6162  = QtWidgets.QTab
-000005a0: 5769 6467 6574 2873 656c 662e 7461 625f  Widget(self.tab_
-000005b0: 3529 0a20 2020 2020 2020 2073 656c 662e  5).        self.
-000005c0: 7461 6257 6964 6765 745f 322e 7365 744f  tabWidget_2.setO
-000005d0: 626a 6563 744e 616d 6528 2274 6162 5769  bjectName("tabWi
-000005e0: 6467 6574 5f32 2229 0a20 2020 2020 2020  dget_2").       
-000005f0: 2073 656c 662e 7461 625f 3620 3d20 5174   self.tab_6 = Qt
-00000600: 5769 6467 6574 732e 5157 6964 6765 7428  Widgets.QWidget(
-00000610: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-00000620: 6162 5f36 2e73 6574 4f62 6a65 6374 4e61  ab_6.setObjectNa
-00000630: 6d65 2822 7461 625f 3622 290a 2020 2020  me("tab_6").    
-00000640: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-00000650: 6f75 745f 3137 203d 2051 7457 6964 6765  out_17 = QtWidge
-00000660: 7473 2e51 4772 6964 4c61 796f 7574 2873  ts.QGridLayout(s
-00000670: 656c 662e 7461 625f 3629 0a20 2020 2020  elf.tab_6).     
-00000680: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-00000690: 7574 5f31 372e 7365 744f 626a 6563 744e  ut_17.setObjectN
-000006a0: 616d 6528 2267 7269 644c 6179 6f75 745f  ame("gridLayout_
-000006b0: 3137 2229 0a20 2020 2020 2020 2073 656c  17").        sel
-000006c0: 662e 665f 7365 6c65 6374 6564 203d 2051  f.f_selected = Q
-000006d0: 7457 6964 6765 7473 2e51 4672 616d 6528  tWidgets.QFrame(
-000006e0: 7365 6c66 2e74 6162 5f36 290a 2020 2020  self.tab_6).    
-000006f0: 2020 2020 7369 7a65 506f 6c69 6379 203d      sizePolicy =
-00000700: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
-00000710: 506f 6c69 6379 2851 7457 6964 6765 7473  Policy(QtWidgets
-00000720: 2e51 5369 7a65 506f 6c69 6379 2e45 7870  .QSizePolicy.Exp
-00000730: 616e 6469 6e67 2c20 5174 5769 6467 6574  anding, QtWidget
-00000740: 732e 5153 697a 6550 6f6c 6963 792e 4578  s.QSizePolicy.Ex
-00000750: 7061 6e64 696e 6729 0a20 2020 2020 2020  panding).       
-00000760: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
-00000770: 6f72 697a 6f6e 7461 6c53 7472 6574 6368  orizontalStretch
-00000780: 2830 290a 2020 2020 2020 2020 7369 7a65  (0).        size
-00000790: 506f 6c69 6379 2e73 6574 5665 7274 6963  Policy.setVertic
-000007a0: 616c 5374 7265 7463 6828 3029 0a20 2020  alStretch(0).   
-000007b0: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
-000007c0: 7365 7448 6569 6768 7446 6f72 5769 6474  setHeightForWidt
-000007d0: 6828 7365 6c66 2e66 5f73 656c 6563 7465  h(self.f_selecte
-000007e0: 642e 7369 7a65 506f 6c69 6379 2829 2e68  d.sizePolicy().h
-000007f0: 6173 4865 6967 6874 466f 7257 6964 7468  asHeightForWidth
-00000800: 2829 290a 2020 2020 2020 2020 7365 6c66  ()).        self
-00000810: 2e66 5f73 656c 6563 7465 642e 7365 7453  .f_selected.setS
-00000820: 697a 6550 6f6c 6963 7928 7369 7a65 506f  izePolicy(sizePo
-00000830: 6c69 6379 290a 2020 2020 2020 2020 7365  licy).        se
-00000840: 6c66 2e66 5f73 656c 6563 7465 642e 7365  lf.f_selected.se
-00000850: 744d 696e 696d 756d 5369 7a65 2851 7443  tMinimumSize(QtC
-00000860: 6f72 652e 5153 697a 6528 3330 302c 2030  ore.QSize(300, 0
-00000870: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00000880: 665f 7365 6c65 6374 6564 2e73 6574 4672  f_selected.setFr
-00000890: 616d 6553 6861 7065 2851 7457 6964 6765  ameShape(QtWidge
-000008a0: 7473 2e51 4672 616d 652e 5374 796c 6564  ts.QFrame.Styled
-000008b0: 5061 6e65 6c29 0a20 2020 2020 2020 2073  Panel).        s
-000008c0: 656c 662e 665f 7365 6c65 6374 6564 2e73  elf.f_selected.s
-000008d0: 6574 4672 616d 6553 6861 646f 7728 5174  etFrameShadow(Qt
-000008e0: 5769 6467 6574 732e 5146 7261 6d65 2e52  Widgets.QFrame.R
-000008f0: 6169 7365 6429 0a20 2020 2020 2020 2073  aised).        s
-00000900: 656c 662e 665f 7365 6c65 6374 6564 2e73  elf.f_selected.s
-00000910: 6574 4f62 6a65 6374 4e61 6d65 2822 665f  etObjectName("f_
-00000920: 7365 6c65 6374 6564 2229 0a20 2020 2020  selected").     
-00000930: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-00000940: 7574 5f31 372e 6164 6457 6964 6765 7428  ut_17.addWidget(
-00000950: 7365 6c66 2e66 5f73 656c 6563 7465 642c  self.f_selected,
-00000960: 2031 2c20 312c 2031 2c20 3129 0a20 2020   1, 1, 1, 1).   
-00000970: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-00000980: 3337 203d 2051 7457 6964 6765 7473 2e51  37 = QtWidgets.Q
-00000990: 4c61 6265 6c28 7365 6c66 2e74 6162 5f36  Label(self.tab_6
-000009a0: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-000009b0: 6c69 6379 203d 2051 7457 6964 6765 7473  licy = QtWidgets
-000009c0: 2e51 5369 7a65 506f 6c69 6379 2851 7457  .QSizePolicy(QtW
-000009d0: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-000009e0: 6379 2e50 7265 6665 7272 6564 2c20 5174  cy.Preferred, Qt
-000009f0: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
-00000a00: 6963 792e 4d69 6e69 6d75 6d29 0a20 2020  icy.Minimum).   
-00000a10: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
-00000a20: 7365 7448 6f72 697a 6f6e 7461 6c53 7472  setHorizontalStr
-00000a30: 6574 6368 2830 290a 2020 2020 2020 2020  etch(0).        
-00000a40: 7369 7a65 506f 6c69 6379 2e73 6574 5665  sizePolicy.setVe
-00000a50: 7274 6963 616c 5374 7265 7463 6828 3029  rticalStretch(0)
-00000a60: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
-00000a70: 6963 792e 7365 7448 6569 6768 7446 6f72  icy.setHeightFor
-00000a80: 5769 6474 6828 7365 6c66 2e6c 6162 656c  Width(self.label
-00000a90: 5f33 372e 7369 7a65 506f 6c69 6379 2829  _37.sizePolicy()
-00000aa0: 2e68 6173 4865 6967 6874 466f 7257 6964  .hasHeightForWid
-00000ab0: 7468 2829 290a 2020 2020 2020 2020 7365  th()).        se
-00000ac0: 6c66 2e6c 6162 656c 5f33 372e 7365 7453  lf.label_37.setS
-00000ad0: 697a 6550 6f6c 6963 7928 7369 7a65 506f  izePolicy(sizePo
-00000ae0: 6c69 6379 290a 2020 2020 2020 2020 7365  licy).        se
-00000af0: 6c66 2e6c 6162 656c 5f33 372e 7365 744f  lf.label_37.setO
-00000b00: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
-00000b10: 5f33 3722 290a 2020 2020 2020 2020 7365  _37").        se
-00000b20: 6c66 2e67 7269 644c 6179 6f75 745f 3137  lf.gridLayout_17
-00000b30: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
-00000b40: 6c61 6265 6c5f 3337 2c20 302c 2031 2c20  label_37, 0, 1, 
-00000b50: 312c 2031 290a 2020 2020 2020 2020 7365  1, 1).        se
-00000b60: 6c66 2e6c 6162 656c 5f33 3520 3d20 5174  lf.label_35 = Qt
-00000b70: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
-00000b80: 656c 662e 7461 625f 3629 0a20 2020 2020  elf.tab_6).     
-00000b90: 2020 2073 697a 6550 6f6c 6963 7920 3d20     sizePolicy = 
-00000ba0: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
-00000bb0: 6f6c 6963 7928 5174 5769 6467 6574 732e  olicy(QtWidgets.
-00000bc0: 5153 697a 6550 6f6c 6963 792e 5072 6566  QSizePolicy.Pref
-00000bd0: 6572 7265 642c 2051 7457 6964 6765 7473  erred, QtWidgets
-00000be0: 2e51 5369 7a65 506f 6c69 6379 2e4d 696e  .QSizePolicy.Min
-00000bf0: 696d 756d 290a 2020 2020 2020 2020 7369  imum).        si
-00000c00: 7a65 506f 6c69 6379 2e73 6574 486f 7269  zePolicy.setHori
-00000c10: 7a6f 6e74 616c 5374 7265 7463 6828 3029  zontalStretch(0)
-00000c20: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
-00000c30: 6963 792e 7365 7456 6572 7469 6361 6c53  icy.setVerticalS
-00000c40: 7472 6574 6368 2830 290a 2020 2020 2020  tretch(0).      
-00000c50: 2020 7369 7a65 506f 6c69 6379 2e73 6574    sizePolicy.set
-00000c60: 4865 6967 6874 466f 7257 6964 7468 2873  HeightForWidth(s
-00000c70: 656c 662e 6c61 6265 6c5f 3335 2e73 697a  elf.label_35.siz
-00000c80: 6550 6f6c 6963 7928 292e 6861 7348 6569  ePolicy().hasHei
-00000c90: 6768 7446 6f72 5769 6474 6828 2929 0a20  ghtForWidth()). 
-00000ca0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00000cb0: 6c5f 3335 2e73 6574 5369 7a65 506f 6c69  l_35.setSizePoli
-00000cc0: 6379 2873 697a 6550 6f6c 6963 7929 0a20  cy(sizePolicy). 
-00000cd0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00000ce0: 6c5f 3335 2e73 6574 4f62 6a65 6374 4e61  l_35.setObjectNa
-00000cf0: 6d65 2822 6c61 6265 6c5f 3335 2229 0a20  me("label_35"). 
-00000d00: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-00000d10: 4c61 796f 7574 5f31 372e 6164 6457 6964  Layout_17.addWid
-00000d20: 6765 7428 7365 6c66 2e6c 6162 656c 5f33  get(self.label_3
-00000d30: 352c 2030 2c20 302c 2031 2c20 3129 0a20  5, 0, 0, 1, 1). 
-00000d40: 2020 2020 2020 2073 656c 662e 6776 5f6f         self.gv_o
-00000d50: 7269 6769 6e61 6c20 3d20 5174 5769 6467  riginal = QtWidg
-00000d60: 6574 732e 5147 7261 7068 6963 7356 6965  ets.QGraphicsVie
-00000d70: 7728 7365 6c66 2e74 6162 5f36 290a 2020  w(self.tab_6).  
-00000d80: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
-00000d90: 203d 2051 7457 6964 6765 7473 2e51 5369   = QtWidgets.QSi
-00000da0: 7a65 506f 6c69 6379 2851 7457 6964 6765  zePolicy(QtWidge
-00000db0: 7473 2e51 5369 7a65 506f 6c69 6379 2e45  ts.QSizePolicy.E
-00000dc0: 7870 616e 6469 6e67 2c20 5174 5769 6467  xpanding, QtWidg
-00000dd0: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
-00000de0: 4578 7061 6e64 696e 6729 0a20 2020 2020  Expanding).     
-00000df0: 2020 2073 697a 6550 6f6c 6963 792e 7365     sizePolicy.se
-00000e00: 7448 6f72 697a 6f6e 7461 6c53 7472 6574  tHorizontalStret
-00000e10: 6368 2830 290a 2020 2020 2020 2020 7369  ch(0).        si
-00000e20: 7a65 506f 6c69 6379 2e73 6574 5665 7274  zePolicy.setVert
-00000e30: 6963 616c 5374 7265 7463 6828 3029 0a20  icalStretch(0). 
-00000e40: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
-00000e50: 792e 7365 7448 6569 6768 7446 6f72 5769  y.setHeightForWi
-00000e60: 6474 6828 7365 6c66 2e67 765f 6f72 6967  dth(self.gv_orig
-00000e70: 696e 616c 2e73 697a 6550 6f6c 6963 7928  inal.sizePolicy(
-00000e80: 292e 6861 7348 6569 6768 7446 6f72 5769  ).hasHeightForWi
-00000e90: 6474 6828 2929 0a20 2020 2020 2020 2073  dth()).        s
-00000ea0: 656c 662e 6776 5f6f 7269 6769 6e61 6c2e  elf.gv_original.
-00000eb0: 7365 7453 697a 6550 6f6c 6963 7928 7369  setSizePolicy(si
-00000ec0: 7a65 506f 6c69 6379 290a 2020 2020 2020  zePolicy).      
-00000ed0: 2020 7365 6c66 2e67 765f 6f72 6967 696e    self.gv_origin
-00000ee0: 616c 2e73 6574 4d69 6e69 6d75 6d53 697a  al.setMinimumSiz
-00000ef0: 6528 5174 436f 7265 2e51 5369 7a65 2833  e(QtCore.QSize(3
-00000f00: 3030 2c20 3029 290a 2020 2020 2020 2020  00, 0)).        
-00000f10: 7365 6c66 2e67 765f 6f72 6967 696e 616c  self.gv_original
-00000f20: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00000f30: 6776 5f6f 7269 6769 6e61 6c22 290a 2020  gv_original").  
-00000f40: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
-00000f50: 6179 6f75 745f 3137 2e61 6464 5769 6467  ayout_17.addWidg
-00000f60: 6574 2873 656c 662e 6776 5f6f 7269 6769  et(self.gv_origi
-00000f70: 6e61 6c2c 2031 2c20 302c 2031 2c20 3129  nal, 1, 0, 1, 1)
-00000f80: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-00000f90: 6257 6964 6765 745f 322e 6164 6454 6162  bWidget_2.addTab
-00000fa0: 2873 656c 662e 7461 625f 362c 2022 2229  (self.tab_6, "")
-00000fb0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-00000fc0: 625f 3920 3d20 5174 5769 6467 6574 732e  b_9 = QtWidgets.
-00000fd0: 5157 6964 6765 7428 290a 2020 2020 2020  QWidget().      
-00000fe0: 2020 7365 6c66 2e74 6162 5f39 2e73 6574    self.tab_9.set
-00000ff0: 4f62 6a65 6374 4e61 6d65 2822 7461 625f  ObjectName("tab_
-00001000: 3922 290a 2020 2020 2020 2020 7365 6c66  9").        self
-00001010: 2e67 7269 644c 6179 6f75 745f 3139 203d  .gridLayout_19 =
-00001020: 2051 7457 6964 6765 7473 2e51 4772 6964   QtWidgets.QGrid
-00001030: 4c61 796f 7574 2873 656c 662e 7461 625f  Layout(self.tab_
-00001040: 3929 0a20 2020 2020 2020 2073 656c 662e  9).        self.
-00001050: 6772 6964 4c61 796f 7574 5f31 392e 7365  gridLayout_19.se
-00001060: 744f 626a 6563 744e 616d 6528 2267 7269  tObjectName("gri
-00001070: 644c 6179 6f75 745f 3139 2229 0a20 2020  dLayout_19").   
-00001080: 2020 2020 2073 656c 662e 665f 7072 6f6a       self.f_proj
-00001090: 5f78 203d 2051 7457 6964 6765 7473 2e51  _x = QtWidgets.Q
-000010a0: 4672 616d 6528 7365 6c66 2e74 6162 5f39  Frame(self.tab_9
-000010b0: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-000010c0: 6c69 6379 203d 2051 7457 6964 6765 7473  licy = QtWidgets
-000010d0: 2e51 5369 7a65 506f 6c69 6379 2851 7457  .QSizePolicy(QtW
-000010e0: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-000010f0: 6379 2e45 7870 616e 6469 6e67 2c20 5174  cy.Expanding, Qt
-00001100: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
-00001110: 6963 792e 5072 6566 6572 7265 6429 0a20  icy.Preferred). 
-00001120: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
-00001130: 792e 7365 7448 6f72 697a 6f6e 7461 6c53  y.setHorizontalS
-00001140: 7472 6574 6368 2830 290a 2020 2020 2020  tretch(0).      
-00001150: 2020 7369 7a65 506f 6c69 6379 2e73 6574    sizePolicy.set
-00001160: 5665 7274 6963 616c 5374 7265 7463 6828  VerticalStretch(
-00001170: 3029 0a20 2020 2020 2020 2073 697a 6550  0).        sizeP
-00001180: 6f6c 6963 792e 7365 7448 6569 6768 7446  olicy.setHeightF
-00001190: 6f72 5769 6474 6828 7365 6c66 2e66 5f70  orWidth(self.f_p
-000011a0: 726f 6a5f 782e 7369 7a65 506f 6c69 6379  roj_x.sizePolicy
-000011b0: 2829 2e68 6173 4865 6967 6874 466f 7257  ().hasHeightForW
-000011c0: 6964 7468 2829 290a 2020 2020 2020 2020  idth()).        
-000011d0: 7365 6c66 2e66 5f70 726f 6a5f 782e 7365  self.f_proj_x.se
-000011e0: 7453 697a 6550 6f6c 6963 7928 7369 7a65  tSizePolicy(size
-000011f0: 506f 6c69 6379 290a 2020 2020 2020 2020  Policy).        
-00001200: 7365 6c66 2e66 5f70 726f 6a5f 782e 7365  self.f_proj_x.se
-00001210: 7446 7261 6d65 5368 6170 6528 5174 5769  tFrameShape(QtWi
-00001220: 6467 6574 732e 5146 7261 6d65 2e53 7479  dgets.QFrame.Sty
-00001230: 6c65 6450 616e 656c 290a 2020 2020 2020  ledPanel).      
-00001240: 2020 7365 6c66 2e66 5f70 726f 6a5f 782e    self.f_proj_x.
-00001250: 7365 7446 7261 6d65 5368 6164 6f77 2851  setFrameShadow(Q
-00001260: 7457 6964 6765 7473 2e51 4672 616d 652e  tWidgets.QFrame.
-00001270: 5261 6973 6564 290a 2020 2020 2020 2020  Raised).        
-00001280: 7365 6c66 2e66 5f70 726f 6a5f 782e 7365  self.f_proj_x.se
-00001290: 744f 626a 6563 744e 616d 6528 2266 5f70  tObjectName("f_p
-000012a0: 726f 6a5f 7822 290a 2020 2020 2020 2020  roj_x").        
-000012b0: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
-000012c0: 3139 2e61 6464 5769 6467 6574 2873 656c  19.addWidget(sel
-000012d0: 662e 665f 7072 6f6a 5f78 2c20 312c 2031  f.f_proj_x, 1, 1
-000012e0: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
-000012f0: 7365 6c66 2e66 5f70 726f 6a5f 7920 3d20  self.f_proj_y = 
-00001300: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-00001310: 2873 656c 662e 7461 625f 3929 0a20 2020  (self.tab_9).   
-00001320: 2020 2020 2073 697a 6550 6f6c 6963 7920       sizePolicy 
-00001330: 3d20 5174 5769 6467 6574 732e 5153 697a  = QtWidgets.QSiz
-00001340: 6550 6f6c 6963 7928 5174 5769 6467 6574  ePolicy(QtWidget
-00001350: 732e 5153 697a 6550 6f6c 6963 792e 4578  s.QSizePolicy.Ex
-00001360: 7061 6e64 696e 672c 2051 7457 6964 6765  panding, QtWidge
-00001370: 7473 2e51 5369 7a65 506f 6c69 6379 2e50  ts.QSizePolicy.P
-00001380: 7265 6665 7272 6564 290a 2020 2020 2020  referred).      
-00001390: 2020 7369 7a65 506f 6c69 6379 2e73 6574    sizePolicy.set
-000013a0: 486f 7269 7a6f 6e74 616c 5374 7265 7463  HorizontalStretc
-000013b0: 6828 3029 0a20 2020 2020 2020 2073 697a  h(0).        siz
-000013c0: 6550 6f6c 6963 792e 7365 7456 6572 7469  ePolicy.setVerti
-000013d0: 6361 6c53 7472 6574 6368 2830 290a 2020  calStretch(0).  
-000013e0: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
-000013f0: 2e73 6574 4865 6967 6874 466f 7257 6964  .setHeightForWid
-00001400: 7468 2873 656c 662e 665f 7072 6f6a 5f79  th(self.f_proj_y
-00001410: 2e73 697a 6550 6f6c 6963 7928 292e 6861  .sizePolicy().ha
-00001420: 7348 6569 6768 7446 6f72 5769 6474 6828  sHeightForWidth(
-00001430: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00001440: 665f 7072 6f6a 5f79 2e73 6574 5369 7a65  f_proj_y.setSize
-00001450: 506f 6c69 6379 2873 697a 6550 6f6c 6963  Policy(sizePolic
-00001460: 7929 0a20 2020 2020 2020 2073 656c 662e  y).        self.
-00001470: 665f 7072 6f6a 5f79 2e73 6574 4672 616d  f_proj_y.setFram
-00001480: 6553 6861 7065 2851 7457 6964 6765 7473  eShape(QtWidgets
-00001490: 2e51 4672 616d 652e 5374 796c 6564 5061  .QFrame.StyledPa
-000014a0: 6e65 6c29 0a20 2020 2020 2020 2073 656c  nel).        sel
-000014b0: 662e 665f 7072 6f6a 5f79 2e73 6574 4672  f.f_proj_y.setFr
-000014c0: 616d 6553 6861 646f 7728 5174 5769 6467  ameShadow(QtWidg
-000014d0: 6574 732e 5146 7261 6d65 2e52 6169 7365  ets.QFrame.Raise
-000014e0: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-000014f0: 665f 7072 6f6a 5f79 2e73 6574 4f62 6a65  f_proj_y.setObje
-00001500: 6374 4e61 6d65 2822 665f 7072 6f6a 5f79  ctName("f_proj_y
-00001510: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00001520: 6772 6964 4c61 796f 7574 5f31 392e 6164  gridLayout_19.ad
-00001530: 6457 6964 6765 7428 7365 6c66 2e66 5f70  dWidget(self.f_p
-00001540: 726f 6a5f 792c 2030 2c20 312c 2031 2c20  roj_y, 0, 1, 1, 
-00001550: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-00001560: 6c61 6265 6c5f 3432 203d 2051 7457 6964  label_42 = QtWid
-00001570: 6765 7473 2e51 4c61 6265 6c28 7365 6c66  gets.QLabel(self
-00001580: 2e74 6162 5f39 290a 2020 2020 2020 2020  .tab_9).        
-00001590: 7369 7a65 506f 6c69 6379 203d 2051 7457  sizePolicy = QtW
-000015a0: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-000015b0: 6379 2851 7457 6964 6765 7473 2e51 5369  cy(QtWidgets.QSi
-000015c0: 7a65 506f 6c69 6379 2e4d 696e 696d 756d  zePolicy.Minimum
-000015d0: 2c20 5174 5769 6467 6574 732e 5153 697a  , QtWidgets.QSiz
-000015e0: 6550 6f6c 6963 792e 5072 6566 6572 7265  ePolicy.Preferre
-000015f0: 6429 0a20 2020 2020 2020 2073 697a 6550  d).        sizeP
-00001600: 6f6c 6963 792e 7365 7448 6f72 697a 6f6e  olicy.setHorizon
-00001610: 7461 6c53 7472 6574 6368 2830 290a 2020  talStretch(0).  
-00001620: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
-00001630: 2e73 6574 5665 7274 6963 616c 5374 7265  .setVerticalStre
-00001640: 7463 6828 3029 0a20 2020 2020 2020 2073  tch(0).        s
-00001650: 697a 6550 6f6c 6963 792e 7365 7448 6569  izePolicy.setHei
-00001660: 6768 7446 6f72 5769 6474 6828 7365 6c66  ghtForWidth(self
-00001670: 2e6c 6162 656c 5f34 322e 7369 7a65 506f  .label_42.sizePo
-00001680: 6c69 6379 2829 2e68 6173 4865 6967 6874  licy().hasHeight
-00001690: 466f 7257 6964 7468 2829 290a 2020 2020  ForWidth()).    
-000016a0: 2020 2020 7365 6c66 2e6c 6162 656c 5f34      self.label_4
-000016b0: 322e 7365 7453 697a 6550 6f6c 6963 7928  2.setSizePolicy(
-000016c0: 7369 7a65 506f 6c69 6379 290a 2020 2020  sizePolicy).    
-000016d0: 2020 2020 7365 6c66 2e6c 6162 656c 5f34      self.label_4
-000016e0: 322e 7365 744f 626a 6563 744e 616d 6528  2.setObjectName(
-000016f0: 226c 6162 656c 5f34 3222 290a 2020 2020  "label_42").    
-00001700: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-00001710: 6f75 745f 3139 2e61 6464 5769 6467 6574  out_19.addWidget
-00001720: 2873 656c 662e 6c61 6265 6c5f 3432 2c20  (self.label_42, 
-00001730: 302c 2030 2c20 312c 2031 290a 2020 2020  0, 0, 1, 1).    
-00001740: 2020 2020 7365 6c66 2e6c 6162 656c 5f34      self.label_4
-00001750: 3520 3d20 5174 5769 6467 6574 732e 514c  5 = QtWidgets.QL
-00001760: 6162 656c 2873 656c 662e 7461 625f 3929  abel(self.tab_9)
-00001770: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
-00001780: 6963 7920 3d20 5174 5769 6467 6574 732e  icy = QtWidgets.
-00001790: 5153 697a 6550 6f6c 6963 7928 5174 5769  QSizePolicy(QtWi
-000017a0: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
-000017b0: 792e 4d69 6e69 6d75 6d2c 2051 7457 6964  y.Minimum, QtWid
-000017c0: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
-000017d0: 2e50 7265 6665 7272 6564 290a 2020 2020  .Preferred).    
-000017e0: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
-000017f0: 6574 486f 7269 7a6f 6e74 616c 5374 7265  etHorizontalStre
-00001800: 7463 6828 3029 0a20 2020 2020 2020 2073  tch(0).        s
-00001810: 697a 6550 6f6c 6963 792e 7365 7456 6572  izePolicy.setVer
-00001820: 7469 6361 6c53 7472 6574 6368 2830 290a  ticalStretch(0).
-00001830: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
-00001840: 6379 2e73 6574 4865 6967 6874 466f 7257  cy.setHeightForW
-00001850: 6964 7468 2873 656c 662e 6c61 6265 6c5f  idth(self.label_
-00001860: 3435 2e73 697a 6550 6f6c 6963 7928 292e  45.sizePolicy().
-00001870: 6861 7348 6569 6768 7446 6f72 5769 6474  hasHeightForWidt
-00001880: 6828 2929 0a20 2020 2020 2020 2073 656c  h()).        sel
-00001890: 662e 6c61 6265 6c5f 3435 2e73 6574 5369  f.label_45.setSi
-000018a0: 7a65 506f 6c69 6379 2873 697a 6550 6f6c  zePolicy(sizePol
-000018b0: 6963 7929 0a20 2020 2020 2020 2073 656c  icy).        sel
-000018c0: 662e 6c61 6265 6c5f 3435 2e73 6574 4f62  f.label_45.setOb
-000018d0: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
-000018e0: 3435 2229 0a20 2020 2020 2020 2073 656c  45").        sel
-000018f0: 662e 6772 6964 4c61 796f 7574 5f31 392e  f.gridLayout_19.
-00001900: 6164 6457 6964 6765 7428 7365 6c66 2e6c  addWidget(self.l
-00001910: 6162 656c 5f34 352c 2031 2c20 302c 2031  abel_45, 1, 0, 1
-00001920: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
-00001930: 662e 7461 6257 6964 6765 745f 322e 6164  f.tabWidget_2.ad
-00001940: 6454 6162 2873 656c 662e 7461 625f 392c  dTab(self.tab_9,
-00001950: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
-00001960: 662e 7461 625f 3720 3d20 5174 5769 6467  f.tab_7 = QtWidg
-00001970: 6574 732e 5157 6964 6765 7428 290a 2020  ets.QWidget().  
-00001980: 2020 2020 2020 7365 6c66 2e74 6162 5f37        self.tab_7
-00001990: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-000019a0: 7461 625f 3722 290a 2020 2020 2020 2020  tab_7").        
-000019b0: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
-000019c0: 3138 203d 2051 7457 6964 6765 7473 2e51  18 = QtWidgets.Q
-000019d0: 4772 6964 4c61 796f 7574 2873 656c 662e  GridLayout(self.
-000019e0: 7461 625f 3729 0a20 2020 2020 2020 2073  tab_7).        s
-000019f0: 656c 662e 6772 6964 4c61 796f 7574 5f31  elf.gridLayout_1
-00001a00: 382e 7365 744f 626a 6563 744e 616d 6528  8.setObjectName(
-00001a10: 2267 7269 644c 6179 6f75 745f 3138 2229  "gridLayout_18")
-00001a20: 0a20 2020 2020 2020 2073 656c 662e 665f  .        self.f_
-00001a30: 785f 7361 6d70 6c65 203d 2051 7457 6964  x_sample = QtWid
-00001a40: 6765 7473 2e51 4672 616d 6528 7365 6c66  gets.QFrame(self
-00001a50: 2e74 6162 5f37 290a 2020 2020 2020 2020  .tab_7).        
-00001a60: 7369 7a65 506f 6c69 6379 203d 2051 7457  sizePolicy = QtW
-00001a70: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-00001a80: 6379 2851 7457 6964 6765 7473 2e51 5369  cy(QtWidgets.QSi
-00001a90: 7a65 506f 6c69 6379 2e45 7870 616e 6469  zePolicy.Expandi
-00001aa0: 6e67 2c20 5174 5769 6467 6574 732e 5153  ng, QtWidgets.QS
-00001ab0: 697a 6550 6f6c 6963 792e 5072 6566 6572  izePolicy.Prefer
-00001ac0: 7265 6429 0a20 2020 2020 2020 2073 697a  red).        siz
-00001ad0: 6550 6f6c 6963 792e 7365 7448 6f72 697a  ePolicy.setHoriz
-00001ae0: 6f6e 7461 6c53 7472 6574 6368 2830 290a  ontalStretch(0).
-00001af0: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
-00001b00: 6379 2e73 6574 5665 7274 6963 616c 5374  cy.setVerticalSt
-00001b10: 7265 7463 6828 3029 0a20 2020 2020 2020  retch(0).       
-00001b20: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
-00001b30: 6569 6768 7446 6f72 5769 6474 6828 7365  eightForWidth(se
-00001b40: 6c66 2e66 5f78 5f73 616d 706c 652e 7369  lf.f_x_sample.si
-00001b50: 7a65 506f 6c69 6379 2829 2e68 6173 4865  zePolicy().hasHe
-00001b60: 6967 6874 466f 7257 6964 7468 2829 290a  ightForWidth()).
-00001b70: 2020 2020 2020 2020 7365 6c66 2e66 5f78          self.f_x
-00001b80: 5f73 616d 706c 652e 7365 7453 697a 6550  _sample.setSizeP
-00001b90: 6f6c 6963 7928 7369 7a65 506f 6c69 6379  olicy(sizePolicy
-00001ba0: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
-00001bb0: 5f78 5f73 616d 706c 652e 7365 7446 7261  _x_sample.setFra
-00001bc0: 6d65 5368 6170 6528 5174 5769 6467 6574  meShape(QtWidget
-00001bd0: 732e 5146 7261 6d65 2e53 7479 6c65 6450  s.QFrame.StyledP
-00001be0: 616e 656c 290a 2020 2020 2020 2020 7365  anel).        se
-00001bf0: 6c66 2e66 5f78 5f73 616d 706c 652e 7365  lf.f_x_sample.se
-00001c00: 7446 7261 6d65 5368 6164 6f77 2851 7457  tFrameShadow(QtW
-00001c10: 6964 6765 7473 2e51 4672 616d 652e 5261  idgets.QFrame.Ra
-00001c20: 6973 6564 290a 2020 2020 2020 2020 7365  ised).        se
-00001c30: 6c66 2e66 5f78 5f73 616d 706c 652e 7365  lf.f_x_sample.se
-00001c40: 744f 626a 6563 744e 616d 6528 2266 5f78  tObjectName("f_x
-00001c50: 5f73 616d 706c 6522 290a 2020 2020 2020  _sample").      
-00001c60: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-00001c70: 745f 3138 2e61 6464 5769 6467 6574 2873  t_18.addWidget(s
-00001c80: 656c 662e 665f 785f 7361 6d70 6c65 2c20  elf.f_x_sample, 
-00001c90: 322c 2032 2c20 312c 2031 290a 2020 2020  2, 2, 1, 1).    
-00001ca0: 2020 2020 7365 6c66 2e66 5f79 5f73 616d      self.f_y_sam
-00001cb0: 706c 6520 3d20 5174 5769 6467 6574 732e  ple = QtWidgets.
-00001cc0: 5146 7261 6d65 2873 656c 662e 7461 625f  QFrame(self.tab_
-00001cd0: 3729 0a20 2020 2020 2020 2073 697a 6550  7).        sizeP
-00001ce0: 6f6c 6963 7920 3d20 5174 5769 6467 6574  olicy = QtWidget
-00001cf0: 732e 5153 697a 6550 6f6c 6963 7928 5174  s.QSizePolicy(Qt
-00001d00: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
-00001d10: 6963 792e 4578 7061 6e64 696e 672c 2051  icy.Expanding, Q
-00001d20: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
-00001d30: 6c69 6379 2e50 7265 6665 7272 6564 290a  licy.Preferred).
-00001d40: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
-00001d50: 6379 2e73 6574 486f 7269 7a6f 6e74 616c  cy.setHorizontal
-00001d60: 5374 7265 7463 6828 3029 0a20 2020 2020  Stretch(0).     
-00001d70: 2020 2073 697a 6550 6f6c 6963 792e 7365     sizePolicy.se
-00001d80: 7456 6572 7469 6361 6c53 7472 6574 6368  tVerticalStretch
-00001d90: 2830 290a 2020 2020 2020 2020 7369 7a65  (0).        size
-00001da0: 506f 6c69 6379 2e73 6574 4865 6967 6874  Policy.setHeight
-00001db0: 466f 7257 6964 7468 2873 656c 662e 665f  ForWidth(self.f_
-00001dc0: 795f 7361 6d70 6c65 2e73 697a 6550 6f6c  y_sample.sizePol
-00001dd0: 6963 7928 292e 6861 7348 6569 6768 7446  icy().hasHeightF
-00001de0: 6f72 5769 6474 6828 2929 0a20 2020 2020  orWidth()).     
-00001df0: 2020 2073 656c 662e 665f 795f 7361 6d70     self.f_y_samp
-00001e00: 6c65 2e73 6574 5369 7a65 506f 6c69 6379  le.setSizePolicy
-00001e10: 2873 697a 6550 6f6c 6963 7929 0a20 2020  (sizePolicy).   
-00001e20: 2020 2020 2073 656c 662e 665f 795f 7361       self.f_y_sa
-00001e30: 6d70 6c65 2e73 6574 4672 616d 6553 6861  mple.setFrameSha
-00001e40: 7065 2851 7457 6964 6765 7473 2e51 4672  pe(QtWidgets.QFr
-00001e50: 616d 652e 5374 796c 6564 5061 6e65 6c29  ame.StyledPanel)
-00001e60: 0a20 2020 2020 2020 2073 656c 662e 665f  .        self.f_
-00001e70: 795f 7361 6d70 6c65 2e73 6574 4672 616d  y_sample.setFram
-00001e80: 6553 6861 646f 7728 5174 5769 6467 6574  eShadow(QtWidget
-00001e90: 732e 5146 7261 6d65 2e52 6169 7365 6429  s.QFrame.Raised)
-00001ea0: 0a20 2020 2020 2020 2073 656c 662e 665f  .        self.f_
-00001eb0: 795f 7361 6d70 6c65 2e73 6574 4f62 6a65  y_sample.setObje
-00001ec0: 6374 4e61 6d65 2822 665f 795f 7361 6d70  ctName("f_y_samp
-00001ed0: 6c65 2229 0a20 2020 2020 2020 2073 656c  le").        sel
-00001ee0: 662e 6772 6964 4c61 796f 7574 5f31 382e  f.gridLayout_18.
-00001ef0: 6164 6457 6964 6765 7428 7365 6c66 2e66  addWidget(self.f
-00001f00: 5f79 5f73 616d 706c 652c 2030 2c20 322c  _y_sample, 0, 2,
-00001f10: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
-00001f20: 656c 662e 6c61 6265 6c5f 3431 203d 2051  elf.label_41 = Q
-00001f30: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
-00001f40: 7365 6c66 2e74 6162 5f37 290a 2020 2020  self.tab_7).    
-00001f50: 2020 2020 7369 7a65 506f 6c69 6379 203d      sizePolicy =
-00001f60: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
-00001f70: 506f 6c69 6379 2851 7457 6964 6765 7473  Policy(QtWidgets
-00001f80: 2e51 5369 7a65 506f 6c69 6379 2e4d 696e  .QSizePolicy.Min
-00001f90: 696d 756d 2c20 5174 5769 6467 6574 732e  imum, QtWidgets.
-00001fa0: 5153 697a 6550 6f6c 6963 792e 5072 6566  QSizePolicy.Pref
-00001fb0: 6572 7265 6429 0a20 2020 2020 2020 2073  erred).        s
-00001fc0: 697a 6550 6f6c 6963 792e 7365 7448 6f72  izePolicy.setHor
-00001fd0: 697a 6f6e 7461 6c53 7472 6574 6368 2830  izontalStretch(0
-00001fe0: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-00001ff0: 6c69 6379 2e73 6574 5665 7274 6963 616c  licy.setVertical
-00002000: 5374 7265 7463 6828 3029 0a20 2020 2020  Stretch(0).     
-00002010: 2020 2073 697a 6550 6f6c 6963 792e 7365     sizePolicy.se
-00002020: 7448 6569 6768 7446 6f72 5769 6474 6828  tHeightForWidth(
-00002030: 7365 6c66 2e6c 6162 656c 5f34 312e 7369  self.label_41.si
-00002040: 7a65 506f 6c69 6379 2829 2e68 6173 4865  zePolicy().hasHe
-00002050: 6967 6874 466f 7257 6964 7468 2829 290a  ightForWidth()).
-00002060: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00002070: 656c 5f34 312e 7365 7453 697a 6550 6f6c  el_41.setSizePol
-00002080: 6963 7928 7369 7a65 506f 6c69 6379 290a  icy(sizePolicy).
-00002090: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-000020a0: 656c 5f34 312e 7365 744f 626a 6563 744e  el_41.setObjectN
-000020b0: 616d 6528 226c 6162 656c 5f34 3122 290a  ame("label_41").
-000020c0: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
-000020d0: 644c 6179 6f75 745f 3138 2e61 6464 5769  dLayout_18.addWi
-000020e0: 6467 6574 2873 656c 662e 6c61 6265 6c5f  dget(self.label_
-000020f0: 3431 2c20 302c 2031 2c20 312c 2031 290a  41, 0, 1, 1, 1).
-00002100: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00002110: 656c 5f34 3020 3d20 5174 5769 6467 6574  el_40 = QtWidget
-00002120: 732e 514c 6162 656c 2873 656c 662e 7461  s.QLabel(self.ta
-00002130: 625f 3729 0a20 2020 2020 2020 2073 697a  b_7).        siz
-00002140: 6550 6f6c 6963 7920 3d20 5174 5769 6467  ePolicy = QtWidg
-00002150: 6574 732e 5153 697a 6550 6f6c 6963 7928  ets.QSizePolicy(
-00002160: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
-00002170: 6f6c 6963 792e 4d69 6e69 6d75 6d2c 2051  olicy.Minimum, Q
-00002180: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
-00002190: 6c69 6379 2e50 7265 6665 7272 6564 290a  licy.Preferred).
-000021a0: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
-000021b0: 6379 2e73 6574 486f 7269 7a6f 6e74 616c  cy.setHorizontal
-000021c0: 5374 7265 7463 6828 3029 0a20 2020 2020  Stretch(0).     
-000021d0: 2020 2073 697a 6550 6f6c 6963 792e 7365     sizePolicy.se
-000021e0: 7456 6572 7469 6361 6c53 7472 6574 6368  tVerticalStretch
-000021f0: 2830 290a 2020 2020 2020 2020 7369 7a65  (0).        size
-00002200: 506f 6c69 6379 2e73 6574 4865 6967 6874  Policy.setHeight
-00002210: 466f 7257 6964 7468 2873 656c 662e 6c61  ForWidth(self.la
-00002220: 6265 6c5f 3430 2e73 697a 6550 6f6c 6963  bel_40.sizePolic
-00002230: 7928 292e 6861 7348 6569 6768 7446 6f72  y().hasHeightFor
-00002240: 5769 6474 6828 2929 0a20 2020 2020 2020  Width()).       
-00002250: 2073 656c 662e 6c61 6265 6c5f 3430 2e73   self.label_40.s
-00002260: 6574 5369 7a65 506f 6c69 6379 2873 697a  etSizePolicy(siz
-00002270: 6550 6f6c 6963 7929 0a20 2020 2020 2020  ePolicy).       
-00002280: 2073 656c 662e 6c61 6265 6c5f 3430 2e73   self.label_40.s
-00002290: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
-000022a0: 6265 6c5f 3430 2229 0a20 2020 2020 2020  bel_40").       
-000022b0: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
-000022c0: 5f31 382e 6164 6457 6964 6765 7428 7365  _18.addWidget(se
-000022d0: 6c66 2e6c 6162 656c 5f34 302c 2032 2c20  lf.label_40, 2, 
-000022e0: 312c 2031 2c20 3129 0a20 2020 2020 2020  1, 1, 1).       
-000022f0: 2073 656c 662e 7461 6257 6964 6765 745f   self.tabWidget_
-00002300: 322e 6164 6454 6162 2873 656c 662e 7461  2.addTab(self.ta
-00002310: 625f 372c 2022 2229 0a20 2020 2020 2020  b_7, "").       
-00002320: 2073 656c 662e 7461 625f 3820 3d20 5174   self.tab_8 = Qt
-00002330: 5769 6467 6574 732e 5157 6964 6765 7428  Widgets.QWidget(
-00002340: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-00002350: 6162 5f38 2e73 6574 4f62 6a65 6374 4e61  ab_8.setObjectNa
-00002360: 6d65 2822 7461 625f 3822 290a 2020 2020  me("tab_8").    
-00002370: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-00002380: 6f75 745f 3136 203d 2051 7457 6964 6765  out_16 = QtWidge
-00002390: 7473 2e51 4772 6964 4c61 796f 7574 2873  ts.QGridLayout(s
-000023a0: 656c 662e 7461 625f 3829 0a20 2020 2020  elf.tab_8).     
-000023b0: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-000023c0: 7574 5f31 362e 7365 744f 626a 6563 744e  ut_16.setObjectN
-000023d0: 616d 6528 2267 7269 644c 6179 6f75 745f  ame("gridLayout_
-000023e0: 3136 2229 0a20 2020 2020 2020 2073 656c  16").        sel
-000023f0: 662e 6c61 6265 6c5f 3434 203d 2051 7457  f.label_44 = QtW
-00002400: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
-00002410: 6c66 2e74 6162 5f38 290a 2020 2020 2020  lf.tab_8).      
-00002420: 2020 7365 6c66 2e6c 6162 656c 5f34 342e    self.label_44.
-00002430: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
-00002440: 6162 656c 5f34 3422 290a 2020 2020 2020  abel_44").      
-00002450: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-00002460: 745f 3136 2e61 6464 5769 6467 6574 2873  t_16.addWidget(s
-00002470: 656c 662e 6c61 6265 6c5f 3434 2c20 302c  elf.label_44, 0,
-00002480: 2031 2c20 312c 2031 290a 2020 2020 2020   1, 1, 1).      
-00002490: 2020 7365 6c66 2e6c 6162 656c 5f34 3320    self.label_43 
-000024a0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-000024b0: 656c 2873 656c 662e 7461 625f 3829 0a20  el(self.tab_8). 
-000024c0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-000024d0: 6c5f 3433 2e73 6574 4f62 6a65 6374 4e61  l_43.setObjectNa
-000024e0: 6d65 2822 6c61 6265 6c5f 3433 2229 0a20  me("label_43"). 
-000024f0: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-00002500: 4c61 796f 7574 5f31 362e 6164 6457 6964  Layout_16.addWid
-00002510: 6765 7428 7365 6c66 2e6c 6162 656c 5f34  get(self.label_4
-00002520: 332c 2030 2c20 302c 2031 2c20 3129 0a20  3, 0, 0, 1, 1). 
-00002530: 2020 2020 2020 2073 656c 662e 665f 725f         self.f_r_
-00002540: 636f 6d70 203d 2051 7457 6964 6765 7473  comp = QtWidgets
-00002550: 2e51 4672 616d 6528 7365 6c66 2e74 6162  .QFrame(self.tab
-00002560: 5f38 290a 2020 2020 2020 2020 7369 7a65  _8).        size
-00002570: 506f 6c69 6379 203d 2051 7457 6964 6765  Policy = QtWidge
-00002580: 7473 2e51 5369 7a65 506f 6c69 6379 2851  ts.QSizePolicy(Q
-00002590: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
-000025a0: 6c69 6379 2e50 7265 6665 7272 6564 2c20  licy.Preferred, 
-000025b0: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
-000025c0: 6f6c 6963 792e 4578 7061 6e64 696e 6729  olicy.Expanding)
-000025d0: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
-000025e0: 6963 792e 7365 7448 6f72 697a 6f6e 7461  icy.setHorizonta
-000025f0: 6c53 7472 6574 6368 2830 290a 2020 2020  lStretch(0).    
-00002600: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
-00002610: 6574 5665 7274 6963 616c 5374 7265 7463  etVerticalStretc
-00002620: 6828 3029 0a20 2020 2020 2020 2073 697a  h(0).        siz
-00002630: 6550 6f6c 6963 792e 7365 7448 6569 6768  ePolicy.setHeigh
-00002640: 7446 6f72 5769 6474 6828 7365 6c66 2e66  tForWidth(self.f
-00002650: 5f72 5f63 6f6d 702e 7369 7a65 506f 6c69  _r_comp.sizePoli
-00002660: 6379 2829 2e68 6173 4865 6967 6874 466f  cy().hasHeightFo
-00002670: 7257 6964 7468 2829 290a 2020 2020 2020  rWidth()).      
-00002680: 2020 7365 6c66 2e66 5f72 5f63 6f6d 702e    self.f_r_comp.
-00002690: 7365 7453 697a 6550 6f6c 6963 7928 7369  setSizePolicy(si
-000026a0: 7a65 506f 6c69 6379 290a 2020 2020 2020  zePolicy).      
-000026b0: 2020 7365 6c66 2e66 5f72 5f63 6f6d 702e    self.f_r_comp.
-000026c0: 7365 7441 7574 6f46 696c 6c42 6163 6b67  setAutoFillBackg
-000026d0: 726f 756e 6428 5472 7565 290a 2020 2020  round(True).    
-000026e0: 2020 2020 7365 6c66 2e66 5f72 5f63 6f6d      self.f_r_com
-000026f0: 702e 7365 7446 7261 6d65 5368 6170 6528  p.setFrameShape(
-00002700: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-00002710: 2e53 7479 6c65 6450 616e 656c 290a 2020  .StyledPanel).  
-00002720: 2020 2020 2020 7365 6c66 2e66 5f72 5f63        self.f_r_c
-00002730: 6f6d 702e 7365 7446 7261 6d65 5368 6164  omp.setFrameShad
-00002740: 6f77 2851 7457 6964 6765 7473 2e51 4672  ow(QtWidgets.QFr
-00002750: 616d 652e 5261 6973 6564 290a 2020 2020  ame.Raised).    
-00002760: 2020 2020 7365 6c66 2e66 5f72 5f63 6f6d      self.f_r_com
-00002770: 702e 7365 744f 626a 6563 744e 616d 6528  p.setObjectName(
-00002780: 2266 5f72 5f63 6f6d 7022 290a 2020 2020  "f_r_comp").    
-00002790: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-000027a0: 6f75 745f 3136 2e61 6464 5769 6467 6574  out_16.addWidget
-000027b0: 2873 656c 662e 665f 725f 636f 6d70 2c20  (self.f_r_comp, 
-000027c0: 312c 2031 2c20 312c 2031 290a 2020 2020  1, 1, 1, 1).    
-000027d0: 2020 2020 7365 6c66 2e66 5f72 5f72 6563      self.f_r_rec
-000027e0: 6f6e 203d 2051 7457 6964 6765 7473 2e51  on = QtWidgets.Q
-000027f0: 4672 616d 6528 7365 6c66 2e74 6162 5f38  Frame(self.tab_8
-00002800: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-00002810: 6c69 6379 203d 2051 7457 6964 6765 7473  licy = QtWidgets
-00002820: 2e51 5369 7a65 506f 6c69 6379 2851 7457  .QSizePolicy(QtW
-00002830: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-00002840: 6379 2e50 7265 6665 7272 6564 2c20 5174  cy.Preferred, Qt
-00002850: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
-00002860: 6963 792e 4578 7061 6e64 696e 6729 0a20  icy.Expanding). 
-00002870: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
-00002880: 792e 7365 7448 6f72 697a 6f6e 7461 6c53  y.setHorizontalS
-00002890: 7472 6574 6368 2830 290a 2020 2020 2020  tretch(0).      
-000028a0: 2020 7369 7a65 506f 6c69 6379 2e73 6574    sizePolicy.set
-000028b0: 5665 7274 6963 616c 5374 7265 7463 6828  VerticalStretch(
-000028c0: 3029 0a20 2020 2020 2020 2073 697a 6550  0).        sizeP
-000028d0: 6f6c 6963 792e 7365 7448 6569 6768 7446  olicy.setHeightF
-000028e0: 6f72 5769 6474 6828 7365 6c66 2e66 5f72  orWidth(self.f_r
-000028f0: 5f72 6563 6f6e 2e73 697a 6550 6f6c 6963  _recon.sizePolic
-00002900: 7928 292e 6861 7348 6569 6768 7446 6f72  y().hasHeightFor
-00002910: 5769 6474 6828 2929 0a20 2020 2020 2020  Width()).       
-00002920: 2073 656c 662e 665f 725f 7265 636f 6e2e   self.f_r_recon.
-00002930: 7365 7453 697a 6550 6f6c 6963 7928 7369  setSizePolicy(si
-00002940: 7a65 506f 6c69 6379 290a 2020 2020 2020  zePolicy).      
-00002950: 2020 7365 6c66 2e66 5f72 5f72 6563 6f6e    self.f_r_recon
-00002960: 2e73 6574 4175 746f 4669 6c6c 4261 636b  .setAutoFillBack
-00002970: 6772 6f75 6e64 2854 7275 6529 0a20 2020  ground(True).   
-00002980: 2020 2020 2073 656c 662e 665f 725f 7265       self.f_r_re
-00002990: 636f 6e2e 7365 7446 7261 6d65 5368 6170  con.setFrameShap
-000029a0: 6528 5174 5769 6467 6574 732e 5146 7261  e(QtWidgets.QFra
-000029b0: 6d65 2e53 7479 6c65 6450 616e 656c 290a  me.StyledPanel).
-000029c0: 2020 2020 2020 2020 7365 6c66 2e66 5f72          self.f_r
-000029d0: 5f72 6563 6f6e 2e73 6574 4672 616d 6553  _recon.setFrameS
-000029e0: 6861 646f 7728 5174 5769 6467 6574 732e  hadow(QtWidgets.
-000029f0: 5146 7261 6d65 2e52 6169 7365 6429 0a20  QFrame.Raised). 
-00002a00: 2020 2020 2020 2073 656c 662e 665f 725f         self.f_r_
-00002a10: 7265 636f 6e2e 7365 744f 626a 6563 744e  recon.setObjectN
-00002a20: 616d 6528 2266 5f72 5f72 6563 6f6e 2229  ame("f_r_recon")
-00002a30: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00002a40: 6964 4c61 796f 7574 5f31 362e 6164 6457  idLayout_16.addW
-00002a50: 6964 6765 7428 7365 6c66 2e66 5f72 5f72  idget(self.f_r_r
-00002a60: 6563 6f6e 2c20 312c 2030 2c20 312c 2031  econ, 1, 0, 1, 1
-00002a70: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-00002a80: 6162 5769 6467 6574 5f32 2e61 6464 5461  abWidget_2.addTa
-00002a90: 6228 7365 6c66 2e74 6162 5f38 2c20 2222  b(self.tab_8, ""
-00002aa0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-00002ab0: 7269 644c 6179 6f75 745f 3133 2e61 6464  ridLayout_13.add
-00002ac0: 5769 6467 6574 2873 656c 662e 7461 6257  Widget(self.tabW
-00002ad0: 6964 6765 745f 322c 2031 2c20 312c 2033  idget_2, 1, 1, 3
-00002ae0: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
-00002af0: 662e 6672 616d 655f 3320 3d20 5174 5769  f.frame_3 = QtWi
-00002b00: 6467 6574 732e 5146 7261 6d65 2873 656c  dgets.QFrame(sel
-00002b10: 662e 7461 625f 3529 0a20 2020 2020 2020  f.tab_5).       
-00002b20: 2073 697a 6550 6f6c 6963 7920 3d20 5174   sizePolicy = Qt
-00002b30: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
-00002b40: 6963 7928 5174 5769 6467 6574 732e 5153  icy(QtWidgets.QS
-00002b50: 697a 6550 6f6c 6963 792e 4d69 6e69 6d75  izePolicy.Minimu
-00002b60: 6d2c 2051 7457 6964 6765 7473 2e51 5369  m, QtWidgets.QSi
-00002b70: 7a65 506f 6c69 6379 2e4d 696e 696d 756d  zePolicy.Minimum
-00002b80: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-00002b90: 6c69 6379 2e73 6574 486f 7269 7a6f 6e74  licy.setHorizont
-00002ba0: 616c 5374 7265 7463 6828 3029 0a20 2020  alStretch(0).   
-00002bb0: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
-00002bc0: 7365 7456 6572 7469 6361 6c53 7472 6574  setVerticalStret
-00002bd0: 6368 2830 290a 2020 2020 2020 2020 7369  ch(0).        si
-00002be0: 7a65 506f 6c69 6379 2e73 6574 4865 6967  zePolicy.setHeig
-00002bf0: 6874 466f 7257 6964 7468 2873 656c 662e  htForWidth(self.
-00002c00: 6672 616d 655f 332e 7369 7a65 506f 6c69  frame_3.sizePoli
-00002c10: 6379 2829 2e68 6173 4865 6967 6874 466f  cy().hasHeightFo
-00002c20: 7257 6964 7468 2829 290a 2020 2020 2020  rWidth()).      
-00002c30: 2020 7365 6c66 2e66 7261 6d65 5f33 2e73    self.frame_3.s
-00002c40: 6574 5369 7a65 506f 6c69 6379 2873 697a  etSizePolicy(siz
-00002c50: 6550 6f6c 6963 7929 0a20 2020 2020 2020  ePolicy).       
-00002c60: 2073 656c 662e 6672 616d 655f 332e 7365   self.frame_3.se
-00002c70: 744d 696e 696d 756d 5369 7a65 2851 7443  tMinimumSize(QtC
-00002c80: 6f72 652e 5153 697a 6528 302c 2031 3530  ore.QSize(0, 150
-00002c90: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00002ca0: 6672 616d 655f 332e 7365 7446 7261 6d65  frame_3.setFrame
-00002cb0: 5368 6170 6528 5174 5769 6467 6574 732e  Shape(QtWidgets.
-00002cc0: 5146 7261 6d65 2e53 7479 6c65 6450 616e  QFrame.StyledPan
-00002cd0: 656c 290a 2020 2020 2020 2020 7365 6c66  el).        self
-00002ce0: 2e66 7261 6d65 5f33 2e73 6574 4672 616d  .frame_3.setFram
-00002cf0: 6553 6861 646f 7728 5174 5769 6467 6574  eShadow(QtWidget
-00002d00: 732e 5146 7261 6d65 2e52 6169 7365 6429  s.QFrame.Raised)
-00002d10: 0a20 2020 2020 2020 2073 656c 662e 6672  .        self.fr
-00002d20: 616d 655f 332e 7365 744f 626a 6563 744e  ame_3.setObjectN
-00002d30: 616d 6528 2266 7261 6d65 5f33 2229 0a20  ame("frame_3"). 
-00002d40: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-00002d50: 4c61 796f 7574 5f31 3420 3d20 5174 5769  Layout_14 = QtWi
-00002d60: 6467 6574 732e 5147 7269 644c 6179 6f75  dgets.QGridLayou
-00002d70: 7428 7365 6c66 2e66 7261 6d65 5f33 290a  t(self.frame_3).
-00002d80: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
-00002d90: 644c 6179 6f75 745f 3134 2e73 6574 4f62  dLayout_14.setOb
-00002da0: 6a65 6374 4e61 6d65 2822 6772 6964 4c61  jectName("gridLa
-00002db0: 796f 7574 5f31 3422 290a 2020 2020 2020  yout_14").      
-00002dc0: 2020 7365 6c66 2e63 625f 4247 435f 7361    self.cb_BGC_sa
-00002dd0: 6d70 6c65 203d 2051 7457 6964 6765 7473  mple = QtWidgets
-00002de0: 2e51 436f 6d62 6f42 6f78 2873 656c 662e  .QComboBox(self.
-00002df0: 6672 616d 655f 3329 0a20 2020 2020 2020  frame_3).       
-00002e00: 2073 656c 662e 6362 5f42 4743 5f73 616d   self.cb_BGC_sam
-00002e10: 706c 652e 7365 744f 626a 6563 744e 616d  ple.setObjectNam
-00002e20: 6528 2263 625f 4247 435f 7361 6d70 6c65  e("cb_BGC_sample
-00002e30: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00002e40: 6362 5f42 4743 5f73 616d 706c 652e 6164  cb_BGC_sample.ad
-00002e50: 6449 7465 6d28 2222 290a 2020 2020 2020  dItem("").      
-00002e60: 2020 7365 6c66 2e63 625f 4247 435f 7361    self.cb_BGC_sa
-00002e70: 6d70 6c65 2e61 6464 4974 656d 2822 2229  mple.addItem("")
-00002e80: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00002e90: 6964 4c61 796f 7574 5f31 342e 6164 6457  idLayout_14.addW
-00002ea0: 6964 6765 7428 7365 6c66 2e63 625f 4247  idget(self.cb_BG
-00002eb0: 435f 7361 6d70 6c65 2c20 332c 2031 2c20  C_sample, 3, 1, 
-00002ec0: 312c 2031 290a 2020 2020 2020 2020 7365  1, 1).        se
-00002ed0: 6c66 2e6c 6162 656c 5f33 3920 3d20 5174  lf.label_39 = Qt
-00002ee0: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
-00002ef0: 656c 662e 6672 616d 655f 3329 0a20 2020  elf.frame_3).   
-00002f00: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-00002f10: 3339 2e73 6574 4f62 6a65 6374 4e61 6d65  39.setObjectName
-00002f20: 2822 6c61 6265 6c5f 3339 2229 0a20 2020  ("label_39").   
-00002f30: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
-00002f40: 796f 7574 5f31 342e 6164 6457 6964 6765  yout_14.addWidge
-00002f50: 7428 7365 6c66 2e6c 6162 656c 5f33 392c  t(self.label_39,
-00002f60: 2032 2c20 312c 2031 2c20 3129 0a20 2020   2, 1, 1, 1).   
-00002f70: 2020 2020 2073 656c 662e 7362 5f73 6e75       self.sb_snu
-00002f80: 6d5f 7361 6d70 6c65 203d 2051 7457 6964  m_sample = QtWid
-00002f90: 6765 7473 2e51 5370 696e 426f 7828 7365  gets.QSpinBox(se
-00002fa0: 6c66 2e66 7261 6d65 5f33 290a 2020 2020  lf.frame_3).    
-00002fb0: 2020 2020 7365 6c66 2e73 625f 736e 756d      self.sb_snum
-00002fc0: 5f73 616d 706c 652e 7365 7445 6e61 626c  _sample.setEnabl
-00002fd0: 6564 2846 616c 7365 290a 2020 2020 2020  ed(False).      
-00002fe0: 2020 7365 6c66 2e73 625f 736e 756d 5f73    self.sb_snum_s
-00002ff0: 616d 706c 652e 7365 744f 626a 6563 744e  ample.setObjectN
-00003000: 616d 6528 2273 625f 736e 756d 5f73 616d  ame("sb_snum_sam
-00003010: 706c 6522 290a 2020 2020 2020 2020 7365  ple").        se
-00003020: 6c66 2e67 7269 644c 6179 6f75 745f 3134  lf.gridLayout_14
-00003030: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
-00003040: 7362 5f73 6e75 6d5f 7361 6d70 6c65 2c20  sb_snum_sample, 
-00003050: 332c 2030 2c20 312c 2031 290a 2020 2020  3, 0, 1, 1).    
-00003060: 2020 2020 7365 6c66 2e6c 6162 656c 5f33      self.label_3
-00003070: 3420 3d20 5174 5769 6467 6574 732e 514c  4 = QtWidgets.QL
-00003080: 6162 656c 2873 656c 662e 6672 616d 655f  abel(self.frame_
-00003090: 3329 0a20 2020 2020 2020 2073 697a 6550  3).        sizeP
-000030a0: 6f6c 6963 7920 3d20 5174 5769 6467 6574  olicy = QtWidget
-000030b0: 732e 5153 697a 6550 6f6c 6963 7928 5174  s.QSizePolicy(Qt
-000030c0: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
-000030d0: 6963 792e 5072 6566 6572 7265 642c 2051  icy.Preferred, Q
-000030e0: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
-000030f0: 6c69 6379 2e4d 696e 696d 756d 290a 2020  licy.Minimum).  
-00003100: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
-00003110: 2e73 6574 486f 7269 7a6f 6e74 616c 5374  .setHorizontalSt
-00003120: 7265 7463 6828 3029 0a20 2020 2020 2020  retch(0).       
-00003130: 2073 697a 6550 6f6c 6963 792e 7365 7456   sizePolicy.setV
-00003140: 6572 7469 6361 6c53 7472 6574 6368 2830  erticalStretch(0
-00003150: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-00003160: 6c69 6379 2e73 6574 4865 6967 6874 466f  licy.setHeightFo
-00003170: 7257 6964 7468 2873 656c 662e 6c61 6265  rWidth(self.labe
-00003180: 6c5f 3334 2e73 697a 6550 6f6c 6963 7928  l_34.sizePolicy(
-00003190: 292e 6861 7348 6569 6768 7446 6f72 5769  ).hasHeightForWi
-000031a0: 6474 6828 2929 0a20 2020 2020 2020 2073  dth()).        s
-000031b0: 656c 662e 6c61 6265 6c5f 3334 2e73 6574  elf.label_34.set
-000031c0: 5369 7a65 506f 6c69 6379 2873 697a 6550  SizePolicy(sizeP
-000031d0: 6f6c 6963 7929 0a20 2020 2020 2020 2073  olicy).        s
-000031e0: 656c 662e 6c61 6265 6c5f 3334 2e73 6574  elf.label_34.set
-000031f0: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
-00003200: 6c5f 3334 2229 0a20 2020 2020 2020 2073  l_34").        s
-00003210: 656c 662e 6772 6964 4c61 796f 7574 5f31  elf.gridLayout_1
-00003220: 342e 6164 6457 6964 6765 7428 7365 6c66  4.addWidget(self
-00003230: 2e6c 6162 656c 5f33 342c 2032 2c20 302c  .label_34, 2, 0,
-00003240: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
-00003250: 656c 662e 6c61 6265 6c5f 3333 203d 2051  elf.label_33 = Q
-00003260: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
-00003270: 7365 6c66 2e66 7261 6d65 5f33 290a 2020  self.frame_3).  
-00003280: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
-00003290: 203d 2051 7457 6964 6765 7473 2e51 5369   = QtWidgets.QSi
-000032a0: 7a65 506f 6c69 6379 2851 7457 6964 6765  zePolicy(QtWidge
-000032b0: 7473 2e51 5369 7a65 506f 6c69 6379 2e50  ts.QSizePolicy.P
-000032c0: 7265 6665 7272 6564 2c20 5174 5769 6467  referred, QtWidg
-000032d0: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
-000032e0: 4d69 6e69 6d75 6d29 0a20 2020 2020 2020  Minimum).       
-000032f0: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
-00003300: 6f72 697a 6f6e 7461 6c53 7472 6574 6368  orizontalStretch
-00003310: 2830 290a 2020 2020 2020 2020 7369 7a65  (0).        size
-00003320: 506f 6c69 6379 2e73 6574 5665 7274 6963  Policy.setVertic
-00003330: 616c 5374 7265 7463 6828 3029 0a20 2020  alStretch(0).   
-00003340: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
-00003350: 7365 7448 6569 6768 7446 6f72 5769 6474  setHeightForWidt
-00003360: 6828 7365 6c66 2e6c 6162 656c 5f33 332e  h(self.label_33.
-00003370: 7369 7a65 506f 6c69 6379 2829 2e68 6173  sizePolicy().has
-00003380: 4865 6967 6874 466f 7257 6964 7468 2829  HeightForWidth()
-00003390: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-000033a0: 6162 656c 5f33 332e 7365 7453 697a 6550  abel_33.setSizeP
-000033b0: 6f6c 6963 7928 7369 7a65 506f 6c69 6379  olicy(sizePolicy
-000033c0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-000033d0: 6162 656c 5f33 332e 7365 744f 626a 6563  abel_33.setObjec
-000033e0: 744e 616d 6528 226c 6162 656c 5f33 3322  tName("label_33"
-000033f0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-00003400: 7269 644c 6179 6f75 745f 3134 2e61 6464  ridLayout_14.add
-00003410: 5769 6467 6574 2873 656c 662e 6c61 6265  Widget(self.labe
-00003420: 6c5f 3333 2c20 302c 2030 2c20 312c 2031  l_33, 0, 0, 1, 1
-00003430: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
-00003440: 7574 746f 6e5f 7361 6d70 6c65 203d 2051  utton_sample = Q
-00003450: 7457 6964 6765 7473 2e51 5075 7368 4275  tWidgets.QPushBu
-00003460: 7474 6f6e 2873 656c 662e 6672 616d 655f  tton(self.frame_
-00003470: 3329 0a20 2020 2020 2020 2073 656c 662e  3).        self.
-00003480: 6275 7474 6f6e 5f73 616d 706c 652e 7365  button_sample.se
-00003490: 744f 626a 6563 744e 616d 6528 2262 7574  tObjectName("but
-000034a0: 746f 6e5f 7361 6d70 6c65 2229 0a20 2020  ton_sample").   
+00000000: 2320 466f 726d 2069 6d70 6c65 6d65 6e74  # Form implement
+00000010: 6174 696f 6e20 6765 6e65 7261 7465 6420  ation generated 
+00000020: 6672 6f6d 2072 6561 6469 6e67 2075 6920  from reading ui 
+00000030: 6669 6c65 2027 4772 6169 6e41 6e61 6c79  file 'GrainAnaly
+00000040: 7a65 722e 7569 270a 230a 2320 4372 6561  zer.ui'.#.# Crea
+00000050: 7465 6420 6279 3a20 5079 5174 3620 5549  ted by: PyQt6 UI
+00000060: 2063 6f64 6520 6765 6e65 7261 746f 7220   code generator 
+00000070: 362e 342e 320a 230a 2320 5741 524e 494e  6.4.2.#.# WARNIN
+00000080: 473a 2041 6e79 206d 616e 7561 6c20 6368  G: Any manual ch
+00000090: 616e 6765 7320 6d61 6465 2074 6f20 7468  anges made to th
+000000a0: 6973 2066 696c 6520 7769 6c6c 2062 6520  is file will be 
+000000b0: 6c6f 7374 2077 6865 6e20 7079 7569 6336  lost when pyuic6
+000000c0: 2069 730a 2320 7275 6e20 6167 6169 6e2e   is.# run again.
+000000d0: 2020 446f 206e 6f74 2065 6469 7420 7468    Do not edit th
+000000e0: 6973 2066 696c 6520 756e 6c65 7373 2079  is file unless y
+000000f0: 6f75 206b 6e6f 7720 7768 6174 2079 6f75  ou know what you
+00000100: 2061 7265 2064 6f69 6e67 2e0a 0a0a 6672   are doing....fr
+00000110: 6f6d 2050 7951 7436 2069 6d70 6f72 7420  om PyQt6 import 
+00000120: 5174 436f 7265 2c20 5174 4775 692c 2051  QtCore, QtGui, Q
+00000130: 7457 6964 6765 7473 0a0a 0a63 6c61 7373  tWidgets...class
+00000140: 2055 695f 4d61 696e 5769 6e64 6f77 286f   Ui_MainWindow(o
+00000150: 626a 6563 7429 3a0a 2020 2020 6465 6620  bject):.    def 
+00000160: 7365 7475 7055 6928 7365 6c66 2c20 4d61  setupUi(self, Ma
+00000170: 696e 5769 6e64 6f77 293a 0a20 2020 2020  inWindow):.     
+00000180: 2020 204d 6169 6e57 696e 646f 772e 7365     MainWindow.se
+00000190: 744f 626a 6563 744e 616d 6528 224d 6169  tObjectName("Mai
+000001a0: 6e57 696e 646f 7722 290a 2020 2020 2020  nWindow").      
+000001b0: 2020 4d61 696e 5769 6e64 6f77 2e72 6573    MainWindow.res
+000001c0: 697a 6528 3130 3934 2c20 3830 3629 0a20  ize(1094, 806). 
+000001d0: 2020 2020 2020 2073 656c 662e 6365 6e74         self.cent
+000001e0: 7261 6c77 6964 6765 7420 3d20 5174 5769  ralwidget = QtWi
+000001f0: 6467 6574 732e 5157 6964 6765 7428 7061  dgets.QWidget(pa
+00000200: 7265 6e74 3d4d 6169 6e57 696e 646f 7729  rent=MainWindow)
+00000210: 0a20 2020 2020 2020 2073 656c 662e 6365  .        self.ce
+00000220: 6e74 7261 6c77 6964 6765 742e 7365 744f  ntralwidget.setO
+00000230: 626a 6563 744e 616d 6528 2263 656e 7472  bjectName("centr
+00000240: 616c 7769 6467 6574 2229 0a20 2020 2020  alwidget").     
+00000250: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
+00000260: 7574 5f37 203d 2051 7457 6964 6765 7473  ut_7 = QtWidgets
+00000270: 2e51 4772 6964 4c61 796f 7574 2873 656c  .QGridLayout(sel
+00000280: 662e 6365 6e74 7261 6c77 6964 6765 7429  f.centralwidget)
+00000290: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+000002a0: 6964 4c61 796f 7574 5f37 2e73 6574 4f62  idLayout_7.setOb
+000002b0: 6a65 6374 4e61 6d65 2822 6772 6964 4c61  jectName("gridLa
+000002c0: 796f 7574 5f37 2229 0a20 2020 2020 2020  yout_7").       
+000002d0: 2073 656c 662e 7461 6257 6964 6765 7420   self.tabWidget 
+000002e0: 3d20 5174 5769 6467 6574 732e 5154 6162  = QtWidgets.QTab
+000002f0: 5769 6467 6574 2870 6172 656e 743d 7365  Widget(parent=se
+00000300: 6c66 2e63 656e 7472 616c 7769 6467 6574  lf.centralwidget
+00000310: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
+00000320: 6c69 6379 203d 2051 7457 6964 6765 7473  licy = QtWidgets
+00000330: 2e51 5369 7a65 506f 6c69 6379 2851 7457  .QSizePolicy(QtW
+00000340: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
+00000350: 6379 2e50 6f6c 6963 792e 4578 7061 6e64  cy.Policy.Expand
+00000360: 696e 672c 2051 7457 6964 6765 7473 2e51  ing, QtWidgets.Q
+00000370: 5369 7a65 506f 6c69 6379 2e50 6f6c 6963  SizePolicy.Polic
+00000380: 792e 4578 7061 6e64 696e 6729 0a20 2020  y.Expanding).   
+00000390: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
+000003a0: 7365 7448 6f72 697a 6f6e 7461 6c53 7472  setHorizontalStr
+000003b0: 6574 6368 2830 290a 2020 2020 2020 2020  etch(0).        
+000003c0: 7369 7a65 506f 6c69 6379 2e73 6574 5665  sizePolicy.setVe
+000003d0: 7274 6963 616c 5374 7265 7463 6828 3029  rticalStretch(0)
+000003e0: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+000003f0: 6963 792e 7365 7448 6569 6768 7446 6f72  icy.setHeightFor
+00000400: 5769 6474 6828 7365 6c66 2e74 6162 5769  Width(self.tabWi
+00000410: 6467 6574 2e73 697a 6550 6f6c 6963 7928  dget.sizePolicy(
+00000420: 292e 6861 7348 6569 6768 7446 6f72 5769  ).hasHeightForWi
+00000430: 6474 6828 2929 0a20 2020 2020 2020 2073  dth()).        s
+00000440: 656c 662e 7461 6257 6964 6765 742e 7365  elf.tabWidget.se
+00000450: 7453 697a 6550 6f6c 6963 7928 7369 7a65  tSizePolicy(size
+00000460: 506f 6c69 6379 290a 2020 2020 2020 2020  Policy).        
+00000470: 7365 6c66 2e74 6162 5769 6467 6574 2e73  self.tabWidget.s
+00000480: 6574 4d69 6e69 6d75 6d53 697a 6528 5174  etMinimumSize(Qt
+00000490: 436f 7265 2e51 5369 7a65 2836 3431 2c20  Core.QSize(641, 
+000004a0: 3430 3929 290a 2020 2020 2020 2020 7365  409)).        se
+000004b0: 6c66 2e74 6162 5769 6467 6574 2e73 6574  lf.tabWidget.set
+000004c0: 5573 6573 5363 726f 6c6c 4275 7474 6f6e  UsesScrollButton
+000004d0: 7328 4661 6c73 6529 0a20 2020 2020 2020  s(False).       
+000004e0: 2073 656c 662e 7461 6257 6964 6765 742e   self.tabWidget.
+000004f0: 7365 744f 626a 6563 744e 616d 6528 2274  setObjectName("t
+00000500: 6162 5769 6467 6574 2229 0a20 2020 2020  abWidget").     
+00000510: 2020 2073 656c 662e 7461 625f 3520 3d20     self.tab_5 = 
+00000520: 5174 5769 6467 6574 732e 5157 6964 6765  QtWidgets.QWidge
+00000530: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+00000540: 2e74 6162 5f35 2e73 6574 4f62 6a65 6374  .tab_5.setObject
+00000550: 4e61 6d65 2822 7461 625f 3522 290a 2020  Name("tab_5").  
+00000560: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
+00000570: 6179 6f75 745f 3133 203d 2051 7457 6964  ayout_13 = QtWid
+00000580: 6765 7473 2e51 4772 6964 4c61 796f 7574  gets.QGridLayout
+00000590: 2873 656c 662e 7461 625f 3529 0a20 2020  (self.tab_5).   
+000005a0: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
+000005b0: 796f 7574 5f31 332e 7365 744f 626a 6563  yout_13.setObjec
+000005c0: 744e 616d 6528 2267 7269 644c 6179 6f75  tName("gridLayou
+000005d0: 745f 3133 2229 0a20 2020 2020 2020 2073  t_13").        s
+000005e0: 656c 662e 7461 6257 6964 6765 745f 3220  elf.tabWidget_2 
+000005f0: 3d20 5174 5769 6467 6574 732e 5154 6162  = QtWidgets.QTab
+00000600: 5769 6467 6574 2870 6172 656e 743d 7365  Widget(parent=se
+00000610: 6c66 2e74 6162 5f35 290a 2020 2020 2020  lf.tab_5).      
+00000620: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
+00000630: 5f32 2e73 6574 4f62 6a65 6374 4e61 6d65  _2.setObjectName
+00000640: 2822 7461 6257 6964 6765 745f 3222 290a  ("tabWidget_2").
+00000650: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+00000660: 5f36 203d 2051 7457 6964 6765 7473 2e51  _6 = QtWidgets.Q
+00000670: 5769 6467 6574 2829 0a20 2020 2020 2020  Widget().       
+00000680: 2073 656c 662e 7461 625f 362e 7365 744f   self.tab_6.setO
+00000690: 626a 6563 744e 616d 6528 2274 6162 5f36  bjectName("tab_6
+000006a0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000006b0: 6772 6964 4c61 796f 7574 5f31 3720 3d20  gridLayout_17 = 
+000006c0: 5174 5769 6467 6574 732e 5147 7269 644c  QtWidgets.QGridL
+000006d0: 6179 6f75 7428 7365 6c66 2e74 6162 5f36  ayout(self.tab_6
+000006e0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+000006f0: 7269 644c 6179 6f75 745f 3137 2e73 6574  ridLayout_17.set
+00000700: 4f62 6a65 6374 4e61 6d65 2822 6772 6964  ObjectName("grid
+00000710: 4c61 796f 7574 5f31 3722 290a 2020 2020  Layout_17").    
+00000720: 2020 2020 7365 6c66 2e66 5f73 656c 6563      self.f_selec
+00000730: 7465 6420 3d20 5174 5769 6467 6574 732e  ted = QtWidgets.
+00000740: 5146 7261 6d65 2870 6172 656e 743d 7365  QFrame(parent=se
+00000750: 6c66 2e74 6162 5f36 290a 2020 2020 2020  lf.tab_6).      
+00000760: 2020 7369 7a65 506f 6c69 6379 203d 2051    sizePolicy = Q
+00000770: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
+00000780: 6c69 6379 2851 7457 6964 6765 7473 2e51  licy(QtWidgets.Q
+00000790: 5369 7a65 506f 6c69 6379 2e50 6f6c 6963  SizePolicy.Polic
+000007a0: 792e 4578 7061 6e64 696e 672c 2051 7457  y.Expanding, QtW
+000007b0: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
+000007c0: 6379 2e50 6f6c 6963 792e 4578 7061 6e64  cy.Policy.Expand
+000007d0: 696e 6729 0a20 2020 2020 2020 2073 697a  ing).        siz
+000007e0: 6550 6f6c 6963 792e 7365 7448 6f72 697a  ePolicy.setHoriz
+000007f0: 6f6e 7461 6c53 7472 6574 6368 2830 290a  ontalStretch(0).
+00000800: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
+00000810: 6379 2e73 6574 5665 7274 6963 616c 5374  cy.setVerticalSt
+00000820: 7265 7463 6828 3029 0a20 2020 2020 2020  retch(0).       
+00000830: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
+00000840: 6569 6768 7446 6f72 5769 6474 6828 7365  eightForWidth(se
+00000850: 6c66 2e66 5f73 656c 6563 7465 642e 7369  lf.f_selected.si
+00000860: 7a65 506f 6c69 6379 2829 2e68 6173 4865  zePolicy().hasHe
+00000870: 6967 6874 466f 7257 6964 7468 2829 290a  ightForWidth()).
+00000880: 2020 2020 2020 2020 7365 6c66 2e66 5f73          self.f_s
+00000890: 656c 6563 7465 642e 7365 7453 697a 6550  elected.setSizeP
+000008a0: 6f6c 6963 7928 7369 7a65 506f 6c69 6379  olicy(sizePolicy
+000008b0: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+000008c0: 5f73 656c 6563 7465 642e 7365 744d 696e  _selected.setMin
+000008d0: 696d 756d 5369 7a65 2851 7443 6f72 652e  imumSize(QtCore.
+000008e0: 5153 697a 6528 3330 302c 2030 2929 0a20  QSize(300, 0)). 
+000008f0: 2020 2020 2020 2073 656c 662e 665f 7365         self.f_se
+00000900: 6c65 6374 6564 2e73 6574 4672 616d 6553  lected.setFrameS
+00000910: 6861 7065 2851 7457 6964 6765 7473 2e51  hape(QtWidgets.Q
+00000920: 4672 616d 652e 5368 6170 652e 5374 796c  Frame.Shape.Styl
+00000930: 6564 5061 6e65 6c29 0a20 2020 2020 2020  edPanel).       
+00000940: 2073 656c 662e 665f 7365 6c65 6374 6564   self.f_selected
+00000950: 2e73 6574 4672 616d 6553 6861 646f 7728  .setFrameShadow(
+00000960: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
+00000970: 2e53 6861 646f 772e 5261 6973 6564 290a  .Shadow.Raised).
+00000980: 2020 2020 2020 2020 7365 6c66 2e66 5f73          self.f_s
+00000990: 656c 6563 7465 642e 7365 744f 626a 6563  elected.setObjec
+000009a0: 744e 616d 6528 2266 5f73 656c 6563 7465  tName("f_selecte
+000009b0: 6422 290a 2020 2020 2020 2020 7365 6c66  d").        self
+000009c0: 2e67 7269 644c 6179 6f75 745f 3137 2e61  .gridLayout_17.a
+000009d0: 6464 5769 6467 6574 2873 656c 662e 665f  ddWidget(self.f_
+000009e0: 7365 6c65 6374 6564 2c20 312c 2031 2c20  selected, 1, 1, 
+000009f0: 312c 2031 290a 2020 2020 2020 2020 7365  1, 1).        se
+00000a00: 6c66 2e6c 6162 656c 5f33 3720 3d20 5174  lf.label_37 = Qt
+00000a10: 5769 6467 6574 732e 514c 6162 656c 2870  Widgets.QLabel(p
+00000a20: 6172 656e 743d 7365 6c66 2e74 6162 5f36  arent=self.tab_6
+00000a30: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
+00000a40: 6c69 6379 203d 2051 7457 6964 6765 7473  licy = QtWidgets
+00000a50: 2e51 5369 7a65 506f 6c69 6379 2851 7457  .QSizePolicy(QtW
+00000a60: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
+00000a70: 6379 2e50 6f6c 6963 792e 5072 6566 6572  cy.Policy.Prefer
+00000a80: 7265 642c 2051 7457 6964 6765 7473 2e51  red, QtWidgets.Q
+00000a90: 5369 7a65 506f 6c69 6379 2e50 6f6c 6963  SizePolicy.Polic
+00000aa0: 792e 4d69 6e69 6d75 6d29 0a20 2020 2020  y.Minimum).     
+00000ab0: 2020 2073 697a 6550 6f6c 6963 792e 7365     sizePolicy.se
+00000ac0: 7448 6f72 697a 6f6e 7461 6c53 7472 6574  tHorizontalStret
+00000ad0: 6368 2830 290a 2020 2020 2020 2020 7369  ch(0).        si
+00000ae0: 7a65 506f 6c69 6379 2e73 6574 5665 7274  zePolicy.setVert
+00000af0: 6963 616c 5374 7265 7463 6828 3029 0a20  icalStretch(0). 
+00000b00: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
+00000b10: 792e 7365 7448 6569 6768 7446 6f72 5769  y.setHeightForWi
+00000b20: 6474 6828 7365 6c66 2e6c 6162 656c 5f33  dth(self.label_3
+00000b30: 372e 7369 7a65 506f 6c69 6379 2829 2e68  7.sizePolicy().h
+00000b40: 6173 4865 6967 6874 466f 7257 6964 7468  asHeightForWidth
+00000b50: 2829 290a 2020 2020 2020 2020 7365 6c66  ()).        self
+00000b60: 2e6c 6162 656c 5f33 372e 7365 7453 697a  .label_37.setSiz
+00000b70: 6550 6f6c 6963 7928 7369 7a65 506f 6c69  ePolicy(sizePoli
+00000b80: 6379 290a 2020 2020 2020 2020 7365 6c66  cy).        self
+00000b90: 2e6c 6162 656c 5f33 372e 7365 744f 626a  .label_37.setObj
+00000ba0: 6563 744e 616d 6528 226c 6162 656c 5f33  ectName("label_3
+00000bb0: 3722 290a 2020 2020 2020 2020 7365 6c66  7").        self
+00000bc0: 2e67 7269 644c 6179 6f75 745f 3137 2e61  .gridLayout_17.a
+00000bd0: 6464 5769 6467 6574 2873 656c 662e 6c61  ddWidget(self.la
+00000be0: 6265 6c5f 3337 2c20 302c 2031 2c20 312c  bel_37, 0, 1, 1,
+00000bf0: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+00000c00: 2e6c 6162 656c 5f33 3520 3d20 5174 5769  .label_35 = QtWi
+00000c10: 6467 6574 732e 514c 6162 656c 2870 6172  dgets.QLabel(par
+00000c20: 656e 743d 7365 6c66 2e74 6162 5f36 290a  ent=self.tab_6).
+00000c30: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
+00000c40: 6379 203d 2051 7457 6964 6765 7473 2e51  cy = QtWidgets.Q
+00000c50: 5369 7a65 506f 6c69 6379 2851 7457 6964  SizePolicy(QtWid
+00000c60: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
+00000c70: 2e50 6f6c 6963 792e 5072 6566 6572 7265  .Policy.Preferre
+00000c80: 642c 2051 7457 6964 6765 7473 2e51 5369  d, QtWidgets.QSi
+00000c90: 7a65 506f 6c69 6379 2e50 6f6c 6963 792e  zePolicy.Policy.
+00000ca0: 4d69 6e69 6d75 6d29 0a20 2020 2020 2020  Minimum).       
+00000cb0: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
+00000cc0: 6f72 697a 6f6e 7461 6c53 7472 6574 6368  orizontalStretch
+00000cd0: 2830 290a 2020 2020 2020 2020 7369 7a65  (0).        size
+00000ce0: 506f 6c69 6379 2e73 6574 5665 7274 6963  Policy.setVertic
+00000cf0: 616c 5374 7265 7463 6828 3029 0a20 2020  alStretch(0).   
+00000d00: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
+00000d10: 7365 7448 6569 6768 7446 6f72 5769 6474  setHeightForWidt
+00000d20: 6828 7365 6c66 2e6c 6162 656c 5f33 352e  h(self.label_35.
+00000d30: 7369 7a65 506f 6c69 6379 2829 2e68 6173  sizePolicy().has
+00000d40: 4865 6967 6874 466f 7257 6964 7468 2829  HeightForWidth()
+00000d50: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00000d60: 6162 656c 5f33 352e 7365 7453 697a 6550  abel_35.setSizeP
+00000d70: 6f6c 6963 7928 7369 7a65 506f 6c69 6379  olicy(sizePolicy
+00000d80: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00000d90: 6162 656c 5f33 352e 7365 744f 626a 6563  abel_35.setObjec
+00000da0: 744e 616d 6528 226c 6162 656c 5f33 3522  tName("label_35"
+00000db0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00000dc0: 7269 644c 6179 6f75 745f 3137 2e61 6464  ridLayout_17.add
+00000dd0: 5769 6467 6574 2873 656c 662e 6c61 6265  Widget(self.labe
+00000de0: 6c5f 3335 2c20 302c 2030 2c20 312c 2031  l_35, 0, 0, 1, 1
+00000df0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00000e00: 765f 6f72 6967 696e 616c 203d 2051 7457  v_original = QtW
+00000e10: 6964 6765 7473 2e51 4772 6170 6869 6373  idgets.QGraphics
+00000e20: 5669 6577 2870 6172 656e 743d 7365 6c66  View(parent=self
+00000e30: 2e74 6162 5f36 290a 2020 2020 2020 2020  .tab_6).        
+00000e40: 7369 7a65 506f 6c69 6379 203d 2051 7457  sizePolicy = QtW
+00000e50: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
+00000e60: 6379 2851 7457 6964 6765 7473 2e51 5369  cy(QtWidgets.QSi
+00000e70: 7a65 506f 6c69 6379 2e50 6f6c 6963 792e  zePolicy.Policy.
+00000e80: 4578 7061 6e64 696e 672c 2051 7457 6964  Expanding, QtWid
+00000e90: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
+00000ea0: 2e50 6f6c 6963 792e 4578 7061 6e64 696e  .Policy.Expandin
+00000eb0: 6729 0a20 2020 2020 2020 2073 697a 6550  g).        sizeP
+00000ec0: 6f6c 6963 792e 7365 7448 6f72 697a 6f6e  olicy.setHorizon
+00000ed0: 7461 6c53 7472 6574 6368 2830 290a 2020  talStretch(0).  
+00000ee0: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
+00000ef0: 2e73 6574 5665 7274 6963 616c 5374 7265  .setVerticalStre
+00000f00: 7463 6828 3029 0a20 2020 2020 2020 2073  tch(0).        s
+00000f10: 697a 6550 6f6c 6963 792e 7365 7448 6569  izePolicy.setHei
+00000f20: 6768 7446 6f72 5769 6474 6828 7365 6c66  ghtForWidth(self
+00000f30: 2e67 765f 6f72 6967 696e 616c 2e73 697a  .gv_original.siz
+00000f40: 6550 6f6c 6963 7928 292e 6861 7348 6569  ePolicy().hasHei
+00000f50: 6768 7446 6f72 5769 6474 6828 2929 0a20  ghtForWidth()). 
+00000f60: 2020 2020 2020 2073 656c 662e 6776 5f6f         self.gv_o
+00000f70: 7269 6769 6e61 6c2e 7365 7453 697a 6550  riginal.setSizeP
+00000f80: 6f6c 6963 7928 7369 7a65 506f 6c69 6379  olicy(sizePolicy
+00000f90: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00000fa0: 765f 6f72 6967 696e 616c 2e73 6574 4d69  v_original.setMi
+00000fb0: 6e69 6d75 6d53 697a 6528 5174 436f 7265  nimumSize(QtCore
+00000fc0: 2e51 5369 7a65 2833 3030 2c20 3029 290a  .QSize(300, 0)).
+00000fd0: 2020 2020 2020 2020 7365 6c66 2e67 765f          self.gv_
+00000fe0: 6f72 6967 696e 616c 2e73 6574 4f62 6a65  original.setObje
+00000ff0: 6374 4e61 6d65 2822 6776 5f6f 7269 6769  ctName("gv_origi
+00001000: 6e61 6c22 290a 2020 2020 2020 2020 7365  nal").        se
+00001010: 6c66 2e67 7269 644c 6179 6f75 745f 3137  lf.gridLayout_17
+00001020: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+00001030: 6776 5f6f 7269 6769 6e61 6c2c 2031 2c20  gv_original, 1, 
+00001040: 302c 2031 2c20 3129 0a20 2020 2020 2020  0, 1, 1).       
+00001050: 2073 656c 662e 7461 6257 6964 6765 745f   self.tabWidget_
+00001060: 322e 6164 6454 6162 2873 656c 662e 7461  2.addTab(self.ta
+00001070: 625f 362c 2022 2229 0a20 2020 2020 2020  b_6, "").       
+00001080: 2073 656c 662e 7461 625f 3920 3d20 5174   self.tab_9 = Qt
+00001090: 5769 6467 6574 732e 5157 6964 6765 7428  Widgets.QWidget(
+000010a0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+000010b0: 6162 5f39 2e73 6574 4f62 6a65 6374 4e61  ab_9.setObjectNa
+000010c0: 6d65 2822 7461 625f 3922 290a 2020 2020  me("tab_9").    
+000010d0: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
+000010e0: 6f75 745f 3139 203d 2051 7457 6964 6765  out_19 = QtWidge
+000010f0: 7473 2e51 4772 6964 4c61 796f 7574 2873  ts.QGridLayout(s
+00001100: 656c 662e 7461 625f 3929 0a20 2020 2020  elf.tab_9).     
+00001110: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
+00001120: 7574 5f31 392e 7365 744f 626a 6563 744e  ut_19.setObjectN
+00001130: 616d 6528 2267 7269 644c 6179 6f75 745f  ame("gridLayout_
+00001140: 3139 2229 0a20 2020 2020 2020 2073 656c  19").        sel
+00001150: 662e 665f 7072 6f6a 5f78 203d 2051 7457  f.f_proj_x = QtW
+00001160: 6964 6765 7473 2e51 4672 616d 6528 7061  idgets.QFrame(pa
+00001170: 7265 6e74 3d73 656c 662e 7461 625f 3929  rent=self.tab_9)
+00001180: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+00001190: 6963 7920 3d20 5174 5769 6467 6574 732e  icy = QtWidgets.
+000011a0: 5153 697a 6550 6f6c 6963 7928 5174 5769  QSizePolicy(QtWi
+000011b0: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
+000011c0: 792e 506f 6c69 6379 2e45 7870 616e 6469  y.Policy.Expandi
+000011d0: 6e67 2c20 5174 5769 6467 6574 732e 5153  ng, QtWidgets.QS
+000011e0: 697a 6550 6f6c 6963 792e 506f 6c69 6379  izePolicy.Policy
+000011f0: 2e50 7265 6665 7272 6564 290a 2020 2020  .Preferred).    
+00001200: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
+00001210: 6574 486f 7269 7a6f 6e74 616c 5374 7265  etHorizontalStre
+00001220: 7463 6828 3029 0a20 2020 2020 2020 2073  tch(0).        s
+00001230: 697a 6550 6f6c 6963 792e 7365 7456 6572  izePolicy.setVer
+00001240: 7469 6361 6c53 7472 6574 6368 2830 290a  ticalStretch(0).
+00001250: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
+00001260: 6379 2e73 6574 4865 6967 6874 466f 7257  cy.setHeightForW
+00001270: 6964 7468 2873 656c 662e 665f 7072 6f6a  idth(self.f_proj
+00001280: 5f78 2e73 697a 6550 6f6c 6963 7928 292e  _x.sizePolicy().
+00001290: 6861 7348 6569 6768 7446 6f72 5769 6474  hasHeightForWidt
+000012a0: 6828 2929 0a20 2020 2020 2020 2073 656c  h()).        sel
+000012b0: 662e 665f 7072 6f6a 5f78 2e73 6574 5369  f.f_proj_x.setSi
+000012c0: 7a65 506f 6c69 6379 2873 697a 6550 6f6c  zePolicy(sizePol
+000012d0: 6963 7929 0a20 2020 2020 2020 2073 656c  icy).        sel
+000012e0: 662e 665f 7072 6f6a 5f78 2e73 6574 4175  f.f_proj_x.setAu
+000012f0: 746f 4669 6c6c 4261 636b 6772 6f75 6e64  toFillBackground
+00001300: 2854 7275 6529 0a20 2020 2020 2020 2073  (True).        s
+00001310: 656c 662e 665f 7072 6f6a 5f78 2e73 6574  elf.f_proj_x.set
+00001320: 4672 616d 6553 6861 7065 2851 7457 6964  FrameShape(QtWid
+00001330: 6765 7473 2e51 4672 616d 652e 5368 6170  gets.QFrame.Shap
+00001340: 652e 5374 796c 6564 5061 6e65 6c29 0a20  e.StyledPanel). 
+00001350: 2020 2020 2020 2073 656c 662e 665f 7072         self.f_pr
+00001360: 6f6a 5f78 2e73 6574 4672 616d 6553 6861  oj_x.setFrameSha
+00001370: 646f 7728 5174 5769 6467 6574 732e 5146  dow(QtWidgets.QF
+00001380: 7261 6d65 2e53 6861 646f 772e 5261 6973  rame.Shadow.Rais
+00001390: 6564 290a 2020 2020 2020 2020 7365 6c66  ed).        self
+000013a0: 2e66 5f70 726f 6a5f 782e 7365 744f 626a  .f_proj_x.setObj
+000013b0: 6563 744e 616d 6528 2266 5f70 726f 6a5f  ectName("f_proj_
+000013c0: 7822 290a 2020 2020 2020 2020 7365 6c66  x").        self
+000013d0: 2e67 7269 644c 6179 6f75 745f 3139 2e61  .gridLayout_19.a
+000013e0: 6464 5769 6467 6574 2873 656c 662e 665f  ddWidget(self.f_
+000013f0: 7072 6f6a 5f78 2c20 312c 2031 2c20 312c  proj_x, 1, 1, 1,
+00001400: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+00001410: 2e66 5f70 726f 6a5f 7920 3d20 5174 5769  .f_proj_y = QtWi
+00001420: 6467 6574 732e 5146 7261 6d65 2870 6172  dgets.QFrame(par
+00001430: 656e 743d 7365 6c66 2e74 6162 5f39 290a  ent=self.tab_9).
+00001440: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
+00001450: 6379 203d 2051 7457 6964 6765 7473 2e51  cy = QtWidgets.Q
+00001460: 5369 7a65 506f 6c69 6379 2851 7457 6964  SizePolicy(QtWid
+00001470: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
+00001480: 2e50 6f6c 6963 792e 4578 7061 6e64 696e  .Policy.Expandin
+00001490: 672c 2051 7457 6964 6765 7473 2e51 5369  g, QtWidgets.QSi
+000014a0: 7a65 506f 6c69 6379 2e50 6f6c 6963 792e  zePolicy.Policy.
+000014b0: 5072 6566 6572 7265 6429 0a20 2020 2020  Preferred).     
+000014c0: 2020 2073 697a 6550 6f6c 6963 792e 7365     sizePolicy.se
+000014d0: 7448 6f72 697a 6f6e 7461 6c53 7472 6574  tHorizontalStret
+000014e0: 6368 2830 290a 2020 2020 2020 2020 7369  ch(0).        si
+000014f0: 7a65 506f 6c69 6379 2e73 6574 5665 7274  zePolicy.setVert
+00001500: 6963 616c 5374 7265 7463 6828 3029 0a20  icalStretch(0). 
+00001510: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
+00001520: 792e 7365 7448 6569 6768 7446 6f72 5769  y.setHeightForWi
+00001530: 6474 6828 7365 6c66 2e66 5f70 726f 6a5f  dth(self.f_proj_
+00001540: 792e 7369 7a65 506f 6c69 6379 2829 2e68  y.sizePolicy().h
+00001550: 6173 4865 6967 6874 466f 7257 6964 7468  asHeightForWidth
+00001560: 2829 290a 2020 2020 2020 2020 7365 6c66  ()).        self
+00001570: 2e66 5f70 726f 6a5f 792e 7365 7453 697a  .f_proj_y.setSiz
+00001580: 6550 6f6c 6963 7928 7369 7a65 506f 6c69  ePolicy(sizePoli
+00001590: 6379 290a 2020 2020 2020 2020 7365 6c66  cy).        self
+000015a0: 2e66 5f70 726f 6a5f 792e 7365 7441 7574  .f_proj_y.setAut
+000015b0: 6f46 696c 6c42 6163 6b67 726f 756e 6428  oFillBackground(
+000015c0: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
+000015d0: 6c66 2e66 5f70 726f 6a5f 792e 7365 7446  lf.f_proj_y.setF
+000015e0: 7261 6d65 5368 6170 6528 5174 5769 6467  rameShape(QtWidg
+000015f0: 6574 732e 5146 7261 6d65 2e53 6861 7065  ets.QFrame.Shape
+00001600: 2e53 7479 6c65 6450 616e 656c 290a 2020  .StyledPanel).  
+00001610: 2020 2020 2020 7365 6c66 2e66 5f70 726f        self.f_pro
+00001620: 6a5f 792e 7365 7446 7261 6d65 5368 6164  j_y.setFrameShad
+00001630: 6f77 2851 7457 6964 6765 7473 2e51 4672  ow(QtWidgets.QFr
+00001640: 616d 652e 5368 6164 6f77 2e52 6169 7365  ame.Shadow.Raise
+00001650: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+00001660: 665f 7072 6f6a 5f79 2e73 6574 4f62 6a65  f_proj_y.setObje
+00001670: 6374 4e61 6d65 2822 665f 7072 6f6a 5f79  ctName("f_proj_y
+00001680: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00001690: 6772 6964 4c61 796f 7574 5f31 392e 6164  gridLayout_19.ad
+000016a0: 6457 6964 6765 7428 7365 6c66 2e66 5f70  dWidget(self.f_p
+000016b0: 726f 6a5f 792c 2030 2c20 312c 2031 2c20  roj_y, 0, 1, 1, 
+000016c0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+000016d0: 6c61 6265 6c5f 3432 203d 2051 7457 6964  label_42 = QtWid
+000016e0: 6765 7473 2e51 4c61 6265 6c28 7061 7265  gets.QLabel(pare
+000016f0: 6e74 3d73 656c 662e 7461 625f 3929 0a20  nt=self.tab_9). 
+00001700: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
+00001710: 7920 3d20 5174 5769 6467 6574 732e 5153  y = QtWidgets.QS
+00001720: 697a 6550 6f6c 6963 7928 5174 5769 6467  izePolicy(QtWidg
+00001730: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
+00001740: 506f 6c69 6379 2e4d 696e 696d 756d 2c20  Policy.Minimum, 
+00001750: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
+00001760: 6f6c 6963 792e 506f 6c69 6379 2e50 7265  olicy.Policy.Pre
+00001770: 6665 7272 6564 290a 2020 2020 2020 2020  ferred).        
+00001780: 7369 7a65 506f 6c69 6379 2e73 6574 486f  sizePolicy.setHo
+00001790: 7269 7a6f 6e74 616c 5374 7265 7463 6828  rizontalStretch(
+000017a0: 3029 0a20 2020 2020 2020 2073 697a 6550  0).        sizeP
+000017b0: 6f6c 6963 792e 7365 7456 6572 7469 6361  olicy.setVertica
+000017c0: 6c53 7472 6574 6368 2830 290a 2020 2020  lStretch(0).    
+000017d0: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
+000017e0: 6574 4865 6967 6874 466f 7257 6964 7468  etHeightForWidth
+000017f0: 2873 656c 662e 6c61 6265 6c5f 3432 2e73  (self.label_42.s
+00001800: 697a 6550 6f6c 6963 7928 292e 6861 7348  izePolicy().hasH
+00001810: 6569 6768 7446 6f72 5769 6474 6828 2929  eightForWidth())
+00001820: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00001830: 6265 6c5f 3432 2e73 6574 5369 7a65 506f  bel_42.setSizePo
+00001840: 6c69 6379 2873 697a 6550 6f6c 6963 7929  licy(sizePolicy)
+00001850: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00001860: 6265 6c5f 3432 2e73 6574 4f62 6a65 6374  bel_42.setObject
+00001870: 4e61 6d65 2822 6c61 6265 6c5f 3432 2229  Name("label_42")
+00001880: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00001890: 6964 4c61 796f 7574 5f31 392e 6164 6457  idLayout_19.addW
+000018a0: 6964 6765 7428 7365 6c66 2e6c 6162 656c  idget(self.label
+000018b0: 5f34 322c 2030 2c20 302c 2031 2c20 3129  _42, 0, 0, 1, 1)
+000018c0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+000018d0: 6265 6c5f 3435 203d 2051 7457 6964 6765  bel_45 = QtWidge
+000018e0: 7473 2e51 4c61 6265 6c28 7061 7265 6e74  ts.QLabel(parent
+000018f0: 3d73 656c 662e 7461 625f 3929 0a20 2020  =self.tab_9).   
+00001900: 2020 2020 2073 697a 6550 6f6c 6963 7920       sizePolicy 
+00001910: 3d20 5174 5769 6467 6574 732e 5153 697a  = QtWidgets.QSiz
+00001920: 6550 6f6c 6963 7928 5174 5769 6467 6574  ePolicy(QtWidget
+00001930: 732e 5153 697a 6550 6f6c 6963 792e 506f  s.QSizePolicy.Po
+00001940: 6c69 6379 2e4d 696e 696d 756d 2c20 5174  licy.Minimum, Qt
+00001950: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
+00001960: 6963 792e 506f 6c69 6379 2e50 7265 6665  icy.Policy.Prefe
+00001970: 7272 6564 290a 2020 2020 2020 2020 7369  rred).        si
+00001980: 7a65 506f 6c69 6379 2e73 6574 486f 7269  zePolicy.setHori
+00001990: 7a6f 6e74 616c 5374 7265 7463 6828 3029  zontalStretch(0)
+000019a0: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+000019b0: 6963 792e 7365 7456 6572 7469 6361 6c53  icy.setVerticalS
+000019c0: 7472 6574 6368 2830 290a 2020 2020 2020  tretch(0).      
+000019d0: 2020 7369 7a65 506f 6c69 6379 2e73 6574    sizePolicy.set
+000019e0: 4865 6967 6874 466f 7257 6964 7468 2873  HeightForWidth(s
+000019f0: 656c 662e 6c61 6265 6c5f 3435 2e73 697a  elf.label_45.siz
+00001a00: 6550 6f6c 6963 7928 292e 6861 7348 6569  ePolicy().hasHei
+00001a10: 6768 7446 6f72 5769 6474 6828 2929 0a20  ghtForWidth()). 
+00001a20: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+00001a30: 6c5f 3435 2e73 6574 5369 7a65 506f 6c69  l_45.setSizePoli
+00001a40: 6379 2873 697a 6550 6f6c 6963 7929 0a20  cy(sizePolicy). 
+00001a50: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+00001a60: 6c5f 3435 2e73 6574 4f62 6a65 6374 4e61  l_45.setObjectNa
+00001a70: 6d65 2822 6c61 6265 6c5f 3435 2229 0a20  me("label_45"). 
+00001a80: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
+00001a90: 4c61 796f 7574 5f31 392e 6164 6457 6964  Layout_19.addWid
+00001aa0: 6765 7428 7365 6c66 2e6c 6162 656c 5f34  get(self.label_4
+00001ab0: 352c 2031 2c20 302c 2031 2c20 3129 0a20  5, 1, 0, 1, 1). 
+00001ac0: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
+00001ad0: 6964 6765 745f 322e 6164 6454 6162 2873  idget_2.addTab(s
+00001ae0: 656c 662e 7461 625f 392c 2022 2229 0a20  elf.tab_9, ""). 
+00001af0: 2020 2020 2020 2073 656c 662e 7461 625f         self.tab_
+00001b00: 3720 3d20 5174 5769 6467 6574 732e 5157  7 = QtWidgets.QW
+00001b10: 6964 6765 7428 290a 2020 2020 2020 2020  idget().        
+00001b20: 7365 6c66 2e74 6162 5f37 2e73 6574 4f62  self.tab_7.setOb
+00001b30: 6a65 6374 4e61 6d65 2822 7461 625f 3722  jectName("tab_7"
+00001b40: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00001b50: 7269 644c 6179 6f75 745f 3138 203d 2051  ridLayout_18 = Q
+00001b60: 7457 6964 6765 7473 2e51 4772 6964 4c61  tWidgets.QGridLa
+00001b70: 796f 7574 2873 656c 662e 7461 625f 3729  yout(self.tab_7)
+00001b80: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00001b90: 6964 4c61 796f 7574 5f31 382e 7365 744f  idLayout_18.setO
+00001ba0: 626a 6563 744e 616d 6528 2267 7269 644c  bjectName("gridL
+00001bb0: 6179 6f75 745f 3138 2229 0a20 2020 2020  ayout_18").     
+00001bc0: 2020 2073 656c 662e 665f 785f 7361 6d70     self.f_x_samp
+00001bd0: 6c65 203d 2051 7457 6964 6765 7473 2e51  le = QtWidgets.Q
+00001be0: 4672 616d 6528 7061 7265 6e74 3d73 656c  Frame(parent=sel
+00001bf0: 662e 7461 625f 3729 0a20 2020 2020 2020  f.tab_7).       
+00001c00: 2073 697a 6550 6f6c 6963 7920 3d20 5174   sizePolicy = Qt
+00001c10: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
+00001c20: 6963 7928 5174 5769 6467 6574 732e 5153  icy(QtWidgets.QS
+00001c30: 697a 6550 6f6c 6963 792e 506f 6c69 6379  izePolicy.Policy
+00001c40: 2e45 7870 616e 6469 6e67 2c20 5174 5769  .Expanding, QtWi
+00001c50: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
+00001c60: 792e 506f 6c69 6379 2e50 7265 6665 7272  y.Policy.Preferr
+00001c70: 6564 290a 2020 2020 2020 2020 7369 7a65  ed).        size
+00001c80: 506f 6c69 6379 2e73 6574 486f 7269 7a6f  Policy.setHorizo
+00001c90: 6e74 616c 5374 7265 7463 6828 3029 0a20  ntalStretch(0). 
+00001ca0: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
+00001cb0: 792e 7365 7456 6572 7469 6361 6c53 7472  y.setVerticalStr
+00001cc0: 6574 6368 2830 290a 2020 2020 2020 2020  etch(0).        
+00001cd0: 7369 7a65 506f 6c69 6379 2e73 6574 4865  sizePolicy.setHe
+00001ce0: 6967 6874 466f 7257 6964 7468 2873 656c  ightForWidth(sel
+00001cf0: 662e 665f 785f 7361 6d70 6c65 2e73 697a  f.f_x_sample.siz
+00001d00: 6550 6f6c 6963 7928 292e 6861 7348 6569  ePolicy().hasHei
+00001d10: 6768 7446 6f72 5769 6474 6828 2929 0a20  ghtForWidth()). 
+00001d20: 2020 2020 2020 2073 656c 662e 665f 785f         self.f_x_
+00001d30: 7361 6d70 6c65 2e73 6574 5369 7a65 506f  sample.setSizePo
+00001d40: 6c69 6379 2873 697a 6550 6f6c 6963 7929  licy(sizePolicy)
+00001d50: 0a20 2020 2020 2020 2073 656c 662e 665f  .        self.f_
+00001d60: 785f 7361 6d70 6c65 2e73 6574 4672 616d  x_sample.setFram
+00001d70: 6553 6861 7065 2851 7457 6964 6765 7473  eShape(QtWidgets
+00001d80: 2e51 4672 616d 652e 5368 6170 652e 5374  .QFrame.Shape.St
+00001d90: 796c 6564 5061 6e65 6c29 0a20 2020 2020  yledPanel).     
+00001da0: 2020 2073 656c 662e 665f 785f 7361 6d70     self.f_x_samp
+00001db0: 6c65 2e73 6574 4672 616d 6553 6861 646f  le.setFrameShado
+00001dc0: 7728 5174 5769 6467 6574 732e 5146 7261  w(QtWidgets.QFra
+00001dd0: 6d65 2e53 6861 646f 772e 5261 6973 6564  me.Shadow.Raised
+00001de0: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+00001df0: 5f78 5f73 616d 706c 652e 7365 744f 626a  _x_sample.setObj
+00001e00: 6563 744e 616d 6528 2266 5f78 5f73 616d  ectName("f_x_sam
+00001e10: 706c 6522 290a 2020 2020 2020 2020 7365  ple").        se
+00001e20: 6c66 2e67 7269 644c 6179 6f75 745f 3138  lf.gridLayout_18
+00001e30: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+00001e40: 665f 785f 7361 6d70 6c65 2c20 322c 2032  f_x_sample, 2, 2
+00001e50: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
+00001e60: 7365 6c66 2e66 5f79 5f73 616d 706c 6520  self.f_y_sample 
+00001e70: 3d20 5174 5769 6467 6574 732e 5146 7261  = QtWidgets.QFra
+00001e80: 6d65 2870 6172 656e 743d 7365 6c66 2e74  me(parent=self.t
+00001e90: 6162 5f37 290a 2020 2020 2020 2020 7369  ab_7).        si
+00001ea0: 7a65 506f 6c69 6379 203d 2051 7457 6964  zePolicy = QtWid
+00001eb0: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
+00001ec0: 2851 7457 6964 6765 7473 2e51 5369 7a65  (QtWidgets.QSize
+00001ed0: 506f 6c69 6379 2e50 6f6c 6963 792e 4578  Policy.Policy.Ex
+00001ee0: 7061 6e64 696e 672c 2051 7457 6964 6765  panding, QtWidge
+00001ef0: 7473 2e51 5369 7a65 506f 6c69 6379 2e50  ts.QSizePolicy.P
+00001f00: 6f6c 6963 792e 5072 6566 6572 7265 6429  olicy.Preferred)
+00001f10: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+00001f20: 6963 792e 7365 7448 6f72 697a 6f6e 7461  icy.setHorizonta
+00001f30: 6c53 7472 6574 6368 2830 290a 2020 2020  lStretch(0).    
+00001f40: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
+00001f50: 6574 5665 7274 6963 616c 5374 7265 7463  etVerticalStretc
+00001f60: 6828 3029 0a20 2020 2020 2020 2073 697a  h(0).        siz
+00001f70: 6550 6f6c 6963 792e 7365 7448 6569 6768  ePolicy.setHeigh
+00001f80: 7446 6f72 5769 6474 6828 7365 6c66 2e66  tForWidth(self.f
+00001f90: 5f79 5f73 616d 706c 652e 7369 7a65 506f  _y_sample.sizePo
+00001fa0: 6c69 6379 2829 2e68 6173 4865 6967 6874  licy().hasHeight
+00001fb0: 466f 7257 6964 7468 2829 290a 2020 2020  ForWidth()).    
+00001fc0: 2020 2020 7365 6c66 2e66 5f79 5f73 616d      self.f_y_sam
+00001fd0: 706c 652e 7365 7453 697a 6550 6f6c 6963  ple.setSizePolic
+00001fe0: 7928 7369 7a65 506f 6c69 6379 290a 2020  y(sizePolicy).  
+00001ff0: 2020 2020 2020 7365 6c66 2e66 5f79 5f73        self.f_y_s
+00002000: 616d 706c 652e 7365 7446 7261 6d65 5368  ample.setFrameSh
+00002010: 6170 6528 5174 5769 6467 6574 732e 5146  ape(QtWidgets.QF
+00002020: 7261 6d65 2e53 6861 7065 2e53 7479 6c65  rame.Shape.Style
+00002030: 6450 616e 656c 290a 2020 2020 2020 2020  dPanel).        
+00002040: 7365 6c66 2e66 5f79 5f73 616d 706c 652e  self.f_y_sample.
+00002050: 7365 7446 7261 6d65 5368 6164 6f77 2851  setFrameShadow(Q
+00002060: 7457 6964 6765 7473 2e51 4672 616d 652e  tWidgets.QFrame.
+00002070: 5368 6164 6f77 2e52 6169 7365 6429 0a20  Shadow.Raised). 
+00002080: 2020 2020 2020 2073 656c 662e 665f 795f         self.f_y_
+00002090: 7361 6d70 6c65 2e73 6574 4f62 6a65 6374  sample.setObject
+000020a0: 4e61 6d65 2822 665f 795f 7361 6d70 6c65  Name("f_y_sample
+000020b0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000020c0: 6772 6964 4c61 796f 7574 5f31 382e 6164  gridLayout_18.ad
+000020d0: 6457 6964 6765 7428 7365 6c66 2e66 5f79  dWidget(self.f_y
+000020e0: 5f73 616d 706c 652c 2030 2c20 322c 2031  _sample, 0, 2, 1
+000020f0: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
+00002100: 662e 6c61 6265 6c5f 3431 203d 2051 7457  f.label_41 = QtW
+00002110: 6964 6765 7473 2e51 4c61 6265 6c28 7061  idgets.QLabel(pa
+00002120: 7265 6e74 3d73 656c 662e 7461 625f 3729  rent=self.tab_7)
+00002130: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+00002140: 6963 7920 3d20 5174 5769 6467 6574 732e  icy = QtWidgets.
+00002150: 5153 697a 6550 6f6c 6963 7928 5174 5769  QSizePolicy(QtWi
+00002160: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
+00002170: 792e 506f 6c69 6379 2e4d 696e 696d 756d  y.Policy.Minimum
+00002180: 2c20 5174 5769 6467 6574 732e 5153 697a  , QtWidgets.QSiz
+00002190: 6550 6f6c 6963 792e 506f 6c69 6379 2e50  ePolicy.Policy.P
+000021a0: 7265 6665 7272 6564 290a 2020 2020 2020  referred).      
+000021b0: 2020 7369 7a65 506f 6c69 6379 2e73 6574    sizePolicy.set
+000021c0: 486f 7269 7a6f 6e74 616c 5374 7265 7463  HorizontalStretc
+000021d0: 6828 3029 0a20 2020 2020 2020 2073 697a  h(0).        siz
+000021e0: 6550 6f6c 6963 792e 7365 7456 6572 7469  ePolicy.setVerti
+000021f0: 6361 6c53 7472 6574 6368 2830 290a 2020  calStretch(0).  
+00002200: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
+00002210: 2e73 6574 4865 6967 6874 466f 7257 6964  .setHeightForWid
+00002220: 7468 2873 656c 662e 6c61 6265 6c5f 3431  th(self.label_41
+00002230: 2e73 697a 6550 6f6c 6963 7928 292e 6861  .sizePolicy().ha
+00002240: 7348 6569 6768 7446 6f72 5769 6474 6828  sHeightForWidth(
+00002250: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00002260: 6c61 6265 6c5f 3431 2e73 6574 5369 7a65  label_41.setSize
+00002270: 506f 6c69 6379 2873 697a 6550 6f6c 6963  Policy(sizePolic
+00002280: 7929 0a20 2020 2020 2020 2073 656c 662e  y).        self.
+00002290: 6c61 6265 6c5f 3431 2e73 6574 4f62 6a65  label_41.setObje
+000022a0: 6374 4e61 6d65 2822 6c61 6265 6c5f 3431  ctName("label_41
+000022b0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000022c0: 6772 6964 4c61 796f 7574 5f31 382e 6164  gridLayout_18.ad
+000022d0: 6457 6964 6765 7428 7365 6c66 2e6c 6162  dWidget(self.lab
+000022e0: 656c 5f34 312c 2030 2c20 312c 2031 2c20  el_41, 0, 1, 1, 
+000022f0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+00002300: 6c61 6265 6c5f 3430 203d 2051 7457 6964  label_40 = QtWid
+00002310: 6765 7473 2e51 4c61 6265 6c28 7061 7265  gets.QLabel(pare
+00002320: 6e74 3d73 656c 662e 7461 625f 3729 0a20  nt=self.tab_7). 
+00002330: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
+00002340: 7920 3d20 5174 5769 6467 6574 732e 5153  y = QtWidgets.QS
+00002350: 697a 6550 6f6c 6963 7928 5174 5769 6467  izePolicy(QtWidg
+00002360: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
+00002370: 506f 6c69 6379 2e4d 696e 696d 756d 2c20  Policy.Minimum, 
+00002380: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
+00002390: 6f6c 6963 792e 506f 6c69 6379 2e50 7265  olicy.Policy.Pre
+000023a0: 6665 7272 6564 290a 2020 2020 2020 2020  ferred).        
+000023b0: 7369 7a65 506f 6c69 6379 2e73 6574 486f  sizePolicy.setHo
+000023c0: 7269 7a6f 6e74 616c 5374 7265 7463 6828  rizontalStretch(
+000023d0: 3029 0a20 2020 2020 2020 2073 697a 6550  0).        sizeP
+000023e0: 6f6c 6963 792e 7365 7456 6572 7469 6361  olicy.setVertica
+000023f0: 6c53 7472 6574 6368 2830 290a 2020 2020  lStretch(0).    
+00002400: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
+00002410: 6574 4865 6967 6874 466f 7257 6964 7468  etHeightForWidth
+00002420: 2873 656c 662e 6c61 6265 6c5f 3430 2e73  (self.label_40.s
+00002430: 697a 6550 6f6c 6963 7928 292e 6861 7348  izePolicy().hasH
+00002440: 6569 6768 7446 6f72 5769 6474 6828 2929  eightForWidth())
+00002450: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00002460: 6265 6c5f 3430 2e73 6574 5369 7a65 506f  bel_40.setSizePo
+00002470: 6c69 6379 2873 697a 6550 6f6c 6963 7929  licy(sizePolicy)
+00002480: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00002490: 6265 6c5f 3430 2e73 6574 4f62 6a65 6374  bel_40.setObject
+000024a0: 4e61 6d65 2822 6c61 6265 6c5f 3430 2229  Name("label_40")
+000024b0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+000024c0: 6964 4c61 796f 7574 5f31 382e 6164 6457  idLayout_18.addW
+000024d0: 6964 6765 7428 7365 6c66 2e6c 6162 656c  idget(self.label
+000024e0: 5f34 302c 2032 2c20 312c 2031 2c20 3129  _40, 2, 1, 1, 1)
+000024f0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+00002500: 6257 6964 6765 745f 322e 6164 6454 6162  bWidget_2.addTab
+00002510: 2873 656c 662e 7461 625f 372c 2022 2229  (self.tab_7, "")
+00002520: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+00002530: 625f 3820 3d20 5174 5769 6467 6574 732e  b_8 = QtWidgets.
+00002540: 5157 6964 6765 7428 290a 2020 2020 2020  QWidget().      
+00002550: 2020 7365 6c66 2e74 6162 5f38 2e73 6574    self.tab_8.set
+00002560: 4f62 6a65 6374 4e61 6d65 2822 7461 625f  ObjectName("tab_
+00002570: 3822 290a 2020 2020 2020 2020 7365 6c66  8").        self
+00002580: 2e67 7269 644c 6179 6f75 745f 3136 203d  .gridLayout_16 =
+00002590: 2051 7457 6964 6765 7473 2e51 4772 6964   QtWidgets.QGrid
+000025a0: 4c61 796f 7574 2873 656c 662e 7461 625f  Layout(self.tab_
+000025b0: 3829 0a20 2020 2020 2020 2073 656c 662e  8).        self.
+000025c0: 6772 6964 4c61 796f 7574 5f31 362e 7365  gridLayout_16.se
+000025d0: 744f 626a 6563 744e 616d 6528 2267 7269  tObjectName("gri
+000025e0: 644c 6179 6f75 745f 3136 2229 0a20 2020  dLayout_16").   
+000025f0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00002600: 3434 203d 2051 7457 6964 6765 7473 2e51  44 = QtWidgets.Q
+00002610: 4c61 6265 6c28 7061 7265 6e74 3d73 656c  Label(parent=sel
+00002620: 662e 7461 625f 3829 0a20 2020 2020 2020  f.tab_8).       
+00002630: 2073 656c 662e 6c61 6265 6c5f 3434 2e73   self.label_44.s
+00002640: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
+00002650: 6265 6c5f 3434 2229 0a20 2020 2020 2020  bel_44").       
+00002660: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
+00002670: 5f31 362e 6164 6457 6964 6765 7428 7365  _16.addWidget(se
+00002680: 6c66 2e6c 6162 656c 5f34 342c 2030 2c20  lf.label_44, 0, 
+00002690: 312c 2031 2c20 3129 0a20 2020 2020 2020  1, 1, 1).       
+000026a0: 2073 656c 662e 6c61 6265 6c5f 3433 203d   self.label_43 =
+000026b0: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
+000026c0: 6c28 7061 7265 6e74 3d73 656c 662e 7461  l(parent=self.ta
+000026d0: 625f 3829 0a20 2020 2020 2020 2073 656c  b_8).        sel
+000026e0: 662e 6c61 6265 6c5f 3433 2e73 6574 4f62  f.label_43.setOb
+000026f0: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
+00002700: 3433 2229 0a20 2020 2020 2020 2073 656c  43").        sel
+00002710: 662e 6772 6964 4c61 796f 7574 5f31 362e  f.gridLayout_16.
+00002720: 6164 6457 6964 6765 7428 7365 6c66 2e6c  addWidget(self.l
+00002730: 6162 656c 5f34 332c 2030 2c20 302c 2031  abel_43, 0, 0, 1
+00002740: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
+00002750: 662e 665f 725f 636f 6d70 203d 2051 7457  f.f_r_comp = QtW
+00002760: 6964 6765 7473 2e51 4672 616d 6528 7061  idgets.QFrame(pa
+00002770: 7265 6e74 3d73 656c 662e 7461 625f 3829  rent=self.tab_8)
+00002780: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+00002790: 6963 7920 3d20 5174 5769 6467 6574 732e  icy = QtWidgets.
+000027a0: 5153 697a 6550 6f6c 6963 7928 5174 5769  QSizePolicy(QtWi
+000027b0: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
+000027c0: 792e 506f 6c69 6379 2e50 7265 6665 7272  y.Policy.Preferr
+000027d0: 6564 2c20 5174 5769 6467 6574 732e 5153  ed, QtWidgets.QS
+000027e0: 697a 6550 6f6c 6963 792e 506f 6c69 6379  izePolicy.Policy
+000027f0: 2e45 7870 616e 6469 6e67 290a 2020 2020  .Expanding).    
+00002800: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
+00002810: 6574 486f 7269 7a6f 6e74 616c 5374 7265  etHorizontalStre
+00002820: 7463 6828 3029 0a20 2020 2020 2020 2073  tch(0).        s
+00002830: 697a 6550 6f6c 6963 792e 7365 7456 6572  izePolicy.setVer
+00002840: 7469 6361 6c53 7472 6574 6368 2830 290a  ticalStretch(0).
+00002850: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
+00002860: 6379 2e73 6574 4865 6967 6874 466f 7257  cy.setHeightForW
+00002870: 6964 7468 2873 656c 662e 665f 725f 636f  idth(self.f_r_co
+00002880: 6d70 2e73 697a 6550 6f6c 6963 7928 292e  mp.sizePolicy().
+00002890: 6861 7348 6569 6768 7446 6f72 5769 6474  hasHeightForWidt
+000028a0: 6828 2929 0a20 2020 2020 2020 2073 656c  h()).        sel
+000028b0: 662e 665f 725f 636f 6d70 2e73 6574 5369  f.f_r_comp.setSi
+000028c0: 7a65 506f 6c69 6379 2873 697a 6550 6f6c  zePolicy(sizePol
+000028d0: 6963 7929 0a20 2020 2020 2020 2073 656c  icy).        sel
+000028e0: 662e 665f 725f 636f 6d70 2e73 6574 4175  f.f_r_comp.setAu
+000028f0: 746f 4669 6c6c 4261 636b 6772 6f75 6e64  toFillBackground
+00002900: 2854 7275 6529 0a20 2020 2020 2020 2073  (True).        s
+00002910: 656c 662e 665f 725f 636f 6d70 2e73 6574  elf.f_r_comp.set
+00002920: 4672 616d 6553 6861 7065 2851 7457 6964  FrameShape(QtWid
+00002930: 6765 7473 2e51 4672 616d 652e 5368 6170  gets.QFrame.Shap
+00002940: 652e 5374 796c 6564 5061 6e65 6c29 0a20  e.StyledPanel). 
+00002950: 2020 2020 2020 2073 656c 662e 665f 725f         self.f_r_
+00002960: 636f 6d70 2e73 6574 4672 616d 6553 6861  comp.setFrameSha
+00002970: 646f 7728 5174 5769 6467 6574 732e 5146  dow(QtWidgets.QF
+00002980: 7261 6d65 2e53 6861 646f 772e 5261 6973  rame.Shadow.Rais
+00002990: 6564 290a 2020 2020 2020 2020 7365 6c66  ed).        self
+000029a0: 2e66 5f72 5f63 6f6d 702e 7365 744f 626a  .f_r_comp.setObj
+000029b0: 6563 744e 616d 6528 2266 5f72 5f63 6f6d  ectName("f_r_com
+000029c0: 7022 290a 2020 2020 2020 2020 7365 6c66  p").        self
+000029d0: 2e67 7269 644c 6179 6f75 745f 3136 2e61  .gridLayout_16.a
+000029e0: 6464 5769 6467 6574 2873 656c 662e 665f  ddWidget(self.f_
+000029f0: 725f 636f 6d70 2c20 312c 2031 2c20 312c  r_comp, 1, 1, 1,
+00002a00: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+00002a10: 2e66 5f72 5f72 6563 6f6e 203d 2051 7457  .f_r_recon = QtW
+00002a20: 6964 6765 7473 2e51 4672 616d 6528 7061  idgets.QFrame(pa
+00002a30: 7265 6e74 3d73 656c 662e 7461 625f 3829  rent=self.tab_8)
+00002a40: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+00002a50: 6963 7920 3d20 5174 5769 6467 6574 732e  icy = QtWidgets.
+00002a60: 5153 697a 6550 6f6c 6963 7928 5174 5769  QSizePolicy(QtWi
+00002a70: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
+00002a80: 792e 506f 6c69 6379 2e50 7265 6665 7272  y.Policy.Preferr
+00002a90: 6564 2c20 5174 5769 6467 6574 732e 5153  ed, QtWidgets.QS
+00002aa0: 697a 6550 6f6c 6963 792e 506f 6c69 6379  izePolicy.Policy
+00002ab0: 2e45 7870 616e 6469 6e67 290a 2020 2020  .Expanding).    
+00002ac0: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
+00002ad0: 6574 486f 7269 7a6f 6e74 616c 5374 7265  etHorizontalStre
+00002ae0: 7463 6828 3029 0a20 2020 2020 2020 2073  tch(0).        s
+00002af0: 697a 6550 6f6c 6963 792e 7365 7456 6572  izePolicy.setVer
+00002b00: 7469 6361 6c53 7472 6574 6368 2830 290a  ticalStretch(0).
+00002b10: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
+00002b20: 6379 2e73 6574 4865 6967 6874 466f 7257  cy.setHeightForW
+00002b30: 6964 7468 2873 656c 662e 665f 725f 7265  idth(self.f_r_re
+00002b40: 636f 6e2e 7369 7a65 506f 6c69 6379 2829  con.sizePolicy()
+00002b50: 2e68 6173 4865 6967 6874 466f 7257 6964  .hasHeightForWid
+00002b60: 7468 2829 290a 2020 2020 2020 2020 7365  th()).        se
+00002b70: 6c66 2e66 5f72 5f72 6563 6f6e 2e73 6574  lf.f_r_recon.set
+00002b80: 5369 7a65 506f 6c69 6379 2873 697a 6550  SizePolicy(sizeP
+00002b90: 6f6c 6963 7929 0a20 2020 2020 2020 2073  olicy).        s
+00002ba0: 656c 662e 665f 725f 7265 636f 6e2e 7365  elf.f_r_recon.se
+00002bb0: 7441 7574 6f46 696c 6c42 6163 6b67 726f  tAutoFillBackgro
+00002bc0: 756e 6428 5472 7565 290a 2020 2020 2020  und(True).      
+00002bd0: 2020 7365 6c66 2e66 5f72 5f72 6563 6f6e    self.f_r_recon
+00002be0: 2e73 6574 4672 616d 6553 6861 7065 2851  .setFrameShape(Q
+00002bf0: 7457 6964 6765 7473 2e51 4672 616d 652e  tWidgets.QFrame.
+00002c00: 5368 6170 652e 5374 796c 6564 5061 6e65  Shape.StyledPane
+00002c10: 6c29 0a20 2020 2020 2020 2073 656c 662e  l).        self.
+00002c20: 665f 725f 7265 636f 6e2e 7365 7446 7261  f_r_recon.setFra
+00002c30: 6d65 5368 6164 6f77 2851 7457 6964 6765  meShadow(QtWidge
+00002c40: 7473 2e51 4672 616d 652e 5368 6164 6f77  ts.QFrame.Shadow
+00002c50: 2e52 6169 7365 6429 0a20 2020 2020 2020  .Raised).       
+00002c60: 2073 656c 662e 665f 725f 7265 636f 6e2e   self.f_r_recon.
+00002c70: 7365 744f 626a 6563 744e 616d 6528 2266  setObjectName("f
+00002c80: 5f72 5f72 6563 6f6e 2229 0a20 2020 2020  _r_recon").     
+00002c90: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
+00002ca0: 7574 5f31 362e 6164 6457 6964 6765 7428  ut_16.addWidget(
+00002cb0: 7365 6c66 2e66 5f72 5f72 6563 6f6e 2c20  self.f_r_recon, 
+00002cc0: 312c 2030 2c20 312c 2031 290a 2020 2020  1, 0, 1, 1).    
+00002cd0: 2020 2020 7365 6c66 2e74 6162 5769 6467      self.tabWidg
+00002ce0: 6574 5f32 2e61 6464 5461 6228 7365 6c66  et_2.addTab(self
+00002cf0: 2e74 6162 5f38 2c20 2222 290a 2020 2020  .tab_8, "").    
+00002d00: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
+00002d10: 6f75 745f 3133 2e61 6464 5769 6467 6574  out_13.addWidget
+00002d20: 2873 656c 662e 7461 6257 6964 6765 745f  (self.tabWidget_
+00002d30: 322c 2031 2c20 312c 2033 2c20 3129 0a20  2, 1, 1, 3, 1). 
+00002d40: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
+00002d50: 655f 3320 3d20 5174 5769 6467 6574 732e  e_3 = QtWidgets.
+00002d60: 5146 7261 6d65 2870 6172 656e 743d 7365  QFrame(parent=se
+00002d70: 6c66 2e74 6162 5f35 290a 2020 2020 2020  lf.tab_5).      
+00002d80: 2020 7369 7a65 506f 6c69 6379 203d 2051    sizePolicy = Q
+00002d90: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
+00002da0: 6c69 6379 2851 7457 6964 6765 7473 2e51  licy(QtWidgets.Q
+00002db0: 5369 7a65 506f 6c69 6379 2e50 6f6c 6963  SizePolicy.Polic
+00002dc0: 792e 4d69 6e69 6d75 6d2c 2051 7457 6964  y.Minimum, QtWid
+00002dd0: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
+00002de0: 2e50 6f6c 6963 792e 4d69 6e69 6d75 6d29  .Policy.Minimum)
+00002df0: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+00002e00: 6963 792e 7365 7448 6f72 697a 6f6e 7461  icy.setHorizonta
+00002e10: 6c53 7472 6574 6368 2830 290a 2020 2020  lStretch(0).    
+00002e20: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
+00002e30: 6574 5665 7274 6963 616c 5374 7265 7463  etVerticalStretc
+00002e40: 6828 3029 0a20 2020 2020 2020 2073 697a  h(0).        siz
+00002e50: 6550 6f6c 6963 792e 7365 7448 6569 6768  ePolicy.setHeigh
+00002e60: 7446 6f72 5769 6474 6828 7365 6c66 2e66  tForWidth(self.f
+00002e70: 7261 6d65 5f33 2e73 697a 6550 6f6c 6963  rame_3.sizePolic
+00002e80: 7928 292e 6861 7348 6569 6768 7446 6f72  y().hasHeightFor
+00002e90: 5769 6474 6828 2929 0a20 2020 2020 2020  Width()).       
+00002ea0: 2073 656c 662e 6672 616d 655f 332e 7365   self.frame_3.se
+00002eb0: 7453 697a 6550 6f6c 6963 7928 7369 7a65  tSizePolicy(size
+00002ec0: 506f 6c69 6379 290a 2020 2020 2020 2020  Policy).        
+00002ed0: 7365 6c66 2e66 7261 6d65 5f33 2e73 6574  self.frame_3.set
+00002ee0: 4d69 6e69 6d75 6d53 697a 6528 5174 436f  MinimumSize(QtCo
+00002ef0: 7265 2e51 5369 7a65 2830 2c20 3135 3029  re.QSize(0, 150)
+00002f00: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+00002f10: 7261 6d65 5f33 2e73 6574 4672 616d 6553  rame_3.setFrameS
+00002f20: 6861 7065 2851 7457 6964 6765 7473 2e51  hape(QtWidgets.Q
+00002f30: 4672 616d 652e 5368 6170 652e 5374 796c  Frame.Shape.Styl
+00002f40: 6564 5061 6e65 6c29 0a20 2020 2020 2020  edPanel).       
+00002f50: 2073 656c 662e 6672 616d 655f 332e 7365   self.frame_3.se
+00002f60: 7446 7261 6d65 5368 6164 6f77 2851 7457  tFrameShadow(QtW
+00002f70: 6964 6765 7473 2e51 4672 616d 652e 5368  idgets.QFrame.Sh
+00002f80: 6164 6f77 2e52 6169 7365 6429 0a20 2020  adow.Raised).   
+00002f90: 2020 2020 2073 656c 662e 6672 616d 655f       self.frame_
+00002fa0: 332e 7365 744f 626a 6563 744e 616d 6528  3.setObjectName(
+00002fb0: 2266 7261 6d65 5f33 2229 0a20 2020 2020  "frame_3").     
+00002fc0: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
+00002fd0: 7574 5f31 3420 3d20 5174 5769 6467 6574  ut_14 = QtWidget
+00002fe0: 732e 5147 7269 644c 6179 6f75 7428 7365  s.QGridLayout(se
+00002ff0: 6c66 2e66 7261 6d65 5f33 290a 2020 2020  lf.frame_3).    
+00003000: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
+00003010: 6f75 745f 3134 2e73 6574 4f62 6a65 6374  out_14.setObject
+00003020: 4e61 6d65 2822 6772 6964 4c61 796f 7574  Name("gridLayout
+00003030: 5f31 3422 290a 2020 2020 2020 2020 7365  _14").        se
+00003040: 6c66 2e63 625f 4247 435f 7361 6d70 6c65  lf.cb_BGC_sample
+00003050: 203d 2051 7457 6964 6765 7473 2e51 436f   = QtWidgets.QCo
+00003060: 6d62 6f42 6f78 2870 6172 656e 743d 7365  mboBox(parent=se
+00003070: 6c66 2e66 7261 6d65 5f33 290a 2020 2020  lf.frame_3).    
+00003080: 2020 2020 7365 6c66 2e63 625f 4247 435f      self.cb_BGC_
+00003090: 7361 6d70 6c65 2e73 6574 4f62 6a65 6374  sample.setObject
+000030a0: 4e61 6d65 2822 6362 5f42 4743 5f73 616d  Name("cb_BGC_sam
+000030b0: 706c 6522 290a 2020 2020 2020 2020 7365  ple").        se
+000030c0: 6c66 2e63 625f 4247 435f 7361 6d70 6c65  lf.cb_BGC_sample
+000030d0: 2e61 6464 4974 656d 2822 2229 0a20 2020  .addItem("").   
+000030e0: 2020 2020 2073 656c 662e 6362 5f42 4743       self.cb_BGC
+000030f0: 5f73 616d 706c 652e 6164 6449 7465 6d28  _sample.addItem(
+00003100: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
+00003110: 2e67 7269 644c 6179 6f75 745f 3134 2e61  .gridLayout_14.a
+00003120: 6464 5769 6467 6574 2873 656c 662e 6362  ddWidget(self.cb
+00003130: 5f42 4743 5f73 616d 706c 652c 2033 2c20  _BGC_sample, 3, 
+00003140: 312c 2031 2c20 3129 0a20 2020 2020 2020  1, 1, 1).       
+00003150: 2073 656c 662e 6c61 6265 6c5f 3339 203d   self.label_39 =
+00003160: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
+00003170: 6c28 7061 7265 6e74 3d73 656c 662e 6672  l(parent=self.fr
+00003180: 616d 655f 3329 0a20 2020 2020 2020 2073  ame_3).        s
+00003190: 656c 662e 6c61 6265 6c5f 3339 2e73 6574  elf.label_39.set
+000031a0: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
+000031b0: 6c5f 3339 2229 0a20 2020 2020 2020 2073  l_39").        s
+000031c0: 656c 662e 6772 6964 4c61 796f 7574 5f31  elf.gridLayout_1
+000031d0: 342e 6164 6457 6964 6765 7428 7365 6c66  4.addWidget(self
+000031e0: 2e6c 6162 656c 5f33 392c 2032 2c20 312c  .label_39, 2, 1,
+000031f0: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
+00003200: 656c 662e 7362 5f73 6e75 6d5f 7361 6d70  elf.sb_snum_samp
+00003210: 6c65 203d 2051 7457 6964 6765 7473 2e51  le = QtWidgets.Q
+00003220: 5370 696e 426f 7828 7061 7265 6e74 3d73  SpinBox(parent=s
+00003230: 656c 662e 6672 616d 655f 3329 0a20 2020  elf.frame_3).   
+00003240: 2020 2020 2073 656c 662e 7362 5f73 6e75       self.sb_snu
+00003250: 6d5f 7361 6d70 6c65 2e73 6574 456e 6162  m_sample.setEnab
+00003260: 6c65 6428 4661 6c73 6529 0a20 2020 2020  led(False).     
+00003270: 2020 2073 656c 662e 7362 5f73 6e75 6d5f     self.sb_snum_
+00003280: 7361 6d70 6c65 2e73 6574 4f62 6a65 6374  sample.setObject
+00003290: 4e61 6d65 2822 7362 5f73 6e75 6d5f 7361  Name("sb_snum_sa
+000032a0: 6d70 6c65 2229 0a20 2020 2020 2020 2073  mple").        s
+000032b0: 656c 662e 6772 6964 4c61 796f 7574 5f31  elf.gridLayout_1
+000032c0: 342e 6164 6457 6964 6765 7428 7365 6c66  4.addWidget(self
+000032d0: 2e73 625f 736e 756d 5f73 616d 706c 652c  .sb_snum_sample,
+000032e0: 2033 2c20 302c 2031 2c20 3129 0a20 2020   3, 0, 1, 1).   
+000032f0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00003300: 3334 203d 2051 7457 6964 6765 7473 2e51  34 = QtWidgets.Q
+00003310: 4c61 6265 6c28 7061 7265 6e74 3d73 656c  Label(parent=sel
+00003320: 662e 6672 616d 655f 3329 0a20 2020 2020  f.frame_3).     
+00003330: 2020 2073 697a 6550 6f6c 6963 7920 3d20     sizePolicy = 
+00003340: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
+00003350: 6f6c 6963 7928 5174 5769 6467 6574 732e  olicy(QtWidgets.
+00003360: 5153 697a 6550 6f6c 6963 792e 506f 6c69  QSizePolicy.Poli
+00003370: 6379 2e50 7265 6665 7272 6564 2c20 5174  cy.Preferred, Qt
+00003380: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
+00003390: 6963 792e 506f 6c69 6379 2e4d 696e 696d  icy.Policy.Minim
+000033a0: 756d 290a 2020 2020 2020 2020 7369 7a65  um).        size
+000033b0: 506f 6c69 6379 2e73 6574 486f 7269 7a6f  Policy.setHorizo
+000033c0: 6e74 616c 5374 7265 7463 6828 3029 0a20  ntalStretch(0). 
+000033d0: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
+000033e0: 792e 7365 7456 6572 7469 6361 6c53 7472  y.setVerticalStr
+000033f0: 6574 6368 2830 290a 2020 2020 2020 2020  etch(0).        
+00003400: 7369 7a65 506f 6c69 6379 2e73 6574 4865  sizePolicy.setHe
+00003410: 6967 6874 466f 7257 6964 7468 2873 656c  ightForWidth(sel
+00003420: 662e 6c61 6265 6c5f 3334 2e73 697a 6550  f.label_34.sizeP
+00003430: 6f6c 6963 7928 292e 6861 7348 6569 6768  olicy().hasHeigh
+00003440: 7446 6f72 5769 6474 6828 2929 0a20 2020  tForWidth()).   
+00003450: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00003460: 3334 2e73 6574 5369 7a65 506f 6c69 6379  34.setSizePolicy
+00003470: 2873 697a 6550 6f6c 6963 7929 0a20 2020  (sizePolicy).   
+00003480: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00003490: 3334 2e73 6574 4f62 6a65 6374 4e61 6d65  34.setObjectName
+000034a0: 2822 6c61 6265 6c5f 3334 2229 0a20 2020  ("label_34").   
 000034b0: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
 000034c0: 796f 7574 5f31 342e 6164 6457 6964 6765  yout_14.addWidge
-000034d0: 7428 7365 6c66 2e62 7574 746f 6e5f 7361  t(self.button_sa
-000034e0: 6d70 6c65 2c20 312c 2030 2c20 312c 2031  mple, 1, 0, 1, 1
-000034f0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00003500: 625f 6d68 5f73 616d 706c 6520 3d20 5174  b_mh_sample = Qt
-00003510: 5769 6467 6574 732e 5153 7069 6e42 6f78  Widgets.QSpinBox
-00003520: 2873 656c 662e 6672 616d 655f 3329 0a20  (self.frame_3). 
-00003530: 2020 2020 2020 2073 656c 662e 7362 5f6d         self.sb_m
-00003540: 685f 7361 6d70 6c65 2e73 6574 4d69 6e69  h_sample.setMini
-00003550: 6d75 6d28 3129 0a20 2020 2020 2020 2073  mum(1).        s
-00003560: 656c 662e 7362 5f6d 685f 7361 6d70 6c65  elf.sb_mh_sample
-00003570: 2e73 6574 4d61 7869 6d75 6d28 3330 3029  .setMaximum(300)
-00003580: 0a20 2020 2020 2020 2073 656c 662e 7362  .        self.sb
-00003590: 5f6d 685f 7361 6d70 6c65 2e73 6574 5072  _mh_sample.setPr
-000035a0: 6f70 6572 7479 2822 7661 6c75 6522 2c20  operty("value", 
-000035b0: 3330 290a 2020 2020 2020 2020 7365 6c66  30).        self
-000035c0: 2e73 625f 6d68 5f73 616d 706c 652e 7365  .sb_mh_sample.se
-000035d0: 744f 626a 6563 744e 616d 6528 2273 625f  tObjectName("sb_
-000035e0: 6d68 5f73 616d 706c 6522 290a 2020 2020  mh_sample").    
-000035f0: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-00003600: 6f75 745f 3134 2e61 6464 5769 6467 6574  out_14.addWidget
-00003610: 2873 656c 662e 7362 5f6d 685f 7361 6d70  (self.sb_mh_samp
-00003620: 6c65 2c20 312c 2031 2c20 312c 2031 290a  le, 1, 1, 1, 1).
-00003630: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00003640: 656c 5f33 3820 3d20 5174 5769 6467 6574  el_38 = QtWidget
-00003650: 732e 514c 6162 656c 2873 656c 662e 6672  s.QLabel(self.fr
-00003660: 616d 655f 3329 0a20 2020 2020 2020 2073  ame_3).        s
-00003670: 656c 662e 6c61 6265 6c5f 3338 2e73 6574  elf.label_38.set
-00003680: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
-00003690: 6c5f 3338 2229 0a20 2020 2020 2020 2073  l_38").        s
-000036a0: 656c 662e 6772 6964 4c61 796f 7574 5f31  elf.gridLayout_1
-000036b0: 342e 6164 6457 6964 6765 7428 7365 6c66  4.addWidget(self
-000036c0: 2e6c 6162 656c 5f33 382c 2030 2c20 312c  .label_38, 0, 1,
-000036d0: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
-000036e0: 656c 662e 6275 7474 6f6e 5f73 7461 7274  elf.button_start
-000036f0: 7361 6d70 6c65 203d 2051 7457 6964 6765  sample = QtWidge
-00003700: 7473 2e51 5075 7368 4275 7474 6f6e 2873  ts.QPushButton(s
-00003710: 656c 662e 6672 616d 655f 3329 0a20 2020  elf.frame_3).   
-00003720: 2020 2020 2073 697a 6550 6f6c 6963 7920       sizePolicy 
-00003730: 3d20 5174 5769 6467 6574 732e 5153 697a  = QtWidgets.QSiz
-00003740: 6550 6f6c 6963 7928 5174 5769 6467 6574  ePolicy(QtWidget
-00003750: 732e 5153 697a 6550 6f6c 6963 792e 4d69  s.QSizePolicy.Mi
-00003760: 6e69 6d75 6d2c 2051 7457 6964 6765 7473  nimum, QtWidgets
-00003770: 2e51 5369 7a65 506f 6c69 6379 2e45 7870  .QSizePolicy.Exp
-00003780: 616e 6469 6e67 290a 2020 2020 2020 2020  anding).        
-00003790: 7369 7a65 506f 6c69 6379 2e73 6574 486f  sizePolicy.setHo
-000037a0: 7269 7a6f 6e74 616c 5374 7265 7463 6828  rizontalStretch(
-000037b0: 3029 0a20 2020 2020 2020 2073 697a 6550  0).        sizeP
-000037c0: 6f6c 6963 792e 7365 7456 6572 7469 6361  olicy.setVertica
-000037d0: 6c53 7472 6574 6368 2830 290a 2020 2020  lStretch(0).    
-000037e0: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
-000037f0: 6574 4865 6967 6874 466f 7257 6964 7468  etHeightForWidth
-00003800: 2873 656c 662e 6275 7474 6f6e 5f73 7461  (self.button_sta
-00003810: 7274 7361 6d70 6c65 2e73 697a 6550 6f6c  rtsample.sizePol
-00003820: 6963 7928 292e 6861 7348 6569 6768 7446  icy().hasHeightF
-00003830: 6f72 5769 6474 6828 2929 0a20 2020 2020  orWidth()).     
-00003840: 2020 2073 656c 662e 6275 7474 6f6e 5f73     self.button_s
-00003850: 7461 7274 7361 6d70 6c65 2e73 6574 5369  tartsample.setSi
-00003860: 7a65 506f 6c69 6379 2873 697a 6550 6f6c  zePolicy(sizePol
-00003870: 6963 7929 0a20 2020 2020 2020 2073 656c  icy).        sel
-00003880: 662e 6275 7474 6f6e 5f73 7461 7274 7361  f.button_startsa
-00003890: 6d70 6c65 2e73 6574 4963 6f6e 5369 7a65  mple.setIconSize
-000038a0: 2851 7443 6f72 652e 5153 697a 6528 3139  (QtCore.QSize(19
-000038b0: 2c20 3139 2929 0a20 2020 2020 2020 2073  , 19)).        s
-000038c0: 656c 662e 6275 7474 6f6e 5f73 7461 7274  elf.button_start
-000038d0: 7361 6d70 6c65 2e73 6574 4f62 6a65 6374  sample.setObject
-000038e0: 4e61 6d65 2822 6275 7474 6f6e 5f73 7461  Name("button_sta
-000038f0: 7274 7361 6d70 6c65 2229 0a20 2020 2020  rtsample").     
-00003900: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-00003910: 7574 5f31 342e 6164 6457 6964 6765 7428  ut_14.addWidget(
-00003920: 7365 6c66 2e62 7574 746f 6e5f 7374 6172  self.button_star
-00003930: 7473 616d 706c 652c 2030 2c20 322c 2033  tsample, 0, 2, 3
-00003940: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
-00003950: 662e 6275 7474 6f6e 5f73 6176 655f 7361  f.button_save_sa
-00003960: 6d70 6c65 203d 2051 7457 6964 6765 7473  mple = QtWidgets
-00003970: 2e51 5075 7368 4275 7474 6f6e 2873 656c  .QPushButton(sel
-00003980: 662e 6672 616d 655f 3329 0a20 2020 2020  f.frame_3).     
-00003990: 2020 2073 656c 662e 6275 7474 6f6e 5f73     self.button_s
-000039a0: 6176 655f 7361 6d70 6c65 2e73 6574 4f62  ave_sample.setOb
-000039b0: 6a65 6374 4e61 6d65 2822 6275 7474 6f6e  jectName("button
-000039c0: 5f73 6176 655f 7361 6d70 6c65 2229 0a20  _save_sample"). 
-000039d0: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-000039e0: 4c61 796f 7574 5f31 342e 6164 6457 6964  Layout_14.addWid
-000039f0: 6765 7428 7365 6c66 2e62 7574 746f 6e5f  get(self.button_
-00003a00: 7361 7665 5f73 616d 706c 652c 2033 2c20  save_sample, 3, 
-00003a10: 322c 2031 2c20 3129 0a20 2020 2020 2020  2, 1, 1).       
-00003a20: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
-00003a30: 5f31 332e 6164 6457 6964 6765 7428 7365  _13.addWidget(se
-00003a40: 6c66 2e66 7261 6d65 5f33 2c20 302c 2031  lf.frame_3, 0, 1
-00003a50: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
-00003a60: 7365 6c66 2e74 6162 5769 6467 6574 2e61  self.tabWidget.a
-00003a70: 6464 5461 6228 7365 6c66 2e74 6162 5f35  ddTab(self.tab_5
-00003a80: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
-00003a90: 6c66 2e74 6162 203d 2051 7457 6964 6765  lf.tab = QtWidge
-00003aa0: 7473 2e51 5769 6467 6574 2829 0a20 2020  ts.QWidget().   
-00003ab0: 2020 2020 2073 656c 662e 7461 622e 7365       self.tab.se
-00003ac0: 744f 626a 6563 744e 616d 6528 2274 6162  tObjectName("tab
-00003ad0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00003ae0: 6772 6964 4c61 796f 7574 5f39 203d 2051  gridLayout_9 = Q
-00003af0: 7457 6964 6765 7473 2e51 4772 6964 4c61  tWidgets.QGridLa
-00003b00: 796f 7574 2873 656c 662e 7461 6229 0a20  yout(self.tab). 
-00003b10: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-00003b20: 4c61 796f 7574 5f39 2e73 6574 4f62 6a65  Layout_9.setObje
-00003b30: 6374 4e61 6d65 2822 6772 6964 4c61 796f  ctName("gridLayo
-00003b40: 7574 5f39 2229 0a20 2020 2020 2020 2073  ut_9").        s
-00003b50: 656c 662e 6672 616d 6520 3d20 5174 5769  elf.frame = QtWi
-00003b60: 6467 6574 732e 5146 7261 6d65 2873 656c  dgets.QFrame(sel
-00003b70: 662e 7461 6229 0a20 2020 2020 2020 2073  f.tab).        s
-00003b80: 697a 6550 6f6c 6963 7920 3d20 5174 5769  izePolicy = QtWi
-00003b90: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
-00003ba0: 7928 5174 5769 6467 6574 732e 5153 697a  y(QtWidgets.QSiz
-00003bb0: 6550 6f6c 6963 792e 4578 7061 6e64 696e  ePolicy.Expandin
-00003bc0: 672c 2051 7457 6964 6765 7473 2e51 5369  g, QtWidgets.QSi
-00003bd0: 7a65 506f 6c69 6379 2e45 7870 616e 6469  zePolicy.Expandi
-00003be0: 6e67 290a 2020 2020 2020 2020 7369 7a65  ng).        size
-00003bf0: 506f 6c69 6379 2e73 6574 486f 7269 7a6f  Policy.setHorizo
-00003c00: 6e74 616c 5374 7265 7463 6828 3029 0a20  ntalStretch(0). 
-00003c10: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
-00003c20: 792e 7365 7456 6572 7469 6361 6c53 7472  y.setVerticalStr
-00003c30: 6574 6368 2830 290a 2020 2020 2020 2020  etch(0).        
-00003c40: 7369 7a65 506f 6c69 6379 2e73 6574 4865  sizePolicy.setHe
-00003c50: 6967 6874 466f 7257 6964 7468 2873 656c  ightForWidth(sel
-00003c60: 662e 6672 616d 652e 7369 7a65 506f 6c69  f.frame.sizePoli
-00003c70: 6379 2829 2e68 6173 4865 6967 6874 466f  cy().hasHeightFo
-00003c80: 7257 6964 7468 2829 290a 2020 2020 2020  rWidth()).      
-00003c90: 2020 7365 6c66 2e66 7261 6d65 2e73 6574    self.frame.set
-00003ca0: 5369 7a65 506f 6c69 6379 2873 697a 6550  SizePolicy(sizeP
-00003cb0: 6f6c 6963 7929 0a20 2020 2020 2020 2073  olicy).        s
-00003cc0: 656c 662e 6672 616d 652e 7365 7446 7261  elf.frame.setFra
-00003cd0: 6d65 5368 6170 6528 5174 5769 6467 6574  meShape(QtWidget
-00003ce0: 732e 5146 7261 6d65 2e53 7479 6c65 6450  s.QFrame.StyledP
-00003cf0: 616e 656c 290a 2020 2020 2020 2020 7365  anel).        se
-00003d00: 6c66 2e66 7261 6d65 2e73 6574 4672 616d  lf.frame.setFram
-00003d10: 6553 6861 646f 7728 5174 5769 6467 6574  eShadow(QtWidget
-00003d20: 732e 5146 7261 6d65 2e52 6169 7365 6429  s.QFrame.Raised)
-00003d30: 0a20 2020 2020 2020 2073 656c 662e 6672  .        self.fr
-00003d40: 616d 652e 7365 744f 626a 6563 744e 616d  ame.setObjectNam
-00003d50: 6528 2266 7261 6d65 2229 0a20 2020 2020  e("frame").     
-00003d60: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-00003d70: 7574 5f34 203d 2051 7457 6964 6765 7473  ut_4 = QtWidgets
-00003d80: 2e51 4772 6964 4c61 796f 7574 2873 656c  .QGridLayout(sel
-00003d90: 662e 6672 616d 6529 0a20 2020 2020 2020  f.frame).       
-00003da0: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
-00003db0: 5f34 2e73 6574 4f62 6a65 6374 4e61 6d65  _4.setObjectName
-00003dc0: 2822 6772 6964 4c61 796f 7574 5f34 2229  ("gridLayout_4")
-00003dd0: 0a20 2020 2020 2020 2073 656c 662e 6275  .        self.bu
-00003de0: 7474 6f6e 5f46 5053 203d 2051 7457 6964  tton_FPS = QtWid
-00003df0: 6765 7473 2e51 5075 7368 4275 7474 6f6e  gets.QPushButton
-00003e00: 2873 656c 662e 6672 616d 6529 0a20 2020  (self.frame).   
-00003e10: 2020 2020 2073 697a 6550 6f6c 6963 7920       sizePolicy 
-00003e20: 3d20 5174 5769 6467 6574 732e 5153 697a  = QtWidgets.QSiz
-00003e30: 6550 6f6c 6963 7928 5174 5769 6467 6574  ePolicy(QtWidget
-00003e40: 732e 5153 697a 6550 6f6c 6963 792e 4669  s.QSizePolicy.Fi
-00003e50: 7865 642c 2051 7457 6964 6765 7473 2e51  xed, QtWidgets.Q
-00003e60: 5369 7a65 506f 6c69 6379 2e46 6978 6564  SizePolicy.Fixed
-00003e70: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-00003e80: 6c69 6379 2e73 6574 486f 7269 7a6f 6e74  licy.setHorizont
-00003e90: 616c 5374 7265 7463 6828 3029 0a20 2020  alStretch(0).   
-00003ea0: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
-00003eb0: 7365 7456 6572 7469 6361 6c53 7472 6574  setVerticalStret
-00003ec0: 6368 2830 290a 2020 2020 2020 2020 7369  ch(0).        si
-00003ed0: 7a65 506f 6c69 6379 2e73 6574 4865 6967  zePolicy.setHeig
-00003ee0: 6874 466f 7257 6964 7468 2873 656c 662e  htForWidth(self.
-00003ef0: 6275 7474 6f6e 5f46 5053 2e73 697a 6550  button_FPS.sizeP
-00003f00: 6f6c 6963 7928 292e 6861 7348 6569 6768  olicy().hasHeigh
-00003f10: 7446 6f72 5769 6474 6828 2929 0a20 2020  tForWidth()).   
-00003f20: 2020 2020 2073 656c 662e 6275 7474 6f6e       self.button
-00003f30: 5f46 5053 2e73 6574 5369 7a65 506f 6c69  _FPS.setSizePoli
-00003f40: 6379 2873 697a 6550 6f6c 6963 7929 0a20  cy(sizePolicy). 
-00003f50: 2020 2020 2020 2073 656c 662e 6275 7474         self.butt
-00003f60: 6f6e 5f46 5053 2e73 6574 4f62 6a65 6374  on_FPS.setObject
-00003f70: 4e61 6d65 2822 6275 7474 6f6e 5f46 5053  Name("button_FPS
-00003f80: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00003f90: 6772 6964 4c61 796f 7574 5f34 2e61 6464  gridLayout_4.add
-00003fa0: 5769 6467 6574 2873 656c 662e 6275 7474  Widget(self.butt
-00003fb0: 6f6e 5f46 5053 2c20 322c 2031 2c20 312c  on_FPS, 2, 1, 1,
-00003fc0: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
-00003fd0: 2e70 726f 6772 6573 7342 6172 203d 2051  .progressBar = Q
-00003fe0: 7457 6964 6765 7473 2e51 5072 6f67 7265  tWidgets.QProgre
-00003ff0: 7373 4261 7228 7365 6c66 2e66 7261 6d65  ssBar(self.frame
-00004000: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
-00004010: 726f 6772 6573 7342 6172 2e73 6574 5072  rogressBar.setPr
-00004020: 6f70 6572 7479 2822 7661 6c75 6522 2c20  operty("value", 
-00004030: 3029 0a20 2020 2020 2020 2073 656c 662e  0).        self.
-00004040: 7072 6f67 7265 7373 4261 722e 7365 744f  progressBar.setO
-00004050: 626a 6563 744e 616d 6528 2270 726f 6772  bjectName("progr
-00004060: 6573 7342 6172 2229 0a20 2020 2020 2020  essBar").       
-00004070: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
-00004080: 5f34 2e61 6464 5769 6467 6574 2873 656c  _4.addWidget(sel
-00004090: 662e 7072 6f67 7265 7373 4261 722c 2032  f.progressBar, 2
-000040a0: 2c20 302c 2031 2c20 3129 0a20 2020 2020  , 0, 1, 1).     
-000040b0: 2020 2073 656c 662e 6c6f 6762 6f78 203d     self.logbox =
-000040c0: 2051 7457 6964 6765 7473 2e51 5465 7874   QtWidgets.QText
-000040d0: 4564 6974 2873 656c 662e 6672 616d 6529  Edit(self.frame)
-000040e0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
-000040f0: 6762 6f78 2e73 6574 4f62 6a65 6374 4e61  gbox.setObjectNa
-00004100: 6d65 2822 6c6f 6762 6f78 2229 0a20 2020  me("logbox").   
-00004110: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
-00004120: 796f 7574 5f34 2e61 6464 5769 6467 6574  yout_4.addWidget
-00004130: 2873 656c 662e 6c6f 6762 6f78 2c20 312c  (self.logbox, 1,
-00004140: 2030 2c20 312c 2032 290a 2020 2020 2020   0, 1, 2).      
-00004150: 2020 7365 6c66 2e6c 6162 656c 5f32 203d    self.label_2 =
-00004160: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
-00004170: 6c28 7365 6c66 2e66 7261 6d65 290a 2020  l(self.frame).  
-00004180: 2020 2020 2020 666f 6e74 203d 2051 7447        font = QtG
-00004190: 7569 2e51 466f 6e74 2829 0a20 2020 2020  ui.QFont().     
-000041a0: 2020 2066 6f6e 742e 7365 7442 6f6c 6428     font.setBold(
-000041b0: 5472 7565 290a 2020 2020 2020 2020 666f  True).        fo
-000041c0: 6e74 2e73 6574 5765 6967 6874 2837 3529  nt.setWeight(75)
-000041d0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-000041e0: 6265 6c5f 322e 7365 7446 6f6e 7428 666f  bel_2.setFont(fo
-000041f0: 6e74 290a 2020 2020 2020 2020 7365 6c66  nt).        self
-00004200: 2e6c 6162 656c 5f32 2e73 6574 4f62 6a65  .label_2.setObje
-00004210: 6374 4e61 6d65 2822 6c61 6265 6c5f 3222  ctName("label_2"
-00004220: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-00004230: 7269 644c 6179 6f75 745f 342e 6164 6457  ridLayout_4.addW
-00004240: 6964 6765 7428 7365 6c66 2e6c 6162 656c  idget(self.label
-00004250: 5f32 2c20 302c 2030 2c20 312c 2031 290a  _2, 0, 0, 1, 1).
-00004260: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
-00004270: 644c 6179 6f75 745f 392e 6164 6457 6964  dLayout_9.addWid
-00004280: 6765 7428 7365 6c66 2e66 7261 6d65 2c20  get(self.frame, 
-00004290: 302c 2032 2c20 312c 2031 290a 2020 2020  0, 2, 1, 1).    
-000042a0: 2020 2020 7365 6c66 2e73 6372 6f6c 6c41      self.scrollA
-000042b0: 7265 615f 3220 3d20 5174 5769 6467 6574  rea_2 = QtWidget
-000042c0: 732e 5153 6372 6f6c 6c41 7265 6128 7365  s.QScrollArea(se
-000042d0: 6c66 2e74 6162 290a 2020 2020 2020 2020  lf.tab).        
-000042e0: 7369 7a65 506f 6c69 6379 203d 2051 7457  sizePolicy = QtW
-000042f0: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-00004300: 6379 2851 7457 6964 6765 7473 2e51 5369  cy(QtWidgets.QSi
-00004310: 7a65 506f 6c69 6379 2e45 7870 616e 6469  zePolicy.Expandi
-00004320: 6e67 2c20 5174 5769 6467 6574 732e 5153  ng, QtWidgets.QS
-00004330: 697a 6550 6f6c 6963 792e 4578 7061 6e64  izePolicy.Expand
-00004340: 696e 6729 0a20 2020 2020 2020 2073 697a  ing).        siz
-00004350: 6550 6f6c 6963 792e 7365 7448 6f72 697a  ePolicy.setHoriz
-00004360: 6f6e 7461 6c53 7472 6574 6368 2830 290a  ontalStretch(0).
-00004370: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
-00004380: 6379 2e73 6574 5665 7274 6963 616c 5374  cy.setVerticalSt
-00004390: 7265 7463 6828 3029 0a20 2020 2020 2020  retch(0).       
-000043a0: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
-000043b0: 6569 6768 7446 6f72 5769 6474 6828 7365  eightForWidth(se
-000043c0: 6c66 2e73 6372 6f6c 6c41 7265 615f 322e  lf.scrollArea_2.
-000043d0: 7369 7a65 506f 6c69 6379 2829 2e68 6173  sizePolicy().has
-000043e0: 4865 6967 6874 466f 7257 6964 7468 2829  HeightForWidth()
-000043f0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00004400: 6372 6f6c 6c41 7265 615f 322e 7365 7453  crollArea_2.setS
-00004410: 697a 6550 6f6c 6963 7928 7369 7a65 506f  izePolicy(sizePo
-00004420: 6c69 6379 290a 2020 2020 2020 2020 7365  licy).        se
-00004430: 6c66 2e73 6372 6f6c 6c41 7265 615f 322e  lf.scrollArea_2.
-00004440: 7365 744d 696e 696d 756d 5369 7a65 2851  setMinimumSize(Q
-00004450: 7443 6f72 652e 5153 697a 6528 3230 302c  tCore.QSize(200,
-00004460: 2033 3731 2929 0a20 2020 2020 2020 2073   371)).        s
-00004470: 656c 662e 7363 726f 6c6c 4172 6561 5f32  elf.scrollArea_2
-00004480: 2e73 6574 4d61 7869 6d75 6d53 697a 6528  .setMaximumSize(
-00004490: 5174 436f 7265 2e51 5369 7a65 2833 3030  QtCore.QSize(300
-000044a0: 2c20 3136 3737 3732 3135 2929 0a20 2020  , 16777215)).   
-000044b0: 2020 2020 2073 656c 662e 7363 726f 6c6c       self.scroll
-000044c0: 4172 6561 5f32 2e73 6574 4c69 6e65 5769  Area_2.setLineWi
-000044d0: 6474 6828 3129 0a20 2020 2020 2020 2073  dth(1).        s
-000044e0: 656c 662e 7363 726f 6c6c 4172 6561 5f32  elf.scrollArea_2
-000044f0: 2e73 6574 5665 7274 6963 616c 5363 726f  .setVerticalScro
-00004500: 6c6c 4261 7250 6f6c 6963 7928 5174 436f  llBarPolicy(QtCo
-00004510: 7265 2e51 742e 5363 726f 6c6c 4261 7241  re.Qt.ScrollBarA
-00004520: 6c77 6179 734f 6e29 0a20 2020 2020 2020  lwaysOn).       
-00004530: 2073 656c 662e 7363 726f 6c6c 4172 6561   self.scrollArea
-00004540: 5f32 2e73 6574 5769 6467 6574 5265 7369  _2.setWidgetResi
-00004550: 7a61 626c 6528 5472 7565 290a 2020 2020  zable(True).    
-00004560: 2020 2020 7365 6c66 2e73 6372 6f6c 6c41      self.scrollA
-00004570: 7265 615f 322e 7365 744f 626a 6563 744e  rea_2.setObjectN
-00004580: 616d 6528 2273 6372 6f6c 6c41 7265 615f  ame("scrollArea_
-00004590: 3222 290a 2020 2020 2020 2020 7365 6c66  2").        self
-000045a0: 2e73 6372 6f6c 6c41 7265 6157 6964 6765  .scrollAreaWidge
-000045b0: 7443 6f6e 7465 6e74 735f 3220 3d20 5174  tContents_2 = Qt
-000045c0: 5769 6467 6574 732e 5157 6964 6765 7428  Widgets.QWidget(
-000045d0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-000045e0: 6372 6f6c 6c41 7265 6157 6964 6765 7443  crollAreaWidgetC
-000045f0: 6f6e 7465 6e74 735f 322e 7365 7447 656f  ontents_2.setGeo
-00004600: 6d65 7472 7928 5174 436f 7265 2e51 5265  metry(QtCore.QRe
-00004610: 6374 2830 2c20 302c 2033 3030 2c20 3639  ct(0, 0, 300, 69
-00004620: 3629 290a 2020 2020 2020 2020 7365 6c66  6)).        self
-00004630: 2e73 6372 6f6c 6c41 7265 6157 6964 6765  .scrollAreaWidge
-00004640: 7443 6f6e 7465 6e74 735f 322e 7365 744f  tContents_2.setO
-00004650: 626a 6563 744e 616d 6528 2273 6372 6f6c  bjectName("scrol
-00004660: 6c41 7265 6157 6964 6765 7443 6f6e 7465  lAreaWidgetConte
-00004670: 6e74 735f 3222 290a 2020 2020 2020 2020  nts_2").        
-00004680: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
-00004690: 3220 3d20 5174 5769 6467 6574 732e 5147  2 = QtWidgets.QG
-000046a0: 7269 644c 6179 6f75 7428 7365 6c66 2e73  ridLayout(self.s
-000046b0: 6372 6f6c 6c41 7265 6157 6964 6765 7443  crollAreaWidgetC
-000046c0: 6f6e 7465 6e74 735f 3229 0a20 2020 2020  ontents_2).     
-000046d0: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-000046e0: 7574 5f32 2e73 6574 4f62 6a65 6374 4e61  ut_2.setObjectNa
-000046f0: 6d65 2822 6772 6964 4c61 796f 7574 5f32  me("gridLayout_2
-00004700: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00004710: 7363 616c 655f 6d65 6e75 203d 2051 7457  scale_menu = QtW
-00004720: 6964 6765 7473 2e51 4672 616d 6528 7365  idgets.QFrame(se
-00004730: 6c66 2e73 6372 6f6c 6c41 7265 6157 6964  lf.scrollAreaWid
-00004740: 6765 7443 6f6e 7465 6e74 735f 3229 0a20  getContents_2). 
-00004750: 2020 2020 2020 2073 656c 662e 7363 616c         self.scal
-00004760: 655f 6d65 6e75 2e73 6574 456e 6162 6c65  e_menu.setEnable
-00004770: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
-00004780: 2073 697a 6550 6f6c 6963 7920 3d20 5174   sizePolicy = Qt
-00004790: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
-000047a0: 6963 7928 5174 5769 6467 6574 732e 5153  icy(QtWidgets.QS
-000047b0: 697a 6550 6f6c 6963 792e 5072 6566 6572  izePolicy.Prefer
-000047c0: 7265 642c 2051 7457 6964 6765 7473 2e51  red, QtWidgets.Q
-000047d0: 5369 7a65 506f 6c69 6379 2e46 6978 6564  SizePolicy.Fixed
-000047e0: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-000047f0: 6c69 6379 2e73 6574 486f 7269 7a6f 6e74  licy.setHorizont
-00004800: 616c 5374 7265 7463 6828 3029 0a20 2020  alStretch(0).   
-00004810: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
-00004820: 7365 7456 6572 7469 6361 6c53 7472 6574  setVerticalStret
-00004830: 6368 2830 290a 2020 2020 2020 2020 7369  ch(0).        si
-00004840: 7a65 506f 6c69 6379 2e73 6574 4865 6967  zePolicy.setHeig
-00004850: 6874 466f 7257 6964 7468 2873 656c 662e  htForWidth(self.
-00004860: 7363 616c 655f 6d65 6e75 2e73 697a 6550  scale_menu.sizeP
-00004870: 6f6c 6963 7928 292e 6861 7348 6569 6768  olicy().hasHeigh
-00004880: 7446 6f72 5769 6474 6828 2929 0a20 2020  tForWidth()).   
-00004890: 2020 2020 2073 656c 662e 7363 616c 655f       self.scale_
-000048a0: 6d65 6e75 2e73 6574 5369 7a65 506f 6c69  menu.setSizePoli
-000048b0: 6379 2873 697a 6550 6f6c 6963 7929 0a20  cy(sizePolicy). 
-000048c0: 2020 2020 2020 2073 656c 662e 7363 616c         self.scal
-000048d0: 655f 6d65 6e75 2e73 6574 4672 616d 6553  e_menu.setFrameS
-000048e0: 6861 7065 2851 7457 6964 6765 7473 2e51  hape(QtWidgets.Q
-000048f0: 4672 616d 652e 5374 796c 6564 5061 6e65  Frame.StyledPane
-00004900: 6c29 0a20 2020 2020 2020 2073 656c 662e  l).        self.
-00004910: 7363 616c 655f 6d65 6e75 2e73 6574 4672  scale_menu.setFr
-00004920: 616d 6553 6861 646f 7728 5174 5769 6467  ameShadow(QtWidg
-00004930: 6574 732e 5146 7261 6d65 2e52 6169 7365  ets.QFrame.Raise
-00004940: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00004950: 7363 616c 655f 6d65 6e75 2e73 6574 4f62  scale_menu.setOb
-00004960: 6a65 6374 4e61 6d65 2822 7363 616c 655f  jectName("scale_
-00004970: 6d65 6e75 2229 0a20 2020 2020 2020 2073  menu").        s
-00004980: 656c 662e 6772 6964 4c61 796f 7574 5f33  elf.gridLayout_3
-00004990: 203d 2051 7457 6964 6765 7473 2e51 4772   = QtWidgets.QGr
-000049a0: 6964 4c61 796f 7574 2873 656c 662e 7363  idLayout(self.sc
-000049b0: 616c 655f 6d65 6e75 290a 2020 2020 2020  ale_menu).      
-000049c0: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-000049d0: 745f 332e 7365 744f 626a 6563 744e 616d  t_3.setObjectNam
-000049e0: 6528 2267 7269 644c 6179 6f75 745f 3322  e("gridLayout_3"
-000049f0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00004a00: 6162 656c 5f39 203d 2051 7457 6964 6765  abel_9 = QtWidge
-00004a10: 7473 2e51 4c61 6265 6c28 7365 6c66 2e73  ts.QLabel(self.s
-00004a20: 6361 6c65 5f6d 656e 7529 0a20 2020 2020  cale_menu).     
-00004a30: 2020 2073 656c 662e 6c61 6265 6c5f 392e     self.label_9.
-00004a40: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
-00004a50: 6162 656c 5f39 2229 0a20 2020 2020 2020  abel_9").       
-00004a60: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
-00004a70: 5f33 2e61 6464 5769 6467 6574 2873 656c  _3.addWidget(sel
-00004a80: 662e 6c61 6265 6c5f 392c 2030 2c20 302c  f.label_9, 0, 0,
-00004a90: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
-00004aa0: 656c 662e 6c61 6265 6c5f 3820 3d20 5174  elf.label_8 = Qt
-00004ab0: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
-00004ac0: 656c 662e 7363 616c 655f 6d65 6e75 290a  elf.scale_menu).
-00004ad0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00004ae0: 656c 5f38 2e73 6574 4f62 6a65 6374 4e61  el_8.setObjectNa
-00004af0: 6d65 2822 6c61 6265 6c5f 3822 290a 2020  me("label_8").  
-00004b00: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
-00004b10: 6179 6f75 745f 332e 6164 6457 6964 6765  ayout_3.addWidge
-00004b20: 7428 7365 6c66 2e6c 6162 656c 5f38 2c20  t(self.label_8, 
-00004b30: 312c 2030 2c20 312c 2031 290a 2020 2020  1, 0, 1, 1).    
-00004b40: 2020 2020 7365 6c66 2e74 6578 7442 6f78      self.textBox
-00004b50: 5f73 6361 6c65 5520 3d20 5174 5769 6467  _scaleU = QtWidg
-00004b60: 6574 732e 514c 696e 6545 6469 7428 7365  ets.QLineEdit(se
-00004b70: 6c66 2e73 6361 6c65 5f6d 656e 7529 0a20  lf.scale_menu). 
-00004b80: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
-00004b90: 426f 785f 7363 616c 6555 2e73 6574 4f62  Box_scaleU.setOb
-00004ba0: 6a65 6374 4e61 6d65 2822 7465 7874 426f  jectName("textBo
-00004bb0: 785f 7363 616c 6555 2229 0a20 2020 2020  x_scaleU").     
-00004bc0: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-00004bd0: 7574 5f33 2e61 6464 5769 6467 6574 2873  ut_3.addWidget(s
-00004be0: 656c 662e 7465 7874 426f 785f 7363 616c  elf.textBox_scal
-00004bf0: 6555 2c20 302c 2031 2c20 312c 2031 290a  eU, 0, 1, 1, 1).
-00004c00: 2020 2020 2020 2020 7365 6c66 2e73 7062          self.spb
-00004c10: 5f73 6361 6c65 5369 7a65 203d 2051 7457  _scaleSize = QtW
-00004c20: 6964 6765 7473 2e51 446f 7562 6c65 5370  idgets.QDoubleSp
-00004c30: 696e 426f 7828 7365 6c66 2e73 6361 6c65  inBox(self.scale
-00004c40: 5f6d 656e 7529 0a20 2020 2020 2020 2073  _menu).        s
-00004c50: 656c 662e 7370 625f 7363 616c 6553 697a  elf.spb_scaleSiz
-00004c60: 652e 7365 744d 6178 696d 756d 2839 3939  e.setMaximum(999
-00004c70: 3939 2e30 290a 2020 2020 2020 2020 7365  99.0).        se
-00004c80: 6c66 2e73 7062 5f73 6361 6c65 5369 7a65  lf.spb_scaleSize
-00004c90: 2e73 6574 5369 6e67 6c65 5374 6570 2830  .setSingleStep(0
-00004ca0: 2e31 290a 2020 2020 2020 2020 7365 6c66  .1).        self
-00004cb0: 2e73 7062 5f73 6361 6c65 5369 7a65 2e73  .spb_scaleSize.s
-00004cc0: 6574 5072 6f70 6572 7479 2822 7661 6c75  etProperty("valu
-00004cd0: 6522 2c20 312e 3029 0a20 2020 2020 2020  e", 1.0).       
-00004ce0: 2073 656c 662e 7370 625f 7363 616c 6553   self.spb_scaleS
-00004cf0: 697a 652e 7365 744f 626a 6563 744e 616d  ize.setObjectNam
-00004d00: 6528 2273 7062 5f73 6361 6c65 5369 7a65  e("spb_scaleSize
-00004d10: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00004d20: 6772 6964 4c61 796f 7574 5f33 2e61 6464  gridLayout_3.add
-00004d30: 5769 6467 6574 2873 656c 662e 7370 625f  Widget(self.spb_
-00004d40: 7363 616c 6553 697a 652c 2031 2c20 312c  scaleSize, 1, 1,
-00004d50: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
-00004d60: 656c 662e 6c61 6265 6c5f 3130 203d 2051  elf.label_10 = Q
-00004d70: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
-00004d80: 7365 6c66 2e73 6361 6c65 5f6d 656e 7529  self.scale_menu)
-00004d90: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00004da0: 6265 6c5f 3130 2e73 6574 4f62 6a65 6374  bel_10.setObject
-00004db0: 4e61 6d65 2822 6c61 6265 6c5f 3130 2229  Name("label_10")
-00004dc0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00004dd0: 6964 4c61 796f 7574 5f33 2e61 6464 5769  idLayout_3.addWi
-00004de0: 6467 6574 2873 656c 662e 6c61 6265 6c5f  dget(self.label_
-00004df0: 3130 2c20 322c 2030 2c20 312c 2031 290a  10, 2, 0, 1, 1).
-00004e00: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
-00004e10: 5f73 6361 6c65 506f 7320 3d20 5174 5769  _scalePos = QtWi
-00004e20: 6467 6574 732e 5143 6f6d 626f 426f 7828  dgets.QComboBox(
-00004e30: 7365 6c66 2e73 6361 6c65 5f6d 656e 7529  self.scale_menu)
-00004e40: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
-00004e50: 625f 7363 616c 6550 6f73 2e73 6574 4f62  b_scalePos.setOb
-00004e60: 6a65 6374 4e61 6d65 2822 636d 625f 7363  jectName("cmb_sc
-00004e70: 616c 6550 6f73 2229 0a20 2020 2020 2020  alePos").       
-00004e80: 2073 656c 662e 636d 625f 7363 616c 6550   self.cmb_scaleP
-00004e90: 6f73 2e61 6464 4974 656d 2822 2229 0a20  os.addItem(""). 
-00004ea0: 2020 2020 2020 2073 656c 662e 636d 625f         self.cmb_
-00004eb0: 7363 616c 6550 6f73 2e61 6464 4974 656d  scalePos.addItem
-00004ec0: 2822 2229 0a20 2020 2020 2020 2073 656c  ("").        sel
-00004ed0: 662e 636d 625f 7363 616c 6550 6f73 2e61  f.cmb_scalePos.a
-00004ee0: 6464 4974 656d 2822 2229 0a20 2020 2020  ddItem("").     
-00004ef0: 2020 2073 656c 662e 636d 625f 7363 616c     self.cmb_scal
-00004f00: 6550 6f73 2e61 6464 4974 656d 2822 2229  ePos.addItem("")
-00004f10: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00004f20: 6964 4c61 796f 7574 5f33 2e61 6464 5769  idLayout_3.addWi
-00004f30: 6467 6574 2873 656c 662e 636d 625f 7363  dget(self.cmb_sc
-00004f40: 616c 6550 6f73 2c20 322c 2031 2c20 312c  alePos, 2, 1, 1,
-00004f50: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
-00004f60: 2e67 7269 644c 6179 6f75 745f 322e 6164  .gridLayout_2.ad
-00004f70: 6457 6964 6765 7428 7365 6c66 2e73 6361  dWidget(self.sca
-00004f80: 6c65 5f6d 656e 752c 2032 362c 2030 2c20  le_menu, 26, 0, 
-00004f90: 312c 2033 290a 2020 2020 2020 2020 7365  1, 3).        se
-00004fa0: 6c66 2e6c 6162 656c 5f34 203d 2051 7457  lf.label_4 = QtW
-00004fb0: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
-00004fc0: 6c66 2e73 6372 6f6c 6c41 7265 6157 6964  lf.scrollAreaWid
-00004fd0: 6765 7443 6f6e 7465 6e74 735f 3229 0a20  getContents_2). 
-00004fe0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00004ff0: 6c5f 342e 7365 744c 6179 6f75 7444 6972  l_4.setLayoutDir
-00005000: 6563 7469 6f6e 2851 7443 6f72 652e 5174  ection(QtCore.Qt
-00005010: 2e4c 6566 7454 6f52 6967 6874 290a 2020  .LeftToRight).  
-00005020: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00005030: 5f34 2e73 6574 4f62 6a65 6374 4e61 6d65  _4.setObjectName
-00005040: 2822 6c61 6265 6c5f 3422 290a 2020 2020  ("label_4").    
-00005050: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-00005060: 6f75 745f 322e 6164 6457 6964 6765 7428  out_2.addWidget(
-00005070: 7365 6c66 2e6c 6162 656c 5f34 2c20 3230  self.label_4, 20
-00005080: 2c20 302c 2031 2c20 3129 0a20 2020 2020  , 0, 1, 1).     
-00005090: 2020 2073 656c 662e 6c61 6265 6c5f 7361     self.label_sa
-000050a0: 7665 203d 2051 7457 6964 6765 7473 2e51  ve = QtWidgets.Q
-000050b0: 4c61 6265 6c28 7365 6c66 2e73 6372 6f6c  Label(self.scrol
-000050c0: 6c41 7265 6157 6964 6765 7443 6f6e 7465  lAreaWidgetConte
-000050d0: 6e74 735f 3229 0a20 2020 2020 2020 2073  nts_2).        s
-000050e0: 697a 6550 6f6c 6963 7920 3d20 5174 5769  izePolicy = QtWi
-000050f0: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
-00005100: 7928 5174 5769 6467 6574 732e 5153 697a  y(QtWidgets.QSiz
-00005110: 6550 6f6c 6963 792e 5072 6566 6572 7265  ePolicy.Preferre
-00005120: 642c 2051 7457 6964 6765 7473 2e51 5369  d, QtWidgets.QSi
-00005130: 7a65 506f 6c69 6379 2e46 6978 6564 290a  zePolicy.Fixed).
-00005140: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
-00005150: 6379 2e73 6574 486f 7269 7a6f 6e74 616c  cy.setHorizontal
-00005160: 5374 7265 7463 6828 3029 0a20 2020 2020  Stretch(0).     
-00005170: 2020 2073 697a 6550 6f6c 6963 792e 7365     sizePolicy.se
-00005180: 7456 6572 7469 6361 6c53 7472 6574 6368  tVerticalStretch
-00005190: 2830 290a 2020 2020 2020 2020 7369 7a65  (0).        size
-000051a0: 506f 6c69 6379 2e73 6574 4865 6967 6874  Policy.setHeight
-000051b0: 466f 7257 6964 7468 2873 656c 662e 6c61  ForWidth(self.la
-000051c0: 6265 6c5f 7361 7665 2e73 697a 6550 6f6c  bel_save.sizePol
-000051d0: 6963 7928 292e 6861 7348 6569 6768 7446  icy().hasHeightF
-000051e0: 6f72 5769 6474 6828 2929 0a20 2020 2020  orWidth()).     
-000051f0: 2020 2073 656c 662e 6c61 6265 6c5f 7361     self.label_sa
-00005200: 7665 2e73 6574 5369 7a65 506f 6c69 6379  ve.setSizePolicy
-00005210: 2873 697a 6550 6f6c 6963 7929 0a20 2020  (sizePolicy).   
-00005220: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-00005230: 7361 7665 2e73 6574 4f62 6a65 6374 4e61  save.setObjectNa
-00005240: 6d65 2822 6c61 6265 6c5f 7361 7665 2229  me("label_save")
-00005250: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00005260: 6964 4c61 796f 7574 5f32 2e61 6464 5769  idLayout_2.addWi
-00005270: 6467 6574 2873 656c 662e 6c61 6265 6c5f  dget(self.label_
-00005280: 7361 7665 2c20 3135 2c20 302c 2031 2c20  save, 15, 0, 1, 
-00005290: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-000052a0: 6c69 6e65 203d 2051 7457 6964 6765 7473  line = QtWidgets
-000052b0: 2e51 4672 616d 6528 7365 6c66 2e73 6372  .QFrame(self.scr
-000052c0: 6f6c 6c41 7265 6157 6964 6765 7443 6f6e  ollAreaWidgetCon
-000052d0: 7465 6e74 735f 3229 0a20 2020 2020 2020  tents_2).       
-000052e0: 2073 656c 662e 6c69 6e65 2e73 6574 4672   self.line.setFr
-000052f0: 616d 6553 6861 7065 2851 7457 6964 6765  ameShape(QtWidge
-00005300: 7473 2e51 4672 616d 652e 484c 696e 6529  ts.QFrame.HLine)
-00005310: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00005320: 6e65 2e73 6574 4672 616d 6553 6861 646f  ne.setFrameShado
-00005330: 7728 5174 5769 6467 6574 732e 5146 7261  w(QtWidgets.QFra
-00005340: 6d65 2e53 756e 6b65 6e29 0a20 2020 2020  me.Sunken).     
-00005350: 2020 2073 656c 662e 6c69 6e65 2e73 6574     self.line.set
-00005360: 4f62 6a65 6374 4e61 6d65 2822 6c69 6e65  ObjectName("line
-00005370: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00005380: 6772 6964 4c61 796f 7574 5f32 2e61 6464  gridLayout_2.add
-00005390: 5769 6467 6574 2873 656c 662e 6c69 6e65  Widget(self.line
-000053a0: 2c20 322c 2030 2c20 312c 2033 290a 2020  , 2, 0, 1, 3).  
-000053b0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-000053c0: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
-000053d0: 6265 6c28 7365 6c66 2e73 6372 6f6c 6c41  bel(self.scrollA
-000053e0: 7265 6157 6964 6765 7443 6f6e 7465 6e74  reaWidgetContent
-000053f0: 735f 3229 0a20 2020 2020 2020 2073 656c  s_2).        sel
-00005400: 662e 6c61 6265 6c2e 7365 744f 626a 6563  f.label.setObjec
-00005410: 744e 616d 6528 226c 6162 656c 2229 0a20  tName("label"). 
-00005420: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-00005430: 4c61 796f 7574 5f32 2e61 6464 5769 6467  Layout_2.addWidg
-00005440: 6574 2873 656c 662e 6c61 6265 6c2c 2033  et(self.label, 3
-00005450: 2c20 302c 2031 2c20 3129 0a20 2020 2020  , 0, 1, 1).     
-00005460: 2020 2073 656c 662e 6c69 6e65 5f32 203d     self.line_2 =
-00005470: 2051 7457 6964 6765 7473 2e51 4672 616d   QtWidgets.QFram
-00005480: 6528 7365 6c66 2e73 6372 6f6c 6c41 7265  e(self.scrollAre
-00005490: 6157 6964 6765 7443 6f6e 7465 6e74 735f  aWidgetContents_
-000054a0: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
-000054b0: 6c69 6e65 5f32 2e73 6574 4672 616d 6553  line_2.setFrameS
-000054c0: 6861 7065 2851 7457 6964 6765 7473 2e51  hape(QtWidgets.Q
-000054d0: 4672 616d 652e 484c 696e 6529 0a20 2020  Frame.HLine).   
-000054e0: 2020 2020 2073 656c 662e 6c69 6e65 5f32       self.line_2
-000054f0: 2e73 6574 4672 616d 6553 6861 646f 7728  .setFrameShadow(
-00005500: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-00005510: 2e53 756e 6b65 6e29 0a20 2020 2020 2020  .Sunken).       
-00005520: 2073 656c 662e 6c69 6e65 5f32 2e73 6574   self.line_2.set
-00005530: 4f62 6a65 6374 4e61 6d65 2822 6c69 6e65  ObjectName("line
-00005540: 5f32 2229 0a20 2020 2020 2020 2073 656c  _2").        sel
-00005550: 662e 6772 6964 4c61 796f 7574 5f32 2e61  f.gridLayout_2.a
-00005560: 6464 5769 6467 6574 2873 656c 662e 6c69  ddWidget(self.li
-00005570: 6e65 5f32 2c20 382c 2030 2c20 312c 2033  ne_2, 8, 0, 1, 3
-00005580: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
-00005590: 7574 746f 6e5f 7361 7665 203d 2051 7457  utton_save = QtW
-000055a0: 6964 6765 7473 2e51 5075 7368 4275 7474  idgets.QPushButt
-000055b0: 6f6e 2873 656c 662e 7363 726f 6c6c 4172  on(self.scrollAr
-000055c0: 6561 5769 6467 6574 436f 6e74 656e 7473  eaWidgetContents
-000055d0: 5f32 290a 2020 2020 2020 2020 7365 6c66  _2).        self
-000055e0: 2e62 7574 746f 6e5f 7361 7665 2e73 6574  .button_save.set
-000055f0: 4f62 6a65 6374 4e61 6d65 2822 6275 7474  ObjectName("butt
-00005600: 6f6e 5f73 6176 6522 290a 2020 2020 2020  on_save").      
-00005610: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-00005620: 745f 322e 6164 6457 6964 6765 7428 7365  t_2.addWidget(se
-00005630: 6c66 2e62 7574 746f 6e5f 7361 7665 2c20  lf.button_save, 
-00005640: 3136 2c20 322c 2031 2c20 3129 0a20 2020  16, 2, 1, 1).   
-00005650: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-00005660: 3320 3d20 5174 5769 6467 6574 732e 514c  3 = QtWidgets.QL
-00005670: 6162 656c 2873 656c 662e 7363 726f 6c6c  abel(self.scroll
-00005680: 4172 6561 5769 6467 6574 436f 6e74 656e  AreaWidgetConten
-00005690: 7473 5f32 290a 2020 2020 2020 2020 7369  ts_2).        si
-000056a0: 7a65 506f 6c69 6379 203d 2051 7457 6964  zePolicy = QtWid
-000056b0: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
-000056c0: 2851 7457 6964 6765 7473 2e51 5369 7a65  (QtWidgets.QSize
-000056d0: 506f 6c69 6379 2e50 7265 6665 7272 6564  Policy.Preferred
-000056e0: 2c20 5174 5769 6467 6574 732e 5153 697a  , QtWidgets.QSiz
-000056f0: 6550 6f6c 6963 792e 4669 7865 6429 0a20  ePolicy.Fixed). 
-00005700: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
-00005710: 792e 7365 7448 6f72 697a 6f6e 7461 6c53  y.setHorizontalS
-00005720: 7472 6574 6368 2830 290a 2020 2020 2020  tretch(0).      
-00005730: 2020 7369 7a65 506f 6c69 6379 2e73 6574    sizePolicy.set
-00005740: 5665 7274 6963 616c 5374 7265 7463 6828  VerticalStretch(
-00005750: 3029 0a20 2020 2020 2020 2073 697a 6550  0).        sizeP
-00005760: 6f6c 6963 792e 7365 7448 6569 6768 7446  olicy.setHeightF
-00005770: 6f72 5769 6474 6828 7365 6c66 2e6c 6162  orWidth(self.lab
-00005780: 656c 5f33 2e73 697a 6550 6f6c 6963 7928  el_3.sizePolicy(
-00005790: 292e 6861 7348 6569 6768 7446 6f72 5769  ).hasHeightForWi
-000057a0: 6474 6828 2929 0a20 2020 2020 2020 2073  dth()).        s
-000057b0: 656c 662e 6c61 6265 6c5f 332e 7365 7453  elf.label_3.setS
-000057c0: 697a 6550 6f6c 6963 7928 7369 7a65 506f  izePolicy(sizePo
-000057d0: 6c69 6379 290a 2020 2020 2020 2020 666f  licy).        fo
-000057e0: 6e74 203d 2051 7447 7569 2e51 466f 6e74  nt = QtGui.QFont
-000057f0: 2829 0a20 2020 2020 2020 2066 6f6e 742e  ().        font.
-00005800: 7365 7442 6f6c 6428 5472 7565 290a 2020  setBold(True).  
-00005810: 2020 2020 2020 666f 6e74 2e73 6574 556e        font.setUn
-00005820: 6465 726c 696e 6528 5472 7565 290a 2020  derline(True).  
-00005830: 2020 2020 2020 666f 6e74 2e73 6574 5765        font.setWe
-00005840: 6967 6874 2837 3529 0a20 2020 2020 2020  ight(75).       
-00005850: 2073 656c 662e 6c61 6265 6c5f 332e 7365   self.label_3.se
-00005860: 7446 6f6e 7428 666f 6e74 290a 2020 2020  tFont(font).    
-00005870: 2020 2020 7365 6c66 2e6c 6162 656c 5f33      self.label_3
-00005880: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00005890: 6c61 6265 6c5f 3322 290a 2020 2020 2020  label_3").      
-000058a0: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-000058b0: 745f 322e 6164 6457 6964 6765 7428 7365  t_2.addWidget(se
-000058c0: 6c66 2e6c 6162 656c 5f33 2c20 302c 2030  lf.label_3, 0, 0
-000058d0: 2c20 312c 2033 290a 2020 2020 2020 2020  , 1, 3).        
-000058e0: 7365 6c66 2e6c 696e 655f 666f 6c64 6120  self.line_folda 
-000058f0: 3d20 5174 5769 6467 6574 732e 514c 696e  = QtWidgets.QLin
-00005900: 6545 6469 7428 7365 6c66 2e73 6372 6f6c  eEdit(self.scrol
-00005910: 6c41 7265 6157 6964 6765 7443 6f6e 7465  lAreaWidgetConte
-00005920: 6e74 735f 3229 0a20 2020 2020 2020 2073  nts_2).        s
-00005930: 656c 662e 6c69 6e65 5f66 6f6c 6461 2e73  elf.line_folda.s
-00005940: 6574 5265 6164 4f6e 6c79 2846 616c 7365  etReadOnly(False
-00005950: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00005960: 696e 655f 666f 6c64 612e 7365 744f 626a  ine_folda.setObj
-00005970: 6563 744e 616d 6528 226c 696e 655f 666f  ectName("line_fo
-00005980: 6c64 6122 290a 2020 2020 2020 2020 7365  lda").        se
-00005990: 6c66 2e67 7269 644c 6179 6f75 745f 322e  lf.gridLayout_2.
-000059a0: 6164 6457 6964 6765 7428 7365 6c66 2e6c  addWidget(self.l
-000059b0: 696e 655f 666f 6c64 612c 2031 322c 2030  ine_folda, 12, 0
-000059c0: 2c20 312c 2032 290a 2020 2020 2020 2020  , 1, 2).        
-000059d0: 7365 6c66 2e6c 696e 655f 7361 7665 203d  self.line_save =
-000059e0: 2051 7457 6964 6765 7473 2e51 4c69 6e65   QtWidgets.QLine
-000059f0: 4564 6974 2873 656c 662e 7363 726f 6c6c  Edit(self.scroll
-00005a00: 4172 6561 5769 6467 6574 436f 6e74 656e  AreaWidgetConten
-00005a10: 7473 5f32 290a 2020 2020 2020 2020 7365  ts_2).        se
-00005a20: 6c66 2e6c 696e 655f 7361 7665 2e73 6574  lf.line_save.set
-00005a30: 5265 6164 4f6e 6c79 2846 616c 7365 290a  ReadOnly(False).
-00005a40: 2020 2020 2020 2020 7365 6c66 2e6c 696e          self.lin
-00005a50: 655f 7361 7665 2e73 6574 4f62 6a65 6374  e_save.setObject
-00005a60: 4e61 6d65 2822 6c69 6e65 5f73 6176 6522  Name("line_save"
-00005a70: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-00005a80: 7269 644c 6179 6f75 745f 322e 6164 6457  ridLayout_2.addW
-00005a90: 6964 6765 7428 7365 6c66 2e6c 696e 655f  idget(self.line_
-00005aa0: 7361 7665 2c20 3136 2c20 302c 2031 2c20  save, 16, 0, 1, 
-00005ab0: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
-00005ac0: 6275 7474 6f6e 5f66 6f6c 6461 203d 2051  button_folda = Q
-00005ad0: 7457 6964 6765 7473 2e51 5075 7368 4275  tWidgets.QPushBu
-00005ae0: 7474 6f6e 2873 656c 662e 7363 726f 6c6c  tton(self.scroll
-00005af0: 4172 6561 5769 6467 6574 436f 6e74 656e  AreaWidgetConten
-00005b00: 7473 5f32 290a 2020 2020 2020 2020 7365  ts_2).        se
-00005b10: 6c66 2e62 7574 746f 6e5f 666f 6c64 612e  lf.button_folda.
-00005b20: 7365 744f 626a 6563 744e 616d 6528 2262  setObjectName("b
-00005b30: 7574 746f 6e5f 666f 6c64 6122 290a 2020  utton_folda").  
-00005b40: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
-00005b50: 6179 6f75 745f 322e 6164 6457 6964 6765  ayout_2.addWidge
-00005b60: 7428 7365 6c66 2e62 7574 746f 6e5f 666f  t(self.button_fo
-00005b70: 6c64 612c 2031 322c 2032 2c20 312c 2031  lda, 12, 2, 1, 1
-00005b80: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00005b90: 6162 656c 5f33 3120 3d20 5174 5769 6467  abel_31 = QtWidg
-00005ba0: 6574 732e 514c 6162 656c 2873 656c 662e  ets.QLabel(self.
-00005bb0: 7363 726f 6c6c 4172 6561 5769 6467 6574  scrollAreaWidget
-00005bc0: 436f 6e74 656e 7473 5f32 290a 2020 2020  Contents_2).    
-00005bd0: 2020 2020 7369 7a65 506f 6c69 6379 203d      sizePolicy =
-00005be0: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
-00005bf0: 506f 6c69 6379 2851 7457 6964 6765 7473  Policy(QtWidgets
-00005c00: 2e51 5369 7a65 506f 6c69 6379 2e50 7265  .QSizePolicy.Pre
-00005c10: 6665 7272 6564 2c20 5174 5769 6467 6574  ferred, QtWidget
-00005c20: 732e 5153 697a 6550 6f6c 6963 792e 4669  s.QSizePolicy.Fi
-00005c30: 7865 6429 0a20 2020 2020 2020 2073 697a  xed).        siz
-00005c40: 6550 6f6c 6963 792e 7365 7448 6f72 697a  ePolicy.setHoriz
-00005c50: 6f6e 7461 6c53 7472 6574 6368 2830 290a  ontalStretch(0).
-00005c60: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
-00005c70: 6379 2e73 6574 5665 7274 6963 616c 5374  cy.setVerticalSt
-00005c80: 7265 7463 6828 3029 0a20 2020 2020 2020  retch(0).       
-00005c90: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
-00005ca0: 6569 6768 7446 6f72 5769 6474 6828 7365  eightForWidth(se
-00005cb0: 6c66 2e6c 6162 656c 5f33 312e 7369 7a65  lf.label_31.size
-00005cc0: 506f 6c69 6379 2829 2e68 6173 4865 6967  Policy().hasHeig
-00005cd0: 6874 466f 7257 6964 7468 2829 290a 2020  htForWidth()).  
-00005ce0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00005cf0: 5f33 312e 7365 7453 697a 6550 6f6c 6963  _31.setSizePolic
-00005d00: 7928 7369 7a65 506f 6c69 6379 290a 2020  y(sizePolicy).  
-00005d10: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00005d20: 5f33 312e 7365 744f 626a 6563 744e 616d  _31.setObjectNam
-00005d30: 6528 226c 6162 656c 5f33 3122 290a 2020  e("label_31").  
-00005d40: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
-00005d50: 6179 6f75 745f 322e 6164 6457 6964 6765  ayout_2.addWidge
-00005d60: 7428 7365 6c66 2e6c 6162 656c 5f33 312c  t(self.label_31,
-00005d70: 2031 382c 2030 2c20 312c 2033 290a 2020   18, 0, 1, 3).  
-00005d80: 2020 2020 2020 7365 6c66 2e63 625f 7361        self.cb_sa
-00005d90: 7665 416c 6c20 3d20 5174 5769 6467 6574  veAll = QtWidget
-00005da0: 732e 5143 6865 636b 426f 7828 7365 6c66  s.QCheckBox(self
-00005db0: 2e73 6372 6f6c 6c41 7265 6157 6964 6765  .scrollAreaWidge
-00005dc0: 7443 6f6e 7465 6e74 735f 3229 0a20 2020  tContents_2).   
-00005dd0: 2020 2020 2073 656c 662e 6362 5f73 6176       self.cb_sav
-00005de0: 6541 6c6c 2e73 6574 4f62 6a65 6374 4e61  eAll.setObjectNa
-00005df0: 6d65 2822 6362 5f73 6176 6541 6c6c 2229  me("cb_saveAll")
-00005e00: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00005e10: 6964 4c61 796f 7574 5f32 2e61 6464 5769  idLayout_2.addWi
-00005e20: 6467 6574 2873 656c 662e 6362 5f73 6176  dget(self.cb_sav
-00005e30: 6541 6c6c 2c20 3137 2c20 302c 2031 2c20  eAll, 17, 0, 1, 
-00005e40: 3329 0a20 2020 2020 2020 2073 656c 662e  3).        self.
-00005e50: 7262 5f66 696c 656e 616d 6520 3d20 5174  rb_filename = Qt
-00005e60: 5769 6467 6574 732e 5152 6164 696f 4275  Widgets.QRadioBu
-00005e70: 7474 6f6e 2873 656c 662e 7363 726f 6c6c  tton(self.scroll
-00005e80: 4172 6561 5769 6467 6574 436f 6e74 656e  AreaWidgetConten
-00005e90: 7473 5f32 290a 2020 2020 2020 2020 7365  ts_2).        se
-00005ea0: 6c66 2e72 625f 6669 6c65 6e61 6d65 2e73  lf.rb_filename.s
-00005eb0: 6574 4f62 6a65 6374 4e61 6d65 2822 7262  etObjectName("rb
-00005ec0: 5f66 696c 656e 616d 6522 290a 2020 2020  _filename").    
-00005ed0: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-00005ee0: 6f75 745f 322e 6164 6457 6964 6765 7428  out_2.addWidget(
-00005ef0: 7365 6c66 2e72 625f 6669 6c65 6e61 6d65  self.rb_filename
-00005f00: 2c20 372c 2030 2c20 312c 2033 290a 2020  , 7, 0, 1, 3).  
-00005f10: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00005f20: 5f33 3220 3d20 5174 5769 6467 6574 732e  _32 = QtWidgets.
-00005f30: 514c 6162 656c 2873 656c 662e 7363 726f  QLabel(self.scro
-00005f40: 6c6c 4172 6561 5769 6467 6574 436f 6e74  llAreaWidgetCont
-00005f50: 656e 7473 5f32 290a 2020 2020 2020 2020  ents_2).        
-00005f60: 7369 7a65 506f 6c69 6379 203d 2051 7457  sizePolicy = QtW
-00005f70: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-00005f80: 6379 2851 7457 6964 6765 7473 2e51 5369  cy(QtWidgets.QSi
-00005f90: 7a65 506f 6c69 6379 2e50 7265 6665 7272  zePolicy.Preferr
-00005fa0: 6564 2c20 5174 5769 6467 6574 732e 5153  ed, QtWidgets.QS
-00005fb0: 697a 6550 6f6c 6963 792e 4669 7865 6429  izePolicy.Fixed)
-00005fc0: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
-00005fd0: 6963 792e 7365 7448 6f72 697a 6f6e 7461  icy.setHorizonta
-00005fe0: 6c53 7472 6574 6368 2830 290a 2020 2020  lStretch(0).    
-00005ff0: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
-00006000: 6574 5665 7274 6963 616c 5374 7265 7463  etVerticalStretc
-00006010: 6828 3029 0a20 2020 2020 2020 2073 697a  h(0).        siz
-00006020: 6550 6f6c 6963 792e 7365 7448 6569 6768  ePolicy.setHeigh
-00006030: 7446 6f72 5769 6474 6828 7365 6c66 2e6c  tForWidth(self.l
-00006040: 6162 656c 5f33 322e 7369 7a65 506f 6c69  abel_32.sizePoli
-00006050: 6379 2829 2e68 6173 4865 6967 6874 466f  cy().hasHeightFo
-00006060: 7257 6964 7468 2829 290a 2020 2020 2020  rWidth()).      
-00006070: 2020 7365 6c66 2e6c 6162 656c 5f33 322e    self.label_32.
-00006080: 7365 7453 697a 6550 6f6c 6963 7928 7369  setSizePolicy(si
-00006090: 7a65 506f 6c69 6379 290a 2020 2020 2020  zePolicy).      
-000060a0: 2020 7365 6c66 2e6c 6162 656c 5f33 322e    self.label_32.
-000060b0: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
-000060c0: 6162 656c 5f33 3222 290a 2020 2020 2020  abel_32").      
-000060d0: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-000060e0: 745f 322e 6164 6457 6964 6765 7428 7365  t_2.addWidget(se
-000060f0: 6c66 2e6c 6162 656c 5f33 322c 2034 2c20  lf.label_32, 4, 
-00006100: 302c 2031 2c20 3329 0a20 2020 2020 2020  0, 1, 3).       
-00006110: 2073 656c 662e 7262 5f73 7562 666f 6c64   self.rb_subfold
-00006120: 6120 3d20 5174 5769 6467 6574 732e 5152  a = QtWidgets.QR
-00006130: 6164 696f 4275 7474 6f6e 2873 656c 662e  adioButton(self.
-00006140: 7363 726f 6c6c 4172 6561 5769 6467 6574  scrollAreaWidget
-00006150: 436f 6e74 656e 7473 5f32 290a 2020 2020  Contents_2).    
-00006160: 2020 2020 7365 6c66 2e72 625f 7375 6266      self.rb_subf
-00006170: 6f6c 6461 2e73 6574 4368 6563 6b65 6428  olda.setChecked(
-00006180: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
-00006190: 6c66 2e72 625f 7375 6266 6f6c 6461 2e73  lf.rb_subfolda.s
-000061a0: 6574 4f62 6a65 6374 4e61 6d65 2822 7262  etObjectName("rb
-000061b0: 5f73 7562 666f 6c64 6122 290a 2020 2020  _subfolda").    
-000061c0: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-000061d0: 6f75 745f 322e 6164 6457 6964 6765 7428  out_2.addWidget(
-000061e0: 7365 6c66 2e72 625f 7375 6266 6f6c 6461  self.rb_subfolda
-000061f0: 2c20 362c 2030 2c20 312c 2033 290a 2020  , 6, 0, 1, 3).  
-00006200: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00006210: 5f35 203d 2051 7457 6964 6765 7473 2e51  _5 = QtWidgets.Q
-00006220: 4c61 6265 6c28 7365 6c66 2e73 6372 6f6c  Label(self.scrol
-00006230: 6c41 7265 6157 6964 6765 7443 6f6e 7465  lAreaWidgetConte
-00006240: 6e74 735f 3229 0a20 2020 2020 2020 2073  nts_2).        s
-00006250: 656c 662e 6c61 6265 6c5f 352e 7365 744c  elf.label_5.setL
-00006260: 6179 6f75 7444 6972 6563 7469 6f6e 2851  ayoutDirection(Q
-00006270: 7443 6f72 652e 5174 2e4c 6566 7454 6f52  tCore.Qt.LeftToR
-00006280: 6967 6874 290a 2020 2020 2020 2020 7365  ight).        se
-00006290: 6c66 2e6c 6162 656c 5f35 2e73 6574 4f62  lf.label_5.setOb
-000062a0: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
-000062b0: 3522 290a 2020 2020 2020 2020 7365 6c66  5").        self
-000062c0: 2e67 7269 644c 6179 6f75 745f 322e 6164  .gridLayout_2.ad
-000062d0: 6457 6964 6765 7428 7365 6c66 2e6c 6162  dWidget(self.lab
-000062e0: 656c 5f35 2c20 3233 2c20 302c 2031 2c20  el_5, 23, 0, 1, 
-000062f0: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
-00006300: 6c69 6e65 5f68 6561 6465 7220 3d20 5174  line_header = Qt
-00006310: 5769 6467 6574 732e 514c 696e 6545 6469  Widgets.QLineEdi
-00006320: 7428 7365 6c66 2e73 6372 6f6c 6c41 7265  t(self.scrollAre
-00006330: 6157 6964 6765 7443 6f6e 7465 6e74 735f  aWidgetContents_
-00006340: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
-00006350: 6c69 6e65 5f68 6561 6465 722e 7365 744f  line_header.setO
-00006360: 626a 6563 744e 616d 6528 226c 696e 655f  bjectName("line_
-00006370: 6865 6164 6572 2229 0a20 2020 2020 2020  header").       
-00006380: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
-00006390: 5f32 2e61 6464 5769 6467 6574 2873 656c  _2.addWidget(sel
-000063a0: 662e 6c69 6e65 5f68 6561 6465 722c 2031  f.line_header, 1
-000063b0: 342c 2030 2c20 312c 2032 290a 2020 2020  4, 0, 1, 2).    
-000063c0: 2020 2020 7365 6c66 2e6c 6162 656c 5f66      self.label_f
-000063d0: 6f6c 6461 203d 2051 7457 6964 6765 7473  olda = QtWidgets
-000063e0: 2e51 4c61 6265 6c28 7365 6c66 2e73 6372  .QLabel(self.scr
-000063f0: 6f6c 6c41 7265 6157 6964 6765 7443 6f6e  ollAreaWidgetCon
-00006400: 7465 6e74 735f 3229 0a20 2020 2020 2020  tents_2).       
-00006410: 2073 697a 6550 6f6c 6963 7920 3d20 5174   sizePolicy = Qt
-00006420: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
-00006430: 6963 7928 5174 5769 6467 6574 732e 5153  icy(QtWidgets.QS
-00006440: 697a 6550 6f6c 6963 792e 5072 6566 6572  izePolicy.Prefer
-00006450: 7265 642c 2051 7457 6964 6765 7473 2e51  red, QtWidgets.Q
-00006460: 5369 7a65 506f 6c69 6379 2e46 6978 6564  SizePolicy.Fixed
-00006470: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-00006480: 6c69 6379 2e73 6574 486f 7269 7a6f 6e74  licy.setHorizont
-00006490: 616c 5374 7265 7463 6828 3029 0a20 2020  alStretch(0).   
-000064a0: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
-000064b0: 7365 7456 6572 7469 6361 6c53 7472 6574  setVerticalStret
-000064c0: 6368 2830 290a 2020 2020 2020 2020 7369  ch(0).        si
-000064d0: 7a65 506f 6c69 6379 2e73 6574 4865 6967  zePolicy.setHeig
-000064e0: 6874 466f 7257 6964 7468 2873 656c 662e  htForWidth(self.
-000064f0: 6c61 6265 6c5f 666f 6c64 612e 7369 7a65  label_folda.size
-00006500: 506f 6c69 6379 2829 2e68 6173 4865 6967  Policy().hasHeig
-00006510: 6874 466f 7257 6964 7468 2829 290a 2020  htForWidth()).  
-00006520: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00006530: 5f66 6f6c 6461 2e73 6574 5369 7a65 506f  _folda.setSizePo
-00006540: 6c69 6379 2873 697a 6550 6f6c 6963 7929  licy(sizePolicy)
-00006550: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00006560: 6265 6c5f 666f 6c64 612e 7365 744f 626a  bel_folda.setObj
-00006570: 6563 744e 616d 6528 226c 6162 656c 5f66  ectName("label_f
-00006580: 6f6c 6461 2229 0a20 2020 2020 2020 2073  olda").        s
-00006590: 656c 662e 6772 6964 4c61 796f 7574 5f32  elf.gridLayout_2
-000065a0: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
-000065b0: 6c61 6265 6c5f 666f 6c64 612c 2031 302c  label_folda, 10,
-000065c0: 2030 2c20 312c 2033 290a 2020 2020 2020   0, 1, 3).      
-000065d0: 2020 7365 6c66 2e6c 6162 656c 5f31 3720    self.label_17 
-000065e0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-000065f0: 656c 2873 656c 662e 7363 726f 6c6c 4172  el(self.scrollAr
-00006600: 6561 5769 6467 6574 436f 6e74 656e 7473  eaWidgetContents
-00006610: 5f32 290a 2020 2020 2020 2020 7369 7a65  _2).        size
-00006620: 506f 6c69 6379 203d 2051 7457 6964 6765  Policy = QtWidge
-00006630: 7473 2e51 5369 7a65 506f 6c69 6379 2851  ts.QSizePolicy(Q
-00006640: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
-00006650: 6c69 6379 2e50 7265 6665 7272 6564 2c20  licy.Preferred, 
-00006660: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
-00006670: 6f6c 6963 792e 4669 7865 6429 0a20 2020  olicy.Fixed).   
-00006680: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
-00006690: 7365 7448 6f72 697a 6f6e 7461 6c53 7472  setHorizontalStr
-000066a0: 6574 6368 2830 290a 2020 2020 2020 2020  etch(0).        
-000066b0: 7369 7a65 506f 6c69 6379 2e73 6574 5665  sizePolicy.setVe
-000066c0: 7274 6963 616c 5374 7265 7463 6828 3029  rticalStretch(0)
-000066d0: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
-000066e0: 6963 792e 7365 7448 6569 6768 7446 6f72  icy.setHeightFor
-000066f0: 5769 6474 6828 7365 6c66 2e6c 6162 656c  Width(self.label
-00006700: 5f31 372e 7369 7a65 506f 6c69 6379 2829  _17.sizePolicy()
-00006710: 2e68 6173 4865 6967 6874 466f 7257 6964  .hasHeightForWid
-00006720: 7468 2829 290a 2020 2020 2020 2020 7365  th()).        se
-00006730: 6c66 2e6c 6162 656c 5f31 372e 7365 7453  lf.label_17.setS
-00006740: 697a 6550 6f6c 6963 7928 7369 7a65 506f  izePolicy(sizePo
-00006750: 6c69 6379 290a 2020 2020 2020 2020 7365  licy).        se
-00006760: 6c66 2e6c 6162 656c 5f31 372e 7365 744f  lf.label_17.setO
-00006770: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
-00006780: 5f31 3722 290a 2020 2020 2020 2020 7365  _17").        se
-00006790: 6c66 2e67 7269 644c 6179 6f75 745f 322e  lf.gridLayout_2.
-000067a0: 6164 6457 6964 6765 7428 7365 6c66 2e6c  addWidget(self.l
-000067b0: 6162 656c 5f31 372c 2031 332c 2030 2c20  abel_17, 13, 0, 
-000067c0: 312c 2033 290a 2020 2020 2020 2020 7365  1, 3).        se
-000067d0: 6c66 2e62 7574 746f 6e5f 6865 6164 6572  lf.button_header
-000067e0: 203d 2051 7457 6964 6765 7473 2e51 5075   = QtWidgets.QPu
-000067f0: 7368 4275 7474 6f6e 2873 656c 662e 7363  shButton(self.sc
-00006800: 726f 6c6c 4172 6561 5769 6467 6574 436f  rollAreaWidgetCo
-00006810: 6e74 656e 7473 5f32 290a 2020 2020 2020  ntents_2).      
-00006820: 2020 7365 6c66 2e62 7574 746f 6e5f 6865    self.button_he
-00006830: 6164 6572 2e73 6574 4f62 6a65 6374 4e61  ader.setObjectNa
-00006840: 6d65 2822 6275 7474 6f6e 5f68 6561 6465  me("button_heade
-00006850: 7222 290a 2020 2020 2020 2020 7365 6c66  r").        self
-00006860: 2e67 7269 644c 6179 6f75 745f 322e 6164  .gridLayout_2.ad
-00006870: 6457 6964 6765 7428 7365 6c66 2e62 7574  dWidget(self.but
-00006880: 746f 6e5f 6865 6164 6572 2c20 3134 2c20  ton_header, 14, 
-00006890: 322c 2031 2c20 3129 0a20 2020 2020 2020  2, 1, 1).       
-000068a0: 2073 656c 662e 636d 625f 666f 726d 6174   self.cmb_format
-000068b0: 203d 2051 7457 6964 6765 7473 2e51 436f   = QtWidgets.QCo
-000068c0: 6d62 6f42 6f78 2873 656c 662e 7363 726f  mboBox(self.scro
-000068d0: 6c6c 4172 6561 5769 6467 6574 436f 6e74  llAreaWidgetCont
-000068e0: 656e 7473 5f32 290a 2020 2020 2020 2020  ents_2).        
-000068f0: 7365 6c66 2e63 6d62 5f66 6f72 6d61 742e  self.cmb_format.
-00006900: 7365 744f 626a 6563 744e 616d 6528 2263  setObjectName("c
-00006910: 6d62 5f66 6f72 6d61 7422 290a 2020 2020  mb_format").    
-00006920: 2020 2020 7365 6c66 2e63 6d62 5f66 6f72      self.cmb_for
-00006930: 6d61 742e 6164 6449 7465 6d28 2222 290a  mat.addItem("").
-00006940: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
-00006950: 5f66 6f72 6d61 742e 6164 6449 7465 6d28  _format.addItem(
-00006960: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
-00006970: 2e63 6d62 5f66 6f72 6d61 742e 6164 6449  .cmb_format.addI
-00006980: 7465 6d28 2222 290a 2020 2020 2020 2020  tem("").        
-00006990: 7365 6c66 2e63 6d62 5f66 6f72 6d61 742e  self.cmb_format.
-000069a0: 6164 6449 7465 6d28 2222 290a 2020 2020  addItem("").    
-000069b0: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-000069c0: 6f75 745f 322e 6164 6457 6964 6765 7428  out_2.addWidget(
-000069d0: 7365 6c66 2e63 6d62 5f66 6f72 6d61 742c  self.cmb_format,
-000069e0: 2033 2c20 322c 2031 2c20 3129 0a20 2020   3, 2, 1, 1).   
-000069f0: 2020 2020 2073 656c 662e 636d 625f 7363       self.cmb_sc
-00006a00: 616c 6554 7970 6520 3d20 5174 5769 6467  aleType = QtWidg
-00006a10: 6574 732e 5143 6f6d 626f 426f 7828 7365  ets.QComboBox(se
-00006a20: 6c66 2e73 6372 6f6c 6c41 7265 6157 6964  lf.scrollAreaWid
-00006a30: 6765 7443 6f6e 7465 6e74 735f 3229 0a20  getContents_2). 
-00006a40: 2020 2020 2020 2073 656c 662e 636d 625f         self.cmb_
-00006a50: 7363 616c 6554 7970 652e 7365 744f 626a  scaleType.setObj
-00006a60: 6563 744e 616d 6528 2263 6d62 5f73 6361  ectName("cmb_sca
-00006a70: 6c65 5479 7065 2229 0a20 2020 2020 2020  leType").       
-00006a80: 2073 656c 662e 636d 625f 7363 616c 6554   self.cmb_scaleT
-00006a90: 7970 652e 6164 6449 7465 6d28 2222 290a  ype.addItem("").
-00006aa0: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
-00006ab0: 5f73 6361 6c65 5479 7065 2e61 6464 4974  _scaleType.addIt
-00006ac0: 656d 2822 2229 0a20 2020 2020 2020 2073  em("").        s
-00006ad0: 656c 662e 636d 625f 7363 616c 6554 7970  elf.cmb_scaleTyp
-00006ae0: 652e 6164 6449 7465 6d28 2222 290a 2020  e.addItem("").  
-00006af0: 2020 2020 2020 7365 6c66 2e63 6d62 5f73        self.cmb_s
-00006b00: 6361 6c65 5479 7065 2e61 6464 4974 656d  caleType.addItem
-00006b10: 2822 2229 0a20 2020 2020 2020 2073 656c  ("").        sel
-00006b20: 662e 6772 6964 4c61 796f 7574 5f32 2e61  f.gridLayout_2.a
-00006b30: 6464 5769 6467 6574 2873 656c 662e 636d  ddWidget(self.cm
-00006b40: 625f 7363 616c 6554 7970 652c 2032 352c  b_scaleType, 25,
-00006b50: 2031 2c20 312c 2032 290a 2020 2020 2020   1, 1, 2).      
-00006b60: 2020 7365 6c66 2e73 7062 5f6d 7078 6120    self.spb_mpxa 
-00006b70: 3d20 5174 5769 6467 6574 732e 5153 7069  = QtWidgets.QSpi
-00006b80: 6e42 6f78 2873 656c 662e 7363 726f 6c6c  nBox(self.scroll
-00006b90: 4172 6561 5769 6467 6574 436f 6e74 656e  AreaWidgetConten
-00006ba0: 7473 5f32 290a 2020 2020 2020 2020 7365  ts_2).        se
-00006bb0: 6c66 2e73 7062 5f6d 7078 612e 7365 744d  lf.spb_mpxa.setM
-00006bc0: 696e 696d 756d 2831 3030 290a 2020 2020  inimum(100).    
-00006bd0: 2020 2020 7365 6c66 2e73 7062 5f6d 7078      self.spb_mpx
-00006be0: 612e 7365 744d 6178 696d 756d 2834 3939  a.setMaximum(499
-00006bf0: 3939 3929 0a20 2020 2020 2020 2073 656c  999).        sel
-00006c00: 662e 7370 625f 6d70 7861 2e73 6574 5072  f.spb_mpxa.setPr
-00006c10: 6f70 6572 7479 2822 7661 6c75 6522 2c20  operty("value", 
-00006c20: 3230 3029 0a20 2020 2020 2020 2073 656c  200).        sel
-00006c30: 662e 7370 625f 6d70 7861 2e73 6574 4f62  f.spb_mpxa.setOb
-00006c40: 6a65 6374 4e61 6d65 2822 7370 625f 6d70  jectName("spb_mp
-00006c50: 7861 2229 0a20 2020 2020 2020 2073 656c  xa").        sel
-00006c60: 662e 6772 6964 4c61 796f 7574 5f32 2e61  f.gridLayout_2.a
-00006c70: 6464 5769 6467 6574 2873 656c 662e 7370  ddWidget(self.sp
-00006c80: 625f 6d70 7861 2c20 3233 2c20 322c 2031  b_mpxa, 23, 2, 1
-00006c90: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
-00006ca0: 662e 6c61 6265 6c5f 3720 3d20 5174 5769  f.label_7 = QtWi
-00006cb0: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-00006cc0: 662e 7363 726f 6c6c 4172 6561 5769 6467  f.scrollAreaWidg
-00006cd0: 6574 436f 6e74 656e 7473 5f32 290a 2020  etContents_2).  
-00006ce0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00006cf0: 5f37 2e73 6574 4f62 6a65 6374 4e61 6d65  _7.setObjectName
-00006d00: 2822 6c61 6265 6c5f 3722 290a 2020 2020  ("label_7").    
-00006d10: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-00006d20: 6f75 745f 322e 6164 6457 6964 6765 7428  out_2.addWidget(
-00006d30: 7365 6c66 2e6c 6162 656c 5f37 2c20 3235  self.label_7, 25
-00006d40: 2c20 302c 2031 2c20 3129 0a20 2020 2020  , 0, 1, 1).     
-00006d50: 2020 2073 656c 662e 6c69 6e65 5f33 203d     self.line_3 =
-00006d60: 2051 7457 6964 6765 7473 2e51 4672 616d   QtWidgets.QFram
-00006d70: 6528 7365 6c66 2e73 6372 6f6c 6c41 7265  e(self.scrollAre
-00006d80: 6157 6964 6765 7443 6f6e 7465 6e74 735f  aWidgetContents_
-00006d90: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
-00006da0: 6c69 6e65 5f33 2e73 6574 4672 616d 6553  line_3.setFrameS
-00006db0: 6861 7065 2851 7457 6964 6765 7473 2e51  hape(QtWidgets.Q
-00006dc0: 4672 616d 652e 484c 696e 6529 0a20 2020  Frame.HLine).   
-00006dd0: 2020 2020 2073 656c 662e 6c69 6e65 5f33       self.line_3
-00006de0: 2e73 6574 4672 616d 6553 6861 646f 7728  .setFrameShadow(
-00006df0: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-00006e00: 2e53 756e 6b65 6e29 0a20 2020 2020 2020  .Sunken).       
-00006e10: 2073 656c 662e 6c69 6e65 5f33 2e73 6574   self.line_3.set
-00006e20: 4f62 6a65 6374 4e61 6d65 2822 6c69 6e65  ObjectName("line
-00006e30: 5f33 2229 0a20 2020 2020 2020 2073 656c  _3").        sel
-00006e40: 662e 6772 6964 4c61 796f 7574 5f32 2e61  f.gridLayout_2.a
-00006e50: 6464 5769 6467 6574 2873 656c 662e 6c69  ddWidget(self.li
-00006e60: 6e65 5f33 2c20 3139 2c20 302c 2031 2c20  ne_3, 19, 0, 1, 
-00006e70: 3329 0a20 2020 2020 2020 2073 656c 662e  3).        self.
-00006e80: 7262 5f6e 6f6e 6520 3d20 5174 5769 6467  rb_none = QtWidg
-00006e90: 6574 732e 5152 6164 696f 4275 7474 6f6e  ets.QRadioButton
-00006ea0: 2873 656c 662e 7363 726f 6c6c 4172 6561  (self.scrollArea
-00006eb0: 5769 6467 6574 436f 6e74 656e 7473 5f32  WidgetContents_2
-00006ec0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-00006ed0: 625f 6e6f 6e65 2e73 6574 4368 6563 6b65  b_none.setChecke
-00006ee0: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
-00006ef0: 2073 656c 662e 7262 5f6e 6f6e 652e 7365   self.rb_none.se
-00006f00: 744f 626a 6563 744e 616d 6528 2272 625f  tObjectName("rb_
-00006f10: 6e6f 6e65 2229 0a20 2020 2020 2020 2073  none").        s
-00006f20: 656c 662e 6772 6964 4c61 796f 7574 5f32  elf.gridLayout_2
-00006f30: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
-00006f40: 7262 5f6e 6f6e 652c 2035 2c20 302c 2031  rb_none, 5, 0, 1
-00006f50: 2c20 3329 0a20 2020 2020 2020 2073 656c  , 3).        sel
-00006f60: 662e 7370 625f 4e20 3d20 5174 5769 6467  f.spb_N = QtWidg
-00006f70: 6574 732e 5153 7069 6e42 6f78 2873 656c  ets.QSpinBox(sel
-00006f80: 662e 7363 726f 6c6c 4172 6561 5769 6467  f.scrollAreaWidg
-00006f90: 6574 436f 6e74 656e 7473 5f32 290a 2020  etContents_2).  
-00006fa0: 2020 2020 2020 7365 6c66 2e73 7062 5f4e        self.spb_N
-00006fb0: 2e73 6574 4d69 6e69 6d75 6d28 3329 0a20  .setMinimum(3). 
-00006fc0: 2020 2020 2020 2073 656c 662e 7370 625f         self.spb_
-00006fd0: 4e2e 7365 744d 6178 696d 756d 2832 3030  N.setMaximum(200
-00006fe0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00006ff0: 7062 5f4e 2e73 6574 5072 6f70 6572 7479  pb_N.setProperty
-00007000: 2822 7661 6c75 6522 2c20 3330 290a 2020  ("value", 30).  
-00007010: 2020 2020 2020 7365 6c66 2e73 7062 5f4e        self.spb_N
-00007020: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00007030: 7370 625f 4e22 290a 2020 2020 2020 2020  spb_N").        
-00007040: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
-00007050: 322e 6164 6457 6964 6765 7428 7365 6c66  2.addWidget(self
-00007060: 2e73 7062 5f4e 2c20 3230 2c20 322c 2031  .spb_N, 20, 2, 1
-00007070: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
-00007080: 662e 6c61 6265 6c5f 3620 3d20 5174 5769  f.label_6 = QtWi
-00007090: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-000070a0: 662e 7363 726f 6c6c 4172 6561 5769 6467  f.scrollAreaWidg
-000070b0: 6574 436f 6e74 656e 7473 5f32 290a 2020  etContents_2).  
-000070c0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-000070d0: 5f36 2e73 6574 4f62 6a65 6374 4e61 6d65  _6.setObjectName
-000070e0: 2822 6c61 6265 6c5f 3622 290a 2020 2020  ("label_6").    
-000070f0: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-00007100: 6f75 745f 322e 6164 6457 6964 6765 7428  out_2.addWidget(
-00007110: 7365 6c66 2e6c 6162 656c 5f36 2c20 3234  self.label_6, 24
-00007120: 2c20 302c 2031 2c20 3129 0a20 2020 2020  , 0, 1, 1).     
-00007130: 2020 2073 656c 662e 636d 625f 7361 6d70     self.cmb_samp
-00007140: 6c65 5479 7065 203d 2051 7457 6964 6765  leType = QtWidge
-00007150: 7473 2e51 436f 6d62 6f42 6f78 2873 656c  ts.QComboBox(sel
-00007160: 662e 7363 726f 6c6c 4172 6561 5769 6467  f.scrollAreaWidg
-00007170: 6574 436f 6e74 656e 7473 5f32 290a 2020  etContents_2).  
-00007180: 2020 2020 2020 7365 6c66 2e63 6d62 5f73        self.cmb_s
-00007190: 616d 706c 6554 7970 652e 7365 744f 626a  ampleType.setObj
-000071a0: 6563 744e 616d 6528 2263 6d62 5f73 616d  ectName("cmb_sam
-000071b0: 706c 6554 7970 6522 290a 2020 2020 2020  pleType").      
-000071c0: 2020 7365 6c66 2e63 6d62 5f73 616d 706c    self.cmb_sampl
-000071d0: 6554 7970 652e 6164 6449 7465 6d28 2222  eType.addItem(""
-000071e0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-000071f0: 6d62 5f73 616d 706c 6554 7970 652e 6164  mb_sampleType.ad
-00007200: 6449 7465 6d28 2222 290a 2020 2020 2020  dItem("").      
-00007210: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-00007220: 745f 322e 6164 6457 6964 6765 7428 7365  t_2.addWidget(se
-00007230: 6c66 2e63 6d62 5f73 616d 706c 6554 7970  lf.cmb_sampleTyp
-00007240: 652c 2032 342c 2032 2c20 312c 2031 290a  e, 24, 2, 1, 1).
-00007250: 2020 2020 2020 2020 7365 6c66 2e73 6372          self.scr
-00007260: 6f6c 6c41 7265 615f 322e 7365 7457 6964  ollArea_2.setWid
-00007270: 6765 7428 7365 6c66 2e73 6372 6f6c 6c41  get(self.scrollA
-00007280: 7265 6157 6964 6765 7443 6f6e 7465 6e74  reaWidgetContent
-00007290: 735f 3229 0a20 2020 2020 2020 2073 656c  s_2).        sel
-000072a0: 662e 6772 6964 4c61 796f 7574 5f39 2e61  f.gridLayout_9.a
-000072b0: 6464 5769 6467 6574 2873 656c 662e 7363  ddWidget(self.sc
-000072c0: 726f 6c6c 4172 6561 5f32 2c20 302c 2031  rollArea_2, 0, 1
-000072d0: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
-000072e0: 7365 6c66 2e74 6162 5769 6467 6574 2e61  self.tabWidget.a
-000072f0: 6464 5461 6228 7365 6c66 2e74 6162 2c20  ddTab(self.tab, 
-00007300: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
-00007310: 2e74 6162 5f32 203d 2051 7457 6964 6765  .tab_2 = QtWidge
-00007320: 7473 2e51 5769 6467 6574 2829 0a20 2020  ts.QWidget().   
-00007330: 2020 2020 2073 656c 662e 7461 625f 322e       self.tab_2.
-00007340: 7365 744f 626a 6563 744e 616d 6528 2274  setObjectName("t
-00007350: 6162 5f32 2229 0a20 2020 2020 2020 2073  ab_2").        s
-00007360: 656c 662e 686f 7269 7a6f 6e74 616c 4c61  elf.horizontalLa
-00007370: 796f 7574 203d 2051 7457 6964 6765 7473  yout = QtWidgets
-00007380: 2e51 4842 6f78 4c61 796f 7574 2873 656c  .QHBoxLayout(sel
-00007390: 662e 7461 625f 3229 0a20 2020 2020 2020  f.tab_2).       
-000073a0: 2073 656c 662e 686f 7269 7a6f 6e74 616c   self.horizontal
-000073b0: 4c61 796f 7574 2e73 6574 4f62 6a65 6374  Layout.setObject
-000073c0: 4e61 6d65 2822 686f 7269 7a6f 6e74 616c  Name("horizontal
-000073d0: 4c61 796f 7574 2229 0a20 2020 2020 2020  Layout").       
-000073e0: 2073 656c 662e 7363 726f 6c6c 4172 6561   self.scrollArea
-000073f0: 203d 2051 7457 6964 6765 7473 2e51 5363   = QtWidgets.QSc
-00007400: 726f 6c6c 4172 6561 2873 656c 662e 7461  rollArea(self.ta
-00007410: 625f 3229 0a20 2020 2020 2020 2073 656c  b_2).        sel
-00007420: 662e 7363 726f 6c6c 4172 6561 2e73 6574  f.scrollArea.set
-00007430: 4d69 6e69 6d75 6d53 697a 6528 5174 436f  MinimumSize(QtCo
-00007440: 7265 2e51 5369 7a65 2832 3430 2c20 3029  re.QSize(240, 0)
-00007450: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00007460: 6372 6f6c 6c41 7265 612e 7365 744d 6178  crollArea.setMax
-00007470: 696d 756d 5369 7a65 2851 7443 6f72 652e  imumSize(QtCore.
-00007480: 5153 697a 6528 3330 302c 2031 3637 3737  QSize(300, 16777
-00007490: 3231 3529 290a 2020 2020 2020 2020 7365  215)).        se
-000074a0: 6c66 2e73 6372 6f6c 6c41 7265 612e 7365  lf.scrollArea.se
-000074b0: 7457 6964 6765 7452 6573 697a 6162 6c65  tWidgetResizable
-000074c0: 2854 7275 6529 0a20 2020 2020 2020 2073  (True).        s
-000074d0: 656c 662e 7363 726f 6c6c 4172 6561 2e73  elf.scrollArea.s
-000074e0: 6574 4f62 6a65 6374 4e61 6d65 2822 7363  etObjectName("sc
-000074f0: 726f 6c6c 4172 6561 2229 0a20 2020 2020  rollArea").     
-00007500: 2020 2073 656c 662e 7363 726f 6c6c 4172     self.scrollAr
-00007510: 6561 5769 6467 6574 436f 6e74 656e 7473  eaWidgetContents
-00007520: 203d 2051 7457 6964 6765 7473 2e51 5769   = QtWidgets.QWi
-00007530: 6467 6574 2829 0a20 2020 2020 2020 2073  dget().        s
-00007540: 656c 662e 7363 726f 6c6c 4172 6561 5769  elf.scrollAreaWi
-00007550: 6467 6574 436f 6e74 656e 7473 2e73 6574  dgetContents.set
-00007560: 4765 6f6d 6574 7279 2851 7443 6f72 652e  Geometry(QtCore.
-00007570: 5152 6563 7428 302c 2030 2c20 3235 392c  QRect(0, 0, 259,
-00007580: 2038 3135 2929 0a20 2020 2020 2020 2073   815)).        s
-00007590: 656c 662e 7363 726f 6c6c 4172 6561 5769  elf.scrollAreaWi
-000075a0: 6467 6574 436f 6e74 656e 7473 2e73 6574  dgetContents.set
-000075b0: 4f62 6a65 6374 4e61 6d65 2822 7363 726f  ObjectName("scro
-000075c0: 6c6c 4172 6561 5769 6467 6574 436f 6e74  llAreaWidgetCont
-000075d0: 656e 7473 2229 0a20 2020 2020 2020 2073  ents").        s
-000075e0: 656c 662e 6772 6964 4c61 796f 7574 5f35  elf.gridLayout_5
-000075f0: 203d 2051 7457 6964 6765 7473 2e51 4772   = QtWidgets.QGr
-00007600: 6964 4c61 796f 7574 2873 656c 662e 7363  idLayout(self.sc
-00007610: 726f 6c6c 4172 6561 5769 6467 6574 436f  rollAreaWidgetCo
-00007620: 6e74 656e 7473 290a 2020 2020 2020 2020  ntents).        
-00007630: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
-00007640: 352e 7365 744f 626a 6563 744e 616d 6528  5.setObjectName(
-00007650: 2267 7269 644c 6179 6f75 745f 3522 290a  "gridLayout_5").
-00007660: 2020 2020 2020 2020 7365 6c66 2e74 6578          self.tex
-00007670: 7462 6f78 5f66 7073 5061 7468 203d 2051  tbox_fpsPath = Q
-00007680: 7457 6964 6765 7473 2e51 4c69 6e65 4564  tWidgets.QLineEd
-00007690: 6974 2873 656c 662e 7363 726f 6c6c 4172  it(self.scrollAr
-000076a0: 6561 5769 6467 6574 436f 6e74 656e 7473  eaWidgetContents
-000076b0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-000076c0: 6578 7462 6f78 5f66 7073 5061 7468 2e73  extbox_fpsPath.s
-000076d0: 6574 4f62 6a65 6374 4e61 6d65 2822 7465  etObjectName("te
-000076e0: 7874 626f 785f 6670 7350 6174 6822 290a  xtbox_fpsPath").
-000076f0: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
-00007700: 644c 6179 6f75 745f 352e 6164 6457 6964  dLayout_5.addWid
-00007710: 6765 7428 7365 6c66 2e74 6578 7462 6f78  get(self.textbox
-00007720: 5f66 7073 5061 7468 2c20 352c 2030 2c20  _fpsPath, 5, 0, 
-00007730: 312c 2033 290a 2020 2020 2020 2020 7365  1, 3).        se
-00007740: 6c66 2e6c 696e 655f 3420 3d20 5174 5769  lf.line_4 = QtWi
-00007750: 6467 6574 732e 5146 7261 6d65 2873 656c  dgets.QFrame(sel
-00007760: 662e 7363 726f 6c6c 4172 6561 5769 6467  f.scrollAreaWidg
-00007770: 6574 436f 6e74 656e 7473 290a 2020 2020  etContents).    
-00007780: 2020 2020 7365 6c66 2e6c 696e 655f 342e      self.line_4.
-00007790: 7365 7446 7261 6d65 5368 6170 6528 5174  setFrameShape(Qt
-000077a0: 5769 6467 6574 732e 5146 7261 6d65 2e48  Widgets.QFrame.H
-000077b0: 4c69 6e65 290a 2020 2020 2020 2020 7365  Line).        se
-000077c0: 6c66 2e6c 696e 655f 342e 7365 7446 7261  lf.line_4.setFra
-000077d0: 6d65 5368 6164 6f77 2851 7457 6964 6765  meShadow(QtWidge
-000077e0: 7473 2e51 4672 616d 652e 5375 6e6b 656e  ts.QFrame.Sunken
-000077f0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00007800: 696e 655f 342e 7365 744f 626a 6563 744e  ine_4.setObjectN
-00007810: 616d 6528 226c 696e 655f 3422 290a 2020  ame("line_4").  
-00007820: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
-00007830: 6179 6f75 745f 352e 6164 6457 6964 6765  ayout_5.addWidge
-00007840: 7428 7365 6c66 2e6c 696e 655f 342c 2031  t(self.line_4, 1
-00007850: 322c 2030 2c20 312c 2033 290a 2020 2020  2, 0, 1, 3).    
-00007860: 2020 2020 7365 6c66 2e74 6578 7462 6f78      self.textbox
-00007870: 5f70 6361 5361 7665 203d 2051 7457 6964  _pcaSave = QtWid
-00007880: 6765 7473 2e51 4c69 6e65 4564 6974 2873  gets.QLineEdit(s
-00007890: 656c 662e 7363 726f 6c6c 4172 6561 5769  elf.scrollAreaWi
-000078a0: 6467 6574 436f 6e74 656e 7473 290a 2020  dgetContents).  
-000078b0: 2020 2020 2020 7365 6c66 2e74 6578 7462        self.textb
-000078c0: 6f78 5f70 6361 5361 7665 2e73 6574 4f62  ox_pcaSave.setOb
-000078d0: 6a65 6374 4e61 6d65 2822 7465 7874 626f  jectName("textbo
-000078e0: 785f 7063 6153 6176 6522 290a 2020 2020  x_pcaSave").    
-000078f0: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-00007900: 6f75 745f 352e 6164 6457 6964 6765 7428  out_5.addWidget(
-00007910: 7365 6c66 2e74 6578 7462 6f78 5f70 6361  self.textbox_pca
-00007920: 5361 7665 2c20 372c 2030 2c20 312c 2033  Save, 7, 0, 1, 3
-00007930: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00007940: 6162 656c 5f31 3120 3d20 5174 5769 6467  abel_11 = QtWidg
-00007950: 6574 732e 514c 6162 656c 2873 656c 662e  ets.QLabel(self.
-00007960: 7363 726f 6c6c 4172 6561 5769 6467 6574  scrollAreaWidget
-00007970: 436f 6e74 656e 7473 290a 2020 2020 2020  Contents).      
-00007980: 2020 7365 6c66 2e6c 6162 656c 5f31 312e    self.label_11.
-00007990: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
-000079a0: 6162 656c 5f31 3122 290a 2020 2020 2020  abel_11").      
-000079b0: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-000079c0: 745f 352e 6164 6457 6964 6765 7428 7365  t_5.addWidget(se
-000079d0: 6c66 2e6c 6162 656c 5f31 312c 2032 2c20  lf.label_11, 2, 
-000079e0: 302c 2031 2c20 3129 0a20 2020 2020 2020  0, 1, 1).       
-000079f0: 2073 656c 662e 636d 625f 6d61 7472 6978   self.cmb_matrix
-00007a00: 5043 4120 3d20 5174 5769 6467 6574 732e  PCA = QtWidgets.
-00007a10: 5143 6f6d 626f 426f 7828 7365 6c66 2e73  QComboBox(self.s
-00007a20: 6372 6f6c 6c41 7265 6157 6964 6765 7443  crollAreaWidgetC
-00007a30: 6f6e 7465 6e74 7329 0a20 2020 2020 2020  ontents).       
-00007a40: 2073 656c 662e 636d 625f 6d61 7472 6978   self.cmb_matrix
-00007a50: 5043 412e 7365 744f 626a 6563 744e 616d  PCA.setObjectNam
-00007a60: 6528 2263 6d62 5f6d 6174 7269 7850 4341  e("cmb_matrixPCA
-00007a70: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00007a80: 636d 625f 6d61 7472 6978 5043 412e 6164  cmb_matrixPCA.ad
-00007a90: 6449 7465 6d28 2222 290a 2020 2020 2020  dItem("").      
-00007aa0: 2020 7365 6c66 2e63 6d62 5f6d 6174 7269    self.cmb_matri
-00007ab0: 7850 4341 2e61 6464 4974 656d 2822 2229  xPCA.addItem("")
-00007ac0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00007ad0: 6964 4c61 796f 7574 5f35 2e61 6464 5769  idLayout_5.addWi
-00007ae0: 6467 6574 2873 656c 662e 636d 625f 6d61  dget(self.cmb_ma
-00007af0: 7472 6978 5043 412c 2032 2c20 312c 2031  trixPCA, 2, 1, 1
-00007b00: 2c20 3229 0a20 2020 2020 2020 2073 656c  , 2).        sel
-00007b10: 662e 6c61 6265 6c5f 3134 203d 2051 7457  f.label_14 = QtW
-00007b20: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
-00007b30: 6c66 2e73 6372 6f6c 6c41 7265 6157 6964  lf.scrollAreaWid
-00007b40: 6765 7443 6f6e 7465 6e74 7329 0a20 2020  getContents).   
-00007b50: 2020 2020 2066 6f6e 7420 3d20 5174 4775       font = QtGu
-00007b60: 692e 5146 6f6e 7428 290a 2020 2020 2020  i.QFont().      
-00007b70: 2020 666f 6e74 2e73 6574 426f 6c64 2854    font.setBold(T
-00007b80: 7275 6529 0a20 2020 2020 2020 2066 6f6e  rue).        fon
-00007b90: 742e 7365 7455 6e64 6572 6c69 6e65 2854  t.setUnderline(T
-00007ba0: 7275 6529 0a20 2020 2020 2020 2066 6f6e  rue).        fon
-00007bb0: 742e 7365 7457 6569 6768 7428 3735 290a  t.setWeight(75).
-00007bc0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00007bd0: 656c 5f31 342e 7365 7446 6f6e 7428 666f  el_14.setFont(fo
-00007be0: 6e74 290a 2020 2020 2020 2020 7365 6c66  nt).        self
-00007bf0: 2e6c 6162 656c 5f31 342e 7365 744f 626a  .label_14.setObj
-00007c00: 6563 744e 616d 6528 226c 6162 656c 5f31  ectName("label_1
-00007c10: 3422 290a 2020 2020 2020 2020 7365 6c66  4").        self
-00007c20: 2e67 7269 644c 6179 6f75 745f 352e 6164  .gridLayout_5.ad
-00007c30: 6457 6964 6765 7428 7365 6c66 2e6c 6162  dWidget(self.lab
-00007c40: 656c 5f31 342c 2030 2c20 302c 2031 2c20  el_14, 0, 0, 1, 
-00007c50: 3329 0a20 2020 2020 2020 2073 656c 662e  3).        self.
-00007c60: 636d 625f 4650 5320 3d20 5174 5769 6467  cmb_FPS = QtWidg
-00007c70: 6574 732e 5143 6f6d 626f 426f 7828 7365  ets.QComboBox(se
-00007c80: 6c66 2e73 6372 6f6c 6c41 7265 6157 6964  lf.scrollAreaWid
-00007c90: 6765 7443 6f6e 7465 6e74 7329 0a20 2020  getContents).   
-00007ca0: 2020 2020 2073 656c 662e 636d 625f 4650       self.cmb_FP
-00007cb0: 532e 7365 744f 626a 6563 744e 616d 6528  S.setObjectName(
-00007cc0: 2263 6d62 5f46 5053 2229 0a20 2020 2020  "cmb_FPS").     
-00007cd0: 2020 2073 656c 662e 636d 625f 4650 532e     self.cmb_FPS.
-00007ce0: 6164 6449 7465 6d28 2222 290a 2020 2020  addItem("").    
-00007cf0: 2020 2020 7365 6c66 2e63 6d62 5f46 5053      self.cmb_FPS
-00007d00: 2e61 6464 4974 656d 2822 2229 0a20 2020  .addItem("").   
-00007d10: 2020 2020 2073 656c 662e 636d 625f 4650       self.cmb_FP
-00007d20: 532e 6164 6449 7465 6d28 2222 290a 2020  S.addItem("").  
-00007d30: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
-00007d40: 6179 6f75 745f 352e 6164 6457 6964 6765  ayout_5.addWidge
-00007d50: 7428 7365 6c66 2e63 6d62 5f46 5053 2c20  t(self.cmb_FPS, 
-00007d60: 312c 2030 2c20 312c 2033 290a 2020 2020  1, 0, 1, 3).    
-00007d70: 2020 2020 7365 6c66 2e6c 6162 656c 5f31      self.label_1
-00007d80: 3320 3d20 5174 5769 6467 6574 732e 514c  3 = QtWidgets.QL
-00007d90: 6162 656c 2873 656c 662e 7363 726f 6c6c  abel(self.scroll
-00007da0: 4172 6561 5769 6467 6574 436f 6e74 656e  AreaWidgetConten
-00007db0: 7473 290a 2020 2020 2020 2020 7365 6c66  ts).        self
-00007dc0: 2e6c 6162 656c 5f31 332e 7365 744f 626a  .label_13.setObj
-00007dd0: 6563 744e 616d 6528 226c 6162 656c 5f31  ectName("label_1
-00007de0: 3322 290a 2020 2020 2020 2020 7365 6c66  3").        self
-00007df0: 2e67 7269 644c 6179 6f75 745f 352e 6164  .gridLayout_5.ad
-00007e00: 6457 6964 6765 7428 7365 6c66 2e6c 6162  dWidget(self.lab
-00007e10: 656c 5f31 332c 2036 2c20 302c 2031 2c20  el_13, 6, 0, 1, 
-00007e20: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
-00007e30: 6c69 6e65 5f38 203d 2051 7457 6964 6765  line_8 = QtWidge
-00007e40: 7473 2e51 4672 616d 6528 7365 6c66 2e73  ts.QFrame(self.s
-00007e50: 6372 6f6c 6c41 7265 6157 6964 6765 7443  crollAreaWidgetC
-00007e60: 6f6e 7465 6e74 7329 0a20 2020 2020 2020  ontents).       
-00007e70: 2073 656c 662e 6c69 6e65 5f38 2e73 6574   self.line_8.set
-00007e80: 4672 616d 6553 6861 7065 2851 7457 6964  FrameShape(QtWid
-00007e90: 6765 7473 2e51 4672 616d 652e 484c 696e  gets.QFrame.HLin
-00007ea0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00007eb0: 6c69 6e65 5f38 2e73 6574 4672 616d 6553  line_8.setFrameS
-00007ec0: 6861 646f 7728 5174 5769 6467 6574 732e  hadow(QtWidgets.
-00007ed0: 5146 7261 6d65 2e53 756e 6b65 6e29 0a20  QFrame.Sunken). 
-00007ee0: 2020 2020 2020 2073 656c 662e 6c69 6e65         self.line
-00007ef0: 5f38 2e73 6574 4f62 6a65 6374 4e61 6d65  _8.setObjectName
-00007f00: 2822 6c69 6e65 5f38 2229 0a20 2020 2020  ("line_8").     
-00007f10: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-00007f20: 7574 5f35 2e61 6464 5769 6467 6574 2873  ut_5.addWidget(s
-00007f30: 656c 662e 6c69 6e65 5f38 2c20 382c 2030  elf.line_8, 8, 0
-00007f40: 2c20 312c 2033 290a 2020 2020 2020 2020  , 1, 3).        
-00007f50: 7365 6c66 2e6c 696e 655f 3720 3d20 5174  self.line_7 = Qt
-00007f60: 5769 6467 6574 732e 5146 7261 6d65 2873  Widgets.QFrame(s
-00007f70: 656c 662e 7363 726f 6c6c 4172 6561 5769  elf.scrollAreaWi
-00007f80: 6467 6574 436f 6e74 656e 7473 290a 2020  dgetContents).  
-00007f90: 2020 2020 2020 7365 6c66 2e6c 696e 655f        self.line_
-00007fa0: 372e 7365 7446 7261 6d65 5368 6170 6528  7.setFrameShape(
-00007fb0: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-00007fc0: 2e48 4c69 6e65 290a 2020 2020 2020 2020  .HLine).        
-00007fd0: 7365 6c66 2e6c 696e 655f 372e 7365 7446  self.line_7.setF
-00007fe0: 7261 6d65 5368 6164 6f77 2851 7457 6964  rameShadow(QtWid
-00007ff0: 6765 7473 2e51 4672 616d 652e 5375 6e6b  gets.QFrame.Sunk
-00008000: 656e 290a 2020 2020 2020 2020 7365 6c66  en).        self
-00008010: 2e6c 696e 655f 372e 7365 744f 626a 6563  .line_7.setObjec
-00008020: 744e 616d 6528 226c 696e 655f 3722 290a  tName("line_7").
-00008030: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
-00008040: 644c 6179 6f75 745f 352e 6164 6457 6964  dLayout_5.addWid
-00008050: 6765 7428 7365 6c66 2e6c 696e 655f 372c  get(self.line_7,
-00008060: 2033 2c20 302c 2031 2c20 3329 0a20 2020   3, 0, 1, 3).   
-00008070: 2020 2020 2073 656c 662e 6275 7474 6f6e       self.button
-00008080: 5f46 5053 7061 7468 203d 2051 7457 6964  _FPSpath = QtWid
-00008090: 6765 7473 2e51 5075 7368 4275 7474 6f6e  gets.QPushButton
-000080a0: 2873 656c 662e 7363 726f 6c6c 4172 6561  (self.scrollArea
-000080b0: 5769 6467 6574 436f 6e74 656e 7473 290a  WidgetContents).
-000080c0: 2020 2020 2020 2020 7365 6c66 2e62 7574          self.but
-000080d0: 746f 6e5f 4650 5370 6174 682e 7365 744f  ton_FPSpath.setO
-000080e0: 626a 6563 744e 616d 6528 2262 7574 746f  bjectName("butto
-000080f0: 6e5f 4650 5370 6174 6822 290a 2020 2020  n_FPSpath").    
-00008100: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-00008110: 6f75 745f 352e 6164 6457 6964 6765 7428  out_5.addWidget(
-00008120: 7365 6c66 2e62 7574 746f 6e5f 4650 5370  self.button_FPSp
-00008130: 6174 682c 2034 2c20 322c 2031 2c20 3129  ath, 4, 2, 1, 1)
-00008140: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00008150: 6265 6c5f 3132 203d 2051 7457 6964 6765  bel_12 = QtWidge
-00008160: 7473 2e51 4c61 6265 6c28 7365 6c66 2e73  ts.QLabel(self.s
-00008170: 6372 6f6c 6c41 7265 6157 6964 6765 7443  crollAreaWidgetC
-00008180: 6f6e 7465 6e74 7329 0a20 2020 2020 2020  ontents).       
-00008190: 2073 656c 662e 6c61 6265 6c5f 3132 2e73   self.label_12.s
-000081a0: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
-000081b0: 6265 6c5f 3132 2229 0a20 2020 2020 2020  bel_12").       
-000081c0: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
-000081d0: 5f35 2e61 6464 5769 6467 6574 2873 656c  _5.addWidget(sel
-000081e0: 662e 6c61 6265 6c5f 3132 2c20 342c 2030  f.label_12, 4, 0
-000081f0: 2c20 312c 2032 290a 2020 2020 2020 2020  , 1, 2).        
-00008200: 7365 6c66 2e62 7574 746f 6e5f 7361 7665  self.button_save
-00008210: 5043 4170 6174 6820 3d20 5174 5769 6467  PCApath = QtWidg
-00008220: 6574 732e 5150 7573 6842 7574 746f 6e28  ets.QPushButton(
-00008230: 7365 6c66 2e73 6372 6f6c 6c41 7265 6157  self.scrollAreaW
-00008240: 6964 6765 7443 6f6e 7465 6e74 7329 0a20  idgetContents). 
-00008250: 2020 2020 2020 2073 656c 662e 6275 7474         self.butt
-00008260: 6f6e 5f73 6176 6550 4341 7061 7468 2e73  on_savePCApath.s
-00008270: 6574 4f62 6a65 6374 4e61 6d65 2822 6275  etObjectName("bu
-00008280: 7474 6f6e 5f73 6176 6550 4341 7061 7468  tton_savePCApath
-00008290: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-000082a0: 6772 6964 4c61 796f 7574 5f35 2e61 6464  gridLayout_5.add
-000082b0: 5769 6467 6574 2873 656c 662e 6275 7474  Widget(self.butt
-000082c0: 6f6e 5f73 6176 6550 4341 7061 7468 2c20  on_savePCApath, 
-000082d0: 362c 2032 2c20 312c 2031 290a 2020 2020  6, 2, 1, 1).    
-000082e0: 2020 2020 7365 6c66 2e66 7261 6d65 5f67      self.frame_g
-000082f0: 7261 7068 203d 2051 7457 6964 6765 7473  raph = QtWidgets
-00008300: 2e51 4672 616d 6528 7365 6c66 2e73 6372  .QFrame(self.scr
-00008310: 6f6c 6c41 7265 6157 6964 6765 7443 6f6e  ollAreaWidgetCon
-00008320: 7465 6e74 7329 0a20 2020 2020 2020 2073  tents).        s
-00008330: 656c 662e 6672 616d 655f 6772 6170 682e  elf.frame_graph.
-00008340: 7365 7445 6e61 626c 6564 2846 616c 7365  setEnabled(False
-00008350: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
-00008360: 7261 6d65 5f67 7261 7068 2e73 6574 4672  rame_graph.setFr
-00008370: 616d 6553 6861 7065 2851 7457 6964 6765  ameShape(QtWidge
-00008380: 7473 2e51 4672 616d 652e 5374 796c 6564  ts.QFrame.Styled
-00008390: 5061 6e65 6c29 0a20 2020 2020 2020 2073  Panel).        s
-000083a0: 656c 662e 6672 616d 655f 6772 6170 682e  elf.frame_graph.
-000083b0: 7365 7446 7261 6d65 5368 6164 6f77 2851  setFrameShadow(Q
-000083c0: 7457 6964 6765 7473 2e51 4672 616d 652e  tWidgets.QFrame.
-000083d0: 5261 6973 6564 290a 2020 2020 2020 2020  Raised).        
-000083e0: 7365 6c66 2e66 7261 6d65 5f67 7261 7068  self.frame_graph
-000083f0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00008400: 6672 616d 655f 6772 6170 6822 290a 2020  frame_graph").  
-00008410: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
-00008420: 6179 6f75 745f 3620 3d20 5174 5769 6467  ayout_6 = QtWidg
-00008430: 6574 732e 5147 7269 644c 6179 6f75 7428  ets.QGridLayout(
-00008440: 7365 6c66 2e66 7261 6d65 5f67 7261 7068  self.frame_graph
-00008450: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-00008460: 7269 644c 6179 6f75 745f 362e 7365 744f  ridLayout_6.setO
-00008470: 626a 6563 744e 616d 6528 2267 7269 644c  bjectName("gridL
-00008480: 6179 6f75 745f 3622 290a 2020 2020 2020  ayout_6").      
-00008490: 2020 7365 6c66 2e6c 6162 656c 5f32 3820    self.label_28 
-000084a0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-000084b0: 656c 2873 656c 662e 6672 616d 655f 6772  el(self.frame_gr
-000084c0: 6170 6829 0a20 2020 2020 2020 2073 656c  aph).        sel
-000084d0: 662e 6c61 6265 6c5f 3238 2e73 6574 4f62  f.label_28.setOb
-000084e0: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
-000084f0: 3238 2229 0a20 2020 2020 2020 2073 656c  28").        sel
-00008500: 662e 6772 6964 4c61 796f 7574 5f36 2e61  f.gridLayout_6.a
-00008510: 6464 5769 6467 6574 2873 656c 662e 6c61  ddWidget(self.la
-00008520: 6265 6c5f 3238 2c20 3130 2c20 302c 2031  bel_28, 10, 0, 1
-00008530: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
-00008540: 662e 7075 7368 4275 7474 6f6e 5f32 203d  f.pushButton_2 =
-00008550: 2051 7457 6964 6765 7473 2e51 5075 7368   QtWidgets.QPush
-00008560: 4275 7474 6f6e 2873 656c 662e 6672 616d  Button(self.fram
-00008570: 655f 6772 6170 6829 0a20 2020 2020 2020  e_graph).       
-00008580: 2073 656c 662e 7075 7368 4275 7474 6f6e   self.pushButton
-00008590: 5f32 2e73 6574 4f62 6a65 6374 4e61 6d65  _2.setObjectName
-000085a0: 2822 7075 7368 4275 7474 6f6e 5f32 2229  ("pushButton_2")
-000085b0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-000085c0: 6964 4c61 796f 7574 5f36 2e61 6464 5769  idLayout_6.addWi
-000085d0: 6467 6574 2873 656c 662e 7075 7368 4275  dget(self.pushBu
-000085e0: 7474 6f6e 5f32 2c20 3135 2c20 302c 2031  tton_2, 15, 0, 1
-000085f0: 2c20 3229 0a20 2020 2020 2020 2073 656c  , 2).        sel
-00008600: 662e 6c61 6265 6c5f 3232 203d 2051 7457  f.label_22 = QtW
-00008610: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
-00008620: 6c66 2e66 7261 6d65 5f67 7261 7068 290a  lf.frame_graph).
-00008630: 2020 2020 2020 2020 666f 6e74 203d 2051          font = Q
-00008640: 7447 7569 2e51 466f 6e74 2829 0a20 2020  tGui.QFont().   
-00008650: 2020 2020 2066 6f6e 742e 7365 7442 6f6c       font.setBol
-00008660: 6428 5472 7565 290a 2020 2020 2020 2020  d(True).        
-00008670: 666f 6e74 2e73 6574 556e 6465 726c 696e  font.setUnderlin
-00008680: 6528 5472 7565 290a 2020 2020 2020 2020  e(True).        
-00008690: 666f 6e74 2e73 6574 5765 6967 6874 2837  font.setWeight(7
-000086a0: 3529 0a20 2020 2020 2020 2073 656c 662e  5).        self.
-000086b0: 6c61 6265 6c5f 3232 2e73 6574 466f 6e74  label_22.setFont
-000086c0: 2866 6f6e 7429 0a20 2020 2020 2020 2073  (font).        s
-000086d0: 656c 662e 6c61 6265 6c5f 3232 2e73 6574  elf.label_22.set
-000086e0: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
-000086f0: 6c5f 3232 2229 0a20 2020 2020 2020 2073  l_22").        s
-00008700: 656c 662e 6772 6964 4c61 796f 7574 5f36  elf.gridLayout_6
-00008710: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
-00008720: 6c61 6265 6c5f 3232 2c20 302c 2030 2c20  label_22, 0, 0, 
-00008730: 312c 2032 290a 2020 2020 2020 2020 7365  1, 2).        se
-00008740: 6c66 2e63 6d62 5f78 203d 2051 7457 6964  lf.cmb_x = QtWid
-00008750: 6765 7473 2e51 436f 6d62 6f42 6f78 2873  gets.QComboBox(s
-00008760: 656c 662e 6672 616d 655f 6772 6170 6829  elf.frame_graph)
-00008770: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
-00008780: 625f 782e 7365 744f 626a 6563 744e 616d  b_x.setObjectNam
-00008790: 6528 2263 6d62 5f78 2229 0a20 2020 2020  e("cmb_x").     
-000087a0: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-000087b0: 7574 5f36 2e61 6464 5769 6467 6574 2873  ut_6.addWidget(s
-000087c0: 656c 662e 636d 625f 782c 2032 2c20 312c  elf.cmb_x, 2, 1,
-000087d0: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
-000087e0: 656c 662e 6473 625f 6d61 726b 6572 5369  elf.dsb_markerSi
-000087f0: 7a65 203d 2051 7457 6964 6765 7473 2e51  ze = QtWidgets.Q
-00008800: 446f 7562 6c65 5370 696e 426f 7828 7365  DoubleSpinBox(se
-00008810: 6c66 2e66 7261 6d65 5f67 7261 7068 290a  lf.frame_graph).
-00008820: 2020 2020 2020 2020 7365 6c66 2e64 7362          self.dsb
-00008830: 5f6d 6172 6b65 7253 697a 652e 7365 744d  _markerSize.setM
-00008840: 696e 696d 756d 2830 2e31 290a 2020 2020  inimum(0.1).    
-00008850: 2020 2020 7365 6c66 2e64 7362 5f6d 6172      self.dsb_mar
-00008860: 6b65 7253 697a 652e 7365 744d 6178 696d  kerSize.setMaxim
-00008870: 756d 2833 302e 3029 0a20 2020 2020 2020  um(30.0).       
-00008880: 2073 656c 662e 6473 625f 6d61 726b 6572   self.dsb_marker
-00008890: 5369 7a65 2e73 6574 5369 6e67 6c65 5374  Size.setSingleSt
-000088a0: 6570 2830 2e31 290a 2020 2020 2020 2020  ep(0.1).        
-000088b0: 7365 6c66 2e64 7362 5f6d 6172 6b65 7253  self.dsb_markerS
-000088c0: 697a 652e 7365 7450 726f 7065 7274 7928  ize.setProperty(
-000088d0: 2276 616c 7565 222c 2035 2e30 290a 2020  "value", 5.0).  
-000088e0: 2020 2020 2020 7365 6c66 2e64 7362 5f6d        self.dsb_m
-000088f0: 6172 6b65 7253 697a 652e 7365 744f 626a  arkerSize.setObj
-00008900: 6563 744e 616d 6528 2264 7362 5f6d 6172  ectName("dsb_mar
-00008910: 6b65 7253 697a 6522 290a 2020 2020 2020  kerSize").      
-00008920: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-00008930: 745f 362e 6164 6457 6964 6765 7428 7365  t_6.addWidget(se
-00008940: 6c66 2e64 7362 5f6d 6172 6b65 7253 697a  lf.dsb_markerSiz
-00008950: 652c 2035 2c20 312c 2031 2c20 3129 0a20  e, 5, 1, 1, 1). 
-00008960: 2020 2020 2020 2073 656c 662e 636d 625f         self.cmb_
-00008970: 736f 7274 203d 2051 7457 6964 6765 7473  sort = QtWidgets
-00008980: 2e51 436f 6d62 6f42 6f78 2873 656c 662e  .QComboBox(self.
-00008990: 6672 616d 655f 6772 6170 6829 0a20 2020  frame_graph).   
-000089a0: 2020 2020 2073 656c 662e 636d 625f 736f       self.cmb_so
-000089b0: 7274 2e73 6574 4f62 6a65 6374 4e61 6d65  rt.setObjectName
-000089c0: 2822 636d 625f 736f 7274 2229 0a20 2020  ("cmb_sort").   
-000089d0: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
-000089e0: 796f 7574 5f36 2e61 6464 5769 6467 6574  yout_6.addWidget
-000089f0: 2873 656c 662e 636d 625f 736f 7274 2c20  (self.cmb_sort, 
-00008a00: 392c 2031 2c20 312c 2031 290a 2020 2020  9, 1, 1, 1).    
-00008a10: 2020 2020 7365 6c66 2e70 7573 6842 7574      self.pushBut
-00008a20: 746f 6e20 3d20 5174 5769 6467 6574 732e  ton = QtWidgets.
-00008a30: 5150 7573 6842 7574 746f 6e28 7365 6c66  QPushButton(self
-00008a40: 2e66 7261 6d65 5f67 7261 7068 290a 2020  .frame_graph).  
-00008a50: 2020 2020 2020 7365 6c66 2e70 7573 6842        self.pushB
-00008a60: 7574 746f 6e2e 7365 744f 626a 6563 744e  utton.setObjectN
-00008a70: 616d 6528 2270 7573 6842 7574 746f 6e22  ame("pushButton"
-00008a80: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-00008a90: 7269 644c 6179 6f75 745f 362e 6164 6457  ridLayout_6.addW
-00008aa0: 6964 6765 7428 7365 6c66 2e70 7573 6842  idget(self.pushB
-00008ab0: 7574 746f 6e2c 2031 342c 2031 2c20 312c  utton, 14, 1, 1,
-00008ac0: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
-00008ad0: 2e6c 6162 656c 5f32 3020 3d20 5174 5769  .label_20 = QtWi
-00008ae0: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-00008af0: 662e 6672 616d 655f 6772 6170 6829 0a20  f.frame_graph). 
-00008b00: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00008b10: 6c5f 3230 2e73 6574 4f62 6a65 6374 4e61  l_20.setObjectNa
-00008b20: 6d65 2822 6c61 6265 6c5f 3230 2229 0a20  me("label_20"). 
-00008b30: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-00008b40: 4c61 796f 7574 5f36 2e61 6464 5769 6467  Layout_6.addWidg
-00008b50: 6574 2873 656c 662e 6c61 6265 6c5f 3230  et(self.label_20
-00008b60: 2c20 382c 2030 2c20 312c 2031 290a 2020  , 8, 0, 1, 1).  
-00008b70: 2020 2020 2020 7365 6c66 2e63 6d62 5f63        self.cmb_c
-00008b80: 6f6c 6f72 203d 2051 7457 6964 6765 7473  olor = QtWidgets
-00008b90: 2e51 436f 6d62 6f42 6f78 2873 656c 662e  .QComboBox(self.
-00008ba0: 6672 616d 655f 6772 6170 6829 0a20 2020  frame_graph).   
-00008bb0: 2020 2020 2073 656c 662e 636d 625f 636f       self.cmb_co
-00008bc0: 6c6f 722e 7365 744f 626a 6563 744e 616d  lor.setObjectNam
-00008bd0: 6528 2263 6d62 5f63 6f6c 6f72 2229 0a20  e("cmb_color"). 
-00008be0: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-00008bf0: 4c61 796f 7574 5f36 2e61 6464 5769 6467  Layout_6.addWidg
-00008c00: 6574 2873 656c 662e 636d 625f 636f 6c6f  et(self.cmb_colo
-00008c10: 722c 2038 2c20 312c 2031 2c20 3129 0a20  r, 8, 1, 1, 1). 
-00008c20: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00008c30: 6c5f 3138 203d 2051 7457 6964 6765 7473  l_18 = QtWidgets
-00008c40: 2e51 4c61 6265 6c28 7365 6c66 2e66 7261  .QLabel(self.fra
-00008c50: 6d65 5f67 7261 7068 290a 2020 2020 2020  me_graph).      
-00008c60: 2020 7365 6c66 2e6c 6162 656c 5f31 382e    self.label_18.
-00008c70: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
-00008c80: 6162 656c 5f31 3822 290a 2020 2020 2020  abel_18").      
-00008c90: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-00008ca0: 745f 362e 6164 6457 6964 6765 7428 7365  t_6.addWidget(se
-00008cb0: 6c66 2e6c 6162 656c 5f31 382c 2032 2c20  lf.label_18, 2, 
-00008cc0: 302c 2031 2c20 3129 0a20 2020 2020 2020  0, 1, 1).       
-00008cd0: 2073 656c 662e 636d 625f 7920 3d20 5174   self.cmb_y = Qt
-00008ce0: 5769 6467 6574 732e 5143 6f6d 626f 426f  Widgets.QComboBo
-00008cf0: 7828 7365 6c66 2e66 7261 6d65 5f67 7261  x(self.frame_gra
-00008d00: 7068 290a 2020 2020 2020 2020 7365 6c66  ph).        self
-00008d10: 2e63 6d62 5f79 2e73 6574 4f62 6a65 6374  .cmb_y.setObject
-00008d20: 4e61 6d65 2822 636d 625f 7922 290a 2020  Name("cmb_y").  
-00008d30: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
-00008d40: 6179 6f75 745f 362e 6164 6457 6964 6765  ayout_6.addWidge
-00008d50: 7428 7365 6c66 2e63 6d62 5f79 2c20 342c  t(self.cmb_y, 4,
-00008d60: 2031 2c20 312c 2031 290a 2020 2020 2020   1, 1, 1).      
-00008d70: 2020 7365 6c66 2e6c 6162 656c 5f32 3420    self.label_24 
-00008d80: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-00008d90: 656c 2873 656c 662e 6672 616d 655f 6772  el(self.frame_gr
-00008da0: 6170 6829 0a20 2020 2020 2020 2073 656c  aph).        sel
-00008db0: 662e 6c61 6265 6c5f 3234 2e73 6574 4f62  f.label_24.setOb
-00008dc0: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
-00008dd0: 3234 2229 0a20 2020 2020 2020 2073 656c  24").        sel
-00008de0: 662e 6772 6964 4c61 796f 7574 5f36 2e61  f.gridLayout_6.a
-00008df0: 6464 5769 6467 6574 2873 656c 662e 6c61  ddWidget(self.la
-00008e00: 6265 6c5f 3234 2c20 312c 2030 2c20 312c  bel_24, 1, 0, 1,
-00008e10: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
-00008e20: 2e6c 6162 656c 5f32 3120 3d20 5174 5769  .label_21 = QtWi
-00008e30: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-00008e40: 662e 6672 616d 655f 6772 6170 6829 0a20  f.frame_graph). 
-00008e50: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00008e60: 6c5f 3231 2e73 6574 4f62 6a65 6374 4e61  l_21.setObjectNa
-00008e70: 6d65 2822 6c61 6265 6c5f 3231 2229 0a20  me("label_21"). 
-00008e80: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-00008e90: 4c61 796f 7574 5f36 2e61 6464 5769 6467  Layout_6.addWidg
-00008ea0: 6574 2873 656c 662e 6c61 6265 6c5f 3231  et(self.label_21
-00008eb0: 2c20 352c 2030 2c20 312c 2031 290a 2020  , 5, 0, 1, 1).  
-00008ec0: 2020 2020 2020 7365 6c66 2e63 6d62 5f70        self.cmb_p
-00008ed0: 6c6f 7420 3d20 5174 5769 6467 6574 732e  lot = QtWidgets.
-00008ee0: 5143 6f6d 626f 426f 7828 7365 6c66 2e66  QComboBox(self.f
-00008ef0: 7261 6d65 5f67 7261 7068 290a 2020 2020  rame_graph).    
-00008f00: 2020 2020 7365 6c66 2e63 6d62 5f70 6c6f      self.cmb_plo
-00008f10: 742e 7365 744f 626a 6563 744e 616d 6528  t.setObjectName(
-00008f20: 2263 6d62 5f70 6c6f 7422 290a 2020 2020  "cmb_plot").    
-00008f30: 2020 2020 7365 6c66 2e63 6d62 5f70 6c6f      self.cmb_plo
-00008f40: 742e 6164 6449 7465 6d28 2222 290a 2020  t.addItem("").  
-00008f50: 2020 2020 2020 7365 6c66 2e63 6d62 5f70        self.cmb_p
-00008f60: 6c6f 742e 6164 6449 7465 6d28 2222 290a  lot.addItem("").
-00008f70: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
-00008f80: 5f70 6c6f 742e 6164 6449 7465 6d28 2222  _plot.addItem(""
-00008f90: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-00008fa0: 7269 644c 6179 6f75 745f 362e 6164 6457  ridLayout_6.addW
-00008fb0: 6964 6765 7428 7365 6c66 2e63 6d62 5f70  idget(self.cmb_p
-00008fc0: 6c6f 742c 2031 2c20 312c 2031 2c20 3129  lot, 1, 1, 1, 1)
-00008fd0: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
-00008fe0: 625f 7375 6273 7562 636f 6c6f 7220 3d20  b_subsubcolor = 
-00008ff0: 5174 5769 6467 6574 732e 5143 6f6d 626f  QtWidgets.QCombo
-00009000: 426f 7828 7365 6c66 2e66 7261 6d65 5f67  Box(self.frame_g
-00009010: 7261 7068 290a 2020 2020 2020 2020 7365  raph).        se
-00009020: 6c66 2e63 6d62 5f73 7562 7375 6263 6f6c  lf.cmb_subsubcol
-00009030: 6f72 2e73 6574 4f62 6a65 6374 4e61 6d65  or.setObjectName
-00009040: 2822 636d 625f 7375 6273 7562 636f 6c6f  ("cmb_subsubcolo
-00009050: 7222 290a 2020 2020 2020 2020 7365 6c66  r").        self
-00009060: 2e67 7269 644c 6179 6f75 745f 362e 6164  .gridLayout_6.ad
-00009070: 6457 6964 6765 7428 7365 6c66 2e63 6d62  dWidget(self.cmb
-00009080: 5f73 7562 7375 6263 6f6c 6f72 2c20 3132  _subsubcolor, 12
-00009090: 2c20 312c 2031 2c20 3129 0a20 2020 2020  , 1, 1, 1).     
-000090a0: 2020 2073 656c 662e 636d 625f 7375 6263     self.cmb_subc
-000090b0: 6f6c 6f72 203d 2051 7457 6964 6765 7473  olor = QtWidgets
-000090c0: 2e51 436f 6d62 6f42 6f78 2873 656c 662e  .QComboBox(self.
-000090d0: 6672 616d 655f 6772 6170 6829 0a20 2020  frame_graph).   
-000090e0: 2020 2020 2073 656c 662e 636d 625f 7375       self.cmb_su
-000090f0: 6263 6f6c 6f72 2e73 6574 4f62 6a65 6374  bcolor.setObject
-00009100: 4e61 6d65 2822 636d 625f 7375 6263 6f6c  Name("cmb_subcol
-00009110: 6f72 2229 0a20 2020 2020 2020 2073 656c  or").        sel
-00009120: 662e 6772 6964 4c61 796f 7574 5f36 2e61  f.gridLayout_6.a
-00009130: 6464 5769 6467 6574 2873 656c 662e 636d  ddWidget(self.cm
-00009140: 625f 7375 6263 6f6c 6f72 2c20 3130 2c20  b_subcolor, 10, 
-00009150: 312c 2031 2c20 3129 0a20 2020 2020 2020  1, 1, 1).       
-00009160: 2073 656c 662e 636d 625f 7375 6273 6f72   self.cmb_subsor
-00009170: 7420 3d20 5174 5769 6467 6574 732e 5143  t = QtWidgets.QC
-00009180: 6f6d 626f 426f 7828 7365 6c66 2e66 7261  omboBox(self.fra
-00009190: 6d65 5f67 7261 7068 290a 2020 2020 2020  me_graph).      
-000091a0: 2020 7365 6c66 2e63 6d62 5f73 7562 736f    self.cmb_subso
-000091b0: 7274 2e73 6574 4f62 6a65 6374 4e61 6d65  rt.setObjectName
-000091c0: 2822 636d 625f 7375 6273 6f72 7422 290a  ("cmb_subsort").
-000091d0: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
-000091e0: 644c 6179 6f75 745f 362e 6164 6457 6964  dLayout_6.addWid
-000091f0: 6765 7428 7365 6c66 2e63 6d62 5f73 7562  get(self.cmb_sub
-00009200: 736f 7274 2c20 3131 2c20 312c 2031 2c20  sort, 11, 1, 1, 
-00009210: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-00009220: 636d 625f 7375 6273 7562 736f 7274 203d  cmb_subsubsort =
-00009230: 2051 7457 6964 6765 7473 2e51 436f 6d62   QtWidgets.QComb
-00009240: 6f42 6f78 2873 656c 662e 6672 616d 655f  oBox(self.frame_
-00009250: 6772 6170 6829 0a20 2020 2020 2020 2073  graph).        s
-00009260: 656c 662e 636d 625f 7375 6273 7562 736f  elf.cmb_subsubso
-00009270: 7274 2e73 6574 4f62 6a65 6374 4e61 6d65  rt.setObjectName
-00009280: 2822 636d 625f 7375 6273 7562 736f 7274  ("cmb_subsubsort
-00009290: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-000092a0: 6772 6964 4c61 796f 7574 5f36 2e61 6464  gridLayout_6.add
-000092b0: 5769 6467 6574 2873 656c 662e 636d 625f  Widget(self.cmb_
-000092c0: 7375 6273 7562 736f 7274 2c20 3133 2c20  subsubsort, 13, 
-000092d0: 312c 2031 2c20 3129 0a20 2020 2020 2020  1, 1, 1).       
-000092e0: 2073 656c 662e 6c61 6265 6c5f 3239 203d   self.label_29 =
-000092f0: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
-00009300: 6c28 7365 6c66 2e66 7261 6d65 5f67 7261  l(self.frame_gra
-00009310: 7068 290a 2020 2020 2020 2020 7365 6c66  ph).        self
-00009320: 2e6c 6162 656c 5f32 392e 7365 744f 626a  .label_29.setObj
-00009330: 6563 744e 616d 6528 226c 6162 656c 5f32  ectName("label_2
-00009340: 3922 290a 2020 2020 2020 2020 7365 6c66  9").        self
-00009350: 2e67 7269 644c 6179 6f75 745f 362e 6164  .gridLayout_6.ad
-00009360: 6457 6964 6765 7428 7365 6c66 2e6c 6162  dWidget(self.lab
-00009370: 656c 5f32 392c 2031 322c 2030 2c20 312c  el_29, 12, 0, 1,
-00009380: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
-00009390: 2e6c 6162 656c 5f31 3920 3d20 5174 5769  .label_19 = QtWi
-000093a0: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-000093b0: 662e 6672 616d 655f 6772 6170 6829 0a20  f.frame_graph). 
-000093c0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-000093d0: 6c5f 3139 2e73 6574 4f62 6a65 6374 4e61  l_19.setObjectNa
-000093e0: 6d65 2822 6c61 6265 6c5f 3139 2229 0a20  me("label_19"). 
-000093f0: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-00009400: 4c61 796f 7574 5f36 2e61 6464 5769 6467  Layout_6.addWidg
-00009410: 6574 2873 656c 662e 6c61 6265 6c5f 3139  et(self.label_19
-00009420: 2c20 342c 2030 2c20 312c 2031 290a 2020  , 4, 0, 1, 1).  
-00009430: 2020 2020 2020 7365 6c66 2e73 7062 5f62        self.spb_b
-00009440: 696e 7320 3d20 5174 5769 6467 6574 732e  ins = QtWidgets.
-00009450: 5153 7069 6e42 6f78 2873 656c 662e 6672  QSpinBox(self.fr
-00009460: 616d 655f 6772 6170 6829 0a20 2020 2020  ame_graph).     
-00009470: 2020 2073 656c 662e 7370 625f 6269 6e73     self.spb_bins
-00009480: 2e73 6574 4d69 6e69 6d75 6d28 3129 0a20  .setMinimum(1). 
-00009490: 2020 2020 2020 2073 656c 662e 7370 625f         self.spb_
-000094a0: 6269 6e73 2e73 6574 4d61 7869 6d75 6d28  bins.setMaximum(
-000094b0: 3230 3029 0a20 2020 2020 2020 2073 656c  200).        sel
-000094c0: 662e 7370 625f 6269 6e73 2e73 6574 5072  f.spb_bins.setPr
-000094d0: 6f70 6572 7479 2822 7661 6c75 6522 2c20  operty("value", 
-000094e0: 3130 290a 2020 2020 2020 2020 7365 6c66  10).        self
-000094f0: 2e73 7062 5f62 696e 732e 7365 744f 626a  .spb_bins.setObj
-00009500: 6563 744e 616d 6528 2273 7062 5f62 696e  ectName("spb_bin
-00009510: 7322 290a 2020 2020 2020 2020 7365 6c66  s").        self
-00009520: 2e67 7269 644c 6179 6f75 745f 362e 6164  .gridLayout_6.ad
-00009530: 6457 6964 6765 7428 7365 6c66 2e73 7062  dWidget(self.spb
-00009540: 5f62 696e 732c 2036 2c20 312c 2031 2c20  _bins, 6, 1, 1, 
-00009550: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-00009560: 6c61 6265 6c5f 6269 6e73 203d 2051 7457  label_bins = QtW
-00009570: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
-00009580: 6c66 2e66 7261 6d65 5f67 7261 7068 290a  lf.frame_graph).
-00009590: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-000095a0: 656c 5f62 696e 732e 7365 744f 626a 6563  el_bins.setObjec
-000095b0: 744e 616d 6528 226c 6162 656c 5f62 696e  tName("label_bin
-000095c0: 7322 290a 2020 2020 2020 2020 7365 6c66  s").        self
-000095d0: 2e67 7269 644c 6179 6f75 745f 362e 6164  .gridLayout_6.ad
-000095e0: 6457 6964 6765 7428 7365 6c66 2e6c 6162  dWidget(self.lab
-000095f0: 656c 5f62 696e 732c 2036 2c20 302c 2031  el_bins, 6, 0, 1
-00009600: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
-00009610: 662e 6473 625f 616c 7068 6120 3d20 5174  f.dsb_alpha = Qt
-00009620: 5769 6467 6574 732e 5144 6f75 626c 6553  Widgets.QDoubleS
-00009630: 7069 6e42 6f78 2873 656c 662e 6672 616d  pinBox(self.fram
-00009640: 655f 6772 6170 6829 0a20 2020 2020 2020  e_graph).       
-00009650: 2073 656c 662e 6473 625f 616c 7068 612e   self.dsb_alpha.
-00009660: 7365 7444 6563 696d 616c 7328 3129 0a20  setDecimals(1). 
-00009670: 2020 2020 2020 2073 656c 662e 6473 625f         self.dsb_
-00009680: 616c 7068 612e 7365 744d 696e 696d 756d  alpha.setMinimum
-00009690: 2830 2e31 290a 2020 2020 2020 2020 7365  (0.1).        se
-000096a0: 6c66 2e64 7362 5f61 6c70 6861 2e73 6574  lf.dsb_alpha.set
-000096b0: 4d61 7869 6d75 6d28 312e 3029 0a20 2020  Maximum(1.0).   
-000096c0: 2020 2020 2073 656c 662e 6473 625f 616c       self.dsb_al
-000096d0: 7068 612e 7365 7453 696e 676c 6553 7465  pha.setSingleSte
-000096e0: 7028 302e 3129 0a20 2020 2020 2020 2073  p(0.1).        s
-000096f0: 656c 662e 6473 625f 616c 7068 612e 7365  elf.dsb_alpha.se
-00009700: 7450 726f 7065 7274 7928 2276 616c 7565  tProperty("value
-00009710: 222c 2031 2e30 290a 2020 2020 2020 2020  ", 1.0).        
-00009720: 7365 6c66 2e64 7362 5f61 6c70 6861 2e73  self.dsb_alpha.s
-00009730: 6574 4f62 6a65 6374 4e61 6d65 2822 6473  etObjectName("ds
-00009740: 625f 616c 7068 6122 290a 2020 2020 2020  b_alpha").      
-00009750: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-00009760: 745f 362e 6164 6457 6964 6765 7428 7365  t_6.addWidget(se
-00009770: 6c66 2e64 7362 5f61 6c70 6861 2c20 372c  lf.dsb_alpha, 7,
-00009780: 2031 2c20 312c 2031 290a 2020 2020 2020   1, 1, 1).      
-00009790: 2020 7365 6c66 2e6c 6162 656c 5f33 3020    self.label_30 
-000097a0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-000097b0: 656c 2873 656c 662e 6672 616d 655f 6772  el(self.frame_gr
-000097c0: 6170 6829 0a20 2020 2020 2020 2073 656c  aph).        sel
-000097d0: 662e 6c61 6265 6c5f 3330 2e73 6574 4f62  f.label_30.setOb
-000097e0: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
-000097f0: 3330 2229 0a20 2020 2020 2020 2073 656c  30").        sel
-00009800: 662e 6772 6964 4c61 796f 7574 5f36 2e61  f.gridLayout_6.a
-00009810: 6464 5769 6467 6574 2873 656c 662e 6c61  ddWidget(self.la
-00009820: 6265 6c5f 3330 2c20 372c 2030 2c20 312c  bel_30, 7, 0, 1,
-00009830: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
-00009840: 2e67 7269 644c 6179 6f75 745f 352e 6164  .gridLayout_5.ad
-00009850: 6457 6964 6765 7428 7365 6c66 2e66 7261  dWidget(self.fra
-00009860: 6d65 5f67 7261 7068 2c20 3133 2c20 302c  me_graph, 13, 0,
-00009870: 2031 2c20 3329 0a20 2020 2020 2020 2073   1, 3).        s
-00009880: 656c 662e 6275 7474 6f6e 5f50 4341 203d  elf.button_PCA =
-00009890: 2051 7457 6964 6765 7473 2e51 5075 7368   QtWidgets.QPush
-000098a0: 4275 7474 6f6e 2873 656c 662e 7363 726f  Button(self.scro
-000098b0: 6c6c 4172 6561 5769 6467 6574 436f 6e74  llAreaWidgetCont
-000098c0: 656e 7473 290a 2020 2020 2020 2020 7365  ents).        se
-000098d0: 6c66 2e62 7574 746f 6e5f 5043 412e 7365  lf.button_PCA.se
-000098e0: 744f 626a 6563 744e 616d 6528 2262 7574  tObjectName("but
-000098f0: 746f 6e5f 5043 4122 290a 2020 2020 2020  ton_PCA").      
-00009900: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-00009910: 745f 352e 6164 6457 6964 6765 7428 7365  t_5.addWidget(se
-00009920: 6c66 2e62 7574 746f 6e5f 5043 412c 2039  lf.button_PCA, 9
-00009930: 2c20 302c 2031 2c20 3329 0a20 2020 2020  , 0, 1, 3).     
-00009940: 2020 2073 656c 662e 6c61 6265 6c5f 3134     self.label_14
-00009950: 2e72 6169 7365 5f28 290a 2020 2020 2020  .raise_().      
-00009960: 2020 7365 6c66 2e6c 696e 655f 372e 7261    self.line_7.ra
-00009970: 6973 655f 2829 0a20 2020 2020 2020 2073  ise_().        s
-00009980: 656c 662e 6c61 6265 6c5f 3132 2e72 6169  elf.label_12.rai
-00009990: 7365 5f28 290a 2020 2020 2020 2020 7365  se_().        se
-000099a0: 6c66 2e62 7574 746f 6e5f 4650 5370 6174  lf.button_FPSpat
-000099b0: 682e 7261 6973 655f 2829 0a20 2020 2020  h.raise_().     
-000099c0: 2020 2073 656c 662e 7465 7874 626f 785f     self.textbox_
-000099d0: 6670 7350 6174 682e 7261 6973 655f 2829  fpsPath.raise_()
-000099e0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-000099f0: 6265 6c5f 3133 2e72 6169 7365 5f28 290a  bel_13.raise_().
-00009a00: 2020 2020 2020 2020 7365 6c66 2e62 7574          self.but
-00009a10: 746f 6e5f 7361 7665 5043 4170 6174 682e  ton_savePCApath.
-00009a20: 7261 6973 655f 2829 0a20 2020 2020 2020  raise_().       
-00009a30: 2073 656c 662e 7465 7874 626f 785f 7063   self.textbox_pc
-00009a40: 6153 6176 652e 7261 6973 655f 2829 0a20  aSave.raise_(). 
-00009a50: 2020 2020 2020 2073 656c 662e 6c69 6e65         self.line
-00009a60: 5f38 2e72 6169 7365 5f28 290a 2020 2020  _8.raise_().    
-00009a70: 2020 2020 7365 6c66 2e6c 696e 655f 342e      self.line_4.
-00009a80: 7261 6973 655f 2829 0a20 2020 2020 2020  raise_().       
-00009a90: 2073 656c 662e 6672 616d 655f 6772 6170   self.frame_grap
-00009aa0: 682e 7261 6973 655f 2829 0a20 2020 2020  h.raise_().     
-00009ab0: 2020 2073 656c 662e 636d 625f 4650 532e     self.cmb_FPS.
-00009ac0: 7261 6973 655f 2829 0a20 2020 2020 2020  raise_().       
-00009ad0: 2073 656c 662e 6c61 6265 6c5f 3131 2e72   self.label_11.r
-00009ae0: 6169 7365 5f28 290a 2020 2020 2020 2020  aise_().        
-00009af0: 7365 6c66 2e63 6d62 5f6d 6174 7269 7850  self.cmb_matrixP
-00009b00: 4341 2e72 6169 7365 5f28 290a 2020 2020  CA.raise_().    
-00009b10: 2020 2020 7365 6c66 2e62 7574 746f 6e5f      self.button_
-00009b20: 5043 412e 7261 6973 655f 2829 0a20 2020  PCA.raise_().   
-00009b30: 2020 2020 2073 656c 662e 7363 726f 6c6c       self.scroll
-00009b40: 4172 6561 2e73 6574 5769 6467 6574 2873  Area.setWidget(s
-00009b50: 656c 662e 7363 726f 6c6c 4172 6561 5769  elf.scrollAreaWi
-00009b60: 6467 6574 436f 6e74 656e 7473 290a 2020  dgetContents).  
-00009b70: 2020 2020 2020 7365 6c66 2e68 6f72 697a        self.horiz
-00009b80: 6f6e 7461 6c4c 6179 6f75 742e 6164 6457  ontalLayout.addW
-00009b90: 6964 6765 7428 7365 6c66 2e73 6372 6f6c  idget(self.scrol
-00009ba0: 6c41 7265 6129 0a20 2020 2020 2020 2073  lArea).        s
-00009bb0: 656c 662e 7461 625f 7063 6120 3d20 5174  elf.tab_pca = Qt
-00009bc0: 5769 6467 6574 732e 5154 6162 5769 6467  Widgets.QTabWidg
-00009bd0: 6574 2873 656c 662e 7461 625f 3229 0a20  et(self.tab_2). 
-00009be0: 2020 2020 2020 2073 656c 662e 7461 625f         self.tab_
-00009bf0: 7063 612e 7365 7454 6162 506f 7369 7469  pca.setTabPositi
-00009c00: 6f6e 2851 7457 6964 6765 7473 2e51 5461  on(QtWidgets.QTa
-00009c10: 6257 6964 6765 742e 4e6f 7274 6829 0a20  bWidget.North). 
-00009c20: 2020 2020 2020 2073 656c 662e 7461 625f         self.tab_
-00009c30: 7063 612e 7365 7454 6162 5368 6170 6528  pca.setTabShape(
-00009c40: 5174 5769 6467 6574 732e 5154 6162 5769  QtWidgets.QTabWi
-00009c50: 6467 6574 2e52 6f75 6e64 6564 290a 2020  dget.Rounded).  
-00009c60: 2020 2020 2020 7365 6c66 2e74 6162 5f70        self.tab_p
-00009c70: 6361 2e73 6574 4f62 6a65 6374 4e61 6d65  ca.setObjectName
-00009c80: 2822 7461 625f 7063 6122 290a 2020 2020  ("tab_pca").    
-00009c90: 2020 2020 7365 6c66 2e74 6162 5f34 203d      self.tab_4 =
-00009ca0: 2051 7457 6964 6765 7473 2e51 5769 6467   QtWidgets.QWidg
-00009cb0: 6574 2829 0a20 2020 2020 2020 2073 656c  et().        sel
-00009cc0: 662e 7461 625f 342e 7365 744f 626a 6563  f.tab_4.setObjec
-00009cd0: 744e 616d 6528 2274 6162 5f34 2229 0a20  tName("tab_4"). 
-00009ce0: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-00009cf0: 4c61 796f 7574 5f31 3220 3d20 5174 5769  Layout_12 = QtWi
-00009d00: 6467 6574 732e 5147 7269 644c 6179 6f75  dgets.QGridLayou
-00009d10: 7428 7365 6c66 2e74 6162 5f34 290a 2020  t(self.tab_4).  
-00009d20: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
-00009d30: 6179 6f75 745f 3132 2e73 6574 4f62 6a65  ayout_12.setObje
-00009d40: 6374 4e61 6d65 2822 6772 6964 4c61 796f  ctName("gridLayo
-00009d50: 7574 5f31 3222 290a 2020 2020 2020 2020  ut_12").        
-00009d60: 7365 6c66 2e6c 6f67 626f 785f 7063 6120  self.logbox_pca 
-00009d70: 3d20 5174 5769 6467 6574 732e 5154 6578  = QtWidgets.QTex
-00009d80: 7445 6469 7428 7365 6c66 2e74 6162 5f34  tEdit(self.tab_4
-00009d90: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00009da0: 6f67 626f 785f 7063 612e 7365 744f 626a  ogbox_pca.setObj
-00009db0: 6563 744e 616d 6528 226c 6f67 626f 785f  ectName("logbox_
-00009dc0: 7063 6122 290a 2020 2020 2020 2020 7365  pca").        se
-00009dd0: 6c66 2e67 7269 644c 6179 6f75 745f 3132  lf.gridLayout_12
-00009de0: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
-00009df0: 6c6f 6762 6f78 5f70 6361 2c20 302c 2030  logbox_pca, 0, 0
-00009e00: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
-00009e10: 7365 6c66 2e74 6162 5f70 6361 2e61 6464  self.tab_pca.add
-00009e20: 5461 6228 7365 6c66 2e74 6162 5f34 2c20  Tab(self.tab_4, 
-00009e30: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
-00009e40: 2e74 6e5f 7375 6d6d 6172 7920 3d20 5174  .tn_summary = Qt
-00009e50: 5769 6467 6574 732e 5157 6964 6765 7428  Widgets.QWidget(
-00009e60: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-00009e70: 6e5f 7375 6d6d 6172 792e 7365 744f 626a  n_summary.setObj
-00009e80: 6563 744e 616d 6528 2274 6e5f 7375 6d6d  ectName("tn_summ
-00009e90: 6172 7922 290a 2020 2020 2020 2020 7365  ary").        se
-00009ea0: 6c66 2e67 7269 644c 6179 6f75 7420 3d20  lf.gridLayout = 
-00009eb0: 5174 5769 6467 6574 732e 5147 7269 644c  QtWidgets.QGridL
-00009ec0: 6179 6f75 7428 7365 6c66 2e74 6e5f 7375  ayout(self.tn_su
-00009ed0: 6d6d 6172 7929 0a20 2020 2020 2020 2073  mmary).        s
-00009ee0: 656c 662e 6772 6964 4c61 796f 7574 2e73  elf.gridLayout.s
-00009ef0: 6574 4f62 6a65 6374 4e61 6d65 2822 6772  etObjectName("gr
-00009f00: 6964 4c61 796f 7574 2229 0a20 2020 2020  idLayout").     
-00009f10: 2020 2073 656c 662e 6c61 6265 6c5f 3135     self.label_15
-00009f20: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
-00009f30: 6265 6c28 7365 6c66 2e74 6e5f 7375 6d6d  bel(self.tn_summ
-00009f40: 6172 7929 0a20 2020 2020 2020 2073 656c  ary).        sel
-00009f50: 662e 6c61 6265 6c5f 3135 2e73 6574 4f62  f.label_15.setOb
-00009f60: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
-00009f70: 3135 2229 0a20 2020 2020 2020 2073 656c  15").        sel
-00009f80: 662e 6772 6964 4c61 796f 7574 2e61 6464  f.gridLayout.add
-00009f90: 5769 6467 6574 2873 656c 662e 6c61 6265  Widget(self.labe
-00009fa0: 6c5f 3135 2c20 302c 2030 2c20 312c 2031  l_15, 0, 0, 1, 1
-00009fb0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-00009fc0: 6162 6c65 5f73 756d 6d61 7279 203d 2051  able_summary = Q
-00009fd0: 7457 6964 6765 7473 2e51 5461 626c 6556  tWidgets.QTableV
-00009fe0: 6965 7728 7365 6c66 2e74 6e5f 7375 6d6d  iew(self.tn_summ
-00009ff0: 6172 7929 0a20 2020 2020 2020 2073 656c  ary).        sel
-0000a000: 662e 7461 626c 655f 7375 6d6d 6172 792e  f.table_summary.
-0000a010: 7365 744f 626a 6563 744e 616d 6528 2274  setObjectName("t
-0000a020: 6162 6c65 5f73 756d 6d61 7279 2229 0a20  able_summary"). 
-0000a030: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-0000a040: 4c61 796f 7574 2e61 6464 5769 6467 6574  Layout.addWidget
-0000a050: 2873 656c 662e 7461 626c 655f 7375 6d6d  (self.table_summ
-0000a060: 6172 792c 2031 2c20 302c 2031 2c20 3129  ary, 1, 0, 1, 1)
-0000a070: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-0000a080: 6265 6c5f 3136 203d 2051 7457 6964 6765  bel_16 = QtWidge
-0000a090: 7473 2e51 4c61 6265 6c28 7365 6c66 2e74  ts.QLabel(self.t
-0000a0a0: 6e5f 7375 6d6d 6172 7929 0a20 2020 2020  n_summary).     
-0000a0b0: 2020 2073 656c 662e 6c61 6265 6c5f 3136     self.label_16
-0000a0c0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-0000a0d0: 6c61 6265 6c5f 3136 2229 0a20 2020 2020  label_16").     
-0000a0e0: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-0000a0f0: 7574 2e61 6464 5769 6467 6574 2873 656c  ut.addWidget(sel
-0000a100: 662e 6c61 6265 6c5f 3136 2c20 322c 2030  f.label_16, 2, 0
-0000a110: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
-0000a120: 7365 6c66 2e74 6162 6c65 5f76 6563 746f  self.table_vecto
-0000a130: 7220 3d20 5174 5769 6467 6574 732e 5154  r = QtWidgets.QT
-0000a140: 6162 6c65 5669 6577 2873 656c 662e 746e  ableView(self.tn
-0000a150: 5f73 756d 6d61 7279 290a 2020 2020 2020  _summary).      
-0000a160: 2020 7365 6c66 2e74 6162 6c65 5f76 6563    self.table_vec
-0000a170: 746f 722e 7365 744f 626a 6563 744e 616d  tor.setObjectNam
-0000a180: 6528 2274 6162 6c65 5f76 6563 746f 7222  e("table_vector"
-0000a190: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-0000a1a0: 7269 644c 6179 6f75 742e 6164 6457 6964  ridLayout.addWid
-0000a1b0: 6765 7428 7365 6c66 2e74 6162 6c65 5f76  get(self.table_v
-0000a1c0: 6563 746f 722c 2033 2c20 302c 2031 2c20  ector, 3, 0, 1, 
-0000a1d0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-0000a1e0: 7461 625f 7063 612e 6164 6454 6162 2873  tab_pca.addTab(s
-0000a1f0: 656c 662e 746e 5f73 756d 6d61 7279 2c20  elf.tn_summary, 
-0000a200: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
-0000a210: 2e74 6e5f 6772 6170 6820 3d20 5174 5769  .tn_graph = QtWi
-0000a220: 6467 6574 732e 5157 6964 6765 7428 290a  dgets.QWidget().
-0000a230: 2020 2020 2020 2020 7365 6c66 2e74 6e5f          self.tn_
-0000a240: 6772 6170 682e 7365 744f 626a 6563 744e  graph.setObjectN
-0000a250: 616d 6528 2274 6e5f 6772 6170 6822 290a  ame("tn_graph").
-0000a260: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
-0000a270: 644c 6179 6f75 745f 3131 203d 2051 7457  dLayout_11 = QtW
-0000a280: 6964 6765 7473 2e51 4772 6964 4c61 796f  idgets.QGridLayo
-0000a290: 7574 2873 656c 662e 746e 5f67 7261 7068  ut(self.tn_graph
-0000a2a0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-0000a2b0: 7269 644c 6179 6f75 745f 3131 2e73 6574  ridLayout_11.set
-0000a2c0: 4f62 6a65 6374 4e61 6d65 2822 6772 6964  ObjectName("grid
-0000a2d0: 4c61 796f 7574 5f31 3122 290a 2020 2020  Layout_11").    
-0000a2e0: 2020 2020 7365 6c66 2e63 616e 7661 7320      self.canvas 
-0000a2f0: 3d20 5174 5769 6467 6574 732e 5153 6372  = QtWidgets.QScr
-0000a300: 6f6c 6c41 7265 6128 7365 6c66 2e74 6e5f  ollArea(self.tn_
-0000a310: 6772 6170 6829 0a20 2020 2020 2020 2073  graph).        s
-0000a320: 656c 662e 6361 6e76 6173 2e73 6574 5769  elf.canvas.setWi
-0000a330: 6467 6574 5265 7369 7a61 626c 6528 5472  dgetResizable(Tr
-0000a340: 7565 290a 2020 2020 2020 2020 7365 6c66  ue).        self
-0000a350: 2e63 616e 7661 732e 7365 744f 626a 6563  .canvas.setObjec
-0000a360: 744e 616d 6528 2263 616e 7661 7322 290a  tName("canvas").
-0000a370: 2020 2020 2020 2020 7365 6c66 2e73 6372          self.scr
-0000a380: 6f6c 6c41 7265 6157 6964 6765 7443 6f6e  ollAreaWidgetCon
-0000a390: 7465 6e74 735f 3320 3d20 5174 5769 6467  tents_3 = QtWidg
-0000a3a0: 6574 732e 5157 6964 6765 7428 290a 2020  ets.QWidget().  
-0000a3b0: 2020 2020 2020 7365 6c66 2e73 6372 6f6c        self.scrol
-0000a3c0: 6c41 7265 6157 6964 6765 7443 6f6e 7465  lAreaWidgetConte
-0000a3d0: 6e74 735f 332e 7365 7447 656f 6d65 7472  nts_3.setGeometr
-0000a3e0: 7928 5174 436f 7265 2e51 5265 6374 2830  y(QtCore.QRect(0
-0000a3f0: 2c20 302c 2039 382c 2032 3829 290a 2020  , 0, 98, 28)).  
-0000a400: 2020 2020 2020 7365 6c66 2e73 6372 6f6c        self.scrol
-0000a410: 6c41 7265 6157 6964 6765 7443 6f6e 7465  lAreaWidgetConte
-0000a420: 6e74 735f 332e 7365 744f 626a 6563 744e  nts_3.setObjectN
-0000a430: 616d 6528 2273 6372 6f6c 6c41 7265 6157  ame("scrollAreaW
-0000a440: 6964 6765 7443 6f6e 7465 6e74 735f 3322  idgetContents_3"
-0000a450: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-0000a460: 616e 7661 732e 7365 7457 6964 6765 7428  anvas.setWidget(
-0000a470: 7365 6c66 2e73 6372 6f6c 6c41 7265 6157  self.scrollAreaW
-0000a480: 6964 6765 7443 6f6e 7465 6e74 735f 3329  idgetContents_3)
-0000a490: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-0000a4a0: 6964 4c61 796f 7574 5f31 312e 6164 6457  idLayout_11.addW
-0000a4b0: 6964 6765 7428 7365 6c66 2e63 616e 7661  idget(self.canva
-0000a4c0: 732c 2030 2c20 302c 2031 2c20 3129 0a20  s, 0, 0, 1, 1). 
-0000a4d0: 2020 2020 2020 2073 656c 662e 7461 625f         self.tab_
-0000a4e0: 7063 612e 6164 6454 6162 2873 656c 662e  pca.addTab(self.
-0000a4f0: 746e 5f67 7261 7068 2c20 2222 290a 2020  tn_graph, "").  
-0000a500: 2020 2020 2020 7365 6c66 2e68 6f72 697a        self.horiz
-0000a510: 6f6e 7461 6c4c 6179 6f75 742e 6164 6457  ontalLayout.addW
-0000a520: 6964 6765 7428 7365 6c66 2e74 6162 5f70  idget(self.tab_p
-0000a530: 6361 290a 2020 2020 2020 2020 7365 6c66  ca).        self
-0000a540: 2e74 6162 5769 6467 6574 2e61 6464 5461  .tabWidget.addTa
-0000a550: 6228 7365 6c66 2e74 6162 5f32 2c20 2222  b(self.tab_2, ""
-0000a560: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-0000a570: 6162 5f33 203d 2051 7457 6964 6765 7473  ab_3 = QtWidgets
-0000a580: 2e51 5769 6467 6574 2829 0a20 2020 2020  .QWidget().     
-0000a590: 2020 2073 656c 662e 7461 625f 332e 7365     self.tab_3.se
-0000a5a0: 744f 626a 6563 744e 616d 6528 2274 6162  tObjectName("tab
-0000a5b0: 5f33 2229 0a20 2020 2020 2020 2073 656c  _3").        sel
-0000a5c0: 662e 6772 6964 4c61 796f 7574 5f31 3020  f.gridLayout_10 
-0000a5d0: 3d20 5174 5769 6467 6574 732e 5147 7269  = QtWidgets.QGri
-0000a5e0: 644c 6179 6f75 7428 7365 6c66 2e74 6162  dLayout(self.tab
-0000a5f0: 5f33 290a 2020 2020 2020 2020 7365 6c66  _3).        self
-0000a600: 2e67 7269 644c 6179 6f75 745f 3130 2e73  .gridLayout_10.s
-0000a610: 6574 4f62 6a65 6374 4e61 6d65 2822 6772  etObjectName("gr
-0000a620: 6964 4c61 796f 7574 5f31 3022 290a 2020  idLayout_10").  
-0000a630: 2020 2020 2020 7365 6c66 2e66 7261 6d65        self.frame
-0000a640: 5f39 203d 2051 7457 6964 6765 7473 2e51  _9 = QtWidgets.Q
-0000a650: 4672 616d 6528 7365 6c66 2e74 6162 5f33  Frame(self.tab_3
-0000a660: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
-0000a670: 7261 6d65 5f39 2e73 6574 4d61 7869 6d75  rame_9.setMaximu
-0000a680: 6d53 697a 6528 5174 436f 7265 2e51 5369  mSize(QtCore.QSi
-0000a690: 7a65 2831 3530 2c20 3730 2929 0a20 2020  ze(150, 70)).   
-0000a6a0: 2020 2020 2073 656c 662e 6672 616d 655f       self.frame_
-0000a6b0: 392e 7365 7446 7261 6d65 5368 6170 6528  9.setFrameShape(
-0000a6c0: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-0000a6d0: 2e53 7479 6c65 6450 616e 656c 290a 2020  .StyledPanel).  
-0000a6e0: 2020 2020 2020 7365 6c66 2e66 7261 6d65        self.frame
-0000a6f0: 5f39 2e73 6574 4672 616d 6553 6861 646f  _9.setFrameShado
-0000a700: 7728 5174 5769 6467 6574 732e 5146 7261  w(QtWidgets.QFra
-0000a710: 6d65 2e52 6169 7365 6429 0a20 2020 2020  me.Raised).     
-0000a720: 2020 2073 656c 662e 6672 616d 655f 392e     self.frame_9.
-0000a730: 7365 744f 626a 6563 744e 616d 6528 2266  setObjectName("f
-0000a740: 7261 6d65 5f39 2229 0a20 2020 2020 2020  rame_9").       
-0000a750: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
-0000a760: 5f31 3520 3d20 5174 5769 6467 6574 732e  _15 = QtWidgets.
-0000a770: 5147 7269 644c 6179 6f75 7428 7365 6c66  QGridLayout(self
-0000a780: 2e66 7261 6d65 5f39 290a 2020 2020 2020  .frame_9).      
-0000a790: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-0000a7a0: 745f 3135 2e73 6574 4f62 6a65 6374 4e61  t_15.setObjectNa
-0000a7b0: 6d65 2822 6772 6964 4c61 796f 7574 5f31  me("gridLayout_1
-0000a7c0: 3522 290a 2020 2020 2020 2020 7365 6c66  5").        self
-0000a7d0: 2e6c 6162 656c 5f33 3620 3d20 5174 5769  .label_36 = QtWi
-0000a7e0: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-0000a7f0: 662e 6672 616d 655f 3929 0a20 2020 2020  f.frame_9).     
-0000a800: 2020 2066 6f6e 7420 3d20 5174 4775 692e     font = QtGui.
-0000a810: 5146 6f6e 7428 290a 2020 2020 2020 2020  QFont().        
-0000a820: 666f 6e74 2e73 6574 426f 6c64 2854 7275  font.setBold(Tru
-0000a830: 6529 0a20 2020 2020 2020 2066 6f6e 742e  e).        font.
-0000a840: 7365 7457 6569 6768 7428 3735 290a 2020  setWeight(75).  
-0000a850: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-0000a860: 5f33 362e 7365 7446 6f6e 7428 666f 6e74  _36.setFont(font
-0000a870: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-0000a880: 6162 656c 5f33 362e 7365 744f 626a 6563  abel_36.setObjec
-0000a890: 744e 616d 6528 226c 6162 656c 5f33 3622  tName("label_36"
-0000a8a0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-0000a8b0: 7269 644c 6179 6f75 745f 3135 2e61 6464  ridLayout_15.add
-0000a8c0: 5769 6467 6574 2873 656c 662e 6c61 6265  Widget(self.labe
-0000a8d0: 6c5f 3336 2c20 302c 2030 2c20 312c 2031  l_36, 0, 0, 1, 1
-0000a8e0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-0000a8f0: 6d62 5f72 6563 5479 7065 203d 2051 7457  mb_recType = QtW
-0000a900: 6964 6765 7473 2e51 436f 6d62 6f42 6f78  idgets.QComboBox
-0000a910: 2873 656c 662e 6672 616d 655f 3929 0a20  (self.frame_9). 
-0000a920: 2020 2020 2020 2073 656c 662e 636d 625f         self.cmb_
-0000a930: 7265 6354 7970 652e 7365 744f 626a 6563  recType.setObjec
-0000a940: 744e 616d 6528 2263 6d62 5f72 6563 5479  tName("cmb_recTy
-0000a950: 7065 2229 0a20 2020 2020 2020 2073 656c  pe").        sel
-0000a960: 662e 636d 625f 7265 6354 7970 652e 6164  f.cmb_recType.ad
-0000a970: 6449 7465 6d28 2222 290a 2020 2020 2020  dItem("").      
-0000a980: 2020 7365 6c66 2e63 6d62 5f72 6563 5479    self.cmb_recTy
-0000a990: 7065 2e61 6464 4974 656d 2822 2229 0a20  pe.addItem(""). 
-0000a9a0: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-0000a9b0: 4c61 796f 7574 5f31 352e 6164 6457 6964  Layout_15.addWid
-0000a9c0: 6765 7428 7365 6c66 2e63 6d62 5f72 6563  get(self.cmb_rec
-0000a9d0: 5479 7065 2c20 312c 2030 2c20 312c 2031  Type, 1, 0, 1, 1
-0000a9e0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-0000a9f0: 7269 644c 6179 6f75 745f 3130 2e61 6464  ridLayout_10.add
-0000aa00: 5769 6467 6574 2873 656c 662e 6672 616d  Widget(self.fram
-0000aa10: 655f 392c 2030 2c20 302c 2031 2c20 3129  e_9, 0, 0, 1, 1)
-0000aa20: 0a20 2020 2020 2020 2073 656c 662e 6667  .        self.fg
-0000aa30: 5f31 5f31 203d 2051 7457 6964 6765 7473  _1_1 = QtWidgets
-0000aa40: 2e51 4672 616d 6528 7365 6c66 2e74 6162  .QFrame(self.tab
-0000aa50: 5f33 290a 2020 2020 2020 2020 7365 6c66  _3).        self
-0000aa60: 2e66 675f 315f 312e 7365 7446 7261 6d65  .fg_1_1.setFrame
-0000aa70: 5368 6170 6528 5174 5769 6467 6574 732e  Shape(QtWidgets.
-0000aa80: 5146 7261 6d65 2e53 7479 6c65 6450 616e  QFrame.StyledPan
-0000aa90: 656c 290a 2020 2020 2020 2020 7365 6c66  el).        self
-0000aaa0: 2e66 675f 315f 312e 7365 7446 7261 6d65  .fg_1_1.setFrame
-0000aab0: 5368 6164 6f77 2851 7457 6964 6765 7473  Shadow(QtWidgets
-0000aac0: 2e51 4672 616d 652e 5261 6973 6564 290a  .QFrame.Raised).
-0000aad0: 2020 2020 2020 2020 7365 6c66 2e66 675f          self.fg_
-0000aae0: 315f 312e 7365 744f 626a 6563 744e 616d  1_1.setObjectNam
-0000aaf0: 6528 2266 675f 315f 3122 290a 2020 2020  e("fg_1_1").    
-0000ab00: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
-0000ab10: 6f75 745f 3130 2e61 6464 5769 6467 6574  out_10.addWidget
-0000ab20: 2873 656c 662e 6667 5f31 5f31 2c20 302c  (self.fg_1_1, 0,
-0000ab30: 2031 2c20 322c 2031 290a 2020 2020 2020   1, 2, 1).      
-0000ab40: 2020 7365 6c66 2e66 7261 6d65 5f32 203d    self.frame_2 =
-0000ab50: 2051 7457 6964 6765 7473 2e51 4672 616d   QtWidgets.QFram
-0000ab60: 6528 7365 6c66 2e74 6162 5f33 290a 2020  e(self.tab_3).  
-0000ab70: 2020 2020 2020 7365 6c66 2e66 7261 6d65        self.frame
-0000ab80: 5f32 2e73 6574 4d61 7869 6d75 6d53 697a  _2.setMaximumSiz
-0000ab90: 6528 5174 436f 7265 2e51 5369 7a65 2831  e(QtCore.QSize(1
-0000aba0: 3530 2c20 3136 3737 3732 3135 2929 0a20  50, 16777215)). 
-0000abb0: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
-0000abc0: 655f 322e 7365 7446 7261 6d65 5368 6170  e_2.setFrameShap
-0000abd0: 6528 5174 5769 6467 6574 732e 5146 7261  e(QtWidgets.QFra
-0000abe0: 6d65 2e53 7479 6c65 6450 616e 656c 290a  me.StyledPanel).
-0000abf0: 2020 2020 2020 2020 7365 6c66 2e66 7261          self.fra
-0000ac00: 6d65 5f32 2e73 6574 4672 616d 6553 6861  me_2.setFrameSha
-0000ac10: 646f 7728 5174 5769 6467 6574 732e 5146  dow(QtWidgets.QF
-0000ac20: 7261 6d65 2e52 6169 7365 6429 0a20 2020  rame.Raised).   
-0000ac30: 2020 2020 2073 656c 662e 6672 616d 655f       self.frame_
-0000ac40: 322e 7365 744f 626a 6563 744e 616d 6528  2.setObjectName(
-0000ac50: 2266 7261 6d65 5f32 2229 0a20 2020 2020  "frame_2").     
-0000ac60: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-0000ac70: 7574 5f38 203d 2051 7457 6964 6765 7473  ut_8 = QtWidgets
-0000ac80: 2e51 4772 6964 4c61 796f 7574 2873 656c  .QGridLayout(sel
-0000ac90: 662e 6672 616d 655f 3229 0a20 2020 2020  f.frame_2).     
-0000aca0: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
-0000acb0: 7574 5f38 2e73 6574 4f62 6a65 6374 4e61  ut_8.setObjectNa
-0000acc0: 6d65 2822 6772 6964 4c61 796f 7574 5f38  me("gridLayout_8
-0000acd0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000ace0: 6275 7474 6f6e 5f73 6176 6552 6563 6f6e  button_saveRecon
-0000acf0: 7374 203d 2051 7457 6964 6765 7473 2e51  st = QtWidgets.Q
-0000ad00: 5075 7368 4275 7474 6f6e 2873 656c 662e  PushButton(self.
-0000ad10: 6672 616d 655f 3229 0a20 2020 2020 2020  frame_2).       
-0000ad20: 2073 656c 662e 6275 7474 6f6e 5f73 6176   self.button_sav
-0000ad30: 6552 6563 6f6e 7374 2e73 6574 4f62 6a65  eReconst.setObje
-0000ad40: 6374 4e61 6d65 2822 6275 7474 6f6e 5f73  ctName("button_s
-0000ad50: 6176 6552 6563 6f6e 7374 2229 0a20 2020  aveReconst").   
-0000ad60: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
-0000ad70: 796f 7574 5f38 2e61 6464 5769 6467 6574  yout_8.addWidget
-0000ad80: 2873 656c 662e 6275 7474 6f6e 5f73 6176  (self.button_sav
-0000ad90: 6552 6563 6f6e 7374 2c20 3130 2c20 302c  eReconst, 10, 0,
-0000ada0: 2031 2c20 3229 0a20 2020 2020 2020 2073   1, 2).        s
-0000adb0: 656c 662e 636d 625f 4949 4950 203d 2051  elf.cmb_IIIP = Q
-0000adc0: 7457 6964 6765 7473 2e51 436f 6d62 6f42  tWidgets.QComboB
-0000add0: 6f78 2873 656c 662e 6672 616d 655f 3229  ox(self.frame_2)
-0000ade0: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
-0000adf0: 625f 4949 4950 2e73 6574 456e 6162 6c65  b_IIIP.setEnable
-0000ae00: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
-0000ae10: 2073 656c 662e 636d 625f 4949 4950 2e73   self.cmb_IIIP.s
-0000ae20: 6574 4f62 6a65 6374 4e61 6d65 2822 636d  etObjectName("cm
-0000ae30: 625f 4949 4950 2229 0a20 2020 2020 2020  b_IIIP").       
-0000ae40: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
-0000ae50: 5f38 2e61 6464 5769 6467 6574 2873 656c  _8.addWidget(sel
-0000ae60: 662e 636d 625f 4949 4950 2c20 362c 2030  f.cmb_IIIP, 6, 0
-0000ae70: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
-0000ae80: 7365 6c66 2e64 7362 5f49 4949 6420 3d20  self.dsb_IIId = 
-0000ae90: 5174 5769 6467 6574 732e 5144 6f75 626c  QtWidgets.QDoubl
-0000aea0: 6553 7069 6e42 6f78 2873 656c 662e 6672  eSpinBox(self.fr
-0000aeb0: 616d 655f 3229 0a20 2020 2020 2020 2073  ame_2).        s
-0000aec0: 656c 662e 6473 625f 4949 4964 2e73 6574  elf.dsb_IIId.set
-0000aed0: 456e 6162 6c65 6428 4661 6c73 6529 0a20  Enabled(False). 
-0000aee0: 2020 2020 2020 2073 656c 662e 6473 625f         self.dsb_
-0000aef0: 4949 4964 2e73 6574 4465 6369 6d61 6c73  IIId.setDecimals
-0000af00: 2831 290a 2020 2020 2020 2020 7365 6c66  (1).        self
-0000af10: 2e64 7362 5f49 4949 642e 7365 744d 696e  .dsb_IIId.setMin
-0000af20: 696d 756d 282d 352e 3029 0a20 2020 2020  imum(-5.0).     
-0000af30: 2020 2073 656c 662e 6473 625f 4949 4964     self.dsb_IIId
-0000af40: 2e73 6574 4d61 7869 6d75 6d28 352e 3029  .setMaximum(5.0)
-0000af50: 0a20 2020 2020 2020 2073 656c 662e 6473  .        self.ds
-0000af60: 625f 4949 4964 2e73 6574 5369 6e67 6c65  b_IIId.setSingle
-0000af70: 5374 6570 2830 2e31 290a 2020 2020 2020  Step(0.1).      
-0000af80: 2020 7365 6c66 2e64 7362 5f49 4949 642e    self.dsb_IIId.
-0000af90: 7365 744f 626a 6563 744e 616d 6528 2264  setObjectName("d
-0000afa0: 7362 5f49 4949 6422 290a 2020 2020 2020  sb_IIId").      
-0000afb0: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
-0000afc0: 745f 382e 6164 6457 6964 6765 7428 7365  t_8.addWidget(se
-0000afd0: 6c66 2e64 7362 5f49 4949 642c 2036 2c20  lf.dsb_IIId, 6, 
-0000afe0: 312c 2031 2c20 3129 0a20 2020 2020 2020  1, 1, 1).       
-0000aff0: 2073 656c 662e 636d 625f 7375 6d44 6576   self.cmb_sumDev
-0000b000: 203d 2051 7457 6964 6765 7473 2e51 436f   = QtWidgets.QCo
-0000b010: 6d62 6f42 6f78 2873 656c 662e 6672 616d  mboBox(self.fram
-0000b020: 655f 3229 0a20 2020 2020 2020 2073 656c  e_2).        sel
-0000b030: 662e 636d 625f 7375 6d44 6576 2e73 6574  f.cmb_sumDev.set
-0000b040: 4f62 6a65 6374 4e61 6d65 2822 636d 625f  ObjectName("cmb_
-0000b050: 7375 6d44 6576 2229 0a20 2020 2020 2020  sumDev").       
-0000b060: 2073 656c 662e 636d 625f 7375 6d44 6576   self.cmb_sumDev
-0000b070: 2e61 6464 4974 656d 2822 2229 0a20 2020  .addItem("").   
-0000b080: 2020 2020 2073 656c 662e 636d 625f 7375       self.cmb_su
-0000b090: 6d44 6576 2e61 6464 4974 656d 2822 2229  mDev.addItem("")
-0000b0a0: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
-0000b0b0: 625f 7375 6d44 6576 2e61 6464 4974 656d  b_sumDev.addItem
-0000b0c0: 2822 2229 0a20 2020 2020 2020 2073 656c  ("").        sel
-0000b0d0: 662e 636d 625f 7375 6d44 6576 2e61 6464  f.cmb_sumDev.add
-0000b0e0: 4974 656d 2822 2229 0a20 2020 2020 2020  Item("").       
-0000b0f0: 2073 656c 662e 636d 625f 7375 6d44 6576   self.cmb_sumDev
-0000b100: 2e61 6464 4974 656d 2822 2229 0a20 2020  .addItem("").   
-0000b110: 2020 2020 2073 656c 662e 636d 625f 7375       self.cmb_su
-0000b120: 6d44 6576 2e61 6464 4974 656d 2822 2229  mDev.addItem("")
-0000b130: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-0000b140: 6964 4c61 796f 7574 5f38 2e61 6464 5769  idLayout_8.addWi
-0000b150: 6467 6574 2873 656c 662e 636d 625f 7375  dget(self.cmb_su
-0000b160: 6d44 6576 2c20 312c 2030 2c20 312c 2032  mDev, 1, 0, 1, 2
-0000b170: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
-0000b180: 7574 746f 6e5f 6765 6e65 7261 7465 203d  utton_generate =
-0000b190: 2051 7457 6964 6765 7473 2e51 5075 7368   QtWidgets.QPush
-0000b1a0: 4275 7474 6f6e 2873 656c 662e 6672 616d  Button(self.fram
-0000b1b0: 655f 3229 0a20 2020 2020 2020 2073 656c  e_2).        sel
-0000b1c0: 662e 6275 7474 6f6e 5f67 656e 6572 6174  f.button_generat
-0000b1d0: 652e 7365 744f 626a 6563 744e 616d 6528  e.setObjectName(
-0000b1e0: 2262 7574 746f 6e5f 6765 6e65 7261 7465  "button_generate
-0000b1f0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000b200: 6772 6964 4c61 796f 7574 5f38 2e61 6464  gridLayout_8.add
-0000b210: 5769 6467 6574 2873 656c 662e 6275 7474  Widget(self.butt
-0000b220: 6f6e 5f67 656e 6572 6174 652c 2039 2c20  on_generate, 9, 
-0000b230: 302c 2031 2c20 3229 0a20 2020 2020 2020  0, 1, 2).       
-0000b240: 2073 656c 662e 6c61 6265 6c5f 3236 203d   self.label_26 =
-0000b250: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
-0000b260: 6c28 7365 6c66 2e66 7261 6d65 5f32 290a  l(self.frame_2).
-0000b270: 2020 2020 2020 2020 666f 6e74 203d 2051          font = Q
-0000b280: 7447 7569 2e51 466f 6e74 2829 0a20 2020  tGui.QFont().   
-0000b290: 2020 2020 2066 6f6e 742e 7365 7450 6f69       font.setPoi
-0000b2a0: 6e74 5369 7a65 2831 3329 0a20 2020 2020  ntSize(13).     
-0000b2b0: 2020 2066 6f6e 742e 7365 7442 6f6c 6428     font.setBold(
-0000b2c0: 4661 6c73 6529 0a20 2020 2020 2020 2066  False).        f
-0000b2d0: 6f6e 742e 7365 7457 6569 6768 7428 3530  ont.setWeight(50
-0000b2e0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-0000b2f0: 6162 656c 5f32 362e 7365 7446 6f6e 7428  abel_26.setFont(
-0000b300: 666f 6e74 290a 2020 2020 2020 2020 7365  font).        se
-0000b310: 6c66 2e6c 6162 656c 5f32 362e 7365 744f  lf.label_26.setO
-0000b320: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
-0000b330: 5f32 3622 290a 2020 2020 2020 2020 7365  _26").        se
-0000b340: 6c66 2e67 7269 644c 6179 6f75 745f 382e  lf.gridLayout_8.
-0000b350: 6164 6457 6964 6765 7428 7365 6c66 2e6c  addWidget(self.l
-0000b360: 6162 656c 5f32 362c 2033 2c20 312c 2031  abel_26, 3, 1, 1
-0000b370: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
-0000b380: 662e 6473 625f 4964 203d 2051 7457 6964  f.dsb_Id = QtWid
-0000b390: 6765 7473 2e51 446f 7562 6c65 5370 696e  gets.QDoubleSpin
-0000b3a0: 426f 7828 7365 6c66 2e66 7261 6d65 5f32  Box(self.frame_2
-0000b3b0: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
-0000b3c0: 7362 5f49 642e 7365 7445 6e61 626c 6564  sb_Id.setEnabled
-0000b3d0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
-0000b3e0: 7365 6c66 2e64 7362 5f49 642e 7365 7444  self.dsb_Id.setD
-0000b3f0: 6563 696d 616c 7328 3129 0a20 2020 2020  ecimals(1).     
-0000b400: 2020 2073 656c 662e 6473 625f 4964 2e73     self.dsb_Id.s
-0000b410: 6574 4d69 6e69 6d75 6d28 2d35 2e30 290a  etMinimum(-5.0).
-0000b420: 2020 2020 2020 2020 7365 6c66 2e64 7362          self.dsb
-0000b430: 5f49 642e 7365 744d 6178 696d 756d 2835  _Id.setMaximum(5
-0000b440: 2e30 290a 2020 2020 2020 2020 7365 6c66  .0).        self
-0000b450: 2e64 7362 5f49 642e 7365 7453 696e 676c  .dsb_Id.setSingl
-0000b460: 6553 7465 7028 302e 3129 0a20 2020 2020  eStep(0.1).     
-0000b470: 2020 2073 656c 662e 6473 625f 4964 2e73     self.dsb_Id.s
-0000b480: 6574 4f62 6a65 6374 4e61 6d65 2822 6473  etObjectName("ds
-0000b490: 625f 4964 2229 0a20 2020 2020 2020 2073  b_Id").        s
-0000b4a0: 656c 662e 6772 6964 4c61 796f 7574 5f38  elf.gridLayout_8
-0000b4b0: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
-0000b4c0: 6473 625f 4964 2c20 342c 2031 2c20 312c  dsb_Id, 4, 1, 1,
-0000b4d0: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
-0000b4e0: 2e6c 6162 656c 5f32 3720 3d20 5174 5769  .label_27 = QtWi
-0000b4f0: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-0000b500: 662e 6672 616d 655f 3229 0a20 2020 2020  f.frame_2).     
-0000b510: 2020 2066 6f6e 7420 3d20 5174 4775 692e     font = QtGui.
-0000b520: 5146 6f6e 7428 290a 2020 2020 2020 2020  QFont().        
-0000b530: 666f 6e74 2e73 6574 426f 6c64 2854 7275  font.setBold(Tru
-0000b540: 6529 0a20 2020 2020 2020 2066 6f6e 742e  e).        font.
-0000b550: 7365 7457 6569 6768 7428 3735 290a 2020  setWeight(75).  
-0000b560: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-0000b570: 5f32 372e 7365 7446 6f6e 7428 666f 6e74  _27.setFont(font
-0000b580: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-0000b590: 6162 656c 5f32 372e 7365 744f 626a 6563  abel_27.setObjec
-0000b5a0: 744e 616d 6528 226c 6162 656c 5f32 3722  tName("label_27"
-0000b5b0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-0000b5c0: 7269 644c 6179 6f75 745f 382e 6164 6457  ridLayout_8.addW
-0000b5d0: 6964 6765 7428 7365 6c66 2e6c 6162 656c  idget(self.label
-0000b5e0: 5f32 372c 2032 2c20 302c 2031 2c20 3229  _27, 2, 0, 1, 2)
-0000b5f0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-0000b600: 6265 6c5f 3235 203d 2051 7457 6964 6765  bel_25 = QtWidge
-0000b610: 7473 2e51 4c61 6265 6c28 7365 6c66 2e66  ts.QLabel(self.f
-0000b620: 7261 6d65 5f32 290a 2020 2020 2020 2020  rame_2).        
-0000b630: 7365 6c66 2e6c 6162 656c 5f32 352e 7365  self.label_25.se
-0000b640: 744f 626a 6563 744e 616d 6528 226c 6162  tObjectName("lab
-0000b650: 656c 5f32 3522 290a 2020 2020 2020 2020  el_25").        
-0000b660: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
-0000b670: 382e 6164 6457 6964 6765 7428 7365 6c66  8.addWidget(self
-0000b680: 2e6c 6162 656c 5f32 352c 2033 2c20 302c  .label_25, 3, 0,
-0000b690: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
-0000b6a0: 656c 662e 6c61 6265 6c5f 3233 203d 2051  elf.label_23 = Q
-0000b6b0: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
-0000b6c0: 7365 6c66 2e66 7261 6d65 5f32 290a 2020  self.frame_2).  
-0000b6d0: 2020 2020 2020 666f 6e74 203d 2051 7447        font = QtG
-0000b6e0: 7569 2e51 466f 6e74 2829 0a20 2020 2020  ui.QFont().     
-0000b6f0: 2020 2066 6f6e 742e 7365 7442 6f6c 6428     font.setBold(
-0000b700: 5472 7565 290a 2020 2020 2020 2020 666f  True).        fo
-0000b710: 6e74 2e73 6574 5765 6967 6874 2837 3529  nt.setWeight(75)
-0000b720: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-0000b730: 6265 6c5f 3233 2e73 6574 466f 6e74 2866  bel_23.setFont(f
-0000b740: 6f6e 7429 0a20 2020 2020 2020 2073 656c  ont).        sel
-0000b750: 662e 6c61 6265 6c5f 3233 2e73 6574 4f62  f.label_23.setOb
-0000b760: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
-0000b770: 3233 2229 0a20 2020 2020 2020 2073 656c  23").        sel
-0000b780: 662e 6772 6964 4c61 796f 7574 5f38 2e61  f.gridLayout_8.a
-0000b790: 6464 5769 6467 6574 2873 656c 662e 6c61  ddWidget(self.la
-0000b7a0: 6265 6c5f 3233 2c20 302c 2030 2c20 312c  bel_23, 0, 0, 1,
-0000b7b0: 2032 290a 2020 2020 2020 2020 7365 6c66   2).        self
-0000b7c0: 2e64 7362 5f49 4964 203d 2051 7457 6964  .dsb_IId = QtWid
-0000b7d0: 6765 7473 2e51 446f 7562 6c65 5370 696e  gets.QDoubleSpin
-0000b7e0: 426f 7828 7365 6c66 2e66 7261 6d65 5f32  Box(self.frame_2
-0000b7f0: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
-0000b800: 7362 5f49 4964 2e73 6574 456e 6162 6c65  sb_IId.setEnable
-0000b810: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
-0000b820: 2073 656c 662e 6473 625f 4949 642e 7365   self.dsb_IId.se
-0000b830: 7444 6563 696d 616c 7328 3129 0a20 2020  tDecimals(1).   
-0000b840: 2020 2020 2073 656c 662e 6473 625f 4949       self.dsb_II
-0000b850: 642e 7365 744d 696e 696d 756d 282d 352e  d.setMinimum(-5.
-0000b860: 3029 0a20 2020 2020 2020 2073 656c 662e  0).        self.
-0000b870: 6473 625f 4949 642e 7365 744d 6178 696d  dsb_IId.setMaxim
-0000b880: 756d 2835 2e30 290a 2020 2020 2020 2020  um(5.0).        
-0000b890: 7365 6c66 2e64 7362 5f49 4964 2e73 6574  self.dsb_IId.set
-0000b8a0: 5369 6e67 6c65 5374 6570 2830 2e31 290a  SingleStep(0.1).
-0000b8b0: 2020 2020 2020 2020 7365 6c66 2e64 7362          self.dsb
-0000b8c0: 5f49 4964 2e73 6574 4f62 6a65 6374 4e61  _IId.setObjectNa
-0000b8d0: 6d65 2822 6473 625f 4949 6422 290a 2020  me("dsb_IId").  
-0000b8e0: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
-0000b8f0: 6179 6f75 745f 382e 6164 6457 6964 6765  ayout_8.addWidge
-0000b900: 7428 7365 6c66 2e64 7362 5f49 4964 2c20  t(self.dsb_IId, 
-0000b910: 352c 2031 2c20 312c 2031 290a 2020 2020  5, 1, 1, 1).    
-0000b920: 2020 2020 7365 6c66 2e63 6d62 5f49 5020      self.cmb_IP 
-0000b930: 3d20 5174 5769 6467 6574 732e 5143 6f6d  = QtWidgets.QCom
-0000b940: 626f 426f 7828 7365 6c66 2e66 7261 6d65  boBox(self.frame
-0000b950: 5f32 290a 2020 2020 2020 2020 7365 6c66  _2).        self
-0000b960: 2e63 6d62 5f49 502e 7365 7445 6e61 626c  .cmb_IP.setEnabl
-0000b970: 6564 2846 616c 7365 290a 2020 2020 2020  ed(False).      
-0000b980: 2020 7365 6c66 2e63 6d62 5f49 502e 7365    self.cmb_IP.se
-0000b990: 744f 626a 6563 744e 616d 6528 2263 6d62  tObjectName("cmb
-0000b9a0: 5f49 5022 290a 2020 2020 2020 2020 7365  _IP").        se
-0000b9b0: 6c66 2e67 7269 644c 6179 6f75 745f 382e  lf.gridLayout_8.
-0000b9c0: 6164 6457 6964 6765 7428 7365 6c66 2e63  addWidget(self.c
-0000b9d0: 6d62 5f49 502c 2034 2c20 302c 2031 2c20  mb_IP, 4, 0, 1, 
-0000b9e0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-0000b9f0: 636d 625f 4949 5020 3d20 5174 5769 6467  cmb_IIP = QtWidg
-0000ba00: 6574 732e 5143 6f6d 626f 426f 7828 7365  ets.QComboBox(se
-0000ba10: 6c66 2e66 7261 6d65 5f32 290a 2020 2020  lf.frame_2).    
-0000ba20: 2020 2020 7365 6c66 2e63 6d62 5f49 4950      self.cmb_IIP
-0000ba30: 2e73 6574 456e 6162 6c65 6428 4661 6c73  .setEnabled(Fals
-0000ba40: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-0000ba50: 636d 625f 4949 502e 7365 744f 626a 6563  cmb_IIP.setObjec
-0000ba60: 744e 616d 6528 2263 6d62 5f49 4950 2229  tName("cmb_IIP")
-0000ba70: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-0000ba80: 6964 4c61 796f 7574 5f38 2e61 6464 5769  idLayout_8.addWi
-0000ba90: 6467 6574 2873 656c 662e 636d 625f 4949  dget(self.cmb_II
-0000baa0: 502c 2035 2c20 302c 2031 2c20 3129 0a20  P, 5, 0, 1, 1). 
-0000bab0: 2020 2020 2020 2073 656c 662e 6c69 6e65         self.line
-0000bac0: 5f36 203d 2051 7457 6964 6765 7473 2e51  _6 = QtWidgets.Q
-0000bad0: 4672 616d 6528 7365 6c66 2e66 7261 6d65  Frame(self.frame
-0000bae0: 5f32 290a 2020 2020 2020 2020 7365 6c66  _2).        self
-0000baf0: 2e6c 696e 655f 362e 7365 7446 7261 6d65  .line_6.setFrame
-0000bb00: 5368 6170 6528 5174 5769 6467 6574 732e  Shape(QtWidgets.
-0000bb10: 5146 7261 6d65 2e48 4c69 6e65 290a 2020  QFrame.HLine).  
-0000bb20: 2020 2020 2020 7365 6c66 2e6c 696e 655f        self.line_
-0000bb30: 362e 7365 7446 7261 6d65 5368 6164 6f77  6.setFrameShadow
-0000bb40: 2851 7457 6964 6765 7473 2e51 4672 616d  (QtWidgets.QFram
-0000bb50: 652e 5375 6e6b 656e 290a 2020 2020 2020  e.Sunken).      
-0000bb60: 2020 7365 6c66 2e6c 696e 655f 362e 7365    self.line_6.se
-0000bb70: 744f 626a 6563 744e 616d 6528 226c 696e  tObjectName("lin
-0000bb80: 655f 3622 290a 2020 2020 2020 2020 7365  e_6").        se
-0000bb90: 6c66 2e67 7269 644c 6179 6f75 745f 382e  lf.gridLayout_8.
-0000bba0: 6164 6457 6964 6765 7428 7365 6c66 2e6c  addWidget(self.l
-0000bbb0: 696e 655f 362c 2037 2c20 302c 2031 2c20  ine_6, 7, 0, 1, 
-0000bbc0: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
-0000bbd0: 6772 6964 4c61 796f 7574 5f31 302e 6164  gridLayout_10.ad
-0000bbe0: 6457 6964 6765 7428 7365 6c66 2e66 7261  dWidget(self.fra
-0000bbf0: 6d65 5f32 2c20 312c 2030 2c20 312c 2031  me_2, 1, 0, 1, 1
-0000bc00: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-0000bc10: 6162 5769 6467 6574 2e61 6464 5461 6228  abWidget.addTab(
-0000bc20: 7365 6c66 2e74 6162 5f33 2c20 2222 290a  self.tab_3, "").
-0000bc30: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
-0000bc40: 644c 6179 6f75 745f 372e 6164 6457 6964  dLayout_7.addWid
-0000bc50: 6765 7428 7365 6c66 2e74 6162 5769 6467  get(self.tabWidg
-0000bc60: 6574 2c20 302c 2031 2c20 312c 2031 290a  et, 0, 1, 1, 1).
-0000bc70: 2020 2020 2020 2020 4d61 696e 5769 6e64          MainWind
-0000bc80: 6f77 2e73 6574 4365 6e74 7261 6c57 6964  ow.setCentralWid
-0000bc90: 6765 7428 7365 6c66 2e63 656e 7472 616c  get(self.central
-0000bca0: 7769 6467 6574 290a 2020 2020 2020 2020  widget).        
-0000bcb0: 7365 6c66 2e6d 656e 7562 6172 203d 2051  self.menubar = Q
-0000bcc0: 7457 6964 6765 7473 2e51 4d65 6e75 4261  tWidgets.QMenuBa
-0000bcd0: 7228 4d61 696e 5769 6e64 6f77 290a 2020  r(MainWindow).  
-0000bce0: 2020 2020 2020 7365 6c66 2e6d 656e 7562        self.menub
-0000bcf0: 6172 2e73 6574 4765 6f6d 6574 7279 2851  ar.setGeometry(Q
-0000bd00: 7443 6f72 652e 5152 6563 7428 302c 2030  tCore.QRect(0, 0
-0000bd10: 2c20 3831 302c 2032 3229 290a 2020 2020  , 810, 22)).    
-0000bd20: 2020 2020 7365 6c66 2e6d 656e 7562 6172      self.menubar
-0000bd30: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-0000bd40: 6d65 6e75 6261 7222 290a 2020 2020 2020  menubar").      
-0000bd50: 2020 7365 6c66 2e6d 656e 7574 6573 7420    self.menutest 
-0000bd60: 3d20 5174 5769 6467 6574 732e 514d 656e  = QtWidgets.QMen
-0000bd70: 7528 7365 6c66 2e6d 656e 7562 6172 290a  u(self.menubar).
-0000bd80: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
-0000bd90: 7574 6573 742e 7365 744f 626a 6563 744e  utest.setObjectN
-0000bda0: 616d 6528 226d 656e 7574 6573 7422 290a  ame("menutest").
-0000bdb0: 2020 2020 2020 2020 4d61 696e 5769 6e64          MainWind
-0000bdc0: 6f77 2e73 6574 4d65 6e75 4261 7228 7365  ow.setMenuBar(se
-0000bdd0: 6c66 2e6d 656e 7562 6172 290a 2020 2020  lf.menubar).    
-0000bde0: 2020 2020 7365 6c66 2e73 7461 7475 7362      self.statusb
-0000bdf0: 6172 203d 2051 7457 6964 6765 7473 2e51  ar = QtWidgets.Q
-0000be00: 5374 6174 7573 4261 7228 4d61 696e 5769  StatusBar(MainWi
-0000be10: 6e64 6f77 290a 2020 2020 2020 2020 7365  ndow).        se
-0000be20: 6c66 2e73 7461 7475 7362 6172 2e73 6574  lf.statusbar.set
-0000be30: 4f62 6a65 6374 4e61 6d65 2822 7374 6174  ObjectName("stat
-0000be40: 7573 6261 7222 290a 2020 2020 2020 2020  usbar").        
-0000be50: 4d61 696e 5769 6e64 6f77 2e73 6574 5374  MainWindow.setSt
-0000be60: 6174 7573 4261 7228 7365 6c66 2e73 7461  atusBar(self.sta
-0000be70: 7475 7362 6172 290a 2020 2020 2020 2020  tusbar).        
-0000be80: 7365 6c66 2e61 6374 696f 6e41 626f 7574  self.actionAbout
-0000be90: 203d 2051 7457 6964 6765 7473 2e51 4163   = QtWidgets.QAc
-0000bea0: 7469 6f6e 284d 6169 6e57 696e 646f 7729  tion(MainWindow)
-0000beb0: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-0000bec0: 7469 6f6e 4162 6f75 742e 7365 744f 626a  tionAbout.setObj
-0000bed0: 6563 744e 616d 6528 2261 6374 696f 6e41  ectName("actionA
-0000bee0: 626f 7574 2229 0a20 2020 2020 2020 2073  bout").        s
-0000bef0: 656c 662e 6d65 6e75 7465 7374 2e61 6464  elf.menutest.add
-0000bf00: 4163 7469 6f6e 2873 656c 662e 6163 7469  Action(self.acti
-0000bf10: 6f6e 4162 6f75 7429 0a20 2020 2020 2020  onAbout).       
-0000bf20: 2073 656c 662e 6d65 6e75 6261 722e 6164   self.menubar.ad
-0000bf30: 6441 6374 696f 6e28 7365 6c66 2e6d 656e  dAction(self.men
-0000bf40: 7574 6573 742e 6d65 6e75 4163 7469 6f6e  utest.menuAction
-0000bf50: 2829 290a 0a20 2020 2020 2020 2073 656c  ())..        sel
-0000bf60: 662e 7265 7472 616e 736c 6174 6555 6928  f.retranslateUi(
-0000bf70: 4d61 696e 5769 6e64 6f77 290a 2020 2020  MainWindow).    
-0000bf80: 2020 2020 7365 6c66 2e74 6162 5769 6467      self.tabWidg
-0000bf90: 6574 2e73 6574 4375 7272 656e 7449 6e64  et.setCurrentInd
-0000bfa0: 6578 2830 290a 2020 2020 2020 2020 7365  ex(0).        se
-0000bfb0: 6c66 2e74 6162 5769 6467 6574 5f32 2e73  lf.tabWidget_2.s
-0000bfc0: 6574 4375 7272 656e 7449 6e64 6578 2832  etCurrentIndex(2
-0000bfd0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-0000bfe0: 6162 5f70 6361 2e73 6574 4375 7272 656e  ab_pca.setCurren
-0000bff0: 7449 6e64 6578 2830 290a 2020 2020 2020  tIndex(0).      
-0000c000: 2020 7365 6c66 2e63 6d62 5f66 6f72 6d61    self.cmb_forma
-0000c010: 742e 6375 7272 656e 7449 6e64 6578 4368  t.currentIndexCh
-0000c020: 616e 6765 645b 2751 5374 7269 6e67 275d  anged['QString']
-0000c030: 2e63 6f6e 6e65 6374 284d 6169 6e57 696e  .connect(MainWin
-0000c040: 646f 772e 7365 7446 6f72 6d61 7429 0a20  dow.setFormat). 
-0000c050: 2020 2020 2020 2073 656c 662e 6275 7474         self.butt
-0000c060: 6f6e 5f66 6f6c 6461 2e63 6c69 636b 6564  on_folda.clicked
-0000c070: 2e63 6f6e 6e65 6374 284d 6169 6e57 696e  .connect(MainWin
-0000c080: 646f 772e 7365 7446 6f6c 6461 5061 7468  dow.setFoldaPath
-0000c090: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
-0000c0a0: 7574 746f 6e5f 7361 7665 2e63 6c69 636b  utton_save.click
-0000c0b0: 6564 2e63 6f6e 6e65 6374 284d 6169 6e57  ed.connect(MainW
-0000c0c0: 696e 646f 772e 7365 7453 6176 6550 6174  indow.setSavePat
-0000c0d0: 6829 0a20 2020 2020 2020 2073 656c 662e  h).        self.
-0000c0e0: 636d 625f 7361 6d70 6c65 5479 7065 2e63  cmb_sampleType.c
-0000c0f0: 7572 7265 6e74 496e 6465 7843 6861 6e67  urrentIndexChang
-0000c100: 6564 5b27 5153 7472 696e 6727 5d2e 636f  ed['QString'].co
-0000c110: 6e6e 6563 7428 4d61 696e 5769 6e64 6f77  nnect(MainWindow
-0000c120: 2e73 6574 4247 4329 0a20 2020 2020 2020  .setBGC).       
-0000c130: 2073 656c 662e 7370 625f 4e2e 7661 6c75   self.spb_N.valu
-0000c140: 6543 6861 6e67 6564 5b27 696e 7427 5d2e  eChanged['int'].
-0000c150: 636f 6e6e 6563 7428 4d61 696e 5769 6e64  connect(MainWind
-0000c160: 6f77 2e73 6574 4e29 0a20 2020 2020 2020  ow.setN).       
-0000c170: 2073 656c 662e 7370 625f 6d70 7861 2e76   self.spb_mpxa.v
-0000c180: 616c 7565 4368 616e 6765 645b 2769 6e74  alueChanged['int
-0000c190: 275d 2e63 6f6e 6e65 6374 284d 6169 6e57  '].connect(MainW
-0000c1a0: 696e 646f 772e 7365 744d 5041 290a 2020  indow.setMPA).  
-0000c1b0: 2020 2020 2020 7365 6c66 2e62 7574 746f        self.butto
-0000c1c0: 6e5f 4650 532e 636c 6963 6b65 642e 636f  n_FPS.clicked.co
-0000c1d0: 6e6e 6563 7428 4d61 696e 5769 6e64 6f77  nnect(MainWindow
-0000c1e0: 2e73 7461 7274 4546 4129 0a20 2020 2020  .startEFA).     
-0000c1f0: 2020 2073 656c 662e 636d 625f 7363 616c     self.cmb_scal
-0000c200: 6554 7970 652e 6375 7272 656e 7449 6e64  eType.currentInd
-0000c210: 6578 4368 616e 6765 645b 2769 6e74 275d  exChanged['int']
-0000c220: 2e63 6f6e 6e65 6374 284d 6169 6e57 696e  .connect(MainWin
-0000c230: 646f 772e 7365 7453 6361 6c65 5479 7065  dow.setScaleType
-0000c240: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-0000c250: 6578 7442 6f78 5f73 6361 6c65 552e 7465  extBox_scaleU.te
-0000c260: 7874 4564 6974 6564 5b27 5153 7472 696e  xtEdited['QStrin
-0000c270: 6727 5d2e 636f 6e6e 6563 7428 4d61 696e  g'].connect(Main
-0000c280: 5769 6e64 6f77 2e73 6574 5363 616c 6555  Window.setScaleU
-0000c290: 6e69 7429 0a20 2020 2020 2020 2073 656c  nit).        sel
-0000c2a0: 662e 7370 625f 7363 616c 6553 697a 652e  f.spb_scaleSize.
-0000c2b0: 7661 6c75 6543 6861 6e67 6564 5b27 646f  valueChanged['do
-0000c2c0: 7562 6c65 275d 2e63 6f6e 6e65 6374 284d  uble'].connect(M
-0000c2d0: 6169 6e57 696e 646f 772e 7365 7453 6361  ainWindow.setSca
-0000c2e0: 6c65 5661 6c75 6529 0a20 2020 2020 2020  leValue).       
-0000c2f0: 2073 656c 662e 636d 625f 7363 616c 6550   self.cmb_scaleP
-0000c300: 6f73 2e63 7572 7265 6e74 496e 6465 7843  os.currentIndexC
-0000c310: 6861 6e67 6564 5b27 696e 7427 5d2e 636f  hanged['int'].co
-0000c320: 6e6e 6563 7428 4d61 696e 5769 6e64 6f77  nnect(MainWindow
-0000c330: 2e73 6574 5363 616c 6550 6f73 6974 696f  .setScalePositio
-0000c340: 6e29 0a20 2020 2020 2020 2073 656c 662e  n).        self.
-0000c350: 6275 7474 6f6e 5f68 6561 6465 722e 636c  button_header.cl
-0000c360: 6963 6b65 642e 636f 6e6e 6563 7428 4d61  icked.connect(Ma
-0000c370: 696e 5769 6e64 6f77 2e73 6574 4865 6164  inWindow.setHead
-0000c380: 6572 4e61 6d65 290a 2020 2020 2020 2020  erName).        
-0000c390: 7365 6c66 2e62 7574 746f 6e5f 4650 5370  self.button_FPSp
-0000c3a0: 6174 682e 636c 6963 6b65 642e 636f 6e6e  ath.clicked.conn
-0000c3b0: 6563 7428 4d61 696e 5769 6e64 6f77 2e73  ect(MainWindow.s
-0000c3c0: 6574 4650 5350 6174 6829 0a20 2020 2020  etFPSPath).     
-0000c3d0: 2020 2073 656c 662e 6275 7474 6f6e 5f73     self.button_s
-0000c3e0: 6176 6550 4341 7061 7468 2e63 6c69 636b  avePCApath.click
-0000c3f0: 6564 2e63 6f6e 6e65 6374 284d 6169 6e57  ed.connect(MainW
-0000c400: 696e 646f 772e 7365 7453 6176 6550 4341  indow.setSavePCA
-0000c410: 5061 7468 290a 2020 2020 2020 2020 7365  Path).        se
-0000c420: 6c66 2e63 6d62 5f6d 6174 7269 7850 4341  lf.cmb_matrixPCA
-0000c430: 2e63 7572 7265 6e74 496e 6465 7843 6861  .currentIndexCha
-0000c440: 6e67 6564 5b27 696e 7427 5d2e 636f 6e6e  nged['int'].conn
-0000c450: 6563 7428 4d61 696e 5769 6e64 6f77 2e73  ect(MainWindow.s
-0000c460: 6574 5043 416d 6174 7269 7829 0a20 2020  etPCAmatrix).   
-0000c470: 2020 2020 2073 656c 662e 6275 7474 6f6e       self.button
-0000c480: 5f50 4341 2e63 6c69 636b 6564 2e63 6f6e  _PCA.clicked.con
-0000c490: 6e65 6374 284d 6169 6e57 696e 646f 772e  nect(MainWindow.
-0000c4a0: 7374 6172 7450 4341 290a 2020 2020 2020  startPCA).      
-0000c4b0: 2020 7365 6c66 2e63 6d62 5f78 2e63 7572    self.cmb_x.cur
-0000c4c0: 7265 6e74 496e 6465 7843 6861 6e67 6564  rentIndexChanged
-0000c4d0: 5b27 696e 7427 5d2e 636f 6e6e 6563 7428  ['int'].connect(
-0000c4e0: 4d61 696e 5769 6e64 6f77 2e73 6574 5861  MainWindow.setXa
-0000c4f0: 7869 7329 0a20 2020 2020 2020 2073 656c  xis).        sel
-0000c500: 662e 636d 625f 792e 6375 7272 656e 7449  f.cmb_y.currentI
-0000c510: 6e64 6578 4368 616e 6765 645b 2769 6e74  ndexChanged['int
-0000c520: 275d 2e63 6f6e 6e65 6374 284d 6169 6e57  '].connect(MainW
-0000c530: 696e 646f 772e 7365 7459 6178 6973 290a  indow.setYaxis).
-0000c540: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
-0000c550: 5f63 6f6c 6f72 2e63 7572 7265 6e74 496e  _color.currentIn
-0000c560: 6465 7843 6861 6e67 6564 5b27 696e 7427  dexChanged['int'
-0000c570: 5d2e 636f 6e6e 6563 7428 4d61 696e 5769  ].connect(MainWi
-0000c580: 6e64 6f77 2e73 6574 436f 6c6f 7229 0a20  ndow.setColor). 
-0000c590: 2020 2020 2020 2073 656c 662e 7075 7368         self.push
-0000c5a0: 4275 7474 6f6e 2e63 6c69 636b 6564 2e63  Button.clicked.c
-0000c5b0: 6f6e 6e65 6374 284d 6169 6e57 696e 646f  onnect(MainWindo
-0000c5c0: 772e 6772 6170 6844 7261 7729 0a20 2020  w.graphDraw).   
-0000c5d0: 2020 2020 2073 656c 662e 7075 7368 4275       self.pushBu
-0000c5e0: 7474 6f6e 5f32 2e63 6c69 636b 6564 2e63  tton_2.clicked.c
-0000c5f0: 6f6e 6e65 6374 284d 6169 6e57 696e 646f  onnect(MainWindo
-0000c600: 772e 7361 7665 5043 4669 6729 0a20 2020  w.savePCFig).   
-0000c610: 2020 2020 2073 656c 662e 636d 625f 736f       self.cmb_so
-0000c620: 7274 2e63 7572 7265 6e74 496e 6465 7843  rt.currentIndexC
-0000c630: 6861 6e67 6564 5b27 696e 7427 5d2e 636f  hanged['int'].co
-0000c640: 6e6e 6563 7428 4d61 696e 5769 6e64 6f77  nnect(MainWindow
-0000c650: 2e73 6574 536f 7274 290a 2020 2020 2020  .setSort).      
-0000c660: 2020 7365 6c66 2e63 6d62 5f70 6c6f 742e    self.cmb_plot.
-0000c670: 6375 7272 656e 7449 6e64 6578 4368 616e  currentIndexChan
-0000c680: 6765 645b 2769 6e74 275d 2e63 6f6e 6e65  ged['int'].conne
-0000c690: 6374 284d 6169 6e57 696e 646f 772e 7365  ct(MainWindow.se
-0000c6a0: 7450 6c6f 7454 7970 6529 0a20 2020 2020  tPlotType).     
-0000c6b0: 2020 2073 656c 662e 636d 625f 7265 6354     self.cmb_recT
-0000c6c0: 7970 652e 6375 7272 656e 7449 6e64 6578  ype.currentIndex
-0000c6d0: 4368 616e 6765 645b 2769 6e74 275d 2e63  Changed['int'].c
-0000c6e0: 6f6e 6e65 6374 284d 6169 6e57 696e 646f  onnect(MainWindo
-0000c6f0: 772e 7365 7452 6563 6f6e 7374 4d6f 6465  w.setReconstMode
-0000c700: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-0000c710: 6d62 5f73 756d 4465 762e 6375 7272 656e  mb_sumDev.curren
-0000c720: 7449 6e64 6578 4368 616e 6765 645b 2769  tIndexChanged['i
-0000c730: 6e74 275d 2e63 6f6e 6e65 6374 284d 6169  nt'].connect(Mai
-0000c740: 6e57 696e 646f 772e 7365 7453 756d 4465  nWindow.setSumDe
-0000c750: 7629 0a20 2020 2020 2020 2073 656c 662e  v).        self.
-0000c760: 636d 625f 4950 2e63 7572 7265 6e74 496e  cmb_IP.currentIn
-0000c770: 6465 7843 6861 6e67 6564 5b27 696e 7427  dexChanged['int'
-0000c780: 5d2e 636f 6e6e 6563 7428 4d61 696e 5769  ].connect(MainWi
-0000c790: 6e64 6f77 2e73 6574 4950 4361 7869 7329  ndow.setIPCaxis)
-0000c7a0: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
-0000c7b0: 625f 4949 502e 6375 7272 656e 7449 6e64  b_IIP.currentInd
-0000c7c0: 6578 4368 616e 6765 645b 2769 6e74 275d  exChanged['int']
-0000c7d0: 2e63 6f6e 6e65 6374 284d 6169 6e57 696e  .connect(MainWin
-0000c7e0: 646f 772e 7365 7449 4950 4361 7869 7329  dow.setIIPCaxis)
-0000c7f0: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
-0000c800: 625f 4949 4950 2e63 7572 7265 6e74 496e  b_IIIP.currentIn
-0000c810: 6465 7843 6861 6e67 6564 5b27 696e 7427  dexChanged['int'
-0000c820: 5d2e 636f 6e6e 6563 7428 4d61 696e 5769  ].connect(MainWi
-0000c830: 6e64 6f77 2e73 6574 4949 4950 4361 7869  ndow.setIIIPCaxi
-0000c840: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-0000c850: 6473 625f 4964 2e76 616c 7565 4368 616e  dsb_Id.valueChan
-0000c860: 6765 645b 2764 6f75 626c 6527 5d2e 636f  ged['double'].co
-0000c870: 6e6e 6563 7428 4d61 696e 5769 6e64 6f77  nnect(MainWindow
-0000c880: 2e73 6574 4964 6576 290a 2020 2020 2020  .setIdev).      
-0000c890: 2020 7365 6c66 2e64 7362 5f49 4964 2e76    self.dsb_IId.v
-0000c8a0: 616c 7565 4368 616e 6765 645b 2764 6f75  alueChanged['dou
-0000c8b0: 626c 6527 5d2e 636f 6e6e 6563 7428 4d61  ble'].connect(Ma
-0000c8c0: 696e 5769 6e64 6f77 2e73 6574 4949 6465  inWindow.setIIde
-0000c8d0: 7629 0a20 2020 2020 2020 2073 656c 662e  v).        self.
-0000c8e0: 6473 625f 4949 4964 2e76 616c 7565 4368  dsb_IIId.valueCh
-0000c8f0: 616e 6765 645b 2764 6f75 626c 6527 5d2e  anged['double'].
-0000c900: 636f 6e6e 6563 7428 4d61 696e 5769 6e64  connect(MainWind
-0000c910: 6f77 2e73 6574 4949 4964 6576 290a 2020  ow.setIIIdev).  
-0000c920: 2020 2020 2020 7365 6c66 2e62 7574 746f        self.butto
-0000c930: 6e5f 6765 6e65 7261 7465 2e63 6c69 636b  n_generate.click
-0000c940: 6564 2e63 6f6e 6e65 6374 284d 6169 6e57  ed.connect(MainW
-0000c950: 696e 646f 772e 7265 636f 6e73 7447 7261  indow.reconstGra
-0000c960: 7068 290a 2020 2020 2020 2020 7365 6c66  ph).        self
-0000c970: 2e62 7574 746f 6e5f 7361 7665 5265 636f  .button_saveReco
-0000c980: 6e73 742e 636c 6963 6b65 642e 636f 6e6e  nst.clicked.conn
-0000c990: 6563 7428 4d61 696e 5769 6e64 6f77 2e73  ect(MainWindow.s
-0000c9a0: 6176 6552 6563 6f6e 7374 4772 6170 6829  aveReconstGraph)
-0000c9b0: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
-0000c9c0: 625f 4650 532e 6375 7272 656e 7449 6e64  b_FPS.currentInd
-0000c9d0: 6578 4368 616e 6765 645b 2769 6e74 275d  exChanged['int']
-0000c9e0: 2e63 6f6e 6e65 6374 284d 6169 6e57 696e  .connect(MainWin
-0000c9f0: 646f 772e 7365 7446 5053 6f72 4546 4429  dow.setFPSorEFD)
-0000ca00: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
-0000ca10: 625f 7375 6263 6f6c 6f72 2e63 7572 7265  b_subcolor.curre
-0000ca20: 6e74 496e 6465 7843 6861 6e67 6564 5b27  ntIndexChanged['
-0000ca30: 696e 7427 5d2e 636f 6e6e 6563 7428 4d61  int'].connect(Ma
-0000ca40: 696e 5769 6e64 6f77 2e73 6574 5375 6243  inWindow.setSubC
-0000ca50: 6f6c 6f72 290a 2020 2020 2020 2020 7365  olor).        se
-0000ca60: 6c66 2e63 6d62 5f73 7562 736f 7274 2e63  lf.cmb_subsort.c
-0000ca70: 7572 7265 6e74 496e 6465 7843 6861 6e67  urrentIndexChang
-0000ca80: 6564 5b27 696e 7427 5d2e 636f 6e6e 6563  ed['int'].connec
-0000ca90: 7428 4d61 696e 5769 6e64 6f77 2e73 6574  t(MainWindow.set
-0000caa0: 5375 6253 6f72 7429 0a20 2020 2020 2020  SubSort).       
-0000cab0: 2073 656c 662e 636d 625f 7375 6273 7562   self.cmb_subsub
-0000cac0: 636f 6c6f 722e 6375 7272 656e 7449 6e64  color.currentInd
-0000cad0: 6578 4368 616e 6765 645b 2769 6e74 275d  exChanged['int']
-0000cae0: 2e63 6f6e 6e65 6374 284d 6169 6e57 696e  .connect(MainWin
-0000caf0: 646f 772e 7365 7453 7562 7375 6243 6f6c  dow.setSubsubCol
-0000cb00: 6f72 290a 2020 2020 2020 2020 7365 6c66  or).        self
-0000cb10: 2e63 6d62 5f73 7562 7375 6273 6f72 742e  .cmb_subsubsort.
-0000cb20: 6375 7272 656e 7449 6e64 6578 4368 616e  currentIndexChan
-0000cb30: 6765 645b 2769 6e74 275d 2e63 6f6e 6e65  ged['int'].conne
-0000cb40: 6374 284d 6169 6e57 696e 646f 772e 7365  ct(MainWindow.se
-0000cb50: 7453 7562 7375 6253 6f72 7429 0a20 2020  tSubsubSort).   
-0000cb60: 2020 2020 2073 656c 662e 7262 5f6e 6f6e       self.rb_non
-0000cb70: 652e 746f 6767 6c65 645b 2762 6f6f 6c27  e.toggled['bool'
-0000cb80: 5d2e 636f 6e6e 6563 7428 4d61 696e 5769  ].connect(MainWi
-0000cb90: 6e64 6f77 2e73 6574 4361 7465 676f 7269  ndow.setCategori
-0000cba0: 7a65 290a 2020 2020 2020 2020 7365 6c66  ze).        self
-0000cbb0: 2e72 625f 7375 6266 6f6c 6461 2e74 6f67  .rb_subfolda.tog
-0000cbc0: 676c 6564 5b27 626f 6f6c 275d 2e63 6f6e  gled['bool'].con
-0000cbd0: 6e65 6374 284d 6169 6e57 696e 646f 772e  nect(MainWindow.
-0000cbe0: 7365 7443 6174 6567 6f72 697a 6529 0a20  setCategorize). 
-0000cbf0: 2020 2020 2020 2073 656c 662e 7262 5f66         self.rb_f
-0000cc00: 696c 656e 616d 652e 746f 6767 6c65 645b  ilename.toggled[
-0000cc10: 2762 6f6f 6c27 5d2e 636f 6e6e 6563 7428  'bool'].connect(
-0000cc20: 4d61 696e 5769 6e64 6f77 2e73 6574 4361  MainWindow.setCa
-0000cc30: 7465 676f 7269 7a65 290a 2020 2020 2020  tegorize).      
-0000cc40: 2020 7365 6c66 2e62 7574 746f 6e5f 7361    self.button_sa
-0000cc50: 6d70 6c65 2e63 6c69 636b 6564 2e63 6f6e  mple.clicked.con
-0000cc60: 6e65 6374 284d 6169 6e57 696e 646f 772e  nect(MainWindow.
-0000cc70: 7365 7453 616d 706c 6549 6d61 6765 290a  setSampleImage).
-0000cc80: 2020 2020 2020 2020 7365 6c66 2e62 7574          self.but
-0000cc90: 746f 6e5f 7374 6172 7473 616d 706c 652e  ton_startsample.
-0000cca0: 636c 6963 6b65 642e 636f 6e6e 6563 7428  clicked.connect(
-0000ccb0: 4d61 696e 5769 6e64 6f77 2e73 7461 7274  MainWindow.start
-0000ccc0: 506c 6179 6772 6f75 6e64 290a 2020 2020  Playground).    
-0000ccd0: 2020 2020 7365 6c66 2e62 7574 746f 6e5f      self.button_
-0000cce0: 7361 7665 5f73 616d 706c 652e 636c 6963  save_sample.clic
-0000ccf0: 6b65 642e 636f 6e6e 6563 7428 4d61 696e  ked.connect(Main
-0000cd00: 5769 6e64 6f77 2e73 6176 6553 616d 706c  Window.saveSampl
-0000cd10: 6529 0a20 2020 2020 2020 2051 7443 6f72  e).        QtCor
-0000cd20: 652e 514d 6574 614f 626a 6563 742e 636f  e.QMetaObject.co
-0000cd30: 6e6e 6563 7453 6c6f 7473 4279 4e61 6d65  nnectSlotsByName
-0000cd40: 284d 6169 6e57 696e 646f 7729 0a0a 2020  (MainWindow)..  
-0000cd50: 2020 6465 6620 7265 7472 616e 736c 6174    def retranslat
-0000cd60: 6555 6928 7365 6c66 2c20 4d61 696e 5769  eUi(self, MainWi
-0000cd70: 6e64 6f77 293a 0a20 2020 2020 2020 205f  ndow):.        _
-0000cd80: 7472 616e 736c 6174 6520 3d20 5174 436f  translate = QtCo
-0000cd90: 7265 2e51 436f 7265 4170 706c 6963 6174  re.QCoreApplicat
-0000cda0: 696f 6e2e 7472 616e 736c 6174 650a 2020  ion.translate.  
-0000cdb0: 2020 2020 2020 4d61 696e 5769 6e64 6f77        MainWindow
-0000cdc0: 2e73 6574 5769 6e64 6f77 5469 746c 6528  .setWindowTitle(
-0000cdd0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-0000cde0: 5769 6e64 6f77 222c 2022 4d61 696e 5769  Window", "MainWi
-0000cdf0: 6e64 6f77 2229 290a 2020 2020 2020 2020  ndow")).        
-0000ce00: 7365 6c66 2e6c 6162 656c 5f33 372e 7365  self.label_37.se
-0000ce10: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
-0000ce20: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-0000ce30: 5365 6c65 6374 6564 2053 616d 706c 6522  Selected Sample"
-0000ce40: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000ce50: 6c61 6265 6c5f 3335 2e73 6574 5465 7874  label_35.setText
-0000ce60: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-0000ce70: 6e57 696e 646f 7722 2c20 2253 656c 6563  nWindow", "Selec
-0000ce80: 7465 6420 496d 6167 6522 2929 0a20 2020  ted Image")).   
-0000ce90: 2020 2020 2073 656c 662e 7461 6257 6964       self.tabWid
-0000cea0: 6765 745f 322e 7365 7454 6162 5465 7874  get_2.setTabText
-0000ceb0: 2873 656c 662e 7461 6257 6964 6765 745f  (self.tabWidget_
-0000cec0: 322e 696e 6465 784f 6628 7365 6c66 2e74  2.indexOf(self.t
-0000ced0: 6162 5f36 292c 205f 7472 616e 736c 6174  ab_6), _translat
-0000cee0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-0000cef0: 224f 7269 6769 6e61 6c22 2929 0a20 2020  "Original")).   
-0000cf00: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-0000cf10: 3432 2e73 6574 5465 7874 285f 7472 616e  42.setText(_tran
-0000cf20: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-0000cf30: 7722 2c20 2259 2229 290a 2020 2020 2020  w", "Y")).      
-0000cf40: 2020 7365 6c66 2e6c 6162 656c 5f34 352e    self.label_45.
-0000cf50: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-0000cf60: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-0000cf70: 2022 5822 2929 0a20 2020 2020 2020 2073   "X")).        s
-0000cf80: 656c 662e 7461 6257 6964 6765 745f 322e  elf.tabWidget_2.
-0000cf90: 7365 7454 6162 5465 7874 2873 656c 662e  setTabText(self.
-0000cfa0: 7461 6257 6964 6765 745f 322e 696e 6465  tabWidget_2.inde
-0000cfb0: 784f 6628 7365 6c66 2e74 6162 5f39 292c  xOf(self.tab_9),
-0000cfc0: 205f 7472 616e 736c 6174 6528 224d 6169   _translate("Mai
-0000cfd0: 6e57 696e 646f 7722 2c20 2250 726f 6a65  nWindow", "Proje
-0000cfe0: 6374 696f 6e22 2929 0a20 2020 2020 2020  ction")).       
-0000cff0: 2073 656c 662e 6c61 6265 6c5f 3431 2e73   self.label_41.s
-0000d000: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-0000d010: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-0000d020: 2259 2043 6f6f 7264 696e 6174 6522 2929  "Y Coordinate"))
-0000d030: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-0000d040: 6265 6c5f 3430 2e73 6574 5465 7874 285f  bel_40.setText(_
-0000d050: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-0000d060: 696e 646f 7722 2c20 2258 2043 6f6f 7264  indow", "X Coord
-0000d070: 696e 6174 6522 2929 0a20 2020 2020 2020  inate")).       
-0000d080: 2073 656c 662e 7461 6257 6964 6765 745f   self.tabWidget_
-0000d090: 322e 7365 7454 6162 5465 7874 2873 656c  2.setTabText(sel
-0000d0a0: 662e 7461 6257 6964 6765 745f 322e 696e  f.tabWidget_2.in
-0000d0b0: 6465 784f 6628 7365 6c66 2e74 6162 5f37  dexOf(self.tab_7
-0000d0c0: 292c 205f 7472 616e 736c 6174 6528 224d  ), _translate("M
-0000d0d0: 6169 6e57 696e 646f 7722 2c20 2246 6f75  ainWindow", "Fou
-0000d0e0: 7269 6572 2041 7070 726f 7869 6d61 7469  rier Approximati
-0000d0f0: 6f6e 2229 290a 2020 2020 2020 2020 7365  on")).        se
-0000d100: 6c66 2e6c 6162 656c 5f34 342e 7365 7454  lf.label_44.setT
-0000d110: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-0000d120: 4d61 696e 5769 6e64 6f77 222c 2022 436f  MainWindow", "Co
-0000d130: 6d70 6572 6973 6f6e 2229 290a 2020 2020  mperison")).    
-0000d140: 2020 2020 7365 6c66 2e6c 6162 656c 5f34      self.label_4
-0000d150: 332e 7365 7454 6578 7428 5f74 7261 6e73  3.setText(_trans
-0000d160: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-0000d170: 222c 2022 5265 636f 6e73 7472 7563 7465  ", "Reconstructe
-0000d180: 6420 2845 4641 2922 2929 0a20 2020 2020  d (EFA)")).     
-0000d190: 2020 2073 656c 662e 7461 6257 6964 6765     self.tabWidge
-0000d1a0: 745f 322e 7365 7454 6162 5465 7874 2873  t_2.setTabText(s
-0000d1b0: 656c 662e 7461 6257 6964 6765 745f 322e  elf.tabWidget_2.
-0000d1c0: 696e 6465 784f 6628 7365 6c66 2e74 6162  indexOf(self.tab
-0000d1d0: 5f38 292c 205f 7472 616e 736c 6174 6528  _8), _translate(
-0000d1e0: 224d 6169 6e57 696e 646f 7722 2c20 2252  "MainWindow", "R
-0000d1f0: 6563 6f6e 7374 7275 6374 2229 290a 2020  econstruct")).  
-0000d200: 2020 2020 2020 7365 6c66 2e63 625f 4247        self.cb_BG
-0000d210: 435f 7361 6d70 6c65 2e73 6574 4974 656d  C_sample.setItem
-0000d220: 5465 7874 2830 2c20 5f74 7261 6e73 6c61  Text(0, _transla
-0000d230: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-0000d240: 2022 5768 6974 6522 2929 0a20 2020 2020   "White")).     
-0000d250: 2020 2073 656c 662e 6362 5f42 4743 5f73     self.cb_BGC_s
-0000d260: 616d 706c 652e 7365 7449 7465 6d54 6578  ample.setItemTex
-0000d270: 7428 312c 205f 7472 616e 736c 6174 6528  t(1, _translate(
-0000d280: 224d 6169 6e57 696e 646f 7722 2c20 2242  "MainWindow", "B
-0000d290: 6c61 636b 2229 290a 2020 2020 2020 2020  lack")).        
-0000d2a0: 7365 6c66 2e6c 6162 656c 5f33 392e 7365  self.label_39.se
-0000d2b0: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
-0000d2c0: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-0000d2d0: 4261 636b 6772 6f75 6e64 2043 6f6c 6f72  Background Color
-0000d2e0: 206f 6620 496d 6167 6522 2929 0a20 2020   of Image")).   
-0000d2f0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-0000d300: 3334 2e73 6574 5465 7874 285f 7472 616e  34.setText(_tran
-0000d310: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-0000d320: 7722 2c20 2253 656c 6563 7420 5361 6d70  w", "Select Samp
-0000d330: 6c65 206e 756d 6265 7222 2929 0a20 2020  le number")).   
-0000d340: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-0000d350: 3333 2e73 6574 5465 7874 285f 7472 616e  33.setText(_tran
-0000d360: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-0000d370: 7722 2c20 2253 656c 6563 7420 496d 6167  w", "Select Imag
-0000d380: 6522 2929 0a20 2020 2020 2020 2073 656c  e")).        sel
-0000d390: 662e 6275 7474 6f6e 5f73 616d 706c 652e  f.button_sample.
-0000d3a0: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-0000d3b0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-0000d3c0: 2022 4368 6f6f 7365 2229 290a 2020 2020   "Choose")).    
-0000d3d0: 2020 2020 7365 6c66 2e6c 6162 656c 5f33      self.label_3
-0000d3e0: 382e 7365 7454 6578 7428 5f74 7261 6e73  8.setText(_trans
-0000d3f0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-0000d400: 222c 2022 4d61 7869 6d75 6d20 4861 726d  ", "Maximum Harm
-0000d410: 6f6e 6963 7320 4e75 6d62 6572 2229 290a  onics Number")).
-0000d420: 2020 2020 2020 2020 7365 6c66 2e62 7574          self.but
-0000d430: 746f 6e5f 7374 6172 7473 616d 706c 652e  ton_startsample.
-0000d440: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-0000d450: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-0000d460: 2022 5374 6172 7421 2229 290a 2020 2020   "Start!")).    
-0000d470: 2020 2020 7365 6c66 2e62 7574 746f 6e5f      self.button_
-0000d480: 7361 7665 5f73 616d 706c 652e 7365 7454  save_sample.setT
-0000d490: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-0000d4a0: 4d61 696e 5769 6e64 6f77 222c 2022 5361  MainWindow", "Sa
-0000d4b0: 7665 2229 290a 2020 2020 2020 2020 7365  ve")).        se
-0000d4c0: 6c66 2e74 6162 5769 6467 6574 2e73 6574  lf.tabWidget.set
-0000d4d0: 5461 6254 6578 7428 7365 6c66 2e74 6162  TabText(self.tab
-0000d4e0: 5769 6467 6574 2e69 6e64 6578 4f66 2873  Widget.indexOf(s
-0000d4f0: 656c 662e 7461 625f 3529 2c20 5f74 7261  elf.tab_5), _tra
-0000d500: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-0000d510: 6f77 222c 2022 506c 6179 6772 6f75 6e64  ow", "Playground
-0000d520: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-0000d530: 2e62 7574 746f 6e5f 4650 532e 7365 7454  .button_FPS.setT
-0000d540: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-0000d550: 4d61 696e 5769 6e64 6f77 222c 2022 416e  MainWindow", "An
-0000d560: 616c 797a 6522 2929 0a20 2020 2020 2020  alyze")).       
-0000d570: 2073 656c 662e 6c6f 6762 6f78 2e73 6574   self.logbox.set
-0000d580: 4874 6d6c 285f 7472 616e 736c 6174 6528  Html(_translate(
-0000d590: 224d 6169 6e57 696e 646f 7722 2c20 223c  "MainWindow", "<
-0000d5a0: 2144 4f43 5459 5045 2048 544d 4c20 5055  !DOCTYPE HTML PU
-0000d5b0: 424c 4943 205c 222d 2f2f 5733 432f 2f44  BLIC \"-//W3C//D
-0000d5c0: 5444 2048 544d 4c20 342e 302f 2f45 4e5c  TD HTML 4.0//EN\
-0000d5d0: 2220 5c22 6874 7470 3a2f 2f77 7777 2e77  " \"http://www.w
-0000d5e0: 332e 6f72 672f 5452 2f52 4543 2d68 746d  3.org/TR/REC-htm
-0000d5f0: 6c34 302f 7374 7269 6374 2e64 7464 5c22  l40/strict.dtd\"
-0000d600: 3e5c 6e22 0a22 3c68 746d 6c3e 3c68 6561  >\n"."<html><hea
-0000d610: 643e 3c6d 6574 6120 6e61 6d65 3d5c 2271  d><meta name=\"q
-0000d620: 7269 6368 7465 7874 5c22 2063 6f6e 7465  richtext\" conte
-0000d630: 6e74 3d5c 2231 5c22 202f 3e3c 7374 796c  nt=\"1\" /><styl
-0000d640: 6520 7479 7065 3d5c 2274 6578 742f 6373  e type=\"text/cs
-0000d650: 735c 223e 5c6e 220a 2270 2c20 6c69 207b  s\">\n"."p, li {
-0000d660: 2077 6869 7465 2d73 7061 6365 3a20 7072   white-space: pr
-0000d670: 652d 7772 6170 3b20 7d5c 6e22 0a22 3c2f  e-wrap; }\n"."</
-0000d680: 7374 796c 653e 3c2f 6865 6164 3e3c 626f  style></head><bo
-0000d690: 6479 2073 7479 6c65 3d5c 2220 666f 6e74  dy style=\" font
-0000d6a0: 2d66 616d 696c 793a 5c27 2e53 4620 4e53  -family:\'.SF NS
-0000d6b0: 2054 6578 745c 273b 2066 6f6e 742d 7369   Text\'; font-si
-0000d6c0: 7a65 3a31 3370 743b 2066 6f6e 742d 7765  ze:13pt; font-we
-0000d6d0: 6967 6874 3a34 3030 3b20 666f 6e74 2d73  ight:400; font-s
-0000d6e0: 7479 6c65 3a6e 6f72 6d61 6c3b 5c22 3e5c  tyle:normal;\">\
-0000d6f0: 6e22 0a22 3c70 2073 7479 6c65 3d5c 2220  n"."<p style=\" 
-0000d700: 6d61 7267 696e 2d74 6f70 3a30 7078 3b20  margin-top:0px; 
-0000d710: 6d61 7267 696e 2d62 6f74 746f 6d3a 3070  margin-bottom:0p
-0000d720: 783b 206d 6172 6769 6e2d 6c65 6674 3a30  x; margin-left:0
-0000d730: 7078 3b20 6d61 7267 696e 2d72 6967 6874  px; margin-right
-0000d740: 3a30 7078 3b20 2d71 742d 626c 6f63 6b2d  :0px; -qt-block-
-0000d750: 696e 6465 6e74 3a30 3b20 7465 7874 2d69  indent:0; text-i
-0000d760: 6e64 656e 743a 3070 783b 5c22 3e3c 7370  ndent:0px;\"><sp
-0000d770: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
-0000d780: 2d77 6569 6768 743a 3630 303b 2074 6578  -weight:600; tex
-0000d790: 742d 6465 636f 7261 7469 6f6e 3a20 756e  t-decoration: un
-0000d7a0: 6465 726c 696e 653b 5c22 3e49 6d61 6765  derline;\">Image
-0000d7b0: 2041 6e61 6c79 7369 733c 2f73 7061 6e3e   Analysis</span>
-0000d7c0: 3c2f 703e 5c6e 220a 223c 7020 7374 796c  </p>\n"."<p styl
-0000d7d0: 653d 5c22 2d71 742d 7061 7261 6772 6170  e=\"-qt-paragrap
-0000d7e0: 682d 7479 7065 3a65 6d70 7479 3b20 6d61  h-type:empty; ma
-0000d7f0: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
-0000d800: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
-0000d810: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
-0000d820: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
-0000d830: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
-0000d840: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
-0000d850: 656e 743a 3070 783b 2066 6f6e 742d 7765  ent:0px; font-we
-0000d860: 6967 6874 3a36 3030 3b20 7465 7874 2d64  ight:600; text-d
-0000d870: 6563 6f72 6174 696f 6e3a 2075 6e64 6572  ecoration: under
-0000d880: 6c69 6e65 3b5c 223e 3c62 7220 2f3e 3c2f  line;\"><br /></
-0000d890: 703e 5c6e 220a 223c 7020 7374 796c 653d  p>\n"."<p style=
-0000d8a0: 5c22 206d 6172 6769 6e2d 746f 703a 3070  \" margin-top:0p
-0000d8b0: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
-0000d8c0: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
-0000d8d0: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
-0000d8e0: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
-0000d8f0: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
-0000d900: 742d 696e 6465 6e74 3a30 7078 3b5c 223e  t-indent:0px;\">
-0000d910: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
-0000d920: 6f6e 742d 7765 6967 6874 3a36 3030 3b5c  ont-weight:600;\
-0000d930: 223e 5768 6174 2079 6f75 2063 616e 2064  ">What you can d
-0000d940: 6f20 6865 7265 2069 7320 746f 2065 7874  o here is to ext
-0000d950: 7261 6374 2070 6172 616d 6574 6572 7320  ract parameters 
-0000d960: 6f66 2046 6f75 7269 6572 2073 6572 6965  of Fourier serie
-0000d970: 7320 616e 6420 6f74 6865 7220 6261 7369  s and other basi
-0000d980: 6320 7368 6170 6520 7061 7261 6d65 7465  c shape paramete
-0000d990: 7273 2066 726f 6d20 796f 7572 2064 6174  rs from your dat
-0000d9a0: 6173 6574 2e3c 2f73 7061 6e3e 3c2f 703e  aset.</span></p>
-0000d9b0: 5c6e 220a 223c 7020 7374 796c 653d 5c22  \n"."<p style=\"
-0000d9c0: 206d 6172 6769 6e2d 746f 703a 3070 783b   margin-top:0px;
-0000d9d0: 206d 6172 6769 6e2d 626f 7474 6f6d 3a30   margin-bottom:0
-0000d9e0: 7078 3b20 6d61 7267 696e 2d6c 6566 743a  px; margin-left:
-0000d9f0: 3070 783b 206d 6172 6769 6e2d 7269 6768  0px; margin-righ
-0000da00: 743a 3070 783b 202d 7174 2d62 6c6f 636b  t:0px; -qt-block
-0000da10: 2d69 6e64 656e 743a 303b 2074 6578 742d  -indent:0; text-
-0000da20: 696e 6465 6e74 3a30 7078 3b5c 223e 4166  indent:0px;\">Af
-0000da30: 7465 7220 7468 6520 616e 616c 7973 6973  ter the analysis
-0000da40: 2c20 7468 6520 7265 7375 6c74 7320 7769  , the results wi
-0000da50: 6c6c 2062 6520 7361 7665 6420 6173 2026  ll be saved as &
-0000da60: 7175 6f74 3b3c 7370 616e 2073 7479 6c65  quot;<span style
-0000da70: 3d5c 2220 636f 6c6f 723a 2330 3030 3030  =\" color:#00000
-0000da80: 303b 5c22 3e46 5053 2e63 7376 3c2f 7370  0;\">FPS.csv</sp
-0000da90: 616e 3e26 7175 6f74 3b2e 3c2f 703e 5c6e  an>&quot;.</p>\n
-0000daa0: 220a 223c 7020 7374 796c 653d 5c22 206d  "."<p style=\" m
-0000dab0: 6172 6769 6e2d 746f 703a 3070 783b 206d  argin-top:0px; m
-0000dac0: 6172 6769 6e2d 626f 7474 6f6d 3a30 7078  argin-bottom:0px
-0000dad0: 3b20 6d61 7267 696e 2d6c 6566 743a 3070  ; margin-left:0p
-0000dae0: 783b 206d 6172 6769 6e2d 7269 6768 743a  x; margin-right:
-0000daf0: 3070 783b 202d 7174 2d62 6c6f 636b 2d69  0px; -qt-block-i
-0000db00: 6e64 656e 743a 303b 2074 6578 742d 696e  ndent:0; text-in
-0000db10: 6465 6e74 3a30 7078 3b5c 223e 3c73 7061  dent:0px;\"><spa
-0000db20: 6e20 7374 796c 653d 5c22 2074 6578 742d  n style=\" text-
-0000db30: 6465 636f 7261 7469 6f6e 3a20 756e 6465  decoration: unde
-0000db40: 726c 696e 653b 5c22 3e50 7269 6e63 6970  rline;\">Princip
-0000db50: 616c 2043 6f6d 706f 6e65 6e74 2041 6e61  al Component Ana
-0000db60: 6c79 7369 733c 2f73 7061 6e3e 2028 3c73  lysis</span> (<s
-0000db70: 7061 6e20 7374 796c 653d 5c22 2063 6f6c  pan style=\" col
-0000db80: 6f72 3a23 3030 3030 3030 3b5c 223e 5043  or:#000000;\">PC
-0000db90: 413c 2f73 7061 6e3e 2920 7769 6c6c 2062  A</span>) will b
-0000dba0: 6520 6865 6c64 2061 7420 6e65 7874 2074  e held at next t
-0000dbb0: 7562 2061 6e64 2069 7420 6973 2062 6173  ub and it is bas
-0000dbc0: 6564 206f 6e20 7468 6520 6f75 7470 7574  ed on the output
-0000dbd0: 2043 5356 2066 696c 6520 5c27 3c73 7061   CSV file \'<spa
-0000dbe0: 6e20 7374 796c 653d 5c22 2063 6f6c 6f72  n style=\" color
-0000dbf0: 3a23 3030 3030 3030 3b5c 223e 4650 532e  :#000000;\">FPS.
-0000dc00: 6373 763c 2f73 7061 6e3e 5c27 2e3c 2f70  csv</span>\'.</p
-0000dc10: 3e5c 6e22 0a22 3c70 2073 7479 6c65 3d5c  >\n"."<p style=\
-0000dc20: 222d 7174 2d70 6172 6167 7261 7068 2d74  "-qt-paragraph-t
-0000dc30: 7970 653a 656d 7074 793b 206d 6172 6769  ype:empty; margi
-0000dc40: 6e2d 746f 703a 3070 783b 206d 6172 6769  n-top:0px; margi
-0000dc50: 6e2d 626f 7474 6f6d 3a30 7078 3b20 6d61  n-bottom:0px; ma
-0000dc60: 7267 696e 2d6c 6566 743a 3070 783b 206d  rgin-left:0px; m
-0000dc70: 6172 6769 6e2d 7269 6768 743a 3070 783b  argin-right:0px;
-0000dc80: 202d 7174 2d62 6c6f 636b 2d69 6e64 656e   -qt-block-inden
-0000dc90: 743a 303b 2074 6578 742d 696e 6465 6e74  t:0; text-indent
-0000dca0: 3a30 7078 3b5c 223e 3c62 7220 2f3e 3c2f  :0px;\"><br /></
-0000dcb0: 703e 5c6e 220a 223c 7020 7374 796c 653d  p>\n"."<p style=
-0000dcc0: 5c22 206d 6172 6769 6e2d 746f 703a 3070  \" margin-top:0p
-0000dcd0: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
-0000dce0: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
-0000dcf0: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
-0000dd00: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
-0000dd10: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
-0000dd20: 742d 696e 6465 6e74 3a30 7078 3b5c 223e  t-indent:0px;\">
-0000dd30: 3c73 7061 6e20 7374 796c 653d 5c22 2074  <span style=\" t
-0000dd40: 6578 742d 6465 636f 7261 7469 6f6e 3a20  ext-decoration: 
-0000dd50: 756e 6465 726c 696e 653b 5c22 3e42 7269  underline;\">Bri
-0000dd60: 6566 2055 7361 6765 3c2f 7370 616e 3e3c  ef Usage</span><
-0000dd70: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
-0000dd80: 3d5c 222d 7174 2d70 6172 6167 7261 7068  =\"-qt-paragraph
-0000dd90: 2d74 7970 653a 656d 7074 793b 206d 6172  -type:empty; mar
-0000dda0: 6769 6e2d 746f 703a 3070 783b 206d 6172  gin-top:0px; mar
-0000ddb0: 6769 6e2d 626f 7474 6f6d 3a30 7078 3b20  gin-bottom:0px; 
-0000ddc0: 6d61 7267 696e 2d6c 6566 743a 3070 783b  margin-left:0px;
-0000ddd0: 206d 6172 6769 6e2d 7269 6768 743a 3070   margin-right:0p
-0000dde0: 783b 202d 7174 2d62 6c6f 636b 2d69 6e64  x; -qt-block-ind
-0000ddf0: 656e 743a 303b 2074 6578 742d 696e 6465  ent:0; text-inde
-0000de00: 6e74 3a30 7078 3b20 7465 7874 2d64 6563  nt:0px; text-dec
-0000de10: 6f72 6174 696f 6e3a 2075 6e64 6572 6c69  oration: underli
-0000de20: 6e65 3b5c 223e 3c62 7220 2f3e 3c2f 703e  ne;\"><br /></p>
-0000de30: 5c6e 220a 223c 7020 7374 796c 653d 5c22  \n"."<p style=\"
-0000de40: 206d 6172 6769 6e2d 746f 703a 3070 783b   margin-top:0px;
-0000de50: 206d 6172 6769 6e2d 626f 7474 6f6d 3a30   margin-bottom:0
-0000de60: 7078 3b20 6d61 7267 696e 2d6c 6566 743a  px; margin-left:
-0000de70: 3070 783b 206d 6172 6769 6e2d 7269 6768  0px; margin-righ
-0000de80: 743a 3070 783b 202d 7174 2d62 6c6f 636b  t:0px; -qt-block
-0000de90: 2d69 6e64 656e 743a 303b 2074 6578 742d  -indent:0; text-
-0000dea0: 696e 6465 6e74 3a30 7078 3b5c 223e 312e  indent:0px;\">1.
-0000deb0: 2053 656c 6563 7420 796f 7572 2066 696c   Select your fil
-0000dec0: 6520 666f 726d 6174 206f 6620 696d 6167  e format of imag
-0000ded0: 6520 6669 6c65 732e 3c2f 703e 5c6e 220a  e files.</p>\n".
-0000dee0: 223c 7020 7374 796c 653d 5c22 206d 6172  "<p style=\" mar
-0000def0: 6769 6e2d 746f 703a 3070 783b 206d 6172  gin-top:0px; mar
-0000df00: 6769 6e2d 626f 7474 6f6d 3a30 7078 3b20  gin-bottom:0px; 
-0000df10: 6d61 7267 696e 2d6c 6566 743a 3070 783b  margin-left:0px;
-0000df20: 206d 6172 6769 6e2d 7269 6768 743a 3070   margin-right:0p
-0000df30: 783b 202d 7174 2d62 6c6f 636b 2d69 6e64  x; -qt-block-ind
-0000df40: 656e 743a 303b 2074 6578 742d 696e 6465  ent:0; text-inde
-0000df50: 6e74 3a30 7078 3b5c 223e 322e 2043 686f  nt:0px;\">2. Cho
-0000df60: 6f73 6520 7468 6520 6d65 7468 6f64 2066  ose the method f
-0000df70: 6f72 2063 6174 6567 6f72 697a 6174 696f  or categorizatio
-0000df80: 6e3c 2f70 3e5c 6e22 0a22 3c70 2073 7479  n</p>\n"."<p sty
-0000df90: 6c65 3d5c 2220 6d61 7267 696e 2d74 6f70  le=\" margin-top
-0000dfa0: 3a30 7078 3b20 6d61 7267 696e 2d62 6f74  :0px; margin-bot
-0000dfb0: 746f 6d3a 3070 783b 206d 6172 6769 6e2d  tom:0px; margin-
-0000dfc0: 6c65 6674 3a30 7078 3b20 6d61 7267 696e  left:0px; margin
-0000dfd0: 2d72 6967 6874 3a30 7078 3b20 2d71 742d  -right:0px; -qt-
-0000dfe0: 626c 6f63 6b2d 696e 6465 6e74 3a30 3b20  block-indent:0; 
-0000dff0: 7465 7874 2d69 6e64 656e 743a 3070 783b  text-indent:0px;
-0000e000: 5c22 3e33 2e20 5365 6c65 6374 2074 6865  \">3. Select the
-0000e010: 2066 6f6c 6461 2069 6e20 7768 6963 6820   folda in which 
-0000e020: 616c 6c20 796f 7572 2069 6d61 6765 2066  all your image f
-0000e030: 696c 6573 2063 6f6e 7461 696e 733c 2f70  iles contains</p
-0000e040: 3e5c 6e22 0a22 3c70 2073 7479 6c65 3d5c  >\n"."<p style=\
-0000e050: 2220 6d61 7267 696e 2d74 6f70 3a30 7078  " margin-top:0px
-0000e060: 3b20 6d61 7267 696e 2d62 6f74 746f 6d3a  ; margin-bottom:
-0000e070: 3070 783b 206d 6172 6769 6e2d 6c65 6674  0px; margin-left
-0000e080: 3a30 7078 3b20 6d61 7267 696e 2d72 6967  :0px; margin-rig
-0000e090: 6874 3a30 7078 3b20 2d71 742d 626c 6f63  ht:0px; -qt-bloc
-0000e0a0: 6b2d 696e 6465 6e74 3a30 3b20 7465 7874  k-indent:0; text
-0000e0b0: 2d69 6e64 656e 743a 3070 783b 5c22 3e34  -indent:0px;\">4
-0000e0c0: 2e20 4966 2079 6f75 2061 7265 2067 6f69  . If you are goi
-0000e0d0: 6e67 2074 6f20 6361 7465 676f 7269 7a65  ng to categorize
-0000e0e0: 2079 6f75 7220 6461 7461 2062 6173 6564   your data based
-0000e0f0: 206f 6e20 7375 6266 6f6c 6461 206f 7220   on subfolda or 
-0000e100: 6669 6c65 6e61 6d65 732c 2061 7373 6967  filenames, assig
-0000e110: 6e20 6561 6368 2063 6174 6567 6f72 7920  n each category 
-0000e120: 636c 6173 732e 3c2f 703e 5c6e 220a 223c  class.</p>\n"."<
-0000e130: 7020 7374 796c 653d 5c22 206d 6172 6769  p style=\" margi
-0000e140: 6e2d 746f 703a 3070 783b 206d 6172 6769  n-top:0px; margi
-0000e150: 6e2d 626f 7474 6f6d 3a30 7078 3b20 6d61  n-bottom:0px; ma
-0000e160: 7267 696e 2d6c 6566 743a 3070 783b 206d  rgin-left:0px; m
-0000e170: 6172 6769 6e2d 7269 6768 743a 3070 783b  argin-right:0px;
-0000e180: 202d 7174 2d62 6c6f 636b 2d69 6e64 656e   -qt-block-inden
-0000e190: 743a 303b 2074 6578 742d 696e 6465 6e74  t:0; text-indent
-0000e1a0: 3a30 7078 3b5c 223e 2020 203c 7370 616e  :0px;\">   <span
-0000e1b0: 2073 7479 6c65 3d5c 2220 666f 6e74 2d77   style=\" font-w
-0000e1c0: 6569 6768 743a 3630 303b 5c22 3e4e 4f54  eight:600;\">NOT
-0000e1d0: 453a 3c2f 7370 616e 3e20 3c73 7061 6e20  E:</span> <span 
-0000e1e0: 7374 796c 653d 5c22 2066 6f6e 742d 7765  style=\" font-we
-0000e1f0: 6967 6874 3a36 3030 3b5c 223e 796f 7520  ight:600;\">you 
-0000e200: 6d75 7374 2064 6576 6964 6564 2065 6163  must devided eac
-0000e210: 6820 6361 7465 676f 7279 206e 616d 6520  h category name 
-0000e220: 6279 2075 7369 6e67 2075 6e64 6572 6261  by using underba
-0000e230: 7220 5c27 5f5c 273c 2f73 7061 6e3e 3c2f  r \'_\'</span></
-0000e240: 703e 5c6e 220a 223c 7020 7374 796c 653d  p>\n"."<p style=
-0000e250: 5c22 206d 6172 6769 6e2d 746f 703a 3070  \" margin-top:0p
-0000e260: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
-0000e270: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
-0000e280: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
-0000e290: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
-0000e2a0: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
-0000e2b0: 742d 696e 6465 6e74 3a30 7078 3b5c 223e  t-indent:0px;\">
-0000e2c0: 466f 7220 6578 616d 706c 652c 2079 6f75  For example, you
-0000e2d0: 7220 666f 6c64 6120 6469 7265 6374 6f72  r folda director
-0000e2e0: 7920 6973 206c 696b 653c 2f70 3e5c 6e22  y is like</p>\n"
-0000e2f0: 0a22 3c70 2073 7479 6c65 3d5c 2220 6d61  ."<p style=\" ma
-0000e300: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
-0000e310: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
-0000e320: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
-0000e330: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
-0000e340: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
-0000e350: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
-0000e360: 656e 743a 3070 783b 5c22 3e44 6174 6120  ent:0px;\">Data 
-0000e370: 2d2d 2d20 5459 5045 5f41 202d 2d20 4e6f  --- TYPE_A -- No
-0000e380: 3120 2d2d 2d20 7361 6d70 6c65 5f30 3031  1 --- sample_001
-0000e390: 2e70 6e67 3c2f 703e 5c6e 220a 223c 7020  .png</p>\n"."<p 
-0000e3a0: 7374 796c 653d 5c22 206d 6172 6769 6e2d  style=\" margin-
-0000e3b0: 746f 703a 3070 783b 206d 6172 6769 6e2d  top:0px; margin-
-0000e3c0: 626f 7474 6f6d 3a30 7078 3b20 6d61 7267  bottom:0px; marg
-0000e3d0: 696e 2d6c 6566 743a 3070 783b 206d 6172  in-left:0px; mar
-0000e3e0: 6769 6e2d 7269 6768 743a 3070 783b 202d  gin-right:0px; -
-0000e3f0: 7174 2d62 6c6f 636b 2d69 6e64 656e 743a  qt-block-indent:
-0000e400: 303b 2074 6578 742d 696e 6465 6e74 3a30  0; text-indent:0
-0000e410: 7078 3b5c 223e 2020 2020 2020 2020 2020  px;\">          
-0000e420: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0000e430: 2020 2020 202d 204e 6f32 202d 2d2d 2073       - No2 --- s
-0000e440: 616d 706c 655f 3030 322e 706e 673c 2f70  ample_002.png</p
-0000e450: 3e5c 6e22 0a22 3c70 2073 7479 6c65 3d5c  >\n"."<p style=\
-0000e460: 2220 6d61 7267 696e 2d74 6f70 3a30 7078  " margin-top:0px
-0000e470: 3b20 6d61 7267 696e 2d62 6f74 746f 6d3a  ; margin-bottom:
-0000e480: 3070 783b 206d 6172 6769 6e2d 6c65 6674  0px; margin-left
-0000e490: 3a30 7078 3b20 6d61 7267 696e 2d72 6967  :0px; margin-rig
-0000e4a0: 6874 3a30 7078 3b20 2d71 742d 626c 6f63  ht:0px; -qt-bloc
-0000e4b0: 6b2d 696e 6465 6e74 3a30 3b20 7465 7874  k-indent:0; text
-0000e4c0: 2d69 6e64 656e 743a 3070 783b 5c22 3e20  -indent:0px;\"> 
-0000e4d0: 2020 2020 2020 2020 2020 2d2d 2054 5950            -- TYP
-0000e4e0: 455f 4220 2d2d 204e 6f32 202d 2d2d 2073  E_B -- No2 --- s
-0000e4f0: 616d 706c 655f 3030 332e 706e 673c 2f70  ample_003.png</p
-0000e500: 3e5c 6e22 0a22 3c70 2073 7479 6c65 3d5c  >\n"."<p style=\
-0000e510: 2220 6d61 7267 696e 2d74 6f70 3a30 7078  " margin-top:0px
-0000e520: 3b20 6d61 7267 696e 2d62 6f74 746f 6d3a  ; margin-bottom:
-0000e530: 3070 783b 206d 6172 6769 6e2d 6c65 6674  0px; margin-left
-0000e540: 3a30 7078 3b20 6d61 7267 696e 2d72 6967  :0px; margin-rig
-0000e550: 6874 3a30 7078 3b20 2d71 742d 626c 6f63  ht:0px; -qt-bloc
-0000e560: 6b2d 696e 6465 6e74 3a30 3b20 7465 7874  k-indent:0; text
-0000e570: 2d69 6e64 656e 743a 3070 783b 5c22 3e20  -indent:0px;\"> 
-0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e590: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000e5a0: 2020 2020 2020 2020 2020 2d2d 2073 616d            -- sam
-0000e5b0: 706c 655f 3030 342e 706e 673c 2f70 3e5c  ple_004.png</p>\
-0000e5c0: 6e22 0a22 3c70 2073 7479 6c65 3d5c 2220  n"."<p style=\" 
-0000e5d0: 6d61 7267 696e 2d74 6f70 3a30 7078 3b20  margin-top:0px; 
-0000e5e0: 6d61 7267 696e 2d62 6f74 746f 6d3a 3070  margin-bottom:0p
-0000e5f0: 783b 206d 6172 6769 6e2d 6c65 6674 3a30  x; margin-left:0
-0000e600: 7078 3b20 6d61 7267 696e 2d72 6967 6874  px; margin-right
-0000e610: 3a30 7078 3b20 2d71 742d 626c 6f63 6b2d  :0px; -qt-block-
-0000e620: 696e 6465 6e74 3a30 3b20 7465 7874 2d69  indent:0; text-i
-0000e630: 6e64 656e 743a 3070 783b 5c22 3e20 2020  ndent:0px;\">   
-0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e650: 2020 2020 2020 2020 2020 2020 202d 204e               - N
-0000e660: 6f33 202d 2d2d 2073 616d 706c 655f 3030  o3 --- sample_00
-0000e670: 352e 706e 673c 2f70 3e5c 6e22 0a22 3c70  5.png</p>\n"."<p
-0000e680: 2073 7479 6c65 3d5c 2220 6d61 7267 696e   style=\" margin
-0000e690: 2d74 6f70 3a30 7078 3b20 6d61 7267 696e  -top:0px; margin
-0000e6a0: 2d62 6f74 746f 6d3a 3070 783b 206d 6172  -bottom:0px; mar
-0000e6b0: 6769 6e2d 6c65 6674 3a30 7078 3b20 6d61  gin-left:0px; ma
-0000e6c0: 7267 696e 2d72 6967 6874 3a30 7078 3b20  rgin-right:0px; 
-0000e6d0: 2d71 742d 626c 6f63 6b2d 696e 6465 6e74  -qt-block-indent
-0000e6e0: 3a30 3b20 7465 7874 2d69 6e64 656e 743a  :0; text-indent:
-0000e6f0: 3070 783b 5c22 3e74 6865 6e2c 2079 6f75  0px;\">then, you
-0000e700: 2073 686f 756c 6420 7075 742c 2066 6f72   should put, for
-0000e710: 2069 6e73 7461 6e63 652c 205c 2754 5950   instance, \'TYP
-0000e720: 455f 4e75 6d62 6572 5f73 616d 706c 655c  E_Number_sample\
-0000e730: 2720 696e 746f 2074 6865 2074 6578 7462  ' into the textb
-0000e740: 6f78 206f 6620 6361 7465 676f 7279 2063  ox of category c
-0000e750: 6c61 7373 2e3c 2f70 3e5c 6e22 0a22 3c70  lass.</p>\n"."<p
-0000e760: 2073 7479 6c65 3d5c 2220 6d61 7267 696e   style=\" margin
-0000e770: 2d74 6f70 3a30 7078 3b20 6d61 7267 696e  -top:0px; margin
-0000e780: 2d62 6f74 746f 6d3a 3070 783b 206d 6172  -bottom:0px; mar
-0000e790: 6769 6e2d 6c65 6674 3a30 7078 3b20 6d61  gin-left:0px; ma
-0000e7a0: 7267 696e 2d72 6967 6874 3a30 7078 3b20  rgin-right:0px; 
-0000e7b0: 2d71 742d 626c 6f63 6b2d 696e 6465 6e74  -qt-block-indent
-0000e7c0: 3a30 3b20 7465 7874 2d69 6e64 656e 743a  :0; text-indent:
-0000e7d0: 3070 783b 5c22 3e54 6865 6e2c 2074 6865  0px;\">Then, the
-0000e7e0: 2068 6561 6465 7220 726f 7720 6f66 2065   header row of e
-0000e7f0: 7870 6f72 7465 6420 6373 7620 6669 6c65  xported csv file
-0000e800: 2077 696c 6c20 6265 2061 7574 6f6d 6174   will be automat
-0000e810: 6963 616c 6c79 2061 7373 6967 6e65 6420  ically assigned 
-0000e820: 6261 7365 6420 6f6e 2074 6865 7365 2063  based on these c
-0000e830: 6174 6567 6f72 7920 6e61 6d65 732e 3c2f  ategory names.</
-0000e840: 703e 5c6e 220a 223c 7020 7374 796c 653d  p>\n"."<p style=
-0000e850: 5c22 2d71 742d 7061 7261 6772 6170 682d  \"-qt-paragraph-
-0000e860: 7479 7065 3a65 6d70 7479 3b20 6d61 7267  type:empty; marg
-0000e870: 696e 2d74 6f70 3a30 7078 3b20 6d61 7267  in-top:0px; marg
-0000e880: 696e 2d62 6f74 746f 6d3a 3070 783b 206d  in-bottom:0px; m
-0000e890: 6172 6769 6e2d 6c65 6674 3a30 7078 3b20  argin-left:0px; 
-0000e8a0: 6d61 7267 696e 2d72 6967 6874 3a30 7078  margin-right:0px
-0000e8b0: 3b20 2d71 742d 626c 6f63 6b2d 696e 6465  ; -qt-block-inde
-0000e8c0: 6e74 3a30 3b20 7465 7874 2d69 6e64 656e  nt:0; text-inden
-0000e8d0: 743a 3070 783b 5c22 3e3c 6272 202f 3e3c  t:0px;\"><br /><
-0000e8e0: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
-0000e8f0: 3d5c 2220 6d61 7267 696e 2d74 6f70 3a30  =\" margin-top:0
-0000e900: 7078 3b20 6d61 7267 696e 2d62 6f74 746f  px; margin-botto
-0000e910: 6d3a 3070 783b 206d 6172 6769 6e2d 6c65  m:0px; margin-le
-0000e920: 6674 3a30 7078 3b20 6d61 7267 696e 2d72  ft:0px; margin-r
-0000e930: 6967 6874 3a30 7078 3b20 2d71 742d 626c  ight:0px; -qt-bl
-0000e940: 6f63 6b2d 696e 6465 6e74 3a30 3b20 7465  ock-indent:0; te
-0000e950: 7874 2d69 6e64 656e 743a 3070 783b 5c22  xt-indent:0px;\"
-0000e960: 3e35 2e20 5365 6c65 6374 2074 6865 2066  >5. Select the f
-0000e970: 6f6c 6461 2069 6e20 7768 6963 6820 7468  olda in which th
-0000e980: 6520 7265 7375 6c74 616e 7420 4353 5620  e resultant CSV 
-0000e990: 6669 6c65 2069 7320 746f 2073 6176 652e  file is to save.
-0000e9a0: 3c2f 703e 5c6e 220a 223c 7020 7374 796c  </p>\n"."<p styl
-0000e9b0: 653d 5c22 206d 6172 6769 6e2d 746f 703a  e=\" margin-top:
-0000e9c0: 3070 783b 206d 6172 6769 6e2d 626f 7474  0px; margin-bott
-0000e9d0: 6f6d 3a30 7078 3b20 6d61 7267 696e 2d6c  om:0px; margin-l
-0000e9e0: 6566 743a 3070 783b 206d 6172 6769 6e2d  eft:0px; margin-
-0000e9f0: 7269 6768 743a 3070 783b 202d 7174 2d62  right:0px; -qt-b
-0000ea00: 6c6f 636b 2d69 6e64 656e 743a 303b 2074  lock-indent:0; t
-0000ea10: 6578 742d 696e 6465 6e74 3a30 7078 3b5c  ext-indent:0px;\
-0000ea20: 223e 362e 2053 6574 2074 6865 2062 6163  ">6. Set the bac
-0000ea30: 6b67 726f 756e 6420 636f 6c6f 7220 2869  kground color (i
-0000ea40: 6620 7768 6963 6820 6973 2077 726f 6e67  f which is wrong
-0000ea50: 6c79 2063 686f 6f73 6564 2c20 7468 6520  ly choosed, the 
-0000ea60: 6461 7461 2067 6f65 7320 7772 6f6e 6729  data goes wrong)
-0000ea70: 2e3c 2f70 3e5c 6e22 0a22 3c70 2073 7479  .</p>\n"."<p sty
-0000ea80: 6c65 3d5c 2220 6d61 7267 696e 2d74 6f70  le=\" margin-top
-0000ea90: 3a30 7078 3b20 6d61 7267 696e 2d62 6f74  :0px; margin-bot
-0000eaa0: 746f 6d3a 3070 783b 206d 6172 6769 6e2d  tom:0px; margin-
-0000eab0: 6c65 6674 3a30 7078 3b20 6d61 7267 696e  left:0px; margin
-0000eac0: 2d72 6967 6874 3a30 7078 3b20 2d71 742d  -right:0px; -qt-
-0000ead0: 626c 6f63 6b2d 696e 6465 6e74 3a30 3b20  block-indent:0; 
-0000eae0: 7465 7874 2d69 6e64 656e 743a 3070 783b  text-indent:0px;
-0000eaf0: 5c22 3e37 2e20 5365 6c65 6374 2074 6865  \">7. Select the
-0000eb00: 204d 6178 696d 756d 2048 6172 6d6f 6e69   Maximum Harmoni
-0000eb10: 6373 206e 756d 6265 722e 3c2f 703e 5c6e  cs number.</p>\n
-0000eb20: 220a 223c 7020 7374 796c 653d 5c22 206d  "."<p style=\" m
-0000eb30: 6172 6769 6e2d 746f 703a 3070 783b 206d  argin-top:0px; m
-0000eb40: 6172 6769 6e2d 626f 7474 6f6d 3a30 7078  argin-bottom:0px
-0000eb50: 3b20 6d61 7267 696e 2d6c 6566 743a 3070  ; margin-left:0p
-0000eb60: 783b 206d 6172 6769 6e2d 7269 6768 743a  x; margin-right:
-0000eb70: 3070 783b 202d 7174 2d62 6c6f 636b 2d69  0px; -qt-block-i
-0000eb80: 6e64 656e 743a 303b 2074 6578 742d 696e  ndent:0; text-in
-0000eb90: 6465 6e74 3a30 7078 3b5c 223e 2020 5768  dent:0px;\">  Wh
-0000eba0: 6174 2069 7320 6d61 7869 6d75 6d20 6861  at is maximum ha
-0000ebb0: 726d 6f6e 6963 7320 6e75 6d62 6572 2028  rmonics number (
-0000ebc0: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
-0000ebd0: 6f6e 742d 7374 796c 653a 6974 616c 6963  ont-style:italic
-0000ebe0: 3b5c 223e 4e3c 2f73 7061 6e3e 293f 2059  ;\">N</span>)? Y
-0000ebf0: 6f75 2063 616e 2063 6865 636b 2068 6f77  ou can check how
-0000ec00: 2074 6869 7320 6e75 6d62 6572 2061 6666   this number aff
-0000ec10: 6563 7473 2074 6865 2072 6573 756c 7473  ects the results
-0000ec20: 2061 7420 2671 756f 743b 506c 6179 6772   at &quot;Playgr
-0000ec30: 6f75 6e64 2671 756f 743b 2074 6162 2e3c  ound&quot; tab.<
-0000ec40: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
-0000ec50: 3d5c 2220 6d61 7267 696e 2d74 6f70 3a30  =\" margin-top:0
-0000ec60: 7078 3b20 6d61 7267 696e 2d62 6f74 746f  px; margin-botto
-0000ec70: 6d3a 3070 783b 206d 6172 6769 6e2d 6c65  m:0px; margin-le
-0000ec80: 6674 3a30 7078 3b20 6d61 7267 696e 2d72  ft:0px; margin-r
-0000ec90: 6967 6874 3a30 7078 3b20 2d71 742d 626c  ight:0px; -qt-bl
-0000eca0: 6f63 6b2d 696e 6465 6e74 3a30 3b20 7465  ock-indent:0; te
-0000ecb0: 7874 2d69 6e64 656e 743a 3070 783b 5c22  xt-indent:0px;\"
-0000ecc0: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
-0000ecd0: 666f 6e74 2d77 6569 6768 743a 3630 303b  font-weight:600;
-0000ece0: 2063 6f6c 6f72 3a23 6663 3031 3037 3b5c   color:#fc0107;\
-0000ecf0: 223e 4e4f 5445 3a20 596f 7572 2073 616d  ">NOTE: Your sam
-0000ed00: 706c 6520 7369 7a65 206d 7573 7420 6265  ple size must be
-0000ed10: 206c 6172 6765 7220 7468 616e 2061 7420   larger than at 
-0000ed20: 6c65 6173 7420 342a 3c2f 7370 616e 3e3c  least 4*</span><
-0000ed30: 7370 616e 2073 7479 6c65 3d5c 2220 666f  span style=\" fo
-0000ed40: 6e74 2d77 6569 6768 743a 3630 303b 2066  nt-weight:600; f
-0000ed50: 6f6e 742d 7374 796c 653a 6974 616c 6963  ont-style:italic
-0000ed60: 3b20 636f 6c6f 723a 2366 6330 3130 373b  ; color:#fc0107;
-0000ed70: 5c22 3e4e 3c2f 7370 616e 3e3c 7370 616e  \">N</span><span
-0000ed80: 2073 7479 6c65 3d5c 2220 666f 6e74 2d77   style=\" font-w
-0000ed90: 6569 6768 743a 3630 303b 2063 6f6c 6f72  eight:600; color
-0000eda0: 3a23 6663 3031 3037 3b5c 223e 2c20 6f74  :#fc0107;\">, ot
-0000edb0: 6865 7277 6973 6520 796f 7520 4341 4e4e  herwise you CANN
-0000edc0: 4f54 2063 6f6e 6475 6374 2050 4341 2061  OT conduct PCA a
-0000edd0: 7420 6e65 7874 2074 7562 2e3c 2f73 7061  t next tub.</spa
-0000ede0: 6e3e 3c2f 703e 5c6e 220a 223c 7020 7374  n></p>\n"."<p st
-0000edf0: 796c 653d 5c22 206d 6172 6769 6e2d 746f  yle=\" margin-to
-0000ee00: 703a 3070 783b 206d 6172 6769 6e2d 626f  p:0px; margin-bo
-0000ee10: 7474 6f6d 3a30 7078 3b20 6d61 7267 696e  ttom:0px; margin
-0000ee20: 2d6c 6566 743a 3070 783b 206d 6172 6769  -left:0px; margi
-0000ee30: 6e2d 7269 6768 743a 3070 783b 202d 7174  n-right:0px; -qt
-0000ee40: 2d62 6c6f 636b 2d69 6e64 656e 743a 303b  -block-indent:0;
-0000ee50: 2074 6578 742d 696e 6465 6e74 3a30 7078   text-indent:0px
-0000ee60: 3b5c 223e 382e 2043 686f 6f73 6520 6d69  ;\">8. Choose mi
-0000ee70: 6e69 6d75 6d20 7069 7865 6c20 6172 6561  nimum pixel area
-0000ee80: 206f 6620 7361 6d70 6c65 7320 736f 2074   of samples so t
-0000ee90: 6861 7420 796f 7520 6361 6e20 6578 636c  hat you can excl
-0000eea0: 7564 6520 6e6f 6973 6520 6672 6f6d 2079  ude noise from y
-0000eeb0: 6f75 7220 6461 7461 2e3c 2f70 3e5c 6e22  our data.</p>\n"
-0000eec0: 0a22 3c70 2073 7479 6c65 3d5c 2220 6d61  ."<p style=\" ma
-0000eed0: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
-0000eee0: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
-0000eef0: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
-0000ef00: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
-0000ef10: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
-0000ef20: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
-0000ef30: 656e 743a 3070 783b 5c22 3e39 2e20 7365  ent:0px;\">9. se
-0000ef40: 7420 5363 616c 652e 203c 2f70 3e5c 6e22  t Scale. </p>\n"
-0000ef50: 0a22 3c70 2073 7479 6c65 3d5c 2220 6d61  ."<p style=\" ma
-0000ef60: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
-0000ef70: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
-0000ef80: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
-0000ef90: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
-0000efa0: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
-0000efb0: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
-0000efc0: 656e 743a 3070 783b 5c22 3e59 6f75 2063  ent:0px;\">You c
-0000efd0: 616e 2063 686f 6f73 6520 3244 206f 7220  an choose 2D or 
-0000efe0: 3144 2073 6361 6c65 2e3c 2f70 3e5c 6e22  1D scale.</p>\n"
-0000eff0: 0a22 3c70 2073 7479 6c65 3d5c 2220 6d61  ."<p style=\" ma
-0000f000: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
-0000f010: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
-0000f020: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
-0000f030: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
-0000f040: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
-0000f050: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
-0000f060: 656e 743a 3070 783b 5c22 3e49 6e20 7468  ent:0px;\">In th
-0000f070: 6520 6361 7365 206f 6620 3244 2073 6361  e case of 2D sca
-0000f080: 6c65 2c20 796f 7572 2064 6174 6120 7769  le, your data wi
-0000f090: 6c6c 2062 6520 7363 616c 6564 2062 6173  ll be scaled bas
-0000f0a0: 6564 206f 6e20 7468 6520 6172 6561 206f  ed on the area o
-0000f0b0: 6620 7468 6520 7363 616c 6520 6f62 6a65  f the scale obje
-0000f0c0: 6374 2e3c 2f70 3e5c 6e22 0a22 3c70 2073  ct.</p>\n"."<p s
-0000f0d0: 7479 6c65 3d5c 2220 6d61 7267 696e 2d74  tyle=\" margin-t
-0000f0e0: 6f70 3a30 7078 3b20 6d61 7267 696e 2d62  op:0px; margin-b
-0000f0f0: 6f74 746f 6d3a 3070 783b 206d 6172 6769  ottom:0px; margi
-0000f100: 6e2d 6c65 6674 3a30 7078 3b20 6d61 7267  n-left:0px; marg
-0000f110: 696e 2d72 6967 6874 3a30 7078 3b20 2d71  in-right:0px; -q
-0000f120: 742d 626c 6f63 6b2d 696e 6465 6e74 3a30  t-block-indent:0
-0000f130: 3b20 7465 7874 2d69 6e64 656e 743a 3070  ; text-indent:0p
-0000f140: 783b 5c22 3e49 6e20 7468 6520 6361 7365  x;\">In the case
-0000f150: 206f 6620 3144 2073 6361 6c65 2c20 796f   of 1D scale, yo
-0000f160: 7572 2064 6174 6120 7769 6c6c 2062 6520  ur data will be 
-0000f170: 7363 616c 6564 2062 6173 6564 206f 6e20  scaled based on 
-0000f180: 7468 6520 206c 656e 6774 6820 6f66 2074  the  length of t
-0000f190: 6865 2073 6361 6c65 206f 626a 6563 742e  he scale object.
-0000f1a0: 3c2f 703e 5c6e 220a 223c 7020 7374 796c  </p>\n"."<p styl
-0000f1b0: 653d 5c22 2d71 742d 7061 7261 6772 6170  e=\"-qt-paragrap
-0000f1c0: 682d 7479 7065 3a65 6d70 7479 3b20 6d61  h-type:empty; ma
-0000f1d0: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
-0000f1e0: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
-0000f1f0: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
-0000f200: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
-0000f210: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
-0000f220: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
-0000f230: 656e 743a 3070 783b 5c22 3e3c 6272 202f  ent:0px;\"><br /
-0000f240: 3e3c 2f70 3e5c 6e22 0a22 3c70 2073 7479  ></p>\n"."<p sty
-0000f250: 6c65 3d5c 2220 6d61 7267 696e 2d74 6f70  le=\" margin-top
-0000f260: 3a30 7078 3b20 6d61 7267 696e 2d62 6f74  :0px; margin-bot
-0000f270: 746f 6d3a 3070 783b 206d 6172 6769 6e2d  tom:0px; margin-
-0000f280: 6c65 6674 3a30 7078 3b20 6d61 7267 696e  left:0px; margin
-0000f290: 2d72 6967 6874 3a30 7078 3b20 2d71 742d  -right:0px; -qt-
-0000f2a0: 626c 6f63 6b2d 696e 6465 6e74 3a30 3b20  block-indent:0; 
-0000f2b0: 7465 7874 2d69 6e64 656e 743a 3070 783b  text-indent:0px;
-0000f2c0: 5c22 3e31 302e 2050 7265 7373 2026 7175  \">10. Press &qu
-0000f2d0: 6f74 3b41 6e61 6c79 7a65 2671 756f 743b  ot;Analyze&quot;
-0000f2e0: 2062 7574 746f 6e2e 3c2f 703e 5c6e 220a   button.</p>\n".
-0000f2f0: 223c 7020 7374 796c 653d 5c22 2d71 742d  "<p style=\"-qt-
-0000f300: 7061 7261 6772 6170 682d 7479 7065 3a65  paragraph-type:e
-0000f310: 6d70 7479 3b20 6d61 7267 696e 2d74 6f70  mpty; margin-top
-0000f320: 3a30 7078 3b20 6d61 7267 696e 2d62 6f74  :0px; margin-bot
-0000f330: 746f 6d3a 3070 783b 206d 6172 6769 6e2d  tom:0px; margin-
-0000f340: 6c65 6674 3a30 7078 3b20 6d61 7267 696e  left:0px; margin
-0000f350: 2d72 6967 6874 3a30 7078 3b20 2d71 742d  -right:0px; -qt-
-0000f360: 626c 6f63 6b2d 696e 6465 6e74 3a30 3b20  block-indent:0; 
-0000f370: 7465 7874 2d69 6e64 656e 743a 3070 783b  text-indent:0px;
-0000f380: 5c22 3e3c 6272 202f 3e3c 2f70 3e5c 6e22  \"><br /></p>\n"
-0000f390: 0a22 3c70 2073 7479 6c65 3d5c 2220 6d61  ."<p style=\" ma
-0000f3a0: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
-0000f3b0: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
-0000f3c0: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
-0000f3d0: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
-0000f3e0: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
-0000f3f0: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
-0000f400: 656e 743a 3070 783b 5c22 3e49 6620 796f  ent:0px;\">If yo
-0000f410: 7572 2061 6e61 6c79 7369 7320 656e 6473  ur analysis ends
-0000f420: 2c20 706c 6561 7365 2067 6f20 746f 2074  , please go to t
-0000f430: 6865 2050 4341 2074 6162 2e3c 2f70 3e5c  he PCA tab.</p>\
-0000f440: 6e22 0a22 3c70 2073 7479 6c65 3d5c 2220  n"."<p style=\" 
-0000f450: 6d61 7267 696e 2d74 6f70 3a30 7078 3b20  margin-top:0px; 
-0000f460: 6d61 7267 696e 2d62 6f74 746f 6d3a 3070  margin-bottom:0p
-0000f470: 783b 206d 6172 6769 6e2d 6c65 6674 3a30  x; margin-left:0
-0000f480: 7078 3b20 6d61 7267 696e 2d72 6967 6874  px; margin-right
-0000f490: 3a30 7078 3b20 2d71 742d 626c 6f63 6b2d  :0px; -qt-block-
-0000f4a0: 696e 6465 6e74 3a30 3b20 7465 7874 2d69  indent:0; text-i
-0000f4b0: 6e64 656e 743a 3070 783b 5c22 3e23 2d2d  ndent:0px;\">#--
-0000f4c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000f4d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3c  ---------------<
-0000f4e0: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
-0000f4f0: 3d5c 222d 7174 2d70 6172 6167 7261 7068  =\"-qt-paragraph
-0000f500: 2d74 7970 653a 656d 7074 793b 206d 6172  -type:empty; mar
-0000f510: 6769 6e2d 746f 703a 3070 783b 206d 6172  gin-top:0px; mar
-0000f520: 6769 6e2d 626f 7474 6f6d 3a30 7078 3b20  gin-bottom:0px; 
-0000f530: 6d61 7267 696e 2d6c 6566 743a 3070 783b  margin-left:0px;
-0000f540: 206d 6172 6769 6e2d 7269 6768 743a 3070   margin-right:0p
-0000f550: 783b 202d 7174 2d62 6c6f 636b 2d69 6e64  x; -qt-block-ind
-0000f560: 656e 743a 303b 2074 6578 742d 696e 6465  ent:0; text-inde
-0000f570: 6e74 3a30 7078 3b5c 223e 3c62 7220 2f3e  nt:0px;\"><br />
-0000f580: 3c2f 703e 3c2f 626f 6479 3e3c 2f68 746d  </p></body></htm
-0000f590: 6c3e 2229 290a 2020 2020 2020 2020 7365  l>")).        se
-0000f5a0: 6c66 2e6c 6162 656c 5f32 2e73 6574 5465  lf.label_2.setTe
-0000f5b0: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-0000f5c0: 6169 6e57 696e 646f 7722 2c20 2220 4c6f  ainWindow", " Lo
-0000f5d0: 6722 2929 0a20 2020 2020 2020 2073 656c  g")).        sel
-0000f5e0: 662e 6c61 6265 6c5f 392e 7365 7454 6578  f.label_9.setTex
-0000f5f0: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
-0000f600: 696e 5769 6e64 6f77 222c 2022 5363 616c  inWindow", "Scal
-0000f610: 6520 556e 6974 2229 290a 2020 2020 2020  e Unit")).      
-0000f620: 2020 7365 6c66 2e6c 6162 656c 5f38 2e73    self.label_8.s
-0000f630: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-0000f640: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-0000f650: 2253 6361 6c65 2053 697a 6522 2929 0a20  "Scale Size")). 
-0000f660: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-0000f670: 6c5f 3130 2e73 6574 5465 7874 285f 7472  l_10.setText(_tr
-0000f680: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-0000f690: 646f 7722 2c20 2250 6f73 6974 696f 6e22  dow", "Position"
-0000f6a0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000f6b0: 636d 625f 7363 616c 6550 6f73 2e73 6574  cmb_scalePos.set
-0000f6c0: 4974 656d 5465 7874 2830 2c20 5f74 7261  ItemText(0, _tra
-0000f6d0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-0000f6e0: 6f77 222c 2022 546f 7022 2929 0a20 2020  ow", "Top")).   
-0000f6f0: 2020 2020 2073 656c 662e 636d 625f 7363       self.cmb_sc
-0000f700: 616c 6550 6f73 2e73 6574 4974 656d 5465  alePos.setItemTe
-0000f710: 7874 2831 2c20 5f74 7261 6e73 6c61 7465  xt(1, _translate
-0000f720: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-0000f730: 426f 7474 6f6d 2229 290a 2020 2020 2020  Bottom")).      
-0000f740: 2020 7365 6c66 2e63 6d62 5f73 6361 6c65    self.cmb_scale
-0000f750: 506f 732e 7365 7449 7465 6d54 6578 7428  Pos.setItemText(
-0000f760: 322c 205f 7472 616e 736c 6174 6528 224d  2, _translate("M
-0000f770: 6169 6e57 696e 646f 7722 2c20 2252 6967  ainWindow", "Rig
-0000f780: 6874 2229 290a 2020 2020 2020 2020 7365  ht")).        se
-0000f790: 6c66 2e63 6d62 5f73 6361 6c65 506f 732e  lf.cmb_scalePos.
-0000f7a0: 7365 7449 7465 6d54 6578 7428 332c 205f  setItemText(3, _
-0000f7b0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-0000f7c0: 696e 646f 7722 2c20 224c 6566 7422 2929  indow", "Left"))
-0000f7d0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-0000f7e0: 6265 6c5f 342e 7365 7454 6578 7428 5f74  bel_4.setText(_t
-0000f7f0: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-0000f800: 6e64 6f77 222c 2022 4d61 7869 6d75 6d20  ndow", "Maximum 
-0000f810: 4861 726d 6f6e 6963 7322 2929 0a20 2020  Harmonics")).   
-0000f820: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-0000f830: 7361 7665 2e73 6574 5465 7874 285f 7472  save.setText(_tr
-0000f840: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-0000f850: 646f 7722 2c20 2253 6176 6520 7265 7375  dow", "Save resu
-0000f860: 6c74 7320 746f 202a 2229 290a 2020 2020  lts to *")).    
-0000f870: 2020 2020 7365 6c66 2e6c 6162 656c 2e73      self.label.s
-0000f880: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-0000f890: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-0000f8a0: 2249 6d61 6765 2066 6f72 6d61 7422 2929  "Image format"))
-0000f8b0: 0a20 2020 2020 2020 2073 656c 662e 6275  .        self.bu
-0000f8c0: 7474 6f6e 5f73 6176 652e 7365 7454 6578  tton_save.setTex
-0000f8d0: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
-0000f8e0: 696e 5769 6e64 6f77 222c 2022 7365 6c65  inWindow", "sele
-0000f8f0: 6374 2229 290a 2020 2020 2020 2020 7365  ct")).        se
-0000f900: 6c66 2e6c 6162 656c 5f33 2e73 6574 5465  lf.label_3.setTe
-0000f910: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-0000f920: 6169 6e57 696e 646f 7722 2c20 2249 6e69  ainWindow", "Ini
-0000f930: 7469 616c 2053 6574 7469 6e67 206f 6620  tial Setting of 
-0000f940: 466f 7572 6965 7220 416e 616c 7973 6973  Fourier Analysis
-0000f950: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-0000f960: 2e62 7574 746f 6e5f 666f 6c64 612e 7365  .button_folda.se
-0000f970: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
-0000f980: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-0000f990: 5365 6c65 6374 2229 290a 2020 2020 2020  Select")).      
-0000f9a0: 2020 7365 6c66 2e6c 6162 656c 5f33 312e    self.label_31.
-0000f9b0: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-0000f9c0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-0000f9d0: 2022 4e4f 5445 3a20 4974 206d 6967 6874   "NOTE: It might
-0000f9e0: 2074 616b 6520 6c6f 6e67 2074 696d 6522   take long time"
-0000f9f0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000fa00: 6362 5f73 6176 6541 6c6c 2e73 6574 5465  cb_saveAll.setTe
-0000fa10: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-0000fa20: 6169 6e57 696e 646f 7722 2c20 2253 6176  ainWindow", "Sav
-0000fa30: 6520 616c 6c20 4e6f 726d 616c 697a 6564  e all Normalized
-0000fa40: 2073 616d 706c 6573 2064 6174 6122 2929   samples data"))
-0000fa50: 0a20 2020 2020 2020 2073 656c 662e 7262  .        self.rb
-0000fa60: 5f66 696c 656e 616d 652e 7365 7454 6578  _filename.setTex
-0000fa70: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
-0000fa80: 696e 5769 6e64 6f77 222c 2022 6669 6c65  inWindow", "file
-0000fa90: 206e 616d 6520 2864 6576 6964 6520 6561   name (devide ea
-0000faa0: 6368 2063 6174 6567 6f72 7920 6279 205c  ch category by \
-0000fab0: 275f 5c27 2922 2929 0a20 2020 2020 2020  '_\')")).       
-0000fac0: 2073 656c 662e 6c61 6265 6c5f 3332 2e73   self.label_32.s
-0000fad0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-0000fae0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-0000faf0: 2243 6174 6567 6f72 697a 6520 796f 7572  "Categorize your
-0000fb00: 2066 696c 6573 2062 6173 6564 206f 6e2e   files based on.
-0000fb10: 2e2e 2229 290a 2020 2020 2020 2020 7365  ..")).        se
-0000fb20: 6c66 2e72 625f 7375 6266 6f6c 6461 2e73  lf.rb_subfolda.s
-0000fb30: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-0000fb40: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-0000fb50: 226e 616d 6520 6f66 2073 7562 666f 6c64  "name of subfold
-0000fb60: 6122 2929 0a20 2020 2020 2020 2073 656c  a")).        sel
-0000fb70: 662e 6c61 6265 6c5f 352e 7365 7454 6578  f.label_5.setTex
-0000fb80: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
-0000fb90: 696e 5769 6e64 6f77 222c 2022 6d69 6e69  inWindow", "mini
-0000fba0: 6d75 6d20 5069 7865 6c20 4172 6561 2229  mum Pixel Area")
-0000fbb0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-0000fbc0: 6162 656c 5f66 6f6c 6461 2e73 6574 5465  abel_folda.setTe
-0000fbd0: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-0000fbe0: 6169 6e57 696e 646f 7722 2c20 2249 6d70  ainWindow", "Imp
-0000fbf0: 6f72 7420 696d 6167 6573 2066 726f 6d20  ort images from 
-0000fc00: 2a22 2929 0a20 2020 2020 2020 2073 656c  *")).        sel
-0000fc10: 662e 6c61 6265 6c5f 3137 2e73 6574 5465  f.label_17.setTe
-0000fc20: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-0000fc30: 6169 6e57 696e 646f 7722 2c20 2243 6174  ainWindow", "Cat
-0000fc40: 6567 6f72 7920 636c 6173 7320 6e61 6d65  egory class name
-0000fc50: 2028 6e6f 7420 6d61 6e64 6174 6f72 7929   (not mandatory)
-0000fc60: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-0000fc70: 2e62 7574 746f 6e5f 6865 6164 6572 2e73  .button_header.s
-0000fc80: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-0000fc90: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-0000fca0: 2261 7373 6967 6e22 2929 0a20 2020 2020  "assign")).     
-0000fcb0: 2020 2073 656c 662e 636d 625f 666f 726d     self.cmb_form
-0000fcc0: 6174 2e73 6574 4974 656d 5465 7874 2830  at.setItemText(0
-0000fcd0: 2c20 5f74 7261 6e73 6c61 7465 2822 4d61  , _translate("Ma
-0000fce0: 696e 5769 6e64 6f77 222c 2022 2e70 6e67  inWindow", ".png
-0000fcf0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-0000fd00: 2e63 6d62 5f66 6f72 6d61 742e 7365 7449  .cmb_format.setI
-0000fd10: 7465 6d54 6578 7428 312c 205f 7472 616e  temText(1, _tran
-0000fd20: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-0000fd30: 7722 2c20 222e 424d 5022 2929 0a20 2020  w", ".BMP")).   
-0000fd40: 2020 2020 2073 656c 662e 636d 625f 666f       self.cmb_fo
-0000fd50: 726d 6174 2e73 6574 4974 656d 5465 7874  rmat.setItemText
-0000fd60: 2832 2c20 5f74 7261 6e73 6c61 7465 2822  (2, _translate("
-0000fd70: 4d61 696e 5769 6e64 6f77 222c 2022 2e6a  MainWindow", ".j
-0000fd80: 7065 6722 2929 0a20 2020 2020 2020 2073  peg")).        s
-0000fd90: 656c 662e 636d 625f 666f 726d 6174 2e73  elf.cmb_format.s
-0000fda0: 6574 4974 656d 5465 7874 2833 2c20 5f74  etItemText(3, _t
-0000fdb0: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-0000fdc0: 6e64 6f77 222c 2022 2e6a 7067 2229 290a  ndow", ".jpg")).
-0000fdd0: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
-0000fde0: 5f73 6361 6c65 5479 7065 2e73 6574 4974  _scaleType.setIt
-0000fdf0: 656d 5465 7874 2830 2c20 5f74 7261 6e73  emText(0, _trans
-0000fe00: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-0000fe10: 222c 2022 4e6f 2073 6361 6c65 2229 290a  ", "No scale")).
-0000fe20: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
-0000fe30: 5f73 6361 6c65 5479 7065 2e73 6574 4974  _scaleType.setIt
-0000fe40: 656d 5465 7874 2831 2c20 5f74 7261 6e73  emText(1, _trans
-0000fe50: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-0000fe60: 222c 2022 322d 4420 2841 7265 6129 2229  ", "2-D (Area)")
-0000fe70: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-0000fe80: 6d62 5f73 6361 6c65 5479 7065 2e73 6574  mb_scaleType.set
-0000fe90: 4974 656d 5465 7874 2832 2c20 5f74 7261  ItemText(2, _tra
-0000fea0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-0000feb0: 6f77 222c 2022 312d 4420 2858 2d4c 656e  ow", "1-D (X-Len
-0000fec0: 6774 6829 2229 290a 2020 2020 2020 2020  gth)")).        
-0000fed0: 7365 6c66 2e63 6d62 5f73 6361 6c65 5479  self.cmb_scaleTy
-0000fee0: 7065 2e73 6574 4974 656d 5465 7874 2833  pe.setItemText(3
-0000fef0: 2c20 5f74 7261 6e73 6c61 7465 2822 4d61  , _translate("Ma
-0000ff00: 696e 5769 6e64 6f77 222c 2022 312d 4420  inWindow", "1-D 
-0000ff10: 2859 2d4c 656e 6774 6829 2229 290a 2020  (Y-Length)")).  
-0000ff20: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-0000ff30: 5f37 2e73 6574 5465 7874 285f 7472 616e  _7.setText(_tran
-0000ff40: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-0000ff50: 7722 2c20 2253 6361 6c65 2073 6574 7469  w", "Scale setti
-0000ff60: 6e67 2229 290a 2020 2020 2020 2020 7365  ng")).        se
-0000ff70: 6c66 2e72 625f 6e6f 6e65 2e73 6574 5465  lf.rb_none.setTe
-0000ff80: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-0000ff90: 6169 6e57 696e 646f 7722 2c20 224e 6f6e  ainWindow", "Non
-0000ffa0: 6522 2929 0a20 2020 2020 2020 2073 656c  e")).        sel
-0000ffb0: 662e 6c61 6265 6c5f 362e 7365 7454 6578  f.label_6.setTex
-0000ffc0: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
-0000ffd0: 696e 5769 6e64 6f77 222c 2022 4261 636b  inWindow", "Back
-0000ffe0: 6772 6f75 6e64 2043 6f6c 6f72 2229 290a  ground Color")).
-0000fff0: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
-00010000: 5f73 616d 706c 6554 7970 652e 7365 7449  _sampleType.setI
-00010010: 7465 6d54 6578 7428 302c 205f 7472 616e  temText(0, _tran
-00010020: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-00010030: 7722 2c20 2257 6869 7465 2229 290a 2020  w", "White")).  
-00010040: 2020 2020 2020 7365 6c66 2e63 6d62 5f73        self.cmb_s
-00010050: 616d 706c 6554 7970 652e 7365 7449 7465  ampleType.setIte
-00010060: 6d54 6578 7428 312c 205f 7472 616e 736c  mText(1, _transl
-00010070: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00010080: 2c20 2242 6c61 636b 2229 290a 2020 2020  , "Black")).    
-00010090: 2020 2020 7365 6c66 2e74 6162 5769 6467      self.tabWidg
-000100a0: 6574 2e73 6574 5461 6254 6578 7428 7365  et.setTabText(se
-000100b0: 6c66 2e74 6162 5769 6467 6574 2e69 6e64  lf.tabWidget.ind
-000100c0: 6578 4f66 2873 656c 662e 7461 6229 2c20  exOf(self.tab), 
-000100d0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-000100e0: 5769 6e64 6f77 222c 2022 496d 6167 6520  Window", "Image 
-000100f0: 416e 616c 7973 6973 2229 290a 2020 2020  Analysis")).    
-00010100: 2020 2020 7365 6c66 2e6c 6162 656c 5f31      self.label_1
-00010110: 312e 7365 7454 6578 7428 5f74 7261 6e73  1.setText(_trans
-00010120: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00010130: 222c 2022 4d61 7472 6978 2229 290a 2020  ", "Matrix")).  
-00010140: 2020 2020 2020 7365 6c66 2e63 6d62 5f6d        self.cmb_m
-00010150: 6174 7269 7850 4341 2e73 6574 4974 656d  atrixPCA.setItem
-00010160: 5465 7874 2830 2c20 5f74 7261 6e73 6c61  Text(0, _transla
-00010170: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-00010180: 2022 436f 7272 656c 6174 696f 6e22 2929   "Correlation"))
-00010190: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
-000101a0: 625f 6d61 7472 6978 5043 412e 7365 7449  b_matrixPCA.setI
-000101b0: 7465 6d54 6578 7428 312c 205f 7472 616e  temText(1, _tran
-000101c0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-000101d0: 7722 2c20 2243 6f76 6172 6961 6e63 6522  w", "Covariance"
-000101e0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-000101f0: 6c61 6265 6c5f 3134 2e73 6574 5465 7874  label_14.setText
-00010200: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-00010210: 6e57 696e 646f 7722 2c20 2249 6e69 7469  nWindow", "Initi
-00010220: 616c 2053 6574 7469 6e67 206f 6620 5043  al Setting of PC
-00010230: 4122 2929 0a20 2020 2020 2020 2073 656c  A")).        sel
-00010240: 662e 636d 625f 4650 532e 7365 7449 7465  f.cmb_FPS.setIte
-00010250: 6d54 6578 7428 302c 205f 7472 616e 736c  mText(0, _transl
-00010260: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00010270: 2c20 2246 5053 2028 4e6f 6e2d 4469 7265  , "FPS (Non-Dire
-00010280: 6374 696f 6e61 6c29 2229 290a 2020 2020  ctional)")).    
-00010290: 2020 2020 7365 6c66 2e63 6d62 5f46 5053      self.cmb_FPS
-000102a0: 2e73 6574 4974 656d 5465 7874 2831 2c20  .setItemText(1, 
-000102b0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-000102c0: 5769 6e64 6f77 222c 2022 416d 706c 6974  Window", "Amplit
-000102d0: 7564 6520 6f66 2048 6172 6d6f 6e69 6373  ude of Harmonics
-000102e0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-000102f0: 2e63 6d62 5f46 5053 2e73 6574 4974 656d  .cmb_FPS.setItem
-00010300: 5465 7874 2832 2c20 5f74 7261 6e73 6c61  Text(2, _transla
-00010310: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-00010320: 2022 4546 4420 2844 6972 6563 7469 6f6e   "EFD (Direction
-00010330: 616c 2922 2929 0a20 2020 2020 2020 2073  al)")).        s
-00010340: 656c 662e 6c61 6265 6c5f 3133 2e73 6574  elf.label_13.set
-00010350: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
-00010360: 224d 6169 6e57 696e 646f 7722 2c20 2253  "MainWindow", "S
-00010370: 6176 6520 466f 6c64 612a 2229 290a 2020  ave Folda*")).  
-00010380: 2020 2020 2020 7365 6c66 2e62 7574 746f        self.butto
-00010390: 6e5f 4650 5370 6174 682e 7365 7454 6578  n_FPSpath.setTex
-000103a0: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
-000103b0: 696e 5769 6e64 6f77 222c 2022 5365 6c65  inWindow", "Sele
-000103c0: 6374 2229 290a 2020 2020 2020 2020 7365  ct")).        se
-000103d0: 6c66 2e6c 6162 656c 5f31 322e 7365 7454  lf.label_12.setT
-000103e0: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-000103f0: 4d61 696e 5769 6e64 6f77 222c 2022 4669  MainWindow", "Fi
-00010400: 6c65 2046 6f6c 6461 2a22 2929 0a20 2020  le Folda*")).   
-00010410: 2020 2020 2073 656c 662e 6275 7474 6f6e       self.button
-00010420: 5f73 6176 6550 4341 7061 7468 2e73 6574  _savePCApath.set
-00010430: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
-00010440: 224d 6169 6e57 696e 646f 7722 2c20 2253  "MainWindow", "S
-00010450: 656c 6563 7422 2929 0a20 2020 2020 2020  elect")).       
-00010460: 2073 656c 662e 6c61 6265 6c5f 3238 2e73   self.label_28.s
-00010470: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-00010480: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00010490: 2253 7562 4772 6f75 7022 2929 0a20 2020  "SubGroup")).   
-000104a0: 2020 2020 2073 656c 662e 7075 7368 4275       self.pushBu
-000104b0: 7474 6f6e 5f32 2e73 6574 5465 7874 285f  tton_2.setText(_
-000104c0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-000104d0: 696e 646f 7722 2c20 2253 6176 6520 4173  indow", "Save As
-000104e0: 2e2e 2e22 2929 0a20 2020 2020 2020 2073  ...")).        s
-000104f0: 656c 662e 6c61 6265 6c5f 3232 2e73 6574  elf.label_22.set
-00010500: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
-00010510: 224d 6169 6e57 696e 646f 7722 2c20 2247  "MainWindow", "G
-00010520: 7261 7068 2053 6574 7469 6e67 2229 290a  raph Setting")).
-00010530: 2020 2020 2020 2020 7365 6c66 2e70 7573          self.pus
-00010540: 6842 7574 746f 6e2e 7365 7454 6578 7428  hButton.setText(
-00010550: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00010560: 5769 6e64 6f77 222c 2022 5072 6576 6965  Window", "Previe
-00010570: 7722 2929 0a20 2020 2020 2020 2073 656c  w")).        sel
-00010580: 662e 6c61 6265 6c5f 3230 2e73 6574 5465  f.label_20.setTe
-00010590: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-000105a0: 6169 6e57 696e 646f 7722 2c20 2243 6174  ainWindow", "Cat
-000105b0: 6567 6f72 7922 2929 0a20 2020 2020 2020  egory")).       
-000105c0: 2073 656c 662e 6c61 6265 6c5f 3138 2e73   self.label_18.s
-000105d0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-000105e0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-000105f0: 2258 2d61 7869 7322 2929 0a20 2020 2020  "X-axis")).     
-00010600: 2020 2073 656c 662e 6c61 6265 6c5f 3234     self.label_24
-00010610: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
-00010620: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00010630: 2c20 2250 6c6f 7422 2929 0a20 2020 2020  , "Plot")).     
-00010640: 2020 2073 656c 662e 6c61 6265 6c5f 3231     self.label_21
-00010650: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
-00010660: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00010670: 2c20 2253 697a 6522 2929 0a20 2020 2020  , "Size")).     
-00010680: 2020 2073 656c 662e 636d 625f 706c 6f74     self.cmb_plot
-00010690: 2e73 6574 4974 656d 5465 7874 2830 2c20  .setItemText(0, 
-000106a0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-000106b0: 5769 6e64 6f77 222c 2022 5363 6174 7465  Window", "Scatte
-000106c0: 7222 2929 0a20 2020 2020 2020 2073 656c  r")).        sel
-000106d0: 662e 636d 625f 706c 6f74 2e73 6574 4974  f.cmb_plot.setIt
-000106e0: 656d 5465 7874 2831 2c20 5f74 7261 6e73  emText(1, _trans
-000106f0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00010700: 222c 2022 4465 6e73 6974 7922 2929 0a20  ", "Density")). 
-00010710: 2020 2020 2020 2073 656c 662e 636d 625f         self.cmb_
-00010720: 706c 6f74 2e73 6574 4974 656d 5465 7874  plot.setItemText
-00010730: 2832 2c20 5f74 7261 6e73 6c61 7465 2822  (2, _translate("
-00010740: 4d61 696e 5769 6e64 6f77 222c 2022 4869  MainWindow", "Hi
-00010750: 7374 6f67 7261 6d22 2929 0a20 2020 2020  stogram")).     
-00010760: 2020 2073 656c 662e 6c61 6265 6c5f 3239     self.label_29
-00010770: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
-00010780: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00010790: 2c20 2253 7562 7375 6247 726f 7570 2229  , "SubsubGroup")
-000107a0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-000107b0: 6162 656c 5f31 392e 7365 7454 6578 7428  abel_19.setText(
-000107c0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-000107d0: 5769 6e64 6f77 222c 2022 592d 6178 6973  Window", "Y-axis
-000107e0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-000107f0: 2e6c 6162 656c 5f62 696e 732e 7365 7454  .label_bins.setT
-00010800: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-00010810: 4d61 696e 5769 6e64 6f77 222c 2022 6269  MainWindow", "bi
-00010820: 6e73 2229 290a 2020 2020 2020 2020 7365  ns")).        se
-00010830: 6c66 2e6c 6162 656c 5f33 302e 7365 7454  lf.label_30.setT
-00010840: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-00010850: 4d61 696e 5769 6e64 6f77 222c 2022 616c  MainWindow", "al
-00010860: 7068 6122 2929 0a20 2020 2020 2020 2073  pha")).        s
-00010870: 656c 662e 6275 7474 6f6e 5f50 4341 2e73  elf.button_PCA.s
-00010880: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-00010890: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-000108a0: 2250 4341 2229 290a 2020 2020 2020 2020  "PCA")).        
-000108b0: 7365 6c66 2e6c 6f67 626f 785f 7063 612e  self.logbox_pca.
-000108c0: 7365 7448 746d 6c28 5f74 7261 6e73 6c61  setHtml(_transla
-000108d0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-000108e0: 2022 3c21 444f 4354 5950 4520 4854 4d4c   "<!DOCTYPE HTML
-000108f0: 2050 5542 4c49 4320 5c22 2d2f 2f57 3343   PUBLIC \"-//W3C
-00010900: 2f2f 4454 4420 4854 4d4c 2034 2e30 2f2f  //DTD HTML 4.0//
-00010910: 454e 5c22 205c 2268 7474 703a 2f2f 7777  EN\" \"http://ww
-00010920: 772e 7733 2e6f 7267 2f54 522f 5245 432d  w.w3.org/TR/REC-
-00010930: 6874 6d6c 3430 2f73 7472 6963 742e 6474  html40/strict.dt
-00010940: 645c 223e 5c6e 220a 223c 6874 6d6c 3e3c  d\">\n"."<html><
-00010950: 6865 6164 3e3c 6d65 7461 206e 616d 653d  head><meta name=
-00010960: 5c22 7172 6963 6874 6578 745c 2220 636f  \"qrichtext\" co
-00010970: 6e74 656e 743d 5c22 315c 2220 2f3e 3c73  ntent=\"1\" /><s
-00010980: 7479 6c65 2074 7970 653d 5c22 7465 7874  tyle type=\"text
-00010990: 2f63 7373 5c22 3e5c 6e22 0a22 702c 206c  /css\">\n"."p, l
-000109a0: 6920 7b20 7768 6974 652d 7370 6163 653a  i { white-space:
-000109b0: 2070 7265 2d77 7261 703b 207d 5c6e 220a   pre-wrap; }\n".
-000109c0: 223c 2f73 7479 6c65 3e3c 2f68 6561 643e  "</style></head>
-000109d0: 3c62 6f64 7920 7374 796c 653d 5c22 2066  <body style=\" f
-000109e0: 6f6e 742d 6661 6d69 6c79 3a5c 272e 5346  ont-family:\'.SF
-000109f0: 204e 5320 5465 7874 5c27 3b20 666f 6e74   NS Text\'; font
-00010a00: 2d73 697a 653a 3133 7074 3b20 666f 6e74  -size:13pt; font
-00010a10: 2d77 6569 6768 743a 3430 303b 2066 6f6e  -weight:400; fon
-00010a20: 742d 7374 796c 653a 6e6f 726d 616c 3b5c  t-style:normal;\
-00010a30: 223e 5c6e 220a 223c 7020 7374 796c 653d  ">\n"."<p style=
-00010a40: 5c22 206d 6172 6769 6e2d 746f 703a 3070  \" margin-top:0p
-00010a50: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
-00010a60: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
-00010a70: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
-00010a80: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
-00010a90: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
-00010aa0: 742d 696e 6465 6e74 3a30 7078 3b5c 223e  t-indent:0px;\">
-00010ab0: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
-00010ac0: 6f6e 742d 7765 6967 6874 3a36 3030 3b20  ont-weight:600; 
-00010ad0: 7465 7874 2d64 6563 6f72 6174 696f 6e3a  text-decoration:
-00010ae0: 2075 6e64 6572 6c69 6e65 3b5c 223e 5072   underline;\">Pr
-00010af0: 696e 6369 7061 6c20 436f 6d70 6f6e 656e  incipal Componen
-00010b00: 7420 416e 616c 7973 7973 2028 5043 4129  t Analysys (PCA)
-00010b10: 3c2f 7370 616e 3e3c 2f70 3e5c 6e22 0a22  </span></p>\n"."
-00010b20: 3c70 2073 7479 6c65 3d5c 222d 7174 2d70  <p style=\"-qt-p
-00010b30: 6172 6167 7261 7068 2d74 7970 653a 656d  aragraph-type:em
-00010b40: 7074 793b 206d 6172 6769 6e2d 746f 703a  pty; margin-top:
-00010b50: 3070 783b 206d 6172 6769 6e2d 626f 7474  0px; margin-bott
-00010b60: 6f6d 3a30 7078 3b20 6d61 7267 696e 2d6c  om:0px; margin-l
-00010b70: 6566 743a 3070 783b 206d 6172 6769 6e2d  eft:0px; margin-
-00010b80: 7269 6768 743a 3070 783b 202d 7174 2d62  right:0px; -qt-b
-00010b90: 6c6f 636b 2d69 6e64 656e 743a 303b 2074  lock-indent:0; t
-00010ba0: 6578 742d 696e 6465 6e74 3a30 7078 3b20  ext-indent:0px; 
-00010bb0: 666f 6e74 2d77 6569 6768 743a 3630 303b  font-weight:600;
-00010bc0: 2074 6578 742d 6465 636f 7261 7469 6f6e   text-decoration
-00010bd0: 3a20 756e 6465 726c 696e 653b 5c22 3e3c  : underline;\"><
-00010be0: 6272 202f 3e3c 2f70 3e5c 6e22 0a22 3c70  br /></p>\n"."<p
-00010bf0: 2073 7479 6c65 3d5c 2220 6d61 7267 696e   style=\" margin
-00010c00: 2d74 6f70 3a30 7078 3b20 6d61 7267 696e  -top:0px; margin
-00010c10: 2d62 6f74 746f 6d3a 3070 783b 206d 6172  -bottom:0px; mar
-00010c20: 6769 6e2d 6c65 6674 3a30 7078 3b20 6d61  gin-left:0px; ma
-00010c30: 7267 696e 2d72 6967 6874 3a30 7078 3b20  rgin-right:0px; 
-00010c40: 2d71 742d 626c 6f63 6b2d 696e 6465 6e74  -qt-block-indent
-00010c50: 3a30 3b20 7465 7874 2d69 6e64 656e 743a  :0; text-indent:
-00010c60: 3070 783b 5c22 3e59 6f75 2063 616e 2063  0px;\">You can c
-00010c70: 686f 6f73 6520 4650 5320 6f72 2045 4644  hoose FPS or EFD
-00010c80: 2066 6f72 2050 4341 2062 6f74 6820 6f66   for PCA both of
-00010c90: 2077 6869 6368 2061 7265 2065 7870 6f72   which are expor
-00010ca0: 7465 6420 6173 2046 5053 2e63 7376 2062  ted as FPS.csv b
-00010cb0: 7920 7468 6520 696d 6167 6520 616e 616c  y the image anal
-00010cc0: 7973 6973 3c2f 703e 5c6e 220a 223c 7020  ysis</p>\n"."<p 
-00010cd0: 7374 796c 653d 5c22 206d 6172 6769 6e2d  style=\" margin-
-00010ce0: 746f 703a 3070 783b 206d 6172 6769 6e2d  top:0px; margin-
-00010cf0: 626f 7474 6f6d 3a30 7078 3b20 6d61 7267  bottom:0px; marg
-00010d00: 696e 2d6c 6566 743a 3070 783b 206d 6172  in-left:0px; mar
-00010d10: 6769 6e2d 7269 6768 743a 3070 783b 202d  gin-right:0px; -
-00010d20: 7174 2d62 6c6f 636b 2d69 6e64 656e 743a  qt-block-indent:
-00010d30: 303b 2074 6578 742d 696e 6465 6e74 3a30  0; text-indent:0
-00010d40: 7078 3b5c 223e 3c73 7061 6e20 7374 796c  px;\"><span styl
-00010d50: 653d 5c22 2063 6f6c 6f72 3a23 6663 3030  e=\" color:#fc00
-00010d60: 3061 3b5c 223e 4e6f 7465 2074 6861 7420  0a;\">Note that 
-00010d70: 796f 7520 6861 7665 2074 6f20 6368 6f6f  you have to choo
-00010d80: 7365 2074 6865 2066 6f6c 6461 2077 6869  se the folda whi
-00010d90: 6368 2069 6e63 6c75 6465 2046 5053 2e63  ch include FPS.c
-00010da0: 7376 2061 7320 4669 6c65 2050 6174 6820  sv as File Path 
-00010db0: 6f74 6865 7277 6973 6520 796f 7520 3c2f  otherwise you </
-00010dc0: 7370 616e 3e3c 7370 616e 2073 7479 6c65  span><span style
-00010dd0: 3d5c 2220 7465 7874 2d64 6563 6f72 6174  =\" text-decorat
-00010de0: 696f 6e3a 2075 6e64 6572 6c69 6e65 3b20  ion: underline; 
-00010df0: 636f 6c6f 723a 2366 6330 3030 613b 5c22  color:#fc000a;\"
-00010e00: 3e63 616e 6e6f 743c 2f73 7061 6e3e 3c73  >cannot</span><s
-00010e10: 7061 6e20 7374 796c 653d 5c22 2063 6f6c  pan style=\" col
-00010e20: 6f72 3a23 6663 3030 3061 3b5c 223e 2064  or:#fc000a;\"> d
-00010e30: 6f20 5043 412e 3c2f 7370 616e 3e3c 2f70  o PCA.</span></p
-00010e40: 3e5c 6e22 0a22 3c70 2073 7479 6c65 3d5c  >\n"."<p style=\
-00010e50: 2220 6d61 7267 696e 2d74 6f70 3a30 7078  " margin-top:0px
-00010e60: 3b20 6d61 7267 696e 2d62 6f74 746f 6d3a  ; margin-bottom:
-00010e70: 3070 783b 206d 6172 6769 6e2d 6c65 6674  0px; margin-left
-00010e80: 3a30 7078 3b20 6d61 7267 696e 2d72 6967  :0px; margin-rig
-00010e90: 6874 3a30 7078 3b20 2d71 742d 626c 6f63  ht:0px; -qt-bloc
-00010ea0: 6b2d 696e 6465 6e74 3a30 3b20 7465 7874  k-indent:0; text
-00010eb0: 2d69 6e64 656e 743a 3070 783b 5c22 3e3c  -indent:0px;\"><
-00010ec0: 7370 616e 2073 7479 6c65 3d5c 2220 636f  span style=\" co
-00010ed0: 6c6f 723a 2330 3030 3030 303b 5c22 3e46  lor:#000000;\">F
-00010ee0: 5053 2e63 7376 2069 7320 7468 6520 6669  PS.csv is the fi
-00010ef0: 6c65 2077 6869 6368 2073 686f 756c 6420  le which should 
-00010f00: 6265 2065 7870 6f72 7465 6420 6174 2069  be exported at i
-00010f10: 6d61 6765 2061 6e61 6c79 7369 7320 5061  mage analysis Pa
-00010f20: 6765 2e3c 2f73 7061 6e3e 3c2f 703e 5c6e  ge.</span></p>\n
-00010f30: 220a 223c 7020 7374 796c 653d 5c22 2d71  "."<p style=\"-q
-00010f40: 742d 7061 7261 6772 6170 682d 7479 7065  t-paragraph-type
-00010f50: 3a65 6d70 7479 3b20 6d61 7267 696e 2d74  :empty; margin-t
-00010f60: 6f70 3a30 7078 3b20 6d61 7267 696e 2d62  op:0px; margin-b
-00010f70: 6f74 746f 6d3a 3070 783b 206d 6172 6769  ottom:0px; margi
-00010f80: 6e2d 6c65 6674 3a30 7078 3b20 6d61 7267  n-left:0px; marg
-00010f90: 696e 2d72 6967 6874 3a30 7078 3b20 2d71  in-right:0px; -q
-00010fa0: 742d 626c 6f63 6b2d 696e 6465 6e74 3a30  t-block-indent:0
-00010fb0: 3b20 7465 7874 2d69 6e64 656e 743a 3070  ; text-indent:0p
-00010fc0: 783b 2063 6f6c 6f72 3a23 3030 3030 3030  x; color:#000000
-00010fd0: 3b5c 223e 3c62 7220 2f3e 3c2f 703e 5c6e  ;\"><br /></p>\n
-00010fe0: 220a 223c 7020 7374 796c 653d 5c22 206d  "."<p style=\" m
-00010ff0: 6172 6769 6e2d 746f 703a 3070 783b 206d  argin-top:0px; m
-00011000: 6172 6769 6e2d 626f 7474 6f6d 3a30 7078  argin-bottom:0px
-00011010: 3b20 6d61 7267 696e 2d6c 6566 743a 3070  ; margin-left:0p
-00011020: 783b 206d 6172 6769 6e2d 7269 6768 743a  x; margin-right:
-00011030: 3070 783b 202d 7174 2d62 6c6f 636b 2d69  0px; -qt-block-i
-00011040: 6e64 656e 743a 303b 2074 6578 742d 696e  ndent:0; text-in
-00011050: 6465 6e74 3a30 7078 3b5c 223e 3c73 7061  dent:0px;\"><spa
-00011060: 6e20 7374 796c 653d 5c22 2074 6578 742d  n style=\" text-
-00011070: 6465 636f 7261 7469 6f6e 3a20 756e 6465  decoration: unde
-00011080: 726c 696e 653b 2063 6f6c 6f72 3a23 3030  rline; color:#00
-00011090: 3030 3030 3b5c 223e 312e 2042 7269 6566  0000;\">1. Brief
-000110a0: 2065 7870 6c61 6e61 7469 6f6e 206f 6620   explanation of 
-000110b0: 6d65 7468 6f64 6f6c 6f67 793c 2f73 7061  methodology</spa
-000110c0: 6e3e 3c2f 703e 5c6e 220a 223c 7020 7374  n></p>\n"."<p st
-000110d0: 796c 653d 5c22 206d 6172 6769 6e2d 746f  yle=\" margin-to
-000110e0: 703a 3070 783b 206d 6172 6769 6e2d 626f  p:0px; margin-bo
-000110f0: 7474 6f6d 3a30 7078 3b20 6d61 7267 696e  ttom:0px; margin
-00011100: 2d6c 6566 743a 3070 783b 206d 6172 6769  -left:0px; margi
-00011110: 6e2d 7269 6768 743a 3070 783b 202d 7174  n-right:0px; -qt
-00011120: 2d62 6c6f 636b 2d69 6e64 656e 743a 303b  -block-indent:0;
-00011130: 2074 6578 742d 696e 6465 6e74 3a30 7078   text-indent:0px
-00011140: 3b5c 223e 3c73 7061 6e20 7374 796c 653d  ;\"><span style=
-00011150: 5c22 2063 6f6c 6f72 3a23 3030 3030 3030  \" color:#000000
-00011160: 3b5c 223e 596f 7520 6361 6e20 6368 6f6f  ;\">You can choo
-00011170: 7365 2077 6869 6368 2070 6172 616d 6574  se which paramet
-00011180: 6572 2079 6f75 2075 7365 2066 6f72 2074  er you use for t
-00011190: 6865 2070 7269 6e63 6970 616c 2063 6f6d  he principal com
-000111a0: 706f 6e65 6e74 2061 6e61 6c79 7369 7320  ponent analysis 
-000111b0: 2850 4341 292e 3c2f 7370 616e 3e3c 2f70  (PCA).</span></p
-000111c0: 3e5c 6e22 0a22 3c70 2073 7479 6c65 3d5c  >\n"."<p style=\
-000111d0: 2220 6d61 7267 696e 2d74 6f70 3a30 7078  " margin-top:0px
-000111e0: 3b20 6d61 7267 696e 2d62 6f74 746f 6d3a  ; margin-bottom:
-000111f0: 3070 783b 206d 6172 6769 6e2d 6c65 6674  0px; margin-left
-00011200: 3a30 7078 3b20 6d61 7267 696e 2d72 6967  :0px; margin-rig
-00011210: 6874 3a30 7078 3b20 2d71 742d 626c 6f63  ht:0px; -qt-bloc
-00011220: 6b2d 696e 6465 6e74 3a30 3b20 7465 7874  k-indent:0; text
-00011230: 2d69 6e64 656e 743a 3070 783b 5c22 3e3c  -indent:0px;\"><
-00011240: 7370 616e 2073 7479 6c65 3d5c 2220 636f  span style=\" co
-00011250: 6c6f 723a 2330 3030 3030 303b 5c22 3e54  lor:#000000;\">T
-00011260: 6865 7265 2061 7265 2074 6872 6565 206f  here are three o
-00011270: 7074 696f 6e73 3a20 4650 532c 2041 6d70  ptions: FPS, Amp
-00011280: 6c69 7475 6465 7320 6f66 2048 6172 6d6f  litudes of Harmo
-00011290: 6e69 6373 2061 6e64 2074 7261 6469 7469  nics and traditi
-000112a0: 6f6e 616c 2045 4644 2e3c 2f73 7061 6e3e  onal EFD.</span>
-000112b0: 3c2f 703e 5c6e 220a 223c 7020 7374 796c  </p>\n"."<p styl
-000112c0: 653d 5c22 2d71 742d 7061 7261 6772 6170  e=\"-qt-paragrap
-000112d0: 682d 7479 7065 3a65 6d70 7479 3b20 6d61  h-type:empty; ma
-000112e0: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
-000112f0: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
-00011300: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
-00011310: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
-00011320: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
-00011330: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
-00011340: 656e 743a 3070 783b 5c22 3e3c 6272 202f  ent:0px;\"><br /
-00011350: 3e3c 2f70 3e5c 6e22 0a22 3c70 2073 7479  ></p>\n"."<p sty
-00011360: 6c65 3d5c 2220 6d61 7267 696e 2d74 6f70  le=\" margin-top
-00011370: 3a30 7078 3b20 6d61 7267 696e 2d62 6f74  :0px; margin-bot
-00011380: 746f 6d3a 3070 783b 206d 6172 6769 6e2d  tom:0px; margin-
-00011390: 6c65 6674 3a30 7078 3b20 6d61 7267 696e  left:0px; margin
-000113a0: 2d72 6967 6874 3a30 7078 3b20 2d71 742d  -right:0px; -qt-
-000113b0: 626c 6f63 6b2d 696e 6465 6e74 3a30 3b20  block-indent:0; 
-000113c0: 7465 7874 2d69 6e64 656e 743a 3070 783b  text-indent:0px;
-000113d0: 5c22 3e3c 7370 616e 2073 7479 6c65 3d5c  \"><span style=\
-000113e0: 2220 636f 6c6f 723a 2330 3030 3030 303b  " color:#000000;
-000113f0: 5c22 3e46 6973 7420 6f66 2061 6c6c 2c20  \">Fist of all, 
-00011400: 7468 6520 7368 6170 6520 6f66 2073 616d  the shape of sam
-00011410: 706c 6573 2077 6572 6520 636f 6e76 6572  ples were conver
-00011420: 7465 6420 696e 746f 2074 6865 206e 756d  ted into the num
-00011430: 6572 6963 616c 2064 6174 6173 6574 2061  erical dataset a
-00011440: 7420 2671 756f 743b 496d 6167 6520 416e  t &quot;Image An
-00011450: 616c 7973 6973 2671 756f 743b 2073 6563  alysis&quot; sec
-00011460: 7469 6f6e 7320 6173 2045 4644 732e 3c2f  tions as EFDs.</
-00011470: 7370 616e 3e3c 2f70 3e5c 6e22 0a22 3c70  span></p>\n"."<p
-00011480: 2073 7479 6c65 3d5c 2220 6d61 7267 696e   style=\" margin
-00011490: 2d74 6f70 3a30 7078 3b20 6d61 7267 696e  -top:0px; margin
-000114a0: 2d62 6f74 746f 6d3a 3070 783b 206d 6172  -bottom:0px; mar
-000114b0: 6769 6e2d 6c65 6674 3a30 7078 3b20 6d61  gin-left:0px; ma
-000114c0: 7267 696e 2d72 6967 6874 3a30 7078 3b20  rgin-right:0px; 
-000114d0: 2d71 742d 626c 6f63 6b2d 696e 6465 6e74  -qt-block-indent
-000114e0: 3a30 3b20 7465 7874 2d69 6e64 656e 743a  :0; text-indent:
-000114f0: 3070 783b 5c22 3e3c 7370 616e 2073 7479  0px;\"><span sty
-00011500: 6c65 3d5c 2220 636f 6c6f 723a 2330 3030  le=\" color:#000
-00011510: 3030 303b 5c22 3e45 6163 6820 6f66 2079  000;\">Each of y
-00011520: 6f75 7220 7361 6d70 6c65 7320 7761 7320  our samples was 
-00011530: 6465 636f 6d70 6f73 6564 2069 6e74 6f20  decomposed into 
-00011540: 7468 6520 6861 726d 6f6e 6963 7320 656c  the harmonics el
-00011550: 6c69 7073 6573 206f 6620 7768 6963 6820  lipses of which 
-00011560: 746f 7461 6c20 6e75 6d62 6572 2069 7320  total number is 
-00011570: 3c2f 7370 616e 3e3c 7370 616e 2073 7479  </span><span sty
-00011580: 6c65 3d5c 2220 666f 6e74 2d73 7479 6c65  le=\" font-style
-00011590: 3a69 7461 6c69 633b 2063 6f6c 6f72 3a23  :italic; color:#
-000115a0: 3030 3030 3030 3b5c 223e 4e3c 2f73 7061  000000;\">N</spa
-000115b0: 6e3e 3c73 7061 6e20 7374 796c 653d 5c22  n><span style=\"
-000115c0: 2063 6f6c 6f72 3a23 3030 3030 3030 3b5c   color:#000000;\
-000115d0: 223e 2028 4d61 7869 6d75 6d20 6861 726d  "> (Maximum harm
-000115e0: 6f6e 6963 7320 6e75 6d62 6572 292e 3c2f  onics number).</
-000115f0: 7370 616e 3e3c 2f70 3e5c 6e22 0a22 3c70  span></p>\n"."<p
-00011600: 2073 7479 6c65 3d5c 2220 6d61 7267 696e   style=\" margin
-00011610: 2d74 6f70 3a30 7078 3b20 6d61 7267 696e  -top:0px; margin
-00011620: 2d62 6f74 746f 6d3a 3070 783b 206d 6172  -bottom:0px; mar
-00011630: 6769 6e2d 6c65 6674 3a30 7078 3b20 6d61  gin-left:0px; ma
-00011640: 7267 696e 2d72 6967 6874 3a30 7078 3b20  rgin-right:0px; 
-00011650: 2d71 742d 626c 6f63 6b2d 696e 6465 6e74  -qt-block-indent
-00011660: 3a30 3b20 7465 7874 2d69 6e64 656e 743a  :0; text-indent:
-00011670: 3070 783b 5c22 3e3c 7370 616e 2073 7479  0px;\"><span sty
-00011680: 6c65 3d5c 2220 636f 6c6f 723a 2330 3030  le=\" color:#000
-00011690: 3030 303b 5c22 3e45 6163 6820 6861 726d  000;\">Each harm
-000116a0: 6f6e 6963 7320 656c 6c69 7073 6573 2063  onics ellipses c
-000116b0: 616e 2062 6520 6465 7363 7269 6265 6420  an be described 
-000116c0: 7769 7468 2066 6f75 7220 636f 6e73 7461  with four consta
-000116d0: 6e74 2063 6f65 6666 6963 6965 6e74 7320  nt coefficients 
-000116e0: 3c2f 7370 616e 3e3c 7370 616e 2073 7479  </span><span sty
-000116f0: 6c65 3d5c 2220 666f 6e74 2d73 7479 6c65  le=\" font-style
-00011700: 3a69 7461 6c69 633b 2063 6f6c 6f72 3a23  :italic; color:#
-00011710: 3030 3030 3030 3b5c 223e 613c 2f73 7061  000000;\">a</spa
-00011720: 6e3e 3c73 7061 6e20 7374 796c 653d 5c22  n><span style=\"
-00011730: 2066 6f6e 742d 7374 796c 653a 6974 616c   font-style:ital
-00011740: 6963 3b20 636f 6c6f 723a 2330 3030 3030  ic; color:#00000
-00011750: 303b 2076 6572 7469 6361 6c2d 616c 6967  0; vertical-alig
-00011760: 6e3a 7375 623b 5c22 3e6e 3c2f 7370 616e  n:sub;\">n</span
-00011770: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
-00011780: 636f 6c6f 723a 2330 3030 3030 303b 5c22  color:#000000;\"
-00011790: 3e2c 203c 2f73 7061 6e3e 3c73 7061 6e20  >, </span><span 
-000117a0: 7374 796c 653d 5c22 2066 6f6e 742d 7374  style=\" font-st
-000117b0: 796c 653a 6974 616c 6963 3b20 636f 6c6f  yle:italic; colo
-000117c0: 723a 2330 3030 3030 303b 5c22 3e62 3c2f  r:#000000;\">b</
-000117d0: 7370 616e 3e3c 7370 616e 2073 7479 6c65  span><span style
-000117e0: 3d5c 2220 666f 6e74 2d73 7479 6c65 3a69  =\" font-style:i
-000117f0: 7461 6c69 633b 2063 6f6c 6f72 3a23 3030  talic; color:#00
-00011800: 3030 3030 3b20 7665 7274 6963 616c 2d61  0000; vertical-a
-00011810: 6c69 676e 3a73 7562 3b5c 223e 6e3c 2f73  lign:sub;\">n</s
-00011820: 7061 6e3e 3c73 7061 6e20 7374 796c 653d  pan><span style=
-00011830: 5c22 2063 6f6c 6f72 3a23 3030 3030 3030  \" color:#000000
-00011840: 3b5c 223e 2c20 3c2f 7370 616e 3e3c 7370  ;\">, </span><sp
-00011850: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
-00011860: 2d73 7479 6c65 3a69 7461 6c69 633b 2063  -style:italic; c
-00011870: 6f6c 6f72 3a23 3030 3030 3030 3b5c 223e  olor:#000000;\">
-00011880: 633c 2f73 7061 6e3e 3c73 7061 6e20 7374  c</span><span st
-00011890: 796c 653d 5c22 2066 6f6e 742d 7374 796c  yle=\" font-styl
-000118a0: 653a 6974 616c 6963 3b20 636f 6c6f 723a  e:italic; color:
-000118b0: 2330 3030 3030 303b 2076 6572 7469 6361  #000000; vertica
-000118c0: 6c2d 616c 6967 6e3a 7375 623b 5c22 3e6e  l-align:sub;\">n
-000118d0: 3c2f 7370 616e 3e3c 7370 616e 2073 7479  </span><span sty
-000118e0: 6c65 3d5c 2220 636f 6c6f 723a 2330 3030  le=\" color:#000
-000118f0: 3030 303b 5c22 3e20 616e 6420 3c2f 7370  000;\"> and </sp
-00011900: 616e 3e3c 7370 616e 2073 7479 6c65 3d5c  an><span style=\
-00011910: 2220 666f 6e74 2d73 7479 6c65 3a69 7461  " font-style:ita
-00011920: 6c69 633b 2063 6f6c 6f72 3a23 3030 3030  lic; color:#0000
-00011930: 3030 3b5c 223e 643c 2f73 7061 6e3e 3c73  00;\">d</span><s
-00011940: 7061 6e20 7374 796c 653d 5c22 2066 6f6e  pan style=\" fon
-00011950: 742d 7374 796c 653a 6974 616c 6963 3b20  t-style:italic; 
-00011960: 636f 6c6f 723a 2330 3030 3030 303b 2076  color:#000000; v
-00011970: 6572 7469 6361 6c2d 616c 6967 6e3a 7375  ertical-align:su
-00011980: 623b 5c22 3e6e 3c2f 7370 616e 3e3c 7370  b;\">n</span><sp
-00011990: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
-000119a0: 2d73 7479 6c65 3a69 7461 6c69 633b 2063  -style:italic; c
-000119b0: 6f6c 6f72 3a23 3030 3030 3030 3b5c 223e  olor:#000000;\">
-000119c0: 203c 2f73 7061 6e3e 3c73 7061 6e20 7374   </span><span st
-000119d0: 796c 653d 5c22 2063 6f6c 6f72 3a23 3030  yle=\" color:#00
-000119e0: 3030 3030 3b5c 223e 7768 6572 6520 3c2f  0000;\">where </
-000119f0: 7370 616e 3e3c 7370 616e 2073 7479 6c65  span><span style
-00011a00: 3d5c 2220 666f 6e74 2d73 7479 6c65 3a69  =\" font-style:i
-00011a10: 7461 6c69 633b 2063 6f6c 6f72 3a23 3030  talic; color:#00
-00011a20: 3030 3030 3b5c 223e 6e20 3c2f 7370 616e  0000;\">n </span
-00011a30: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
-00011a40: 636f 6c6f 723a 2330 3030 3030 303b 5c22  color:#000000;\"
-00011a50: 3e3d 3c2f 7370 616e 3e3c 7370 616e 2073  >=</span><span s
-00011a60: 7479 6c65 3d5c 2220 666f 6e74 2d73 7479  tyle=\" font-sty
-00011a70: 6c65 3a69 7461 6c69 633b 2063 6f6c 6f72  le:italic; color
-00011a80: 3a23 3030 3030 3030 3b5c 223e 312c 322c  :#000000;\">1,2,
-00011a90: 2e2e 2e4e 3c2f 7370 616e 3e3c 7370 616e  ...N</span><span
-00011aa0: 2073 7479 6c65 3d5c 2220 636f 6c6f 723a   style=\" color:
-00011ab0: 2330 3030 3030 303b 5c22 3e2e 2020 3c2f  #000000;\">.  </
-00011ac0: 7370 616e 3e3c 2f70 3e5c 6e22 0a22 3c70  span></p>\n"."<p
-00011ad0: 2073 7479 6c65 3d5c 2220 6d61 7267 696e   style=\" margin
-00011ae0: 2d74 6f70 3a30 7078 3b20 6d61 7267 696e  -top:0px; margin
-00011af0: 2d62 6f74 746f 6d3a 3070 783b 206d 6172  -bottom:0px; mar
-00011b00: 6769 6e2d 6c65 6674 3a30 7078 3b20 6d61  gin-left:0px; ma
-00011b10: 7267 696e 2d72 6967 6874 3a30 7078 3b20  rgin-right:0px; 
-00011b20: 2d71 742d 626c 6f63 6b2d 696e 6465 6e74  -qt-block-indent
-00011b30: 3a30 3b20 7465 7874 2d69 6e64 656e 743a  :0; text-indent:
-00011b40: 3070 783b 5c22 3e3c 7370 616e 2073 7479  0px;\"><span sty
-00011b50: 6c65 3d5c 2220 636f 6c6f 723a 2330 3030  le=\" color:#000
-00011b60: 3030 303b 5c22 3e54 6875 7320 6561 6368  000;\">Thus each
-00011b70: 2073 616d 706c 6520 6861 7320 3c2f 7370   sample has </sp
-00011b80: 616e 3e3c 7370 616e 2073 7479 6c65 3d5c  an><span style=\
-00011b90: 2220 666f 6e74 2d73 7479 6c65 3a69 7461  " font-style:ita
-00011ba0: 6c69 633b 2063 6f6c 6f72 3a23 3030 3030  lic; color:#0000
-00011bb0: 3030 3b5c 223e 342a 4e3c 2f73 7061 6e3e  00;\">4*N</span>
-00011bc0: 3c73 7061 6e20 7374 796c 653d 5c22 2063  <span style=\" c
-00011bd0: 6f6c 6f72 3a23 3030 3030 3030 3b5c 223e  olor:#000000;\">
-00011be0: 2063 6f65 6666 6963 6965 6e74 732e 3c2f   coefficients.</
-00011bf0: 7370 616e 3e3c 2f70 3e5c 6e22 0a22 3c70  span></p>\n"."<p
-00011c00: 2073 7479 6c65 3d5c 222d 7174 2d70 6172   style=\"-qt-par
-00011c10: 6167 7261 7068 2d74 7970 653a 656d 7074  agraph-type:empt
-00011c20: 793b 206d 6172 6769 6e2d 746f 703a 3070  y; margin-top:0p
-00011c30: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
-00011c40: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
-00011c50: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
-00011c60: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
-00011c70: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
-00011c80: 742d 696e 6465 6e74 3a30 7078 3b20 636f  t-indent:0px; co
-00011c90: 6c6f 723a 2330 3030 3030 303b 5c22 3e3c  lor:#000000;\"><
-00011ca0: 6272 202f 3e3c 2f70 3e5c 6e22 0a22 3c70  br /></p>\n"."<p
-00011cb0: 2073 7479 6c65 3d5c 2220 6d61 7267 696e   style=\" margin
-00011cc0: 2d74 6f70 3a30 7078 3b20 6d61 7267 696e  -top:0px; margin
-00011cd0: 2d62 6f74 746f 6d3a 3070 783b 206d 6172  -bottom:0px; mar
-00011ce0: 6769 6e2d 6c65 6674 3a30 7078 3b20 6d61  gin-left:0px; ma
-00011cf0: 7267 696e 2d72 6967 6874 3a30 7078 3b20  rgin-right:0px; 
-00011d00: 2d71 742d 626c 6f63 6b2d 696e 6465 6e74  -qt-block-indent
-00011d10: 3a30 3b20 7465 7874 2d69 6e64 656e 743a  :0; text-indent:
-00011d20: 3070 783b 5c22 3e3c 7370 616e 2073 7479  0px;\"><span sty
-00011d30: 6c65 3d5c 2220 666f 6e74 2d77 6569 6768  le=\" font-weigh
-00011d40: 743a 3630 303b 5c22 3e45 4644 203c 2f73  t:600;\">EFD </s
-00011d50: 7061 6e3e 2845 6c6c 6970 7469 6320 466f  pan>(Elliptic Fo
-00011d60: 7572 6965 7220 4465 7363 7269 7074 6f72  urier Descriptor
-00011d70: 293c 2f70 3e5c 6e22 0a22 3c70 2073 7479  )</p>\n"."<p sty
-00011d80: 6c65 3d5c 2220 6d61 7267 696e 2d74 6f70  le=\" margin-top
-00011d90: 3a30 7078 3b20 6d61 7267 696e 2d62 6f74  :0px; margin-bot
-00011da0: 746f 6d3a 3070 783b 206d 6172 6769 6e2d  tom:0px; margin-
-00011db0: 6c65 6674 3a30 7078 3b20 6d61 7267 696e  left:0px; margin
-00011dc0: 2d72 6967 6874 3a30 7078 3b20 2d71 742d  -right:0px; -qt-
-00011dd0: 626c 6f63 6b2d 696e 6465 6e74 3a30 3b20  block-indent:0; 
-00011de0: 7465 7874 2d69 6e64 656e 743a 3070 783b  text-indent:0px;
-00011df0: 5c22 3e54 6869 7320 6973 2074 7261 6469  \">This is tradi
-00011e00: 7469 6f6e 616c 2064 6573 6372 6970 746f  tional descripto
-00011e10: 7220 7768 6963 6820 636f 7272 6573 706f  r which correspo
-00011e20: 6e64 7320 746f 2065 6163 6820 636f 6566  nds to each coef
-00011e30: 6669 6369 656e 7420 6f66 2068 6172 6d6f  ficient of harmo
-00011e40: 6e69 6373 3a20 3c73 7061 6e20 7374 796c  nics: <span styl
-00011e50: 653d 5c22 2066 6f6e 742d 7374 796c 653a  e=\" font-style:
-00011e60: 6974 616c 6963 3b20 636f 6c6f 723a 2330  italic; color:#0
-00011e70: 3030 3030 303b 5c22 3e61 3c2f 7370 616e  00000;\">a</span
-00011e80: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
-00011e90: 666f 6e74 2d73 7479 6c65 3a69 7461 6c69  font-style:itali
-00011ea0: 633b 2063 6f6c 6f72 3a23 3030 3030 3030  c; color:#000000
-00011eb0: 3b20 7665 7274 6963 616c 2d61 6c69 676e  ; vertical-align
-00011ec0: 3a73 7562 3b5c 223e 6e3c 2f73 7061 6e3e  :sub;\">n</span>
-00011ed0: 3c73 7061 6e20 7374 796c 653d 5c22 2063  <span style=\" c
-00011ee0: 6f6c 6f72 3a23 3030 3030 3030 3b5c 223e  olor:#000000;\">
-00011ef0: 2c20 3c2f 7370 616e 3e3c 7370 616e 2073  , </span><span s
-00011f00: 7479 6c65 3d5c 2220 666f 6e74 2d73 7479  tyle=\" font-sty
-00011f10: 6c65 3a69 7461 6c69 633b 2063 6f6c 6f72  le:italic; color
-00011f20: 3a23 3030 3030 3030 3b5c 223e 623c 2f73  :#000000;\">b</s
-00011f30: 7061 6e3e 3c73 7061 6e20 7374 796c 653d  pan><span style=
-00011f40: 5c22 2066 6f6e 742d 7374 796c 653a 6974  \" font-style:it
-00011f50: 616c 6963 3b20 636f 6c6f 723a 2330 3030  alic; color:#000
-00011f60: 3030 303b 2076 6572 7469 6361 6c2d 616c  000; vertical-al
-00011f70: 6967 6e3a 7375 623b 5c22 3e6e 3c2f 7370  ign:sub;\">n</sp
-00011f80: 616e 3e3c 7370 616e 2073 7479 6c65 3d5c  an><span style=\
-00011f90: 2220 636f 6c6f 723a 2330 3030 3030 303b  " color:#000000;
-00011fa0: 5c22 3e2c 203c 2f73 7061 6e3e 3c73 7061  \">, </span><spa
-00011fb0: 6e20 7374 796c 653d 5c22 2066 6f6e 742d  n style=\" font-
-00011fc0: 7374 796c 653a 6974 616c 6963 3b20 636f  style:italic; co
-00011fd0: 6c6f 723a 2330 3030 3030 303b 5c22 3e63  lor:#000000;\">c
-00011fe0: 3c2f 7370 616e 3e3c 7370 616e 2073 7479  </span><span sty
-00011ff0: 6c65 3d5c 2220 666f 6e74 2d73 7479 6c65  le=\" font-style
-00012000: 3a69 7461 6c69 633b 2063 6f6c 6f72 3a23  :italic; color:#
-00012010: 3030 3030 3030 3b20 7665 7274 6963 616c  000000; vertical
-00012020: 2d61 6c69 676e 3a73 7562 3b5c 223e 6e3c  -align:sub;\">n<
-00012030: 2f73 7061 6e3e 3c73 7061 6e20 7374 796c  /span><span styl
-00012040: 653d 5c22 2063 6f6c 6f72 3a23 3030 3030  e=\" color:#0000
-00012050: 3030 3b5c 223e 2061 6e64 203c 2f73 7061  00;\"> and </spa
-00012060: 6e3e 3c73 7061 6e20 7374 796c 653d 5c22  n><span style=\"
-00012070: 2066 6f6e 742d 7374 796c 653a 6974 616c   font-style:ital
-00012080: 6963 3b20 636f 6c6f 723a 2330 3030 3030  ic; color:#00000
-00012090: 303b 5c22 3e64 3c2f 7370 616e 3e3c 7370  0;\">d</span><sp
-000120a0: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
-000120b0: 2d73 7479 6c65 3a69 7461 6c69 633b 2063  -style:italic; c
-000120c0: 6f6c 6f72 3a23 3030 3030 3030 3b20 7665  olor:#000000; ve
-000120d0: 7274 6963 616c 2d61 6c69 676e 3a73 7562  rtical-align:sub
-000120e0: 3b5c 223e 6e3c 2f73 7061 6e3e 3c2f 703e  ;\">n</span></p>
-000120f0: 5c6e 220a 223c 7020 7374 796c 653d 5c22  \n"."<p style=\"
-00012100: 206d 6172 6769 6e2d 746f 703a 3070 783b   margin-top:0px;
-00012110: 206d 6172 6769 6e2d 626f 7474 6f6d 3a30   margin-bottom:0
-00012120: 7078 3b20 6d61 7267 696e 2d6c 6566 743a  px; margin-left:
-00012130: 3070 783b 206d 6172 6769 6e2d 7269 6768  0px; margin-righ
-00012140: 743a 3070 783b 202d 7174 2d62 6c6f 636b  t:0px; -qt-block
-00012150: 2d69 6e64 656e 743a 303b 2074 6578 742d  -indent:0; text-
-00012160: 696e 6465 6e74 3a30 7078 3b5c 223e 4546  indent:0px;\">EF
-00012170: 442d 6261 7365 6420 5043 4120 6973 2073  D-based PCA is s
-00012180: 7569 7462 6c65 2066 6f72 2064 6972 6563  uitble for direc
-00012190: 7469 6f6e 616c 2064 6174 6120 7375 6368  tional data such
-000121a0: 2061 7320 666f 7373 696c 7320 616e 6420   as fossils and 
-000121b0: 6f74 6865 7220 6f72 6761 6e69 6320 6d61  other organic ma
-000121c0: 7474 6572 7320 2873 6565 204b 7568 6c20  tters (see Kuhl 
-000121d0: 616e 6420 4769 6172 6469 6e61 2031 3938  and Giardina 198
-000121e0: 3229 202e 2020 484f 5745 5645 522c 2069  2) .  HOWEVER, i
-000121f0: 6e20 7468 6520 6361 7365 206f 6620 6e6f  n the case of no
-00012200: 6e2d 6469 7265 6374 696f 6e61 6c20 6461  n-directional da
-00012210: 7461 7365 7420 7375 6368 2061 7320 6772  taset such as gr
-00012220: 6169 6e73 2c20 4546 442d 6261 7365 6420  ains, EFD-based 
-00012230: 5043 4120 6f66 7465 6e20 646f 206e 6f74  PCA often do not
-00012240: 2077 6f72 6b20 7765 6c6c 2e20 3c2f 703e   work well. </p>
-00012250: 5c6e 220a 223c 7020 7374 796c 653d 5c22  \n"."<p style=\"
-00012260: 206d 6172 6769 6e2d 746f 703a 3070 783b   margin-top:0px;
-00012270: 206d 6172 6769 6e2d 626f 7474 6f6d 3a30   margin-bottom:0
-00012280: 7078 3b20 6d61 7267 696e 2d6c 6566 743a  px; margin-left:
-00012290: 3070 783b 206d 6172 6769 6e2d 7269 6768  0px; margin-righ
-000122a0: 743a 3070 783b 202d 7174 2d62 6c6f 636b  t:0px; -qt-block
-000122b0: 2d69 6e64 656e 743a 303b 2074 6578 742d  -indent:0; text-
-000122c0: 696e 6465 6e74 3a30 7078 3b5c 223e 5468  indent:0px;\">Th
-000122d0: 6973 2069 7320 6265 6361 7573 6520 4546  is is because EF
-000122e0: 442d 6261 7365 6420 5043 4120 6f66 7465  D-based PCA ofte
-000122f0: 6e20 656e 6473 2075 7020 2063 6f6e 636c  n ends up  concl
-00012300: 7564 696e 6720 7468 6174 2074 6865 2073  uding that the s
-00012310: 6861 7065 2076 6172 6961 7469 6f6e 2069  hape variation i
-00012320: 7320 7375 6d6d 6172 697a 6564 2062 7920  s summarized by 
-00012330: 6d69 7272 6f72 2073 796d 6d65 7472 6963  mirror symmetric
-00012340: 2070 726f 7065 7274 6965 7320 7768 6963   properties whic
-00012350: 682c 2069 6e20 6d6f 7374 2063 6173 6573  h, in most cases
-00012360: 2c20 6861 7665 206e 6f20 7363 6965 6e74  , have no scient
-00012370: 6966 6963 2069 6e74 6572 6573 7420 6f66  ific interest of
-00012380: 2070 6172 7469 636c 6520 7368 6170 6573   particle shapes
-00012390: 2e3c 2f70 3e5c 6e22 0a22 3c70 2073 7479  .</p>\n"."<p sty
-000123a0: 6c65 3d5c 222d 7174 2d70 6172 6167 7261  le=\"-qt-paragra
-000123b0: 7068 2d74 7970 653a 656d 7074 793b 206d  ph-type:empty; m
-000123c0: 6172 6769 6e2d 746f 703a 3070 783b 206d  argin-top:0px; m
-000123d0: 6172 6769 6e2d 626f 7474 6f6d 3a30 7078  argin-bottom:0px
-000123e0: 3b20 6d61 7267 696e 2d6c 6566 743a 3070  ; margin-left:0p
-000123f0: 783b 206d 6172 6769 6e2d 7269 6768 743a  x; margin-right:
-00012400: 3070 783b 202d 7174 2d62 6c6f 636b 2d69  0px; -qt-block-i
-00012410: 6e64 656e 743a 303b 2074 6578 742d 696e  ndent:0; text-in
-00012420: 6465 6e74 3a30 7078 3b20 636f 6c6f 723a  dent:0px; color:
-00012430: 2330 3030 3030 303b 5c22 3e3c 6272 202f  #000000;\"><br /
-00012440: 3e3c 2f70 3e5c 6e22 0a22 3c70 2073 7479  ></p>\n"."<p sty
-00012450: 6c65 3d5c 2220 6d61 7267 696e 2d74 6f70  le=\" margin-top
-00012460: 3a30 7078 3b20 6d61 7267 696e 2d62 6f74  :0px; margin-bot
-00012470: 746f 6d3a 3070 783b 206d 6172 6769 6e2d  tom:0px; margin-
-00012480: 6c65 6674 3a30 7078 3b20 6d61 7267 696e  left:0px; margin
-00012490: 2d72 6967 6874 3a30 7078 3b20 2d71 742d  -right:0px; -qt-
-000124a0: 626c 6f63 6b2d 696e 6465 6e74 3a30 3b20  block-indent:0; 
-000124b0: 7465 7874 2d69 6e64 656e 743a 3070 783b  text-indent:0px;
-000124c0: 5c22 3e3c 7370 616e 2073 7479 6c65 3d5c  \"><span style=\
-000124d0: 2220 666f 6e74 2d77 6569 6768 743a 3630  " font-weight:60
-000124e0: 303b 5c22 3e46 5053 3c2f 7370 616e 3e20  0;\">FPS</span> 
-000124f0: 2846 6f75 7269 6572 2050 6f77 6572 2053  (Fourier Power S
-00012500: 7065 6374 7261 293c 2f70 3e5c 6e22 0a22  pectra)</p>\n"."
-00012510: 3c70 2073 7479 6c65 3d5c 2220 6d61 7267  <p style=\" marg
-00012520: 696e 2d74 6f70 3a30 7078 3b20 6d61 7267  in-top:0px; marg
-00012530: 696e 2d62 6f74 746f 6d3a 3070 783b 206d  in-bottom:0px; m
-00012540: 6172 6769 6e2d 6c65 6674 3a30 7078 3b20  argin-left:0px; 
-00012550: 6d61 7267 696e 2d72 6967 6874 3a30 7078  margin-right:0px
-00012560: 3b20 2d71 742d 626c 6f63 6b2d 696e 6465  ; -qt-block-inde
-00012570: 6e74 3a30 3b20 7465 7874 2d69 6e64 656e  nt:0; text-inden
-00012580: 743a 3070 783b 5c22 3e49 7420 636f 7272  t:0px;\">It corr
-00012590: 6573 706f 6e64 7320 746f 2074 6865 6861  esponds to theha
-000125a0: 6c66 206f 6620 7375 6d20 6f66 2073 7175  lf of sum of squ
-000125b0: 6172 6573 206f 6620 4546 4473 3a20 4650  ares of EFDs: FP
-000125c0: 533c 7370 616e 2073 7479 6c65 3d5c 2220  S<span style=\" 
-000125d0: 7665 7274 6963 616c 2d61 6c69 676e 3a73  vertical-align:s
-000125e0: 7562 3b5c 223e 6e3c 2f73 7061 6e3e 203d  ub;\">n</span> =
-000125f0: 2028 3c73 7061 6e20 7374 796c 653d 5c22   (<span style=\"
-00012600: 2066 6f6e 742d 7374 796c 653a 6974 616c   font-style:ital
-00012610: 6963 3b20 636f 6c6f 723a 2330 3030 3030  ic; color:#00000
-00012620: 303b 5c22 3e61 3c2f 7370 616e 3e3c 7370  0;\">a</span><sp
-00012630: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
-00012640: 2d73 7479 6c65 3a69 7461 6c69 633b 2063  -style:italic; c
-00012650: 6f6c 6f72 3a23 3030 3030 3030 3b20 7665  olor:#000000; ve
-00012660: 7274 6963 616c 2d61 6c69 676e 3a73 7562  rtical-align:sub
-00012670: 3b5c 223e 6e3c 2f73 7061 6e3e 3c73 7061  ;\">n</span><spa
-00012680: 6e20 7374 796c 653d 5c22 2063 6f6c 6f72  n style=\" color
-00012690: 3a23 3030 3030 3030 3b5c 223e 2c5e 3220  :#000000;\">,^2 
-000126a0: 2b20 3c2f 7370 616e 3e3c 7370 616e 2073  + </span><span s
-000126b0: 7479 6c65 3d5c 2220 666f 6e74 2d73 7479  tyle=\" font-sty
-000126c0: 6c65 3a69 7461 6c69 633b 2063 6f6c 6f72  le:italic; color
-000126d0: 3a23 3030 3030 3030 3b5c 223e 623c 2f73  :#000000;\">b</s
-000126e0: 7061 6e3e 3c73 7061 6e20 7374 796c 653d  pan><span style=
-000126f0: 5c22 2066 6f6e 742d 7374 796c 653a 6974  \" font-style:it
-00012700: 616c 6963 3b20 636f 6c6f 723a 2330 3030  alic; color:#000
-00012710: 3030 303b 2076 6572 7469 6361 6c2d 616c  000; vertical-al
-00012720: 6967 6e3a 7375 623b 5c22 3e6e 3c2f 7370  ign:sub;\">n</sp
-00012730: 616e 3e3c 7370 616e 2073 7479 6c65 3d5c  an><span style=\
-00012740: 2220 636f 6c6f 723a 2330 3030 3030 303b  " color:#000000;
-00012750: 5c22 3e5e 3220 2b20 3c2f 7370 616e 3e3c  \">^2 + </span><
-00012760: 7370 616e 2073 7479 6c65 3d5c 2220 666f  span style=\" fo
-00012770: 6e74 2d73 7479 6c65 3a69 7461 6c69 633b  nt-style:italic;
-00012780: 2063 6f6c 6f72 3a23 3030 3030 3030 3b5c   color:#000000;\
-00012790: 223e 633c 2f73 7061 6e3e 3c73 7061 6e20  ">c</span><span 
-000127a0: 7374 796c 653d 5c22 2066 6f6e 742d 7374  style=\" font-st
-000127b0: 796c 653a 6974 616c 6963 3b20 636f 6c6f  yle:italic; colo
-000127c0: 723a 2330 3030 3030 303b 2076 6572 7469  r:#000000; verti
-000127d0: 6361 6c2d 616c 6967 6e3a 7375 623b 5c22  cal-align:sub;\"
-000127e0: 3e6e 3c2f 7370 616e 3e3c 7370 616e 2073  >n</span><span s
-000127f0: 7479 6c65 3d5c 2220 636f 6c6f 723a 2330  tyle=\" color:#0
-00012800: 3030 3030 303b 5c22 3e5e 3220 2b20 3c2f  00000;\">^2 + </
-00012810: 7370 616e 3e3c 7370 616e 2073 7479 6c65  span><span style
-00012820: 3d5c 2220 666f 6e74 2d73 7479 6c65 3a69  =\" font-style:i
-00012830: 7461 6c69 633b 2063 6f6c 6f72 3a23 3030  talic; color:#00
-00012840: 3030 3030 3b5c 223e 643c 2f73 7061 6e3e  0000;\">d</span>
-00012850: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
-00012860: 6f6e 742d 7374 796c 653a 6974 616c 6963  ont-style:italic
-00012870: 3b20 636f 6c6f 723a 2330 3030 3030 303b  ; color:#000000;
-00012880: 2076 6572 7469 6361 6c2d 616c 6967 6e3a   vertical-align:
-00012890: 7375 623b 5c22 3e6e 3c2f 7370 616e 3e3c  sub;\">n</span><
-000128a0: 7370 616e 2073 7479 6c65 3d5c 2220 636f  span style=\" co
-000128b0: 6c6f 723a 2330 3030 3030 303b 5c22 3e5e  lor:#000000;\">^
-000128c0: 323c 2f73 7061 6e3e 292f 322e 2054 6869  2</span>)/2. Thi
-000128d0: 7320 7061 7261 6d65 7465 7273 206e 6f20  s parameters no 
-000128e0: 6c6f 6e67 6572 2068 6176 6520 7468 6520  longer have the 
-000128f0: 696e 666f 726d 6174 696f 6e20 6f66 2070  information of p
-00012900: 6861 7365 2073 6869 6674 206f 6620 6561  hase shift of ea
-00012910: 6368 2068 6172 6d6f 6e69 6373 2065 6c6c  ch harmonics ell
-00012920: 6970 7365 7320 616e 6420 736f 6c76 6520  ipses and solve 
-00012930: 7468 6520 2671 756f 743b 6d69 7272 6f72  the &quot;mirror
-00012940: 2d73 796d 6d65 7472 6963 2070 726f 7065  -symmetric prope
-00012950: 7274 7926 7175 6f74 3b20 7072 6f62 6c65  rty&quot; proble
-00012960: 6d73 2e3c 2f70 3e5c 6e22 0a22 3c70 2073  ms.</p>\n"."<p s
-00012970: 7479 6c65 3d5c 222d 7174 2d70 6172 6167  tyle=\"-qt-parag
-00012980: 7261 7068 2d74 7970 653a 656d 7074 793b  raph-type:empty;
-00012990: 206d 6172 6769 6e2d 746f 703a 3070 783b   margin-top:0px;
-000129a0: 206d 6172 6769 6e2d 626f 7474 6f6d 3a30   margin-bottom:0
-000129b0: 7078 3b20 6d61 7267 696e 2d6c 6566 743a  px; margin-left:
-000129c0: 3070 783b 206d 6172 6769 6e2d 7269 6768  0px; margin-righ
-000129d0: 743a 3070 783b 202d 7174 2d62 6c6f 636b  t:0px; -qt-block
-000129e0: 2d69 6e64 656e 743a 303b 2074 6578 742d  -indent:0; text-
-000129f0: 696e 6465 6e74 3a30 7078 3b5c 223e 3c62  indent:0px;\"><b
-00012a00: 7220 2f3e 3c2f 703e 5c6e 220a 223c 7020  r /></p>\n"."<p 
-00012a10: 7374 796c 653d 5c22 206d 6172 6769 6e2d  style=\" margin-
-00012a20: 746f 703a 3070 783b 206d 6172 6769 6e2d  top:0px; margin-
-00012a30: 626f 7474 6f6d 3a30 7078 3b20 6d61 7267  bottom:0px; marg
-00012a40: 696e 2d6c 6566 743a 3070 783b 206d 6172  in-left:0px; mar
-00012a50: 6769 6e2d 7269 6768 743a 3070 783b 202d  gin-right:0px; -
-00012a60: 7174 2d62 6c6f 636b 2d69 6e64 656e 743a  qt-block-indent:
-00012a70: 303b 2074 6578 742d 696e 6465 6e74 3a30  0; text-indent:0
-00012a80: 7078 3b5c 223e 3c73 7061 6e20 7374 796c  px;\"><span styl
-00012a90: 653d 5c22 2066 6f6e 742d 7765 6967 6874  e=\" font-weight
-00012aa0: 3a36 3030 3b5c 223e 416d 706c 6974 7564  :600;\">Amplitud
-00012ab0: 6520 6261 7365 643c 2f73 7061 6e3e 3c2f  e based</span></
-00012ac0: 703e 5c6e 220a 223c 7020 7374 796c 653d  p>\n"."<p style=
-00012ad0: 5c22 206d 6172 6769 6e2d 746f 703a 3070  \" margin-top:0p
-00012ae0: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
-00012af0: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
-00012b00: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
-00012b10: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
-00012b20: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
-00012b30: 742d 696e 6465 6e74 3a30 7078 3b5c 223e  t-indent:0px;\">
-00012b40: 4974 2063 6f72 7265 7370 6f6e 6473 2074  It corresponds t
-00012b50: 6f20 7468 6520 616d 706c 6974 7564 6520  o the amplitude 
-00012b60: 6f66 2074 6865 2065 6163 6820 6861 726d  of the each harm
-00012b70: 6f6e 6963 7320 696e 2074 6572 6d73 206f  onics in terms o
-00012b80: 6620 582d 636f 6f72 6469 6e61 7465 2061  f X-coordinate a
-00012b90: 6e64 2059 2d63 6f6f 7264 696e 6174 6520  nd Y-coordinate 
-00012ba0: 7265 7370 6563 7469 7665 6c79 2e3c 2f70  respectively.</p
-00012bb0: 3e5c 6e22 0a22 3c70 2073 7479 6c65 3d5c  >\n"."<p style=\
-00012bc0: 2220 6d61 7267 696e 2d74 6f70 3a30 7078  " margin-top:0px
-00012bd0: 3b20 6d61 7267 696e 2d62 6f74 746f 6d3a  ; margin-bottom:
-00012be0: 3070 783b 206d 6172 6769 6e2d 6c65 6674  0px; margin-left
-00012bf0: 3a30 7078 3b20 6d61 7267 696e 2d72 6967  :0px; margin-rig
-00012c00: 6874 3a30 7078 3b20 2d71 742d 626c 6f63  ht:0px; -qt-bloc
-00012c10: 6b2d 696e 6465 6e74 3a30 3b20 7465 7874  k-indent:0; text
-00012c20: 2d69 6e64 656e 743a 3070 783b 5c22 3e49  -indent:0px;\">I
-00012c30: 7420 6973 2067 6976 656e 2062 7920 583c  t is given by X<
-00012c40: 7370 616e 2073 7479 6c65 3d5c 2220 7665  span style=\" ve
-00012c50: 7274 6963 616c 2d61 6c69 676e 3a73 7562  rtical-align:sub
-00012c60: 3b5c 223e 616d 3c2f 7370 616e 3e20 3d20  ;\">am</span> = 
-00012c70: 283c 7370 616e 2073 7479 6c65 3d5c 2220  (<span style=\" 
-00012c80: 666f 6e74 2d73 7479 6c65 3a69 7461 6c69  font-style:itali
-00012c90: 633b 2063 6f6c 6f72 3a23 3030 3030 3030  c; color:#000000
-00012ca0: 3b5c 223e 613c 2f73 7061 6e3e 3c73 7061  ;\">a</span><spa
-00012cb0: 6e20 7374 796c 653d 5c22 2066 6f6e 742d  n style=\" font-
-00012cc0: 7374 796c 653a 6974 616c 6963 3b20 636f  style:italic; co
-00012cd0: 6c6f 723a 2330 3030 3030 303b 2076 6572  lor:#000000; ver
-00012ce0: 7469 6361 6c2d 616c 6967 6e3a 7375 623b  tical-align:sub;
-00012cf0: 5c22 3e6e 3c2f 7370 616e 3e3c 7370 616e  \">n</span><span
-00012d00: 2073 7479 6c65 3d5c 2220 636f 6c6f 723a   style=\" color:
-00012d10: 2330 3030 3030 303b 5c22 3e2c 5e32 202b  #000000;\">,^2 +
-00012d20: 203c 2f73 7061 6e3e 3c73 7061 6e20 7374   </span><span st
-00012d30: 796c 653d 5c22 2066 6f6e 742d 7374 796c  yle=\" font-styl
-00012d40: 653a 6974 616c 6963 3b20 636f 6c6f 723a  e:italic; color:
-00012d50: 2330 3030 3030 303b 5c22 3e62 3c2f 7370  #000000;\">b</sp
-00012d60: 616e 3e3c 7370 616e 2073 7479 6c65 3d5c  an><span style=\
-00012d70: 2220 666f 6e74 2d73 7479 6c65 3a69 7461  " font-style:ita
-00012d80: 6c69 633b 2063 6f6c 6f72 3a23 3030 3030  lic; color:#0000
-00012d90: 3030 3b20 7665 7274 6963 616c 2d61 6c69  00; vertical-ali
-00012da0: 676e 3a73 7562 3b5c 223e 6e3c 2f73 7061  gn:sub;\">n</spa
-00012db0: 6e3e 3c73 7061 6e20 7374 796c 653d 5c22  n><span style=\"
-00012dc0: 2063 6f6c 6f72 3a23 3030 3030 3030 3b5c   color:#000000;\
-00012dd0: 223e 5e32 2920 2f32 202c 203c 2f73 7061  ">^2) /2 , </spa
-00012de0: 6e3e 2059 3c73 7061 6e20 7374 796c 653d  n> Y<span style=
-00012df0: 5c22 2076 6572 7469 6361 6c2d 616c 6967  \" vertical-alig
-00012e00: 6e3a 7375 623b 5c22 3e61 6d3c 2f73 7061  n:sub;\">am</spa
-00012e10: 6e3e 203d 2028 633c 7370 616e 2073 7479  n> = (c<span sty
-00012e20: 6c65 3d5c 2220 666f 6e74 2d73 7479 6c65  le=\" font-style
-00012e30: 3a69 7461 6c69 633b 2063 6f6c 6f72 3a23  :italic; color:#
-00012e40: 3030 3030 3030 3b20 7665 7274 6963 616c  000000; vertical
-00012e50: 2d61 6c69 676e 3a73 7562 3b5c 223e 6e3c  -align:sub;\">n<
-00012e60: 2f73 7061 6e3e 3c73 7061 6e20 7374 796c  /span><span styl
-00012e70: 653d 5c22 2063 6f6c 6f72 3a23 3030 3030  e=\" color:#0000
-00012e80: 3030 3b5c 223e 2c5e 3220 2b20 643c 2f73  00;\">,^2 + d</s
-00012e90: 7061 6e3e 3c73 7061 6e20 7374 796c 653d  pan><span style=
-00012ea0: 5c22 2066 6f6e 742d 7374 796c 653a 6974  \" font-style:it
-00012eb0: 616c 6963 3b20 636f 6c6f 723a 2330 3030  alic; color:#000
-00012ec0: 3030 303b 2076 6572 7469 6361 6c2d 616c  000; vertical-al
-00012ed0: 6967 6e3a 7375 623b 5c22 3e6e 3c2f 7370  ign:sub;\">n</sp
-00012ee0: 616e 3e3c 7370 616e 2073 7479 6c65 3d5c  an><span style=\
-00012ef0: 2220 636f 6c6f 723a 2330 3030 3030 303b  " color:#000000;
-00012f00: 5c22 3e5e 3229 202f 323c 2f73 7061 6e3e  \">^2) /2</span>
-00012f10: 3c2f 703e 5c6e 220a 223c 7020 7374 796c  </p>\n"."<p styl
-00012f20: 653d 5c22 206d 6172 6769 6e2d 746f 703a  e=\" margin-top:
-00012f30: 3070 783b 206d 6172 6769 6e2d 626f 7474  0px; margin-bott
-00012f40: 6f6d 3a30 7078 3b20 6d61 7267 696e 2d6c  om:0px; margin-l
-00012f50: 6566 743a 3070 783b 206d 6172 6769 6e2d  eft:0px; margin-
-00012f60: 7269 6768 743a 3070 783b 202d 7174 2d62  right:0px; -qt-b
-00012f70: 6c6f 636b 2d69 6e64 656e 743a 303b 2074  lock-indent:0; t
-00012f80: 6578 742d 696e 6465 6e74 3a30 7078 3b5c  ext-indent:0px;\
-00012f90: 223e 3c73 7061 6e20 7374 796c 653d 5c22  "><span style=\"
-00012fa0: 2063 6f6c 6f72 3a23 3030 3030 3030 3b5c   color:#000000;\
-00012fb0: 223e 5468 6973 2061 6c73 6f20 736f 6c76  ">This also solv
-00012fc0: 6573 203c 2f73 7061 6e3e 2671 756f 743b  es </span>&quot;
-00012fd0: 6d69 7272 6f72 2d73 796d 6d65 7472 6963  mirror-symmetric
-00012fe0: 2070 726f 7065 7274 7926 7175 6f74 3b20   property&quot; 
-00012ff0: 7072 6f62 6c65 6d73 2e3c 2f70 3e5c 6e22  problems.</p>\n"
-00013000: 0a22 3c70 2073 7479 6c65 3d5c 222d 7174  ."<p style=\"-qt
-00013010: 2d70 6172 6167 7261 7068 2d74 7970 653a  -paragraph-type:
-00013020: 656d 7074 793b 206d 6172 6769 6e2d 746f  empty; margin-to
-00013030: 703a 3070 783b 206d 6172 6769 6e2d 626f  p:0px; margin-bo
-00013040: 7474 6f6d 3a30 7078 3b20 6d61 7267 696e  ttom:0px; margin
-00013050: 2d6c 6566 743a 3070 783b 206d 6172 6769  -left:0px; margi
-00013060: 6e2d 7269 6768 743a 3070 783b 202d 7174  n-right:0px; -qt
-00013070: 2d62 6c6f 636b 2d69 6e64 656e 743a 303b  -block-indent:0;
-00013080: 2074 6578 742d 696e 6465 6e74 3a30 7078   text-indent:0px
-00013090: 3b5c 223e 3c62 7220 2f3e 3c2f 703e 5c6e  ;\"><br /></p>\n
-000130a0: 220a 223c 7020 7374 796c 653d 5c22 206d  "."<p style=\" m
-000130b0: 6172 6769 6e2d 746f 703a 3070 783b 206d  argin-top:0px; m
-000130c0: 6172 6769 6e2d 626f 7474 6f6d 3a30 7078  argin-bottom:0px
-000130d0: 3b20 6d61 7267 696e 2d6c 6566 743a 3070  ; margin-left:0p
-000130e0: 783b 206d 6172 6769 6e2d 7269 6768 743a  x; margin-right:
-000130f0: 3070 783b 202d 7174 2d62 6c6f 636b 2d69  0px; -qt-block-i
-00013100: 6e64 656e 743a 303b 2074 6578 742d 696e  ndent:0; text-in
-00013110: 6465 6e74 3a30 7078 3b5c 223e 232d 2d2d  dent:0px;\">#---
-00013120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3c2f  --------------</
-00013140: 703e 5c6e 220a 223c 7020 7374 796c 653d  p>\n"."<p style=
-00013150: 5c22 2d71 742d 7061 7261 6772 6170 682d  \"-qt-paragraph-
-00013160: 7479 7065 3a65 6d70 7479 3b20 6d61 7267  type:empty; marg
-00013170: 696e 2d74 6f70 3a30 7078 3b20 6d61 7267  in-top:0px; marg
-00013180: 696e 2d62 6f74 746f 6d3a 3070 783b 206d  in-bottom:0px; m
-00013190: 6172 6769 6e2d 6c65 6674 3a30 7078 3b20  argin-left:0px; 
-000131a0: 6d61 7267 696e 2d72 6967 6874 3a30 7078  margin-right:0px
-000131b0: 3b20 2d71 742d 626c 6f63 6b2d 696e 6465  ; -qt-block-inde
-000131c0: 6e74 3a30 3b20 7465 7874 2d69 6e64 656e  nt:0; text-inden
-000131d0: 743a 3070 783b 5c22 3e3c 6272 202f 3e3c  t:0px;\"><br /><
-000131e0: 2f70 3e3c 2f62 6f64 793e 3c2f 6874 6d6c  /p></body></html
-000131f0: 3e22 2929 0a20 2020 2020 2020 2073 656c  >")).        sel
-00013200: 662e 7461 625f 7063 612e 7365 7454 6162  f.tab_pca.setTab
-00013210: 5465 7874 2873 656c 662e 7461 625f 7063  Text(self.tab_pc
-00013220: 612e 696e 6465 784f 6628 7365 6c66 2e74  a.indexOf(self.t
-00013230: 6162 5f34 292c 205f 7472 616e 736c 6174  ab_4), _translat
-00013240: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00013250: 224c 6f67 2229 290a 2020 2020 2020 2020  "Log")).        
-00013260: 7365 6c66 2e6c 6162 656c 5f31 352e 7365  self.label_15.se
-00013270: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
-00013280: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00013290: 5043 4120 7375 6d6d 6172 7922 2929 0a20  PCA summary")). 
-000132a0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-000132b0: 6c5f 3136 2e73 6574 5465 7874 285f 7472  l_16.setText(_tr
-000132c0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-000132d0: 646f 7722 2c20 2250 4341 2065 6967 656e  dow", "PCA eigen
-000132e0: 2076 6563 746f 7222 2929 0a20 2020 2020   vector")).     
-000132f0: 2020 2073 656c 662e 7461 625f 7063 612e     self.tab_pca.
-00013300: 7365 7454 6162 5465 7874 2873 656c 662e  setTabText(self.
-00013310: 7461 625f 7063 612e 696e 6465 784f 6628  tab_pca.indexOf(
-00013320: 7365 6c66 2e74 6e5f 7375 6d6d 6172 7929  self.tn_summary)
-00013330: 2c20 5f74 7261 6e73 6c61 7465 2822 4d61  , _translate("Ma
-00013340: 696e 5769 6e64 6f77 222c 2022 5375 6d6d  inWindow", "Summ
-00013350: 6172 7922 2929 0a20 2020 2020 2020 2073  ary")).        s
-00013360: 656c 662e 7461 625f 7063 612e 7365 7454  elf.tab_pca.setT
-00013370: 6162 5465 7874 2873 656c 662e 7461 625f  abText(self.tab_
-00013380: 7063 612e 696e 6465 784f 6628 7365 6c66  pca.indexOf(self
-00013390: 2e74 6e5f 6772 6170 6829 2c20 5f74 7261  .tn_graph), _tra
-000133a0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-000133b0: 6f77 222c 2022 4772 6170 6822 2929 0a20  ow", "Graph")). 
-000133c0: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
-000133d0: 6964 6765 742e 7365 7454 6162 5465 7874  idget.setTabText
-000133e0: 2873 656c 662e 7461 6257 6964 6765 742e  (self.tabWidget.
-000133f0: 696e 6465 784f 6628 7365 6c66 2e74 6162  indexOf(self.tab
-00013400: 5f32 292c 205f 7472 616e 736c 6174 6528  _2), _translate(
-00013410: 224d 6169 6e57 696e 646f 7722 2c20 2250  "MainWindow", "P
-00013420: 4341 2229 290a 2020 2020 2020 2020 7365  CA")).        se
-00013430: 6c66 2e6c 6162 656c 5f33 362e 7365 7454  lf.label_36.setT
-00013440: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-00013450: 4d61 696e 5769 6e64 6f77 222c 2022 5368  MainWindow", "Sh
-00013460: 6170 6520 5265 636f 6e73 742e 2229 290a  ape Reconst.")).
-00013470: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
-00013480: 5f72 6563 5479 7065 2e73 6574 4974 656d  _recType.setItem
-00013490: 5465 7874 2830 2c20 5f74 7261 6e73 6c61  Text(0, _transla
-000134a0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-000134b0: 2022 5375 6d6d 6172 7922 2929 0a20 2020   "Summary")).   
-000134c0: 2020 2020 2073 656c 662e 636d 625f 7265       self.cmb_re
-000134d0: 6354 7970 652e 7365 7449 7465 6d54 6578  cType.setItemTex
-000134e0: 7428 312c 205f 7472 616e 736c 6174 6528  t(1, _translate(
-000134f0: 224d 6169 6e57 696e 646f 7722 2c20 2244  "MainWindow", "D
-00013500: 6574 6169 6c22 2929 0a20 2020 2020 2020  etail")).       
-00013510: 2073 656c 662e 6275 7474 6f6e 5f73 6176   self.button_sav
-00013520: 6552 6563 6f6e 7374 2e73 6574 5465 7874  eReconst.setText
-00013530: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-00013540: 6e57 696e 646f 7722 2c20 2253 6176 6520  nWindow", "Save 
-00013550: 4669 6722 2929 0a20 2020 2020 2020 2073  Fig")).        s
-00013560: 656c 662e 636d 625f 7375 6d44 6576 2e73  elf.cmb_sumDev.s
-00013570: 6574 4974 656d 5465 7874 2830 2c20 5f74  etItemText(0, _t
-00013580: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-00013590: 6e64 6f77 222c 2022 c2b1 302e 3520 cf83  ndow", "..0.5 ..
-000135a0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-000135b0: 2e63 6d62 5f73 756d 4465 762e 7365 7449  .cmb_sumDev.setI
-000135c0: 7465 6d54 6578 7428 312c 205f 7472 616e  temText(1, _tran
-000135d0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-000135e0: 7722 2c20 22c2 b131 2e30 20cf 8322 2929  w", "..1.0 .."))
-000135f0: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
-00013600: 625f 7375 6d44 6576 2e73 6574 4974 656d  b_sumDev.setItem
-00013610: 5465 7874 2832 2c20 5f74 7261 6e73 6c61  Text(2, _transla
-00013620: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-00013630: 2022 c2b1 312e 3520 cf83 2229 290a 2020   "..1.5 ..")).  
-00013640: 2020 2020 2020 7365 6c66 2e63 6d62 5f73        self.cmb_s
-00013650: 756d 4465 762e 7365 7449 7465 6d54 6578  umDev.setItemTex
-00013660: 7428 332c 205f 7472 616e 736c 6174 6528  t(3, _translate(
-00013670: 224d 6169 6e57 696e 646f 7722 2c20 22c2  "MainWindow", ".
-00013680: b132 2e30 20cf 8322 2929 0a20 2020 2020  .2.0 ..")).     
-00013690: 2020 2073 656c 662e 636d 625f 7375 6d44     self.cmb_sumD
-000136a0: 6576 2e73 6574 4974 656d 5465 7874 2834  ev.setItemText(4
-000136b0: 2c20 5f74 7261 6e73 6c61 7465 2822 4d61  , _translate("Ma
-000136c0: 696e 5769 6e64 6f77 222c 2022 c2b1 322e  inWindow", "..2.
-000136d0: 3520 cf83 2229 290a 2020 2020 2020 2020  5 ..")).        
-000136e0: 7365 6c66 2e63 6d62 5f73 756d 4465 762e  self.cmb_sumDev.
-000136f0: 7365 7449 7465 6d54 6578 7428 352c 205f  setItemText(5, _
-00013700: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00013710: 696e 646f 7722 2c20 22c2 b133 2e30 20cf  indow", "..3.0 .
-00013720: 8322 2929 0a20 2020 2020 2020 2073 656c  .")).        sel
-00013730: 662e 6275 7474 6f6e 5f67 656e 6572 6174  f.button_generat
-00013740: 652e 7365 7454 6578 7428 5f74 7261 6e73  e.setText(_trans
-00013750: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00013760: 222c 2022 4765 6e65 7261 7465 2229 290a  ", "Generate")).
-00013770: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00013780: 656c 5f32 362e 7365 7454 6578 7428 5f74  el_26.setText(_t
-00013790: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-000137a0: 6e64 6f77 222c 2022 2064 6576 2e28 cf83  ndow", " dev.(..
-000137b0: 2922 2929 0a20 2020 2020 2020 2073 656c  )")).        sel
-000137c0: 662e 6c61 6265 6c5f 3237 2e73 6574 5465  f.label_27.setTe
-000137d0: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-000137e0: 6169 6e57 696e 646f 7722 2c20 2244 6574  ainWindow", "Det
-000137f0: 6169 6c20 4d6f 6465 2229 290a 2020 2020  ail Mode")).    
-00013800: 2020 2020 7365 6c66 2e6c 6162 656c 5f32      self.label_2
-00013810: 352e 7365 7454 6578 7428 5f74 7261 6e73  5.setText(_trans
-00013820: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00013830: 222c 2022 5043 2229 290a 2020 2020 2020  ", "PC")).      
-00013840: 2020 7365 6c66 2e6c 6162 656c 5f32 332e    self.label_23.
-00013850: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-00013860: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-00013870: 2022 5375 6d6d 6172 7920 4d4f 4445 2229   "Summary MODE")
-00013880: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-00013890: 6162 5769 6467 6574 2e73 6574 5461 6254  abWidget.setTabT
-000138a0: 6578 7428 7365 6c66 2e74 6162 5769 6467  ext(self.tabWidg
-000138b0: 6574 2e69 6e64 6578 4f66 2873 656c 662e  et.indexOf(self.
-000138c0: 7461 625f 3329 2c20 5f74 7261 6e73 6c61  tab_3), _transla
-000138d0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-000138e0: 2022 5368 6170 6522 2929 0a20 2020 2020   "Shape")).     
-000138f0: 2020 2073 656c 662e 6d65 6e75 7465 7374     self.menutest
-00013900: 2e73 6574 5469 746c 6528 5f74 7261 6e73  .setTitle(_trans
-00013910: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00013920: 222c 2022 4669 6c65 2229 290a 2020 2020  ", "File")).    
-00013930: 2020 2020 7365 6c66 2e61 6374 696f 6e41      self.actionA
-00013940: 626f 7574 2e73 6574 5465 7874 285f 7472  bout.setText(_tr
-00013950: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-00013960: 646f 7722 2c20 2241 626f 7574 2229 290a  dow", "About")).
+000034d0: 7428 7365 6c66 2e6c 6162 656c 5f33 342c  t(self.label_34,
+000034e0: 2032 2c20 302c 2031 2c20 3129 0a20 2020   2, 0, 1, 1).   
+000034f0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00003500: 3333 203d 2051 7457 6964 6765 7473 2e51  33 = QtWidgets.Q
+00003510: 4c61 6265 6c28 7061 7265 6e74 3d73 656c  Label(parent=sel
+00003520: 662e 6672 616d 655f 3329 0a20 2020 2020  f.frame_3).     
+00003530: 2020 2073 697a 6550 6f6c 6963 7920 3d20     sizePolicy = 
+00003540: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
+00003550: 6f6c 6963 7928 5174 5769 6467 6574 732e  olicy(QtWidgets.
+00003560: 5153 697a 6550 6f6c 6963 792e 506f 6c69  QSizePolicy.Poli
+00003570: 6379 2e50 7265 6665 7272 6564 2c20 5174  cy.Preferred, Qt
+00003580: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
+00003590: 6963 792e 506f 6c69 6379 2e4d 696e 696d  icy.Policy.Minim
+000035a0: 756d 290a 2020 2020 2020 2020 7369 7a65  um).        size
+000035b0: 506f 6c69 6379 2e73 6574 486f 7269 7a6f  Policy.setHorizo
+000035c0: 6e74 616c 5374 7265 7463 6828 3029 0a20  ntalStretch(0). 
+000035d0: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
+000035e0: 792e 7365 7456 6572 7469 6361 6c53 7472  y.setVerticalStr
+000035f0: 6574 6368 2830 290a 2020 2020 2020 2020  etch(0).        
+00003600: 7369 7a65 506f 6c69 6379 2e73 6574 4865  sizePolicy.setHe
+00003610: 6967 6874 466f 7257 6964 7468 2873 656c  ightForWidth(sel
+00003620: 662e 6c61 6265 6c5f 3333 2e73 697a 6550  f.label_33.sizeP
+00003630: 6f6c 6963 7928 292e 6861 7348 6569 6768  olicy().hasHeigh
+00003640: 7446 6f72 5769 6474 6828 2929 0a20 2020  tForWidth()).   
+00003650: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00003660: 3333 2e73 6574 5369 7a65 506f 6c69 6379  33.setSizePolicy
+00003670: 2873 697a 6550 6f6c 6963 7929 0a20 2020  (sizePolicy).   
+00003680: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00003690: 3333 2e73 6574 4f62 6a65 6374 4e61 6d65  33.setObjectName
+000036a0: 2822 6c61 6265 6c5f 3333 2229 0a20 2020  ("label_33").   
+000036b0: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
+000036c0: 796f 7574 5f31 342e 6164 6457 6964 6765  yout_14.addWidge
+000036d0: 7428 7365 6c66 2e6c 6162 656c 5f33 332c  t(self.label_33,
+000036e0: 2030 2c20 302c 2031 2c20 3129 0a20 2020   0, 0, 1, 1).   
+000036f0: 2020 2020 2073 656c 662e 6275 7474 6f6e       self.button
+00003700: 5f73 616d 706c 6520 3d20 5174 5769 6467  _sample = QtWidg
+00003710: 6574 732e 5150 7573 6842 7574 746f 6e28  ets.QPushButton(
+00003720: 7061 7265 6e74 3d73 656c 662e 6672 616d  parent=self.fram
+00003730: 655f 3329 0a20 2020 2020 2020 2073 656c  e_3).        sel
+00003740: 662e 6275 7474 6f6e 5f73 616d 706c 652e  f.button_sample.
+00003750: 7365 744f 626a 6563 744e 616d 6528 2262  setObjectName("b
+00003760: 7574 746f 6e5f 7361 6d70 6c65 2229 0a20  utton_sample"). 
+00003770: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
+00003780: 4c61 796f 7574 5f31 342e 6164 6457 6964  Layout_14.addWid
+00003790: 6765 7428 7365 6c66 2e62 7574 746f 6e5f  get(self.button_
+000037a0: 7361 6d70 6c65 2c20 312c 2030 2c20 312c  sample, 1, 0, 1,
+000037b0: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+000037c0: 2e73 625f 6d68 5f73 616d 706c 6520 3d20  .sb_mh_sample = 
+000037d0: 5174 5769 6467 6574 732e 5153 7069 6e42  QtWidgets.QSpinB
+000037e0: 6f78 2870 6172 656e 743d 7365 6c66 2e66  ox(parent=self.f
+000037f0: 7261 6d65 5f33 290a 2020 2020 2020 2020  rame_3).        
+00003800: 7365 6c66 2e73 625f 6d68 5f73 616d 706c  self.sb_mh_sampl
+00003810: 652e 7365 744d 696e 696d 756d 2831 290a  e.setMinimum(1).
+00003820: 2020 2020 2020 2020 7365 6c66 2e73 625f          self.sb_
+00003830: 6d68 5f73 616d 706c 652e 7365 744d 6178  mh_sample.setMax
+00003840: 696d 756d 2833 3030 290a 2020 2020 2020  imum(300).      
+00003850: 2020 7365 6c66 2e73 625f 6d68 5f73 616d    self.sb_mh_sam
+00003860: 706c 652e 7365 7450 726f 7065 7274 7928  ple.setProperty(
+00003870: 2276 616c 7565 222c 2033 3029 0a20 2020  "value", 30).   
+00003880: 2020 2020 2073 656c 662e 7362 5f6d 685f       self.sb_mh_
+00003890: 7361 6d70 6c65 2e73 6574 4f62 6a65 6374  sample.setObject
+000038a0: 4e61 6d65 2822 7362 5f6d 685f 7361 6d70  Name("sb_mh_samp
+000038b0: 6c65 2229 0a20 2020 2020 2020 2073 656c  le").        sel
+000038c0: 662e 6772 6964 4c61 796f 7574 5f31 342e  f.gridLayout_14.
+000038d0: 6164 6457 6964 6765 7428 7365 6c66 2e73  addWidget(self.s
+000038e0: 625f 6d68 5f73 616d 706c 652c 2031 2c20  b_mh_sample, 1, 
+000038f0: 312c 2031 2c20 3129 0a20 2020 2020 2020  1, 1, 1).       
+00003900: 2073 656c 662e 6c61 6265 6c5f 3338 203d   self.label_38 =
+00003910: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
+00003920: 6c28 7061 7265 6e74 3d73 656c 662e 6672  l(parent=self.fr
+00003930: 616d 655f 3329 0a20 2020 2020 2020 2073  ame_3).        s
+00003940: 656c 662e 6c61 6265 6c5f 3338 2e73 6574  elf.label_38.set
+00003950: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
+00003960: 6c5f 3338 2229 0a20 2020 2020 2020 2073  l_38").        s
+00003970: 656c 662e 6772 6964 4c61 796f 7574 5f31  elf.gridLayout_1
+00003980: 342e 6164 6457 6964 6765 7428 7365 6c66  4.addWidget(self
+00003990: 2e6c 6162 656c 5f33 382c 2030 2c20 312c  .label_38, 0, 1,
+000039a0: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
+000039b0: 656c 662e 6275 7474 6f6e 5f73 7461 7274  elf.button_start
+000039c0: 7361 6d70 6c65 203d 2051 7457 6964 6765  sample = QtWidge
+000039d0: 7473 2e51 5075 7368 4275 7474 6f6e 2870  ts.QPushButton(p
+000039e0: 6172 656e 743d 7365 6c66 2e66 7261 6d65  arent=self.frame
+000039f0: 5f33 290a 2020 2020 2020 2020 7369 7a65  _3).        size
+00003a00: 506f 6c69 6379 203d 2051 7457 6964 6765  Policy = QtWidge
+00003a10: 7473 2e51 5369 7a65 506f 6c69 6379 2851  ts.QSizePolicy(Q
+00003a20: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
+00003a30: 6c69 6379 2e50 6f6c 6963 792e 4d69 6e69  licy.Policy.Mini
+00003a40: 6d75 6d2c 2051 7457 6964 6765 7473 2e51  mum, QtWidgets.Q
+00003a50: 5369 7a65 506f 6c69 6379 2e50 6f6c 6963  SizePolicy.Polic
+00003a60: 792e 4578 7061 6e64 696e 6729 0a20 2020  y.Expanding).   
+00003a70: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
+00003a80: 7365 7448 6f72 697a 6f6e 7461 6c53 7472  setHorizontalStr
+00003a90: 6574 6368 2830 290a 2020 2020 2020 2020  etch(0).        
+00003aa0: 7369 7a65 506f 6c69 6379 2e73 6574 5665  sizePolicy.setVe
+00003ab0: 7274 6963 616c 5374 7265 7463 6828 3029  rticalStretch(0)
+00003ac0: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+00003ad0: 6963 792e 7365 7448 6569 6768 7446 6f72  icy.setHeightFor
+00003ae0: 5769 6474 6828 7365 6c66 2e62 7574 746f  Width(self.butto
+00003af0: 6e5f 7374 6172 7473 616d 706c 652e 7369  n_startsample.si
+00003b00: 7a65 506f 6c69 6379 2829 2e68 6173 4865  zePolicy().hasHe
+00003b10: 6967 6874 466f 7257 6964 7468 2829 290a  ightForWidth()).
+00003b20: 2020 2020 2020 2020 7365 6c66 2e62 7574          self.but
+00003b30: 746f 6e5f 7374 6172 7473 616d 706c 652e  ton_startsample.
+00003b40: 7365 7453 697a 6550 6f6c 6963 7928 7369  setSizePolicy(si
+00003b50: 7a65 506f 6c69 6379 290a 2020 2020 2020  zePolicy).      
+00003b60: 2020 7365 6c66 2e62 7574 746f 6e5f 7374    self.button_st
+00003b70: 6172 7473 616d 706c 652e 7365 7449 636f  artsample.setIco
+00003b80: 6e53 697a 6528 5174 436f 7265 2e51 5369  nSize(QtCore.QSi
+00003b90: 7a65 2831 392c 2031 3929 290a 2020 2020  ze(19, 19)).    
+00003ba0: 2020 2020 7365 6c66 2e62 7574 746f 6e5f      self.button_
+00003bb0: 7374 6172 7473 616d 706c 652e 7365 744f  startsample.setO
+00003bc0: 626a 6563 744e 616d 6528 2262 7574 746f  bjectName("butto
+00003bd0: 6e5f 7374 6172 7473 616d 706c 6522 290a  n_startsample").
+00003be0: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
+00003bf0: 644c 6179 6f75 745f 3134 2e61 6464 5769  dLayout_14.addWi
+00003c00: 6467 6574 2873 656c 662e 6275 7474 6f6e  dget(self.button
+00003c10: 5f73 7461 7274 7361 6d70 6c65 2c20 302c  _startsample, 0,
+00003c20: 2032 2c20 332c 2031 290a 2020 2020 2020   2, 3, 1).      
+00003c30: 2020 7365 6c66 2e62 7574 746f 6e5f 7361    self.button_sa
+00003c40: 7665 5f73 616d 706c 6520 3d20 5174 5769  ve_sample = QtWi
+00003c50: 6467 6574 732e 5150 7573 6842 7574 746f  dgets.QPushButto
+00003c60: 6e28 7061 7265 6e74 3d73 656c 662e 6672  n(parent=self.fr
+00003c70: 616d 655f 3329 0a20 2020 2020 2020 2073  ame_3).        s
+00003c80: 656c 662e 6275 7474 6f6e 5f73 6176 655f  elf.button_save_
+00003c90: 7361 6d70 6c65 2e73 6574 4f62 6a65 6374  sample.setObject
+00003ca0: 4e61 6d65 2822 6275 7474 6f6e 5f73 6176  Name("button_sav
+00003cb0: 655f 7361 6d70 6c65 2229 0a20 2020 2020  e_sample").     
+00003cc0: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
+00003cd0: 7574 5f31 342e 6164 6457 6964 6765 7428  ut_14.addWidget(
+00003ce0: 7365 6c66 2e62 7574 746f 6e5f 7361 7665  self.button_save
+00003cf0: 5f73 616d 706c 652c 2033 2c20 322c 2031  _sample, 3, 2, 1
+00003d00: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
+00003d10: 662e 6772 6964 4c61 796f 7574 5f31 332e  f.gridLayout_13.
+00003d20: 6164 6457 6964 6765 7428 7365 6c66 2e66  addWidget(self.f
+00003d30: 7261 6d65 5f33 2c20 302c 2031 2c20 312c  rame_3, 0, 1, 1,
+00003d40: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+00003d50: 2e74 6162 5769 6467 6574 2e61 6464 5461  .tabWidget.addTa
+00003d60: 6228 7365 6c66 2e74 6162 5f35 2c20 2222  b(self.tab_5, ""
+00003d70: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+00003d80: 6162 203d 2051 7457 6964 6765 7473 2e51  ab = QtWidgets.Q
+00003d90: 5769 6467 6574 2829 0a20 2020 2020 2020  Widget().       
+00003da0: 2073 656c 662e 7461 622e 7365 744f 626a   self.tab.setObj
+00003db0: 6563 744e 616d 6528 2274 6162 2229 0a20  ectName("tab"). 
+00003dc0: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
+00003dd0: 4c61 796f 7574 5f39 203d 2051 7457 6964  Layout_9 = QtWid
+00003de0: 6765 7473 2e51 4772 6964 4c61 796f 7574  gets.QGridLayout
+00003df0: 2873 656c 662e 7461 6229 0a20 2020 2020  (self.tab).     
+00003e00: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
+00003e10: 7574 5f39 2e73 6574 4f62 6a65 6374 4e61  ut_9.setObjectNa
+00003e20: 6d65 2822 6772 6964 4c61 796f 7574 5f39  me("gridLayout_9
+00003e30: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00003e40: 7363 726f 6c6c 4172 6561 5f32 203d 2051  scrollArea_2 = Q
+00003e50: 7457 6964 6765 7473 2e51 5363 726f 6c6c  tWidgets.QScroll
+00003e60: 4172 6561 2870 6172 656e 743d 7365 6c66  Area(parent=self
+00003e70: 2e74 6162 290a 2020 2020 2020 2020 7369  .tab).        si
+00003e80: 7a65 506f 6c69 6379 203d 2051 7457 6964  zePolicy = QtWid
+00003e90: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
+00003ea0: 2851 7457 6964 6765 7473 2e51 5369 7a65  (QtWidgets.QSize
+00003eb0: 506f 6c69 6379 2e50 6f6c 6963 792e 4578  Policy.Policy.Ex
+00003ec0: 7061 6e64 696e 672c 2051 7457 6964 6765  panding, QtWidge
+00003ed0: 7473 2e51 5369 7a65 506f 6c69 6379 2e50  ts.QSizePolicy.P
+00003ee0: 6f6c 6963 792e 4578 7061 6e64 696e 6729  olicy.Expanding)
+00003ef0: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+00003f00: 6963 792e 7365 7448 6f72 697a 6f6e 7461  icy.setHorizonta
+00003f10: 6c53 7472 6574 6368 2830 290a 2020 2020  lStretch(0).    
+00003f20: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
+00003f30: 6574 5665 7274 6963 616c 5374 7265 7463  etVerticalStretc
+00003f40: 6828 3029 0a20 2020 2020 2020 2073 697a  h(0).        siz
+00003f50: 6550 6f6c 6963 792e 7365 7448 6569 6768  ePolicy.setHeigh
+00003f60: 7446 6f72 5769 6474 6828 7365 6c66 2e73  tForWidth(self.s
+00003f70: 6372 6f6c 6c41 7265 615f 322e 7369 7a65  crollArea_2.size
+00003f80: 506f 6c69 6379 2829 2e68 6173 4865 6967  Policy().hasHeig
+00003f90: 6874 466f 7257 6964 7468 2829 290a 2020  htForWidth()).  
+00003fa0: 2020 2020 2020 7365 6c66 2e73 6372 6f6c        self.scrol
+00003fb0: 6c41 7265 615f 322e 7365 7453 697a 6550  lArea_2.setSizeP
+00003fc0: 6f6c 6963 7928 7369 7a65 506f 6c69 6379  olicy(sizePolicy
+00003fd0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00003fe0: 6372 6f6c 6c41 7265 615f 322e 7365 744d  crollArea_2.setM
+00003ff0: 696e 696d 756d 5369 7a65 2851 7443 6f72  inimumSize(QtCor
+00004000: 652e 5153 697a 6528 3230 302c 2033 3731  e.QSize(200, 371
+00004010: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00004020: 7363 726f 6c6c 4172 6561 5f32 2e73 6574  scrollArea_2.set
+00004030: 4d61 7869 6d75 6d53 697a 6528 5174 436f  MaximumSize(QtCo
+00004040: 7265 2e51 5369 7a65 2839 3030 2c20 3136  re.QSize(900, 16
+00004050: 3737 3732 3135 2929 0a20 2020 2020 2020  777215)).       
+00004060: 2073 656c 662e 7363 726f 6c6c 4172 6561   self.scrollArea
+00004070: 5f32 2e73 6574 4c69 6e65 5769 6474 6828  _2.setLineWidth(
+00004080: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+00004090: 7363 726f 6c6c 4172 6561 5f32 2e73 6574  scrollArea_2.set
+000040a0: 5665 7274 6963 616c 5363 726f 6c6c 4261  VerticalScrollBa
+000040b0: 7250 6f6c 6963 7928 5174 436f 7265 2e51  rPolicy(QtCore.Q
+000040c0: 742e 5363 726f 6c6c 4261 7250 6f6c 6963  t.ScrollBarPolic
+000040d0: 792e 5363 726f 6c6c 4261 7241 6c77 6179  y.ScrollBarAlway
+000040e0: 734f 6e29 0a20 2020 2020 2020 2073 656c  sOn).        sel
+000040f0: 662e 7363 726f 6c6c 4172 6561 5f32 2e73  f.scrollArea_2.s
+00004100: 6574 5769 6467 6574 5265 7369 7a61 626c  etWidgetResizabl
+00004110: 6528 5472 7565 290a 2020 2020 2020 2020  e(True).        
+00004120: 7365 6c66 2e73 6372 6f6c 6c41 7265 615f  self.scrollArea_
+00004130: 322e 7365 744f 626a 6563 744e 616d 6528  2.setObjectName(
+00004140: 2273 6372 6f6c 6c41 7265 615f 3222 290a  "scrollArea_2").
+00004150: 2020 2020 2020 2020 7365 6c66 2e73 6372          self.scr
+00004160: 6f6c 6c41 7265 6157 6964 6765 7443 6f6e  ollAreaWidgetCon
+00004170: 7465 6e74 735f 3220 3d20 5174 5769 6467  tents_2 = QtWidg
+00004180: 6574 732e 5157 6964 6765 7428 290a 2020  ets.QWidget().  
+00004190: 2020 2020 2020 7365 6c66 2e73 6372 6f6c        self.scrol
+000041a0: 6c41 7265 6157 6964 6765 7443 6f6e 7465  lAreaWidgetConte
+000041b0: 6e74 735f 322e 7365 7447 656f 6d65 7472  nts_2.setGeometr
+000041c0: 7928 5174 436f 7265 2e51 5265 6374 2830  y(QtCore.QRect(0
+000041d0: 2c20 2d35 352c 2035 3230 2c20 3739 3629  , -55, 520, 796)
+000041e0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+000041f0: 6372 6f6c 6c41 7265 6157 6964 6765 7443  crollAreaWidgetC
+00004200: 6f6e 7465 6e74 735f 322e 7365 744f 626a  ontents_2.setObj
+00004210: 6563 744e 616d 6528 2273 6372 6f6c 6c41  ectName("scrollA
+00004220: 7265 6157 6964 6765 7443 6f6e 7465 6e74  reaWidgetContent
+00004230: 735f 3222 290a 2020 2020 2020 2020 7365  s_2").        se
+00004240: 6c66 2e67 7269 644c 6179 6f75 745f 3220  lf.gridLayout_2 
+00004250: 3d20 5174 5769 6467 6574 732e 5147 7269  = QtWidgets.QGri
+00004260: 644c 6179 6f75 7428 7365 6c66 2e73 6372  dLayout(self.scr
+00004270: 6f6c 6c41 7265 6157 6964 6765 7443 6f6e  ollAreaWidgetCon
+00004280: 7465 6e74 735f 3229 0a20 2020 2020 2020  tents_2).       
+00004290: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
+000042a0: 5f32 2e73 6574 4f62 6a65 6374 4e61 6d65  _2.setObjectName
+000042b0: 2822 6772 6964 4c61 796f 7574 5f32 2229  ("gridLayout_2")
+000042c0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+000042d0: 6265 6c5f 3331 203d 2051 7457 6964 6765  bel_31 = QtWidge
+000042e0: 7473 2e51 4c61 6265 6c28 7061 7265 6e74  ts.QLabel(parent
+000042f0: 3d73 656c 662e 7363 726f 6c6c 4172 6561  =self.scrollArea
+00004300: 5769 6467 6574 436f 6e74 656e 7473 5f32  WidgetContents_2
+00004310: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
+00004320: 6c69 6379 203d 2051 7457 6964 6765 7473  licy = QtWidgets
+00004330: 2e51 5369 7a65 506f 6c69 6379 2851 7457  .QSizePolicy(QtW
+00004340: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
+00004350: 6379 2e50 6f6c 6963 792e 5072 6566 6572  cy.Policy.Prefer
+00004360: 7265 642c 2051 7457 6964 6765 7473 2e51  red, QtWidgets.Q
+00004370: 5369 7a65 506f 6c69 6379 2e50 6f6c 6963  SizePolicy.Polic
+00004380: 792e 4669 7865 6429 0a20 2020 2020 2020  y.Fixed).       
+00004390: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
+000043a0: 6f72 697a 6f6e 7461 6c53 7472 6574 6368  orizontalStretch
+000043b0: 2830 290a 2020 2020 2020 2020 7369 7a65  (0).        size
+000043c0: 506f 6c69 6379 2e73 6574 5665 7274 6963  Policy.setVertic
+000043d0: 616c 5374 7265 7463 6828 3029 0a20 2020  alStretch(0).   
+000043e0: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
+000043f0: 7365 7448 6569 6768 7446 6f72 5769 6474  setHeightForWidt
+00004400: 6828 7365 6c66 2e6c 6162 656c 5f33 312e  h(self.label_31.
+00004410: 7369 7a65 506f 6c69 6379 2829 2e68 6173  sizePolicy().has
+00004420: 4865 6967 6874 466f 7257 6964 7468 2829  HeightForWidth()
+00004430: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00004440: 6162 656c 5f33 312e 7365 7453 697a 6550  abel_31.setSizeP
+00004450: 6f6c 6963 7928 7369 7a65 506f 6c69 6379  olicy(sizePolicy
+00004460: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00004470: 6162 656c 5f33 312e 7365 744f 626a 6563  abel_31.setObjec
+00004480: 744e 616d 6528 226c 6162 656c 5f33 3122  tName("label_31"
+00004490: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+000044a0: 7269 644c 6179 6f75 745f 322e 6164 6457  ridLayout_2.addW
+000044b0: 6964 6765 7428 7365 6c66 2e6c 6162 656c  idget(self.label
+000044c0: 5f33 312c 2032 362c 2030 2c20 312c 2033  _31, 26, 0, 1, 3
+000044d0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+000044e0: 696e 655f 666f 6c64 6120 3d20 5174 5769  ine_folda = QtWi
+000044f0: 6467 6574 732e 514c 696e 6545 6469 7428  dgets.QLineEdit(
+00004500: 7061 7265 6e74 3d73 656c 662e 7363 726f  parent=self.scro
+00004510: 6c6c 4172 6561 5769 6467 6574 436f 6e74  llAreaWidgetCont
+00004520: 656e 7473 5f32 290a 2020 2020 2020 2020  ents_2).        
+00004530: 7365 6c66 2e6c 696e 655f 666f 6c64 612e  self.line_folda.
+00004540: 7365 7452 6561 644f 6e6c 7928 4661 6c73  setReadOnly(Fals
+00004550: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+00004560: 6c69 6e65 5f66 6f6c 6461 2e73 6574 4f62  line_folda.setOb
+00004570: 6a65 6374 4e61 6d65 2822 6c69 6e65 5f66  jectName("line_f
+00004580: 6f6c 6461 2229 0a20 2020 2020 2020 2073  olda").        s
+00004590: 656c 662e 6772 6964 4c61 796f 7574 5f32  elf.gridLayout_2
+000045a0: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+000045b0: 6c69 6e65 5f66 6f6c 6461 2c20 322c 2030  line_folda, 2, 0
+000045c0: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
+000045d0: 7365 6c66 2e63 6d62 5f66 6f72 6d61 7420  self.cmb_format 
+000045e0: 3d20 5174 5769 6467 6574 732e 5143 6f6d  = QtWidgets.QCom
+000045f0: 626f 426f 7828 7061 7265 6e74 3d73 656c  boBox(parent=sel
+00004600: 662e 7363 726f 6c6c 4172 6561 5769 6467  f.scrollAreaWidg
+00004610: 6574 436f 6e74 656e 7473 5f32 290a 2020  etContents_2).  
+00004620: 2020 2020 2020 7365 6c66 2e63 6d62 5f66        self.cmb_f
+00004630: 6f72 6d61 742e 7365 744f 626a 6563 744e  ormat.setObjectN
+00004640: 616d 6528 2263 6d62 5f66 6f72 6d61 7422  ame("cmb_format"
+00004650: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00004660: 6d62 5f66 6f72 6d61 742e 6164 6449 7465  mb_format.addIte
+00004670: 6d28 2222 290a 2020 2020 2020 2020 7365  m("").        se
+00004680: 6c66 2e63 6d62 5f66 6f72 6d61 742e 6164  lf.cmb_format.ad
+00004690: 6449 7465 6d28 2222 290a 2020 2020 2020  dItem("").      
+000046a0: 2020 7365 6c66 2e63 6d62 5f66 6f72 6d61    self.cmb_forma
+000046b0: 742e 6164 6449 7465 6d28 2222 290a 2020  t.addItem("").  
+000046c0: 2020 2020 2020 7365 6c66 2e63 6d62 5f66        self.cmb_f
+000046d0: 6f72 6d61 742e 6164 6449 7465 6d28 2222  ormat.addItem(""
+000046e0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+000046f0: 7269 644c 6179 6f75 745f 322e 6164 6457  ridLayout_2.addW
+00004700: 6964 6765 7428 7365 6c66 2e63 6d62 5f66  idget(self.cmb_f
+00004710: 6f72 6d61 742c 2036 2c20 312c 2031 2c20  ormat, 6, 1, 1, 
+00004720: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+00004730: 636d 625f 7363 616c 6554 7970 6520 3d20  cmb_scaleType = 
+00004740: 5174 5769 6467 6574 732e 5143 6f6d 626f  QtWidgets.QCombo
+00004750: 426f 7828 7061 7265 6e74 3d73 656c 662e  Box(parent=self.
+00004760: 7363 726f 6c6c 4172 6561 5769 6467 6574  scrollAreaWidget
+00004770: 436f 6e74 656e 7473 5f32 290a 2020 2020  Contents_2).    
+00004780: 2020 2020 7365 6c66 2e63 6d62 5f73 6361      self.cmb_sca
+00004790: 6c65 5479 7065 2e73 6574 4f62 6a65 6374  leType.setObject
+000047a0: 4e61 6d65 2822 636d 625f 7363 616c 6554  Name("cmb_scaleT
+000047b0: 7970 6522 290a 2020 2020 2020 2020 7365  ype").        se
+000047c0: 6c66 2e63 6d62 5f73 6361 6c65 5479 7065  lf.cmb_scaleType
+000047d0: 2e61 6464 4974 656d 2822 2229 0a20 2020  .addItem("").   
+000047e0: 2020 2020 2073 656c 662e 636d 625f 7363       self.cmb_sc
+000047f0: 616c 6554 7970 652e 6164 6449 7465 6d28  aleType.addItem(
+00004800: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
+00004810: 2e63 6d62 5f73 6361 6c65 5479 7065 2e61  .cmb_scaleType.a
+00004820: 6464 4974 656d 2822 2229 0a20 2020 2020  ddItem("").     
+00004830: 2020 2073 656c 662e 636d 625f 7363 616c     self.cmb_scal
+00004840: 6554 7970 652e 6164 6449 7465 6d28 2222  eType.addItem(""
+00004850: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00004860: 7269 644c 6179 6f75 745f 322e 6164 6457  ridLayout_2.addW
+00004870: 6964 6765 7428 7365 6c66 2e63 6d62 5f73  idget(self.cmb_s
+00004880: 6361 6c65 5479 7065 2c20 3333 2c20 312c  caleType, 33, 1,
+00004890: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
+000048a0: 656c 662e 6c61 6265 6c20 3d20 5174 5769  elf.label = QtWi
+000048b0: 6467 6574 732e 514c 6162 656c 2870 6172  dgets.QLabel(par
+000048c0: 656e 743d 7365 6c66 2e73 6372 6f6c 6c41  ent=self.scrollA
+000048d0: 7265 6157 6964 6765 7443 6f6e 7465 6e74  reaWidgetContent
+000048e0: 735f 3229 0a20 2020 2020 2020 2073 656c  s_2).        sel
+000048f0: 662e 6c61 6265 6c2e 7365 744f 626a 6563  f.label.setObjec
+00004900: 744e 616d 6528 226c 6162 656c 2229 0a20  tName("label"). 
+00004910: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
+00004920: 4c61 796f 7574 5f32 2e61 6464 5769 6467  Layout_2.addWidg
+00004930: 6574 2873 656c 662e 6c61 6265 6c2c 2036  et(self.label, 6
+00004940: 2c20 302c 2031 2c20 3129 0a20 2020 2020  , 0, 1, 1).     
+00004950: 2020 2073 656c 662e 6275 7474 6f6e 5f66     self.button_f
+00004960: 6f6c 6461 203d 2051 7457 6964 6765 7473  olda = QtWidgets
+00004970: 2e51 5075 7368 4275 7474 6f6e 2870 6172  .QPushButton(par
+00004980: 656e 743d 7365 6c66 2e73 6372 6f6c 6c41  ent=self.scrollA
+00004990: 7265 6157 6964 6765 7443 6f6e 7465 6e74  reaWidgetContent
+000049a0: 735f 3229 0a20 2020 2020 2020 2073 656c  s_2).        sel
+000049b0: 662e 6275 7474 6f6e 5f66 6f6c 6461 2e73  f.button_folda.s
+000049c0: 6574 4f62 6a65 6374 4e61 6d65 2822 6275  etObjectName("bu
+000049d0: 7474 6f6e 5f66 6f6c 6461 2229 0a20 2020  tton_folda").   
+000049e0: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
+000049f0: 796f 7574 5f32 2e61 6464 5769 6467 6574  yout_2.addWidget
+00004a00: 2873 656c 662e 6275 7474 6f6e 5f66 6f6c  (self.button_fol
+00004a10: 6461 2c20 322c 2031 2c20 312c 2031 290a  da, 2, 1, 1, 1).
+00004a20: 2020 2020 2020 2020 7365 6c66 2e73 7062          self.spb
+00004a30: 5f6d 7078 6120 3d20 5174 5769 6467 6574  _mpxa = QtWidget
+00004a40: 732e 5153 7069 6e42 6f78 2870 6172 656e  s.QSpinBox(paren
+00004a50: 743d 7365 6c66 2e73 6372 6f6c 6c41 7265  t=self.scrollAre
+00004a60: 6157 6964 6765 7443 6f6e 7465 6e74 735f  aWidgetContents_
+00004a70: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
+00004a80: 7370 625f 6d70 7861 2e73 6574 4d69 6e69  spb_mpxa.setMini
+00004a90: 6d75 6d28 3130 3029 0a20 2020 2020 2020  mum(100).       
+00004aa0: 2073 656c 662e 7370 625f 6d70 7861 2e73   self.spb_mpxa.s
+00004ab0: 6574 4d61 7869 6d75 6d28 3439 3939 3939  etMaximum(499999
+00004ac0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00004ad0: 7062 5f6d 7078 612e 7365 7450 726f 7065  pb_mpxa.setPrope
+00004ae0: 7274 7928 2276 616c 7565 222c 2032 3030  rty("value", 200
+00004af0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00004b00: 7062 5f6d 7078 612e 7365 744f 626a 6563  pb_mpxa.setObjec
+00004b10: 744e 616d 6528 2273 7062 5f6d 7078 6122  tName("spb_mpxa"
+00004b20: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00004b30: 7269 644c 6179 6f75 745f 322e 6164 6457  ridLayout_2.addW
+00004b40: 6964 6765 7428 7365 6c66 2e73 7062 5f6d  idget(self.spb_m
+00004b50: 7078 612c 2033 312c 2031 2c20 312c 2031  pxa, 31, 1, 1, 1
+00004b60: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00004b70: 696e 655f 3220 3d20 5174 5769 6467 6574  ine_2 = QtWidget
+00004b80: 732e 5146 7261 6d65 2870 6172 656e 743d  s.QFrame(parent=
+00004b90: 7365 6c66 2e73 6372 6f6c 6c41 7265 6157  self.scrollAreaW
+00004ba0: 6964 6765 7443 6f6e 7465 6e74 735f 3229  idgetContents_2)
+00004bb0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004bc0: 6e65 5f32 2e73 6574 4672 616d 6553 6861  ne_2.setFrameSha
+00004bd0: 7065 2851 7457 6964 6765 7473 2e51 4672  pe(QtWidgets.QFr
+00004be0: 616d 652e 5368 6170 652e 484c 696e 6529  ame.Shape.HLine)
+00004bf0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004c00: 6e65 5f32 2e73 6574 4672 616d 6553 6861  ne_2.setFrameSha
+00004c10: 646f 7728 5174 5769 6467 6574 732e 5146  dow(QtWidgets.QF
+00004c20: 7261 6d65 2e53 6861 646f 772e 5375 6e6b  rame.Shadow.Sunk
+00004c30: 656e 290a 2020 2020 2020 2020 7365 6c66  en).        self
+00004c40: 2e6c 696e 655f 322e 7365 744f 626a 6563  .line_2.setObjec
+00004c50: 744e 616d 6528 226c 696e 655f 3222 290a  tName("line_2").
+00004c60: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
+00004c70: 644c 6179 6f75 745f 322e 6164 6457 6964  dLayout_2.addWid
+00004c80: 6765 7428 7365 6c66 2e6c 696e 655f 322c  get(self.line_2,
+00004c90: 2031 342c 2030 2c20 312c 2033 290a 2020   14, 0, 1, 3).  
+00004ca0: 2020 2020 2020 7365 6c66 2e63 6d62 5f73        self.cmb_s
+00004cb0: 616d 706c 6554 7970 6520 3d20 5174 5769  ampleType = QtWi
+00004cc0: 6467 6574 732e 5143 6f6d 626f 426f 7828  dgets.QComboBox(
+00004cd0: 7061 7265 6e74 3d73 656c 662e 7363 726f  parent=self.scro
+00004ce0: 6c6c 4172 6561 5769 6467 6574 436f 6e74  llAreaWidgetCont
+00004cf0: 656e 7473 5f32 290a 2020 2020 2020 2020  ents_2).        
+00004d00: 7365 6c66 2e63 6d62 5f73 616d 706c 6554  self.cmb_sampleT
+00004d10: 7970 652e 7365 744f 626a 6563 744e 616d  ype.setObjectNam
+00004d20: 6528 2263 6d62 5f73 616d 706c 6554 7970  e("cmb_sampleTyp
+00004d30: 6522 290a 2020 2020 2020 2020 7365 6c66  e").        self
+00004d40: 2e63 6d62 5f73 616d 706c 6554 7970 652e  .cmb_sampleType.
+00004d50: 6164 6449 7465 6d28 2222 290a 2020 2020  addItem("").    
+00004d60: 2020 2020 7365 6c66 2e63 6d62 5f73 616d      self.cmb_sam
+00004d70: 706c 6554 7970 652e 6164 6449 7465 6d28  pleType.addItem(
+00004d80: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
+00004d90: 2e67 7269 644c 6179 6f75 745f 322e 6164  .gridLayout_2.ad
+00004da0: 6457 6964 6765 7428 7365 6c66 2e63 6d62  dWidget(self.cmb
+00004db0: 5f73 616d 706c 6554 7970 652c 2033 322c  _sampleType, 32,
+00004dc0: 2031 2c20 312c 2031 290a 2020 2020 2020   1, 1, 1).      
+00004dd0: 2020 7365 6c66 2e73 6361 6c65 5f6d 656e    self.scale_men
+00004de0: 7520 3d20 5174 5769 6467 6574 732e 5146  u = QtWidgets.QF
+00004df0: 7261 6d65 2870 6172 656e 743d 7365 6c66  rame(parent=self
+00004e00: 2e73 6372 6f6c 6c41 7265 6157 6964 6765  .scrollAreaWidge
+00004e10: 7443 6f6e 7465 6e74 735f 3229 0a20 2020  tContents_2).   
+00004e20: 2020 2020 2073 656c 662e 7363 616c 655f       self.scale_
+00004e30: 6d65 6e75 2e73 6574 456e 6162 6c65 6428  menu.setEnabled(
+00004e40: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
+00004e50: 697a 6550 6f6c 6963 7920 3d20 5174 5769  izePolicy = QtWi
+00004e60: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
+00004e70: 7928 5174 5769 6467 6574 732e 5153 697a  y(QtWidgets.QSiz
+00004e80: 6550 6f6c 6963 792e 506f 6c69 6379 2e50  ePolicy.Policy.P
+00004e90: 7265 6665 7272 6564 2c20 5174 5769 6467  referred, QtWidg
+00004ea0: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
+00004eb0: 506f 6c69 6379 2e46 6978 6564 290a 2020  Policy.Fixed).  
+00004ec0: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
+00004ed0: 2e73 6574 486f 7269 7a6f 6e74 616c 5374  .setHorizontalSt
+00004ee0: 7265 7463 6828 3029 0a20 2020 2020 2020  retch(0).       
+00004ef0: 2073 697a 6550 6f6c 6963 792e 7365 7456   sizePolicy.setV
+00004f00: 6572 7469 6361 6c53 7472 6574 6368 2830  erticalStretch(0
+00004f10: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
+00004f20: 6c69 6379 2e73 6574 4865 6967 6874 466f  licy.setHeightFo
+00004f30: 7257 6964 7468 2873 656c 662e 7363 616c  rWidth(self.scal
+00004f40: 655f 6d65 6e75 2e73 697a 6550 6f6c 6963  e_menu.sizePolic
+00004f50: 7928 292e 6861 7348 6569 6768 7446 6f72  y().hasHeightFor
+00004f60: 5769 6474 6828 2929 0a20 2020 2020 2020  Width()).       
+00004f70: 2073 656c 662e 7363 616c 655f 6d65 6e75   self.scale_menu
+00004f80: 2e73 6574 5369 7a65 506f 6c69 6379 2873  .setSizePolicy(s
+00004f90: 697a 6550 6f6c 6963 7929 0a20 2020 2020  izePolicy).     
+00004fa0: 2020 2073 656c 662e 7363 616c 655f 6d65     self.scale_me
+00004fb0: 6e75 2e73 6574 4672 616d 6553 6861 7065  nu.setFrameShape
+00004fc0: 2851 7457 6964 6765 7473 2e51 4672 616d  (QtWidgets.QFram
+00004fd0: 652e 5368 6170 652e 5374 796c 6564 5061  e.Shape.StyledPa
+00004fe0: 6e65 6c29 0a20 2020 2020 2020 2073 656c  nel).        sel
+00004ff0: 662e 7363 616c 655f 6d65 6e75 2e73 6574  f.scale_menu.set
+00005000: 4672 616d 6553 6861 646f 7728 5174 5769  FrameShadow(QtWi
+00005010: 6467 6574 732e 5146 7261 6d65 2e53 6861  dgets.QFrame.Sha
+00005020: 646f 772e 5261 6973 6564 290a 2020 2020  dow.Raised).    
+00005030: 2020 2020 7365 6c66 2e73 6361 6c65 5f6d      self.scale_m
+00005040: 656e 752e 7365 744f 626a 6563 744e 616d  enu.setObjectNam
+00005050: 6528 2273 6361 6c65 5f6d 656e 7522 290a  e("scale_menu").
+00005060: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
+00005070: 644c 6179 6f75 745f 3320 3d20 5174 5769  dLayout_3 = QtWi
+00005080: 6467 6574 732e 5147 7269 644c 6179 6f75  dgets.QGridLayou
+00005090: 7428 7365 6c66 2e73 6361 6c65 5f6d 656e  t(self.scale_men
+000050a0: 7529 0a20 2020 2020 2020 2073 656c 662e  u).        self.
+000050b0: 6772 6964 4c61 796f 7574 5f33 2e73 6574  gridLayout_3.set
+000050c0: 4f62 6a65 6374 4e61 6d65 2822 6772 6964  ObjectName("grid
+000050d0: 4c61 796f 7574 5f33 2229 0a20 2020 2020  Layout_3").     
+000050e0: 2020 2073 656c 662e 6c61 6265 6c5f 3920     self.label_9 
+000050f0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
+00005100: 656c 2870 6172 656e 743d 7365 6c66 2e73  el(parent=self.s
+00005110: 6361 6c65 5f6d 656e 7529 0a20 2020 2020  cale_menu).     
+00005120: 2020 2073 656c 662e 6c61 6265 6c5f 392e     self.label_9.
+00005130: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
+00005140: 6162 656c 5f39 2229 0a20 2020 2020 2020  abel_9").       
+00005150: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
+00005160: 5f33 2e61 6464 5769 6467 6574 2873 656c  _3.addWidget(sel
+00005170: 662e 6c61 6265 6c5f 392c 2030 2c20 302c  f.label_9, 0, 0,
+00005180: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
+00005190: 656c 662e 6c61 6265 6c5f 3820 3d20 5174  elf.label_8 = Qt
+000051a0: 5769 6467 6574 732e 514c 6162 656c 2870  Widgets.QLabel(p
+000051b0: 6172 656e 743d 7365 6c66 2e73 6361 6c65  arent=self.scale
+000051c0: 5f6d 656e 7529 0a20 2020 2020 2020 2073  _menu).        s
+000051d0: 656c 662e 6c61 6265 6c5f 382e 7365 744f  elf.label_8.setO
+000051e0: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+000051f0: 5f38 2229 0a20 2020 2020 2020 2073 656c  _8").        sel
+00005200: 662e 6772 6964 4c61 796f 7574 5f33 2e61  f.gridLayout_3.a
+00005210: 6464 5769 6467 6574 2873 656c 662e 6c61  ddWidget(self.la
+00005220: 6265 6c5f 382c 2031 2c20 302c 2031 2c20  bel_8, 1, 0, 1, 
+00005230: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+00005240: 7465 7874 426f 785f 7363 616c 6555 203d  textBox_scaleU =
+00005250: 2051 7457 6964 6765 7473 2e51 4c69 6e65   QtWidgets.QLine
+00005260: 4564 6974 2870 6172 656e 743d 7365 6c66  Edit(parent=self
+00005270: 2e73 6361 6c65 5f6d 656e 7529 0a20 2020  .scale_menu).   
+00005280: 2020 2020 2073 656c 662e 7465 7874 426f       self.textBo
+00005290: 785f 7363 616c 6555 2e73 6574 4f62 6a65  x_scaleU.setObje
+000052a0: 6374 4e61 6d65 2822 7465 7874 426f 785f  ctName("textBox_
+000052b0: 7363 616c 6555 2229 0a20 2020 2020 2020  scaleU").       
+000052c0: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
+000052d0: 5f33 2e61 6464 5769 6467 6574 2873 656c  _3.addWidget(sel
+000052e0: 662e 7465 7874 426f 785f 7363 616c 6555  f.textBox_scaleU
+000052f0: 2c20 302c 2031 2c20 312c 2031 290a 2020  , 0, 1, 1, 1).  
+00005300: 2020 2020 2020 7365 6c66 2e73 7062 5f73        self.spb_s
+00005310: 6361 6c65 5369 7a65 203d 2051 7457 6964  caleSize = QtWid
+00005320: 6765 7473 2e51 446f 7562 6c65 5370 696e  gets.QDoubleSpin
+00005330: 426f 7828 7061 7265 6e74 3d73 656c 662e  Box(parent=self.
+00005340: 7363 616c 655f 6d65 6e75 290a 2020 2020  scale_menu).    
+00005350: 2020 2020 7365 6c66 2e73 7062 5f73 6361      self.spb_sca
+00005360: 6c65 5369 7a65 2e73 6574 4d61 7869 6d75  leSize.setMaximu
+00005370: 6d28 3939 3939 392e 3029 0a20 2020 2020  m(99999.0).     
+00005380: 2020 2073 656c 662e 7370 625f 7363 616c     self.spb_scal
+00005390: 6553 697a 652e 7365 7453 696e 676c 6553  eSize.setSingleS
+000053a0: 7465 7028 302e 3129 0a20 2020 2020 2020  tep(0.1).       
+000053b0: 2073 656c 662e 7370 625f 7363 616c 6553   self.spb_scaleS
+000053c0: 697a 652e 7365 7450 726f 7065 7274 7928  ize.setProperty(
+000053d0: 2276 616c 7565 222c 2031 2e30 290a 2020  "value", 1.0).  
+000053e0: 2020 2020 2020 7365 6c66 2e73 7062 5f73        self.spb_s
+000053f0: 6361 6c65 5369 7a65 2e73 6574 4f62 6a65  caleSize.setObje
+00005400: 6374 4e61 6d65 2822 7370 625f 7363 616c  ctName("spb_scal
+00005410: 6553 697a 6522 290a 2020 2020 2020 2020  eSize").        
+00005420: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
+00005430: 332e 6164 6457 6964 6765 7428 7365 6c66  3.addWidget(self
+00005440: 2e73 7062 5f73 6361 6c65 5369 7a65 2c20  .spb_scaleSize, 
+00005450: 312c 2031 2c20 312c 2031 290a 2020 2020  1, 1, 1, 1).    
+00005460: 2020 2020 7365 6c66 2e6c 6162 656c 5f31      self.label_1
+00005470: 3020 3d20 5174 5769 6467 6574 732e 514c  0 = QtWidgets.QL
+00005480: 6162 656c 2870 6172 656e 743d 7365 6c66  abel(parent=self
+00005490: 2e73 6361 6c65 5f6d 656e 7529 0a20 2020  .scale_menu).   
+000054a0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+000054b0: 3130 2e73 6574 4f62 6a65 6374 4e61 6d65  10.setObjectName
+000054c0: 2822 6c61 6265 6c5f 3130 2229 0a20 2020  ("label_10").   
+000054d0: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
+000054e0: 796f 7574 5f33 2e61 6464 5769 6467 6574  yout_3.addWidget
+000054f0: 2873 656c 662e 6c61 6265 6c5f 3130 2c20  (self.label_10, 
+00005500: 322c 2030 2c20 312c 2031 290a 2020 2020  2, 0, 1, 1).    
+00005510: 2020 2020 7365 6c66 2e63 6d62 5f73 6361      self.cmb_sca
+00005520: 6c65 506f 7320 3d20 5174 5769 6467 6574  lePos = QtWidget
+00005530: 732e 5143 6f6d 626f 426f 7828 7061 7265  s.QComboBox(pare
+00005540: 6e74 3d73 656c 662e 7363 616c 655f 6d65  nt=self.scale_me
+00005550: 6e75 290a 2020 2020 2020 2020 7365 6c66  nu).        self
+00005560: 2e63 6d62 5f73 6361 6c65 506f 732e 7365  .cmb_scalePos.se
+00005570: 744f 626a 6563 744e 616d 6528 2263 6d62  tObjectName("cmb
+00005580: 5f73 6361 6c65 506f 7322 290a 2020 2020  _scalePos").    
+00005590: 2020 2020 7365 6c66 2e63 6d62 5f73 6361      self.cmb_sca
+000055a0: 6c65 506f 732e 6164 6449 7465 6d28 2222  lePos.addItem(""
+000055b0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+000055c0: 6d62 5f73 6361 6c65 506f 732e 6164 6449  mb_scalePos.addI
+000055d0: 7465 6d28 2222 290a 2020 2020 2020 2020  tem("").        
+000055e0: 7365 6c66 2e63 6d62 5f73 6361 6c65 506f  self.cmb_scalePo
+000055f0: 732e 6164 6449 7465 6d28 2222 290a 2020  s.addItem("").  
+00005600: 2020 2020 2020 7365 6c66 2e63 6d62 5f73        self.cmb_s
+00005610: 6361 6c65 506f 732e 6164 6449 7465 6d28  calePos.addItem(
+00005620: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
+00005630: 2e67 7269 644c 6179 6f75 745f 332e 6164  .gridLayout_3.ad
+00005640: 6457 6964 6765 7428 7365 6c66 2e63 6d62  dWidget(self.cmb
+00005650: 5f73 6361 6c65 506f 732c 2032 2c20 312c  _scalePos, 2, 1,
+00005660: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
+00005670: 656c 662e 6772 6964 4c61 796f 7574 5f32  elf.gridLayout_2
+00005680: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+00005690: 7363 616c 655f 6d65 6e75 2c20 3334 2c20  scale_menu, 34, 
+000056a0: 302c 2031 2c20 3329 0a20 2020 2020 2020  0, 1, 3).       
+000056b0: 2073 656c 662e 6c61 6265 6c5f 3420 3d20   self.label_4 = 
+000056c0: 5174 5769 6467 6574 732e 514c 6162 656c  QtWidgets.QLabel
+000056d0: 2870 6172 656e 743d 7365 6c66 2e73 6372  (parent=self.scr
+000056e0: 6f6c 6c41 7265 6157 6964 6765 7443 6f6e  ollAreaWidgetCon
+000056f0: 7465 6e74 735f 3229 0a20 2020 2020 2020  tents_2).       
+00005700: 2073 656c 662e 6c61 6265 6c5f 342e 7365   self.label_4.se
+00005710: 744c 6179 6f75 7444 6972 6563 7469 6f6e  tLayoutDirection
+00005720: 2851 7443 6f72 652e 5174 2e4c 6179 6f75  (QtCore.Qt.Layou
+00005730: 7444 6972 6563 7469 6f6e 2e4c 6566 7454  tDirection.LeftT
+00005740: 6f52 6967 6874 290a 2020 2020 2020 2020  oRight).        
+00005750: 7365 6c66 2e6c 6162 656c 5f34 2e73 6574  self.label_4.set
+00005760: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
+00005770: 6c5f 3422 290a 2020 2020 2020 2020 7365  l_4").        se
+00005780: 6c66 2e67 7269 644c 6179 6f75 745f 322e  lf.gridLayout_2.
+00005790: 6164 6457 6964 6765 7428 7365 6c66 2e6c  addWidget(self.l
+000057a0: 6162 656c 5f34 2c20 3238 2c20 302c 2031  abel_4, 28, 0, 1
+000057b0: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
+000057c0: 662e 6c61 6265 6c5f 3620 3d20 5174 5769  f.label_6 = QtWi
+000057d0: 6467 6574 732e 514c 6162 656c 2870 6172  dgets.QLabel(par
+000057e0: 656e 743d 7365 6c66 2e73 6372 6f6c 6c41  ent=self.scrollA
+000057f0: 7265 6157 6964 6765 7443 6f6e 7465 6e74  reaWidgetContent
+00005800: 735f 3229 0a20 2020 2020 2020 2073 656c  s_2).        sel
+00005810: 662e 6c61 6265 6c5f 362e 7365 744f 626a  f.label_6.setObj
+00005820: 6563 744e 616d 6528 226c 6162 656c 5f36  ectName("label_6
+00005830: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00005840: 6772 6964 4c61 796f 7574 5f32 2e61 6464  gridLayout_2.add
+00005850: 5769 6467 6574 2873 656c 662e 6c61 6265  Widget(self.labe
+00005860: 6c5f 362c 2033 322c 2030 2c20 312c 2031  l_6, 32, 0, 1, 1
+00005870: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00005880: 6162 656c 5f37 203d 2051 7457 6964 6765  abel_7 = QtWidge
+00005890: 7473 2e51 4c61 6265 6c28 7061 7265 6e74  ts.QLabel(parent
+000058a0: 3d73 656c 662e 7363 726f 6c6c 4172 6561  =self.scrollArea
+000058b0: 5769 6467 6574 436f 6e74 656e 7473 5f32  WidgetContents_2
+000058c0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+000058d0: 6162 656c 5f37 2e73 6574 4f62 6a65 6374  abel_7.setObject
+000058e0: 4e61 6d65 2822 6c61 6265 6c5f 3722 290a  Name("label_7").
+000058f0: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
+00005900: 644c 6179 6f75 745f 322e 6164 6457 6964  dLayout_2.addWid
+00005910: 6765 7428 7365 6c66 2e6c 6162 656c 5f37  get(self.label_7
+00005920: 2c20 3333 2c20 302c 2031 2c20 3129 0a20  , 33, 0, 1, 1). 
+00005930: 2020 2020 2020 2073 656c 662e 6c69 6e65         self.line
+00005940: 203d 2051 7457 6964 6765 7473 2e51 4672   = QtWidgets.QFr
+00005950: 616d 6528 7061 7265 6e74 3d73 656c 662e  ame(parent=self.
+00005960: 7363 726f 6c6c 4172 6561 5769 6467 6574  scrollAreaWidget
+00005970: 436f 6e74 656e 7473 5f32 290a 2020 2020  Contents_2).    
+00005980: 2020 2020 7365 6c66 2e6c 696e 652e 7365      self.line.se
+00005990: 7446 7261 6d65 5368 6170 6528 5174 5769  tFrameShape(QtWi
+000059a0: 6467 6574 732e 5146 7261 6d65 2e53 6861  dgets.QFrame.Sha
+000059b0: 7065 2e48 4c69 6e65 290a 2020 2020 2020  pe.HLine).      
+000059c0: 2020 7365 6c66 2e6c 696e 652e 7365 7446    self.line.setF
+000059d0: 7261 6d65 5368 6164 6f77 2851 7457 6964  rameShadow(QtWid
+000059e0: 6765 7473 2e51 4672 616d 652e 5368 6164  gets.QFrame.Shad
+000059f0: 6f77 2e53 756e 6b65 6e29 0a20 2020 2020  ow.Sunken).     
+00005a00: 2020 2073 656c 662e 6c69 6e65 2e73 6574     self.line.set
+00005a10: 4f62 6a65 6374 4e61 6d65 2822 6c69 6e65  ObjectName("line
+00005a20: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00005a30: 6772 6964 4c61 796f 7574 5f32 2e61 6464  gridLayout_2.add
+00005a40: 5769 6467 6574 2873 656c 662e 6c69 6e65  Widget(self.line
+00005a50: 2c20 352c 2030 2c20 312c 2033 290a 2020  , 5, 0, 1, 3).  
+00005a60: 2020 2020 2020 7365 6c66 2e6c 696e 655f        self.line_
+00005a70: 3320 3d20 5174 5769 6467 6574 732e 5146  3 = QtWidgets.QF
+00005a80: 7261 6d65 2870 6172 656e 743d 7365 6c66  rame(parent=self
+00005a90: 2e73 6372 6f6c 6c41 7265 6157 6964 6765  .scrollAreaWidge
+00005aa0: 7443 6f6e 7465 6e74 735f 3229 0a20 2020  tContents_2).   
+00005ab0: 2020 2020 2073 656c 662e 6c69 6e65 5f33       self.line_3
+00005ac0: 2e73 6574 4672 616d 6553 6861 7065 2851  .setFrameShape(Q
+00005ad0: 7457 6964 6765 7473 2e51 4672 616d 652e  tWidgets.QFrame.
+00005ae0: 5368 6170 652e 484c 696e 6529 0a20 2020  Shape.HLine).   
+00005af0: 2020 2020 2073 656c 662e 6c69 6e65 5f33       self.line_3
+00005b00: 2e73 6574 4672 616d 6553 6861 646f 7728  .setFrameShadow(
+00005b10: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
+00005b20: 2e53 6861 646f 772e 5375 6e6b 656e 290a  .Shadow.Sunken).
+00005b30: 2020 2020 2020 2020 7365 6c66 2e6c 696e          self.lin
+00005b40: 655f 332e 7365 744f 626a 6563 744e 616d  e_3.setObjectNam
+00005b50: 6528 226c 696e 655f 3322 290a 2020 2020  e("line_3").    
+00005b60: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
+00005b70: 6f75 745f 322e 6164 6457 6964 6765 7428  out_2.addWidget(
+00005b80: 7365 6c66 2e6c 696e 655f 332c 2032 372c  self.line_3, 27,
+00005b90: 2030 2c20 312c 2033 290a 2020 2020 2020   0, 1, 3).      
+00005ba0: 2020 7365 6c66 2e6c 6162 656c 5f66 6f6c    self.label_fol
+00005bb0: 6461 203d 2051 7457 6964 6765 7473 2e51  da = QtWidgets.Q
+00005bc0: 4c61 6265 6c28 7061 7265 6e74 3d73 656c  Label(parent=sel
+00005bd0: 662e 7363 726f 6c6c 4172 6561 5769 6467  f.scrollAreaWidg
+00005be0: 6574 436f 6e74 656e 7473 5f32 290a 2020  etContents_2).  
+00005bf0: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
+00005c00: 203d 2051 7457 6964 6765 7473 2e51 5369   = QtWidgets.QSi
+00005c10: 7a65 506f 6c69 6379 2851 7457 6964 6765  zePolicy(QtWidge
+00005c20: 7473 2e51 5369 7a65 506f 6c69 6379 2e50  ts.QSizePolicy.P
+00005c30: 6f6c 6963 792e 5072 6566 6572 7265 642c  olicy.Preferred,
+00005c40: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
+00005c50: 506f 6c69 6379 2e50 6f6c 6963 792e 4669  Policy.Policy.Fi
+00005c60: 7865 6429 0a20 2020 2020 2020 2073 697a  xed).        siz
+00005c70: 6550 6f6c 6963 792e 7365 7448 6f72 697a  ePolicy.setHoriz
+00005c80: 6f6e 7461 6c53 7472 6574 6368 2830 290a  ontalStretch(0).
+00005c90: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
+00005ca0: 6379 2e73 6574 5665 7274 6963 616c 5374  cy.setVerticalSt
+00005cb0: 7265 7463 6828 3029 0a20 2020 2020 2020  retch(0).       
+00005cc0: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
+00005cd0: 6569 6768 7446 6f72 5769 6474 6828 7365  eightForWidth(se
+00005ce0: 6c66 2e6c 6162 656c 5f66 6f6c 6461 2e73  lf.label_folda.s
+00005cf0: 697a 6550 6f6c 6963 7928 292e 6861 7348  izePolicy().hasH
+00005d00: 6569 6768 7446 6f72 5769 6474 6828 2929  eightForWidth())
+00005d10: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00005d20: 6265 6c5f 666f 6c64 612e 7365 7453 697a  bel_folda.setSiz
+00005d30: 6550 6f6c 6963 7928 7369 7a65 506f 6c69  ePolicy(sizePoli
+00005d40: 6379 290a 2020 2020 2020 2020 7365 6c66  cy).        self
+00005d50: 2e6c 6162 656c 5f66 6f6c 6461 2e73 6574  .label_folda.set
+00005d60: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
+00005d70: 6c5f 666f 6c64 6122 290a 2020 2020 2020  l_folda").      
+00005d80: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
+00005d90: 745f 322e 6164 6457 6964 6765 7428 7365  t_2.addWidget(se
+00005da0: 6c66 2e6c 6162 656c 5f66 6f6c 6461 2c20  lf.label_folda, 
+00005db0: 312c 2030 2c20 312c 2031 290a 2020 2020  1, 0, 1, 1).    
+00005dc0: 2020 2020 7365 6c66 2e63 625f 7361 7665      self.cb_save
+00005dd0: 416c 6c20 3d20 5174 5769 6467 6574 732e  All = QtWidgets.
+00005de0: 5143 6865 636b 426f 7828 7061 7265 6e74  QCheckBox(parent
+00005df0: 3d73 656c 662e 7363 726f 6c6c 4172 6561  =self.scrollArea
+00005e00: 5769 6467 6574 436f 6e74 656e 7473 5f32  WidgetContents_2
+00005e10: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00005e20: 625f 7361 7665 416c 6c2e 7365 744f 626a  b_saveAll.setObj
+00005e30: 6563 744e 616d 6528 2263 625f 7361 7665  ectName("cb_save
+00005e40: 416c 6c22 290a 2020 2020 2020 2020 7365  All").        se
+00005e50: 6c66 2e67 7269 644c 6179 6f75 745f 322e  lf.gridLayout_2.
+00005e60: 6164 6457 6964 6765 7428 7365 6c66 2e63  addWidget(self.c
+00005e70: 625f 7361 7665 416c 6c2c 2032 352c 2030  b_saveAll, 25, 0
+00005e80: 2c20 312c 2033 290a 2020 2020 2020 2020  , 1, 3).        
+00005e90: 7365 6c66 2e6c 6162 656c 5f31 3720 3d20  self.label_17 = 
+00005ea0: 5174 5769 6467 6574 732e 514c 6162 656c  QtWidgets.QLabel
+00005eb0: 2870 6172 656e 743d 7365 6c66 2e73 6372  (parent=self.scr
+00005ec0: 6f6c 6c41 7265 6157 6964 6765 7443 6f6e  ollAreaWidgetCon
+00005ed0: 7465 6e74 735f 3229 0a20 2020 2020 2020  tents_2).       
+00005ee0: 2073 697a 6550 6f6c 6963 7920 3d20 5174   sizePolicy = Qt
+00005ef0: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
+00005f00: 6963 7928 5174 5769 6467 6574 732e 5153  icy(QtWidgets.QS
+00005f10: 697a 6550 6f6c 6963 792e 506f 6c69 6379  izePolicy.Policy
+00005f20: 2e50 7265 6665 7272 6564 2c20 5174 5769  .Preferred, QtWi
+00005f30: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
+00005f40: 792e 506f 6c69 6379 2e46 6978 6564 290a  y.Policy.Fixed).
+00005f50: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
+00005f60: 6379 2e73 6574 486f 7269 7a6f 6e74 616c  cy.setHorizontal
+00005f70: 5374 7265 7463 6828 3029 0a20 2020 2020  Stretch(0).     
+00005f80: 2020 2073 697a 6550 6f6c 6963 792e 7365     sizePolicy.se
+00005f90: 7456 6572 7469 6361 6c53 7472 6574 6368  tVerticalStretch
+00005fa0: 2830 290a 2020 2020 2020 2020 7369 7a65  (0).        size
+00005fb0: 506f 6c69 6379 2e73 6574 4865 6967 6874  Policy.setHeight
+00005fc0: 466f 7257 6964 7468 2873 656c 662e 6c61  ForWidth(self.la
+00005fd0: 6265 6c5f 3137 2e73 697a 6550 6f6c 6963  bel_17.sizePolic
+00005fe0: 7928 292e 6861 7348 6569 6768 7446 6f72  y().hasHeightFor
+00005ff0: 5769 6474 6828 2929 0a20 2020 2020 2020  Width()).       
+00006000: 2073 656c 662e 6c61 6265 6c5f 3137 2e73   self.label_17.s
+00006010: 6574 5369 7a65 506f 6c69 6379 2873 697a  etSizePolicy(siz
+00006020: 6550 6f6c 6963 7929 0a20 2020 2020 2020  ePolicy).       
+00006030: 2073 656c 662e 6c61 6265 6c5f 3137 2e73   self.label_17.s
+00006040: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
+00006050: 6265 6c5f 3137 2229 0a20 2020 2020 2020  bel_17").       
+00006060: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
+00006070: 5f32 2e61 6464 5769 6467 6574 2873 656c  _2.addWidget(sel
+00006080: 662e 6c61 6265 6c5f 3137 2c20 3132 2c20  f.label_17, 12, 
+00006090: 302c 2031 2c20 3129 0a20 2020 2020 2020  0, 1, 1).       
+000060a0: 2073 656c 662e 6c61 6265 6c5f 7361 7665   self.label_save
+000060b0: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
+000060c0: 6265 6c28 7061 7265 6e74 3d73 656c 662e  bel(parent=self.
+000060d0: 7363 726f 6c6c 4172 6561 5769 6467 6574  scrollAreaWidget
+000060e0: 436f 6e74 656e 7473 5f32 290a 2020 2020  Contents_2).    
+000060f0: 2020 2020 7369 7a65 506f 6c69 6379 203d      sizePolicy =
+00006100: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
+00006110: 506f 6c69 6379 2851 7457 6964 6765 7473  Policy(QtWidgets
+00006120: 2e51 5369 7a65 506f 6c69 6379 2e50 6f6c  .QSizePolicy.Pol
+00006130: 6963 792e 5072 6566 6572 7265 642c 2051  icy.Preferred, Q
+00006140: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
+00006150: 6c69 6379 2e50 6f6c 6963 792e 4669 7865  licy.Policy.Fixe
+00006160: 6429 0a20 2020 2020 2020 2073 697a 6550  d).        sizeP
+00006170: 6f6c 6963 792e 7365 7448 6f72 697a 6f6e  olicy.setHorizon
+00006180: 7461 6c53 7472 6574 6368 2830 290a 2020  talStretch(0).  
+00006190: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
+000061a0: 2e73 6574 5665 7274 6963 616c 5374 7265  .setVerticalStre
+000061b0: 7463 6828 3029 0a20 2020 2020 2020 2073  tch(0).        s
+000061c0: 697a 6550 6f6c 6963 792e 7365 7448 6569  izePolicy.setHei
+000061d0: 6768 7446 6f72 5769 6474 6828 7365 6c66  ghtForWidth(self
+000061e0: 2e6c 6162 656c 5f73 6176 652e 7369 7a65  .label_save.size
+000061f0: 506f 6c69 6379 2829 2e68 6173 4865 6967  Policy().hasHeig
+00006200: 6874 466f 7257 6964 7468 2829 290a 2020  htForWidth()).  
+00006210: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00006220: 5f73 6176 652e 7365 7453 697a 6550 6f6c  _save.setSizePol
+00006230: 6963 7928 7369 7a65 506f 6c69 6379 290a  icy(sizePolicy).
+00006240: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00006250: 656c 5f73 6176 652e 7365 744f 626a 6563  el_save.setObjec
+00006260: 744e 616d 6528 226c 6162 656c 5f73 6176  tName("label_sav
+00006270: 6522 290a 2020 2020 2020 2020 7365 6c66  e").        self
+00006280: 2e67 7269 644c 6179 6f75 745f 322e 6164  .gridLayout_2.ad
+00006290: 6457 6964 6765 7428 7365 6c66 2e6c 6162  dWidget(self.lab
+000062a0: 656c 5f73 6176 652c 2033 2c20 302c 2031  el_save, 3, 0, 1
+000062b0: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
+000062c0: 662e 6c61 6265 6c5f 3520 3d20 5174 5769  f.label_5 = QtWi
+000062d0: 6467 6574 732e 514c 6162 656c 2870 6172  dgets.QLabel(par
+000062e0: 656e 743d 7365 6c66 2e73 6372 6f6c 6c41  ent=self.scrollA
+000062f0: 7265 6157 6964 6765 7443 6f6e 7465 6e74  reaWidgetContent
+00006300: 735f 3229 0a20 2020 2020 2020 2073 656c  s_2).        sel
+00006310: 662e 6c61 6265 6c5f 352e 7365 744c 6179  f.label_5.setLay
+00006320: 6f75 7444 6972 6563 7469 6f6e 2851 7443  outDirection(QtC
+00006330: 6f72 652e 5174 2e4c 6179 6f75 7444 6972  ore.Qt.LayoutDir
+00006340: 6563 7469 6f6e 2e4c 6566 7454 6f52 6967  ection.LeftToRig
+00006350: 6874 290a 2020 2020 2020 2020 7365 6c66  ht).        self
+00006360: 2e6c 6162 656c 5f35 2e73 6574 4f62 6a65  .label_5.setObje
+00006370: 6374 4e61 6d65 2822 6c61 6265 6c5f 3522  ctName("label_5"
+00006380: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00006390: 7269 644c 6179 6f75 745f 322e 6164 6457  ridLayout_2.addW
+000063a0: 6964 6765 7428 7365 6c66 2e6c 6162 656c  idget(self.label
+000063b0: 5f35 2c20 3331 2c20 302c 2031 2c20 3129  _5, 31, 0, 1, 1)
+000063c0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+000063d0: 6265 6c5f 3320 3d20 5174 5769 6467 6574  bel_3 = QtWidget
+000063e0: 732e 514c 6162 656c 2870 6172 656e 743d  s.QLabel(parent=
+000063f0: 7365 6c66 2e73 6372 6f6c 6c41 7265 6157  self.scrollAreaW
+00006400: 6964 6765 7443 6f6e 7465 6e74 735f 3229  idgetContents_2)
+00006410: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+00006420: 6963 7920 3d20 5174 5769 6467 6574 732e  icy = QtWidgets.
+00006430: 5153 697a 6550 6f6c 6963 7928 5174 5769  QSizePolicy(QtWi
+00006440: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
+00006450: 792e 506f 6c69 6379 2e50 7265 6665 7272  y.Policy.Preferr
+00006460: 6564 2c20 5174 5769 6467 6574 732e 5153  ed, QtWidgets.QS
+00006470: 697a 6550 6f6c 6963 792e 506f 6c69 6379  izePolicy.Policy
+00006480: 2e46 6978 6564 290a 2020 2020 2020 2020  .Fixed).        
+00006490: 7369 7a65 506f 6c69 6379 2e73 6574 486f  sizePolicy.setHo
+000064a0: 7269 7a6f 6e74 616c 5374 7265 7463 6828  rizontalStretch(
+000064b0: 3029 0a20 2020 2020 2020 2073 697a 6550  0).        sizeP
+000064c0: 6f6c 6963 792e 7365 7456 6572 7469 6361  olicy.setVertica
+000064d0: 6c53 7472 6574 6368 2830 290a 2020 2020  lStretch(0).    
+000064e0: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
+000064f0: 6574 4865 6967 6874 466f 7257 6964 7468  etHeightForWidth
+00006500: 2873 656c 662e 6c61 6265 6c5f 332e 7369  (self.label_3.si
+00006510: 7a65 506f 6c69 6379 2829 2e68 6173 4865  zePolicy().hasHe
+00006520: 6967 6874 466f 7257 6964 7468 2829 290a  ightForWidth()).
+00006530: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00006540: 656c 5f33 2e73 6574 5369 7a65 506f 6c69  el_3.setSizePoli
+00006550: 6379 2873 697a 6550 6f6c 6963 7929 0a20  cy(sizePolicy). 
+00006560: 2020 2020 2020 2066 6f6e 7420 3d20 5174         font = Qt
+00006570: 4775 692e 5146 6f6e 7428 290a 2020 2020  Gui.QFont().    
+00006580: 2020 2020 666f 6e74 2e73 6574 426f 6c64      font.setBold
+00006590: 2854 7275 6529 0a20 2020 2020 2020 2066  (True).        f
+000065a0: 6f6e 742e 7365 7455 6e64 6572 6c69 6e65  ont.setUnderline
+000065b0: 2854 7275 6529 0a20 2020 2020 2020 2066  (True).        f
+000065c0: 6f6e 742e 7365 7457 6569 6768 7428 3735  ont.setWeight(75
+000065d0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+000065e0: 6162 656c 5f33 2e73 6574 466f 6e74 2866  abel_3.setFont(f
+000065f0: 6f6e 7429 0a20 2020 2020 2020 2073 656c  ont).        sel
+00006600: 662e 6c61 6265 6c5f 332e 7365 744f 626a  f.label_3.setObj
+00006610: 6563 744e 616d 6528 226c 6162 656c 5f33  ectName("label_3
+00006620: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00006630: 6772 6964 4c61 796f 7574 5f32 2e61 6464  gridLayout_2.add
+00006640: 5769 6467 6574 2873 656c 662e 6c61 6265  Widget(self.labe
+00006650: 6c5f 332c 2030 2c20 302c 2031 2c20 3329  l_3, 0, 0, 1, 3)
+00006660: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00006670: 6e65 5f73 6176 6520 3d20 5174 5769 6467  ne_save = QtWidg
+00006680: 6574 732e 514c 696e 6545 6469 7428 7061  ets.QLineEdit(pa
+00006690: 7265 6e74 3d73 656c 662e 7363 726f 6c6c  rent=self.scroll
+000066a0: 4172 6561 5769 6467 6574 436f 6e74 656e  AreaWidgetConten
+000066b0: 7473 5f32 290a 2020 2020 2020 2020 7365  ts_2).        se
+000066c0: 6c66 2e6c 696e 655f 7361 7665 2e73 6574  lf.line_save.set
+000066d0: 5265 6164 4f6e 6c79 2846 616c 7365 290a  ReadOnly(False).
+000066e0: 2020 2020 2020 2020 7365 6c66 2e6c 696e          self.lin
+000066f0: 655f 7361 7665 2e73 6574 4f62 6a65 6374  e_save.setObject
+00006700: 4e61 6d65 2822 6c69 6e65 5f73 6176 6522  Name("line_save"
+00006710: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00006720: 7269 644c 6179 6f75 745f 322e 6164 6457  ridLayout_2.addW
+00006730: 6964 6765 7428 7365 6c66 2e6c 696e 655f  idget(self.line_
+00006740: 7361 7665 2c20 342c 2030 2c20 312c 2031  save, 4, 0, 1, 1
+00006750: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
+00006760: 7574 746f 6e5f 7361 7665 203d 2051 7457  utton_save = QtW
+00006770: 6964 6765 7473 2e51 5075 7368 4275 7474  idgets.QPushButt
+00006780: 6f6e 2870 6172 656e 743d 7365 6c66 2e73  on(parent=self.s
+00006790: 6372 6f6c 6c41 7265 6157 6964 6765 7443  crollAreaWidgetC
+000067a0: 6f6e 7465 6e74 735f 3229 0a20 2020 2020  ontents_2).     
+000067b0: 2020 2073 656c 662e 6275 7474 6f6e 5f73     self.button_s
+000067c0: 6176 652e 7365 744f 626a 6563 744e 616d  ave.setObjectNam
+000067d0: 6528 2262 7574 746f 6e5f 7361 7665 2229  e("button_save")
+000067e0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+000067f0: 6964 4c61 796f 7574 5f32 2e61 6464 5769  idLayout_2.addWi
+00006800: 6467 6574 2873 656c 662e 6275 7474 6f6e  dget(self.button
+00006810: 5f73 6176 652c 2034 2c20 312c 2031 2c20  _save, 4, 1, 1, 
+00006820: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+00006830: 7370 625f 4e20 3d20 5174 5769 6467 6574  spb_N = QtWidget
+00006840: 732e 5153 7069 6e42 6f78 2870 6172 656e  s.QSpinBox(paren
+00006850: 743d 7365 6c66 2e73 6372 6f6c 6c41 7265  t=self.scrollAre
+00006860: 6157 6964 6765 7443 6f6e 7465 6e74 735f  aWidgetContents_
+00006870: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
+00006880: 7370 625f 4e2e 7365 744d 696e 696d 756d  spb_N.setMinimum
+00006890: 2833 290a 2020 2020 2020 2020 7365 6c66  (3).        self
+000068a0: 2e73 7062 5f4e 2e73 6574 4d61 7869 6d75  .spb_N.setMaximu
+000068b0: 6d28 3230 3029 0a20 2020 2020 2020 2073  m(200).        s
+000068c0: 656c 662e 7370 625f 4e2e 7365 7450 726f  elf.spb_N.setPro
+000068d0: 7065 7274 7928 2276 616c 7565 222c 2033  perty("value", 3
+000068e0: 3029 0a20 2020 2020 2020 2073 656c 662e  0).        self.
+000068f0: 7370 625f 4e2e 7365 744f 626a 6563 744e  spb_N.setObjectN
+00006900: 616d 6528 2273 7062 5f4e 2229 0a20 2020  ame("spb_N").   
+00006910: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
+00006920: 796f 7574 5f32 2e61 6464 5769 6467 6574  yout_2.addWidget
+00006930: 2873 656c 662e 7370 625f 4e2c 2032 382c  (self.spb_N, 28,
+00006940: 2031 2c20 312c 2031 290a 2020 2020 2020   1, 1, 1).      
+00006950: 2020 7365 6c66 2e6c 696e 655f 6865 6164    self.line_head
+00006960: 6572 203d 2051 7457 6964 6765 7473 2e51  er = QtWidgets.Q
+00006970: 4c69 6e65 4564 6974 2870 6172 656e 743d  LineEdit(parent=
+00006980: 7365 6c66 2e73 6372 6f6c 6c41 7265 6157  self.scrollAreaW
+00006990: 6964 6765 7443 6f6e 7465 6e74 735f 3229  idgetContents_2)
+000069a0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000069b0: 6e65 5f68 6561 6465 722e 7365 744f 626a  ne_header.setObj
+000069c0: 6563 744e 616d 6528 226c 696e 655f 6865  ectName("line_he
+000069d0: 6164 6572 2229 0a20 2020 2020 2020 2073  ader").        s
+000069e0: 656c 662e 6772 6964 4c61 796f 7574 5f32  elf.gridLayout_2
+000069f0: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+00006a00: 6c69 6e65 5f68 6561 6465 722c 2031 332c  line_header, 13,
+00006a10: 2030 2c20 312c 2031 290a 2020 2020 2020   0, 1, 1).      
+00006a20: 2020 7365 6c66 2e62 7574 746f 6e5f 6865    self.button_he
+00006a30: 6164 6572 203d 2051 7457 6964 6765 7473  ader = QtWidgets
+00006a40: 2e51 5075 7368 4275 7474 6f6e 2870 6172  .QPushButton(par
+00006a50: 656e 743d 7365 6c66 2e73 6372 6f6c 6c41  ent=self.scrollA
+00006a60: 7265 6157 6964 6765 7443 6f6e 7465 6e74  reaWidgetContent
+00006a70: 735f 3229 0a20 2020 2020 2020 2073 656c  s_2).        sel
+00006a80: 662e 6275 7474 6f6e 5f68 6561 6465 722e  f.button_header.
+00006a90: 7365 744f 626a 6563 744e 616d 6528 2262  setObjectName("b
+00006aa0: 7574 746f 6e5f 6865 6164 6572 2229 0a20  utton_header"). 
+00006ab0: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
+00006ac0: 4c61 796f 7574 5f32 2e61 6464 5769 6467  Layout_2.addWidg
+00006ad0: 6574 2873 656c 662e 6275 7474 6f6e 5f68  et(self.button_h
+00006ae0: 6561 6465 722c 2031 332c 2031 2c20 312c  eader, 13, 1, 1,
+00006af0: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+00006b00: 2e72 625f 6669 6c65 6e61 6d65 203d 2051  .rb_filename = Q
+00006b10: 7457 6964 6765 7473 2e51 5261 6469 6f42  tWidgets.QRadioB
+00006b20: 7574 746f 6e28 7061 7265 6e74 3d73 656c  utton(parent=sel
+00006b30: 662e 7363 726f 6c6c 4172 6561 5769 6467  f.scrollAreaWidg
+00006b40: 6574 436f 6e74 656e 7473 5f32 290a 2020  etContents_2).  
+00006b50: 2020 2020 2020 7365 6c66 2e72 625f 6669        self.rb_fi
+00006b60: 6c65 6e61 6d65 2e73 6574 4f62 6a65 6374  lename.setObject
+00006b70: 4e61 6d65 2822 7262 5f66 696c 656e 616d  Name("rb_filenam
+00006b80: 6522 290a 2020 2020 2020 2020 7365 6c66  e").        self
+00006b90: 2e67 7269 644c 6179 6f75 745f 322e 6164  .gridLayout_2.ad
+00006ba0: 6457 6964 6765 7428 7365 6c66 2e72 625f  dWidget(self.rb_
+00006bb0: 6669 6c65 6e61 6d65 2c20 3131 2c20 302c  filename, 11, 0,
+00006bc0: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
+00006bd0: 656c 662e 7262 5f6e 6f6e 6520 3d20 5174  elf.rb_none = Qt
+00006be0: 5769 6467 6574 732e 5152 6164 696f 4275  Widgets.QRadioBu
+00006bf0: 7474 6f6e 2870 6172 656e 743d 7365 6c66  tton(parent=self
+00006c00: 2e73 6372 6f6c 6c41 7265 6157 6964 6765  .scrollAreaWidge
+00006c10: 7443 6f6e 7465 6e74 735f 3229 0a20 2020  tContents_2).   
+00006c20: 2020 2020 2073 656c 662e 7262 5f6e 6f6e       self.rb_non
+00006c30: 652e 7365 7443 6865 636b 6564 2846 616c  e.setChecked(Fal
+00006c40: 7365 290a 2020 2020 2020 2020 7365 6c66  se).        self
+00006c50: 2e72 625f 6e6f 6e65 2e73 6574 4f62 6a65  .rb_none.setObje
+00006c60: 6374 4e61 6d65 2822 7262 5f6e 6f6e 6522  ctName("rb_none"
+00006c70: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00006c80: 7269 644c 6179 6f75 745f 322e 6164 6457  ridLayout_2.addW
+00006c90: 6964 6765 7428 7365 6c66 2e72 625f 6e6f  idget(self.rb_no
+00006ca0: 6e65 2c20 392c 2030 2c20 312c 2031 290a  ne, 9, 0, 1, 1).
+00006cb0: 2020 2020 2020 2020 7365 6c66 2e72 625f          self.rb_
+00006cc0: 7375 6266 6f6c 6461 203d 2051 7457 6964  subfolda = QtWid
+00006cd0: 6765 7473 2e51 5261 6469 6f42 7574 746f  gets.QRadioButto
+00006ce0: 6e28 7061 7265 6e74 3d73 656c 662e 7363  n(parent=self.sc
+00006cf0: 726f 6c6c 4172 6561 5769 6467 6574 436f  rollAreaWidgetCo
+00006d00: 6e74 656e 7473 5f32 290a 2020 2020 2020  ntents_2).      
+00006d10: 2020 7365 6c66 2e72 625f 7375 6266 6f6c    self.rb_subfol
+00006d20: 6461 2e73 6574 4368 6563 6b65 6428 5472  da.setChecked(Tr
+00006d30: 7565 290a 2020 2020 2020 2020 7365 6c66  ue).        self
+00006d40: 2e72 625f 7375 6266 6f6c 6461 2e73 6574  .rb_subfolda.set
+00006d50: 4f62 6a65 6374 4e61 6d65 2822 7262 5f73  ObjectName("rb_s
+00006d60: 7562 666f 6c64 6122 290a 2020 2020 2020  ubfolda").      
+00006d70: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
+00006d80: 745f 322e 6164 6457 6964 6765 7428 7365  t_2.addWidget(se
+00006d90: 6c66 2e72 625f 7375 6266 6f6c 6461 2c20  lf.rb_subfolda, 
+00006da0: 3130 2c20 302c 2031 2c20 3129 0a20 2020  10, 0, 1, 1).   
+00006db0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00006dc0: 3332 203d 2051 7457 6964 6765 7473 2e51  32 = QtWidgets.Q
+00006dd0: 4c61 6265 6c28 7061 7265 6e74 3d73 656c  Label(parent=sel
+00006de0: 662e 7363 726f 6c6c 4172 6561 5769 6467  f.scrollAreaWidg
+00006df0: 6574 436f 6e74 656e 7473 5f32 290a 2020  etContents_2).  
+00006e00: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
+00006e10: 203d 2051 7457 6964 6765 7473 2e51 5369   = QtWidgets.QSi
+00006e20: 7a65 506f 6c69 6379 2851 7457 6964 6765  zePolicy(QtWidge
+00006e30: 7473 2e51 5369 7a65 506f 6c69 6379 2e50  ts.QSizePolicy.P
+00006e40: 6f6c 6963 792e 5072 6566 6572 7265 642c  olicy.Preferred,
+00006e50: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
+00006e60: 506f 6c69 6379 2e50 6f6c 6963 792e 4669  Policy.Policy.Fi
+00006e70: 7865 6429 0a20 2020 2020 2020 2073 697a  xed).        siz
+00006e80: 6550 6f6c 6963 792e 7365 7448 6f72 697a  ePolicy.setHoriz
+00006e90: 6f6e 7461 6c53 7472 6574 6368 2830 290a  ontalStretch(0).
+00006ea0: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
+00006eb0: 6379 2e73 6574 5665 7274 6963 616c 5374  cy.setVerticalSt
+00006ec0: 7265 7463 6828 3029 0a20 2020 2020 2020  retch(0).       
+00006ed0: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
+00006ee0: 6569 6768 7446 6f72 5769 6474 6828 7365  eightForWidth(se
+00006ef0: 6c66 2e6c 6162 656c 5f33 322e 7369 7a65  lf.label_32.size
+00006f00: 506f 6c69 6379 2829 2e68 6173 4865 6967  Policy().hasHeig
+00006f10: 6874 466f 7257 6964 7468 2829 290a 2020  htForWidth()).  
+00006f20: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00006f30: 5f33 322e 7365 7453 697a 6550 6f6c 6963  _32.setSizePolic
+00006f40: 7928 7369 7a65 506f 6c69 6379 290a 2020  y(sizePolicy).  
+00006f50: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00006f60: 5f33 322e 7365 744f 626a 6563 744e 616d  _32.setObjectNam
+00006f70: 6528 226c 6162 656c 5f33 3222 290a 2020  e("label_32").  
+00006f80: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
+00006f90: 6179 6f75 745f 322e 6164 6457 6964 6765  ayout_2.addWidge
+00006fa0: 7428 7365 6c66 2e6c 6162 656c 5f33 322c  t(self.label_32,
+00006fb0: 2038 2c20 302c 2031 2c20 3129 0a20 2020   8, 0, 1, 1).   
+00006fc0: 2020 2020 2073 656c 662e 7363 726f 6c6c       self.scroll
+00006fd0: 4172 6561 5f32 2e73 6574 5769 6467 6574  Area_2.setWidget
+00006fe0: 2873 656c 662e 7363 726f 6c6c 4172 6561  (self.scrollArea
+00006ff0: 5769 6467 6574 436f 6e74 656e 7473 5f32  WidgetContents_2
+00007000: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00007010: 7269 644c 6179 6f75 745f 392e 6164 6457  ridLayout_9.addW
+00007020: 6964 6765 7428 7365 6c66 2e73 6372 6f6c  idget(self.scrol
+00007030: 6c41 7265 615f 322c 2030 2c20 312c 2031  lArea_2, 0, 1, 1
+00007040: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
+00007050: 662e 6672 616d 6520 3d20 5174 5769 6467  f.frame = QtWidg
+00007060: 6574 732e 5146 7261 6d65 2870 6172 656e  ets.QFrame(paren
+00007070: 743d 7365 6c66 2e74 6162 290a 2020 2020  t=self.tab).    
+00007080: 2020 2020 7369 7a65 506f 6c69 6379 203d      sizePolicy =
+00007090: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
+000070a0: 506f 6c69 6379 2851 7457 6964 6765 7473  Policy(QtWidgets
+000070b0: 2e51 5369 7a65 506f 6c69 6379 2e50 6f6c  .QSizePolicy.Pol
+000070c0: 6963 792e 4578 7061 6e64 696e 672c 2051  icy.Expanding, Q
+000070d0: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
+000070e0: 6c69 6379 2e50 6f6c 6963 792e 4578 7061  licy.Policy.Expa
+000070f0: 6e64 696e 6729 0a20 2020 2020 2020 2073  nding).        s
+00007100: 697a 6550 6f6c 6963 792e 7365 7448 6f72  izePolicy.setHor
+00007110: 697a 6f6e 7461 6c53 7472 6574 6368 2830  izontalStretch(0
+00007120: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
+00007130: 6c69 6379 2e73 6574 5665 7274 6963 616c  licy.setVertical
+00007140: 5374 7265 7463 6828 3029 0a20 2020 2020  Stretch(0).     
+00007150: 2020 2073 697a 6550 6f6c 6963 792e 7365     sizePolicy.se
+00007160: 7448 6569 6768 7446 6f72 5769 6474 6828  tHeightForWidth(
+00007170: 7365 6c66 2e66 7261 6d65 2e73 697a 6550  self.frame.sizeP
+00007180: 6f6c 6963 7928 292e 6861 7348 6569 6768  olicy().hasHeigh
+00007190: 7446 6f72 5769 6474 6828 2929 0a20 2020  tForWidth()).   
+000071a0: 2020 2020 2073 656c 662e 6672 616d 652e       self.frame.
+000071b0: 7365 7453 697a 6550 6f6c 6963 7928 7369  setSizePolicy(si
+000071c0: 7a65 506f 6c69 6379 290a 2020 2020 2020  zePolicy).      
+000071d0: 2020 7365 6c66 2e66 7261 6d65 2e73 6574    self.frame.set
+000071e0: 4d61 7869 6d75 6d53 697a 6528 5174 436f  MaximumSize(QtCo
+000071f0: 7265 2e51 5369 7a65 2835 3030 2c20 3136  re.QSize(500, 16
+00007200: 3737 3732 3135 2929 0a20 2020 2020 2020  777215)).       
+00007210: 2073 656c 662e 6672 616d 652e 7365 7446   self.frame.setF
+00007220: 7261 6d65 5368 6170 6528 5174 5769 6467  rameShape(QtWidg
+00007230: 6574 732e 5146 7261 6d65 2e53 6861 7065  ets.QFrame.Shape
+00007240: 2e53 7479 6c65 6450 616e 656c 290a 2020  .StyledPanel).  
+00007250: 2020 2020 2020 7365 6c66 2e66 7261 6d65        self.frame
+00007260: 2e73 6574 4672 616d 6553 6861 646f 7728  .setFrameShadow(
+00007270: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
+00007280: 2e53 6861 646f 772e 5261 6973 6564 290a  .Shadow.Raised).
+00007290: 2020 2020 2020 2020 7365 6c66 2e66 7261          self.fra
+000072a0: 6d65 2e73 6574 4f62 6a65 6374 4e61 6d65  me.setObjectName
+000072b0: 2822 6672 616d 6522 290a 2020 2020 2020  ("frame").      
+000072c0: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
+000072d0: 745f 3420 3d20 5174 5769 6467 6574 732e  t_4 = QtWidgets.
+000072e0: 5147 7269 644c 6179 6f75 7428 7365 6c66  QGridLayout(self
+000072f0: 2e66 7261 6d65 290a 2020 2020 2020 2020  .frame).        
+00007300: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
+00007310: 342e 7365 744f 626a 6563 744e 616d 6528  4.setObjectName(
+00007320: 2267 7269 644c 6179 6f75 745f 3422 290a  "gridLayout_4").
+00007330: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00007340: 6772 6573 7342 6172 203d 2051 7457 6964  gressBar = QtWid
+00007350: 6765 7473 2e51 5072 6f67 7265 7373 4261  gets.QProgressBa
+00007360: 7228 7061 7265 6e74 3d73 656c 662e 6672  r(parent=self.fr
+00007370: 616d 6529 0a20 2020 2020 2020 2073 656c  ame).        sel
+00007380: 662e 7072 6f67 7265 7373 4261 722e 7365  f.progressBar.se
+00007390: 7450 726f 7065 7274 7928 2276 616c 7565  tProperty("value
+000073a0: 222c 2030 290a 2020 2020 2020 2020 7365  ", 0).        se
+000073b0: 6c66 2e70 726f 6772 6573 7342 6172 2e73  lf.progressBar.s
+000073c0: 6574 4f62 6a65 6374 4e61 6d65 2822 7072  etObjectName("pr
+000073d0: 6f67 7265 7373 4261 7222 290a 2020 2020  ogressBar").    
+000073e0: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
+000073f0: 6f75 745f 342e 6164 6457 6964 6765 7428  out_4.addWidget(
+00007400: 7365 6c66 2e70 726f 6772 6573 7342 6172  self.progressBar
+00007410: 2c20 322c 2030 2c20 312c 2031 290a 2020  , 2, 0, 1, 1).  
+00007420: 2020 2020 2020 7365 6c66 2e62 7574 746f        self.butto
+00007430: 6e5f 4650 5320 3d20 5174 5769 6467 6574  n_FPS = QtWidget
+00007440: 732e 5150 7573 6842 7574 746f 6e28 7061  s.QPushButton(pa
+00007450: 7265 6e74 3d73 656c 662e 6672 616d 6529  rent=self.frame)
+00007460: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
+00007470: 6963 7920 3d20 5174 5769 6467 6574 732e  icy = QtWidgets.
+00007480: 5153 697a 6550 6f6c 6963 7928 5174 5769  QSizePolicy(QtWi
+00007490: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
+000074a0: 792e 506f 6c69 6379 2e46 6978 6564 2c20  y.Policy.Fixed, 
+000074b0: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
+000074c0: 6f6c 6963 792e 506f 6c69 6379 2e46 6978  olicy.Policy.Fix
+000074d0: 6564 290a 2020 2020 2020 2020 7369 7a65  ed).        size
+000074e0: 506f 6c69 6379 2e73 6574 486f 7269 7a6f  Policy.setHorizo
+000074f0: 6e74 616c 5374 7265 7463 6828 3029 0a20  ntalStretch(0). 
+00007500: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
+00007510: 792e 7365 7456 6572 7469 6361 6c53 7472  y.setVerticalStr
+00007520: 6574 6368 2830 290a 2020 2020 2020 2020  etch(0).        
+00007530: 7369 7a65 506f 6c69 6379 2e73 6574 4865  sizePolicy.setHe
+00007540: 6967 6874 466f 7257 6964 7468 2873 656c  ightForWidth(sel
+00007550: 662e 6275 7474 6f6e 5f46 5053 2e73 697a  f.button_FPS.siz
+00007560: 6550 6f6c 6963 7928 292e 6861 7348 6569  ePolicy().hasHei
+00007570: 6768 7446 6f72 5769 6474 6828 2929 0a20  ghtForWidth()). 
+00007580: 2020 2020 2020 2073 656c 662e 6275 7474         self.butt
+00007590: 6f6e 5f46 5053 2e73 6574 5369 7a65 506f  on_FPS.setSizePo
+000075a0: 6c69 6379 2873 697a 6550 6f6c 6963 7929  licy(sizePolicy)
+000075b0: 0a20 2020 2020 2020 2073 656c 662e 6275  .        self.bu
+000075c0: 7474 6f6e 5f46 5053 2e73 6574 4f62 6a65  tton_FPS.setObje
+000075d0: 6374 4e61 6d65 2822 6275 7474 6f6e 5f46  ctName("button_F
+000075e0: 5053 2229 0a20 2020 2020 2020 2073 656c  PS").        sel
+000075f0: 662e 6772 6964 4c61 796f 7574 5f34 2e61  f.gridLayout_4.a
+00007600: 6464 5769 6467 6574 2873 656c 662e 6275  ddWidget(self.bu
+00007610: 7474 6f6e 5f46 5053 2c20 322c 2031 2c20  tton_FPS, 2, 1, 
+00007620: 312c 2031 290a 2020 2020 2020 2020 7365  1, 1).        se
+00007630: 6c66 2e6c 6f67 626f 7820 3d20 5174 5769  lf.logbox = QtWi
+00007640: 6467 6574 732e 5154 6578 7445 6469 7428  dgets.QTextEdit(
+00007650: 7061 7265 6e74 3d73 656c 662e 6672 616d  parent=self.fram
+00007660: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+00007670: 6c6f 6762 6f78 2e73 6574 4f62 6a65 6374  logbox.setObject
+00007680: 4e61 6d65 2822 6c6f 6762 6f78 2229 0a20  Name("logbox"). 
+00007690: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
+000076a0: 4c61 796f 7574 5f34 2e61 6464 5769 6467  Layout_4.addWidg
+000076b0: 6574 2873 656c 662e 6c6f 6762 6f78 2c20  et(self.logbox, 
+000076c0: 312c 2030 2c20 312c 2032 290a 2020 2020  1, 0, 1, 2).    
+000076d0: 2020 2020 7365 6c66 2e6c 6162 656c 5f32      self.label_2
+000076e0: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
+000076f0: 6265 6c28 7061 7265 6e74 3d73 656c 662e  bel(parent=self.
+00007700: 6672 616d 6529 0a20 2020 2020 2020 2066  frame).        f
+00007710: 6f6e 7420 3d20 5174 4775 692e 5146 6f6e  ont = QtGui.QFon
+00007720: 7428 290a 2020 2020 2020 2020 666f 6e74  t().        font
+00007730: 2e73 6574 426f 6c64 2854 7275 6529 0a20  .setBold(True). 
+00007740: 2020 2020 2020 2066 6f6e 742e 7365 7457         font.setW
+00007750: 6569 6768 7428 3735 290a 2020 2020 2020  eight(75).      
+00007760: 2020 7365 6c66 2e6c 6162 656c 5f32 2e73    self.label_2.s
+00007770: 6574 466f 6e74 2866 6f6e 7429 0a20 2020  etFont(font).   
+00007780: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00007790: 322e 7365 744f 626a 6563 744e 616d 6528  2.setObjectName(
+000077a0: 226c 6162 656c 5f32 2229 0a20 2020 2020  "label_2").     
+000077b0: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
+000077c0: 7574 5f34 2e61 6464 5769 6467 6574 2873  ut_4.addWidget(s
+000077d0: 656c 662e 6c61 6265 6c5f 322c 2030 2c20  elf.label_2, 0, 
+000077e0: 302c 2031 2c20 3129 0a20 2020 2020 2020  0, 1, 1).       
+000077f0: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
+00007800: 5f39 2e61 6464 5769 6467 6574 2873 656c  _9.addWidget(sel
+00007810: 662e 6672 616d 652c 2030 2c20 322c 2031  f.frame, 0, 2, 1
+00007820: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
+00007830: 662e 7461 6257 6964 6765 742e 6164 6454  f.tabWidget.addT
+00007840: 6162 2873 656c 662e 7461 622c 2022 2229  ab(self.tab, "")
+00007850: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+00007860: 625f 3220 3d20 5174 5769 6467 6574 732e  b_2 = QtWidgets.
+00007870: 5157 6964 6765 7428 290a 2020 2020 2020  QWidget().      
+00007880: 2020 7365 6c66 2e74 6162 5f32 2e73 6574    self.tab_2.set
+00007890: 4f62 6a65 6374 4e61 6d65 2822 7461 625f  ObjectName("tab_
+000078a0: 3222 290a 2020 2020 2020 2020 7365 6c66  2").        self
+000078b0: 2e68 6f72 697a 6f6e 7461 6c4c 6179 6f75  .horizontalLayou
+000078c0: 7420 3d20 5174 5769 6467 6574 732e 5148  t = QtWidgets.QH
+000078d0: 426f 784c 6179 6f75 7428 7365 6c66 2e74  BoxLayout(self.t
+000078e0: 6162 5f32 290a 2020 2020 2020 2020 7365  ab_2).        se
+000078f0: 6c66 2e68 6f72 697a 6f6e 7461 6c4c 6179  lf.horizontalLay
+00007900: 6f75 742e 7365 744f 626a 6563 744e 616d  out.setObjectNam
+00007910: 6528 2268 6f72 697a 6f6e 7461 6c4c 6179  e("horizontalLay
+00007920: 6f75 7422 290a 2020 2020 2020 2020 7365  out").        se
+00007930: 6c66 2e73 6372 6f6c 6c41 7265 6120 3d20  lf.scrollArea = 
+00007940: 5174 5769 6467 6574 732e 5153 6372 6f6c  QtWidgets.QScrol
+00007950: 6c41 7265 6128 7061 7265 6e74 3d73 656c  lArea(parent=sel
+00007960: 662e 7461 625f 3229 0a20 2020 2020 2020  f.tab_2).       
+00007970: 2073 656c 662e 7363 726f 6c6c 4172 6561   self.scrollArea
+00007980: 2e73 6574 4d69 6e69 6d75 6d53 697a 6528  .setMinimumSize(
+00007990: 5174 436f 7265 2e51 5369 7a65 2832 3430  QtCore.QSize(240
+000079a0: 2c20 3029 290a 2020 2020 2020 2020 7365  , 0)).        se
+000079b0: 6c66 2e73 6372 6f6c 6c41 7265 612e 7365  lf.scrollArea.se
+000079c0: 744d 6178 696d 756d 5369 7a65 2851 7443  tMaximumSize(QtC
+000079d0: 6f72 652e 5153 697a 6528 3330 302c 2031  ore.QSize(300, 1
+000079e0: 3637 3737 3231 3529 290a 2020 2020 2020  6777215)).      
+000079f0: 2020 7365 6c66 2e73 6372 6f6c 6c41 7265    self.scrollAre
+00007a00: 612e 7365 7457 6964 6765 7452 6573 697a  a.setWidgetResiz
+00007a10: 6162 6c65 2854 7275 6529 0a20 2020 2020  able(True).     
+00007a20: 2020 2073 656c 662e 7363 726f 6c6c 4172     self.scrollAr
+00007a30: 6561 2e73 6574 4f62 6a65 6374 4e61 6d65  ea.setObjectName
+00007a40: 2822 7363 726f 6c6c 4172 6561 2229 0a20  ("scrollArea"). 
+00007a50: 2020 2020 2020 2073 656c 662e 7363 726f         self.scro
+00007a60: 6c6c 4172 6561 5769 6467 6574 436f 6e74  llAreaWidgetCont
+00007a70: 656e 7473 203d 2051 7457 6964 6765 7473  ents = QtWidgets
+00007a80: 2e51 5769 6467 6574 2829 0a20 2020 2020  .QWidget().     
+00007a90: 2020 2073 656c 662e 7363 726f 6c6c 4172     self.scrollAr
+00007aa0: 6561 5769 6467 6574 436f 6e74 656e 7473  eaWidgetContents
+00007ab0: 2e73 6574 4765 6f6d 6574 7279 2851 7443  .setGeometry(QtC
+00007ac0: 6f72 652e 5152 6563 7428 302c 2030 2c20  ore.QRect(0, 0, 
+00007ad0: 3238 312c 2039 3132 2929 0a20 2020 2020  281, 912)).     
+00007ae0: 2020 2073 656c 662e 7363 726f 6c6c 4172     self.scrollAr
+00007af0: 6561 5769 6467 6574 436f 6e74 656e 7473  eaWidgetContents
+00007b00: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00007b10: 7363 726f 6c6c 4172 6561 5769 6467 6574  scrollAreaWidget
+00007b20: 436f 6e74 656e 7473 2229 0a20 2020 2020  Contents").     
+00007b30: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
+00007b40: 7574 5f35 203d 2051 7457 6964 6765 7473  ut_5 = QtWidgets
+00007b50: 2e51 4772 6964 4c61 796f 7574 2873 656c  .QGridLayout(sel
+00007b60: 662e 7363 726f 6c6c 4172 6561 5769 6467  f.scrollAreaWidg
+00007b70: 6574 436f 6e74 656e 7473 290a 2020 2020  etContents).    
+00007b80: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
+00007b90: 6f75 745f 352e 7365 744f 626a 6563 744e  out_5.setObjectN
+00007ba0: 616d 6528 2267 7269 644c 6179 6f75 745f  ame("gridLayout_
+00007bb0: 3522 290a 2020 2020 2020 2020 7365 6c66  5").        self
+00007bc0: 2e74 6578 7462 6f78 5f66 7073 5061 7468  .textbox_fpsPath
+00007bd0: 203d 2051 7457 6964 6765 7473 2e51 4c69   = QtWidgets.QLi
+00007be0: 6e65 4564 6974 2870 6172 656e 743d 7365  neEdit(parent=se
+00007bf0: 6c66 2e73 6372 6f6c 6c41 7265 6157 6964  lf.scrollAreaWid
+00007c00: 6765 7443 6f6e 7465 6e74 7329 0a20 2020  getContents).   
+00007c10: 2020 2020 2073 656c 662e 7465 7874 626f       self.textbo
+00007c20: 785f 6670 7350 6174 682e 7365 744f 626a  x_fpsPath.setObj
+00007c30: 6563 744e 616d 6528 2274 6578 7462 6f78  ectName("textbox
+00007c40: 5f66 7073 5061 7468 2229 0a20 2020 2020  _fpsPath").     
+00007c50: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
+00007c60: 7574 5f35 2e61 6464 5769 6467 6574 2873  ut_5.addWidget(s
+00007c70: 656c 662e 7465 7874 626f 785f 6670 7350  elf.textbox_fpsP
+00007c80: 6174 682c 2035 2c20 302c 2031 2c20 3329  ath, 5, 0, 1, 3)
+00007c90: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007ca0: 6e65 5f34 203d 2051 7457 6964 6765 7473  ne_4 = QtWidgets
+00007cb0: 2e51 4672 616d 6528 7061 7265 6e74 3d73  .QFrame(parent=s
+00007cc0: 656c 662e 7363 726f 6c6c 4172 6561 5769  elf.scrollAreaWi
+00007cd0: 6467 6574 436f 6e74 656e 7473 290a 2020  dgetContents).  
+00007ce0: 2020 2020 2020 7365 6c66 2e6c 696e 655f        self.line_
+00007cf0: 342e 7365 7446 7261 6d65 5368 6170 6528  4.setFrameShape(
+00007d00: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
+00007d10: 2e53 6861 7065 2e48 4c69 6e65 290a 2020  .Shape.HLine).  
+00007d20: 2020 2020 2020 7365 6c66 2e6c 696e 655f        self.line_
+00007d30: 342e 7365 7446 7261 6d65 5368 6164 6f77  4.setFrameShadow
+00007d40: 2851 7457 6964 6765 7473 2e51 4672 616d  (QtWidgets.QFram
+00007d50: 652e 5368 6164 6f77 2e53 756e 6b65 6e29  e.Shadow.Sunken)
+00007d60: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007d70: 6e65 5f34 2e73 6574 4f62 6a65 6374 4e61  ne_4.setObjectNa
+00007d80: 6d65 2822 6c69 6e65 5f34 2229 0a20 2020  me("line_4").   
+00007d90: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
+00007da0: 796f 7574 5f35 2e61 6464 5769 6467 6574  yout_5.addWidget
+00007db0: 2873 656c 662e 6c69 6e65 5f34 2c20 3132  (self.line_4, 12
+00007dc0: 2c20 302c 2031 2c20 3329 0a20 2020 2020  , 0, 1, 3).     
+00007dd0: 2020 2073 656c 662e 7465 7874 626f 785f     self.textbox_
+00007de0: 7063 6153 6176 6520 3d20 5174 5769 6467  pcaSave = QtWidg
+00007df0: 6574 732e 514c 696e 6545 6469 7428 7061  ets.QLineEdit(pa
+00007e00: 7265 6e74 3d73 656c 662e 7363 726f 6c6c  rent=self.scroll
+00007e10: 4172 6561 5769 6467 6574 436f 6e74 656e  AreaWidgetConten
+00007e20: 7473 290a 2020 2020 2020 2020 7365 6c66  ts).        self
+00007e30: 2e74 6578 7462 6f78 5f70 6361 5361 7665  .textbox_pcaSave
+00007e40: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00007e50: 7465 7874 626f 785f 7063 6153 6176 6522  textbox_pcaSave"
+00007e60: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00007e70: 7269 644c 6179 6f75 745f 352e 6164 6457  ridLayout_5.addW
+00007e80: 6964 6765 7428 7365 6c66 2e74 6578 7462  idget(self.textb
+00007e90: 6f78 5f70 6361 5361 7665 2c20 372c 2030  ox_pcaSave, 7, 0
+00007ea0: 2c20 312c 2033 290a 2020 2020 2020 2020  , 1, 3).        
+00007eb0: 7365 6c66 2e6c 6162 656c 5f31 3120 3d20  self.label_11 = 
+00007ec0: 5174 5769 6467 6574 732e 514c 6162 656c  QtWidgets.QLabel
+00007ed0: 2870 6172 656e 743d 7365 6c66 2e73 6372  (parent=self.scr
+00007ee0: 6f6c 6c41 7265 6157 6964 6765 7443 6f6e  ollAreaWidgetCon
+00007ef0: 7465 6e74 7329 0a20 2020 2020 2020 2073  tents).        s
+00007f00: 656c 662e 6c61 6265 6c5f 3131 2e73 6574  elf.label_11.set
+00007f10: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
+00007f20: 6c5f 3131 2229 0a20 2020 2020 2020 2073  l_11").        s
+00007f30: 656c 662e 6772 6964 4c61 796f 7574 5f35  elf.gridLayout_5
+00007f40: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+00007f50: 6c61 6265 6c5f 3131 2c20 322c 2030 2c20  label_11, 2, 0, 
+00007f60: 312c 2031 290a 2020 2020 2020 2020 7365  1, 1).        se
+00007f70: 6c66 2e63 6d62 5f6d 6174 7269 7850 4341  lf.cmb_matrixPCA
+00007f80: 203d 2051 7457 6964 6765 7473 2e51 436f   = QtWidgets.QCo
+00007f90: 6d62 6f42 6f78 2870 6172 656e 743d 7365  mboBox(parent=se
+00007fa0: 6c66 2e73 6372 6f6c 6c41 7265 6157 6964  lf.scrollAreaWid
+00007fb0: 6765 7443 6f6e 7465 6e74 7329 0a20 2020  getContents).   
+00007fc0: 2020 2020 2073 656c 662e 636d 625f 6d61       self.cmb_ma
+00007fd0: 7472 6978 5043 412e 7365 744f 626a 6563  trixPCA.setObjec
+00007fe0: 744e 616d 6528 2263 6d62 5f6d 6174 7269  tName("cmb_matri
+00007ff0: 7850 4341 2229 0a20 2020 2020 2020 2073  xPCA").        s
+00008000: 656c 662e 636d 625f 6d61 7472 6978 5043  elf.cmb_matrixPC
+00008010: 412e 6164 6449 7465 6d28 2222 290a 2020  A.addItem("").  
+00008020: 2020 2020 2020 7365 6c66 2e63 6d62 5f6d        self.cmb_m
+00008030: 6174 7269 7850 4341 2e61 6464 4974 656d  atrixPCA.addItem
+00008040: 2822 2229 0a20 2020 2020 2020 2073 656c  ("").        sel
+00008050: 662e 6772 6964 4c61 796f 7574 5f35 2e61  f.gridLayout_5.a
+00008060: 6464 5769 6467 6574 2873 656c 662e 636d  ddWidget(self.cm
+00008070: 625f 6d61 7472 6978 5043 412c 2032 2c20  b_matrixPCA, 2, 
+00008080: 312c 2031 2c20 3229 0a20 2020 2020 2020  1, 1, 2).       
+00008090: 2073 656c 662e 6c61 6265 6c5f 3134 203d   self.label_14 =
+000080a0: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
+000080b0: 6c28 7061 7265 6e74 3d73 656c 662e 7363  l(parent=self.sc
+000080c0: 726f 6c6c 4172 6561 5769 6467 6574 436f  rollAreaWidgetCo
+000080d0: 6e74 656e 7473 290a 2020 2020 2020 2020  ntents).        
+000080e0: 666f 6e74 203d 2051 7447 7569 2e51 466f  font = QtGui.QFo
+000080f0: 6e74 2829 0a20 2020 2020 2020 2066 6f6e  nt().        fon
+00008100: 742e 7365 7442 6f6c 6428 5472 7565 290a  t.setBold(True).
+00008110: 2020 2020 2020 2020 666f 6e74 2e73 6574          font.set
+00008120: 556e 6465 726c 696e 6528 5472 7565 290a  Underline(True).
+00008130: 2020 2020 2020 2020 666f 6e74 2e73 6574          font.set
+00008140: 5765 6967 6874 2837 3529 0a20 2020 2020  Weight(75).     
+00008150: 2020 2073 656c 662e 6c61 6265 6c5f 3134     self.label_14
+00008160: 2e73 6574 466f 6e74 2866 6f6e 7429 0a20  .setFont(font). 
+00008170: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+00008180: 6c5f 3134 2e73 6574 4f62 6a65 6374 4e61  l_14.setObjectNa
+00008190: 6d65 2822 6c61 6265 6c5f 3134 2229 0a20  me("label_14"). 
+000081a0: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
+000081b0: 4c61 796f 7574 5f35 2e61 6464 5769 6467  Layout_5.addWidg
+000081c0: 6574 2873 656c 662e 6c61 6265 6c5f 3134  et(self.label_14
+000081d0: 2c20 302c 2030 2c20 312c 2033 290a 2020  , 0, 0, 1, 3).  
+000081e0: 2020 2020 2020 7365 6c66 2e63 6d62 5f46        self.cmb_F
+000081f0: 5053 203d 2051 7457 6964 6765 7473 2e51  PS = QtWidgets.Q
+00008200: 436f 6d62 6f42 6f78 2870 6172 656e 743d  ComboBox(parent=
+00008210: 7365 6c66 2e73 6372 6f6c 6c41 7265 6157  self.scrollAreaW
+00008220: 6964 6765 7443 6f6e 7465 6e74 7329 0a20  idgetContents). 
+00008230: 2020 2020 2020 2073 656c 662e 636d 625f         self.cmb_
+00008240: 4650 532e 7365 744f 626a 6563 744e 616d  FPS.setObjectNam
+00008250: 6528 2263 6d62 5f46 5053 2229 0a20 2020  e("cmb_FPS").   
+00008260: 2020 2020 2073 656c 662e 636d 625f 4650       self.cmb_FP
+00008270: 532e 6164 6449 7465 6d28 2222 290a 2020  S.addItem("").  
+00008280: 2020 2020 2020 7365 6c66 2e63 6d62 5f46        self.cmb_F
+00008290: 5053 2e61 6464 4974 656d 2822 2229 0a20  PS.addItem(""). 
+000082a0: 2020 2020 2020 2073 656c 662e 636d 625f         self.cmb_
+000082b0: 4650 532e 6164 6449 7465 6d28 2222 290a  FPS.addItem("").
+000082c0: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
+000082d0: 644c 6179 6f75 745f 352e 6164 6457 6964  dLayout_5.addWid
+000082e0: 6765 7428 7365 6c66 2e63 6d62 5f46 5053  get(self.cmb_FPS
+000082f0: 2c20 312c 2030 2c20 312c 2033 290a 2020  , 1, 0, 1, 3).  
+00008300: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00008310: 5f31 3320 3d20 5174 5769 6467 6574 732e  _13 = QtWidgets.
+00008320: 514c 6162 656c 2870 6172 656e 743d 7365  QLabel(parent=se
+00008330: 6c66 2e73 6372 6f6c 6c41 7265 6157 6964  lf.scrollAreaWid
+00008340: 6765 7443 6f6e 7465 6e74 7329 0a20 2020  getContents).   
+00008350: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00008360: 3133 2e73 6574 4f62 6a65 6374 4e61 6d65  13.setObjectName
+00008370: 2822 6c61 6265 6c5f 3133 2229 0a20 2020  ("label_13").   
+00008380: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
+00008390: 796f 7574 5f35 2e61 6464 5769 6467 6574  yout_5.addWidget
+000083a0: 2873 656c 662e 6c61 6265 6c5f 3133 2c20  (self.label_13, 
+000083b0: 362c 2030 2c20 312c 2032 290a 2020 2020  6, 0, 1, 2).    
+000083c0: 2020 2020 7365 6c66 2e6c 696e 655f 3820      self.line_8 
+000083d0: 3d20 5174 5769 6467 6574 732e 5146 7261  = QtWidgets.QFra
+000083e0: 6d65 2870 6172 656e 743d 7365 6c66 2e73  me(parent=self.s
+000083f0: 6372 6f6c 6c41 7265 6157 6964 6765 7443  crollAreaWidgetC
+00008400: 6f6e 7465 6e74 7329 0a20 2020 2020 2020  ontents).       
+00008410: 2073 656c 662e 6c69 6e65 5f38 2e73 6574   self.line_8.set
+00008420: 4672 616d 6553 6861 7065 2851 7457 6964  FrameShape(QtWid
+00008430: 6765 7473 2e51 4672 616d 652e 5368 6170  gets.QFrame.Shap
+00008440: 652e 484c 696e 6529 0a20 2020 2020 2020  e.HLine).       
+00008450: 2073 656c 662e 6c69 6e65 5f38 2e73 6574   self.line_8.set
+00008460: 4672 616d 6553 6861 646f 7728 5174 5769  FrameShadow(QtWi
+00008470: 6467 6574 732e 5146 7261 6d65 2e53 6861  dgets.QFrame.Sha
+00008480: 646f 772e 5375 6e6b 656e 290a 2020 2020  dow.Sunken).    
+00008490: 2020 2020 7365 6c66 2e6c 696e 655f 382e      self.line_8.
+000084a0: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
+000084b0: 696e 655f 3822 290a 2020 2020 2020 2020  ine_8").        
+000084c0: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
+000084d0: 352e 6164 6457 6964 6765 7428 7365 6c66  5.addWidget(self
+000084e0: 2e6c 696e 655f 382c 2038 2c20 302c 2031  .line_8, 8, 0, 1
+000084f0: 2c20 3329 0a20 2020 2020 2020 2073 656c  , 3).        sel
+00008500: 662e 6c69 6e65 5f37 203d 2051 7457 6964  f.line_7 = QtWid
+00008510: 6765 7473 2e51 4672 616d 6528 7061 7265  gets.QFrame(pare
+00008520: 6e74 3d73 656c 662e 7363 726f 6c6c 4172  nt=self.scrollAr
+00008530: 6561 5769 6467 6574 436f 6e74 656e 7473  eaWidgetContents
+00008540: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00008550: 696e 655f 372e 7365 7446 7261 6d65 5368  ine_7.setFrameSh
+00008560: 6170 6528 5174 5769 6467 6574 732e 5146  ape(QtWidgets.QF
+00008570: 7261 6d65 2e53 6861 7065 2e48 4c69 6e65  rame.Shape.HLine
+00008580: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00008590: 696e 655f 372e 7365 7446 7261 6d65 5368  ine_7.setFrameSh
+000085a0: 6164 6f77 2851 7457 6964 6765 7473 2e51  adow(QtWidgets.Q
+000085b0: 4672 616d 652e 5368 6164 6f77 2e53 756e  Frame.Shadow.Sun
+000085c0: 6b65 6e29 0a20 2020 2020 2020 2073 656c  ken).        sel
+000085d0: 662e 6c69 6e65 5f37 2e73 6574 4f62 6a65  f.line_7.setObje
+000085e0: 6374 4e61 6d65 2822 6c69 6e65 5f37 2229  ctName("line_7")
+000085f0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00008600: 6964 4c61 796f 7574 5f35 2e61 6464 5769  idLayout_5.addWi
+00008610: 6467 6574 2873 656c 662e 6c69 6e65 5f37  dget(self.line_7
+00008620: 2c20 332c 2030 2c20 312c 2033 290a 2020  , 3, 0, 1, 3).  
+00008630: 2020 2020 2020 7365 6c66 2e62 7574 746f        self.butto
+00008640: 6e5f 4650 5370 6174 6820 3d20 5174 5769  n_FPSpath = QtWi
+00008650: 6467 6574 732e 5150 7573 6842 7574 746f  dgets.QPushButto
+00008660: 6e28 7061 7265 6e74 3d73 656c 662e 7363  n(parent=self.sc
+00008670: 726f 6c6c 4172 6561 5769 6467 6574 436f  rollAreaWidgetCo
+00008680: 6e74 656e 7473 290a 2020 2020 2020 2020  ntents).        
+00008690: 7365 6c66 2e62 7574 746f 6e5f 4650 5370  self.button_FPSp
+000086a0: 6174 682e 7365 744f 626a 6563 744e 616d  ath.setObjectNam
+000086b0: 6528 2262 7574 746f 6e5f 4650 5370 6174  e("button_FPSpat
+000086c0: 6822 290a 2020 2020 2020 2020 7365 6c66  h").        self
+000086d0: 2e67 7269 644c 6179 6f75 745f 352e 6164  .gridLayout_5.ad
+000086e0: 6457 6964 6765 7428 7365 6c66 2e62 7574  dWidget(self.but
+000086f0: 746f 6e5f 4650 5370 6174 682c 2034 2c20  ton_FPSpath, 4, 
+00008700: 322c 2031 2c20 3129 0a20 2020 2020 2020  2, 1, 1).       
+00008710: 2073 656c 662e 6c61 6265 6c5f 3132 203d   self.label_12 =
+00008720: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
+00008730: 6c28 7061 7265 6e74 3d73 656c 662e 7363  l(parent=self.sc
+00008740: 726f 6c6c 4172 6561 5769 6467 6574 436f  rollAreaWidgetCo
+00008750: 6e74 656e 7473 290a 2020 2020 2020 2020  ntents).        
+00008760: 7365 6c66 2e6c 6162 656c 5f31 322e 7365  self.label_12.se
+00008770: 744f 626a 6563 744e 616d 6528 226c 6162  tObjectName("lab
+00008780: 656c 5f31 3222 290a 2020 2020 2020 2020  el_12").        
+00008790: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
+000087a0: 352e 6164 6457 6964 6765 7428 7365 6c66  5.addWidget(self
+000087b0: 2e6c 6162 656c 5f31 322c 2034 2c20 302c  .label_12, 4, 0,
+000087c0: 2031 2c20 3229 0a20 2020 2020 2020 2073   1, 2).        s
+000087d0: 656c 662e 6275 7474 6f6e 5f73 6176 6550  elf.button_saveP
+000087e0: 4341 7061 7468 203d 2051 7457 6964 6765  CApath = QtWidge
+000087f0: 7473 2e51 5075 7368 4275 7474 6f6e 2870  ts.QPushButton(p
+00008800: 6172 656e 743d 7365 6c66 2e73 6372 6f6c  arent=self.scrol
+00008810: 6c41 7265 6157 6964 6765 7443 6f6e 7465  lAreaWidgetConte
+00008820: 6e74 7329 0a20 2020 2020 2020 2073 656c  nts).        sel
+00008830: 662e 6275 7474 6f6e 5f73 6176 6550 4341  f.button_savePCA
+00008840: 7061 7468 2e73 6574 4f62 6a65 6374 4e61  path.setObjectNa
+00008850: 6d65 2822 6275 7474 6f6e 5f73 6176 6550  me("button_saveP
+00008860: 4341 7061 7468 2229 0a20 2020 2020 2020  CApath").       
+00008870: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
+00008880: 5f35 2e61 6464 5769 6467 6574 2873 656c  _5.addWidget(sel
+00008890: 662e 6275 7474 6f6e 5f73 6176 6550 4341  f.button_savePCA
+000088a0: 7061 7468 2c20 362c 2032 2c20 312c 2031  path, 6, 2, 1, 1
+000088b0: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+000088c0: 7261 6d65 5f67 7261 7068 203d 2051 7457  rame_graph = QtW
+000088d0: 6964 6765 7473 2e51 4672 616d 6528 7061  idgets.QFrame(pa
+000088e0: 7265 6e74 3d73 656c 662e 7363 726f 6c6c  rent=self.scroll
+000088f0: 4172 6561 5769 6467 6574 436f 6e74 656e  AreaWidgetConten
+00008900: 7473 290a 2020 2020 2020 2020 7365 6c66  ts).        self
+00008910: 2e66 7261 6d65 5f67 7261 7068 2e73 6574  .frame_graph.set
+00008920: 456e 6162 6c65 6428 4661 6c73 6529 0a20  Enabled(False). 
+00008930: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
+00008940: 655f 6772 6170 682e 7365 7446 7261 6d65  e_graph.setFrame
+00008950: 5368 6170 6528 5174 5769 6467 6574 732e  Shape(QtWidgets.
+00008960: 5146 7261 6d65 2e53 6861 7065 2e53 7479  QFrame.Shape.Sty
+00008970: 6c65 6450 616e 656c 290a 2020 2020 2020  ledPanel).      
+00008980: 2020 7365 6c66 2e66 7261 6d65 5f67 7261    self.frame_gra
+00008990: 7068 2e73 6574 4672 616d 6553 6861 646f  ph.setFrameShado
+000089a0: 7728 5174 5769 6467 6574 732e 5146 7261  w(QtWidgets.QFra
+000089b0: 6d65 2e53 6861 646f 772e 5261 6973 6564  me.Shadow.Raised
+000089c0: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+000089d0: 7261 6d65 5f67 7261 7068 2e73 6574 4f62  rame_graph.setOb
+000089e0: 6a65 6374 4e61 6d65 2822 6672 616d 655f  jectName("frame_
+000089f0: 6772 6170 6822 290a 2020 2020 2020 2020  graph").        
+00008a00: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
+00008a10: 3620 3d20 5174 5769 6467 6574 732e 5147  6 = QtWidgets.QG
+00008a20: 7269 644c 6179 6f75 7428 7365 6c66 2e66  ridLayout(self.f
+00008a30: 7261 6d65 5f67 7261 7068 290a 2020 2020  rame_graph).    
+00008a40: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
+00008a50: 6f75 745f 362e 7365 744f 626a 6563 744e  out_6.setObjectN
+00008a60: 616d 6528 2267 7269 644c 6179 6f75 745f  ame("gridLayout_
+00008a70: 3622 290a 2020 2020 2020 2020 7365 6c66  6").        self
+00008a80: 2e6c 6162 656c 5f32 3820 3d20 5174 5769  .label_28 = QtWi
+00008a90: 6467 6574 732e 514c 6162 656c 2870 6172  dgets.QLabel(par
+00008aa0: 656e 743d 7365 6c66 2e66 7261 6d65 5f67  ent=self.frame_g
+00008ab0: 7261 7068 290a 2020 2020 2020 2020 7365  raph).        se
+00008ac0: 6c66 2e6c 6162 656c 5f32 382e 7365 744f  lf.label_28.setO
+00008ad0: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+00008ae0: 5f32 3822 290a 2020 2020 2020 2020 7365  _28").        se
+00008af0: 6c66 2e67 7269 644c 6179 6f75 745f 362e  lf.gridLayout_6.
+00008b00: 6164 6457 6964 6765 7428 7365 6c66 2e6c  addWidget(self.l
+00008b10: 6162 656c 5f32 382c 2031 302c 2030 2c20  abel_28, 10, 0, 
+00008b20: 312c 2031 290a 2020 2020 2020 2020 7365  1, 1).        se
+00008b30: 6c66 2e70 7573 6842 7574 746f 6e5f 3220  lf.pushButton_2 
+00008b40: 3d20 5174 5769 6467 6574 732e 5150 7573  = QtWidgets.QPus
+00008b50: 6842 7574 746f 6e28 7061 7265 6e74 3d73  hButton(parent=s
+00008b60: 656c 662e 6672 616d 655f 6772 6170 6829  elf.frame_graph)
+00008b70: 0a20 2020 2020 2020 2073 656c 662e 7075  .        self.pu
+00008b80: 7368 4275 7474 6f6e 5f32 2e73 6574 4f62  shButton_2.setOb
+00008b90: 6a65 6374 4e61 6d65 2822 7075 7368 4275  jectName("pushBu
+00008ba0: 7474 6f6e 5f32 2229 0a20 2020 2020 2020  tton_2").       
+00008bb0: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
+00008bc0: 5f36 2e61 6464 5769 6467 6574 2873 656c  _6.addWidget(sel
+00008bd0: 662e 7075 7368 4275 7474 6f6e 5f32 2c20  f.pushButton_2, 
+00008be0: 3135 2c20 302c 2031 2c20 3229 0a20 2020  15, 0, 1, 2).   
+00008bf0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00008c00: 3232 203d 2051 7457 6964 6765 7473 2e51  22 = QtWidgets.Q
+00008c10: 4c61 6265 6c28 7061 7265 6e74 3d73 656c  Label(parent=sel
+00008c20: 662e 6672 616d 655f 6772 6170 6829 0a20  f.frame_graph). 
+00008c30: 2020 2020 2020 2066 6f6e 7420 3d20 5174         font = Qt
+00008c40: 4775 692e 5146 6f6e 7428 290a 2020 2020  Gui.QFont().    
+00008c50: 2020 2020 666f 6e74 2e73 6574 426f 6c64      font.setBold
+00008c60: 2854 7275 6529 0a20 2020 2020 2020 2066  (True).        f
+00008c70: 6f6e 742e 7365 7455 6e64 6572 6c69 6e65  ont.setUnderline
+00008c80: 2854 7275 6529 0a20 2020 2020 2020 2066  (True).        f
+00008c90: 6f6e 742e 7365 7457 6569 6768 7428 3735  ont.setWeight(75
+00008ca0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00008cb0: 6162 656c 5f32 322e 7365 7446 6f6e 7428  abel_22.setFont(
+00008cc0: 666f 6e74 290a 2020 2020 2020 2020 7365  font).        se
+00008cd0: 6c66 2e6c 6162 656c 5f32 322e 7365 744f  lf.label_22.setO
+00008ce0: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+00008cf0: 5f32 3222 290a 2020 2020 2020 2020 7365  _22").        se
+00008d00: 6c66 2e67 7269 644c 6179 6f75 745f 362e  lf.gridLayout_6.
+00008d10: 6164 6457 6964 6765 7428 7365 6c66 2e6c  addWidget(self.l
+00008d20: 6162 656c 5f32 322c 2030 2c20 302c 2031  abel_22, 0, 0, 1
+00008d30: 2c20 3229 0a20 2020 2020 2020 2073 656c  , 2).        sel
+00008d40: 662e 636d 625f 7820 3d20 5174 5769 6467  f.cmb_x = QtWidg
+00008d50: 6574 732e 5143 6f6d 626f 426f 7828 7061  ets.QComboBox(pa
+00008d60: 7265 6e74 3d73 656c 662e 6672 616d 655f  rent=self.frame_
+00008d70: 6772 6170 6829 0a20 2020 2020 2020 2073  graph).        s
+00008d80: 656c 662e 636d 625f 782e 7365 744f 626a  elf.cmb_x.setObj
+00008d90: 6563 744e 616d 6528 2263 6d62 5f78 2229  ectName("cmb_x")
+00008da0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00008db0: 6964 4c61 796f 7574 5f36 2e61 6464 5769  idLayout_6.addWi
+00008dc0: 6467 6574 2873 656c 662e 636d 625f 782c  dget(self.cmb_x,
+00008dd0: 2032 2c20 312c 2031 2c20 3129 0a20 2020   2, 1, 1, 1).   
+00008de0: 2020 2020 2073 656c 662e 6473 625f 6d61       self.dsb_ma
+00008df0: 726b 6572 5369 7a65 203d 2051 7457 6964  rkerSize = QtWid
+00008e00: 6765 7473 2e51 446f 7562 6c65 5370 696e  gets.QDoubleSpin
+00008e10: 426f 7828 7061 7265 6e74 3d73 656c 662e  Box(parent=self.
+00008e20: 6672 616d 655f 6772 6170 6829 0a20 2020  frame_graph).   
+00008e30: 2020 2020 2073 656c 662e 6473 625f 6d61       self.dsb_ma
+00008e40: 726b 6572 5369 7a65 2e73 6574 4d69 6e69  rkerSize.setMini
+00008e50: 6d75 6d28 302e 3129 0a20 2020 2020 2020  mum(0.1).       
+00008e60: 2073 656c 662e 6473 625f 6d61 726b 6572   self.dsb_marker
+00008e70: 5369 7a65 2e73 6574 4d61 7869 6d75 6d28  Size.setMaximum(
+00008e80: 3330 2e30 290a 2020 2020 2020 2020 7365  30.0).        se
+00008e90: 6c66 2e64 7362 5f6d 6172 6b65 7253 697a  lf.dsb_markerSiz
+00008ea0: 652e 7365 7453 696e 676c 6553 7465 7028  e.setSingleStep(
+00008eb0: 302e 3129 0a20 2020 2020 2020 2073 656c  0.1).        sel
+00008ec0: 662e 6473 625f 6d61 726b 6572 5369 7a65  f.dsb_markerSize
+00008ed0: 2e73 6574 5072 6f70 6572 7479 2822 7661  .setProperty("va
+00008ee0: 6c75 6522 2c20 352e 3029 0a20 2020 2020  lue", 5.0).     
+00008ef0: 2020 2073 656c 662e 6473 625f 6d61 726b     self.dsb_mark
+00008f00: 6572 5369 7a65 2e73 6574 4f62 6a65 6374  erSize.setObject
+00008f10: 4e61 6d65 2822 6473 625f 6d61 726b 6572  Name("dsb_marker
+00008f20: 5369 7a65 2229 0a20 2020 2020 2020 2073  Size").        s
+00008f30: 656c 662e 6772 6964 4c61 796f 7574 5f36  elf.gridLayout_6
+00008f40: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+00008f50: 6473 625f 6d61 726b 6572 5369 7a65 2c20  dsb_markerSize, 
+00008f60: 352c 2031 2c20 312c 2031 290a 2020 2020  5, 1, 1, 1).    
+00008f70: 2020 2020 7365 6c66 2e63 6d62 5f73 6f72      self.cmb_sor
+00008f80: 7420 3d20 5174 5769 6467 6574 732e 5143  t = QtWidgets.QC
+00008f90: 6f6d 626f 426f 7828 7061 7265 6e74 3d73  omboBox(parent=s
+00008fa0: 656c 662e 6672 616d 655f 6772 6170 6829  elf.frame_graph)
+00008fb0: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
+00008fc0: 625f 736f 7274 2e73 6574 4f62 6a65 6374  b_sort.setObject
+00008fd0: 4e61 6d65 2822 636d 625f 736f 7274 2229  Name("cmb_sort")
+00008fe0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00008ff0: 6964 4c61 796f 7574 5f36 2e61 6464 5769  idLayout_6.addWi
+00009000: 6467 6574 2873 656c 662e 636d 625f 736f  dget(self.cmb_so
+00009010: 7274 2c20 392c 2031 2c20 312c 2031 290a  rt, 9, 1, 1, 1).
+00009020: 2020 2020 2020 2020 7365 6c66 2e70 7573          self.pus
+00009030: 6842 7574 746f 6e20 3d20 5174 5769 6467  hButton = QtWidg
+00009040: 6574 732e 5150 7573 6842 7574 746f 6e28  ets.QPushButton(
+00009050: 7061 7265 6e74 3d73 656c 662e 6672 616d  parent=self.fram
+00009060: 655f 6772 6170 6829 0a20 2020 2020 2020  e_graph).       
+00009070: 2073 656c 662e 7075 7368 4275 7474 6f6e   self.pushButton
+00009080: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00009090: 7075 7368 4275 7474 6f6e 2229 0a20 2020  pushButton").   
+000090a0: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
+000090b0: 796f 7574 5f36 2e61 6464 5769 6467 6574  yout_6.addWidget
+000090c0: 2873 656c 662e 7075 7368 4275 7474 6f6e  (self.pushButton
+000090d0: 2c20 3134 2c20 312c 2031 2c20 3129 0a20  , 14, 1, 1, 1). 
+000090e0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+000090f0: 6c5f 3230 203d 2051 7457 6964 6765 7473  l_20 = QtWidgets
+00009100: 2e51 4c61 6265 6c28 7061 7265 6e74 3d73  .QLabel(parent=s
+00009110: 656c 662e 6672 616d 655f 6772 6170 6829  elf.frame_graph)
+00009120: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00009130: 6265 6c5f 3230 2e73 6574 4f62 6a65 6374  bel_20.setObject
+00009140: 4e61 6d65 2822 6c61 6265 6c5f 3230 2229  Name("label_20")
+00009150: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00009160: 6964 4c61 796f 7574 5f36 2e61 6464 5769  idLayout_6.addWi
+00009170: 6467 6574 2873 656c 662e 6c61 6265 6c5f  dget(self.label_
+00009180: 3230 2c20 382c 2030 2c20 312c 2031 290a  20, 8, 0, 1, 1).
+00009190: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
+000091a0: 5f63 6f6c 6f72 203d 2051 7457 6964 6765  _color = QtWidge
+000091b0: 7473 2e51 436f 6d62 6f42 6f78 2870 6172  ts.QComboBox(par
+000091c0: 656e 743d 7365 6c66 2e66 7261 6d65 5f67  ent=self.frame_g
+000091d0: 7261 7068 290a 2020 2020 2020 2020 7365  raph).        se
+000091e0: 6c66 2e63 6d62 5f63 6f6c 6f72 2e73 6574  lf.cmb_color.set
+000091f0: 4f62 6a65 6374 4e61 6d65 2822 636d 625f  ObjectName("cmb_
+00009200: 636f 6c6f 7222 290a 2020 2020 2020 2020  color").        
+00009210: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
+00009220: 362e 6164 6457 6964 6765 7428 7365 6c66  6.addWidget(self
+00009230: 2e63 6d62 5f63 6f6c 6f72 2c20 382c 2031  .cmb_color, 8, 1
+00009240: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
+00009250: 7365 6c66 2e6c 6162 656c 5f31 3820 3d20  self.label_18 = 
+00009260: 5174 5769 6467 6574 732e 514c 6162 656c  QtWidgets.QLabel
+00009270: 2870 6172 656e 743d 7365 6c66 2e66 7261  (parent=self.fra
+00009280: 6d65 5f67 7261 7068 290a 2020 2020 2020  me_graph).      
+00009290: 2020 7365 6c66 2e6c 6162 656c 5f31 382e    self.label_18.
+000092a0: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
+000092b0: 6162 656c 5f31 3822 290a 2020 2020 2020  abel_18").      
+000092c0: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
+000092d0: 745f 362e 6164 6457 6964 6765 7428 7365  t_6.addWidget(se
+000092e0: 6c66 2e6c 6162 656c 5f31 382c 2032 2c20  lf.label_18, 2, 
+000092f0: 302c 2031 2c20 3129 0a20 2020 2020 2020  0, 1, 1).       
+00009300: 2073 656c 662e 636d 625f 7920 3d20 5174   self.cmb_y = Qt
+00009310: 5769 6467 6574 732e 5143 6f6d 626f 426f  Widgets.QComboBo
+00009320: 7828 7061 7265 6e74 3d73 656c 662e 6672  x(parent=self.fr
+00009330: 616d 655f 6772 6170 6829 0a20 2020 2020  ame_graph).     
+00009340: 2020 2073 656c 662e 636d 625f 792e 7365     self.cmb_y.se
+00009350: 744f 626a 6563 744e 616d 6528 2263 6d62  tObjectName("cmb
+00009360: 5f79 2229 0a20 2020 2020 2020 2073 656c  _y").        sel
+00009370: 662e 6772 6964 4c61 796f 7574 5f36 2e61  f.gridLayout_6.a
+00009380: 6464 5769 6467 6574 2873 656c 662e 636d  ddWidget(self.cm
+00009390: 625f 792c 2034 2c20 312c 2031 2c20 3129  b_y, 4, 1, 1, 1)
+000093a0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+000093b0: 6265 6c5f 3234 203d 2051 7457 6964 6765  bel_24 = QtWidge
+000093c0: 7473 2e51 4c61 6265 6c28 7061 7265 6e74  ts.QLabel(parent
+000093d0: 3d73 656c 662e 6672 616d 655f 6772 6170  =self.frame_grap
+000093e0: 6829 0a20 2020 2020 2020 2073 656c 662e  h).        self.
+000093f0: 6c61 6265 6c5f 3234 2e73 6574 4f62 6a65  label_24.setObje
+00009400: 6374 4e61 6d65 2822 6c61 6265 6c5f 3234  ctName("label_24
+00009410: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00009420: 6772 6964 4c61 796f 7574 5f36 2e61 6464  gridLayout_6.add
+00009430: 5769 6467 6574 2873 656c 662e 6c61 6265  Widget(self.labe
+00009440: 6c5f 3234 2c20 312c 2030 2c20 312c 2031  l_24, 1, 0, 1, 1
+00009450: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00009460: 6162 656c 5f32 3120 3d20 5174 5769 6467  abel_21 = QtWidg
+00009470: 6574 732e 514c 6162 656c 2870 6172 656e  ets.QLabel(paren
+00009480: 743d 7365 6c66 2e66 7261 6d65 5f67 7261  t=self.frame_gra
+00009490: 7068 290a 2020 2020 2020 2020 7365 6c66  ph).        self
+000094a0: 2e6c 6162 656c 5f32 312e 7365 744f 626a  .label_21.setObj
+000094b0: 6563 744e 616d 6528 226c 6162 656c 5f32  ectName("label_2
+000094c0: 3122 290a 2020 2020 2020 2020 7365 6c66  1").        self
+000094d0: 2e67 7269 644c 6179 6f75 745f 362e 6164  .gridLayout_6.ad
+000094e0: 6457 6964 6765 7428 7365 6c66 2e6c 6162  dWidget(self.lab
+000094f0: 656c 5f32 312c 2035 2c20 302c 2031 2c20  el_21, 5, 0, 1, 
+00009500: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+00009510: 636d 625f 706c 6f74 203d 2051 7457 6964  cmb_plot = QtWid
+00009520: 6765 7473 2e51 436f 6d62 6f42 6f78 2870  gets.QComboBox(p
+00009530: 6172 656e 743d 7365 6c66 2e66 7261 6d65  arent=self.frame
+00009540: 5f67 7261 7068 290a 2020 2020 2020 2020  _graph).        
+00009550: 7365 6c66 2e63 6d62 5f70 6c6f 742e 7365  self.cmb_plot.se
+00009560: 744f 626a 6563 744e 616d 6528 2263 6d62  tObjectName("cmb
+00009570: 5f70 6c6f 7422 290a 2020 2020 2020 2020  _plot").        
+00009580: 7365 6c66 2e63 6d62 5f70 6c6f 742e 6164  self.cmb_plot.ad
+00009590: 6449 7465 6d28 2222 290a 2020 2020 2020  dItem("").      
+000095a0: 2020 7365 6c66 2e63 6d62 5f70 6c6f 742e    self.cmb_plot.
+000095b0: 6164 6449 7465 6d28 2222 290a 2020 2020  addItem("").    
+000095c0: 2020 2020 7365 6c66 2e63 6d62 5f70 6c6f      self.cmb_plo
+000095d0: 742e 6164 6449 7465 6d28 2222 290a 2020  t.addItem("").  
+000095e0: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
+000095f0: 6179 6f75 745f 362e 6164 6457 6964 6765  ayout_6.addWidge
+00009600: 7428 7365 6c66 2e63 6d62 5f70 6c6f 742c  t(self.cmb_plot,
+00009610: 2031 2c20 312c 2031 2c20 3129 0a20 2020   1, 1, 1, 1).   
+00009620: 2020 2020 2073 656c 662e 636d 625f 7375       self.cmb_su
+00009630: 6273 7562 636f 6c6f 7220 3d20 5174 5769  bsubcolor = QtWi
+00009640: 6467 6574 732e 5143 6f6d 626f 426f 7828  dgets.QComboBox(
+00009650: 7061 7265 6e74 3d73 656c 662e 6672 616d  parent=self.fram
+00009660: 655f 6772 6170 6829 0a20 2020 2020 2020  e_graph).       
+00009670: 2073 656c 662e 636d 625f 7375 6273 7562   self.cmb_subsub
+00009680: 636f 6c6f 722e 7365 744f 626a 6563 744e  color.setObjectN
+00009690: 616d 6528 2263 6d62 5f73 7562 7375 6263  ame("cmb_subsubc
+000096a0: 6f6c 6f72 2229 0a20 2020 2020 2020 2073  olor").        s
+000096b0: 656c 662e 6772 6964 4c61 796f 7574 5f36  elf.gridLayout_6
+000096c0: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+000096d0: 636d 625f 7375 6273 7562 636f 6c6f 722c  cmb_subsubcolor,
+000096e0: 2031 322c 2031 2c20 312c 2031 290a 2020   12, 1, 1, 1).  
+000096f0: 2020 2020 2020 7365 6c66 2e63 6d62 5f73        self.cmb_s
+00009700: 7562 636f 6c6f 7220 3d20 5174 5769 6467  ubcolor = QtWidg
+00009710: 6574 732e 5143 6f6d 626f 426f 7828 7061  ets.QComboBox(pa
+00009720: 7265 6e74 3d73 656c 662e 6672 616d 655f  rent=self.frame_
+00009730: 6772 6170 6829 0a20 2020 2020 2020 2073  graph).        s
+00009740: 656c 662e 636d 625f 7375 6263 6f6c 6f72  elf.cmb_subcolor
+00009750: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00009760: 636d 625f 7375 6263 6f6c 6f72 2229 0a20  cmb_subcolor"). 
+00009770: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
+00009780: 4c61 796f 7574 5f36 2e61 6464 5769 6467  Layout_6.addWidg
+00009790: 6574 2873 656c 662e 636d 625f 7375 6263  et(self.cmb_subc
+000097a0: 6f6c 6f72 2c20 3130 2c20 312c 2031 2c20  olor, 10, 1, 1, 
+000097b0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+000097c0: 636d 625f 7375 6273 6f72 7420 3d20 5174  cmb_subsort = Qt
+000097d0: 5769 6467 6574 732e 5143 6f6d 626f 426f  Widgets.QComboBo
+000097e0: 7828 7061 7265 6e74 3d73 656c 662e 6672  x(parent=self.fr
+000097f0: 616d 655f 6772 6170 6829 0a20 2020 2020  ame_graph).     
+00009800: 2020 2073 656c 662e 636d 625f 7375 6273     self.cmb_subs
+00009810: 6f72 742e 7365 744f 626a 6563 744e 616d  ort.setObjectNam
+00009820: 6528 2263 6d62 5f73 7562 736f 7274 2229  e("cmb_subsort")
+00009830: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00009840: 6964 4c61 796f 7574 5f36 2e61 6464 5769  idLayout_6.addWi
+00009850: 6467 6574 2873 656c 662e 636d 625f 7375  dget(self.cmb_su
+00009860: 6273 6f72 742c 2031 312c 2031 2c20 312c  bsort, 11, 1, 1,
+00009870: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+00009880: 2e63 6d62 5f73 7562 7375 6273 6f72 7420  .cmb_subsubsort 
+00009890: 3d20 5174 5769 6467 6574 732e 5143 6f6d  = QtWidgets.QCom
+000098a0: 626f 426f 7828 7061 7265 6e74 3d73 656c  boBox(parent=sel
+000098b0: 662e 6672 616d 655f 6772 6170 6829 0a20  f.frame_graph). 
+000098c0: 2020 2020 2020 2073 656c 662e 636d 625f         self.cmb_
+000098d0: 7375 6273 7562 736f 7274 2e73 6574 4f62  subsubsort.setOb
+000098e0: 6a65 6374 4e61 6d65 2822 636d 625f 7375  jectName("cmb_su
+000098f0: 6273 7562 736f 7274 2229 0a20 2020 2020  bsubsort").     
+00009900: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
+00009910: 7574 5f36 2e61 6464 5769 6467 6574 2873  ut_6.addWidget(s
+00009920: 656c 662e 636d 625f 7375 6273 7562 736f  elf.cmb_subsubso
+00009930: 7274 2c20 3133 2c20 312c 2031 2c20 3129  rt, 13, 1, 1, 1)
+00009940: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00009950: 6265 6c5f 3239 203d 2051 7457 6964 6765  bel_29 = QtWidge
+00009960: 7473 2e51 4c61 6265 6c28 7061 7265 6e74  ts.QLabel(parent
+00009970: 3d73 656c 662e 6672 616d 655f 6772 6170  =self.frame_grap
+00009980: 6829 0a20 2020 2020 2020 2073 656c 662e  h).        self.
+00009990: 6c61 6265 6c5f 3239 2e73 6574 4f62 6a65  label_29.setObje
+000099a0: 6374 4e61 6d65 2822 6c61 6265 6c5f 3239  ctName("label_29
+000099b0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000099c0: 6772 6964 4c61 796f 7574 5f36 2e61 6464  gridLayout_6.add
+000099d0: 5769 6467 6574 2873 656c 662e 6c61 6265  Widget(self.labe
+000099e0: 6c5f 3239 2c20 3132 2c20 302c 2031 2c20  l_29, 12, 0, 1, 
+000099f0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+00009a00: 6c61 6265 6c5f 3139 203d 2051 7457 6964  label_19 = QtWid
+00009a10: 6765 7473 2e51 4c61 6265 6c28 7061 7265  gets.QLabel(pare
+00009a20: 6e74 3d73 656c 662e 6672 616d 655f 6772  nt=self.frame_gr
+00009a30: 6170 6829 0a20 2020 2020 2020 2073 656c  aph).        sel
+00009a40: 662e 6c61 6265 6c5f 3139 2e73 6574 4f62  f.label_19.setOb
+00009a50: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
+00009a60: 3139 2229 0a20 2020 2020 2020 2073 656c  19").        sel
+00009a70: 662e 6772 6964 4c61 796f 7574 5f36 2e61  f.gridLayout_6.a
+00009a80: 6464 5769 6467 6574 2873 656c 662e 6c61  ddWidget(self.la
+00009a90: 6265 6c5f 3139 2c20 342c 2030 2c20 312c  bel_19, 4, 0, 1,
+00009aa0: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+00009ab0: 2e73 7062 5f62 696e 7320 3d20 5174 5769  .spb_bins = QtWi
+00009ac0: 6467 6574 732e 5153 7069 6e42 6f78 2870  dgets.QSpinBox(p
+00009ad0: 6172 656e 743d 7365 6c66 2e66 7261 6d65  arent=self.frame
+00009ae0: 5f67 7261 7068 290a 2020 2020 2020 2020  _graph).        
+00009af0: 7365 6c66 2e73 7062 5f62 696e 732e 7365  self.spb_bins.se
+00009b00: 744d 696e 696d 756d 2831 290a 2020 2020  tMinimum(1).    
+00009b10: 2020 2020 7365 6c66 2e73 7062 5f62 696e      self.spb_bin
+00009b20: 732e 7365 744d 6178 696d 756d 2832 3030  s.setMaximum(200
+00009b30: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00009b40: 7062 5f62 696e 732e 7365 7450 726f 7065  pb_bins.setPrope
+00009b50: 7274 7928 2276 616c 7565 222c 2031 3029  rty("value", 10)
+00009b60: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
+00009b70: 625f 6269 6e73 2e73 6574 4f62 6a65 6374  b_bins.setObject
+00009b80: 4e61 6d65 2822 7370 625f 6269 6e73 2229  Name("spb_bins")
+00009b90: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00009ba0: 6964 4c61 796f 7574 5f36 2e61 6464 5769  idLayout_6.addWi
+00009bb0: 6467 6574 2873 656c 662e 7370 625f 6269  dget(self.spb_bi
+00009bc0: 6e73 2c20 362c 2031 2c20 312c 2031 290a  ns, 6, 1, 1, 1).
+00009bd0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00009be0: 656c 5f62 696e 7320 3d20 5174 5769 6467  el_bins = QtWidg
+00009bf0: 6574 732e 514c 6162 656c 2870 6172 656e  ets.QLabel(paren
+00009c00: 743d 7365 6c66 2e66 7261 6d65 5f67 7261  t=self.frame_gra
+00009c10: 7068 290a 2020 2020 2020 2020 7365 6c66  ph).        self
+00009c20: 2e6c 6162 656c 5f62 696e 732e 7365 744f  .label_bins.setO
+00009c30: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+00009c40: 5f62 696e 7322 290a 2020 2020 2020 2020  _bins").        
+00009c50: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
+00009c60: 362e 6164 6457 6964 6765 7428 7365 6c66  6.addWidget(self
+00009c70: 2e6c 6162 656c 5f62 696e 732c 2036 2c20  .label_bins, 6, 
+00009c80: 302c 2031 2c20 3129 0a20 2020 2020 2020  0, 1, 1).       
+00009c90: 2073 656c 662e 6473 625f 616c 7068 6120   self.dsb_alpha 
+00009ca0: 3d20 5174 5769 6467 6574 732e 5144 6f75  = QtWidgets.QDou
+00009cb0: 626c 6553 7069 6e42 6f78 2870 6172 656e  bleSpinBox(paren
+00009cc0: 743d 7365 6c66 2e66 7261 6d65 5f67 7261  t=self.frame_gra
+00009cd0: 7068 290a 2020 2020 2020 2020 7365 6c66  ph).        self
+00009ce0: 2e64 7362 5f61 6c70 6861 2e73 6574 4465  .dsb_alpha.setDe
+00009cf0: 6369 6d61 6c73 2831 290a 2020 2020 2020  cimals(1).      
+00009d00: 2020 7365 6c66 2e64 7362 5f61 6c70 6861    self.dsb_alpha
+00009d10: 2e73 6574 4d69 6e69 6d75 6d28 302e 3129  .setMinimum(0.1)
+00009d20: 0a20 2020 2020 2020 2073 656c 662e 6473  .        self.ds
+00009d30: 625f 616c 7068 612e 7365 744d 6178 696d  b_alpha.setMaxim
+00009d40: 756d 2831 2e30 290a 2020 2020 2020 2020  um(1.0).        
+00009d50: 7365 6c66 2e64 7362 5f61 6c70 6861 2e73  self.dsb_alpha.s
+00009d60: 6574 5369 6e67 6c65 5374 6570 2830 2e31  etSingleStep(0.1
+00009d70: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
+00009d80: 7362 5f61 6c70 6861 2e73 6574 5072 6f70  sb_alpha.setProp
+00009d90: 6572 7479 2822 7661 6c75 6522 2c20 312e  erty("value", 1.
+00009da0: 3029 0a20 2020 2020 2020 2073 656c 662e  0).        self.
+00009db0: 6473 625f 616c 7068 612e 7365 744f 626a  dsb_alpha.setObj
+00009dc0: 6563 744e 616d 6528 2264 7362 5f61 6c70  ectName("dsb_alp
+00009dd0: 6861 2229 0a20 2020 2020 2020 2073 656c  ha").        sel
+00009de0: 662e 6772 6964 4c61 796f 7574 5f36 2e61  f.gridLayout_6.a
+00009df0: 6464 5769 6467 6574 2873 656c 662e 6473  ddWidget(self.ds
+00009e00: 625f 616c 7068 612c 2037 2c20 312c 2031  b_alpha, 7, 1, 1
+00009e10: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
+00009e20: 662e 6c61 6265 6c5f 3330 203d 2051 7457  f.label_30 = QtW
+00009e30: 6964 6765 7473 2e51 4c61 6265 6c28 7061  idgets.QLabel(pa
+00009e40: 7265 6e74 3d73 656c 662e 6672 616d 655f  rent=self.frame_
+00009e50: 6772 6170 6829 0a20 2020 2020 2020 2073  graph).        s
+00009e60: 656c 662e 6c61 6265 6c5f 3330 2e73 6574  elf.label_30.set
+00009e70: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
+00009e80: 6c5f 3330 2229 0a20 2020 2020 2020 2073  l_30").        s
+00009e90: 656c 662e 6772 6964 4c61 796f 7574 5f36  elf.gridLayout_6
+00009ea0: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+00009eb0: 6c61 6265 6c5f 3330 2c20 372c 2030 2c20  label_30, 7, 0, 
+00009ec0: 312c 2031 290a 2020 2020 2020 2020 7365  1, 1).        se
+00009ed0: 6c66 2e67 7269 644c 6179 6f75 745f 352e  lf.gridLayout_5.
+00009ee0: 6164 6457 6964 6765 7428 7365 6c66 2e66  addWidget(self.f
+00009ef0: 7261 6d65 5f67 7261 7068 2c20 3133 2c20  rame_graph, 13, 
+00009f00: 302c 2031 2c20 3329 0a20 2020 2020 2020  0, 1, 3).       
+00009f10: 2073 656c 662e 6275 7474 6f6e 5f50 4341   self.button_PCA
+00009f20: 203d 2051 7457 6964 6765 7473 2e51 5075   = QtWidgets.QPu
+00009f30: 7368 4275 7474 6f6e 2870 6172 656e 743d  shButton(parent=
+00009f40: 7365 6c66 2e73 6372 6f6c 6c41 7265 6157  self.scrollAreaW
+00009f50: 6964 6765 7443 6f6e 7465 6e74 7329 0a20  idgetContents). 
+00009f60: 2020 2020 2020 2073 656c 662e 6275 7474         self.butt
+00009f70: 6f6e 5f50 4341 2e73 6574 4f62 6a65 6374  on_PCA.setObject
+00009f80: 4e61 6d65 2822 6275 7474 6f6e 5f50 4341  Name("button_PCA
+00009f90: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00009fa0: 6772 6964 4c61 796f 7574 5f35 2e61 6464  gridLayout_5.add
+00009fb0: 5769 6467 6574 2873 656c 662e 6275 7474  Widget(self.butt
+00009fc0: 6f6e 5f50 4341 2c20 392c 2030 2c20 312c  on_PCA, 9, 0, 1,
+00009fd0: 2033 290a 2020 2020 2020 2020 7365 6c66   3).        self
+00009fe0: 2e6c 6162 656c 5f31 342e 7261 6973 655f  .label_14.raise_
+00009ff0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000a000: 6c69 6e65 5f37 2e72 6169 7365 5f28 290a  line_7.raise_().
+0000a010: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+0000a020: 656c 5f31 322e 7261 6973 655f 2829 0a20  el_12.raise_(). 
+0000a030: 2020 2020 2020 2073 656c 662e 6275 7474         self.butt
+0000a040: 6f6e 5f46 5053 7061 7468 2e72 6169 7365  on_FPSpath.raise
+0000a050: 5f28 290a 2020 2020 2020 2020 7365 6c66  _().        self
+0000a060: 2e74 6578 7462 6f78 5f66 7073 5061 7468  .textbox_fpsPath
+0000a070: 2e72 6169 7365 5f28 290a 2020 2020 2020  .raise_().      
+0000a080: 2020 7365 6c66 2e6c 6162 656c 5f31 332e    self.label_13.
+0000a090: 7261 6973 655f 2829 0a20 2020 2020 2020  raise_().       
+0000a0a0: 2073 656c 662e 6275 7474 6f6e 5f73 6176   self.button_sav
+0000a0b0: 6550 4341 7061 7468 2e72 6169 7365 5f28  ePCApath.raise_(
+0000a0c0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+0000a0d0: 6578 7462 6f78 5f70 6361 5361 7665 2e72  extbox_pcaSave.r
+0000a0e0: 6169 7365 5f28 290a 2020 2020 2020 2020  aise_().        
+0000a0f0: 7365 6c66 2e6c 696e 655f 382e 7261 6973  self.line_8.rais
+0000a100: 655f 2829 0a20 2020 2020 2020 2073 656c  e_().        sel
+0000a110: 662e 6c69 6e65 5f34 2e72 6169 7365 5f28  f.line_4.raise_(
+0000a120: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+0000a130: 7261 6d65 5f67 7261 7068 2e72 6169 7365  rame_graph.raise
+0000a140: 5f28 290a 2020 2020 2020 2020 7365 6c66  _().        self
+0000a150: 2e63 6d62 5f46 5053 2e72 6169 7365 5f28  .cmb_FPS.raise_(
+0000a160: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+0000a170: 6162 656c 5f31 312e 7261 6973 655f 2829  abel_11.raise_()
+0000a180: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
+0000a190: 625f 6d61 7472 6978 5043 412e 7261 6973  b_matrixPCA.rais
+0000a1a0: 655f 2829 0a20 2020 2020 2020 2073 656c  e_().        sel
+0000a1b0: 662e 6275 7474 6f6e 5f50 4341 2e72 6169  f.button_PCA.rai
+0000a1c0: 7365 5f28 290a 2020 2020 2020 2020 7365  se_().        se
+0000a1d0: 6c66 2e73 6372 6f6c 6c41 7265 612e 7365  lf.scrollArea.se
+0000a1e0: 7457 6964 6765 7428 7365 6c66 2e73 6372  tWidget(self.scr
+0000a1f0: 6f6c 6c41 7265 6157 6964 6765 7443 6f6e  ollAreaWidgetCon
+0000a200: 7465 6e74 7329 0a20 2020 2020 2020 2073  tents).        s
+0000a210: 656c 662e 686f 7269 7a6f 6e74 616c 4c61  elf.horizontalLa
+0000a220: 796f 7574 2e61 6464 5769 6467 6574 2873  yout.addWidget(s
+0000a230: 656c 662e 7363 726f 6c6c 4172 6561 290a  elf.scrollArea).
+0000a240: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+0000a250: 5f70 6361 203d 2051 7457 6964 6765 7473  _pca = QtWidgets
+0000a260: 2e51 5461 6257 6964 6765 7428 7061 7265  .QTabWidget(pare
+0000a270: 6e74 3d73 656c 662e 7461 625f 3229 0a20  nt=self.tab_2). 
+0000a280: 2020 2020 2020 2073 656c 662e 7461 625f         self.tab_
+0000a290: 7063 612e 7365 7454 6162 506f 7369 7469  pca.setTabPositi
+0000a2a0: 6f6e 2851 7457 6964 6765 7473 2e51 5461  on(QtWidgets.QTa
+0000a2b0: 6257 6964 6765 742e 5461 6250 6f73 6974  bWidget.TabPosit
+0000a2c0: 696f 6e2e 4e6f 7274 6829 0a20 2020 2020  ion.North).     
+0000a2d0: 2020 2073 656c 662e 7461 625f 7063 612e     self.tab_pca.
+0000a2e0: 7365 7454 6162 5368 6170 6528 5174 5769  setTabShape(QtWi
+0000a2f0: 6467 6574 732e 5154 6162 5769 6467 6574  dgets.QTabWidget
+0000a300: 2e54 6162 5368 6170 652e 526f 756e 6465  .TabShape.Rounde
+0000a310: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+0000a320: 7461 625f 7063 612e 7365 744f 626a 6563  tab_pca.setObjec
+0000a330: 744e 616d 6528 2274 6162 5f70 6361 2229  tName("tab_pca")
+0000a340: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+0000a350: 625f 3420 3d20 5174 5769 6467 6574 732e  b_4 = QtWidgets.
+0000a360: 5157 6964 6765 7428 290a 2020 2020 2020  QWidget().      
+0000a370: 2020 7365 6c66 2e74 6162 5f34 2e73 6574    self.tab_4.set
+0000a380: 4f62 6a65 6374 4e61 6d65 2822 7461 625f  ObjectName("tab_
+0000a390: 3422 290a 2020 2020 2020 2020 7365 6c66  4").        self
+0000a3a0: 2e67 7269 644c 6179 6f75 745f 3132 203d  .gridLayout_12 =
+0000a3b0: 2051 7457 6964 6765 7473 2e51 4772 6964   QtWidgets.QGrid
+0000a3c0: 4c61 796f 7574 2873 656c 662e 7461 625f  Layout(self.tab_
+0000a3d0: 3429 0a20 2020 2020 2020 2073 656c 662e  4).        self.
+0000a3e0: 6772 6964 4c61 796f 7574 5f31 322e 7365  gridLayout_12.se
+0000a3f0: 744f 626a 6563 744e 616d 6528 2267 7269  tObjectName("gri
+0000a400: 644c 6179 6f75 745f 3132 2229 0a20 2020  dLayout_12").   
+0000a410: 2020 2020 2073 656c 662e 6c6f 6762 6f78       self.logbox
+0000a420: 5f70 6361 203d 2051 7457 6964 6765 7473  _pca = QtWidgets
+0000a430: 2e51 5465 7874 4564 6974 2870 6172 656e  .QTextEdit(paren
+0000a440: 743d 7365 6c66 2e74 6162 5f34 290a 2020  t=self.tab_4).  
+0000a450: 2020 2020 2020 7365 6c66 2e6c 6f67 626f        self.logbo
+0000a460: 785f 7063 612e 7365 744f 626a 6563 744e  x_pca.setObjectN
+0000a470: 616d 6528 226c 6f67 626f 785f 7063 6122  ame("logbox_pca"
+0000a480: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+0000a490: 7269 644c 6179 6f75 745f 3132 2e61 6464  ridLayout_12.add
+0000a4a0: 5769 6467 6574 2873 656c 662e 6c6f 6762  Widget(self.logb
+0000a4b0: 6f78 5f70 6361 2c20 302c 2030 2c20 312c  ox_pca, 0, 0, 1,
+0000a4c0: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+0000a4d0: 2e74 6162 5f70 6361 2e61 6464 5461 6228  .tab_pca.addTab(
+0000a4e0: 7365 6c66 2e74 6162 5f34 2c20 2222 290a  self.tab_4, "").
+0000a4f0: 2020 2020 2020 2020 7365 6c66 2e74 6e5f          self.tn_
+0000a500: 7375 6d6d 6172 7920 3d20 5174 5769 6467  summary = QtWidg
+0000a510: 6574 732e 5157 6964 6765 7428 290a 2020  ets.QWidget().  
+0000a520: 2020 2020 2020 7365 6c66 2e74 6e5f 7375        self.tn_su
+0000a530: 6d6d 6172 792e 7365 744f 626a 6563 744e  mmary.setObjectN
+0000a540: 616d 6528 2274 6e5f 7375 6d6d 6172 7922  ame("tn_summary"
+0000a550: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+0000a560: 7269 644c 6179 6f75 7420 3d20 5174 5769  ridLayout = QtWi
+0000a570: 6467 6574 732e 5147 7269 644c 6179 6f75  dgets.QGridLayou
+0000a580: 7428 7365 6c66 2e74 6e5f 7375 6d6d 6172  t(self.tn_summar
+0000a590: 7929 0a20 2020 2020 2020 2073 656c 662e  y).        self.
+0000a5a0: 6772 6964 4c61 796f 7574 2e73 6574 4f62  gridLayout.setOb
+0000a5b0: 6a65 6374 4e61 6d65 2822 6772 6964 4c61  jectName("gridLa
+0000a5c0: 796f 7574 2229 0a20 2020 2020 2020 2073  yout").        s
+0000a5d0: 656c 662e 6c61 6265 6c5f 3135 203d 2051  elf.label_15 = Q
+0000a5e0: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
+0000a5f0: 7061 7265 6e74 3d73 656c 662e 746e 5f73  parent=self.tn_s
+0000a600: 756d 6d61 7279 290a 2020 2020 2020 2020  ummary).        
+0000a610: 7365 6c66 2e6c 6162 656c 5f31 352e 7365  self.label_15.se
+0000a620: 744f 626a 6563 744e 616d 6528 226c 6162  tObjectName("lab
+0000a630: 656c 5f31 3522 290a 2020 2020 2020 2020  el_15").        
+0000a640: 7365 6c66 2e67 7269 644c 6179 6f75 742e  self.gridLayout.
+0000a650: 6164 6457 6964 6765 7428 7365 6c66 2e6c  addWidget(self.l
+0000a660: 6162 656c 5f31 352c 2030 2c20 302c 2031  abel_15, 0, 0, 1
+0000a670: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
+0000a680: 662e 7461 626c 655f 7375 6d6d 6172 7920  f.table_summary 
+0000a690: 3d20 5174 5769 6467 6574 732e 5154 6162  = QtWidgets.QTab
+0000a6a0: 6c65 5669 6577 2870 6172 656e 743d 7365  leView(parent=se
+0000a6b0: 6c66 2e74 6e5f 7375 6d6d 6172 7929 0a20  lf.tn_summary). 
+0000a6c0: 2020 2020 2020 2073 656c 662e 7461 626c         self.tabl
+0000a6d0: 655f 7375 6d6d 6172 792e 7365 744f 626a  e_summary.setObj
+0000a6e0: 6563 744e 616d 6528 2274 6162 6c65 5f73  ectName("table_s
+0000a6f0: 756d 6d61 7279 2229 0a20 2020 2020 2020  ummary").       
+0000a700: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
+0000a710: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+0000a720: 7461 626c 655f 7375 6d6d 6172 792c 2031  table_summary, 1
+0000a730: 2c20 302c 2031 2c20 3129 0a20 2020 2020  , 0, 1, 1).     
+0000a740: 2020 2073 656c 662e 6c61 6265 6c5f 3136     self.label_16
+0000a750: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
+0000a760: 6265 6c28 7061 7265 6e74 3d73 656c 662e  bel(parent=self.
+0000a770: 746e 5f73 756d 6d61 7279 290a 2020 2020  tn_summary).    
+0000a780: 2020 2020 7365 6c66 2e6c 6162 656c 5f31      self.label_1
+0000a790: 362e 7365 744f 626a 6563 744e 616d 6528  6.setObjectName(
+0000a7a0: 226c 6162 656c 5f31 3622 290a 2020 2020  "label_16").    
+0000a7b0: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
+0000a7c0: 6f75 742e 6164 6457 6964 6765 7428 7365  out.addWidget(se
+0000a7d0: 6c66 2e6c 6162 656c 5f31 362c 2032 2c20  lf.label_16, 2, 
+0000a7e0: 302c 2031 2c20 3129 0a20 2020 2020 2020  0, 1, 1).       
+0000a7f0: 2073 656c 662e 7461 626c 655f 7665 6374   self.table_vect
+0000a800: 6f72 203d 2051 7457 6964 6765 7473 2e51  or = QtWidgets.Q
+0000a810: 5461 626c 6556 6965 7728 7061 7265 6e74  TableView(parent
+0000a820: 3d73 656c 662e 746e 5f73 756d 6d61 7279  =self.tn_summary
+0000a830: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+0000a840: 6162 6c65 5f76 6563 746f 722e 7365 744f  able_vector.setO
+0000a850: 626a 6563 744e 616d 6528 2274 6162 6c65  bjectName("table
+0000a860: 5f76 6563 746f 7222 290a 2020 2020 2020  _vector").      
+0000a870: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
+0000a880: 742e 6164 6457 6964 6765 7428 7365 6c66  t.addWidget(self
+0000a890: 2e74 6162 6c65 5f76 6563 746f 722c 2033  .table_vector, 3
+0000a8a0: 2c20 302c 2031 2c20 3129 0a20 2020 2020  , 0, 1, 1).     
+0000a8b0: 2020 2073 656c 662e 7461 625f 7063 612e     self.tab_pca.
+0000a8c0: 6164 6454 6162 2873 656c 662e 746e 5f73  addTab(self.tn_s
+0000a8d0: 756d 6d61 7279 2c20 2222 290a 2020 2020  ummary, "").    
+0000a8e0: 2020 2020 7365 6c66 2e74 6e5f 6772 6170      self.tn_grap
+0000a8f0: 6820 3d20 5174 5769 6467 6574 732e 5157  h = QtWidgets.QW
+0000a900: 6964 6765 7428 290a 2020 2020 2020 2020  idget().        
+0000a910: 7365 6c66 2e74 6e5f 6772 6170 682e 7365  self.tn_graph.se
+0000a920: 744f 626a 6563 744e 616d 6528 2274 6e5f  tObjectName("tn_
+0000a930: 6772 6170 6822 290a 2020 2020 2020 2020  graph").        
+0000a940: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
+0000a950: 3131 203d 2051 7457 6964 6765 7473 2e51  11 = QtWidgets.Q
+0000a960: 4772 6964 4c61 796f 7574 2873 656c 662e  GridLayout(self.
+0000a970: 746e 5f67 7261 7068 290a 2020 2020 2020  tn_graph).      
+0000a980: 2020 7365 6c66 2e67 7269 644c 6179 6f75    self.gridLayou
+0000a990: 745f 3131 2e73 6574 4f62 6a65 6374 4e61  t_11.setObjectNa
+0000a9a0: 6d65 2822 6772 6964 4c61 796f 7574 5f31  me("gridLayout_1
+0000a9b0: 3122 290a 2020 2020 2020 2020 7365 6c66  1").        self
+0000a9c0: 2e63 616e 7661 7320 3d20 5174 5769 6467  .canvas = QtWidg
+0000a9d0: 6574 732e 5153 6372 6f6c 6c41 7265 6128  ets.QScrollArea(
+0000a9e0: 7061 7265 6e74 3d73 656c 662e 746e 5f67  parent=self.tn_g
+0000a9f0: 7261 7068 290a 2020 2020 2020 2020 7365  raph).        se
+0000aa00: 6c66 2e63 616e 7661 732e 7365 7457 6964  lf.canvas.setWid
+0000aa10: 6765 7452 6573 697a 6162 6c65 2854 7275  getResizable(Tru
+0000aa20: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+0000aa30: 6361 6e76 6173 2e73 6574 4f62 6a65 6374  canvas.setObject
+0000aa40: 4e61 6d65 2822 6361 6e76 6173 2229 0a20  Name("canvas"). 
+0000aa50: 2020 2020 2020 2073 656c 662e 7363 726f         self.scro
+0000aa60: 6c6c 4172 6561 5769 6467 6574 436f 6e74  llAreaWidgetCont
+0000aa70: 656e 7473 5f33 203d 2051 7457 6964 6765  ents_3 = QtWidge
+0000aa80: 7473 2e51 5769 6467 6574 2829 0a20 2020  ts.QWidget().   
+0000aa90: 2020 2020 2073 656c 662e 7363 726f 6c6c       self.scroll
+0000aaa0: 4172 6561 5769 6467 6574 436f 6e74 656e  AreaWidgetConten
+0000aab0: 7473 5f33 2e73 6574 4765 6f6d 6574 7279  ts_3.setGeometry
+0000aac0: 2851 7443 6f72 652e 5152 6563 7428 302c  (QtCore.QRect(0,
+0000aad0: 2030 2c20 3539 2c20 3136 2929 0a20 2020   0, 59, 16)).   
+0000aae0: 2020 2020 2073 656c 662e 7363 726f 6c6c       self.scroll
+0000aaf0: 4172 6561 5769 6467 6574 436f 6e74 656e  AreaWidgetConten
+0000ab00: 7473 5f33 2e73 6574 4f62 6a65 6374 4e61  ts_3.setObjectNa
+0000ab10: 6d65 2822 7363 726f 6c6c 4172 6561 5769  me("scrollAreaWi
+0000ab20: 6467 6574 436f 6e74 656e 7473 5f33 2229  dgetContents_3")
+0000ab30: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
+0000ab40: 6e76 6173 2e73 6574 5769 6467 6574 2873  nvas.setWidget(s
+0000ab50: 656c 662e 7363 726f 6c6c 4172 6561 5769  elf.scrollAreaWi
+0000ab60: 6467 6574 436f 6e74 656e 7473 5f33 290a  dgetContents_3).
+0000ab70: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
+0000ab80: 644c 6179 6f75 745f 3131 2e61 6464 5769  dLayout_11.addWi
+0000ab90: 6467 6574 2873 656c 662e 6361 6e76 6173  dget(self.canvas
+0000aba0: 2c20 302c 2030 2c20 312c 2031 290a 2020  , 0, 0, 1, 1).  
+0000abb0: 2020 2020 2020 7365 6c66 2e74 6162 5f70        self.tab_p
+0000abc0: 6361 2e61 6464 5461 6228 7365 6c66 2e74  ca.addTab(self.t
+0000abd0: 6e5f 6772 6170 682c 2022 2229 0a20 2020  n_graph, "").   
+0000abe0: 2020 2020 2073 656c 662e 686f 7269 7a6f       self.horizo
+0000abf0: 6e74 616c 4c61 796f 7574 2e61 6464 5769  ntalLayout.addWi
+0000ac00: 6467 6574 2873 656c 662e 7461 625f 7063  dget(self.tab_pc
+0000ac10: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
+0000ac20: 7461 6257 6964 6765 742e 6164 6454 6162  tabWidget.addTab
+0000ac30: 2873 656c 662e 7461 625f 322c 2022 2229  (self.tab_2, "")
+0000ac40: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+0000ac50: 625f 3320 3d20 5174 5769 6467 6574 732e  b_3 = QtWidgets.
+0000ac60: 5157 6964 6765 7428 290a 2020 2020 2020  QWidget().      
+0000ac70: 2020 7365 6c66 2e74 6162 5f33 2e73 6574    self.tab_3.set
+0000ac80: 4f62 6a65 6374 4e61 6d65 2822 7461 625f  ObjectName("tab_
+0000ac90: 3322 290a 2020 2020 2020 2020 7365 6c66  3").        self
+0000aca0: 2e67 7269 644c 6179 6f75 745f 3130 203d  .gridLayout_10 =
+0000acb0: 2051 7457 6964 6765 7473 2e51 4772 6964   QtWidgets.QGrid
+0000acc0: 4c61 796f 7574 2873 656c 662e 7461 625f  Layout(self.tab_
+0000acd0: 3329 0a20 2020 2020 2020 2073 656c 662e  3).        self.
+0000ace0: 6772 6964 4c61 796f 7574 5f31 302e 7365  gridLayout_10.se
+0000acf0: 744f 626a 6563 744e 616d 6528 2267 7269  tObjectName("gri
+0000ad00: 644c 6179 6f75 745f 3130 2229 0a20 2020  dLayout_10").   
+0000ad10: 2020 2020 2073 656c 662e 6672 616d 655f       self.frame_
+0000ad20: 3920 3d20 5174 5769 6467 6574 732e 5146  9 = QtWidgets.QF
+0000ad30: 7261 6d65 2870 6172 656e 743d 7365 6c66  rame(parent=self
+0000ad40: 2e74 6162 5f33 290a 2020 2020 2020 2020  .tab_3).        
+0000ad50: 7365 6c66 2e66 7261 6d65 5f39 2e73 6574  self.frame_9.set
+0000ad60: 4d61 7869 6d75 6d53 697a 6528 5174 436f  MaximumSize(QtCo
+0000ad70: 7265 2e51 5369 7a65 2831 3530 2c20 3730  re.QSize(150, 70
+0000ad80: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000ad90: 6672 616d 655f 392e 7365 7446 7261 6d65  frame_9.setFrame
+0000ada0: 5368 6170 6528 5174 5769 6467 6574 732e  Shape(QtWidgets.
+0000adb0: 5146 7261 6d65 2e53 6861 7065 2e53 7479  QFrame.Shape.Sty
+0000adc0: 6c65 6450 616e 656c 290a 2020 2020 2020  ledPanel).      
+0000add0: 2020 7365 6c66 2e66 7261 6d65 5f39 2e73    self.frame_9.s
+0000ade0: 6574 4672 616d 6553 6861 646f 7728 5174  etFrameShadow(Qt
+0000adf0: 5769 6467 6574 732e 5146 7261 6d65 2e53  Widgets.QFrame.S
+0000ae00: 6861 646f 772e 5261 6973 6564 290a 2020  hadow.Raised).  
+0000ae10: 2020 2020 2020 7365 6c66 2e66 7261 6d65        self.frame
+0000ae20: 5f39 2e73 6574 4f62 6a65 6374 4e61 6d65  _9.setObjectName
+0000ae30: 2822 6672 616d 655f 3922 290a 2020 2020  ("frame_9").    
+0000ae40: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
+0000ae50: 6f75 745f 3135 203d 2051 7457 6964 6765  out_15 = QtWidge
+0000ae60: 7473 2e51 4772 6964 4c61 796f 7574 2873  ts.QGridLayout(s
+0000ae70: 656c 662e 6672 616d 655f 3929 0a20 2020  elf.frame_9).   
+0000ae80: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
+0000ae90: 796f 7574 5f31 352e 7365 744f 626a 6563  yout_15.setObjec
+0000aea0: 744e 616d 6528 2267 7269 644c 6179 6f75  tName("gridLayou
+0000aeb0: 745f 3135 2229 0a20 2020 2020 2020 2073  t_15").        s
+0000aec0: 656c 662e 6c61 6265 6c5f 3336 203d 2051  elf.label_36 = Q
+0000aed0: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
+0000aee0: 7061 7265 6e74 3d73 656c 662e 6672 616d  parent=self.fram
+0000aef0: 655f 3929 0a20 2020 2020 2020 2066 6f6e  e_9).        fon
+0000af00: 7420 3d20 5174 4775 692e 5146 6f6e 7428  t = QtGui.QFont(
+0000af10: 290a 2020 2020 2020 2020 666f 6e74 2e73  ).        font.s
+0000af20: 6574 426f 6c64 2854 7275 6529 0a20 2020  etBold(True).   
+0000af30: 2020 2020 2066 6f6e 742e 7365 7457 6569       font.setWei
+0000af40: 6768 7428 3735 290a 2020 2020 2020 2020  ght(75).        
+0000af50: 7365 6c66 2e6c 6162 656c 5f33 362e 7365  self.label_36.se
+0000af60: 7446 6f6e 7428 666f 6e74 290a 2020 2020  tFont(font).    
+0000af70: 2020 2020 7365 6c66 2e6c 6162 656c 5f33      self.label_3
+0000af80: 362e 7365 744f 626a 6563 744e 616d 6528  6.setObjectName(
+0000af90: 226c 6162 656c 5f33 3622 290a 2020 2020  "label_36").    
+0000afa0: 2020 2020 7365 6c66 2e67 7269 644c 6179      self.gridLay
+0000afb0: 6f75 745f 3135 2e61 6464 5769 6467 6574  out_15.addWidget
+0000afc0: 2873 656c 662e 6c61 6265 6c5f 3336 2c20  (self.label_36, 
+0000afd0: 302c 2030 2c20 312c 2031 290a 2020 2020  0, 0, 1, 1).    
+0000afe0: 2020 2020 7365 6c66 2e63 6d62 5f72 6563      self.cmb_rec
+0000aff0: 5479 7065 203d 2051 7457 6964 6765 7473  Type = QtWidgets
+0000b000: 2e51 436f 6d62 6f42 6f78 2870 6172 656e  .QComboBox(paren
+0000b010: 743d 7365 6c66 2e66 7261 6d65 5f39 290a  t=self.frame_9).
+0000b020: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
+0000b030: 5f72 6563 5479 7065 2e73 6574 4f62 6a65  _recType.setObje
+0000b040: 6374 4e61 6d65 2822 636d 625f 7265 6354  ctName("cmb_recT
+0000b050: 7970 6522 290a 2020 2020 2020 2020 7365  ype").        se
+0000b060: 6c66 2e63 6d62 5f72 6563 5479 7065 2e61  lf.cmb_recType.a
+0000b070: 6464 4974 656d 2822 2229 0a20 2020 2020  ddItem("").     
+0000b080: 2020 2073 656c 662e 636d 625f 7265 6354     self.cmb_recT
+0000b090: 7970 652e 6164 6449 7465 6d28 2222 290a  ype.addItem("").
+0000b0a0: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
+0000b0b0: 644c 6179 6f75 745f 3135 2e61 6464 5769  dLayout_15.addWi
+0000b0c0: 6467 6574 2873 656c 662e 636d 625f 7265  dget(self.cmb_re
+0000b0d0: 6354 7970 652c 2031 2c20 302c 2031 2c20  cType, 1, 0, 1, 
+0000b0e0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+0000b0f0: 6772 6964 4c61 796f 7574 5f31 302e 6164  gridLayout_10.ad
+0000b100: 6457 6964 6765 7428 7365 6c66 2e66 7261  dWidget(self.fra
+0000b110: 6d65 5f39 2c20 302c 2030 2c20 312c 2031  me_9, 0, 0, 1, 1
+0000b120: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+0000b130: 675f 315f 3120 3d20 5174 5769 6467 6574  g_1_1 = QtWidget
+0000b140: 732e 5146 7261 6d65 2870 6172 656e 743d  s.QFrame(parent=
+0000b150: 7365 6c66 2e74 6162 5f33 290a 2020 2020  self.tab_3).    
+0000b160: 2020 2020 7365 6c66 2e66 675f 315f 312e      self.fg_1_1.
+0000b170: 7365 7446 7261 6d65 5368 6170 6528 5174  setFrameShape(Qt
+0000b180: 5769 6467 6574 732e 5146 7261 6d65 2e53  Widgets.QFrame.S
+0000b190: 6861 7065 2e53 7479 6c65 6450 616e 656c  hape.StyledPanel
+0000b1a0: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+0000b1b0: 675f 315f 312e 7365 7446 7261 6d65 5368  g_1_1.setFrameSh
+0000b1c0: 6164 6f77 2851 7457 6964 6765 7473 2e51  adow(QtWidgets.Q
+0000b1d0: 4672 616d 652e 5368 6164 6f77 2e52 6169  Frame.Shadow.Rai
+0000b1e0: 7365 6429 0a20 2020 2020 2020 2073 656c  sed).        sel
+0000b1f0: 662e 6667 5f31 5f31 2e73 6574 4f62 6a65  f.fg_1_1.setObje
+0000b200: 6374 4e61 6d65 2822 6667 5f31 5f31 2229  ctName("fg_1_1")
+0000b210: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+0000b220: 6964 4c61 796f 7574 5f31 302e 6164 6457  idLayout_10.addW
+0000b230: 6964 6765 7428 7365 6c66 2e66 675f 315f  idget(self.fg_1_
+0000b240: 312c 2030 2c20 312c 2032 2c20 3129 0a20  1, 0, 1, 2, 1). 
+0000b250: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
+0000b260: 655f 3220 3d20 5174 5769 6467 6574 732e  e_2 = QtWidgets.
+0000b270: 5146 7261 6d65 2870 6172 656e 743d 7365  QFrame(parent=se
+0000b280: 6c66 2e74 6162 5f33 290a 2020 2020 2020  lf.tab_3).      
+0000b290: 2020 7365 6c66 2e66 7261 6d65 5f32 2e73    self.frame_2.s
+0000b2a0: 6574 4d61 7869 6d75 6d53 697a 6528 5174  etMaximumSize(Qt
+0000b2b0: 436f 7265 2e51 5369 7a65 2831 3530 2c20  Core.QSize(150, 
+0000b2c0: 3136 3737 3732 3135 2929 0a20 2020 2020  16777215)).     
+0000b2d0: 2020 2073 656c 662e 6672 616d 655f 322e     self.frame_2.
+0000b2e0: 7365 7446 7261 6d65 5368 6170 6528 5174  setFrameShape(Qt
+0000b2f0: 5769 6467 6574 732e 5146 7261 6d65 2e53  Widgets.QFrame.S
+0000b300: 6861 7065 2e53 7479 6c65 6450 616e 656c  hape.StyledPanel
+0000b310: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+0000b320: 7261 6d65 5f32 2e73 6574 4672 616d 6553  rame_2.setFrameS
+0000b330: 6861 646f 7728 5174 5769 6467 6574 732e  hadow(QtWidgets.
+0000b340: 5146 7261 6d65 2e53 6861 646f 772e 5261  QFrame.Shadow.Ra
+0000b350: 6973 6564 290a 2020 2020 2020 2020 7365  ised).        se
+0000b360: 6c66 2e66 7261 6d65 5f32 2e73 6574 4f62  lf.frame_2.setOb
+0000b370: 6a65 6374 4e61 6d65 2822 6672 616d 655f  jectName("frame_
+0000b380: 3222 290a 2020 2020 2020 2020 7365 6c66  2").        self
+0000b390: 2e67 7269 644c 6179 6f75 745f 3820 3d20  .gridLayout_8 = 
+0000b3a0: 5174 5769 6467 6574 732e 5147 7269 644c  QtWidgets.QGridL
+0000b3b0: 6179 6f75 7428 7365 6c66 2e66 7261 6d65  ayout(self.frame
+0000b3c0: 5f32 290a 2020 2020 2020 2020 7365 6c66  _2).        self
+0000b3d0: 2e67 7269 644c 6179 6f75 745f 382e 7365  .gridLayout_8.se
+0000b3e0: 744f 626a 6563 744e 616d 6528 2267 7269  tObjectName("gri
+0000b3f0: 644c 6179 6f75 745f 3822 290a 2020 2020  dLayout_8").    
+0000b400: 2020 2020 7365 6c66 2e62 7574 746f 6e5f      self.button_
+0000b410: 7361 7665 5265 636f 6e73 7420 3d20 5174  saveReconst = Qt
+0000b420: 5769 6467 6574 732e 5150 7573 6842 7574  Widgets.QPushBut
+0000b430: 746f 6e28 7061 7265 6e74 3d73 656c 662e  ton(parent=self.
+0000b440: 6672 616d 655f 3229 0a20 2020 2020 2020  frame_2).       
+0000b450: 2073 656c 662e 6275 7474 6f6e 5f73 6176   self.button_sav
+0000b460: 6552 6563 6f6e 7374 2e73 6574 4f62 6a65  eReconst.setObje
+0000b470: 6374 4e61 6d65 2822 6275 7474 6f6e 5f73  ctName("button_s
+0000b480: 6176 6552 6563 6f6e 7374 2229 0a20 2020  aveReconst").   
+0000b490: 2020 2020 2073 656c 662e 6772 6964 4c61       self.gridLa
+0000b4a0: 796f 7574 5f38 2e61 6464 5769 6467 6574  yout_8.addWidget
+0000b4b0: 2873 656c 662e 6275 7474 6f6e 5f73 6176  (self.button_sav
+0000b4c0: 6552 6563 6f6e 7374 2c20 3130 2c20 302c  eReconst, 10, 0,
+0000b4d0: 2031 2c20 3229 0a20 2020 2020 2020 2073   1, 2).        s
+0000b4e0: 656c 662e 636d 625f 4949 4950 203d 2051  elf.cmb_IIIP = Q
+0000b4f0: 7457 6964 6765 7473 2e51 436f 6d62 6f42  tWidgets.QComboB
+0000b500: 6f78 2870 6172 656e 743d 7365 6c66 2e66  ox(parent=self.f
+0000b510: 7261 6d65 5f32 290a 2020 2020 2020 2020  rame_2).        
+0000b520: 7365 6c66 2e63 6d62 5f49 4949 502e 7365  self.cmb_IIIP.se
+0000b530: 7445 6e61 626c 6564 2846 616c 7365 290a  tEnabled(False).
+0000b540: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
+0000b550: 5f49 4949 502e 7365 744f 626a 6563 744e  _IIIP.setObjectN
+0000b560: 616d 6528 2263 6d62 5f49 4949 5022 290a  ame("cmb_IIIP").
+0000b570: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
+0000b580: 644c 6179 6f75 745f 382e 6164 6457 6964  dLayout_8.addWid
+0000b590: 6765 7428 7365 6c66 2e63 6d62 5f49 4949  get(self.cmb_III
+0000b5a0: 502c 2036 2c20 302c 2031 2c20 3129 0a20  P, 6, 0, 1, 1). 
+0000b5b0: 2020 2020 2020 2073 656c 662e 6473 625f         self.dsb_
+0000b5c0: 4949 4964 203d 2051 7457 6964 6765 7473  IIId = QtWidgets
+0000b5d0: 2e51 446f 7562 6c65 5370 696e 426f 7828  .QDoubleSpinBox(
+0000b5e0: 7061 7265 6e74 3d73 656c 662e 6672 616d  parent=self.fram
+0000b5f0: 655f 3229 0a20 2020 2020 2020 2073 656c  e_2).        sel
+0000b600: 662e 6473 625f 4949 4964 2e73 6574 456e  f.dsb_IIId.setEn
+0000b610: 6162 6c65 6428 4661 6c73 6529 0a20 2020  abled(False).   
+0000b620: 2020 2020 2073 656c 662e 6473 625f 4949       self.dsb_II
+0000b630: 4964 2e73 6574 4465 6369 6d61 6c73 2831  Id.setDecimals(1
+0000b640: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
+0000b650: 7362 5f49 4949 642e 7365 744d 696e 696d  sb_IIId.setMinim
+0000b660: 756d 282d 352e 3029 0a20 2020 2020 2020  um(-5.0).       
+0000b670: 2073 656c 662e 6473 625f 4949 4964 2e73   self.dsb_IIId.s
+0000b680: 6574 4d61 7869 6d75 6d28 352e 3029 0a20  etMaximum(5.0). 
+0000b690: 2020 2020 2020 2073 656c 662e 6473 625f         self.dsb_
+0000b6a0: 4949 4964 2e73 6574 5369 6e67 6c65 5374  IIId.setSingleSt
+0000b6b0: 6570 2830 2e31 290a 2020 2020 2020 2020  ep(0.1).        
+0000b6c0: 7365 6c66 2e64 7362 5f49 4949 642e 7365  self.dsb_IIId.se
+0000b6d0: 744f 626a 6563 744e 616d 6528 2264 7362  tObjectName("dsb
+0000b6e0: 5f49 4949 6422 290a 2020 2020 2020 2020  _IIId").        
+0000b6f0: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
+0000b700: 382e 6164 6457 6964 6765 7428 7365 6c66  8.addWidget(self
+0000b710: 2e64 7362 5f49 4949 642c 2036 2c20 312c  .dsb_IIId, 6, 1,
+0000b720: 2031 2c20 3129 0a20 2020 2020 2020 2073   1, 1).        s
+0000b730: 656c 662e 636d 625f 7375 6d44 6576 203d  elf.cmb_sumDev =
+0000b740: 2051 7457 6964 6765 7473 2e51 436f 6d62   QtWidgets.QComb
+0000b750: 6f42 6f78 2870 6172 656e 743d 7365 6c66  oBox(parent=self
+0000b760: 2e66 7261 6d65 5f32 290a 2020 2020 2020  .frame_2).      
+0000b770: 2020 7365 6c66 2e63 6d62 5f73 756d 4465    self.cmb_sumDe
+0000b780: 762e 7365 744f 626a 6563 744e 616d 6528  v.setObjectName(
+0000b790: 2263 6d62 5f73 756d 4465 7622 290a 2020  "cmb_sumDev").  
+0000b7a0: 2020 2020 2020 7365 6c66 2e63 6d62 5f73        self.cmb_s
+0000b7b0: 756d 4465 762e 6164 6449 7465 6d28 2222  umDev.addItem(""
+0000b7c0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000b7d0: 6d62 5f73 756d 4465 762e 6164 6449 7465  mb_sumDev.addIte
+0000b7e0: 6d28 2222 290a 2020 2020 2020 2020 7365  m("").        se
+0000b7f0: 6c66 2e63 6d62 5f73 756d 4465 762e 6164  lf.cmb_sumDev.ad
+0000b800: 6449 7465 6d28 2222 290a 2020 2020 2020  dItem("").      
+0000b810: 2020 7365 6c66 2e63 6d62 5f73 756d 4465    self.cmb_sumDe
+0000b820: 762e 6164 6449 7465 6d28 2222 290a 2020  v.addItem("").  
+0000b830: 2020 2020 2020 7365 6c66 2e63 6d62 5f73        self.cmb_s
+0000b840: 756d 4465 762e 6164 6449 7465 6d28 2222  umDev.addItem(""
+0000b850: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000b860: 6d62 5f73 756d 4465 762e 6164 6449 7465  mb_sumDev.addIte
+0000b870: 6d28 2222 290a 2020 2020 2020 2020 7365  m("").        se
+0000b880: 6c66 2e67 7269 644c 6179 6f75 745f 382e  lf.gridLayout_8.
+0000b890: 6164 6457 6964 6765 7428 7365 6c66 2e63  addWidget(self.c
+0000b8a0: 6d62 5f73 756d 4465 762c 2031 2c20 302c  mb_sumDev, 1, 0,
+0000b8b0: 2031 2c20 3229 0a20 2020 2020 2020 2073   1, 2).        s
+0000b8c0: 656c 662e 6275 7474 6f6e 5f67 656e 6572  elf.button_gener
+0000b8d0: 6174 6520 3d20 5174 5769 6467 6574 732e  ate = QtWidgets.
+0000b8e0: 5150 7573 6842 7574 746f 6e28 7061 7265  QPushButton(pare
+0000b8f0: 6e74 3d73 656c 662e 6672 616d 655f 3229  nt=self.frame_2)
+0000b900: 0a20 2020 2020 2020 2073 656c 662e 6275  .        self.bu
+0000b910: 7474 6f6e 5f67 656e 6572 6174 652e 7365  tton_generate.se
+0000b920: 744f 626a 6563 744e 616d 6528 2262 7574  tObjectName("but
+0000b930: 746f 6e5f 6765 6e65 7261 7465 2229 0a20  ton_generate"). 
+0000b940: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
+0000b950: 4c61 796f 7574 5f38 2e61 6464 5769 6467  Layout_8.addWidg
+0000b960: 6574 2873 656c 662e 6275 7474 6f6e 5f67  et(self.button_g
+0000b970: 656e 6572 6174 652c 2039 2c20 302c 2031  enerate, 9, 0, 1
+0000b980: 2c20 3229 0a20 2020 2020 2020 2073 656c  , 2).        sel
+0000b990: 662e 6c61 6265 6c5f 3236 203d 2051 7457  f.label_26 = QtW
+0000b9a0: 6964 6765 7473 2e51 4c61 6265 6c28 7061  idgets.QLabel(pa
+0000b9b0: 7265 6e74 3d73 656c 662e 6672 616d 655f  rent=self.frame_
+0000b9c0: 3229 0a20 2020 2020 2020 2066 6f6e 7420  2).        font 
+0000b9d0: 3d20 5174 4775 692e 5146 6f6e 7428 290a  = QtGui.QFont().
+0000b9e0: 2020 2020 2020 2020 666f 6e74 2e73 6574          font.set
+0000b9f0: 506f 696e 7453 697a 6528 3133 290a 2020  PointSize(13).  
+0000ba00: 2020 2020 2020 666f 6e74 2e73 6574 426f        font.setBo
+0000ba10: 6c64 2846 616c 7365 290a 2020 2020 2020  ld(False).      
+0000ba20: 2020 666f 6e74 2e73 6574 5765 6967 6874    font.setWeight
+0000ba30: 2835 3029 0a20 2020 2020 2020 2073 656c  (50).        sel
+0000ba40: 662e 6c61 6265 6c5f 3236 2e73 6574 466f  f.label_26.setFo
+0000ba50: 6e74 2866 6f6e 7429 0a20 2020 2020 2020  nt(font).       
+0000ba60: 2073 656c 662e 6c61 6265 6c5f 3236 2e73   self.label_26.s
+0000ba70: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
+0000ba80: 6265 6c5f 3236 2229 0a20 2020 2020 2020  bel_26").       
+0000ba90: 2073 656c 662e 6772 6964 4c61 796f 7574   self.gridLayout
+0000baa0: 5f38 2e61 6464 5769 6467 6574 2873 656c  _8.addWidget(sel
+0000bab0: 662e 6c61 6265 6c5f 3236 2c20 332c 2031  f.label_26, 3, 1
+0000bac0: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
+0000bad0: 7365 6c66 2e64 7362 5f49 6420 3d20 5174  self.dsb_Id = Qt
+0000bae0: 5769 6467 6574 732e 5144 6f75 626c 6553  Widgets.QDoubleS
+0000baf0: 7069 6e42 6f78 2870 6172 656e 743d 7365  pinBox(parent=se
+0000bb00: 6c66 2e66 7261 6d65 5f32 290a 2020 2020  lf.frame_2).    
+0000bb10: 2020 2020 7365 6c66 2e64 7362 5f49 642e      self.dsb_Id.
+0000bb20: 7365 7445 6e61 626c 6564 2846 616c 7365  setEnabled(False
+0000bb30: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
+0000bb40: 7362 5f49 642e 7365 7444 6563 696d 616c  sb_Id.setDecimal
+0000bb50: 7328 3129 0a20 2020 2020 2020 2073 656c  s(1).        sel
+0000bb60: 662e 6473 625f 4964 2e73 6574 4d69 6e69  f.dsb_Id.setMini
+0000bb70: 6d75 6d28 2d35 2e30 290a 2020 2020 2020  mum(-5.0).      
+0000bb80: 2020 7365 6c66 2e64 7362 5f49 642e 7365    self.dsb_Id.se
+0000bb90: 744d 6178 696d 756d 2835 2e30 290a 2020  tMaximum(5.0).  
+0000bba0: 2020 2020 2020 7365 6c66 2e64 7362 5f49        self.dsb_I
+0000bbb0: 642e 7365 7453 696e 676c 6553 7465 7028  d.setSingleStep(
+0000bbc0: 302e 3129 0a20 2020 2020 2020 2073 656c  0.1).        sel
+0000bbd0: 662e 6473 625f 4964 2e73 6574 4f62 6a65  f.dsb_Id.setObje
+0000bbe0: 6374 4e61 6d65 2822 6473 625f 4964 2229  ctName("dsb_Id")
+0000bbf0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+0000bc00: 6964 4c61 796f 7574 5f38 2e61 6464 5769  idLayout_8.addWi
+0000bc10: 6467 6574 2873 656c 662e 6473 625f 4964  dget(self.dsb_Id
+0000bc20: 2c20 342c 2031 2c20 312c 2031 290a 2020  , 4, 1, 1, 1).  
+0000bc30: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+0000bc40: 5f32 3720 3d20 5174 5769 6467 6574 732e  _27 = QtWidgets.
+0000bc50: 514c 6162 656c 2870 6172 656e 743d 7365  QLabel(parent=se
+0000bc60: 6c66 2e66 7261 6d65 5f32 290a 2020 2020  lf.frame_2).    
+0000bc70: 2020 2020 666f 6e74 203d 2051 7447 7569      font = QtGui
+0000bc80: 2e51 466f 6e74 2829 0a20 2020 2020 2020  .QFont().       
+0000bc90: 2066 6f6e 742e 7365 7442 6f6c 6428 5472   font.setBold(Tr
+0000bca0: 7565 290a 2020 2020 2020 2020 666f 6e74  ue).        font
+0000bcb0: 2e73 6574 5765 6967 6874 2837 3529 0a20  .setWeight(75). 
+0000bcc0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+0000bcd0: 6c5f 3237 2e73 6574 466f 6e74 2866 6f6e  l_27.setFont(fon
+0000bce0: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+0000bcf0: 6c61 6265 6c5f 3237 2e73 6574 4f62 6a65  label_27.setObje
+0000bd00: 6374 4e61 6d65 2822 6c61 6265 6c5f 3237  ctName("label_27
+0000bd10: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000bd20: 6772 6964 4c61 796f 7574 5f38 2e61 6464  gridLayout_8.add
+0000bd30: 5769 6467 6574 2873 656c 662e 6c61 6265  Widget(self.labe
+0000bd40: 6c5f 3237 2c20 322c 2030 2c20 312c 2032  l_27, 2, 0, 1, 2
+0000bd50: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+0000bd60: 6162 656c 5f32 3520 3d20 5174 5769 6467  abel_25 = QtWidg
+0000bd70: 6574 732e 514c 6162 656c 2870 6172 656e  ets.QLabel(paren
+0000bd80: 743d 7365 6c66 2e66 7261 6d65 5f32 290a  t=self.frame_2).
+0000bd90: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+0000bda0: 656c 5f32 352e 7365 744f 626a 6563 744e  el_25.setObjectN
+0000bdb0: 616d 6528 226c 6162 656c 5f32 3522 290a  ame("label_25").
+0000bdc0: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
+0000bdd0: 644c 6179 6f75 745f 382e 6164 6457 6964  dLayout_8.addWid
+0000bde0: 6765 7428 7365 6c66 2e6c 6162 656c 5f32  get(self.label_2
+0000bdf0: 352c 2033 2c20 302c 2031 2c20 3129 0a20  5, 3, 0, 1, 1). 
+0000be00: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+0000be10: 6c5f 3233 203d 2051 7457 6964 6765 7473  l_23 = QtWidgets
+0000be20: 2e51 4c61 6265 6c28 7061 7265 6e74 3d73  .QLabel(parent=s
+0000be30: 656c 662e 6672 616d 655f 3229 0a20 2020  elf.frame_2).   
+0000be40: 2020 2020 2066 6f6e 7420 3d20 5174 4775       font = QtGu
+0000be50: 692e 5146 6f6e 7428 290a 2020 2020 2020  i.QFont().      
+0000be60: 2020 666f 6e74 2e73 6574 426f 6c64 2854    font.setBold(T
+0000be70: 7275 6529 0a20 2020 2020 2020 2066 6f6e  rue).        fon
+0000be80: 742e 7365 7457 6569 6768 7428 3735 290a  t.setWeight(75).
+0000be90: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+0000bea0: 656c 5f32 332e 7365 7446 6f6e 7428 666f  el_23.setFont(fo
+0000beb0: 6e74 290a 2020 2020 2020 2020 7365 6c66  nt).        self
+0000bec0: 2e6c 6162 656c 5f32 332e 7365 744f 626a  .label_23.setObj
+0000bed0: 6563 744e 616d 6528 226c 6162 656c 5f32  ectName("label_2
+0000bee0: 3322 290a 2020 2020 2020 2020 7365 6c66  3").        self
+0000bef0: 2e67 7269 644c 6179 6f75 745f 382e 6164  .gridLayout_8.ad
+0000bf00: 6457 6964 6765 7428 7365 6c66 2e6c 6162  dWidget(self.lab
+0000bf10: 656c 5f32 332c 2030 2c20 302c 2031 2c20  el_23, 0, 0, 1, 
+0000bf20: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
+0000bf30: 6473 625f 4949 6420 3d20 5174 5769 6467  dsb_IId = QtWidg
+0000bf40: 6574 732e 5144 6f75 626c 6553 7069 6e42  ets.QDoubleSpinB
+0000bf50: 6f78 2870 6172 656e 743d 7365 6c66 2e66  ox(parent=self.f
+0000bf60: 7261 6d65 5f32 290a 2020 2020 2020 2020  rame_2).        
+0000bf70: 7365 6c66 2e64 7362 5f49 4964 2e73 6574  self.dsb_IId.set
+0000bf80: 456e 6162 6c65 6428 4661 6c73 6529 0a20  Enabled(False). 
+0000bf90: 2020 2020 2020 2073 656c 662e 6473 625f         self.dsb_
+0000bfa0: 4949 642e 7365 7444 6563 696d 616c 7328  IId.setDecimals(
+0000bfb0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+0000bfc0: 6473 625f 4949 642e 7365 744d 696e 696d  dsb_IId.setMinim
+0000bfd0: 756d 282d 352e 3029 0a20 2020 2020 2020  um(-5.0).       
+0000bfe0: 2073 656c 662e 6473 625f 4949 642e 7365   self.dsb_IId.se
+0000bff0: 744d 6178 696d 756d 2835 2e30 290a 2020  tMaximum(5.0).  
+0000c000: 2020 2020 2020 7365 6c66 2e64 7362 5f49        self.dsb_I
+0000c010: 4964 2e73 6574 5369 6e67 6c65 5374 6570  Id.setSingleStep
+0000c020: 2830 2e31 290a 2020 2020 2020 2020 7365  (0.1).        se
+0000c030: 6c66 2e64 7362 5f49 4964 2e73 6574 4f62  lf.dsb_IId.setOb
+0000c040: 6a65 6374 4e61 6d65 2822 6473 625f 4949  jectName("dsb_II
+0000c050: 6422 290a 2020 2020 2020 2020 7365 6c66  d").        self
+0000c060: 2e67 7269 644c 6179 6f75 745f 382e 6164  .gridLayout_8.ad
+0000c070: 6457 6964 6765 7428 7365 6c66 2e64 7362  dWidget(self.dsb
+0000c080: 5f49 4964 2c20 352c 2031 2c20 312c 2031  _IId, 5, 1, 1, 1
+0000c090: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000c0a0: 6d62 5f49 5020 3d20 5174 5769 6467 6574  mb_IP = QtWidget
+0000c0b0: 732e 5143 6f6d 626f 426f 7828 7061 7265  s.QComboBox(pare
+0000c0c0: 6e74 3d73 656c 662e 6672 616d 655f 3229  nt=self.frame_2)
+0000c0d0: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
+0000c0e0: 625f 4950 2e73 6574 456e 6162 6c65 6428  b_IP.setEnabled(
+0000c0f0: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
+0000c100: 656c 662e 636d 625f 4950 2e73 6574 4f62  elf.cmb_IP.setOb
+0000c110: 6a65 6374 4e61 6d65 2822 636d 625f 4950  jectName("cmb_IP
+0000c120: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000c130: 6772 6964 4c61 796f 7574 5f38 2e61 6464  gridLayout_8.add
+0000c140: 5769 6467 6574 2873 656c 662e 636d 625f  Widget(self.cmb_
+0000c150: 4950 2c20 342c 2030 2c20 312c 2031 290a  IP, 4, 0, 1, 1).
+0000c160: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
+0000c170: 5f49 4950 203d 2051 7457 6964 6765 7473  _IIP = QtWidgets
+0000c180: 2e51 436f 6d62 6f42 6f78 2870 6172 656e  .QComboBox(paren
+0000c190: 743d 7365 6c66 2e66 7261 6d65 5f32 290a  t=self.frame_2).
+0000c1a0: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
+0000c1b0: 5f49 4950 2e73 6574 456e 6162 6c65 6428  _IIP.setEnabled(
+0000c1c0: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
+0000c1d0: 656c 662e 636d 625f 4949 502e 7365 744f  elf.cmb_IIP.setO
+0000c1e0: 626a 6563 744e 616d 6528 2263 6d62 5f49  bjectName("cmb_I
+0000c1f0: 4950 2229 0a20 2020 2020 2020 2073 656c  IP").        sel
+0000c200: 662e 6772 6964 4c61 796f 7574 5f38 2e61  f.gridLayout_8.a
+0000c210: 6464 5769 6467 6574 2873 656c 662e 636d  ddWidget(self.cm
+0000c220: 625f 4949 502c 2035 2c20 302c 2031 2c20  b_IIP, 5, 0, 1, 
+0000c230: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+0000c240: 6c69 6e65 5f36 203d 2051 7457 6964 6765  line_6 = QtWidge
+0000c250: 7473 2e51 4672 616d 6528 7061 7265 6e74  ts.QFrame(parent
+0000c260: 3d73 656c 662e 6672 616d 655f 3229 0a20  =self.frame_2). 
+0000c270: 2020 2020 2020 2073 656c 662e 6c69 6e65         self.line
+0000c280: 5f36 2e73 6574 4672 616d 6553 6861 7065  _6.setFrameShape
+0000c290: 2851 7457 6964 6765 7473 2e51 4672 616d  (QtWidgets.QFram
+0000c2a0: 652e 5368 6170 652e 484c 696e 6529 0a20  e.Shape.HLine). 
+0000c2b0: 2020 2020 2020 2073 656c 662e 6c69 6e65         self.line
+0000c2c0: 5f36 2e73 6574 4672 616d 6553 6861 646f  _6.setFrameShado
+0000c2d0: 7728 5174 5769 6467 6574 732e 5146 7261  w(QtWidgets.QFra
+0000c2e0: 6d65 2e53 6861 646f 772e 5375 6e6b 656e  me.Shadow.Sunken
+0000c2f0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+0000c300: 696e 655f 362e 7365 744f 626a 6563 744e  ine_6.setObjectN
+0000c310: 616d 6528 226c 696e 655f 3622 290a 2020  ame("line_6").  
+0000c320: 2020 2020 2020 7365 6c66 2e67 7269 644c        self.gridL
+0000c330: 6179 6f75 745f 382e 6164 6457 6964 6765  ayout_8.addWidge
+0000c340: 7428 7365 6c66 2e6c 696e 655f 362c 2037  t(self.line_6, 7
+0000c350: 2c20 302c 2031 2c20 3229 0a20 2020 2020  , 0, 1, 2).     
+0000c360: 2020 2073 656c 662e 6772 6964 4c61 796f     self.gridLayo
+0000c370: 7574 5f31 302e 6164 6457 6964 6765 7428  ut_10.addWidget(
+0000c380: 7365 6c66 2e66 7261 6d65 5f32 2c20 312c  self.frame_2, 1,
+0000c390: 2030 2c20 312c 2031 290a 2020 2020 2020   0, 1, 1).      
+0000c3a0: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
+0000c3b0: 2e61 6464 5461 6228 7365 6c66 2e74 6162  .addTab(self.tab
+0000c3c0: 5f33 2c20 2222 290a 2020 2020 2020 2020  _3, "").        
+0000c3d0: 7365 6c66 2e67 7269 644c 6179 6f75 745f  self.gridLayout_
+0000c3e0: 372e 6164 6457 6964 6765 7428 7365 6c66  7.addWidget(self
+0000c3f0: 2e74 6162 5769 6467 6574 2c20 302c 2031  .tabWidget, 0, 1
+0000c400: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
+0000c410: 4d61 696e 5769 6e64 6f77 2e73 6574 4365  MainWindow.setCe
+0000c420: 6e74 7261 6c57 6964 6765 7428 7365 6c66  ntralWidget(self
+0000c430: 2e63 656e 7472 616c 7769 6467 6574 290a  .centralwidget).
+0000c440: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
+0000c450: 7562 6172 203d 2051 7457 6964 6765 7473  ubar = QtWidgets
+0000c460: 2e51 4d65 6e75 4261 7228 7061 7265 6e74  .QMenuBar(parent
+0000c470: 3d4d 6169 6e57 696e 646f 7729 0a20 2020  =MainWindow).   
+0000c480: 2020 2020 2073 656c 662e 6d65 6e75 6261       self.menuba
+0000c490: 722e 7365 7447 656f 6d65 7472 7928 5174  r.setGeometry(Qt
+0000c4a0: 436f 7265 2e51 5265 6374 2830 2c20 302c  Core.QRect(0, 0,
+0000c4b0: 2031 3039 342c 2032 3729 290a 2020 2020   1094, 27)).    
+0000c4c0: 2020 2020 7365 6c66 2e6d 656e 7562 6172      self.menubar
+0000c4d0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+0000c4e0: 6d65 6e75 6261 7222 290a 2020 2020 2020  menubar").      
+0000c4f0: 2020 7365 6c66 2e6d 656e 7574 6573 7420    self.menutest 
+0000c500: 3d20 5174 5769 6467 6574 732e 514d 656e  = QtWidgets.QMen
+0000c510: 7528 7061 7265 6e74 3d73 656c 662e 6d65  u(parent=self.me
+0000c520: 6e75 6261 7229 0a20 2020 2020 2020 2073  nubar).        s
+0000c530: 656c 662e 6d65 6e75 7465 7374 2e73 6574  elf.menutest.set
+0000c540: 4f62 6a65 6374 4e61 6d65 2822 6d65 6e75  ObjectName("menu
+0000c550: 7465 7374 2229 0a20 2020 2020 2020 204d  test").        M
+0000c560: 6169 6e57 696e 646f 772e 7365 744d 656e  ainWindow.setMen
+0000c570: 7542 6172 2873 656c 662e 6d65 6e75 6261  uBar(self.menuba
+0000c580: 7229 0a20 2020 2020 2020 2073 656c 662e  r).        self.
+0000c590: 7374 6174 7573 6261 7220 3d20 5174 5769  statusbar = QtWi
+0000c5a0: 6467 6574 732e 5153 7461 7475 7342 6172  dgets.QStatusBar
+0000c5b0: 2870 6172 656e 743d 4d61 696e 5769 6e64  (parent=MainWind
+0000c5c0: 6f77 290a 2020 2020 2020 2020 7365 6c66  ow).        self
+0000c5d0: 2e73 7461 7475 7362 6172 2e73 6574 4f62  .statusbar.setOb
+0000c5e0: 6a65 6374 4e61 6d65 2822 7374 6174 7573  jectName("status
+0000c5f0: 6261 7222 290a 2020 2020 2020 2020 4d61  bar").        Ma
+0000c600: 696e 5769 6e64 6f77 2e73 6574 5374 6174  inWindow.setStat
+0000c610: 7573 4261 7228 7365 6c66 2e73 7461 7475  usBar(self.statu
+0000c620: 7362 6172 290a 2020 2020 2020 2020 7365  sbar).        se
+0000c630: 6c66 2e61 6374 696f 6e41 626f 7574 203d  lf.actionAbout =
+0000c640: 2051 7447 7569 2e51 4163 7469 6f6e 2870   QtGui.QAction(p
+0000c650: 6172 656e 743d 4d61 696e 5769 6e64 6f77  arent=MainWindow
+0000c660: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000c670: 6374 696f 6e41 626f 7574 2e73 6574 4f62  ctionAbout.setOb
+0000c680: 6a65 6374 4e61 6d65 2822 6163 7469 6f6e  jectName("action
+0000c690: 4162 6f75 7422 290a 2020 2020 2020 2020  About").        
+0000c6a0: 7365 6c66 2e6d 656e 7574 6573 742e 6164  self.menutest.ad
+0000c6b0: 6441 6374 696f 6e28 7365 6c66 2e61 6374  dAction(self.act
+0000c6c0: 696f 6e41 626f 7574 290a 2020 2020 2020  ionAbout).      
+0000c6d0: 2020 7365 6c66 2e6d 656e 7562 6172 2e61    self.menubar.a
+0000c6e0: 6464 4163 7469 6f6e 2873 656c 662e 6d65  ddAction(self.me
+0000c6f0: 6e75 7465 7374 2e6d 656e 7541 6374 696f  nutest.menuActio
+0000c700: 6e28 2929 0a0a 2020 2020 2020 2020 7365  n())..        se
+0000c710: 6c66 2e72 6574 7261 6e73 6c61 7465 5569  lf.retranslateUi
+0000c720: 284d 6169 6e57 696e 646f 7729 0a20 2020  (MainWindow).   
+0000c730: 2020 2020 2073 656c 662e 7461 6257 6964       self.tabWid
+0000c740: 6765 742e 7365 7443 7572 7265 6e74 496e  get.setCurrentIn
+0000c750: 6465 7828 3029 0a20 2020 2020 2020 2073  dex(0).        s
+0000c760: 656c 662e 7461 6257 6964 6765 745f 322e  elf.tabWidget_2.
+0000c770: 7365 7443 7572 7265 6e74 496e 6465 7828  setCurrentIndex(
+0000c780: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+0000c790: 7461 625f 7063 612e 7365 7443 7572 7265  tab_pca.setCurre
+0000c7a0: 6e74 496e 6465 7828 3029 0a20 2020 2020  ntIndex(0).     
+0000c7b0: 2020 2051 7443 6f72 652e 514d 6574 614f     QtCore.QMetaO
+0000c7c0: 626a 6563 742e 636f 6e6e 6563 7453 6c6f  bject.connectSlo
+0000c7d0: 7473 4279 4e61 6d65 284d 6169 6e57 696e  tsByName(MainWin
+0000c7e0: 646f 7729 0a0a 2020 2020 6465 6620 7265  dow)..    def re
+0000c7f0: 7472 616e 736c 6174 6555 6928 7365 6c66  translateUi(self
+0000c800: 2c20 4d61 696e 5769 6e64 6f77 293a 0a20  , MainWindow):. 
+0000c810: 2020 2020 2020 205f 7472 616e 736c 6174         _translat
+0000c820: 6520 3d20 5174 436f 7265 2e51 436f 7265  e = QtCore.QCore
+0000c830: 4170 706c 6963 6174 696f 6e2e 7472 616e  Application.tran
+0000c840: 736c 6174 650a 2020 2020 2020 2020 4d61  slate.        Ma
+0000c850: 696e 5769 6e64 6f77 2e73 6574 5769 6e64  inWindow.setWind
+0000c860: 6f77 5469 746c 6528 5f74 7261 6e73 6c61  owTitle(_transla
+0000c870: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+0000c880: 2022 4d61 696e 5769 6e64 6f77 2229 290a   "MainWindow")).
+0000c890: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+0000c8a0: 656c 5f33 372e 7365 7454 6578 7428 5f74  el_37.setText(_t
+0000c8b0: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+0000c8c0: 6e64 6f77 222c 2022 5365 6c65 6374 6564  ndow", "Selected
+0000c8d0: 2053 616d 706c 6522 2929 0a20 2020 2020   Sample")).     
+0000c8e0: 2020 2073 656c 662e 6c61 6265 6c5f 3335     self.label_35
+0000c8f0: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+0000c900: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+0000c910: 2c20 2253 656c 6563 7465 6420 496d 6167  , "Selected Imag
+0000c920: 6522 2929 0a20 2020 2020 2020 2073 656c  e")).        sel
+0000c930: 662e 7461 6257 6964 6765 745f 322e 7365  f.tabWidget_2.se
+0000c940: 7454 6162 5465 7874 2873 656c 662e 7461  tTabText(self.ta
+0000c950: 6257 6964 6765 745f 322e 696e 6465 784f  bWidget_2.indexO
+0000c960: 6628 7365 6c66 2e74 6162 5f36 292c 205f  f(self.tab_6), _
+0000c970: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+0000c980: 696e 646f 7722 2c20 224f 7269 6769 6e61  indow", "Origina
+0000c990: 6c22 2929 0a20 2020 2020 2020 2073 656c  l")).        sel
+0000c9a0: 662e 6c61 6265 6c5f 3432 2e73 6574 5465  f.label_42.setTe
+0000c9b0: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
+0000c9c0: 6169 6e57 696e 646f 7722 2c20 2259 2229  ainWindow", "Y")
+0000c9d0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+0000c9e0: 6162 656c 5f34 352e 7365 7454 6578 7428  abel_45.setText(
+0000c9f0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+0000ca00: 5769 6e64 6f77 222c 2022 5822 2929 0a20  Window", "X")). 
+0000ca10: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
+0000ca20: 6964 6765 745f 322e 7365 7454 6162 5465  idget_2.setTabTe
+0000ca30: 7874 2873 656c 662e 7461 6257 6964 6765  xt(self.tabWidge
+0000ca40: 745f 322e 696e 6465 784f 6628 7365 6c66  t_2.indexOf(self
+0000ca50: 2e74 6162 5f39 292c 205f 7472 616e 736c  .tab_9), _transl
+0000ca60: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+0000ca70: 2c20 2250 726f 6a65 6374 696f 6e22 2929  , "Projection"))
+0000ca80: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+0000ca90: 6265 6c5f 3431 2e73 6574 5465 7874 285f  bel_41.setText(_
+0000caa0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+0000cab0: 696e 646f 7722 2c20 2259 2043 6f6f 7264  indow", "Y Coord
+0000cac0: 696e 6174 6522 2929 0a20 2020 2020 2020  inate")).       
+0000cad0: 2073 656c 662e 6c61 6265 6c5f 3430 2e73   self.label_40.s
+0000cae0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
+0000caf0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+0000cb00: 2258 2043 6f6f 7264 696e 6174 6522 2929  "X Coordinate"))
+0000cb10: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+0000cb20: 6257 6964 6765 745f 322e 7365 7454 6162  bWidget_2.setTab
+0000cb30: 5465 7874 2873 656c 662e 7461 6257 6964  Text(self.tabWid
+0000cb40: 6765 745f 322e 696e 6465 784f 6628 7365  get_2.indexOf(se
+0000cb50: 6c66 2e74 6162 5f37 292c 205f 7472 616e  lf.tab_7), _tran
+0000cb60: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+0000cb70: 7722 2c20 2246 6f75 7269 6572 2041 7070  w", "Fourier App
+0000cb80: 726f 7869 6d61 7469 6f6e 2229 290a 2020  roximation")).  
+0000cb90: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+0000cba0: 5f34 342e 7365 7454 6578 7428 5f74 7261  _44.setText(_tra
+0000cbb0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+0000cbc0: 6f77 222c 2022 436f 6d70 6572 6973 6f6e  ow", "Comperison
+0000cbd0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000cbe0: 2e6c 6162 656c 5f34 332e 7365 7454 6578  .label_43.setTex
+0000cbf0: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+0000cc00: 696e 5769 6e64 6f77 222c 2022 5265 636f  inWindow", "Reco
+0000cc10: 6e73 7472 7563 7465 6420 2845 4641 2922  nstructed (EFA)"
+0000cc20: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000cc30: 7461 6257 6964 6765 745f 322e 7365 7454  tabWidget_2.setT
+0000cc40: 6162 5465 7874 2873 656c 662e 7461 6257  abText(self.tabW
+0000cc50: 6964 6765 745f 322e 696e 6465 784f 6628  idget_2.indexOf(
+0000cc60: 7365 6c66 2e74 6162 5f38 292c 205f 7472  self.tab_8), _tr
+0000cc70: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+0000cc80: 646f 7722 2c20 2252 6563 6f6e 7374 7275  dow", "Reconstru
+0000cc90: 6374 2229 290a 2020 2020 2020 2020 7365  ct")).        se
+0000cca0: 6c66 2e63 625f 4247 435f 7361 6d70 6c65  lf.cb_BGC_sample
+0000ccb0: 2e73 6574 4974 656d 5465 7874 2830 2c20  .setItemText(0, 
+0000ccc0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+0000ccd0: 5769 6e64 6f77 222c 2022 5768 6974 6522  Window", "White"
+0000cce0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000ccf0: 6362 5f42 4743 5f73 616d 706c 652e 7365  cb_BGC_sample.se
+0000cd00: 7449 7465 6d54 6578 7428 312c 205f 7472  tItemText(1, _tr
+0000cd10: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+0000cd20: 646f 7722 2c20 2242 6c61 636b 2229 290a  dow", "Black")).
+0000cd30: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+0000cd40: 656c 5f33 392e 7365 7454 6578 7428 5f74  el_39.setText(_t
+0000cd50: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+0000cd60: 6e64 6f77 222c 2022 4261 636b 6772 6f75  ndow", "Backgrou
+0000cd70: 6e64 2043 6f6c 6f72 206f 6620 496d 6167  nd Color of Imag
+0000cd80: 6522 2929 0a20 2020 2020 2020 2073 656c  e")).        sel
+0000cd90: 662e 6c61 6265 6c5f 3334 2e73 6574 5465  f.label_34.setTe
+0000cda0: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
+0000cdb0: 6169 6e57 696e 646f 7722 2c20 2253 656c  ainWindow", "Sel
+0000cdc0: 6563 7420 5361 6d70 6c65 206e 756d 6265  ect Sample numbe
+0000cdd0: 7222 2929 0a20 2020 2020 2020 2073 656c  r")).        sel
+0000cde0: 662e 6c61 6265 6c5f 3333 2e73 6574 5465  f.label_33.setTe
+0000cdf0: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
+0000ce00: 6169 6e57 696e 646f 7722 2c20 2253 656c  ainWindow", "Sel
+0000ce10: 6563 7420 496d 6167 6522 2929 0a20 2020  ect Image")).   
+0000ce20: 2020 2020 2073 656c 662e 6275 7474 6f6e       self.button
+0000ce30: 5f73 616d 706c 652e 7365 7454 6578 7428  _sample.setText(
+0000ce40: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+0000ce50: 5769 6e64 6f77 222c 2022 4368 6f6f 7365  Window", "Choose
+0000ce60: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000ce70: 2e6c 6162 656c 5f33 382e 7365 7454 6578  .label_38.setTex
+0000ce80: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+0000ce90: 696e 5769 6e64 6f77 222c 2022 4d61 7869  inWindow", "Maxi
+0000cea0: 6d75 6d20 4861 726d 6f6e 6963 7320 4e75  mum Harmonics Nu
+0000ceb0: 6d62 6572 2229 290a 2020 2020 2020 2020  mber")).        
+0000cec0: 7365 6c66 2e62 7574 746f 6e5f 7374 6172  self.button_star
+0000ced0: 7473 616d 706c 652e 7365 7454 6578 7428  tsample.setText(
+0000cee0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+0000cef0: 5769 6e64 6f77 222c 2022 5374 6172 7421  Window", "Start!
+0000cf00: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000cf10: 2e62 7574 746f 6e5f 7361 7665 5f73 616d  .button_save_sam
+0000cf20: 706c 652e 7365 7454 6578 7428 5f74 7261  ple.setText(_tra
+0000cf30: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+0000cf40: 6f77 222c 2022 5361 7665 2229 290a 2020  ow", "Save")).  
+0000cf50: 2020 2020 2020 7365 6c66 2e74 6162 5769        self.tabWi
+0000cf60: 6467 6574 2e73 6574 5461 6254 6578 7428  dget.setTabText(
+0000cf70: 7365 6c66 2e74 6162 5769 6467 6574 2e69  self.tabWidget.i
+0000cf80: 6e64 6578 4f66 2873 656c 662e 7461 625f  ndexOf(self.tab_
+0000cf90: 3529 2c20 5f74 7261 6e73 6c61 7465 2822  5), _translate("
+0000cfa0: 4d61 696e 5769 6e64 6f77 222c 2022 506c  MainWindow", "Pl
+0000cfb0: 6179 6772 6f75 6e64 2229 290a 2020 2020  ayground")).    
+0000cfc0: 2020 2020 7365 6c66 2e6c 6162 656c 5f33      self.label_3
+0000cfd0: 312e 7365 7454 6578 7428 5f74 7261 6e73  1.setText(_trans
+0000cfe0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+0000cff0: 222c 2022 4e4f 5445 3a20 4974 206d 6179  ", "NOTE: It may
+0000d000: 2074 616b 6520 6120 6c6f 6e67 2074 696d   take a long tim
+0000d010: 6522 2929 0a20 2020 2020 2020 2073 656c  e")).        sel
+0000d020: 662e 636d 625f 666f 726d 6174 2e73 6574  f.cmb_format.set
+0000d030: 4974 656d 5465 7874 2830 2c20 5f74 7261  ItemText(0, _tra
+0000d040: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+0000d050: 6f77 222c 2022 2e70 6e67 2229 290a 2020  ow", ".png")).  
+0000d060: 2020 2020 2020 7365 6c66 2e63 6d62 5f66        self.cmb_f
+0000d070: 6f72 6d61 742e 7365 7449 7465 6d54 6578  ormat.setItemTex
+0000d080: 7428 312c 205f 7472 616e 736c 6174 6528  t(1, _translate(
+0000d090: 224d 6169 6e57 696e 646f 7722 2c20 222e  "MainWindow", ".
+0000d0a0: 424d 5022 2929 0a20 2020 2020 2020 2073  BMP")).        s
+0000d0b0: 656c 662e 636d 625f 666f 726d 6174 2e73  elf.cmb_format.s
+0000d0c0: 6574 4974 656d 5465 7874 2832 2c20 5f74  etItemText(2, _t
+0000d0d0: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+0000d0e0: 6e64 6f77 222c 2022 2e6a 7065 6722 2929  ndow", ".jpeg"))
+0000d0f0: 0a20 2020 2020 2020 2073 656c 662e 636d  .        self.cm
+0000d100: 625f 666f 726d 6174 2e73 6574 4974 656d  b_format.setItem
+0000d110: 5465 7874 2833 2c20 5f74 7261 6e73 6c61  Text(3, _transla
+0000d120: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+0000d130: 2022 2e6a 7067 2229 290a 2020 2020 2020   ".jpg")).      
+0000d140: 2020 7365 6c66 2e63 6d62 5f73 6361 6c65    self.cmb_scale
+0000d150: 5479 7065 2e73 6574 4974 656d 5465 7874  Type.setItemText
+0000d160: 2830 2c20 5f74 7261 6e73 6c61 7465 2822  (0, _translate("
+0000d170: 4d61 696e 5769 6e64 6f77 222c 2022 4e6f  MainWindow", "No
+0000d180: 2073 6361 6c65 2229 290a 2020 2020 2020   scale")).      
+0000d190: 2020 7365 6c66 2e63 6d62 5f73 6361 6c65    self.cmb_scale
+0000d1a0: 5479 7065 2e73 6574 4974 656d 5465 7874  Type.setItemText
+0000d1b0: 2831 2c20 5f74 7261 6e73 6c61 7465 2822  (1, _translate("
+0000d1c0: 4d61 696e 5769 6e64 6f77 222c 2022 322d  MainWindow", "2-
+0000d1d0: 4420 2841 7265 6129 2229 290a 2020 2020  D (Area)")).    
+0000d1e0: 2020 2020 7365 6c66 2e63 6d62 5f73 6361      self.cmb_sca
+0000d1f0: 6c65 5479 7065 2e73 6574 4974 656d 5465  leType.setItemTe
+0000d200: 7874 2832 2c20 5f74 7261 6e73 6c61 7465  xt(2, _translate
+0000d210: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+0000d220: 312d 4420 2858 2d4c 656e 6774 6829 2229  1-D (X-Length)")
+0000d230: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000d240: 6d62 5f73 6361 6c65 5479 7065 2e73 6574  mb_scaleType.set
+0000d250: 4974 656d 5465 7874 2833 2c20 5f74 7261  ItemText(3, _tra
+0000d260: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+0000d270: 6f77 222c 2022 312d 4420 2859 2d4c 656e  ow", "1-D (Y-Len
+0000d280: 6774 6829 2229 290a 2020 2020 2020 2020  gth)")).        
+0000d290: 7365 6c66 2e6c 6162 656c 2e73 6574 5465  self.label.setTe
+0000d2a0: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
+0000d2b0: 6169 6e57 696e 646f 7722 2c20 2233 2e20  ainWindow", "3. 
+0000d2c0: 496d 6167 6520 666f 726d 6174 2229 290a  Image format")).
+0000d2d0: 2020 2020 2020 2020 7365 6c66 2e62 7574          self.but
+0000d2e0: 746f 6e5f 666f 6c64 612e 7365 7454 6578  ton_folda.setTex
+0000d2f0: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+0000d300: 696e 5769 6e64 6f77 222c 2022 5365 6c65  inWindow", "Sele
+0000d310: 6374 2229 290a 2020 2020 2020 2020 7365  ct")).        se
+0000d320: 6c66 2e63 6d62 5f73 616d 706c 6554 7970  lf.cmb_sampleTyp
+0000d330: 652e 7365 7449 7465 6d54 6578 7428 302c  e.setItemText(0,
+0000d340: 205f 7472 616e 736c 6174 6528 224d 6169   _translate("Mai
+0000d350: 6e57 696e 646f 7722 2c20 2257 6869 7465  nWindow", "White
+0000d360: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000d370: 2e63 6d62 5f73 616d 706c 6554 7970 652e  .cmb_sampleType.
+0000d380: 7365 7449 7465 6d54 6578 7428 312c 205f  setItemText(1, _
+0000d390: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+0000d3a0: 696e 646f 7722 2c20 2242 6c61 636b 2229  indow", "Black")
+0000d3b0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+0000d3c0: 6162 656c 5f39 2e73 6574 5465 7874 285f  abel_9.setText(_
+0000d3d0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+0000d3e0: 696e 646f 7722 2c20 2253 6361 6c65 2055  indow", "Scale U
+0000d3f0: 6e69 7422 2929 0a20 2020 2020 2020 2073  nit")).        s
+0000d400: 656c 662e 6c61 6265 6c5f 382e 7365 7454  elf.label_8.setT
+0000d410: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+0000d420: 4d61 696e 5769 6e64 6f77 222c 2022 5363  MainWindow", "Sc
+0000d430: 616c 6520 5369 7a65 2229 290a 2020 2020  ale Size")).    
+0000d440: 2020 2020 7365 6c66 2e6c 6162 656c 5f31      self.label_1
+0000d450: 302e 7365 7454 6578 7428 5f74 7261 6e73  0.setText(_trans
+0000d460: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+0000d470: 222c 2022 506f 7369 7469 6f6e 2229 290a  ", "Position")).
+0000d480: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
+0000d490: 5f73 6361 6c65 506f 732e 7365 7449 7465  _scalePos.setIte
+0000d4a0: 6d54 6578 7428 302c 205f 7472 616e 736c  mText(0, _transl
+0000d4b0: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+0000d4c0: 2c20 2254 6f70 2229 290a 2020 2020 2020  , "Top")).      
+0000d4d0: 2020 7365 6c66 2e63 6d62 5f73 6361 6c65    self.cmb_scale
+0000d4e0: 506f 732e 7365 7449 7465 6d54 6578 7428  Pos.setItemText(
+0000d4f0: 312c 205f 7472 616e 736c 6174 6528 224d  1, _translate("M
+0000d500: 6169 6e57 696e 646f 7722 2c20 2242 6f74  ainWindow", "Bot
+0000d510: 746f 6d22 2929 0a20 2020 2020 2020 2073  tom")).        s
+0000d520: 656c 662e 636d 625f 7363 616c 6550 6f73  elf.cmb_scalePos
+0000d530: 2e73 6574 4974 656d 5465 7874 2832 2c20  .setItemText(2, 
+0000d540: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+0000d550: 5769 6e64 6f77 222c 2022 5269 6768 7422  Window", "Right"
+0000d560: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000d570: 636d 625f 7363 616c 6550 6f73 2e73 6574  cmb_scalePos.set
+0000d580: 4974 656d 5465 7874 2833 2c20 5f74 7261  ItemText(3, _tra
+0000d590: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+0000d5a0: 6f77 222c 2022 4c65 6674 2229 290a 2020  ow", "Left")).  
+0000d5b0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+0000d5c0: 5f34 2e73 6574 5465 7874 285f 7472 616e  _4.setText(_tran
+0000d5d0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+0000d5e0: 7722 2c20 224d 6178 696d 756d 2048 6172  w", "Maximum Har
+0000d5f0: 6d6f 6e69 6373 2229 290a 2020 2020 2020  monics")).      
+0000d600: 2020 7365 6c66 2e6c 6162 656c 5f36 2e73    self.label_6.s
+0000d610: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
+0000d620: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+0000d630: 2242 6163 6b67 726f 756e 6420 436f 6c6f  "Background Colo
+0000d640: 7222 2929 0a20 2020 2020 2020 2073 656c  r")).        sel
+0000d650: 662e 6c61 6265 6c5f 372e 7365 7454 6578  f.label_7.setTex
+0000d660: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+0000d670: 696e 5769 6e64 6f77 222c 2022 5363 616c  inWindow", "Scal
+0000d680: 6520 7365 7474 696e 6722 2929 0a20 2020  e setting")).   
+0000d690: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+0000d6a0: 666f 6c64 612e 7365 7454 6578 7428 5f74  folda.setText(_t
+0000d6b0: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+0000d6c0: 6e64 6f77 222c 2022 312e 2046 696c 6520  ndow", "1. File 
+0000d6d0: 7061 7468 206f 6620 7468 6520 696d 6167  path of the imag
+0000d6e0: 6573 2229 290a 2020 2020 2020 2020 7365  es")).        se
+0000d6f0: 6c66 2e63 625f 7361 7665 416c 6c2e 7365  lf.cb_saveAll.se
+0000d700: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
+0000d710: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+0000d720: 5361 7665 2061 6c6c 206e 6f72 6d61 6c69  Save all normali
+0000d730: 7a65 6420 7361 6d70 6c65 7320 6461 7461  zed samples data
+0000d740: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000d750: 2e6c 6162 656c 5f31 372e 7365 7454 6578  .label_17.setTex
+0000d760: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+0000d770: 696e 5769 6e64 6f77 222c 2022 4361 7465  inWindow", "Cate
+0000d780: 676f 7279 2063 6c61 7373 206e 616d 6520  gory class name 
+0000d790: 286f 7074 696f 6e61 6c2c 2073 6570 6172  (optional, separ
+0000d7a0: 6174 6f72 203d 205c 275f 5c27 2922 2929  ator = \'_\')"))
+0000d7b0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+0000d7c0: 6265 6c5f 7361 7665 2e73 6574 5465 7874  bel_save.setText
+0000d7d0: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+0000d7e0: 6e57 696e 646f 7722 2c20 2232 2e20 5361  nWindow", "2. Sa
+0000d7f0: 7665 2070 6174 6820 666f 7220 466f 7572  ve path for Four
+0000d800: 6965 7220 616e 616c 7973 6973 2229 290a  ier analysis")).
+0000d810: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+0000d820: 656c 5f35 2e73 6574 5465 7874 285f 7472  el_5.setText(_tr
+0000d830: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+0000d840: 646f 7722 2c20 226d 696e 696d 756d 2073  dow", "minimum s
+0000d850: 697a 6520 2870 6978 656c 2922 2929 0a20  ize (pixel)")). 
+0000d860: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+0000d870: 6c5f 332e 7365 7454 6578 7428 5f74 7261  l_3.setText(_tra
+0000d880: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+0000d890: 6f77 222c 2022 496e 6974 6961 6c20 5365  ow", "Initial Se
+0000d8a0: 7474 696e 6720 6f66 2046 6f75 7269 6572  tting of Fourier
+0000d8b0: 2041 6e61 6c79 7369 7322 2929 0a20 2020   Analysis")).   
+0000d8c0: 2020 2020 2073 656c 662e 6275 7474 6f6e       self.button
+0000d8d0: 5f73 6176 652e 7365 7454 6578 7428 5f74  _save.setText(_t
+0000d8e0: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+0000d8f0: 6e64 6f77 222c 2022 7365 6c65 6374 2229  ndow", "select")
+0000d900: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
+0000d910: 7574 746f 6e5f 6865 6164 6572 2e73 6574  utton_header.set
+0000d920: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+0000d930: 224d 6169 6e57 696e 646f 7722 2c20 2261  "MainWindow", "a
+0000d940: 7373 6967 6e22 2929 0a20 2020 2020 2020  ssign")).       
+0000d950: 2073 656c 662e 7262 5f66 696c 656e 616d   self.rb_filenam
+0000d960: 652e 7365 7454 6578 7428 5f74 7261 6e73  e.setText(_trans
+0000d970: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+0000d980: 222c 2022 6669 6c65 206e 616d 6573 2229  ", "file names")
+0000d990: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+0000d9a0: 625f 6e6f 6e65 2e73 6574 5465 7874 285f  b_none.setText(_
+0000d9b0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+0000d9c0: 696e 646f 7722 2c20 224e 6f6e 6522 2929  indow", "None"))
+0000d9d0: 0a20 2020 2020 2020 2073 656c 662e 7262  .        self.rb
+0000d9e0: 5f73 7562 666f 6c64 612e 7365 7454 6578  _subfolda.setTex
+0000d9f0: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+0000da00: 696e 5769 6e64 6f77 222c 2022 666f 6c64  inWindow", "fold
+0000da10: 6572 206e 616d 6573 2229 290a 2020 2020  er names")).    
+0000da20: 2020 2020 7365 6c66 2e6c 6162 656c 5f33      self.label_3
+0000da30: 322e 7365 7454 6578 7428 5f74 7261 6e73  2.setText(_trans
+0000da40: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+0000da50: 222c 2022 342e 2043 6174 6567 6f72 697a  ", "4. Categoriz
+0000da60: 6174 696f 6e20 6d65 7468 6f64 2022 2929  ation method "))
+0000da70: 0a20 2020 2020 2020 2073 656c 662e 6275  .        self.bu
+0000da80: 7474 6f6e 5f46 5053 2e73 6574 5465 7874  tton_FPS.setText
+0000da90: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+0000daa0: 6e57 696e 646f 7722 2c20 2241 6e61 6c79  nWindow", "Analy
+0000dab0: 7a65 2229 290a 2020 2020 2020 2020 7365  ze")).        se
+0000dac0: 6c66 2e6c 6f67 626f 782e 7365 7448 746d  lf.logbox.setHtm
+0000dad0: 6c28 5f74 7261 6e73 6c61 7465 2822 4d61  l(_translate("Ma
+0000dae0: 696e 5769 6e64 6f77 222c 2022 3c21 444f  inWindow", "<!DO
+0000daf0: 4354 5950 4520 4854 4d4c 2050 5542 4c49  CTYPE HTML PUBLI
+0000db00: 4320 5c22 2d2f 2f57 3343 2f2f 4454 4420  C \"-//W3C//DTD 
+0000db10: 4854 4d4c 2034 2e30 2f2f 454e 5c22 205c  HTML 4.0//EN\" \
+0000db20: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+0000db30: 7267 2f54 522f 5245 432d 6874 6d6c 3430  rg/TR/REC-html40
+0000db40: 2f73 7472 6963 742e 6474 645c 223e 5c6e  /strict.dtd\">\n
+0000db50: 220a 223c 6874 6d6c 3e3c 6865 6164 3e3c  "."<html><head><
+0000db60: 6d65 7461 206e 616d 653d 5c22 7172 6963  meta name=\"qric
+0000db70: 6874 6578 745c 2220 636f 6e74 656e 743d  htext\" content=
+0000db80: 5c22 315c 2220 2f3e 3c73 7479 6c65 2074  \"1\" /><style t
+0000db90: 7970 653d 5c22 7465 7874 2f63 7373 5c22  ype=\"text/css\"
+0000dba0: 3e5c 6e22 0a22 702c 206c 6920 7b20 7768  >\n"."p, li { wh
+0000dbb0: 6974 652d 7370 6163 653a 2070 7265 2d77  ite-space: pre-w
+0000dbc0: 7261 703b 207d 5c6e 220a 223c 2f73 7479  rap; }\n"."</sty
+0000dbd0: 6c65 3e3c 2f68 6561 643e 3c62 6f64 7920  le></head><body 
+0000dbe0: 7374 796c 653d 5c22 2066 6f6e 742d 6661  style=\" font-fa
+0000dbf0: 6d69 6c79 3a5c 2753 616e 7320 5365 7269  mily:\'Sans Seri
+0000dc00: 665c 273b 2066 6f6e 742d 7369 7a65 3a39  f\'; font-size:9
+0000dc10: 7074 3b20 666f 6e74 2d77 6569 6768 743a  pt; font-weight:
+0000dc20: 3430 303b 2066 6f6e 742d 7374 796c 653a  400; font-style:
+0000dc30: 6e6f 726d 616c 3b5c 223e 5c6e 220a 223c  normal;\">\n"."<
+0000dc40: 7020 7374 796c 653d 5c22 206d 6172 6769  p style=\" margi
+0000dc50: 6e2d 746f 703a 3070 783b 206d 6172 6769  n-top:0px; margi
+0000dc60: 6e2d 626f 7474 6f6d 3a30 7078 3b20 6d61  n-bottom:0px; ma
+0000dc70: 7267 696e 2d6c 6566 743a 3070 783b 206d  rgin-left:0px; m
+0000dc80: 6172 6769 6e2d 7269 6768 743a 3070 783b  argin-right:0px;
+0000dc90: 202d 7174 2d62 6c6f 636b 2d69 6e64 656e   -qt-block-inden
+0000dca0: 743a 303b 2074 6578 742d 696e 6465 6e74  t:0; text-indent
+0000dcb0: 3a30 7078 3b5c 223e 3c73 7061 6e20 7374  :0px;\"><span st
+0000dcc0: 796c 653d 5c22 2066 6f6e 742d 6661 6d69  yle=\" font-fami
+0000dcd0: 6c79 3a5c 272e 5346 204e 5320 5465 7874  ly:\'.SF NS Text
+0000dce0: 5c27 3b20 666f 6e74 2d77 6569 6768 743a  \'; font-weight:
+0000dcf0: 3630 303b 2074 6578 742d 6465 636f 7261  600; text-decora
+0000dd00: 7469 6f6e 3a20 756e 6465 726c 696e 653b  tion: underline;
+0000dd10: 5c22 3e49 6d61 6765 2041 6e61 6c79 7369  \">Image Analysi
+0000dd20: 7320 5461 623c 2f73 7061 6e3e 3c2f 703e  s Tab</span></p>
+0000dd30: 5c6e 220a 223c 7020 7374 796c 653d 5c22  \n"."<p style=\"
+0000dd40: 2d71 742d 7061 7261 6772 6170 682d 7479  -qt-paragraph-ty
+0000dd50: 7065 3a65 6d70 7479 3b20 6d61 7267 696e  pe:empty; margin
+0000dd60: 2d74 6f70 3a30 7078 3b20 6d61 7267 696e  -top:0px; margin
+0000dd70: 2d62 6f74 746f 6d3a 3070 783b 206d 6172  -bottom:0px; mar
+0000dd80: 6769 6e2d 6c65 6674 3a30 7078 3b20 6d61  gin-left:0px; ma
+0000dd90: 7267 696e 2d72 6967 6874 3a30 7078 3b20  rgin-right:0px; 
+0000dda0: 2d71 742d 626c 6f63 6b2d 696e 6465 6e74  -qt-block-indent
+0000ddb0: 3a30 3b20 7465 7874 2d69 6e64 656e 743a  :0; text-indent:
+0000ddc0: 3070 783b 2066 6f6e 742d 6661 6d69 6c79  0px; font-family
+0000ddd0: 3a5c 272e 5346 204e 5320 5465 7874 5c27  :\'.SF NS Text\'
+0000dde0: 3b20 666f 6e74 2d77 6569 6768 743a 3630  ; font-weight:60
+0000ddf0: 303b 2074 6578 742d 6465 636f 7261 7469  0; text-decorati
+0000de00: 6f6e 3a20 756e 6465 726c 696e 653b 5c22  on: underline;\"
+0000de10: 3e3c 6272 202f 3e3c 2f70 3e5c 6e22 0a22  ><br /></p>\n"."
+0000de20: 3c70 2073 7479 6c65 3d5c 2220 6d61 7267  <p style=\" marg
+0000de30: 696e 2d74 6f70 3a30 7078 3b20 6d61 7267  in-top:0px; marg
+0000de40: 696e 2d62 6f74 746f 6d3a 3070 783b 206d  in-bottom:0px; m
+0000de50: 6172 6769 6e2d 6c65 6674 3a30 7078 3b20  argin-left:0px; 
+0000de60: 6d61 7267 696e 2d72 6967 6874 3a30 7078  margin-right:0px
+0000de70: 3b20 2d71 742d 626c 6f63 6b2d 696e 6465  ; -qt-block-inde
+0000de80: 6e74 3a30 3b20 7465 7874 2d69 6e64 656e  nt:0; text-inden
+0000de90: 743a 3070 783b 5c22 3e3c 7370 616e 2073  t:0px;\"><span s
+0000dea0: 7479 6c65 3d5c 2220 666f 6e74 2d66 616d  tyle=\" font-fam
+0000deb0: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+0000dec0: 745c 273b 2066 6f6e 742d 7765 6967 6874  t\'; font-weight
+0000ded0: 3a36 3030 3b5c 223e 496e 2074 6869 7320  :600;\">In this 
+0000dee0: 7461 622c 2079 6f75 2063 616e 2069 6d70  tab, you can imp
+0000def0: 6f72 7420 796f 7572 2069 6d61 6765 2066  ort your image f
+0000df00: 696c 6573 2061 6e64 2061 7070 6c79 2046  iles and apply F
+0000df10: 6f75 7269 6572 2074 7261 6e73 6f66 726d  ourier transofrm
+0000df20: 2e20 5468 6520 7265 7375 6c74 7320 7769  . The results wi
+0000df30: 6c6c 2062 6520 7361 7665 6420 6173 2046  ll be saved as F
+0000df40: 5053 2e63 7376 2e3c 2f73 7061 6e3e 3c2f  PS.csv.</span></
+0000df50: 703e 5c6e 220a 223c 7020 7374 796c 653d  p>\n"."<p style=
+0000df60: 5c22 206d 6172 6769 6e2d 746f 703a 3070  \" margin-top:0p
+0000df70: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
+0000df80: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
+0000df90: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
+0000dfa0: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
+0000dfb0: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
+0000dfc0: 742d 696e 6465 6e74 3a30 7078 3b5c 223e  t-indent:0px;\">
+0000dfd0: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
+0000dfe0: 6f6e 742d 6661 6d69 6c79 3a5c 272e 5346  ont-family:\'.SF
+0000dff0: 204e 5320 5465 7874 5c27 3b20 666f 6e74   NS Text\'; font
+0000e000: 2d77 6569 6768 743a 3630 303b 5c22 3e42  -weight:600;\">B
+0000e010: 6520 6177 6172 6520 7468 6174 2074 6869  e aware that thi
+0000e020: 7320 4650 532e 6373 7620 7769 6c6c 2062  s FPS.csv will b
+0000e030: 6520 7573 6564 2062 7920 6e65 7874 2050  e used by next P
+0000e040: 4341 2074 6162 2028 646f 206e 6f74 2063  CA tab (do not c
+0000e050: 6861 6e67 6520 7468 6520 6669 6c65 206e  hange the file n
+0000e060: 616d 6520 6d61 6e75 616c 6c79 292e 3c2f  ame manually).</
+0000e070: 7370 616e 3e3c 2f70 3e5c 6e22 0a22 3c70  span></p>\n"."<p
+0000e080: 2073 7479 6c65 3d5c 222d 7174 2d70 6172   style=\"-qt-par
+0000e090: 6167 7261 7068 2d74 7970 653a 656d 7074  agraph-type:empt
+0000e0a0: 793b 206d 6172 6769 6e2d 746f 703a 3070  y; margin-top:0p
+0000e0b0: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
+0000e0c0: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
+0000e0d0: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
+0000e0e0: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
+0000e0f0: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
+0000e100: 742d 696e 6465 6e74 3a30 7078 3b5c 223e  t-indent:0px;\">
+0000e110: 3c62 7220 2f3e 3c2f 703e 5c6e 220a 223c  <br /></p>\n"."<
+0000e120: 7020 7374 796c 653d 5c22 206d 6172 6769  p style=\" margi
+0000e130: 6e2d 746f 703a 3070 783b 206d 6172 6769  n-top:0px; margi
+0000e140: 6e2d 626f 7474 6f6d 3a30 7078 3b20 6d61  n-bottom:0px; ma
+0000e150: 7267 696e 2d6c 6566 743a 3070 783b 206d  rgin-left:0px; m
+0000e160: 6172 6769 6e2d 7269 6768 743a 3070 783b  argin-right:0px;
+0000e170: 202d 7174 2d62 6c6f 636b 2d69 6e64 656e   -qt-block-inden
+0000e180: 743a 303b 2074 6578 742d 696e 6465 6e74  t:0; text-indent
+0000e190: 3a30 7078 3b5c 223e 3c73 7061 6e20 7374  :0px;\"><span st
+0000e1a0: 796c 653d 5c22 2066 6f6e 742d 6661 6d69  yle=\" font-fami
+0000e1b0: 6c79 3a5c 272e 5346 204e 5320 5465 7874  ly:\'.SF NS Text
+0000e1c0: 5c27 3b20 7465 7874 2d64 6563 6f72 6174  \'; text-decorat
+0000e1d0: 696f 6e3a 2075 6e64 6572 6c69 6e65 3b5c  ion: underline;\
+0000e1e0: 223e 496e 7374 7275 6374 696f 6e3c 2f73  ">Instruction</s
+0000e1f0: 7061 6e3e 3c2f 703e 5c6e 220a 223c 7020  pan></p>\n"."<p 
+0000e200: 7374 796c 653d 5c22 2d71 742d 7061 7261  style=\"-qt-para
+0000e210: 6772 6170 682d 7479 7065 3a65 6d70 7479  graph-type:empty
+0000e220: 3b20 6d61 7267 696e 2d74 6f70 3a30 7078  ; margin-top:0px
+0000e230: 3b20 6d61 7267 696e 2d62 6f74 746f 6d3a  ; margin-bottom:
+0000e240: 3070 783b 206d 6172 6769 6e2d 6c65 6674  0px; margin-left
+0000e250: 3a30 7078 3b20 6d61 7267 696e 2d72 6967  :0px; margin-rig
+0000e260: 6874 3a30 7078 3b20 2d71 742d 626c 6f63  ht:0px; -qt-bloc
+0000e270: 6b2d 696e 6465 6e74 3a30 3b20 7465 7874  k-indent:0; text
+0000e280: 2d69 6e64 656e 743a 3070 783b 2066 6f6e  -indent:0px; fon
+0000e290: 742d 6661 6d69 6c79 3a5c 272e 5346 204e  t-family:\'.SF N
+0000e2a0: 5320 5465 7874 5c27 3b20 7465 7874 2d64  S Text\'; text-d
+0000e2b0: 6563 6f72 6174 696f 6e3a 2075 6e64 6572  ecoration: under
+0000e2c0: 6c69 6e65 3b5c 223e 3c62 7220 2f3e 3c2f  line;\"><br /></
+0000e2d0: 703e 5c6e 220a 223c 7020 7374 796c 653d  p>\n"."<p style=
+0000e2e0: 5c22 206d 6172 6769 6e2d 746f 703a 3070  \" margin-top:0p
+0000e2f0: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
+0000e300: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
+0000e310: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
+0000e320: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
+0000e330: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
+0000e340: 742d 696e 6465 6e74 3a30 7078 3b5c 223e  t-indent:0px;\">
+0000e350: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
+0000e360: 6f6e 742d 6661 6d69 6c79 3a5c 272e 5346  ont-family:\'.SF
+0000e370: 204e 5320 5465 7874 5c27 3b5c 223e 312e   NS Text\';\">1.
+0000e380: 2053 656c 6563 7420 796f 7572 2066 696c   Select your fil
+0000e390: 6520 666f 726d 6174 206f 6620 696d 6167  e format of imag
+0000e3a0: 6520 6669 6c65 732e 3c2f 7370 616e 3e3c  e files.</span><
+0000e3b0: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
+0000e3c0: 3d5c 222d 7174 2d70 6172 6167 7261 7068  =\"-qt-paragraph
+0000e3d0: 2d74 7970 653a 656d 7074 793b 206d 6172  -type:empty; mar
+0000e3e0: 6769 6e2d 746f 703a 3070 783b 206d 6172  gin-top:0px; mar
+0000e3f0: 6769 6e2d 626f 7474 6f6d 3a30 7078 3b20  gin-bottom:0px; 
+0000e400: 6d61 7267 696e 2d6c 6566 743a 3070 783b  margin-left:0px;
+0000e410: 206d 6172 6769 6e2d 7269 6768 743a 3070   margin-right:0p
+0000e420: 783b 202d 7174 2d62 6c6f 636b 2d69 6e64  x; -qt-block-ind
+0000e430: 656e 743a 303b 2074 6578 742d 696e 6465  ent:0; text-inde
+0000e440: 6e74 3a30 7078 3b20 666f 6e74 2d66 616d  nt:0px; font-fam
+0000e450: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+0000e460: 745c 273b 5c22 3e3c 6272 202f 3e3c 2f70  t\';\"><br /></p
+0000e470: 3e5c 6e22 0a22 3c70 2073 7479 6c65 3d5c  >\n"."<p style=\
+0000e480: 2220 6d61 7267 696e 2d74 6f70 3a30 7078  " margin-top:0px
+0000e490: 3b20 6d61 7267 696e 2d62 6f74 746f 6d3a  ; margin-bottom:
+0000e4a0: 3070 783b 206d 6172 6769 6e2d 6c65 6674  0px; margin-left
+0000e4b0: 3a30 7078 3b20 6d61 7267 696e 2d72 6967  :0px; margin-rig
+0000e4c0: 6874 3a30 7078 3b20 2d71 742d 626c 6f63  ht:0px; -qt-bloc
+0000e4d0: 6b2d 696e 6465 6e74 3a30 3b20 7465 7874  k-indent:0; text
+0000e4e0: 2d69 6e64 656e 743a 3070 783b 5c22 3e3c  -indent:0px;\"><
+0000e4f0: 7370 616e 2073 7479 6c65 3d5c 2220 666f  span style=\" fo
+0000e500: 6e74 2d66 616d 696c 793a 5c27 2e53 4620  nt-family:\'.SF 
+0000e510: 4e53 2054 6578 745c 273b 5c22 3e32 2e20  NS Text\';\">2. 
+0000e520: 4368 6f6f 7365 2074 6865 206d 6574 686f  Choose the metho
+0000e530: 6420 666f 7220 6361 7465 676f 7269 7a61  d for categoriza
+0000e540: 7469 6f6e 3c2f 7370 616e 3e3c 2f70 3e5c  tion</span></p>\
+0000e550: 6e22 0a22 3c70 2073 7479 6c65 3d5c 2220  n"."<p style=\" 
+0000e560: 6d61 7267 696e 2d74 6f70 3a30 7078 3b20  margin-top:0px; 
+0000e570: 6d61 7267 696e 2d62 6f74 746f 6d3a 3070  margin-bottom:0p
+0000e580: 783b 206d 6172 6769 6e2d 6c65 6674 3a30  x; margin-left:0
+0000e590: 7078 3b20 6d61 7267 696e 2d72 6967 6874  px; margin-right
+0000e5a0: 3a30 7078 3b20 2d71 742d 626c 6f63 6b2d  :0px; -qt-block-
+0000e5b0: 696e 6465 6e74 3a30 3b20 7465 7874 2d69  indent:0; text-i
+0000e5c0: 6e64 656e 743a 3070 783b 5c22 3e3c 7370  ndent:0px;\"><sp
+0000e5d0: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
+0000e5e0: 2d66 616d 696c 793a 5c27 2e53 4620 4e53  -family:\'.SF NS
+0000e5f0: 2054 6578 745c 273b 5c22 3e20 2020 203c   Text\';\">    <
+0000e600: 2f73 7061 6e3e 3c2f 703e 5c6e 220a 223c  /span></p>\n"."<
+0000e610: 7020 7374 796c 653d 5c22 206d 6172 6769  p style=\" margi
+0000e620: 6e2d 746f 703a 3070 783b 206d 6172 6769  n-top:0px; margi
+0000e630: 6e2d 626f 7474 6f6d 3a30 7078 3b20 6d61  n-bottom:0px; ma
+0000e640: 7267 696e 2d6c 6566 743a 3070 783b 206d  rgin-left:0px; m
+0000e650: 6172 6769 6e2d 7269 6768 743a 3070 783b  argin-right:0px;
+0000e660: 202d 7174 2d62 6c6f 636b 2d69 6e64 656e   -qt-block-inden
+0000e670: 743a 303b 2074 6578 742d 696e 6465 6e74  t:0; text-indent
+0000e680: 3a30 7078 3b5c 223e 3c73 7061 6e20 7374  :0px;\"><span st
+0000e690: 796c 653d 5c22 2066 6f6e 742d 6661 6d69  yle=\" font-fami
+0000e6a0: 6c79 3a5c 272e 5346 204e 5320 5465 7874  ly:\'.SF NS Text
+0000e6b0: 5c27 3b5c 223e 332e 2053 656c 6563 7420  \';\">3. Select 
+0000e6c0: 7468 6520 666f 6c64 6120 696e 2077 6869  the folda in whi
+0000e6d0: 6368 2061 6c6c 2079 6f75 7220 696d 6167  ch all your imag
+0000e6e0: 6520 6669 6c65 7320 636f 6e74 6169 6e73  e files contains
+0000e6f0: 3c2f 7370 616e 3e3c 2f70 3e5c 6e22 0a22  </span></p>\n"."
+0000e700: 3c70 2073 7479 6c65 3d5c 222d 7174 2d70  <p style=\"-qt-p
+0000e710: 6172 6167 7261 7068 2d74 7970 653a 656d  aragraph-type:em
+0000e720: 7074 793b 206d 6172 6769 6e2d 746f 703a  pty; margin-top:
+0000e730: 3070 783b 206d 6172 6769 6e2d 626f 7474  0px; margin-bott
+0000e740: 6f6d 3a30 7078 3b20 6d61 7267 696e 2d6c  om:0px; margin-l
+0000e750: 6566 743a 3070 783b 206d 6172 6769 6e2d  eft:0px; margin-
+0000e760: 7269 6768 743a 3070 783b 202d 7174 2d62  right:0px; -qt-b
+0000e770: 6c6f 636b 2d69 6e64 656e 743a 303b 2074  lock-indent:0; t
+0000e780: 6578 742d 696e 6465 6e74 3a30 7078 3b20  ext-indent:0px; 
+0000e790: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+0000e7a0: 4620 4e53 2054 6578 745c 273b 5c22 3e3c  F NS Text\';\"><
+0000e7b0: 6272 202f 3e3c 2f70 3e5c 6e22 0a22 3c70  br /></p>\n"."<p
+0000e7c0: 2073 7479 6c65 3d5c 2220 6d61 7267 696e   style=\" margin
+0000e7d0: 2d74 6f70 3a30 7078 3b20 6d61 7267 696e  -top:0px; margin
+0000e7e0: 2d62 6f74 746f 6d3a 3070 783b 206d 6172  -bottom:0px; mar
+0000e7f0: 6769 6e2d 6c65 6674 3a30 7078 3b20 6d61  gin-left:0px; ma
+0000e800: 7267 696e 2d72 6967 6874 3a30 7078 3b20  rgin-right:0px; 
+0000e810: 2d71 742d 626c 6f63 6b2d 696e 6465 6e74  -qt-block-indent
+0000e820: 3a30 3b20 7465 7874 2d69 6e64 656e 743a  :0; text-indent:
+0000e830: 3070 783b 5c22 3e3c 7370 616e 2073 7479  0px;\"><span sty
+0000e840: 6c65 3d5c 2220 666f 6e74 2d66 616d 696c  le=\" font-famil
+0000e850: 793a 5c27 2e53 4620 4e53 2054 6578 745c  y:\'.SF NS Text\
+0000e860: 273b 5c22 3e34 2e20 284f 7074 696f 6e61  ';\">4. (Optiona
+0000e870: 6c29 2053 6574 2074 6865 206e 616d 6520  l) Set the name 
+0000e880: 6f66 2063 6174 6567 6f72 6965 732e 203c  of categories. <
+0000e890: 2f73 7061 6e3e 3c2f 703e 5c6e 220a 223c  /span></p>\n"."<
+0000e8a0: 7020 7374 796c 653d 5c22 206d 6172 6769  p style=\" margi
+0000e8b0: 6e2d 746f 703a 3070 783b 206d 6172 6769  n-top:0px; margi
+0000e8c0: 6e2d 626f 7474 6f6d 3a30 7078 3b20 6d61  n-bottom:0px; ma
+0000e8d0: 7267 696e 2d6c 6566 743a 3070 783b 206d  rgin-left:0px; m
+0000e8e0: 6172 6769 6e2d 7269 6768 743a 3070 783b  argin-right:0px;
+0000e8f0: 202d 7174 2d62 6c6f 636b 2d69 6e64 656e   -qt-block-inden
+0000e900: 743a 303b 2074 6578 742d 696e 6465 6e74  t:0; text-indent
+0000e910: 3a30 7078 3b5c 223e 3c73 7061 6e20 7374  :0px;\"><span st
+0000e920: 796c 653d 5c22 2066 6f6e 742d 6661 6d69  yle=\" font-fami
+0000e930: 6c79 3a5c 272e 5346 204e 5320 5465 7874  ly:\'.SF NS Text
+0000e940: 5c27 3b5c 223e 2020 203c 2f73 7061 6e3e  \';\">   </span>
+0000e950: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
+0000e960: 6f6e 742d 6661 6d69 6c79 3a5c 272e 5346  ont-family:\'.SF
+0000e970: 204e 5320 5465 7874 5c27 3b20 666f 6e74   NS Text\'; font
+0000e980: 2d77 6569 6768 743a 3630 303b 5c22 3e4e  -weight:600;\">N
+0000e990: 4f54 453a 3c2f 7370 616e 3e3c 7370 616e  OTE:</span><span
+0000e9a0: 2073 7479 6c65 3d5c 2220 666f 6e74 2d66   style=\" font-f
+0000e9b0: 616d 696c 793a 5c27 2e53 4620 4e53 2054  amily:\'.SF NS T
+0000e9c0: 6578 745c 273b 5c22 3e20 3c2f 7370 616e  ext\';\"> </span
+0000e9d0: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
+0000e9e0: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+0000e9f0: 4620 4e53 2054 6578 745c 273b 2066 6f6e  F NS Text\'; fon
+0000ea00: 742d 7765 6967 6874 3a36 3030 3b5c 223e  t-weight:600;\">
+0000ea10: 796f 7520 6d75 7374 2064 6576 6964 6564  you must devided
+0000ea20: 2065 6163 6820 6361 7465 676f 7279 206e   each category n
+0000ea30: 616d 6520 6279 2075 7369 6e67 2075 6e64  ame by using und
+0000ea40: 6572 6261 7220 5c27 5f5c 273c 2f73 7061  erbar \'_\'</spa
+0000ea50: 6e3e 3c2f 703e 5c6e 220a 223c 7020 7374  n></p>\n"."<p st
+0000ea60: 796c 653d 5c22 206d 6172 6769 6e2d 746f  yle=\" margin-to
+0000ea70: 703a 3070 783b 206d 6172 6769 6e2d 626f  p:0px; margin-bo
+0000ea80: 7474 6f6d 3a30 7078 3b20 6d61 7267 696e  ttom:0px; margin
+0000ea90: 2d6c 6566 743a 3070 783b 206d 6172 6769  -left:0px; margi
+0000eaa0: 6e2d 7269 6768 743a 3070 783b 202d 7174  n-right:0px; -qt
+0000eab0: 2d62 6c6f 636b 2d69 6e64 656e 743a 303b  -block-indent:0;
+0000eac0: 2074 6578 742d 696e 6465 6e74 3a30 7078   text-indent:0px
+0000ead0: 3b5c 223e 3c73 7061 6e20 7374 796c 653d  ;\"><span style=
+0000eae0: 5c22 2066 6f6e 742d 6661 6d69 6c79 3a5c  \" font-family:\
+0000eaf0: 272e 5346 204e 5320 5465 7874 5c27 3b20  '.SF NS Text\'; 
+0000eb00: 666f 6e74 2d77 6569 6768 743a 3630 303b  font-weight:600;
+0000eb10: 5c22 3e45 7861 6d70 6c65 3a3c 2f73 7061  \">Example:</spa
+0000eb20: 6e3e 3c2f 703e 5c6e 220a 223c 7020 7374  n></p>\n"."<p st
+0000eb30: 796c 653d 5c22 206d 6172 6769 6e2d 746f  yle=\" margin-to
+0000eb40: 703a 3070 783b 206d 6172 6769 6e2d 626f  p:0px; margin-bo
+0000eb50: 7474 6f6d 3a30 7078 3b20 6d61 7267 696e  ttom:0px; margin
+0000eb60: 2d6c 6566 743a 3070 783b 206d 6172 6769  -left:0px; margi
+0000eb70: 6e2d 7269 6768 743a 3070 783b 202d 7174  n-right:0px; -qt
+0000eb80: 2d62 6c6f 636b 2d69 6e64 656e 743a 303b  -block-indent:0;
+0000eb90: 2074 6578 742d 696e 6465 6e74 3a30 7078   text-indent:0px
+0000eba0: 3b5c 223e 3c73 7061 6e20 7374 796c 653d  ;\"><span style=
+0000ebb0: 5c22 2066 6f6e 742d 6661 6d69 6c79 3a5c  \" font-family:\
+0000ebc0: 272e 5346 204e 5320 5465 7874 5c27 3b5c  '.SF NS Text\';\
+0000ebd0: 223e 596f 7572 2066 6f6c 6465 7220 6469  ">Your folder di
+0000ebe0: 7265 6374 6f72 7920 6d61 7920 6265 206f  rectory may be o
+0000ebf0: 7267 616e 6973 6564 206c 696b 6520 6265  rganised like be
+0000ec00: 6c6c 6f77 2e3c 2f73 7061 6e3e 3c2f 703e  llow.</span></p>
+0000ec10: 5c6e 220a 223c 7020 7374 796c 653d 5c22  \n"."<p style=\"
+0000ec20: 206d 6172 6769 6e2d 746f 703a 3070 783b   margin-top:0px;
+0000ec30: 206d 6172 6769 6e2d 626f 7474 6f6d 3a30   margin-bottom:0
+0000ec40: 7078 3b20 6d61 7267 696e 2d6c 6566 743a  px; margin-left:
+0000ec50: 3070 783b 206d 6172 6769 6e2d 7269 6768  0px; margin-righ
+0000ec60: 743a 3070 783b 202d 7174 2d62 6c6f 636b  t:0px; -qt-block
+0000ec70: 2d69 6e64 656e 743a 303b 2074 6578 742d  -indent:0; text-
+0000ec80: 696e 6465 6e74 3a30 7078 3b5c 223e 3c73  indent:0px;\"><s
+0000ec90: 7061 6e20 7374 796c 653d 5c22 2066 6f6e  pan style=\" fon
+0000eca0: 742d 6661 6d69 6c79 3a5c 272e 5346 204e  t-family:\'.SF N
+0000ecb0: 5320 5465 7874 5c27 3b5c 223e 4461 7461  S Text\';\">Data
+0000ecc0: 202d 2d2d 2074 7970 655f 4120 2d2d 2070   --- type_A -- p
+0000ecd0: 6c61 6365 5f41 202d 2d2d 2073 616d 706c  lace_A --- sampl
+0000ece0: 655f 3030 312e 706e 673c 2f73 7061 6e3e  e_001.png</span>
+0000ecf0: 3c2f 703e 5c6e 220a 223c 7020 7374 796c  </p>\n"."<p styl
+0000ed00: 653d 5c22 206d 6172 6769 6e2d 746f 703a  e=\" margin-top:
+0000ed10: 3070 783b 206d 6172 6769 6e2d 626f 7474  0px; margin-bott
+0000ed20: 6f6d 3a30 7078 3b20 6d61 7267 696e 2d6c  om:0px; margin-l
+0000ed30: 6566 743a 3070 783b 206d 6172 6769 6e2d  eft:0px; margin-
+0000ed40: 7269 6768 743a 3070 783b 202d 7174 2d62  right:0px; -qt-b
+0000ed50: 6c6f 636b 2d69 6e64 656e 743a 303b 2074  lock-indent:0; t
+0000ed60: 6578 742d 696e 6465 6e74 3a30 7078 3b5c  ext-indent:0px;\
+0000ed70: 223e 3c73 7061 6e20 7374 796c 653d 5c22  "><span style=\"
+0000ed80: 2066 6f6e 742d 6661 6d69 6c79 3a5c 272e   font-family:\'.
+0000ed90: 5346 204e 5320 5465 7874 5c27 3b5c 223e  SF NS Text\';\">
+0000eda0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+0000edb0: 2020 2020 2020 2020 2020 202d 2d20 706c             -- pl
+0000edc0: 6163 655f 4220 2d2d 2d20 7361 6d70 6c65  ace_B --- sample
+0000edd0: 5f30 3032 2e70 6e67 3c2f 7370 616e 3e3c  _002.png</span><
+0000ede0: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
+0000edf0: 3d5c 2220 6d61 7267 696e 2d74 6f70 3a30  =\" margin-top:0
+0000ee00: 7078 3b20 6d61 7267 696e 2d62 6f74 746f  px; margin-botto
+0000ee10: 6d3a 3070 783b 206d 6172 6769 6e2d 6c65  m:0px; margin-le
+0000ee20: 6674 3a30 7078 3b20 6d61 7267 696e 2d72  ft:0px; margin-r
+0000ee30: 6967 6874 3a30 7078 3b20 2d71 742d 626c  ight:0px; -qt-bl
+0000ee40: 6f63 6b2d 696e 6465 6e74 3a30 3b20 7465  ock-indent:0; te
+0000ee50: 7874 2d69 6e64 656e 743a 3070 783b 5c22  xt-indent:0px;\"
+0000ee60: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
+0000ee70: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+0000ee80: 4620 4e53 2054 6578 745c 273b 5c22 3e20  F NS Text\';\"> 
+0000ee90: 2020 2020 2020 2020 202d 2d2d 2074 7970           --- typ
+0000eea0: 655f 4220 2d2d 2070 6c61 6365 5f41 202d  e_B -- place_A -
+0000eeb0: 2d2d 2073 616d 706c 655f 3030 332e 706e  -- sample_003.pn
+0000eec0: 673c 2f73 7061 6e3e 3c2f 703e 5c6e 220a  g</span></p>\n".
+0000eed0: 223c 7020 7374 796c 653d 5c22 206d 6172  "<p style=\" mar
+0000eee0: 6769 6e2d 746f 703a 3070 783b 206d 6172  gin-top:0px; mar
+0000eef0: 6769 6e2d 626f 7474 6f6d 3a30 7078 3b20  gin-bottom:0px; 
+0000ef00: 6d61 7267 696e 2d6c 6566 743a 3070 783b  margin-left:0px;
+0000ef10: 206d 6172 6769 6e2d 7269 6768 743a 3070   margin-right:0p
+0000ef20: 783b 202d 7174 2d62 6c6f 636b 2d69 6e64  x; -qt-block-ind
+0000ef30: 656e 743a 303b 2074 6578 742d 696e 6465  ent:0; text-inde
+0000ef40: 6e74 3a30 7078 3b5c 223e 3c73 7061 6e20  nt:0px;\"><span 
+0000ef50: 7374 796c 653d 5c22 2066 6f6e 742d 6661  style=\" font-fa
+0000ef60: 6d69 6c79 3a5c 272e 5346 204e 5320 5465  mily:\'.SF NS Te
+0000ef70: 7874 5c27 3b5c 223e 2020 2020 2020 2020  xt\';\">        
+0000ef80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efa0: 2020 2020 2020 202d 2d2d 2073 616d 706c         --- sampl
+0000efb0: 655f 3030 342e 706e 673c 2f73 7061 6e3e  e_004.png</span>
+0000efc0: 3c2f 703e 5c6e 220a 223c 7020 7374 796c  </p>\n"."<p styl
+0000efd0: 653d 5c22 206d 6172 6769 6e2d 746f 703a  e=\" margin-top:
+0000efe0: 3070 783b 206d 6172 6769 6e2d 626f 7474  0px; margin-bott
+0000eff0: 6f6d 3a30 7078 3b20 6d61 7267 696e 2d6c  om:0px; margin-l
+0000f000: 6566 743a 3070 783b 206d 6172 6769 6e2d  eft:0px; margin-
+0000f010: 7269 6768 743a 3070 783b 202d 7174 2d62  right:0px; -qt-b
+0000f020: 6c6f 636b 2d69 6e64 656e 743a 303b 2074  lock-indent:0; t
+0000f030: 6578 742d 696e 6465 6e74 3a30 7078 3b5c  ext-indent:0px;\
+0000f040: 223e 3c73 7061 6e20 7374 796c 653d 5c22  "><span style=\"
+0000f050: 2066 6f6e 742d 6661 6d69 6c79 3a5c 272e   font-family:\'.
+0000f060: 5346 204e 5320 5465 7874 5c27 3b5c 223e  SF NS Text\';\">
+0000f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f080: 2020 2020 2020 2020 2020 2020 2d2d 2070              -- p
+0000f090: 6c61 6365 5f42 2020 2d2d 2d20 7361 6d70  lace_B  --- samp
+0000f0a0: 6c65 5f30 3035 2e70 6e67 3c2f 7370 616e  le_005.png</span
+0000f0b0: 3e3c 2f70 3e5c 6e22 0a22 3c70 2073 7479  ></p>\n"."<p sty
+0000f0c0: 6c65 3d5c 2220 6d61 7267 696e 2d74 6f70  le=\" margin-top
+0000f0d0: 3a30 7078 3b20 6d61 7267 696e 2d62 6f74  :0px; margin-bot
+0000f0e0: 746f 6d3a 3070 783b 206d 6172 6769 6e2d  tom:0px; margin-
+0000f0f0: 6c65 6674 3a30 7078 3b20 6d61 7267 696e  left:0px; margin
+0000f100: 2d72 6967 6874 3a30 7078 3b20 2d71 742d  -right:0px; -qt-
+0000f110: 626c 6f63 6b2d 696e 6465 6e74 3a30 3b20  block-indent:0; 
+0000f120: 7465 7874 2d69 6e64 656e 743a 3070 783b  text-indent:0px;
+0000f130: 5c22 3e3c 7370 616e 2073 7479 6c65 3d5c  \"><span style=\
+0000f140: 2220 666f 6e74 2d66 616d 696c 793a 5c27  " font-family:\'
+0000f150: 2e53 4620 4e53 2054 6578 745c 273b 5c22  .SF NS Text\';\"
+0000f160: 3e74 6865 6e2c 2079 6f75 206d 6179 2077  >then, you may w
+0000f170: 7269 7465 2c20 666f 7220 696e 7374 616e  rite, for instan
+0000f180: 6365 2c20 5c27 5459 5045 5f50 6c61 6365  ce, \'TYPE_Place
+0000f190: 5f73 616d 706c 655c 2720 696e 2074 6865  _sample\' in the
+0000f1a0: 2074 6578 7462 6f78 206f 6620 6361 7465   textbox of cate
+0000f1b0: 676f 7279 2063 6c61 7373 206e 616d 652e  gory class name.
+0000f1c0: 3c2f 7370 616e 3e3c 2f70 3e5c 6e22 0a22  </span></p>\n"."
+0000f1d0: 3c70 2073 7479 6c65 3d5c 2220 6d61 7267  <p style=\" marg
+0000f1e0: 696e 2d74 6f70 3a30 7078 3b20 6d61 7267  in-top:0px; marg
+0000f1f0: 696e 2d62 6f74 746f 6d3a 3070 783b 206d  in-bottom:0px; m
+0000f200: 6172 6769 6e2d 6c65 6674 3a30 7078 3b20  argin-left:0px; 
+0000f210: 6d61 7267 696e 2d72 6967 6874 3a30 7078  margin-right:0px
+0000f220: 3b20 2d71 742d 626c 6f63 6b2d 696e 6465  ; -qt-block-inde
+0000f230: 6e74 3a30 3b20 7465 7874 2d69 6e64 656e  nt:0; text-inden
+0000f240: 743a 3070 783b 5c22 3e3c 7370 616e 2073  t:0px;\"><span s
+0000f250: 7479 6c65 3d5c 2220 666f 6e74 2d66 616d  tyle=\" font-fam
+0000f260: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+0000f270: 745c 273b 5c22 3e54 6865 6e2c 2074 6872  t\';\">Then, thr
+0000f280: 6565 2064 6174 6120 636f 6c75 6d6e 7320  ee data columns 
+0000f290: 6e61 6d65 6420 5459 5045 2c20 506c 6163  named TYPE, Plac
+0000f2a0: 652c 2061 6e64 2073 616d 706c 6520 7769  e, and sample wi
+0000f2b0: 6c6c 2062 6520 696e 7365 7274 6564 2069  ll be inserted i
+0000f2c0: 6e74 6f20 7468 6520 6f75 7470 7574 2063  nto the output c
+0000f2d0: 7376 2e20 3c2f 7370 616e 3e3c 2f70 3e5c  sv. </span></p>\
+0000f2e0: 6e22 0a22 3c70 2073 7479 6c65 3d5c 222d  n"."<p style=\"-
+0000f2f0: 7174 2d70 6172 6167 7261 7068 2d74 7970  qt-paragraph-typ
+0000f300: 653a 656d 7074 793b 206d 6172 6769 6e2d  e:empty; margin-
+0000f310: 746f 703a 3070 783b 206d 6172 6769 6e2d  top:0px; margin-
+0000f320: 626f 7474 6f6d 3a30 7078 3b20 6d61 7267  bottom:0px; marg
+0000f330: 696e 2d6c 6566 743a 3070 783b 206d 6172  in-left:0px; mar
+0000f340: 6769 6e2d 7269 6768 743a 3070 783b 202d  gin-right:0px; -
+0000f350: 7174 2d62 6c6f 636b 2d69 6e64 656e 743a  qt-block-indent:
+0000f360: 303b 2074 6578 742d 696e 6465 6e74 3a30  0; text-indent:0
+0000f370: 7078 3b20 666f 6e74 2d66 616d 696c 793a  px; font-family:
+0000f380: 5c27 2e53 4620 4e53 2054 6578 745c 273b  \'.SF NS Text\';
+0000f390: 5c22 3e3c 6272 202f 3e3c 2f70 3e5c 6e22  \"><br /></p>\n"
+0000f3a0: 0a22 3c70 2073 7479 6c65 3d5c 2220 6d61  ."<p style=\" ma
+0000f3b0: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
+0000f3c0: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
+0000f3d0: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
+0000f3e0: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
+0000f3f0: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
+0000f400: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
+0000f410: 656e 743a 3070 783b 5c22 3e3c 7370 616e  ent:0px;\"><span
+0000f420: 2073 7479 6c65 3d5c 2220 666f 6e74 2d66   style=\" font-f
+0000f430: 616d 696c 793a 5c27 2e53 4620 4e53 2054  amily:\'.SF NS T
+0000f440: 6578 745c 273b 5c22 3e35 2e20 5365 6c65  ext\';\">5. Sele
+0000f450: 6374 2074 6865 2066 6f6c 6465 7220 746f  ct the folder to
+0000f460: 2073 6176 6520 7468 6520 6f75 7470 7574   save the output
+0000f470: 2043 5356 2066 696c 652e 3c2f 7370 616e   CSV file.</span
+0000f480: 3e3c 2f70 3e5c 6e22 0a22 3c70 2073 7479  ></p>\n"."<p sty
+0000f490: 6c65 3d5c 222d 7174 2d70 6172 6167 7261  le=\"-qt-paragra
+0000f4a0: 7068 2d74 7970 653a 656d 7074 793b 206d  ph-type:empty; m
+0000f4b0: 6172 6769 6e2d 746f 703a 3070 783b 206d  argin-top:0px; m
+0000f4c0: 6172 6769 6e2d 626f 7474 6f6d 3a30 7078  argin-bottom:0px
+0000f4d0: 3b20 6d61 7267 696e 2d6c 6566 743a 3070  ; margin-left:0p
+0000f4e0: 783b 206d 6172 6769 6e2d 7269 6768 743a  x; margin-right:
+0000f4f0: 3070 783b 202d 7174 2d62 6c6f 636b 2d69  0px; -qt-block-i
+0000f500: 6e64 656e 743a 303b 2074 6578 742d 696e  ndent:0; text-in
+0000f510: 6465 6e74 3a30 7078 3b20 666f 6e74 2d66  dent:0px; font-f
+0000f520: 616d 696c 793a 5c27 2e53 4620 4e53 2054  amily:\'.SF NS T
+0000f530: 6578 745c 273b 5c22 3e3c 6272 202f 3e3c  ext\';\"><br /><
+0000f540: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
+0000f550: 3d5c 2220 6d61 7267 696e 2d74 6f70 3a30  =\" margin-top:0
+0000f560: 7078 3b20 6d61 7267 696e 2d62 6f74 746f  px; margin-botto
+0000f570: 6d3a 3070 783b 206d 6172 6769 6e2d 6c65  m:0px; margin-le
+0000f580: 6674 3a30 7078 3b20 6d61 7267 696e 2d72  ft:0px; margin-r
+0000f590: 6967 6874 3a30 7078 3b20 2d71 742d 626c  ight:0px; -qt-bl
+0000f5a0: 6f63 6b2d 696e 6465 6e74 3a30 3b20 7465  ock-indent:0; te
+0000f5b0: 7874 2d69 6e64 656e 743a 3070 783b 5c22  xt-indent:0px;\"
+0000f5c0: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
+0000f5d0: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+0000f5e0: 4620 4e53 2054 6578 745c 273b 5c22 3e36  F NS Text\';\">6
+0000f5f0: 2e20 5365 7420 7468 6520 6261 636b 6772  . Set the backgr
+0000f600: 6f75 6e64 2063 6f6c 6f72 206f 6620 696d  ound color of im
+0000f610: 6167 6520 2869 6620 7468 6520 636f 6c6f  age (if the colo
+0000f620: 7220 6973 2077 726f 6e67 6c79 2063 686f  r is wrongly cho
+0000f630: 6f73 6564 2c20 7468 6520 6461 7461 2067  osed, the data g
+0000f640: 6f65 7320 7772 6f6e 6729 2e3c 2f73 7061  oes wrong).</spa
+0000f650: 6e3e 3c2f 703e 5c6e 220a 223c 7020 7374  n></p>\n"."<p st
+0000f660: 796c 653d 5c22 206d 6172 6769 6e2d 746f  yle=\" margin-to
+0000f670: 703a 3070 783b 206d 6172 6769 6e2d 626f  p:0px; margin-bo
+0000f680: 7474 6f6d 3a30 7078 3b20 6d61 7267 696e  ttom:0px; margin
+0000f690: 2d6c 6566 743a 3070 783b 206d 6172 6769  -left:0px; margi
+0000f6a0: 6e2d 7269 6768 743a 3070 783b 202d 7174  n-right:0px; -qt
+0000f6b0: 2d62 6c6f 636b 2d69 6e64 656e 743a 303b  -block-indent:0;
+0000f6c0: 2074 6578 742d 696e 6465 6e74 3a30 7078   text-indent:0px
+0000f6d0: 3b5c 223e 3c73 7061 6e20 7374 796c 653d  ;\"><span style=
+0000f6e0: 5c22 2066 6f6e 742d 6661 6d69 6c79 3a5c  \" font-family:\
+0000f6f0: 272e 5346 204e 5320 5465 7874 5c27 3b5c  '.SF NS Text\';\
+0000f700: 223e 372e 2053 656c 6563 7420 7468 6520  ">7. Select the 
+0000f710: 4d61 7869 6d75 6d20 4861 726d 6f6e 6963  Maximum Harmonic
+0000f720: 7320 6e75 6d62 6572 2028 5468 6520 6869  s number (The hi
+0000f730: 6768 6573 7420 6672 6571 7565 6e63 7920  ghest frequency 
+0000f740: 7761 7665 2079 6f75 2077 616e 7420 746f  wave you want to
+0000f750: 2075 7365 2069 6e20 7468 6520 466f 7572   use in the Four
+0000f760: 6965 7220 616e 616c 7973 6973 292e 2054  ier analysis). T
+0000f770: 6865 206c 6172 6765 722c 2074 6865 206d  he larger, the m
+0000f780: 6f72 6520 6163 6375 7261 7465 2e20 5965  ore accurate. Ye
+0000f790: 742c 2079 6f75 2073 686f 756c 6420 6361  t, you should ca
+0000f7a0: 7265 6675 6c6c 7920 6368 6f73 6520 6974  refully chose it
+0000f7b0: 2063 6f6e 7369 6465 7269 6e67 2074 6865   considering the
+0000f7c0: 203c 2f73 7061 6e3e 3c73 7061 6e20 7374   </span><span st
+0000f7d0: 796c 653d 5c22 2066 6f6e 742d 6661 6d69  yle=\" font-fami
+0000f7e0: 6c79 3a5c 272e 5346 204e 5320 5465 7874  ly:\'.SF NS Text
+0000f7f0: 5c27 3b20 666f 6e74 2d73 7479 6c65 3a69  \'; font-style:i
+0000f800: 7461 6c69 633b 5c22 3e4e 7971 7565 7374  talic;\">Nyquest
+0000f810: 2046 7265 7175 656e 6379 3c2f 7370 616e   Frequency</span
+0000f820: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
+0000f830: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+0000f840: 4620 4e53 2054 6578 745c 273b 5c22 3e20  F NS Text\';\"> 
+0000f850: 6f66 2079 6f75 7220 6461 7461 2e3c 2f73  of your data.</s
+0000f860: 7061 6e3e 3c2f 703e 5c6e 220a 223c 7020  pan></p>\n"."<p 
+0000f870: 7374 796c 653d 5c22 206d 6172 6769 6e2d  style=\" margin-
+0000f880: 746f 703a 3070 783b 206d 6172 6769 6e2d  top:0px; margin-
+0000f890: 626f 7474 6f6d 3a30 7078 3b20 6d61 7267  bottom:0px; marg
+0000f8a0: 696e 2d6c 6566 743a 3070 783b 206d 6172  in-left:0px; mar
+0000f8b0: 6769 6e2d 7269 6768 743a 3070 783b 202d  gin-right:0px; -
+0000f8c0: 7174 2d62 6c6f 636b 2d69 6e64 656e 743a  qt-block-indent:
+0000f8d0: 303b 2074 6578 742d 696e 6465 6e74 3a30  0; text-indent:0
+0000f8e0: 7078 3b5c 223e 3c73 7061 6e20 7374 796c  px;\"><span styl
+0000f8f0: 653d 5c22 2066 6f6e 742d 6661 6d69 6c79  e=\" font-family
+0000f900: 3a5c 272e 5346 204e 5320 5465 7874 5c27  :\'.SF NS Text\'
+0000f910: 3b20 666f 6e74 2d77 6569 6768 743a 3630  ; font-weight:60
+0000f920: 303b 2063 6f6c 6f72 3a23 6663 3031 3037  0; color:#fc0107
+0000f930: 3b5c 223e 4e4f 5445 3a20 596f 7572 2073  ;\">NOTE: Your s
+0000f940: 616d 706c 6520 7369 7a65 206d 7573 7420  ample size must 
+0000f950: 6265 206c 6172 6765 7220 7468 616e 2061  be larger than a
+0000f960: 7420 6c65 6173 7420 342a 3c2f 7370 616e  t least 4*</span
+0000f970: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
+0000f980: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+0000f990: 4620 4e53 2054 6578 745c 273b 2066 6f6e  F NS Text\'; fon
+0000f9a0: 742d 7765 6967 6874 3a36 3030 3b20 666f  t-weight:600; fo
+0000f9b0: 6e74 2d73 7479 6c65 3a69 7461 6c69 633b  nt-style:italic;
+0000f9c0: 2063 6f6c 6f72 3a23 6663 3031 3037 3b5c   color:#fc0107;\
+0000f9d0: 223e 4e3c 2f73 7061 6e3e 3c73 7061 6e20  ">N</span><span 
+0000f9e0: 7374 796c 653d 5c22 2066 6f6e 742d 6661  style=\" font-fa
+0000f9f0: 6d69 6c79 3a5c 272e 5346 204e 5320 5465  mily:\'.SF NS Te
+0000fa00: 7874 5c27 3b20 666f 6e74 2d77 6569 6768  xt\'; font-weigh
+0000fa10: 743a 3630 303b 2063 6f6c 6f72 3a23 6663  t:600; color:#fc
+0000fa20: 3031 3037 3b5c 223e 2c20 6f74 6865 7277  0107;\">, otherw
+0000fa30: 6973 6520 796f 7520 4341 4e4e 4f54 2063  ise you CANNOT c
+0000fa40: 6f6e 6475 6374 2050 4341 2061 7420 6e65  onduct PCA at ne
+0000fa50: 7874 2074 7562 2e3c 2f73 7061 6e3e 3c2f  xt tub.</span></
+0000fa60: 703e 5c6e 220a 223c 7020 7374 796c 653d  p>\n"."<p style=
+0000fa70: 5c22 206d 6172 6769 6e2d 746f 703a 3070  \" margin-top:0p
+0000fa80: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
+0000fa90: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
+0000faa0: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
+0000fab0: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
+0000fac0: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
+0000fad0: 742d 696e 6465 6e74 3a30 7078 3b5c 223e  t-indent:0px;\">
+0000fae0: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
+0000faf0: 6f6e 742d 6661 6d69 6c79 3a5c 272e 5346  ont-family:\'.SF
+0000fb00: 204e 5320 5465 7874 5c27 3b5c 223e 382e   NS Text\';\">8.
+0000fb10: 2043 686f 6f73 6520 6d69 6e69 6d75 6d20   Choose minimum 
+0000fb20: 7069 7865 6c20 6172 6561 206f 6620 7361  pixel area of sa
+0000fb30: 6d70 6c65 7320 736f 2074 6861 7420 796f  mples so that yo
+0000fb40: 7520 6361 6e20 6578 636c 7564 6520 6e6f  u can exclude no
+0000fb50: 6973 6520 6672 6f6d 2079 6f75 7220 6461  ise from your da
+0000fb60: 7461 2e3c 2f73 7061 6e3e 3c2f 703e 5c6e  ta.</span></p>\n
+0000fb70: 220a 223c 7020 7374 796c 653d 5c22 206d  "."<p style=\" m
+0000fb80: 6172 6769 6e2d 746f 703a 3070 783b 206d  argin-top:0px; m
+0000fb90: 6172 6769 6e2d 626f 7474 6f6d 3a30 7078  argin-bottom:0px
+0000fba0: 3b20 6d61 7267 696e 2d6c 6566 743a 3070  ; margin-left:0p
+0000fbb0: 783b 206d 6172 6769 6e2d 7269 6768 743a  x; margin-right:
+0000fbc0: 3070 783b 202d 7174 2d62 6c6f 636b 2d69  0px; -qt-block-i
+0000fbd0: 6e64 656e 743a 303b 2074 6578 742d 696e  ndent:0; text-in
+0000fbe0: 6465 6e74 3a30 7078 3b5c 223e 3c73 7061  dent:0px;\"><spa
+0000fbf0: 6e20 7374 796c 653d 5c22 2066 6f6e 742d  n style=\" font-
+0000fc00: 6661 6d69 6c79 3a5c 272e 5346 204e 5320  family:\'.SF NS 
+0000fc10: 5465 7874 5c27 3b5c 223e 392e 2073 6574  Text\';\">9. set
+0000fc20: 2053 6361 6c65 2e20 3c2f 7370 616e 3e3c   Scale. </span><
+0000fc30: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
+0000fc40: 3d5c 2220 6d61 7267 696e 2d74 6f70 3a30  =\" margin-top:0
+0000fc50: 7078 3b20 6d61 7267 696e 2d62 6f74 746f  px; margin-botto
+0000fc60: 6d3a 3070 783b 206d 6172 6769 6e2d 6c65  m:0px; margin-le
+0000fc70: 6674 3a30 7078 3b20 6d61 7267 696e 2d72  ft:0px; margin-r
+0000fc80: 6967 6874 3a30 7078 3b20 2d71 742d 626c  ight:0px; -qt-bl
+0000fc90: 6f63 6b2d 696e 6465 6e74 3a30 3b20 7465  ock-indent:0; te
+0000fca0: 7874 2d69 6e64 656e 743a 3070 783b 5c22  xt-indent:0px;\"
+0000fcb0: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
+0000fcc0: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+0000fcd0: 4620 4e53 2054 6578 745c 273b 5c22 3e59  F NS Text\';\">Y
+0000fce0: 6f75 2063 616e 2063 686f 6f73 6520 3244  ou can choose 2D
+0000fcf0: 206f 7220 3144 2073 6361 6c65 2e3c 2f73   or 1D scale.</s
+0000fd00: 7061 6e3e 3c2f 703e 5c6e 220a 223c 7020  pan></p>\n"."<p 
+0000fd10: 7374 796c 653d 5c22 206d 6172 6769 6e2d  style=\" margin-
+0000fd20: 746f 703a 3070 783b 206d 6172 6769 6e2d  top:0px; margin-
+0000fd30: 626f 7474 6f6d 3a30 7078 3b20 6d61 7267  bottom:0px; marg
+0000fd40: 696e 2d6c 6566 743a 3070 783b 206d 6172  in-left:0px; mar
+0000fd50: 6769 6e2d 7269 6768 743a 3070 783b 202d  gin-right:0px; -
+0000fd60: 7174 2d62 6c6f 636b 2d69 6e64 656e 743a  qt-block-indent:
+0000fd70: 303b 2074 6578 742d 696e 6465 6e74 3a30  0; text-indent:0
+0000fd80: 7078 3b5c 223e 3c73 7061 6e20 7374 796c  px;\"><span styl
+0000fd90: 653d 5c22 2066 6f6e 742d 6661 6d69 6c79  e=\" font-family
+0000fda0: 3a5c 272e 5346 204e 5320 5465 7874 5c27  :\'.SF NS Text\'
+0000fdb0: 3b5c 223e 496e 2074 6865 2063 6173 6520  ;\">In the case 
+0000fdc0: 6f66 2032 4420 7363 616c 652c 2079 6f75  of 2D scale, you
+0000fdd0: 7220 6461 7461 2077 696c 6c20 6265 2073  r data will be s
+0000fde0: 6361 6c65 6420 6261 7365 6420 6f6e 2074  caled based on t
+0000fdf0: 6865 2061 7265 6120 6f66 2074 6865 2073  he area of the s
+0000fe00: 6361 6c65 206f 626a 6563 742e 3c2f 7370  cale object.</sp
+0000fe10: 616e 3e3c 2f70 3e5c 6e22 0a22 3c70 2073  an></p>\n"."<p s
+0000fe20: 7479 6c65 3d5c 2220 6d61 7267 696e 2d74  tyle=\" margin-t
+0000fe30: 6f70 3a30 7078 3b20 6d61 7267 696e 2d62  op:0px; margin-b
+0000fe40: 6f74 746f 6d3a 3070 783b 206d 6172 6769  ottom:0px; margi
+0000fe50: 6e2d 6c65 6674 3a30 7078 3b20 6d61 7267  n-left:0px; marg
+0000fe60: 696e 2d72 6967 6874 3a30 7078 3b20 2d71  in-right:0px; -q
+0000fe70: 742d 626c 6f63 6b2d 696e 6465 6e74 3a30  t-block-indent:0
+0000fe80: 3b20 7465 7874 2d69 6e64 656e 743a 3070  ; text-indent:0p
+0000fe90: 783b 5c22 3e3c 7370 616e 2073 7479 6c65  x;\"><span style
+0000fea0: 3d5c 2220 666f 6e74 2d66 616d 696c 793a  =\" font-family:
+0000feb0: 5c27 2e53 4620 4e53 2054 6578 745c 273b  \'.SF NS Text\';
+0000fec0: 5c22 3e49 6e20 7468 6520 6361 7365 206f  \">In the case o
+0000fed0: 6620 3144 2073 6361 6c65 2c20 796f 7572  f 1D scale, your
+0000fee0: 2064 6174 6120 7769 6c6c 2062 6520 7363   data will be sc
+0000fef0: 616c 6564 2062 6173 6564 206f 6e20 7468  aled based on th
+0000ff00: 6520 206c 656e 6774 6820 6f66 2074 6865  e  length of the
+0000ff10: 2073 6361 6c65 206f 626a 6563 742e 3c2f   scale object.</
+0000ff20: 7370 616e 3e3c 2f70 3e5c 6e22 0a22 3c70  span></p>\n"."<p
+0000ff30: 2073 7479 6c65 3d5c 222d 7174 2d70 6172   style=\"-qt-par
+0000ff40: 6167 7261 7068 2d74 7970 653a 656d 7074  agraph-type:empt
+0000ff50: 793b 206d 6172 6769 6e2d 746f 703a 3070  y; margin-top:0p
+0000ff60: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
+0000ff70: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
+0000ff80: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
+0000ff90: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
+0000ffa0: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
+0000ffb0: 742d 696e 6465 6e74 3a30 7078 3b20 666f  t-indent:0px; fo
+0000ffc0: 6e74 2d66 616d 696c 793a 5c27 2e53 4620  nt-family:\'.SF 
+0000ffd0: 4e53 2054 6578 745c 273b 5c22 3e3c 6272  NS Text\';\"><br
+0000ffe0: 202f 3e3c 2f70 3e5c 6e22 0a22 3c70 2073   /></p>\n"."<p s
+0000fff0: 7479 6c65 3d5c 2220 6d61 7267 696e 2d74  tyle=\" margin-t
+00010000: 6f70 3a30 7078 3b20 6d61 7267 696e 2d62  op:0px; margin-b
+00010010: 6f74 746f 6d3a 3070 783b 206d 6172 6769  ottom:0px; margi
+00010020: 6e2d 6c65 6674 3a30 7078 3b20 6d61 7267  n-left:0px; marg
+00010030: 696e 2d72 6967 6874 3a30 7078 3b20 2d71  in-right:0px; -q
+00010040: 742d 626c 6f63 6b2d 696e 6465 6e74 3a30  t-block-indent:0
+00010050: 3b20 7465 7874 2d69 6e64 656e 743a 3070  ; text-indent:0p
+00010060: 783b 5c22 3e3c 7370 616e 2073 7479 6c65  x;\"><span style
+00010070: 3d5c 2220 666f 6e74 2d66 616d 696c 793a  =\" font-family:
+00010080: 5c27 2e53 4620 4e53 2054 6578 745c 273b  \'.SF NS Text\';
+00010090: 5c22 3e31 302e 2050 7265 7373 2026 7175  \">10. Press &qu
+000100a0: 6f74 3b41 6e61 6c79 7a65 2671 756f 743b  ot;Analyze&quot;
+000100b0: 2062 7574 746f 6e2e 3c2f 7370 616e 3e3c   button.</span><
+000100c0: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
+000100d0: 3d5c 222d 7174 2d70 6172 6167 7261 7068  =\"-qt-paragraph
+000100e0: 2d74 7970 653a 656d 7074 793b 206d 6172  -type:empty; mar
+000100f0: 6769 6e2d 746f 703a 3070 783b 206d 6172  gin-top:0px; mar
+00010100: 6769 6e2d 626f 7474 6f6d 3a30 7078 3b20  gin-bottom:0px; 
+00010110: 6d61 7267 696e 2d6c 6566 743a 3070 783b  margin-left:0px;
+00010120: 206d 6172 6769 6e2d 7269 6768 743a 3070   margin-right:0p
+00010130: 783b 202d 7174 2d62 6c6f 636b 2d69 6e64  x; -qt-block-ind
+00010140: 656e 743a 303b 2074 6578 742d 696e 6465  ent:0; text-inde
+00010150: 6e74 3a30 7078 3b20 666f 6e74 2d66 616d  nt:0px; font-fam
+00010160: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+00010170: 745c 273b 5c22 3e3c 6272 202f 3e3c 2f70  t\';\"><br /></p
+00010180: 3e5c 6e22 0a22 3c70 2073 7479 6c65 3d5c  >\n"."<p style=\
+00010190: 2220 6d61 7267 696e 2d74 6f70 3a30 7078  " margin-top:0px
+000101a0: 3b20 6d61 7267 696e 2d62 6f74 746f 6d3a  ; margin-bottom:
+000101b0: 3070 783b 206d 6172 6769 6e2d 6c65 6674  0px; margin-left
+000101c0: 3a30 7078 3b20 6d61 7267 696e 2d72 6967  :0px; margin-rig
+000101d0: 6874 3a30 7078 3b20 2d71 742d 626c 6f63  ht:0px; -qt-bloc
+000101e0: 6b2d 696e 6465 6e74 3a30 3b20 7465 7874  k-indent:0; text
+000101f0: 2d69 6e64 656e 743a 3070 783b 5c22 3e3c  -indent:0px;\"><
+00010200: 7370 616e 2073 7479 6c65 3d5c 2220 666f  span style=\" fo
+00010210: 6e74 2d66 616d 696c 793a 5c27 2e53 4620  nt-family:\'.SF 
+00010220: 4e53 2054 6578 745c 273b 5c22 3e49 6620  NS Text\';\">If 
+00010230: 796f 7572 2061 6e61 6c79 7369 7320 656e  your analysis en
+00010240: 6473 2c20 706c 6561 7365 2067 6f20 746f  ds, please go to
+00010250: 2074 6865 2050 4341 2074 6162 2e3c 2f73   the PCA tab.</s
+00010260: 7061 6e3e 3c2f 703e 5c6e 220a 223c 7020  pan></p>\n"."<p 
+00010270: 7374 796c 653d 5c22 206d 6172 6769 6e2d  style=\" margin-
+00010280: 746f 703a 3070 783b 206d 6172 6769 6e2d  top:0px; margin-
+00010290: 626f 7474 6f6d 3a30 7078 3b20 6d61 7267  bottom:0px; marg
+000102a0: 696e 2d6c 6566 743a 3070 783b 206d 6172  in-left:0px; mar
+000102b0: 6769 6e2d 7269 6768 743a 3070 783b 202d  gin-right:0px; -
+000102c0: 7174 2d62 6c6f 636b 2d69 6e64 656e 743a  qt-block-indent:
+000102d0: 303b 2074 6578 742d 696e 6465 6e74 3a30  0; text-indent:0
+000102e0: 7078 3b5c 223e 3c73 7061 6e20 7374 796c  px;\"><span styl
+000102f0: 653d 5c22 2066 6f6e 742d 6661 6d69 6c79  e=\" font-family
+00010300: 3a5c 272e 5346 204e 5320 5465 7874 5c27  :\'.SF NS Text\'
+00010310: 3b5c 223e 232d 2d2d 2d2d 2d2d 2d2d 2d2d  ;\">#-----------
+00010320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00010330: 2d2d 2d2d 2d2d 3c2f 7370 616e 3e3c 2f70  ------</span></p
+00010340: 3e5c 6e22 0a22 3c70 2073 7479 6c65 3d5c  >\n"."<p style=\
+00010350: 222d 7174 2d70 6172 6167 7261 7068 2d74  "-qt-paragraph-t
+00010360: 7970 653a 656d 7074 793b 206d 6172 6769  ype:empty; margi
+00010370: 6e2d 746f 703a 3070 783b 206d 6172 6769  n-top:0px; margi
+00010380: 6e2d 626f 7474 6f6d 3a30 7078 3b20 6d61  n-bottom:0px; ma
+00010390: 7267 696e 2d6c 6566 743a 3070 783b 206d  rgin-left:0px; m
+000103a0: 6172 6769 6e2d 7269 6768 743a 3070 783b  argin-right:0px;
+000103b0: 202d 7174 2d62 6c6f 636b 2d69 6e64 656e   -qt-block-inden
+000103c0: 743a 303b 2074 6578 742d 696e 6465 6e74  t:0; text-indent
+000103d0: 3a30 7078 3b20 666f 6e74 2d66 616d 696c  :0px; font-famil
+000103e0: 793a 5c27 2e53 4620 4e53 2054 6578 745c  y:\'.SF NS Text\
+000103f0: 273b 2066 6f6e 742d 7369 7a65 3a31 3370  '; font-size:13p
+00010400: 743b 5c22 3e3c 6272 202f 3e3c 2f70 3e3c  t;\"><br /></p><
+00010410: 2f62 6f64 793e 3c2f 6874 6d6c 3e22 2929  /body></html>"))
+00010420: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00010430: 6265 6c5f 322e 7365 7454 6578 7428 5f74  bel_2.setText(_t
+00010440: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+00010450: 6e64 6f77 222c 2022 204c 6f67 2229 290a  ndow", " Log")).
+00010460: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+00010470: 5769 6467 6574 2e73 6574 5461 6254 6578  Widget.setTabTex
+00010480: 7428 7365 6c66 2e74 6162 5769 6467 6574  t(self.tabWidget
+00010490: 2e69 6e64 6578 4f66 2873 656c 662e 7461  .indexOf(self.ta
+000104a0: 6229 2c20 5f74 7261 6e73 6c61 7465 2822  b), _translate("
+000104b0: 4d61 696e 5769 6e64 6f77 222c 2022 496d  MainWindow", "Im
+000104c0: 6167 6520 416e 616c 7973 6973 2229 290a  age Analysis")).
+000104d0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+000104e0: 656c 5f31 312e 7365 7454 6578 7428 5f74  el_11.setText(_t
+000104f0: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+00010500: 6e64 6f77 222c 2022 4d61 7472 6978 2229  ndow", "Matrix")
+00010510: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00010520: 6d62 5f6d 6174 7269 7850 4341 2e73 6574  mb_matrixPCA.set
+00010530: 4974 656d 5465 7874 2830 2c20 5f74 7261  ItemText(0, _tra
+00010540: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00010550: 6f77 222c 2022 436f 7272 656c 6174 696f  ow", "Correlatio
+00010560: 6e22 2929 0a20 2020 2020 2020 2073 656c  n")).        sel
+00010570: 662e 636d 625f 6d61 7472 6978 5043 412e  f.cmb_matrixPCA.
+00010580: 7365 7449 7465 6d54 6578 7428 312c 205f  setItemText(1, _
+00010590: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+000105a0: 696e 646f 7722 2c20 2243 6f76 6172 6961  indow", "Covaria
+000105b0: 6e63 6522 2929 0a20 2020 2020 2020 2073  nce")).        s
+000105c0: 656c 662e 6c61 6265 6c5f 3134 2e73 6574  elf.label_14.set
+000105d0: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+000105e0: 224d 6169 6e57 696e 646f 7722 2c20 2249  "MainWindow", "I
+000105f0: 6e69 7469 616c 2053 6574 7469 6e67 206f  nitial Setting o
+00010600: 6620 5043 4122 2929 0a20 2020 2020 2020  f PCA")).       
+00010610: 2073 656c 662e 636d 625f 4650 532e 7365   self.cmb_FPS.se
+00010620: 7449 7465 6d54 6578 7428 302c 205f 7472  tItemText(0, _tr
+00010630: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00010640: 646f 7722 2c20 2246 5053 2028 4e6f 6e2d  dow", "FPS (Non-
+00010650: 4469 7265 6374 696f 6e61 6c29 2229 290a  Directional)")).
+00010660: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
+00010670: 5f46 5053 2e73 6574 4974 656d 5465 7874  _FPS.setItemText
+00010680: 2831 2c20 5f74 7261 6e73 6c61 7465 2822  (1, _translate("
+00010690: 4d61 696e 5769 6e64 6f77 222c 2022 416d  MainWindow", "Am
+000106a0: 706c 6974 7564 6520 6f66 2048 6172 6d6f  plitude of Harmo
+000106b0: 6e69 6373 2229 290a 2020 2020 2020 2020  nics")).        
+000106c0: 7365 6c66 2e63 6d62 5f46 5053 2e73 6574  self.cmb_FPS.set
+000106d0: 4974 656d 5465 7874 2832 2c20 5f74 7261  ItemText(2, _tra
+000106e0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+000106f0: 6f77 222c 2022 4546 4420 2844 6972 6563  ow", "EFD (Direc
+00010700: 7469 6f6e 616c 2922 2929 0a20 2020 2020  tional)")).     
+00010710: 2020 2073 656c 662e 6c61 6265 6c5f 3133     self.label_13
+00010720: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+00010730: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00010740: 2c20 2253 6176 6520 466f 6c64 612a 2229  , "Save Folda*")
+00010750: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
+00010760: 7574 746f 6e5f 4650 5370 6174 682e 7365  utton_FPSpath.se
+00010770: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
+00010780: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+00010790: 5365 6c65 6374 2229 290a 2020 2020 2020  Select")).      
+000107a0: 2020 7365 6c66 2e6c 6162 656c 5f31 322e    self.label_12.
+000107b0: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
+000107c0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+000107d0: 2022 4669 6c65 2046 6f6c 6461 2a22 2929   "File Folda*"))
+000107e0: 0a20 2020 2020 2020 2073 656c 662e 6275  .        self.bu
+000107f0: 7474 6f6e 5f73 6176 6550 4341 7061 7468  tton_savePCApath
+00010800: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+00010810: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00010820: 2c20 2253 656c 6563 7422 2929 0a20 2020  , "Select")).   
+00010830: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00010840: 3238 2e73 6574 5465 7874 285f 7472 616e  28.setText(_tran
+00010850: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00010860: 7722 2c20 2253 7562 4772 6f75 7022 2929  w", "SubGroup"))
+00010870: 0a20 2020 2020 2020 2073 656c 662e 7075  .        self.pu
+00010880: 7368 4275 7474 6f6e 5f32 2e73 6574 5465  shButton_2.setTe
+00010890: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
+000108a0: 6169 6e57 696e 646f 7722 2c20 2253 6176  ainWindow", "Sav
+000108b0: 6520 4173 2e2e 2e22 2929 0a20 2020 2020  e As...")).     
+000108c0: 2020 2073 656c 662e 6c61 6265 6c5f 3232     self.label_22
+000108d0: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+000108e0: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+000108f0: 2c20 2247 7261 7068 2053 6574 7469 6e67  , "Graph Setting
+00010900: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00010910: 2e70 7573 6842 7574 746f 6e2e 7365 7454  .pushButton.setT
+00010920: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+00010930: 4d61 696e 5769 6e64 6f77 222c 2022 5072  MainWindow", "Pr
+00010940: 6576 6965 7722 2929 0a20 2020 2020 2020  eview")).       
+00010950: 2073 656c 662e 6c61 6265 6c5f 3230 2e73   self.label_20.s
+00010960: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
+00010970: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00010980: 2243 6174 6567 6f72 7922 2929 0a20 2020  "Category")).   
+00010990: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+000109a0: 3138 2e73 6574 5465 7874 285f 7472 616e  18.setText(_tran
+000109b0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+000109c0: 7722 2c20 2258 2d61 7869 7322 2929 0a20  w", "X-axis")). 
+000109d0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+000109e0: 6c5f 3234 2e73 6574 5465 7874 285f 7472  l_24.setText(_tr
+000109f0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00010a00: 646f 7722 2c20 2250 6c6f 7422 2929 0a20  dow", "Plot")). 
+00010a10: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+00010a20: 6c5f 3231 2e73 6574 5465 7874 285f 7472  l_21.setText(_tr
+00010a30: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00010a40: 646f 7722 2c20 2253 697a 6522 2929 0a20  dow", "Size")). 
+00010a50: 2020 2020 2020 2073 656c 662e 636d 625f         self.cmb_
+00010a60: 706c 6f74 2e73 6574 4974 656d 5465 7874  plot.setItemText
+00010a70: 2830 2c20 5f74 7261 6e73 6c61 7465 2822  (0, _translate("
+00010a80: 4d61 696e 5769 6e64 6f77 222c 2022 5363  MainWindow", "Sc
+00010a90: 6174 7465 7222 2929 0a20 2020 2020 2020  atter")).       
+00010aa0: 2073 656c 662e 636d 625f 706c 6f74 2e73   self.cmb_plot.s
+00010ab0: 6574 4974 656d 5465 7874 2831 2c20 5f74  etItemText(1, _t
+00010ac0: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+00010ad0: 6e64 6f77 222c 2022 4465 6e73 6974 7922  ndow", "Density"
+00010ae0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00010af0: 636d 625f 706c 6f74 2e73 6574 4974 656d  cmb_plot.setItem
+00010b00: 5465 7874 2832 2c20 5f74 7261 6e73 6c61  Text(2, _transla
+00010b10: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00010b20: 2022 4869 7374 6f67 7261 6d22 2929 0a20   "Histogram")). 
+00010b30: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+00010b40: 6c5f 3239 2e73 6574 5465 7874 285f 7472  l_29.setText(_tr
+00010b50: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00010b60: 646f 7722 2c20 2253 7562 7375 6247 726f  dow", "SubsubGro
+00010b70: 7570 2229 290a 2020 2020 2020 2020 7365  up")).        se
+00010b80: 6c66 2e6c 6162 656c 5f31 392e 7365 7454  lf.label_19.setT
+00010b90: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+00010ba0: 4d61 696e 5769 6e64 6f77 222c 2022 592d  MainWindow", "Y-
+00010bb0: 6178 6973 2229 290a 2020 2020 2020 2020  axis")).        
+00010bc0: 7365 6c66 2e6c 6162 656c 5f62 696e 732e  self.label_bins.
+00010bd0: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
+00010be0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00010bf0: 2022 6269 6e73 2229 290a 2020 2020 2020   "bins")).      
+00010c00: 2020 7365 6c66 2e6c 6162 656c 5f33 302e    self.label_30.
+00010c10: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
+00010c20: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00010c30: 2022 616c 7068 6122 2929 0a20 2020 2020   "alpha")).     
+00010c40: 2020 2073 656c 662e 6275 7474 6f6e 5f50     self.button_P
+00010c50: 4341 2e73 6574 5465 7874 285f 7472 616e  CA.setText(_tran
+00010c60: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00010c70: 7722 2c20 2250 4341 2229 290a 2020 2020  w", "PCA")).    
+00010c80: 2020 2020 7365 6c66 2e6c 6f67 626f 785f      self.logbox_
+00010c90: 7063 612e 7365 7448 746d 6c28 5f74 7261  pca.setHtml(_tra
+00010ca0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00010cb0: 6f77 222c 2022 3c21 444f 4354 5950 4520  ow", "<!DOCTYPE 
+00010cc0: 4854 4d4c 2050 5542 4c49 4320 5c22 2d2f  HTML PUBLIC \"-/
+00010cd0: 2f57 3343 2f2f 4454 4420 4854 4d4c 2034  /W3C//DTD HTML 4
+00010ce0: 2e30 2f2f 454e 5c22 205c 2268 7474 703a  .0//EN\" \"http:
+00010cf0: 2f2f 7777 772e 7733 2e6f 7267 2f54 522f  //www.w3.org/TR/
+00010d00: 5245 432d 6874 6d6c 3430 2f73 7472 6963  REC-html40/stric
+00010d10: 742e 6474 645c 223e 5c6e 220a 223c 6874  t.dtd\">\n"."<ht
+00010d20: 6d6c 3e3c 6865 6164 3e3c 6d65 7461 206e  ml><head><meta n
+00010d30: 616d 653d 5c22 7172 6963 6874 6578 745c  ame=\"qrichtext\
+00010d40: 2220 636f 6e74 656e 743d 5c22 315c 2220  " content=\"1\" 
+00010d50: 2f3e 3c73 7479 6c65 2074 7970 653d 5c22  /><style type=\"
+00010d60: 7465 7874 2f63 7373 5c22 3e5c 6e22 0a22  text/css\">\n"."
+00010d70: 702c 206c 6920 7b20 7768 6974 652d 7370  p, li { white-sp
+00010d80: 6163 653a 2070 7265 2d77 7261 703b 207d  ace: pre-wrap; }
+00010d90: 5c6e 220a 223c 2f73 7479 6c65 3e3c 2f68  \n"."</style></h
+00010da0: 6561 643e 3c62 6f64 7920 7374 796c 653d  ead><body style=
+00010db0: 5c22 2066 6f6e 742d 6661 6d69 6c79 3a5c  \" font-family:\
+00010dc0: 2753 616e 7320 5365 7269 665c 273b 2066  'Sans Serif\'; f
+00010dd0: 6f6e 742d 7369 7a65 3a39 7074 3b20 666f  ont-size:9pt; fo
+00010de0: 6e74 2d77 6569 6768 743a 3430 303b 2066  nt-weight:400; f
+00010df0: 6f6e 742d 7374 796c 653a 6e6f 726d 616c  ont-style:normal
+00010e00: 3b5c 223e 5c6e 220a 223c 7020 7374 796c  ;\">\n"."<p styl
+00010e10: 653d 5c22 206d 6172 6769 6e2d 746f 703a  e=\" margin-top:
+00010e20: 3070 783b 206d 6172 6769 6e2d 626f 7474  0px; margin-bott
+00010e30: 6f6d 3a30 7078 3b20 6d61 7267 696e 2d6c  om:0px; margin-l
+00010e40: 6566 743a 3070 783b 206d 6172 6769 6e2d  eft:0px; margin-
+00010e50: 7269 6768 743a 3070 783b 202d 7174 2d62  right:0px; -qt-b
+00010e60: 6c6f 636b 2d69 6e64 656e 743a 303b 2074  lock-indent:0; t
+00010e70: 6578 742d 696e 6465 6e74 3a30 7078 3b5c  ext-indent:0px;\
+00010e80: 223e 3c73 7061 6e20 7374 796c 653d 5c22  "><span style=\"
+00010e90: 2066 6f6e 742d 6661 6d69 6c79 3a5c 272e   font-family:\'.
+00010ea0: 5346 204e 5320 5465 7874 5c27 3b20 666f  SF NS Text\'; fo
+00010eb0: 6e74 2d73 697a 653a 3133 7074 3b20 666f  nt-size:13pt; fo
+00010ec0: 6e74 2d77 6569 6768 743a 3630 303b 2074  nt-weight:600; t
+00010ed0: 6578 742d 6465 636f 7261 7469 6f6e 3a20  ext-decoration: 
+00010ee0: 756e 6465 726c 696e 653b 5c22 3e50 7269  underline;\">Pri
+00010ef0: 6e63 6970 616c 2043 6f6d 706f 6e65 6e74  ncipal Component
+00010f00: 2041 6e61 6c79 7379 7320 2850 4341 293c   Analysys (PCA)<
+00010f10: 2f73 7061 6e3e 3c2f 703e 5c6e 220a 223c  /span></p>\n"."<
+00010f20: 7020 7374 796c 653d 5c22 2d71 742d 7061  p style=\"-qt-pa
+00010f30: 7261 6772 6170 682d 7479 7065 3a65 6d70  ragraph-type:emp
+00010f40: 7479 3b20 6d61 7267 696e 2d74 6f70 3a30  ty; margin-top:0
+00010f50: 7078 3b20 6d61 7267 696e 2d62 6f74 746f  px; margin-botto
+00010f60: 6d3a 3070 783b 206d 6172 6769 6e2d 6c65  m:0px; margin-le
+00010f70: 6674 3a30 7078 3b20 6d61 7267 696e 2d72  ft:0px; margin-r
+00010f80: 6967 6874 3a30 7078 3b20 2d71 742d 626c  ight:0px; -qt-bl
+00010f90: 6f63 6b2d 696e 6465 6e74 3a30 3b20 7465  ock-indent:0; te
+00010fa0: 7874 2d69 6e64 656e 743a 3070 783b 2066  xt-indent:0px; f
+00010fb0: 6f6e 742d 6661 6d69 6c79 3a5c 272e 5346  ont-family:\'.SF
+00010fc0: 204e 5320 5465 7874 5c27 3b20 666f 6e74   NS Text\'; font
+00010fd0: 2d73 697a 653a 3133 7074 3b20 666f 6e74  -size:13pt; font
+00010fe0: 2d77 6569 6768 743a 3630 303b 2074 6578  -weight:600; tex
+00010ff0: 742d 6465 636f 7261 7469 6f6e 3a20 756e  t-decoration: un
+00011000: 6465 726c 696e 653b 5c22 3e3c 6272 202f  derline;\"><br /
+00011010: 3e3c 2f70 3e5c 6e22 0a22 3c70 2073 7479  ></p>\n"."<p sty
+00011020: 6c65 3d5c 2220 6d61 7267 696e 2d74 6f70  le=\" margin-top
+00011030: 3a30 7078 3b20 6d61 7267 696e 2d62 6f74  :0px; margin-bot
+00011040: 746f 6d3a 3070 783b 206d 6172 6769 6e2d  tom:0px; margin-
+00011050: 6c65 6674 3a30 7078 3b20 6d61 7267 696e  left:0px; margin
+00011060: 2d72 6967 6874 3a30 7078 3b20 2d71 742d  -right:0px; -qt-
+00011070: 626c 6f63 6b2d 696e 6465 6e74 3a30 3b20  block-indent:0; 
+00011080: 7465 7874 2d69 6e64 656e 743a 3070 783b  text-indent:0px;
+00011090: 5c22 3e3c 7370 616e 2073 7479 6c65 3d5c  \"><span style=\
+000110a0: 2220 666f 6e74 2d66 616d 696c 793a 5c27  " font-family:\'
+000110b0: 2e53 4620 4e53 2054 6578 745c 273b 2066  .SF NS Text\'; f
+000110c0: 6f6e 742d 7369 7a65 3a31 3370 743b 5c22  ont-size:13pt;\"
+000110d0: 3e59 6f75 2063 616e 2063 686f 6f73 6520  >You can choose 
+000110e0: 4650 5320 6f72 2045 4644 2066 6f72 2050  FPS or EFD for P
+000110f0: 4341 2062 6f74 6820 6f66 2077 6869 6368  CA both of which
+00011100: 2061 7265 2065 7870 6f72 7465 6420 6173   are exported as
+00011110: 2046 5053 2e63 7376 2062 7920 7468 6520   FPS.csv by the 
+00011120: 696d 6167 6520 616e 616c 7973 6973 3c2f  image analysis</
+00011130: 7370 616e 3e3c 2f70 3e5c 6e22 0a22 3c70  span></p>\n"."<p
+00011140: 2073 7479 6c65 3d5c 2220 6d61 7267 696e   style=\" margin
+00011150: 2d74 6f70 3a30 7078 3b20 6d61 7267 696e  -top:0px; margin
+00011160: 2d62 6f74 746f 6d3a 3070 783b 206d 6172  -bottom:0px; mar
+00011170: 6769 6e2d 6c65 6674 3a30 7078 3b20 6d61  gin-left:0px; ma
+00011180: 7267 696e 2d72 6967 6874 3a30 7078 3b20  rgin-right:0px; 
+00011190: 2d71 742d 626c 6f63 6b2d 696e 6465 6e74  -qt-block-indent
+000111a0: 3a30 3b20 7465 7874 2d69 6e64 656e 743a  :0; text-indent:
+000111b0: 3070 783b 5c22 3e3c 7370 616e 2073 7479  0px;\"><span sty
+000111c0: 6c65 3d5c 2220 666f 6e74 2d66 616d 696c  le=\" font-famil
+000111d0: 793a 5c27 2e53 4620 4e53 2054 6578 745c  y:\'.SF NS Text\
+000111e0: 273b 2066 6f6e 742d 7369 7a65 3a31 3370  '; font-size:13p
+000111f0: 743b 2063 6f6c 6f72 3a23 6663 3030 3061  t; color:#fc000a
+00011200: 3b5c 223e 4e6f 7465 2074 6861 7420 796f  ;\">Note that yo
+00011210: 7520 6861 7665 2074 6f20 6368 6f6f 7365  u have to choose
+00011220: 2074 6865 2066 6f6c 6461 2077 6869 6368   the folda which
+00011230: 2069 6e63 6c75 6465 2046 5053 2e63 7376   include FPS.csv
+00011240: 2061 7320 4669 6c65 2050 6174 6820 6f74   as File Path ot
+00011250: 6865 7277 6973 6520 796f 7520 3c2f 7370  herwise you </sp
+00011260: 616e 3e3c 7370 616e 2073 7479 6c65 3d5c  an><span style=\
+00011270: 2220 666f 6e74 2d66 616d 696c 793a 5c27  " font-family:\'
+00011280: 2e53 4620 4e53 2054 6578 745c 273b 2066  .SF NS Text\'; f
+00011290: 6f6e 742d 7369 7a65 3a31 3370 743b 2074  ont-size:13pt; t
+000112a0: 6578 742d 6465 636f 7261 7469 6f6e 3a20  ext-decoration: 
+000112b0: 756e 6465 726c 696e 653b 2063 6f6c 6f72  underline; color
+000112c0: 3a23 6663 3030 3061 3b5c 223e 6361 6e6e  :#fc000a;\">cann
+000112d0: 6f74 3c2f 7370 616e 3e3c 7370 616e 2073  ot</span><span s
+000112e0: 7479 6c65 3d5c 2220 666f 6e74 2d66 616d  tyle=\" font-fam
+000112f0: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+00011300: 745c 273b 2066 6f6e 742d 7369 7a65 3a31  t\'; font-size:1
+00011310: 3370 743b 2063 6f6c 6f72 3a23 6663 3030  3pt; color:#fc00
+00011320: 3061 3b5c 223e 2064 6f20 5043 412e 3c2f  0a;\"> do PCA.</
+00011330: 7370 616e 3e3c 2f70 3e5c 6e22 0a22 3c70  span></p>\n"."<p
+00011340: 2073 7479 6c65 3d5c 2220 6d61 7267 696e   style=\" margin
+00011350: 2d74 6f70 3a30 7078 3b20 6d61 7267 696e  -top:0px; margin
+00011360: 2d62 6f74 746f 6d3a 3070 783b 206d 6172  -bottom:0px; mar
+00011370: 6769 6e2d 6c65 6674 3a30 7078 3b20 6d61  gin-left:0px; ma
+00011380: 7267 696e 2d72 6967 6874 3a30 7078 3b20  rgin-right:0px; 
+00011390: 2d71 742d 626c 6f63 6b2d 696e 6465 6e74  -qt-block-indent
+000113a0: 3a30 3b20 7465 7874 2d69 6e64 656e 743a  :0; text-indent:
+000113b0: 3070 783b 5c22 3e3c 7370 616e 2073 7479  0px;\"><span sty
+000113c0: 6c65 3d5c 2220 666f 6e74 2d66 616d 696c  le=\" font-famil
+000113d0: 793a 5c27 2e53 4620 4e53 2054 6578 745c  y:\'.SF NS Text\
+000113e0: 273b 2066 6f6e 742d 7369 7a65 3a31 3370  '; font-size:13p
+000113f0: 743b 2063 6f6c 6f72 3a23 3030 3030 3030  t; color:#000000
+00011400: 3b5c 223e 4650 532e 6373 7620 6973 2074  ;\">FPS.csv is t
+00011410: 6865 2066 696c 6520 7768 6963 6820 7368  he file which sh
+00011420: 6f75 6c64 2062 6520 6578 706f 7274 6564  ould be exported
+00011430: 2061 7420 696d 6167 6520 616e 616c 7973   at image analys
+00011440: 6973 2050 6167 652e 3c2f 7370 616e 3e3c  is Page.</span><
+00011450: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
+00011460: 3d5c 222d 7174 2d70 6172 6167 7261 7068  =\"-qt-paragraph
+00011470: 2d74 7970 653a 656d 7074 793b 206d 6172  -type:empty; mar
+00011480: 6769 6e2d 746f 703a 3070 783b 206d 6172  gin-top:0px; mar
+00011490: 6769 6e2d 626f 7474 6f6d 3a30 7078 3b20  gin-bottom:0px; 
+000114a0: 6d61 7267 696e 2d6c 6566 743a 3070 783b  margin-left:0px;
+000114b0: 206d 6172 6769 6e2d 7269 6768 743a 3070   margin-right:0p
+000114c0: 783b 202d 7174 2d62 6c6f 636b 2d69 6e64  x; -qt-block-ind
+000114d0: 656e 743a 303b 2074 6578 742d 696e 6465  ent:0; text-inde
+000114e0: 6e74 3a30 7078 3b20 666f 6e74 2d66 616d  nt:0px; font-fam
+000114f0: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+00011500: 745c 273b 2066 6f6e 742d 7369 7a65 3a31  t\'; font-size:1
+00011510: 3370 743b 2063 6f6c 6f72 3a23 3030 3030  3pt; color:#0000
+00011520: 3030 3b5c 223e 3c62 7220 2f3e 3c2f 703e  00;\"><br /></p>
+00011530: 5c6e 220a 223c 7020 7374 796c 653d 5c22  \n"."<p style=\"
+00011540: 206d 6172 6769 6e2d 746f 703a 3070 783b   margin-top:0px;
+00011550: 206d 6172 6769 6e2d 626f 7474 6f6d 3a30   margin-bottom:0
+00011560: 7078 3b20 6d61 7267 696e 2d6c 6566 743a  px; margin-left:
+00011570: 3070 783b 206d 6172 6769 6e2d 7269 6768  0px; margin-righ
+00011580: 743a 3070 783b 202d 7174 2d62 6c6f 636b  t:0px; -qt-block
+00011590: 2d69 6e64 656e 743a 303b 2074 6578 742d  -indent:0; text-
+000115a0: 696e 6465 6e74 3a30 7078 3b5c 223e 3c73  indent:0px;\"><s
+000115b0: 7061 6e20 7374 796c 653d 5c22 2066 6f6e  pan style=\" fon
+000115c0: 742d 6661 6d69 6c79 3a5c 272e 5346 204e  t-family:\'.SF N
+000115d0: 5320 5465 7874 5c27 3b20 666f 6e74 2d73  S Text\'; font-s
+000115e0: 697a 653a 3133 7074 3b20 7465 7874 2d64  ize:13pt; text-d
+000115f0: 6563 6f72 6174 696f 6e3a 2075 6e64 6572  ecoration: under
+00011600: 6c69 6e65 3b20 636f 6c6f 723a 2330 3030  line; color:#000
+00011610: 3030 303b 5c22 3e31 2e20 4272 6965 6620  000;\">1. Brief 
+00011620: 6578 706c 616e 6174 696f 6e20 6f66 206d  explanation of m
+00011630: 6574 686f 646f 6c6f 6779 3c2f 7370 616e  ethodology</span
+00011640: 3e3c 2f70 3e5c 6e22 0a22 3c70 2073 7479  ></p>\n"."<p sty
+00011650: 6c65 3d5c 2220 6d61 7267 696e 2d74 6f70  le=\" margin-top
+00011660: 3a30 7078 3b20 6d61 7267 696e 2d62 6f74  :0px; margin-bot
+00011670: 746f 6d3a 3070 783b 206d 6172 6769 6e2d  tom:0px; margin-
+00011680: 6c65 6674 3a30 7078 3b20 6d61 7267 696e  left:0px; margin
+00011690: 2d72 6967 6874 3a30 7078 3b20 2d71 742d  -right:0px; -qt-
+000116a0: 626c 6f63 6b2d 696e 6465 6e74 3a30 3b20  block-indent:0; 
+000116b0: 7465 7874 2d69 6e64 656e 743a 3070 783b  text-indent:0px;
+000116c0: 5c22 3e3c 7370 616e 2073 7479 6c65 3d5c  \"><span style=\
+000116d0: 2220 666f 6e74 2d66 616d 696c 793a 5c27  " font-family:\'
+000116e0: 2e53 4620 4e53 2054 6578 745c 273b 2066  .SF NS Text\'; f
+000116f0: 6f6e 742d 7369 7a65 3a31 3370 743b 2063  ont-size:13pt; c
+00011700: 6f6c 6f72 3a23 3030 3030 3030 3b5c 223e  olor:#000000;\">
+00011710: 596f 7520 6361 6e20 6368 6f6f 7365 2077  You can choose w
+00011720: 6869 6368 2070 6172 616d 6574 6572 2079  hich parameter y
+00011730: 6f75 2075 7365 2066 6f72 2074 6865 2070  ou use for the p
+00011740: 7269 6e63 6970 616c 2063 6f6d 706f 6e65  rincipal compone
+00011750: 6e74 2061 6e61 6c79 7369 7320 2850 4341  nt analysis (PCA
+00011760: 292e 3c2f 7370 616e 3e3c 2f70 3e5c 6e22  ).</span></p>\n"
+00011770: 0a22 3c70 2073 7479 6c65 3d5c 2220 6d61  ."<p style=\" ma
+00011780: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
+00011790: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
+000117a0: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
+000117b0: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
+000117c0: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
+000117d0: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
+000117e0: 656e 743a 3070 783b 5c22 3e3c 7370 616e  ent:0px;\"><span
+000117f0: 2073 7479 6c65 3d5c 2220 666f 6e74 2d66   style=\" font-f
+00011800: 616d 696c 793a 5c27 2e53 4620 4e53 2054  amily:\'.SF NS T
+00011810: 6578 745c 273b 2066 6f6e 742d 7369 7a65  ext\'; font-size
+00011820: 3a31 3370 743b 2063 6f6c 6f72 3a23 3030  :13pt; color:#00
+00011830: 3030 3030 3b5c 223e 5468 6572 6520 6172  0000;\">There ar
+00011840: 6520 7468 7265 6520 6f70 7469 6f6e 733a  e three options:
+00011850: 2046 5053 2c20 416d 706c 6974 7564 6573   FPS, Amplitudes
+00011860: 206f 6620 4861 726d 6f6e 6963 7320 616e   of Harmonics an
+00011870: 6420 7472 6164 6974 696f 6e61 6c20 4546  d traditional EF
+00011880: 442e 3c2f 7370 616e 3e3c 2f70 3e5c 6e22  D.</span></p>\n"
+00011890: 0a22 3c70 2073 7479 6c65 3d5c 222d 7174  ."<p style=\"-qt
+000118a0: 2d70 6172 6167 7261 7068 2d74 7970 653a  -paragraph-type:
+000118b0: 656d 7074 793b 206d 6172 6769 6e2d 746f  empty; margin-to
+000118c0: 703a 3070 783b 206d 6172 6769 6e2d 626f  p:0px; margin-bo
+000118d0: 7474 6f6d 3a30 7078 3b20 6d61 7267 696e  ttom:0px; margin
+000118e0: 2d6c 6566 743a 3070 783b 206d 6172 6769  -left:0px; margi
+000118f0: 6e2d 7269 6768 743a 3070 783b 202d 7174  n-right:0px; -qt
+00011900: 2d62 6c6f 636b 2d69 6e64 656e 743a 303b  -block-indent:0;
+00011910: 2074 6578 742d 696e 6465 6e74 3a30 7078   text-indent:0px
+00011920: 3b20 666f 6e74 2d66 616d 696c 793a 5c27  ; font-family:\'
+00011930: 2e53 4620 4e53 2054 6578 745c 273b 2066  .SF NS Text\'; f
+00011940: 6f6e 742d 7369 7a65 3a31 3370 743b 5c22  ont-size:13pt;\"
+00011950: 3e3c 6272 202f 3e3c 2f70 3e5c 6e22 0a22  ><br /></p>\n"."
+00011960: 3c70 2073 7479 6c65 3d5c 2220 6d61 7267  <p style=\" marg
+00011970: 696e 2d74 6f70 3a30 7078 3b20 6d61 7267  in-top:0px; marg
+00011980: 696e 2d62 6f74 746f 6d3a 3070 783b 206d  in-bottom:0px; m
+00011990: 6172 6769 6e2d 6c65 6674 3a30 7078 3b20  argin-left:0px; 
+000119a0: 6d61 7267 696e 2d72 6967 6874 3a30 7078  margin-right:0px
+000119b0: 3b20 2d71 742d 626c 6f63 6b2d 696e 6465  ; -qt-block-inde
+000119c0: 6e74 3a30 3b20 7465 7874 2d69 6e64 656e  nt:0; text-inden
+000119d0: 743a 3070 783b 5c22 3e3c 7370 616e 2073  t:0px;\"><span s
+000119e0: 7479 6c65 3d5c 2220 666f 6e74 2d66 616d  tyle=\" font-fam
+000119f0: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+00011a00: 745c 273b 2066 6f6e 742d 7369 7a65 3a31  t\'; font-size:1
+00011a10: 3370 743b 2063 6f6c 6f72 3a23 3030 3030  3pt; color:#0000
+00011a20: 3030 3b5c 223e 4669 7374 206f 6620 616c  00;\">Fist of al
+00011a30: 6c2c 2074 6865 2073 6861 7065 206f 6620  l, the shape of 
+00011a40: 7361 6d70 6c65 7320 7765 7265 2063 6f6e  samples were con
+00011a50: 7665 7274 6564 2069 6e74 6f20 7468 6520  verted into the 
+00011a60: 6e75 6d65 7269 6361 6c20 6461 7461 7365  numerical datase
+00011a70: 7420 6174 2026 7175 6f74 3b49 6d61 6765  t at &quot;Image
+00011a80: 2041 6e61 6c79 7369 7326 7175 6f74 3b20   Analysis&quot; 
+00011a90: 7365 6374 696f 6e73 2061 7320 4546 4473  sections as EFDs
+00011aa0: 2e3c 2f73 7061 6e3e 3c2f 703e 5c6e 220a  .</span></p>\n".
+00011ab0: 223c 7020 7374 796c 653d 5c22 206d 6172  "<p style=\" mar
+00011ac0: 6769 6e2d 746f 703a 3070 783b 206d 6172  gin-top:0px; mar
+00011ad0: 6769 6e2d 626f 7474 6f6d 3a30 7078 3b20  gin-bottom:0px; 
+00011ae0: 6d61 7267 696e 2d6c 6566 743a 3070 783b  margin-left:0px;
+00011af0: 206d 6172 6769 6e2d 7269 6768 743a 3070   margin-right:0p
+00011b00: 783b 202d 7174 2d62 6c6f 636b 2d69 6e64  x; -qt-block-ind
+00011b10: 656e 743a 303b 2074 6578 742d 696e 6465  ent:0; text-inde
+00011b20: 6e74 3a30 7078 3b5c 223e 3c73 7061 6e20  nt:0px;\"><span 
+00011b30: 7374 796c 653d 5c22 2066 6f6e 742d 6661  style=\" font-fa
+00011b40: 6d69 6c79 3a5c 272e 5346 204e 5320 5465  mily:\'.SF NS Te
+00011b50: 7874 5c27 3b20 666f 6e74 2d73 697a 653a  xt\'; font-size:
+00011b60: 3133 7074 3b20 636f 6c6f 723a 2330 3030  13pt; color:#000
+00011b70: 3030 303b 5c22 3e45 6163 6820 6f66 2079  000;\">Each of y
+00011b80: 6f75 7220 7361 6d70 6c65 7320 7761 7320  our samples was 
+00011b90: 6465 636f 6d70 6f73 6564 2069 6e74 6f20  decomposed into 
+00011ba0: 7468 6520 6861 726d 6f6e 6963 7320 656c  the harmonics el
+00011bb0: 6c69 7073 6573 206f 6620 7768 6963 6820  lipses of which 
+00011bc0: 746f 7461 6c20 6e75 6d62 6572 2069 7320  total number is 
+00011bd0: 3c2f 7370 616e 3e3c 7370 616e 2073 7479  </span><span sty
+00011be0: 6c65 3d5c 2220 666f 6e74 2d66 616d 696c  le=\" font-famil
+00011bf0: 793a 5c27 2e53 4620 4e53 2054 6578 745c  y:\'.SF NS Text\
+00011c00: 273b 2066 6f6e 742d 7369 7a65 3a31 3370  '; font-size:13p
+00011c10: 743b 2066 6f6e 742d 7374 796c 653a 6974  t; font-style:it
+00011c20: 616c 6963 3b20 636f 6c6f 723a 2330 3030  alic; color:#000
+00011c30: 3030 303b 5c22 3e4e 3c2f 7370 616e 3e3c  000;\">N</span><
+00011c40: 7370 616e 2073 7479 6c65 3d5c 2220 666f  span style=\" fo
+00011c50: 6e74 2d66 616d 696c 793a 5c27 2e53 4620  nt-family:\'.SF 
+00011c60: 4e53 2054 6578 745c 273b 2066 6f6e 742d  NS Text\'; font-
+00011c70: 7369 7a65 3a31 3370 743b 2063 6f6c 6f72  size:13pt; color
+00011c80: 3a23 3030 3030 3030 3b5c 223e 2028 4d61  :#000000;\"> (Ma
+00011c90: 7869 6d75 6d20 6861 726d 6f6e 6963 7320  ximum harmonics 
+00011ca0: 6e75 6d62 6572 292e 3c2f 7370 616e 3e3c  number).</span><
+00011cb0: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
+00011cc0: 3d5c 2220 6d61 7267 696e 2d74 6f70 3a30  =\" margin-top:0
+00011cd0: 7078 3b20 6d61 7267 696e 2d62 6f74 746f  px; margin-botto
+00011ce0: 6d3a 3070 783b 206d 6172 6769 6e2d 6c65  m:0px; margin-le
+00011cf0: 6674 3a30 7078 3b20 6d61 7267 696e 2d72  ft:0px; margin-r
+00011d00: 6967 6874 3a30 7078 3b20 2d71 742d 626c  ight:0px; -qt-bl
+00011d10: 6f63 6b2d 696e 6465 6e74 3a30 3b20 7465  ock-indent:0; te
+00011d20: 7874 2d69 6e64 656e 743a 3070 783b 5c22  xt-indent:0px;\"
+00011d30: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
+00011d40: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+00011d50: 4620 4e53 2054 6578 745c 273b 2066 6f6e  F NS Text\'; fon
+00011d60: 742d 7369 7a65 3a31 3370 743b 2063 6f6c  t-size:13pt; col
+00011d70: 6f72 3a23 3030 3030 3030 3b5c 223e 4561  or:#000000;\">Ea
+00011d80: 6368 2068 6172 6d6f 6e69 6373 2065 6c6c  ch harmonics ell
+00011d90: 6970 7365 7320 6361 6e20 6265 2064 6573  ipses can be des
+00011da0: 6372 6962 6564 2077 6974 6820 666f 7572  cribed with four
+00011db0: 2063 6f6e 7374 616e 7420 636f 6566 6669   constant coeffi
+00011dc0: 6369 656e 7473 203c 2f73 7061 6e3e 3c73  cients </span><s
+00011dd0: 7061 6e20 7374 796c 653d 5c22 2066 6f6e  pan style=\" fon
+00011de0: 742d 6661 6d69 6c79 3a5c 272e 5346 204e  t-family:\'.SF N
+00011df0: 5320 5465 7874 5c27 3b20 666f 6e74 2d73  S Text\'; font-s
+00011e00: 697a 653a 3133 7074 3b20 666f 6e74 2d73  ize:13pt; font-s
+00011e10: 7479 6c65 3a69 7461 6c69 633b 2063 6f6c  tyle:italic; col
+00011e20: 6f72 3a23 3030 3030 3030 3b5c 223e 613c  or:#000000;\">a<
+00011e30: 2f73 7061 6e3e 3c73 7061 6e20 7374 796c  /span><span styl
+00011e40: 653d 5c22 2066 6f6e 742d 6661 6d69 6c79  e=\" font-family
+00011e50: 3a5c 272e 5346 204e 5320 5465 7874 5c27  :\'.SF NS Text\'
+00011e60: 3b20 666f 6e74 2d73 697a 653a 3133 7074  ; font-size:13pt
+00011e70: 3b20 666f 6e74 2d73 7479 6c65 3a69 7461  ; font-style:ita
+00011e80: 6c69 633b 2063 6f6c 6f72 3a23 3030 3030  lic; color:#0000
+00011e90: 3030 3b20 7665 7274 6963 616c 2d61 6c69  00; vertical-ali
+00011ea0: 676e 3a73 7562 3b5c 223e 6e3c 2f73 7061  gn:sub;\">n</spa
+00011eb0: 6e3e 3c73 7061 6e20 7374 796c 653d 5c22  n><span style=\"
+00011ec0: 2066 6f6e 742d 6661 6d69 6c79 3a5c 272e   font-family:\'.
+00011ed0: 5346 204e 5320 5465 7874 5c27 3b20 666f  SF NS Text\'; fo
+00011ee0: 6e74 2d73 697a 653a 3133 7074 3b20 636f  nt-size:13pt; co
+00011ef0: 6c6f 723a 2330 3030 3030 303b 5c22 3e2c  lor:#000000;\">,
+00011f00: 203c 2f73 7061 6e3e 3c73 7061 6e20 7374   </span><span st
+00011f10: 796c 653d 5c22 2066 6f6e 742d 6661 6d69  yle=\" font-fami
+00011f20: 6c79 3a5c 272e 5346 204e 5320 5465 7874  ly:\'.SF NS Text
+00011f30: 5c27 3b20 666f 6e74 2d73 697a 653a 3133  \'; font-size:13
+00011f40: 7074 3b20 666f 6e74 2d73 7479 6c65 3a69  pt; font-style:i
+00011f50: 7461 6c69 633b 2063 6f6c 6f72 3a23 3030  talic; color:#00
+00011f60: 3030 3030 3b5c 223e 623c 2f73 7061 6e3e  0000;\">b</span>
+00011f70: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
+00011f80: 6f6e 742d 6661 6d69 6c79 3a5c 272e 5346  ont-family:\'.SF
+00011f90: 204e 5320 5465 7874 5c27 3b20 666f 6e74   NS Text\'; font
+00011fa0: 2d73 697a 653a 3133 7074 3b20 666f 6e74  -size:13pt; font
+00011fb0: 2d73 7479 6c65 3a69 7461 6c69 633b 2063  -style:italic; c
+00011fc0: 6f6c 6f72 3a23 3030 3030 3030 3b20 7665  olor:#000000; ve
+00011fd0: 7274 6963 616c 2d61 6c69 676e 3a73 7562  rtical-align:sub
+00011fe0: 3b5c 223e 6e3c 2f73 7061 6e3e 3c73 7061  ;\">n</span><spa
+00011ff0: 6e20 7374 796c 653d 5c22 2066 6f6e 742d  n style=\" font-
+00012000: 6661 6d69 6c79 3a5c 272e 5346 204e 5320  family:\'.SF NS 
+00012010: 5465 7874 5c27 3b20 666f 6e74 2d73 697a  Text\'; font-siz
+00012020: 653a 3133 7074 3b20 636f 6c6f 723a 2330  e:13pt; color:#0
+00012030: 3030 3030 303b 5c22 3e2c 203c 2f73 7061  00000;\">, </spa
+00012040: 6e3e 3c73 7061 6e20 7374 796c 653d 5c22  n><span style=\"
+00012050: 2066 6f6e 742d 6661 6d69 6c79 3a5c 272e   font-family:\'.
+00012060: 5346 204e 5320 5465 7874 5c27 3b20 666f  SF NS Text\'; fo
+00012070: 6e74 2d73 697a 653a 3133 7074 3b20 666f  nt-size:13pt; fo
+00012080: 6e74 2d73 7479 6c65 3a69 7461 6c69 633b  nt-style:italic;
+00012090: 2063 6f6c 6f72 3a23 3030 3030 3030 3b5c   color:#000000;\
+000120a0: 223e 633c 2f73 7061 6e3e 3c73 7061 6e20  ">c</span><span 
+000120b0: 7374 796c 653d 5c22 2066 6f6e 742d 6661  style=\" font-fa
+000120c0: 6d69 6c79 3a5c 272e 5346 204e 5320 5465  mily:\'.SF NS Te
+000120d0: 7874 5c27 3b20 666f 6e74 2d73 697a 653a  xt\'; font-size:
+000120e0: 3133 7074 3b20 666f 6e74 2d73 7479 6c65  13pt; font-style
+000120f0: 3a69 7461 6c69 633b 2063 6f6c 6f72 3a23  :italic; color:#
+00012100: 3030 3030 3030 3b20 7665 7274 6963 616c  000000; vertical
+00012110: 2d61 6c69 676e 3a73 7562 3b5c 223e 6e3c  -align:sub;\">n<
+00012120: 2f73 7061 6e3e 3c73 7061 6e20 7374 796c  /span><span styl
+00012130: 653d 5c22 2066 6f6e 742d 6661 6d69 6c79  e=\" font-family
+00012140: 3a5c 272e 5346 204e 5320 5465 7874 5c27  :\'.SF NS Text\'
+00012150: 3b20 666f 6e74 2d73 697a 653a 3133 7074  ; font-size:13pt
+00012160: 3b20 636f 6c6f 723a 2330 3030 3030 303b  ; color:#000000;
+00012170: 5c22 3e20 616e 6420 3c2f 7370 616e 3e3c  \"> and </span><
+00012180: 7370 616e 2073 7479 6c65 3d5c 2220 666f  span style=\" fo
+00012190: 6e74 2d66 616d 696c 793a 5c27 2e53 4620  nt-family:\'.SF 
+000121a0: 4e53 2054 6578 745c 273b 2066 6f6e 742d  NS Text\'; font-
+000121b0: 7369 7a65 3a31 3370 743b 2066 6f6e 742d  size:13pt; font-
+000121c0: 7374 796c 653a 6974 616c 6963 3b20 636f  style:italic; co
+000121d0: 6c6f 723a 2330 3030 3030 303b 5c22 3e64  lor:#000000;\">d
+000121e0: 3c2f 7370 616e 3e3c 7370 616e 2073 7479  </span><span sty
+000121f0: 6c65 3d5c 2220 666f 6e74 2d66 616d 696c  le=\" font-famil
+00012200: 793a 5c27 2e53 4620 4e53 2054 6578 745c  y:\'.SF NS Text\
+00012210: 273b 2066 6f6e 742d 7369 7a65 3a31 3370  '; font-size:13p
+00012220: 743b 2066 6f6e 742d 7374 796c 653a 6974  t; font-style:it
+00012230: 616c 6963 3b20 636f 6c6f 723a 2330 3030  alic; color:#000
+00012240: 3030 303b 2076 6572 7469 6361 6c2d 616c  000; vertical-al
+00012250: 6967 6e3a 7375 623b 5c22 3e6e 3c2f 7370  ign:sub;\">n</sp
+00012260: 616e 3e3c 7370 616e 2073 7479 6c65 3d5c  an><span style=\
+00012270: 2220 666f 6e74 2d66 616d 696c 793a 5c27  " font-family:\'
+00012280: 2e53 4620 4e53 2054 6578 745c 273b 2066  .SF NS Text\'; f
+00012290: 6f6e 742d 7369 7a65 3a31 3370 743b 2066  ont-size:13pt; f
+000122a0: 6f6e 742d 7374 796c 653a 6974 616c 6963  ont-style:italic
+000122b0: 3b20 636f 6c6f 723a 2330 3030 3030 303b  ; color:#000000;
+000122c0: 5c22 3e20 3c2f 7370 616e 3e3c 7370 616e  \"> </span><span
+000122d0: 2073 7479 6c65 3d5c 2220 666f 6e74 2d66   style=\" font-f
+000122e0: 616d 696c 793a 5c27 2e53 4620 4e53 2054  amily:\'.SF NS T
+000122f0: 6578 745c 273b 2066 6f6e 742d 7369 7a65  ext\'; font-size
+00012300: 3a31 3370 743b 2063 6f6c 6f72 3a23 3030  :13pt; color:#00
+00012310: 3030 3030 3b5c 223e 7768 6572 6520 3c2f  0000;\">where </
+00012320: 7370 616e 3e3c 7370 616e 2073 7479 6c65  span><span style
+00012330: 3d5c 2220 666f 6e74 2d66 616d 696c 793a  =\" font-family:
+00012340: 5c27 2e53 4620 4e53 2054 6578 745c 273b  \'.SF NS Text\';
+00012350: 2066 6f6e 742d 7369 7a65 3a31 3370 743b   font-size:13pt;
+00012360: 2066 6f6e 742d 7374 796c 653a 6974 616c   font-style:ital
+00012370: 6963 3b20 636f 6c6f 723a 2330 3030 3030  ic; color:#00000
+00012380: 303b 5c22 3e6e 203c 2f73 7061 6e3e 3c73  0;\">n </span><s
+00012390: 7061 6e20 7374 796c 653d 5c22 2066 6f6e  pan style=\" fon
+000123a0: 742d 6661 6d69 6c79 3a5c 272e 5346 204e  t-family:\'.SF N
+000123b0: 5320 5465 7874 5c27 3b20 666f 6e74 2d73  S Text\'; font-s
+000123c0: 697a 653a 3133 7074 3b20 636f 6c6f 723a  ize:13pt; color:
+000123d0: 2330 3030 3030 303b 5c22 3e3d 3c2f 7370  #000000;\">=</sp
+000123e0: 616e 3e3c 7370 616e 2073 7479 6c65 3d5c  an><span style=\
+000123f0: 2220 666f 6e74 2d66 616d 696c 793a 5c27  " font-family:\'
+00012400: 2e53 4620 4e53 2054 6578 745c 273b 2066  .SF NS Text\'; f
+00012410: 6f6e 742d 7369 7a65 3a31 3370 743b 2066  ont-size:13pt; f
+00012420: 6f6e 742d 7374 796c 653a 6974 616c 6963  ont-style:italic
+00012430: 3b20 636f 6c6f 723a 2330 3030 3030 303b  ; color:#000000;
+00012440: 5c22 3e31 2c32 2c2e 2e2e 4e3c 2f73 7061  \">1,2,...N</spa
+00012450: 6e3e 3c73 7061 6e20 7374 796c 653d 5c22  n><span style=\"
+00012460: 2066 6f6e 742d 6661 6d69 6c79 3a5c 272e   font-family:\'.
+00012470: 5346 204e 5320 5465 7874 5c27 3b20 666f  SF NS Text\'; fo
+00012480: 6e74 2d73 697a 653a 3133 7074 3b20 636f  nt-size:13pt; co
+00012490: 6c6f 723a 2330 3030 3030 303b 5c22 3e2e  lor:#000000;\">.
+000124a0: 2020 3c2f 7370 616e 3e3c 2f70 3e5c 6e22    </span></p>\n"
+000124b0: 0a22 3c70 2073 7479 6c65 3d5c 2220 6d61  ."<p style=\" ma
+000124c0: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
+000124d0: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
+000124e0: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
+000124f0: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
+00012500: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
+00012510: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
+00012520: 656e 743a 3070 783b 5c22 3e3c 7370 616e  ent:0px;\"><span
+00012530: 2073 7479 6c65 3d5c 2220 666f 6e74 2d66   style=\" font-f
+00012540: 616d 696c 793a 5c27 2e53 4620 4e53 2054  amily:\'.SF NS T
+00012550: 6578 745c 273b 2066 6f6e 742d 7369 7a65  ext\'; font-size
+00012560: 3a31 3370 743b 2063 6f6c 6f72 3a23 3030  :13pt; color:#00
+00012570: 3030 3030 3b5c 223e 5468 7573 2065 6163  0000;\">Thus eac
+00012580: 6820 7361 6d70 6c65 2068 6173 203c 2f73  h sample has </s
+00012590: 7061 6e3e 3c73 7061 6e20 7374 796c 653d  pan><span style=
+000125a0: 5c22 2066 6f6e 742d 6661 6d69 6c79 3a5c  \" font-family:\
+000125b0: 272e 5346 204e 5320 5465 7874 5c27 3b20  '.SF NS Text\'; 
+000125c0: 666f 6e74 2d73 697a 653a 3133 7074 3b20  font-size:13pt; 
+000125d0: 666f 6e74 2d73 7479 6c65 3a69 7461 6c69  font-style:itali
+000125e0: 633b 2063 6f6c 6f72 3a23 3030 3030 3030  c; color:#000000
+000125f0: 3b5c 223e 342a 4e3c 2f73 7061 6e3e 3c73  ;\">4*N</span><s
+00012600: 7061 6e20 7374 796c 653d 5c22 2066 6f6e  pan style=\" fon
+00012610: 742d 6661 6d69 6c79 3a5c 272e 5346 204e  t-family:\'.SF N
+00012620: 5320 5465 7874 5c27 3b20 666f 6e74 2d73  S Text\'; font-s
+00012630: 697a 653a 3133 7074 3b20 636f 6c6f 723a  ize:13pt; color:
+00012640: 2330 3030 3030 303b 5c22 3e20 636f 6566  #000000;\"> coef
+00012650: 6669 6369 656e 7473 2e3c 2f73 7061 6e3e  ficients.</span>
+00012660: 3c2f 703e 5c6e 220a 223c 7020 7374 796c  </p>\n"."<p styl
+00012670: 653d 5c22 2d71 742d 7061 7261 6772 6170  e=\"-qt-paragrap
+00012680: 682d 7479 7065 3a65 6d70 7479 3b20 6d61  h-type:empty; ma
+00012690: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
+000126a0: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
+000126b0: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
+000126c0: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
+000126d0: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
+000126e0: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
+000126f0: 656e 743a 3070 783b 2066 6f6e 742d 6661  ent:0px; font-fa
+00012700: 6d69 6c79 3a5c 272e 5346 204e 5320 5465  mily:\'.SF NS Te
+00012710: 7874 5c27 3b20 666f 6e74 2d73 697a 653a  xt\'; font-size:
+00012720: 3133 7074 3b20 636f 6c6f 723a 2330 3030  13pt; color:#000
+00012730: 3030 303b 5c22 3e3c 6272 202f 3e3c 2f70  000;\"><br /></p
+00012740: 3e5c 6e22 0a22 3c70 2073 7479 6c65 3d5c  >\n"."<p style=\
+00012750: 2220 6d61 7267 696e 2d74 6f70 3a30 7078  " margin-top:0px
+00012760: 3b20 6d61 7267 696e 2d62 6f74 746f 6d3a  ; margin-bottom:
+00012770: 3070 783b 206d 6172 6769 6e2d 6c65 6674  0px; margin-left
+00012780: 3a30 7078 3b20 6d61 7267 696e 2d72 6967  :0px; margin-rig
+00012790: 6874 3a30 7078 3b20 2d71 742d 626c 6f63  ht:0px; -qt-bloc
+000127a0: 6b2d 696e 6465 6e74 3a30 3b20 7465 7874  k-indent:0; text
+000127b0: 2d69 6e64 656e 743a 3070 783b 5c22 3e3c  -indent:0px;\"><
+000127c0: 7370 616e 2073 7479 6c65 3d5c 2220 666f  span style=\" fo
+000127d0: 6e74 2d66 616d 696c 793a 5c27 2e53 4620  nt-family:\'.SF 
+000127e0: 4e53 2054 6578 745c 273b 2066 6f6e 742d  NS Text\'; font-
+000127f0: 7369 7a65 3a31 3370 743b 2066 6f6e 742d  size:13pt; font-
+00012800: 7765 6967 6874 3a36 3030 3b5c 223e 4546  weight:600;\">EF
+00012810: 4420 3c2f 7370 616e 3e3c 7370 616e 2073  D </span><span s
+00012820: 7479 6c65 3d5c 2220 666f 6e74 2d66 616d  tyle=\" font-fam
+00012830: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+00012840: 745c 273b 2066 6f6e 742d 7369 7a65 3a31  t\'; font-size:1
+00012850: 3370 743b 5c22 3e28 456c 6c69 7074 6963  3pt;\">(Elliptic
+00012860: 2046 6f75 7269 6572 2044 6573 6372 6970   Fourier Descrip
+00012870: 746f 7229 3c2f 7370 616e 3e3c 2f70 3e5c  tor)</span></p>\
+00012880: 6e22 0a22 3c70 2073 7479 6c65 3d5c 2220  n"."<p style=\" 
+00012890: 6d61 7267 696e 2d74 6f70 3a30 7078 3b20  margin-top:0px; 
+000128a0: 6d61 7267 696e 2d62 6f74 746f 6d3a 3070  margin-bottom:0p
+000128b0: 783b 206d 6172 6769 6e2d 6c65 6674 3a30  x; margin-left:0
+000128c0: 7078 3b20 6d61 7267 696e 2d72 6967 6874  px; margin-right
+000128d0: 3a30 7078 3b20 2d71 742d 626c 6f63 6b2d  :0px; -qt-block-
+000128e0: 696e 6465 6e74 3a30 3b20 7465 7874 2d69  indent:0; text-i
+000128f0: 6e64 656e 743a 3070 783b 5c22 3e3c 7370  ndent:0px;\"><sp
+00012900: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
+00012910: 2d66 616d 696c 793a 5c27 2e53 4620 4e53  -family:\'.SF NS
+00012920: 2054 6578 745c 273b 2066 6f6e 742d 7369   Text\'; font-si
+00012930: 7a65 3a31 3370 743b 5c22 3e54 6869 7320  ze:13pt;\">This 
+00012940: 6973 2074 7261 6469 7469 6f6e 616c 2064  is traditional d
+00012950: 6573 6372 6970 746f 7220 7768 6963 6820  escriptor which 
+00012960: 636f 7272 6573 706f 6e64 7320 746f 2065  corresponds to e
+00012970: 6163 6820 636f 6566 6669 6369 656e 7420  ach coefficient 
+00012980: 6f66 2068 6172 6d6f 6e69 6373 3a20 3c2f  of harmonics: </
+00012990: 7370 616e 3e3c 7370 616e 2073 7479 6c65  span><span style
+000129a0: 3d5c 2220 666f 6e74 2d66 616d 696c 793a  =\" font-family:
+000129b0: 5c27 2e53 4620 4e53 2054 6578 745c 273b  \'.SF NS Text\';
+000129c0: 2066 6f6e 742d 7369 7a65 3a31 3370 743b   font-size:13pt;
+000129d0: 2066 6f6e 742d 7374 796c 653a 6974 616c   font-style:ital
+000129e0: 6963 3b20 636f 6c6f 723a 2330 3030 3030  ic; color:#00000
+000129f0: 303b 5c22 3e61 3c2f 7370 616e 3e3c 7370  0;\">a</span><sp
+00012a00: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
+00012a10: 2d66 616d 696c 793a 5c27 2e53 4620 4e53  -family:\'.SF NS
+00012a20: 2054 6578 745c 273b 2066 6f6e 742d 7369   Text\'; font-si
+00012a30: 7a65 3a31 3370 743b 2066 6f6e 742d 7374  ze:13pt; font-st
+00012a40: 796c 653a 6974 616c 6963 3b20 636f 6c6f  yle:italic; colo
+00012a50: 723a 2330 3030 3030 303b 2076 6572 7469  r:#000000; verti
+00012a60: 6361 6c2d 616c 6967 6e3a 7375 623b 5c22  cal-align:sub;\"
+00012a70: 3e6e 3c2f 7370 616e 3e3c 7370 616e 2073  >n</span><span s
+00012a80: 7479 6c65 3d5c 2220 666f 6e74 2d66 616d  tyle=\" font-fam
+00012a90: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+00012aa0: 745c 273b 2066 6f6e 742d 7369 7a65 3a31  t\'; font-size:1
+00012ab0: 3370 743b 2063 6f6c 6f72 3a23 3030 3030  3pt; color:#0000
+00012ac0: 3030 3b5c 223e 2c20 3c2f 7370 616e 3e3c  00;\">, </span><
+00012ad0: 7370 616e 2073 7479 6c65 3d5c 2220 666f  span style=\" fo
+00012ae0: 6e74 2d66 616d 696c 793a 5c27 2e53 4620  nt-family:\'.SF 
+00012af0: 4e53 2054 6578 745c 273b 2066 6f6e 742d  NS Text\'; font-
+00012b00: 7369 7a65 3a31 3370 743b 2066 6f6e 742d  size:13pt; font-
+00012b10: 7374 796c 653a 6974 616c 6963 3b20 636f  style:italic; co
+00012b20: 6c6f 723a 2330 3030 3030 303b 5c22 3e62  lor:#000000;\">b
+00012b30: 3c2f 7370 616e 3e3c 7370 616e 2073 7479  </span><span sty
+00012b40: 6c65 3d5c 2220 666f 6e74 2d66 616d 696c  le=\" font-famil
+00012b50: 793a 5c27 2e53 4620 4e53 2054 6578 745c  y:\'.SF NS Text\
+00012b60: 273b 2066 6f6e 742d 7369 7a65 3a31 3370  '; font-size:13p
+00012b70: 743b 2066 6f6e 742d 7374 796c 653a 6974  t; font-style:it
+00012b80: 616c 6963 3b20 636f 6c6f 723a 2330 3030  alic; color:#000
+00012b90: 3030 303b 2076 6572 7469 6361 6c2d 616c  000; vertical-al
+00012ba0: 6967 6e3a 7375 623b 5c22 3e6e 3c2f 7370  ign:sub;\">n</sp
+00012bb0: 616e 3e3c 7370 616e 2073 7479 6c65 3d5c  an><span style=\
+00012bc0: 2220 666f 6e74 2d66 616d 696c 793a 5c27  " font-family:\'
+00012bd0: 2e53 4620 4e53 2054 6578 745c 273b 2066  .SF NS Text\'; f
+00012be0: 6f6e 742d 7369 7a65 3a31 3370 743b 2063  ont-size:13pt; c
+00012bf0: 6f6c 6f72 3a23 3030 3030 3030 3b5c 223e  olor:#000000;\">
+00012c00: 2c20 3c2f 7370 616e 3e3c 7370 616e 2073  , </span><span s
+00012c10: 7479 6c65 3d5c 2220 666f 6e74 2d66 616d  tyle=\" font-fam
+00012c20: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+00012c30: 745c 273b 2066 6f6e 742d 7369 7a65 3a31  t\'; font-size:1
+00012c40: 3370 743b 2066 6f6e 742d 7374 796c 653a  3pt; font-style:
+00012c50: 6974 616c 6963 3b20 636f 6c6f 723a 2330  italic; color:#0
+00012c60: 3030 3030 303b 5c22 3e63 3c2f 7370 616e  00000;\">c</span
+00012c70: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
+00012c80: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+00012c90: 4620 4e53 2054 6578 745c 273b 2066 6f6e  F NS Text\'; fon
+00012ca0: 742d 7369 7a65 3a31 3370 743b 2066 6f6e  t-size:13pt; fon
+00012cb0: 742d 7374 796c 653a 6974 616c 6963 3b20  t-style:italic; 
+00012cc0: 636f 6c6f 723a 2330 3030 3030 303b 2076  color:#000000; v
+00012cd0: 6572 7469 6361 6c2d 616c 6967 6e3a 7375  ertical-align:su
+00012ce0: 623b 5c22 3e6e 3c2f 7370 616e 3e3c 7370  b;\">n</span><sp
+00012cf0: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
+00012d00: 2d66 616d 696c 793a 5c27 2e53 4620 4e53  -family:\'.SF NS
+00012d10: 2054 6578 745c 273b 2066 6f6e 742d 7369   Text\'; font-si
+00012d20: 7a65 3a31 3370 743b 2063 6f6c 6f72 3a23  ze:13pt; color:#
+00012d30: 3030 3030 3030 3b5c 223e 2061 6e64 203c  000000;\"> and <
+00012d40: 2f73 7061 6e3e 3c73 7061 6e20 7374 796c  /span><span styl
+00012d50: 653d 5c22 2066 6f6e 742d 6661 6d69 6c79  e=\" font-family
+00012d60: 3a5c 272e 5346 204e 5320 5465 7874 5c27  :\'.SF NS Text\'
+00012d70: 3b20 666f 6e74 2d73 697a 653a 3133 7074  ; font-size:13pt
+00012d80: 3b20 666f 6e74 2d73 7479 6c65 3a69 7461  ; font-style:ita
+00012d90: 6c69 633b 2063 6f6c 6f72 3a23 3030 3030  lic; color:#0000
+00012da0: 3030 3b5c 223e 643c 2f73 7061 6e3e 3c73  00;\">d</span><s
+00012db0: 7061 6e20 7374 796c 653d 5c22 2066 6f6e  pan style=\" fon
+00012dc0: 742d 6661 6d69 6c79 3a5c 272e 5346 204e  t-family:\'.SF N
+00012dd0: 5320 5465 7874 5c27 3b20 666f 6e74 2d73  S Text\'; font-s
+00012de0: 697a 653a 3133 7074 3b20 666f 6e74 2d73  ize:13pt; font-s
+00012df0: 7479 6c65 3a69 7461 6c69 633b 2063 6f6c  tyle:italic; col
+00012e00: 6f72 3a23 3030 3030 3030 3b20 7665 7274  or:#000000; vert
+00012e10: 6963 616c 2d61 6c69 676e 3a73 7562 3b5c  ical-align:sub;\
+00012e20: 223e 6e3c 2f73 7061 6e3e 3c2f 703e 5c6e  ">n</span></p>\n
+00012e30: 220a 223c 7020 7374 796c 653d 5c22 206d  "."<p style=\" m
+00012e40: 6172 6769 6e2d 746f 703a 3070 783b 206d  argin-top:0px; m
+00012e50: 6172 6769 6e2d 626f 7474 6f6d 3a30 7078  argin-bottom:0px
+00012e60: 3b20 6d61 7267 696e 2d6c 6566 743a 3070  ; margin-left:0p
+00012e70: 783b 206d 6172 6769 6e2d 7269 6768 743a  x; margin-right:
+00012e80: 3070 783b 202d 7174 2d62 6c6f 636b 2d69  0px; -qt-block-i
+00012e90: 6e64 656e 743a 303b 2074 6578 742d 696e  ndent:0; text-in
+00012ea0: 6465 6e74 3a30 7078 3b5c 223e 3c73 7061  dent:0px;\"><spa
+00012eb0: 6e20 7374 796c 653d 5c22 2066 6f6e 742d  n style=\" font-
+00012ec0: 6661 6d69 6c79 3a5c 272e 5346 204e 5320  family:\'.SF NS 
+00012ed0: 5465 7874 5c27 3b20 666f 6e74 2d73 697a  Text\'; font-siz
+00012ee0: 653a 3133 7074 3b5c 223e 4546 442d 6261  e:13pt;\">EFD-ba
+00012ef0: 7365 6420 5043 4120 6973 2073 7569 7462  sed PCA is suitb
+00012f00: 6c65 2066 6f72 2064 6972 6563 7469 6f6e  le for direction
+00012f10: 616c 2064 6174 6120 7375 6368 2061 7320  al data such as 
+00012f20: 666f 7373 696c 7320 616e 6420 6f74 6865  fossils and othe
+00012f30: 7220 6f72 6761 6e69 6320 6d61 7474 6572  r organic matter
+00012f40: 7320 2873 6565 204b 7568 6c20 616e 6420  s (see Kuhl and 
+00012f50: 4769 6172 6469 6e61 2031 3938 3229 202e  Giardina 1982) .
+00012f60: 2020 484f 5745 5645 522c 2069 6e20 7468    HOWEVER, in th
+00012f70: 6520 6361 7365 206f 6620 6e6f 6e2d 6469  e case of non-di
+00012f80: 7265 6374 696f 6e61 6c20 6461 7461 7365  rectional datase
+00012f90: 7420 7375 6368 2061 7320 6772 6169 6e73  t such as grains
+00012fa0: 2c20 4546 442d 6261 7365 6420 5043 4120  , EFD-based PCA 
+00012fb0: 6f66 7465 6e20 646f 206e 6f74 2077 6f72  often do not wor
+00012fc0: 6b20 7765 6c6c 2e20 3c2f 7370 616e 3e3c  k well. </span><
+00012fd0: 2f70 3e5c 6e22 0a22 3c70 2073 7479 6c65  /p>\n"."<p style
+00012fe0: 3d5c 2220 6d61 7267 696e 2d74 6f70 3a30  =\" margin-top:0
+00012ff0: 7078 3b20 6d61 7267 696e 2d62 6f74 746f  px; margin-botto
+00013000: 6d3a 3070 783b 206d 6172 6769 6e2d 6c65  m:0px; margin-le
+00013010: 6674 3a30 7078 3b20 6d61 7267 696e 2d72  ft:0px; margin-r
+00013020: 6967 6874 3a30 7078 3b20 2d71 742d 626c  ight:0px; -qt-bl
+00013030: 6f63 6b2d 696e 6465 6e74 3a30 3b20 7465  ock-indent:0; te
+00013040: 7874 2d69 6e64 656e 743a 3070 783b 5c22  xt-indent:0px;\"
+00013050: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
+00013060: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+00013070: 4620 4e53 2054 6578 745c 273b 2066 6f6e  F NS Text\'; fon
+00013080: 742d 7369 7a65 3a31 3370 743b 5c22 3e54  t-size:13pt;\">T
+00013090: 6869 7320 6973 2062 6563 6175 7365 2045  his is because E
+000130a0: 4644 2d62 6173 6564 2050 4341 206f 6674  FD-based PCA oft
+000130b0: 656e 2065 6e64 7320 7570 2020 636f 6e63  en ends up  conc
+000130c0: 6c75 6469 6e67 2074 6861 7420 7468 6520  luding that the 
+000130d0: 7368 6170 6520 7661 7269 6174 696f 6e20  shape variation 
+000130e0: 6973 2073 756d 6d61 7269 7a65 6420 6279  is summarized by
+000130f0: 206d 6972 726f 7220 7379 6d6d 6574 7269   mirror symmetri
+00013100: 6320 7072 6f70 6572 7469 6573 2077 6869  c properties whi
+00013110: 6368 2c20 696e 206d 6f73 7420 6361 7365  ch, in most case
+00013120: 732c 2068 6176 6520 6e6f 2073 6369 656e  s, have no scien
+00013130: 7469 6669 6320 696e 7465 7265 7374 206f  tific interest o
+00013140: 6620 7061 7274 6963 6c65 2073 6861 7065  f particle shape
+00013150: 732e 3c2f 7370 616e 3e3c 2f70 3e5c 6e22  s.</span></p>\n"
+00013160: 0a22 3c70 2073 7479 6c65 3d5c 222d 7174  ."<p style=\"-qt
+00013170: 2d70 6172 6167 7261 7068 2d74 7970 653a  -paragraph-type:
+00013180: 656d 7074 793b 206d 6172 6769 6e2d 746f  empty; margin-to
+00013190: 703a 3070 783b 206d 6172 6769 6e2d 626f  p:0px; margin-bo
+000131a0: 7474 6f6d 3a30 7078 3b20 6d61 7267 696e  ttom:0px; margin
+000131b0: 2d6c 6566 743a 3070 783b 206d 6172 6769  -left:0px; margi
+000131c0: 6e2d 7269 6768 743a 3070 783b 202d 7174  n-right:0px; -qt
+000131d0: 2d62 6c6f 636b 2d69 6e64 656e 743a 303b  -block-indent:0;
+000131e0: 2074 6578 742d 696e 6465 6e74 3a30 7078   text-indent:0px
+000131f0: 3b20 666f 6e74 2d66 616d 696c 793a 5c27  ; font-family:\'
+00013200: 2e53 4620 4e53 2054 6578 745c 273b 2066  .SF NS Text\'; f
+00013210: 6f6e 742d 7369 7a65 3a31 3370 743b 2063  ont-size:13pt; c
+00013220: 6f6c 6f72 3a23 3030 3030 3030 3b5c 223e  olor:#000000;\">
+00013230: 3c62 7220 2f3e 3c2f 703e 5c6e 220a 223c  <br /></p>\n"."<
+00013240: 7020 7374 796c 653d 5c22 206d 6172 6769  p style=\" margi
+00013250: 6e2d 746f 703a 3070 783b 206d 6172 6769  n-top:0px; margi
+00013260: 6e2d 626f 7474 6f6d 3a30 7078 3b20 6d61  n-bottom:0px; ma
+00013270: 7267 696e 2d6c 6566 743a 3070 783b 206d  rgin-left:0px; m
+00013280: 6172 6769 6e2d 7269 6768 743a 3070 783b  argin-right:0px;
+00013290: 202d 7174 2d62 6c6f 636b 2d69 6e64 656e   -qt-block-inden
+000132a0: 743a 303b 2074 6578 742d 696e 6465 6e74  t:0; text-indent
+000132b0: 3a30 7078 3b5c 223e 3c73 7061 6e20 7374  :0px;\"><span st
+000132c0: 796c 653d 5c22 2066 6f6e 742d 6661 6d69  yle=\" font-fami
+000132d0: 6c79 3a5c 272e 5346 204e 5320 5465 7874  ly:\'.SF NS Text
+000132e0: 5c27 3b20 666f 6e74 2d73 697a 653a 3133  \'; font-size:13
+000132f0: 7074 3b20 666f 6e74 2d77 6569 6768 743a  pt; font-weight:
+00013300: 3630 303b 5c22 3e46 5053 3c2f 7370 616e  600;\">FPS</span
+00013310: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
+00013320: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+00013330: 4620 4e53 2054 6578 745c 273b 2066 6f6e  F NS Text\'; fon
+00013340: 742d 7369 7a65 3a31 3370 743b 5c22 3e20  t-size:13pt;\"> 
+00013350: 2846 6f75 7269 6572 2050 6f77 6572 2053  (Fourier Power S
+00013360: 7065 6374 7261 293c 2f73 7061 6e3e 3c2f  pectra)</span></
+00013370: 703e 5c6e 220a 223c 7020 7374 796c 653d  p>\n"."<p style=
+00013380: 5c22 206d 6172 6769 6e2d 746f 703a 3070  \" margin-top:0p
+00013390: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
+000133a0: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
+000133b0: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
+000133c0: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
+000133d0: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
+000133e0: 742d 696e 6465 6e74 3a30 7078 3b5c 223e  t-indent:0px;\">
+000133f0: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
+00013400: 6f6e 742d 6661 6d69 6c79 3a5c 272e 5346  ont-family:\'.SF
+00013410: 204e 5320 5465 7874 5c27 3b20 666f 6e74   NS Text\'; font
+00013420: 2d73 697a 653a 3133 7074 3b5c 223e 4974  -size:13pt;\">It
+00013430: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
+00013440: 7468 6568 616c 6620 6f66 2073 756d 206f  thehalf of sum o
+00013450: 6620 7371 7561 7265 7320 6f66 2045 4644  f squares of EFD
+00013460: 733a 2046 5053 3c2f 7370 616e 3e3c 7370  s: FPS</span><sp
+00013470: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
+00013480: 2d66 616d 696c 793a 5c27 2e53 4620 4e53  -family:\'.SF NS
+00013490: 2054 6578 745c 273b 2066 6f6e 742d 7369   Text\'; font-si
+000134a0: 7a65 3a31 3370 743b 2076 6572 7469 6361  ze:13pt; vertica
+000134b0: 6c2d 616c 6967 6e3a 7375 623b 5c22 3e6e  l-align:sub;\">n
+000134c0: 3c2f 7370 616e 3e3c 7370 616e 2073 7479  </span><span sty
+000134d0: 6c65 3d5c 2220 666f 6e74 2d66 616d 696c  le=\" font-famil
+000134e0: 793a 5c27 2e53 4620 4e53 2054 6578 745c  y:\'.SF NS Text\
+000134f0: 273b 2066 6f6e 742d 7369 7a65 3a31 3370  '; font-size:13p
+00013500: 743b 5c22 3e20 3d20 283c 2f73 7061 6e3e  t;\"> = (</span>
+00013510: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
+00013520: 6f6e 742d 6661 6d69 6c79 3a5c 272e 5346  ont-family:\'.SF
+00013530: 204e 5320 5465 7874 5c27 3b20 666f 6e74   NS Text\'; font
+00013540: 2d73 697a 653a 3133 7074 3b20 666f 6e74  -size:13pt; font
+00013550: 2d73 7479 6c65 3a69 7461 6c69 633b 2063  -style:italic; c
+00013560: 6f6c 6f72 3a23 3030 3030 3030 3b5c 223e  olor:#000000;\">
+00013570: 613c 2f73 7061 6e3e 3c73 7061 6e20 7374  a</span><span st
+00013580: 796c 653d 5c22 2066 6f6e 742d 6661 6d69  yle=\" font-fami
+00013590: 6c79 3a5c 272e 5346 204e 5320 5465 7874  ly:\'.SF NS Text
+000135a0: 5c27 3b20 666f 6e74 2d73 697a 653a 3133  \'; font-size:13
+000135b0: 7074 3b20 666f 6e74 2d73 7479 6c65 3a69  pt; font-style:i
+000135c0: 7461 6c69 633b 2063 6f6c 6f72 3a23 3030  talic; color:#00
+000135d0: 3030 3030 3b20 7665 7274 6963 616c 2d61  0000; vertical-a
+000135e0: 6c69 676e 3a73 7562 3b5c 223e 6e3c 2f73  lign:sub;\">n</s
+000135f0: 7061 6e3e 3c73 7061 6e20 7374 796c 653d  pan><span style=
+00013600: 5c22 2066 6f6e 742d 6661 6d69 6c79 3a5c  \" font-family:\
+00013610: 272e 5346 204e 5320 5465 7874 5c27 3b20  '.SF NS Text\'; 
+00013620: 666f 6e74 2d73 697a 653a 3133 7074 3b20  font-size:13pt; 
+00013630: 636f 6c6f 723a 2330 3030 3030 303b 5c22  color:#000000;\"
+00013640: 3e2c 5e32 202b 203c 2f73 7061 6e3e 3c73  >,^2 + </span><s
+00013650: 7061 6e20 7374 796c 653d 5c22 2066 6f6e  pan style=\" fon
+00013660: 742d 6661 6d69 6c79 3a5c 272e 5346 204e  t-family:\'.SF N
+00013670: 5320 5465 7874 5c27 3b20 666f 6e74 2d73  S Text\'; font-s
+00013680: 697a 653a 3133 7074 3b20 666f 6e74 2d73  ize:13pt; font-s
+00013690: 7479 6c65 3a69 7461 6c69 633b 2063 6f6c  tyle:italic; col
+000136a0: 6f72 3a23 3030 3030 3030 3b5c 223e 623c  or:#000000;\">b<
+000136b0: 2f73 7061 6e3e 3c73 7061 6e20 7374 796c  /span><span styl
+000136c0: 653d 5c22 2066 6f6e 742d 6661 6d69 6c79  e=\" font-family
+000136d0: 3a5c 272e 5346 204e 5320 5465 7874 5c27  :\'.SF NS Text\'
+000136e0: 3b20 666f 6e74 2d73 697a 653a 3133 7074  ; font-size:13pt
+000136f0: 3b20 666f 6e74 2d73 7479 6c65 3a69 7461  ; font-style:ita
+00013700: 6c69 633b 2063 6f6c 6f72 3a23 3030 3030  lic; color:#0000
+00013710: 3030 3b20 7665 7274 6963 616c 2d61 6c69  00; vertical-ali
+00013720: 676e 3a73 7562 3b5c 223e 6e3c 2f73 7061  gn:sub;\">n</spa
+00013730: 6e3e 3c73 7061 6e20 7374 796c 653d 5c22  n><span style=\"
+00013740: 2066 6f6e 742d 6661 6d69 6c79 3a5c 272e   font-family:\'.
+00013750: 5346 204e 5320 5465 7874 5c27 3b20 666f  SF NS Text\'; fo
+00013760: 6e74 2d73 697a 653a 3133 7074 3b20 636f  nt-size:13pt; co
+00013770: 6c6f 723a 2330 3030 3030 303b 5c22 3e5e  lor:#000000;\">^
+00013780: 3220 2b20 3c2f 7370 616e 3e3c 7370 616e  2 + </span><span
+00013790: 2073 7479 6c65 3d5c 2220 666f 6e74 2d66   style=\" font-f
+000137a0: 616d 696c 793a 5c27 2e53 4620 4e53 2054  amily:\'.SF NS T
+000137b0: 6578 745c 273b 2066 6f6e 742d 7369 7a65  ext\'; font-size
+000137c0: 3a31 3370 743b 2066 6f6e 742d 7374 796c  :13pt; font-styl
+000137d0: 653a 6974 616c 6963 3b20 636f 6c6f 723a  e:italic; color:
+000137e0: 2330 3030 3030 303b 5c22 3e63 3c2f 7370  #000000;\">c</sp
+000137f0: 616e 3e3c 7370 616e 2073 7479 6c65 3d5c  an><span style=\
+00013800: 2220 666f 6e74 2d66 616d 696c 793a 5c27  " font-family:\'
+00013810: 2e53 4620 4e53 2054 6578 745c 273b 2066  .SF NS Text\'; f
+00013820: 6f6e 742d 7369 7a65 3a31 3370 743b 2066  ont-size:13pt; f
+00013830: 6f6e 742d 7374 796c 653a 6974 616c 6963  ont-style:italic
+00013840: 3b20 636f 6c6f 723a 2330 3030 3030 303b  ; color:#000000;
+00013850: 2076 6572 7469 6361 6c2d 616c 6967 6e3a   vertical-align:
+00013860: 7375 623b 5c22 3e6e 3c2f 7370 616e 3e3c  sub;\">n</span><
+00013870: 7370 616e 2073 7479 6c65 3d5c 2220 666f  span style=\" fo
+00013880: 6e74 2d66 616d 696c 793a 5c27 2e53 4620  nt-family:\'.SF 
+00013890: 4e53 2054 6578 745c 273b 2066 6f6e 742d  NS Text\'; font-
+000138a0: 7369 7a65 3a31 3370 743b 2063 6f6c 6f72  size:13pt; color
+000138b0: 3a23 3030 3030 3030 3b5c 223e 5e32 202b  :#000000;\">^2 +
+000138c0: 203c 2f73 7061 6e3e 3c73 7061 6e20 7374   </span><span st
+000138d0: 796c 653d 5c22 2066 6f6e 742d 6661 6d69  yle=\" font-fami
+000138e0: 6c79 3a5c 272e 5346 204e 5320 5465 7874  ly:\'.SF NS Text
+000138f0: 5c27 3b20 666f 6e74 2d73 697a 653a 3133  \'; font-size:13
+00013900: 7074 3b20 666f 6e74 2d73 7479 6c65 3a69  pt; font-style:i
+00013910: 7461 6c69 633b 2063 6f6c 6f72 3a23 3030  talic; color:#00
+00013920: 3030 3030 3b5c 223e 643c 2f73 7061 6e3e  0000;\">d</span>
+00013930: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
+00013940: 6f6e 742d 6661 6d69 6c79 3a5c 272e 5346  ont-family:\'.SF
+00013950: 204e 5320 5465 7874 5c27 3b20 666f 6e74   NS Text\'; font
+00013960: 2d73 697a 653a 3133 7074 3b20 666f 6e74  -size:13pt; font
+00013970: 2d73 7479 6c65 3a69 7461 6c69 633b 2063  -style:italic; c
+00013980: 6f6c 6f72 3a23 3030 3030 3030 3b20 7665  olor:#000000; ve
+00013990: 7274 6963 616c 2d61 6c69 676e 3a73 7562  rtical-align:sub
+000139a0: 3b5c 223e 6e3c 2f73 7061 6e3e 3c73 7061  ;\">n</span><spa
+000139b0: 6e20 7374 796c 653d 5c22 2066 6f6e 742d  n style=\" font-
+000139c0: 6661 6d69 6c79 3a5c 272e 5346 204e 5320  family:\'.SF NS 
+000139d0: 5465 7874 5c27 3b20 666f 6e74 2d73 697a  Text\'; font-siz
+000139e0: 653a 3133 7074 3b20 636f 6c6f 723a 2330  e:13pt; color:#0
+000139f0: 3030 3030 303b 5c22 3e5e 323c 2f73 7061  00000;\">^2</spa
+00013a00: 6e3e 3c73 7061 6e20 7374 796c 653d 5c22  n><span style=\"
+00013a10: 2066 6f6e 742d 6661 6d69 6c79 3a5c 272e   font-family:\'.
+00013a20: 5346 204e 5320 5465 7874 5c27 3b20 666f  SF NS Text\'; fo
+00013a30: 6e74 2d73 697a 653a 3133 7074 3b5c 223e  nt-size:13pt;\">
+00013a40: 292f 322e 2054 6869 7320 7061 7261 6d65  )/2. This parame
+00013a50: 7465 7273 206e 6f20 6c6f 6e67 6572 2068  ters no longer h
+00013a60: 6176 6520 7468 6520 696e 666f 726d 6174  ave the informat
+00013a70: 696f 6e20 6f66 2070 6861 7365 2073 6869  ion of phase shi
+00013a80: 6674 206f 6620 6561 6368 2068 6172 6d6f  ft of each harmo
+00013a90: 6e69 6373 2065 6c6c 6970 7365 7320 616e  nics ellipses an
+00013aa0: 6420 736f 6c76 6520 7468 6520 2671 756f  d solve the &quo
+00013ab0: 743b 6d69 7272 6f72 2d73 796d 6d65 7472  t;mirror-symmetr
+00013ac0: 6963 2070 726f 7065 7274 7926 7175 6f74  ic property&quot
+00013ad0: 3b20 7072 6f62 6c65 6d73 2e3c 2f73 7061  ; problems.</spa
+00013ae0: 6e3e 3c2f 703e 5c6e 220a 223c 7020 7374  n></p>\n"."<p st
+00013af0: 796c 653d 5c22 2d71 742d 7061 7261 6772  yle=\"-qt-paragr
+00013b00: 6170 682d 7479 7065 3a65 6d70 7479 3b20  aph-type:empty; 
+00013b10: 6d61 7267 696e 2d74 6f70 3a30 7078 3b20  margin-top:0px; 
+00013b20: 6d61 7267 696e 2d62 6f74 746f 6d3a 3070  margin-bottom:0p
+00013b30: 783b 206d 6172 6769 6e2d 6c65 6674 3a30  x; margin-left:0
+00013b40: 7078 3b20 6d61 7267 696e 2d72 6967 6874  px; margin-right
+00013b50: 3a30 7078 3b20 2d71 742d 626c 6f63 6b2d  :0px; -qt-block-
+00013b60: 696e 6465 6e74 3a30 3b20 7465 7874 2d69  indent:0; text-i
+00013b70: 6e64 656e 743a 3070 783b 2066 6f6e 742d  ndent:0px; font-
+00013b80: 6661 6d69 6c79 3a5c 272e 5346 204e 5320  family:\'.SF NS 
+00013b90: 5465 7874 5c27 3b20 666f 6e74 2d73 697a  Text\'; font-siz
+00013ba0: 653a 3133 7074 3b5c 223e 3c62 7220 2f3e  e:13pt;\"><br />
+00013bb0: 3c2f 703e 5c6e 220a 223c 7020 7374 796c  </p>\n"."<p styl
+00013bc0: 653d 5c22 206d 6172 6769 6e2d 746f 703a  e=\" margin-top:
+00013bd0: 3070 783b 206d 6172 6769 6e2d 626f 7474  0px; margin-bott
+00013be0: 6f6d 3a30 7078 3b20 6d61 7267 696e 2d6c  om:0px; margin-l
+00013bf0: 6566 743a 3070 783b 206d 6172 6769 6e2d  eft:0px; margin-
+00013c00: 7269 6768 743a 3070 783b 202d 7174 2d62  right:0px; -qt-b
+00013c10: 6c6f 636b 2d69 6e64 656e 743a 303b 2074  lock-indent:0; t
+00013c20: 6578 742d 696e 6465 6e74 3a30 7078 3b5c  ext-indent:0px;\
+00013c30: 223e 3c73 7061 6e20 7374 796c 653d 5c22  "><span style=\"
+00013c40: 2066 6f6e 742d 6661 6d69 6c79 3a5c 272e   font-family:\'.
+00013c50: 5346 204e 5320 5465 7874 5c27 3b20 666f  SF NS Text\'; fo
+00013c60: 6e74 2d73 697a 653a 3133 7074 3b20 666f  nt-size:13pt; fo
+00013c70: 6e74 2d77 6569 6768 743a 3630 303b 5c22  nt-weight:600;\"
+00013c80: 3e41 6d70 6c69 7475 6465 2062 6173 6564  >Amplitude based
+00013c90: 3c2f 7370 616e 3e3c 2f70 3e5c 6e22 0a22  </span></p>\n"."
+00013ca0: 3c70 2073 7479 6c65 3d5c 2220 6d61 7267  <p style=\" marg
+00013cb0: 696e 2d74 6f70 3a30 7078 3b20 6d61 7267  in-top:0px; marg
+00013cc0: 696e 2d62 6f74 746f 6d3a 3070 783b 206d  in-bottom:0px; m
+00013cd0: 6172 6769 6e2d 6c65 6674 3a30 7078 3b20  argin-left:0px; 
+00013ce0: 6d61 7267 696e 2d72 6967 6874 3a30 7078  margin-right:0px
+00013cf0: 3b20 2d71 742d 626c 6f63 6b2d 696e 6465  ; -qt-block-inde
+00013d00: 6e74 3a30 3b20 7465 7874 2d69 6e64 656e  nt:0; text-inden
+00013d10: 743a 3070 783b 5c22 3e3c 7370 616e 2073  t:0px;\"><span s
+00013d20: 7479 6c65 3d5c 2220 666f 6e74 2d66 616d  tyle=\" font-fam
+00013d30: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+00013d40: 745c 273b 2066 6f6e 742d 7369 7a65 3a31  t\'; font-size:1
+00013d50: 3370 743b 5c22 3e49 7420 636f 7272 6573  3pt;\">It corres
+00013d60: 706f 6e64 7320 746f 2074 6865 2061 6d70  ponds to the amp
+00013d70: 6c69 7475 6465 206f 6620 7468 6520 6561  litude of the ea
+00013d80: 6368 2068 6172 6d6f 6e69 6373 2069 6e20  ch harmonics in 
+00013d90: 7465 726d 7320 6f66 2058 2d63 6f6f 7264  terms of X-coord
+00013da0: 696e 6174 6520 616e 6420 592d 636f 6f72  inate and Y-coor
+00013db0: 6469 6e61 7465 2072 6573 7065 6374 6976  dinate respectiv
+00013dc0: 656c 792e 3c2f 7370 616e 3e3c 2f70 3e5c  ely.</span></p>\
+00013dd0: 6e22 0a22 3c70 2073 7479 6c65 3d5c 2220  n"."<p style=\" 
+00013de0: 6d61 7267 696e 2d74 6f70 3a30 7078 3b20  margin-top:0px; 
+00013df0: 6d61 7267 696e 2d62 6f74 746f 6d3a 3070  margin-bottom:0p
+00013e00: 783b 206d 6172 6769 6e2d 6c65 6674 3a30  x; margin-left:0
+00013e10: 7078 3b20 6d61 7267 696e 2d72 6967 6874  px; margin-right
+00013e20: 3a30 7078 3b20 2d71 742d 626c 6f63 6b2d  :0px; -qt-block-
+00013e30: 696e 6465 6e74 3a30 3b20 7465 7874 2d69  indent:0; text-i
+00013e40: 6e64 656e 743a 3070 783b 5c22 3e3c 7370  ndent:0px;\"><sp
+00013e50: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
+00013e60: 2d66 616d 696c 793a 5c27 2e53 4620 4e53  -family:\'.SF NS
+00013e70: 2054 6578 745c 273b 2066 6f6e 742d 7369   Text\'; font-si
+00013e80: 7a65 3a31 3370 743b 5c22 3e49 7420 6973  ze:13pt;\">It is
+00013e90: 2067 6976 656e 2062 7920 583c 2f73 7061   given by X</spa
+00013ea0: 6e3e 3c73 7061 6e20 7374 796c 653d 5c22  n><span style=\"
+00013eb0: 2066 6f6e 742d 6661 6d69 6c79 3a5c 272e   font-family:\'.
+00013ec0: 5346 204e 5320 5465 7874 5c27 3b20 666f  SF NS Text\'; fo
+00013ed0: 6e74 2d73 697a 653a 3133 7074 3b20 7665  nt-size:13pt; ve
+00013ee0: 7274 6963 616c 2d61 6c69 676e 3a73 7562  rtical-align:sub
+00013ef0: 3b5c 223e 616d 3c2f 7370 616e 3e3c 7370  ;\">am</span><sp
+00013f00: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
+00013f10: 2d66 616d 696c 793a 5c27 2e53 4620 4e53  -family:\'.SF NS
+00013f20: 2054 6578 745c 273b 2066 6f6e 742d 7369   Text\'; font-si
+00013f30: 7a65 3a31 3370 743b 5c22 3e20 3d20 283c  ze:13pt;\"> = (<
+00013f40: 2f73 7061 6e3e 3c73 7061 6e20 7374 796c  /span><span styl
+00013f50: 653d 5c22 2066 6f6e 742d 6661 6d69 6c79  e=\" font-family
+00013f60: 3a5c 272e 5346 204e 5320 5465 7874 5c27  :\'.SF NS Text\'
+00013f70: 3b20 666f 6e74 2d73 697a 653a 3133 7074  ; font-size:13pt
+00013f80: 3b20 666f 6e74 2d73 7479 6c65 3a69 7461  ; font-style:ita
+00013f90: 6c69 633b 2063 6f6c 6f72 3a23 3030 3030  lic; color:#0000
+00013fa0: 3030 3b5c 223e 613c 2f73 7061 6e3e 3c73  00;\">a</span><s
+00013fb0: 7061 6e20 7374 796c 653d 5c22 2066 6f6e  pan style=\" fon
+00013fc0: 742d 6661 6d69 6c79 3a5c 272e 5346 204e  t-family:\'.SF N
+00013fd0: 5320 5465 7874 5c27 3b20 666f 6e74 2d73  S Text\'; font-s
+00013fe0: 697a 653a 3133 7074 3b20 666f 6e74 2d73  ize:13pt; font-s
+00013ff0: 7479 6c65 3a69 7461 6c69 633b 2063 6f6c  tyle:italic; col
+00014000: 6f72 3a23 3030 3030 3030 3b20 7665 7274  or:#000000; vert
+00014010: 6963 616c 2d61 6c69 676e 3a73 7562 3b5c  ical-align:sub;\
+00014020: 223e 6e3c 2f73 7061 6e3e 3c73 7061 6e20  ">n</span><span 
+00014030: 7374 796c 653d 5c22 2066 6f6e 742d 6661  style=\" font-fa
+00014040: 6d69 6c79 3a5c 272e 5346 204e 5320 5465  mily:\'.SF NS Te
+00014050: 7874 5c27 3b20 666f 6e74 2d73 697a 653a  xt\'; font-size:
+00014060: 3133 7074 3b20 636f 6c6f 723a 2330 3030  13pt; color:#000
+00014070: 3030 303b 5c22 3e2c 5e32 202b 203c 2f73  000;\">,^2 + </s
+00014080: 7061 6e3e 3c73 7061 6e20 7374 796c 653d  pan><span style=
+00014090: 5c22 2066 6f6e 742d 6661 6d69 6c79 3a5c  \" font-family:\
+000140a0: 272e 5346 204e 5320 5465 7874 5c27 3b20  '.SF NS Text\'; 
+000140b0: 666f 6e74 2d73 697a 653a 3133 7074 3b20  font-size:13pt; 
+000140c0: 666f 6e74 2d73 7479 6c65 3a69 7461 6c69  font-style:itali
+000140d0: 633b 2063 6f6c 6f72 3a23 3030 3030 3030  c; color:#000000
+000140e0: 3b5c 223e 623c 2f73 7061 6e3e 3c73 7061  ;\">b</span><spa
+000140f0: 6e20 7374 796c 653d 5c22 2066 6f6e 742d  n style=\" font-
+00014100: 6661 6d69 6c79 3a5c 272e 5346 204e 5320  family:\'.SF NS 
+00014110: 5465 7874 5c27 3b20 666f 6e74 2d73 697a  Text\'; font-siz
+00014120: 653a 3133 7074 3b20 666f 6e74 2d73 7479  e:13pt; font-sty
+00014130: 6c65 3a69 7461 6c69 633b 2063 6f6c 6f72  le:italic; color
+00014140: 3a23 3030 3030 3030 3b20 7665 7274 6963  :#000000; vertic
+00014150: 616c 2d61 6c69 676e 3a73 7562 3b5c 223e  al-align:sub;\">
+00014160: 6e3c 2f73 7061 6e3e 3c73 7061 6e20 7374  n</span><span st
+00014170: 796c 653d 5c22 2066 6f6e 742d 6661 6d69  yle=\" font-fami
+00014180: 6c79 3a5c 272e 5346 204e 5320 5465 7874  ly:\'.SF NS Text
+00014190: 5c27 3b20 666f 6e74 2d73 697a 653a 3133  \'; font-size:13
+000141a0: 7074 3b20 636f 6c6f 723a 2330 3030 3030  pt; color:#00000
+000141b0: 303b 5c22 3e5e 3229 202f 3220 2c20 3c2f  0;\">^2) /2 , </
+000141c0: 7370 616e 3e3c 7370 616e 2073 7479 6c65  span><span style
+000141d0: 3d5c 2220 666f 6e74 2d66 616d 696c 793a  =\" font-family:
+000141e0: 5c27 2e53 4620 4e53 2054 6578 745c 273b  \'.SF NS Text\';
+000141f0: 2066 6f6e 742d 7369 7a65 3a31 3370 743b   font-size:13pt;
+00014200: 5c22 3e20 593c 2f73 7061 6e3e 3c73 7061  \"> Y</span><spa
+00014210: 6e20 7374 796c 653d 5c22 2066 6f6e 742d  n style=\" font-
+00014220: 6661 6d69 6c79 3a5c 272e 5346 204e 5320  family:\'.SF NS 
+00014230: 5465 7874 5c27 3b20 666f 6e74 2d73 697a  Text\'; font-siz
+00014240: 653a 3133 7074 3b20 7665 7274 6963 616c  e:13pt; vertical
+00014250: 2d61 6c69 676e 3a73 7562 3b5c 223e 616d  -align:sub;\">am
+00014260: 3c2f 7370 616e 3e3c 7370 616e 2073 7479  </span><span sty
+00014270: 6c65 3d5c 2220 666f 6e74 2d66 616d 696c  le=\" font-famil
+00014280: 793a 5c27 2e53 4620 4e53 2054 6578 745c  y:\'.SF NS Text\
+00014290: 273b 2066 6f6e 742d 7369 7a65 3a31 3370  '; font-size:13p
+000142a0: 743b 5c22 3e20 3d20 2863 3c2f 7370 616e  t;\"> = (c</span
+000142b0: 3e3c 7370 616e 2073 7479 6c65 3d5c 2220  ><span style=\" 
+000142c0: 666f 6e74 2d66 616d 696c 793a 5c27 2e53  font-family:\'.S
+000142d0: 4620 4e53 2054 6578 745c 273b 2066 6f6e  F NS Text\'; fon
+000142e0: 742d 7369 7a65 3a31 3370 743b 2066 6f6e  t-size:13pt; fon
+000142f0: 742d 7374 796c 653a 6974 616c 6963 3b20  t-style:italic; 
+00014300: 636f 6c6f 723a 2330 3030 3030 303b 2076  color:#000000; v
+00014310: 6572 7469 6361 6c2d 616c 6967 6e3a 7375  ertical-align:su
+00014320: 623b 5c22 3e6e 3c2f 7370 616e 3e3c 7370  b;\">n</span><sp
+00014330: 616e 2073 7479 6c65 3d5c 2220 666f 6e74  an style=\" font
+00014340: 2d66 616d 696c 793a 5c27 2e53 4620 4e53  -family:\'.SF NS
+00014350: 2054 6578 745c 273b 2066 6f6e 742d 7369   Text\'; font-si
+00014360: 7a65 3a31 3370 743b 2063 6f6c 6f72 3a23  ze:13pt; color:#
+00014370: 3030 3030 3030 3b5c 223e 2c5e 3220 2b20  000000;\">,^2 + 
+00014380: 643c 2f73 7061 6e3e 3c73 7061 6e20 7374  d</span><span st
+00014390: 796c 653d 5c22 2066 6f6e 742d 6661 6d69  yle=\" font-fami
+000143a0: 6c79 3a5c 272e 5346 204e 5320 5465 7874  ly:\'.SF NS Text
+000143b0: 5c27 3b20 666f 6e74 2d73 697a 653a 3133  \'; font-size:13
+000143c0: 7074 3b20 666f 6e74 2d73 7479 6c65 3a69  pt; font-style:i
+000143d0: 7461 6c69 633b 2063 6f6c 6f72 3a23 3030  talic; color:#00
+000143e0: 3030 3030 3b20 7665 7274 6963 616c 2d61  0000; vertical-a
+000143f0: 6c69 676e 3a73 7562 3b5c 223e 6e3c 2f73  lign:sub;\">n</s
+00014400: 7061 6e3e 3c73 7061 6e20 7374 796c 653d  pan><span style=
+00014410: 5c22 2066 6f6e 742d 6661 6d69 6c79 3a5c  \" font-family:\
+00014420: 272e 5346 204e 5320 5465 7874 5c27 3b20  '.SF NS Text\'; 
+00014430: 666f 6e74 2d73 697a 653a 3133 7074 3b20  font-size:13pt; 
+00014440: 636f 6c6f 723a 2330 3030 3030 303b 5c22  color:#000000;\"
+00014450: 3e5e 3229 202f 323c 2f73 7061 6e3e 3c2f  >^2) /2</span></
+00014460: 703e 5c6e 220a 223c 7020 7374 796c 653d  p>\n"."<p style=
+00014470: 5c22 206d 6172 6769 6e2d 746f 703a 3070  \" margin-top:0p
+00014480: 783b 206d 6172 6769 6e2d 626f 7474 6f6d  x; margin-bottom
+00014490: 3a30 7078 3b20 6d61 7267 696e 2d6c 6566  :0px; margin-lef
+000144a0: 743a 3070 783b 206d 6172 6769 6e2d 7269  t:0px; margin-ri
+000144b0: 6768 743a 3070 783b 202d 7174 2d62 6c6f  ght:0px; -qt-blo
+000144c0: 636b 2d69 6e64 656e 743a 303b 2074 6578  ck-indent:0; tex
+000144d0: 742d 696e 6465 6e74 3a30 7078 3b5c 223e  t-indent:0px;\">
+000144e0: 3c73 7061 6e20 7374 796c 653d 5c22 2066  <span style=\" f
+000144f0: 6f6e 742d 6661 6d69 6c79 3a5c 272e 5346  ont-family:\'.SF
+00014500: 204e 5320 5465 7874 5c27 3b20 666f 6e74   NS Text\'; font
+00014510: 2d73 697a 653a 3133 7074 3b20 636f 6c6f  -size:13pt; colo
+00014520: 723a 2330 3030 3030 303b 5c22 3e54 6869  r:#000000;\">Thi
+00014530: 7320 616c 736f 2073 6f6c 7665 7320 3c2f  s also solves </
+00014540: 7370 616e 3e3c 7370 616e 2073 7479 6c65  span><span style
+00014550: 3d5c 2220 666f 6e74 2d66 616d 696c 793a  =\" font-family:
+00014560: 5c27 2e53 4620 4e53 2054 6578 745c 273b  \'.SF NS Text\';
+00014570: 2066 6f6e 742d 7369 7a65 3a31 3370 743b   font-size:13pt;
+00014580: 5c22 3e26 7175 6f74 3b6d 6972 726f 722d  \">&quot;mirror-
+00014590: 7379 6d6d 6574 7269 6320 7072 6f70 6572  symmetric proper
+000145a0: 7479 2671 756f 743b 2070 726f 626c 656d  ty&quot; problem
+000145b0: 732e 3c2f 7370 616e 3e3c 2f70 3e5c 6e22  s.</span></p>\n"
+000145c0: 0a22 3c70 2073 7479 6c65 3d5c 222d 7174  ."<p style=\"-qt
+000145d0: 2d70 6172 6167 7261 7068 2d74 7970 653a  -paragraph-type:
+000145e0: 656d 7074 793b 206d 6172 6769 6e2d 746f  empty; margin-to
+000145f0: 703a 3070 783b 206d 6172 6769 6e2d 626f  p:0px; margin-bo
+00014600: 7474 6f6d 3a30 7078 3b20 6d61 7267 696e  ttom:0px; margin
+00014610: 2d6c 6566 743a 3070 783b 206d 6172 6769  -left:0px; margi
+00014620: 6e2d 7269 6768 743a 3070 783b 202d 7174  n-right:0px; -qt
+00014630: 2d62 6c6f 636b 2d69 6e64 656e 743a 303b  -block-indent:0;
+00014640: 2074 6578 742d 696e 6465 6e74 3a30 7078   text-indent:0px
+00014650: 3b20 666f 6e74 2d66 616d 696c 793a 5c27  ; font-family:\'
+00014660: 2e53 4620 4e53 2054 6578 745c 273b 2066  .SF NS Text\'; f
+00014670: 6f6e 742d 7369 7a65 3a31 3370 743b 5c22  ont-size:13pt;\"
+00014680: 3e3c 6272 202f 3e3c 2f70 3e5c 6e22 0a22  ><br /></p>\n"."
+00014690: 3c70 2073 7479 6c65 3d5c 2220 6d61 7267  <p style=\" marg
+000146a0: 696e 2d74 6f70 3a30 7078 3b20 6d61 7267  in-top:0px; marg
+000146b0: 696e 2d62 6f74 746f 6d3a 3070 783b 206d  in-bottom:0px; m
+000146c0: 6172 6769 6e2d 6c65 6674 3a30 7078 3b20  argin-left:0px; 
+000146d0: 6d61 7267 696e 2d72 6967 6874 3a30 7078  margin-right:0px
+000146e0: 3b20 2d71 742d 626c 6f63 6b2d 696e 6465  ; -qt-block-inde
+000146f0: 6e74 3a30 3b20 7465 7874 2d69 6e64 656e  nt:0; text-inden
+00014700: 743a 3070 783b 5c22 3e3c 7370 616e 2073  t:0px;\"><span s
+00014710: 7479 6c65 3d5c 2220 666f 6e74 2d66 616d  tyle=\" font-fam
+00014720: 696c 793a 5c27 2e53 4620 4e53 2054 6578  ily:\'.SF NS Tex
+00014730: 745c 273b 2066 6f6e 742d 7369 7a65 3a31  t\'; font-size:1
+00014740: 3370 743b 5c22 3e23 2d2d 2d2d 2d2d 2d2d  3pt;\">#--------
+00014750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00014760: 2d2d 2d2d 2d2d 2d2d 2d3c 2f73 7061 6e3e  ---------</span>
+00014770: 3c2f 703e 5c6e 220a 223c 7020 7374 796c  </p>\n"."<p styl
+00014780: 653d 5c22 2d71 742d 7061 7261 6772 6170  e=\"-qt-paragrap
+00014790: 682d 7479 7065 3a65 6d70 7479 3b20 6d61  h-type:empty; ma
+000147a0: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
+000147b0: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
+000147c0: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
+000147d0: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
+000147e0: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
+000147f0: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
+00014800: 656e 743a 3070 783b 2066 6f6e 742d 6661  ent:0px; font-fa
+00014810: 6d69 6c79 3a5c 272e 5346 204e 5320 5465  mily:\'.SF NS Te
+00014820: 7874 5c27 3b20 666f 6e74 2d73 697a 653a  xt\'; font-size:
+00014830: 3133 7074 3b5c 223e 3c62 7220 2f3e 3c2f  13pt;\"><br /></
+00014840: 703e 3c2f 626f 6479 3e3c 2f68 746d 6c3e  p></body></html>
+00014850: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00014860: 2e74 6162 5f70 6361 2e73 6574 5461 6254  .tab_pca.setTabT
+00014870: 6578 7428 7365 6c66 2e74 6162 5f70 6361  ext(self.tab_pca
+00014880: 2e69 6e64 6578 4f66 2873 656c 662e 7461  .indexOf(self.ta
+00014890: 625f 3429 2c20 5f74 7261 6e73 6c61 7465  b_4), _translate
+000148a0: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+000148b0: 4c6f 6722 2929 0a20 2020 2020 2020 2073  Log")).        s
+000148c0: 656c 662e 6c61 6265 6c5f 3135 2e73 6574  elf.label_15.set
+000148d0: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+000148e0: 224d 6169 6e57 696e 646f 7722 2c20 2250  "MainWindow", "P
+000148f0: 4341 2073 756d 6d61 7279 2229 290a 2020  CA summary")).  
+00014900: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00014910: 5f31 362e 7365 7454 6578 7428 5f74 7261  _16.setText(_tra
+00014920: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00014930: 6f77 222c 2022 5043 4120 6569 6765 6e20  ow", "PCA eigen 
+00014940: 7665 6374 6f72 2229 290a 2020 2020 2020  vector")).      
+00014950: 2020 7365 6c66 2e74 6162 5f70 6361 2e73    self.tab_pca.s
+00014960: 6574 5461 6254 6578 7428 7365 6c66 2e74  etTabText(self.t
+00014970: 6162 5f70 6361 2e69 6e64 6578 4f66 2873  ab_pca.indexOf(s
+00014980: 656c 662e 746e 5f73 756d 6d61 7279 292c  elf.tn_summary),
+00014990: 205f 7472 616e 736c 6174 6528 224d 6169   _translate("Mai
+000149a0: 6e57 696e 646f 7722 2c20 2253 756d 6d61  nWindow", "Summa
+000149b0: 7279 2229 290a 2020 2020 2020 2020 7365  ry")).        se
+000149c0: 6c66 2e74 6162 5f70 6361 2e73 6574 5461  lf.tab_pca.setTa
+000149d0: 6254 6578 7428 7365 6c66 2e74 6162 5f70  bText(self.tab_p
+000149e0: 6361 2e69 6e64 6578 4f66 2873 656c 662e  ca.indexOf(self.
+000149f0: 746e 5f67 7261 7068 292c 205f 7472 616e  tn_graph), _tran
+00014a00: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00014a10: 7722 2c20 2247 7261 7068 2229 290a 2020  w", "Graph")).  
+00014a20: 2020 2020 2020 7365 6c66 2e74 6162 5769        self.tabWi
+00014a30: 6467 6574 2e73 6574 5461 6254 6578 7428  dget.setTabText(
+00014a40: 7365 6c66 2e74 6162 5769 6467 6574 2e69  self.tabWidget.i
+00014a50: 6e64 6578 4f66 2873 656c 662e 7461 625f  ndexOf(self.tab_
+00014a60: 3229 2c20 5f74 7261 6e73 6c61 7465 2822  2), _translate("
+00014a70: 4d61 696e 5769 6e64 6f77 222c 2022 5043  MainWindow", "PC
+00014a80: 4122 2929 0a20 2020 2020 2020 2073 656c  A")).        sel
+00014a90: 662e 6c61 6265 6c5f 3336 2e73 6574 5465  f.label_36.setTe
+00014aa0: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
+00014ab0: 6169 6e57 696e 646f 7722 2c20 2253 6861  ainWindow", "Sha
+00014ac0: 7065 2052 6563 6f6e 7374 2e22 2929 0a20  pe Reconst.")). 
+00014ad0: 2020 2020 2020 2073 656c 662e 636d 625f         self.cmb_
+00014ae0: 7265 6354 7970 652e 7365 7449 7465 6d54  recType.setItemT
+00014af0: 6578 7428 302c 205f 7472 616e 736c 6174  ext(0, _translat
+00014b00: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00014b10: 2253 756d 6d61 7279 2229 290a 2020 2020  "Summary")).    
+00014b20: 2020 2020 7365 6c66 2e63 6d62 5f72 6563      self.cmb_rec
+00014b30: 5479 7065 2e73 6574 4974 656d 5465 7874  Type.setItemText
+00014b40: 2831 2c20 5f74 7261 6e73 6c61 7465 2822  (1, _translate("
+00014b50: 4d61 696e 5769 6e64 6f77 222c 2022 4465  MainWindow", "De
+00014b60: 7461 696c 2229 290a 2020 2020 2020 2020  tail")).        
+00014b70: 7365 6c66 2e62 7574 746f 6e5f 7361 7665  self.button_save
+00014b80: 5265 636f 6e73 742e 7365 7454 6578 7428  Reconst.setText(
+00014b90: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+00014ba0: 5769 6e64 6f77 222c 2022 5361 7665 2046  Window", "Save F
+00014bb0: 6967 2229 290a 2020 2020 2020 2020 7365  ig")).        se
+00014bc0: 6c66 2e63 6d62 5f73 756d 4465 762e 7365  lf.cmb_sumDev.se
+00014bd0: 7449 7465 6d54 6578 7428 302c 205f 7472  tItemText(0, _tr
+00014be0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00014bf0: 646f 7722 2c20 22c2 b130 2e35 20cf 8322  dow", "..0.5 .."
+00014c00: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00014c10: 636d 625f 7375 6d44 6576 2e73 6574 4974  cmb_sumDev.setIt
+00014c20: 656d 5465 7874 2831 2c20 5f74 7261 6e73  emText(1, _trans
+00014c30: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+00014c40: 222c 2022 c2b1 312e 3020 cf83 2229 290a  ", "..1.0 ..")).
+00014c50: 2020 2020 2020 2020 7365 6c66 2e63 6d62          self.cmb
+00014c60: 5f73 756d 4465 762e 7365 7449 7465 6d54  _sumDev.setItemT
+00014c70: 6578 7428 322c 205f 7472 616e 736c 6174  ext(2, _translat
+00014c80: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00014c90: 22c2 b131 2e35 20cf 8322 2929 0a20 2020  "..1.5 ..")).   
+00014ca0: 2020 2020 2073 656c 662e 636d 625f 7375       self.cmb_su
+00014cb0: 6d44 6576 2e73 6574 4974 656d 5465 7874  mDev.setItemText
+00014cc0: 2833 2c20 5f74 7261 6e73 6c61 7465 2822  (3, _translate("
+00014cd0: 4d61 696e 5769 6e64 6f77 222c 2022 c2b1  MainWindow", "..
+00014ce0: 322e 3020 cf83 2229 290a 2020 2020 2020  2.0 ..")).      
+00014cf0: 2020 7365 6c66 2e63 6d62 5f73 756d 4465    self.cmb_sumDe
+00014d00: 762e 7365 7449 7465 6d54 6578 7428 342c  v.setItemText(4,
+00014d10: 205f 7472 616e 736c 6174 6528 224d 6169   _translate("Mai
+00014d20: 6e57 696e 646f 7722 2c20 22c2 b132 2e35  nWindow", "..2.5
+00014d30: 20cf 8322 2929 0a20 2020 2020 2020 2073   ..")).        s
+00014d40: 656c 662e 636d 625f 7375 6d44 6576 2e73  elf.cmb_sumDev.s
+00014d50: 6574 4974 656d 5465 7874 2835 2c20 5f74  etItemText(5, _t
+00014d60: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+00014d70: 6e64 6f77 222c 2022 c2b1 332e 3020 cf83  ndow", "..3.0 ..
+00014d80: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00014d90: 2e62 7574 746f 6e5f 6765 6e65 7261 7465  .button_generate
+00014da0: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+00014db0: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00014dc0: 2c20 2247 656e 6572 6174 6522 2929 0a20  , "Generate")). 
+00014dd0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+00014de0: 6c5f 3236 2e73 6574 5465 7874 285f 7472  l_26.setText(_tr
+00014df0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00014e00: 646f 7722 2c20 2220 6465 762e 28cf 8329  dow", " dev.(..)
+00014e10: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00014e20: 2e6c 6162 656c 5f32 372e 7365 7454 6578  .label_27.setTex
+00014e30: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+00014e40: 696e 5769 6e64 6f77 222c 2022 4465 7461  inWindow", "Deta
+00014e50: 696c 204d 6f64 6522 2929 0a20 2020 2020  il Mode")).     
+00014e60: 2020 2073 656c 662e 6c61 6265 6c5f 3235     self.label_25
+00014e70: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+00014e80: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00014e90: 2c20 2250 4322 2929 0a20 2020 2020 2020  , "PC")).       
+00014ea0: 2073 656c 662e 6c61 6265 6c5f 3233 2e73   self.label_23.s
+00014eb0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
+00014ec0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00014ed0: 2253 756d 6d61 7279 204d 4f44 4522 2929  "Summary MODE"))
+00014ee0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+00014ef0: 6257 6964 6765 742e 7365 7454 6162 5465  bWidget.setTabTe
+00014f00: 7874 2873 656c 662e 7461 6257 6964 6765  xt(self.tabWidge
+00014f10: 742e 696e 6465 784f 6628 7365 6c66 2e74  t.indexOf(self.t
+00014f20: 6162 5f33 292c 205f 7472 616e 736c 6174  ab_3), _translat
+00014f30: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00014f40: 2253 6861 7065 2229 290a 2020 2020 2020  "Shape")).      
+00014f50: 2020 7365 6c66 2e6d 656e 7574 6573 742e    self.menutest.
+00014f60: 7365 7454 6974 6c65 285f 7472 616e 736c  setTitle(_transl
+00014f70: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00014f80: 2c20 2246 696c 6522 2929 0a20 2020 2020  , "File")).     
+00014f90: 2020 2073 656c 662e 6163 7469 6f6e 4162     self.actionAb
+00014fa0: 6f75 742e 7365 7454 6578 7428 5f74 7261  out.setText(_tra
+00014fb0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00014fc0: 6f77 222c 2022 4162 6f75 7422 2929 0a    ow", "About")).
```

### Comparing `efshape-0.0.5/efshape.egg-info/PKG-INFO` & `efshape-0.1.0/efshape.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: efshape
-Version: 0.0.5
+Version: 0.1.0
 Summary: Package Dependency: Validates package requirements
 Home-page: https://github.com/SojiroFukuda/efshape
 Author: SojiroFukuda
 Author-email: S.Fukuda-2018@hull.ac.uk
 Maintainer: SojiroFukuda
 Maintainer-email: S.Fukuda-2018@hull.ac.uk
 License: SojiroFukuda
-Description: # ef-shape
-        
-        efshape is a python package for shape analysis of 2D image.
-        The method is based on the combination between 'Elliptic Fourier Analysis (EFA)' and 'Principal Component Analysis (PCA)' and called EF-PCA method.
-        The basic idea is to convert the 2D closed contour into a numeric dataset by EFA and then, using multivariate analysis (PCA) , detect the major shape variation of the dataset. 
-        EFA enables you to describe the complicated shape complehensively as a number of dataset called elliptic Fourire descriptors.
-        One of the merits of this method is that you can easily reconstruct the shape from the descriptors, which also make it easier to interpret the shape variation of detected principal component axes.
-        
-        In this package, you can choose three different types of EF-PCA methods: one of which, EFD-based EF-PCA, is suitable for directional object like bio-forms and the others, Amplitude- and FPS-based EF-PCA, are suitable for non-directional object such as sedimentary grain.
-        This package provides you both CUI- and GUI-based package.
-        
-        # About license
-        © 2019 Sojiro Fukuda All Rightss Reserved.
-        Free to modify and redistribute by your own responsibility.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
+
+# ef-shape
+
+efshape is a python package for shape analysis of 2D image.
+The method is based on the combination between 'Elliptic Fourier Analysis (EFA)' and 'Principal Component Analysis (PCA)' and called EF-PCA method.
+The basic idea is to convert the 2D closed contour into a numeric dataset by EFA and then, using multivariate analysis (PCA) , detect the major shape variation of the dataset. 
+EFA enables you to describe the complicated shape complehensively as a number of dataset called elliptic Fourire descriptors.
+One of the merits of this method is that you can easily reconstruct the shape from the descriptors, which also make it easier to interpret the shape variation of detected principal component axes.
+
+In this package, you can choose three different types of EF-PCA methods: one of which, EFD-based EF-PCA, is suitable for directional object like bio-forms and the others, Amplitude- and FPS-based EF-PCA, are suitable for non-directional object such as sedimentary grain.
+This package provides you both CUI- and GUI-based package.
+
+# About license
+© 2019 Sojiro Fukuda All Rightss Reserved.
+Free to modify and redistribute by your own responsibility.
+
```

### Comparing `efshape-0.0.5/setup.py` & `efshape-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # version
 here = os.path.dirname(os.path.abspath(__file__))
 version = next((line.split('=')[1].strip().replace("'", '')
                 for line in open(os.path.join(here,
                                               'efshape',
                                               '__init__.py'))
-                if line.startswith('__version__ = ')),'0.0.5')
+                if line.startswith('__version__ = ')),'0.1.0')
 
 
 setup(
     name="efshape",
     version=version,
     url='https://github.com/SojiroFukuda/efshape',
     author='SojiroFukuda',
@@ -31,15 +31,15 @@
     maintainer='SojiroFukuda',
     maintainer_email='S.Fukuda-2018@hull.ac.uk',
     description='Package Dependency: Validates package requirements',
     long_description=readme,
     packages=find_packages(),
     install_requires=[
 #         "sys >= 3.7.3",
-        "PyQt5 >= 5.7.0",
+        "PyQt6 >= 6.4.2",
         "numpy >= 1.16.0",
         "pandas >= 0.24.0",
         "matplotlib >= 3.0.0",
         "Pathlib2 >= 2.3.0",
         "scipy >= 1.2.0",
         "cmocean >= 2.0",
         "seaborn >= 0.9.0",
```


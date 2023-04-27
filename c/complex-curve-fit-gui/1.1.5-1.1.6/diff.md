# Comparing `tmp/complex_curve_fit_gui-1.1.5.tar.gz` & `tmp/complex_curve_fit_gui-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex_curve_fit_gui-1.1.5.tar", last modified: Mon Apr 24 04:57:58 2023, max compression
+gzip compressed data, was "complex_curve_fit_gui-1.1.6.tar", last modified: Thu Apr 27 09:44:30 2023, max compression
```

## Comparing `complex_curve_fit_gui-1.1.5.tar` & `complex_curve_fit_gui-1.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 04:57:58.840525 complex_curve_fit_gui-1.1.5/
--rw-r--r--   0 kojo       (501) staff       (20)       44 2023-04-24 04:46:49.000000 complex_curve_fit_gui-1.1.5/MANIFEST.in
--rw-r--r--   0 kojo       (501) staff       (20)     9285 2023-04-24 04:57:58.840608 complex_curve_fit_gui-1.1.5/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)     8826 2023-04-24 04:31:29.000000 complex_curve_fit_gui-1.1.5/README.md
--rw-rw-rw-   0 kojo       (501) staff       (20)       79 2023-04-24 04:57:58.840939 complex_curve_fit_gui-1.1.5/setup.cfg
--rw-rw-rw-   0 kojo       (501) staff       (20)     1299 2023-04-24 04:40:32.000000 complex_curve_fit_gui-1.1.5/setup.py
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 04:57:58.836330 complex_curve_fit_gui-1.1.5/src/
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 04:57:58.839593 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/
--rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-04-24 04:32:54.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/__init__.py
--rw-rw-rw-   0 kojo       (501) staff       (20)     7183 2023-04-24 04:32:54.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/_curvefitgui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    15529 2023-04-24 04:54:11.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/_gui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)     1539 2023-04-24 04:52:01.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/_settings.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    16588 2023-04-24 04:54:10.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/_tools.py
--rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-04-24 04:57:53.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/_version.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    30979 2023-04-24 04:32:54.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/_widgets.py
--rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-04-24 04:32:54.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/config.txt
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 04:57:58.840400 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui.egg-info/
--rw-r--r--   0 kojo       (501) staff       (20)     9285 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui.egg-info/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)      582 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui.egg-info/SOURCES.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui.egg-info/dependency_links.txt
--rw-r--r--   0 kojo       (501) staff       (20)       22 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui.egg-info/top_level.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui.egg-info/zip-safe
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-27 09:44:30.190835 complex_curve_fit_gui-1.1.6/
+-rw-r--r--   0 kojo       (501) staff       (20)       44 2023-04-24 04:46:49.000000 complex_curve_fit_gui-1.1.6/MANIFEST.in
+-rw-r--r--   0 kojo       (501) staff       (20)     9399 2023-04-27 09:44:30.190926 complex_curve_fit_gui-1.1.6/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)     8940 2023-04-27 04:46:22.000000 complex_curve_fit_gui-1.1.6/README.md
+-rw-rw-rw-   0 kojo       (501) staff       (20)       79 2023-04-27 09:44:30.191215 complex_curve_fit_gui-1.1.6/setup.cfg
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1299 2023-04-24 04:40:32.000000 complex_curve_fit_gui-1.1.6/setup.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-27 09:44:30.188503 complex_curve_fit_gui-1.1.6/src/
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-27 09:44:30.189996 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/
+-rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/__init__.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)     7155 2023-04-27 04:39:20.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_curvefitgui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    15964 2023-04-27 09:32:17.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_gui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1529 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_settings.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    16635 2023-04-27 08:22:23.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_tools.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-04-27 09:42:11.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_version.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    33637 2023-04-27 09:31:48.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_widgets.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/config.txt
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-27 09:44:30.190562 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/
+-rw-r--r--   0 kojo       (501) staff       (20)     9399 2023-04-27 09:44:30.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)      582 2023-04-27 09:44:30.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-27 09:44:30.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 kojo       (501) staff       (20)       22 2023-04-27 09:44:30.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/top_level.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/zip-safe
```

### Comparing `complex_curve_fit_gui-1.1.5/PKG-INFO` & `complex_curve_fit_gui-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex_curve_fit_gui
-Version: 1.1.5
+Version: 1.1.6
 Summary: GUI for lmfit using matplotlib
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,19 +22,19 @@
     pip install complex-curve-fit-gui
 
 The GUI is supported on Python 3.7 and above.  
 **Note**: only `complex-curve-fit-gui` is installed without any required dependencies. Depending on if you are using pip or conda to manage your environment you should manually install the following additional packages:  
 
 - Using `pip`:
 
-      pip install numpy scipy matplotlib PyQt5
+      pip install numpy scipy matplotlib PyQt5 lmfit sympy
 
 - Using `conda` (required for M1 Mac):    
 
-      conda install numpy scipy matplotlib qtpy pyqt
+      conda install numpy scipy matplotlib qtpy pyqt && conda install -c conda-forge lmfit
 
 ### Getting Started
 1. If on MacOS M1 a conda environment will be needed
 2. import the gui:
        `from curvefitgui import curve_fit_gui`
 3. define x and y data as 1 dimensional numpy arrays of equal length
        `xdata = np.array([1, 2, 3, 4, 5])`
@@ -89,14 +89,17 @@
        2. Array containing the standard error (+/-)
        3. lmfit Model_Result object pertaining to the best fit, reference here: https://lmfit.github.io/lmfit-py/model.html#the-modelresult-class
 
 ### User defined functions
  - To make a user defined function create a function and pass to curve_fit_gui as f. For example: 
  ```python
        def linear(x, a, b, c): 
+              '''
+              y = a * x + b
+              '''
               return y = a * x + b
 
        curve_fit_gui(linear, xdata, ydata)
 ```
 
 ### User defined complex functions
  - When defining a complex function add the **complex=True** keyword argument and use `1j` in the equation. For example for Euler's equation e^(ix)cs:
```

### Comparing `complex_curve_fit_gui-1.1.5/README.md` & `complex_curve_fit_gui-1.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     pip install complex-curve-fit-gui
 
 The GUI is supported on Python 3.7 and above.  
 **Note**: only `complex-curve-fit-gui` is installed without any required dependencies. Depending on if you are using pip or conda to manage your environment you should manually install the following additional packages:  
 
 - Using `pip`:
 
-      pip install numpy scipy matplotlib PyQt5
+      pip install numpy scipy matplotlib PyQt5 lmfit sympy
 
 - Using `conda` (required for M1 Mac):    
 
-      conda install numpy scipy matplotlib qtpy pyqt
+      conda install numpy scipy matplotlib qtpy pyqt && conda install -c conda-forge lmfit
 
 ### Getting Started
 1. If on MacOS M1 a conda environment will be needed
 2. import the gui:
        `from curvefitgui import curve_fit_gui`
 3. define x and y data as 1 dimensional numpy arrays of equal length
        `xdata = np.array([1, 2, 3, 4, 5])`
@@ -75,14 +75,17 @@
        2. Array containing the standard error (+/-)
        3. lmfit Model_Result object pertaining to the best fit, reference here: https://lmfit.github.io/lmfit-py/model.html#the-modelresult-class
 
 ### User defined functions
  - To make a user defined function create a function and pass to curve_fit_gui as f. For example: 
  ```python
        def linear(x, a, b, c): 
+              '''
+              y = a * x + b
+              '''
               return y = a * x + b
 
        curve_fit_gui(linear, xdata, ydata)
 ```
 
 ### User defined complex functions
  - When defining a complex function add the **complex=True** keyword argument and use `1j` in the equation. For example for Euler's equation e^(ix)cs:
```

### Comparing `complex_curve_fit_gui-1.1.5/setup.py` & `complex_curve_fit_gui-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/_curvefitgui.py` & `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_curvefitgui.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         ydata,
         xerr,
         yerr,
         p0,
         xlabel,
         ylabel,
         absolute_sigma,
-        jac,
         showgui,
         **kwargs,
     )
     return res
 
 
 def curve_fit_gui(
@@ -200,15 +199,14 @@
         ydata,
         xerr,
         yerr,
         p0,
         xlabel,
         ylabel,
         absolute_sigma,
-        jac,
         **kwargs,
     )
     return res
 
 
 def __main__():
     # example of use and testing"
```

### Comparing `complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/_gui.py` & `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # import the required packages
 import random
 import sys
 import warnings
 from inspect import signature
 
+
 import numpy as np
 from PyQt5 import QtCore, QtWidgets
 from scipy.optimize import OptimizeWarning
 
 from ._settings import settings
 from ._tools import Fitter, value_to_string
 from ._version import __version__ as CFGversion
@@ -150,26 +151,38 @@
         try:
             self.modelview.read_values()
         except ValueError:
             self.showdialog(
                 "Not a valid input initial parameter values", "critical"
             )
             return None
-        # print(self.plotwidget.selected_curve)
+        # print("selected", self.plotwidget.selected_curve)
+        # print("here", self.plotwidget.canvas.ax1.get_lines())
+
         try:
-            selected_line = next(
-                x
-                for x in self.plotwidget.canvas.ax1.get_lines()
-                if x.get_label() == self.plotwidget.selected_curve
-            )
-            # print(selected_line)
-            (current_x, current_y) = selected_line.get_data()
-            self.fitter.change_data(current_x, current_y, None, None)
-            # print("after change", self.fitter.data)
-        except:
+            if self.plotwidget.selected_curve is not None:
+                selected_line = next(
+                    x
+                    for x in self.plotwidget.canvas.ax1.get_lines()
+                    if x.get_label() == self.plotwidget.selected_curve
+                )
+                # print("sel", selected_line)
+
+                if not self.plotwidget.canvas.fitter.is_complex:
+                    (current_x, current_y) = selected_line.get_data()
+
+                else:
+                    (current_x, current_y) = self.plotwidget.data_map[
+                        selected_line.get_label()
+                    ]
+                self.fitter.change_data(current_x, current_y, None, None)
+                # print("after change", self.fitter.data)
+
+        except Exception as e:
+            # print("exp", e)
             self.showdialog("Can't find plot", "critical")
         # update fitrange
         self.plotwidget.canvas.get_range()
 
         # show warning on xerror data
         if (self.fitter.data.xe is not None) and self.xerrorwarning:
             self.showdialog("The error in x is ignored in the fit!", "warning")
@@ -248,25 +261,15 @@
             self.fitcontrollayout.addWidget(widget)
 
         self.fitcontrolframe
 
 
 # add is_complex parameter
 def execute_gui(
-    f,
-    xdata,
-    ydata,
-    xerr,
-    yerr,
-    p0,
-    xlabel,
-    ylabel,
-    absolute_sigma,
-    jac,
-    **kwargs
+    f, xdata, ydata, xerr, yerr, p0, xlabel, ylabel, absolute_sigma, **kwargs
 ):
     """
     helper function that executes the GUI with an instance of the fitter class
     """
 
     if not QtWidgets.QApplication.instance():
         app = QtWidgets.QApplication([])
@@ -282,15 +285,14 @@
             f,
             xdata,
             ydata,
             xerr,
             yerr,
             p0,
             absolute_sigma,
-            jac,
             is_complex,
             **kwargs,
         )
         return afitter.fit()
 
     class CustomDialog(QtWidgets.QDialog):
         """
@@ -393,18 +395,22 @@
             On ok from starting pop up this function sets the fit function
             """
             self.is_complex = (
                 True if "i" in self.combobox.currentText() else self.is_complex
             )
             self.func = self.function_map[self.combobox.currentText()]
 
-    dlg = CustomDialog()
-    dlg.exec_()
     if f is None:
+        dlg = CustomDialog()
+        dlg.exec_()
         f = dlg.func
+        # Here so that complex bool passes through to widgets
+        if dlg.is_complex:
+            kwargs["complex"] = True
+            is_complex = True
 
     """
     !!!
     From this line up to sfitter = Fitter(...) will not be needed in final product this
     is just for testing
     !!!
     """
@@ -437,28 +443,24 @@
         y_noise = test_yerr * rng.normal(size=xdata.size)
         ydata = y + y_noise
         ydata = np.asarray(ydata)
 
     """
     gonna have to add sigma to this and other places
     """
-    # Here so that complex bool passes through to widgets
-    if dlg.is_complex:
-        kwargs["complex"] = True
 
     afitter = Fitter(
         f,
         xdata,
         ydata,
         xerr,
         yerr,
         p0,
         absolute_sigma,
-        jac,
-        dlg.is_complex,
+        is_complex,
         **kwargs,
     )
 
     # print("original", afitter.data)
     MyApplication = MainWindow(afitter, xlabel, ylabel, **kwargs)
     MyApplication.show()
     app.exec_()
```

### Comparing `complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/_settings.py` & `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib import resources as _resources
 import configparser
 
 
 _config = configparser.ConfigParser()
-with _resources.path("complex_curve_fit_gui", "config.txt") as _path:
+with _resources.path("curvefitgui", "config.txt") as _path:
     _config.read(str(_path))
 
 settings = {}
 
 # general
 settings['MODEL_NUMPOINTS'] = int(_config['general']['numpoints'])
 settings['SIGNIFICANT_DIGITS'] = int(_config['general']['significant_digits'])
```

### Comparing `complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/_tools.py` & `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,14 @@
         func,
         xdata,
         ydata,
         xerr,
         yerr,
         p0,
         absolute_sigma,
-        jac,
         is_complex,
         **kwargs,
     ):
 
         self.kwargs = kwargs
         self.data = self._init_data(xdata, ydata, xerr, yerr)
         self.model = self._init_model(func, p0, absolute_sigma)
@@ -116,14 +115,15 @@
         self.mean_squared_error = None
         self.fitreport = {}
         self.is_complex = is_complex
         self.method = "leastsq"
         if "method" in kwargs:
             self.method = kwargs["method"]
         self.orig_model = copy.deepcopy(self.model)
+        self.orig_complex = copy.deepcopy(is_complex)
 
     def _init_data(self, x, y, xe, ye):
 
         # validate data
         for var in [x, y]:
             if type(var) is not np.ndarray:
                 raise Exception("data should have type numpy array")
@@ -269,17 +269,17 @@
         if check is True(default) only returns values if a valid fit is performed.
         """
 
         if not self.fit_is_valid and check:
             return None
         if not self.model_result:
             return None
-        # return self.data.y - self.model.evaluate(self.data.x)
+        return self.data.y - self.model.evaluate(self.data.x)
         # lmfit
-        return self.model_result.residual
+        # return self.model_result.residual
 
     def _degrees_of_freedom(self):
         return int(self.data.get_numfitpoints() - self.model.get_numfitpars())
 
     def _create_report(self):
         def pars_to_dict():
             parsdict = {
@@ -379,15 +379,15 @@
     result = model.lmfit_model.fit(
         pargs[1],
         params,
         x=pargs[0],
         calc_covar=True,
         nan_policy="omit",
         method=method,
-        max_nfev=500,
+        max_nfev=100000000,
     )
 
     popt = np.array(list(result.best_values.values()))
     # print("cov values", result.covar)
     cov = np.array(result.covar)
     # print("cov values after arrayed", cov)
```

### Comparing `complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/_widgets.py` & `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Callable
 import warnings
 from collections import defaultdict
 import io
 import string
 from sympy.solvers import solve
 from sympy import symbols
+import re
 
 warnings.filterwarnings("ignore")
 
 
 import matplotlib.patches as patches
 import numpy as np
 from lmfit import Model
@@ -130,25 +131,32 @@
     )  # emits when plot is updated
 
     def __init__(self, fitter, xlabel, ylabel, **kwargs):
         QtWidgets.QWidget.__init__(self)
         self.setLayout(QtWidgets.QVBoxLayout())
         self.canvas = PlotCanvas(fitter, xlabel, ylabel, **kwargs)
         self.toolbar = NavigationToolbar(self.canvas, self)
-        self.selected_curve = self.canvas.ax1.get_lines()[0].get_label()
+        self.selected_curve = None
+        self.initial_complex_curve = (
+            self.canvas.ax1.get_lines()[0].get_label()
+            if not self.canvas.fitter.is_complex
+            else self.canvas.ax1.get_lines()[1].get_label()
+        )  # This data is an edge case of selected curve that needs to be saved
+        # print("init select", self.selected_curve)
         self.selected_model = None
         self.input_func = None
+        self.data_map = {}
 
         self.hideRes = QtWidgets.QAction("TOGGLE RESIDUAL")
         self.hideRes.setIconText("TOGGLE RESIDUAL")
         self.hideRes.setFont(QtGui.QFont("Times", 12, QtGui.QFont.Bold))
         self.hideRes.triggered.connect(self.toggle_residual_visibility)
 
         self.switchData = QtWidgets.QAction("Switch Data")
-        self.switchData.setIconText("SWITCH DATA")
+        self.switchData.setIconText("SELECT DATA")
         self.switchData.setFont(QtGui.QFont("Times", 12, QtGui.QFont.Bold))
         self.switchData.triggered.connect(self.switch_data)
 
         self.ACshowselector = QtWidgets.QAction("Activate/Clear RangeSelector")
         self.ACshowselector.setIconText("RANGE SELECTOR")
         self.ACshowselector.setFont(QtGui.QFont("Times", 12, QtGui.QFont.Bold))
         self.ACshowselector.triggered.connect(self._toggle_showselector)
@@ -290,15 +298,36 @@
 
         # button.clicked.connect(dialog.close)
 
         # dialog.setLayout(layout)
         # dialog.exec_()
 
     def switch_data(self):
+        def save_complex_data():
+            """
+            before switching curve add complex data to a map of label to x data and y data
+            Since complex plots y real and imag, xdata is lost in matplotlib
+            """
+
+            if self.canvas.fitter.is_complex:
+
+                if self.selected_curve:
+                    self.data_map[self.selected_curve] = (
+                        self.canvas.fitter.data.x,
+                        self.canvas.fitter.data.y,
+                    )
+                else:
+                    self.data_map[self.initial_complex_curve] = (
+                        self.canvas.fitter.data.x,
+                        self.canvas.fitter.data.y,
+                    )
+
         def get_selected_curve():
+            save_complex_data()
+            # print(self.data_map[self.selected_curve])
             self.selected_curve = self.combobox.currentText()
 
         def get_selected_model():
             self.selected_model = self.model_combobox.currentText()
 
         # print(self.canvas.ax1.get_lines()[1].get_label())
         self.dialog = QtWidgets.QDialog()
@@ -312,45 +341,51 @@
         self.button.clicked.connect(get_selected_curve)
         self.button.clicked.connect(get_selected_model)
         self.button.clicked.connect(self.re_init_model)
         # self.button.clicked.connect(self.create_callable)
         self.button.clicked.connect(self.dialog.close)
 
         for item in self.canvas.ax1.get_lines():
-            if item.get_label() != "fitted_curve":
+            if not re.match(r"fitted curve.*?", item.get_label()):
                 self.combobox.addItem(item.get_label())
+            # else:
+            #     # print(item)
 
-        for item in self.canvas.ax1.get_lines():
-            if item.get_label() == "fitted_curve":
-                self.combobox.addItem(item.get_label())
+        # for item in self.canvas.ax1.get_lines():
+        #     if item.get_label() == "fitted_curve":
+        #         self.combobox.addItem(item.get_label())
 
         self.model_combobox.addItem(
             self.canvas.fitter.orig_model.func.__name__
+            if self.canvas.fitter.orig_model.func.__name__
+            else "custom_user_function"
         )
         for item in self.function_map:
             self.model_combobox.addItem(item)
 
         self.layout.addWidget(self.combobox)
         self.layout.addWidget(self.model_combobox)
         # self.layout.addWidget(self.user_input)
         self.layout.addWidget(self.button)
 
         self.dialog.setLayout(self.layout)
         self.dialog.exec_()
 
     def re_init_model(self, event):
-        new_model = None
+        new_model = self.canvas.fitter.orig_model.func
+        self.canvas.fitter.is_complex = self.canvas.fitter.orig_complex
         if self.selected_model != self.canvas.fitter.orig_model.func.__name__:
             new_model = self.function_map[self.selected_model]
-        if "i" in self.selected_model:
-            self.canvas.fitter.is_complex = True
-        else:
-            self.canvas.fitter.is_complex = False
+            if "i" in self.selected_model:
+                self.canvas.fitter.is_complex = True
+            else:
+                self.canvas.fitter.is_complex = False
         self.re_init.emit(new_model, None, None)
 
+    # Not fully implemented supposed to allow custom user input during execution
     def custom_user_function(self, *args):
         n = len(args) - 1
         symbol_str = "x" + ":" + str(n)
         return solve(self.input_func, symbols(symbol_str))
 
     def create_callable(self):
         if len(self.user_input.text()) > 2:
@@ -589,19 +624,19 @@
         self.result_box.set_visible(True)
 
     def disable_results_box(self):
         self.result_box.set_visible(False)
 
     def toggle_rangeselector(self):
         if self.range_selector is None:
-            if self.complex:
+            if self.fitter.is_complex:
                 self.range_selector = RangeSelector(
                     self.ax1,
-                    np.min(self.fitter.data.y),
-                    np.max(self.fitter.data.y),
+                    np.min(self.fitter.data.y.real),
+                    np.max(self.fitter.data.y.real),
                 )
             else:
                 self.range_selector = RangeSelector(
                     self.ax1,
                     np.min(self.fitter.data.x),
                     np.max(self.fitter.data.x),
                 )
@@ -661,29 +696,53 @@
             #     self.data_line.remove()
             if self.fitted_line:
                 self.fitted_line.remove()
             if self.initial_guess_line:
                 self.initial_guess_line.remove()
                 self.initial_guess_line = None
 
-            self.ax2.lines.clear()
+            # self.ax2.lines.clear()
             # if self.complex_residuals:
             #     self.complex_residuals.cla()
 
             # (self.data_line,) = self.plot_complex(self.data.y, **self.kwargs)
 
             (self.fitted_line,) = self.plot_complex(
                 fit_s21, "--k", **self.fitline_kwargs
             )
-            self.complex_residuals = self.fitter.model_result.plot_residuals(
-                ax=self.ax2,
-                datafmt=".-k",
-                parse_complex="abs",
-                data_kws={"label": "residual"},
-            )
+            """
+            Lmfit had wierd residuals fro complex values
+            """
+            # self.complex_residuals = self.fitter.model_result.plot_residuals(
+            #     ax=self.ax2,
+            #     datafmt=".-k",
+            #     parse_complex="abs",
+            #     data_kws={"label": "residual"},
+            # )
+            if self.residuals is not None:
+                # if the zero residual line is not yet created, do so
+                if self.zero_res is None:
+                    self.ax2.axhline(y=0, linestyle="--", color="black")
+
+                # sort data if required
+                if settings["SORT_RESIDUALS"]:
+                    order = np.argsort(self.fitter.data.y.real)
+                else:
+                    order = np.arange(0, len(self.fitter.data.y.real))
+
+                data_copy = np.array([])
+                for i in range(len(self.fitter.data.y)):
+                    if self.fitter.data.mask[i] == True:
+                        data_copy = np.append(
+                            data_copy, [self.fitter.data.y.real[i]]
+                        )
+                self.residual_line.set_data(
+                    data_copy[order[: len(self.residuals)]],
+                    self.residuals.real[order[: len(self.residuals)]],
+                )
             self.ax1.legend()
         else:
             if self.residuals is not None:
                 # if the zero residual line is not yet created, do so
                 if self.zero_res is None:
                     self.ax2.axhline(y=0, linestyle="--", color="black")
```

### Comparing `complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui/config.txt` & `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/config.txt`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui.egg-info/PKG-INFO` & `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-curve-fit-gui
-Version: 1.1.5
+Version: 1.1.6
 Summary: GUI for lmfit using matplotlib
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,19 +22,19 @@
     pip install complex-curve-fit-gui
 
 The GUI is supported on Python 3.7 and above.  
 **Note**: only `complex-curve-fit-gui` is installed without any required dependencies. Depending on if you are using pip or conda to manage your environment you should manually install the following additional packages:  
 
 - Using `pip`:
 
-      pip install numpy scipy matplotlib PyQt5
+      pip install numpy scipy matplotlib PyQt5 lmfit sympy
 
 - Using `conda` (required for M1 Mac):    
 
-      conda install numpy scipy matplotlib qtpy pyqt
+      conda install numpy scipy matplotlib qtpy pyqt && conda install -c conda-forge lmfit
 
 ### Getting Started
 1. If on MacOS M1 a conda environment will be needed
 2. import the gui:
        `from curvefitgui import curve_fit_gui`
 3. define x and y data as 1 dimensional numpy arrays of equal length
        `xdata = np.array([1, 2, 3, 4, 5])`
@@ -89,14 +89,17 @@
        2. Array containing the standard error (+/-)
        3. lmfit Model_Result object pertaining to the best fit, reference here: https://lmfit.github.io/lmfit-py/model.html#the-modelresult-class
 
 ### User defined functions
  - To make a user defined function create a function and pass to curve_fit_gui as f. For example: 
  ```python
        def linear(x, a, b, c): 
+              '''
+              y = a * x + b
+              '''
               return y = a * x + b
 
        curve_fit_gui(linear, xdata, ydata)
 ```
 
 ### User defined complex functions
  - When defining a complex function add the **complex=True** keyword argument and use `1j` in the equation. For example for Euler's equation e^(ix)cs:
```

### Comparing `complex_curve_fit_gui-1.1.5/src/complex_curve_fit_gui.egg-info/SOURCES.txt` & `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*


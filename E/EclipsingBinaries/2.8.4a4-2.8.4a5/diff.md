# Comparing `tmp/EclipsingBinaries-2.8.4a4.tar.gz` & `tmp/EclipsingBinaries-2.8.4a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-2.8.4a4.tar", last modified: Tue Apr 25 17:55:22 2023, max compression
+gzip compressed data, was "EclipsingBinaries-2.8.4a5.tar", last modified: Thu Apr 27 19:28:33 2023, max compression
```

## Comparing `EclipsingBinaries-2.8.4a4.tar` & `EclipsingBinaries-2.8.4a5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:55:22.139181 EclipsingBinaries-2.8.4a4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:55:22.135181 EclipsingBinaries-2.8.4a4/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-04-25 17:55:02.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-04-25 17:55:02.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19634 2023-04-25 17:55:02.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-04-25 17:55:02.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 17:55:02.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-04-25 17:55:02.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    28069 2023-04-25 17:55:02.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:55:22.139181 EclipsingBinaries-2.8.4a4/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:55:22.139181 EclipsingBinaries-2.8.4a4/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:55:22.139181 EclipsingBinaries-2.8.4a4/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-25 17:55:22.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-25 17:55:22.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:55:22.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-25 17:55:22.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 17:55:22.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 17:55:22.000000 EclipsingBinaries-2.8.4a4/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-25 17:55:22.139181 EclipsingBinaries-2.8.4a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 17:55:22.139181 EclipsingBinaries-2.8.4a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-25 17:55:07.000000 EclipsingBinaries-2.8.4a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:28:33.035633 EclipsingBinaries-2.8.4a5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:28:33.031633 EclipsingBinaries-2.8.4a5/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-04-27 19:28:10.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-04-27 19:28:10.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-04-27 19:28:10.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-04-27 19:28:10.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 19:28:10.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-04-27 19:28:10.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29452 2023-04-27 19:28:10.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:28:33.031633 EclipsingBinaries-2.8.4a5/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:28:33.035633 EclipsingBinaries-2.8.4a5/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:28:33.031633 EclipsingBinaries-2.8.4a5/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-27 19:28:33.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-27 19:28:33.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:28:33.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 19:28:33.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-27 19:28:33.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 19:28:33.000000 EclipsingBinaries-2.8.4a5/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-27 19:28:33.035633 EclipsingBinaries-2.8.4a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:28:33.035633 EclipsingBinaries-2.8.4a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-27 19:28:15.000000 EclipsingBinaries-2.8.4a5/setup.py
```

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/OC_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Author: Kyle Koeller
 Created: 12/19/2022
-Last Edited: 04/02/2023
+Last Edited: 04/27/2023
 
 This calculates O-C values and produces an O-C plot.
 """
 
-from math import sqrt
+from math import sqrt, floor
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.polynomial import Polynomial
 import statsmodels.formula.api as smf
 import seaborn as sns
 from numba import jit
@@ -299,15 +299,15 @@
     """
     if T0 == 0:
         T0 = m
         T0_err = err
     # get the exact E value
     E_act = (m - T0) / p
     # estimate for the primary or secondary eclipse by rounding to the nearest 0.5
-    e = round(E_act * 2) / 2
+    e = floor(E_act * 2) / 2
     # caluclate the calculated ToM and find the O-C value
     T_calc = T0 + (e * p)
     OC = "%.5f" % (m - T_calc)
 
     # determine the error of the O-C
     OC_err = "%.5f" % sqrt(T0_err ** 2 + err ** 2)
```

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/apass.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/color_light_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Sep 17 12:45:40 2020
 Created on Tue Feb 16 19:29:16 2021
 @author: Alec Neal
 
-Last Edited: 03/16/2022
+Last Edited: 04/27/2022
 Editor: Kyle Koeller
 """
 
 # import vseq  # testing purposes
 from . import vseq_updated as vseq
 import numpy as np
 import matplotlib.pyplot as plt
@@ -132,17 +132,19 @@
     aVphase, aV_mag, aB_interp_mag = vseq.plot.aliasing2(Vphase, V_mag, B_interp_mag)[:3:]
     aBphase, aB_mag = vseq.plot.aliasing2(Bphase, B_mag, B_mag)[:2:]
     aB_minus_V = vseq.plot.aliasing2(Vphase, B_minus_V, B_minus_V)[1]
     B_V = [B_minus_V, BV_mean, BV_err, aB_minus_V]
     B = [aBphase, aB_mag, aB_interp_mag]
     V = [aVphase, aV_mag]
 
-    print('T =', vseq.Flower.T.Teff(quadcolor - (0.641 / 3.1)))
+    # print('T =', vseq.Flower.T.Teff(quadcolor - (0.641 / 3.1)))
 
-    return B_V, B, V, quadcolor, colorerr
+    temp = vseq.Flower.T.Teff(quadcolor - (0.641 / 3.1))
+
+    return B_V, B, V, quadcolor, colorerr, temp
 
 
 # use this function below
 def color_plot(Bfile, Vfile, Epoch, period, max_tol=0.03, lower_lim=0.05, Rfile='', FTinterp=True,
                save=False, outName='noname_color.png', fs=12):
     """
     This is a function version of the GUI and produces the same values but without the plotting aspect
@@ -312,15 +314,15 @@
     root = Tk()
     root.option_add('*Font', '12')
     root.title('CLC-gui v0.2.1')
     # root.geometry('1200x800')
     # disp=3
     # T=Text(root,height=disp,width=25)
     # T.grid(row=0,column=1)
-    Intro = Label(root, text='Color Light Curve - gui\nversion 0.2.1 (2/19/21)\nby Alec Neal\n')
+    Intro = Label(root, text='Color Light Curve - gui\nversion 0.2.2 (2/19/21)\nby Alec Neal\n')
     Intro.grid(row=0, column=0, columnspan=2)
     # Intro.config(font=('Arial',12))
     # T.insert(END,'Hello world!')
 
     Label(root, text=autowrap('Program to determine light curve colors. Mouse over the fields for more information.',
                               width=50) + '\n').grid(row=1, column=0, columnspan=2)
     entries = [['B file'],
@@ -413,33 +415,38 @@
         ' If this field is left blank, it will make only a B-V plot. If R is entered,'
         ' the three light curves will be shown along with interpolated B-V, V-R colors.'))
     # ====================
     getit = lambda entr: entr[1].get()
     temp = Label(root, text='')
     BVL = Label(root, text='')
     BVL.grid(row=len(entries) + 6, column=0, columnspan=2)
+    BVL_temp = Label(root, text='')
+    BVL_temp.grid(row=len(entries) + 7, column=0, columnspan=2)
     VRL = Label(root, text='')
-    VRL.grid(row=len(entries) + 5, column=0, columnspan=2)
+    VRL_temp = Label(root, text='')
+    VRL.grid(row=len(entries) + 4, column=0, columnspan=2)
+    VRL_temp.grid(row=len(entries) + 5, column=0, columnspan=2)
     # B2=gui.Field(root,'B file',2,0)
     fs = 14
 
     def call_colorplot2():
         """
         Calls to create the color plot after clicking the plot button.
 
-        This creates plots for both the B-V and the V-R
+        This creates plots for both the B-V and the V-R2458403.58763
         """
         B_V = subtract_LC(Bfile=getit(B), Vfile=getit(V), Epoch=float(getit(Epoch)), period=float(getit(Period)),
                           max_tol=float(getit(MaxT)), lower_lim=float(getit(LL)))
         # B_V=subtract_LC(Bfile=B,Vfile=V,Epoch=Epoch,period=Period,
         # max_tol=MaxT,lower_lim=LL)
         Bphase, Bmag, B_interp_mag = B_V[1][:3:]
         Vphase, Vmag = B_V[2][:2:]
         aB_minus_V = B_V[0][3]
         quadcolor, colorerr = B_V[3:5:]
+        eff_temp = B_V[5]
         if getit(R) == '':
             """
             Checks whether the user has entered a R band text file
             """
             fig = Figure(figsize=(7, 7.8), dpi=90, tight_layout=True)
             # canvas = FigureCanvasTkAgg(fig, master=root)
             # canvas.destroy()
@@ -466,27 +473,29 @@
             mag.text(ytickpad, (max(Vmag) + min(Vmag)) / 2, 'V', rotation=90, fontsize=fs * 1.2)
             # bv.set_xlabel('$\Phi$',fontsize=fs*1.2)
             bv.set_xlabel('$\Phi$', fontsize=fs * 1.2, usetex=False)
             bv.set_ylabel(r'$\rm B-V$', fontsize=fs * 1.2)
             # quadcolor,colorerr=B_V[3:5:]
             # bv.axhline(quadcolor,color='gray',linewidth=None)
             VRL.config(text='', bg=None, relief=None, padx=0, pady=0, borderwidth=0)
+            VRL_temp.config(text='', bg=None, relief=None, padx=0, pady=0, borderwidth=0)
             # canvas.draw()
             # canvas.get_tk_widget().grid(row=0,column=3,rowspan=100,padx=5)
             # if getit(Save) == 'True':
             # plt.savefig(getit(Out),bbox_inches='tight')
         else:
             V_R = subtract_LC(Bfile=getit(V), Vfile=getit(R), Epoch=float(getit(Epoch)), period=float(getit(Period)),
                               max_tol=float(getit(MaxT)), lower_lim=float(getit(LL)))
             # V_R=subtract_LC(Bfile=V,Vfile=R,Epoch=Epoch,period=Period,
             # max_tol=MaxT,lower_lim=LL)
             VRc, VRerr = V_R[3:5:]
             Rphase, Rmag = V_R[2][:2:]
             V_interp_mag = V_R[1][2]
             aV_minus_R = V_R[0][3]
+            VR_temp = V_R[5]
             fig = Figure(figsize=(7, 9), dpi=90, tight_layout=True)
             # canvas = FigureCanvasTkAgg(fig, master=root)
             # canvas.destroy()
             axs = vseq.plot.multiplot(height_ratios=[8, 3, 3], fig=fig)
             mag = axs[0]
             bv = axs[2]
             vr = axs[1]
@@ -517,14 +526,17 @@
             mag.text(ytickpad, (max(Rmag) + min(Rmag)) / 2, r'$\rm R_C$', rotation=90, fontsize=fs * 1.2)
             bv.set_ylabel(r'$\rm B-V$', fontsize=fs * 1.2)
             vr.set_ylabel(r'$\rm V-R_C$', fontsize=fs * 1.2)
             bv.set_xlabel(r'$\Phi$', fontsize=fs * 1.2)
 
             VRL.config(text='(V-R) = ' + str(round(VRc, 6)) + ' +/- ' + str(round(VRerr, 6)), bg='white',
                        relief='solid', borderwidth=1, padx=5, pady=5, font=('None', 14))
+            VRL_temp.config(text='T_{\\rm eff, V-R} = ' + str(VR_temp), bg='white', relief='solid', borderwidth=1,
+                            padx=5,
+                            pady=5, font=('None', 14))
             show_color = False
             if show_color:
                 # vr.annotate(r'$V-R_{\rm C}='+str(round(VRc,4))+'\pm'+str(round(VRerr,4))+'$',xy=(0.25,vr.get_ylim()[-1]),ha='center')
                 # vr.plot([''])
                 # vr.annotate(r'$V-R_{\rm C}='+str(round(VRc,4))+'\pm'+str(round(VRerr,4))+'$',xy=(0.25,VRc),ha='center',va='center',bbox=dict(facecolor='white', edgecolor='gray',boxstyle='round',pad=0.1),fontsize=11)
 
                 vr.annotate(r'$V-R_{\rm C}=' + str(round(VRc, 4)) + '\pm' + str(round(VRerr, 4)) + '$',
@@ -548,23 +560,33 @@
                 # vr.annotate('>',xy=(vr.get_xlim()[0],VRc),va='center',ha='center',color='magenta')
                 # vr.annotate('<',xy=(vr.get_xlim()[-1],VRc),va='center',ha='center',color='magenta')
             # canvas.draw()
             # canvas.get_tk_widget().grid(row=0,column=3,rowspan=100,padx=5)
             # if getit(Save) == 'True':
             # plt.savefig(getit(Out),bbox_inches='tight')
 
-        temp.config(text='(B-V) = ' + str(round(quadcolor, 6)) + ' +/- ' + str(round(colorerr, 6)), bg='white',
-                   relief='solid', borderwidth=1, padx=5, pady=5, font=('None', 14))
+        # temp.config(text='(B-V) = ' + str(round(quadcolor, 6)) + ' +/- ' + str(round(colorerr, 6)), bg='white',
+        #            relief='solid', borderwidth=1, padx=5, pady=5, font=('None', 14))
 
         BVL.config(text='(B-V) = ' + str(round(quadcolor, 6)) + ' +/- ' + str(round(colorerr, 6)), bg='white',
                    relief='solid', borderwidth=1, padx=5, pady=5, font=('None', 14))
+        BVL_temp.config(text='T_{\\rm eff, B-V} = ' + str(eff_temp), bg='white', relief='solid', borderwidth=1, padx=5,
+                        pady=5, font=('None', 14))
         CreateToolTip(BVL, text=autowrap(
             'These values are calculated using an average of the (X-Y) values within phase 0.075 of quadrature (phase = +/- 0.25).'
             ' The given error is the standard\ndeviation of these values.', 50))
 
+        CreateToolTip(VRL, text=autowrap(
+            'These values are calculated using an average of the (X-Y) values within phase 0.075 of quadrature (phase = +/- 0.25).'
+            ' The given error is the standard\ndeviation of these values.', 50))
+
+        CreateToolTip(VRL_temp, text=autowrap('This value has not been tested and should not be used without verifying'
+                                              ' by another method. Use the B-V temperature as the true effective '
+                                              'temperature', 50))
+
         # =============================
         canvas = FigureCanvasTkAgg(fig, master=root)  # A tk.DrawingArea.
         # canvas.delete('all')
         canvas.draw()
         canvas.get_tk_widget().grid(row=0, column=3, rowspan=100, padx=5)
         # if getit(Save) == 'True':
         # fig.savefig(getit(Out),bbox_inches='tight')
@@ -583,11 +605,11 @@
 
     root.mainloop()
 
 
 # =======================
 
 # If you want to use the gui
-# color_gui(False)
+color_gui(False)
 
 # or just the function itself
 # color_plot('Bfile','Vfile',Epoch,period)
```

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/find_min.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/gaia.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/menu.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/tess_data_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Look up the TESS data and download that data onto a local drive.
 Author: Kyle Koeller
 Created: 2/19/2022
-Last Updated: 04/20/2023
+Last Updated: 04/26/2023
 """
 
 # import required packages
 import astroquery.exceptions
 from astroquery.mast import Tesscut
 from .tesscut import main as tCut
 # from tesscut import main as tCut  # testing purposes
 from os.path import exists
 import pandas as pd
 
 from astropy import units as u
+import pkg_resources
 
 
 def main():
     """
     This function allows the user to enter a TIC ID to be entered, and it also makes sure that number is valid or exists.
     This program will also list off the sector data to be downloaded for cross-referencing if needed.
     :return: Downloaded pixel data in the form of .fits files to be extracted later
@@ -33,15 +34,16 @@
             break
         except astroquery.exceptions.ResolverError:
             print("\nThe TIC number you entered is invalid or there is no data for this given system.\n")
 
     if system_name.lower() == "close":
         exit()
 
-    dc = pd.read_csv("tess_ccd_info.txt", header=None, sep="\t", skiprows=[0])
+    filename = pkg_resources.resource_filename(__name__, 'tess_ccd_info.txt')
+    dc = pd.read_csv(filename, header=None, sep="\t", skiprows=[0])
 
     gain = dc[6]  # gain for the individual camera/ccd
     tess_camera = dc[0]  # camera number
     tess_ccd = dc[1]  # ccd number
     # slice = dc[2]  # could be used in the future
 
     sector_camera = []
```

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/tests/test_OC_plot.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a4
+Version: 2.8.4a5
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-2.8.4a4/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-2.8.4a5/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/LICENSE` & `EclipsingBinaries-2.8.4a5/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/PKG-INFO` & `EclipsingBinaries-2.8.4a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a4
+Version: 2.8.4a5
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-2.8.4a4/README.md` & `EclipsingBinaries-2.8.4a5/README.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a4/setup.py` & `EclipsingBinaries-2.8.4a5/setup.py`

 * *Files identical despite different names*


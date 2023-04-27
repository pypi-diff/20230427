# Comparing `tmp/scikeo-0.2.0.tar.gz` & `tmp/scikeo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikeo-0.2.0.tar", last modified: Tue Mar 28 22:13:53 2023, max compression
+gzip compressed data, was "scikeo-0.2.1.tar", last modified: Thu Apr 27 17:06:07 2023, max compression
```

## Comparing `scikeo-0.2.0.tar` & `scikeo-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 22:13:53.520529 scikeo-0.2.0/
--rw-rw-rw-   0        0        0      613 2023-03-17 15:59:10.000000 scikeo-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      130 2023-03-17 15:59:10.000000 scikeo-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8739 2023-03-28 22:13:53.520529 scikeo-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7982 2023-03-17 15:59:10.000000 scikeo-0.2.0/README.md
--rw-rw-rw-   0        0        0       62 2023-03-17 15:59:10.000000 scikeo-0.2.0/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-03-28 22:13:53.480080 scikeo-0.2.0/scikeo/
--rw-rw-rw-   0        0        0      143 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/__init__.py
--rw-rw-rw-   0        0        0    10900 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/atmosCorr.py
--rw-rw-rw-   0        0        0     5794 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/calkmeans.py
--rw-rw-rw-   0        0        0    19966 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/calmla.py
--rw-rw-rw-   0        0        0     9131 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/deeplearning.py
--rw-rw-rw-   0        0        0     6113 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/fusionrs.py
--rw-rw-rw-   0        0        0     6668 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/linearTrend.py
--rw-rw-rw-   0        0        0    25713 2023-03-23 01:18:16.000000 scikeo-0.2.0/scikeo/mla.py
--rw-rw-rw-   0        0        0     5043 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/pca.py
--rw-rw-rw-   0        0        0     5789 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/plot.py
--rw-rw-rw-   0        0        0     9903 2023-03-28 22:10:59.000000 scikeo-0.2.0/scikeo/process.py
--rw-rw-rw-   0        0        0     1871 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/rkmeans.py
--rw-rw-rw-   0        0        0     3819 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/sma.py
--rw-rw-rw-   0        0        0     5235 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/tassCap.py
--rw-rw-rw-   0        0        0     2068 2023-03-17 15:59:10.000000 scikeo-0.2.0/scikeo/writeRaster.py
-drwxrwxrwx   0        0        0        0 2023-03-28 22:13:53.519519 scikeo-0.2.0/scikeo.egg-info/
--rw-rw-rw-   0        0        0     8739 2023-03-28 22:13:53.000000 scikeo-0.2.0/scikeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-03-28 22:13:53.000000 scikeo-0.2.0/scikeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       56 2023-03-28 22:13:53.000000 scikeo-0.2.0/scikeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-20 19:51:08.000000 scikeo-0.2.0/scikeo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-03-28 22:13:53.000000 scikeo-0.2.0/scikeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-28 22:13:53.000000 scikeo-0.2.0/scikeo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      414 2023-03-28 22:13:53.522385 scikeo-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1755 2023-03-28 22:11:42.000000 scikeo-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:06:07.375306 scikeo-0.2.1/
+-rw-rw-rw-   0        0        0      613 2023-03-17 15:59:10.000000 scikeo-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      130 2023-03-17 15:59:10.000000 scikeo-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8976 2023-04-27 17:06:07.375306 scikeo-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8013 2023-03-31 15:29:00.000000 scikeo-0.2.1/README.md
+-rw-rw-rw-   0        0        0       62 2023-03-17 15:59:10.000000 scikeo-0.2.1/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 17:06:07.340357 scikeo-0.2.1/scikeo/
+-rw-rw-rw-   0        0        0      143 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/__init__.py
+-rw-rw-rw-   0        0        0    10900 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/atmosCorr.py
+-rw-rw-rw-   0        0        0     5794 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/calkmeans.py
+-rw-rw-rw-   0        0        0    19966 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/calmla.py
+-rw-rw-rw-   0        0        0     9131 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/deeplearning.py
+-rw-rw-rw-   0        0        0     6113 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/fusionrs.py
+-rw-rw-rw-   0        0        0     6668 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/linearTrend.py
+-rw-rw-rw-   0        0        0    25713 2023-03-23 01:18:16.000000 scikeo-0.2.1/scikeo/mla.py
+-rw-rw-rw-   0        0        0     5043 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/pca.py
+-rw-rw-rw-   0        0        0     5789 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/plot.py
+-rw-rw-rw-   0        0        0    10277 2023-04-27 16:42:51.000000 scikeo-0.2.1/scikeo/process.py
+-rw-rw-rw-   0        0        0     1871 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/rkmeans.py
+-rw-rw-rw-   0        0        0     3819 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/sma.py
+-rw-rw-rw-   0        0        0     5235 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/tassCap.py
+-rw-rw-rw-   0        0        0     2068 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/writeRaster.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:06:07.373241 scikeo-0.2.1/scikeo.egg-info/
+-rw-rw-rw-   0        0        0     8976 2023-04-27 17:06:06.000000 scikeo-0.2.1/scikeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-04-27 17:06:07.000000 scikeo-0.2.1/scikeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       56 2023-04-27 17:06:06.000000 scikeo-0.2.1/scikeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-20 19:51:08.000000 scikeo-0.2.1/scikeo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-04-27 17:06:06.000000 scikeo-0.2.1/scikeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 17:06:06.000000 scikeo-0.2.1/scikeo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      414 2023-04-27 17:06:07.375306 scikeo-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1755 2023-04-27 16:59:24.000000 scikeo-0.2.1/setup.py
```

### Comparing `scikeo-0.2.0/LICENSE` & `scikeo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/PKG-INFO` & `scikeo-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikeo
-Version: 0.2.0
+Version: 0.2.1
 Summary: Remote Sensing Tools
 Home-page: https://github.com/ytarazona/scikit-eo
 Author: Yonatan Tarazona Coronel
 Author-email: geoyons@gmail.com
 License: Apache Software License 2.0
 Keywords: scikeo
 Classifier: Intended Audience :: Developers
@@ -43,14 +43,15 @@
 
 # Tools for Remote Sensing
 
 | Name of functions  | Description|
 | -------------------| --------------------------------------------------------------------------|
 | **`mla`**          | Machine Learning                                                          |
 | **`calmla`**       | Calibrating supervised classification in Remote Sensing                   |
+| **`confintervalML`**       | Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval and estimated area with confidence interval as well.                                    |
 | **`rkmeans`**      | K-means classification                                                    |
 | **`calkmeans`**    | This function allows to calibrate the kmeans algorithm. It is possible to obtain the best k value and the best embedded algorithm in kmeans.                               |
 | **`pca`**          | Principal Components Analysis                                             |
 | **`atmosCorr`**    | Atmospheric Correction of satellite imagery                               |
 | **`deepLearning`** | Deep Learning algorithms                                                  |
 | **`linearTrend`**  | Linear trend is useful for mapping forest degradation or land degradation |
 | **`fusionrs`**     | This algorithm allows to fusion images coming from different spectral sensors (e.g., optical-optical, optical and SAR or SAR-SAR). Among many of the qualities of this function, it is possible to obtain the contribution (%) of each variable in the fused image |
```

### Comparing `scikeo-0.2.0/README.md` & `scikeo-0.2.1/scikeo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: scikeo
+Version: 0.2.1
+Summary: Remote Sensing Tools
+Home-page: https://github.com/ytarazona/scikit-eo
+Author: Yonatan Tarazona Coronel
+Author-email: geoyons@gmail.com
+License: Apache Software License 2.0
+Keywords: scikeo
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!-- #region -->
 # scikit-eo: A Python package for Remote Sensing Tools
 
 [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
 [![License: MIT](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PythonVersion]( https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-green)]()
 [![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
@@ -22,14 +43,15 @@
 
 # Tools for Remote Sensing
 
 | Name of functions  | Description|
 | -------------------| --------------------------------------------------------------------------|
 | **`mla`**          | Machine Learning                                                          |
 | **`calmla`**       | Calibrating supervised classification in Remote Sensing                   |
+| **`confintervalML`**       | Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval and estimated area with confidence interval as well.                                    |
 | **`rkmeans`**      | K-means classification                                                    |
 | **`calkmeans`**    | This function allows to calibrate the kmeans algorithm. It is possible to obtain the best k value and the best embedded algorithm in kmeans.                               |
 | **`pca`**          | Principal Components Analysis                                             |
 | **`atmosCorr`**    | Atmospheric Correction of satellite imagery                               |
 | **`deepLearning`** | Deep Learning algorithms                                                  |
 | **`linearTrend`**  | Linear trend is useful for mapping forest degradation or land degradation |
 | **`fusionrs`**     | This algorithm allows to fusion images coming from different spectral sensors (e.g., optical-optical, optical and SAR or SAR-SAR). Among many of the qualities of this function, it is possible to obtain the contribution (%) of each variable in the fused image |
@@ -163,15 +185,15 @@
 # Let's define the color palette
 palette = mpl.colors.ListedColormap(["#2232F9","#F922AE","#229954","#7CED5E"])
 ```
 
 Applying the ```plotRGB()``` algorithm is easy:
 
 ```python
-# Let´s plot
+# LetÂ´s plot
 fig, axes = plt.subplots(nrows = 1, ncols = 2, figsize = (15, 9))
 
 # satellite image
 plotRGB(img, title = 'Image in Surface Reflectance', ax = axes[0])
 
 # class results
 axes[1].imshow(svm_class.get('Classification_Map'), cmap = palette)
@@ -193,13 +215,13 @@
 Special thanks to:
 - [David Montero Loaiza](https://github.com/davemlz) for the idea of the package name **scikit-eo**.
 
 - [Qiusheng Wu](https://github.com/giswqs) for the suggestions that helped to improve the package.
 
 ## Dedication and inspiration
 
-Yonatan Tarazona dedicates this package to [María Griselda Miyasiro López](https://github.com/geolomera), the person who inspired to develop it. In fact, the logo of the package is inspired by fog oasis known as "Lomas", an ecosystem that she loves deeply.
+Yonatan Tarazona dedicates this package to [MarÃ­a Griselda Miyasiro LÃ³pez](https://github.com/geolomera), the person who inspired to develop it. In fact, the logo of the package is inspired by fog oasis known as "Lomas", an ecosystem that she loves deeply.
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter)
 <!-- #endregion -->
```

### Comparing `scikeo-0.2.0/scikeo/atmosCorr.py` & `scikeo-0.2.1/scikeo/atmosCorr.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/calkmeans.py` & `scikeo-0.2.1/scikeo/calkmeans.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/calmla.py` & `scikeo-0.2.1/scikeo/calmla.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/deeplearning.py` & `scikeo-0.2.1/scikeo/deeplearning.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/fusionrs.py` & `scikeo-0.2.1/scikeo/fusionrs.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/linearTrend.py` & `scikeo-0.2.1/scikeo/linearTrend.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/mla.py` & `scikeo-0.2.1/scikeo/mla.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/pca.py` & `scikeo-0.2.1/scikeo/pca.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/plot.py` & `scikeo-0.2.1/scikeo/plot.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/process.py` & `scikeo-0.2.1/scikeo/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,18 +151,14 @@
 
     if join_df.isnull().values.any():
         raise TypeError('DataFrame contains nan values. Check it out')
         
     return join_df
 
 
-import copy
-import numpy as np
-import pandas as pd
-
 def confintervalML(matrix, image_pred, pixel_size = 10, conf = 1.96, nodata = None):
     
     '''
     The error matrix is a simple cross-tabulation of the class labels allocated by the classification of the remotely 
     sensed data against the reference data for the sample sites. The error matrix organizes the acquired sample data 
     in a way that summarizes key results and aids the quantification of accuracy and area. The main diagonal of the error 
     matrix highlights correct classifications while the off-diagonal elements show omission and commission errors. 
@@ -184,14 +180,19 @@
     Return:
         
         Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval 
         and estimated area with confidence interval as well.
         
     Note:
         Columns and rows in a confusion matrix indicate reference and prediction respectively. 
+        
+    Reference:
+    - Olofsson, P., Foody, G.M., Herold, M., Stehman, S.V., Woodcock, C.E., and Wulder, M.A. 2014. “Good practices 
+      for estimating area and assessing accuracy of land change.” Remote Sensing of Environment, Vol. 148: 42–57. 
+      doi:https://doi.org/10.1016/j.rse.2014.02.015.
     
     '''
     
     if not isinstance(matrix, (np.ndarray)):
         raise TypeError('"matrix" must be numpy.ndarray with rows and cols.')
         
     if not isinstance(image_pred, (np.ndarray)):
@@ -218,15 +219,15 @@
         pixels.append((image_pred == i).sum()) #((30**2)/10000) # ha    
     
     wi = (np.array([pixels])/np.array([pixels]).sum()).flatten()
     
     pixels = np.array(pixels)
     
     # copy of matrix
-    matConf = matrix.copy()
+    matConf = matrix.astype(float).copy()
     
     for i in range(n):
         matConf[i,:] = (matConf[i,:]/ni[i])*wi[i]
     
     # user's accuracy
     ua = np.diag(matConf)/np.sum(matConf, axis = 1)
     
@@ -255,47 +256,48 @@
     cm_prop_area = pd.DataFrame(np.round(mat_conf, 4), columns = namesCol, index = namesRow)
     
     # overall accuracy
     oa = np.diag(matConf).sum()/np.sum(matConf)
     
     # confidence interval for Overall accuracy at 95% 1.96
     conf_int_oa = list(map(lambda Wi, UA, Ni: (Wi)**2*UA*(1-UA)/(Ni-1), wi, ua, ni))
-    conf_int_oa = conf*(np.array(conf_int_oa).sum())
+    conf_int_oa = conf*np.sqrt(np.nansum((np.array(conf_int_oa))))
         
     # confidence interval for user's accuracy at 95% 1.96
-    conf_int_ua = conf*np.array(list(map(lambda UA, Ni: UA*(1-UA)/(Ni-1), ua, ni)))
+    conf_int_ua = conf*np.sqrt(np.array(list(map(lambda UA, Ni: UA*(1-UA)/(Ni-1), ua, ni))))
+    conf_int_ua[np.isnan(conf_int_ua)] = 0
     
     # confidence interval for the area at 95%
     sp = []
     for i in np.arange(n):
         s_pi = list(map(lambda Wi, Pik, Ni: (Wi*Pik - Pik**2)/(Ni-1), wi, matConf[:,i], ni))
-        s_pi = np.sqrt(np.array(s_pi).sum())
+        s_pi = np.sqrt(np.nansum(np.array(s_pi)))
         sp.append(s_pi)
     
     # S(A)=1.96*s(p)*A(total) in ha
     SA = conf*np.array(sp)*(np.array(pixels).sum())*(pixel_size**2/10000)
     
     # Area total estimated
     A = total[0:n]*(np.array(pixels).sum())*(pixel_size**2/10000)
     
     # print info
     def print_info(matrixCEA, a, b, c, d):
-        print('***** Confusion Matrix by Estimated Proportions of area *****')
+        print('***** Confusion Matrix by Estimated Proportions of area an uncertainty*****')
         print('')
-        print('Overall accuracy')
+        print('Overall accuracy with 95%')
         print(f'{oa:.4f} ± {conf_int_oa:.4f}')
         print('')
         print('Confusion matrix')
         print(matrixCEA)
         print('')
-        print('User´s accuracy at 95%')
+        print('User´s accuracy with 95%')
         for i in range(b.shape[0]):
             print(f'{iclass[i]}: {a[i]:.4f} ± {b[i]:.4f}')
         print('')
-        print('Estimating area (Ha) and uncertainty at 95%')
+        print('Estimating area (Ha) and uncertainty with 95%')
         for i in range(b.shape[0]):
             print(f'{iclass[i]}: {c[i]:.4f} ± {d[i]:.4f}')
             
     return print_info(cm_prop_area, 
                       ua, 
                       conf_int_ua, 
                       A,
```

### Comparing `scikeo-0.2.0/scikeo/rkmeans.py` & `scikeo-0.2.1/scikeo/rkmeans.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/sma.py` & `scikeo-0.2.1/scikeo/sma.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/tassCap.py` & `scikeo-0.2.1/scikeo/tassCap.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo/writeRaster.py` & `scikeo-0.2.1/scikeo/writeRaster.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/scikeo.egg-info/PKG-INFO` & `scikeo-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,226 +1,206 @@
-Metadata-Version: 2.1
-Name: scikeo
-Version: 0.2.0
-Summary: Remote Sensing Tools
-Home-page: https://github.com/ytarazona/scikit-eo
-Author: Yonatan Tarazona Coronel
-Author-email: geoyons@gmail.com
-License: Apache Software License 2.0
-Keywords: scikeo
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<!-- #region -->
-# scikit-eo: A Python package for Remote Sensing Tools
-
-[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
-[![License: MIT](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![PythonVersion]( https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-green)]()
-[![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
-[![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()     
-[![Twitter](https://img.shields.io/twitter/url?label=Follow%20%40GeoYons&style=social&url=https%3A%2F%2Ftwitter.com%2FGeoYons)](https://twitter.com/GeoYons)
-[![Downloads](https://pepy.tech/badge/scikeo)](https://pepy.tech/project/scikeo)
-[![Downloads](https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/docs-passing-brightgreen.svg)]()
-
-<img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/scikit-eo_logo.jpg" align="right" width="220"/>
-
-
-<!-- #region -->
-# Introduction
-
-Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are using to monitor a variaty of environmental issues such as deforestation, land degradation, crop classifications, among other. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users in developing Python lines of code. Algorithms for mapping land degradation through linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, calibration of machine learning lagorithms, among others, are not available yet.
-
-Therefore, **scikit-eo** is a Python package that provides tools for remote sensing. This package was developed to fill the gaps in remotely sensed data processing tools. Most of the tools are based on scientific publications, and others are useful algorithms that will allow processing to be done in a few lines of code. With these tools, the user will be able to invest time in analyzing the results of their data and not spend time on elaborating lines of code, which can sometimes be stressful.
-
-# Tools for Remote Sensing
-
-| Name of functions  | Description|
-| -------------------| --------------------------------------------------------------------------|
-| **`mla`**          | Machine Learning                                                          |
-| **`calmla`**       | Calibrating supervised classification in Remote Sensing                   |
-| **`rkmeans`**      | K-means classification                                                    |
-| **`calkmeans`**    | This function allows to calibrate the kmeans algorithm. It is possible to obtain the best k value and the best embedded algorithm in kmeans.                               |
-| **`pca`**          | Principal Components Analysis                                             |
-| **`atmosCorr`**    | Atmospheric Correction of satellite imagery                               |
-| **`deepLearning`** | Deep Learning algorithms                                                  |
-| **`linearTrend`**  | Linear trend is useful for mapping forest degradation or land degradation |
-| **`fusionrs`**     | This algorithm allows to fusion images coming from different spectral sensors (e.g., optical-optical, optical and SAR or SAR-SAR). Among many of the qualities of this function, it is possible to obtain the contribution (%) of each variable in the fused image |
-| **`sma`**          | Spectral Mixture Analysis - Classification sup-pixel                      |
-| **`tassCap`**      | The Tasseled-Cap Transformation                                           |
-
-You will find more algorithms!.
-
-
-# Installation
-
-To use **scikit-eo** it is necessary to install it. There are two options:
-
-## 1. From PyPI
-
-**scikit-eo** is available on [PyPI](https://pypi.org/project/scikeo/), so to install it, run this command in your terminal:
-
-```python
-pip install scikeo
-```
-
-## 2. Installing from source
-
-It is also possible to install the latest development version directly from the GitHub repository with:
-
-```python
-pip install git+https://github.com/ytarazona/scikit-eo
-```
-<!-- #endregion -->
-
-# Example
-
-## 1. Applying Machine Learning
-
-Libraries to be used:
-
-```python
-import rasterio
-import numpy as np
-from scikeo.mla import MLA
-import matplotlib.pyplot as plt
-from dbfread import DBF
-import matplotlib as mpl
-import pandas as pd
-```
-
-## 2.0 Optical image
-
-
-Landsat-8 OLI (Operational Land Imager) will be used to obtain in order to classify using Random Forest (RF). This image, which is in surface reflectance with bands:
-- Blue -> B2
-- Green -> B3 
-- Red -> B4
-- Nir -> B5
-- Swir1 -> B6
-- Swir2 -> B7
-
-The image and signatures to be used can be downloaded [here](https://drive.google.com/drive/folders/193RhNpACu9THcOZu8OzMh-btnFCOgHrU?usp=sharing):
-
-
-## 3.0 Supervised Classification using Random Forest
-
-Image and endmembers
-
-```python
-path_raster = r"C:\data\ml\LC08_232066_20190727_SR.tif"
-img = rasterio.open(path_raster)
-
-path_endm = r"C:\data\ml\endmembers.dbf"
-endm = DBF(path_endm)
-```
-
-```python
-# endmembers
-df = pd.DataFrame(iter(endm))
-df.head()
-```
-<p align="left">
-  <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/endembers.png" alt ="header" width = 75%>
-</a>
-</p>
-
-
-Instance of ```mla()```:
-
-```python
-inst = MLA(image = img, endmembers = endm)
-```
-
-Applying Random Forest:
-
-```python
-svm_class = inst.SVM(training_split = 0.7)
-```
-
-## 4.0 Results
-
-Dictionary of results
-
-```python
-svm_class.keys()
-```
-
-Overall accuracy
-
-```python
-svm_class.get('Overall_Accuracy')
-```
-
-Kappa index
-
-```python
-svm_class.get('Kappa_Index')
-```
-
-Confusion matrix or error matrix
-
-```python
-svm_class.get('Confusion_Matrix')
-```
-
-<p align="left">
-  <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/confusion_matrix.png" alt ="header" width = 80%>
-</a>
-</p>
-
-
-Preparing the image before plotting
-
-```python
-# Let's define the color palette
-palette = mpl.colors.ListedColormap(["#2232F9","#F922AE","#229954","#7CED5E"])
-```
-
-Applying the ```plotRGB()``` algorithm is easy:
-
-```python
-# LetÂ´s plot
-fig, axes = plt.subplots(nrows = 1, ncols = 2, figsize = (15, 9))
-
-# satellite image
-plotRGB(img, title = 'Image in Surface Reflectance', ax = axes[0])
-
-# class results
-axes[1].imshow(svm_class.get('Classification_Map'), cmap = palette)
-axes[1].set_title("Classification map")
-axes[1].grid(False)
-```
-
-<p align="left">
-  <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/classification.png" alt ="header" width = "750">
-</a>
-</p>
-
-<!-- #region -->
--   Free software: Apache Software License 2.0
--   Documentation: 
-
-## Acknowledgment
-
-Special thanks to:
-- [David Montero Loaiza](https://github.com/davemlz) for the idea of the package name **scikit-eo**.
-
-- [Qiusheng Wu](https://github.com/giswqs) for the suggestions that helped to improve the package.
-
-## Dedication and inspiration
-
-Yonatan Tarazona dedicates this package to [MarÃ­a Griselda Miyasiro LÃ³pez](https://github.com/geolomera), the person who inspired to develop it. In fact, the logo of the package is inspired by fog oasis known as "Lomas", an ecosystem that she loves deeply.
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter)
-<!-- #endregion -->
+<!-- #region -->
+# scikit-eo: A Python package for Remote Sensing Tools
+
+[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
+[![License: MIT](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![PythonVersion]( https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-green)]()
+[![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
+[![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()     
+[![Twitter](https://img.shields.io/twitter/url?label=Follow%20%40GeoYons&style=social&url=https%3A%2F%2Ftwitter.com%2FGeoYons)](https://twitter.com/GeoYons)
+[![Downloads](https://pepy.tech/badge/scikeo)](https://pepy.tech/project/scikeo)
+[![Downloads](https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/docs-passing-brightgreen.svg)]()
+
+<img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/scikit-eo_logo.jpg" align="right" width="220"/>
+
+
+<!-- #region -->
+# Introduction
+
+Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are using to monitor a variaty of environmental issues such as deforestation, land degradation, crop classifications, among other. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users in developing Python lines of code. Algorithms for mapping land degradation through linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, calibration of machine learning lagorithms, among others, are not available yet.
+
+Therefore, **scikit-eo** is a Python package that provides tools for remote sensing. This package was developed to fill the gaps in remotely sensed data processing tools. Most of the tools are based on scientific publications, and others are useful algorithms that will allow processing to be done in a few lines of code. With these tools, the user will be able to invest time in analyzing the results of their data and not spend time on elaborating lines of code, which can sometimes be stressful.
+
+# Tools for Remote Sensing
+
+| Name of functions  | Description|
+| -------------------| --------------------------------------------------------------------------|
+| **`mla`**          | Machine Learning                                                          |
+| **`calmla`**       | Calibrating supervised classification in Remote Sensing                   |
+| **`confintervalML`**       | Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval and estimated area with confidence interval as well.                                    |
+| **`rkmeans`**      | K-means classification                                                    |
+| **`calkmeans`**    | This function allows to calibrate the kmeans algorithm. It is possible to obtain the best k value and the best embedded algorithm in kmeans.                               |
+| **`pca`**          | Principal Components Analysis                                             |
+| **`atmosCorr`**    | Atmospheric Correction of satellite imagery                               |
+| **`deepLearning`** | Deep Learning algorithms                                                  |
+| **`linearTrend`**  | Linear trend is useful for mapping forest degradation or land degradation |
+| **`fusionrs`**     | This algorithm allows to fusion images coming from different spectral sensors (e.g., optical-optical, optical and SAR or SAR-SAR). Among many of the qualities of this function, it is possible to obtain the contribution (%) of each variable in the fused image |
+| **`sma`**          | Spectral Mixture Analysis - Classification sup-pixel                      |
+| **`tassCap`**      | The Tasseled-Cap Transformation                                           |
+
+You will find more algorithms!.
+
+
+# Installation
+
+To use **scikit-eo** it is necessary to install it. There are two options:
+
+## 1. From PyPI
+
+**scikit-eo** is available on [PyPI](https://pypi.org/project/scikeo/), so to install it, run this command in your terminal:
+
+```python
+pip install scikeo
+```
+
+## 2. Installing from source
+
+It is also possible to install the latest development version directly from the GitHub repository with:
+
+```python
+pip install git+https://github.com/ytarazona/scikit-eo
+```
+<!-- #endregion -->
+
+# Example
+
+## 1. Applying Machine Learning
+
+Libraries to be used:
+
+```python
+import rasterio
+import numpy as np
+from scikeo.mla import MLA
+import matplotlib.pyplot as plt
+from dbfread import DBF
+import matplotlib as mpl
+import pandas as pd
+```
+
+## 2.0 Optical image
+
+
+Landsat-8 OLI (Operational Land Imager) will be used to obtain in order to classify using Random Forest (RF). This image, which is in surface reflectance with bands:
+- Blue -> B2
+- Green -> B3 
+- Red -> B4
+- Nir -> B5
+- Swir1 -> B6
+- Swir2 -> B7
+
+The image and signatures to be used can be downloaded [here](https://drive.google.com/drive/folders/193RhNpACu9THcOZu8OzMh-btnFCOgHrU?usp=sharing):
+
+
+## 3.0 Supervised Classification using Random Forest
+
+Image and endmembers
+
+```python
+path_raster = r"C:\data\ml\LC08_232066_20190727_SR.tif"
+img = rasterio.open(path_raster)
+
+path_endm = r"C:\data\ml\endmembers.dbf"
+endm = DBF(path_endm)
+```
+
+```python
+# endmembers
+df = pd.DataFrame(iter(endm))
+df.head()
+```
+<p align="left">
+  <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/endembers.png" alt ="header" width = 75%>
+</a>
+</p>
+
+
+Instance of ```mla()```:
+
+```python
+inst = MLA(image = img, endmembers = endm)
+```
+
+Applying Random Forest:
+
+```python
+svm_class = inst.SVM(training_split = 0.7)
+```
+
+## 4.0 Results
+
+Dictionary of results
+
+```python
+svm_class.keys()
+```
+
+Overall accuracy
+
+```python
+svm_class.get('Overall_Accuracy')
+```
+
+Kappa index
+
+```python
+svm_class.get('Kappa_Index')
+```
+
+Confusion matrix or error matrix
+
+```python
+svm_class.get('Confusion_Matrix')
+```
+
+<p align="left">
+  <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/confusion_matrix.png" alt ="header" width = 80%>
+</a>
+</p>
+
+
+Preparing the image before plotting
+
+```python
+# Let's define the color palette
+palette = mpl.colors.ListedColormap(["#2232F9","#F922AE","#229954","#7CED5E"])
+```
+
+Applying the ```plotRGB()``` algorithm is easy:
+
+```python
+# Let´s plot
+fig, axes = plt.subplots(nrows = 1, ncols = 2, figsize = (15, 9))
+
+# satellite image
+plotRGB(img, title = 'Image in Surface Reflectance', ax = axes[0])
+
+# class results
+axes[1].imshow(svm_class.get('Classification_Map'), cmap = palette)
+axes[1].set_title("Classification map")
+axes[1].grid(False)
+```
+
+<p align="left">
+  <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/classification.png" alt ="header" width = "750">
+</a>
+</p>
+
+<!-- #region -->
+-   Free software: Apache Software License 2.0
+-   Documentation: 
+
+## Acknowledgment
+
+Special thanks to:
+- [David Montero Loaiza](https://github.com/davemlz) for the idea of the package name **scikit-eo**.
+
+- [Qiusheng Wu](https://github.com/giswqs) for the suggestions that helped to improve the package.
+
+## Dedication and inspiration
+
+Yonatan Tarazona dedicates this package to [María Griselda Miyasiro López](https://github.com/geolomera), the person who inspired to develop it. In fact, the logo of the package is inspired by fog oasis known as "Lomas", an ecosystem that she loves deeply.
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter)
+<!-- #endregion -->
```

### Comparing `scikeo-0.2.0/scikeo.egg-info/SOURCES.txt` & `scikeo-0.2.1/scikeo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.0/setup.py` & `scikeo-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='scikeo',
     name='scikeo',
     packages=find_packages(include=['scikeo', 'scikeo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ytarazona/scikit-eo',
-    version='0.2.0',
+    version='0.2.1',
     zip_safe=False,
 )
```


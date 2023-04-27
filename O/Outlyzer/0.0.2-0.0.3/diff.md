# Comparing `tmp/Outlyzer-0.0.2.tar.gz` & `tmp/Outlyzer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Outlyzer-0.0.2.tar", last modified: Fri Apr 21 18:42:36 2023, max compression
+gzip compressed data, was "Outlyzer-0.0.3.tar", last modified: Thu Apr 27 16:23:51 2023, max compression
```

## Comparing `Outlyzer-0.0.2.tar` & `Outlyzer-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:09:30.000000 Outlyzer-0.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/Outlyzer/
--rw-rw-rw-   0        0        0        0 2023-04-21 18:31:57.000000 Outlyzer-0.0.2/Outlyzer/__init__.py
--rw-rw-rw-   0        0        0      835 2023-04-21 18:13:33.000000 Outlyzer-0.0.2/Outlyzer/iqr.py
--rw-rw-rw-   0        0        0      982 2023-04-21 18:22:27.000000 Outlyzer-0.0.2/Outlyzer/visual.py
--rw-rw-rw-   0        0        0      644 2023-04-21 18:33:47.000000 Outlyzer-0.0.2/Outlyzer/zscore.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/Outlyzer.egg-info/
--rw-rw-rw-   0        0        0     1509 2023-04-21 18:42:35.000000 Outlyzer-0.0.2/Outlyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/Outlyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:42:35.000000 Outlyzer-0.0.2/Outlyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-21 18:42:35.000000 Outlyzer-0.0.2/Outlyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 18:42:35.000000 Outlyzer-0.0.2/Outlyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1509 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-21 18:09:30.000000 Outlyzer-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1839 2023-04-21 18:42:19.000000 Outlyzer-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 16:23:51.570791 Outlyzer-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-04-24 08:52:04.000000 Outlyzer-0.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-27 16:23:51.539548 Outlyzer-0.0.3/Outlyzer/
+-rw-rw-rw-   0        0        0        0 2023-04-24 08:52:04.000000 Outlyzer-0.0.3/Outlyzer/__init__.py
+-rw-rw-rw-   0        0        0      831 2023-04-27 16:20:33.000000 Outlyzer-0.0.3/Outlyzer/iqr.py
+-rw-rw-rw-   0        0        0      730 2023-04-24 08:52:04.000000 Outlyzer-0.0.3/Outlyzer/least_squares.py
+-rw-rw-rw-   0        0        0      641 2023-04-24 08:52:04.000000 Outlyzer-0.0.3/Outlyzer/probabilistic.py
+-rw-rw-rw-   0        0        0      988 2023-04-24 14:36:53.000000 Outlyzer-0.0.3/Outlyzer/visual.py
+-rw-rw-rw-   0        0        0      644 2023-04-24 08:52:04.000000 Outlyzer-0.0.3/Outlyzer/zscore.py
+drwxrwxrwx   0        0        0        0 2023-04-27 16:23:51.570791 Outlyzer-0.0.3/Outlyzer.egg-info/
+-rw-rw-rw-   0        0        0     1529 2023-04-27 16:23:51.000000 Outlyzer-0.0.3/Outlyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-04-27 16:23:51.000000 Outlyzer-0.0.3/Outlyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 16:23:51.000000 Outlyzer-0.0.3/Outlyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-27 16:23:51.000000 Outlyzer-0.0.3/Outlyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 16:23:51.000000 Outlyzer-0.0.3/Outlyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1529 2023-04-27 16:23:51.570791 Outlyzer-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      870 2023-04-24 08:52:04.000000 Outlyzer-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 16:23:51.570791 Outlyzer-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-04-27 16:20:44.000000 Outlyzer-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Outlyzer-0.0.2/LICENSE` & `Outlyzer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Outlyzer-0.0.2/Outlyzer/iqr.py` & `Outlyzer-0.0.3/Outlyzer/iqr.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Detects outliers in data using the Interquartile Range (IQR) method.
     
     Args:
         data (numpy.ndarray): Input data as a NumPy array.
         multiplier (float): Multiplier for IQR. Data points below Q1 - multiplier * IQR
                            and above Q3 + multiplier * IQR are considered as outliers.
                            Default is 1.5.
-    
+
     Returns:
         numpy.ndarray: Boolean array with True for outlier data points and False otherwise.
     """
     q1 = np.percentile(data, 25)
     q3 = np.percentile(data, 75)
     iqr = q3 - q1
     lower_bound = q1 - multiplier * iqr
```

### Comparing `Outlyzer-0.0.2/Outlyzer/visual.py` & `Outlyzer-0.0.3/Outlyzer/visual.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     """
     plt.scatter(data[x_column], data[y_column])
     plt.xlabel(x_column)
     plt.ylabel(y_column)
     plt.title(f'Scatter plot of {x_column} vs {y_column}')
     plt.show()
 
+    
 def box_plot(data, column):
     """
     Creates a box plot of the data for the specified column.
     
     Parameters:
         -- data (DataFrame): The input data in DataFrame format
         -- column (str): The column name for box plot
```

### Comparing `Outlyzer-0.0.2/Outlyzer/zscore.py` & `Outlyzer-0.0.3/Outlyzer/zscore.py`

 * *Files identical despite different names*

### Comparing `Outlyzer-0.0.2/Outlyzer.egg-info/PKG-INFO` & `Outlyzer-0.0.3/Outlyzer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: Outlyzer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Outlier detection
+Home-page: https://github.com/Devparihar5/Outlyzer
 Author: Devendra Parihar
 Author-email: devendraparihar340@gmail.com
 Keywords: outliers,outlier-detection,data-science,machine-learning,statistics,zscore,iqr,visualization
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Outlyzer -A Python package to detect outliers in a dataset
 
 
-A Python package to detect outliers in a dataset
-
-Outlyzer: A Python library for outlier detection
-
 Outlyzer is a Python library that provides various methods for detecting outliers in a dataset. It includes implementation of Z-score, IQR, and Mahalanobis distance methods for identifying outliers, as well as visualization-based methods using scatter plots, box plots, and other types of visualizations.
 
 Usage:
+
     - Import the desired method from the library, e.g.:
-        from Outlyzer.zscore import detect_outliers_zscore
+        from Outlyzer.zscore import detect_outliers_zscore        
         from Outlyzer.iqr import detect_outliers_iqr
 
     - Pass your dataset or data series to the respective function, e.g.:
         outliers_zscore = detect_outliers_zscore(data)
         outliers_iqr = detect_outliers_iqr(data)
-
-    - The functions will return a boolean array indicating whether each data point is an outlier (True) or not (False).
-
+    
+    The functions will return a boolean array indicating whether each data point is an outlier (True) or not (False).
```

### Comparing `Outlyzer-0.0.2/PKG-INFO` & `Outlyzer-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: Outlyzer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Outlier detection
+Home-page: https://github.com/Devparihar5/Outlyzer
 Author: Devendra Parihar
 Author-email: devendraparihar340@gmail.com
 Keywords: outliers,outlier-detection,data-science,machine-learning,statistics,zscore,iqr,visualization
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Outlyzer -A Python package to detect outliers in a dataset
 
 
-A Python package to detect outliers in a dataset
-
-Outlyzer: A Python library for outlier detection
-
 Outlyzer is a Python library that provides various methods for detecting outliers in a dataset. It includes implementation of Z-score, IQR, and Mahalanobis distance methods for identifying outliers, as well as visualization-based methods using scatter plots, box plots, and other types of visualizations.
 
 Usage:
+
     - Import the desired method from the library, e.g.:
-        from Outlyzer.zscore import detect_outliers_zscore
+        from Outlyzer.zscore import detect_outliers_zscore        
         from Outlyzer.iqr import detect_outliers_iqr
 
     - Pass your dataset or data series to the respective function, e.g.:
         outliers_zscore = detect_outliers_zscore(data)
         outliers_iqr = detect_outliers_iqr(data)
-
-    - The functions will return a boolean array indicating whether each data point is an outlier (True) or not (False).
-
+    
+    The functions will return a boolean array indicating whether each data point is an outlier (True) or not (False).
```

### Comparing `Outlyzer-0.0.2/setup.py` & `Outlyzer-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,21 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Outlier detection'
-LONG_DESCRIPTION = '''
-
-A Python package to detect outliers in a dataset
-
-Outlyzer: A Python library for outlier detection
-
-Outlyzer is a Python library that provides various methods for detecting outliers in a dataset. It includes implementation of Z-score, IQR, and Mahalanobis distance methods for identifying outliers, as well as visualization-based methods using scatter plots, box plots, and other types of visualizations.
-
-Usage:
-    - Import the desired method from the library, e.g.:
-        from Outlyzer.zscore import detect_outliers_zscore
-        from Outlyzer.iqr import detect_outliers_iqr
-
-    - Pass your dataset or data series to the respective function, e.g.:
-        outliers_zscore = detect_outliers_zscore(data)
-        outliers_iqr = detect_outliers_iqr(data)
-
-    - The functions will return a boolean array indicating whether each data point is an outlier (True) or not (False).
-
-'''
+with open('README.md', 'r') as f:
+    LONG_DESCRIPTION = f.read()
 
 # Setting up
 setup(
     name="Outlyzer",
     version=VERSION,
     author="Devendra Parihar",
     author_email="devendraparihar340@gmail.com",
+    url='https://github.com/Devparihar5/Outlyzer',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=['numpy', 'scipy', 'pandas', 'matplotlib'],
     keywords=['outliers', 'outlier-detection', 'data-science', 'machine-learning', 'statistics', 'zscore', 'iqr', 'visualization'],
     classifiers=[
```


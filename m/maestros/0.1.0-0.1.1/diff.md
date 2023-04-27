# Comparing `tmp/maestros-0.1.0.tar.gz` & `tmp/maestros-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestros-0.1.0.tar", last modified: Mon Apr 17 17:11:24 2023, max compression
+gzip compressed data, was "maestros-0.1.1.tar", last modified: Thu Apr 27 08:22:29 2023, max compression
```

## Comparing `maestros-0.1.0.tar` & `maestros-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 emile     (1000) emile     (1000)        0 2023-04-17 17:11:24.492561 maestros-0.1.0/
--rw-rw-r--   0 emile     (1000) emile     (1000)     1058 2023-04-17 16:35:15.000000 maestros-0.1.0/LICENSE
--rw-rw-r--   0 emile     (1000) emile     (1000)      828 2023-04-17 17:11:24.492561 maestros-0.1.0/PKG-INFO
--rw-rw-r--   0 emile     (1000) emile     (1000)     5265 2023-04-17 17:06:08.000000 maestros-0.1.0/README.md
-drwxrwxr-x   0 emile     (1000) emile     (1000)        0 2023-04-17 17:11:24.492561 maestros-0.1.0/maestros/
--rw-rw-r--   0 emile     (1000) emile     (1000)       61 2023-04-17 17:01:21.000000 maestros-0.1.0/maestros/__init__.py
--rw-rw-r--   0 emile     (1000) emile     (1000)    13805 2023-04-17 16:56:16.000000 maestros-0.1.0/maestros/functions.py
-drwxrwxr-x   0 emile     (1000) emile     (1000)        0 2023-04-17 17:11:24.492561 maestros-0.1.0/maestros.egg-info/
--rw-rw-r--   0 emile     (1000) emile     (1000)      828 2023-04-17 17:11:24.000000 maestros-0.1.0/maestros.egg-info/PKG-INFO
--rw-rw-r--   0 emile     (1000) emile     (1000)      228 2023-04-17 17:11:24.000000 maestros-0.1.0/maestros.egg-info/SOURCES.txt
--rw-rw-r--   0 emile     (1000) emile     (1000)        1 2023-04-17 17:11:24.000000 maestros-0.1.0/maestros.egg-info/dependency_links.txt
--rw-rw-r--   0 emile     (1000) emile     (1000)       99 2023-04-17 17:11:24.000000 maestros-0.1.0/maestros.egg-info/requires.txt
--rw-rw-r--   0 emile     (1000) emile     (1000)        9 2023-04-17 17:11:24.000000 maestros-0.1.0/maestros.egg-info/top_level.txt
--rw-rw-r--   0 emile     (1000) emile     (1000)       38 2023-04-17 17:11:24.492561 maestros-0.1.0/setup.cfg
--rw-rw-r--   0 emile     (1000) emile     (1000)     1108 2023-04-17 16:59:28.000000 maestros-0.1.0/setup.py
+drwxrwxr-x   0 emile     (1000) emile     (1000)        0 2023-04-27 08:22:29.080749 maestros-0.1.1/
+-rw-rw-r--   0 emile     (1000) emile     (1000)     1058 2023-04-17 16:35:15.000000 maestros-0.1.1/LICENSE
+-rw-rw-r--   0 emile     (1000) emile     (1000)     1137 2023-04-27 08:22:29.080749 maestros-0.1.1/PKG-INFO
+-rw-rw-r--   0 emile     (1000) emile     (1000)     5688 2023-04-18 06:43:14.000000 maestros-0.1.1/README.md
+drwxrwxr-x   0 emile     (1000) emile     (1000)        0 2023-04-27 08:22:29.080749 maestros-0.1.1/maestros/
+-rw-rw-r--   0 emile     (1000) emile     (1000)       61 2023-04-27 08:21:07.000000 maestros-0.1.1/maestros/__init__.py
+-rw-rw-r--   0 emile     (1000) emile     (1000)    14092 2023-04-27 08:11:07.000000 maestros-0.1.1/maestros/functions.py
+drwxrwxr-x   0 emile     (1000) emile     (1000)        0 2023-04-27 08:22:29.080749 maestros-0.1.1/maestros.egg-info/
+-rw-rw-r--   0 emile     (1000) emile     (1000)     1137 2023-04-27 08:22:29.000000 maestros-0.1.1/maestros.egg-info/PKG-INFO
+-rw-rw-r--   0 emile     (1000) emile     (1000)      228 2023-04-27 08:22:29.000000 maestros-0.1.1/maestros.egg-info/SOURCES.txt
+-rw-rw-r--   0 emile     (1000) emile     (1000)        1 2023-04-27 08:22:29.000000 maestros-0.1.1/maestros.egg-info/dependency_links.txt
+-rw-rw-r--   0 emile     (1000) emile     (1000)       99 2023-04-27 08:22:29.000000 maestros-0.1.1/maestros.egg-info/requires.txt
+-rw-rw-r--   0 emile     (1000) emile     (1000)        9 2023-04-27 08:22:29.000000 maestros-0.1.1/maestros.egg-info/top_level.txt
+-rw-rw-r--   0 emile     (1000) emile     (1000)       38 2023-04-27 08:22:29.080749 maestros-0.1.1/setup.cfg
+-rw-rw-r--   0 emile     (1000) emile     (1000)     1440 2023-04-27 08:20:54.000000 maestros-0.1.1/setup.py
```

### Comparing `maestros-0.1.0/LICENSE` & `maestros-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maestros-0.1.0/README.md` & `maestros-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # maestros - Multi-label Stratified Group Splits
 
-`maestros` is a Python library that provides functionality for performing multi-label stratified group splits. This library is particularly useful for machine learning tasks involving multi-label data with grouped samples, where the train and test sets need to be stratified to maintain the label distribution, while ensuring the groups are disjoint. The multi-label stratification is done through the [iterative-stratification](https://github.com/trent-b/iterative-stratification) library.
+`maestros` is a Python library that provides functionality for performing multi-label stratified group splits. This library is particularly useful for machine learning tasks involving multi-label data with grouped samples, where the train and test sets need to be stratified to maintain the label distribution, while ensuring the groups are disjoint. The multi-label stratification is done through the [iterative-stratification](https://github.com/trent-b/iterative-stratification) library. The included stratification chart and report can also be used for multi-label data where samples do not belong to groups.
+
+## Features
+
+- Perform multi-label stratified group splits, ensuring that groups are disjoint.
+- Create stratification reports to analyze the distribution of labels across the complete dataset and the train and test sets.
+- Visualize the stratification results using a chart.
+- Features adapt when a validation set is included.
+- Easy-to-use with mock data generation for testing purposes.
 
 ## Installation
 
 Install the `maestros` package using `pip`:
 
 ```python
 pip install maestros
@@ -16,22 +24,14 @@
 iterative_stratification==0.1.7
 matplotlib==3.5.3
 numpy==1.22.3
 pandas==1.5.1
 scikit_learn==1.0.2
 ```
 
-## Features
-
-- Perform multi-label stratified group splits, ensuring that groups are disjoint.
-- Create stratification reports to analyze the distribution of labels across the complete dataset and the train and test sets.
-- Visualize the stratification results using a chart.
-- Features adapt when a validation set is included.
-- Easy-to-use with mock data generation for testing purposes.
-
 ## Usage
 
 Import the needed functions from the library.
 
 ```python
 from maestros import *
 ```
@@ -60,15 +60,15 @@
 
 Print a stratification report.
 
 ```
 stratification_report(y, y_train, y_test, labels=labels)
 ```
 
-A lower mean difference is a better stratified set. A mean of 0 is perfectly stratified set.
+The label distribution shows the percentage of class '1' samples of the complete, training, (validation) and test set. The difference shows how much the distribution of a set differs from that of the complete set. A mean difference closer to 0 is a better stratified set.
 
 ```
 Label distribution:
 Label            Complete   Train      Test  
 Beach           0.789      0.787     0.795
 Water           0.799      0.799     0.800
 Tree            0.824      0.833     0.790
@@ -87,22 +87,22 @@
 Train-Complete: 0.005
 Test-Complete: 0.021
 ```
 
 Plot the stratification chart.
 
 ```
-msg_split.create_stratification_chart(y, y_train, y_test, labels=labels)
+create_stratification_chart(y, y_train, y_test, labels=labels)
 ```
 
 ![Stratification Chart](img/stratification_chart.png)
 
 ### Including Validation Set
 
-To include a validation set, simply execute the `multilabel-stratified-group-split` twice: once to create `train_val` and `test` sets, and once to create a `train`  and `test`  set from `train_val`.
+To include a validation set, simply execute the `multilabel-stratified-group-split` twice: once to create `train_val` and `test` sets, and once to create a `train`  and `test`  set from `train_val`. For the stratification report and chart, include y_val when calling the function.
 
 ```
 # First, split the data into 80% train+val and 20% test
 X_train_val, X_test, y_train_val, y_test, train_val_indices, test_indices = multilabel_stratified_group_split(
     X, y, groups, test_size=0.2, random_state=42, shuffle=True
 )
 
@@ -119,15 +119,15 @@
 create_stratification_chart(y, y_train, y_test, y_val=y_val, labels=labels)
 ```
 
 Stratification report with validation set included:
 
 ```
 Label distribution:
-Label            Complete   Train      Val        Test      
+Label            Complete   Train      Val        Test    
 Beach           0.788      0.801     0.750     0.785
 Water           0.788      0.770     0.880     0.760
 Tree            0.812      0.805     0.793     0.843
 House           0.808      0.822     0.783     0.793
 Mountain        0.804      0.801     0.793     0.818
 
 Differences:
@@ -140,12 +140,14 @@
 
 Mean Differences:
 Train-Complete: 0.011
 Val-Complete: 0.037
 Test-Complete: 0.018
 ```
 
+Stratification chart with validation set included:
+
 ![Stratification Chart](img/stratification_chart_with_val.png)
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `maestros-0.1.0/maestros/functions.py` & `maestros-0.1.1/maestros/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,90 +99,99 @@
     distribution : array-like, shape (n_labels,)
         The distribution of labels.
     """
     return np.sum(y, axis=0) / y.shape[0]
 
 def stratification_report(y, y_train, y_test, y_val=None, labels=None):
     """
-    Print a stratification report comparing the label distributions in the complete dataset, training set, and test set.
+    Return a stratification report comparing the label distributions in the complete dataset, training set, and test set.
     
     Parameters
     ----------
     y : array-like, shape (n_samples, n_labels)
         The complete multilabel target matrix.
     y_train : array-like, shape (n_train_samples, n_labels)
         The training multilabel target matrix.
     y_test : array-like, shape (n_test_samples, n_labels)
         The test multilabel target matrix.
     y_val : array-like, shape (n_val_samples, n_labels), optional (default=None)
         The validation multilabel target matrix.
     labels : list of str, optional (default=None)
         The names of the labels. If None, generic names will be used.
+
+    Returns
+    -------
+    retrun_str : string
+        The stratification report as a string.
     """
     complete_set_distribution = label_distribution(y)
     train_set_distribution = label_distribution(y_train)
     test_set_distribution = label_distribution(y_test)
     if y_val is not None:
         val_set_distribution = label_distribution(y_val)
 
-    print("\nLabel distribution:")
+    return_str = ""
+
+    return_str += "\nLabel distribution:\n"
     header = "{:<16} {:<10} {:<10}".format("Label", "Complete", "Train")
     if y_val is not None:
         header += " {:<10}".format("Val")
     header += " {:<10}".format("Test")
-    print(header)
+    return_str += header + "\n"
 
     for i, (complete, train, test) in enumerate(zip(complete_set_distribution, train_set_distribution, test_set_distribution)):
         if y_val is not None:
             val = val_set_distribution[i]
         else:
             val = ""
 
         if labels:
             row = f"{labels[i]:<15} {complete:.3f}{' '*5} {train:.3f}{' '*5}"
         else:
             row = f"Label {i:<10} {complete:.3f}{' '*5} {train:.3f}{' '*5}"
         if y_val is not None:
             row += f"{val:.3f}{' '*5}"
         row += f"{test:.3f}"
-        print(row)
+        return_str += row + "\n"
 
-    print("\nDifferences:")
+    return_str += "\nLabel distribution difference:\n"
     header_diff = "{:<16} {:<15}".format("Label", "Train-Complete")
     if y_val is not None:
         header_diff += " {:<15}".format("Val-Complete")
     header_diff += " {:<15}".format("Test-Complete")
-    print(header_diff)
+    return_str += header_diff + "\n"
 
     for i, (train_diff, test_diff) in enumerate(zip(np.abs(train_set_distribution - complete_set_distribution), np.abs(test_set_distribution - complete_set_distribution))):
         if y_val is not None:
             val_diff = np.abs(val_set_distribution[i] - complete_set_distribution[i])
         else:
             val_diff = ""
 
         if labels:
             row_diff = f"{labels[i]:<20} {train_diff:.3f}{' '*10}"
         else:
             row_diff = f"Label {i:<10} {train_diff:.3f}{' '*10}"
         if y_val is not None:
             row_diff += f"{val_diff:.3f}{' '*10}"
         row_diff += f"{test_diff:.3f}"
-        print(row_diff)
+        return_str += row_diff + "\n"
 
-    print("\nMean Differences:")
+    return_str += "\nMean label distribution difference:\n"
     mean_train_diff = np.mean(np.abs(train_set_distribution - complete_set_distribution))
     if y_val is not None:
         mean_val_diff = np.mean(np.abs(val_set_distribution - complete_set_distribution))
     mean_test_diff = np.mean(np.abs(test_set_distribution - complete_set_distribution))
 
-    print(f"Train-Complete: {mean_train_diff:.3f}")
+    return_str += f"Train-Complete: {mean_train_diff:.3f}\n"
     if y_val is not None:
         mean_val_diff = np.mean(np.abs(val_set_distribution - complete_set_distribution))
-        print(f"Val-Complete: {mean_val_diff:.3f}")
-    print(f"Test-Complete: {mean_test_diff:.3f}")
+        return_str += f"Val-Complete: {mean_val_diff:.3f}\n"
+    return_str += f"Test-Complete: {mean_test_diff:.3f}\n"
+
+    return return_str
 
 def check_disjoint_groups(train_indices, test_indices, groups):
     """
     Check if the groups in the train set and test set are disjoint.
     
     Parameters
     ----------
```

### Comparing `maestros-0.1.0/setup.py` & `maestros-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="maestros",
-    version="0.1.0",
+    version="0.1.1",
+    long_description="A package for splitting multilabel datasets into train and test sets, while preserving the distribution of labels and keeping samples from the same group together. Includes a report and chart for visualizing the stratification. Multi-label stratificatin is done through the iterative-stratification package.",
     description="A package for splitting multilabel datasets into train and test sets, while preserving the distribution of labels and keeping samples from the same group together. Includes a report and chart for visualizing the stratification.",
     author="Emile Lampe",
     author_email="emilelampe@outlook.com",
     url="https://github.com/emilelampe/maestros",
     packages=find_packages(),
     install_requires=[
         "numpy>=1.19.5",
```


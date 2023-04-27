# Comparing `tmp/principal-feature-analysis-1.0.8.tar.gz` & `tmp/principal-feature-analysis-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "principal-feature-analysis-1.0.8.tar", last modified: Fri Apr  7 12:46:49 2023, max compression
+gzip compressed data, was "principal-feature-analysis-1.0.9.tar", last modified: Thu Apr 27 14:50:56 2023, max compression
```

## Comparing `principal-feature-analysis-1.0.8.tar` & `principal-feature-analysis-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 12:46:49.528861 principal-feature-analysis-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-07 12:46:39.000000 principal-feature-analysis-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-07 12:46:49.528861 principal-feature-analysis-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-07 12:46:39.000000 principal-feature-analysis-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 12:46:39.000000 principal-feature-analysis-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 12:46:49.528861 principal-feature-analysis-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-07 12:46:39.000000 principal-feature-analysis-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 12:46:49.524861 principal-feature-analysis-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 12:46:49.528861 principal-feature-analysis-1.0.8/src/principal_feature_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-07 12:46:39.000000 principal-feature-analysis-1.0.8/src/principal_feature_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-07 12:46:39.000000 principal-feature-analysis-1.0.8/src/principal_feature_analysis/execute_PFA.py
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-04-07 12:46:39.000000 principal-feature-analysis-1.0.8/src/principal_feature_analysis/find_relevant_principal_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-04-07 12:46:39.000000 principal-feature-analysis-1.0.8/src/principal_feature_analysis/get_mutual_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-07 12:46:39.000000 principal-feature-analysis-1.0.8/src/principal_feature_analysis/principal_feature_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 12:46:49.528861 principal-feature-analysis-1.0.8/src/principal_feature_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-07 12:46:49.000000 principal-feature-analysis-1.0.8/src/principal_feature_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-07 12:46:49.000000 principal-feature-analysis-1.0.8/src/principal_feature_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 12:46:49.000000 principal-feature-analysis-1.0.8/src/principal_feature_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-07 12:46:49.000000 principal-feature-analysis-1.0.8/src/principal_feature_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-07 12:46:49.000000 principal-feature-analysis-1.0.8/src/principal_feature_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:50:56.006567 principal-feature-analysis-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-27 14:50:43.000000 principal-feature-analysis-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-27 14:50:56.006567 principal-feature-analysis-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-27 14:50:43.000000 principal-feature-analysis-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-27 14:50:43.000000 principal-feature-analysis-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:50:56.006567 principal-feature-analysis-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-27 14:50:43.000000 principal-feature-analysis-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:50:56.002566 principal-feature-analysis-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:50:56.006567 principal-feature-analysis-1.0.9/src/principal_feature_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-27 14:50:43.000000 principal-feature-analysis-1.0.9/src/principal_feature_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-27 14:50:43.000000 principal-feature-analysis-1.0.9/src/principal_feature_analysis/execute_PFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-04-27 14:50:43.000000 principal-feature-analysis-1.0.9/src/principal_feature_analysis/find_relevant_principal_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-27 14:50:43.000000 principal-feature-analysis-1.0.9/src/principal_feature_analysis/get_mutual_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-27 14:50:43.000000 principal-feature-analysis-1.0.9/src/principal_feature_analysis/principal_feature_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:50:56.006567 principal-feature-analysis-1.0.9/src/principal_feature_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-27 14:50:55.000000 principal-feature-analysis-1.0.9/src/principal_feature_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-27 14:50:55.000000 principal-feature-analysis-1.0.9/src/principal_feature_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:50:55.000000 principal-feature-analysis-1.0.9/src/principal_feature_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 14:50:55.000000 principal-feature-analysis-1.0.9/src/principal_feature_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 14:50:55.000000 principal-feature-analysis-1.0.9/src/principal_feature_analysis.egg-info/top_level.txt
```

### Comparing `principal-feature-analysis-1.0.8/LICENSE` & `principal-feature-analysis-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `principal-feature-analysis-1.0.8/PKG-INFO` & `principal-feature-analysis-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: principal-feature-analysis
-Version: 1.0.8
+Version: 1.0.9
 Summary: The first package for Principal Feature Analysis
 Author: Tim Breitenbach & Lauritz Rasbach
 Author-email: tim.breitenbach@mathematik.uni-wuerzburg.de, rasbachlauritz@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `principal-feature-analysis-1.0.8/README.md` & `principal-feature-analysis-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `principal-feature-analysis-1.0.8/setup.py` & `principal-feature-analysis-1.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="principal-feature-analysis",
-    version="1.0.8",
+    version="1.0.9",
     author="Tim Breitenbach & Lauritz Rasbach",
     author_email="tim.breitenbach@mathematik.uni-wuerzburg.de, rasbachlauritz@googlemail.com",
     description="The first package for Principal Feature Analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `principal-feature-analysis-1.0.8/src/principal_feature_analysis/execute_PFA.py` & `principal-feature-analysis-1.0.9/src/principal_feature_analysis/execute_PFA.py`

 * *Files identical despite different names*

### Comparing `principal-feature-analysis-1.0.8/src/principal_feature_analysis/find_relevant_principal_features.py` & `principal-feature-analysis-1.0.9/src/principal_feature_analysis/find_relevant_principal_features.py`

 * *Files identical despite different names*

### Comparing `principal-feature-analysis-1.0.8/src/principal_feature_analysis/get_mutual_information.py` & `principal-feature-analysis-1.0.9/src/principal_feature_analysis/get_mutual_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     # Calculate the mutual information for each feature with the corresponding component of the output function
     list_of_data_frames=[]
     mutual_info = np.ones((1, len(left_features) - number_output_functions + 1))  # number of featuers plus one component of the output-function
     for i in range(0,number_output_functions):
         list_of_features=list(range(number_output_functions,len(left_features)))
         list_of_features.insert(0,i)
-        id_features=np.array(list_variables)[left_features]
+        id_features=np.array(list_variables)[list_of_features]
         
         for j in list_of_features:
             freq_data_product = ((np.histogram2d(data[i,:], data[left_features[j], :], bins=(l[i], l[left_features[j]]))[0])) / n
             expfreq = (np.outer(freq_data[i], freq_data[left_features[j]])) / (n * n)
             if j<number_output_functions:
                 mutual_info[0, 0] = np.sum(np.array(list(map(make_summand_from_frequencies, freq_data_product.flatten().tolist(),expfreq.flatten().tolist()))))
             else:
```

### Comparing `principal-feature-analysis-1.0.8/src/principal_feature_analysis/principal_feature_analysis.py` & `principal-feature-analysis-1.0.9/src/principal_feature_analysis/principal_feature_analysis.py`

 * *Files identical despite different names*

### Comparing `principal-feature-analysis-1.0.8/src/principal_feature_analysis.egg-info/PKG-INFO` & `principal-feature-analysis-1.0.9/src/principal_feature_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: principal-feature-analysis
-Version: 1.0.8
+Version: 1.0.9
 Summary: The first package for Principal Feature Analysis
 Author: Tim Breitenbach & Lauritz Rasbach
 Author-email: tim.breitenbach@mathematik.uni-wuerzburg.de, rasbachlauritz@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `principal-feature-analysis-1.0.8/src/principal_feature_analysis.egg-info/SOURCES.txt` & `principal-feature-analysis-1.0.9/src/principal_feature_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*


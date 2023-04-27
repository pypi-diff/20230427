# Comparing `tmp/responsibleai_text-0.1.0.tar.gz` & `tmp/responsibleai_text-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/responsibleai_text-0.1.0.tar", last modified: Wed Apr 12 20:55:46 2023, max compression
+gzip compressed data, was "dist/responsibleai_text-0.1.1.tar", last modified: Thu Apr 27 20:24:24 2023, max compression
```

## Comparing `responsibleai_text-0.1.0.tar` & `responsibleai_text-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text/common/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/common/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/managers/error_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/managers/explainer_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text/rai_text_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/rai_text_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25718 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/rai_text_insights/rai_text_insights.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/utils/feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/utils/question_answering.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/tests/test_rai_text_insights.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/tests/test_rai_text_insights_save_and_load_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/common/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/managers/error_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/managers/explainer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text/rai_text_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/rai_text_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25644 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/rai_text_insights/rai_text_insights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/utils/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/utils/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/responsibleai_text/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/responsibleai_text.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:24:24.000000 responsibleai_text-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/tests/test_rai_text_insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-27 20:21:44.000000 responsibleai_text-0.1.1/tests/test_rai_text_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_text-0.1.0/PKG-INFO` & `responsibleai_text-0.1.1/responsibleai_text.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: responsibleai_text
-Version: 0.1.0
+Name: responsibleai-text
+Version: 0.1.1
 Summary: SDK API to assess text Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_text-0.1.0/README.md` & `responsibleai_text-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.0/responsibleai_text/common/constants.py` & `responsibleai_text-0.1.1/responsibleai_text/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.0/responsibleai_text/managers/error_analysis_manager.py` & `responsibleai_text-0.1.1/responsibleai_text/managers/error_analysis_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,60 +62,64 @@
         :type classes: list
         """
         self.model = model
         self.dataset = dataset
         self.classes = classes
         self.is_multilabel = is_multilabel
         self.task_type = task_type
-
-    def predict(self, X):
-        """Predict the class labels for the provided data.
-
-        :param X: Data to predict the labels for.
-        :type X: pandas.DataFrame
-        :return: Predicted class labels.
-        :rtype: list
-        """
-        index = X.index
-        indexed_dataset = self.dataset.iloc[index]
-
         if self.task_type in [ModelTask.TEXT_CLASSIFICATION, ModelTask.MULTILABEL_TEXT_CLASSIFICATION]:
-            predictions = self.model.predict(indexed_dataset.iloc[:, 0].tolist())
+            self.predictions = self.model.predict(self.dataset.iloc[:, 0].tolist())
         elif self.task_type == ModelTask.QUESTION_ANSWERING:
-            predictions = self.model.predict(indexed_dataset.loc[:, ['context', 'questions']])
+            self.predictions = self.model.predict(self.dataset.loc[:, ['context', 'questions']])
+            self.predictions = np.array(self.predictions)
         else:
             raise ValueError("Unknown task type: {}".format(self.task_type))
 
         if self.is_multilabel:
             predictions_joined = []
-            for row in predictions:
+            for row in self.predictions:
                 # get all labels where prediction is 1
                 pred_labels = [i for i in range(len(row)) if row[i]]
                 if self.classes is not None:
                     pred_labels = [self.classes[i] for i in pred_labels]
                 else:
                     pred_labels = [str(i) for i in pred_labels]
                 # concatenate all predicted labels into a single string
                 predictions_joined.append(','.join(pred_labels))
-            return np.array(predictions_joined)
+            self.predictions = np.array(predictions_joined)
+        if self.task_type != ModelTask.QUESTION_ANSWERING:
+            self.predict_proba = self.model.predict_proba(self.dataset.iloc[:, 0].tolist())
+
+    def predict(self, X):
+        """Predict the class labels for the provided data.
+
+        :param X: Data to predict the labels for.
+        :type X: pandas.DataFrame
+        :return: Predicted class labels.
+        :rtype: list
+        """
+        index = X.index
+        predictions = self.predictions[index]
+        if self.task_type == ModelTask.MULTILABEL_TEXT_CLASSIFICATION:
+            return predictions
         if self.classes is not None:
             predictions = [self.classes[y] for y in predictions]
         return predictions
 
     def predict_proba(self, X):
         """Predict the class probabilities for the provided data.
 
         :param X: Data to predict the probabilities for.
         :type X: pandas.DataFrame
         :return: Predicted class probabilities.
         :rtype: list[list]
         """
         index = X.index
-        indexed_dataset = self.dataset.iloc[index]
-        return self.model.predict_proba(indexed_dataset.iloc[:, 0].tolist())
+        pred_proba = self.predict_proba[index]
+        return pred_proba
 
 
 class ErrorAnalysisManager(BaseErrorAnalysisManager):
 
     """Defines a wrapper class of Error Analysis for text scenario."""
 
     def __init__(self, model: Any, dataset: pd.DataFrame,
```

### Comparing `responsibleai_text-0.1.0/responsibleai_text/managers/explainer_manager.py` & `responsibleai_text-0.1.1/responsibleai_text/managers/explainer_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.0/responsibleai_text/rai_text_insights/rai_text_insights.py` & `responsibleai_text-0.1.1/responsibleai_text/rai_text_insights/rai_text_insights.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,17 +101,16 @@
                                                   task_type)
         self._ext_test = ext_test
         self._ext_features = ext_features
         self._ext_test_df = pd.DataFrame(ext_test, columns=ext_features)
         self._ext_test_df[target_column] = test[target_column]
         self.predict_output = None
 
-        # TODO: on next responsibleai package upgrade pass None for train
         super(RAITextInsights, self).__init__(
-            model, test, test, target_column, task_type,
+            model, None, test, target_column, task_type,
             serializer)
         self._initialize_managers()
 
     def _initialize_managers(self):
         """Initializes the managers.
 
         Initializes the explainer and error analysis managers.
```

### Comparing `responsibleai_text-0.1.0/responsibleai_text/utils/feature_extractors.py` & `responsibleai_text-0.1.1/responsibleai_text/utils/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.0/responsibleai_text/utils/question_answering.py` & `responsibleai_text-0.1.1/responsibleai_text/utils/question_answering.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.0/responsibleai_text.egg-info/PKG-INFO` & `responsibleai_text-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: responsibleai-text
-Version: 0.1.0
+Name: responsibleai_text
+Version: 0.1.1
 Summary: SDK API to assess text Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_text-0.1.0/responsibleai_text.egg-info/SOURCES.txt` & `responsibleai_text-0.1.1/responsibleai_text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.0/setup.py` & `responsibleai_text-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.0/tests/test_rai_text_insights.py` & `responsibleai_text-0.1.1/tests/test_rai_text_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.0/tests/test_rai_text_insights_save_and_load_scenarios.py` & `responsibleai_text-0.1.1/tests/test_rai_text_insights_save_and_load_scenarios.py`

 * *Files identical despite different names*


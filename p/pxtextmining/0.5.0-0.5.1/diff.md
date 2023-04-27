# Comparing `tmp/pxtextmining-0.5.0.tar.gz` & `tmp/pxtextmining-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxtextmining-0.5.0.tar", max compression
+gzip compressed data, was "pxtextmining-0.5.1.tar", max compression
```

## Comparing `pxtextmining-0.5.0.tar` & `pxtextmining-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1068 2022-11-17 15:31:00.811802 pxtextmining-0.5.0/LICENSE
--rw-r--r--   0        0        0      949 2023-04-03 08:21:59.385245 pxtextmining-0.5.0/README.md
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.0/pxtextmining/__init__.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.0/pxtextmining/factories/__init__.py
--rw-r--r--   0        0        0    20715 2023-04-03 08:21:49.655245 pxtextmining-0.5.0/pxtextmining/factories/factory_data_load_and_split.py
--rw-r--r--   0        0        0     5292 2023-04-03 08:21:49.655245 pxtextmining-0.5.0/pxtextmining/factories/factory_model_performance.py
--rw-r--r--   0        0        0    16008 2023-04-03 08:21:49.655245 pxtextmining-0.5.0/pxtextmining/factories/factory_pipeline.py
--rw-r--r--   0        0        0     5911 2023-04-03 08:21:49.655245 pxtextmining-0.5.0/pxtextmining/factories/factory_predict_unlabelled_text.py
--rw-r--r--   0        0        0     1128 2023-04-03 08:21:49.655245 pxtextmining-0.5.0/pxtextmining/factories/factory_write_results.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.0/pxtextmining/helpers/__init__.py
--rw-r--r--   0        0        0      945 2023-04-03 08:21:49.655245 pxtextmining-0.5.0/pxtextmining/helpers/text_preprocessor.py
--rw-r--r--   0        0        0      688 2023-04-03 08:21:49.655245 pxtextmining-0.5.0/pxtextmining/helpers/tokenization.py
--rw-r--r--   0        0        0      461 2023-04-03 08:21:49.655245 pxtextmining-0.5.0/pxtextmining/params.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.0/pxtextmining/pipelines/__init__.py
--rw-r--r--   0        0        0     7864 2023-04-03 08:21:49.655245 pxtextmining-0.5.0/pxtextmining/pipelines/multilabel_pipeline.py
--rw-r--r--   0        0        0     1082 2023-04-03 08:21:59.385245 pxtextmining-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 pxtextmining-0.5.0/setup.py
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 pxtextmining-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-11-17 15:31:00.811802 pxtextmining-0.5.1/LICENSE
+-rw-r--r--   0        0        0      949 2023-04-03 08:21:59.385245 pxtextmining-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.1/pxtextmining/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.1/pxtextmining/factories/__init__.py
+-rw-r--r--   0        0        0    12184 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/factories/factory_data_load_and_split.py
+-rw-r--r--   0        0        0     7047 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/factories/factory_model_performance.py
+-rw-r--r--   0        0        0    17430 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/factories/factory_pipeline.py
+-rw-r--r--   0        0        0    10996 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/factories/factory_predict_unlabelled_text.py
+-rw-r--r--   0        0        0     3529 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/factories/factory_write_results.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.1/pxtextmining/helpers/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-03 08:21:49.655245 pxtextmining-0.5.1/pxtextmining/helpers/text_preprocessor.py
+-rw-r--r--   0        0        0      688 2023-04-03 08:21:49.655245 pxtextmining-0.5.1/pxtextmining/helpers/tokenization.py
+-rw-r--r--   0        0        0     6918 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/params.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.1/pxtextmining/pipelines/__init__.py
+-rw-r--r--   0        0        0    11542 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/pipelines/multilabel_pipeline.py
+-rw-r--r--   0        0        0     1082 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 pxtextmining-0.5.1/setup.py
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 pxtextmining-0.5.1/PKG-INFO
```

### Comparing `pxtextmining-0.5.0/LICENSE` & `pxtextmining-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.0/README.md` & `pxtextmining-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.0/pxtextmining/factories/factory_pipeline.py` & `pxtextmining-0.5.1/pxtextmining/factories/factory_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import datetime
 import time
 
 import numpy as np
+import xgboost as xgb
 from scipy import stats
 from sklearn.compose import make_column_transformer
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.feature_extraction.text import TfidfVectorizer
-from sklearn.model_selection import RandomizedSearchCV
+from sklearn.model_selection import RandomizedSearchCV, GridSearchCV
 from sklearn.multioutput import MultiOutputClassifier
 from sklearn.naive_bayes import MultinomialNB
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.pipeline import make_pipeline
 from sklearn.preprocessing import OneHotEncoder, RobustScaler
 from sklearn.svm import SVC
 from sklearn.utils.class_weight import compute_class_weight
+from sklearn.model_selection import cross_validate
 from tensorflow.keras import Sequential, layers
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras.initializers import TruncatedNormal
 from tensorflow.keras.layers import Dense, Dropout, Input, concatenate
 from tensorflow.keras.losses import BinaryCrossentropy
 from tensorflow.keras.models import Model
 from tensorflow.keras.optimizers import Adam
@@ -242,38 +244,24 @@
 
     Returns:
         (tuple): Tuple containing the `sklearn.pipeline.Pipeline` with the selected estimator, and a `dict` containing the hyperparameters to be tuned.
     """
     if additional_features == True:
         cat_transformer = OneHotEncoder(handle_unknown="ignore")
         vectorizer = create_sklearn_vectorizer(tokenizer=None)
-        num_transformer = RobustScaler()
+        # num_transformer = RobustScaler()
         preproc = make_column_transformer(
             (cat_transformer, ["FFT_q_standardised"]),
             (vectorizer, "FFT answer"),
-            (num_transformer, ["text_length"]),
+            # (num_transformer, ["text_length"]),
         )
         params = {
             "columntransformer__tfidfvectorizer__ngram_range": ((1, 1), (1, 2), (2, 2)),
-            "columntransformer__tfidfvectorizer__max_df": [
-                0.85,
-                0.86,
-                0.87,
-                0.88,
-                0.89,
-                0.9,
-                0.91,
-                0.92,
-                0.93,
-                0.94,
-                0.95,
-                0.96,
-                0.97,
-            ],
-            "columntransformer__tfidfvectorizer__min_df": stats.uniform(0, 0.15),
+            "columntransformer__tfidfvectorizer__max_df": [0.85,0.86,0.87,0.88,0.89,0.9,0.91,0.92,0.93,0.94,0.95,0.96,0.97,0.98,0.99],
+            "columntransformer__tfidfvectorizer__min_df": stats.uniform(0, 0.1),
         }
     else:
         preproc = create_sklearn_vectorizer(tokenizer=tokenizer)
         params = {
             "tfidfvectorizer__ngram_range": ((1, 1), (1, 2), (2, 2)),
             "tfidfvectorizer__max_df": stats.uniform(0.8, 1),
             "tfidfvectorizer__min_df": stats.uniform(0.01, 0.1),
@@ -289,15 +277,15 @@
         pipe = make_pipeline(
             preproc,
             MultiOutputClassifier(
                 SVC(
                     probability=True,
                     class_weight="balanced",
                     max_iter=1000,
-                    cache_size=500,
+                    cache_size=1000,
                 ),
                 n_jobs=-1,
             ),
         )
         params["multioutputclassifier__estimator__C"] = stats.uniform(0.1, 20)
         params["multioutputclassifier__estimator__kernel"] = [
             "linear",
@@ -311,14 +299,17 @@
         params["randomforestclassifier__class_weight"] = [
             "balanced",
             "balanced_subsample",
             None,
         ]
         params["randomforestclassifier__min_samples_leaf"] = stats.randint(1, 10)
         params["randomforestclassifier__max_features"] = ["sqrt", "log2", None, 0.3]
+    if model_type == 'xgb':
+        pipe = make_pipeline(preproc, xgb.XGBClassifier(tree_method="hist"))
+
     return pipe, params
 
 
 def search_sklearn_pipelines(X_train, Y_train, models_to_try, additional_features=True):
     """Iterates through selected estimators, instantiating the relevant sklearn pipelines and searching for the optimum hyperparameters.
 
     Args:
@@ -332,17 +323,17 @@
 
     Returns:
         (tuple): Tuple containing: a `list` containing the refitted pipelines with the best hyperparameters identified in the search, and a `list` containing the training times for each of the pipelines.
     """
     models = []
     training_times = []
     for model_type in models_to_try:
-        if model_type not in ["mnb", "knn", "svm", "rfc"]:
+        if model_type not in ["mnb", "knn", "svm", "rfc", "xgb"]:
             raise ValueError(
-                "Please choose valid model_type. Options are mnb, knn, svm, or rfc"
+                "Please choose valid model_type. Options are mnb, knn, svm, xgb or rfc"
             )
         else:
             if additional_features == False:
                 pipe, params = create_sklearn_pipeline(
                     model_type, additional_features=False
                 )
             elif additional_features == True:
@@ -355,7 +346,41 @@
                 pipe, params, scoring="f1_macro", n_iter=50, cv=4, n_jobs=-2, refit=True
             )
             search.fit(X_train, Y_train)
             models.append(search.best_estimator_)
             training_time = round(time.time() - start_time, 0)
             training_times.append(str(datetime.timedelta(seconds=training_time)))
     return models, training_times
+
+
+def create_and_train_svc_model(X_train, Y_train):
+    """Creates pipeline with a Support Vector Classifier using specific hyperparameters identified through previous gridsearching.
+
+    Args:
+        X_train (pd.DataFrame): DataFrame containing the features to be fed into the estimator
+        Y_train (pd.DataFrame): DataFrame containing the targets
+
+    Returns:
+        (tuple): Tuple containing: a fitted `pipeline` with a MultiOutputClassifier utilising a Support Vector Classifier estimator, and a `str` of the training time taken for the fitting of the pipeline.
+    """
+    cat_transformer = OneHotEncoder(handle_unknown="ignore")
+    vectorizer = TfidfVectorizer(max_df = 0.9, min_df = 0, ngram_range=(1, 2))
+    preproc = make_column_transformer(
+                (cat_transformer, ["FFT_q_standardised"]),
+                (vectorizer, "FFT answer"),
+            )
+    pipe = make_pipeline(
+                preproc,
+                MultiOutputClassifier(
+                    SVC(C = 15,
+                        probability=True,
+                        class_weight="balanced",
+                        max_iter=1000,
+                        cache_size=1000,
+                    ),
+                ),
+            )
+    start_time = time.time()
+    pipe.fit(X_train, Y_train)
+    training_time = round(time.time() - start_time, 0)
+    training_time = str(datetime.timedelta(seconds=training_time))
+    return pipe, training_time
```

### Comparing `pxtextmining-0.5.0/pxtextmining/helpers/text_preprocessor.py` & `pxtextmining-0.5.1/pxtextmining/helpers/text_preprocessor.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.0/pxtextmining/helpers/tokenization.py` & `pxtextmining-0.5.1/pxtextmining/helpers/tokenization.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.0/pxtextmining/pipelines/multilabel_pipeline.py` & `pxtextmining-0.5.1/pxtextmining/pipelines/multilabel_pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,259 @@
 import random
+import pandas as pd
 
 from sklearn.model_selection import train_test_split
 
 from pxtextmining.factories.factory_data_load_and_split import (
-    bert_data_to_dataset, load_multilabel_data,
-    process_and_split_multilabel_data)
-from pxtextmining.factories.factory_model_performance import \
-    get_multilabel_metrics
+    bert_data_to_dataset,
+    load_multilabel_data,
+    process_and_split_multilabel_data,
+)
+from pxtextmining.factories.factory_model_performance import (
+    get_multilabel_metrics,
+    parse_metrics_file,
+)
 from pxtextmining.factories.factory_pipeline import (
-    calculating_class_weights, create_bert_model,
-    create_bert_model_additional_features, create_tf_model,
-    search_sklearn_pipelines, train_bert_model, train_tf_model)
-from pxtextmining.factories.factory_write_results import \
-    write_multilabel_models_and_metrics
+    calculating_class_weights,
+    create_bert_model,
+    create_bert_model_additional_features,
+    create_tf_model,
+    create_and_train_svc_model,
+    search_sklearn_pipelines,
+    train_bert_model,
+    train_tf_model,
+)
+from pxtextmining.factories.factory_write_results import (
+    write_multilabel_models_and_metrics,
+    write_model_preds,
+)
 from pxtextmining.helpers.text_preprocessor import tf_preprocessing
-from pxtextmining.params import major_cats
+from pxtextmining.params import major_cats, minor_cats, dataset, merged_minor_cats
 
-def run_sklearn_pipeline(additional_features = False, target= major_cats, models_to_try = ["mnb", "knn", "svm", "rfc"], path = 'test_multilabel'):
+
+def run_sklearn_pipeline(
+    additional_features=False,
+    target=major_cats,
+    models_to_try=["mnb", "knn", "svm", "rfc"],
+    path="test_multilabel",
+):
     """Runs all the functions required to load multilabel data, preprocess it, and split it into training and test sets.
     Creates sklearn pipelines and hyperparameters to search, using specified estimators.
     For each estimator type selected, performs a randomized search across the hyperparameters to identify the parameters providing the best
     results on the holdout data within the randomized search.
     Evaluates the performance of the refitted estimator with the best hyperparameters on the test set, and saves the model
     and the performance metrics to a specified folder.
 
     Args:
         additional_features (bool, optional): Whether or not additional features (question type and text length) are used. Defaults to False.
         target (list, optional): The target labels, which should be columns in the dataset DataFrame. Defaults to major_cats.
         models_to_try (list, optional): List of the estimators to try. Defaults to ["mnb", "knn", "svm", "rfc"]. Permitted values are "mnb" (Multinomial Naive Bayes), "knn" (K Nearest Neighbours), "svm" (Support Vector Classifier), or "rfc" (Random Forest Classifier).
         path (str, optional): Path where the models are to be saved. If path does not exist, it will be created. Defaults to 'test_multilabel'.
     """
-    random_state = random.randint(1,999)
-    # This line on loading dataframe has to be manually edited depending on the target and the filename, currently
-    df = load_multilabel_data(filename = 'datasets/hidden/multilabeldata_2.csv', target = 'major_categories')
-    X_train, X_test, Y_train, Y_test = process_and_split_multilabel_data(df, target = target,
-                                                                         additional_features =additional_features, random_state = random_state)
-    models, training_times = search_sklearn_pipelines(X_train, Y_train, models_to_try = models_to_try, additional_features = additional_features)
+    random_state = random.randint(1, 999)
+    if target == major_cats:
+        target_name = "major_categories"
+    if target == minor_cats:
+        target_name = "minor_categories"
+    df = load_multilabel_data(filename=dataset, target=target_name)
+    X_train, X_test, Y_train, Y_test = process_and_split_multilabel_data(
+        df,
+        target=target,
+        additional_features=additional_features,
+        random_state=random_state,
+    )
+    models, training_times = search_sklearn_pipelines(
+        X_train,
+        Y_train,
+        models_to_try=models_to_try,
+        additional_features=additional_features,
+    )
     model_metrics = []
     for i in range(len(models)):
         m = models[i]
         t = training_times[i]
-        model_metrics.append(get_multilabel_metrics(X_test, Y_test, random_state = random_state,
-                                                    labels = target, model_type = 'sklearn', model = m, training_time = t))
-    write_multilabel_models_and_metrics(models,model_metrics,path=path)
+        model_metrics.append(
+            get_multilabel_metrics(
+                X_test,
+                Y_test,
+                random_state=random_state,
+                labels=target,
+                model_type="sklearn",
+                model=m,
+                training_time=t,
+            )
+        )
+    write_multilabel_models_and_metrics(models, model_metrics, path=path)
+
+
+def run_svc_pipeline(
+    additional_features=False,
+    target=major_cats,
+    path="test_multilabel",
+    include_analysis=False,
+):
+    """Runs all the functions required to load multilabel data, preprocess it, and split it into training and test sets.
+    Creates sklearn pipeline using a MultiOutputClassifier and Support Vector Classifier estimator, with specific hyperparameters.
+    Fits the pipeline on the training data.
+    Evaluates the performance of the refitted estimator with the best hyperparameters on the test set, and saves the model and the performance metrics to a specified folder, together with optional further analysis in the form of Excel files.
+
+    Args:
+        additional_features (bool, optional): Whether or not additional features (question type and text length) are used. Defaults to False.
+        target (list, optional): The target labels, which should be columns in the dataset DataFrame. Defaults to major_cats.
+        path (str, optional): Path where the models are to be saved. If path does not exist, it will be created. Defaults to 'test_multilabel'.
+        include_analysis (bool, optional): Whether or not to create Excel files including further analysis of the model's performance. Defaults to False. If True, writes two Excel files to the specified folder, one containing the labels and the performance metrics for each label, and one containing the predicted labels and the actual labels for the test set, with the model's probabilities for both.
+
+    """
+    random_state = random.randint(1, 999)
+    if target == major_cats:
+        target_name = "major_categories"
+    if target == minor_cats:
+        target_name = "minor_categories"
+    if target == merged_minor_cats:
+        target_name = "test"
+    df = load_multilabel_data(filename=dataset, target=target_name)
+    X_train, X_test, Y_train, Y_test = process_and_split_multilabel_data(
+        df,
+        target=target,
+        additional_features=additional_features,
+        random_state=random_state,
+    )
+    model, training_time = create_and_train_svc_model(X_train, Y_train)
+    model_metrics = get_multilabel_metrics(
+        X_test,
+        Y_test,
+        random_state=random_state,
+        labels=target,
+        model_type="sklearn",
+        model=model,
+        training_time=training_time,
+        additional_features=additional_features,
+    )
+    write_multilabel_models_and_metrics([model], [model_metrics], path=path)
+    if include_analysis == True:
+        write_model_preds(
+            X_test,
+            Y_test,
+            model,
+            labels=target,
+            additional_features=additional_features,
+            path=f"{path}/labels.xlsx"
+        )
+        metrics_df = parse_metrics_file(f"{path}/model_0.txt", labels=target)
+        label_counts = pd.DataFrame(df[target].sum())
+        label_counts = label_counts.reset_index()
+        label_counts = label_counts.rename(columns={"index": "label", 0: "label_count"})
+        metrics_df = metrics_df.merge(label_counts, on="label")
+        metrics_df.to_excel(f"{path}/perf.xlsx", index=False)
 
-def run_tf_pipeline(target= major_cats, path = 'test_multilabel/tf'):
+
+def run_tf_pipeline(target=major_cats, path="test_multilabel/tf"):
     """Runs all the functions required to load multilabel data, preprocess it, and split it into training and test sets.
     Creates tf.keras LSTM model and trains it on the train set.
     Evaluates the performance of trained model with the best hyperparameters on the test set, and saves the model
     and the performance metrics to a specified folder.
     Cannot currently take additional features, is only designed for text data alone.
     This model architecture performs very poorly and may be taken out of the model.
 
     Args:
         target (list, optional): The target labels, which should be columns in the dataset DataFrame. Defaults to major_cats.
         path (str, optional): Path where the models are to be saved. If path does not exist, it will be created. Defaults to 'test_multilabel'.
     """
-    random_state = random.randint(1,999)
-    df = load_multilabel_data(filename = 'datasets/multilabeldata_2.csv', target = 'major_categories')
-    X_train, X_test, Y_train, Y_test = process_and_split_multilabel_data(df, target = target, random_state = random_state)
+    random_state = random.randint(1, 999)
+    df = load_multilabel_data(
+        filename="datasets/multilabeldata_2.csv", target="major_categories"
+    )
+    X_train, X_test, Y_train, Y_test = process_and_split_multilabel_data(
+        df, target=target, random_state=random_state
+    )
     X_train_pad, vocab_size = tf_preprocessing(X_train)
     X_test_pad, _ = tf_preprocessing(X_test)
     class_weights_dict = calculating_class_weights(Y_train)
     model = create_tf_model(vocab_size)
-    model_trained, training_time = train_tf_model(X_train_pad, Y_train, model, class_weights_dict = class_weights_dict)
-    model_metrics = get_multilabel_metrics(X_test_pad, Y_test, random_state = random_state, labels = major_cats,
-                                           model_type = 'tf',
-                                           model = model_trained, training_time = training_time)
-    write_multilabel_models_and_metrics([model_trained],[model_metrics],path=path)
+    model_trained, training_time = train_tf_model(
+        X_train_pad, Y_train, model, class_weights_dict=class_weights_dict
+    )
+    model_metrics = get_multilabel_metrics(
+        X_test_pad,
+        Y_test,
+        random_state=random_state,
+        labels=major_cats,
+        model_type="tf",
+        model=model_trained,
+        training_time=training_time,
+    )
+    write_multilabel_models_and_metrics([model_trained], [model_metrics], path=path)
+
 
-def run_bert_pipeline(additional_features = False, path = 'test_multilabel/bert'):
+def run_bert_pipeline(
+    additional_features=False, path="test_multilabel/bert", target=major_cats
+):
     """Runs all the functions required to load multilabel data, preprocess it, and split it into training, test and validation sets.
     Creates tf.keras Transformer model with additional layers specific to the classification task, and trains it on the train set.
     Evaluates the performance of trained model with the best hyperparameters on the test set, and saves the model
     and the performance metrics to a specified folder.
 
     Args:
         additional_features (bool, optional): Whether or not additional features (question type and text length) are used. Defaults to False.
         path (str, optional): Path where the models are to be saved. If path does not exist, it will be created. Defaults to 'test_multilabel'.
     """
-    random_state = random.randint(1,999)
-    print(f'random_state is: {random_state}')
-    # This line on loading dataframe has to be manually edited depending on the target and the filename, currently
-    df = load_multilabel_data(filename = 'datasets/hidden/multilabeldata_2.csv', target = 'major_categories')
-    X_train_val, X_test, Y_train_val, Y_test = process_and_split_multilabel_data(df, target = major_cats, preprocess_text = False,
-                                                                                 additional_features = additional_features, random_state = random_state)
-    X_train, X_val, Y_train, Y_val = train_test_split(X_train_val, Y_train_val, test_size=0.2, random_state = random_state)
-    train_dataset = bert_data_to_dataset(X_train, Y_train, additional_features = additional_features)
-    val_dataset = bert_data_to_dataset(X_val, Y_val, additional_features = additional_features)
-    test_dataset = bert_data_to_dataset(X_test, Y = None, additional_features = additional_features)
+    random_state = random.randint(1, 999)
+    print(f"random_state is: {random_state}")
+    if target == major_cats:
+        target_name = "major_categories"
+    if target == minor_cats:
+        target_name = "minor_categories"
+    df = load_multilabel_data(filename=dataset, target=target_name)
+    X_train_val, X_test, Y_train_val, Y_test = process_and_split_multilabel_data(
+        df,
+        target=target,
+        preprocess_text=False,
+        additional_features=additional_features,
+        random_state=random_state,
+    )
+    X_train, X_val, Y_train, Y_val = train_test_split(
+        X_train_val, Y_train_val, test_size=0.2, random_state=random_state
+    )
+    train_dataset = bert_data_to_dataset(
+        X_train, Y_train, additional_features=additional_features
+    )
+    val_dataset = bert_data_to_dataset(
+        X_val, Y_val, additional_features=additional_features
+    )
+    test_dataset = bert_data_to_dataset(
+        X_test, Y=None, additional_features=additional_features
+    )
     class_weights_dict = calculating_class_weights(Y_train_val)
     if additional_features == True:
         model = create_bert_model_additional_features(Y_train)
     else:
         model = create_bert_model(Y_train)
-    model_trained, training_time = train_bert_model(train_dataset, val_dataset, model,
-                                                    class_weights_dict = class_weights_dict, epochs = 25)
-    model_metrics = get_multilabel_metrics(test_dataset, Y_test, random_state = random_state, labels = major_cats,
-                                           model_type = 'bert',
-                                           model = model_trained, training_time = training_time,
-                                           additional_features = additional_features, already_encoded = True)
-    write_multilabel_models_and_metrics([model_trained],[model_metrics],path=path)
+    model_trained, training_time = train_bert_model(
+        train_dataset,
+        val_dataset,
+        model,
+        class_weights_dict=class_weights_dict,
+        epochs=25,
+    )
+    model_metrics = get_multilabel_metrics(
+        test_dataset,
+        Y_test,
+        random_state=random_state,
+        labels=target,
+        model_type="bert",
+        model=model_trained,
+        training_time=training_time,
+        additional_features=additional_features,
+        already_encoded=True,
+    )
+    write_multilabel_models_and_metrics([model_trained], [model_metrics], path=path)
+
 
-if __name__ == '__main__':
-    run_sklearn_pipeline(additional_features = True)
+if __name__ == "__main__":
+    # run_bert_pipeline(additional_features = True, path = 'test_multilabel/bert_minorcats', target = minor_cats)
+    # run_sklearn_pipeline(additional_features = True, target= minor_cats, models_to_try = ["knn", "svm", "rfc"], path = 'test_multilabel/minorcats_sklearn')
+    run_svc_pipeline(
+        additional_features=True,
+        target=merged_minor_cats,
+        path="test_multilabel/minorcats_merged_230420",
+        include_analysis=True
+    )
```

### Comparing `pxtextmining-0.5.0/pyproject.toml` & `pxtextmining-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pxtextmining"
-version = "0.5.0"
+version = "0.5.1"
 description = "Multilabel text classification of patient experience feedback."
 authors = ['CDU Data Science <cdudatascience@nottshc.nhs.uk>',
 'YiWen Hon <yiwen.hon@nottshc.nhs.uk>']
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/CDU-data-science-team/pxtextmining"
 documentation = "https://cdu-data-science-team.github.io/pxtextmining"
```

### Comparing `pxtextmining-0.5.0/setup.py` & `pxtextmining-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'scipy>=1.10.1,<2.0.0',
  'spacy>=3.4.4,<4.0.0',
  'tensorflow>=2.11.0,<3.0.0',
  'transformers>=4.26.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'pxtextmining',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'Multilabel text classification of patient experience feedback.',
     'long_description': '# pxtextmining: Text Classification of Patient Experience feedback\n\n## Project description\n**pxtextmining** is a Python package for classifying patient feedback comments collected via the [NHS England Friends and Family Test](https://www.england.nhs.uk/fft/) (FFT). It is part of the [Patient Experience Qualitative Data Categorisation project](https://cdu-data-science-team.github.io/PatientExperience-QDC/), funded by NHS England and hosted by Nottinghamshire Healthcare NHS Foundation Trust.\n\n__We are working openly by [open-sourcing](https://github.com/CDU-data-science-team/pxtextmining/blob/main/LICENSE) the analysis code and data where possible to promote replication, reproducibility and further developments. Pull requests are more than welcome.__\n\n## Documentation and installation\n\nFull documentation, including installation instructions, is available on our [documentation page](https://cdu-data-science-team.github.io/pxtextmining/).\n',
     'author': 'CDU Data Science',
     'author_email': 'cdudatascience@nottshc.nhs.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CDU-data-science-team/pxtextmining',
```

### Comparing `pxtextmining-0.5.0/PKG-INFO` & `pxtextmining-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxtextmining
-Version: 0.5.0
+Version: 0.5.1
 Summary: Multilabel text classification of patient experience feedback.
 Home-page: https://github.com/CDU-data-science-team/pxtextmining
 License: MIT
 Author: CDU Data Science
 Author-email: cdudatascience@nottshc.nhs.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```


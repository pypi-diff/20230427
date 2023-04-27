# Comparing `tmp/pxtextmining-0.5.1.tar.gz` & `tmp/pxtextmining-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxtextmining-0.5.1.tar", max compression
+gzip compressed data, was "pxtextmining-0.5.2.tar", max compression
```

## Comparing `pxtextmining-0.5.1.tar` & `pxtextmining-0.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1068 2022-11-17 15:31:00.811802 pxtextmining-0.5.1/LICENSE
--rw-r--r--   0        0        0      949 2023-04-03 08:21:59.385245 pxtextmining-0.5.1/README.md
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.1/pxtextmining/__init__.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.1/pxtextmining/factories/__init__.py
--rw-r--r--   0        0        0    12184 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/factories/factory_data_load_and_split.py
--rw-r--r--   0        0        0     7047 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/factories/factory_model_performance.py
--rw-r--r--   0        0        0    17430 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/factories/factory_pipeline.py
--rw-r--r--   0        0        0    10996 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/factories/factory_predict_unlabelled_text.py
--rw-r--r--   0        0        0     3529 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/factories/factory_write_results.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.1/pxtextmining/helpers/__init__.py
--rw-r--r--   0        0        0      945 2023-04-03 08:21:49.655245 pxtextmining-0.5.1/pxtextmining/helpers/text_preprocessor.py
--rw-r--r--   0        0        0      688 2023-04-03 08:21:49.655245 pxtextmining-0.5.1/pxtextmining/helpers/tokenization.py
--rw-r--r--   0        0        0     6918 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/params.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.1/pxtextmining/pipelines/__init__.py
--rw-r--r--   0        0        0    11542 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pxtextmining/pipelines/multilabel_pipeline.py
--rw-r--r--   0        0        0     1082 2023-04-27 10:50:35.275927 pxtextmining-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 pxtextmining-0.5.1/setup.py
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 pxtextmining-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-11-17 15:31:00.811802 pxtextmining-0.5.2/LICENSE
+-rw-r--r--   0        0        0      949 2023-04-03 08:21:59.385245 pxtextmining-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.2/pxtextmining/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.2/pxtextmining/factories/__init__.py
+-rw-r--r--   0        0        0    12184 2023-04-27 10:50:35.275927 pxtextmining-0.5.2/pxtextmining/factories/factory_data_load_and_split.py
+-rw-r--r--   0        0        0     7047 2023-04-27 11:01:34.635944 pxtextmining-0.5.2/pxtextmining/factories/factory_model_performance.py
+-rw-r--r--   0        0        0    17408 2023-04-27 14:20:24.575856 pxtextmining-0.5.2/pxtextmining/factories/factory_pipeline.py
+-rw-r--r--   0        0        0    10996 2023-04-27 11:01:34.635944 pxtextmining-0.5.2/pxtextmining/factories/factory_predict_unlabelled_text.py
+-rw-r--r--   0        0        0     3529 2023-04-27 11:01:34.635944 pxtextmining-0.5.2/pxtextmining/factories/factory_write_results.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.2/pxtextmining/helpers/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-03 08:21:49.655245 pxtextmining-0.5.2/pxtextmining/helpers/text_preprocessor.py
+-rw-r--r--   0        0        0      688 2023-04-03 08:21:49.655245 pxtextmining-0.5.2/pxtextmining/helpers/tokenization.py
+-rw-r--r--   0        0        0     6918 2023-04-27 10:50:35.275927 pxtextmining-0.5.2/pxtextmining/params.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.2/pxtextmining/pipelines/__init__.py
+-rw-r--r--   0        0        0    11542 2023-04-27 11:01:34.635944 pxtextmining-0.5.2/pxtextmining/pipelines/multilabel_pipeline.py
+-rw-r--r--   0        0        0     1082 2023-04-27 14:30:31.355856 pxtextmining-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 pxtextmining-0.5.2/setup.py
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 pxtextmining-0.5.2/PKG-INFO
```

### Comparing `pxtextmining-0.5.1/LICENSE` & `pxtextmining-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.1/README.md` & `pxtextmining-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.1/pxtextmining/factories/factory_data_load_and_split.py` & `pxtextmining-0.5.2/pxtextmining/factories/factory_data_load_and_split.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.1/pxtextmining/factories/factory_model_performance.py` & `pxtextmining-0.5.2/pxtextmining/factories/factory_model_performance.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.1/pxtextmining/factories/factory_pipeline.py` & `pxtextmining-0.5.2/pxtextmining/factories/factory_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import datetime
 import time
 
 import numpy as np
-import xgboost as xgb
 from scipy import stats
 from sklearn.compose import make_column_transformer
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.model_selection import RandomizedSearchCV, GridSearchCV
 from sklearn.multioutput import MultiOutputClassifier
 from sklearn.naive_bayes import MultinomialNB
```

### Comparing `pxtextmining-0.5.1/pxtextmining/factories/factory_predict_unlabelled_text.py` & `pxtextmining-0.5.2/pxtextmining/factories/factory_predict_unlabelled_text.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.1/pxtextmining/factories/factory_write_results.py` & `pxtextmining-0.5.2/pxtextmining/factories/factory_write_results.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.1/pxtextmining/helpers/text_preprocessor.py` & `pxtextmining-0.5.2/pxtextmining/helpers/text_preprocessor.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.1/pxtextmining/helpers/tokenization.py` & `pxtextmining-0.5.2/pxtextmining/helpers/tokenization.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.1/pxtextmining/params.py` & `pxtextmining-0.5.2/pxtextmining/params.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.1/pxtextmining/pipelines/multilabel_pipeline.py` & `pxtextmining-0.5.2/pxtextmining/pipelines/multilabel_pipeline.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.1/pyproject.toml` & `pxtextmining-0.5.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pxtextmining"
-version = "0.5.1"
+version = "0.5.2"
 description = "Multilabel text classification of patient experience feedback."
 authors = ['CDU Data Science <cdudatascience@nottshc.nhs.uk>',
 'YiWen Hon <yiwen.hon@nottshc.nhs.uk>']
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/CDU-data-science-team/pxtextmining"
 documentation = "https://cdu-data-science-team.github.io/pxtextmining"
```

### Comparing `pxtextmining-0.5.1/setup.py` & `pxtextmining-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'scipy>=1.10.1,<2.0.0',
  'spacy>=3.4.4,<4.0.0',
  'tensorflow>=2.11.0,<3.0.0',
  'transformers>=4.26.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'pxtextmining',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': 'Multilabel text classification of patient experience feedback.',
     'long_description': '# pxtextmining: Text Classification of Patient Experience feedback\n\n## Project description\n**pxtextmining** is a Python package for classifying patient feedback comments collected via the [NHS England Friends and Family Test](https://www.england.nhs.uk/fft/) (FFT). It is part of the [Patient Experience Qualitative Data Categorisation project](https://cdu-data-science-team.github.io/PatientExperience-QDC/), funded by NHS England and hosted by Nottinghamshire Healthcare NHS Foundation Trust.\n\n__We are working openly by [open-sourcing](https://github.com/CDU-data-science-team/pxtextmining/blob/main/LICENSE) the analysis code and data where possible to promote replication, reproducibility and further developments. Pull requests are more than welcome.__\n\n## Documentation and installation\n\nFull documentation, including installation instructions, is available on our [documentation page](https://cdu-data-science-team.github.io/pxtextmining/).\n',
     'author': 'CDU Data Science',
     'author_email': 'cdudatascience@nottshc.nhs.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CDU-data-science-team/pxtextmining',
```

### Comparing `pxtextmining-0.5.1/PKG-INFO` & `pxtextmining-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxtextmining
-Version: 0.5.1
+Version: 0.5.2
 Summary: Multilabel text classification of patient experience feedback.
 Home-page: https://github.com/CDU-data-science-team/pxtextmining
 License: MIT
 Author: CDU Data Science
 Author-email: cdudatascience@nottshc.nhs.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```


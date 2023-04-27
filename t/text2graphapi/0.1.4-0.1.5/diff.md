# Comparing `tmp/text2graphapi-0.1.4.tar.gz` & `tmp/text2graphapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2graphapi-0.1.4.tar", last modified: Tue Apr 25 17:23:09 2023, max compression
+gzip compressed data, was "text2graphapi-0.1.5.tar", last modified: Thu Apr 27 14:19:56 2023, max compression
```

## Comparing `text2graphapi-0.1.4.tar` & `text2graphapi-0.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.471457 text2graphapi-0.1.4/
--rw-rw-rw-   0        0        0       82 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2022-12-02 17:54:23.000000 text2graphapi-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2022-12-02 17:54:23.000000 text2graphapi-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5410 2023-04-25 17:23:09.470422 text2graphapi-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4877 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.368109 text2graphapi-0.1.4/docs/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.334046 text2graphapi-0.1.4/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.335048 text2graphapi-0.1.4/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.379112 text2graphapi-0.1.4/docs/_build/html/_sources/
--rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.4/docs/_build/html/_sources/Cooocurrence.rst.txt
--rw-rw-rw-   0        0        0     1663 2023-03-30 14:12:11.000000 text2graphapi-0.1.4/docs/_build/html/_sources/index.rst.txt
--rw-rw-rw-   0        0        0       46 2022-12-05 21:50:59.000000 text2graphapi-0.1.4/docs/_build/html/_sources/modules.rst.txt
--rw-rw-rw-   0        0        0      408 2022-12-05 21:50:59.000000 text2graphapi-0.1.4/docs/_build/html/_sources/src.rst.txt
--rw-rw-rw-   0        0        0     1783 2022-12-05 21:50:59.000000 text2graphapi-0.1.4/docs/conf.py
--rw-rw-rw-   0        0        0      590 2023-03-30 04:06:40.000000 text2graphapi-0.1.4/notes.txt
--rw-rw-rw-   0        0        0      201 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 17:23:09.471977 text2graphapi-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-04-25 17:22:52.000000 text2graphapi-0.1.4/setup.py
--rw-rw-rw-   0        0        0      379 2023-03-16 18:14:42.000000 text2graphapi-0.1.4/test_spacy.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.383108 text2graphapi-0.1.4/tests/
--rw-rw-rw-   0        0        0        0 2022-10-12 14:46:40.000000 text2graphapi-0.1.4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.390105 text2graphapi-0.1.4/text2graphapi/
--rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.343064 text2graphapi-0.1.4/text2graphapi/docs/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.340075 text2graphapi-0.1.4/text2graphapi/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.341046 text2graphapi-0.1.4/text2graphapi/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.438263 text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/
--rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt
--rw-rw-rw-   0        0        0     1768 2023-03-30 13:07:45.000000 text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt
--rw-rw-rw-   0        0        0     1702 2023-03-30 11:19:22.000000 text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.441259 text2graphapi-0.1.4/text2graphapi/docs/source/
--rw-rw-rw-   0        0        0     1352 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/text2graphapi/docs/source/conf.py
--rw-rw-rw-   0        0        0     8000 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/text2graphapi/main.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.461438 text2graphapi-0.1.4/text2graphapi/src/
--rw-rw-rw-   0        0        0     7155 2023-04-25 17:20:48.000000 text2graphapi-0.1.4/text2graphapi/src/Cooccurrence.py
--rw-rw-rw-   0        0        0     1088 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/src/Graph.py
--rw-rw-rw-   0        0        0     1018 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/src/GraphTransformation.py
--rw-rw-rw-   0        0        0    13651 2023-04-25 17:20:54.000000 text2graphapi-0.1.4/text2graphapi/src/Heterogeneous.py
--rw-rw-rw-   0        0        0     8833 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/text2graphapi/src/Preprocessing.py
--rw-rw-rw-   0        0        0     1873 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/text2graphapi/src/Utils.py
--rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/src/__init__.py
--rw-rw-rw-   0        0        0      482 2023-04-25 17:11:34.000000 text2graphapi-0.1.4/text2graphapi/src/configs.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.468420 text2graphapi-0.1.4/text2graphapi/src/resources/
--rw-rw-rw-   0        0        0     4160 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_english.txt
--rw-rw-rw-   0        0        0     5256 2023-03-08 18:09:28.000000 text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_french.txt
--rw-rw-rw-   0        0        0     4852 2023-01-17 01:14:45.000000 text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_spanish.txt
--rw-rw-rw-   0        0        0     2248 2023-03-30 02:11:28.000000 text2graphapi-0.1.4/text2graphapi/testing.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:23:09.429264 text2graphapi-0.1.4/text2graphapi.egg-info/
--rw-rw-rw-   0        0        0     5410 2023-04-25 17:23:09.000000 text2graphapi-0.1.4/text2graphapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-04-25 17:23:09.000000 text2graphapi-0.1.4/text2graphapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 17:23:09.000000 text2graphapi-0.1.4/text2graphapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-04-25 17:23:09.000000 text2graphapi-0.1.4/text2graphapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-25 17:23:09.000000 text2graphapi-0.1.4/text2graphapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.182045 text2graphapi-0.1.5/
+-rw-rw-rw-   0        0        0       82 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2022-12-02 17:54:23.000000 text2graphapi-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2022-12-02 17:54:23.000000 text2graphapi-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5410 2023-04-27 14:19:56.180033 text2graphapi-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4877 2023-04-25 17:11:34.000000 text2graphapi-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.058283 text2graphapi-0.1.5/docs/
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.000754 text2graphapi-0.1.5/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.001651 text2graphapi-0.1.5/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.066281 text2graphapi-0.1.5/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.5/docs/_build/html/_sources/Cooocurrence.rst.txt
+-rw-rw-rw-   0        0        0     1663 2023-03-30 14:12:11.000000 text2graphapi-0.1.5/docs/_build/html/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0       46 2022-12-05 21:50:59.000000 text2graphapi-0.1.5/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-rw-   0        0        0      408 2022-12-05 21:50:59.000000 text2graphapi-0.1.5/docs/_build/html/_sources/src.rst.txt
+-rw-rw-rw-   0        0        0     1783 2022-12-05 21:50:59.000000 text2graphapi-0.1.5/docs/conf.py
+-rw-rw-rw-   0        0        0      590 2023-03-30 04:06:40.000000 text2graphapi-0.1.5/notes.txt
+-rw-rw-rw-   0        0        0      201 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 14:19:56.183064 text2graphapi-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-04-27 14:19:45.000000 text2graphapi-0.1.5/setup.py
+-rw-rw-rw-   0        0        0      379 2023-03-16 18:14:42.000000 text2graphapi-0.1.5/test_spacy.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.069282 text2graphapi-0.1.5/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-12 14:46:40.000000 text2graphapi-0.1.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.075281 text2graphapi-0.1.5/text2graphapi/
+-rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.011710 text2graphapi-0.1.5/text2graphapi/docs/
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.007651 text2graphapi-0.1.5/text2graphapi/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.009653 text2graphapi-0.1.5/text2graphapi/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.122277 text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/
+-rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt
+-rw-rw-rw-   0        0        0     1768 2023-03-30 13:07:45.000000 text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt
+-rw-rw-rw-   0        0        0     1702 2023-03-30 11:19:22.000000 text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.125707 text2graphapi-0.1.5/text2graphapi/docs/source/
+-rw-rw-rw-   0        0        0     1352 2023-04-25 17:11:34.000000 text2graphapi-0.1.5/text2graphapi/docs/source/conf.py
+-rw-rw-rw-   0        0        0     8063 2023-04-27 14:12:46.000000 text2graphapi-0.1.5/text2graphapi/main.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.170010 text2graphapi-0.1.5/text2graphapi/src/
+-rw-rw-rw-   0        0        0     7155 2023-04-25 17:20:48.000000 text2graphapi-0.1.5/text2graphapi/src/Cooccurrence.py
+-rw-rw-rw-   0        0        0     1088 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/src/Graph.py
+-rw-rw-rw-   0        0        0     1018 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/src/GraphTransformation.py
+-rw-rw-rw-   0        0        0    13651 2023-04-27 14:05:50.000000 text2graphapi-0.1.5/text2graphapi/src/Heterogeneous.py
+-rw-rw-rw-   0        0        0     8833 2023-04-25 17:11:34.000000 text2graphapi-0.1.5/text2graphapi/src/Preprocessing.py
+-rw-rw-rw-   0        0        0     1873 2023-04-25 17:11:34.000000 text2graphapi-0.1.5/text2graphapi/src/Utils.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/src/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-04-25 17:11:34.000000 text2graphapi-0.1.5/text2graphapi/src/configs.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.178056 text2graphapi-0.1.5/text2graphapi/src/resources/
+-rw-rw-rw-   0        0        0     4160 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_english.txt
+-rw-rw-rw-   0        0        0     5256 2023-03-08 18:09:28.000000 text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_french.txt
+-rw-rw-rw-   0        0        0     4852 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_spanish.txt
+-rw-rw-rw-   0        0        0     2248 2023-03-30 02:11:28.000000 text2graphapi-0.1.5/text2graphapi/testing.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.112273 text2graphapi-0.1.5/text2graphapi.egg-info/
+-rw-rw-rw-   0        0        0     5410 2023-04-27 14:19:55.000000 text2graphapi-0.1.5/text2graphapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-04-27 14:19:55.000000 text2graphapi-0.1.5/text2graphapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 14:19:55.000000 text2graphapi-0.1.5/text2graphapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-04-27 14:19:55.000000 text2graphapi-0.1.5/text2graphapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-27 14:19:55.000000 text2graphapi-0.1.5/text2graphapi.egg-info/top_level.txt
```

### Comparing `text2graphapi-0.1.4/LICENSE.txt` & `text2graphapi-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/PKG-INFO` & `text2graphapi-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2graphapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Use this library to transform raw text into differents graph representations.
 Home-page: UNKNOWN
 Author: PLN-disca-iimas
 Author-email: andric.valdez@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `text2graphapi-0.1.4/README.md` & `text2graphapi-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/docs/_build/html/_sources/Cooocurrence.rst.txt` & `text2graphapi-0.1.5/docs/_build/html/_sources/Cooocurrence.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/docs/_build/html/_sources/index.rst.txt` & `text2graphapi-0.1.5/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/docs/conf.py` & `text2graphapi-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/notes.txt` & `text2graphapi-0.1.5/notes.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/setup.py` & `text2graphapi-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ROOT = path.abspath(path.dirname(__file__))
 
 with open(path.join(ROOT, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="text2graphapi",
-    version="0.1.4",
+    version="0.1.5",
     description="Use this library to transform raw text into differents graph representations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="PLN-disca-iimas",
     author_email="andric.valdez@gmail.com",
     license="MIT",
```

### Comparing `text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt` & `text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt` & `text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/docs/build/html/_sources/index.rst.txt` & `text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/docs/source/conf.py` & `text2graphapi-0.1.5/text2graphapi/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/main.py` & `text2graphapi-0.1.5/text2graphapi/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,22 +19,23 @@
 # *** Logging configs
 logging.basicConfig(stream=sys.stdout, level=logging.INFO, format="%(asctime)s; - %(levelname)s; - %(message)s")
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 # *** Configs
 ROOT_DIR = os.path.dirname(os.path.dirname(__file__))
-TEST_API_FROM = 'LOCAL' #posible values: LOCAL, PYPI
+TEST_API_FROM = 'PYPY' #posible values: LOCAL, PYPI
 PRINT_NUM_OUTPUT_GRAPHS = 5
 
 
 
 # TEST API PYPI
 if TEST_API_FROM == 'PYPY':
     from text2graphapi.src.Cooccurrence  import Cooccurrence
+    from text2graphapi.src.Heterogeneous  import Heterogeneous
 # TEST API LOCAL
 else:
     from src.Cooccurrence import Cooccurrence
     from src.Heterogeneous import Heterogeneous
 
 
 def read_dataset(dataset, file):
```

### Comparing `text2graphapi-0.1.4/text2graphapi/src/Cooccurrence.py` & `text2graphapi-0.1.5/text2graphapi/src/Cooccurrence.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/src/Graph.py` & `text2graphapi-0.1.5/text2graphapi/src/Graph.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/src/GraphTransformation.py` & `text2graphapi-0.1.5/text2graphapi/src/GraphTransformation.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/src/Heterogeneous.py` & `text2graphapi-0.1.5/text2graphapi/src/Heterogeneous.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/src/Preprocessing.py` & `text2graphapi-0.1.5/text2graphapi/src/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/src/Utils.py` & `text2graphapi-0.1.5/text2graphapi/src/Utils.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_english.txt` & `text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_english.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_french.txt` & `text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_french.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/src/resources/stopwords_spanish.txt` & `text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_spanish.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi/testing.py` & `text2graphapi-0.1.5/text2graphapi/testing.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.4/text2graphapi.egg-info/PKG-INFO` & `text2graphapi-0.1.5/text2graphapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2graphapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Use this library to transform raw text into differents graph representations.
 Home-page: UNKNOWN
 Author: PLN-disca-iimas
 Author-email: andric.valdez@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `text2graphapi-0.1.4/text2graphapi.egg-info/SOURCES.txt` & `text2graphapi-0.1.5/text2graphapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


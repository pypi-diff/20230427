# Comparing `tmp/bigquery_ml_utils-0.1.1-py3-none-any.whl.zip` & `tmp/bigquery_ml_utils-0.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,21 @@
-Zip file size: 15038 bytes, number of entries: 11
--rw-r--r--  2.0 unx      694 b- defN 23-Mar-28 19:15 bigquery_ml_utils/__init__.py
--rw-r--r--  2.0 unx      575 b- defN 23-Mar-28 19:15 bigquery_ml_utils/inference/__init__.py
--rw-r--r--  2.0 unx      609 b- defN 23-Mar-28 19:15 bigquery_ml_utils/inference/transform_predictor/__init__.py
--rw-r--r--  2.0 unx     7631 b- defN 23-Mar-28 19:15 bigquery_ml_utils/inference/transform_predictor/predictor.py
--rw-r--r--  2.0 unx      609 b- defN 23-Mar-28 19:15 bigquery_ml_utils/inference/xgboost_predictor/__init__.py
--rw-r--r--  2.0 unx    19037 b- defN 23-Mar-28 19:15 bigquery_ml_utils/inference/xgboost_predictor/predictor.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-28 19:18 bigquery_ml_utils-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2575 b- defN 23-Mar-28 19:18 bigquery_ml_utils-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 19:18 bigquery_ml_utils-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Mar-28 19:18 bigquery_ml_utils-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1078 b- defN 23-Mar-28 19:18 bigquery_ml_utils-0.1.1.dist-info/RECORD
-11 files, 44275 bytes uncompressed, 13158 bytes compressed:  70.3%
+Zip file size: 1595297 bytes, number of entries: 19
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-27 21:18 bigquery_ml_utils.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-27 21:18 inference/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-27 21:18 bigquery_ml_utils-0.1.2.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-27 21:18 tensorflow_ops/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-27 21:18 inference/transform_predictor/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-27 21:18 inference/xgboost_predictor/
+-rw-r--r--  2.0 unx      575 b- defN 23-Apr-27 21:18 inference/__init__.py
+-rw-r--r--  2.0 unx      609 b- defN 23-Apr-27 21:18 inference/transform_predictor/__init__.py
+-rw-r--r--  2.0 unx     7631 b- defN 23-Apr-27 21:18 inference/transform_predictor/predictor.py
+-rw-r--r--  2.0 unx      609 b- defN 23-Apr-27 21:18 inference/xgboost_predictor/__init__.py
+-rw-r--r--  2.0 unx    19037 b- defN 23-Apr-27 21:18 inference/xgboost_predictor/predictor.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-27 21:18 bigquery_ml_utils-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      148 b- defN 23-Apr-27 21:18 bigquery_ml_utils-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx     2563 b- defN 23-Apr-27 21:18 bigquery_ml_utils-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-27 21:18 bigquery_ml_utils-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1178 b- defN 23-Apr-27 21:18 bigquery_ml_utils-0.1.2.dist-info/RECORD
+-rwxr-xr-x  2.0 unx  5749945 b- defN 23-Apr-27 21:18 tensorflow_ops/timestamp_ops.so
+-rw-r--r--  2.0 unx      575 b- defN 23-Apr-27 21:18 tensorflow_ops/__init__.py
+-rw-r--r--  2.0 unx     1720 b- defN 23-Apr-27 21:18 tensorflow_ops/timestamp_ops.py
+19 files, 5795972 bytes uncompressed, 1592591 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -1,34 +1,58 @@
-Filename: bigquery_ml_utils/__init__.py
+Filename: bigquery_ml_utils.libs/
 Comment: 
 
-Filename: bigquery_ml_utils/inference/__init__.py
+Filename: inference/
 Comment: 
 
-Filename: bigquery_ml_utils/inference/transform_predictor/__init__.py
+Filename: bigquery_ml_utils-0.1.2.dist-info/
 Comment: 
 
-Filename: bigquery_ml_utils/inference/transform_predictor/predictor.py
+Filename: tensorflow_ops/
 Comment: 
 
-Filename: bigquery_ml_utils/inference/xgboost_predictor/__init__.py
+Filename: inference/transform_predictor/
 Comment: 
 
-Filename: bigquery_ml_utils/inference/xgboost_predictor/predictor.py
+Filename: inference/xgboost_predictor/
 Comment: 
 
-Filename: bigquery_ml_utils-0.1.1.dist-info/LICENSE
+Filename: inference/__init__.py
 Comment: 
 
-Filename: bigquery_ml_utils-0.1.1.dist-info/METADATA
+Filename: inference/transform_predictor/__init__.py
 Comment: 
 
-Filename: bigquery_ml_utils-0.1.1.dist-info/WHEEL
+Filename: inference/transform_predictor/predictor.py
 Comment: 
 
-Filename: bigquery_ml_utils-0.1.1.dist-info/top_level.txt
+Filename: inference/xgboost_predictor/__init__.py
 Comment: 
 
-Filename: bigquery_ml_utils-0.1.1.dist-info/RECORD
+Filename: inference/xgboost_predictor/predictor.py
+Comment: 
+
+Filename: bigquery_ml_utils-0.1.2.dist-info/LICENSE
+Comment: 
+
+Filename: bigquery_ml_utils-0.1.2.dist-info/WHEEL
+Comment: 
+
+Filename: bigquery_ml_utils-0.1.2.dist-info/METADATA
+Comment: 
+
+Filename: bigquery_ml_utils-0.1.2.dist-info/top_level.txt
+Comment: 
+
+Filename: bigquery_ml_utils-0.1.2.dist-info/RECORD
+Comment: 
+
+Filename: tensorflow_ops/timestamp_ops.so
+Comment: 
+
+Filename: tensorflow_ops/__init__.py
+Comment: 
+
+Filename: tensorflow_ops/timestamp_ops.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `bigquery_ml_utils/__init__.py` & `inference/transform_predictor/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,9 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from bigquery_ml_utils.inference import transform_predictor
-from bigquery_ml_utils.inference import xgboost_predictor
+from .predictor import Predictor
```

## Comparing `bigquery_ml_utils/inference/__init__.py` & `inference/__init__.py`

 * *Files identical despite different names*

## Comparing `bigquery_ml_utils/inference/transform_predictor/__init__.py` & `inference/xgboost_predictor/__init__.py`

 * *Files identical despite different names*

## Comparing `bigquery_ml_utils/inference/transform_predictor/predictor.py` & `inference/transform_predictor/predictor.py`

 * *Files identical despite different names*

## Comparing `bigquery_ml_utils/inference/xgboost_predictor/__init__.py` & `tensorflow_ops/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from .predictor import Predictor
```

## Comparing `bigquery_ml_utils/inference/xgboost_predictor/predictor.py` & `inference/xgboost_predictor/predictor.py`

 * *Files identical despite different names*

## Comparing `bigquery_ml_utils-0.1.1.dist-info/LICENSE` & `bigquery_ml_utils-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bigquery_ml_utils-0.1.1.dist-info/METADATA` & `bigquery_ml_utils-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: bigquery-ml-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: BigQuery ML Utils
 Home-page: https://github.com/GoogleCloudPlatform/bigquery-ml-utils
 Author: Google Inc.
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: bqml utils
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: xgboost
 Requires-Dist: numpy
-Requires-Dist: tensorflow
+Requires-Dist: tensorflow (>=2.1.0)
 
 # BigQuery ML Utils
 
 [BigQuery ML](https://cloud.google.com/bigquery-ml/docs/introduction) (aka.
 BQML) lets you create and execute machine learning models in [BigQuery](https://cloud.google.com/bigquery/docs/introduction)
 using standard SQL queries. The BigQuery ML Utils library is an integrated suite
 of machine learning tools for building and using BigQuery ML models.
```


# Comparing `tmp/metal_sdk-1.0.0.tar.gz` & `tmp/metal_sdk-1.0.1.tar.gz`

## Comparing `metal_sdk-1.0.0.tar` & `metal_sdk-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/examples/example.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/examples/example_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/src/metal_sdk/metal.py
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/src/metal_sdk/metal_async.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/tests/test_metal.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/tests/test_metal_async.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/LICENSE
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/examples/example.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/examples/example_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/src/metal_sdk/metal.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/src/metal_sdk/metal_async.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/tests/test_metal.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/tests/test_metal_async.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/LICENSE
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/PKG-INFO
```

### Comparing `metal_sdk-1.0.0/.github/workflows/publish.yml` & `metal_sdk-1.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.0/.github/workflows/test.yml` & `metal_sdk-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.0/examples/example.py` & `metal_sdk-1.0.1/examples/example.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.0/examples/example_async.py` & `metal_sdk-1.0.1/examples/example_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.0/src/metal_sdk/metal.py` & `metal_sdk-1.0.1/src/metal_sdk/metal.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         data = {"index": index}
         if payload.get("id") is not None:
             data["id"] = payload["id"]
 
         if payload.get("metadata") is not None:
             data["metadata"] = payload["metadata"]
 
+        if payload.get("filters") is not None:
+            data["filters"] = payload["filters"]
+
         if payload.get("imageBase64") is not None:
             data["imageBase64"] = payload["imageBase64"]
         elif payload.get("imageUrl") is not None:
             data["imageUrl"] = payload["imageUrl"]
         elif payload.get("text") is not None:
             data["text"] = payload["text"]
         elif payload.get("embedding") is not None:
```

### Comparing `metal_sdk-1.0.0/src/metal_sdk/metal_async.py` & `metal_sdk-1.0.1/src/metal_sdk/metal_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         data = {"index": index}
         if payload.get("id") is not None:
             data["id"] = payload["id"]
 
         if payload.get("metadata") is not None:
             data["metadata"] = payload["metadata"]
 
+        if payload.get("filters") is not None:
+            data["filters"] = payload["filters"]
+
         if payload.get("imageBase64") is not None:
             data["imageBase64"] = payload["imageBase64"]
         elif payload.get("imageUrl") is not None:
             data["imageUrl"] = payload["imageUrl"]
         elif payload.get("text") is not None:
             data["text"] = payload["text"]
         elif payload.get("embedding") is not None:
```

### Comparing `metal_sdk-1.0.0/src/metal_sdk/typings.py` & `metal_sdk-1.0.1/src/metal_sdk/typings.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,18 +15,24 @@
     imageBase64: NotRequired[str]
     imageUrl: NotRequired[str]
     text: NotRequired[str]
     embedding: NotRequired[List[float]]
     metadata: NotRequired[dict]
 
 
+class SearchFilter(TypedDict):
+    field: str
+    value: str | int | float
+
+
 class SearchPayload(TypedDict):
     imageBase64: NotRequired[str]
     imageUrl: NotRequired[str]
     text: NotRequired[str]
     embedding: NotRequired[List[float]]
+    filters: NotRequired[List[SearchFilter]]
 
 
 class TunePayload(TypedDict):
     idA: str
     idB: str
     label: TuneLabel
```

### Comparing `metal_sdk-1.0.0/tests/test_metal.py` & `metal_sdk-1.0.1/tests/test_metal.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             metal.search()
         self.assertEqual(
             str(ctx.exception), "imageBase64, imageUrl, text, or embedding required"
         )
 
     def test_metal_search_with_text(self):
         my_index = "my-index"
-        payload = {"text": "some text"}
+        payload = {"text": "some text", "filters": [{"field": "number_of_the_beast", "value": 666}]}
 
         metal = Metal(API_KEY, CLIENT_ID, my_index)
 
         metal.request = mock.MagicMock(return_value=mock.Mock(status_code=201))
 
         metal.search(payload, ids_only=True)
 
@@ -85,14 +85,15 @@
         )
         self.assertEqual(
             metal.request.call_args[0][1],
             "/v1/search?limit=1&idsOnly=true",
         )
         self.assertEqual(metal.request.call_args[1]["json"]["index"], my_index)
         self.assertEqual(metal.request.call_args[1]["json"]["text"], payload["text"])
+        self.assertEqual(metal.request.call_args[1]["json"]["filters"], payload["filters"])
 
     def test_metal_tune_without_index(self):
         metal = Metal(API_KEY, CLIENT_ID)
         with self.assertRaises(TypeError) as ctx:
             metal.tune()
         self.assertEqual(str(ctx.exception), "index_id required")
```

### Comparing `metal_sdk-1.0.0/tests/test_metal_async.py` & `metal_sdk-1.0.1/tests/test_metal_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.0/.gitignore` & `metal_sdk-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.0/LICENSE` & `metal_sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.0/README.md` & `metal_sdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.0/pyproject.toml` & `metal_sdk-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metal_sdk"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Metal Technologies Inc", email="james@getmetal.io" },
 ]
 description = "SDK for getmetal.io"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `metal_sdk-1.0.0/PKG-INFO` & `metal_sdk-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal_sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: SDK for getmetal.io
 Project-URL: Github, https://github.com/getmetal/metal-python
 Author-email: Metal Technologies Inc <james@getmetal.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```


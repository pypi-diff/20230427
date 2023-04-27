# Comparing `tmp/data_snack-0.3.0.tar.gz` & `tmp/data_snack-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_snack-0.3.0.tar", last modified: Wed Apr 12 14:33:01 2023, max compression
+gzip compressed data, was "data_snack-0.3.1.tar", last modified: Thu Apr 27 13:32:56 2023, max compression
```

## Comparing `data_snack-0.3.0.tar` & `data_snack-0.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:01.720178 data_snack-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 14:32:52.000000 data_snack-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 14:32:52.000000 data_snack-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-12 14:33:01.720178 data_snack-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-12 14:32:52.000000 data_snack-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 14:32:52.000000 data_snack-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 14:32:52.000000 data_snack-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-12 14:33:01.724178 data_snack-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-12 14:32:52.000000 data_snack-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:01.708178 data_snack-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:01.712178 data_snack-0.3.0/src/data_snack/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:01.716178 data_snack-0.3.0/src/data_snack/connections/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/connections/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/connections/memcached.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/connections/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:01.716178 data_snack-0.3.0/src/data_snack/entities/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/entities/entity_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/entities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/entities/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/entities/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:01.720178 data_snack-0.3.0/src/data_snack/key_factories/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/key_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/key_factories/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/key_factories/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/key_factories/non_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:01.720178 data_snack-0.3.0/src/data_snack/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/serializers/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/snack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:01.720178 data_snack-0.3.0/src/data_snack/wrap/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/wrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/wrap/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/wrap/data_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/wrap/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 14:32:52.000000 data_snack-0.3.0/src/data_snack/wrap/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:01.716178 data_snack-0.3.0/src/data_snack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-12 14:33:01.000000 data_snack-0.3.0/src/data_snack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-12 14:33:01.000000 data_snack-0.3.0/src/data_snack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:33:01.000000 data_snack-0.3.0/src/data_snack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 14:33:01.000000 data_snack-0.3.0/src/data_snack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 14:33:01.000000 data_snack-0.3.0/src/data_snack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:32:56.713307 data_snack-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 13:32:45.000000 data_snack-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 13:32:45.000000 data_snack-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-27 13:32:56.713307 data_snack-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-27 13:32:45.000000 data_snack-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 13:32:45.000000 data_snack-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 13:32:45.000000 data_snack-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-27 13:32:56.717307 data_snack-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-27 13:32:45.000000 data_snack-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:32:56.701307 data_snack-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:32:56.705308 data_snack-0.3.1/src/data_snack/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:32:56.709308 data_snack-0.3.1/src/data_snack/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/connections/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/connections/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/connections/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:32:56.713307 data_snack-0.3.1/src/data_snack/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/entities/entity_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/entities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/entities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/entities/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:32:56.713307 data_snack-0.3.1/src/data_snack/key_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/key_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/key_factories/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/key_factories/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/key_factories/non_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:32:56.713307 data_snack-0.3.1/src/data_snack/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/serializers/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/snack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:32:56.713307 data_snack-0.3.1/src/data_snack/wrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/wrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/wrap/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/wrap/data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/wrap/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 13:32:45.000000 data_snack-0.3.1/src/data_snack/wrap/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:32:56.709308 data_snack-0.3.1/src/data_snack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-27 13:32:56.000000 data_snack-0.3.1/src/data_snack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-27 13:32:56.000000 data_snack-0.3.1/src/data_snack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:32:56.000000 data_snack-0.3.1/src/data_snack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 13:32:56.000000 data_snack-0.3.1/src/data_snack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 13:32:56.000000 data_snack-0.3.1/src/data_snack.egg-info/top_level.txt
```

### Comparing `data_snack-0.3.0/LICENSE` & `data_snack-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/PKG-INFO` & `data_snack-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_snack
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/webinterpret-ds/data-snack
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `data_snack-0.3.0/README.md` & `data_snack-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/setup.cfg` & `data_snack-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data-snack
-version = 0.3.0
+version = 0.3.1
 author = webinterpret-datascience
 author_email = data-science@webinterpret.com
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/webinterpret-ds/data-snack
 project_urls =
```

### Comparing `data_snack-0.3.0/setup.py` & `data_snack-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/connections/base.py` & `data_snack-0.3.1/src/data_snack/connections/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/connections/memcached.py` & `data_snack-0.3.1/src/data_snack/connections/memcached.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/connections/redis.py` & `data_snack-0.3.1/src/data_snack/connections/redis.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/entities/entity.py` & `data_snack-0.3.1/src/data_snack/entities/entity.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/entities/entity_meta.py` & `data_snack-0.3.1/src/data_snack/entities/entity_meta.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/entities/schema.py` & `data_snack-0.3.1/src/data_snack/entities/schema.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/key_factories/base.py` & `data_snack-0.3.1/src/data_snack/key_factories/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/serializers/base.py` & `data_snack-0.3.1/src/data_snack/serializers/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/serializers/dataclass.py` & `data_snack-0.3.1/src/data_snack/serializers/dataclass.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/snack.py` & `data_snack-0.3.1/src/data_snack/snack.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/wrap/base.py` & `data_snack-0.3.1/src/data_snack/wrap/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack/wrap/data_frame.py` & `data_snack-0.3.1/src/data_snack/wrap/data_frame.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,8 +34,18 @@
         required_key_columns = self.entity_type.get_keys()
         if missing_columns := set(required_key_columns) - set(df.columns):
             raise DataFrameMissingKeyColumn(
                 f"Provided data frame is missing columns: {missing_columns}"
             )
 
         data = self.get_many(df[required_key_columns].values.tolist())
-        return pd.DataFrame([asdict(row) if row else {} for row in data])
+        output_df = pd.DataFrame(
+            [row for row in data if row],
+            columns=self.entity_type.get_all_fields()
+        )
+
+        return pd.merge(
+            df,
+            output_df,
+            on=required_key_columns,
+            how='left'
+        )
```

### Comparing `data_snack-0.3.0/src/data_snack/wrap/entity.py` & `data_snack-0.3.1/src/data_snack/wrap/entity.py`

 * *Files identical despite different names*

### Comparing `data_snack-0.3.0/src/data_snack.egg-info/PKG-INFO` & `data_snack-0.3.1/src/data_snack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-snack
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/webinterpret-ds/data-snack
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `data_snack-0.3.0/src/data_snack.egg-info/SOURCES.txt` & `data_snack-0.3.1/src/data_snack.egg-info/SOURCES.txt`

 * *Files identical despite different names*


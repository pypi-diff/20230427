# Comparing `tmp/pydantic_enhanced_serializer-1.1.0-py3-none-any.whl.zip` & `tmp/pydantic_enhanced_serializer-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 15782 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      309 b- defN 23-Mar-08 23:12 pydantic_enhanced_serializer/__init__.py
--rw-r--r--  2.0 unx     9416 b- defN 23-Mar-08 23:41 pydantic_enhanced_serializer/fieldsets.py
+-rw-r--r--  2.0 unx     9424 b- defN 23-Apr-27 05:29 pydantic_enhanced_serializer/fieldsets.py
 -rw-r--r--  2.0 unx     2724 b- defN 23-Mar-08 23:35 pydantic_enhanced_serializer/models.py
 -rw-r--r--  2.0 unx     3960 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/path_put.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/py.typed
 -rw-r--r--  2.0 unx     4222 b- defN 23-Mar-08 23:32 pydantic_enhanced_serializer/render.py
 -rw-r--r--  2.0 unx     6996 b- defN 23-Apr-13 21:29 pydantic_enhanced_serializer/schema.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/integrations/__init__.py
 -rw-r--r--  2.0 unx     1401 b- defN 23-Mar-08 23:47 pydantic_enhanced_serializer/integrations/django_ninja.py
 -rw-r--r--  2.0 unx     6078 b- defN 23-Mar-08 23:14 pydantic_enhanced_serializer/integrations/fastapi.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Apr-13 21:52 pydantic_enhanced_serializer-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6021 b- defN 23-Apr-13 21:52 pydantic_enhanced_serializer-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 21:52 pydantic_enhanced_serializer-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       29 b- defN 23-Apr-13 21:52 pydantic_enhanced_serializer-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1488 b- defN 23-Apr-13 21:52 pydantic_enhanced_serializer-1.1.0.dist-info/RECORD
-15 files, 43809 bytes uncompressed, 13224 bytes compressed:  69.8%
+-rw-r--r--  2.0 unx     1073 b- defN 23-Apr-27 05:34 pydantic_enhanced_serializer-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6021 b- defN 23-Apr-27 05:34 pydantic_enhanced_serializer-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 05:34 pydantic_enhanced_serializer-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       29 b- defN 23-Apr-27 05:34 pydantic_enhanced_serializer-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1488 b- defN 23-Apr-27 05:34 pydantic_enhanced_serializer-1.1.1.dist-info/RECORD
+15 files, 43817 bytes uncompressed, 13224 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pydantic_enhanced_serializer/integrations/django_ninja.py
 Comment: 
 
 Filename: pydantic_enhanced_serializer/integrations/fastapi.py
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.0.dist-info/LICENSE
+Filename: pydantic_enhanced_serializer-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.0.dist-info/METADATA
+Filename: pydantic_enhanced_serializer-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.0.dist-info/WHEEL
+Filename: pydantic_enhanced_serializer-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.0.dist-info/top_level.txt
+Filename: pydantic_enhanced_serializer-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.0.dist-info/RECORD
+Filename: pydantic_enhanced_serializer-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pydantic_enhanced_serializer/fieldsets.py

```diff
@@ -167,15 +167,15 @@
 
             elif field_obj.shape in MAPPING_SHAPES:
                 # Field is a dict, values may or may not contain models
                 # or nested dicts/lists of models
                 if field not in current_includes_ptr:
                     current_includes_ptr[field] = {}
 
-                for key, value in getattr(model, field_obj.name).items():
+                for key, value in (getattr(model, field_obj.name) or {}).items():
                     sub_includes, sub_expansions = fieldset_to_includes(
                         subfields, value, path + [field, key]
                     )
 
                     current_includes_ptr[field][key] = sub_includes
                     expansions.update(sub_expansions)
```

## Comparing `pydantic_enhanced_serializer-1.1.0.dist-info/LICENSE` & `pydantic_enhanced_serializer-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pydantic_enhanced_serializer-1.1.0.dist-info/METADATA` & `pydantic_enhanced_serializer-1.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-enhanced-serializer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Pydantic extension that allows user selection of object fields or expansions inline when serializing models
 Home-page: https://github.com/adamsussman/pydantic-enhanced-serializer
 Author: Adam Sussman
 Author-email: adam.sussman@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
```

## Comparing `pydantic_enhanced_serializer-1.1.0.dist-info/RECORD` & `pydantic_enhanced_serializer-1.1.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pydantic_enhanced_serializer/__init__.py,sha256=YDA4Ntaq4mBBR0nDyHFXlvqE_OWJ6mzsCHlxjX71nYc,309
-pydantic_enhanced_serializer/fieldsets.py,sha256=beBS5m3KAyOqmyOhoU9qenIKIF3F-SP3Ss3HsmBHbXA,9416
+pydantic_enhanced_serializer/fieldsets.py,sha256=YU94v7aW5dDNkGmhZXkWYlCKb2up1iXKsYaoPPKApNc,9424
 pydantic_enhanced_serializer/models.py,sha256=ZGoQZ9cHTT9icObGvfWFkeBYRSQUKYYbligdsiDvX94,2724
 pydantic_enhanced_serializer/path_put.py,sha256=CPqpjErHgzvipU6B326A-XpSbhTtWJzGeV9UODzMUjY,3960
 pydantic_enhanced_serializer/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pydantic_enhanced_serializer/render.py,sha256=OsnGmTjDr93Xi1vYWcM5YgNDpsZbpsAa5Ct724-BxBw,4222
 pydantic_enhanced_serializer/schema.py,sha256=p3kUgONZMZ3qMdoCw7qMYgQHjHL39I2kh39fT_gwaks,6996
 pydantic_enhanced_serializer/integrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pydantic_enhanced_serializer/integrations/django_ninja.py,sha256=Z60LR0vfM4wbpvWo_qfEhcsUn4ufXU80xwD4zbPGIdI,1401
 pydantic_enhanced_serializer/integrations/fastapi.py,sha256=6qBNdbafvEAmVDBVS0h_AedDnevh_Ilv3bztF3pcYHY,6078
-pydantic_enhanced_serializer-1.1.0.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
-pydantic_enhanced_serializer-1.1.0.dist-info/METADATA,sha256=e2yGk8ACb6cyr30jglEslf0tRD5XpUnzoBFb1ijwvao,6021
-pydantic_enhanced_serializer-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pydantic_enhanced_serializer-1.1.0.dist-info/top_level.txt,sha256=QCypSWZi8vRHdmuu-4xOAqUWN78nQShuGw0yMB4RLI4,29
-pydantic_enhanced_serializer-1.1.0.dist-info/RECORD,,
+pydantic_enhanced_serializer-1.1.1.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
+pydantic_enhanced_serializer-1.1.1.dist-info/METADATA,sha256=D0ceLYIqy6OSFWziAzHZj2VmLb4g6JIM4dVOM3uj_kw,6021
+pydantic_enhanced_serializer-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pydantic_enhanced_serializer-1.1.1.dist-info/top_level.txt,sha256=QCypSWZi8vRHdmuu-4xOAqUWN78nQShuGw0yMB4RLI4,29
+pydantic_enhanced_serializer-1.1.1.dist-info/RECORD,,
```


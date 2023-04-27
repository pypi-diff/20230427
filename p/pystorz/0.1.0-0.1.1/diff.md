# Comparing `tmp/pystorz-0.1.0.tar.gz` & `tmp/pystorz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystorz-0.1.0.tar", last modified: Tue Apr 25 04:15:02 2023, max compression
+gzip compressed data, was "dist/pystorz-0.1.1.tar", last modified: Wed Apr 26 20:42:18 2023, max compression
```

## Comparing `pystorz-0.1.0.tar` & `pystorz-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.588432 pystorz-0.1.0/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.1.0/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-25 04:15:02.588205 pystorz-0.1.0/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     1133 2023-04-24 16:29:08.000000 pystorz-0.1.0/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.581787 pystorz-0.1.0/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.1.0/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.582994 pystorz-0.1.0/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.1.0/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.1.0/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.584460 pystorz-0.1.0/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.1.0/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.1.0/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4070 2023-04-25 04:09:44.000000 pystorz-0.1.0/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.586251 pystorz-0.1.0/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.1.0/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.1.0/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)      846 2023-04-25 04:12:40.000000 pystorz-0.1.0/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.1.0/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.586549 pystorz-0.1.0/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.1.0/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     9486 2023-04-25 03:48:50.000000 pystorz-0.1.0/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.587818 pystorz-0.1.0/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.1.0/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2295 2023-04-25 03:51:35.000000 pystorz-0.1.0/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4297 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-24 16:09:14.000000 pystorz-0.1.0/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2368 2023-04-25 03:46:31.000000 pystorz-0.1.0/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.582682 pystorz-0.1.0/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-25 04:15:02.000000 pystorz-0.1.0/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-25 04:15:02.000000 pystorz-0.1.0/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-25 04:15:02.000000 pystorz-0.1.0/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-25 04:15:02.000000 pystorz-0.1.0/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-25 04:15:02.000000 pystorz-0.1.0/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-25 04:15:02.588484 pystorz-0.1.0/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-25 04:14:50.000000 pystorz-0.1.0/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-26 20:42:18.653394 pystorz-0.1.1/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.1.1/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-04-26 20:42:18.653128 pystorz-0.1.1/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     2558 2023-04-26 01:57:49.000000 pystorz-0.1.1/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-26 20:42:18.643858 pystorz-0.1.1/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.1.1/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-26 20:42:18.645404 pystorz-0.1.1/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.1.1/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.1.1/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-26 20:42:18.647213 pystorz-0.1.1/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.1.1/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.1.1/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4153 2023-04-26 18:27:43.000000 pystorz-0.1.1/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-26 20:42:18.650661 pystorz-0.1.1/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.1.1/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.1.1/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.1.1/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.1.1/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.1.1/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.1.1/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      846 2023-04-25 04:12:40.000000 pystorz-0.1.1/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.1.1/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.1.1/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.1.1/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-26 20:42:18.651096 pystorz-0.1.1/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.1.1/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     9842 2023-04-26 20:41:12.000000 pystorz-0.1.1/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-26 20:42:18.652665 pystorz-0.1.1/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.1.1/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.1.1/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4297 2023-04-24 14:15:03.000000 pystorz-0.1.1/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-24 16:09:14.000000 pystorz-0.1.1/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2878 2023-04-26 20:32:53.000000 pystorz-0.1.1/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-26 20:42:18.644908 pystorz-0.1.1/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-04-26 20:42:18.000000 pystorz-0.1.1/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-26 20:42:18.000000 pystorz-0.1.1/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-26 20:42:18.000000 pystorz-0.1.1/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-26 20:42:18.000000 pystorz-0.1.1/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-26 20:42:18.000000 pystorz-0.1.1/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-26 20:42:18.653473 pystorz-0.1.1/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-26 20:41:32.000000 pystorz-0.1.1/setup.py
```

### Comparing `pystorz-0.1.0/LICENSE` & `pystorz-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.0/pystorz/mgen/builder.py` & `pystorz-0.1.1/pystorz/mgen/builder.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.0/pystorz/mgen/loader.py` & `pystorz-0.1.1/pystorz/mgen/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,22 +81,22 @@
 
     for y in yamls:
         model = read_model(y)
 
         # log.debug("model: {}".format(jopp(model)))
 
         for m in model["types"]:
-            if m["kind"] == "Struct":
+            if m["kind"].lower() == "struct":
                 if m["name"] in struct_cache:
                     raise Exception("duplicate struct: {}".format(m["name"]))
                 struct_cache.add(m["name"])
 
                 structs.append(Struct(m["name"], "", capitalize_props(m["properties"])))
                 continue
-            if m["kind"] == "Object":
+            if m["kind"].lower() == "object":
                 if m["name"] in resource_cache:
                     raise Exception("duplicate object: {}".format(m["name"]))
                 resource_cache.add(m["name"])
 
                 pkey = "metadata.identity"
                 if "primarykey" in m:
                     pkey = m["primarykey"]
@@ -108,14 +108,16 @@
                 intr = None
                 if "internal" in m:
                     intr = m["internal"]
 
                 resources.append(Resource(m["name"], ext, intr, pkey))
                 continue
 
+            raise Exception("unknown kind: {}".format(m["kind"]))
+
     return structs, resources
 
 
 def read_model(path: str):
     log.debug(f"reading model from {path}")
 
     with open(path, "r") as f:
```

### Comparing `pystorz-0.1.0/pystorz/mgen/templates/structure.py` & `pystorz-0.1.1/pystorz/mgen/templates/structure.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.0/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.1.1/pystorz/mgen/templates/unmarshall.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.0/pystorz/mgen/test.py` & `pystorz-0.1.1/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.0/pystorz/mgen/utils.py` & `pystorz-0.1.1/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.0/pystorz/sql/store.py` & `pystorz-0.1.1/pystorz/sql/store.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         if existing is not None:
             raise Exception(constants.ErrObjectExists)
 
         self.TestConnection()
 
         obj.Metadata().SetCreated(datetime.now())
         obj.Metadata().SetUpdated(obj.Metadata().Created())
+        obj.Metadata().SetRevision(1)
 
         self._setIdentity(
             obj.Metadata().Identity().Path(),
             obj.PrimaryKey(),
             obj.Metadata().Kind())
 
         self._setObject(obj.PrimaryKey(), obj.Metadata().Kind(), obj)
@@ -94,14 +95,15 @@
                           obj.PrimaryKey(), obj.Metadata().Kind())
 
         self._removeObject(existing.PrimaryKey(),
                            existing.Metadata().Kind())
 
         obj.Metadata().SetCreated(existing.Metadata().Created())
         obj.Metadata().SetUpdated(datetime.now())
+        obj.Metadata().SetRevision(existing.Metadata().Revision() + 1)
 
         self._setObject(obj.PrimaryKey(), obj.Metadata().Kind(), obj)
 
         return obj.Clone()
 
     def Delete(self, identity, *opt):
         log.info("delete {}".format(identity.Path()))
@@ -165,15 +167,16 @@
         if copt.prop_filter is not None:
             obj = self.Schema.ObjectForKind(identity.Type())
             if obj is None:
                 raise Exception(constants.ErrNoSuchObject)
             if utils.object_path(obj, copt.prop_filter.key) is None:
                 raise Exception(constants.ErrInvalidFilter)
             query = query + " AND json_extract(Object, '$.{}') = '{}'".format(
-                copt.prop_filter.key, copt.prop_filter.value)
+                copt.prop_filter.key, 
+                utils.encode_string(copt.prop_filter.value))
 
         if copt.order_by is not None and len(copt.order_by) > 0:
             query = """SELECT Object FROM Objects 
             WHERE Type = '{}'
             ORDER BY json_extract(Object, '$.{}')""".format(
                 identity.Type(), copt.order_by)
             if copt.order_incremental is None or copt.order_incremental:
@@ -258,28 +261,31 @@
         WHERE Pkey='{}' AND Type='{}'""".format(
             pkey, typ.lower())
         cursor = self._do_query(query)
         result = cursor.fetchone()
 
         if result is not None:
             data = result[0]
+            data = utils.decode_string(data)
             return self._parseObjectRow(data, typ)
         else:
             raise Exception(constants.ErrNoSuchObject)
 
     def _setObject(self, pkey, typ, obj):
         query = ""
         existing_obj = None
 
         try:
             existing_obj = self._getObject(pkey, typ)
         except Exception as e:
             log.debug("object get failed: {}".format(e))
 
         data = obj.ToJson()
+        # encode the data so it doesn't contain any SQL unfriendly characters
+        data = utils.encode_string(data)
 
         if existing_obj is not None:
             query = """UPDATE Objects SET Object='{}'
             WHERE Pkey = '{}' AND Type = '{}'""".format(data, pkey, typ.lower())
         else:
             query = """INSERT INTO Objects (Object, Pkey, Type)
             VALUES ('{}', '{}', '{}')""".format(data, pkey, typ.lower())
@@ -299,15 +305,16 @@
 
     def _parseObjectRow(self, data, typ):
         return utils.unmarshal_object(data, self.Schema, typ)
 
     def _parseObjectRows(self, rows, typ):
         res = []
         for row in rows:
-            res.append(self._parseObjectRow(row[0], typ))
+            data = utils.decode_string(row[0])
+            res.append(self._parseObjectRow(data, typ))
         return res
 
     def _do_query(self, query):
         cursor = self.DB.cursor()
 
         log.debug("running query: {}".format(query))
```

### Comparing `pystorz-0.1.0/pystorz/store/meta.py` & `pystorz-0.1.1/pystorz/store/meta.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
     def Created(self) -> datetime:
         pass
 
     def Updated(self) -> datetime:
         pass
 
+    def Revision(self) -> int:
+        pass
+
     def ToJson(self) -> str:
         pass
 
     def FromDict(self, d: dict) -> None:
         pass
 
     def ToDict(self) -> str:
@@ -29,28 +32,32 @@
 class MetaSetter:
     def SetKind(self, kind: str) -> None:
         pass
 
     def SetIdentity(self, identity: store.ObjectIdentity) -> None:
         pass
 
-    def SetCreated(self, created: str) -> None:
+    def SetCreated(self, created: datetime) -> None:
+        pass
+
+    def SetUpdated(self, updated: datetime) -> None:
         pass
 
-    def SetUpdated(self, updated: str) -> None:
+    def SetRevision(self, revision: int) -> None:
         pass
 
 
 # class MetaHolder:
 #     def metadata(self) -> Meta:
 #         pass
 
 
 class metaWrapper(Meta, MetaSetter):
     def __init__(self, kind):
+        self.revision_ = 0
         self.kind_ = kind
         self.identity_ = store.ObjectIdentityFactory()
         self.created_ = ""
         self.updated_ = ""
 
     def Kind(self) -> str:
         return self.kind_
@@ -60,41 +67,49 @@
 
     def Updated(self) -> datetime:
         return utils.datetime_parse(self.updated_)
 
     def Identity(self) -> store.ObjectIdentity:
         return self.identity_
 
+    def Revision(self) -> int:
+        return self.revision_
+
     def SetKind(self, kind: str) -> None:
         self.kind_ = kind
 
     def SetIdentity(self, identity: store.ObjectIdentity) -> None:
         self.identity_ = identity
 
     def SetCreated(self, created: datetime) -> None:
         self.created_ = utils.datetime_string(created)
 
     def SetUpdated(self, updated: datetime) -> None:
         self.updated_ = utils.datetime_string(updated)
 
+    def SetRevision(self, revision: int) -> None:
+        self.revision_ = revision
+
     def ToJson(self) -> str:
         return json.dumps(self.ToDict())
 
     def ToDict(self) -> str:
         return {
             "kind": self.Kind(),
             "identity": str(self.Identity()),
             "created": self.created_,
             "updated": self.updated_,
+            "revision": self.revision_,
         }
 
     def FromDict(self, d: dict) -> None:
         self.SetKind(d["kind"])
         self.SetIdentity(store.ObjectIdentityFactory())
         self.Identity().FromString(d["identity"])
         self.created_ = d["created"]
         self.updated_ = d["updated"]
+        self.revision_ = d["revision"]
 
 
 def MetaFactory(kind: str) -> Meta:
     return metaWrapper(kind)
```

### Comparing `pystorz-0.1.0/pystorz/store/options.py` & `pystorz-0.1.1/pystorz/store/options.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.0/pystorz/store/store.py` & `pystorz-0.1.1/pystorz/store/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.0/pystorz/store/utils.py` & `pystorz-0.1.1/pystorz/store/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import json
 import time
+import base64
 import logging
 import pathlib
+
 from jsonpath import JSONPath
 from datetime import datetime
 
 log = logging.getLogger(__name__)
 
 # import gabs
 
@@ -93,7 +95,19 @@
 
 def datetime_parse(dtstr) -> str:
     return datetime.strptime(dtstr, constants.DATETIME_FORMAT)
 
 
 def datetime_string(dt) -> str:
     return dt.strftime(constants.DATETIME_FORMAT)
+
+
+def encode_string(string):
+    return string.replace("'", "$%#")
+    # encoded_message = base64.b64encode(string.encode('utf-8'))  # Encode the message as base64 bytes
+    # return str(encoded_message, 'utf-8')  # Convert the bytes to a string
+
+
+def decode_string(soup):
+    return soup.replace("$%#", "'")
+    # encoded_message = bytes(soup, 'utf-8')  # Convert the soup to bytes
+    # return base64.b64decode(encoded_message).decode('utf-8')  # Decode the base64 bytes and convert to string
```

### Comparing `pystorz-0.1.0/pystorz.egg-info/SOURCES.txt` & `pystorz-0.1.1/pystorz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.0/setup.py` & `pystorz-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.1.0',
+    version='0.1.1',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
```


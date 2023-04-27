# Comparing `tmp/typegraph-0.1.5.tar.gz` & `tmp/typegraph-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegraph-0.1.5.tar", max compression
+gzip compressed data, was "typegraph-0.1.6.tar", max compression
```

## Comparing `typegraph-0.1.5.tar` & `typegraph-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     5252 2023-04-18 10:58:06.594397 typegraph-0.1.5/LICENSE.md
--rw-r--r--   0        0        0     1427 2023-04-18 10:58:06.594397 typegraph-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      225 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/__init__.py
--rw-r--r--   0        0        0      904 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/effects.py
--rw-r--r--   0        0        0     3323 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/auth/__init__.py
--rw-r--r--   0        0        0      377 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/auth/oauth2.py
--rw-r--r--   0        0        0     1868 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/builder.py
--rw-r--r--   0        0        0     3066 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/models.py
--rw-r--r--   0        0        0     1947 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/nodes.py
--rw-r--r--   0        0        0     5774 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/typegraph.py
--rw-r--r--   0        0        0     7955 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/importers/base/importer.py
--rw-r--r--   0        0        0     3667 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/importers/base/typify.py
--rw-r--r--   0        0        0     7499 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/importers/google_discovery.py
--rw-r--r--   0        0        0     4236 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/importers/graphql.py
--rw-r--r--   0        0        0     8909 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/importers/openapi.py
--rw-r--r--   0        0        0     4078 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/policies.py
--rw-r--r--   0        0        0     1675 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/aws/runtimes/s3.py
--rw-r--r--   0        0        0    28490 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/prisma/relations.py
--rw-r--r--   0        0        0    21712 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/prisma/runtimes/prisma.py
--rw-r--r--   0        0        0     6601 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/prisma/schema.py
--rw-r--r--   0        0        0    13927 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/prisma/type_generator.py
--rw-r--r--   0        0        0     2373 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/prisma/utils.py
--rw-r--r--   0        0        0     2209 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/temporal/runtimes/temporal.py
--rw-r--r--   0        0        0     1351 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/base.py
--rw-r--r--   0        0        0     5234 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/deno.py
--rw-r--r--   0        0        0     1403 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/graphql.py
--rw-r--r--   0        0        0     2789 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/http.py
--rw-r--r--   0        0        0     1352 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/python_wasi.py
--rw-r--r--   0        0        0     2880 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/random.py
--rw-r--r--   0        0        0     2053 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/typegate.py
--rw-r--r--   0        0        0     1169 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/wasmedge.py
--rw-r--r--   0        0        0    20231 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/types.py
--rw-r--r--   0        0        0      487 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/utils/__init__.py
--rw-r--r--   0        0        0      644 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/utils/attrs.py
--rw-r--r--   0        0        0     1977 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/utils/jsonschema.py
--rw-r--r--   0        0        0     2198 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/utils/loaders.py
--rw-r--r--   0        0        0      185 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/utils/sanitizers.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 typegraph-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     5252 2023-04-27 09:04:19.742183 typegraph-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0     1427 2023-04-27 09:04:19.742183 typegraph-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/__init__.py
+-rw-r--r--   0        0        0      904 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/effects.py
+-rw-r--r--   0        0        0     3323 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/auth/__init__.py
+-rw-r--r--   0        0        0      377 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/auth/oauth2.py
+-rw-r--r--   0        0        0     1868 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/builder.py
+-rw-r--r--   0        0        0     3066 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/models.py
+-rw-r--r--   0        0        0     1953 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/nodes.py
+-rw-r--r--   0        0        0     5774 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/typegraph.py
+-rw-r--r--   0        0        0     7955 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/importers/base/importer.py
+-rw-r--r--   0        0        0     3667 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/importers/base/typify.py
+-rw-r--r--   0        0        0     7499 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/importers/google_discovery.py
+-rw-r--r--   0        0        0     4236 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/importers/graphql.py
+-rw-r--r--   0        0        0     8909 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/importers/openapi.py
+-rw-r--r--   0        0        0     3904 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/injection.py
+-rw-r--r--   0        0        0     4338 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/policies.py
+-rw-r--r--   0        0        0     1675 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/aws/runtimes/s3.py
+-rw-r--r--   0        0        0    28490 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/prisma/relations.py
+-rw-r--r--   0        0        0    22924 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/prisma/runtimes/prisma.py
+-rw-r--r--   0        0        0     6601 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/prisma/schema.py
+-rw-r--r--   0        0        0    15008 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/prisma/type_generator.py
+-rw-r--r--   0        0        0     2373 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/prisma/utils.py
+-rw-r--r--   0        0        0     2209 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/temporal/runtimes/temporal.py
+-rw-r--r--   0        0        0     1351 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/runtimes/base.py
+-rw-r--r--   0        0        0     5234 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/runtimes/deno.py
+-rw-r--r--   0        0        0     1403 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/graphql.py
+-rw-r--r--   0        0        0     2789 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/http.py
+-rw-r--r--   0        0        0     1352 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/python_wasi.py
+-rw-r--r--   0        0        0     2880 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/random.py
+-rw-r--r--   0        0        0     2053 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/typegate.py
+-rw-r--r--   0        0        0     1169 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/wasmedge.py
+-rw-r--r--   0        0        0    20388 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/types.py
+-rw-r--r--   0        0        0      487 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/utils/__init__.py
+-rw-r--r--   0        0        0      644 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/utils/attrs.py
+-rw-r--r--   0        0        0     1977 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/utils/jsonschema.py
+-rw-r--r--   0        0        0     2198 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/utils/loaders.py
+-rw-r--r--   0        0        0      185 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/utils/sanitizers.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 typegraph-0.1.6/PKG-INFO
```

### Comparing `typegraph-0.1.5/LICENSE.md` & `typegraph-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/pyproject.toml` & `typegraph-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typegraph"
-version = "0.1.5"
+version = "0.1.6"
 description = "Compose your data, anywhere, and build iterative API blocks with zero-trust and serverless deployment, no matter where and how your (legacy) systems are."
 authors = ["Metatype Contributors <support@metatype.dev>"]
 license = "ELv2"
 homepage = "https://metatype.dev"
 repository = "https://github.com/metatypedev/metatype"
 include = ["typegraph/**/*", "LICENSE.md"]
 keywords = ["api", "composition", "typesystem", "graphql", "ecosystem"]
```

### Comparing `typegraph-0.1.5/typegraph/effects.py` & `typegraph-0.1.6/typegraph/effects.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/graph/auth/__init__.py` & `typegraph-0.1.6/typegraph/graph/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/graph/builder.py` & `typegraph-0.1.6/typegraph/graph/builder.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/graph/models.py` & `typegraph-0.1.6/typegraph/graph/models.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/graph/nodes.py` & `typegraph-0.1.6/typegraph/graph/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     def then(self, then_apply: Callable[["t.typedef"], "t.typedef"]):
         return NodeProxy(
             self.graph, self.node, lambda n: then_apply(self.after_apply(n))
         )
 
     def get(self) -> "t.typedef":
-        tpe = self.graph.type_by_names.get(self.node)
+        tpe = self.graph.type_by_names.get(self.node, None)
         if tpe is None:
             raise Exception(f"No registered type named '{self.node}'")
         if self.after_apply is None:
             return tpe
         tpe = self.after_apply(tpe)
         self.graph.type_by_names[tpe.name] = tpe
         self.node, self.after_apply = tpe.name, None
```

### Comparing `typegraph-0.1.5/typegraph/graph/typegraph.py` & `typegraph-0.1.6/typegraph/graph/typegraph.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/importers/base/importer.py` & `typegraph-0.1.6/typegraph/importers/base/importer.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/importers/base/typify.py` & `typegraph-0.1.6/typegraph/importers/base/typify.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/importers/google_discovery.py` & `typegraph-0.1.6/typegraph/importers/google_discovery.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/importers/graphql.py` & `typegraph-0.1.6/typegraph/importers/graphql.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/importers/openapi.py` & `typegraph-0.1.6/typegraph/importers/openapi.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/policies.py` & `typegraph-0.1.6/typegraph/policies.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
 
-from re import sub as reg_sub
-from typing import List, Optional, Union
+import re
+from typing import List, Optional, Pattern, Union
 
 from attrs import evolve, field, frozen
 
 from typegraph.effects import EffectType
 from typegraph.graph.builder import Collector
 from typegraph.graph.nodes import Node
 from typegraph.graph.typegraph import TypegraphContext
@@ -101,30 +101,44 @@
         }
 
 
 def public(name: str = "__public"):
     return Policy(PredefinedFunMat("true")).named(name)
 
 
-def jwt(dotaccess: str, value: str):
+def jwt(dotaccess: str, value: Union[str, Pattern]):
     # join role_name, field with '__jwt' as prefix
-    separator, pattern = "_", r"[^a-zA-Z0-9_]+"
-    prefix = "__jwt"
-    jwt_name = reg_sub(pattern, separator, separator.join([prefix, dotaccess, value]))
-    # build the policy
+    separator = "_"
+    is_regex = isinstance(value, Pattern)
+    value = sanitize_ts_string(value if not is_regex else value.pattern)
     dotaccess = sanitize_ts_string(dotaccess)
-    value = sanitize_ts_string(value)
+    jwt_name = re.sub(
+        "[^a-zA-Z0-9_]+",
+        separator,
+        separator.join(
+            [
+                "__jwt",
+                dotaccess,
+                value,
+            ]
+        ),
+    )
+    check = (
+        f""" value === "{value}" """
+        if not is_regex
+        else f""" new RegExp("{value}").test(value) """
+    )
     src = f"""
             (_, {{ context }}) => {{
                 const role_chunks = "{dotaccess}".split(".");
                 let value = context?.[role_chunks.shift()];
                 for (const chunk of role_chunks) {{
                     value = value?.[chunk];
                 }}
-                return value === "{value}";
+                return {check};
             }}
         """
     return Policy(PureFunMat(src)).named(jwt_name)
 
 
 def internal():
     return Policy(
```

### Comparing `typegraph-0.1.5/typegraph/providers/aws/runtimes/s3.py` & `typegraph-0.1.6/typegraph/providers/aws/runtimes/s3.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/providers/prisma/relations.py` & `typegraph-0.1.6/typegraph/providers/prisma/relations.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/providers/prisma/runtimes/prisma.py` & `typegraph-0.1.6/typegraph/providers/prisma/runtimes/prisma.py`

 * *Files 3% similar despite different names*

```diff
@@ -226,24 +226,26 @@
                 "id": t.uuid().config("id", "auto"),
                 "email": t.email(),
             }
         )
 
         g.expose(
             createUser=db.create(user).add_policy(public),
-            findUser=db.find_unique(user).add_policy(public),
+            findUser=db.find(user).add_policy(public),
             findManyUsers=db.find_many(user).add_policy(public),
         )
     ```
 
     Here is a list of all available generators:
-    - `find_unique`
+    - `find`
+    - `find_first`
     - `find_many`
     - `create`
     - `update`
+    - `upsert`
     - `delete`
     - `delete_many`
 
 
     """
 
     name: str
@@ -353,15 +355,15 @@
         _pref = get_name_generator("Unique", tpe)
         # output = typegen.get_out_type(base_output)
         output = typegen.add_nested_count(tpe)
         if where is None:
             # findUnique's where expression
             # does not allow AND, OR, NOT
             where = (
-                typegen.gen_query_where_expr(tpe, exclude_extra_fields=True)
+                typegen.gen_query_unique_where_expr(tpe)
                 .named(_pref("Where"))
                 .optional()
             )
         return t.func(
             t.struct({"where": where}),
             output.named(_pref("Output")).optional(),
             PrismaOperationMat(self, tpe.name, "findUnique", effect=effects.none()),
@@ -390,14 +392,41 @@
                     .optional(),
                 }
             ),
             t.array(output.named(_pref("Output"))),
             PrismaOperationMat(self, tpe.name, "findMany", effect=effects.none()),
         )
 
+    def find_first(self, tpe: Union[t.struct, t.NodeProxy], where=None) -> t.func:
+        self.__manage(tpe)
+        typegen = self.__typegen
+        _pref = get_name_generator("First", tpe)
+        output = typegen.get_out_type(tpe)
+        rel_cols = tpe.props.keys()
+        output = typegen.get_out_type(tpe)
+        if where is None:
+            where = typegen.gen_query_where_expr(tpe).named(_pref("Where")).optional()
+        return t.func(
+            t.struct(
+                {
+                    "where": where,
+                    "orderBy": typegen.get_order_by_type(tpe)
+                    .named(_pref("OrderBy"))
+                    .optional(),
+                    "take": t.integer().named(_pref("Take")).optional(),
+                    "skip": t.integer().named(_pref("Skip")).optional(),
+                    "distinct": t.array(t.enum(rel_cols))
+                    .named(_pref("Distinct"))
+                    .optional(),
+                }
+            ),
+            output.named(_pref("Output")).optional(),
+            PrismaOperationMat(self, tpe.name, "findFirst", effect=effects.none()),
+        )
+
     def aggregate(self, tpe: Union[t.struct, t.NodeProxy], where=None) -> t.func:
         self.__manage(tpe)
         typegen = self.__typegen
         _pref = get_name_generator("Aggregate", tpe)
         tpe_nums = typegen.extract_number_types(tpe)
         if where is None:
             where = typegen.gen_query_where_expr(tpe).named(_pref("Where")).optional()
@@ -441,15 +470,19 @@
                 "_sum": tpe_nums.named(_pref("Sum")).optional(),
                 "_min": tpe_nums.named(_pref("Min")).optional(),
                 "_max": tpe_nums.named(_pref("Max")).optional(),
             }
         )
         row_def = tpe.compose(aggreg_def.props)
         if where is None:
-            where = typegen.gen_query_where_expr(tpe).named(_pref("Where")).optional()
+            where = (
+                typegen.gen_query_where_expr(tpe, skip_rel=True)
+                .named(_pref("Where"))
+                .optional()
+            )
         if having is None:
             having = (
                 typegen.gen_having_expr(tpe, aggreg_def)
                 .named(_pref("Having"))
                 .optional()
             )
         return t.func(
```

### Comparing `typegraph-0.1.5/typegraph/providers/prisma/schema.py` & `typegraph-0.1.6/typegraph/providers/prisma/schema.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/providers/prisma/type_generator.py` & `typegraph-0.1.6/typegraph/providers/prisma/type_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         base_any_type = rename_with_idx(
             t.union([t.integer(), t.float(), t.boolean(), t.string()]), "base_any_type"
         )
         return t.union([base_any_type, t.array(base_any_type)])
 
     # Example:
     # t.X() => t.either([t.X(), struct_equals, struct_startsWith, ...])
-    def extend_terminal_nodes_props(self, tpe: t.struct) -> t.struct:
+    def extend_terminal_nodes_props(self, tpe: t.struct, skip_rel=False) -> t.struct:
         any_type = self.gen_any_type()
 
         # node level
         term_list = [
             t.struct({"equals": any_type}),
             t.struct({"in": any_type}),  # t.array(any_type) ??
             t.struct({"notIn": any_type}),  # t.array(any_type) ??
@@ -156,30 +156,55 @@
             term = term_list[i]
             # use the first key
             prefix = next(iter(term.props))
             term_list[i] = rename_with_idx(term, prefix)
 
         node_props = {}
         for k, v in tpe.props.items():
-            term = t.either(term_list + [undo_optional(v)])
-            not_node = rename_with_idx(t.struct({"not": term}), "not")
-            node_props[k] = t.either([not_node, term]).optional()
+            v = resolve_proxy(v)
+            if v.runtime is not None and v.runtime != tpe.runtime:
+                continue
+            nested = resolve_proxy(resolve_entity_quantifier(v))
+            if nested.type == "object" and not skip_rel:
+                # nested
+                node_props[k] = self.extend_terminal_nodes_props(
+                    nested, skip_rel=True
+                ).optional()
+            else:
+                # same depth
+                term = t.either(term_list + [undo_optional(v)])
+                not_node = rename_with_idx(t.struct({"not": term}), "not")
+                node_props[k] = t.either([not_node, term]).optional()
 
         return t.struct(node_props)
 
+    def gen_query_unique_where_expr(self, tpe: t.struct) -> t.struct:
+        props = {}
+        for k, v in tpe.props.items():
+            # not for this runtime
+            v = resolve_proxy(v)
+            if v.runtime is not None and v.runtime != tpe.runtime:
+                continue
+            v = resolve_proxy(resolve_entity_quantifier(v))
+            is_id = v.runtime_config.get("id", False)
+            is_unique = v.runtime_config.get("unique", False)
+            if is_id or is_unique:
+                props[k] = v.optional()
+        return t.struct(props)
+
     # Examples:
     # where: { name: { not: { equals: "John" } } }
     # where: { AND: [ { unique: { gt: 2 } }, { name: { startsWith: "P" }}]}
     # where: { NOT: { NOT: { name: { startsWith: "P" }} }}
     # where: { field1: 4, field2: {gt: 3}}
     def gen_query_where_expr(
-        self, tpe: t.struct, exclude_extra_fields=False
+        self, tpe: t.struct, exclude_extra_fields=False, skip_rel=False
     ) -> t.struct:
         tpe = self.get_where_type(tpe)
-        extended_tpe = self.extend_terminal_nodes_props(tpe)
+        extended_tpe = self.extend_terminal_nodes_props(tpe, skip_rel)
         extended_tpe = rename_with_idx(extended_tpe, "extended_tpe")
 
         # define the terminal expression
         temp_props = {k: v.optional() for k, v in extended_tpe.props.items()}
         intermediate = t.proxy("???")
         if not exclude_extra_fields:
             temp_props["AND"] = t.array(intermediate).optional()
```

### Comparing `typegraph-0.1.5/typegraph/providers/prisma/utils.py` & `typegraph-0.1.6/typegraph/providers/prisma/utils.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/providers/temporal/runtimes/temporal.py` & `typegraph-0.1.6/typegraph/providers/temporal/runtimes/temporal.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/runtimes/base.py` & `typegraph-0.1.6/typegraph/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/runtimes/deno.py` & `typegraph-0.1.6/typegraph/runtimes/deno.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/runtimes/graphql.py` & `typegraph-0.1.6/typegraph/runtimes/graphql.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/runtimes/http.py` & `typegraph-0.1.6/typegraph/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/runtimes/python_wasi.py` & `typegraph-0.1.6/typegraph/runtimes/python_wasi.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/runtimes/random.py` & `typegraph-0.1.6/typegraph/runtimes/random.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/runtimes/typegate.py` & `typegraph-0.1.6/typegraph/runtimes/typegate.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/runtimes/wasmedge.py` & `typegraph-0.1.6/typegraph/runtimes/wasmedge.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/types.py` & `typegraph-0.1.6/typegraph/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,33 @@
     Optional,
     Set,
     Tuple,
     Type,
     Union,
     get_args,
     get_origin,
+    overload,
 )
 
 from attrs import evolve, field, frozen
 from frozendict import frozendict
 from typing_extensions import Self
+from typegraph.effects import EffectType
 
 from typegraph.graph.builder import Collector
 from typegraph.graph.nodes import Node, NodeProxy
 from typegraph.graph.typegraph import TypeGraph, TypegraphContext, find
+from typegraph.injection import (
+    Injection,
+    InjectionSwitch,
+    context,
+    parent,
+    secret,
+    static,
+)
 from typegraph.policies import Policy, EffectPolicies
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import SKIP, always, asdict
 
 # if os.environ.get("DEBUG"):
 #     import debugpy
 
@@ -95,16 +105,15 @@
         factory=TypegraphContext.get_active,
         init=False,
         metadata={SKIP: True},
     )
     name: str = field(kw_only=True, default="")
     description: Optional[str] = optional_field()
     runtime: Optional["Runtime"] = optional_field()
-    inject: Optional[Union[str, TypeNode]] = optional_field()
-    injection: Optional[Any] = optional_field()
+    injection: InjectionSwitch = optional_field()
     policies: Tuple[Policy, ...] = field(kw_only=True, factory=tuple)
     # runtime_config: Dict[str, Any] = field(
     #     kw_only=True, factory=dict, hash=False, metadata={SKIP: True}
     # )
     runtime_config: Dict[str, Any] = field(
         kw_only=True, factory=frozendict, hash=False, metadata={SKIP: True}
     )
@@ -113,31 +122,34 @@
     collector_target: Optional[str] = always(Collector.types)
 
     def __attrs_post_init__(self):
         if self.graph is None:
             raise Exception("No typegraph context")
         if self.name == "":
             object.__setattr__(self, "name", f"{self.type}_{self.graph.next_type_id()}")
-        if self.inject is None:
-            object.__setattr__(self, "injection", None)
 
-    def replace(self, **changes):
+    def replace(self, **changes) -> Self:
         return evolve(self, **changes)
 
     @property
     def type(self):
         return type(self).__name__
 
     @property
     def edges(self) -> List[Node]:
-        secret = self.inject if self.injection == "secret" else None
+        secrets = (
+            [Secret(s) for s in self.injection.secrets()]
+            if self.injection is not None
+            else []
+        )
         return (
             super().edges
             + list(self.policies)
-            + list(filter(None, [self.runtime, secret]))
+            + list(filter(None, [self.runtime]))
+            + secrets
         )
 
     @property
     def labeled_edges(self) -> Dict[str, str]:
         return {}
 
     def register_name(self):
@@ -190,40 +202,42 @@
 
         for e in self.edges:
             if isinstance(e, typedef):
                 e._propagate_runtime(self.runtime, visited)
             if isinstance(e, NodeProxy):
                 e.get()._propagate_runtime(self.runtime, visited)
 
-    def set(self, value):
-        if self.inject is not None:
-            raise Exception(f"{self.name} can only have one injection")
+    # TODO @overload
+    @overload
+    def inject(self, injection: Injection) -> Self:
+        pass
+
+    @overload
+    def inject(self, injection: Dict[Optional[EffectType], Injection]) -> Self:
+        pass
 
-        import json
-
-        return self.replace(injection="raw", inject=json.dumps(value))
-
-    def from_secret(self, secret_name):
-        if self.inject is not None:
+    def inject(self, injection) -> Self:
+        if self.injection is not None:
             raise Exception(f"{self.name} can only have one injection")
+        if isinstance(injection, dict):
+            return self.replace(injection=InjectionSwitch.from_dict(injection))
+        return self.replace(injection=InjectionSwitch(default=injection))
 
-        return self.replace(injection="secret", inject=Secret(secret_name))
+    def set(self, value):
+        return self.inject(static(value))
 
-    def from_parent(self, sibiling: "NodeProxy"):
-        # TODO: check for same type and value in same context
-        if self.inject is not None:
-            raise Exception(f"{self.name} can only have one injection")
+    def from_secret(self, secret_name: str):
+        return self.inject(secret(secret_name))
 
-        return self.replace(injection="parent", inject=sibiling)
+    def from_parent(self, sibling: "NodeProxy"):
+        # TODO: check for same type and value in same context
+        return self.inject(parent(sibling))
 
     def from_context(self, claim: str):
-        if self.inject is not None:
-            raise Exception(f"{self.name} can only have one injection")
-
-        return self.replace(injection="context", inject=claim)
+        return self.inject(context(claim))
 
     def add_policy(
         self,
         *policies: List[Union[Policy, Materializer]],
     ):
         return self.replace(
             policies=self.policies + tuple(Policy.create_from(p) for p in policies)
@@ -247,18 +261,17 @@
         ret["type"] = self.type
         ret["title"] = ret.pop("name")
         ret["runtime"] = collector.index(self.runtime)
         ret["policies"] = [
             p.data(collector) if isinstance(p, EffectPolicies) else collector.index(p)
             for p in self.policies
         ]
-        if self.injection == "parent":
-            ret["inject"] = collector.index(self.inject)
-        elif self.injection == "secret":
-            ret["inject"] = self.inject.secret
+
+        if self.injection is not None:
+            ret["injection"] = self.injection.data(collector)
 
         config = self.runtime.get_type_config(self)
         if len(config) > 0:
             ret["config"] = config
 
         if hasattr(type(self), "constraint_data"):
             ret.update(self.constraint_data())
@@ -714,15 +727,18 @@
     if defined is not None:
         return defined
     else:
         return define().named(name)
 
 
 def proxy(name: str) -> NodeProxy:
-    return NodeProxy(TypegraphContext.get_active(), name)
+    g = TypegraphContext.get_active()
+    if g is None:
+        raise Exception("Active typegraph context required for 't.proxy'")
+    return NodeProxy(g, name)
 
 
 def visit_reversed(
     tpe: typedef, fn: Callable[[typedef], Any], visited: Set[str] = set()
 ):
     for node in tpe.edges:
         if isinstance(node, typedef):
```

### Comparing `typegraph-0.1.5/typegraph/utils/attrs.py` & `typegraph-0.1.6/typegraph/utils/attrs.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/utils/jsonschema.py` & `typegraph-0.1.6/typegraph/utils/jsonschema.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/typegraph/utils/loaders.py` & `typegraph-0.1.6/typegraph/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.5/PKG-INFO` & `typegraph-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typegraph
-Version: 0.1.5
+Version: 0.1.6
 Summary: Compose your data, anywhere, and build iterative API blocks with zero-trust and serverless deployment, no matter where and how your (legacy) systems are.
 Home-page: https://metatype.dev
 License: ELv2
 Keywords: api,composition,typesystem,graphql,ecosystem
 Author: Metatype Contributors
 Author-email: support@metatype.dev
 Requires-Python: >=3.8,<4.0
```


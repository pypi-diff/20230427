# Comparing `tmp/bareasgi-graphql-next-5.0.3.tar.gz` & `tmp/bareasgi-graphql-next-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bareasgi-graphql-next-5.0.3.tar", max compression
+gzip compressed data, was "bareasgi-graphql-next-5.0.4.tar", max compression
```

## Comparing `bareasgi-graphql-next-5.0.3.tar` & `bareasgi-graphql-next-5.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2022-02-16 08:31:32.758156 bareasgi-graphql-next-5.0.3/LICENSE
--rw-r--r--   0        0        0      963 2022-02-16 08:31:32.758244 bareasgi-graphql-next-5.0.3/README.md
--rw-r--r--   0        0        0      282 2022-02-16 08:31:32.758368 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/__init__.py
--rw-r--r--   0        0        0    18265 2022-04-12 09:42:40.677562 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/controller.py
--rw-r--r--   0        0        0      170 2022-02-16 08:31:32.758669 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphene/__init__.py
--rw-r--r--   0        0        0     2634 2022-04-12 09:42:11.359074 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphene/controller.py
--rw-r--r--   0        0        0     2820 2022-02-18 06:53:42.548970 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphene/helpers.py
--rw-r--r--   0        0        0      770 2022-04-12 09:40:34.637486 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphene/websocket_handler.py
--rw-r--r--   0        0        0     1438 2022-04-12 09:40:27.271993 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphene/websocket_instance.py
--rw-r--r--   0        0        0      175 2022-02-16 08:31:32.759222 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphql/__init__.py
--rw-r--r--   0        0        0     2850 2022-04-12 09:41:59.707683 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphql/controller.py
--rw-r--r--   0        0        0     2802 2022-04-12 09:41:43.036728 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphql/helpers.py
--rw-r--r--   0        0        0      780 2022-04-12 09:43:47.348490 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphql/websocket_handler.py
--rw-r--r--   0        0        0     1613 2022-04-12 09:40:19.525360 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphql/websocket_instance.py
--rw-r--r--   0        0        0        0 2022-02-16 08:31:32.759561 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/py.typed
--rw-r--r--   0        0        0     5430 2022-02-16 08:31:32.759662 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/template.py
--rw-r--r--   0        0        0     5849 2022-02-18 07:03:44.345056 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/utils.py
--rw-r--r--   0        0        0    11890 2022-04-12 09:44:35.532107 bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/websocket_instance.py
--rw-r--r--   0        0        0      907 2022-04-12 09:42:56.070419 bareasgi-graphql-next-5.0.3/pyproject.toml
--rw-r--r--   0        0        0     1914 2022-04-12 09:45:16.300909 bareasgi-graphql-next-5.0.3/setup.py
--rw-r--r--   0        0        0     1807 2022-04-12 09:45:16.301086 bareasgi-graphql-next-5.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-02-16 08:31:32.758156 bareasgi-graphql-next-5.0.4/LICENSE
+-rw-r--r--   0        0        0      963 2022-02-16 08:31:32.758244 bareasgi-graphql-next-5.0.4/README.md
+-rw-r--r--   0        0        0      282 2022-02-16 08:31:32.758368 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/__init__.py
+-rw-r--r--   0        0        0    18537 2023-04-27 08:27:35.863296 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/controller.py
+-rw-r--r--   0        0        0      170 2022-02-16 08:31:32.758669 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphene/__init__.py
+-rw-r--r--   0        0        0     2634 2022-04-12 09:42:11.359074 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphene/controller.py
+-rw-r--r--   0        0        0     2820 2022-02-18 06:53:42.548970 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphene/helpers.py
+-rw-r--r--   0        0        0      770 2022-04-12 09:40:34.637486 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphene/websocket_handler.py
+-rw-r--r--   0        0        0     1438 2022-04-12 09:40:27.271993 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphene/websocket_instance.py
+-rw-r--r--   0        0        0      175 2022-02-16 08:31:32.759222 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphql/__init__.py
+-rw-r--r--   0        0        0     2850 2022-04-12 09:41:59.707683 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphql/controller.py
+-rw-r--r--   0        0        0     2802 2022-04-12 09:41:43.036728 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphql/helpers.py
+-rw-r--r--   0        0        0      780 2022-04-12 09:43:47.348490 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphql/websocket_handler.py
+-rw-r--r--   0        0        0     1613 2022-04-12 09:40:19.525360 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphql/websocket_instance.py
+-rw-r--r--   0        0        0        0 2022-02-16 08:31:32.759561 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/py.typed
+-rw-r--r--   0        0        0     5430 2022-02-16 08:31:32.759662 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/template.py
+-rw-r--r--   0        0        0     5849 2022-02-18 07:03:44.345056 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/utils.py
+-rw-r--r--   0        0        0    11890 2022-04-12 09:44:35.532107 bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/websocket_instance.py
+-rw-r--r--   0        0        0      907 2023-04-27 08:28:13.102570 bareasgi-graphql-next-5.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1914 2023-04-27 08:28:52.327285 bareasgi-graphql-next-5.0.4/setup.py
+-rw-r--r--   0        0        0     1807 2023-04-27 08:28:52.327449 bareasgi-graphql-next-5.0.4/PKG-INFO
```

### Comparing `bareasgi-graphql-next-5.0.3/LICENSE` & `bareasgi-graphql-next-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/README.md` & `bareasgi-graphql-next-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/controller.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,15 +431,24 @@
             self,
             request: HttpRequest,
             body: Mapping[str, Any]
     ) -> HttpResponse:
         # Handle a subscription by returning 201 (Created) with
         # the url location of the subscription.
         LOGGER.debug("Redirecting subscription request.")
-        scheme = request.scope['scheme']
+        # TODO: handle 'forwarded' header.
+        forwarded_proto = header.find(
+            b'x-forwarded-proto',
+            request.scope['headers']
+        )
+        scheme = (
+            forwarded_proto.decode()
+            if forwarded_proto is not None
+            else request.scope['scheme']
+        )
         host = cast(
             bytes,
             header.find(  # type: ignore
                 b'host',
                 request.scope['headers'],
                 b'localhost'
             )
```

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphene/controller.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphene/controller.py`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphene/helpers.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphene/helpers.py`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphene/websocket_handler.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphene/websocket_handler.py`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphene/websocket_instance.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphene/websocket_instance.py`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphql/controller.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphql/controller.py`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphql/helpers.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphql/helpers.py`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphql/websocket_handler.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphql/websocket_handler.py`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/graphql/websocket_instance.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/graphql/websocket_instance.py`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/template.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/template.py`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/utils.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/utils.py`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/bareasgi_graphql_next/websocket_instance.py` & `bareasgi-graphql-next-5.0.4/bareasgi_graphql_next/websocket_instance.py`

 * *Files identical despite different names*

### Comparing `bareasgi-graphql-next-5.0.3/pyproject.toml` & `bareasgi-graphql-next-5.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bareasgi-graphql-next"
-version = "5.0.3"
+version = "5.0.4"
 description = "GraphQL support for the bareASGI framework"
 authors = ["Rob Blackbourn <rob.blackbourn@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "bareasgi_graphql_next" },
 ]
```

### Comparing `bareasgi-graphql-next-5.0.3/setup.py` & `bareasgi-graphql-next-5.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ['bareASGI>=4.0.0,<5.0.0', 'graphql-core>=3.1,<4.0']
 
 extras_require = \
 {'graphene': ['graphene>=3.0,<4.0']}
 
 setup_kwargs = {
     'name': 'bareasgi-graphql-next',
-    'version': '5.0.3',
+    'version': '5.0.4',
     'description': 'GraphQL support for the bareASGI framework',
     'long_description': "# bareASGI-graphql-next\n\nGraphql support for [bareASGI](http://github.com/rob-blackbourn/bareASGI) (read the [documentation](https://rob-blackbourn.github.io/bareASGI-graphql-next/))\n\nThe controller provides a GraphQL GET and POST route, a WebSocket subscription server, and a Graphiql view.\n\n## Installation\n\nInstall from the pie shop.\n\n```bash\npip install bareasgi-graphql-next\n```\n\nIf you wish to install with the grapheme option:\n\n```bash\npip install 'bareasgi-graphql-next[graphene]'\n```\n\n## Usage\n\nYou can register the graphql controller with the `add_graphql_next` function.\n\n```python\nfrom bareasgi import Application\nfrom bareasgi_graphql_next import add_graphql_next\nimport graphql\n\n# Get the schema ...\nschema = graphql.GraphQLSchema( ... )\n\nimport uvicorn\n\napp = Application()\nadd_graphql_next(app, schema)\n\nuvicorn.run(app, port=9009)\n\n```\n\n## Development\n\nTo develop with the graphene optional package:\n\n```bash\npoetry install --extras graphene\n```\n",
     'author': 'Rob Blackbourn',
     'author_email': 'rob.blackbourn@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/rob-blackbourn/bareasgi-graphql-next',
```

### Comparing `bareasgi-graphql-next-5.0.3/PKG-INFO` & `bareasgi-graphql-next-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bareasgi-graphql-next
-Version: 5.0.3
+Version: 5.0.4
 Summary: GraphQL support for the bareASGI framework
 Home-page: https://github.com/rob-blackbourn/bareasgi-graphql-next
 License: Apache-2.0
 Author: Rob Blackbourn
 Author-email: rob.blackbourn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```


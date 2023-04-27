# Comparing `tmp/drb-xquery-1.1.0.tar.gz` & `tmp/drb-xquery-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-xquery-1.1.0.tar", last modified: Tue Jan  3 09:59:36 2023, max compression
+gzip compressed data, was "drb-xquery-1.2.0.tar", last modified: Thu Apr 27 17:32:42 2023, max compression
```

## Comparing `drb-xquery-1.1.0.tar` & `drb-xquery-1.2.0.tar`

### file list

```diff
@@ -1,46 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 09:59:36.587241 drb-xquery-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      298 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       82 2022-04-29 09:08:07.000000 drb-xquery-1.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1006 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-12-28 16:11:11.000000 drb-xquery-1.1.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1356 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     6948 2023-01-03 09:59:36.587241 drb-xquery-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6503 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 09:59:36.379237 drb-xquery-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 09:59:36.391237 drb-xquery-1.1.0/drb/signatures/
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-01-02 13:02:54.000000 drb-xquery-1.1.0/drb/signatures/xquery.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 09:59:36.587241 drb-xquery-1.1.0/drb/xquery/
--rw-rw-rw-   0 root         (0) root         (0)    37649 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/XQueryLexer.g4
--rw-rw-rw-   0 root         (0) root         (0)   246218 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/XQueryLexer.interp
--rw-rw-rw-   0 root         (0) root         (0)   293030 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/XQueryLexer.py
--rw-rw-rw-   0 root         (0) root         (0)     2832 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/XQueryLexer.tokens
--rw-rw-rw-   0 root         (0) root         (0)    25815 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/XQueryParser.g4
--rw-rw-rw-   0 root         (0) root         (0)    82016 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/XQueryParser.interp
--rw-rw-rw-   0 root         (0) root         (0)   893031 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/XQueryParser.py
--rw-rw-rw-   0 root         (0) root         (0)     2832 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/XQueryParser.tokens
--rw-rw-rw-   0 root         (0) root         (0)    75031 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/XQueryParserListener.py
--rw-rw-rw-   0 root         (0) root         (0)    44354 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/XQueryParserVisitor.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-01-02 13:02:54.000000 drb-xquery-1.1.0/drb/xquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-01-03 09:59:36.587241 drb-xquery-1.1.0/drb/xquery/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/drb_xquery.py
--rwxrwxrwx   0 root         (0) root         (0)     7439 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/drb_xquery_cmd.py
--rw-rw-rw-   0 root         (0) root         (0)    10636 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/drb_xquery_context.py
--rw-rw-rw-   0 root         (0) root         (0)    36718 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/drb_xquery_func.py
--rw-rw-rw-   0 root         (0) root         (0)     4190 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/drb_xquery_item.py
--rw-rw-rw-   0 root         (0) root         (0)    10214 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/drb_xquery_res_to_string.py
--rw-rw-rw-   0 root         (0) root         (0)    17398 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/drb_xquery_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4319 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/drb_xquery_variable.py
--rw-rw-rw-   0 root         (0) root         (0)    64177 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/drb_xquery_visitor.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/drb/xquery/execptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 09:59:36.587241 drb-xquery-1.1.0/drb_xquery.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6948 2023-01-03 09:59:33.000000 drb-xquery-1.1.0/drb_xquery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-01-03 09:59:36.000000 drb-xquery-1.1.0/drb_xquery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-03 09:59:33.000000 drb-xquery-1.1.0/drb_xquery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-01-03 09:59:33.000000 drb-xquery-1.1.0/drb_xquery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      115 2023-01-03 09:59:33.000000 drb-xquery-1.1.0/drb_xquery.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-03 09:59:33.000000 drb-xquery-1.1.0/drb_xquery.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-28 15:41:08.000000 drb-xquery-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-01-03 09:59:36.587241 drb-xquery-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1220 2023-01-02 13:02:54.000000 drb-xquery-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    78254 2022-04-29 09:08:09.000000 drb-xquery-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 17:32:42.390406 drb-xquery-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 17:02:09.000000 drb-xquery-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2022-12-28 16:11:11.000000 drb-xquery-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6880 2023-04-27 17:32:42.390406 drb-xquery-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6503 2022-12-28 15:41:08.000000 drb-xquery-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 17:32:42.358406 drb-xquery-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 17:32:42.366406 drb-xquery-1.2.0/drb/signatures/
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-01-02 13:02:54.000000 drb-xquery-1.2.0/drb/signatures/xquery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 17:32:42.390406 drb-xquery-1.2.0/drb/xquery/
+-rw-rw-rw-   0 root         (0) root         (0)   293030 2022-12-28 15:41:08.000000 drb-xquery-1.2.0/drb/xquery/XQueryLexer.py
+-rw-rw-rw-   0 root         (0) root         (0)   893031 2022-12-28 15:41:08.000000 drb-xquery-1.2.0/drb/xquery/XQueryParser.py
+-rw-rw-rw-   0 root         (0) root         (0)    75031 2022-12-28 15:41:08.000000 drb-xquery-1.2.0/drb/xquery/XQueryParserListener.py
+-rw-rw-rw-   0 root         (0) root         (0)    44354 2022-12-28 15:41:08.000000 drb-xquery-1.2.0/drb/xquery/XQueryParserVisitor.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-01-02 13:02:54.000000 drb-xquery-1.2.0/drb/xquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-27 17:32:42.390406 drb-xquery-1.2.0/drb/xquery/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2023-02-16 15:13:36.000000 drb-xquery-1.2.0/drb/xquery/drb_xquery.py
+-rwxrwxrwx   0 root         (0) root         (0)     7462 2023-02-16 15:13:36.000000 drb-xquery-1.2.0/drb/xquery/drb_xquery_cmd.py
+-rw-rw-rw-   0 root         (0) root         (0)    10673 2023-02-03 08:59:37.000000 drb-xquery-1.2.0/drb/xquery/drb_xquery_context.py
+-rw-rw-rw-   0 root         (0) root         (0)    36740 2023-02-16 15:13:36.000000 drb-xquery-1.2.0/drb/xquery/drb_xquery_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     2882 2023-04-27 12:34:27.000000 drb-xquery-1.2.0/drb/xquery/drb_xquery_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    10214 2022-12-28 15:41:08.000000 drb-xquery-1.2.0/drb/xquery/drb_xquery_res_to_string.py
+-rw-rw-rw-   0 root         (0) root         (0)    17398 2022-12-28 15:41:08.000000 drb-xquery-1.2.0/drb/xquery/drb_xquery_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2023-02-16 15:13:36.000000 drb-xquery-1.2.0/drb/xquery/drb_xquery_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)    64569 2023-04-27 12:34:27.000000 drb-xquery-1.2.0/drb/xquery/drb_xquery_visitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2022-12-28 15:41:08.000000 drb-xquery-1.2.0/drb/xquery/execptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 17:32:42.390406 drb-xquery-1.2.0/drb_xquery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6880 2023-04-27 17:32:42.000000 drb-xquery-1.2.0/drb_xquery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      839 2023-04-27 17:32:42.000000 drb-xquery-1.2.0/drb_xquery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 17:32:42.000000 drb-xquery-1.2.0/drb_xquery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 17:32:42.000000 drb-xquery-1.2.0/drb_xquery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 17:32:41.000000 drb-xquery-1.2.0/drb_xquery.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-27 17:32:42.000000 drb-xquery-1.2.0/drb_xquery.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-27 17:32:42.000000 drb-xquery-1.2.0/drb_xquery.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-02-17 13:29:36.000000 drb-xquery-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-27 09:12:55.000000 drb-xquery-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      920 2023-04-27 17:32:42.390406 drb-xquery-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-02-17 10:05:38.000000 drb-xquery-1.2.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    78254 2022-04-29 09:08:09.000000 drb-xquery-1.2.0/versioneer.py
```

### Comparing `drb-xquery-1.1.0/PKG-INFO` & `drb-xquery-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: drb-xquery
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB xquery request
-Home-page: https://gitlab.com/drb-python/xquery
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # Xquery for DRB
 This xquery module allows execute xquery on DRB nodes.
 
 ## Using this module
 To include this module into your project, the `drb-xquery` module shall be 
 referenced into `requirement.txt` file, or the following pip line can be run:
@@ -192,9 +190,7 @@
 ```
 doc("catalog.xml")/catalog/product[position() = (1 to 3)]
 ```
 
 For compare function the result is only -1,0, 1 , in java thi function return a
 negative value that can be different to -1 or a positive value that represent a
 difference between the two string...
-
-
```

### Comparing `drb-xquery-1.1.0/README.md` & `drb-xquery-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-xquery-1.1.0/drb/signatures/xquery.py` & `drb-xquery-1.2.0/drb/signatures/xquery.py`

 * *Files identical despite different names*

### Comparing `drb-xquery-1.1.0/drb/xquery/XQueryLexer.py` & `drb-xquery-1.2.0/drb/xquery/XQueryLexer.py`

 * *Files identical despite different names*

### Comparing `drb-xquery-1.1.0/drb/xquery/XQueryParser.py` & `drb-xquery-1.2.0/drb/xquery/XQueryParser.py`

 * *Files identical despite different names*

### Comparing `drb-xquery-1.1.0/drb/xquery/XQueryParserListener.py` & `drb-xquery-1.2.0/drb/xquery/XQueryParserListener.py`

 * *Files identical despite different names*

### Comparing `drb-xquery-1.1.0/drb/xquery/XQueryParserVisitor.py` & `drb-xquery-1.2.0/drb/xquery/XQueryParserVisitor.py`

 * *Files identical despite different names*

### Comparing `drb-xquery-1.1.0/drb/xquery/drb_xquery.py` & `drb-xquery-1.2.0/drb/xquery/drb_xquery.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 from antlr4 import InputStream, CommonTokenStream
 from drb.core import DrbNode
 from .XQueryLexer import XQueryLexer
 from .XQueryParser import XQueryParser
 from .drb_xquery_context import DynamicContext
+from .drb_xquery_utils import DrbQueryFuncUtil
 from .drb_xquery_visitor import DrbQueryVisitor, DrbXqueryParserErrorListener
 import io
 import sys
 
 
 class DrbXQuery:
 
     def __init__(self, xquery):
         self.static_context = None
-
         if isinstance(xquery, DrbNode):
             xquery = xquery.get_impl(io.BufferedIOBase)
 
         if isinstance(xquery, io.BufferedIOBase):
-            xquery = xquery.read().decode()
+            reader = xquery
+            xquery = reader.read().decode()
+            reader.close()
 
         # init Lexer with query
         lexer = XQueryLexer(InputStream(xquery))
 
         self.stream = CommonTokenStream(lexer)
         self.parser = XQueryParser(self.stream)
 
         self.parser.addErrorListener(DrbXqueryParserErrorListener())
         # parse query and reject it if error
         self.tree = self.parser.module()
 
     def execute(self, *args, **kwargs):
-
         old_limit = sys.getrecursionlimit()
         sys.setrecursionlimit(10000)
 
         list_nodes = args
 
         if len(list_nodes) == 0:
             list_nodes = [None]
@@ -44,15 +45,40 @@
             visitor = DrbQueryVisitor(DynamicContext(node_item),
                                       tokens=self.stream)
 
             visitor.external_var_map = kwargs
             self.static_context = visitor.static_context
 
             output = visitor.visitModule(self.tree)
+
+            nodes_ouput = []
+
             if not isinstance(output, list):
                 output_list.append(output)
+                if output is not None:
+                    node = DrbQueryFuncUtil.get_node(output)
+                    if node is not None and isinstance(node, DrbNode):
+                        if node not in nodes_ouput:
+                            nodes_ouput.append(node)
             else:
                 output_list.extend(output)
+                for one_ouput in output:
+                    if one_ouput is not None:
+                        node = DrbQueryFuncUtil.get_node(one_ouput)
+                        if node is not None and isinstance(node, DrbNode):
+                            if node not in nodes_ouput:
+                                nodes_ouput.append(node)
+
+            for node in nodes_ouput:
+                parent = node.parent
+                while parent is not None:
+                    if parent not in nodes_ouput:
+                        nodes_ouput.append(parent)
+                    parent = parent.parent
+
+            for node_child in self.static_context.list_children_open:
+                if node_child not in nodes_ouput:
+                    node_child.close()
 
         sys.setrecursionlimit(old_limit)
 
         return output_list
```

### Comparing `drb-xquery-1.1.0/drb/xquery/drb_xquery_cmd.py` & `drb-xquery-1.2.0/drb/xquery/drb_xquery_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     if len(file) > 0:
         if verbose:
             print('query_file :')
             print(file)
         node_query = resolver.create(file)
         buffer = node_query.get_impl(io.BufferedIOBase)
         string = buffer.read().decode('utf-8')
+        buffer.close()
 
     node = None
     if len(url_node) > 0:
         node = resolver.create(url_node)
 
     variables = {}
```

### Comparing `drb-xquery-1.1.0/drb/xquery/drb_xquery_context.py` & `drb-xquery-1.2.0/drb/xquery/drb_xquery_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 
         self.name_space_map = NamespaceMap()
 
         self.namespace_builtin_func = {}
 
         self.imported_module = {}
         self.is_in_predicate = False
+        self.list_children_open = []
 
     def clone(self, other):
         if isinstance(other, StaticContext):
             self.namespace_map = other.namespace_map.copy()
             self.namespace_prefix_map = other.namespace_prefix_map.copy()
             self.namespace_func = other.namespace_func.copy()
             self.namespace_builtin_func = other.namespace_func.copy()
```

### Comparing `drb-xquery-1.1.0/drb/xquery/drb_xquery_func.py` & `drb-xquery-1.2.0/drb/xquery/drb_xquery_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,15 @@
         try:
             signature, n = resolver.resolve(source=url_str)
         except Exception:
             raise DynamicException(ErrorXQUERY.FODC0005, "Unable to resolve :"
                                    + str(args[0]))
         try:
             node_doc = signature.factory.create(n)
+            n.close()
         except Exception:
             raise DynamicException(ErrorXQUERY.FODC0002,
                                    "Unable to create node with url :"
                                    + str(args[0]))
 
     return DynamicContext(node_doc)
```

### Comparing `drb-xquery-1.1.0/drb/xquery/drb_xquery_res_to_string.py` & `drb-xquery-1.2.0/drb/xquery/drb_xquery_res_to_string.py`

 * *Files identical despite different names*

### Comparing `drb-xquery-1.1.0/drb/xquery/drb_xquery_utils.py` & `drb-xquery-1.2.0/drb/xquery/drb_xquery_utils.py`

 * *Files identical despite different names*

### Comparing `drb-xquery-1.1.0/drb/xquery/drb_xquery_variable.py` & `drb-xquery-1.2.0/drb/xquery/drb_xquery_variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .drb_xquery_utils import DrbQueryFuncUtil
 from .execptions import DynamicException, ErrorXQUERY
+from drb.xquery.drb_xquery_func import DrbQueryFuncCall
 
 
 class XqueryBuildIn:
     def __init__(self, name,
                  exp_func,
                  namespace=None,
                  specific_context=None):
@@ -55,15 +56,14 @@
                 if arg_min == 0:
                     return ''
                 else:
                     raise DynamicException(ErrorXQUERY.XPTY0004,
                                            func_msg +
                                            " empty value instead of" +
                                            type_var_namespace + ':' + type_var)
-            from drb.xquery.drb_xquery_func import DrbQueryFuncCall
             if type_var_namespace == 'xs':
                 if isinstance(value, list) and arg_max > 1:
                     result = []
                     for item in value:
                         result.append(DrbQueryFuncCall.xs_type_func[type_var](
                             type_var, None, None, item))
                 else:
```

### Comparing `drb-xquery-1.1.0/drb/xquery/drb_xquery_visitor.py` & `drb-xquery-1.2.0/drb/xquery/drb_xquery_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,27 +86,28 @@
             uri_of_lib = self.visitUriLiteral(ctx.uriLiteral(index_uri))
 
         if uri_of_lib is not None:
             if uri_of_lib in self.static_context.imported_module.keys():
                 return
 
             self.static_context.imported_module[uri_of_lib] = prefix_module
-
             node_module = resolver.create(uri_of_lib)
             if node_module.has_impl(io.RawIOBase):
                 impl = node_module.get_impl(io.BufferedIOBase)
 
                 xquery_buffer = impl.readlines()
+                impl.close()
+                node_module.close()
                 xquery_string = ''
+
                 for line in xquery_buffer:
                     xquery_string = xquery_string + line.decode('utf-8')
                 lexer = XQueryLexer(InputStream(xquery_string))
                 stream = CommonTokenStream(lexer)
                 parser = XQueryParser(stream)
-
                 tree = parser.libraryModule()
 
                 visitor = DrbQueryVisitor(None, is_module=True)
                 visitor.static_context.imported_module = \
                     self.static_context.imported_module.copy()
                 # visitor.static_context.clone(self.static_context)
                 output = visitor.visit(tree)
@@ -828,21 +829,21 @@
                             self.static_context,
                             attribute_name,
                             ns_full)
                     else:
                         if attribute_name == 'xmlns':
                             if node.namespace_uri is None \
                                     or len(node.namespace_uri) == 0:
-                                node._namespace_uri = value_attribute.\
+                                node.namespace_uri = value_attribute.\
                                     strip('"')
                                 NamespaceMap.check_is_predefined_namespace(
-                                    None, node._namespace_uri)
+                                    None, node.namespace_uri)
 
                                 self.dynamic_context.namespace_default_elt = \
-                                    node._namespace_uri
+                                    node.namespace_uri
                         else:
                             if namespace is not None:
                                 namespace = self.\
                                     get_namespace_full_name(namespace)
                             attributes[attribute_name, namespace] = \
                                 value_attribute
         return attributes
@@ -894,21 +895,22 @@
         node = DrbXqueryItem(None, name, namespace, namespace_full)
         self.dynamic_context = DynamicContext(
             node, dynamic_context_prev=self.dynamic_context)
 
         if ctx.dirAttributeList() is not None:
             attributes_node = self.getAttributeValueList(
                 ctx.dirAttributeList(), node)
-            node.set_attribute(attributes_node)
+            for key in attributes_node.keys():
+                node @= (key[0], key[1], attributes_node[key])
 
         if namespace is not None:
-            node._namespace_uri = self.get_namespace_full_name(namespace)
+            node.namespace_uri = self.get_namespace_full_name(namespace)
         elif node.namespace_uri is None and \
                 len(self.dynamic_context.namespace_default_elt) > 0:
-            node._namespace_uri = self.dynamic_context.namespace_default_elt
+            node.namespace_uri = self.dynamic_context.namespace_default_elt
 
         return node
 
     def visitDirElemConstructorOpenClose(self, ctx: XQueryParser.
                                          DirElemConstructorOpenCloseContext):
         if len(ctx.qName()) == 0:
             raise StaticException(ErrorXQUERY.XPST0003,
@@ -933,36 +935,38 @@
             if not isinstance(result_value, list):
                 result_value = [result_value]
 
             value_content = None
             for item_value in result_value:
                 node.order_elt.append(item_value)
                 if isinstance(item_value, DrbNode):
-                    node.append_child(item_value)
+                    node[None] = item_value
                 if isinstance(item_value, DynamicContext):
                     if item_value.is_attribute():
-                        node.add_attribute(item_value.name,
-                                           item_value.value,
-                                           item_value.namespace_uri)
+                        node @= (
+                            item_value.name,
+                            item_value.namespace_uri,
+                            item_value.value
+                        )
                     else:
-                        node.append_child(item_value.node)
+                        node[None] = item_value.node
                 elif value_content is None:
                     value_content = item_value
                 else:
                     value_content = \
                         DrbQueryFuncUtil.get_string(value_content) + ' ' + \
                         DrbQueryFuncUtil.get_string(item_value)
 
             if value_content is not None:
                 if value is None:
                     value = value_content
                 else:
                     value = DrbQueryFuncUtil.get_string(value) + \
                             DrbQueryFuncUtil.get_string(value_content)
-        node.set_value(value)
+        node.value = value
 
         context_to_return = self.dynamic_context
 
         self.dynamic_context = dynamic_context_old
 
         return context_to_return
 
@@ -1198,15 +1202,16 @@
 
                     return node[name, namespace, :]
         except Exception:
             pass
         return []
 
     @staticmethod
-    def get_children(node, current_axe, list_result):
+    def get_children(node, current_axe, list_result,
+                     static_context: StaticContext):
         next_nodes = []
         if current_axe.is_wildcard:
             next_nodes = node.children
         else:
             next_nodes = DrbQueryVisitor.get_children_node(
                 node,
                 current_axe.name,
@@ -1214,28 +1219,31 @@
             if len(next_nodes) == 0 and \
                     current_axe.namespace is not None and \
                     not current_axe.namespace_resolved and \
                     not isinstance(node, XmlNode):
                 child_name = current_axe.namespace + ':' + current_axe.name
                 next_nodes = DrbQueryVisitor.get_children_node(
                     node, child_name, None)
+        if static_context is not None:
+            static_context.list_children_open.extend(next_nodes)
         for node_drb in next_nodes:
             list_result.append(DynamicContext(
                 node_drb,
                 position=len(list_result) + 1))
 
         return list_result
 
     def get_descendant(self, node, current_axe, result, or_self):
         children_of_node = node.children
         if self.current_axe.is_attribute:
             if or_self:
                 self.get_attributes(node, current_axe, result)
         else:
-            self.get_children(node, self.current_axe, result)
+            self.get_children(node, self.current_axe, result,
+                              self.static_context)
 
         for child in children_of_node:
             result = self.get_descendant(child, current_axe, result, True)
         return result
 
     def visitAxisStep(self, ctx: XQueryParser.AxisStepContext):
         list_result = []
@@ -1290,15 +1298,16 @@
                     self.get_descendant(node,
                                         self.current_axe,
                                         list_result,
                                         or_self=False)
                 elif self.current_axe.is_attribute:
                     self.get_attributes(node, self.current_axe, list_result)
                 elif self.current_axe.navigation_step == NavigationStep.CHILD:
-                    self.get_children(node, self.current_axe, list_result)
+                    self.get_children(node, self.current_axe, list_result,
+                                      self.static_context)
             except Exception as Error:
                 # no  node or attribute with this name.
                 pass
         list_node_to_test = list_result
 
         list_predicate = ctx.predicateList()
 
@@ -1415,20 +1424,22 @@
             if not isinstance(result, list):
                 result = [result]
 
             value_node = None
             for res_item in result:
                 if isinstance(res_item, DynamicContext):
                     if res_item.is_node():
-                        res_item.node._parent = self
-                        node.append_child(res_item)
+                        res_item.node.parent = self
+                        node[None] = res_item
                     elif res_item.is_attribute():
-                        node.add_attribute(res_item.name,
-                                           res_item.value,
-                                           res_item.namespace_uri)
+                        node @= (
+                            res_item.name,
+                            res_item.namespace_uri,
+                            res_item.value
+                        )
                     else:
                         if value_node is None:
                             value_node = DrbQueryFuncUtil.get_value(
                                 res_item)
                         else:
                             value_node = str(value_node) + \
                                          DrbQueryFuncUtil.get_string(
@@ -1437,15 +1448,15 @@
                 else:
                     if value_node is None:
                         value_node = DrbQueryFuncUtil.get_value(res_item)
                     else:
                         value_node = str(value_node) + \
                                      DrbQueryFuncUtil.get_string(res_item)
 
-            node._value = value_node
+            node.value = value_node
         return DynamicContext(node=node)
 
     def visitLetBinding(self, ctx: XQueryParser.LetBindingContext):
         var_namespace = None
         varname = self.visitVarName(ctx.varName())
         type_var = None
```

### Comparing `drb-xquery-1.1.0/drb/xquery/execptions.py` & `drb-xquery-1.2.0/drb/xquery/execptions.py`

 * *Files identical despite different names*

### Comparing `drb-xquery-1.1.0/drb_xquery.egg-info/PKG-INFO` & `drb-xquery-1.2.0/drb_xquery.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: drb-xquery
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB xquery request
-Home-page: https://gitlab.com/drb-python/xquery
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # Xquery for DRB
 This xquery module allows execute xquery on DRB nodes.
 
 ## Using this module
 To include this module into your project, the `drb-xquery` module shall be 
 referenced into `requirement.txt` file, or the following pip line can be run:
@@ -192,9 +190,7 @@
 ```
 doc("catalog.xml")/catalog/product[position() = (1 to 3)]
 ```
 
 For compare function the result is only -1,0, 1 , in java thi function return a
 negative value that can be different to -1 or a positive value that represent a
 difference between the two string...
-
-
```

### Comparing `drb-xquery-1.1.0/drb_xquery.egg-info/SOURCES.txt` & `drb-xquery-1.2.0/drb_xquery.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-.coveragerc
-.gitignore
-.gitlab-ci.yml
+LICENCE.txt
 MANIFEST.in
-Makefile
 README.md
-requirements-dev.txt
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 drb/signatures/xquery.py
-drb/xquery/XQueryLexer.g4
-drb/xquery/XQueryLexer.interp
 drb/xquery/XQueryLexer.py
-drb/xquery/XQueryLexer.tokens
-drb/xquery/XQueryParser.g4
-drb/xquery/XQueryParser.interp
 drb/xquery/XQueryParser.py
-drb/xquery/XQueryParser.tokens
 drb/xquery/XQueryParserListener.py
 drb/xquery/XQueryParserVisitor.py
 drb/xquery/__init__.py
 drb/xquery/_version.py
 drb/xquery/drb_xquery.py
 drb/xquery/drb_xquery_cmd.py
 drb/xquery/drb_xquery_context.py
@@ -32,9 +23,10 @@
 drb/xquery/drb_xquery_variable.py
 drb/xquery/drb_xquery_visitor.py
 drb/xquery/execptions.py
 drb_xquery.egg-info/PKG-INFO
 drb_xquery.egg-info/SOURCES.txt
 drb_xquery.egg-info/dependency_links.txt
 drb_xquery.egg-info/entry_points.txt
+drb_xquery.egg-info/not-zip-safe
 drb_xquery.egg-info/requires.txt
 drb_xquery.egg-info/top_level.txt
```

### Comparing `drb-xquery-1.1.0/versioneer.py` & `drb-xquery-1.2.0/versioneer.py`

 * *Files identical despite different names*


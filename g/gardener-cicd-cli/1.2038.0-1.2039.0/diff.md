# Comparing `tmp/gardener-cicd-cli-1.2038.0.tar.gz` & `tmp/gardener-cicd-cli-1.2039.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-cli-1.2038.0.tar", last modified: Mon Apr 24 11:38:26 2023, max compression
+gzip compressed data, was "gardener-cicd-cli-1.2039.0.tar", last modified: Wed Apr 26 09:06:53 2023, max compression
```

## Comparing `gardener-cicd-cli-1.2038.0.tar` & `gardener-cicd-cli-1.2039.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:38:26.096710 gardener-cicd-cli-1.2038.0/
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-24 11:38:26.096710 gardener-cicd-cli-1.2038.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:38:26.088710 gardener-cicd-cli-1.2038.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)    10484 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/bin/component-cli
--rwxr-xr-x   0 root         (0) root         (0)      369 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/bin/helm
--rwxr-xr-x   0 root         (0) root         (0)     5611 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/bin/launch-dockerd.sh
--rwxr-xr-x   0 root         (0) root         (0)     3301 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/bin/purge_history
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/bin/yaml2json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:38:26.092710 gardener-cicd-cli-1.2038.0/gardener_ci/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/_cfg_mgmt.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/_clamav.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/_concourse.py
--rw-r--r--   0 root         (0) root         (0)     7657 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/_oci.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/_osinfo.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/_slack.py
--rw-r--r--   0 root         (0) root         (0)    11329 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/bdba.py
--rw-r--r--   0 root         (0) root         (0)     8458 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/cd.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/checkmarx_cli.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/cli_gen.py
--rw-r--r--   0 root         (0) root         (0)     7669 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/compliance.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/config.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/containerutil.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/docker.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/elastic.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/gh.py
--rw-r--r--   0 root         (0) root         (0)     4935 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/githubutil.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/ocm.py
--rw-r--r--   0 root         (0) root         (0)    12274 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/productutil_v2.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/whdutil.py
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/gardener_ci/yaml2json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:38:26.096710 gardener-cicd-cli-1.2038.0/gardener_cicd_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-24 11:38:26.000000 gardener-cicd-cli-1.2038.0/gardener_cicd_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      960 2023-04-24 11:38:26.000000 gardener-cicd-cli-1.2038.0/gardener_cicd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 11:38:26.000000 gardener-cicd-cli-1.2038.0/gardener_cicd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-04-24 11:38:26.000000 gardener-cicd-cli-1.2038.0/gardener_cicd_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-24 11:38:26.000000 gardener-cicd-cli-1.2038.0/gardener_cicd_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-24 11:38:26.000000 gardener-cicd-cli-1.2038.0/gardener_cicd_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 11:38:26.096710 gardener-cicd-cli-1.2038.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1514 2023-04-24 11:36:41.000000 gardener-cicd-cli-1.2038.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:53.553037 gardener-cicd-cli-1.2039.0/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-26 09:06:53.553037 gardener-cicd-cli-1.2039.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:53.549036 gardener-cicd-cli-1.2039.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    10484 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/bin/component-cli
+-rwxr-xr-x   0 root         (0) root         (0)      369 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/bin/helm
+-rwxr-xr-x   0 root         (0) root         (0)     5611 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/bin/launch-dockerd.sh
+-rwxr-xr-x   0 root         (0) root         (0)     3301 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/bin/purge_history
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/bin/yaml2json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:53.553037 gardener-cicd-cli-1.2039.0/gardener_ci/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/_cfg_mgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/_clamav.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/_concourse.py
+-rw-r--r--   0 root         (0) root         (0)     7657 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/_oci.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/_osinfo.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/_slack.py
+-rw-r--r--   0 root         (0) root         (0)    11329 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/bdba.py
+-rw-r--r--   0 root         (0) root         (0)     8458 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/cd.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/checkmarx_cli.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/cli_gen.py
+-rw-r--r--   0 root         (0) root         (0)     7669 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/compliance.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/config.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/containerutil.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/docker.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/elastic.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/gh.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/githubutil.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/ocm.py
+-rw-r--r--   0 root         (0) root         (0)    12274 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/productutil_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/whdutil.py
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/gardener_ci/yaml2json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:53.553037 gardener-cicd-cli-1.2039.0/gardener_cicd_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-26 09:06:53.000000 gardener-cicd-cli-1.2039.0/gardener_cicd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      960 2023-04-26 09:06:53.000000 gardener-cicd-cli-1.2039.0/gardener_cicd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:06:53.000000 gardener-cicd-cli-1.2039.0/gardener_cicd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-04-26 09:06:53.000000 gardener-cicd-cli-1.2039.0/gardener_cicd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-26 09:06:53.000000 gardener-cicd-cli-1.2039.0/gardener_cicd_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-26 09:06:53.000000 gardener-cicd-cli-1.2039.0/gardener_cicd_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 09:06:53.553037 gardener-cicd-cli-1.2039.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-04-26 08:39:59.000000 gardener-cicd-cli-1.2039.0/setup.py
```

### Comparing `gardener-cicd-cli-1.2038.0/bin/component-cli` & `gardener-cicd-cli-1.2039.0/bin/component-cli`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/bin/launch-dockerd.sh` & `gardener-cicd-cli-1.2039.0/bin/launch-dockerd.sh`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/bin/purge_history` & `gardener-cicd-cli-1.2039.0/bin/purge_history`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/_cfg_mgmt.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/_cfg_mgmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/_clamav.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/_clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/_concourse.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/_concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/_oci.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/_oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/_osinfo.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/_osinfo.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/bdba.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/bdba.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/cd.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/cd.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/checkmarx_cli.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/checkmarx_cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/cli_gen.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/cli_gen.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/compliance.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/compliance.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/config.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/config.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/containerutil.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/containerutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/docker.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/docker.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/elastic.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/elastic.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/gh.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/gh.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/githubutil.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/githubutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/ocm.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/ocm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import enum
+
 import gci.componentmodel as cm
 
 import cnudie.retrieve
 import cnudie.iter
 import ctx
 
 
@@ -12,14 +14,15 @@
     name: str,
     version: str=None,
     ctx_base_url: str=None,
     components: bool=True,
     sources: bool=True,
     resources: bool=True,
     print_expr: str=None,
+    filter_expr: str=None,
 ):
     '''
     name: either component-name, or <component-name>:<version>
     version: optional, if not passed w/ name (no value-checking will be done!)
     components: whether to print components
     sources: whether to print sources
     resources: whether to print resources
@@ -46,36 +49,58 @@
     component = component_descriptor.component
 
     for node in cnudie.iter.iter(
         component=component,
         lookup=component_descriptor_lookup,
     ):
         indent = len(node.path * 2)
-        if isinstance(node, cnudie.iter.ComponentNode):
-            if not components:
+
+        is_component_node = isinstance(node, cnudie.iter.ComponentNode)
+        is_source_node = isinstance(node, cnudie.iter.SourceNode)
+        is_resource_node = isinstance(node, cnudie.iter.ResourceNode)
+
+        if is_component_node and not components:
+            continue
+
+        if is_source_node and not sources:
+            continue
+
+        if is_resource_node and not resources:
+            continue
+
+        if filter_expr:
+            if is_component_node:
+                typestr = 'component'
+            elif is_source_node:
+                typestr = node.source.type
+            elif is_resource_node:
+                typestr = node.resource.type
+
+            if isinstance(typestr, enum.Enum):
+                typestr = typestr.value
+
+            if not eval(filter_expr, {
+                'node': node,
+                'type': typestr,
+            }):
                 continue
 
+        if isinstance(node, cnudie.iter.ComponentNode):
             if not print_expr:
                 prefix = 'c'
                 print(f'{prefix}{" " * indent}{node.component.name}:{node.component.version}')
             else:
                 print(eval(print_expr, {'node': node}))
         if isinstance(node, cnudie.iter.ResourceNode):
-            if not resources:
-                continue
-
             if not print_expr:
                 prefix = 'r'
                 indent += 1
                 print(f'{prefix}{" " * indent}{node.resource.name}')
             else:
                 print(eval(print_expr, {'node': node}))
         if isinstance(node, cnudie.iter.SourceNode):
-            if not sources:
-                continue
-
             if not print_expr:
                 prefix = 'r'
                 indent += 1
                 print(f'{prefix}{" " * indent}{node.source.name}')
             else:
                 print(eval(print_expr, {'node': node}))
```

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/pipeline.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/productutil_v2.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/productutil_v2.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_ci/whdutil.py` & `gardener-cicd-cli-1.2039.0/gardener_ci/whdutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/gardener_cicd_cli.egg-info/SOURCES.txt` & `gardener-cicd-cli-1.2039.0/gardener_cicd_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2038.0/setup.py` & `gardener-cicd-cli-1.2039.0/setup.py`

 * *Files identical despite different names*


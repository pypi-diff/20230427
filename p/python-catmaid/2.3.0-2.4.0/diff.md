# Comparing `tmp/python-catmaid-2.3.0.tar.gz` & `tmp/python-catmaid-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-catmaid-2.3.0.tar", last modified: Thu Jan 12 19:54:53 2023, max compression
+gzip compressed data, was "python-catmaid-2.4.0.tar", last modified: Thu Apr 27 15:37:42 2023, max compression
```

## Comparing `python-catmaid-2.3.0.tar` & `python-catmaid-2.4.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 19:54:53.575632 python-catmaid-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-01-12 19:54:53.575632 python-catmaid-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 19:54:53.575632 python-catmaid-2.3.0/pymaid/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    42637 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47329 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    54250 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    42441 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/cytoscape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 19:54:53.575632 python-catmaid-2.3.0/pymaid/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)   182078 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/fetch/landmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/fetch/skeletons.py
--rw-r--r--   0 runner    (1001) docker     (123)    32422 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/morpho.py
--rw-r--r--   0 runner    (1001) docker     (123)    42045 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)   109417 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/user_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/pymaid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 19:54:53.575632 python-catmaid-2.3.0/python_catmaid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-01-12 19:54:53.000000 python-catmaid-2.3.0/python_catmaid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-12 19:54:53.000000 python-catmaid-2.3.0/python_catmaid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 19:54:53.000000 python-catmaid-2.3.0/python_catmaid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 19:54:53.000000 python-catmaid-2.3.0/python_catmaid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-01-12 19:54:53.000000 python-catmaid-2.3.0/python_catmaid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-12 19:54:53.000000 python-catmaid-2.3.0/python_catmaid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 19:54:53.575632 python-catmaid-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-01-12 19:54:50.000000 python-catmaid-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:37:42.866945 python-catmaid-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-27 15:37:42.866945 python-catmaid-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:37:42.866945 python-catmaid-2.4.0/pymaid/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42637 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47329 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54250 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42441 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/cytoscape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:37:42.866945 python-catmaid-2.4.0/pymaid/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)   176385 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17056 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/fetch/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/fetch/landmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/fetch/skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32422 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/morpho.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42045 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109417 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/pymaid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:37:42.866945 python-catmaid-2.4.0/python_catmaid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-27 15:37:42.000000 python-catmaid-2.4.0/python_catmaid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-27 15:37:42.000000 python-catmaid-2.4.0/python_catmaid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:37:42.000000 python-catmaid-2.4.0/python_catmaid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:37:42.000000 python-catmaid-2.4.0/python_catmaid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-27 15:37:42.000000 python-catmaid-2.4.0/python_catmaid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 15:37:42.000000 python-catmaid-2.4.0/python_catmaid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:37:42.866945 python-catmaid-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-27 15:37:37.000000 python-catmaid-2.4.0/setup.py
```

### Comparing `python-catmaid-2.3.0/LICENSE` & `python-catmaid-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/PKG-INFO` & `python-catmaid-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-catmaid
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python interface to CATMAID servers
 Home-page: https://github.com/navis-org/pymaid
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, http://pymaid.readthedocs.io
 Project-URL: Source, https://github.com/navis-org/pymaid
```

### Comparing `python-catmaid-2.3.0/README.md` & `python-catmaid-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/__init__.py` & `python-catmaid-2.4.0/pymaid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-__version__ = "2.3.0"
-__version_vector__ = (2, 3, 0)
+__version__ = "2.4.0"
+__version_vector__ = (2, 4, 0)
 
 from . import config
 
 logger = config.get_logger(__name__)
 
 # Flatten namespace by importing contents of all modules of pymaid
 from .fetch import *
```

### Comparing `python-catmaid-2.3.0/pymaid/cache.py` & `python-catmaid-2.4.0/pymaid/cache.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/client.py` & `python-catmaid-2.4.0/pymaid/client.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/cluster.py` & `python-catmaid-2.4.0/pymaid/cluster.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/config.py` & `python-catmaid-2.4.0/pymaid/config.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/connectivity.py` & `python-catmaid-2.4.0/pymaid/connectivity.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/core.py` & `python-catmaid-2.4.0/pymaid/core.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/cytoscape.py` & `python-catmaid-2.4.0/pymaid/cytoscape.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/fetch/__init__.py` & `python-catmaid-2.4.0/pymaid/fetch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,22 +52,24 @@
 import networkx as nx
 import pandas as pd
 
 from .. import core, utils, config, cache
 from navis import in_volume
 from .landmarks import get_landmarks, get_landmark_groups
 from .skeletons import get_skeleton_ids
+from .annotations import get_annotation_graph, get_entity_graph, get_annotation_id
 
 
 __all__ = ['get_annotation_details', 'get_annotation_id',
                   'get_annotation_list', 'get_annotations', 'get_annotation_graph',
                   'get_arbor',
                   'get_connector_details', 'get_connectors',
                   'get_connector_tags',
-                  'get_contributor_statistics', 'get_edges', 'get_history',
+                  'get_contributor_statistics', 'get_edges', 'get_entity_graph',
+                  'get_history',
                   'get_logs', 'get_names', 'get_neuron',
                   'get_neurons', 'get_neurons_in_bbox',
                   'get_neurons_in_volume', 'get_node_tags', 'get_node_details',
                   'get_nodes_in_volume', 'get_partners',
                   'get_partners_in_volume', 'get_paths', 'get_review',
                   'get_review_details', 'get_skids_by_annotation',
                   'get_skids_by_name', 'get_node_info',
@@ -1897,199 +1899,14 @@
 
         return(annotation_list)
     except BaseException:
         raise Exception(
             'No annotations retrieved. Make sure that the skeleton IDs exist.')
 
 
-def _entities_to_ann_graph(data, annotations_by_id=False, skeletons_by_id=True):
-    ann_ref = "id" if annotations_by_id else "name"
-    skel_ref = "id" if skeletons_by_id else "name"
-
-    g = nx.DiGraph()
-
-    for e in data["entities"]:
-        is_meta_ann = False
-
-        if e.get("type") == "neuron":
-            skids = e.get("skeleton_ids") or []
-            if len(skids) != 1:
-                logger.warning("Neuron with id %s is modelled by %s skeletons, ignoring", e["id"], len(skids))
-                continue
-            node_data = {
-                "name": e["name"],
-                "neuron_id": e["id"],
-                "is_skeleton": True,
-                "id": skids[0],
-            }
-            node_id = node_data[skel_ref]
-        else:  # is an annotation
-            node_data = {
-                "is_skeleton": False,
-                "id": e["id"],
-                "name": e["name"],
-            }
-            node_id = node_data[ann_ref]
-            is_meta_ann = True
-
-        anns = e.get("annotations", [])
-        if not anns:
-            g.add_node(node_id, **node_data)
-            continue
-
-        for ann in e.get("annotations", []):
-            g.add_edge(
-                ann[ann_ref],
-                node_id,
-                is_meta_annotation=is_meta_ann,
-            )
-
-        g.nodes[node_id].update(**node_data)
-
-    return g
-
-
-@cache.undo_on_error
-def get_annotation_graph(annotations_by_id=False, skeletons_by_id=True, remote_instance=None) -> nx.DiGraph:
-    """Get a networkx DiGraph of (meta)annotations and skeletons.
-
-    Can be slow for large projects.
-
-    Nodes in the graph have data:
-
-    Skeletons have
-    - id
-    - is_skeleton = True
-    - neuron_id (different to the skeleton ID)
-    - name
-
-    Annotations have
-    - id
-    - name
-    - is_skeleton = False
-
-    Edges in the graph have
-    - is_meta_annotation (whether it is between two annotations)
-
-    Parameters
-    ----------
-    annotations_by_id : bool, default False
-        Whether to index nodes representing annotations by their integer ID
-        (uses name by default)
-    skeletons_by_id : bool, default True
-        whether to index nodes representing skeletons by their integer ID
-        (True by default, otherwise uses the neuron name)
-    remote_instance : optional CatmaidInstance
-
-    Returns
-    -------
-    networkx.DiGraph
-    """
-    remote_instance = utils._eval_remote_instance(remote_instance)
-
-    query_url = remote_instance.make_url(remote_instance.project_id, "annotations", "query-targets")
-    post = {
-        "with_annotations": True,
-    }
-    data = remote_instance.fetch(query_url, post)
-
-    return _entities_to_ann_graph(data, annotations_by_id, skeletons_by_id)
-
-
-def filter_by_query(names: pd.Series, query: str, allow_partial: bool = False) -> pd.Series:
-    """Get a logical index series into a series of strings based on a query.
-
-    Parameters
-    ----------
-    names : pd.Series of str
-        Dataframe column of strings to filter
-    query : str
-        Query string. leading "~" and "annotation:" will be ignored.
-        Leading "/" will mean the remainder is used as a regex.
-    allow_partial : bool, default False
-        For non-regex queries, whether to check that the query is an exact match or just contained in the name.
-
-    Returns
-    -------
-    pd.Series of bool
-        Which names match the given query
-    """
-    if not isinstance(names, pd.Series):
-        names = pd.Series(names, dtype=str)
-
-    for prefix in ["annotation:", "~"]:
-        if query.startswith(prefix):
-            logger.warning("Removing '%s' prefix from '%s'", prefix, query)
-            query = query[len(prefix):]
-
-    q = query.strip()
-    # use a regex
-    if q.startswith("/"):
-        re_str = q[1:]
-        filt = names.str.match(re_str)
-    else:
-        filt = names.str.contains(q, regex=False)
-        if not allow_partial:
-            filt = np.logical_and(filt, names.str.len() == len(q))
-
-    return filt
-
-
-@cache.wipe_and_retry
-def get_annotation_id(annotations, allow_partial=False, raise_not_found=True,
-                    remote_instance=None):
-    """Retrieve the annotation ID for single or list of annotation(s).
-
-    Parameters
-    ----------
-    annotations :       str | list of str
-                        Single annotations or list of multiple annotations.
-    allow_partial :     bool, optional
-                        If True, will allow partial matches.
-    raise_not_found :   bool, optional
-                        If True raise Exception if no match for any of the
-                        query annotations is found. Else log warning.
-    remote_instance :   CatmaidInstance, optional
-                        If not passed directly, will try using global.
-
-    Returns
-    -------
-    dict
-                        ``{'annotation_name': 'annotation_id', ...}``
-
-    """
-    remote_instance = utils._eval_remote_instance(remote_instance)
-
-    logger.debug('Retrieving list of annotations...')
-
-    remote_annotation_list_url = remote_instance._get_annotation_list()
-    an_list = remote_instance.fetch(remote_annotation_list_url)
-
-    # Turn into pandas array
-    an_list = pd.DataFrame.from_records(an_list['annotations'])
-
-    annotations = utils._make_iterable(annotations)
-    annotation_ids = {}
-    for an in annotations:
-        filt = filter_by_query(an_list.name, an, allow_partial)
-
-        # Search for matches
-        res = an_list[filt].set_index('name').id.to_dict()
-        if not res:
-            logger.warning('No annotation found for "{}"'.format(an))
-        annotation_ids.update(res)
-
-    if not annotation_ids:
-        if raise_not_found:
-            raise Exception('No matching annotation(s) found')
-        else:
-            logger.warning('No matching annotation(s) found')
-
-    return annotation_ids
-
 
 @cache.undo_on_error
 def find_nodes(tags=None, node_ids=None, skeleton_ids=None,
                    remote_instance=None):
     """Get nodes by tag (label), ID or associated skeleton.
 
     Search intersected (logical AND) across parameters but additive (logical OR)
@@ -3928,15 +3745,15 @@
 
     sources = utils.eval_skids(sources, remote_instance=remote_instance)
     targets = utils.eval_skids(targets, remote_instance=remote_instance)
 
     targets = utils._make_iterable(targets).astype(int)
     sources = utils._make_iterable(sources).astype(int)
 
-    if isinstance(n_hops, (int, np.int)):
+    if isinstance(n_hops, (int, np.integer)):
         n_hops = [n_hops]
 
     if not utils._is_iterable(n_hops):
         raise TypeError('Expected `n_hops` to be iterable or integer, got '
                         f'"{type(n_hops)}"')
 
     if min(n_hops) <= 0:
```

### Comparing `python-catmaid-2.3.0/pymaid/fetch/landmarks.py` & `python-catmaid-2.4.0/pymaid/fetch/landmarks.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/fetch/skeletons.py` & `python-catmaid-2.4.0/pymaid/fetch/skeletons.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/morpho.py` & `python-catmaid-2.4.0/pymaid/morpho.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/tiles.py` & `python-catmaid-2.4.0/pymaid/tiles.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/upload.py` & `python-catmaid-2.4.0/pymaid/upload.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/user_stats.py` & `python-catmaid-2.4.0/pymaid/user_stats.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/pymaid/utils.py` & `python-catmaid-2.4.0/pymaid/utils.py`

 * *Files identical despite different names*

### Comparing `python-catmaid-2.3.0/python_catmaid.egg-info/PKG-INFO` & `python-catmaid-2.4.0/python_catmaid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-catmaid
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python interface to CATMAID servers
 Home-page: https://github.com/navis-org/pymaid
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, http://pymaid.readthedocs.io
 Project-URL: Source, https://github.com/navis-org/pymaid
```

### Comparing `python-catmaid-2.3.0/python_catmaid.egg-info/SOURCES.txt` & `python-catmaid-2.4.0/python_catmaid.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 pymaid/cytoscape.py
 pymaid/morpho.py
 pymaid/tiles.py
 pymaid/upload.py
 pymaid/user_stats.py
 pymaid/utils.py
 pymaid/fetch/__init__.py
+pymaid/fetch/annotations.py
 pymaid/fetch/landmarks.py
 pymaid/fetch/skeletons.py
 python_catmaid.egg-info/PKG-INFO
 python_catmaid.egg-info/SOURCES.txt
 python_catmaid.egg-info/dependency_links.txt
 python_catmaid.egg-info/not-zip-safe
 python_catmaid.egg-info/requires.txt
```

### Comparing `python-catmaid-2.3.0/setup.py` & `python-catmaid-2.4.0/setup.py`

 * *Files identical despite different names*


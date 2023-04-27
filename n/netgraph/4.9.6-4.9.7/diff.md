# Comparing `tmp/netgraph-4.9.6.tar.gz` & `tmp/netgraph-4.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/netgraph-4.9.6.tar", last modified: Mon Sep  5 16:54:22 2022, max compression
+gzip compressed data, was "dist/netgraph-4.9.7.tar", last modified: Wed Sep 28 12:15:52 2022, max compression
```

## Comparing `netgraph-4.9.6.tar` & `netgraph-4.9.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2022-09-05 16:54:22.000000 netgraph-4.9.6/
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2022-09-05 16:54:22.000000 netgraph-4.9.6/netgraph/
--rwxrwxr-x   0 paul      (1000) paul      (1000)    21231 2022-04-19 17:57:59.000000 netgraph-4.9.6/netgraph/_interactive_variants.py
--rwxrwxr-x   0 paul      (1000) paul      (1000)    66309 2022-09-05 16:53:40.000000 netgraph-4.9.6/netgraph/_node_layout.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     1934 2022-04-19 17:57:59.000000 netgraph-4.9.6/netgraph/_line_supercover.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     9994 2022-08-30 13:52:45.000000 netgraph-4.9.6/netgraph/_artists.py
--rwxrwxr-x   0 paul      (1000) paul      (1000)     3434 2022-09-05 16:53:40.000000 netgraph-4.9.6/netgraph/__init__.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    46275 2022-04-28 11:58:46.000000 netgraph-4.9.6/netgraph/_arcdiagram.py
--rwxrwxr-x   0 paul      (1000) paul      (1000)   111546 2022-09-05 16:53:40.000000 netgraph-4.9.6/netgraph/_main.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     2300 2022-04-19 17:57:59.000000 netgraph-4.9.6/netgraph/_deprecated.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    18928 2022-09-05 12:07:46.000000 netgraph-4.9.6/netgraph/_utils.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     8226 2022-08-30 13:52:45.000000 netgraph-4.9.6/netgraph/_parser.py
--rwxrwxr-x   0 paul      (1000) paul      (1000)    34522 2022-09-05 16:15:20.000000 netgraph-4.9.6/netgraph/_edge_layout.py
--rwxrwxrwx   0 paul      (1000) paul      (1000)    35141 2017-11-21 20:08:53.000000 netgraph-4.9.6/LICENSE.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)    11212 2022-09-05 16:53:40.000000 netgraph-4.9.6/README.md
--rw-rw-r--   0 paul      (1000) paul      (1000)     1380 2022-09-05 16:53:40.000000 netgraph-4.9.6/setup.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    14695 2022-09-05 16:54:22.000000 netgraph-4.9.6/PKG-INFO
--rwxrwxrwx   0 paul      (1000) paul      (1000)       79 2022-09-05 16:54:22.000000 netgraph-4.9.6/setup.cfg
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2022-09-05 16:54:22.000000 netgraph-4.9.6/netgraph.egg-info/
--rwxrwxrwx   0 paul      (1000) paul      (1000)      459 2022-09-05 16:54:22.000000 netgraph-4.9.6/netgraph.egg-info/SOURCES.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)        9 2022-09-05 16:54:22.000000 netgraph-4.9.6/netgraph.egg-info/top_level.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)    14695 2022-09-05 16:54:22.000000 netgraph-4.9.6/netgraph.egg-info/PKG-INFO
--rwxrwxrwx   0 paul      (1000) paul      (1000)       76 2022-09-05 16:54:22.000000 netgraph-4.9.6/netgraph.egg-info/requires.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)        1 2022-09-05 16:54:22.000000 netgraph-4.9.6/netgraph.egg-info/dependency_links.txt
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2022-09-28 12:15:52.000000 netgraph-4.9.7/
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2022-09-28 12:15:52.000000 netgraph-4.9.7/netgraph/
+-rwxrwxr-x   0 paul      (1000) paul      (1000)    21231 2022-04-19 17:57:59.000000 netgraph-4.9.7/netgraph/_interactive_variants.py
+-rwxrwxr-x   0 paul      (1000) paul      (1000)    66309 2022-09-27 15:17:59.000000 netgraph-4.9.7/netgraph/_node_layout.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1934 2022-04-19 17:57:59.000000 netgraph-4.9.7/netgraph/_line_supercover.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     9994 2022-08-30 13:52:45.000000 netgraph-4.9.7/netgraph/_artists.py
+-rwxrwxr-x   0 paul      (1000) paul      (1000)     3434 2022-09-28 12:14:45.000000 netgraph-4.9.7/netgraph/__init__.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    46275 2022-04-28 11:58:46.000000 netgraph-4.9.7/netgraph/_arcdiagram.py
+-rwxrwxr-x   0 paul      (1000) paul      (1000)   111546 2022-09-27 15:17:59.000000 netgraph-4.9.7/netgraph/_main.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     2300 2022-04-19 17:57:59.000000 netgraph-4.9.7/netgraph/_deprecated.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    18928 2022-09-05 12:07:46.000000 netgraph-4.9.7/netgraph/_utils.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     8226 2022-08-30 13:52:45.000000 netgraph-4.9.7/netgraph/_parser.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    42556 2022-09-28 12:14:45.000000 netgraph-4.9.7/netgraph/_edge_layout.py
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    35141 2017-11-21 20:08:53.000000 netgraph-4.9.7/LICENSE.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)    11347 2022-09-28 12:14:45.000000 netgraph-4.9.7/README.md
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1380 2022-09-28 12:14:45.000000 netgraph-4.9.7/setup.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    14838 2022-09-28 12:15:52.000000 netgraph-4.9.7/PKG-INFO
+-rwxrwxrwx   0 paul      (1000) paul      (1000)       79 2022-09-28 12:15:52.000000 netgraph-4.9.7/setup.cfg
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2022-09-28 12:15:52.000000 netgraph-4.9.7/netgraph.egg-info/
+-rwxrwxrwx   0 paul      (1000) paul      (1000)      459 2022-09-28 12:15:52.000000 netgraph-4.9.7/netgraph.egg-info/SOURCES.txt
+-rwxrwxrwx   0 paul      (1000) paul      (1000)        9 2022-09-28 12:15:52.000000 netgraph-4.9.7/netgraph.egg-info/top_level.txt
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    14838 2022-09-28 12:15:52.000000 netgraph-4.9.7/netgraph.egg-info/PKG-INFO
+-rwxrwxrwx   0 paul      (1000) paul      (1000)       76 2022-09-28 12:15:52.000000 netgraph-4.9.7/netgraph.egg-info/requires.txt
+-rwxrwxrwx   0 paul      (1000) paul      (1000)        1 2022-09-28 12:15:52.000000 netgraph-4.9.7/netgraph.egg-info/dependency_links.txt
```

### Comparing `netgraph-4.9.6/netgraph/_interactive_variants.py` & `netgraph-4.9.7/netgraph/_interactive_variants.py`

 * *Files identical despite different names*

### Comparing `netgraph-4.9.6/netgraph/_node_layout.py` & `netgraph-4.9.7/netgraph/_node_layout.py`

 * *Files identical despite different names*

### Comparing `netgraph-4.9.6/netgraph/_line_supercover.py` & `netgraph-4.9.7/netgraph/_line_supercover.py`

 * *Files identical despite different names*

### Comparing `netgraph-4.9.6/netgraph/_artists.py` & `netgraph-4.9.7/netgraph/_artists.py`

 * *Files identical despite different names*

### Comparing `netgraph-4.9.6/netgraph/__init__.py` & `netgraph-4.9.7/netgraph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 >>> # Otherwise, the plot instance will be garbage collected after the initial draw
 >>> # and you won't be able to move the plot elements around.
 >>> plt.ion()
 >>> plot_instance = InteractiveGraph(graph_data)
 >>> plt.show()
 """
 
-__version__ = "4.9.6"
+__version__ = "4.9.7"
 __author__ = "Paul Brodersen"
 __email__ = "paulbrodersen+netgraph@gmail.com"
 
 from ._main import (
     BaseGraph,
     Graph,
     InteractiveGraph,
```

### Comparing `netgraph-4.9.6/netgraph/_arcdiagram.py` & `netgraph-4.9.7/netgraph/_arcdiagram.py`

 * *Files identical despite different names*

### Comparing `netgraph-4.9.6/netgraph/_main.py` & `netgraph-4.9.7/netgraph/_main.py`

 * *Files identical despite different names*

### Comparing `netgraph-4.9.6/netgraph/_deprecated.py` & `netgraph-4.9.7/netgraph/_deprecated.py`

 * *Files identical despite different names*

### Comparing `netgraph-4.9.6/netgraph/_utils.py` & `netgraph-4.9.7/netgraph/_utils.py`

 * *Files identical despite different names*

### Comparing `netgraph-4.9.6/netgraph/_parser.py` & `netgraph-4.9.7/netgraph/_parser.py`

 * *Files identical despite different names*

### Comparing `netgraph-4.9.6/netgraph/_edge_layout.py` & `netgraph-4.9.7/netgraph/_edge_layout.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,36 +16,25 @@
 
 from ._utils import (
     _bspline,
     _get_n_points_on_a_circle,
     _get_angle,
     _get_unit_vector,
     _edge_list_to_adjacency_list,
+    _edge_list_to_adjacency_matrix,
     _get_connected_components,
 )
 
-
-# monkeypatch repulsive force
-def _get_fr_repulsion(distance, direction, k):
-    """Compute repulsive forces.
-
-    This is a variant of the implementation in the original FR
-    algorithm, in as much as repulsion only acts between fixed nodes
-    and mobile nodes, not between fixed nodes and other fixed nodes.
-    """
-    total_mobile = distance.shape[1]
-    distance = distance[total_mobile:]
-    direction = direction[total_mobile:]
-    magnitude = k**2 / distance
-    vectors = direction * magnitude[..., None]
-    return np.sum(vectors, axis=0)
-
-import netgraph._node_layout
-netgraph._node_layout._get_fr_repulsion = _get_fr_repulsion
-from netgraph._node_layout import get_fruchterman_reingold_layout, _clip_to_frame
+from ._node_layout import (
+    _get_temperature_decay,
+    _is_within_bbox,
+    _rescale_to_frame,
+    _get_fr_attraction,
+    _clip_to_frame,
+)
 
 
 # for profiling with kernprof/line_profiler
 try:
     profile
 except NameError:
     profile = lambda x: x
@@ -404,29 +393,204 @@
 
     # increase size of nodes so that there is a bit more clearance between edges and nodes
     node_size = {node : 2 * size for node, size in node_size.items()}
 
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", category=UserWarning)
 
-        expanded_node_positions = get_fruchterman_reingold_layout.__wrapped__(
+        expanded_node_positions = _get_fruchterman_reingold_layout(
             expanded_edges,
             node_positions      = expanded_node_positions,
             scale               = scale,
             origin              = origin,
             k                   = k,
             initial_temperature = initial_temperature,
             total_iterations    = total_iterations,
             node_size           = node_size,
             fixed_nodes         = nodes,
         )
 
     return {node : xy for node, xy in expanded_node_positions.items() if node not in nodes}
 
 
+# This is a (slightly simplified) copy of the function defined in _node_layout.
+# This allows us to redefine the internally called function _get_fr_repulsion.
+# TODO: find a way to avoid code repetition.
+# NOTE: Monkey patching did not work as intended (commit 435f187f99b8ff43d1d573c5e9302ea92cfa7eb2).
+def _get_fruchterman_reingold_layout(edges,
+                                     edge_weights        = None,
+                                     k                   = None,
+                                     scale               = None,
+                                     origin              = None,
+                                     initial_temperature = 1.,
+                                     total_iterations    = 50,
+                                     node_size           = 0,
+                                     node_positions      = None,
+                                     fixed_nodes         = None,
+                                     *args, **kwargs):
+    """'Spring' or Fruchterman-Reingold node layout.
+
+    Uses the Fruchterman-Reingold algorithm [Fruchterman1991]_ to compute node positions.
+    This algorithm simulates the graph as a physical system, in which nodes repell each other.
+    For connected nodes, this repulsion is counteracted by an attractive force exerted by the edges, which are simulated as springs.
+    The resulting layout is hence often referred to as a 'spring' layout.
+
+    Parameters
+    ----------
+    edges : list
+        The edges of the graph, with each edge being represented by a (source node ID, target node ID) tuple.
+    edge_weights : dict
+        Mapping of edges to edge weights.
+    k : float or None, default None
+        Expected mean edge length. If None, initialized to the sqrt(area / total nodes).
+    origin : tuple or None, default None
+        The (float x, float y) coordinates corresponding to the lower left hand corner of the bounding box specifying the extent of the canvas.
+        If None is given, the origin is placed at (0, 0).
+    scale : tuple or None, default None
+        The (float x, float y) dimensions representing the width and height of the bounding box specifying the extent of the canvas.
+        If None is given, the scale is set to (1, 1).
+    total_iterations : int, default 50
+        Number of iterations.
+    initial_temperature: float, default 1.
+        Temperature controls the maximum node displacement on each iteration.
+        Temperature is decreased on each iteration to eventually force the algorithm into a particular solution.
+        The size of the initial temperature determines how quickly that happens.
+        Values should be much smaller than the values of `scale`.
+    node_size : scalar or dict, default 0.
+        Size (radius) of nodes.
+        Providing the correct node size minimises the overlap of nodes in the graph,
+        which can otherwise occur if there are many nodes, or if the nodes differ considerably in size.
+    node_positions : dict or None, default None
+        Mapping of nodes to their (initial) x,y positions. If None are given,
+        nodes are initially placed randomly within the bounding box defined by `origin` and `scale`.
+        If the graph has multiple components, explicit initial positions may result in a ValueError,
+        if the initial positions fall outside of the area allocated to that specific component.
+    fixed_nodes : list or None, default None
+        Nodes to keep fixed at their initial positions.
+
+    Returns
+    -------
+    node_positions : dict
+        Dictionary mapping each node ID to (float x, float y) tuple, the node position.
+
+    References
+    ----------
+    .. [Fruchterman1991] Fruchterman, TMJ and Reingold, EM (1991) ‘Graph drawing by force‐directed placement’,
+       Software: Practice and Experience
+
+    """
+
+    origin = np.array(origin)
+    scale = np.array(scale)
+
+    unique_nodes = node_positions.keys()
+    node_positions_as_array = np.array([node_positions[node] for node in unique_nodes])
+    node_size = np.array([node_size[node] if node in node_size else 0. for node in unique_nodes])
+
+    adjacency = _edge_list_to_adjacency_matrix(
+        edges, edge_weights=edge_weights, unique_nodes=unique_nodes)
+
+    # Forces in FR are symmetric.
+    # Hence we need to ensure that the adjacency matrix is also symmetric.
+    adjacency = adjacency + adjacency.transpose()
+
+    # reorder adjacency to separate mobile and fixed positions
+    is_mobile = np.array([False if node in fixed_nodes else True for node in unique_nodes], dtype=bool)
+    mobile_positions = node_positions_as_array[is_mobile]
+    fixed_positions = node_positions_as_array[~is_mobile]
+    mobile_node_sizes = node_size[is_mobile]
+    fixed_node_sizes = node_size[~is_mobile]
+    total_mobile = np.sum(is_mobile)
+    reordered = np.zeros((adjacency.shape[0], total_mobile))
+    reordered[:total_mobile, :total_mobile] = adjacency[is_mobile][:, is_mobile]
+    reordered[total_mobile:, :total_mobile] = adjacency[~is_mobile][:, is_mobile]
+    adjacency = reordered
+
+    temperatures = _get_temperature_decay(initial_temperature, total_iterations)
+
+    # --------------------------------------------------------------------------------
+    # main loop
+
+    for ii, temperature in enumerate(temperatures):
+        candidate_positions = _fruchterman_reingold(mobile_positions, fixed_positions,
+                                                    mobile_node_sizes, fixed_node_sizes,
+                                                    adjacency, temperature, k)
+        is_valid = _is_within_bbox(candidate_positions, origin=origin, scale=scale)
+        mobile_positions[is_valid] = candidate_positions[is_valid]
+
+    # --------------------------------------------------------------------------------
+    # format output
+
+    node_positions_as_array[is_mobile] = mobile_positions
+
+    if np.all(is_mobile):
+        node_positions_as_array = _rescale_to_frame(node_positions_as_array, origin, scale)
+
+    node_positions = dict(zip(unique_nodes, node_positions_as_array))
+
+    return node_positions
+
+
+def _fruchterman_reingold(mobile_positions, fixed_positions,
+                          mobile_node_radii, fixed_node_radii,
+                          adjacency, temperature, k):
+    """Inner loop of Fruchterman-Reingold layout algorithm."""
+
+    combined_positions = np.concatenate([mobile_positions, fixed_positions], axis=0)
+    combined_node_radii = np.concatenate([mobile_node_radii, fixed_node_radii])
+
+    delta = mobile_positions[np.newaxis, :, :] - combined_positions[:, np.newaxis, :]
+    distance = np.linalg.norm(delta, axis=-1)
+
+    # alternatively: (hack adapted from igraph)
+    if np.sum(distance==0) - np.trace(distance==0) > 0: # i.e. if off-diagonal entries in distance are zero
+        warnings.warn("Some nodes have the same position; repulsion between the nodes is undefined.")
+        rand_delta = np.random.rand(*delta.shape) * 1e-9
+        is_zero = distance <= 0
+        delta[is_zero] = rand_delta[is_zero]
+        distance = np.linalg.norm(delta, axis=-1)
+
+    # subtract node radii from distances to prevent nodes from overlapping
+    distance -= mobile_node_radii[np.newaxis, :] + combined_node_radii[:, np.newaxis]
+
+    # prevent distances from becoming less than zero due to overlap of nodes
+    distance[distance <= 0.] = 1e-6 # 1e-13 is numerical accuracy, and we will be taking the square shortly
+
+    with np.errstate(divide='ignore', invalid='ignore'):
+        direction = delta / distance[..., None] # i.e. the unit vector
+
+    # calculate forces
+    repulsion    = _get_fr_repulsion(distance, direction, k)
+    attraction   = _get_fr_attraction(distance, direction, adjacency, k)
+    displacement = attraction + repulsion
+
+    # limit maximum displacement using temperature
+    displacement_length = np.linalg.norm(displacement, axis=-1)
+    displacement = displacement / displacement_length[:, None] * np.clip(displacement_length, None, temperature)[:, None]
+
+    mobile_positions = mobile_positions + displacement
+
+    return mobile_positions
+
+
+def _get_fr_repulsion(distance, direction, k):
+    """Compute repulsive forces.
+
+    This is a variant of the implementation in the original FR
+    algorithm, in as much as repulsion only acts between fixed nodes
+    and mobile nodes, not between fixed nodes and other fixed nodes.
+    """
+    total_mobile = distance.shape[1]
+    distance = distance[total_mobile:]
+    direction = direction[total_mobile:]
+    magnitude = k**2 / distance
+    vectors = direction * magnitude[..., None]
+    return np.sum(vectors, axis=0)
+
+
 def _get_path_through_control_points(edge_to_control_points, node_positions, control_point_positions):
     """Map each edge to an array of (optimised) control points positions."""
     edge_to_path = dict()
     for (source, target), control_points in edge_to_control_points.items():
         path = [node_positions[source]] \
             + [control_point_positions[node] for node in control_points] \
             + [node_positions[target]]
```

### Comparing `netgraph-4.9.6/LICENSE.txt` & `netgraph-4.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netgraph-4.9.6/README.md` & `netgraph-4.9.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -281,14 +281,15 @@
 
 ```python
 from netgraph import Graph; help(Graph)
 ```
 
 ## Recent changes
 
+- 4.9.7 Fixed a bug introduced in version 4.9.5 in the computation of repulsive forces in the spring layout (i.e. the default layout).
 - 4.9.6 Fixed issue #51, which occurred in the community node layout if a node had no connections to other nodes in its community.
 - 4.9.5 Improved the routine that reduces node overlaps in the spring and community node layouts.
 - 4.9.4 Fixed a bug that occurred in get_curved_edges if the k parameter was not set explicitly.
 - 4.9.3 Improved placement of nodes in instances where all nodes are aligned within any one dimension.
 - 4.9.2 Fixed an issue that occurred when using the dot node layout for a graphs with multiple components.
 - 4.9.1 Fixed issue #48, which occurred when computing a curved edge layout for graphs with multiple components. Also improved edge routing slightly.
 - 4.9.0 Implemented a layered and a shell layout for multi-partite graphs.
```

### Comparing `netgraph-4.9.6/setup.py` & `netgraph-4.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
-version = '4.9.6'
+version = '4.9.7'
 
 setup(
     name='netgraph',
     version=version,
     description='Python drawing utilities for publication quality plots of networks.',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
```

### Comparing `netgraph-4.9.6/PKG-INFO` & `netgraph-4.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: netgraph
-Version: 4.9.6
+Version: 4.9.7
 Summary: Python drawing utilities for publication quality plots of networks.
 Home-page: https://github.com/paulbrodersen/netgraph
 Author: Paul Brodersen
 Author-email: paulbrodersen+netgraph@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/paulbrodersen/netgraph/archive/4.9.6.tar.gz
+Download-URL: https://github.com/paulbrodersen/netgraph/archive/4.9.7.tar.gz
 Description: # netgraph
         
         [![Downloads](https://pepy.tech/badge/netgraph)](https://pepy.tech/project/netgraph)
         
         Netgraph is a python library for creating publication quality plots of networks.
         Netgraph is compatible with a variety of network data formats, including `networkx` and `igraph` `Graph` objects.
         
@@ -290,14 +290,15 @@
         
         ```python
         from netgraph import Graph; help(Graph)
         ```
         
         ## Recent changes
         
+        - 4.9.7 Fixed a bug introduced in version 4.9.5 in the computation of repulsive forces in the spring layout (i.e. the default layout).
         - 4.9.6 Fixed issue #51, which occurred in the community node layout if a node had no connections to other nodes in its community.
         - 4.9.5 Improved the routine that reduces node overlaps in the spring and community node layouts.
         - 4.9.4 Fixed a bug that occurred in get_curved_edges if the k parameter was not set explicitly.
         - 4.9.3 Improved placement of nodes in instances where all nodes are aligned within any one dimension.
         - 4.9.2 Fixed an issue that occurred when using the dot node layout for a graphs with multiple components.
         - 4.9.1 Fixed issue #48, which occurred when computing a curved edge layout for graphs with multiple components. Also improved edge routing slightly.
         - 4.9.0 Implemented a layered and a shell layout for multi-partite graphs.
```

### Comparing `netgraph-4.9.6/netgraph.egg-info/PKG-INFO` & `netgraph-4.9.7/netgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: netgraph
-Version: 4.9.6
+Version: 4.9.7
 Summary: Python drawing utilities for publication quality plots of networks.
 Home-page: https://github.com/paulbrodersen/netgraph
 Author: Paul Brodersen
 Author-email: paulbrodersen+netgraph@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/paulbrodersen/netgraph/archive/4.9.6.tar.gz
+Download-URL: https://github.com/paulbrodersen/netgraph/archive/4.9.7.tar.gz
 Description: # netgraph
         
         [![Downloads](https://pepy.tech/badge/netgraph)](https://pepy.tech/project/netgraph)
         
         Netgraph is a python library for creating publication quality plots of networks.
         Netgraph is compatible with a variety of network data formats, including `networkx` and `igraph` `Graph` objects.
         
@@ -290,14 +290,15 @@
         
         ```python
         from netgraph import Graph; help(Graph)
         ```
         
         ## Recent changes
         
+        - 4.9.7 Fixed a bug introduced in version 4.9.5 in the computation of repulsive forces in the spring layout (i.e. the default layout).
         - 4.9.6 Fixed issue #51, which occurred in the community node layout if a node had no connections to other nodes in its community.
         - 4.9.5 Improved the routine that reduces node overlaps in the spring and community node layouts.
         - 4.9.4 Fixed a bug that occurred in get_curved_edges if the k parameter was not set explicitly.
         - 4.9.3 Improved placement of nodes in instances where all nodes are aligned within any one dimension.
         - 4.9.2 Fixed an issue that occurred when using the dot node layout for a graphs with multiple components.
         - 4.9.1 Fixed issue #48, which occurred when computing a curved edge layout for graphs with multiple components. Also improved edge routing slightly.
         - 4.9.0 Implemented a layered and a shell layout for multi-partite graphs.
```


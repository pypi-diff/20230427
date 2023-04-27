# Comparing `tmp/matgl-0.1.0.dev0.tar.gz` & `tmp/matgl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.1.0.dev0.tar", last modified: Thu Feb 16 18:20:26 2023, max compression
+gzip compressed data, was "matgl-0.2.0.tar", last modified: Thu Apr 27 02:35:27 2023, max compression
```

## Comparing `matgl-0.1.0.dev0.tar` & `matgl-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-16 18:20:26.979318 matgl-0.1.0.dev0/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)     3230 2023-02-16 18:20:26.979397 matgl-0.1.0.dev0/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     2074 2023-02-16 18:18:25.000000 matgl-0.1.0.dev0/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-16 18:20:26.893909 matgl-0.1.0.dev0/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)       70 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1627 2023-02-16 18:11:34.000000 matgl-0.1.0.dev0/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-16 18:20:26.902685 matgl-0.1.0.dev0/matgl/dataloader/
--rw-r--r--   0 shyue      (501) staff       (20)       53 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/dataloader/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5235 2023-02-16 17:17:15.000000 matgl-0.1.0.dev0/matgl/dataloader/dataset.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-16 18:20:26.904845 matgl-0.1.0.dev0/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       54 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5361 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)     4633 2023-02-16 17:25:58.000000 matgl-0.1.0.dev0/matgl/graph/converters.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-16 18:20:26.932402 matgl-0.1.0.dev0/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)       60 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     3736 2023-02-16 17:17:15.000000 matgl-0.1.0.dev0/matgl/layers/atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     2117 2023-02-16 17:17:15.000000 matgl-0.1.0.dev0/matgl/layers/bond_expansion.py
--rw-r--r--   0 shyue      (501) staff       (20)     6169 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/layers/core.py
--rw-r--r--   0 shyue      (501) staff       (20)      839 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/layers/cutoff_functions.py
--rw-r--r--   0 shyue      (501) staff       (20)     3048 2023-02-16 17:17:15.000000 matgl-0.1.0.dev0/matgl/layers/embedding_block.py
--rw-r--r--   0 shyue      (501) staff       (20)     9515 2023-02-16 17:30:02.000000 matgl-0.1.0.dev0/matgl/layers/graph_conv.py
--rw-r--r--   0 shyue      (501) staff       (20)     3891 2023-02-16 17:17:15.000000 matgl-0.1.0.dev0/matgl/layers/readout_block.py
--rw-r--r--   0 shyue      (501) staff       (20)     3611 2023-02-16 17:28:58.000000 matgl-0.1.0.dev0/matgl/layers/three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-16 18:20:26.963262 matgl-0.1.0.dev0/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)       89 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     6793 2023-02-16 17:17:15.000000 matgl-0.1.0.dev0/matgl/models/layers.py
--rw-r--r--   0 shyue      (501) staff       (20)     8899 2023-02-16 18:10:08.000000 matgl-0.1.0.dev0/matgl/models/m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     4749 2023-02-16 17:17:15.000000 matgl-0.1.0.dev0/matgl/models/megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     2483 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/models/potential.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-16 18:20:26.964856 matgl-0.1.0.dev0/matgl/nbody/
--rw-r--r--   0 shyue      (501) staff       (20)       52 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/nbody/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4166 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/nbody/three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-16 18:20:26.979053 matgl-0.1.0.dev0/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       63 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    16151 2023-02-16 17:17:15.000000 matgl-0.1.0.dev0/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-02-16 17:15:37.000000 matgl-0.1.0.dev0/matgl/utils/sb_roots.npy
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-16 18:20:26.901471 matgl-0.1.0.dev0/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)     3230 2023-02-16 18:20:26.000000 matgl-0.1.0.dev0/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      850 2023-02-16 18:20:26.000000 matgl-0.1.0.dev0/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-02-16 18:20:26.000000 matgl-0.1.0.dev0/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       10 2023-02-16 18:20:26.000000 matgl-0.1.0.dev0/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-02-16 18:20:26.000000 matgl-0.1.0.dev0/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)      718 2023-02-16 18:14:33.000000 matgl-0.1.0.dev0/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)      318 2023-02-16 18:20:26.979683 matgl-0.1.0.dev0/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     1684 2023-02-16 18:19:52.000000 matgl-0.1.0.dev0/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.734976 matgl-0.2.0/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.2.0/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)     6907 2023-04-27 02:35:27.735064 matgl-0.2.0/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     5756 2023-04-27 02:19:29.000000 matgl-0.2.0/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.726853 matgl-0.2.0/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      128 2023-04-27 02:34:19.000000 matgl-0.2.0/matgl/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1694 2023-04-27 02:11:40.000000 matgl-0.2.0/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.728318 matgl-0.2.0/matgl/dataloader/
+-rw-r--r--   0 shyue      (501) staff       (20)       53 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/dataloader/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11085 2023-04-22 15:03:50.000000 matgl-0.2.0/matgl/dataloader/dataset.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.729465 matgl-0.2.0/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5358 2023-04-27 02:12:23.000000 matgl-0.2.0/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6797 2023-03-24 14:22:00.000000 matgl-0.2.0/matgl/graph/converters.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.732149 matgl-0.2.0/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)       60 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2099 2023-04-22 15:03:50.000000 matgl-0.2.0/matgl/layers/activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3586 2023-04-27 02:11:52.000000 matgl-0.2.0/matgl/layers/atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2168 2023-04-26 23:53:15.000000 matgl-0.2.0/matgl/layers/bond_expansion.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-04-26 23:56:19.000000 matgl-0.2.0/matgl/layers/core.py
+-rw-r--r--   0 shyue      (501) staff       (20)      809 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/layers/cutoff_functions.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3144 2023-04-27 00:46:37.000000 matgl-0.2.0/matgl/layers/embedding_block.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16058 2023-04-26 23:57:55.000000 matgl-0.2.0/matgl/layers/graph_conv.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3972 2023-04-27 00:48:04.000000 matgl-0.2.0/matgl/layers/readout_block.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3726 2023-04-27 00:53:44.000000 matgl-0.2.0/matgl/layers/three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.733730 matgl-0.2.0/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      124 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12940 2023-03-24 14:41:18.000000 matgl-0.2.0/matgl/models/ase_interface.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12293 2023-04-27 00:53:44.000000 matgl-0.2.0/matgl/models/m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9328 2023-04-27 02:31:12.000000 matgl-0.2.0/matgl/models/megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3089 2023-03-24 14:22:00.000000 matgl-0.2.0/matgl/models/potential.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.734724 matgl-0.2.0/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    17703 2023-04-27 02:13:46.000000 matgl-0.2.0/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/utils/sb_roots.npy
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.727858 matgl-0.2.0/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)     6907 2023-04-27 02:35:27.000000 matgl-0.2.0/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      835 2023-04-27 02:35:27.000000 matgl-0.2.0/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-04-27 02:35:27.000000 matgl-0.2.0/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       10 2023-04-27 02:35:27.000000 matgl-0.2.0/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-04-27 02:35:27.000000 matgl-0.2.0/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     3121 2023-03-24 14:22:00.000000 matgl-0.2.0/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)      603 2023-04-27 02:35:27.735378 matgl-0.2.0/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     2075 2023-03-24 21:13:05.000000 matgl-0.2.0/setup.py
```

### Comparing `matgl-0.1.0.dev0/LICENSE` & `matgl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.1.0.dev0/matgl/config.py` & `matgl-0.2.0/matgl/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""Data types"""
+"""Global configuration variables for matgl."""
+from __future__ import annotations
+
 import numpy as np
 
 # import tensorflow as tf
 import torch
 
 DTYPES = {
     "float32": {"numpy": np.float32, "torch": torch.float32},
```

### Comparing `matgl-0.1.0.dev0/matgl/graph/compute.py` & `matgl-0.2.0/matgl/graph/compute.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import torch
 
 
-def compute_3body(g):
+def compute_3body(g: dgl.DGLGraph):
     """
     Calculate the three body indices from pair atom indices
 
     Args:
         g: DGL graph
 
     Returns:
@@ -21,90 +21,91 @@
         n_triple_ij (np.ndarray): number of three-body angles for each bond
         n_triple_i (np.ndarray): number of three-body angles each atom
         n_triple_s (np.ndarray): number of three-body angles for each structure
     """
     bond_atom_indices = g.edges()
     n_atoms = [g.num_nodes()]
     n_atoms_total = np.sum(g.num_nodes())
-    first_col = bond_atom_indices[0].numpy().reshape(-1, 1)
-    all_indices = np.arange(n_atoms_total).reshape(1, -1)
-    n_bond_per_atom = np.count_nonzero(first_col == all_indices, axis=0)
+    first_col = bond_atom_indices[0].reshape(-1, 1)
+    all_indices = torch.arange(n_atoms_total).reshape(1, -1)
+    n_bond_per_atom = torch.count_nonzero(first_col == all_indices, dim=0)
     n_triple_i = n_bond_per_atom * (n_bond_per_atom - 1)
-    n_triple = np.sum(n_triple_i)
-    n_triple_ij = np.repeat(n_bond_per_atom - 1, n_bond_per_atom)
-    triple_bond_indices = np.empty(shape=(n_triple, 2), dtype=np.int32)
+    n_triple = torch.sum(n_triple_i)
+    n_triple_ij = (n_bond_per_atom - 1).repeat_interleave(n_bond_per_atom)
+    triple_bond_indices = torch.empty((n_triple, 2), dtype=torch.int64)
 
     start = 0
     cs = 0
-    for i, n in enumerate(n_bond_per_atom):
+    for n in n_bond_per_atom:
         if n > 0:
             """
             triple_bond_indices is generated from all pair permutations of atom indices. The
             numpy version below does this with much greater efficiency. The equivalent slow
             code is:
 
             ```
             for j, k in itertools.permutations(range(n), 2):
                 triple_bond_indices[index] = [start + j, start + k]
             ```
             """
-            r = np.arange(n)
-            x, y = np.meshgrid(r, r)
-            c = np.stack([y.ravel(), x.ravel()], axis=1)
+            r = torch.arange(n)
+            x, y = torch.meshgrid(r, r)
+            c = torch.stack([y.ravel(), x.ravel()], dim=1)
             final = c[c[:, 0] != c[:, 1]]
             triple_bond_indices[start : start + (n * (n - 1)), :] = final + cs
             start += n * (n - 1)
             cs += n
 
     n_triple_s = []
     i = 0
     for n in n_atoms:
         j = i + n
-        n_triple_s.append(np.sum(n_triple_i[i:j]))
+        n_triple_s.append(torch.sum(n_triple_i[i:j]))
         i = j
 
-    src_id, dst_id = torch.tensor(triple_bond_indices[:, 0]), torch.tensor(triple_bond_indices[:, 1])
+    src_id, dst_id = (triple_bond_indices[:, 0], triple_bond_indices[:, 1])
     l_g = dgl.graph((src_id, dst_id))
     l_g.ndata["bond_dist"] = g.edata["bond_dist"]
     l_g.ndata["bond_vec"] = g.edata["bond_vec"]
     l_g.ndata["pbc_offset"] = g.edata["pbc_offset"]
-    l_g.ndata["n_triple_ij"] = torch.tensor(n_triple_ij)
-    return l_g, triple_bond_indices, n_triple_ij, n_triple_i, np.array(n_triple_s, dtype=np.int32)
+    l_g.ndata["n_triple_ij"] = n_triple_ij
+    n_triple_s = torch.tensor(n_triple_s, dtype=torch.int64)
+    return l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s
 
 
-def compute_pair_vector_and_distance(g):
+def compute_pair_vector_and_distance(g: dgl.DGLGraph):
     """
     Calculate bond vectors and distances using dgl graphs
 
     Args:
     g: DGL graph
 
     Returns:
     bond_vec (torch.tensor): bond distance between two atoms
     bond_dist (torch.tensor): vector from src node to dst node
     """
-    atom_pos = g.ndata["pos"]
     bond_vec = torch.zeros(g.num_edges(), 3)
     bond_dist = torch.zeros(g.num_edges())
     for i in range(g.num_edges()):
         bond_vec[i, :] = (
-            atom_pos[g.edges()[1][i], :]
+            g.ndata["pos"][g.edges()[1][i], :]
             + torch.sum(torch.squeeze(g.edata["pbc_offset"][i][:] * g.edata["lattice"][i][:, None]), dim=0)
-            - atom_pos[g.edges()[0][i], :]
+            - g.ndata["pos"][g.edges()[0][i], :]
         )
     bond_dist = torch.norm(bond_vec, dim=1)
+
     return bond_vec, bond_dist
 
 
-def compute_theta_and_phi(edges):
+def compute_theta_and_phi(edges: dgl.udf.EdgeBatch):
     """
     Calculate bond angle Theta and Phi using dgl graphs
 
     Args:
-    g: DGL graph
+    edges: DGL graph edges
 
     Returns:
     cos_theta: torch.tensor
     phi: torch.tensor
     triple_bond_lengths (torch.tensor):
     """
     vec1 = edges.src["bond_vec"]
@@ -113,15 +114,15 @@
     return {
         "cos_theta": cosine_theta,
         "phi": torch.zeros_like(cosine_theta),
         "triple_bond_lengths": edges.dst["bond_dist"],
     }
 
 
-def create_line_graph(g_batched, threebody_cutoff: float | None = None):
+def create_line_graph(g_batched: dgl.DGLGraph, threebody_cutoff: float):
     """
     Calculate the three body indices from pair atom indices
 
     Args:
         g_batched: Batched DGL graph
         threebody_cutoff (float): cutoff for three-body interactions
 
@@ -137,15 +138,13 @@
             valid_three_body = g.edata["bond_dist"] <= threebody_cutoff
             src_id_with_three_body = bond_atom_indices[0][valid_three_body]
             dst_id_with_three_body = bond_atom_indices[1][valid_three_body]
             graph_with_three_body = dgl.graph((src_id_with_three_body, dst_id_with_three_body))
             graph_with_three_body.edata["bond_dist"] = g.edata["bond_dist"][valid_three_body]
             graph_with_three_body.edata["bond_vec"] = g.edata["bond_vec"][valid_three_body]
             graph_with_three_body.edata["pbc_offset"] = g.edata["pbc_offset"][valid_three_body]
-        else:
-            np.arange(n_bond)
         if graph_with_three_body.edata["bond_dist"].size(dim=0) > 0:
             l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s = compute_3body(graph_with_three_body)
             l_g_unbatched.append(l_g)
 
     l_g_batched = dgl.batch(l_g_unbatched)
     return l_g_batched
```

### Comparing `matgl-0.1.0.dev0/matgl/graph/converters.py` & `matgl-0.2.0/matgl/graph/converters.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import scipy.sparse as sp
 import torch
+from ase import Atoms
 from dgl.backend import tensor
 from pymatgen.core import Element, Molecule, Structure
 from pymatgen.optimization.neighbors import find_points_in_spheres
 
 
 def get_element_list(train_structures: list[Structure | Molecule]) -> tuple[str]:
     """Get the dictionary containing elements in the training set for atomic features
@@ -25,15 +26,15 @@
     for s in train_structures:
         elements.update(s.composition.get_el_amt_dict().keys())
     return tuple(sorted(elements, key=lambda el: Element(el).Z))  # type: ignore
 
 
 class Pmg2Graph:
     """
-    Construct a DGL graph from Pymatgen Molecules or Structures.
+    Construct a DGL graph from Pymatgen Molecules or Structures, ASE atoms is also added.
     """
 
     def __init__(
         self,
         element_types: tuple[str],
         cutoff: float = 5.0,
     ):
@@ -53,52 +54,49 @@
 
         :param mol: pymatgen molecule object
         :return: (dgl graph, state features)
         """
         natoms = len(mol)
         R = mol.cart_coords
         element_types = self.element_types
-        Z = [np.eye(len(element_types))[element_types.index(site.specie.symbol)] for site in mol]
-        Z = np.array(Z)
-        atomic_number = [site.specie.Z for site in mol]
-        atomic_number = np.array(atomic_number)
+        Z = np.array([np.eye(len(element_types))[element_types.index(site.specie.symbol)] for site in mol])
+        np.array([site.specie.Z for site in mol])
         weight = mol.composition.weight / len(mol)
         dist = np.linalg.norm(R[:, None, :] - R[None, :, :], axis=-1)
         dists = mol.distance_matrix.flatten()
         nbonds = (np.count_nonzero(dists <= self.cutoff) - natoms) / 2
         nbonds /= natoms
         adj = sp.csr_matrix(dist <= self.cutoff) - sp.eye(natoms, dtype=np.bool_)
         adj = adj.tocoo()
         u, v = tensor(adj.row), tensor(adj.col)
         g = dgl.graph((u, v))
         g = dgl.to_bidirected(g)
         g.ndata["pos"] = tensor(R)
         g.ndata["attr"] = tensor(Z)
-        g.ndata["Z"] = tensor(atomic_number)
+        g.ndata["node_type"] = tensor(np.hstack([[element_types.index(site.specie.symbol)] for site in mol]))
         g.edata["pbc_offset"] = torch.zeros(g.num_edges(), 3)
         g.edata["lattice"] = torch.zeros(g.num_edges(), 3, 3)
         state_attr = [weight, nbonds]
+        g.edata["pbc_offshift"] = torch.zeros(g.num_edges(), 3)
 
         return g, state_attr
 
     def get_graph_from_structure(self, structure: Structure) -> tuple[dgl.DGLGraph, list]:
         """
         Get a DGL graph from an input Structure.
 
         :param structure: pymatgen structure object
         :return:
             g: DGL graph
             state_attr: state features
         """
-
         numerical_tol = 1.0e-8
         pbc = np.array([1, 1, 1], dtype=int)
         element_types = self.element_types
-        Z = [np.eye(len(element_types))[element_types.index(site.specie.symbol)] for site in structure]
-        Z = np.array(Z)
+        Z = np.array([np.eye(len(element_types))[element_types.index(site.specie.symbol)] for site in structure])
         atomic_number = np.array([site.specie.Z for site in structure])
         lattice_matrix = np.ascontiguousarray(np.array(structure.lattice.matrix), dtype=float)
         volume = structure.volume
         cart_coords = np.ascontiguousarray(np.array(structure.cart_coords), dtype=float)
         src_id, dst_id, images, bond_dist = find_points_in_spheres(
             cart_coords,
             cart_coords,
@@ -115,13 +113,58 @@
             bond_dist[exclude_self],
         )
         u, v = tensor(src_id), tensor(dst_id)
         g = dgl.graph((u, v))
         g.edata["pbc_offset"] = torch.tensor(images)
         g.edata["lattice"] = tensor([[lattice_matrix] for i in range(g.num_edges())])
         g.ndata["attr"] = tensor(Z)
-        g.ndata["Z"] = tensor(atomic_number)
+        g.ndata["node_type"] = tensor(np.hstack([[element_types.index(site.specie.symbol)] for site in structure]))
         g.ndata["pos"] = tensor(cart_coords)
         g.ndata["volume"] = tensor([volume for i in range(atomic_number.shape[0])])
         state_attr = [0.0, 0.0]
+        g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
+        return g, state_attr
+
+    def get_graph_from_atoms(self, atoms: Atoms) -> tuple[dgl.DGLGraph, list]:
+        """
+        Get a DGL graph from an input Structure.
 
+        :param structure: pymatgen structure object
+        :return:
+            g: DGL graph
+            state_attr: state features
+        """
+
+        numerical_tol = 1.0e-8
+        pbc = np.array([1, 1, 1], dtype=int)
+        element_types = self.element_types
+        Z = np.array([np.eye(len(element_types))[element_types.index(i.symbol)] for i in atoms])
+        atomic_number = np.array(atoms.get_atomic_numbers())
+        lattice_matrix = np.ascontiguousarray(np.array(atoms.get_cell()), dtype=float)
+        volume = atoms.get_volume()
+        cart_coords = np.ascontiguousarray(np.array(atoms.get_positions()), dtype=float)
+        src_id, dst_id, images, bond_dist = find_points_in_spheres(
+            cart_coords,
+            cart_coords,
+            r=self.cutoff,
+            pbc=pbc,
+            lattice=lattice_matrix,
+            tol=numerical_tol,
+        )
+        exclude_self = (src_id != dst_id) | (bond_dist > numerical_tol)
+        src_id, dst_id, images, bond_dist = (
+            src_id[exclude_self],
+            dst_id[exclude_self],
+            images[exclude_self],
+            bond_dist[exclude_self],
+        )
+        u, v = tensor(src_id), tensor(dst_id)
+        g = dgl.graph((u, v))
+        g.edata["pbc_offset"] = torch.tensor(images)
+        g.edata["lattice"] = tensor([[lattice_matrix] for i in range(g.num_edges())])
+        g.ndata["attr"] = tensor(Z)
+        g.ndata["node_type"] = tensor(np.hstack([[element_types.index(i.symbol)] for i in atoms]))
+        g.ndata["pos"] = tensor(cart_coords)
+        g.ndata["volume"] = tensor([volume for i in range(atomic_number.shape[0])])
+        state_attr = [0.0, 0.0]
+        g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
         return g, state_attr
```

### Comparing `matgl-0.1.0.dev0/matgl/layers/atom_ref.py` & `matgl-0.2.0/matgl/layers/atom_ref.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,94 @@
 """
 atomic energy offset. Used for predicting extensive properties.
 """
+from __future__ import annotations
+
+import dgl
 import numpy as np
 import torch
 import torch.nn as nn
 from pymatgen.core import Molecule, Structure
-from torch_scatter import scatter
-from typing import List
-import dgl
-
-from matgl.utils.maths import get_segment_indices_from_n
 
 
 class AtomRef(nn.Module):
     """
     Get total property offset for a system:
     """
 
     def __init__(
         self,
-        property_offset: np.array,  # type: ignore # noqa: F821
+        property_offset: np.array,  # type: ignore
     ) -> None:
         """
         Parameters:
         -----------
         property_offset (np.array): a array of elemental property offset
         """
         super().__init__()
         self.property_offset = torch.tensor(property_offset)
         self.max_z = self.property_offset.size(dim=0)
 
-    def get_feature_matrix(self, structs_or_graphs: List, element_list: tuple[str]) -> np.array:
+    def get_feature_matrix(self, structs_or_graphs: list, element_list: tuple[str]) -> np.typing.NDArray:
         """
         Get the number of atoms for different elements in the structure
 
         Args:
         structs_or_graphs (list): a list of pymatgen Structure or dgl graph
         element_list: a dictionary containing element types in the training set
 
         Returns:
         features (np.array): a matrix (num_structures, num_elements)
         """
         n = len(structs_or_graphs)
         features = np.zeros(shape=(n, self.max_z))
         for i, s in enumerate(structs_or_graphs):
-
             if isinstance(s, (Structure, Molecule)):
                 atomic_numbers = [element_list.index(site.specie.symbol) for site in s.sites]
             else:
                 one_hot_vecs = s.ndata["attr"]
                 atomic_numbers = ((one_hot_vecs == 1).nonzero(as_tuple=True)[0]).tolist()
             features[i] = np.bincount(atomic_numbers, minlength=self.max_z)
         return features
 
-    def fit(self, structs_or_graphs: List, element_list: tuple[str], properties: np.array) -> bool:
+    def fit(self, structs_or_graphs: list, element_list: tuple[str], properties: np.typing.NDArray) -> bool:
         """
         Fit the elemental reference values for the properties
 
         Args:
         structs_or_graphs: pymatgen Structures or dgl graphs
         properties (np.ndarray): array of extensive properties
 
         Returns:
         """
         features = self.get_feature_matrix(structs_or_graphs, element_list)
         self.property_offset = np.linalg.pinv(features.T.dot(features)).dot(features.T.dot(properties))
         self.property_offset = torch.tensor(self.property_offset)
         return True
 
-    def forward(self, g: dgl.DGLGraph, state_attr: torch.tensor = None) -> torch.tensor:
+    def forward(self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None):
         """
         Get the total property offset for a system
 
         Args:
         g: a batch of dgl graphs
-        state_attr: state label
+        state_attr: state attributes
 
         Returns:
         offset_per_graph:
         """
         if self.property_offset.ndim > 1:
             offset_batched_with_state = []
             for i in range(0, self.property_offset.size(dim=0)):
                 property_offset_batched = self.property_offset[i].repeat(g.num_nodes(), 1)
                 offset = property_offset_batched * g.ndata["attr"]
-                offset = torch.sum(offset, 1)
-                index = get_segment_indices_from_n(g.batch_num_nodes())
-                offset_batched = scatter(offset, index, reduce="sum")
+                g.ndata["atomic_offset"] = torch.sum(offset, 1)
+                offset_batched = dgl.readout_nodes(g, "atomic_offset")
                 offset_batched_with_state.append(offset_batched)
-            offset_batched_with_state = torch.stack(offset_batched_with_state)
-            return offset_batched_with_state[state_attr]
+            offset_batched_with_state = torch.stack(offset_batched_with_state)  # type: ignore
+            return offset_batched_with_state[state_attr]  # type: ignore
         else:
             property_offset_batched = self.property_offset.repeat(g.num_nodes(), 1)
             offset = property_offset_batched * g.ndata["attr"]
-            offset = torch.sum(offset, 1)
-            index = get_segment_indices_from_n(g.batch_num_nodes())
-            offset_batched = scatter(offset, index, reduce="sum")
+            g.ndata["atomic_offset"] = torch.sum(offset, 1)
+            offset_batched = dgl.readout_nodes(g, "atomic_offset")
             return offset_batched
```

### Comparing `matgl-0.1.0.dev0/matgl/layers/bond_expansion.py` & `matgl-0.2.0/matgl/layers/bond_expansion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Generate bond features based on spherical bessel functions or gaussian expansion
 """
+from __future__ import annotations
+
 import torch
 import torch.nn as nn
 
 from matgl.utils.maths import GaussianExpansion, SphericalBesselFunction
 
 
 class BondExpansion(nn.Module):
@@ -12,15 +14,15 @@
     Expand pair distances into a set of spherical bessel or gaussian functions.
     """
 
     def __init__(
         self,
         max_l: int = 3,
         max_n: int = 3,
-        cutoff: float = 4.0,
+        cutoff: float = 5.0,
         rbf_type: str = "SphericalBessel",
         smooth: bool = False,
         initial: float = 0.0,
         final: float = 5.0,
         num_centers: int = 100,
         width: float = 0.5,
     ) -> None:
@@ -32,35 +34,34 @@
         cutoff (float): cutoff radius
         rbf_type (str): type of radial basis function .i.e. either "SphericalBessel" or 'Gaussian'
         smooth (bool): whether apply the smooth version of spherical bessel functions or not
         initial (float): initial point for gaussian expansion
         final (float): final point for gaussian expansion
         width (float): width of gaussian function
         """
-
         super().__init__()
 
         self.max_n = max_n
         self.cutoff = cutoff
         self.max_l = max_l
         self.smooth = smooth
         self.num_centers = num_centers
         self.width = width
         self.initial = initial
         self.final = final
         self.rbf_type = rbf_type
 
         if rbf_type == "SphericalBessel":
-            self.rbf = SphericalBesselFunction(max_l, max_n, cutoff, smooth)
+            self.rbf = SphericalBesselFunction(max_l, max_n, cutoff, smooth)  # type: ignore
         elif rbf_type == "Gaussian":
-            self.rbf = GaussianExpansion(initial, final, num_centers, width)
+            self.rbf = GaussianExpansion(initial, final, num_centers, width)  # type: ignore
         else:
             raise Exception("undefined rbf_type, please use SphericalBessel or Gaussian instead.")
 
-    def forward(self, bond_dist: torch.tensor) -> torch.tensor:
+    def forward(self, bond_dist: torch.tensor):
         """
         Forward
 
         Args:
         bond_dist: Bond distance
 
         Return:
```

### Comparing `matgl-0.1.0.dev0/matgl/layers/core.py` & `matgl-0.2.0/matgl/layers/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from __future__ import annotations
 
 from typing import Callable
 
 import torch
 import torch.nn as nn
-from dgl import broadcast_edges, softmax_edges, sum_edges
+from dgl import DGLGraph, broadcast_edges, softmax_edges, sum_edges
 from torch.nn import LSTM, Linear, Module, ModuleList
 
 
 class MLP(nn.Module):
     """
     An implementation of a multi-layer perceptron.
     """
@@ -34,40 +34,41 @@
         self.layers = ModuleList()
 
         for i, (in_dim, out_dim) in enumerate(zip(dims[:-1], dims[1:])):
             if i < self._depth - 1:
                 self.layers.append(Linear(in_dim, out_dim, bias=True))
 
                 if activation is not None:
-                    self.layers.append(activation)
+                    self.layers.append(activation)  # type: ignore
             else:
                 self.layers.append(Linear(in_dim, out_dim, bias=bias_last))
 
                 if activation is not None and activate_last:
-                    self.layers.append(activation)
+                    self.layers.append(activation)  # type: ignore
 
     def __repr__(self):
         dims = []
 
         for layer in self.layers:
             if isinstance(layer, Linear):
                 dims.append(f"{layer.in_features} \u2192 {layer.out_features}")
             else:
                 dims.append(layer.__class__.__name__)
 
         return f'MLP({", ".join(dims)})'
 
     @property
-    def last_linear(self) -> Linear:
+    def last_linear(self) -> Linear | None:
         """
         :return: The last linear layer.
         """
         for layer in reversed(self.layers):
             if isinstance(layer, Linear):
                 return layer
+        return None
 
     @property
     def depth(self) -> int:
         """Returns depth of MLP."""
         return self._depth
 
     @property
@@ -79,50 +80,43 @@
     def out_features(self) -> int:
         """Returns output features of MLP."""
         for layer in reversed(self.layers):
             if isinstance(layer, Linear):
                 return layer.out_features
         raise RuntimeError
 
-    def forward(self, inputs: torch.Tensor) -> torch.Tensor:
+    def forward(self, inputs):
         """
         Applies all layers in turn.
 
         :param inputs: Input tensor
         :return: Output tensor
         """
         x = inputs
-
         for layer in self.layers:
             x = layer(x)
 
         return x
 
 
 class GatedMLP(nn.Module):
     """
     An implementation of a Gated multi-layer perceptron.
     """
 
-    def __init__(
-        self,
-        in_feats: int,
-        dims: list[int],
-        activate_last: bool = True,
-        use_bias: bool = True,
-    ):
+    def __init__(self, in_feats: int, dims: list[int], activate_last: bool = True, use_bias: bool = True):
         """
         :param in_feats: Dimension of input features.
         :param dims: Architecture of neural networks.
         :param activate_last: Whether applying activation to last layer or not.
         :param bias_last: Whether applying bias to last layer or not.
         """
         super().__init__()
         self.in_feats = in_feats
-        self.dims = [in_feats] + dims
+        self.dims = [in_feats, *dims]
         self._depth = len(dims)
         self.layers = nn.Sequential()
         self.gates = nn.Sequential()
         self.use_bias = use_bias
         self.activate_last = activate_last
         for i, (in_dim, out_dim) in enumerate(zip(self.dims[:-1], self.dims[1:])):
             if i < self._depth - 1:
@@ -133,15 +127,15 @@
             else:
                 self.layers.append(nn.Linear(in_dim, out_dim, bias=use_bias))
                 if self.activate_last:
                     self.layers.append(nn.SiLU())
                 self.gates.append(nn.Linear(in_dim, out_dim, bias=use_bias))
                 self.gates.append(nn.Sigmoid())
 
-    def forward(self, inputs: torch.tensor) -> torch.tensor:
+    def forward(self, inputs: torch.tensor):
         return self.layers(inputs) * self.gates(inputs)
 
 
 class EdgeSet2Set(Module):
     """
     Implementation of Set2Set.
     """
@@ -160,15 +154,15 @@
         self.lstm = LSTM(self.output_dim, self.input_dim, n_layers)
         self.reset_parameters()
 
     def reset_parameters(self):
         """Reinitialize learnable parameters."""
         self.lstm.reset_parameters()
 
-    def forward(self, g: dgl.DGLGraph, feat: torch.tensor) -> torch.tensor:
+    def forward(self, g: DGLGraph, feat: torch.tensor):
         """
         Defines the computation performed at every call.
 
         :param g: Input graph
         :param feat: Input features.
         :return: One hot vector
         """
```

### Comparing `matgl-0.1.0.dev0/matgl/layers/cutoff_functions.py` & `matgl-0.2.0/matgl/layers/cutoff_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from __future__ import annotations
 
 from math import pi
 
 import torch
 
 
-def polynomial_cutoff(r: torch.tensor, cutoff: float) -> torch.tensor:
+def polynomial_cutoff(r, cutoff: float):
     """
     Polynomial cutoff function
     Args:
         r (torch.tensor): radius distance tensor
         cutoff (float): cutoff distance
 
     Returns: polynomial cutoff functions
 
     """
     ratio = r / cutoff
     return torch.where(r <= cutoff, 1 - 6 * ratio**5 + 15 * ratio**4 - 10 * ratio**3, 0.0)
 
 
-def cosine_cutoff(r: torch.tensor, cutoff: float) -> torch.tensor:
+def cosine_cutoff(r: torch.Tensor, cutoff: float) -> torch.Tensor:
     """
     Cosine cutoff function
     Args:
         r (torch.tensor): radius distance tensor
         cutoff (float): cutoff distance
 
     Returns: cosine cutoff functions
```

### Comparing `matgl-0.1.0.dev0/matgl/layers/embedding_block.py` & `matgl-0.2.0/matgl/layers/embedding_block.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,72 +12,74 @@
 class EmbeddingBlock(nn.Module):
     """
     Embedding block for generating node, bond and state features
     """
 
     def __init__(
         self,
+        degree_rbf: int,
+        activation: nn.Module,
         num_node_feats: int,
         num_edge_feats: int,
+        num_node_types: int | None = None,
         num_state_feats: int | None = None,
         include_states: bool = False,
         num_state_types: int | None = None,
         state_embedding_dim: int | None = None,
-        activation: str = "swish",
     ):
         """
         Parameters:
         -----------
         num_node_feats (int): dimensionality of node features
         num_edge_feats (int): dimensionality of edge features
         num_state_feats (int): dimensionality of state features
         include_states (bool): whether including state for M3GNet or not
         state_embedding_dim (int): dimensionality of state embedding
         activation (str): activation function type
         """
         super().__init__()
-
-        if activation == "swish":
-            self.activation = nn.SiLU()
-        elif activation == "sigmoid":
-            self.activation = nn.Sigmoid()
-        elif activation == "tanh":
-            self.activation = nn.Tanh()
         self.include_states = include_states
         self.num_state_types = num_state_types
         self.num_node_feats = num_node_feats
         self.num_edge_feats = num_edge_feats
         self.num_state_feats = num_state_feats
+        self.num_node_types = num_node_types
         self.state_embedding_dim = state_embedding_dim
-
+        self.activation = activation
         if num_state_types and state_embedding_dim is not None:
-            self.state_embedding = nn.Embedding(num_state_types, state_embedding_dim)
+            self.state_embedding = nn.Embedding(num_state_types, state_embedding_dim)  # type: ignore
+        if num_node_types is not None:
+            self.node_embedding = nn.Embedding(num_node_types, num_node_feats)
+        self.edge_embedding = MLP([degree_rbf, self.num_edge_feats], activation=activation, activate_last=True)
 
-    def forward(self, node_attr: torch.tensor, edge_attr: torch.tensor, state_attr: torch.tensor):
+    def forward(self, node_attr, edge_attr, state_attr):
         """
         Output embedded features
 
         Args:
         node_attr: node attribute
         edge_attr: edge attribute
         state_attr: state attribute
 
         Returns:
         node_feat: embedded node features
         edge_feat: embedded edge features
         state_feat: embedded state features
         """
-        node_embed = MLP([node_attr.shape[-1], self.num_node_feats], activation=self.activation)
-        edge_embed = MLP([edge_attr.shape[-1], self.num_edge_feats], activation=self.activation)
-        node_feat = node_embed(node_attr.to(torch.float32))
-        edge_feat = edge_embed(edge_attr.to(torch.float32))
+
+        if self.num_node_types is not None:
+            node_feat = self.node_embedding(node_attr)
+        else:
+            node_embed = MLP([node_attr.shape[-1], self.num_node_feats], activation=self.activation)
+            node_feat = node_embed(node_attr.to(torch.float32))
+
+        edge_feat = self.edge_embedding(edge_attr.to(torch.float32))
         if self.include_states is True:
             if self.num_state_types and self.state_embedding_dim is not None:
                 state_feat = self.state_embedding(state_attr)
-                state_feat = self.activation(state_feat)
             else:
                 state_attr = torch.unsqueeze(state_attr, 0)
                 state_embed = MLP([state_attr.shape[-1], self.num_state_feats], activation=self.activation)
                 state_feat = state_embed(state_attr.to(torch.float32))
         else:
             state_feat = None
         return node_feat, edge_feat, state_feat
```

### Comparing `matgl-0.1.0.dev0/matgl/layers/readout_block.py` & `matgl-0.2.0/matgl/layers/readout_block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Readout layer for M3GNet
 """
 
+from __future__ import annotations
+
 import dgl
 import torch
 import torch.nn as nn
 from dgl.nn import Set2Set
 
 from matgl.layers.core import EdgeSet2Set, GatedMLP
 
@@ -22,22 +24,21 @@
         field: str,
     ):
         """
         Paramaters:
             num_steps (int): number of LSTM steps
             field (str): the field of MaterialGraph to perform the readout
         """
-
         super().__init__()
         self.field = field
         self.num_steps = num_steps
         self.num_layers = num_layers
 
-    def forward(self, g):
-        s2s_kwargs = dict(n_iters=self.num_steps, n_layers=self.num_layers)
+    def forward(self, g: dgl.DGLGraph):
+        s2s_kwargs = {"n_iters": self.num_steps, "n_layers": self.num_layers}
         if self.field == "node_feat":
             in_feats = g.ndata["node_feat"].size(dim=1)
             set2set = Set2Set(in_feats, **s2s_kwargs)
             out_tensor = set2set(g, g.ndata["node_feat"])
         elif self.field == "edge_feat":
             in_feats = g.edata["edge_feat"].size(dim=1)
             set2set = EdgeSet2Set(in_feats, **s2s_kwargs)
@@ -47,25 +48,25 @@
 
 class ReduceReadOut(nn.Module):
     """
     Reduce atom or bond attributes into lower dimensional tensors as readout.
     This could be summing up the atoms or bonds, or taking the mean, etc.
     """
 
-    def __init__(self, op="mean", field="node_feat"):
+    def __init__(self, op: str = "mean", field: str = "node_feat"):
         super().__init__()
         """
         Parameters:
             op (str): op for the reduction
             field (str): the field of MaterialGraph to perform the reduction
         """
         self.op = op
         self.field = field
 
-    def forward(self, g):
+    def forward(self, g: dgl.DGLGraph):
         """
         Args:
             g: DGL graph
         Returns:
             torch.tensor
         """
         if self.field == "node_feat":
@@ -76,31 +77,27 @@
 
 
 class WeightedReadOut(nn.Module):
     """
     Feed node features into Gated MLP as readout.
     """
 
-    def __init__(self, in_feats, dims, num_targets):
+    def __init__(self, in_feats: int, dims: list[int], num_targets: int):
         """
         Parameters:
            in_feats: input features (nodes)
            dims: NN architecture for Gated MLP
            num_targets: number of target properties
         """
         super().__init__()
         self.in_feats = in_feats
-        self.dims = [in_feats] + dims + [num_targets]
-        self.gated = GatedMLP(
-            in_feats=in_feats,
-            dims=self.dims,
-            activate_last=False,
-        )
+        self.dims = [in_feats, *dims] + [num_targets]
+        self.gated = GatedMLP(in_feats=in_feats, dims=self.dims, activate_last=False)
 
-    def forward(self, g):
+    def forward(self, g: dgl.DGLGraph):
         """
         Args:
             g: DGL graph
         Returns:
             atomic_prperties: torch.tensor
         """
         atomic_properties = self.gated(g.ndata["node_feat"])
@@ -113,18 +110,18 @@
     """
 
     def __init__(self, in_feats, dims, num_targets, activation=None):
         super().__init__()
         self.in_feats = in_feats
         self.activation = activation
         self.num_targets = num_targets
-        self.dims = dims + [num_targets]
+        self.dims = [*dims, num_targets]
         self.gated = GatedMLP(in_feats=in_feats, dims=self.dims, activate_last=False)
 
-    def forward(self, g):
+    def forward(self, g: dgl.DGLGraph):
         num_nodes = g.ndata["node_feat"].size(dim=0)
         pair_properties = torch.zeros(num_nodes, num_nodes, self.num_targets)
         for i in range(num_nodes):
             for j in range(i, num_nodes):
                 in_features = (g.ndata["node_feat"][i][:] + g.ndata["node_feat"][j][:]) / 2.0
                 pair_properties[i][j][:] = self.gated(in_features)[:]
                 pair_properties[j][i][:] = pair_properties[i][j][:]
```

### Comparing `matgl-0.1.0.dev0/matgl/layers/three_body.py` & `matgl-0.2.0/matgl/layers/three_body.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
 Three-Body interaction implementations.
 """
 
-from typing import List
+from __future__ import annotations
 
+import dgl
 import torch
 import torch.nn as nn
-from torch_scatter import scatter
 
 from matgl.utils.maths import (
     SphericalBesselFunction,
     SphericalHarmonicsFunction,
     combine_sbf_shf,
     get_segment_indices_from_n,
+    scatter_sum,
 )
 
 
 class SphericalBesselWithHarmonics(nn.Module):
     """
     Expansion of basis using Spherical Bessel and Harmonics
     """
 
-    def __init__(self, max_n, max_l, cutoff, use_smooth, use_phi):
+    def __init__(self, max_n: int, max_l: int, cutoff: float, use_smooth: bool, use_phi: bool):
         """
         :param max_n: Degree of radial basis functions
         :param max_l: Degree of angular basis functions
         :param cutoff: Cutoff sphere
         :param use_smooth: Whether using smooth version of SBFs or not
         :param use_phi: using phi as angular basis functions
         """
@@ -66,16 +67,23 @@
             **kwargs:
         """
         super().__init__(**kwargs)
         self.update_network_atom = update_network_atom
         self.update_network_bond = update_network_bond
 
     def forward(
-        self, graph, line_graph, three_basis: torch.tensor, three_cutoff: float, node_feat, edge_feat, **kwargs
-    ) -> torch.tensor:
+        self,
+        graph: dgl.DGLGraph,
+        line_graph: dgl.DGLGraph,
+        three_basis: torch.tensor,
+        three_cutoff: float,
+        node_feat: torch.tensor,
+        edge_feat: torch.tensor,
+        **kwargs,
+    ):
         """
         Args:
             graph: dgl graph
             three_basis: three body basis expansion
             three_cutoff: cutoff radius
             node_feat: node features
             edge_feat: edge features
@@ -83,21 +91,21 @@
         Returns:
         """
         end_atom_index = torch.gather(graph.edges()[1], 0, line_graph.edges()[1].to(torch.int64))
         atoms = self.update_network_atom(node_feat)
         end_atom_index = torch.unsqueeze(end_atom_index, 1)
         atoms = torch.squeeze(atoms[end_atom_index])
         basis = three_basis * atoms
-        torch.tensor(graph.num_edges())
-        # three_cutoff = torch.unsqueeze(three_cutoff, dim=1)
-        # weights = torch.reshape(three_cutoff[torch.stack(list(line_graph.edges()), dim=1).to(torch.int64)], (-1, 2))
-        # weights = torch.prod(weights, axis=-1)
-        # weights = basis * weights[:, None]
-        new_bonds = scatter(
+        three_cutoff = torch.unsqueeze(three_cutoff, dim=1)
+        weights = torch.reshape(
+            three_cutoff[torch.stack(list(line_graph.edges()), dim=1).to(torch.int64)], (-1, 2)  # type: ignore
+        )
+        weights = torch.prod(weights, axis=-1)
+        weights = basis * weights[:, None]
+        new_bonds = scatter_sum(
             basis.to(torch.float32),
-            get_segment_indices_from_n(line_graph.ndata["n_triple_ij"]),
+            segment_ids=get_segment_indices_from_n(line_graph.ndata["n_triple_ij"]),
+            num_segments=graph.num_edges(),
             dim=0,
-            reduce="sum",
-            dim_size=graph.num_edges(),
         )
         edge_feat_updated = edge_feat + self.update_network_bond(new_bonds)
         return edge_feat_updated
```

### Comparing `matgl-0.1.0.dev0/matgl/models/potential.py` & `matgl-0.2.0/matgl/models/potential.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,60 +28,69 @@
         :param calc_hessian: Enable hessian calculations
         """
         super().__init__()
         self.model = model
         self.calc_forces = calc_forces
         self.calc_stresses = calc_stresses
         self.calc_hessian = calc_hessian
+        self.graph_converter = model.graph_converter
 
     def forward(
-        self, g: dgl.DGLGraph, graph_attr: torch.tensor
-    ) -> tuple[torch.tensor, torch.tensor, torch.tensor, torch.tensor]:
+        self, g: dgl.DGLGraph, graph_attr: torch.tensor | None = None, l_g: dgl.DGLGraph | None = None
+    ) -> tuple:
         """
         Args:
         g: DGL graph
         graph_attr: State attrs
 
         Returns:
         energies, forces, stresses, hessian: torch.tensor
         """
         forces = torch.zeros(1)
         stresses = torch.zeros(1)
         hessian = torch.zeros(1)
         if self.calc_forces:
             g.ndata["pos"].requires_grad_(True)
-
-        total_energies = self.model(g, graph_attr)
-
+        total_energies = self.model(g=g, state_attr=graph_attr, l_g=l_g)
         if self.calc_forces:
-
             grads = grad(
                 total_energies,
-                g.ndata["pos"],
+                [g.ndata["pos"], g.edata["bond_vec"]],
                 grad_outputs=torch.ones_like(total_energies),
                 create_graph=True,
                 retain_graph=True,
-            )[0]
-
-            forces = -grads
+            )
 
+            forces = -grads[0]
             if self.calc_hessian:
-                r = -grads.view(-1)
+                r = -grads[0].view(-1)
                 s = r.size(0)
                 hessian = total_energies.new_zeros((s, s))
                 for iatom in range(s):
-                    tmp = grad([r[iatom]], g.ndata["pos"], retain_graph=(iatom < s))[0]
+                    tmp = grad([r[iatom]], g.ndata["pos"], retain_graph=iatom < s)[0]
                     if tmp is not None:
                         hessian[iatom] = tmp.view(-1)
         if self.calc_stresses:
-
-            grads = grad(
-                total_energies,
-                g.edata["bond_vec"],
-                grad_outputs=torch.ones_like(total_energies),
-                create_graph=True,
-                retain_graph=True,
-            )
-            f_ij = -grads[0]
-            stresses = -1 * (160.21766208 * torch.matmul(g.edata["bond_vec"].T, f_ij) / g.ndata["volume"][0])
+            f_ij = -grads[1]
+            stresses = []
+            count_edge = 0
+            count_node = 0
+            for graph_id in range(g.batch_size):
+                num_edges = g.batch_num_edges()[graph_id]
+                num_nodes = 0
+                stresses.append(
+                    -1
+                    * (
+                        160.21766208
+                        * torch.matmul(
+                            g.edata["bond_vec"][count_edge : count_edge + num_edges].T,
+                            f_ij[count_edge : count_edge + num_edges],
+                        )
+                        / g.ndata["volume"][count_node + num_nodes]
+                    )
+                )
+                count_edge = count_edge + num_edges
+                num_nodes = g.batch_num_nodes()[graph_id]
+                count_node = count_node + num_nodes
+            stresses = torch.cat(stresses)
 
         return total_energies, forces, stresses, hessian
```

### Comparing `matgl-0.1.0.dev0/matgl/utils/maths.py` & `matgl-0.2.0/matgl/utils/maths.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 
 import numpy as np
 import sympy
 import torch
 import torch.nn as nn
 from scipy.optimize import brentq
 from scipy.special import spherical_jn
-from torch_scatter import scatter
 
 from matgl.config import DataType
 
 CWD = os.path.dirname(os.path.abspath(__file__))
 
 """
-Precomputed Spherical Bessel function roots in a 2D array with dimension [128, 128]. The n-th (0-based index） root of
+Precomputed Spherical Bessel function roots in a 2D array with dimension [128, 128]. The n-th (0-based index) root of
 order l Spherical Bessel function is the `[l, n]` entry.
 """
 SPHERICAL_BESSEL_ROOTS = np.load(os.path.join(CWD, "sb_roots.npy"))
 
 
 class GaussianExpansion(nn.Module):
     r"""
@@ -51,34 +50,33 @@
         number : int
                 Number of Gaussian Basis functions
         width : float
                 Width of Gaussian Basis functions
         """
         super().__init__()
         self.centers = np.linspace(initial, final, num_centers)
-        self.centers = nn.Parameter(torch.tensor(self.centers).float(), requires_grad=False)
+        self.centers = nn.Parameter(torch.tensor(self.centers).float(), requires_grad=False)  # type: ignore
         if width is None:
             self.width = float(1.0 / np.diff(self.centers).mean())
         else:
             self.width = width
 
     def reset_parameters(self):
         """Reinitialize model parameters."""
-        device = self.centers.device
-        self.centers = nn.Parameter(self.centers.clone().detach().float(), requires_grad=False).to(device)
+        self.centers = nn.Parameter(self.centers.clone().detach().float(), requires_grad=False)
 
     def forward(self, bond_dists):
         """Expand distances.
 
         Parameters
         ----------
         bond_dists :
             Bond (edge) distances between two atoms (nodes)
 
-        Returns
+        Returns:
         -------
         A vector of expanded distance with shape [num_centers]
         """
         diff = bond_dists[:, None] - self.centers[None, :]
         return torch.exp(-self.width * (diff**2))
 
 
@@ -148,47 +146,47 @@
         funcs = [sympy.expand_func(sympy.functions.special.bessel.jn(i, x)) for i in range(self.max_l + 1)]
         return [sympy.lambdify(x, func, torch) for func in funcs]
 
     @lru_cache(maxsize=128)
     def _calculate_smooth_symbolic_funcs(self) -> list:
         return _get_lambda_func(max_n=self.max_n, cutoff=self.cutoff)
 
-    def __call__(self, r: torch.tensor) -> torch.tensor:
+    def __call__(self, r):
         """
         Args:
             r: torch.tensor, distance tensor, 1D
 
 
         Returns: [n, max_n * max_l] spherical Bessel function results
 
         """
         if self.smooth:
             return self._call_smooth_sbf(r)
         return self._call_sbf(r)
 
-    def _call_smooth_sbf(self, r: torch.tensor) -> torch.tensor:
+    def _call_smooth_sbf(self, r):
         results = [i(r) for i in self.funcs]
         return torch.t(torch.stack(results))
 
-    def _call_sbf(self, r: torch.tensor) -> torch.tensor:
+    def _call_sbf(self, r):
         roots = self.zeros[: self.max_l, : self.max_n]
 
         results = []
         factor = torch.tensor(sqrt(2.0 / self.cutoff**3))
         for i in range(self.max_l):
             root = roots[i]
             func = self.funcs[i]
             func_add1 = self.funcs[i + 1]
             results.append(
                 func(r[:, None] * root[None, :] / self.cutoff) * factor / torch.abs(func_add1(root[None, :]))
             )
         return torch.cat(results, axis=1)
 
     @staticmethod
-    def rbf_j0(r: torch.tensor, cutoff: float = 5.0, max_n: int = 3) -> torch.tensor:
+    def rbf_j0(r, cutoff: float = 5.0, max_n: int = 3):
         """
         Spherical Bessel function of order 0, ensuring the function value
         vanishes at cutoff
 
         Args:
             r: torch.tensor pytorch tensors
             cutoff: float, the cutoff radius
@@ -196,15 +194,15 @@
         Returns: basis function expansion using first spherical Bessel function
         """
         n = (torch.arange(1, max_n + 1)).type(dtype=DataType.torch_float)[None, :]
         r = r[:, None]
         return sqrt(2.0 / cutoff) * torch.sin(n * pi / cutoff * r) / r
 
 
-def _y00(theta, phi) -> torch.tensor:
+def _y00(theta, phi):
     r"""
     Spherical Harmonics with `l=m=0`
 
     ..math::
         Y_0^0 = \frac{1}{2} \sqrt{\frac{1}{\pi}}
 
     Args:
@@ -213,15 +211,15 @@
 
     Returns: `Y_0^0` results
 
     """
     return 0.5 * torch.ones_like(theta) * sqrt(1.0 / pi)
 
 
-def _conjugate(x) -> torch.tensor:
+def _conjugate(x):
     return torch.conj(x)
 
 
 class SphericalHarmonicsFunction:
     """
     Spherical Harmonics function
     """
@@ -234,29 +232,26 @@
                 the function will compute `Y_l^0`
         """
         self.max_l = max_l
         self.use_phi = use_phi
         funcs = []
         theta, phi = sympy.symbols("theta phi")
         for lval in range(self.max_l):
-            if self.use_phi:
-                m_list = range(-lval, lval + 1)
-            else:
-                m_list = [0]  # type: ignore
+            m_list = range(-lval, lval + 1) if self.use_phi else [0]  # type: ignore
             for m in m_list:
                 func = sympy.functions.special.spherical_harmonics.Znm(lval, m, theta, phi).expand(func=True)
                 funcs.append(func)
         # replace all theta with cos(theta)
         costheta = sympy.symbols("costheta")
         funcs = [i.subs({theta: sympy.acos(costheta)}) for i in funcs]
         self.orig_funcs = [sympy.simplify(i).evalf() for i in funcs]
         self.funcs = [sympy.lambdify([costheta, phi], i, [{"conjugate": _conjugate}, torch]) for i in self.orig_funcs]
         self.funcs[0] = _y00
 
-    def __call__(self, costheta, phi: torch.tensor | None = None) -> torch.tensor:
+    def __call__(self, costheta, phi=None):
         """
         Args:
             theta: torch.tensor, the azimuthal angle
             phi: torch.tensor, the polar angle
 
         Returns: [n, m] spherical harmonic results, where n is the number
             of angles. The column is arranged following
@@ -277,15 +272,15 @@
     for i, b in enumerate(block_size):
         indices.append(torch.tile(col_index[start : start + b], [repeats[i]]))
         start += b
     indices = torch.cat(indices, axis=0)
     return torch.index_select(array, 1, indices)
 
 
-def combine_sbf_shf(sbf: torch.tensor, shf: torch.tensor, max_n: int, max_l: int, use_phi: bool, use_smooth: bool):
+def combine_sbf_shf(sbf, shf, max_n: int, max_l: int, use_phi: bool, use_smooth: bool):
     """
     Combine the spherical Bessel function and the spherical Harmonics function
 
     For the spherical Bessel function, the column is ordered by
         [n=[0, ..., max_n-1], n=[0, ..., max_n-1], ...], max_l blocks,
 
     For the spherical Harmonics function, the column is ordered by
@@ -308,15 +303,15 @@
     if not use_phi:
         repeats_sbf = torch.tensor([1] * max_l * max_n)
         block_size = [1] * max_l
     else:
         # [1, 1, 1, ..., 1, 3, 3, 3, ..., 3, ...]
         repeats_sbf = torch.tensor(np.repeat(2 * np.arange(max_l) + 1, repeats=max_n))
         # tf.repeat(2 * tf.range(max_l) + 1, repeats=max_n)
-        block_size = 2 * np.arange(max_l) + 1
+        block_size = 2 * np.arange(max_l) + 1  # type: ignore
         # 2 * tf.range(max_l) + 1
     expanded_sbf = torch.repeat_interleave(sbf, repeats_sbf, 1)
     expanded_shf = _block_repeat(shf, block_size=block_size, repeats=[max_n] * max_l)
     shape = max_n * max_l
     if use_phi:
         shape *= max_l
     return torch.reshape(expanded_sbf * expanded_shf, [-1, shape])
@@ -356,15 +351,15 @@
         / torch.sqrt(2 * n**2 + 6 * n + 5)
         * (_sinc(r * (n + 1) * pi / cutoff) + _sinc(r * (n + 2) * pi / cutoff))
     )
     en = n**2 * (n + 2) ** 2 / (4 * (n + 1) ** 4 + 1)
     dn = [torch.tensor(1.0)]
     for i in range(1, max_n):
         dn.append(1 - en[0, i] / dn[-1])
-    dn = torch.stack(dn)
+    dn = torch.stack(dn)  # type: ignore
     gn = [fnr[:, 0]]
     for i in range(1, max_n):
         gn.append(1 / torch.sqrt(dn[i]) * (fnr[:, i] + torch.sqrt(en[0, i] / dn[i - 1]) * gn[-1]))
 
     return torch.t(torch.stack(gn))
 
 
@@ -398,15 +393,15 @@
 
     gnr = [fnr[0]]
     for i in range(1, max_n):
         gnr.append(1 / sympy.sqrt(dn[i]) * (fnr[i] + sympy.sqrt(en[i] / dn[i - 1]) * gnr[-1]))
     return [sympy.lambdify([r], sympy.simplify(i), torch) for i in gnr]
 
 
-def get_segment_indices_from_n(ns: torch.tensor) -> torch.tensor:
+def get_segment_indices_from_n(ns):
     """
     Get segment indices from number array. For example if
     ns = [2, 3], then the function will return [0, 0, 1, 1, 1]
 
     Args:
         ns: torch.tensor, the number of atoms/bonds array
 
@@ -416,17 +411,18 @@
     Returns: segment indices tensor
     """
     B = ns
     A = torch.arange(B.size(dim=0))
     return A.repeat_interleave(B, dim=0)
 
 
-def get_range_indices_from_n(ns: torch.tensor) -> torch.tensor:
+def get_range_indices_from_n(ns):
     """
     Give ns = [2, 3], return [0, 1, 0, 1, 2]
+
     Args:
         ns: torch.tensor, the number of atoms/bonds array
 
     Returns: range indices
     """
     max_n = torch.max(ns)
     n = ns.size(dim=0)
@@ -436,81 +432,130 @@
     )
     mask = torch.arange(max_n)[None, :] < ns[:, None]
 
     #    return matrix[mask]
     return torch.masked_select(matrix, mask)
 
 
-def unsorted_segment_fraction(data, segment_ids, num_segments):
-    """
-    Segment fraction
-    Args:
-        data (torch.tensor): original data
-        segment_ids (torch.tensor): segment ids
-        num_segments (torch.tensor): number of segments
-    Returns:
-        data (torch.tensor): data after fraction
-    """
-    segment_sum = scatter(data, segment_ids, dim=0, reduce="sum")
-    sums = torch.gather(segment_sum, 0, segment_ids)
-    data = torch.div(data, sums)
-    return data
+# def unsorted_segment_softmax(data, segment_ids, num_segments, weights=None):
+#    """
+#    Unsorted segment softmax with optional weights
+#    Args:
+#        data (tf.Tensor): original data
+#        segment_ids (tf.Tensor): tensor segment ids
+#        num_segments (int): number of segments
+#    Returns: tf.Tensor
+#    """
+#    if weights is None:
+#        weights = torch.ones(1)
+#    segment_max = scatter(data, segment_ids, dim=0, reduce="max")
+#    maxes = torch.gather(segment_max, 0, segment_ids)
+#    data -= maxes
+#    exp = torch.exp(data) * torch.squeeze(weights)
+#    softmax = torch.div(exp, torch.gather(scatter(exp, segment_ids, dim=0, reduce="sum"), 0, segment_ids))
+#    return softmax
 
 
-def unsorted_segment_softmax(data, segment_ids, num_segments, weights=None):
-    """
-    Unsorted segment softmax with optional weights
-    Args:
-        data (tf.Tensor): original data
-        segment_ids (tf.Tensor): tensor segment ids
-        num_segments (int): number of segments
-    Returns: tf.Tensor
-    """
-    if weights is None:
-        weights = torch.ones(1)
-    segment_max = scatter(data, segment_ids, dim=0, reduce="max")
-    maxes = torch.gather(segment_max, 0, segment_ids)
-    data -= maxes
-    exp = torch.exp(data) * torch.squeeze(weights)
-    softmax = torch.div(exp, torch.gather(scatter(exp, segment_ids, dim=0, reduce="sum"), 0, segment_ids))
-    return softmax
-
-
-def repeat_with_n(ns: torch.tensor, n: torch.tensor) -> torch.tensor:
+def repeat_with_n(ns, n):
     """
     Repeat the first dimension according to n array.
+
     Args:
         ns (torch.tensor): tensor
         n (torch.tensor): a list of replications
 
     Returns: repeated tensor
 
     """
     return torch.repeat_interleave(ns, n, dim=0)
 
 
 def broadcast_states_to_bonds(g, state_feat):
     """
     Broadcast state attributes of shape [Ns, Nstate] to
     bond attributes shape [Nb, Nstate]
+
     Args:
         g: DGL graph
         state_feat: state_feature
 
     Returns: broadcasted state attributes
 
     """
     return state_feat.repeat((g.num_edges(), 1))
 
 
 def broadcast_states_to_atoms(g, state_feat):
     """
     Broadcast state attributes of shape [Ns, Nstate] to
     bond attributes shape [Nb, Nstate]
+
     Args:
         g: DGL graph
         state_feat: state_feature
 
     Returns: broadcasted state attributes
 
     """
     return state_feat.repeat((g.num_nodes(), 1))
+
+
+def scatter_sum(input_tensor: torch.tensor, segment_ids: torch.tensor, num_segments: int, dim: int) -> torch.tensor:
+    """
+    Scatter sum operation along the specified dimension. Modified from the
+    torch_scatter library (https://github.com/rusty1s/pytorch_scatter).
+
+    Args:
+        input_tensor (torch.Tensor): The input tensor to be scattered.
+        segment_ids (torch.Tensor): Segment ID for each element in the input tensor.
+        num_segments (int): The number of segments.
+        dim (int): The dimension along which the scatter sum operation is performed (default: -1).
+
+    Returns:
+        resulting tensor
+    """
+    segment_ids = broadcast(segment_ids, input_tensor, dim)
+    size = list(input_tensor.size())
+    if segment_ids.numel() == 0:
+        size[dim] = 0
+    else:
+        size[dim] = num_segments
+    output = torch.zeros(size, dtype=input_tensor.dtype)
+    return output.scatter_add_(dim, segment_ids, input_tensor)
+
+
+def unsorted_segment_fraction(data: torch.tensor, segment_ids: torch.tensor, num_segments: torch.tensor):
+    """
+    Segment fraction
+    Args:
+        data (torch.tensor): original data
+        segment_ids (torch.tensor): segment ids
+        num_segments (torch.tensor): number of segments
+    Returns:
+        data (torch.tensor): data after fraction
+    """
+    segment_sum = scatter_sum(input_tensor=data, segment_ids=segment_ids, dim=0, num_segments=num_segments)
+    sums = torch.gather(segment_sum, 0, segment_ids)
+    data = torch.div(data, sums)
+    return data
+
+
+def broadcast(input_tensor: torch.tensor, target_tensor: torch.tensor, dim: int):
+    """
+    Broadcast input tensor along a given dimension to match the shape of the target tensor.
+    Modified from torch_scatter library (https://github.com/rusty1s/pytorch_scatter).
+    Args:
+        input_tensor: The tensor to broadcast.
+        target_tensor: The tensor whose shape to match.
+        dim: The dimension along which to broadcast.
+    Returns:
+        resulting inout tensor after broadcasting
+    """
+    if input_tensor.dim() == 1:
+        for _ in range(0, dim):
+            input_tensor = input_tensor.unsqueeze(0)
+    for _ in range(input_tensor.dim(), target_tensor.dim()):
+        input_tensor = input_tensor.unsqueeze(-1)
+    target_shape = list(target_tensor.shape)
+    target_shape[dim] = input_tensor.shape[dim]
+    input_tensor = input_tensor.expand(target_shape)
+    return input_tensor
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `matgl-0.1.0.dev0/matgl/utils/sb_roots.npy` & `matgl-0.2.0/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.1.0.dev0/matgl.egg-info/SOURCES.txt` & `matgl-0.2.0/matgl.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,25 +12,24 @@
 matgl.egg-info/top_level.txt
 matgl/dataloader/__init__.py
 matgl/dataloader/dataset.py
 matgl/graph/__init__.py
 matgl/graph/compute.py
 matgl/graph/converters.py
 matgl/layers/__init__.py
+matgl/layers/activations.py
 matgl/layers/atom_ref.py
 matgl/layers/bond_expansion.py
 matgl/layers/core.py
 matgl/layers/cutoff_functions.py
 matgl/layers/embedding_block.py
 matgl/layers/graph_conv.py
 matgl/layers/readout_block.py
 matgl/layers/three_body.py
 matgl/models/__init__.py
-matgl/models/layers.py
+matgl/models/ase_interface.py
 matgl/models/m3gnet.py
 matgl/models/megnet.py
 matgl/models/potential.py
-matgl/nbody/__init__.py
-matgl/nbody/three_body.py
 matgl/utils/__init__.py
 matgl/utils/maths.py
 matgl/utils/sb_roots.npy
```

### Comparing `matgl-0.1.0.dev0/setup.py` & `matgl-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,36 @@
-from setuptools import find_packages, setup
+from __future__ import annotations
+
+import os
+import re
+
 import numpy
+from setuptools import find_packages, setup
+
+this_dir = os.path.abspath(os.path.dirname(__file__))
+
+with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
+    long_description = f.read()
 
-VERSION = "0.1.0.dev"
+with open("matgl/__init__.py", encoding="utf-8") as fd:
+    for line in fd.readlines():
+        m = re.search('__version__ = "(.*)"', line)
+        if m:
+            version = m.group(1)
+            break
 
 setup(
     name="matgl",
-    version=VERSION,
+    version=version,
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong",
     author_email="ongsp@eng.ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@eng.ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science. ",
-    long_description=open("README.md").read(),
+    long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         "materials",
         "interatomic potential",
         "force field",
         "science",
         "property prediction",
```


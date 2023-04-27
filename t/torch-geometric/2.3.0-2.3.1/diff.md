# Comparing `tmp/torch_geometric-2.3.0.tar.gz` & `tmp/torch_geometric-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_geometric-2.3.0.tar", last modified: Thu Mar 23 06:05:48 2023, max compression
+gzip compressed data, was "torch_geometric-2.3.1.tar", last modified: Thu Apr 27 10:11:37 2023, max compression
```

## Comparing `torch_geometric-2.3.0.tar` & `torch_geometric-2.3.1.tar`

### file list

```diff
@@ -1,609 +1,727 @@
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.216620 torch_geometric-2.3.0/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1067 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/LICENSE
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      187 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/MANIFEST.in
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    61123 2023-03-23 06:05:48.216620 torch_geometric-2.3.0/PKG-INFO
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    59901 2023-03-22 09:27:57.000000 torch_geometric-2.3.0/README.md
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3067 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/pyproject.toml
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      103 2023-03-23 06:05:48.216620 torch_geometric-2.3.0/setup.cfg
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1422 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/setup.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.164620 torch_geometric-2.3.0/torch_geometric/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1043 2023-03-21 16:21:23.000000 torch_geometric-2.3.0/torch_geometric/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3392 2023-03-23 06:05:40.000000 torch_geometric-2.3.0/torch_geometric/compile.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.164620 torch_geometric-2.3.0/torch_geometric/contrib/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      352 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/contrib/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.164620 torch_geometric-2.3.0/torch_geometric/contrib/datasets/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)       23 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/contrib/datasets/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.164620 torch_geometric-2.3.0/torch_geometric/contrib/explain/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      163 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/contrib/explain/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    20540 2023-03-22 08:38:15.000000 torch_geometric-2.3.0/torch_geometric/contrib/explain/graphmask_explainer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    16627 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/contrib/explain/pgm_explainer.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.164620 torch_geometric-2.3.0/torch_geometric/contrib/nn/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)       72 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/contrib/nn/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.164620 torch_geometric-2.3.0/torch_geometric/contrib/nn/conv/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)       23 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/contrib/nn/conv/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.164620 torch_geometric-2.3.0/torch_geometric/contrib/nn/models/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      113 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/contrib/nn/models/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    33261 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/contrib/nn/models/rbcd_attack.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.164620 torch_geometric-2.3.0/torch_geometric/contrib/transforms/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)       23 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/contrib/transforms/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.164620 torch_geometric-2.3.0/torch_geometric/data/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3383 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7436 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/batch.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10181 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/collate.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    37547 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/data.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2897 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/datapipes.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    14850 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1359 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/download.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2252 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/extract.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    21075 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/feature_store.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    13495 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/graph_store.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    42291 2023-03-22 08:38:15.000000 torch_geometric-2.3.0/torch_geometric/data/hetero_data.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7091 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/in_memory_dataset.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.168620 torch_geometric-2.3.0/torch_geometric/data/lightning/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      178 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/lightning/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    28484 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/lightning/datamodule.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      338 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/makedirs.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3962 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/remote_backend_utils.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4279 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/separate.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    24835 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/storage.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2579 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/summary.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     9354 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/data/temporal.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1046 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/data/view.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.176620 torch_geometric-2.3.0/torch_geometric/datasets/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4770 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4220 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/actor.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5584 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/airfrans.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3711 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/airports.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3017 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/amazon.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4099 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/amazon_products.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4942 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/aminer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5266 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/aqsol.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5735 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/attributed_graph_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4063 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/ba2motif_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3518 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/ba_multi_shapes.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3824 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/ba_shapes.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4137 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/bitcoin_otc.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3942 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/citation_full.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2976 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/coauthor.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4564 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/coma.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4538 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/dblp.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5608 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/dbp15k.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2308 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/deezer_europe.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3862 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/dgraph.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5865 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/dynamic_faust.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4236 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/elliptic.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2631 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/email_eu_core.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7009 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/entities.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5817 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/explainer_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2228 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/facebook.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10215 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/datasets/fake.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3924 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/faust.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4099 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/flickr.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3815 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/freebase.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3416 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/gdelt.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     9261 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/ged_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2626 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/gemsec.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3954 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/geometry.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2484 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/github.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6762 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/gnn_benchmark_dataset.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.176620 torch_geometric-2.3.0/torch_geometric/datasets/graph_generator/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/graph_generator/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      965 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/graph_generator/ba_graph.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      949 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/graph_generator/base.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      918 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/graph_generator/er_graph.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1159 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/graph_generator/grid_graph.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3927 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/heterophilous_graph_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8467 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/hgb_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11053 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/hydro_net.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4447 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/icews.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4000 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/imdb.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7169 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/infection_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3439 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/jodie.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3444 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/karate.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4349 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/last_fm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2283 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/lastfm_asia.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6582 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/linkx_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11559 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/lrgb.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5044 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/malnet_tiny.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    16482 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/md17.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3770 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/mixhop_synthetic_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3136 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/mnist_superpixels.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5251 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/modelnet.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6593 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/molecule_net.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.176620 torch_geometric-2.3.0/torch_geometric/datasets/motif_generator/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      227 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/motif_generator/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      910 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/motif_generator/base.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1203 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/motif_generator/custom.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      984 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/motif_generator/cycle.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      801 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/motif_generator/house.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3787 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/movie_lens.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2889 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/nell.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7190 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/ogb_mag.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3415 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/omdb.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3964 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/particle.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10699 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/pascal.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4602 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/pascal_pf.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5716 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/pcpnet_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7016 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/planetoid.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2842 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/polblogs.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4866 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/ppi.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3182 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/qm7.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    16813 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/qm9.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2941 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/reddit.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4439 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/reddit2.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4345 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/rel_link_pred_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4173 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/s3dis.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8140 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/sbm_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8088 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/shapenet.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6150 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/shrec2016.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     9283 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/snap_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3031 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/suite_sparse.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3959 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/taobao.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4451 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/tosca.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7174 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/tu_dataset.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3464 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/twitch.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6929 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/upfd.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.176620 torch_geometric-2.3.0/torch_geometric/datasets/utils/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      156 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/datasets/utils/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1655 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/utils/cheatsheet.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4615 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/webkb.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3674 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/wikics.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6083 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/wikipedia_network.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6322 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/willow_object_class.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7857 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/word_net.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4116 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/yelp.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6171 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/datasets/zinc.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1197 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/debug.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      748 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/deprecation.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2466 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/experimental.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.176620 torch_geometric-2.3.0/torch_geometric/explain/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      359 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.176620 torch_geometric-2.3.0/torch_geometric/explain/algorithm/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      418 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/algorithm/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4491 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/algorithm/attention_explainer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6899 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/algorithm/base.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    12489 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/algorithm/captum.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6540 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/algorithm/captum_explainer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2867 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/algorithm/dummy_explainer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11149 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/algorithm/gnn_explainer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10370 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/algorithm/pg_explainer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2308 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/algorithm/utils.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7834 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/config.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10375 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/explainer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    12886 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/explanation.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.176620 torch_geometric-2.3.0/torch_geometric/explain/metric/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      301 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/metric/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1888 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/metric/basic.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3063 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/metric/faithfulness.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6157 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/explain/metric/fidelity.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2045 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      510 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/benchmark.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2371 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/checkpoint.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      738 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/cmd_args.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    17221 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/config.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    14545 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/config_store.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      389 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/act/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/act/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/config/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/config/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/encoder/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/encoder/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/head/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/head/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/layer/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/layer/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8304 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/layer/generalconv.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/loader/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/loader/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/loss/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/loss/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/network/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/network/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/optimizer/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/optimizer/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/pooling/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/pooling/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/stage/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/stage/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/train/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/train/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/transform/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/contrib/transform/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      375 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/imports.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      490 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/init.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11763 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/loader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11337 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/logger.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1474 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/loss.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2844 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/model_builder.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.180620 torch_geometric-2.3.0/torch_geometric/graphgym/models/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1121 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/models/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      822 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/models/act.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2546 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/models/encoder.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5133 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/models/gnn.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4323 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/models/head.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    12486 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/models/layer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      288 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/models/pooling.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1391 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/models/transform.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2544 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/optim.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3944 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/register.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1887 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/train.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.184620 torch_geometric-2.3.0/torch_geometric/graphgym/utils/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      641 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/utils/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     9513 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/utils/agg_runs.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3056 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/utils/comp_budget.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1352 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/graphgym/utils/device.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      690 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/utils/epoch.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2050 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/utils/io.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      606 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/utils/plot.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      198 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/graphgym/utils/tools.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      830 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/home.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.184620 torch_geometric-2.3.0/torch_geometric/io/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      528 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/io/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      943 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/io/npz.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      957 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/io/obj.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2586 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/io/off.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4191 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/io/planetoid.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      476 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/io/ply.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1136 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/io/sdf.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4733 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/io/tu.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      562 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/io/txt_array.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      768 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/lazy_loader.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.184620 torch_geometric-2.3.0/torch_geometric/loader/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1616 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1433 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/base.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6539 2023-03-22 08:38:15.000000 torch_geometric-2.3.0/torch_geometric/loader/cluster.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1449 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/data_list_loader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3222 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/dataloader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1683 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/dense_data_loader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4285 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/dynamic_batch_sampler.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8448 2023-03-22 08:38:15.000000 torch_geometric-2.3.0/torch_geometric/loader/graph_saint.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5715 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/hgt_loader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3754 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/imbalanced_sampler.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    13217 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/link_loader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11594 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/link_neighbor_loader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6282 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/mixin.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10463 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/neighbor_loader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8513 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/neighbor_sampler.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8634 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/node_loader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2196 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/random_node_loader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4173 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/shadow.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1319 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/temporal_dataloader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10931 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/utils.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3034 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/loader/zip_loader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      832 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/logging.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.188620 torch_geometric-2.3.0/torch_geometric/nn/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      911 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/__init__.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.188620 torch_geometric-2.3.0/torch_geometric/nn/aggr/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1397 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2395 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/attention.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7105 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/base.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10858 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/basic.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2064 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/deep_sets.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6881 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/equilibrium.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    12074 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/fused.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3062 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/gmt.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1464 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/gru.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1484 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/lstm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1995 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/mlp.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8088 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/multi.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5869 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/quantile.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4642 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/scaler.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2517 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/set2set.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3439 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/set_transformer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1772 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/sort.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8322 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/aggr/utils.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.196620 torch_geometric-2.3.0/torch_geometric/nn/conv/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3418 2023-03-21 16:21:26.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3088 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/agnn_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4388 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/antisymmetric_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6010 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/appnp.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6637 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/arma_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4036 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/cg_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6444 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/cheb_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5303 2023-03-23 06:05:40.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/cluster_gcn_conv.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.196620 torch_geometric-2.3.0/torch_geometric/nn/conv/cugraph/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      251 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/cugraph/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7365 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/cugraph/base.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2490 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/cugraph/gat_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4014 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/cugraph/rgcn_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2595 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/cugraph/sage_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    12105 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/dna_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5550 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/edge_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10482 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/eg_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7927 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/fa_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     9193 2023-03-21 16:21:26.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/fast_hgt_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4453 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/feast_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6332 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/film_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4242 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/fused_gat_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    13610 2023-03-22 10:32:22.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/gat_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3582 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/gated_graph_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    12423 2023-03-23 06:05:40.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/gatv2_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7022 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/gcn2_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     9333 2023-03-23 06:05:40.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/gcn_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     9992 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/gen_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7512 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/general_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7444 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/gin_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8320 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/gmm_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5764 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/gps_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3547 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/graph_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5023 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/gravnet_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7354 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/han_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6063 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/heat_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6067 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/hetero_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7891 2023-03-21 16:21:26.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/hgt_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7580 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/hypergraph_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3523 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/le_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2418 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/lg_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11833 2023-03-22 08:38:15.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/message_passing.jinja
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    40307 2023-03-22 08:38:15.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/message_passing.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4321 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/mf_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4743 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/nn_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4913 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/pan_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4916 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/pdn_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8242 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/pna_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4522 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/point_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3288 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/point_gnn_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5889 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/point_transformer_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5422 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/ppf_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4180 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/res_gated_graph_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    22785 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/rgat_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    14623 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/rgcn_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5813 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/sage_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4597 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/sg_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6283 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/signed_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3142 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/simple_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6330 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/spline_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5185 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/ssg_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11980 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/supergat_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4215 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/tag_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     9425 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/transformer_conv.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.196620 torch_geometric-2.3.0/torch_geometric/nn/conv/utils/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      823 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/utils/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2692 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/utils/cheatsheet.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      186 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/utils/helpers.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3267 2023-03-22 08:38:15.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/utils/inspector.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      679 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/utils/jit.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3743 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/utils/typing.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3103 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/wl_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2349 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/wl_conv_continuous.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5955 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/conv/x_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3960 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/data_parallel.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.196620 torch_geometric-2.3.0/torch_geometric/nn/dense/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      712 2023-03-22 08:38:15.000000 torch_geometric-2.3.0/torch_geometric/nn/dense/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4228 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/dense/dense_gat_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2989 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/dense/dense_gcn_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2357 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/dense/dense_gin_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2737 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/dense/dense_graph_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2658 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/dense/dense_sage_conv.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3050 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/dense/diff_pool.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5671 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/dense/dmon_pool.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    15353 2023-03-21 16:21:26.000000 torch_geometric-2.3.0/torch_geometric/nn/dense/linear.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4111 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/dense/mincut_pool.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3125 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/encoding.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.196620 torch_geometric-2.3.0/torch_geometric/nn/functional/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)       92 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/functional/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1549 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/functional/bro.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      863 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/functional/gini.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    15559 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/fx.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1088 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/glob.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2457 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/nn/inits.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.200620 torch_geometric-2.3.0/torch_geometric/nn/kge/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      200 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/kge/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5739 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/kge/base.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3234 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/kge/complex.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2462 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/kge/distmult.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      771 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/kge/loader.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3087 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/kge/transe.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8937 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/lr_scheduler.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     9464 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/model_hub.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.200620 torch_geometric-2.3.0/torch_geometric/nn/models/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1612 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6591 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/attentive_fp.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10656 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/autoencoder.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    27754 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/basic_gnn.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4138 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/captum.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6799 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/correct_and_smooth.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3972 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/deep_graph_infomax.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4223 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/deepgcn.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    34378 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/dimenet.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4611 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/nn/models/dimenet_utils.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7859 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/gnnff.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5397 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/graph_unet.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3397 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/jumping_knowledge.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3725 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/label_prop.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10472 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/lightgcn.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7901 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/linkx.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2566 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/mask_label.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6529 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/meta.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10173 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/metapath2vec.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8676 2023-03-21 12:50:03.000000 torch_geometric-2.3.0/torch_geometric/nn/models/mlp.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     7101 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/node2vec.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8987 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/re_net.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5789 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/rect.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11818 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/rev_gnn.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    16599 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/schnet.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     9840 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/models/signed_gcn.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11447 2023-03-22 08:38:15.000000 torch_geometric-2.3.0/torch_geometric/nn/models/tgn.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1576 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/module_dict.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.204620 torch_geometric-2.3.0/torch_geometric/nn/norm/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      638 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/norm/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8258 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/norm/batch_norm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4706 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/norm/diff_group_norm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2413 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/norm/graph_norm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1222 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/norm/graph_size_norm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4404 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/norm/instance_norm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6399 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/norm/layer_norm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1311 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/norm/mean_subtraction_norm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1654 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/norm/msg_norm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2536 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/norm/pair_norm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1453 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/parameter_dict.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.204620 torch_geometric-2.3.0/torch_geometric/nn/pool/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    10718 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6765 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/asap.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3749 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/avg_pool.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3345 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/base.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.204620 torch_geometric-2.3.0/torch_geometric/nn/pool/connect/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)       56 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/connect/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1369 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/connect/base.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      273 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/consecutive.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1600 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/decimation.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8567 2023-03-22 08:38:15.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/edge_pool.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3627 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/glob.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1292 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/graclus.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4045 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/max_pool.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4832 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/mem_pool.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4353 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/pan_pool.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      631 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/pool.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5919 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/sag_pool.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.204620 torch_geometric-2.3.0/torch_geometric/nn/pool/select/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)       54 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/select/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1308 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/select/base.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8347 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/topk_pool.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2727 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/pool/voxel_grid.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      412 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/nn/reshape.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5675 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/resolver.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1119 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/sequential.jinja
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4577 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/sequential.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5616 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/summary.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1282 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/to_fixed_size_transformer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6395 2023-03-21 16:21:26.000000 torch_geometric-2.3.0/torch_geometric/nn/to_hetero_module.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    18095 2023-03-22 09:59:59.000000 torch_geometric-2.3.0/torch_geometric/nn/to_hetero_transformer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    23139 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/to_hetero_with_bases_transformer.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.204620 torch_geometric-2.3.0/torch_geometric/nn/unpool/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      102 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/nn/unpool/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2586 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/nn/unpool/knn_interpolate.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.204620 torch_geometric-2.3.0/torch_geometric/profile/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      740 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/profile/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3356 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/profile/benchmark.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     8089 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/profile/profile.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    16665 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/profile/profiler.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4563 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/profile/utils.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1391 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/resolver.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.204620 torch_geometric-2.3.0/torch_geometric/sampler/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      481 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/sampler/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    19075 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/sampler/base.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2734 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/sampler/hgt_sampler.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    25362 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/sampler/neighbor_sampler.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4537 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/sampler/utils.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      354 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/seed.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.208620 torch_geometric-2.3.0/torch_geometric/testing/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      602 2023-03-21 16:21:23.000000 torch_geometric-2.3.0/torch_geometric/testing/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1755 2023-03-22 10:32:24.000000 torch_geometric-2.3.0/torch_geometric/testing/data.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3481 2023-03-22 08:38:15.000000 torch_geometric-2.3.0/torch_geometric/testing/decorators.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1847 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/testing/feature_store.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1009 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/testing/graph_store.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.212620 torch_geometric-2.3.0/torch_geometric/transforms/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3933 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    13966 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/add_metapaths.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4939 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/add_positional_encoding.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2019 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/add_self_loops.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1141 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/base_transform.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1937 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/cartesian.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      641 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/center.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      902 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/compose.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1961 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/constant.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1223 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/delaunay.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1810 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/distance.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1035 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/face_to_edge.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2898 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/feature_propagation.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2368 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/fixed_points.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1398 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/gcn_norm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    24216 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/gdc.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1019 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/generate_mesh_normals.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2512 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/grid_sampling.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2544 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/knn_graph.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2466 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/laplacian_lambda_max.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2001 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/largest_connected_components.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3724 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/line_graph.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1998 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/linear_transformation.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1699 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/local_cartesian.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1405 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/local_degree_profile.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4600 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/mask.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      979 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/normalize_features.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1739 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/normalize_rotation.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      621 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/normalize_scale.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1534 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/one_hot_degree.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    21080 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/pad.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1794 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/point_pair_features.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2127 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/polar.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2051 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/radius_graph.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      989 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/random_flip.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1511 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/random_jitter.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    14298 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/random_link_split.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5769 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/random_node_split.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1904 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/random_rotate.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1216 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/random_scale.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1320 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/random_shear.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1806 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/remove_duplicated_edges.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2284 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/remove_isolated_nodes.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      960 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/remove_training_classes.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6180 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/rooted_subgraph.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2141 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/sample_points.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1935 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/sign.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2242 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/spherical.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1003 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/svd_feature_reduction.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1608 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/target_indegree.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2328 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/to_dense.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1456 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/to_device.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5354 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/to_sparse_tensor.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2622 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/to_superpixels.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2973 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/to_undirected.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1283 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/two_hop.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2784 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/transforms/virtual_node.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4707 2023-03-21 16:21:26.000000 torch_geometric-2.3.0/torch_geometric/typing.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.216620 torch_geometric-2.3.0/torch_geometric/utils/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4406 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/utils/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2347 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/assortativity.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     9080 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/augmentation.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4927 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/coalesce.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    14817 2023-03-22 12:46:48.000000 torch_geometric-2.3.0/torch_geometric/utils/convert.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1018 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/degree.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11323 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/dropout.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1657 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/embedding.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4042 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/geodesic.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3755 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/get_laplacian.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4424 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/get_mesh_laplacian.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2536 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/grid.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2154 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/hetero.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4818 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/homophily.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3574 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/isolated.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    15855 2023-03-23 06:05:40.000000 torch_geometric-2.3.0/torch_geometric/utils/loop.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1884 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/mask.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      608 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/mixin.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    14643 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/negative_sampling.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3343 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/nested.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1169 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/normalized_cut.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1487 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/num_nodes.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1404 2023-03-22 11:58:42.000000 torch_geometric-2.3.0/torch_geometric/utils/one_hot.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5154 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/random.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      361 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/utils/repeat.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6835 2023-03-21 10:15:07.000000 torch_geometric-2.3.0/torch_geometric/utils/scatter.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1110 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/segment.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1856 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/select.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     6016 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/smiles.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2718 2023-03-22 09:26:55.000000 torch_geometric-2.3.0/torch_geometric/utils/softmax.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     1017 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/sort.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3034 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/sort_edge_index.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    11176 2023-03-23 06:05:40.000000 torch_geometric-2.3.0/torch_geometric/utils/sparse.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5518 2023-03-21 16:21:26.000000 torch_geometric-2.3.0/torch_geometric/utils/spmm.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    12225 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/subgraph.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3439 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/to_dense_adj.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4267 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/to_dense_batch.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     3489 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/train_test_split_edges.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4867 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/tree_decomposition.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4370 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/trim_to_layer.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     2125 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/unbatch.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     5770 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/utils/undirected.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.216620 torch_geometric-2.3.0/torch_geometric/visualization/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      123 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/visualization/__init__.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)     4149 2023-03-20 18:53:42.000000 torch_geometric-2.3.0/torch_geometric/visualization/graph.py
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      388 2023-03-19 07:27:40.000000 torch_geometric-2.3.0/torch_geometric/visualization/influence.py
-drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-03-23 06:05:48.164620 torch_geometric-2.3.0/torch_geometric.egg-info/
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    61123 2023-03-23 06:05:48.000000 torch_geometric-2.3.0/torch_geometric.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1001) matthias  (1001)    21257 2023-03-23 06:05:48.000000 torch_geometric-2.3.0/torch_geometric.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1001) matthias  (1001)        1 2023-03-23 06:05:48.000000 torch_geometric-2.3.0/torch_geometric.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1001) matthias  (1001)      544 2023-03-23 06:05:48.000000 torch_geometric-2.3.0/torch_geometric.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1001) matthias  (1001)       16 2023-03-23 06:05:48.000000 torch_geometric-2.3.0/torch_geometric.egg-info/top_level.txt
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.727117 torch_geometric-2.3.1/
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.655117 torch_geometric-2.3.1/.github/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5218 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/.github/CONTRIBUTING.md
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.655117 torch_geometric-2.3.1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2610 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      348 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      503 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/ISSUE_TEMPLATE/documentation.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      865 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1467 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/ISSUE_TEMPLATE/installation.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      615 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/ISSUE_TEMPLATE/refactor.yml
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.647117 torch_geometric-2.3.1/.github/actions/
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.655117 torch_geometric-2.3.1/.github/actions/setup/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1736 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/.github/actions/setup/action.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      583 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/labeler.yml
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/.github/workflows/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2683 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/workflows/building_pyg_conda.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2705 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/workflows/building_rusty1s_conda.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      361 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/workflows/changelog.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1243 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/.github/workflows/documentation.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1056 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/workflows/examples.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1069 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/.github/workflows/full_testing.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1256 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/.github/workflows/install.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      667 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.github/workflows/labeler.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1584 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/.github/workflows/linting.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1458 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/.github/workflows/nightly.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1174 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/.github/workflows/prev_testing.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1298 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/.github/workflows/testing.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      349 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/.gitignore
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1388 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/.pre-commit-config.yaml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    73354 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/CHANGELOG.md
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      363 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/CITATION.cff
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1067 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/LICENSE
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      187 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/MANIFEST.in
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    61123 2023-04-27 10:11:37.727117 torch_geometric-2.3.1/PKG-INFO
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    59901 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/README.md
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      252 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/codecov.yml
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.647117 torch_geometric-2.3.1/conda/
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/conda/pyg/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)       77 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/conda/pyg/README.md
+-rwxrwxr-x   0 matthias  (1001) matthias  (1001)     1584 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/conda/pyg/build_conda.sh
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1025 2023-04-27 10:11:11.000000 torch_geometric-2.3.1/conda/pyg/meta.yaml
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/conda/pytorch-geometric/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)       77 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/conda/pytorch-geometric/README.md
+-rwxrwxr-x   0 matthias  (1001) matthias  (1001)     1592 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/conda/pytorch-geometric/build_conda.sh
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1039 2023-04-27 10:10:50.000000 torch_geometric-2.3.1/conda/pytorch-geometric/meta.yaml
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/docker/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5823 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/docker/Dockerfile
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2674 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/docker/README.md
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1938 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/docker/singularity
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/graphgym/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      611 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/agg_batch.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/graphgym/configs/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      602 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/configs/example.yaml
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/graphgym/configs/pyg/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      627 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/configs/pyg/example_graph.yaml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      629 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/configs/pyg/example_link.yaml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      617 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/configs/pyg/example_node.yaml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8842 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/configs_gen.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/graphgym/custom_graphgym/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      389 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/graphgym/custom_graphgym/act/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/act/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      604 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/act/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/graphgym/custom_graphgym/config/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/config/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      708 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/config/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/graphgym/custom_graphgym/encoder/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/encoder/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1526 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/encoder/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.659117 torch_geometric-2.3.1/graphgym/custom_graphgym/head/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/head/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      766 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/head/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/custom_graphgym/layer/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/layer/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2840 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/layer/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/custom_graphgym/loader/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/loader/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      355 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/loader/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/custom_graphgym/loss/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/loss/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      325 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/loss/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/custom_graphgym/network/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/network/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1532 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/network/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/custom_graphgym/optimizer/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/optimizer/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      681 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/optimizer/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/custom_graphgym/pooling/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/pooling/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      307 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/pooling/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/custom_graphgym/stage/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/stage/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      944 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/stage/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/custom_graphgym/train/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/train/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2697 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/train/example.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/custom_graphgym/transform/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/custom_graphgym/transform/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/grids/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      611 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/grids/example.txt
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/grids/pyg/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      428 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/grids/pyg/example.txt
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1796 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/main.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      394 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/parallel.sh
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.651117 torch_geometric-2.3.1/graphgym/results/
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.651117 torch_geometric-2.3.1/graphgym/results/example_node_grid_example/
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/results/example_node_grid_example/agg/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2854 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/results/example_node_grid_example/agg/test.csv
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2829 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/results/example_node_grid_example/agg/test_best.csv
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2843 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/results/example_node_grid_example/agg/test_bestepoch.csv
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2640 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/results/example_node_grid_example/agg/train.csv
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2627 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/results/example_node_grid_example/agg/train_best.csv
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2592 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/results/example_node_grid_example/agg/train_bestepoch.csv
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2867 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/results/example_node_grid_example/agg/val.csv
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2817 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/results/example_node_grid_example/agg/val_best.csv
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2830 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/results/example_node_grid_example/agg/val_bestepoch.csv
+-rwxrwxr-x   0 matthias  (1001) matthias  (1001)     1049 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/run_batch.sh
+-rwxrwxr-x   0 matthias  (1001) matthias  (1001)      363 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/run_single.sh
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.663117 torch_geometric-2.3.1/graphgym/sample/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)       61 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/sample/dimensions.txt
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)        5 2023-04-27 09:48:26.000000 torch_geometric-2.3.1/graphgym/sample/dimensionsatt.txt
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3067 2023-04-27 10:10:45.000000 torch_geometric-2.3.1/pyproject.toml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      198 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/readthedocs.yml
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      103 2023-04-27 10:11:37.731117 torch_geometric-2.3.1/setup.cfg
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1422 2023-04-27 10:10:38.000000 torch_geometric-2.3.1/setup.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.667117 torch_geometric-2.3.1/torch_geometric/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1043 2023-04-27 10:10:32.000000 torch_geometric-2.3.1/torch_geometric/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3392 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/compile.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.667117 torch_geometric-2.3.1/torch_geometric/contrib/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      352 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/contrib/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.667117 torch_geometric-2.3.1/torch_geometric/contrib/datasets/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)       23 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/contrib/datasets/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.667117 torch_geometric-2.3.1/torch_geometric/contrib/explain/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      163 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/contrib/explain/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    20540 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/contrib/explain/graphmask_explainer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    16627 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/contrib/explain/pgm_explainer.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.667117 torch_geometric-2.3.1/torch_geometric/contrib/nn/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)       72 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/contrib/nn/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.667117 torch_geometric-2.3.1/torch_geometric/contrib/nn/conv/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)       23 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/contrib/nn/conv/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.667117 torch_geometric-2.3.1/torch_geometric/contrib/nn/models/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      113 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/contrib/nn/models/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    33261 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/contrib/nn/models/rbcd_attack.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.667117 torch_geometric-2.3.1/torch_geometric/contrib/transforms/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)       23 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/contrib/transforms/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.671117 torch_geometric-2.3.1/torch_geometric/data/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3383 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7436 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/batch.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10432 2023-04-27 09:57:26.000000 torch_geometric-2.3.1/torch_geometric/data/collate.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    37547 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/data/data.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2897 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/data/datapipes.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    14850 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1359 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/download.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2252 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/extract.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    21075 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/feature_store.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    13495 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/graph_store.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    42291 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/hetero_data.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7091 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/in_memory_dataset.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.671117 torch_geometric-2.3.1/torch_geometric/data/lightning/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      178 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/lightning/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    28490 2023-04-27 09:55:40.000000 torch_geometric-2.3.1/torch_geometric/data/lightning/datamodule.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      338 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/makedirs.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3962 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/remote_backend_utils.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4279 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/data/separate.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    24947 2023-04-27 09:55:07.000000 torch_geometric-2.3.1/torch_geometric/data/storage.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2579 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/data/summary.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     9354 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/temporal.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1046 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/data/view.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.679117 torch_geometric-2.3.1/torch_geometric/datasets/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4770 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/datasets/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4220 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/actor.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5584 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/airfrans.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3711 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/airports.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3017 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/amazon.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4099 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/amazon_products.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4942 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/aminer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5266 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/aqsol.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5735 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/attributed_graph_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4063 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/ba2motif_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3518 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/ba_multi_shapes.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3824 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/ba_shapes.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4137 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/bitcoin_otc.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3942 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/citation_full.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2976 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/coauthor.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4564 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/coma.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4538 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/dblp.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5608 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/dbp15k.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2308 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/deezer_europe.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3862 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/dgraph.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5865 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/dynamic_faust.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4236 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/datasets/elliptic.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2631 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/email_eu_core.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7009 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/entities.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5817 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/explainer_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2228 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/facebook.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10215 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/fake.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3924 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/faust.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4099 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/flickr.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3815 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/freebase.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3416 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/gdelt.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     9261 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/ged_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2626 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/gemsec.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3954 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/geometry.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2484 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/github.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6762 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/gnn_benchmark_dataset.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.683117 torch_geometric-2.3.1/torch_geometric/datasets/graph_generator/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/graph_generator/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      965 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/graph_generator/ba_graph.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      949 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/graph_generator/base.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      918 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/graph_generator/er_graph.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1159 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/graph_generator/grid_graph.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3927 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/datasets/heterophilous_graph_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8467 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/hgb_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11053 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/hydro_net.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4447 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/icews.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4000 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/imdb.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7169 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/infection_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3439 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/jodie.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3444 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/karate.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4349 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/last_fm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2283 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/lastfm_asia.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6582 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/linkx_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11559 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/lrgb.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5044 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/malnet_tiny.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    16482 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/md17.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3770 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/mixhop_synthetic_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3136 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/mnist_superpixels.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5251 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/modelnet.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6593 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/molecule_net.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.683117 torch_geometric-2.3.1/torch_geometric/datasets/motif_generator/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      227 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/motif_generator/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      910 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/motif_generator/base.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1203 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/motif_generator/custom.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      984 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/motif_generator/cycle.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      801 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/motif_generator/house.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3787 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/movie_lens.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2889 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/nell.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7190 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/ogb_mag.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3415 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/omdb.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3964 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/particle.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10699 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/pascal.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4602 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/pascal_pf.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5716 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/pcpnet_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7016 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/planetoid.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2842 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/polblogs.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4866 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/ppi.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3182 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/qm7.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    16813 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/qm9.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2941 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/reddit.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4439 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/reddit2.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4345 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/rel_link_pred_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4173 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/s3dis.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8140 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/sbm_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8088 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/shapenet.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6150 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/shrec2016.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     9283 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/snap_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3031 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/suite_sparse.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3959 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/taobao.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4451 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/tosca.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7174 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/tu_dataset.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3464 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/twitch.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6929 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/upfd.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.683117 torch_geometric-2.3.1/torch_geometric/datasets/utils/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      156 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/utils/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1655 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/utils/cheatsheet.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4615 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/webkb.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3674 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/wikics.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6083 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/wikipedia_network.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6322 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/willow_object_class.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7857 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/word_net.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4116 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/yelp.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6171 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/datasets/zinc.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1197 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/debug.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      748 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/deprecation.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2466 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/experimental.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.683117 torch_geometric-2.3.1/torch_geometric/explain/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      359 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.683117 torch_geometric-2.3.1/torch_geometric/explain/algorithm/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      418 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/algorithm/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4491 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/algorithm/attention_explainer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6899 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/algorithm/base.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    12489 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/algorithm/captum.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6540 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/algorithm/captum_explainer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2867 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/algorithm/dummy_explainer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11149 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/algorithm/gnn_explainer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10370 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/algorithm/pg_explainer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2308 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/algorithm/utils.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7834 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/config.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10375 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/explainer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    12882 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/explain/explanation.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.683117 torch_geometric-2.3.1/torch_geometric/explain/metric/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      301 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/metric/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1888 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/metric/basic.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3063 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/metric/faithfulness.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6157 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/explain/metric/fidelity.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2045 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      510 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/benchmark.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2371 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/checkpoint.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      738 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/cmd_args.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    17221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/config.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    14545 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/graphgym/config_store.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      389 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/act/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/act/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/config/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/config/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/encoder/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/encoder/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/head/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/head/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/layer/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/layer/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8304 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/layer/generalconv.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/loader/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/loader/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/loss/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/loss/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/network/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/network/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/optimizer/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/optimizer/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/pooling/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/pooling/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/stage/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/stage/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/train/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/train/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/transform/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      221 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/contrib/transform/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      375 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/imports.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      490 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/init.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11763 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/loader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11337 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/logger.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1474 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/loss.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2844 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/model_builder.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.687117 torch_geometric-2.3.1/torch_geometric/graphgym/models/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1121 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/models/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      822 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/models/act.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2546 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/models/encoder.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5133 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/models/gnn.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4323 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/models/head.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    12486 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/models/layer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      288 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/models/pooling.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1391 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/models/transform.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2544 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/optim.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3944 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/register.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1887 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/train.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.691117 torch_geometric-2.3.1/torch_geometric/graphgym/utils/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)        0 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/utils/LICENSE
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      641 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/utils/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     9513 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/utils/agg_runs.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3056 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/utils/comp_budget.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1352 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/utils/device.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      690 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/utils/epoch.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2050 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/utils/io.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      606 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/utils/plot.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      198 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/graphgym/utils/tools.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      830 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/home.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.691117 torch_geometric-2.3.1/torch_geometric/io/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      528 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/io/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      943 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/io/npz.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      957 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/io/obj.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2586 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/io/off.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4211 2023-04-27 09:58:07.000000 torch_geometric-2.3.1/torch_geometric/io/planetoid.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      476 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/io/ply.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1136 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/io/sdf.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4733 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/io/tu.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      562 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/io/txt_array.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      768 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/lazy_loader.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.691117 torch_geometric-2.3.1/torch_geometric/loader/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1616 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1433 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/base.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6539 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/cluster.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1449 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/data_list_loader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3222 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/dataloader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1683 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/dense_data_loader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4285 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/dynamic_batch_sampler.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8448 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/graph_saint.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5715 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/hgt_loader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3754 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/imbalanced_sampler.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    13217 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/loader/link_loader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11594 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/loader/link_neighbor_loader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6282 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/mixin.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10463 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/loader/neighbor_loader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8513 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/neighbor_sampler.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8634 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/loader/node_loader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2196 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/random_node_loader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4173 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/shadow.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1319 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/temporal_dataloader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10931 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/loader/utils.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3034 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/loader/zip_loader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      832 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/logging.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.695117 torch_geometric-2.3.1/torch_geometric/nn/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      911 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/__init__.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.699117 torch_geometric-2.3.1/torch_geometric/nn/aggr/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1397 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2395 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/attention.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7105 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/base.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10858 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/basic.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2064 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/deep_sets.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6881 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/equilibrium.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    12074 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/fused.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3062 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/gmt.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1464 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/gru.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1484 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/lstm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1995 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/mlp.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8088 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/multi.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5869 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/quantile.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4642 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/scaler.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2517 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/set2set.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3439 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/set_transformer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1772 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/sort.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8322 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/aggr/utils.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.703117 torch_geometric-2.3.1/torch_geometric/nn/conv/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3418 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3088 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/agnn_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4388 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/antisymmetric_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6010 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/appnp.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6637 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/arma_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4036 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/cg_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6444 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/cheb_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5303 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/cluster_gcn_conv.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.707117 torch_geometric-2.3.1/torch_geometric/nn/conv/cugraph/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      251 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/cugraph/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8195 2023-04-27 09:58:30.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/cugraph/base.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2849 2023-04-27 09:58:30.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/cugraph/gat_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4218 2023-04-27 09:58:30.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/cugraph/rgcn_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2802 2023-04-27 09:58:30.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/cugraph/sage_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    12105 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/dna_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5550 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/edge_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10482 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/eg_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7927 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/fa_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     9193 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/fast_hgt_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4453 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/feast_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6332 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/film_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4242 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/fused_gat_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    13610 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/gat_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3582 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/gated_graph_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    12423 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/gatv2_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7022 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/gcn2_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     9333 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/gcn_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     9992 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/gen_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7512 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/general_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7444 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/gin_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8320 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/gmm_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5764 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/gps_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3547 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/graph_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5023 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/gravnet_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7354 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/han_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6063 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/heat_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6067 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/hetero_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7891 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/hgt_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7580 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/hypergraph_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3523 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/le_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2418 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/lg_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11833 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/message_passing.jinja
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    40307 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/message_passing.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4321 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/mf_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4743 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/nn_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4913 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/pan_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4916 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/pdn_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8242 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/pna_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4522 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/point_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3288 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/point_gnn_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5889 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/point_transformer_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5422 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/ppf_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4180 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/res_gated_graph_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    22785 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/rgat_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    14623 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/rgcn_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5813 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/sage_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4597 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/sg_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6283 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/signed_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3142 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/simple_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6330 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/spline_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5185 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/ssg_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11980 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/supergat_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4215 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/tag_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     9425 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/transformer_conv.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.707117 torch_geometric-2.3.1/torch_geometric/nn/conv/utils/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      823 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/utils/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2692 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/utils/cheatsheet.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      186 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/utils/helpers.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3267 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/utils/inspector.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      679 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/utils/jit.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3743 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/utils/typing.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3103 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/wl_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2349 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/wl_conv_continuous.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5955 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/conv/x_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3960 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/data_parallel.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.707117 torch_geometric-2.3.1/torch_geometric/nn/dense/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      712 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/dense/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4228 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/dense/dense_gat_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2989 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/dense/dense_gcn_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2357 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/dense/dense_gin_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2737 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/dense/dense_graph_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2658 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/dense/dense_sage_conv.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3050 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/dense/diff_pool.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5671 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/dense/dmon_pool.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    15353 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/dense/linear.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4111 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/dense/mincut_pool.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3125 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/encoding.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.707117 torch_geometric-2.3.1/torch_geometric/nn/functional/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)       92 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/functional/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1549 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/functional/bro.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      863 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/functional/gini.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    15559 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/fx.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1088 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/glob.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2457 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/inits.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.707117 torch_geometric-2.3.1/torch_geometric/nn/kge/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      200 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/kge/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5739 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/kge/base.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3234 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/kge/complex.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2462 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/kge/distmult.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      771 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/kge/loader.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3087 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/kge/transe.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8937 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/lr_scheduler.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     9464 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/model_hub.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.711117 torch_geometric-2.3.1/torch_geometric/nn/models/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1612 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6591 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/attentive_fp.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10656 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/autoencoder.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    27754 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/basic_gnn.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4138 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/captum.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6799 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/correct_and_smooth.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3972 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/deep_graph_infomax.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4223 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/deepgcn.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    34378 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/models/dimenet.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4611 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/dimenet_utils.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7859 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/gnnff.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5397 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/models/graph_unet.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3397 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/jumping_knowledge.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3725 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/models/label_prop.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10472 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/models/lightgcn.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7901 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/linkx.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2566 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/mask_label.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6529 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/meta.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10173 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/models/metapath2vec.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8676 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/models/mlp.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     7101 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/models/node2vec.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8987 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/re_net.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5789 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/rect.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11818 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/rev_gnn.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    16599 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/schnet.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     9840 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/models/signed_gcn.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11447 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/models/tgn.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1576 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/module_dict.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.711117 torch_geometric-2.3.1/torch_geometric/nn/norm/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      638 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/norm/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8258 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/norm/batch_norm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4706 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/norm/diff_group_norm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2413 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/norm/graph_norm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1222 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/norm/graph_size_norm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4404 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/norm/instance_norm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6399 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/norm/layer_norm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1311 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/norm/mean_subtraction_norm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1654 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/norm/msg_norm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2536 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/norm/pair_norm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1453 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/parameter_dict.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.715117 torch_geometric-2.3.1/torch_geometric/nn/pool/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    10718 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6765 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/asap.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3749 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/avg_pool.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3345 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/base.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.715117 torch_geometric-2.3.1/torch_geometric/nn/pool/connect/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)       56 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/connect/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1369 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/connect/base.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      273 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/consecutive.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1600 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/decimation.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8567 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/edge_pool.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3627 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/glob.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1292 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/graclus.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4045 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/max_pool.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4832 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/mem_pool.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4353 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/pan_pool.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      631 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/pool.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5919 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/sag_pool.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.715117 torch_geometric-2.3.1/torch_geometric/nn/pool/select/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)       54 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/select/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1308 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/select/base.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8347 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/topk_pool.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2727 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/pool/voxel_grid.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      412 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/reshape.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5675 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/resolver.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1119 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/sequential.jinja
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4577 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/sequential.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5616 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/summary.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1282 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/to_fixed_size_transformer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6395 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/to_hetero_module.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    18095 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/nn/to_hetero_transformer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    23139 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/to_hetero_with_bases_transformer.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.715117 torch_geometric-2.3.1/torch_geometric/nn/unpool/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      102 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/unpool/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2586 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/nn/unpool/knn_interpolate.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.715117 torch_geometric-2.3.1/torch_geometric/profile/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      740 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/profile/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3356 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/profile/benchmark.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     8089 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/profile/profile.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    16665 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/profile/profiler.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4563 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/profile/utils.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1391 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/resolver.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.715117 torch_geometric-2.3.1/torch_geometric/sampler/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      481 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/sampler/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    19075 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/sampler/base.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2734 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/sampler/hgt_sampler.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    25362 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/sampler/neighbor_sampler.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4537 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/sampler/utils.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      354 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/seed.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.715117 torch_geometric-2.3.1/torch_geometric/testing/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      602 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/testing/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1755 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/testing/data.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3481 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/testing/decorators.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1847 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/testing/feature_store.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1009 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/testing/graph_store.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.723117 torch_geometric-2.3.1/torch_geometric/transforms/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3933 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/transforms/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    13966 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/add_metapaths.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4939 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/transforms/add_positional_encoding.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2019 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/add_self_loops.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1141 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/base_transform.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1937 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/cartesian.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      641 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/center.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      902 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/transforms/compose.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1961 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/constant.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1223 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/delaunay.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1810 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/distance.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1035 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/face_to_edge.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2898 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/transforms/feature_propagation.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2368 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/fixed_points.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1398 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/gcn_norm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    24216 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/gdc.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1019 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/generate_mesh_normals.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2512 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/grid_sampling.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2544 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/knn_graph.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2466 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/laplacian_lambda_max.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2001 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/largest_connected_components.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3724 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/line_graph.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1998 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/linear_transformation.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1699 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/local_cartesian.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1405 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/local_degree_profile.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4600 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/mask.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      979 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/transforms/normalize_features.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1739 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/normalize_rotation.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      621 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/normalize_scale.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1534 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/one_hot_degree.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    21080 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/pad.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1794 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/point_pair_features.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2127 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/polar.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2051 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/radius_graph.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      989 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/random_flip.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1511 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/random_jitter.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    14298 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/random_link_split.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5769 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/random_node_split.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1904 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/random_rotate.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1216 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/random_scale.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1320 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/random_shear.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1806 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/remove_duplicated_edges.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2284 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/remove_isolated_nodes.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      960 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/remove_training_classes.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6180 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/transforms/rooted_subgraph.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2141 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/sample_points.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1935 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/transforms/sign.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2242 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/spherical.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1003 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/svd_feature_reduction.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1608 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/target_indegree.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2328 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/to_dense.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1456 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/to_device.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5354 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/to_sparse_tensor.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2622 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/to_superpixels.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2973 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/to_undirected.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1283 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/transforms/two_hop.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2784 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/transforms/virtual_node.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4707 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/typing.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.727117 torch_geometric-2.3.1/torch_geometric/utils/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4406 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/utils/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2347 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/assortativity.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     9080 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/augmentation.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4927 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/utils/coalesce.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    14817 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/utils/convert.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1018 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/degree.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11323 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/dropout.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1657 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/embedding.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4042 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/geodesic.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3755 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/get_laplacian.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4424 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/get_mesh_laplacian.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2536 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/grid.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2154 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/utils/hetero.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4818 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/homophily.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3574 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/isolated.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    15855 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/loop.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1884 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/mask.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      608 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/mixin.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    14643 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/negative_sampling.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3343 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/utils/nested.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1169 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/normalized_cut.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1487 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/utils/num_nodes.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1404 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/one_hot.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5154 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/random.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      361 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/repeat.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6835 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/utils/scatter.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1110 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/segment.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1856 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/utils/select.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     6016 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/smiles.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2718 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/softmax.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     1017 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/sort.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3034 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/sort_edge_index.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    11176 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/utils/sparse.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5547 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/spmm.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    12370 2023-04-27 09:56:05.000000 torch_geometric-2.3.1/torch_geometric/utils/subgraph.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3439 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/to_dense_adj.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4267 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/to_dense_batch.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     3489 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/train_test_split_edges.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4867 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/tree_decomposition.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4370 2023-04-27 10:10:22.000000 torch_geometric-2.3.1/torch_geometric/utils/trim_to_layer.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     2125 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/unbatch.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     5770 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/utils/undirected.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.727117 torch_geometric-2.3.1/torch_geometric/visualization/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      123 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/visualization/__init__.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)     4149 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/visualization/graph.py
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      388 2023-04-27 09:48:27.000000 torch_geometric-2.3.1/torch_geometric/visualization/influence.py
+drwxrwxr-x   0 matthias  (1001) matthias  (1001)        0 2023-04-27 10:11:37.667117 torch_geometric-2.3.1/torch_geometric.egg-info/
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    61123 2023-04-27 10:11:37.000000 torch_geometric-2.3.1/torch_geometric.egg-info/PKG-INFO
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)    24394 2023-04-27 10:11:37.000000 torch_geometric-2.3.1/torch_geometric.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)        1 2023-04-27 10:11:37.000000 torch_geometric-2.3.1/torch_geometric.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)      544 2023-04-27 10:11:37.000000 torch_geometric-2.3.1/torch_geometric.egg-info/requires.txt
+-rw-rw-r--   0 matthias  (1001) matthias  (1001)       16 2023-04-27 10:11:37.000000 torch_geometric-2.3.1/torch_geometric.egg-info/top_level.txt
```

### Comparing `torch_geometric-2.3.0/LICENSE` & `torch_geometric-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/PKG-INFO` & `torch_geometric-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_geometric
-Version: 2.3.0
+Version: 2.3.1
 Summary: Graph Neural Network Library for PyTorch
 Author-email: Matthias Fey <matthias@pyg.org>
 Project-URL: homepage, https://pyg.org
 Project-URL: documentation, https://pytorch-geometric.readthedocs.io
 Project-URL: repository, https://github.com/pyg-team/pytorch_geometric.git
 Project-URL: changelog, https://github.com/pyg-team/pytorch_geometric/blob/master/CHANGELOG.md
 Keywords: deep-learning,pytorch,geometric-deep-learning,graph-neural-networks,graph-convolutional-networks
```

### Comparing `torch_geometric-2.3.0/README.md` & `torch_geometric-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/pyproject.toml` & `torch_geometric-2.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="torch_geometric"
-version="2.3.0"
+version="2.3.1"
 authors=[
     {name="Matthias Fey", email="matthias@pyg.org"},
 ]
 description="Graph Neural Network Library for PyTorch"
 readme="README.md"
 requires-python=">=3.7"
 keywords=[
```

### Comparing `torch_geometric-2.3.0/setup.py` & `torch_geometric-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '2.3.0'
+__version__ = '2.3.1'
 
 install_requires = [
     'tqdm',
     'numpy',
     'scipy',
     'jinja2',
     'requests',
```

### Comparing `torch_geometric-2.3.0/torch_geometric/__init__.py` & `torch_geometric-2.3.1/torch_geometric/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .experimental import (is_experimental_mode_enabled, experimental_mode,
                            set_experimental_mode)
 from .lazy_loader import LazyLoader
 
 contrib = LazyLoader('contrib', globals(), 'torch_geometric.contrib')
 graphgym = LazyLoader('graphgym', globals(), 'torch_geometric.graphgym')
 
-__version__ = '2.3.0'
+__version__ = '2.3.1'
 
 __all__ = [
     'seed_everything',
     'get_home_dir',
     'set_home_dir',
     'compile',
     'is_debug_enabled',
```

### Comparing `torch_geometric-2.3.0/torch_geometric/compile.py` & `torch_geometric-2.3.1/torch_geometric/compile.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/contrib/explain/graphmask_explainer.py` & `torch_geometric-2.3.1/torch_geometric/contrib/explain/graphmask_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/contrib/explain/pgm_explainer.py` & `torch_geometric-2.3.1/torch_geometric/contrib/explain/pgm_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/contrib/nn/models/rbcd_attack.py` & `torch_geometric-2.3.1/torch_geometric/contrib/nn/models/rbcd_attack.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/__init__.py` & `torch_geometric-2.3.1/torch_geometric/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/batch.py` & `torch_geometric-2.3.1/torch_geometric/data/batch.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/collate.py` & `torch_geometric-2.3.1/torch_geometric/data/collate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import defaultdict
 from collections.abc import Mapping, Sequence
 from typing import Any, List, Optional, Tuple, Union
 
 import torch
 from torch import Tensor
 
+import torch_geometric.typing
 from torch_geometric.data.data import BaseData
 from torch_geometric.data.storage import BaseStorage, NodeStorage
 from torch_geometric.typing import SparseTensor, torch_sparse
 
 
 def collate(
     cls,
@@ -138,15 +139,19 @@
                 ]
         else:
             incs = None
 
         if torch.utils.data.get_worker_info() is not None:
             # Write directly into shared memory to avoid an extra copy:
             numel = sum(value.numel() for value in values)
-            storage = elem.storage()._new_shared(numel)
+            if torch_geometric.typing.WITH_PT2:
+                storage = elem.untyped_storage()._new_shared(
+                    numel * elem.element_size(), device=elem.device)
+            else:
+                storage = elem.storage()._new_shared(numel, device=elem.device)
             shape = list(elem.size())
             if cat_dim is None or elem.dim() == 0:
                 shape = [len(values)] + shape
             else:
                 shape[cat_dim] = int(slices[-1])
             out = elem.new(storage).resize_(*shape)
         else:
```

### Comparing `torch_geometric-2.3.0/torch_geometric/data/data.py` & `torch_geometric-2.3.1/torch_geometric/data/data.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/datapipes.py` & `torch_geometric-2.3.1/torch_geometric/data/datapipes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/dataset.py` & `torch_geometric-2.3.1/torch_geometric/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/download.py` & `torch_geometric-2.3.1/torch_geometric/data/download.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/extract.py` & `torch_geometric-2.3.1/torch_geometric/data/extract.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/feature_store.py` & `torch_geometric-2.3.1/torch_geometric/data/feature_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/graph_store.py` & `torch_geometric-2.3.1/torch_geometric/data/graph_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/hetero_data.py` & `torch_geometric-2.3.1/torch_geometric/data/hetero_data.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/in_memory_dataset.py` & `torch_geometric-2.3.1/torch_geometric/data/in_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/lightning/datamodule.py` & `torch_geometric-2.3.1/torch_geometric/data/lightning/datamodule.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             warnings.warn("'sampler' option is not supported for "
                           "loader='full'")
             kwargs.pop('sampler', None)
 
         if loader == 'full' and kwargs.get('batch_sampler') is not None:
             warnings.warn("'batch_sampler' option is not supported for "
                           "loader='full'")
-            kwargs.pop('sampler', None)
+            kwargs.pop('batch_sampler', None)
 
         super().__init__(has_val, has_test, **kwargs)
 
         if loader == 'full':
             if kwargs.get('pin_memory', False):
                 warnings.warn(f"Re-setting 'pin_memory' to 'False' in "
                               f"'{self.__class__.__name__}' for loader='full' "
```

### Comparing `torch_geometric-2.3.0/torch_geometric/data/remote_backend_utils.py` & `torch_geometric-2.3.1/torch_geometric/data/remote_backend_utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/separate.py` & `torch_geometric-2.3.1/torch_geometric/data/separate.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/storage.py` & `torch_geometric-2.3.1/torch_geometric/data/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from torch import Tensor
 
 from torch_geometric.data.view import ItemsView, KeysView, ValuesView
 from torch_geometric.typing import EdgeType, NodeType, SparseTensor
 from torch_geometric.utils import (
     coalesce,
     contains_isolated_nodes,
+    is_torch_sparse_tensor,
     is_undirected,
 )
 
 N_KEYS = {'x', 'feat', 'pos', 'batch', 'node_type', 'n_id'}
 E_KEYS = {'edge_index', 'edge_weight', 'edge_attr', 'edge_type', 'e_id'}
 
 
@@ -414,14 +415,16 @@
         for key, value in self.items():
             if isinstance(value, (Tensor, np.ndarray)) and 'edge' in key:
                 cat_dim = self._parent().__cat_dim__(key, value, self)
                 return value.shape[cat_dim]
         for value in self.values('adj', 'adj_t'):
             if isinstance(value, SparseTensor):
                 return value.nnz()
+            elif is_torch_sparse_tensor(value):
+                return value._nnz()
         return 0
 
     @property
     def num_edge_features(self) -> int:
         if ('edge_attr' in self and isinstance(self.edge_attr,
                                                (Tensor, np.ndarray))):
             return 1 if self.edge_attr.ndim == 1 else self.edge_attr.shape[-1]
```

### Comparing `torch_geometric-2.3.0/torch_geometric/data/summary.py` & `torch_geometric-2.3.1/torch_geometric/data/summary.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/temporal.py` & `torch_geometric-2.3.1/torch_geometric/data/temporal.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/data/view.py` & `torch_geometric-2.3.1/torch_geometric/data/view.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/__init__.py` & `torch_geometric-2.3.1/torch_geometric/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/actor.py` & `torch_geometric-2.3.1/torch_geometric/datasets/actor.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/airfrans.py` & `torch_geometric-2.3.1/torch_geometric/datasets/airfrans.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/airports.py` & `torch_geometric-2.3.1/torch_geometric/datasets/airports.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/amazon.py` & `torch_geometric-2.3.1/torch_geometric/datasets/amazon.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/amazon_products.py` & `torch_geometric-2.3.1/torch_geometric/datasets/amazon_products.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/aminer.py` & `torch_geometric-2.3.1/torch_geometric/datasets/aminer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/aqsol.py` & `torch_geometric-2.3.1/torch_geometric/datasets/aqsol.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/attributed_graph_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/attributed_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/ba2motif_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/ba2motif_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/ba_multi_shapes.py` & `torch_geometric-2.3.1/torch_geometric/datasets/ba_multi_shapes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/ba_shapes.py` & `torch_geometric-2.3.1/torch_geometric/datasets/ba_shapes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/bitcoin_otc.py` & `torch_geometric-2.3.1/torch_geometric/datasets/bitcoin_otc.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/citation_full.py` & `torch_geometric-2.3.1/torch_geometric/datasets/citation_full.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/coauthor.py` & `torch_geometric-2.3.1/torch_geometric/datasets/coauthor.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/coma.py` & `torch_geometric-2.3.1/torch_geometric/datasets/coma.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/dblp.py` & `torch_geometric-2.3.1/torch_geometric/datasets/dblp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/dbp15k.py` & `torch_geometric-2.3.1/torch_geometric/datasets/dbp15k.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/deezer_europe.py` & `torch_geometric-2.3.1/torch_geometric/datasets/deezer_europe.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/dgraph.py` & `torch_geometric-2.3.1/torch_geometric/datasets/dgraph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/dynamic_faust.py` & `torch_geometric-2.3.1/torch_geometric/datasets/dynamic_faust.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/elliptic.py` & `torch_geometric-2.3.1/torch_geometric/datasets/elliptic.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/email_eu_core.py` & `torch_geometric-2.3.1/torch_geometric/datasets/email_eu_core.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/entities.py` & `torch_geometric-2.3.1/torch_geometric/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/explainer_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/explainer_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/facebook.py` & `torch_geometric-2.3.1/torch_geometric/datasets/facebook.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/fake.py` & `torch_geometric-2.3.1/torch_geometric/datasets/fake.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/faust.py` & `torch_geometric-2.3.1/torch_geometric/datasets/faust.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/flickr.py` & `torch_geometric-2.3.1/torch_geometric/datasets/flickr.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/freebase.py` & `torch_geometric-2.3.1/torch_geometric/datasets/freebase.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/gdelt.py` & `torch_geometric-2.3.1/torch_geometric/datasets/gdelt.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/ged_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/ged_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/gemsec.py` & `torch_geometric-2.3.1/torch_geometric/datasets/gemsec.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/geometry.py` & `torch_geometric-2.3.1/torch_geometric/datasets/geometry.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/github.py` & `torch_geometric-2.3.1/torch_geometric/datasets/github.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/gnn_benchmark_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/gnn_benchmark_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/graph_generator/ba_graph.py` & `torch_geometric-2.3.1/torch_geometric/datasets/graph_generator/ba_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/graph_generator/base.py` & `torch_geometric-2.3.1/torch_geometric/datasets/graph_generator/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/graph_generator/er_graph.py` & `torch_geometric-2.3.1/torch_geometric/datasets/graph_generator/er_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/graph_generator/grid_graph.py` & `torch_geometric-2.3.1/torch_geometric/datasets/graph_generator/grid_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/heterophilous_graph_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/heterophilous_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/hgb_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/hgb_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/hydro_net.py` & `torch_geometric-2.3.1/torch_geometric/datasets/hydro_net.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/icews.py` & `torch_geometric-2.3.1/torch_geometric/datasets/icews.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/imdb.py` & `torch_geometric-2.3.1/torch_geometric/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/infection_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/infection_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/jodie.py` & `torch_geometric-2.3.1/torch_geometric/datasets/jodie.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/karate.py` & `torch_geometric-2.3.1/torch_geometric/datasets/karate.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/last_fm.py` & `torch_geometric-2.3.1/torch_geometric/datasets/last_fm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/lastfm_asia.py` & `torch_geometric-2.3.1/torch_geometric/datasets/lastfm_asia.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/linkx_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/linkx_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/lrgb.py` & `torch_geometric-2.3.1/torch_geometric/datasets/lrgb.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/malnet_tiny.py` & `torch_geometric-2.3.1/torch_geometric/datasets/malnet_tiny.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/md17.py` & `torch_geometric-2.3.1/torch_geometric/datasets/md17.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/mixhop_synthetic_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/mixhop_synthetic_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/mnist_superpixels.py` & `torch_geometric-2.3.1/torch_geometric/datasets/mnist_superpixels.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/modelnet.py` & `torch_geometric-2.3.1/torch_geometric/datasets/modelnet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/molecule_net.py` & `torch_geometric-2.3.1/torch_geometric/datasets/molecule_net.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/motif_generator/base.py` & `torch_geometric-2.3.1/torch_geometric/datasets/motif_generator/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/motif_generator/custom.py` & `torch_geometric-2.3.1/torch_geometric/datasets/motif_generator/custom.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/motif_generator/cycle.py` & `torch_geometric-2.3.1/torch_geometric/datasets/motif_generator/cycle.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/motif_generator/house.py` & `torch_geometric-2.3.1/torch_geometric/datasets/motif_generator/house.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/movie_lens.py` & `torch_geometric-2.3.1/torch_geometric/datasets/movie_lens.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/nell.py` & `torch_geometric-2.3.1/torch_geometric/datasets/nell.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/ogb_mag.py` & `torch_geometric-2.3.1/torch_geometric/datasets/ogb_mag.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/omdb.py` & `torch_geometric-2.3.1/torch_geometric/datasets/omdb.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/particle.py` & `torch_geometric-2.3.1/torch_geometric/datasets/particle.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/pascal.py` & `torch_geometric-2.3.1/torch_geometric/datasets/pascal.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/pascal_pf.py` & `torch_geometric-2.3.1/torch_geometric/datasets/pascal_pf.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/pcpnet_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/pcpnet_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/planetoid.py` & `torch_geometric-2.3.1/torch_geometric/datasets/planetoid.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/polblogs.py` & `torch_geometric-2.3.1/torch_geometric/datasets/polblogs.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/ppi.py` & `torch_geometric-2.3.1/torch_geometric/datasets/ppi.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/qm7.py` & `torch_geometric-2.3.1/torch_geometric/datasets/qm7.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/qm9.py` & `torch_geometric-2.3.1/torch_geometric/datasets/qm9.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/reddit.py` & `torch_geometric-2.3.1/torch_geometric/datasets/reddit.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/reddit2.py` & `torch_geometric-2.3.1/torch_geometric/datasets/reddit2.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/rel_link_pred_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/rel_link_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/s3dis.py` & `torch_geometric-2.3.1/torch_geometric/datasets/s3dis.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/sbm_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/sbm_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/shapenet.py` & `torch_geometric-2.3.1/torch_geometric/datasets/shapenet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/shrec2016.py` & `torch_geometric-2.3.1/torch_geometric/datasets/shrec2016.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/snap_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/snap_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/suite_sparse.py` & `torch_geometric-2.3.1/torch_geometric/datasets/suite_sparse.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/taobao.py` & `torch_geometric-2.3.1/torch_geometric/datasets/taobao.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/tosca.py` & `torch_geometric-2.3.1/torch_geometric/datasets/tosca.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/tu_dataset.py` & `torch_geometric-2.3.1/torch_geometric/datasets/tu_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/twitch.py` & `torch_geometric-2.3.1/torch_geometric/datasets/twitch.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/upfd.py` & `torch_geometric-2.3.1/torch_geometric/datasets/upfd.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/utils/cheatsheet.py` & `torch_geometric-2.3.1/torch_geometric/datasets/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/webkb.py` & `torch_geometric-2.3.1/torch_geometric/datasets/webkb.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/wikics.py` & `torch_geometric-2.3.1/torch_geometric/datasets/wikics.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/wikipedia_network.py` & `torch_geometric-2.3.1/torch_geometric/datasets/wikipedia_network.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/willow_object_class.py` & `torch_geometric-2.3.1/torch_geometric/datasets/willow_object_class.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/word_net.py` & `torch_geometric-2.3.1/torch_geometric/datasets/word_net.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/yelp.py` & `torch_geometric-2.3.1/torch_geometric/datasets/yelp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/datasets/zinc.py` & `torch_geometric-2.3.1/torch_geometric/datasets/zinc.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/debug.py` & `torch_geometric-2.3.1/torch_geometric/debug.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/deprecation.py` & `torch_geometric-2.3.1/torch_geometric/deprecation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/experimental.py` & `torch_geometric-2.3.1/torch_geometric/experimental.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/algorithm/attention_explainer.py` & `torch_geometric-2.3.1/torch_geometric/explain/algorithm/attention_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/algorithm/base.py` & `torch_geometric-2.3.1/torch_geometric/explain/algorithm/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/algorithm/captum.py` & `torch_geometric-2.3.1/torch_geometric/explain/algorithm/captum.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/algorithm/captum_explainer.py` & `torch_geometric-2.3.1/torch_geometric/explain/algorithm/captum_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/algorithm/dummy_explainer.py` & `torch_geometric-2.3.1/torch_geometric/explain/algorithm/dummy_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/algorithm/gnn_explainer.py` & `torch_geometric-2.3.1/torch_geometric/explain/algorithm/gnn_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/algorithm/pg_explainer.py` & `torch_geometric-2.3.1/torch_geometric/explain/algorithm/pg_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/algorithm/utils.py` & `torch_geometric-2.3.1/torch_geometric/explain/algorithm/utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/config.py` & `torch_geometric-2.3.1/torch_geometric/explain/config.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/explainer.py` & `torch_geometric-2.3.1/torch_geometric/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/explanation.py` & `torch_geometric-2.3.1/torch_geometric/explain/explanation.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
         )
 
     def _apply_masks(
         self,
         node_mask_dict: Dict[NodeType, Tensor],
         edge_mask_dict: Dict[EdgeType, Tensor],
     ) -> 'HeteroExplanation':
-        out = copy.deepcopy(self)
+        out = copy.copy(self)
 
         for edge_type, edge_mask in edge_mask_dict.items():
             for key, value in self[edge_type].items():
                 if key == 'edge_index':
                     out[edge_type].edge_index = value[:, edge_mask]
                 elif self[edge_type].is_edge_attr(key):
                     out[edge_type][key] = value[edge_mask]
```

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/metric/basic.py` & `torch_geometric-2.3.1/torch_geometric/explain/metric/basic.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/metric/faithfulness.py` & `torch_geometric-2.3.1/torch_geometric/explain/metric/faithfulness.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/explain/metric/fidelity.py` & `torch_geometric-2.3.1/torch_geometric/explain/metric/fidelity.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/__init__.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/checkpoint.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/cmd_args.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/cmd_args.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/config.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/config.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/config_store.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/config_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/contrib/layer/generalconv.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/contrib/layer/generalconv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/loader.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/logger.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/logger.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/loss.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/loss.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/model_builder.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/model_builder.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/models/__init__.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/models/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/models/act.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/models/act.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/models/encoder.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/models/encoder.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/models/gnn.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/models/gnn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/models/head.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/models/head.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/models/layer.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/models/layer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/models/transform.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/models/transform.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/optim.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/optim.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/register.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/register.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/train.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/train.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/utils/__init__.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/utils/agg_runs.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/utils/agg_runs.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/utils/comp_budget.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/utils/comp_budget.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/utils/device.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/utils/device.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/utils/epoch.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/utils/epoch.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/utils/io.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/utils/io.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/graphgym/utils/plot.py` & `torch_geometric-2.3.1/torch_geometric/graphgym/utils/plot.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/home.py` & `torch_geometric-2.3.1/torch_geometric/home.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/io/__init__.py` & `torch_geometric-2.3.1/torch_geometric/io/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/io/npz.py` & `torch_geometric-2.3.1/torch_geometric/io/npz.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/io/obj.py` & `torch_geometric-2.3.1/torch_geometric/io/obj.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/io/off.py` & `torch_geometric-2.3.1/torch_geometric/io/off.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/io/planetoid.py` & `torch_geometric-2.3.1/torch_geometric/io/planetoid.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         else:
             out = pickle.load(f)
 
     if name == 'graph':
         return out
 
     out = out.todense() if hasattr(out, 'todense') else out
-    out = torch.Tensor(out)
+    out = torch.from_numpy(out).to(torch.float)
     return out
 
 
 def edge_index_from_dict(graph_dict, num_nodes=None):
     row, col = [], []
     for key, value in graph_dict.items():
         row += repeat(key, len(value))
```

### Comparing `torch_geometric-2.3.0/torch_geometric/io/sdf.py` & `torch_geometric-2.3.1/torch_geometric/io/sdf.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/io/tu.py` & `torch_geometric-2.3.1/torch_geometric/io/tu.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/io/txt_array.py` & `torch_geometric-2.3.1/torch_geometric/io/txt_array.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/lazy_loader.py` & `torch_geometric-2.3.1/torch_geometric/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/__init__.py` & `torch_geometric-2.3.1/torch_geometric/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/base.py` & `torch_geometric-2.3.1/torch_geometric/loader/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/cluster.py` & `torch_geometric-2.3.1/torch_geometric/loader/cluster.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/data_list_loader.py` & `torch_geometric-2.3.1/torch_geometric/loader/data_list_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/dataloader.py` & `torch_geometric-2.3.1/torch_geometric/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/dense_data_loader.py` & `torch_geometric-2.3.1/torch_geometric/loader/dense_data_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/dynamic_batch_sampler.py` & `torch_geometric-2.3.1/torch_geometric/loader/dynamic_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/graph_saint.py` & `torch_geometric-2.3.1/torch_geometric/loader/graph_saint.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/hgt_loader.py` & `torch_geometric-2.3.1/torch_geometric/loader/hgt_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/imbalanced_sampler.py` & `torch_geometric-2.3.1/torch_geometric/loader/imbalanced_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/link_loader.py` & `torch_geometric-2.3.1/torch_geometric/loader/link_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/link_neighbor_loader.py` & `torch_geometric-2.3.1/torch_geometric/loader/link_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/mixin.py` & `torch_geometric-2.3.1/torch_geometric/loader/mixin.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/neighbor_loader.py` & `torch_geometric-2.3.1/torch_geometric/loader/neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/neighbor_sampler.py` & `torch_geometric-2.3.1/torch_geometric/loader/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/node_loader.py` & `torch_geometric-2.3.1/torch_geometric/loader/node_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/random_node_loader.py` & `torch_geometric-2.3.1/torch_geometric/loader/random_node_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/shadow.py` & `torch_geometric-2.3.1/torch_geometric/loader/shadow.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/temporal_dataloader.py` & `torch_geometric-2.3.1/torch_geometric/loader/temporal_dataloader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/utils.py` & `torch_geometric-2.3.1/torch_geometric/loader/utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/loader/zip_loader.py` & `torch_geometric-2.3.1/torch_geometric/loader/zip_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/logging.py` & `torch_geometric-2.3.1/torch_geometric/logging.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/__init__.py` & `torch_geometric-2.3.1/torch_geometric/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/__init__.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/attention.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/attention.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/base.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/basic.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/basic.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/deep_sets.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/deep_sets.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/equilibrium.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/equilibrium.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/fused.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/fused.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/gmt.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/gmt.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/gru.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/gru.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/lstm.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/lstm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/mlp.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/mlp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/multi.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/multi.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/quantile.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/quantile.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/scaler.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/scaler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/set2set.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/set2set.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/set_transformer.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/set_transformer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/sort.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/sort.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/aggr/utils.py` & `torch_geometric-2.3.1/torch_geometric/nn/aggr/utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/__init__.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/agnn_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/agnn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/antisymmetric_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/antisymmetric_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/appnp.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/appnp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/arma_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/arma_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/cg_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/cg_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/cheb_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/cheb_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/cluster_gcn_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/cluster_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/cugraph/base.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/cugraph/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,34 +4,45 @@
 import torch
 from torch import Tensor
 
 from torch_geometric.utils import index_sort
 from torch_geometric.utils.sparse import index2ptr
 
 try:  # pragma: no cover
-    from pylibcugraphops import (
-        make_fg_csr,
-        make_fg_csr_hg,
-        make_mfg_csr,
-        make_mfg_csr_hg,
+    LEGACY_MODE = False
+    from pylibcugraphops.pytorch import (
+        SampledCSC,
+        SampledHeteroCSC,
+        StaticCSC,
+        StaticHeteroCSC,
     )
     HAS_PYLIBCUGRAPHOPS = True
 except ImportError:
     HAS_PYLIBCUGRAPHOPS = False
+    try:  # pragma: no cover
+        from pylibcugraphops import (
+            make_fg_csr,
+            make_fg_csr_hg,
+            make_mfg_csr,
+            make_mfg_csr_hg,
+        )
+        LEGACY_MODE = True
+    except ImportError:
+        pass
 
 
 class CuGraphModule(torch.nn.Module):  # pragma: no cover
     r"""An abstract base class for implementing cugraph message passing layers.
     """
     def __init__(self):
         super().__init__()
 
-        if HAS_PYLIBCUGRAPHOPS is False:
+        if not HAS_PYLIBCUGRAPHOPS and not LEGACY_MODE:
             raise ModuleNotFoundError(f"'{self.__class__.__name__}' requires "
-                                      f"'pylibcugraphops'")
+                                      f"'pylibcugraphops>=23.02'")
 
     def reset_parameters(self):
         r"""Resets all learnable parameters of the module."""
         pass
 
     @staticmethod
     def to_csc(
@@ -95,20 +106,25 @@
             raise RuntimeError(f"'{self.__class__.__name__}' requires GPU-"
                                f"based processing (got CPU tensor)")
 
         if num_src_nodes != colptr.numel() - 1:  # Bipartite graph:
             if max_num_neighbors is None:
                 max_num_neighbors = int((colptr[1:] - colptr[:-1]).max())
 
-            dst_nodes = torch.arange(colptr.numel() - 1, device=row.device)
+            if LEGACY_MODE:
+                dst_nodes = torch.arange(colptr.numel() - 1, device=row.device)
+                return make_mfg_csr(dst_nodes, colptr, row, max_num_neighbors,
+                                    num_src_nodes)
+
+            return SampledCSC(colptr, row, max_num_neighbors, num_src_nodes)
 
-            return make_mfg_csr(dst_nodes, colptr, row, max_num_neighbors,
-                                num_src_nodes)
+        if LEGACY_MODE:
+            return make_fg_csr(colptr, row)
 
-        return make_fg_csr(colptr, row)
+        return StaticCSC(colptr, row)
 
     def get_typed_cugraph(
         self,
         csc: Tuple[Tensor, Tensor, int],
         edge_type: Tensor,
         num_edge_types: Optional[int] = None,
         max_num_neighbors: Optional[int] = None,
@@ -138,25 +154,32 @@
         row, colptr, num_src_nodes = csc
         edge_type = edge_type.int()
 
         if num_src_nodes != colptr.numel() - 1:  # Bipartite graph:
             if max_num_neighbors is None:
                 max_num_neighbors = int((colptr[1:] - colptr[:-1]).max())
 
-            dst_nodes = torch.arange(colptr.numel() - 1, device=row.device)
+            if LEGACY_MODE:
+                dst_nodes = torch.arange(colptr.numel() - 1, device=row.device)
+                return make_mfg_csr_hg(dst_nodes, colptr, row,
+                                       max_num_neighbors, num_src_nodes,
+                                       n_node_types=0,
+                                       n_edge_types=num_edge_types,
+                                       out_node_types=None, in_node_types=None,
+                                       edge_types=edge_type)
+
+            return SampledHeteroCSC(colptr, row, edge_type, max_num_neighbors,
+                                    num_src_nodes, num_edge_types)
+
+        if LEGACY_MODE:
+            return make_fg_csr_hg(colptr, row, n_node_types=0,
+                                  n_edge_types=num_edge_types, node_types=None,
+                                  edge_types=edge_type)
 
-            return make_mfg_csr_hg(dst_nodes, colptr, row, max_num_neighbors,
-                                   num_src_nodes, n_node_types=0,
-                                   n_edge_types=num_edge_types,
-                                   out_node_types=None, in_node_types=None,
-                                   edge_types=edge_type)
-
-        return make_fg_csr_hg(colptr, row, n_node_types=0,
-                              n_edge_types=num_edge_types, node_types=None,
-                              edge_types=edge_type)
+        return StaticHeteroCSC(colptr, row, edge_type, num_edge_types)
 
     def forward(
         self,
         x: Tensor,
         csc: Tuple[Tensor, Tensor, int],
         max_num_neighbors: Optional[int] = None,
     ) -> Tensor:
```

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/cugraph/gat_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/cugraph/gat_conv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from typing import Optional, Tuple
 
 import torch
 from torch import Tensor
 from torch.nn import Linear, Parameter
 
 from torch_geometric.nn.conv.cugraph import CuGraphModule
+from torch_geometric.nn.conv.cugraph.base import LEGACY_MODE
 from torch_geometric.nn.inits import zeros
 
 try:
-    from pylibcugraphops.torch.autograd import mha_gat_n2n as GATConvAgg
+    if LEGACY_MODE:
+        from pylibcugraphops.torch.autograd import mha_gat_n2n as GATConvAgg
+    else:
+        from pylibcugraphops.pytorch.operators import mha_gat_n2n as GATConvAgg
 except ImportError:
     pass
 
 
 class CuGraphGATConv(CuGraphModule):  # pragma: no cover
     r"""The graph attentional operator from the `"Graph Attention Networks"
     <https://arxiv.org/abs/1710.10903>`_ paper.
@@ -63,16 +67,21 @@
         x: Tensor,
         csc: Tuple[Tensor, Tensor, int],
         max_num_neighbors: Optional[int] = None,
     ) -> Tensor:
         graph = self.get_cugraph(csc, max_num_neighbors)
 
         x = self.lin(x)
-        out = GATConvAgg(x, self.att, graph, self.heads, 'LeakyReLU',
-                         self.negative_slope, False, self.concat)
+
+        if LEGACY_MODE:
+            out = GATConvAgg(x, self.att, graph, self.heads, 'LeakyReLU',
+                             self.negative_slope, False, self.concat)
+        else:
+            out = GATConvAgg(x, self.att, graph, self.heads, 'LeakyReLU',
+                             self.negative_slope, self.concat)
 
         if self.bias is not None:
             out = out + self.bias
 
         return out
 
     def __repr__(self) -> str:
```

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/cugraph/rgcn_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/cugraph/rgcn_conv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from typing import Optional, Tuple
 
 import torch
 from torch import Tensor
 from torch.nn import Parameter
 
 from torch_geometric.nn.conv.cugraph import CuGraphModule
+from torch_geometric.nn.conv.cugraph.base import LEGACY_MODE
 from torch_geometric.nn.inits import glorot, zeros
 
 try:
-    from pylibcugraphops.torch.autograd import \
-        agg_hg_basis_n2n_post as RGCNConvAgg
+    if LEGACY_MODE:
+        from pylibcugraphops.torch.autograd import \
+            agg_hg_basis_n2n_post as RGCNConvAgg
+    else:
+        from pylibcugraphops.pytorch.operators import \
+            agg_hg_basis_n2n_post as RGCNConvAgg
 except ImportError:
     pass
 
 
 class CuGraphRGCNConv(CuGraphModule):  # pragma: no cover
     r"""The relational graph convolutional operator from the `"Modeling
     Relational Data with Graph Convolutional Networks"
```

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/cugraph/sage_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/cugraph/sage_conv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from typing import Optional, Tuple
 
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn import Linear
 
 from torch_geometric.nn.conv.cugraph import CuGraphModule
+from torch_geometric.nn.conv.cugraph.base import LEGACY_MODE
 
 try:
-    from pylibcugraphops.torch.autograd import agg_concat_n2n as SAGEConvAgg
+    if LEGACY_MODE:
+        from pylibcugraphops.torch.autograd import \
+            agg_concat_n2n as SAGEConvAgg
+    else:
+        from pylibcugraphops.pytorch.operators import \
+            agg_concat_n2n as SAGEConvAgg
 except ImportError:
     pass
 
 
 class CuGraphSAGEConv(CuGraphModule):  # pragma: no cover
     r"""The GraphSAGE operator from the `"Inductive Representation Learning on
     Large Graphs" <https://arxiv.org/abs/1706.02216>`_ paper.
```

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/dna_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/dna_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/edge_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/edge_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/eg_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/eg_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/fa_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/fa_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/fast_hgt_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/fast_hgt_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                 type_list.append(torch.full((N, ), count, dtype=torch.long))
                 count += 1
             offset[edge_type] = cumsum
             cumsum += N
 
         type_vec = torch.cat(type_list, dim=0)
         k = self.k_rel(torch.cat(ks, dim=0), type_vec).view(-1, H, D)
-        v = self.k_rel(torch.cat(vs, dim=0), type_vec).view(-1, H, D)
+        v = self.v_rel(torch.cat(vs, dim=0), type_vec).view(-1, H, D)
 
         return k, v, offset
 
     def _construct_edge_index(
         self,
         edge_index_dict: Dict[EdgeType, Adj],
         src_offset: Dict[EdgeType, int],
```

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/feast_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/feast_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/film_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/film_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/fused_gat_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/fused_gat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/gat_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/gat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/gated_graph_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/gatv2_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/gcn2_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/gcn2_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/gcn_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/gen_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/gen_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/general_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/general_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/gin_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/gin_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/gmm_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/gps_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/gps_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/graph_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/graph_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/gravnet_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/gravnet_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/han_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/han_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/heat_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/heat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/hetero_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/hetero_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/hgt_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/hgt_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/hypergraph_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/hypergraph_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/le_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/le_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/lg_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/lg_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/message_passing.jinja` & `torch_geometric-2.3.1/torch_geometric/nn/conv/message_passing.jinja`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/message_passing.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/message_passing.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/mf_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/mf_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/nn_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/nn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/pan_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/pan_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/pdn_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/pdn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/pna_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/pna_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/point_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/point_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/point_gnn_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/point_gnn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/point_transformer_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/point_transformer_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/ppf_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/ppf_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/res_gated_graph_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/res_gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/rgat_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/rgat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/rgcn_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/sage_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/sage_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/sg_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/sg_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/signed_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/signed_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/simple_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/simple_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/spline_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/spline_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/ssg_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/ssg_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/supergat_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/supergat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/tag_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/tag_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/transformer_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/transformer_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/utils/__init__.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/utils/cheatsheet.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/utils/inspector.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/utils/inspector.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/utils/jit.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/utils/jit.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/utils/typing.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/utils/typing.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/wl_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/wl_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/wl_conv_continuous.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/wl_conv_continuous.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/conv/x_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/conv/x_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/data_parallel.py` & `torch_geometric-2.3.1/torch_geometric/nn/data_parallel.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/dense/__init__.py` & `torch_geometric-2.3.1/torch_geometric/nn/dense/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/dense/dense_gat_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/dense/dense_gat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/dense/dense_gcn_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/dense/dense_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/dense/dense_gin_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/dense/dense_gin_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/dense/dense_graph_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/dense/dense_graph_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/dense/dense_sage_conv.py` & `torch_geometric-2.3.1/torch_geometric/nn/dense/dense_sage_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/dense/diff_pool.py` & `torch_geometric-2.3.1/torch_geometric/nn/dense/diff_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/dense/dmon_pool.py` & `torch_geometric-2.3.1/torch_geometric/nn/dense/dmon_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/dense/linear.py` & `torch_geometric-2.3.1/torch_geometric/nn/dense/linear.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/dense/mincut_pool.py` & `torch_geometric-2.3.1/torch_geometric/nn/dense/mincut_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/encoding.py` & `torch_geometric-2.3.1/torch_geometric/nn/encoding.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/functional/bro.py` & `torch_geometric-2.3.1/torch_geometric/nn/functional/bro.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/functional/gini.py` & `torch_geometric-2.3.1/torch_geometric/nn/functional/gini.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/fx.py` & `torch_geometric-2.3.1/torch_geometric/nn/fx.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/glob.py` & `torch_geometric-2.3.1/torch_geometric/nn/glob.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/inits.py` & `torch_geometric-2.3.1/torch_geometric/nn/inits.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/kge/base.py` & `torch_geometric-2.3.1/torch_geometric/nn/kge/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/kge/complex.py` & `torch_geometric-2.3.1/torch_geometric/nn/kge/complex.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/kge/distmult.py` & `torch_geometric-2.3.1/torch_geometric/nn/kge/distmult.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/kge/loader.py` & `torch_geometric-2.3.1/torch_geometric/nn/kge/loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/kge/transe.py` & `torch_geometric-2.3.1/torch_geometric/nn/kge/transe.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/lr_scheduler.py` & `torch_geometric-2.3.1/torch_geometric/nn/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/model_hub.py` & `torch_geometric-2.3.1/torch_geometric/nn/model_hub.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/__init__.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/attentive_fp.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/attentive_fp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/autoencoder.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/basic_gnn.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/basic_gnn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/captum.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/captum.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/correct_and_smooth.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/correct_and_smooth.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/deep_graph_infomax.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/deep_graph_infomax.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/deepgcn.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/deepgcn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/dimenet.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/dimenet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/dimenet_utils.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/dimenet_utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/gnnff.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/gnnff.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/graph_unet.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/graph_unet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/jumping_knowledge.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/jumping_knowledge.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/label_prop.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/label_prop.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/lightgcn.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/lightgcn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/linkx.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/linkx.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/mask_label.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/mask_label.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/meta.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/meta.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/metapath2vec.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/metapath2vec.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/mlp.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/mlp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/node2vec.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/node2vec.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/re_net.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/re_net.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/rect.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/rect.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/rev_gnn.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/rev_gnn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/schnet.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/schnet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/signed_gcn.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/signed_gcn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/models/tgn.py` & `torch_geometric-2.3.1/torch_geometric/nn/models/tgn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/module_dict.py` & `torch_geometric-2.3.1/torch_geometric/nn/module_dict.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/norm/__init__.py` & `torch_geometric-2.3.1/torch_geometric/nn/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/norm/batch_norm.py` & `torch_geometric-2.3.1/torch_geometric/nn/norm/batch_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/norm/diff_group_norm.py` & `torch_geometric-2.3.1/torch_geometric/nn/norm/diff_group_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/norm/graph_norm.py` & `torch_geometric-2.3.1/torch_geometric/nn/norm/graph_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/norm/graph_size_norm.py` & `torch_geometric-2.3.1/torch_geometric/nn/norm/graph_size_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/norm/instance_norm.py` & `torch_geometric-2.3.1/torch_geometric/nn/norm/instance_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/norm/layer_norm.py` & `torch_geometric-2.3.1/torch_geometric/nn/norm/layer_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/norm/mean_subtraction_norm.py` & `torch_geometric-2.3.1/torch_geometric/nn/norm/mean_subtraction_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/norm/msg_norm.py` & `torch_geometric-2.3.1/torch_geometric/nn/norm/msg_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/norm/pair_norm.py` & `torch_geometric-2.3.1/torch_geometric/nn/norm/pair_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/parameter_dict.py` & `torch_geometric-2.3.1/torch_geometric/nn/parameter_dict.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/__init__.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/asap.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/asap.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/avg_pool.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/avg_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/base.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/connect/base.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/connect/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/decimation.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/decimation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/edge_pool.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/edge_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/glob.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/glob.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/graclus.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/graclus.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/max_pool.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/max_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/mem_pool.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/mem_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/pan_pool.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/pan_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/pool.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/sag_pool.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/sag_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/select/base.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/select/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/topk_pool.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/topk_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/pool/voxel_grid.py` & `torch_geometric-2.3.1/torch_geometric/nn/pool/voxel_grid.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/resolver.py` & `torch_geometric-2.3.1/torch_geometric/nn/resolver.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/sequential.jinja` & `torch_geometric-2.3.1/torch_geometric/nn/sequential.jinja`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/sequential.py` & `torch_geometric-2.3.1/torch_geometric/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/summary.py` & `torch_geometric-2.3.1/torch_geometric/nn/summary.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/to_fixed_size_transformer.py` & `torch_geometric-2.3.1/torch_geometric/nn/to_fixed_size_transformer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/to_hetero_module.py` & `torch_geometric-2.3.1/torch_geometric/nn/to_hetero_module.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/to_hetero_transformer.py` & `torch_geometric-2.3.1/torch_geometric/nn/to_hetero_transformer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/to_hetero_with_bases_transformer.py` & `torch_geometric-2.3.1/torch_geometric/nn/to_hetero_with_bases_transformer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/nn/unpool/knn_interpolate.py` & `torch_geometric-2.3.1/torch_geometric/nn/unpool/knn_interpolate.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/profile/__init__.py` & `torch_geometric-2.3.1/torch_geometric/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/profile/benchmark.py` & `torch_geometric-2.3.1/torch_geometric/profile/benchmark.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/profile/profile.py` & `torch_geometric-2.3.1/torch_geometric/profile/profile.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/profile/profiler.py` & `torch_geometric-2.3.1/torch_geometric/profile/profiler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/profile/utils.py` & `torch_geometric-2.3.1/torch_geometric/profile/utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/resolver.py` & `torch_geometric-2.3.1/torch_geometric/resolver.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/sampler/base.py` & `torch_geometric-2.3.1/torch_geometric/sampler/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/sampler/hgt_sampler.py` & `torch_geometric-2.3.1/torch_geometric/sampler/hgt_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/sampler/neighbor_sampler.py` & `torch_geometric-2.3.1/torch_geometric/sampler/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/sampler/utils.py` & `torch_geometric-2.3.1/torch_geometric/sampler/utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/testing/__init__.py` & `torch_geometric-2.3.1/torch_geometric/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/testing/data.py` & `torch_geometric-2.3.1/torch_geometric/testing/data.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/testing/decorators.py` & `torch_geometric-2.3.1/torch_geometric/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/testing/feature_store.py` & `torch_geometric-2.3.1/torch_geometric/testing/feature_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/testing/graph_store.py` & `torch_geometric-2.3.1/torch_geometric/testing/graph_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/__init__.py` & `torch_geometric-2.3.1/torch_geometric/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/add_metapaths.py` & `torch_geometric-2.3.1/torch_geometric/transforms/add_metapaths.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/add_positional_encoding.py` & `torch_geometric-2.3.1/torch_geometric/transforms/add_positional_encoding.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/add_self_loops.py` & `torch_geometric-2.3.1/torch_geometric/transforms/add_self_loops.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/base_transform.py` & `torch_geometric-2.3.1/torch_geometric/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/cartesian.py` & `torch_geometric-2.3.1/torch_geometric/transforms/cartesian.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/center.py` & `torch_geometric-2.3.1/torch_geometric/transforms/center.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/compose.py` & `torch_geometric-2.3.1/torch_geometric/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/constant.py` & `torch_geometric-2.3.1/torch_geometric/transforms/constant.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/delaunay.py` & `torch_geometric-2.3.1/torch_geometric/transforms/delaunay.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/distance.py` & `torch_geometric-2.3.1/torch_geometric/transforms/distance.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/face_to_edge.py` & `torch_geometric-2.3.1/torch_geometric/transforms/face_to_edge.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/feature_propagation.py` & `torch_geometric-2.3.1/torch_geometric/transforms/feature_propagation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/fixed_points.py` & `torch_geometric-2.3.1/torch_geometric/transforms/fixed_points.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/gcn_norm.py` & `torch_geometric-2.3.1/torch_geometric/transforms/gcn_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/gdc.py` & `torch_geometric-2.3.1/torch_geometric/transforms/gdc.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/generate_mesh_normals.py` & `torch_geometric-2.3.1/torch_geometric/transforms/generate_mesh_normals.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/grid_sampling.py` & `torch_geometric-2.3.1/torch_geometric/transforms/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/knn_graph.py` & `torch_geometric-2.3.1/torch_geometric/transforms/knn_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/laplacian_lambda_max.py` & `torch_geometric-2.3.1/torch_geometric/transforms/laplacian_lambda_max.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/largest_connected_components.py` & `torch_geometric-2.3.1/torch_geometric/transforms/largest_connected_components.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/line_graph.py` & `torch_geometric-2.3.1/torch_geometric/transforms/line_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/linear_transformation.py` & `torch_geometric-2.3.1/torch_geometric/transforms/linear_transformation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/local_cartesian.py` & `torch_geometric-2.3.1/torch_geometric/transforms/local_cartesian.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/local_degree_profile.py` & `torch_geometric-2.3.1/torch_geometric/transforms/local_degree_profile.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/mask.py` & `torch_geometric-2.3.1/torch_geometric/transforms/mask.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/normalize_features.py` & `torch_geometric-2.3.1/torch_geometric/transforms/normalize_features.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/normalize_rotation.py` & `torch_geometric-2.3.1/torch_geometric/transforms/normalize_rotation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/normalize_scale.py` & `torch_geometric-2.3.1/torch_geometric/transforms/normalize_scale.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/one_hot_degree.py` & `torch_geometric-2.3.1/torch_geometric/transforms/one_hot_degree.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/pad.py` & `torch_geometric-2.3.1/torch_geometric/transforms/pad.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/point_pair_features.py` & `torch_geometric-2.3.1/torch_geometric/transforms/point_pair_features.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/polar.py` & `torch_geometric-2.3.1/torch_geometric/transforms/polar.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/radius_graph.py` & `torch_geometric-2.3.1/torch_geometric/transforms/radius_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/random_flip.py` & `torch_geometric-2.3.1/torch_geometric/transforms/random_flip.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/random_jitter.py` & `torch_geometric-2.3.1/torch_geometric/transforms/random_jitter.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/random_link_split.py` & `torch_geometric-2.3.1/torch_geometric/transforms/random_link_split.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/random_node_split.py` & `torch_geometric-2.3.1/torch_geometric/transforms/random_node_split.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/random_rotate.py` & `torch_geometric-2.3.1/torch_geometric/transforms/random_rotate.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/random_scale.py` & `torch_geometric-2.3.1/torch_geometric/transforms/random_scale.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/random_shear.py` & `torch_geometric-2.3.1/torch_geometric/transforms/random_shear.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/remove_duplicated_edges.py` & `torch_geometric-2.3.1/torch_geometric/transforms/remove_duplicated_edges.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/remove_isolated_nodes.py` & `torch_geometric-2.3.1/torch_geometric/transforms/remove_isolated_nodes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/remove_training_classes.py` & `torch_geometric-2.3.1/torch_geometric/transforms/remove_training_classes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/rooted_subgraph.py` & `torch_geometric-2.3.1/torch_geometric/transforms/rooted_subgraph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/sample_points.py` & `torch_geometric-2.3.1/torch_geometric/transforms/sample_points.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/sign.py` & `torch_geometric-2.3.1/torch_geometric/transforms/sign.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/spherical.py` & `torch_geometric-2.3.1/torch_geometric/transforms/spherical.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/svd_feature_reduction.py` & `torch_geometric-2.3.1/torch_geometric/transforms/svd_feature_reduction.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/target_indegree.py` & `torch_geometric-2.3.1/torch_geometric/transforms/target_indegree.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/to_dense.py` & `torch_geometric-2.3.1/torch_geometric/transforms/to_dense.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/to_device.py` & `torch_geometric-2.3.1/torch_geometric/transforms/to_device.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/to_sparse_tensor.py` & `torch_geometric-2.3.1/torch_geometric/transforms/to_sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/to_superpixels.py` & `torch_geometric-2.3.1/torch_geometric/transforms/to_superpixels.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/to_undirected.py` & `torch_geometric-2.3.1/torch_geometric/transforms/to_undirected.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/two_hop.py` & `torch_geometric-2.3.1/torch_geometric/transforms/two_hop.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/transforms/virtual_node.py` & `torch_geometric-2.3.1/torch_geometric/transforms/virtual_node.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/typing.py` & `torch_geometric-2.3.1/torch_geometric/typing.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/__init__.py` & `torch_geometric-2.3.1/torch_geometric/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/assortativity.py` & `torch_geometric-2.3.1/torch_geometric/utils/assortativity.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/augmentation.py` & `torch_geometric-2.3.1/torch_geometric/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/coalesce.py` & `torch_geometric-2.3.1/torch_geometric/utils/coalesce.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/convert.py` & `torch_geometric-2.3.1/torch_geometric/utils/convert.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/degree.py` & `torch_geometric-2.3.1/torch_geometric/utils/degree.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/dropout.py` & `torch_geometric-2.3.1/torch_geometric/utils/dropout.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/embedding.py` & `torch_geometric-2.3.1/torch_geometric/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/geodesic.py` & `torch_geometric-2.3.1/torch_geometric/utils/geodesic.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/get_laplacian.py` & `torch_geometric-2.3.1/torch_geometric/utils/get_laplacian.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/get_mesh_laplacian.py` & `torch_geometric-2.3.1/torch_geometric/utils/get_mesh_laplacian.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/grid.py` & `torch_geometric-2.3.1/torch_geometric/utils/grid.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/hetero.py` & `torch_geometric-2.3.1/torch_geometric/utils/hetero.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/homophily.py` & `torch_geometric-2.3.1/torch_geometric/utils/homophily.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/isolated.py` & `torch_geometric-2.3.1/torch_geometric/utils/isolated.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/loop.py` & `torch_geometric-2.3.1/torch_geometric/utils/loop.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/mask.py` & `torch_geometric-2.3.1/torch_geometric/utils/mask.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/mixin.py` & `torch_geometric-2.3.1/torch_geometric/utils/mixin.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/negative_sampling.py` & `torch_geometric-2.3.1/torch_geometric/utils/negative_sampling.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/nested.py` & `torch_geometric-2.3.1/torch_geometric/utils/nested.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/normalized_cut.py` & `torch_geometric-2.3.1/torch_geometric/utils/normalized_cut.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/num_nodes.py` & `torch_geometric-2.3.1/torch_geometric/utils/num_nodes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/one_hot.py` & `torch_geometric-2.3.1/torch_geometric/utils/one_hot.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/random.py` & `torch_geometric-2.3.1/torch_geometric/utils/random.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/scatter.py` & `torch_geometric-2.3.1/torch_geometric/utils/scatter.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/segment.py` & `torch_geometric-2.3.1/torch_geometric/utils/segment.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/select.py` & `torch_geometric-2.3.1/torch_geometric/utils/select.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/smiles.py` & `torch_geometric-2.3.1/torch_geometric/utils/smiles.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/softmax.py` & `torch_geometric-2.3.1/torch_geometric/utils/softmax.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/sort.py` & `torch_geometric-2.3.1/torch_geometric/utils/sort.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/sort_edge_index.py` & `torch_geometric-2.3.1/torch_geometric/utils/sort_edge_index.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/sparse.py` & `torch_geometric-2.3.1/torch_geometric/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/spmm.py` & `torch_geometric-2.3.1/torch_geometric/utils/spmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
         elif src.layout == torch.sparse_csc:
             assert src.layout == torch.sparse_csc
             deg = scatter(torch.ones_like(src.values()), src.row_indices(),
                           dim=0, dim_size=src.size(0), reduce='sum')
         else:
             assert src.layout == torch.sparse_coo
             src = src.coalesce()
-            deg = scatter(torch.ones_like(src.values()), src.indices(), dim=0,
-                          dim_size=src.size(0), reduce='sum')
+            deg = scatter(torch.ones_like(src.values()),
+                          src.indices()[0], dim=0, dim_size=src.size(0),
+                          reduce='sum')
 
         return torch.sparse.mm(src, other) / deg.view(-1, 1).clamp_(min=1)
 
     raise ValueError(f"`{reduce}` reduction is not supported for "
                      f"'torch.sparse.Tensor' on device '{src.device}'")
```

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/subgraph.py` & `torch_geometric-2.3.1/torch_geometric/utils/subgraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,29 +83,29 @@
     """
 
     device = edge_index.device
 
     if isinstance(subset, (list, tuple)):
         subset = torch.tensor(subset, dtype=torch.long, device=device)
 
-    if subset.dtype == torch.bool or subset.dtype == torch.uint8:
-        num_nodes = subset.size(0)
-    else:
+    if subset.dtype != torch.bool:
         num_nodes = maybe_num_nodes(edge_index, num_nodes)
-        subset = index_to_mask(subset, size=num_nodes)
+        node_mask = index_to_mask(subset, size=num_nodes)
+    else:
+        num_nodes = subset.size(0)
+        node_mask = subset
 
-    node_mask = subset
     edge_mask = node_mask[edge_index[0]] & node_mask[edge_index[1]]
     edge_index = edge_index[:, edge_mask]
     edge_attr = edge_attr[edge_mask] if edge_attr is not None else None
 
     if relabel_nodes:
         node_idx = torch.zeros(node_mask.size(0), dtype=torch.long,
                                device=device)
-        node_idx[subset] = torch.arange(subset.sum().item(), device=device)
+        node_idx[subset] = torch.arange(node_mask.sum().item(), device=device)
         edge_index = node_idx[edge_index]
 
     if return_edge_mask:
         return edge_index, edge_attr, edge_mask
     else:
         return edge_index, edge_attr
 
@@ -164,30 +164,36 @@
     if not isinstance(src_subset, Tensor):
         src_subset = torch.tensor(src_subset, dtype=torch.long, device=device)
     if not isinstance(dst_subset, Tensor):
         dst_subset = torch.tensor(dst_subset, dtype=torch.long, device=device)
 
     if src_subset.dtype != torch.bool:
         src_size = int(edge_index[0].max()) + 1 if size is None else size[0]
-        src_subset = index_to_mask(src_subset, size=src_size)
+        src_node_mask = index_to_mask(src_subset, size=src_size)
+    else:
+        src_size = src_subset.size(0)
+        src_node_mask = src_subset
+
     if dst_subset.dtype != torch.bool:
         dst_size = int(edge_index[1].max()) + 1 if size is None else size[1]
-        dst_subset = index_to_mask(dst_subset, size=dst_size)
+        dst_node_mask = index_to_mask(dst_subset, size=dst_size)
+    else:
+        dst_size = dst_subset.size(0)
+        dst_node_mask = dst_subset
 
-    # node_mask = subset
-    edge_mask = src_subset[edge_index[0]] & dst_subset[edge_index[1]]
+    edge_mask = src_node_mask[edge_index[0]] & dst_node_mask[edge_index[1]]
     edge_index = edge_index[:, edge_mask]
     edge_attr = edge_attr[edge_mask] if edge_attr is not None else None
 
     if relabel_nodes:
-        node_idx_i = edge_index.new_zeros(src_subset.size(0))
-        node_idx_j = edge_index.new_zeros(dst_subset.size(0))
-        node_idx_i[src_subset] = torch.arange(int(src_subset.sum()),
+        node_idx_i = edge_index.new_zeros(src_node_mask.size(0))
+        node_idx_j = edge_index.new_zeros(dst_node_mask.size(0))
+        node_idx_i[src_subset] = torch.arange(int(src_node_mask.sum()),
                                               device=node_idx_i.device)
-        node_idx_j[dst_subset] = torch.arange(int(dst_subset.sum()),
+        node_idx_j[dst_subset] = torch.arange(int(dst_node_mask.sum()),
                                               device=node_idx_j.device)
         edge_index = torch.stack([
             node_idx_i[edge_index[0]],
             node_idx_j[edge_index[1]],
         ], dim=0)
 
     if return_edge_mask:
```

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/to_dense_adj.py` & `torch_geometric-2.3.1/torch_geometric/utils/to_dense_adj.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/to_dense_batch.py` & `torch_geometric-2.3.1/torch_geometric/utils/to_dense_batch.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/train_test_split_edges.py` & `torch_geometric-2.3.1/torch_geometric/utils/train_test_split_edges.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/tree_decomposition.py` & `torch_geometric-2.3.1/torch_geometric/utils/tree_decomposition.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/trim_to_layer.py` & `torch_geometric-2.3.1/torch_geometric/utils/trim_to_layer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/unbatch.py` & `torch_geometric-2.3.1/torch_geometric/utils/unbatch.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/utils/undirected.py` & `torch_geometric-2.3.1/torch_geometric/utils/undirected.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric/visualization/graph.py` & `torch_geometric-2.3.1/torch_geometric/visualization/graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.3.0/torch_geometric.egg-info/PKG-INFO` & `torch_geometric-2.3.1/torch_geometric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-geometric
-Version: 2.3.0
+Version: 2.3.1
 Summary: Graph Neural Network Library for PyTorch
 Author-email: Matthias Fey <matthias@pyg.org>
 Project-URL: homepage, https://pyg.org
 Project-URL: documentation, https://pytorch-geometric.readthedocs.io
 Project-URL: repository, https://github.com/pyg-team/pytorch_geometric.git
 Project-URL: changelog, https://github.com/pyg-team/pytorch_geometric/blob/master/CHANGELOG.md
 Keywords: deep-learning,pytorch,geometric-deep-learning,graph-neural-networks,graph-convolutional-networks
```

### Comparing `torch_geometric-2.3.0/torch_geometric.egg-info/requires.txt` & `torch_geometric-2.3.1/torch_geometric.egg-info/requires.txt`

 * *Files identical despite different names*


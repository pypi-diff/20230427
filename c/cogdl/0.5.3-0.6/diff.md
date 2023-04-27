# Comparing `tmp/cogdl-0.5.3.tar.gz` & `tmp/cogdl-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cogdl-0.5.3.tar", last modified: Wed Jun  1 12:05:57 2022, max compression
+gzip compressed data, was "cogdl-0.6.tar", last modified: Thu Apr 27 11:06:09 2023, max compression
```

## Comparing `cogdl-0.5.3.tar` & `cogdl-0.6.tar`

### file list

```diff
@@ -1,293 +1,326 @@
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1072 2022-01-21 12:30:57.000000 cogdl-0.5.3/LICENSE
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      140 2022-01-21 12:30:57.000000 cogdl-0.5.3/MANIFEST.in
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    13890 2022-06-01 12:05:57.000000 cogdl-0.5.3/PKG-INFO
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    13017 2022-06-01 12:04:33.000000 cogdl-0.5.3/README.md
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)       91 2022-06-01 12:04:33.000000 cogdl-0.5.3/cogdl/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)       29 2022-05-31 17:54:55.000000 cogdl-0.5.3/cogdl/backend.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    11781 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/configs.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/data/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      262 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/data/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4840 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/data/batch.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    32282 2022-06-01 11:02:18.000000 cogdl-0.5.3/cogdl/data/data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1990 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/data/dataloader.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     8502 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/data/dataset.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6774 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/data/sampler.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/datasets/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     7949 2022-06-01 11:02:18.000000 cogdl-0.5.3/cogdl/datasets/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4333 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/customized_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3164 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/gatne.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5919 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/gcc_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    13408 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/geom_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5547 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/gtn_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5899 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/han_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5789 2022-05-19 11:56:57.000000 cogdl-0.5.3/cogdl/datasets/kg_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5885 2022-05-19 11:56:57.000000 cogdl-0.5.3/cogdl/datasets/matlab_matrix.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2341 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/oagbert_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     8143 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/ogb.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6756 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/planetoid_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5519 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/rd2cd_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5969 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/rec_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     7155 2022-05-19 11:56:57.000000 cogdl-0.5.3/cogdl/datasets/saint_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    12362 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/datasets/tu_data.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    12626 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/experiments.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/layers/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1088 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1838 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/actgcn_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      941 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/actgcnii_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      734 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/actlinear_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2232 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/actmlp_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1883 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/actsage_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      544 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/base_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6376 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/deepergcn_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3653 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/disengcn_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2842 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/gat_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1838 2022-05-31 19:17:05.000000 cogdl-0.5.3/cogdl/layers/gcn_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      891 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/gcnii_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1189 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/gin_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1264 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/gine_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1008 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/han_layer.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/layers/jittor/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)       32 2022-06-01 06:16:58.000000 cogdl-0.5.3/cogdl/layers/jittor/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1698 2022-06-01 06:16:58.000000 cogdl-0.5.3/cogdl/layers/jittor/gcn_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1054 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/mixhop_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2215 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/mlp_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1860 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/pprgo_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    19678 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/reversible_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6064 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/rgcn_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2341 2022-05-31 13:54:42.000000 cogdl-0.5.3/cogdl/layers/sage_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4656 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/saint_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      740 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/se_layer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2271 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/set2set.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      503 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/layers/sgc_layer.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/loggers/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      379 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/loggers/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      206 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/loggers/base_logger.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      619 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/loggers/tensorboard_logger.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      701 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/loggers/wandb_logger.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/models/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4517 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      943 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/base_model.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/models/emb/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)        0 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4344 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/deepwalk.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4616 2022-05-19 11:56:57.000000 cogdl-0.5.3/cogdl/models/emb/dgk.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5977 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/dngr.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    16153 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/gatne.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4326 2022-05-19 11:56:57.000000 cogdl-0.5.3/cogdl/models/emb/graph2vec.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3123 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/grarep.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     8966 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/hin2vec.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2557 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/hope.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     7272 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/line.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5142 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/metapath2vec.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5088 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/netmf.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     7078 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/netsmf.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     7324 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/node2vec.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4295 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/prone.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     7427 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/pronepp.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6638 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/pte.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5688 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/sdne.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1642 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/emb/spectral.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/models/nn/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      708 2022-06-01 11:02:18.000000 cogdl-0.5.3/cogdl/models/nn/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2875 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/actgcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2739 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/agc.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     9014 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/autognn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    11729 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/compgcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6675 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/correct_smooth.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3277 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/daegc.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4778 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/deepergcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2366 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/dgi.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    15685 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/diffpool.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2358 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/disengcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1827 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/drgat.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2298 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/drgcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    23753 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/dropedge_gcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2749 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/gae.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3491 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/gat.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    11030 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/gcc_model.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2671 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/gcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4040 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/gcnii.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3545 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/gcnmix.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6628 2022-05-19 11:56:57.000000 cogdl-0.5.3/cogdl/models/nn/gdc_gcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3897 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/gin.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3085 2022-05-19 11:56:57.000000 cogdl-0.5.3/cogdl/models/nn/grace.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4017 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/grand.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     7252 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/graph_unet.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6331 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/graphsage.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6311 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/graphsaint.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     7239 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/gtn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1747 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/han.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6074 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/infograph.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1935 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/m3s.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1777 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/mixhop.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1610 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/mlp.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4888 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/moe_gcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     7190 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/mvgrl.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     9856 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/patchy_san.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3465 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/ppnp.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2767 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/pprgo.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     9800 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/revgcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5375 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/rgcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     9940 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/sagn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      706 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/sgc.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4876 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/sign.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5027 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/sortpool.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     8696 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/srgcn.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2765 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/models/nn/unsup_graphsage.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/oag/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)       59 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/oag/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    23808 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/oag/bert_model.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5557 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/oag/dual_position_bert_model.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3787 2022-05-19 11:56:57.000000 cogdl-0.5.3/cogdl/oag/oagbert.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    37363 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/oag/oagbert_metainfo.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      661 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/oag/utils.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/operators/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      230 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/__init__.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/operators/edge_softmax/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1897 2022-06-01 06:16:58.000000 cogdl-0.5.3/cogdl/operators/edge_softmax/edge_softmax.cc
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3764 2022-05-31 12:55:30.000000 cogdl-0.5.3/cogdl/operators/edge_softmax/edge_softmax.cu
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      988 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/edge_softmax.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1451 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/fused_gat.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1481 2022-06-01 06:16:58.000000 cogdl-0.5.3/cogdl/operators/jt_spmm.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2301 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/linear.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2093 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/mhspmm.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4181 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/ops.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/operators/sample/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    10001 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/sample/sample.cpp
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      505 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/sample.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/operators/scatter_max/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1816 2022-06-01 06:16:58.000000 cogdl-0.5.3/cogdl/operators/scatter_max/scatter_max.cc
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2723 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/scatter_max/scatter_max.cu
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      930 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/scatter_max.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/operators/spmm/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5007 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/computeUtil.h
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1954 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/mhTranspose.cpp
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3466 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/mhTranspose.cu
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1491 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/multiheadSddmm.cpp
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3801 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/multiheadSddmm.cu
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1459 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/multiheadSpmm.cpp
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2294 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/multiheadSpmm.cu
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2493 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/sddmm.cpp
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    15947 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/sddmm_kernel.cu
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3743 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/spmm.cpp
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2041 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/spmm_cpu.cpp
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    21340 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm/spmm_kernel.cu
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5056 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/operators/spmm.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6588 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/options.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    10456 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/pipelines.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/trainer/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)       29 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/trainer/__init__.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/trainer/controller/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)       96 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/trainer/controller/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2183 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/trainer/controller/data_controller.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2503 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/trainer/controller/training_controller.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2053 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/trainer/embed_trainer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    18496 2022-06-01 11:02:18.000000 cogdl-0.5.3/cogdl/trainer/trainer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2142 2022-06-01 11:02:15.000000 cogdl-0.5.3/cogdl/trainer/trainer_utils.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/utils/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      148 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5200 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/evaluator.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     9003 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/graph_utils.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1010 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/index.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     7714 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/link_prediction_utils.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2617 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/optimizer.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3779 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/ppr_utils.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     7131 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/prone_utils.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/utils/rwalk/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1369 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/rwalk/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2842 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/sampling.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     8344 2022-06-01 11:02:18.000000 cogdl-0.5.3/cogdl/utils/spmm_utils.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     8308 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/srgcn_utils.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2862 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/transform.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     8116 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/utils/utils.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      197 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/__init__.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2631 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     8705 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/base_data_wrapper.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/graph_classification/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      223 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/graph_classification/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2019 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/graph_classification/graph_classification_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1026 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/graph_classification/graph_embedding_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      186 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/graph_classification/infograph_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1406 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/graph_classification/patchy_san_dw.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/heterogeneous/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      202 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/heterogeneous/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      339 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/heterogeneous/heterogeneous_embedding_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      388 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/heterogeneous/heterogeneous_gnn_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      352 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/heterogeneous/multiplex_embedding_dw.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/link_prediction/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      212 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/link_prediction/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2983 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/link_prediction/embedding_link_prediction_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      429 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/link_prediction/gnn_kg_link_prediction_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3168 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/link_prediction/gnn_link_prediction_dw.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      323 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1377 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/cluster_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2468 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/graphsage_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3643 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/m3s_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      684 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/network_embedding_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      515 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/node_classification_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4624 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/pprgo_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3203 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/sagn_dw.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/pretraining/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)       35 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/pretraining/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     9126 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/data_wrapper/pretraining/gcc_dw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5294 2022-05-19 11:56:57.000000 cogdl-0.5.3/cogdl/wrappers/default_match.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3496 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     6239 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/base_model_wrapper.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/clustering/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      112 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/clustering/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1187 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/clustering/agc_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3966 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/clustering/daegc_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1912 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/clustering/gae_mw.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/graph_classification/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      176 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/graph_classification/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1146 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/graph_classification/graph_classification_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      738 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/graph_classification/graph_embedding_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4167 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/graph_classification/infograph_mw.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/heterogeneous/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      205 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/heterogeneous/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1417 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/heterogeneous/heterogeneous_embedding_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1621 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/heterogeneous/heterogeneous_gnn_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3122 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/heterogeneous/multiplex_embedding_mw.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/link_prediction/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      215 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/link_prediction/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1787 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/link_prediction/embedding_link_prediction_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2581 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/link_prediction/gnn_kg_link_prediction_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2983 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/link_prediction/gnn_link_prediction_mw.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      709 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1310 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/correct_smooth_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3262 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/dgi_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     5985 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/gcnmix_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     3889 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/grace_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2164 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/grand_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1367 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/graphsage_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2804 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/m3s_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1122 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/mvgrl_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2412 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/network_embedding_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1688 2022-06-01 11:02:18.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/node_classification_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1661 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/pprgo_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     1943 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/sagn_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    18319 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/self_auxiliary_mw.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2287 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/unsup_graphsage_mw.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/pretraining/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)       36 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/pretraining/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4184 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/model_wrapper/pretraining/gcc_mw.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl/wrappers/tools/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)        0 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/tools/__init__.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     2764 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/tools/memory_moco.py
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     9351 2022-01-21 12:30:57.000000 cogdl-0.5.3/cogdl/wrappers/tools/wrapper_utils.py
-drwxrwxr-x   0 yukuo     (1025) yukuo     (1025)        0 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl.egg-info/
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)    13890 2022-06-01 12:05:56.000000 cogdl-0.5.3/cogdl.egg-info/PKG-INFO
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     9145 2022-06-01 12:05:57.000000 cogdl-0.5.3/cogdl.egg-info/SOURCES.txt
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)        1 2022-06-01 12:05:56.000000 cogdl-0.5.3/cogdl.egg-info/dependency_links.txt
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      163 2022-06-01 12:05:56.000000 cogdl-0.5.3/cogdl.egg-info/requires.txt
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)        6 2022-06-01 12:05:56.000000 cogdl-0.5.3/cogdl.egg-info/top_level.txt
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)      191 2022-01-21 12:30:57.000000 cogdl-0.5.3/pyproject.toml
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)       38 2022-06-01 12:05:57.000000 cogdl-0.5.3/setup.cfg
--rw-rw-r--   0 yukuo     (1025) yukuo     (1025)     4394 2022-05-19 11:56:57.000000 cogdl-0.5.3/setup.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.015191 cogdl-0.6/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1072 2021-01-17 07:39:36.000000 cogdl-0.6/LICENSE
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      140 2021-12-16 11:17:17.000000 cogdl-0.6/MANIFEST.in
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    13973 2023-04-27 11:06:09.015191 cogdl-0.6/PKG-INFO
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    13102 2023-04-27 10:58:03.000000 cogdl-0.6/README.md
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:08.987191 cogdl-0.6/cogdl/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)       89 2023-04-27 10:58:03.000000 cogdl-0.6/cogdl/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    10425 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/configs.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:08.987191 cogdl-0.6/cogdl/data/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      262 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/data/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4840 2023-04-23 10:47:47.000000 cogdl-0.6/cogdl/data/batch.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    32854 2023-04-24 10:47:25.000000 cogdl-0.6/cogdl/data/data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1990 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/data/dataloader.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     8503 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/data/dataset.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    10295 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/data/sampler.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:08.987191 cogdl-0.6/cogdl/datasets/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     9784 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/datasets/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4333 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/datasets/customized_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3164 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/datasets/gatne.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     8797 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/datasets/gcc_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    13408 2021-12-26 09:00:29.000000 cogdl-0.6/cogdl/datasets/geom_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     8506 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/datasets/grb_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5547 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/datasets/gtn_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5899 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/datasets/han_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    11976 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/datasets/kg_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5885 2022-06-06 05:30:54.000000 cogdl-0.6/cogdl/datasets/matlab_matrix.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2341 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/datasets/oagbert_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    10828 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/datasets/ogb.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6756 2022-01-20 08:33:13.000000 cogdl-0.6/cogdl/datasets/planetoid_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5519 2021-12-26 09:00:29.000000 cogdl-0.6/cogdl/datasets/rd2cd_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5969 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/datasets/rec_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     7155 2022-06-06 05:30:54.000000 cogdl-0.6/cogdl/datasets/saint_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     9671 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/datasets/stgat_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     9672 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/datasets/stgcn_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    12362 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/datasets/tu_data.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    13088 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/experiments.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:08.991191 cogdl-0.6/cogdl/layers/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1314 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/layers/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1838 2022-04-15 08:22:47.000000 cogdl-0.6/cogdl/layers/actgcn_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      941 2021-08-13 12:42:57.000000 cogdl-0.6/cogdl/layers/actgcnii_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      734 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/layers/actlinear_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2232 2021-08-13 12:42:57.000000 cogdl-0.6/cogdl/layers/actmlp_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1883 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/layers/actsage_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      544 2021-07-16 11:01:40.000000 cogdl-0.6/cogdl/layers/base_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6116 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/layers/deepergcn_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3653 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/layers/disengcn_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2842 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/layers/gat_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3092 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/layers/gat_layerii.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1838 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/layers/gcn_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1839 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/layers/gcn_layerii.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      891 2021-08-13 12:42:57.000000 cogdl-0.6/cogdl/layers/gcnii_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1189 2021-06-25 06:55:40.000000 cogdl-0.6/cogdl/layers/gin_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1264 2021-07-16 11:01:40.000000 cogdl-0.6/cogdl/layers/gine_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1008 2021-06-25 06:55:40.000000 cogdl-0.6/cogdl/layers/han_layer.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:08.991191 cogdl-0.6/cogdl/layers/jittor/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)       32 2022-06-06 05:30:54.000000 cogdl-0.6/cogdl/layers/jittor/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1698 2022-06-06 05:30:54.000000 cogdl-0.6/cogdl/layers/jittor/gcn_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1054 2021-04-26 15:10:22.000000 cogdl-0.6/cogdl/layers/mixhop_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2251 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/layers/mlp_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1860 2021-06-25 06:55:40.000000 cogdl-0.6/cogdl/layers/pprgo_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    19678 2021-08-13 12:42:57.000000 cogdl-0.6/cogdl/layers/reversible_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6064 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/layers/rgcn_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2341 2021-12-16 11:17:17.000000 cogdl-0.6/cogdl/layers/sage_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4656 2021-06-25 06:55:40.000000 cogdl-0.6/cogdl/layers/saint_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      704 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/layers/se_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2271 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/layers/set2set.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      503 2021-06-25 06:55:40.000000 cogdl-0.6/cogdl/layers/sgc_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      867 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/layers/stgat_layer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4278 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/layers/stgcn_layer.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:08.991191 cogdl-0.6/cogdl/loggers/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      379 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/loggers/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      206 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/loggers/base_logger.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      619 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/loggers/tensorboard_logger.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      701 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/loggers/wandb_logger.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:08.991191 cogdl-0.6/cogdl/models/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4810 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/models/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      943 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/base_model.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:08.995191 cogdl-0.6/cogdl/models/emb/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)        0 2021-04-26 15:10:22.000000 cogdl-0.6/cogdl/models/emb/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1910 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/complex.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4271 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/deepwalk.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4631 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/dgk.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      958 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/distmult.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5977 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/emb/dngr.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    15905 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/gatne.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4326 2022-04-15 08:23:13.000000 cogdl-0.6/cogdl/models/emb/graph2vec.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3123 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/emb/grarep.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     8952 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/hin2vec.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2557 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/emb/hope.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4270 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/knowledge_base.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     7200 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/line.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5151 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/metapath2vec.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5064 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/netmf.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6920 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/netsmf.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     7333 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/node2vec.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4295 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/emb/prone.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     7427 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/emb/pronepp.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6542 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/pte.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2335 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/rotate.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5688 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/emb/sdne.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1642 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/emb/spectral.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1003 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/emb/transe.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:08.999191 cogdl-0.6/cogdl/models/nn/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      802 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/models/nn/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2875 2021-12-16 11:17:17.000000 cogdl-0.6/cogdl/models/nn/actgcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2739 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/agc.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     8932 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/autognn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    11729 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/compgcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6675 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/correct_smooth.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3277 2021-12-16 11:17:17.000000 cogdl-0.6/cogdl/models/nn/daegc.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4778 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/nn/deepergcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2366 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/dgi.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    15685 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/diffpool.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2358 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/disengcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1757 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/drgat.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2298 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/drgcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    23307 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/dropedge_gcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2749 2021-12-16 11:17:17.000000 cogdl-0.6/cogdl/models/nn/gae.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3411 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/gat.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    11480 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/models/nn/gcc_model.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2607 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/gcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4040 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/nn/gcnii.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3545 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/gcnmix.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6628 2022-04-15 08:23:13.000000 cogdl-0.6/cogdl/models/nn/gdc_gcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3897 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/gin.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3037 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/grace.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3945 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/grand.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     7252 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/nn/graph_unet.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     7042 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/models/nn/graphsage.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6311 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/graphsaint.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     7239 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/nn/gtn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1687 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/han.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6074 2021-12-16 11:17:17.000000 cogdl-0.6/cogdl/models/nn/infograph.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1877 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/m3s.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1707 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/mixhop.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1610 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/mlp.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4770 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/moe_gcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     7190 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/mvgrl.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     9856 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/patchy_san.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3403 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/ppnp.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2767 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/pprgo.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     9326 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/models/nn/revgcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5375 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/rgcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     9940 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/sagn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      706 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/sgc.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4876 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/sign.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5027 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/models/nn/sortpool.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     8696 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/models/nn/srgcn.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4202 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/models/nn/stgat.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3476 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/models/nn/stgcn.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:08.999191 cogdl-0.6/cogdl/oag/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)       59 2021-01-17 07:39:36.000000 cogdl-0.6/cogdl/oag/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    23808 2021-04-26 15:10:22.000000 cogdl-0.6/cogdl/oag/bert_model.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5557 2021-11-04 16:16:40.000000 cogdl-0.6/cogdl/oag/dual_position_bert_model.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3787 2022-06-06 05:30:54.000000 cogdl-0.6/cogdl/oag/oagbert.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    37384 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/oag/oagbert_metainfo.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      661 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/oag/utils.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.003191 cogdl-0.6/cogdl/operators/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      230 2021-08-13 12:42:57.000000 cogdl-0.6/cogdl/operators/__init__.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.003191 cogdl-0.6/cogdl/operators/edge_softmax/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1897 2022-06-06 05:30:54.000000 cogdl-0.6/cogdl/operators/edge_softmax/edge_softmax.cc
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3764 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/operators/edge_softmax/edge_softmax.cu
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      988 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/operators/edge_softmax.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1451 2021-11-04 16:16:40.000000 cogdl-0.6/cogdl/operators/fused_gat.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1481 2022-06-06 05:30:54.000000 cogdl-0.6/cogdl/operators/jt_spmm.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2301 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/operators/linear.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2093 2021-11-04 16:16:40.000000 cogdl-0.6/cogdl/operators/mhspmm.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4181 2021-08-13 12:42:57.000000 cogdl-0.6/cogdl/operators/ops.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.003191 cogdl-0.6/cogdl/operators/sample/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    10001 2021-07-16 11:01:40.000000 cogdl-0.6/cogdl/operators/sample/sample.cpp
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      505 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/operators/sample.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.003191 cogdl-0.6/cogdl/operators/scatter_max/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1816 2022-06-06 05:30:54.000000 cogdl-0.6/cogdl/operators/scatter_max/scatter_max.cc
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2723 2021-12-16 11:17:18.000000 cogdl-0.6/cogdl/operators/scatter_max/scatter_max.cu
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      930 2021-12-16 11:17:17.000000 cogdl-0.6/cogdl/operators/scatter_max.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.003191 cogdl-0.6/cogdl/operators/spmm/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5007 2021-06-14 17:03:52.000000 cogdl-0.6/cogdl/operators/spmm/computeUtil.h
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1954 2021-12-16 11:17:18.000000 cogdl-0.6/cogdl/operators/spmm/mhTranspose.cpp
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3466 2021-07-27 12:43:53.000000 cogdl-0.6/cogdl/operators/spmm/mhTranspose.cu
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1491 2021-12-16 11:17:18.000000 cogdl-0.6/cogdl/operators/spmm/multiheadSddmm.cpp
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3801 2021-06-14 17:03:52.000000 cogdl-0.6/cogdl/operators/spmm/multiheadSddmm.cu
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1459 2021-12-16 11:17:18.000000 cogdl-0.6/cogdl/operators/spmm/multiheadSpmm.cpp
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2294 2021-06-14 17:03:52.000000 cogdl-0.6/cogdl/operators/spmm/multiheadSpmm.cu
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2493 2021-12-16 11:17:18.000000 cogdl-0.6/cogdl/operators/spmm/sddmm.cpp
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    15947 2021-04-26 15:10:22.000000 cogdl-0.6/cogdl/operators/spmm/sddmm_kernel.cu
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3743 2022-01-20 08:33:13.000000 cogdl-0.6/cogdl/operators/spmm/spmm.cpp
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2041 2021-12-16 11:17:18.000000 cogdl-0.6/cogdl/operators/spmm/spmm_cpu.cpp
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    21340 2022-01-20 08:33:13.000000 cogdl-0.6/cogdl/operators/spmm/spmm_kernel.cu
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5032 2023-04-24 07:57:11.000000 cogdl-0.6/cogdl/operators/spmm.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6767 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/options.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    10456 2021-12-16 11:17:18.000000 cogdl-0.6/cogdl/pipelines.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.003191 cogdl-0.6/cogdl/trainer/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)       29 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/trainer/__init__.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.003191 cogdl-0.6/cogdl/trainer/controller/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)       96 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/trainer/controller/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2183 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/trainer/controller/data_controller.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2503 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/trainer/controller/training_controller.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2037 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/trainer/embed_trainer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    20872 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/trainer/trainer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2702 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/trainer/trainer_utils.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.007191 cogdl-0.6/cogdl/utils/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      148 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/utils/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5716 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/utils/evaluator.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     9003 2021-12-16 11:17:18.000000 cogdl-0.6/cogdl/utils/graph_utils.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    14697 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/utils/grb_utils.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1010 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/utils/index.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     7714 2022-08-11 05:29:48.000000 cogdl-0.6/cogdl/utils/link_prediction_utils.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2617 2021-11-04 16:16:40.000000 cogdl-0.6/cogdl/utils/optimizer.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3779 2021-07-16 11:01:40.000000 cogdl-0.6/cogdl/utils/ppr_utils.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     7131 2021-07-16 11:01:40.000000 cogdl-0.6/cogdl/utils/prone_utils.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.007191 cogdl-0.6/cogdl/utils/rwalk/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1369 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/utils/rwalk/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3684 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/utils/sampling.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     8568 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/utils/spmm_utils.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     8256 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/utils/srgcn_utils.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2862 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/utils/transform.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     9301 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/utils/utils.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.007191 cogdl-0.6/cogdl/wrappers/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      197 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/__init__.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.007191 cogdl-0.6/cogdl/wrappers/data_wrapper/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2998 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     8876 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/base_data_wrapper.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.007191 cogdl-0.6/cogdl/wrappers/data_wrapper/graph_classification/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      223 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/graph_classification/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2019 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/graph_classification/graph_classification_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1026 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/graph_classification/graph_embedding_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      186 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/graph_classification/infograph_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1406 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/graph_classification/patchy_san_dw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.007191 cogdl-0.6/cogdl/wrappers/data_wrapper/heterogeneous/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      202 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/heterogeneous/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      339 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/heterogeneous/heterogeneous_embedding_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      388 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/heterogeneous/heterogeneous_gnn_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      352 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/heterogeneous/multiplex_embedding_dw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.007191 cogdl-0.6/cogdl/wrappers/data_wrapper/link_prediction/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      269 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/link_prediction/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2983 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/link_prediction/embedding_link_prediction_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      429 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/link_prediction/gnn_kg_link_prediction_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3155 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/link_prediction/gnn_link_prediction_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3829 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/link_prediction/triple_link_prediction_dw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.007191 cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      381 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1377 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/cluster_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2432 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/graphsage_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3609 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/m3s_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      684 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/network_embedding_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      515 2022-04-08 06:01:19.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/node_classification_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4600 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/pprgo_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3203 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/sagn_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2169 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/unsup_graphsage_dw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.007191 cogdl-0.6/cogdl/wrappers/data_wrapper/pretraining/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)       35 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/pretraining/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    16890 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/pretraining/gcc_dw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.007191 cogdl-0.6/cogdl/wrappers/data_wrapper/traffic_prediction/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)       78 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/traffic_prediction/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4910 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/traffic_prediction/stgat_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4888 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/data_wrapper/traffic_prediction/stgcn_dw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6058 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/default_match.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.007191 cogdl-0.6/cogdl/wrappers/model_wrapper/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3766 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6239 2021-12-16 11:17:18.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/base_model_wrapper.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.011191 cogdl-0.6/cogdl/wrappers/model_wrapper/clustering/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      112 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/clustering/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1187 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/clustering/agc_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3966 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/clustering/daegc_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1912 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/clustering/gae_mw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.011191 cogdl-0.6/cogdl/wrappers/model_wrapper/graph_classification/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      176 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/graph_classification/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1146 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/graph_classification/graph_classification_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      738 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/graph_classification/graph_embedding_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4167 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/graph_classification/infograph_mw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.011191 cogdl-0.6/cogdl/wrappers/model_wrapper/heterogeneous/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      205 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/heterogeneous/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1417 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/heterogeneous/heterogeneous_embedding_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1621 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/heterogeneous/heterogeneous_gnn_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3122 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/heterogeneous/multiplex_embedding_mw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.011191 cogdl-0.6/cogdl/wrappers/model_wrapper/link_prediction/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      273 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/link_prediction/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1787 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/link_prediction/embedding_link_prediction_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2581 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/link_prediction/gnn_kg_link_prediction_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2983 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/link_prediction/gnn_link_prediction_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6095 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/link_prediction/triple_link_prediction_mw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.011191 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      709 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1310 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/correct_smooth_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3262 2021-12-16 11:17:18.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/dgi_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5985 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/gcnmix_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3833 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/grace_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2164 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/grand_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1367 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/graphsage_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2804 2021-11-25 08:34:29.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/m3s_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1122 2021-12-16 11:17:18.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/mvgrl_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2412 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/network_embedding_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1687 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/node_classification_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1661 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/pprgo_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1943 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/sagn_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    18239 2022-08-17 07:30:18.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/self_auxiliary_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2270 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/unsup_graphsage_mw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.011191 cogdl-0.6/cogdl/wrappers/model_wrapper/pretraining/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)       36 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/pretraining/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     8841 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/pretraining/gcc_mw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.011191 cogdl-0.6/cogdl/wrappers/model_wrapper/traffic_prediction/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)       79 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/traffic_prediction/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     6324 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/traffic_prediction/stgat_mw.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     5694 2023-04-23 07:04:32.000000 cogdl-0.6/cogdl/wrappers/model_wrapper/traffic_prediction/stgcn_mw.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.011191 cogdl-0.6/cogdl/wrappers/tools/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)        0 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/tools/__init__.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2764 2021-11-04 16:16:40.000000 cogdl-0.6/cogdl/wrappers/tools/memory_moco.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     9351 2021-11-04 07:35:30.000000 cogdl-0.6/cogdl/wrappers/tools/wrapper_utils.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:08.987191 cogdl-0.6/cogdl.egg-info/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    13973 2023-04-27 11:06:08.000000 cogdl-0.6/cogdl.egg-info/PKG-INFO
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)    10253 2023-04-27 11:06:08.000000 cogdl-0.6/cogdl.egg-info/SOURCES.txt
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)        1 2023-04-27 11:06:08.000000 cogdl-0.6/cogdl.egg-info/dependency_links.txt
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      187 2023-04-27 11:06:08.000000 cogdl-0.6/cogdl.egg-info/requires.txt
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)        6 2023-04-27 11:06:08.000000 cogdl-0.6/cogdl.egg-info/top_level.txt
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      191 2021-11-04 07:35:30.000000 cogdl-0.6/pyproject.toml
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)       38 2023-04-27 11:06:09.015191 cogdl-0.6/setup.cfg
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     4429 2023-04-23 07:04:32.000000 cogdl-0.6/setup.py
+drwxrwxr-x   0 yukuo     (1011) yukuo     (1011)        0 2023-04-27 11:06:09.015191 cogdl-0.6/tests/
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2523 2021-11-04 07:35:30.000000 cogdl-0.6/tests/test_args.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3207 2023-04-23 07:04:32.000000 cogdl-0.6/tests/test_experiments.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)      714 2021-07-16 11:01:40.000000 cogdl-0.6/tests/test_layers.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     2408 2021-12-16 11:17:18.000000 cogdl-0.6/tests/test_oag.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     3101 2021-08-13 12:42:57.000000 cogdl-0.6/tests/test_ops.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1247 2021-11-04 07:35:30.000000 cogdl-0.6/tests/test_options.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1711 2022-08-17 07:30:18.000000 cogdl-0.6/tests/test_pipelines.py
+-rw-rw-r--   0 yukuo     (1011) yukuo     (1011)     1239 2021-04-26 15:10:22.000000 cogdl-0.6/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cogdl-0.5.3/LICENSE` & `cogdl-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/PKG-INFO` & `cogdl-0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogdl
-Version: 0.5.3
+Version: 0.6
 Summary: An Extensive Research Toolkit for Deep Learning on Graphs
 Home-page: https://github.com/THUDM/cogdl
 License: MIT
 Keywords: network embedding,graph representation learning,graph neural networks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -19,47 +19,51 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![CogDL](./docs/source/_static/cogdl-logo.png)
 ===
 
 [![PyPI Latest Release](https://badge.fury.io/py/cogdl.svg)](https://pypi.org/project/cogdl/)
-[![Build Status](https://travis-ci.org/THUDM/cogdl.svg?branch=master)](https://travis-ci.org/THUDM/cogdl)
+[![Build Status](https://app.travis-ci.com/THUDM/cogdl.svg?branch=master)](https://app.travis-ci.com/THUDM/cogdl)
 [![Documentation Status](https://readthedocs.org/projects/cogdl/badge/?version=latest)](https://cogdl.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://pepy.tech/badge/cogdl)](https://pepy.tech/project/cogdl)
 [![Coverage Status](https://coveralls.io/repos/github/THUDM/cogdl/badge.svg?branch=master)](https://coveralls.io/github/THUDM/cogdl?branch=master)
 [![License](https://img.shields.io/github/license/thudm/cogdl)](https://github.com/THUDM/cogdl/blob/master/LICENSE)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
-**[Homepage](https://cogdl.ai)** | **[Paper](https://arxiv.org/abs/2103.00959)** | **[100 GNN papers](./gnn_papers.md)** | **[Leaderboards](./results.md)** | **[Documentation](https://cogdl.readthedocs.io)** | **[Datasets](./cogdl/datasets/README.md)** | **[Join our Slack](https://join.slack.com/t/cogdl/shared_invite/zt-b9b4a49j-2aMB035qZKxvjV4vqf0hEg)** | **[中文](./README_CN.md)**
+**[Homepage](https://cogdl.ai)** | **[Paper](https://arxiv.org/abs/2103.00959)** | **[Documentation](https://cogdl.readthedocs.io)** | **[Discussion Forum](https://discuss.cogdl.ai)** | **[Dataset](./cogdl/datasets/README.md)** | **[中文](./README_CN.md)**
 
 CogDL is a graph deep learning toolkit that allows researchers and developers to easily train and compare baseline or customized models for node classification, graph classification, and other important tasks in the graph domain. 
 
 We summarize the contributions of CogDL as follows:
 
 - **Efficiency**: CogDL utilizes well-optimized operators to speed up training and save GPU memory of GNN models.
 - **Ease of Use**: CogDL provides easy-to-use APIs for running experiments with the given models and datasets using hyper-parameter search.
 - **Extensibility**: The design of CogDL makes it easy to apply GNN models to new scenarios based on our framework.
 
 ## ❗ News
 
-- The new **v0.5.3 release** supports mixed-precision training by setting \textit{fp16=True} and provides a basic [example](https://github.com/THUDM/cogdl/blob/master/examples/jittor/gcn.py) written by [Jittor](https://github.com/Jittor/jittor). It also updates the tutorial in the document, fixes downloading links of some datasets, and fixes potential bugs of operators. 
+- [The CogDL paper](https://arxiv.org/abs/2103.00959) was accepted by [WWW 2023](https://www2023.thewebconf.org/). Find us at WWW 2023! We also release the new **v0.6 release** which adds more examples of graph self-supervised learning, including [GraphMAE](https://github.com/THUDM/cogdl/tree/master/examples/graphmae), [GraphMAE2](https://github.com/THUDM/cogdl/tree/master/examples/graphmae2), and [BGRL](https://github.com/THUDM/cogdl/tree/master/examples/bgrl). 
 
-- The new **v0.5.2 release** adds a GNN example for ogbn-products and updates geom datasets. It also fixes some potential bugs including setting devices, using cpu for inference, etc.
+- A free GNN course provided by CogDL Team is present at [this link](https://cogdl.ai/gnn2022/). We also provide a [discussion forum](https://discuss.cogdl.ai) for Chinese users. 
 
-- The new **v0.5.1 release** adds fast operators including SpMM (cpu version) and scatter_max (cuda version). It also adds lots of datasets for node classification which can be found in [this link](./cogdl/datasets/rd2cd_data.py). 🎉
-
-- The new **v0.5.0 release** designs and implements a unified training loop for GNN. It introduces `DataWrapper` to help prepare the training/validation/test data and `ModelWrapper` to define the training/validation/test steps. 🎉
+- The new **v0.5.3 release** supports mixed-precision training by setting \textit{fp16=True} and provides a basic [example](https://github.com/THUDM/cogdl/blob/master/examples/jittor/gcn.py) written by [Jittor](https://github.com/Jittor/jittor). It also updates the tutorial in the document, fixes downloading links of some datasets, and fixes potential bugs of operators. 
 
 <details>
 <summary>
 News History
 </summary>
 <br/>
 
+- The new **v0.5.2 release** adds a GNN example for ogbn-products and updates geom datasets. It also fixes some potential bugs including setting devices, using cpu for inference, etc.
+
+- The new **v0.5.1 release** adds fast operators including SpMM (cpu version) and scatter_max (cuda version). It also adds lots of datasets for node classification which can be found in [this link](./cogdl/datasets/rd2cd_data.py). 🎉
+
+- The new **v0.5.0 release** designs and implements a unified training loop for GNN. It introduces `DataWrapper` to help prepare the training/validation/test data and `ModelWrapper` to define the training/validation/test steps. 🎉
+
 - The new **v0.4.1 release** adds the implementation of Deep GNNs and the recommendation task. It also supports new pipelines for generating embeddings and recommendation. Welcome to join our tutorial on KDD 2021 at 10:30 am - 12:00 am, Aug. 14th (Singapore Time). More details can be found in https://kdd2021graph.github.io/. 🎉
 
 - The new **v0.4.0 release** refactors the data storage (from `Data` to `Graph`) and provides more fast operators to speed up GNN training. It also includes many self-supervised learning methods on graphs. BTW, we are glad to announce that we will give a tutorial on KDD 2021 in August. Please see [this link](https://kdd2021graph.github.io/) for more details. 🎉
 
 - CogDL supports GNN models with Mixture of Experts (MoE). You can install [FastMoE](https://github.com/laekov/fastmoe) and try **[MoE GCN](./cogdl/models/nn/moe_gcn.py)** in CogDL now!
 
 - The new **v0.3.0 release** provides a fast spmm operator to speed up GNN training. We also release the first version of **[CogDL paper](https://arxiv.org/abs/2103.00959)** in arXiv. You can join [our slack](https://join.slack.com/t/cogdl/shared_invite/zt-b9b4a49j-2aMB035qZKxvjV4vqf0hEg) for discussion. 🎉🎉🎉
@@ -127,26 +131,14 @@
         "hidden_size": trial.suggest_categorical("hidden_size", [32, 64, 128]),
         "dropout": trial.suggest_uniform("dropout", 0.5, 0.8),
     }
 
 experiment(dataset="cora", model="gcn", seed=[1, 2], search_space=search_space)
 ```
 
-Some interesting applications can be used through `pipeline` API. An example can be found in the [pipeline.py](https://github.com/THUDM/cogdl/tree/master/examples/pipeline.py). 
-
-```python
-from cogdl import pipeline
-
-# load OAGBert model and perform inference
-oagbert = pipeline("oagbert")
-outputs = oagbert(["CogDL is developed by KEG, Tsinghua.", "OAGBert is developed by KEG, Tsinghua."])
-```
-
-More details of the OAGBert usage can be found [here](./cogdl/oag/README.md).
-
 ### Command-Line Usage
 
 You can also use `python scripts/train.py --dataset example_dataset --model example_model` to run example_model on example_data.
 
 - --dataset, dataset name to run, can be a list of datasets with space like `cora citeseer`. Supported datasets include
 'cora', 'citeseer', 'pumbed', 'ppi', 'wikipedia', 'blogcatalog', 'flickr'. More datasets can be found in the [cogdl/datasets](https://github.com/THUDM/cogdl/tree/master/cogdl/datasets).
 - --model, model name to run, can be a list of models like `gcn gat`. Supported models include
@@ -234,23 +226,23 @@
 
 * Let's say you implement a GNN model in a script `models/nn/abcgnn.py` that does the task of node classification. Then, you need to add a unit test inside the script `tests/tasks/test_node_classification.py` (or whatever relevant task your model does). 
 * To add the unit test, you simply add a function *test_abcgnn_cora()* (just follow the format of the other unit tests already in the script), fill it with required arguments and the last line in the function *'assert 0 <= ret["Acc"] <= 1'* is the very basic sanity check conducted by the unit test. 
 * After modifying `tests/tasks/test_node_classification.py`, commit it together with your `models/nn/abcgnn.py` and your pull request should pass.
 </details>
 
 ## CogDL Team
-CogDL is developed and maintained by [Tsinghua, ZJU, BAAI, DAMO Academy, and ZHIPU.AI](https://cogdl.ai/about/). 
+CogDL is developed and maintained by [Tsinghua, ZJU, DAMO Academy, and ZHIPU.AI](https://cogdl.ai/about/). 
 
 The core development team can be reached at [cogdlteam@gmail.com](mailto:cogdlteam@gmail.com).
 
 ## Citing CogDL
 
 Please cite [our paper](https://arxiv.org/abs/2103.00959) if you find our code or results useful for your research:
 
 ```
-@article{cen2021cogdl,
-    title={CogDL: A Toolkit for Deep Learning on Graphs},
+@inproceedings{cen2023cogdl,
+    title={CogDL: A Comprehensive Library for Graph Deep Learning},
     author={Yukuo Cen and Zhenyu Hou and Yan Wang and Qibin Chen and Yizhen Luo and Zhongming Yu and Hengrui Zhang and Xingcheng Yao and Aohan Zeng and Shiguang Guo and Yuxiao Dong and Yang Yang and Peng Zhang and Guohao Dai and Yu Wang and Chang Zhou and Hongxia Yang and Jie Tang},
-    journal={arXiv preprint arXiv:2103.00959},
-    year={2021}
+    booktitle={Proceedings of the ACM Web Conference 2023 (WWW'23)},
+    year={2023}
 }
 ```
```

### Comparing `cogdl-0.5.3/README.md` & `cogdl-0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 ![CogDL](./docs/source/_static/cogdl-logo.png)
 ===
 
 [![PyPI Latest Release](https://badge.fury.io/py/cogdl.svg)](https://pypi.org/project/cogdl/)
-[![Build Status](https://travis-ci.org/THUDM/cogdl.svg?branch=master)](https://travis-ci.org/THUDM/cogdl)
+[![Build Status](https://app.travis-ci.com/THUDM/cogdl.svg?branch=master)](https://app.travis-ci.com/THUDM/cogdl)
 [![Documentation Status](https://readthedocs.org/projects/cogdl/badge/?version=latest)](https://cogdl.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://pepy.tech/badge/cogdl)](https://pepy.tech/project/cogdl)
 [![Coverage Status](https://coveralls.io/repos/github/THUDM/cogdl/badge.svg?branch=master)](https://coveralls.io/github/THUDM/cogdl?branch=master)
 [![License](https://img.shields.io/github/license/thudm/cogdl)](https://github.com/THUDM/cogdl/blob/master/LICENSE)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
-**[Homepage](https://cogdl.ai)** | **[Paper](https://arxiv.org/abs/2103.00959)** | **[100 GNN papers](./gnn_papers.md)** | **[Leaderboards](./results.md)** | **[Documentation](https://cogdl.readthedocs.io)** | **[Datasets](./cogdl/datasets/README.md)** | **[Join our Slack](https://join.slack.com/t/cogdl/shared_invite/zt-b9b4a49j-2aMB035qZKxvjV4vqf0hEg)** | **[中文](./README_CN.md)**
+**[Homepage](https://cogdl.ai)** | **[Paper](https://arxiv.org/abs/2103.00959)** | **[Documentation](https://cogdl.readthedocs.io)** | **[Discussion Forum](https://discuss.cogdl.ai)** | **[Dataset](./cogdl/datasets/README.md)** | **[中文](./README_CN.md)**
 
 CogDL is a graph deep learning toolkit that allows researchers and developers to easily train and compare baseline or customized models for node classification, graph classification, and other important tasks in the graph domain. 
 
 We summarize the contributions of CogDL as follows:
 
 - **Efficiency**: CogDL utilizes well-optimized operators to speed up training and save GPU memory of GNN models.
 - **Ease of Use**: CogDL provides easy-to-use APIs for running experiments with the given models and datasets using hyper-parameter search.
 - **Extensibility**: The design of CogDL makes it easy to apply GNN models to new scenarios based on our framework.
 
 ## ❗ News
 
-- The new **v0.5.3 release** supports mixed-precision training by setting \textit{fp16=True} and provides a basic [example](https://github.com/THUDM/cogdl/blob/master/examples/jittor/gcn.py) written by [Jittor](https://github.com/Jittor/jittor). It also updates the tutorial in the document, fixes downloading links of some datasets, and fixes potential bugs of operators. 
+- [The CogDL paper](https://arxiv.org/abs/2103.00959) was accepted by [WWW 2023](https://www2023.thewebconf.org/). Find us at WWW 2023! We also release the new **v0.6 release** which adds more examples of graph self-supervised learning, including [GraphMAE](https://github.com/THUDM/cogdl/tree/master/examples/graphmae), [GraphMAE2](https://github.com/THUDM/cogdl/tree/master/examples/graphmae2), and [BGRL](https://github.com/THUDM/cogdl/tree/master/examples/bgrl). 
 
-- The new **v0.5.2 release** adds a GNN example for ogbn-products and updates geom datasets. It also fixes some potential bugs including setting devices, using cpu for inference, etc.
+- A free GNN course provided by CogDL Team is present at [this link](https://cogdl.ai/gnn2022/). We also provide a [discussion forum](https://discuss.cogdl.ai) for Chinese users. 
 
-- The new **v0.5.1 release** adds fast operators including SpMM (cpu version) and scatter_max (cuda version). It also adds lots of datasets for node classification which can be found in [this link](./cogdl/datasets/rd2cd_data.py). 🎉
-
-- The new **v0.5.0 release** designs and implements a unified training loop for GNN. It introduces `DataWrapper` to help prepare the training/validation/test data and `ModelWrapper` to define the training/validation/test steps. 🎉
+- The new **v0.5.3 release** supports mixed-precision training by setting \textit{fp16=True} and provides a basic [example](https://github.com/THUDM/cogdl/blob/master/examples/jittor/gcn.py) written by [Jittor](https://github.com/Jittor/jittor). It also updates the tutorial in the document, fixes downloading links of some datasets, and fixes potential bugs of operators. 
 
 <details>
 <summary>
 News History
 </summary>
 <br/>
 
+- The new **v0.5.2 release** adds a GNN example for ogbn-products and updates geom datasets. It also fixes some potential bugs including setting devices, using cpu for inference, etc.
+
+- The new **v0.5.1 release** adds fast operators including SpMM (cpu version) and scatter_max (cuda version). It also adds lots of datasets for node classification which can be found in [this link](./cogdl/datasets/rd2cd_data.py). 🎉
+
+- The new **v0.5.0 release** designs and implements a unified training loop for GNN. It introduces `DataWrapper` to help prepare the training/validation/test data and `ModelWrapper` to define the training/validation/test steps. 🎉
+
 - The new **v0.4.1 release** adds the implementation of Deep GNNs and the recommendation task. It also supports new pipelines for generating embeddings and recommendation. Welcome to join our tutorial on KDD 2021 at 10:30 am - 12:00 am, Aug. 14th (Singapore Time). More details can be found in https://kdd2021graph.github.io/. 🎉
 
 - The new **v0.4.0 release** refactors the data storage (from `Data` to `Graph`) and provides more fast operators to speed up GNN training. It also includes many self-supervised learning methods on graphs. BTW, we are glad to announce that we will give a tutorial on KDD 2021 in August. Please see [this link](https://kdd2021graph.github.io/) for more details. 🎉
 
 - CogDL supports GNN models with Mixture of Experts (MoE). You can install [FastMoE](https://github.com/laekov/fastmoe) and try **[MoE GCN](./cogdl/models/nn/moe_gcn.py)** in CogDL now!
 
 - The new **v0.3.0 release** provides a fast spmm operator to speed up GNN training. We also release the first version of **[CogDL paper](https://arxiv.org/abs/2103.00959)** in arXiv. You can join [our slack](https://join.slack.com/t/cogdl/shared_invite/zt-b9b4a49j-2aMB035qZKxvjV4vqf0hEg) for discussion. 🎉🎉🎉
@@ -106,26 +110,14 @@
         "hidden_size": trial.suggest_categorical("hidden_size", [32, 64, 128]),
         "dropout": trial.suggest_uniform("dropout", 0.5, 0.8),
     }
 
 experiment(dataset="cora", model="gcn", seed=[1, 2], search_space=search_space)
 ```
 
-Some interesting applications can be used through `pipeline` API. An example can be found in the [pipeline.py](https://github.com/THUDM/cogdl/tree/master/examples/pipeline.py). 
-
-```python
-from cogdl import pipeline
-
-# load OAGBert model and perform inference
-oagbert = pipeline("oagbert")
-outputs = oagbert(["CogDL is developed by KEG, Tsinghua.", "OAGBert is developed by KEG, Tsinghua."])
-```
-
-More details of the OAGBert usage can be found [here](./cogdl/oag/README.md).
-
 ### Command-Line Usage
 
 You can also use `python scripts/train.py --dataset example_dataset --model example_model` to run example_model on example_data.
 
 - --dataset, dataset name to run, can be a list of datasets with space like `cora citeseer`. Supported datasets include
 'cora', 'citeseer', 'pumbed', 'ppi', 'wikipedia', 'blogcatalog', 'flickr'. More datasets can be found in the [cogdl/datasets](https://github.com/THUDM/cogdl/tree/master/cogdl/datasets).
 - --model, model name to run, can be a list of models like `gcn gat`. Supported models include
@@ -213,23 +205,23 @@
 
 * Let's say you implement a GNN model in a script `models/nn/abcgnn.py` that does the task of node classification. Then, you need to add a unit test inside the script `tests/tasks/test_node_classification.py` (or whatever relevant task your model does). 
 * To add the unit test, you simply add a function *test_abcgnn_cora()* (just follow the format of the other unit tests already in the script), fill it with required arguments and the last line in the function *'assert 0 <= ret["Acc"] <= 1'* is the very basic sanity check conducted by the unit test. 
 * After modifying `tests/tasks/test_node_classification.py`, commit it together with your `models/nn/abcgnn.py` and your pull request should pass.
 </details>
 
 ## CogDL Team
-CogDL is developed and maintained by [Tsinghua, ZJU, BAAI, DAMO Academy, and ZHIPU.AI](https://cogdl.ai/about/). 
+CogDL is developed and maintained by [Tsinghua, ZJU, DAMO Academy, and ZHIPU.AI](https://cogdl.ai/about/). 
 
 The core development team can be reached at [cogdlteam@gmail.com](mailto:cogdlteam@gmail.com).
 
 ## Citing CogDL
 
 Please cite [our paper](https://arxiv.org/abs/2103.00959) if you find our code or results useful for your research:
 
 ```
-@article{cen2021cogdl,
-    title={CogDL: A Toolkit for Deep Learning on Graphs},
+@inproceedings{cen2023cogdl,
+    title={CogDL: A Comprehensive Library for Graph Deep Learning},
     author={Yukuo Cen and Zhenyu Hou and Yan Wang and Qibin Chen and Yizhen Luo and Zhongming Yu and Hengrui Zhang and Xingcheng Yao and Aohan Zeng and Shiguang Guo and Yuxiao Dong and Yang Yang and Peng Zhang and Guohao Dai and Yu Wang and Chang Zhou and Hongxia Yang and Jie Tang},
-    journal={arXiv preprint arXiv:2103.00959},
-    year={2021}
+    booktitle={Proceedings of the ACM Web Conference 2023 (WWW'23)},
+    year={2023}
 }
 ```
```

### Comparing `cogdl-0.5.3/cogdl/configs.py` & `cogdl-0.6/cogdl/configs.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,52 +22,30 @@
             "lr": 0.005,
             "hidden_size": 2048,
             "num_layers": 2,
             "dropout": 0.3,
             "epochs": 7000,
             # 78.04
         },
-        "flickr": {
-            "lr": 0.01,
-            "dropout": 0.5,
-            "weight_decay": 0.0,
-            "hidden_size": 256,
-        },
-    },
-    "sage": {
-        "general": {},
+        "flickr": {"lr": 0.01, "dropout": 0.5, "weight_decay": 0.0, "hidden_size": 256,},
     },
+    "sage": {"general": {},},
     "gcnii": {
-        "general": {
-            "epochs": 1000,
-            "dropout": 0.5,
-            "wd1": 0.001,
-            "wd2": 5e-4,
-        },
-        "cora": {
-            "num_layers": 64,
-            "hidden_size": 64,
-            "dropout": 0.6,
-        },
+        "general": {"epochs": 1000, "dropout": 0.5, "wd1": 0.001, "wd2": 5e-4,},
+        "cora": {"num_layers": 64, "hidden_size": 64, "dropout": 0.6,},
         "citeseer": {
             "num_layers": 32,
             "hidden_size": 256,
             "lr": 0.001,
             "patience": 200,
             "epochs": 2000,
             "lmbda": 0.6,
             "dropout": 0.7,
         },
-        "pubmed": {
-            "num_layers": 16,
-            "hidden_size": 256,
-            "lmbda": 0.4,
-            "dropout": 0.5,
-            "wd1": 5e-4,
-        },
+        "pubmed": {"num_layers": 16, "hidden_size": 256, "lmbda": 0.4, "dropout": 0.5, "wd1": 5e-4,},
         "reddit": {
             "num_layers": 3,
             "hidden_size": 256,
             "alpha": 0.2,
             "wd1": 0,
             "wd2": 0,
             "lr": 0.001,
@@ -83,21 +61,17 @@
             "wd1": 0.0005,
             "wd2": 0.0005,
             "lmbda": 1.0,
             "alpha": 0.1,
         }
         # 52.54
     },
-    "gdc_gcn": {
-        "general": {"hidden_size": 16},
-    },
+    "gdc_gcn": {"general": {"hidden_size": 16},},
     "grand": {
-        "general": {
-            "epochs": 1000,
-        },
+        "general": {"epochs": 1000,},
         "cora": {
             "order": 8,
             "sample": 4,
             "lam": 1.0,
             "tem": 0.5,
             "alpha": 0.5,
             "patience": 200,
@@ -122,49 +96,28 @@
             "alpha": 0.5,
             "lr": 0.2,
             "bn": True,
             "input_dropout": 0.6,
             "hidden_dropout": 0.8,
         },
     },
-    "graphsage": {
-        "general": {},
-    },
-    "sgc": {
-        "general": {
-            "hidden_size": 16,
-            "dropout": 0.5,
-        },
-    },
+    "graphsage": {"general": {},},
+    "sgc": {"general": {"hidden_size": 16, "dropout": 0.5,},},
     "sgcpn": {
         "general": {
             "lr": 0.005,
             "epochs": 1000,
             "patience": 1000,
             "norm_mode": "PN",
             "norm_scale": 10,
             "dropout": 0.6,
         },
     },
-    "sign": {
-        "general": {
-            "lr": 0.00005,
-            "hidden_size": 2048,
-            "dropout": 0.5,
-            "dropedge_rate": 0.2,
-        },
-    },
-    "srgcn": {
-        "general": {
-            "lr": 0.005,
-            "epochs": 1000,
-        },
-        "cora": {"dropout": 0.6},
-        "citeseer": {"dropout": 0.6},
-    },
+    "sign": {"general": {"lr": 0.00005, "hidden_size": 2048, "dropout": 0.5, "dropedge_rate": 0.2,},},
+    "srgcn": {"general": {"lr": 0.005, "epochs": 1000,}, "cora": {"dropout": 0.6}, "citeseer": {"dropout": 0.6},},
     "unet": {
         "general": {
             "epochs": 1000,
             "n_dropout": 0.90,
             "adj_dropout": 0.05,
             "hidden_size": 128,
             "aug_adj": False,
@@ -250,21 +203,15 @@
             "autoscale": False,
             "scale": 10.0,
             "norm": "batchnorm",
             "act_first": True,
         },
     },
     "sagn": {
-        "general": {
-            "data_gpu": True,
-            "lr": 0.001,
-            "hidden-size": 512,
-            "attn-drop": 0.0,
-            "dropout": 0.7,
-        },
+        "general": {"data_gpu": True, "lr": 0.001, "hidden-size": 512, "attn-drop": 0.0, "dropout": 0.7,},
         "flickr": {
             "threshold": 0.5,
             "label-hop": 2,
             "weight-decay": 3e-6,
             "nstage": [50, 50, 50],
             "nhop": 2,
             "batch-size": 256,
@@ -275,77 +222,54 @@
             "batch-size": 1000,
             "nhop": 2,
             "label-nhop": 4,
             "weight-decay": 0.0,
             "nstage": [500, 500, 500],
         },
     },
-    "deepwalk": {
-        "general": {},
-    },
+    "deepwalk": {"general": {},},
     "dngr": {
         "general": {
             "hidden_size": 128,
             "lr": 0.001,
             "epochs": 500,
             "hidden_size1": 1000,
             "hidden_size2": 128,
             "noise": 0.2,
             "alpha": 0.1,
             "step": 10,
         },
     },
-    "grarep": {
-        "general": {},
-    },
-    "hope": {
-        "general": {},
-    },
-    "line": {
-        "general": {},
-        "blogcatalog": {"walk_num": 40},
-    },
+    "grarep": {"general": {},},
+    "hope": {"general": {},},
+    "line": {"general": {}, "blogcatalog": {"walk_num": 40},},
     "netmf": {
         "general": {},
         "ppi-ne": {"window_size": 10, "is_large": True},
         "blogcatalog": {"window_size": 10, "is_large": True},
         "wikipedia": {"window_size": 1},
     },
     "netsmf": {
         "general": {"window_size": 10, "num_round": 1000},
         "wikipedia": {"window_size": 1},
         "blogcatalog": {"num_round": 10000},
     },
-    "node2vec": {
-        "general": {},
-    },
+    "node2vec": {"general": {},},
     "prone": {
         "general": {"step": 10},
         "ppi-ne": {"mu": 0.0},
         "wikipedia": {"mu": -4.0},
         "dblp-ne": {"mu": -1.2, "theta": 2.0},
     },
-    "sdne": {
-        "general": {},
-    },
-    "spectral": {
-        "general": {},
-    },
-    "dgi": {
-        "general": {"weight_decay": 0},
-    },
-    "gcc": {
-        "general": {},
-    },
+    "sdne": {"general": {},},
+    "spectral": {"general": {},},
+    "dgi": {"general": {"weight_decay": 0},},
+    "gcc": {"general": {},},
     "grace": {
-        "general": {
-            "weight_decay": 0,
-            "epochs": 1000,
-            "patience": 20,
-        },
+        "general": {"weight_decay": 0, "epochs": 1000, "patience": 20,},
         "cora": {
             "lr": 0.0005,
             "weight_decay": 0.00001,
             "tau": 0.4,
             "drop_feature_rates": [0.3, 0.4],
             "drop_edge_rates": [0.2, 0.4],
             "epochs": 200,
@@ -368,19 +292,15 @@
             "drop_edge_rates": [0.4, 0.1],
             "drop_feature_rates": [0.0, 0.2],
             "tau": 0.7,
             "lr": 0.001,
             "weight_decay": 0.00001,
         },
     },
-    "unsup_graphsage": {
-        "lr": 0.001,
-        "weight_decay": 0,
-        "epochs": 3000,
-    },
+    "unsup_graphsage": {"lr": 0.001, "weight_decay": 0, "epochs": 3000,},
     "revgcn": {
         "general": {},
         "cora": {
             "hidden_size": 128,
             "lr": 0.001,
             "dropout": 0.4706458854,
             "weight_decay": 0.0008907,
@@ -390,94 +310,37 @@
         },
     },
     "gin": {
         "general": {"lr": 0.001},
         "imdb-b": {"degree_feature": True},
         "imdb-m": {"degree_feature": True},
         "collab": {"degree_feature": True},
-        "proteins": {
-            "num_layers": 5,
-            "dropout": 0.0,
-        },
-        "nci1": {
-            "num_layers": 5,
-            "dropout": 0.3,
-            "hidden_size": 64,
-        },
+        "proteins": {"num_layers": 5, "dropout": 0.0,},
+        "nci1": {"num_layers": 5, "dropout": 0.3, "hidden_size": 64,},
     },
     "infograph": {
-        "general": {
-            "lr": 0.0001,
-            "weight_decay": 5e-4,
-            "sup": False,
-        },
-        "mutag": {
-            "num_layers": 1,
-            "epochs": 20,
-        },
+        "general": {"lr": 0.0001, "weight_decay": 5e-4, "sup": False,},
+        "mutag": {"num_layers": 1, "epochs": 20,},
         "imdb-b": {"degree_feature": True},
         "imdb-m": {"degree_feature": True},
         "collab": {"degree_feature": True},
         "nci1": {"num_layers": 3},
     },
-    "sortpool": {
-        "nci1": {
-            "dropout": 0.3,
-            "hidden_size": 64,
-            "num_layers": 5,
-        },
-    },
+    "sortpool": {"nci1": {"dropout": 0.3, "hidden_size": 64, "num_layers": 5,},},
     "patchy_san": {
-        "general": {
-            "lr": 0.001,
-            "hidden_size": 32,
-            "gamma": 0.5,
-            "dropout": 0.5,
-        },
+        "general": {"lr": 0.001, "hidden_size": 32, "gamma": 0.5, "dropout": 0.5,},
         "imdb-b": {"degree_feature": True},
         "imdb-m": {"degree_feature": True},
         "collab": {"degree_feature": True},
     },
     "graph2vec": {
         "general": {},
-        "nci1": {
-            "lr": 0.001,
-            "window_size": 8,
-            "epochs": 10,
-            "iteration": 4,
-        },
-        "reddit-b": {
-            "lr": 0.01,
-            "degree_feature": True,
-            "hidden_size": 128,
-        },
-    },
-    "gatne": {
-        "general": {},
-        "twitter": {"eval_type": "1"},
-    },
-    "hin2vec": {
-        "general": {
-            "lr": 0.025,
-        },
-    },
-    "metapath2vec": {
-        "general": {
-            "walk_num": 40,
-        },
+        "nci1": {"lr": 0.001, "window_size": 8, "epochs": 10, "iteration": 4,},
+        "reddit-b": {"lr": 0.01, "degree_feature": True, "hidden_size": 128,},
     },
+    "gatne": {"general": {}, "twitter": {"eval_type": "1"},},
+    "hin2vec": {"general": {"lr": 0.025,},},
+    "metapath2vec": {"general": {"walk_num": 40,},},
     "pte": {},
-    "gtn": {
-        "general": {
-            "hidden_size": 128,
-            "lr": 0.005,
-            "weight_decay": 0.001,
-        },
-    },
-    "han": {
-        "general": {
-            "hidden_size": 128,
-            "lr": 0.005,
-            "weight_decay": 0.001,
-        }
-    },
+    "gtn": {"general": {"hidden_size": 128, "lr": 0.005, "weight_decay": 0.001,},},
+    "han": {"general": {"hidden_size": 128, "lr": 0.005, "weight_decay": 0.001,}},
 }
```

### Comparing `cogdl-0.5.3/cogdl/data/batch.py` & `cogdl-0.6/cogdl/data/batch.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/data/data.py` & `cogdl-0.6/cogdl/data/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,19 +432,19 @@
             weight = self.get_weight().tolist()
             gnx.add_weighted_edges_from([(row[i], col[i], weight[i]) for i in range(len(row))])
         else:
             edges = torch.stack((row, col)).cpu().numpy().transpose()
             gnx.add_edges_from(edges)
         return gnx
 
-    def random_walk(self, seeds, length=1, restart_p=0.0):
+    def random_walk(self, seeds, length=1, restart_p=0.0, parallel=True):
         if not hasattr(self, "__walker__"):
             scipy_adj = self.to_scipy_csr()
             self.__walker__ = RandomWalker(scipy_adj)
-        return self.__walker__.walk(seeds, length, restart_p=restart_p)
+        return self.__walker__.walk(seeds, length, restart_p=restart_p, parallel=parallel)
 
     @staticmethod
     def from_dict(dictionary):
         r"""Creates a data object from a python dictionary."""
         data = Adjacency()
         for key, item in dictionary.items():
             data[key] = item
@@ -475,22 +475,26 @@
     def __init__(self, x=None, y=None, **kwargs):
         super(Graph, self).__init__()
         if x is not None:
             if not torch.is_tensor(x):
                 raise ValueError("Node features must be Tensor")
         self.x = x
         self.y = y
+        self.grb_adj = None
+        num_nodes = x.shape[0] if x is not None else None
 
         for key, item in kwargs.items():
             if key == "num_nodes":
                 self.__num_nodes__ = item
+                num_nodes = item
+            elif key == "grb_adj":
+                self.grb_adj = item
             elif not is_read_adj_key(key):
                 self[key] = item
 
-        num_nodes = x.shape[0] if x is not None else None
         if "edge_index_train" in kwargs:
             self._adj_train = Adjacency(num_nodes=num_nodes)
             for key, item in kwargs.items():
                 if is_adj_key_train(key):
                     _key = re.search(r"(.*)_train", key).group(1)
                     if _key.startswith("edge_"):
                         _key = _key.split("edge_")[1]
@@ -527,22 +531,25 @@
         self.__is_train__ = False
         return self
 
     def add_remaining_self_loops(self):
         self._adj_full.add_remaining_self_loops()
         if self._adj_train is not None:
             self._adj_train.add_remaining_self_loops()
+        return self
 
     def padding_self_loops(self):
         self._adj.padding_self_loops()
+        return self
 
     def remove_self_loops(self):
         self._adj_full.remove_self_loops()
         if self._adj_train is not None:
             self._adj_train.remove_self_loops()
+        return self
 
     def row_norm(self):
         self._adj.row_norm()
 
     def col_norm(self):
         self._adj.col_norm()
 
@@ -783,15 +790,15 @@
         return "{}({})".format(self.__class__.__name__, ", ".join(info))
 
     def sample_adj(self, batch, size=-1, replace=True):
         if sample_adj_c is not None:
             if not torch.is_tensor(batch):
                 batch = torch.tensor(batch, dtype=torch.long)
             (row_ptr, col_indices, nodes, edges) = sample_adj_c(
-                self._adj.row_indptr, self.col_indices, batch, size, replace
+                self.row_indptr, self.col_indices, batch, size, replace
             )
         else:
             if torch.is_tensor(batch):
                 batch = batch.cpu().numpy()
             if self.__is_train__ and self._adj_train is not None:
                 key = "__mx_train__"
             else:
@@ -884,21 +891,26 @@
                 key = "__mx__"
             if not hasattr(self, key):
                 row = self._adj.row.numpy()
                 col = self._adj.col.numpy()
                 val = self.edge_weight.numpy()
                 N = self.num_nodes
                 self[key] = sp.csr_matrix((val, (row, col)), shape=(N, N))
-            sub_adj = self[key][node_idx, :][:, node_idx]
+            sub_adj = self[key][node_idx, :][:, node_idx].tocoo()
             sub_g = Graph()
-            sub_g.row_indptr = torch.from_numpy(sub_adj.indptr).long()
-            sub_g.col_indices = torch.from_numpy(sub_adj.indices).long()
+            # sub_g.row_indptr = torch.from_numpy(sub_adj.indptr).long()
+            # sub_g.col_indices = torch.from_numpy(sub_adj.indices).long()
+            row = torch.from_numpy(sub_adj.row).long()
+            col = torch.from_numpy(sub_adj.col).long()
+            sub_g.edge_index = (row, col)
             sub_g.edge_weight = torch.from_numpy(sub_adj.data)
+            sub_g.num_nodes = len(node_idx)
             for key in self.__keys__():
                 sub_g[key] = self[key][node_idx]
+            sub_g._adj._to_csr()
             return sub_g.to(self._adj.device)
 
     def edge_subgraph(self, edge_idx, require_idx=True):
         row, col = self._adj.edge_index
         row = row[edge_idx]
         col = col[edge_idx]
         edge_index = torch.stack([row, col])
@@ -908,19 +920,19 @@
             g[key] = self[key][nodes]
 
         if require_idx:
             return g, nodes, edge_idx
         else:
             return g
 
-    def random_walk(self, seeds, max_nodes_per_seed, restart_p=0.0):
-        return self._adj.random_walk(seeds, max_nodes_per_seed, restart_p)
+    def random_walk(self, seeds, max_nodes_per_seed, restart_p=0.0, parallel=True):
+        return self._adj.random_walk(seeds, max_nodes_per_seed, restart_p, parallel)
 
-    def random_walk_with_restart(self, seeds, max_nodes_per_seed, restart_p=0.0):
-        return self._adj.random_walk(seeds, max_nodes_per_seed, restart_p)
+    def random_walk_with_restart(self, seeds, max_nodes_per_seed, restart_p=0.0, parallel=True):
+        return self._adj.random_walk(seeds, max_nodes_per_seed, restart_p, parallel)
 
     def to_scipy_csr(self):
         return self._adj.to_scipy_csr()
 
     def to_networkx(self):
         return self._adj.to_networkx()
 
@@ -931,14 +943,17 @@
         for key, item in dictionary.items():
             data[key] = item
         return data
 
     def nodes(self):
         return torch.arange(self.num_nodes)
 
+    def set_grb_adj(self, adj):
+        self.grb_adj = adj
+
     # @property
     # def requires_grad(self):
     #     return False
     #
     # @requires_grad.setter
     # def requires_grad(self, x):
     #     print(f"Set `requires_grad` to {x}")
```

### Comparing `cogdl-0.5.3/cogdl/data/dataloader.py` & `cogdl-0.6/cogdl/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/data/dataset.py` & `cogdl-0.6/cogdl/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import collections
 import os.path as osp
 from itertools import repeat
+
 import numpy as np
 
 import torch.utils.data
 
 from cogdl.data import Adjacency, Graph
 from cogdl.utils import makedirs
 from cogdl.utils import Accuracy, CrossEntropyLoss
```

### Comparing `cogdl-0.5.3/cogdl/datasets/__init__.py` & `cogdl-0.6/cogdl/datasets/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -56,18 +56,38 @@
     for key in inspect.signature(dataset_class.__init__).parameters.keys():
         if key == "split":
             return dataset_class(split=split)
 
     return dataset_class()
 
 
+def build_dataset_pretrain(args):
+    args.pretrain = False
+    dataset_names = args.dataset
+    if ' ' in args.dataset:
+        datasets_name = args.dataset.split(' ')
+        dataset = []
+        for dataset_ in datasets_name:
+            args.dataset = dataset_
+            dataset.append(build_dataset(args))
+    else:
+        dataset = [build_dataset(args)]
+    args.pretrain = True
+    args.dataset = dataset_names
+    dataset_class = getattr(importlib.import_module("cogdl.datasets.gcc_data"), "PretrainDataset")
+    return dataset_class(args.dataset, [x.data for x in dataset])
+
+
 def build_dataset(args):
     if not hasattr(args, "split"):
         args.split = 0
-    dataset = build_dataset_from_name(args.dataset, args.split)
+    if not hasattr(args, "pretrain") or not args.pretrain:
+        dataset = build_dataset_from_name(args.dataset, args.split)
+    else:
+        dataset = build_dataset_pretrain(args)
 
     if hasattr(dataset, "num_classes") and dataset.num_classes > 0:
         args.num_classes = dataset.num_classes
     if hasattr(dataset, "num_features") and dataset.num_features > 0:
         args.num_features = dataset.num_features
 
     return dataset
@@ -92,27 +112,38 @@
         except Exception as e:
             print(e)
             exit(0)
     raise ValueError("You are expected to specify `dataset` and `data_path`")
 
 
 SUPPORTED_DATASETS = {
+    "gcc_academic": "cogdl.datasets.gcc_data.Academic_GCCDataset",
+    "gcc_dblp_netrep": "cogdl.datasets.gcc_data.DBLPNetrep_GCCDataset",
+    "gcc_dblp_snap": "cogdl.datasets.gcc_data.DBLPSnap_GCCDataset",
+    "gcc_facebook": "cogdl.datasets.gcc_data.Facebook_GCCDataset",
+    "gcc_imdb": "cogdl.datasets.gcc_data.IMDB_GCCDataset",
+    "gcc_livejournal": "cogdl.datasets.gcc_data.Livejournal_GCCDataset",
     "kdd_icdm": "cogdl.datasets.gcc_data.KDD_ICDM_GCCDataset",
     "sigir_cikm": "cogdl.datasets.gcc_data.SIGIR_CIKM_GCCDataset",
     "sigmod_icde": "cogdl.datasets.gcc_data.SIGMOD_ICDE_GCCDataset",
     "usa-airport": "cogdl.datasets.gcc_data.USAAirportDataset",
+    "h-index": "cogdl.datasets.gcc_data.HIndexDataset",
     "ogbn-arxiv": "cogdl.datasets.ogb.OGBArxivDataset",
     "ogbn-products": "cogdl.datasets.ogb.OGBProductsDataset",
     "ogbn-proteins": "cogdl.datasets.ogb.OGBProteinsDataset",
     "ogbn-papers100M": "cogdl.datasets.ogb.OGBPapers100MDataset",
     "ogbg-molbace": "cogdl.datasets.ogb.OGBMolbaceDataset",
     "ogbg-molhiv": "cogdl.datasets.ogb.OGBMolhivDataset",
     "ogbg-molpcba": "cogdl.datasets.ogb.OGBMolpcbaDataset",
     "ogbg-ppa": "cogdl.datasets.ogb.OGBPpaDataset",
     "ogbg-code": "cogdl.datasets.ogb.OGBCodeDataset",
+    "ogbl-ppa": "cogdl.datasets.ogb.OGBLPpaDataset",
+    "ogbl-ddi": "cogdl.datasets.ogb.OGBLDdiDataset",
+    "ogbl-collab": "cogdl.datasets.ogb.OGBLCollabDataset",
+    "ogbl-citation2": "cogdl.datasets.ogb.OGBLCitation2Dataset",
     "amazon": "cogdl.datasets.gatne.AmazonDataset",
     "twitter": "cogdl.datasets.gatne.TwitterDataset",
     "youtube": "cogdl.datasets.gatne.YouTubeDataset",
     "gtn-acm": "cogdl.datasets.gtn_data.ACM_GTNDataset",
     "gtn-dblp": "cogdl.datasets.gtn_data.DBLP_GTNDataset",
     "gtn-imdb": "cogdl.datasets.gtn_data.IMDB_GTNDataset",
     "fb13": "cogdl.datasets.kg_data.FB13Datset",
@@ -178,8 +209,15 @@
     "Weibo": "cogdl.datasets.rd2cd_data.Weibo",
     "bgp": "cogdl.datasets.rd2cd_data.bgp",
     "ssn5": "cogdl.datasets.rd2cd_data.ssn5",
     "ssn7": "cogdl.datasets.rd2cd_data.ssn7",
     "Aids": "cogdl.datasets.rd2cd_data.Aids",
     "Nba": "cogdl.datasets.rd2cd_data.Nba",
     "Pokec_z": "cogdl.datasets.rd2cd_data.Pokec_z",
+    "grb-cora": "cogdl.datasets.grb_data.Cora_GRBDataset",
+    "grb-citeseer": "cogdl.datasets.grb_data.Citeseer_GRBDataset",
+    "grb-reddit": "cogdl.datasets.grb_data.Reddit_GRBDataset",
+    "grb-aminer": "cogdl.datasets.grb_data.Aminer_GRBDataset",
+    "grb-flickr": "cogdl.datasets.grb_data.Flickr_GRBDataset",
+    "pems-stgcn": "cogdl.datasets.stgcn_data.PeMS_Dataset",
+    "pems-stgat": "cogdl.datasets.stgat_data.PeMS_Dataset",
 }
```

### Comparing `cogdl-0.5.3/cogdl/datasets/customized_data.py` & `cogdl-0.6/cogdl/datasets/customized_data.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/datasets/gatne.py` & `cogdl-0.6/cogdl/datasets/gatne.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/datasets/gcc_data.py` & `cogdl-0.6/cogdl/datasets/gcc_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 from collections import defaultdict
 
 import torch
 
 from cogdl.data import Graph, Dataset
 from cogdl.utils import download_url
+from cogdl.utils import Accuracy, CrossEntropyLoss
 
 
 class GCCDataset(Dataset):
     url = "https://github.com/cenyk1230/gcc-data/raw/master"
 
     def __init__(self, root, name):
         self.name = name
@@ -92,15 +93,18 @@
     def __init__(self, root, name):
         self.name = name
         super(Edgelist, self).__init__(root)
         self.data = torch.load(self.processed_paths[0])
 
     @property
     def raw_file_names(self):
-        names = ["edgelist.txt", "nodelabel.txt"]
+        if self.name in UNLABELED_GCCDATASETS:
+            names = ["edgelist.txt"]
+        else:
+            names = ["edgelist.txt", "nodelabel.txt"]
         return names
 
     @property
     def processed_file_names(self):
         return ["data.pt"]
 
     @property
@@ -138,30 +142,69 @@
             labels = []
             label2id = defaultdict(int)
             for line in f:
                 x, label = list(map(int, line.split()))
                 if label not in label2id:
                     label2id[label] = len(label2id)
                 nodes.append(node2id[x])
-                if "hindex" in self.name:
+                if "h-index" in self.name:
                     labels.append(label)
                 else:
                     labels.append(label2id[label])
-            if "hindex" in self.name:
+            if "h-index" in self.name:
                 median = np.median(labels)
                 labels = [int(label > median) for label in labels]
         assert num_nodes == len(set(nodes))
         y = torch.zeros(num_nodes, len(label2id))
         y[nodes, labels] = 1
 
         data = Graph(edge_index=torch.LongTensor(edge_list).t(), x=None, y=y)
 
         torch.save(data, self.processed_paths[0])
 
 
+class PretrainDataset(object):
+
+    class DataList(object):
+
+        def __init__(self, graphs):
+            for graph in graphs:
+                graph.y = None
+            self.graphs = graphs
+
+        def to(self, device):
+            return [graph.to(device) for graph in self.graphs]
+
+        def train(self):
+            return [graph.train() for graph in self.graphs]
+
+        def eval(self):
+            return [graph.eval() for graph in self.graphs]
+
+    def __init__(self, name, data):
+        super(PretrainDataset, self).__init__()
+        self.name = name
+        # self.data = data
+        self.data = self.DataList(data)
+
+    def get_evaluator(self):
+        return Accuracy()
+
+    def get_loss_fn(self):
+        return CrossEntropyLoss()
+
+    @property
+    def num_features(self):
+        return 0
+
+    def get(self, idx):
+        assert idx == 0
+        return self.data.graphs
+
+
 class KDD_ICDM_GCCDataset(GCCDataset):
     def __init__(self, data_path="data"):
         dataset = "kdd_icdm"
         path = osp.join(data_path, dataset)
         super(KDD_ICDM_GCCDataset, self).__init__(path, dataset)
 
 
@@ -180,7 +223,65 @@
 
 
 class USAAirportDataset(Edgelist):
     def __init__(self, data_path="data"):
         dataset = "usa-airport"
         path = osp.join(data_path, dataset)
         super(USAAirportDataset, self).__init__(path, dataset)
+
+
+class HIndexDataset(Edgelist):
+    def __init__(self, data_path="data"):
+        dataset = "h-index"
+        path = osp.join(data_path, dataset)
+        super(HIndexDataset, self).__init__(path, dataset)
+
+
+class Academic_GCCDataset(Edgelist):
+    def __init__(self, data_path="data"):
+        dataset = "gcc_academic"
+        path = osp.join(data_path, dataset)
+        super(Academic_GCCDataset, self).__init__(path, dataset)
+
+
+class DBLPNetrep_GCCDataset(Edgelist):
+    def __init__(self, data_path="data"):
+        dataset = "gcc_dblp_netrep"
+        path = osp.join(data_path, dataset)
+        super(DBLPNetrep_GCCDataset, self).__init__(path, dataset)
+
+
+class DBLPSnap_GCCDataset(Edgelist):
+    def __init__(self, data_path="data"):
+        dataset = "gcc_dblp_snap"
+        path = osp.join(data_path, dataset)
+        super(DBLPSnap_GCCDataset, self).__init__(path, dataset)
+
+
+class Facebook_GCCDataset(Edgelist):
+    def __init__(self, data_path="data"):
+        dataset = "gcc_facebook"
+        path = osp.join(data_path, dataset)
+        super(Facebook_GCCDataset, self).__init__(path, dataset)
+
+
+class IMDB_GCCDataset(Edgelist):
+    def __init__(self, data_path="data"):
+        dataset = "gcc_imdb"
+        path = osp.join(data_path, dataset)
+        super(IMDB_GCCDataset, self).__init__(path, dataset)
+
+
+class Livejournal_GCCDataset(Edgelist):
+    def __init__(self, data_path="data"):
+        dataset = "gcc_livejournal"
+        path = osp.join(data_path, dataset)
+        super(Livejournal_GCCDataset, self).__init__(path, dataset)
+
+
+UNLABELED_GCCDATASETS = ["gcc_academic", 
+                         "gcc_dblp_netrep",
+                         "gcc_dblp_snap",
+                         "gcc_facebook",
+                         "gcc_imdb",
+                         "gcc_livejournal"
+                         ]
```

### Comparing `cogdl-0.5.3/cogdl/datasets/geom_data.py` & `cogdl-0.6/cogdl/datasets/geom_data.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/datasets/gtn_data.py` & `cogdl-0.6/cogdl/datasets/gtn_data.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/datasets/han_data.py` & `cogdl-0.6/cogdl/datasets/han_data.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/datasets/matlab_matrix.py` & `cogdl-0.6/cogdl/datasets/matlab_matrix.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/datasets/oagbert_data.py` & `cogdl-0.6/cogdl/datasets/oagbert_data.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/datasets/ogb.py` & `cogdl-0.6/cogdl/datasets/ogb.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import torch
 
 from ogb.nodeproppred import NodePropPredDataset
 from ogb.nodeproppred import Evaluator as NodeEvaluator
 from ogb.graphproppred import GraphPropPredDataset
+from ogb.linkproppred import LinkPropPredDataset
 
 from cogdl.data import Dataset, Graph, DataLoader
 from cogdl.utils import CrossEntropyLoss, Accuracy, remove_self_loops, coalesce, BCEWithLogitsLoss
 
 
 class OGBNDataset(Dataset):
     def __init__(self, root, name, transform=None):
@@ -230,7 +231,89 @@
         super(OGBPpaDataset, self).__init__(path, dataset)
 
 
 class OGBCodeDataset(OGBGDataset):
     def __init__(self, data_path="data"):
         dataset = "ogbg-code"
         super(OGBCodeDataset, self).__init__(data_path, dataset)
+
+
+#This part is for ogbl datasets
+
+class OGBLDataset(Dataset):
+    def __init__(self, root, name):
+        """
+           - name (str): name of the dataset
+            - root (str): root directory to store the dataset folder
+        """        
+        
+        self.name = name
+        
+        dataset = LinkPropPredDataset(name, root)
+        graph= dataset[0]
+        x = torch.tensor(graph["node_feat"]).contiguous() if graph["node_feat"] is not None else None
+        row, col = graph["edge_index"][0], graph["edge_index"][1]
+        row = torch.from_numpy(row)
+        col = torch.from_numpy(col)
+        edge_index = torch.stack([row, col], dim=0)
+        edge_attr = torch.as_tensor(graph["edge_feat"]) if graph["edge_feat"] is not None else graph["edge_feat"]
+        edge_index, edge_attr = remove_self_loops(edge_index, edge_attr)
+        row = torch.cat([edge_index[0], edge_index[1]])
+        col = torch.cat([edge_index[1], edge_index[0]])
+
+        row, col, _ = coalesce(row, col)
+        edge_index = torch.stack([row, col], dim=0)
+
+        self.data = Graph(x=x, edge_index=edge_index, edge_attr=edge_attr, y=None)
+        self.data.num_nodes = graph["num_nodes"]
+        
+    def get(self, idx):
+        assert idx == 0
+        return self.data
+
+    def get_loss_fn(self):
+        return CrossEntropyLoss()
+
+    def get_evaluator(self):
+        return Accuracy()
+
+    def _download(self):
+        pass
+    
+    @property
+    def processed_file_names(self):
+        return "data_cogdl.pt"
+    
+    def _process(self):
+        pass
+    
+    def get_edge_split(self):
+        idx = self.dataset.get_edge_split()
+        train_edge = torch.from_numpy(idx['train']['edge'].T)
+        val_edge = torch.from_numpy(idx['valid']['edge'].T)
+        test_edge = torch.from_numpy(idx['test']['edge'].T)
+        return train_edge, val_edge, test_edge
+
+class OGBLPpaDataset(OGBLDataset):
+    def __init__(self, data_path="data"):
+        dataset = "ogbl-ppa"
+        super(OGBLPpaDataset, self).__init__(data_path, dataset)
+        
+        
+class OGBLCollabDataset(OGBLDataset):
+    def __init__(self, data_path="data"):
+        dataset = "ogbl-collab"
+        super(OGBLCollabDataset, self).__init__(data_path, dataset)
+        
+
+class OGBLDdiDataset(OGBLDataset):
+    def __init__(self, data_path="data"):
+        dataset = "ogbl-ddi"
+        super(OGBLDdiDataset, self).__init__(data_path, dataset)
+
+        
+class OGBLCitation2Dataset(OGBLDataset):
+    def __init__(self, data_path="data"):
+        dataset = "ogbl-citation2"
+        super(OGBLCitation2Dataset, self).__init__(data_path, dataset)
+                           
+
```

### Comparing `cogdl-0.5.3/cogdl/datasets/planetoid_data.py` & `cogdl-0.6/cogdl/datasets/planetoid_data.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/datasets/rd2cd_data.py` & `cogdl-0.6/cogdl/datasets/rd2cd_data.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/datasets/rec_data.py` & `cogdl-0.6/cogdl/datasets/rec_data.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/datasets/saint_data.py` & `cogdl-0.6/cogdl/datasets/saint_data.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/datasets/tu_data.py` & `cogdl-0.6/cogdl/datasets/tu_data.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/experiments.py` & `cogdl-0.6/cogdl/experiments.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import torch
 import torch.nn as nn
 import torch.multiprocessing as mp
 import optuna
 from tabulate import tabulate
 
-from cogdl.utils import set_random_seed, tabulate_results
+from cogdl.utils import set_random_seed, tabulate_results, build_model_path
 from cogdl.configs import BEST_CONFIGS
 from cogdl.data import Dataset
 from cogdl.models import build_model
 from cogdl.datasets import build_dataset
 from cogdl.wrappers import fetch_model_wrapper, fetch_data_wrapper
 from cogdl.options import get_default_args
 from cogdl.trainer import Trainer
@@ -107,14 +107,17 @@
     print(
         f""" 
 |-------------------------------------{'-' * (len(str(args.dataset)) + len(model_name) + len(dw_name) + len(mw_name))}|
     *** Running (`{args.dataset}`, `{model_name}`, `{dw_name}`, `{mw_name}`)
 |-------------------------------------{'-' * (len(str(args.dataset)) + len(model_name) + len(dw_name) + len(mw_name))}|"""
     )
 
+    if hasattr(args, "save_model_path"):
+        args = build_model_path(args, model_name)
+
     if getattr(args, "use_best_config", False):
         args = set_best_config(args)
 
     # setup dataset and specify `num_features` and `num_classes` for model
     if isinstance(args.dataset, Dataset):
         dataset = args.dataset
     else:
@@ -177,14 +180,20 @@
         epochs=args.epochs,
         batch_size=args.batch_size if hasattr(args, "batch_size") else 0,
     )
 
     if hasattr(args, "hidden_size"):
         optimizer_cfg["hidden_size"] = args.hidden_size
 
+    if hasattr(args, "beta1") and hasattr(args, "beta2"):
+        optimizer_cfg["betas"] = (args.beta1, args.beta2)
+
+    if hasattr(dataset_wrapper, "train_dataset"):
+        optimizer_cfg["total"] = len(dataset_wrapper.train_dataset)
+
     # setup model_wrapper
     if isinstance(args.mw, str) and "embedding" in args.mw:
         model_wrapper = mw_class(model, **model_wrapper_args)
     else:
         model_wrapper = mw_class(model, optimizer_cfg, **model_wrapper_args)
 
     os.makedirs("./checkpoints", exist_ok=True)
@@ -202,18 +211,21 @@
         checkpoint_path=args.checkpoint_path,
         resume_training=args.resume_training,
         patience=args.patience,
         eval_step=args.eval_step,
         logger=args.logger,
         log_path=args.log_path,
         project=args.project,
-        no_test=args.no_test,
+        return_model=args.return_model,
         nstage=args.nstage,
         actnn=args.actnn,
         fp16=args.fp16,
+        do_test=args.do_test,
+        do_valid=args.do_valid,
+        clip_grad_norm=args.clip_grad_norm,
     )
 
     # Go!!!
     result = trainer.run(model_wrapper, dataset_wrapper)
 
     return result
```

### Comparing `cogdl-0.5.3/cogdl/layers/__init__.py` & `cogdl-0.6/cogdl/layers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 from .han_layer import HANLayer
 from .pprgo_layer import PPRGoLayer
 from .rgcn_layer import RGCNLayer
 from .sgc_layer import SGCLayer
 from .mixhop_layer import MixHopLayer
 from .reversible_layer import RevGNNLayer
 from .set2set import Set2Set
+from .stgcn_layer import STConvLayer
+from .stgat_layer import STGATConvLayer
+from .gcn_layerii import GCNLayerST
+from .gat_layerii import GATLayerST
 
 
 __all__ = [
     "BaseLayer",
     "GCNLayer",
     "MeanAggregator",
     "SumAggregator",
@@ -38,8 +42,12 @@
     "PPRGoLayer",
     "RGCNLayer",
     "SGCLayer",
     "MixHopLayer",
     "MLP",
     "RevGNNLayer",
     "Set2Set",
+    "STConvLayer",
+    "STGATConvLayer",
+    "GCNLayerST",
+    "GATLayerST",
 ]
```

### Comparing `cogdl-0.5.3/cogdl/layers/actgcn_layer.py` & `cogdl-0.6/cogdl/layers/actgcn_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/actgcnii_layer.py` & `cogdl-0.6/cogdl/layers/actgcnii_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/actlinear_layer.py` & `cogdl-0.6/cogdl/layers/actlinear_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/actmlp_layer.py` & `cogdl-0.6/cogdl/layers/actmlp_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/actsage_layer.py` & `cogdl-0.6/cogdl/layers/actsage_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/base_layer.py` & `cogdl-0.6/cogdl/layers/base_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/deepergcn_layer.py` & `cogdl-0.6/cogdl/layers/deepergcn_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,33 +31,19 @@
         self.use_msg_norm = use_msg_norm
         self.mlp = MLP(in_feats, out_feats, in_feats * 2, num_layers=num_mlp_layers, activation=activation, norm=norm)
 
         self.message_encoder = torch.nn.ReLU()
 
         self.aggr = aggr
         if aggr == "softmax_sg":
-            self.beta = torch.nn.Parameter(
-                torch.Tensor(
-                    [
-                        beta,
-                    ]
-                ),
-                requires_grad=learn_beta,
-            )
+            self.beta = torch.nn.Parameter(torch.Tensor([beta,]), requires_grad=learn_beta,)
         else:
             self.register_buffer("beta", None)
         if aggr == "powermean":
-            self.p = torch.nn.Parameter(
-                torch.Tensor(
-                    [
-                        p,
-                    ]
-                ),
-                requires_grad=learn_p,
-            )
+            self.p = torch.nn.Parameter(torch.Tensor([p,]), requires_grad=learn_p,)
         else:
             self.register_buffer("p", None)
         self.eps = 1e-7
 
         self.s = torch.nn.Parameter(torch.Tensor([1.0]), requires_grad=learn_msg_scale and use_msg_norm)
         self.residual = residual
```

### Comparing `cogdl-0.5.3/cogdl/layers/disengcn_layer.py` & `cogdl-0.6/cogdl/layers/disengcn_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/gat_layer.py` & `cogdl-0.6/cogdl/layers/gat_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/gcn_layer.py` & `cogdl-0.6/cogdl/layers/gcn_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/gcnii_layer.py` & `cogdl-0.6/cogdl/layers/gcnii_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/gin_layer.py` & `cogdl-0.6/cogdl/layers/gin_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/gine_layer.py` & `cogdl-0.6/cogdl/layers/gine_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/han_layer.py` & `cogdl-0.6/cogdl/layers/han_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/jittor/gcn_layer.py` & `cogdl-0.6/cogdl/layers/jittor/gcn_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/mixhop_layer.py` & `cogdl-0.6/cogdl/layers/mixhop_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/mlp_layer.py` & `cogdl-0.6/cogdl/layers/mlp_layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         bias=True,
     ):
         super(MLP, self).__init__()
         self.norm = norm
         self.activation = get_activation(activation)
         self.act_first = act_first
         self.dropout = dropout
+        self.output_dim = out_feats
         shapes = [in_feats] + [hidden_size] * (num_layers - 1) + [out_feats]
         self.mlp = nn.ModuleList(
             [nn.Linear(shapes[layer], shapes[layer + 1], bias=bias) for layer in range(num_layers)]
         )
         if norm is not None and num_layers > 1:
             if norm == "layernorm":
                 self.norm_list = nn.ModuleList(nn.LayerNorm(x) for x in shapes[1:-1])
```

### Comparing `cogdl-0.5.3/cogdl/layers/pprgo_layer.py` & `cogdl-0.6/cogdl/layers/pprgo_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/reversible_layer.py` & `cogdl-0.6/cogdl/layers/reversible_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/rgcn_layer.py` & `cogdl-0.6/cogdl/layers/rgcn_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/sage_layer.py` & `cogdl-0.6/cogdl/layers/sage_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/saint_layer.py` & `cogdl-0.6/cogdl/layers/saint_layer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/layers/se_layer.py` & `cogdl-0.6/cogdl/layers/se_layer.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,18 +8,15 @@
     def __init__(self, in_channels, se_channels):
         super(SELayer, self).__init__()
 
         self.in_channels = in_channels
         self.se_channels = se_channels
 
         self.encoder_decoder = nn.Sequential(
-            nn.Linear(in_channels, se_channels),
-            nn.ELU(),
-            nn.Linear(se_channels, in_channels),
-            nn.Sigmoid(),
+            nn.Linear(in_channels, se_channels), nn.ELU(), nn.Linear(se_channels, in_channels), nn.Sigmoid(),
         )
 
         # self.reset_parameters()
 
     def forward(self, x):
         """"""
         # Aggregate input representation
```

### Comparing `cogdl-0.5.3/cogdl/layers/set2set.py` & `cogdl-0.6/cogdl/layers/set2set.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/loggers/tensorboard_logger.py` & `cogdl-0.6/cogdl/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/loggers/wandb_logger.py` & `cogdl-0.6/cogdl/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/__init__.py` & `cogdl-0.6/cogdl/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     else:
         raise NotImplementedError(f"Failed to import {model} model.")
     class_name = SUPPORTED_MODELS[model].split(".")[-1]
     return getattr(module, class_name).build_model_from_args(args)
 
 
 SUPPORTED_MODELS = {
+    "transe": "cogdl.models.emb.transe.TransE",
+    "complex": "cogdl.models.emb.complex.ComplEx",
+    "distmult": "cogdl.models.emb.distmult.DistMult",
+    "rotate": "cogdl.models.emb.rotate.RotatE",
     "hope": "cogdl.models.emb.hope.HOPE",
     "spectral": "cogdl.models.emb.spectral.Spectral",
     "hin2vec": "cogdl.models.emb.hin2vec.Hin2vec",
     "netmf": "cogdl.models.emb.netmf.NetMF",
     "deepwalk": "cogdl.models.emb.deepwalk.DeepWalk",
     "gatne": "cogdl.models.emb.gatne.GATNE",
     "dgk": "cogdl.models.emb.dgk.DeepGraphKernel",
@@ -96,20 +100,22 @@
     "dropedge_gcn": "cogdl.models.nn.dropedge_gcn.DropEdge_GCN",
     "disengcn": "cogdl.models.nn.disengcn.DisenGCN",
     "mlp": "cogdl.models.nn.mlp.MLP",
     "sgc": "cogdl.models.nn.sgc.sgc",
     "sortpool": "cogdl.models.nn.sortpool.SortPool",
     "srgcn": "cogdl.models.nn.srgcn.SRGCN",
     "gcc": "cogdl.models.nn.gcc_model.GCCModel",
-    "unsup_graphsage": "cogdl.models.nn.unsup_graphsage.SAGE",
+    "unsup_graphsage": "cogdl.models.nn.graphsage.UnsupGraphsage",
     "graphsaint": "cogdl.models.nn.graphsaint.GraphSAINT",
     "m3s": "cogdl.models.nn.m3s.M3S",
     "moe_gcn": "cogdl.models.nn.moe_gcn.MoEGCN",
     "lightgcn": "cogdl.models.nn.lightgcn.LightGCN",
     "correct_smooth_mlp": "cogdl.models.nn.correct_smooth.CorrectSmoothMLP",
     "sagn": "cogdl.models.nn.sagn.SAGN",
     "revgcn": "cogdl.models.nn.revgcn.RevGCN",
     "revgat": "cogdl.models.nn.revgcn.RevGAT",
     "revgen": "cogdl.models.nn.revgcn.RevGEN",
     "sage": "cogdl.models.nn.graphsage.SAGE",
     "autognn": "cogdl.models.nn.autognn.AutoGNN",
+    "stgcn": "cogdl.models.nn.stgcn.STGCN",
+    "stgat": "cogdl.models.nn.stgat.STGAT",
 }
```

### Comparing `cogdl-0.5.3/cogdl/models/base_model.py` & `cogdl-0.6/cogdl/models/base_model.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/emb/deepwalk.py` & `cogdl-0.6/cogdl/models/emb/deepwalk.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,22 +36,15 @@
         parser.add_argument("--iteration", type=int, default=10,
                             help="Number of iterations. Default is 10.")
         parser.add_argument("--hidden-size", type=int, default=128)
         # fmt: on
 
     @classmethod
     def build_model_from_args(cls, args) -> "DeepWalk":
-        return cls(
-            args.hidden_size,
-            args.walk_length,
-            args.walk_num,
-            args.window_size,
-            args.worker,
-            args.iteration,
-        )
+        return cls(args.hidden_size, args.walk_length, args.walk_num, args.window_size, args.worker, args.iteration,)
 
     def __init__(self, dimension, walk_length, walk_num, window_size, worker, iteration):
         super(DeepWalk, self).__init__()
         self.dimension = dimension
         self.walk_length = walk_length
         self.walk_num = walk_num
         self.window_size = window_size
@@ -62,20 +55,20 @@
         nx_g = graph.to_networkx()
         self.G = nx_g
         walks = self._simulate_walks(self.walk_length, self.walk_num)
         walks = [[str(node) for node in walk] for walk in walks]
         print("training word2vec...")
         model = embedding_model_creator(
             walks,
-            size=self.dimension,
+            vector_size=self.dimension,
             window=self.window_size,
             min_count=0,
             sg=1,
             workers=self.worker,
-            iter=self.iteration,
+            epochs=self.iteration,
         )
         id2node = dict([(vid, node) for vid, node in enumerate(nx_g.nodes())])
         embeddings = np.asarray([model.wv[str(id2node[i])] for i in range(len(id2node))])
 
         if return_dict:
             features_matrix = dict()
             for vid, node in enumerate(nx_g.nodes()):
```

### Comparing `cogdl-0.5.3/cogdl/models/emb/dgk.py` & `cogdl-0.6/cogdl/models/emb/dgk.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,25 +84,25 @@
         if self.gl_collections is None:
             self.gl_collections = Parallel(n_jobs=self.n_workers)(
                 delayed(DeepGraphKernel.feature_extractor)(graph, self.rounds, str(i)) for i, graph in enumerate(graphs)
             )
 
         model = Word2Vec(
             self.gl_collections,
-            size=self.hidden_dim,
+            vector_size=self.hidden_dim,
             window=self.window,
             min_count=self.min_count,
             sample=self.sampling_rate,
             workers=self.n_workers,
-            iter=self.epochs,
+            epochs=self.epochs,
             alpha=self.alpha,
         )
-        vectors = np.asarray([model.wv[str(node)] for node in model.wv.index2word])
+        vectors = np.asarray([model.wv[str(node)] for node in model.wv.index_to_key])
         S = vectors.dot(vectors.T)
-        node2id = dict(zip(model.wv.index2word, range(len(model.wv.index2word))))
+        node2id = dict(zip(model.wv.index_to_key, range(len(model.wv.index_to_key))))
 
         num_graph, size_vocab = len(graphs), len(node2id)
         norm_prob = np.zeros((num_graph, size_vocab))
         for i, gls in enumerate(self.gl_collections):
             for gl in gls:
                 if gl in node2id:
                     norm_prob[i, node2id[gl]] += 1
```

### Comparing `cogdl-0.5.3/cogdl/models/emb/dngr.py` & `cogdl-0.6/cogdl/models/emb/dngr.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/emb/gatne.py` & `cogdl-0.6/cogdl/models/emb/gatne.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import networkx as nx
 from collections import defaultdict
-from gensim.models.keyedvectors import Vocab
+from gensim.models.keyedvectors import Vocab  # Retained for now to ease the loading of older models.
+# See: https://radimrehurek.com/gensim/models/keyedvectors.html?highlight=vocab#gensim.models.keyedvectors.CompatVocab
 import random
 import math
 import tqdm
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn.parameter import Parameter
@@ -106,20 +107,20 @@
         self.neighbor_samples = neighbor_samples
         self.schema = schema
         self.multiplicity = True
 
     def forward(self, network_data):
         device = "cpu" if not torch.cuda.is_available() else "cuda"
         all_walks = generate_walks(network_data, self.walk_num, self.walk_length, schema=self.schema)
-        vocab, index2word = generate_vocab(all_walks)
+        vocab, index_to_key = generate_vocab(all_walks)
         train_pairs = generate_pairs(all_walks, vocab)
 
         edge_types = list(network_data.keys())
 
-        num_nodes = len(index2word)
+        num_nodes = len(index_to_key)
         edge_type_count = len(edge_types)
 
         epochs = self.epochs
         batch_size = self.batch_size
         embedding_size = self.embedding_size
         embedding_u_size = self.embedding_u_size
         num_sampled = self.num_sampled
@@ -135,20 +136,15 @@
                 neighbors[ix][r].append(iy)
                 neighbors[iy][r].append(ix)
             for i in range(num_nodes):
                 if len(neighbors[i][r]) == 0:
                     neighbors[i][r] = [i] * neighbor_samples
                 elif len(neighbors[i][r]) < neighbor_samples:
                     neighbors[i][r].extend(
-                        list(
-                            np.random.choice(
-                                neighbors[i][r],
-                                size=neighbor_samples - len(neighbors[i][r]),
-                            )
-                        )
+                        list(np.random.choice(neighbors[i][r], size=neighbor_samples - len(neighbors[i][r]),))
                     )
                 elif len(neighbors[i][r]) > neighbor_samples:
                     neighbors[i][r] = list(np.random.choice(neighbors[i][r], size=neighbor_samples))
 
         model = GATNEModel(num_nodes, embedding_size, embedding_u_size, edge_type_count, dim_att)
         nsloss = NSLoss(num_nodes, num_sampled, embedding_size)
 
@@ -167,19 +163,15 @@
                 total=(len(train_pairs) + (batch_size - 1)) // batch_size,
                 bar_format="{l_bar}{r_bar}",
             )
             avg_loss = 0.0
 
             for i, data in enumerate(data_iter):
                 optimizer.zero_grad()
-                embs = model(
-                    data[0].to(device),
-                    data[2].to(device),
-                    data[3].to(device),
-                )
+                embs = model(data[0].to(device), data[2].to(device), data[3].to(device),)
                 loss = nsloss(data[0].to(device), embs, data[1].to(device))
                 loss.backward()
                 optimizer.step()
 
                 avg_loss += loss.item()
 
                 if i % 5000 == 0:
@@ -194,15 +186,15 @@
         final_model = dict(zip(edge_types, [dict() for _ in range(edge_type_count)]))
         for i in range(num_nodes):
             train_inputs = torch.tensor([i for _ in range(edge_type_count)]).to(device)
             train_types = torch.tensor(list(range(edge_type_count))).to(device)
             node_neigh = torch.tensor([neighbors[i] for _ in range(edge_type_count)]).to(device)
             node_emb = model(train_inputs, train_types, node_neigh)
             for j in range(edge_type_count):
-                final_model[edge_types[j]][index2word[i]] = node_emb[j].cpu().detach().numpy()
+                final_model[edge_types[j]][index_to_key[i]] = node_emb[j].cpu().detach().numpy()
         return final_model
 
 
 class GATNEModel(nn.Module):
     def __init__(self, num_nodes, embedding_size, embedding_u_size, edge_type_count, dim_a):
         super(GATNEModel, self).__init__()
         self.num_nodes = num_nodes
@@ -226,16 +218,15 @@
         self.trans_weights_s1.data.normal_(std=1.0 / math.sqrt(self.embedding_size))
         self.trans_weights_s2.data.normal_(std=1.0 / math.sqrt(self.embedding_size))
 
     def forward(self, train_inputs, train_types, node_neigh):
         node_embed = self.node_embeddings[train_inputs]
         node_embed_neighbors = self.node_type_embeddings[node_neigh]
         node_embed_tmp = torch.cat(
-            [node_embed_neighbors[:, i, :, i, :].unsqueeze(1) for i in range(self.edge_type_count)],
-            dim=1,
+            [node_embed_neighbors[:, i, :, i, :].unsqueeze(1) for i in range(self.edge_type_count)], dim=1,
         )
         node_type_embed = torch.sum(node_embed_tmp, dim=2)
 
         trans_w = self.trans_weights[train_types]
         trans_w_s1 = self.trans_weights_s1[train_types]
         trans_w_s2 = self.trans_weights_s2[train_types]
 
@@ -317,21 +308,15 @@
             random.shuffle(nodes)
             for node in nodes:
                 if schema is None:
                     walks.append(self.walk(walk_length=walk_length, start=node))
                 else:
                     for schema_iter in schema_list:
                         if schema_iter.split("-")[0] == self.node_type[node]:
-                            walks.append(
-                                self.walk(
-                                    walk_length=walk_length,
-                                    start=node,
-                                    schema=schema_iter,
-                                )
-                            )
+                            walks.append(self.walk(walk_length=walk_length, start=node, schema=schema_iter,))
 
         return walks
 
 
 def get_G_from_edges(edges):
     edge_dict = dict()
     for edge in edges:
@@ -361,32 +346,32 @@
                         pairs.append((vocab[walk[i]].index, vocab[walk[i - j]].index, layer_id))
                     if i + j < len(walk):
                         pairs.append((vocab[walk[i]].index, vocab[walk[i + j]].index, layer_id))
     return pairs
 
 
 def generate_vocab(all_walks):
-    index2word = []
+    index_to_key = []
     raw_vocab = defaultdict(int)
 
     for walks in all_walks:
         for walk in walks:
             for word in walk:
                 raw_vocab[word] += 1
 
     vocab = {}
     for word, v in raw_vocab.items():
-        vocab[word] = Vocab(count=v, index=len(index2word))
-        index2word.append(word)
+        vocab[word] = Vocab(count=v, index=len(index_to_key))
+        index_to_key.append(word)
 
-    index2word.sort(key=lambda word: vocab[word].count, reverse=True)
-    for i, word in enumerate(index2word):
+    index_to_key.sort(key=lambda word: vocab[word].count, reverse=True)
+    for i, word in enumerate(index_to_key):
         vocab[word].index = i
 
-    return vocab, index2word
+    return vocab, index_to_key
 
 
 def get_batches(pairs, neighbors, batch_size):
     n_batches = (len(pairs) + (batch_size - 1)) // batch_size
 
     # result = []
     for idx in range(n_batches):
```

### Comparing `cogdl-0.5.3/cogdl/models/emb/graph2vec.py` & `cogdl-0.6/cogdl/models/emb/graph2vec.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/emb/grarep.py` & `cogdl-0.6/cogdl/models/emb/grarep.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/emb/hin2vec.py` & `cogdl-0.6/cogdl/models/emb/hin2vec.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,17 +43,15 @@
         self.re_embr = self.regulartion(self.embr)
         self.preds = torch.unsqueeze(
             torch.sigmoid(torch.sum(torch.mul(torch.mul(self.embx, self.emby), self.re_embr), 1)), 1
         )
         self.logits = torch.cat((self.preds, 1 - self.preds), 1)
         return self.logits, self.criterion(self.logits, l)
 
-    def get_emb(
-        self,
-    ):
+    def get_emb(self,):
         x = F.one_hot(torch.arange(0, self.num_node), num_classes=self.num_node).float().to(self.device)
         return torch.mm(x, self.Wx)
 
 
 class RWgraph:
     def __init__(self, nx_G, node_type=None):
         self.G = nx_G
```

### Comparing `cogdl-0.5.3/cogdl/models/emb/hope.py` & `cogdl-0.6/cogdl/models/emb/hope.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/emb/line.py` & `cogdl-0.6/cogdl/models/emb/line.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,15 @@
                             help="Order of proximity in LINE. Default is 3 for 1+2.")
         parser.add_argument("--hidden-size", type=int, default=128)
         # fmt: on
 
     @classmethod
     def build_model_from_args(cls, args):
         return cls(
-            args.hidden_size,
-            args.walk_length,
-            args.walk_num,
-            args.negative,
-            args.batch_size,
-            args.alpha,
-            args.order,
+            args.hidden_size, args.walk_length, args.walk_num, args.negative, args.batch_size, args.alpha, args.order,
         )
 
     def __init__(self, dimension, walk_length, walk_num, negative, batch_size, alpha, order):
         super(LINE, self).__init__()
         self.dimension = dimension
         self.walk_length = walk_length
         self.walk_num = walk_num
```

### Comparing `cogdl-0.5.3/cogdl/models/emb/metapath2vec.py` & `cogdl-0.6/cogdl/models/emb/metapath2vec.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,20 +69,20 @@
         G.add_edges_from(list(zip(row.numpy(), col.numpy())))
         self.G = G
         self.node_type = [str(a) for a in data.pos.tolist()]
         walks = self._simulate_walks(self.walk_length, self.walk_num, self.schema)
         walks = [[str(node) for node in walk] for walk in walks]
         model = Word2Vec(
             walks,
-            size=self.dimension,
+            vector_size=self.dimension,
             window=self.window_size,
             min_count=0,
             sg=1,
             workers=self.worker,
-            iter=self.iteration,
+            epochs=self.iteration,
         )
         id2node = dict([(vid, node) for vid, node in enumerate(G.nodes())])
         embeddings = np.asarray([model.wv[str(id2node[i])] for i in range(len(id2node))])
         return embeddings
 
     def _walk(self, start_node, walk_length, schema=None):
         # Simulate a random walk starting from start node.
```

### Comparing `cogdl-0.5.3/cogdl/models/emb/netmf.py` & `cogdl-0.6/cogdl/models/emb/netmf.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,15 @@
 
     def _deepwalk_filter(self, evals, window):
         for i in range(len(evals)):
             x = evals[i]
             evals[i] = 1.0 if x >= 1 else x * (1 - x ** window) / (1 - x) / window
         evals = np.maximum(evals, 0)
         print(
-            "After filtering, max eigenvalue=%f, min eigenvalue=%f",
-            np.max(evals),
-            np.min(evals),
+            "After filtering, max eigenvalue=%f, min eigenvalue=%f", np.max(evals), np.min(evals),
         )
         return evals
 
     def _approximate_deepwalk_matrix(self, evals, D_rt_invU, window, vol, b):
         # approximate deepwalk matrix
         evals = self._deepwalk_filter(evals, window=window)
         X = sp.diags(np.sqrt(evals)).dot(D_rt_invU.T).T
```

### Comparing `cogdl-0.5.3/cogdl/models/emb/netsmf.py` & `cogdl-0.6/cogdl/models/emb/netsmf.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,15 @@
         parser.add_argument("--worker", type=int, default=10,
                             help="Number of parallel workers. Default is 10.")
         parser.add_argument("--hidden-size", type=int, default=128)
         # fmt: on
 
     @classmethod
     def build_model_from_args(cls, args):
-        return cls(
-            args.hidden_size,
-            args.window_size,
-            args.negative,
-            args.num_round,
-            args.worker,
-        )
+        return cls(args.hidden_size, args.window_size, args.negative, args.num_round, args.worker,)
 
     def __init__(self, dimension, window_size, negative, num_round, worker):
         super(NetSMF, self).__init__()
         self.dimension = dimension
         self.window_size = window_size
         self.negative = negative
         self.worker = worker
@@ -72,20 +66,15 @@
         self.alias_nodes = {}
         self.node_weight = {}
         for i in range(self.num_node):
             unnormalized_probs = [self.G[id2node[i]][nbr].get("weight", 1.0) for nbr in self.G.neighbors(id2node[i])]
             norm_const = sum(unnormalized_probs)
             normalized_probs = [float(u_prob) / norm_const for u_prob in unnormalized_probs]
             self.alias_nodes[i] = alias_setup(normalized_probs)
-            self.node_weight[i] = dict(
-                zip(
-                    [node2id[nbr] for nbr in self.G.neighbors(id2node[i])],
-                    unnormalized_probs,
-                )
-            )
+            self.node_weight[i] = dict(zip([node2id[nbr] for nbr in self.G.neighbors(id2node[i])], unnormalized_probs,))
 
         t = time.time()
         print("alias_nodes", t - s)
 
         # run netsmf algorithm with multiprocessing and apply randomized svd
         print("number of sample edges ", self.num_round * self.num_edge * self.window_size)
         print("random walk start...")
```

### Comparing `cogdl-0.5.3/cogdl/models/emb/node2vec.py` & `cogdl-0.6/cogdl/models/emb/node2vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,20 +78,20 @@
             if not is_directed:
                 G[j][i]["weight"] = G[j][i].get("weight", 1.0)
         self._preprocess_transition_probs()
         walks = self._simulate_walks(self.walk_num, self.walk_length)
         walks = [[str(node) for node in walk] for walk in walks]
         model = Word2Vec(
             walks,
-            size=self.dimension,
+            vector_size=self.dimension,
             window=self.window_size,
             min_count=0,
             sg=1,
             workers=self.worker,
-            iter=self.iteration,
+            epochs=self.iteration,
         )
         id2node = dict([(vid, node) for vid, node in enumerate(G.nodes())])
         embeddings = np.asarray([model.wv[str(id2node[i])] for i in range(len(id2node))])
 
         if return_dict:
             features_matrix = dict()
             for vid, node in enumerate(G.nodes()):
```

### Comparing `cogdl-0.5.3/cogdl/models/emb/prone.py` & `cogdl-0.6/cogdl/models/emb/prone.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/emb/pronepp.py` & `cogdl-0.6/cogdl/models/emb/pronepp.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/emb/pte.py` & `cogdl-0.6/cogdl/models/emb/pte.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,22 +36,15 @@
                             help='Batch size in SGD training process. Default is 1000.')
         parser.add_argument('--alpha', type=float, default=0.025,
                             help='Initial learning rate of SGD. Default is 0.025.')
         # fmt: on
 
     @classmethod
     def build_model_from_args(cls, args):
-        return cls(
-            args.hidden_size,
-            args.walk_length,
-            args.walk_num,
-            args.negative,
-            args.batch_size,
-            args.alpha,
-        )
+        return cls(args.hidden_size, args.walk_length, args.walk_num, args.negative, args.batch_size, args.alpha,)
 
     def __init__(self, dimension, walk_length, walk_num, negative, batch_size, alpha):
         super(PTE, self).__init__()
         self.dimension = dimension
         self.walk_length = walk_length
         self.walk_num = walk_num
         self.negative = negative
@@ -116,17 +109,15 @@
     def _update(self, vec_u, vec_v, vec_error, label):
         # update vetex embedding and vec_error
         f = 1 / (1 + np.exp(-np.sum(vec_u * vec_v, axis=1)))
         g = (self.alpha * (label - f)).reshape((len(label), 1))
         vec_error += g * vec_v
         vec_v += g * vec_u
 
-    def _train_line(
-        self,
-    ):
+    def _train_line(self,):
         # train Line model with order
         self.alpha = self.init_alpha
         batch_size = self.batch_size
         t0 = time.time()
         num_batch = int(self.num_sampling_edge / batch_size)
         epoch_iter = tqdm(range(num_batch))
         for b in epoch_iter:
```

### Comparing `cogdl-0.5.3/cogdl/models/emb/sdne.py` & `cogdl-0.6/cogdl/models/emb/sdne.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/emb/spectral.py` & `cogdl-0.6/cogdl/models/emb/spectral.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/__init__.py` & `cogdl-0.6/cogdl/models/nn/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from .compgcn import CompGCN
 from .dgi import DGIModel
 from .disengcn import DisenGCN
 from .gcn import GCN
 from .gcnii import GCNII
 from .gdc_gcn import GDC_GCN
 from .grace import GRACE
-from .graphsage import Graphsage
+from .graphsage import Graphsage, SAGE
 from .mvgrl import MVGRL
 from .patchy_san import PatchySAN
 from .ppnp import PPNP
 from .rgcn import RGCN
 from .sgc import sgc
 from .revgcn import RevGCN, RevGEN, RevGAT
 from .deepergcn import DeeperGCN, ResGNNLayer
+from .stgcn import STGCN
+from .stgat import STGAT
 
 __all__ = [
     "CompGCN",
     "DGIModel",
     "DisenGCN",
     "GCN",
     "GCNII",
@@ -29,8 +31,11 @@
     "RGCN",
     "sgc",
     "RevGCN",
     "RevGAT",
     "RevGEN",
     "DeeperGCN",
     "ResGNNLayer",
+    "SAGE",
+    "STGCN",
+    "STGAT",
 ]
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/actgcn.py` & `cogdl-0.6/cogdl/models/nn/actgcn.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/agc.py` & `cogdl-0.6/cogdl/models/nn/agc.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/autognn.py` & `cogdl-0.6/cogdl/models/nn/autognn.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,22 +51,15 @@
             )
         )
         layers.append(nn.ELU())
 
     if dropout > 0.0:
         layers.append(nn.Dropout(p=dropout))
     layers.append(
-        GATLayer(
-            hidden_size * nhead,
-            out_feats,
-            attn_drop=attn_drop,
-            alpha=alpha,
-            nhead=last_nhead,
-            residual=False,
-        )
+        GATLayer(hidden_size * nhead, out_feats, attn_drop=attn_drop, alpha=alpha, nhead=last_nhead, residual=False,)
     )
 
     return layers
 
 
 def grand_model(in_feats, hidden_size, out_feats, dropout, dropout2, norm):
     layers = nn.ModuleList()
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/compgcn.py` & `cogdl-0.6/cogdl/models/nn/compgcn.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/correct_smooth.py` & `cogdl-0.6/cogdl/models/nn/correct_smooth.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/daegc.py` & `cogdl-0.6/cogdl/models/nn/daegc.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/deepergcn.py` & `cogdl-0.6/cogdl/models/nn/deepergcn.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/dgi.py` & `cogdl-0.6/cogdl/models/nn/dgi.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/diffpool.py` & `cogdl-0.6/cogdl/models/nn/diffpool.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/disengcn.py` & `cogdl-0.6/cogdl/models/nn/disengcn.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/drgat.py` & `cogdl-0.6/cogdl/models/nn/drgat.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,21 +16,15 @@
         parser.add_argument("--hidden-size", type=int, default=8)
         parser.add_argument("--nhead", type=int, default=8)
         parser.add_argument("--dropout", type=float, default=0.6)
         # fmt: on
 
     @classmethod
     def build_model_from_args(cls, args):
-        return cls(
-            args.num_features,
-            args.num_classes,
-            args.hidden_size,
-            args.nhead,
-            args.dropout,
-        )
+        return cls(args.num_features, args.num_classes, args.hidden_size, args.nhead, args.dropout,)
 
     def __init__(self, num_features, num_classes, hidden_size, num_heads, dropout):
         super(DrGAT, self).__init__()
         self.num_features = num_features
         self.num_classes = num_classes
         self.hidden_size = hidden_size
         self.num_heads = num_heads
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/drgcn.py` & `cogdl-0.6/cogdl/models/nn/drgcn.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/dropedge_gcn.py` & `cogdl-0.6/cogdl/models/nn/dropedge_gcn.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,22 +12,15 @@
 
 class GraphConvolutionBS(Module):
     """
     GCN Layer with BN, Self-loop and Res connection.
     """
 
     def __init__(
-        self,
-        in_features,
-        out_features,
-        activation=lambda x: x,
-        withbn=True,
-        withloop=True,
-        bias=True,
-        res=False,
+        self, in_features, out_features, activation=lambda x: x, withbn=True, withloop=True, bias=True, res=False,
     ):
         """
         Initial function.
         :param in_features: the input feature dimension.
         :param out_features: the output feature dimension.
         :param activation: the activation function.
         :param withbn: using batch normalization.
@@ -133,28 +126,18 @@
             raise NotImplementedError("The aggregation method only support 'concat','add' and 'nores'.")
 
     def __makehidden(self):
         # for i in xrange(self.nhiddenlayer):
         for i in range(self.nhiddenlayer):
             if i == 0:
                 layer = GraphConvolutionBS(
-                    self.in_features,
-                    self.hiddendim,
-                    self.activation,
-                    self.withbn,
-                    self.withloop,
+                    self.in_features, self.hiddendim, self.activation, self.withbn, self.withloop,
                 )
             else:
-                layer = GraphConvolutionBS(
-                    self.hiddendim,
-                    self.hiddendim,
-                    self.activation,
-                    self.withbn,
-                    self.withloop,
-                )
+                layer = GraphConvolutionBS(self.hiddendim, self.hiddendim, self.activation, self.withbn, self.withloop,)
             self.hiddenlayers.append(layer)
 
     def _doconcat(self, x, subx):
         if x is None:
             return subx
         if self.aggrmethod == "concat":
             return torch.cat((x, subx), 1)
@@ -424,27 +407,19 @@
         # for j in xrange(self.nhiddenlayer):
         for j in range(self.nbaselayer):
             reslayer = nn.ModuleList()
             # for i in xrange(j + 1):
             for i in range(j + 1):
                 if i == 0:
                     layer = GraphConvolutionBS(
-                        self.in_features,
-                        self.hiddendim,
-                        self.activation,
-                        self.withbn,
-                        self.withloop,
+                        self.in_features, self.hiddendim, self.activation, self.withbn, self.withloop,
                     )
                 else:
                     layer = GraphConvolutionBS(
-                        self.hiddendim,
-                        self.hiddendim,
-                        self.activation,
-                        self.withbn,
-                        self.withloop,
+                        self.hiddendim, self.hiddendim, self.activation, self.withbn, self.withloop,
                     )
                 reslayer.append(layer)
             self.midlayers.append(reslayer)
 
     def forward(self, graph, x):
         for reslayer in self.midlayers:
             subx = x
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/gae.py` & `cogdl-0.6/cogdl/models/nn/gae.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/gat.py` & `cogdl-0.6/cogdl/models/nn/gat.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,20 +82,15 @@
                     alpha=alpha,
                     residual=residual,
                     norm=norm,
                 )
             )
         self.attentions.append(
             GATLayer(
-                hidden_size * nhead,
-                out_features,
-                attn_drop=attn_drop,
-                alpha=alpha,
-                nhead=last_nhead,
-                residual=False,
+                hidden_size * nhead, out_features, attn_drop=attn_drop, alpha=alpha, nhead=last_nhead, residual=False,
             )
         )
         self.num_layers = num_layers
         self.last_nhead = last_nhead
         self.residual = residual
 
     def forward(self, graph):
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/gcc_model.py` & `cogdl-0.6/cogdl/models/nn/gcc_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,25 +64,26 @@
         out_feats,
         num_mlp_layers,
         eps=0,
         pooling="sum",
         train_eps=False,
         dropout=0.5,
         final_dropout=0.2,
+        use_selayer=False,
     ):
         super(GINModel, self).__init__()
         self.gin_layers = nn.ModuleList()
         self.batch_norm = nn.ModuleList()
         self.num_layers = num_layers
         for i in range(num_layers - 1):
             if i == 0:
                 mlp = MLP(in_feats, hidden_dim, hidden_dim, num_mlp_layers, norm="batchnorm")
             else:
                 mlp = MLP(hidden_dim, hidden_dim, hidden_dim, num_mlp_layers, norm="batchnorm")
-            self.gin_layers.append(GINLayer(mlp, eps, train_eps))
+            self.gin_layers.append(GINLayer(ApplyNodeFunc(mlp, use_selayer), eps, train_eps))
             self.batch_norm.append(nn.BatchNorm1d(hidden_dim))
 
         self.linear_prediction = nn.ModuleList()
         for i in range(self.num_layers):
             if i == 0:
                 self.linear_prediction.append(nn.Linear(in_feats, out_feats))
             else:
@@ -151,30 +152,36 @@
         parser.add_argument("--hidden-size", type=int, default=64)
         parser.add_argument("--positional-embedding-size", type=int, default=32)
         parser.add_argument("--degree-embedding-size", type=int, default=16)
         parser.add_argument("--max-node-freq", type=int, default=16)
         parser.add_argument("--max-edge-freq", type=int, default=16)
         parser.add_argument("--max-degree", type=int, default=512)
         parser.add_argument("--freq-embedding-size", type=int, default=16)
-        parser.add_argument("--num-layers", type=int, default=2)
+        parser.add_argument("--num-layers", type=int, default=5)
         parser.add_argument("--num-heads", type=int, default=2)
-        parser.add_argument("--output-size", type=int, default=32)
+        parser.add_argument("--output-size", type=int, default=64)
+        parser.add_argument("--norm", type=bool, default=True)
+        parser.add_argument("--gnn-model", type=str, default="gin")
+        parser.add_argument("--degree-input", type=bool, default=True)
 
     @classmethod
     def build_model_from_args(cls, args):
         return cls(
             positional_embedding_size=args.positional_embedding_size,
             max_node_freq=args.max_node_freq,
             max_edge_freq=args.max_edge_freq,
             max_degree=args.max_degree,
             num_layers=args.num_layers,
             num_heads=args.num_heads,
             degree_embedding_size=args.degree_embedding_size,
             node_hidden_dim=args.hidden_size,
+            norm=args.norm,
+            gnn_model=args.gnn_model,
             output_dim=args.output_size,
+            degree_input=args.degree_input
         )
 
     def __init__(
         self,
         positional_embedding_size=32,
         max_node_freq=8,
         max_edge_freq=8,
@@ -186,15 +193,15 @@
         edge_hidden_dim=32,
         num_layers=6,
         num_heads=4,
         num_step_set2set=6,
         num_layer_set2set=3,
         norm=False,
         gnn_model="gin",
-        degree_input=False,
+        degree_input=True,
     ):
         super(GCCModel, self).__init__()
 
         if degree_input:
             node_input_dim = positional_embedding_size + degree_embedding_size + 1
         else:
             node_input_dim = positional_embedding_size + 1
@@ -225,31 +232,31 @@
             )
         self.gnn_model = gnn_model
 
         self.max_node_freq = max_node_freq
         self.max_edge_freq = max_edge_freq
         self.max_degree = max_degree
         self.degree_input = degree_input
+        self.output_dim = output_dim
+        self.hidden_size = node_hidden_dim
 
         # self.node_freq_embedding = nn.Embedding(
         #     num_embeddings=max_node_freq + 1, embedding_dim=freq_embedding_size
         # )
         if degree_input:
             self.degree_embedding = nn.Embedding(num_embeddings=max_degree + 1, embedding_dim=degree_embedding_size)
 
         # self.edge_freq_embedding = nn.Embedding(
         #     num_embeddings=max_edge_freq + 1, embedding_dim=freq_embedding_size
         # )
 
         self.set2set = Set2Set(node_hidden_dim, num_step_set2set, num_layer_set2set)
         if gnn_model != "gin":
             self.lin_readout = nn.Sequential(
-                nn.Linear(2 * node_hidden_dim, node_hidden_dim),
-                nn.ReLU(),
-                nn.Linear(node_hidden_dim, output_dim),
+                nn.Linear(2 * node_hidden_dim, node_hidden_dim), nn.ReLU(), nn.Linear(node_hidden_dim, output_dim),
             )
         else:
             self.lin_readout = None
         self.norm = norm
 
     def forward(self, g, return_all_outputs=False):
         """Predict molecule labels
@@ -275,14 +282,15 @@
             seed_emb = torch.Tensor(seed_emb)
 
         if self.degree_input:
             degrees = g.degrees()
             if device != torch.device("cpu"):
                 degrees = degrees.cuda(device)
 
+            degrees = degrees.long()
             deg_emb = self.degree_embedding(degrees.clamp(0, self.max_degree))
 
             n_feat = torch.cat((pos_undirected, deg_emb, seed_emb), dim=-1)
         else:
             n_feat = torch.cat(
                 (
                     pos_undirected,
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/gcn.py` & `cogdl-0.6/cogdl/models/nn/gcn.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,23 +39,15 @@
             args.dropout,
             args.activation,
             args.residual,
             args.norm,
         )
 
     def __init__(
-        self,
-        in_feats,
-        hidden_size,
-        out_feats,
-        num_layers,
-        dropout,
-        activation="relu",
-        residual=False,
-        norm=None,
+        self, in_feats, hidden_size, out_feats, num_layers, dropout, activation="relu", residual=False, norm=None,
     ):
         super(GCN, self).__init__()
         shapes = [in_feats] + [hidden_size] * (num_layers - 1) + [out_feats]
         self.layers = nn.ModuleList(
             [
                 GCNLayer(
                     shapes[i],
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/gcnii.py` & `cogdl-0.6/cogdl/models/nn/gcnii.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/gcnmix.py` & `cogdl-0.6/cogdl/models/nn/gcnmix.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/gdc_gcn.py` & `cogdl-0.6/cogdl/models/nn/gdc_gcn.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/gin.py` & `cogdl-0.6/cogdl/models/nn/gin.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/grace.py` & `cogdl-0.6/cogdl/models/nn/grace.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 from cogdl.layers import GCNLayer
 from cogdl.utils import get_activation
 from cogdl.data import Graph
 
 
 class GraceEncoder(nn.Module):
     def __init__(
-        self,
-        in_feats: int,
-        out_feats: int,
-        num_layers: int,
-        activation: str = "relu",
+        self, in_feats: int, out_feats: int, num_layers: int, activation: str = "relu",
     ):
         super(GraceEncoder, self).__init__()
         shapes = [in_feats] + [2 * out_feats] * (num_layers - 1) + [out_feats]
         self.layers = nn.ModuleList([GCNLayer(shapes[i], shapes[i + 1]) for i in range(num_layers)])
         self.activation = get_activation(activation)
 
     def forward(self, graph: Graph, x: torch.Tensor):
@@ -79,17 +75,15 @@
 
         self.project_head = nn.Sequential(
             nn.Linear(hidden_size, proj_hidden_size), nn.ELU(), nn.Linear(proj_hidden_size, hidden_size)
         )
         self.encoder = GraceEncoder(in_feats, hidden_size, num_layers, activation)
 
     def forward(
-        self,
-        graph: Graph,
-        x: torch.Tensor = None,
+        self, graph: Graph, x: torch.Tensor = None,
     ):
         if x is None:
             x = graph.x
         graph.sym_norm()
         return self.encoder(graph, x)
 
     def embed(self, data):
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/grand.py` & `cogdl-0.6/cogdl/models/nn/grand.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,24 +65,15 @@
             args.bn,
             args.dropnode_rate,
             args.order,
             args.alpha,
         )
 
     def __init__(
-        self,
-        nfeat,
-        nhid,
-        nclass,
-        input_droprate,
-        hidden_droprate,
-        use_bn,
-        dropnode_rate,
-        order,
-        alpha,
+        self, nfeat, nhid, nclass, input_droprate, hidden_droprate, use_bn, dropnode_rate, order, alpha,
     ):
         super(Grand, self).__init__()
         self.layer1 = nn.Linear(nfeat, nhid)
         self.layer2 = nn.Linear(nhid, nclass)
         self.input_droprate = input_droprate
         self.hidden_droprate = hidden_droprate
         self.bn1 = nn.BatchNorm1d(nfeat)
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/graph_unet.py` & `cogdl-0.6/cogdl/models/nn/graph_unet.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/graphsage.py` & `cogdl-0.6/cogdl/models/nn/graphsage.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,15 @@
             edge_index_sp = self.sampling(graph.edge_index, self.sample_size[i]).to(x.device)
             with graph.local_graph():
                 graph.edge_index = edge_index_sp
                 x = self.convs[i](graph, x)
             if i != self.num_layers - 1:
                 x = F.relu(x)
                 x = F.dropout(x, p=self.dropout, training=self.training)
+        self.adjlist.clear()
         return x
 
     def forward(self, *args):
         if isinstance(args[0], Graph):
             return self.mini_forward(*args)
         else:
             device = next(self.parameters()).device
@@ -184,7 +185,23 @@
         )
 
     def forward(self, graph):
         x = graph.x
         for layer in self.layers:
             x = layer(graph, x)
         return x
+
+class UnsupGraphsage(Graphsage):
+    def __init__(self, num_features, num_classes, hidden_size, num_layers, sample_size, dropout, aggr):
+        super(Graphsage, self).__init__()
+        assert num_layers == len(sample_size)
+        self.adjlist = {}
+        self.num_features = num_features
+        self.num_classes = num_classes
+        self.hidden_size = hidden_size
+        self.num_layers = num_layers
+        self.sample_size = sample_size
+        self.dropout = dropout
+        shapes = [num_features] + hidden_size * num_layers
+        self.convs = nn.ModuleList(
+            [SAGELayer(shapes[layer], shapes[layer + 1], aggr=aggr) for layer in range(num_layers)]
+        )
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/graphsaint.py` & `cogdl-0.6/cogdl/models/nn/graphsaint.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/gtn.py` & `cogdl-0.6/cogdl/models/nn/gtn.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/han.py` & `cogdl-0.6/cogdl/models/nn/han.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,20 +17,15 @@
         parser.add_argument("--num-layers", type=int, default=2)
         parser.add_argument("--num-edge", type=int, default=2)
         # fmt: on
 
     @classmethod
     def build_model_from_args(cls, args):
         return cls(
-            args.num_edge,
-            args.num_features,
-            args.hidden_size,
-            args.num_classes,
-            args.num_nodes,
-            args.num_layers,
+            args.num_edge, args.num_features, args.hidden_size, args.num_classes, args.num_nodes, args.num_layers,
         )
 
     def __init__(self, num_edge, w_in, w_out, num_class, num_nodes, num_layers):
         super(HAN, self).__init__()
         self.num_edge = num_edge
         self.num_nodes = num_nodes
         self.w_in = w_in
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/infograph.py` & `cogdl-0.6/cogdl/models/nn/infograph.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/m3s.py` & `cogdl-0.6/cogdl/models/nn/m3s.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,20 +20,15 @@
         parser.add_argument("--num-new-labels", type=int, default=2)
         parser.add_argument("--alpha", type=float, default=1)
         parser.add_argument("--approximate", action="store_true")
         # fmt: on
 
     @classmethod
     def build_model_from_args(cls, args):
-        return cls(
-            args.num_features,
-            args.hidden_size,
-            args.num_classes,
-            args.dropout,
-        )
+        return cls(args.num_features, args.hidden_size, args.num_classes, args.dropout,)
 
     def __init__(self, num_features, hidden_size, num_classes, dropout):
         super(M3S, self).__init__()
         self.dropout = dropout
         self.gcn1 = GCNLayer(num_features, hidden_size)
         self.gcn2 = GCNLayer(hidden_size, num_classes)
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/mixhop.py` & `cogdl-0.6/cogdl/models/nn/mixhop.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,15 @@
         parser.add_argument("--dropout", type=float, default=0.7)
         parser.add_argument("--layer1-pows", type=int, nargs="+", default=[200, 200, 200])
         parser.add_argument("--layer2-pows", type=int, nargs="+", default=[20, 20, 20])
         # fmt: on
 
     @classmethod
     def build_model_from_args(cls, args):
-        return cls(
-            args.num_features,
-            args.num_classes,
-            args.dropout,
-            args.layer1_pows,
-            args.layer2_pows,
-        )
+        return cls(args.num_features, args.num_classes, args.dropout, args.layer1_pows, args.layer2_pows,)
 
     def __init__(self, num_features, num_classes, dropout, layer1_pows, layer2_pows):
         super(MixHop, self).__init__()
 
         self.dropout = dropout
 
         self.num_features = num_features
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/mlp.py` & `cogdl-0.6/cogdl/models/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/moe_gcn.py` & `cogdl-0.6/cogdl/models/nn/moe_gcn.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,21 +107,15 @@
             "dropout": dropout,
             "norm": norm,
             "residual": residual,
             "activation": activation,
         }
         self.layers = nn.ModuleList(
             [
-                GraphConvBlock(
-                    conv_func,
-                    conv_params,
-                    shapes[i],
-                    shapes[i + 1],
-                    dropout=dropout,
-                )
+                GraphConvBlock(conv_func, conv_params, shapes[i], shapes[i + 1], dropout=dropout,)
                 for i in range(num_layers)
             ]
         )
         self.num_layers = num_layers
         self.dropout = dropout
         self.act = get_activation(activation)
         self.final_cls = nn.Linear(hidden_size, out_feats)
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/mvgrl.py` & `cogdl-0.6/cogdl/models/nn/mvgrl.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/patchy_san.py` & `cogdl-0.6/cogdl/models/nn/patchy_san.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/ppnp.py` & `cogdl-0.6/cogdl/models/nn/ppnp.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,15 @@
 
     def forward(self, graph):
         def get_ready_format(input, edge_index, edge_attr=None):
             if isinstance(edge_index, tuple):
                 edge_index = torch.stack(edge_index)
             if edge_attr is None:
                 edge_attr = torch.ones(edge_index.shape[1]).float().to(input.device)
-            adj = torch.sparse_coo_tensor(
-                edge_index,
-                edge_attr,
-                (input.shape[0], input.shape[0]),
-            ).to(input.device)
+            adj = torch.sparse_coo_tensor(edge_index, edge_attr, (input.shape[0], input.shape[0]),).to(input.device)
             return adj
 
         x = graph.x
         graph.sym_norm()
         # get prediction
         x = F.dropout(x, p=self.dropout, training=self.training)
         local_preds = self.nn.forward(x)
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/pprgo.py` & `cogdl-0.6/cogdl/models/nn/pprgo.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/revgcn.py` & `cogdl-0.6/cogdl/models/nn/revgcn.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,28 +61,19 @@
         self.num_layers = num_layers
         self.layers = nn.ModuleList()
         self.norm = get_norm_layer(norm, hidden_size)
         self.act = get_activation(activation)
 
         for i in range(num_layers):
             if i == 0:
-                self.layers.append(
-                    GCNLayer(
-                        in_feats,
-                        hidden_size,
-                        residual=True,
-                    )
-                )
+                self.layers.append(GCNLayer(in_feats, hidden_size, residual=True,))
             elif i == num_layers - 1:
                 self.layers.append(GCNLayer(hidden_size, out_feats, residual=True))
             else:
-                conv = GCNLayer(
-                    hidden_size // group,
-                    hidden_size // group,
-                )
+                conv = GCNLayer(hidden_size // group, hidden_size // group,)
                 res_conv = ResGNNLayer(
                     conv,
                     hidden_size // group,
                     activation=activation,
                     norm=norm,
                     out_norm=norm,
                     out_channels=hidden_size // group,
@@ -257,33 +248,20 @@
         self.dropout = dropout
         self.num_layers = num_layers
         self.layers = nn.ModuleList()
         self.norm = get_norm_layer(norm, hidden_size * nhead)
         self.act = get_activation(activation)
         for i in range(num_layers):
             if i == 0:
-                self.layers.append(
-                    GATLayer(
-                        in_feats,
-                        hidden_size,
-                        nhead,
-                        alpha,
-                        attn_drop,
-                        residual=True,
-                    )
-                )
+                self.layers.append(GATLayer(in_feats, hidden_size, nhead, alpha, attn_drop, residual=True,))
             elif i == num_layers - 1:
                 self.layers.append(GATLayer(hidden_size * nhead, out_feats, 1, alpha, attn_drop, residual=True))
             else:
                 conv = GATLayer(
-                    hidden_size * nhead // group,
-                    hidden_size // group,
-                    nhead=nhead,
-                    alpha=alpha,
-                    attn_drop=attn_drop,
+                    hidden_size * nhead // group, hidden_size // group, nhead=nhead, alpha=alpha, attn_drop=attn_drop,
                 )
                 res_conv = ResGNNLayer(
                     conv,
                     hidden_size * nhead // group,
                     activation=activation,
                     norm=norm,
                     out_norm=norm,
```

### Comparing `cogdl-0.5.3/cogdl/models/nn/rgcn.py` & `cogdl-0.6/cogdl/models/nn/rgcn.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/sagn.py` & `cogdl-0.6/cogdl/models/nn/sagn.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/sgc.py` & `cogdl-0.6/cogdl/models/nn/sgc.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/sign.py` & `cogdl-0.6/cogdl/models/nn/sign.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/sortpool.py` & `cogdl-0.6/cogdl/models/nn/sortpool.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/models/nn/srgcn.py` & `cogdl-0.6/cogdl/models/nn/srgcn.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/oag/bert_model.py` & `cogdl-0.6/cogdl/oag/bert_model.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/oag/dual_position_bert_model.py` & `cogdl-0.6/cogdl/oag/dual_position_bert_model.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/oag/oagbert.py` & `cogdl-0.6/cogdl/oag/oagbert.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/oag/oagbert_metainfo.py` & `cogdl-0.6/cogdl/oag/oagbert_metainfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,22 +338,23 @@
             "pooled_output": [],
         }
 
         output = {"text": [], "venue": [], "authors": [], "concepts": [], "affiliations": []}
 
         split_index = {"text": [], "venue": [], "authors": [], "concepts": [], "affiliations": []}
 
+        device = next(self.parameters()).device
         sequence_output, pooled_output = self.bert.forward(
-            input_ids=torch.LongTensor(input_ids).unsqueeze(0),
-            token_type_ids=torch.LongTensor(token_type_ids).unsqueeze(0),
-            attention_mask=torch.LongTensor(input_masks).unsqueeze(0),
+            input_ids=torch.LongTensor(input_ids).unsqueeze(0).to(device),
+            token_type_ids=torch.LongTensor(token_type_ids).unsqueeze(0).to(device),
+            attention_mask=torch.LongTensor(input_masks).unsqueeze(0).to(device),
             output_all_encoded_layers=False,
             checkpoint_activations=False,
-            position_ids=torch.LongTensor(position_ids).unsqueeze(0),
-            position_ids_second=torch.LongTensor(position_ids_second).unsqueeze(0),
+            position_ids=torch.LongTensor(position_ids).unsqueeze(0).to(device),
+            position_ids_second=torch.LongTensor(position_ids_second).unsqueeze(0).to(device),
         )
 
         entities = {0: "text", 2: "venue", 1: "authors", 4: "concepts", 3: "affiliations"}
         for num, name in entities.items():
             if num in token_type_ids:
                 start_index = position_ids[token_type_ids.index(num)]
                 split_index[name].append(position_ids.index(start_index) - 1)
@@ -604,18 +605,15 @@
                         break
 
             if debug:
                 print("beam search, rest length: %d" % (decode_span_length - i))
                 for _input_ids, _masked_lm_labels, _masked_positions, _last_logprob in q:
                     print(
                         "  %8.4f, %s"
-                        % (
-                            _last_logprob,
-                            self._convert_token_ids_to_string(_input_ids[-decode_span_length:]),
-                        )
+                        % (_last_logprob, self._convert_token_ids_to_string(_input_ids[-decode_span_length:]),)
                     )
 
         results = []
         for (_input_ids, _masked_lm_labels, _masked_positions, _logprob) in q:
             generated_entity = self._convert_token_ids_to_text(_input_ids[-decode_span_length:])
             results.append((generated_entity, np.exp(_logprob)))
         return results
```

### Comparing `cogdl-0.5.3/cogdl/oag/utils.py` & `cogdl-0.6/cogdl/oag/utils.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/edge_softmax/edge_softmax.cc` & `cogdl-0.6/cogdl/operators/edge_softmax/edge_softmax.cc`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/edge_softmax/edge_softmax.cu` & `cogdl-0.6/cogdl/operators/edge_softmax/edge_softmax.cu`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/edge_softmax.py` & `cogdl-0.6/cogdl/operators/edge_softmax.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/fused_gat.py` & `cogdl-0.6/cogdl/operators/fused_gat.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/jt_spmm.py` & `cogdl-0.6/cogdl/operators/jt_spmm.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/linear.py` & `cogdl-0.6/cogdl/operators/linear.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/mhspmm.py` & `cogdl-0.6/cogdl/operators/mhspmm.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/ops.py` & `cogdl-0.6/cogdl/operators/ops.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/sample/sample.cpp` & `cogdl-0.6/cogdl/operators/sample/sample.cpp`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/scatter_max/scatter_max.cc` & `cogdl-0.6/cogdl/operators/scatter_max/scatter_max.cc`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/scatter_max/scatter_max.cu` & `cogdl-0.6/cogdl/operators/scatter_max/scatter_max.cu`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/scatter_max.py` & `cogdl-0.6/cogdl/operators/scatter_max.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/computeUtil.h` & `cogdl-0.6/cogdl/operators/spmm/computeUtil.h`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/mhTranspose.cpp` & `cogdl-0.6/cogdl/operators/spmm/mhTranspose.cpp`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/mhTranspose.cu` & `cogdl-0.6/cogdl/operators/spmm/mhTranspose.cu`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/multiheadSddmm.cpp` & `cogdl-0.6/cogdl/operators/spmm/multiheadSddmm.cpp`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/multiheadSddmm.cu` & `cogdl-0.6/cogdl/operators/spmm/multiheadSddmm.cu`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/multiheadSpmm.cpp` & `cogdl-0.6/cogdl/operators/spmm/multiheadSpmm.cpp`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/multiheadSpmm.cu` & `cogdl-0.6/cogdl/operators/spmm/multiheadSpmm.cu`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/sddmm.cpp` & `cogdl-0.6/cogdl/operators/spmm/sddmm.cpp`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/sddmm_kernel.cu` & `cogdl-0.6/cogdl/operators/spmm/sddmm_kernel.cu`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/spmm.cpp` & `cogdl-0.6/cogdl/operators/spmm/spmm.cpp`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/spmm_cpu.cpp` & `cogdl-0.6/cogdl/operators/spmm/spmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm/spmm_kernel.cu` & `cogdl-0.6/cogdl/operators/spmm/spmm_kernel.cu`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/operators/spmm.py` & `cogdl-0.6/cogdl/operators/spmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,15 @@
 
 except Exception:
     csrspmm = None
 
 
 try:
     spmm_cpu = load(
-        name="spmm_cpu",
-        extra_cflags=["-fopenmp"],
-        sources=[os.path.join(path, "spmm/spmm_cpu.cpp")],
-        verbose=False,
+        name="spmm_cpu", extra_cflags=["-fopenmp"], sources=[os.path.join(path, "spmm/spmm_cpu.cpp")], verbose=False,
     )
     spmm_cpu = spmm_cpu.csr_spmm_cpu
 except Exception:
     spmm_cpu = None
 
 
 class SPMMFunction(torch.autograd.Function):
```

### Comparing `cogdl-0.5.3/cogdl/options.py` & `cogdl-0.6/cogdl/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
     parser.add_argument("--seed", default=[1], type=int, nargs="+", metavar="N",
                         help="pseudo random number generator seed")
     parser.add_argument("--epochs", default=500, type=int)
     parser.add_argument("--max-epoch", default=None, type=int)
     parser.add_argument("--patience", type=int, default=100)
     parser.add_argument("--lr", default=0.01, type=float)
     parser.add_argument("--weight-decay", default=0, type=float)
-    parser.add_argument("--n-warmup-steps", type=int, default=0)
+    parser.add_argument("--n-warmup-steps", type=float, default=0.)
     parser.add_argument("--split", default=[0], type=int, nargs="+", metavar="N")
+    parser.add_argument("--clip-grad-norm", default=5., type=float)
 
     parser.add_argument("--checkpoint-path", type=str, default="./checkpoints/model.pt", help="path to save model")
     parser.add_argument("--save-emb-path", type=str, default=None, help="path to save embeddings")
     parser.add_argument("--load-emb-path", type=str, default=None, help="path to load embeddings")
     parser.add_argument("--resume-training", action="store_true")
     parser.add_argument("--logger", type=str, default=None)
     parser.add_argument("--log-path", type=str, default=".", help="path to save logs")
@@ -42,19 +43,21 @@
     parser.add_argument("--cpu-inference", action="store_true", help="do validation and test in cpu")
     parser.add_argument("--distributed", action="store_true")
     parser.add_argument("--progress-bar", type=str, default="epoch")
     parser.add_argument("--local_rank", type=int, default=0)
     parser.add_argument("--master-port", type=int, default=13425)
     parser.add_argument("--master-addr", type=str, default="localhost")
 
-    parser.add_argument("--no-test", action="store_true")
+    parser.add_argument("--return_model", action="store_true")
 
     parser.add_argument("--actnn", action="store_true")
     parser.add_argument("--fp16", action="store_true")
     parser.add_argument("--rp-ratio", type=int, default=1)
+    parser.add_argument("--do_test", default=True)
+    parser.add_argument("--do_valid", default=True)
     # fmt: on
     return parser
 
 
 def add_data_wrapper_args(parser):
     group = parser.add_argument_group("Data wrapper configuration")
     # fmt: off
```

### Comparing `cogdl-0.5.3/cogdl/pipelines.py` & `cogdl-0.6/cogdl/pipelines.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/trainer/controller/data_controller.py` & `cogdl-0.6/cogdl/trainer/controller/data_controller.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/trainer/controller/training_controller.py` & `cogdl-0.6/cogdl/trainer/controller/training_controller.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/trainer/embed_trainer.py` & `cogdl-0.6/cogdl/trainer/embed_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 import time
 from typing import Optional
 import torch
 
 
 class EmbeddingTrainer(object):
     def __init__(
-        self,
-        save_emb_path: Optional[str] = None,
-        load_emb_path: Optional[str] = None,
+        self, save_emb_path: Optional[str] = None, load_emb_path: Optional[str] = None,
     ):
         self.save_emb_path = save_emb_path
         self.load_emb_path = load_emb_path
         self.default_emb_dir = "./embeddings"
 
     def run(self, model_w, dataset_w):
         self.prepare_data_wrapper(dataset_w)
```

### Comparing `cogdl-0.5.3/cogdl/trainer/trainer.py` & `cogdl-0.6/cogdl/trainer/trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,27 @@
 import torch.multiprocessing as mp
 from torch.nn.parallel import DistributedDataParallel
 from torch.cuda.amp import GradScaler, autocast
 
 
 from cogdl.wrappers.data_wrapper.base_data_wrapper import DataWrapper
 from cogdl.wrappers.model_wrapper.base_model_wrapper import ModelWrapper, EmbeddingModelWrapper
-from cogdl.trainer.trainer_utils import evaluation_comp, load_model, save_model, ddp_end, ddp_after_epoch, Printer
+from cogdl.trainer.trainer_utils import (
+    evaluation_comp,
+    load_model,
+    save_model,
+    ddp_end,
+    ddp_after_epoch,
+    Printer,
+)
 from cogdl.trainer.embed_trainer import EmbeddingTrainer
 from cogdl.trainer.controller import DataController
 from cogdl.loggers import build_logger
 from cogdl.data import Graph
+from cogdl.utils.grb_utils import adj_preprocess, updateGraph, adj_to_tensor
 
 
 def move_to_device(batch, device):
     if isinstance(batch, list) or isinstance(batch, tuple):
         if isinstance(batch, tuple):
             batch = list(batch)
         for i, x in enumerate(batch):
@@ -66,18 +74,22 @@
         load_emb_path: Optional[str] = None,
         cpu_inference: bool = False,
         progress_bar: str = "epoch",
         clip_grad_norm: float = 5.0,
         logger: str = None,
         log_path: str = "./runs",
         project: str = "cogdl-exp",
-        no_test: bool = False,
+        return_model: bool = False,
         actnn: bool = False,
         fp16: bool = False,
         rp_ratio: int = 1,
+        attack=None,
+        attack_mode="injection",
+        do_test: bool = True,
+        do_valid: bool = True,
     ):
         self.epochs = epochs
         self.nstage = nstage
         self.patience = patience
         self.early_stopping = early_stopping
         self.eval_step = eval_step
         self.monitor = None
@@ -97,15 +109,15 @@
         self.distributed_inference = distributed_inference
 
         self.master_addr = master_addr
         self.master_port = master_port
 
         self.cpu_inference = cpu_inference
 
-        self.no_test = no_test
+        self.return_model = return_model
 
         self.on_train_batch_transform = None
         self.on_eval_batch_transform = None
         self.clip_grad_norm = clip_grad_norm
 
         self.save_emb_path = save_emb_path
         self.load_emb_path = load_emb_path
@@ -121,14 +133,18 @@
         if distributed_training:
             self.register_training_end_hook(ddp_end)
             self.register_out_epoch_hook(ddp_after_epoch)
 
         self.eval_data_back_to_cpu = False
 
         self.fp16 = fp16
+        self.attack = attack
+        self.attack_mode = attack_mode
+        self.do_test = do_test
+        self.do_valid = do_valid
 
         if actnn:
             try:
                 import actnn
                 from actnn.conf import config
 
                 actnn.set_optimization_level("L3")
@@ -184,35 +200,41 @@
         if self.distributed_training:
             torch.multiprocessing.set_sharing_strategy("file_system")
             self.dist_train(model_w, dataset_w)
         else:
             self.train(self.devices[0], model_w, dataset_w)
         best_model_w = load_model(model_w, self.checkpoint_path).to(self.devices[0])
 
-        if self.no_test:
+        if self.return_model:
             return best_model_w.model
 
         final_test = self.evaluate(best_model_w, dataset_w)
 
         # clear the GPU memory
         dataset = dataset_w.get_dataset()
-        if isinstance(dataset.data, Graph):
+        if isinstance(dataset.data, Graph) or hasattr(dataset.data, "graphs"):
             dataset.data.to("cpu")
 
         return final_test
 
     def evaluate(self, model_w: ModelWrapper, dataset_w: DataWrapper, cpu=False):
         if cpu:
             self.devices = [torch.device("cpu")]
 
         # disable `distributed` to inference once only
         self.distributed_training = False
         dataset_w.prepare_test_data()
-        final_val = self.validate(model_w, dataset_w, self.devices[0])
-        final_test = self.test(model_w, dataset_w, self.devices[0])
+        if self.do_valid:
+            final_val = self.validate(model_w, dataset_w, self.devices[0])
+        else:
+            final_val = {}
+        if self.do_test:
+            final_test = self.test(model_w, dataset_w, self.devices[0])
+        else:
+            final_test = {}
 
         if final_val is not None and "val_metric" in final_val:
             final_val[f"val_{self.evaluation_metric}"] = final_val["val_metric"]
             final_val.pop("val_metric")
             if "val_loss" in final_val:
                 final_val.pop("val_loss")
 
@@ -317,47 +339,70 @@
                 epoch_printer = Printer(epoch_iter.set_description, rank=rank, world_size=self.world_size)
             else:
                 epoch_iter = range(1, self.epochs + 1)
                 epoch_printer = Printer(print, rank=rank, world_size=self.world_size)
 
             self.logger.start()
             print_str_dict = dict()
+            if self.attack is not None:
+                graph = dataset_w.dataset.data
+                graph_backup = copy.deepcopy(graph)
+                graph0 = copy.deepcopy(graph)
+                num_train = torch.sum(graph.train_mask).item()
             for epoch in epoch_iter:
                 for hook in self.pre_epoch_hooks:
                     hook(self)
 
                 # inductive setting ..
                 dataset_w.train()
                 train_loader = dataset_w.on_train_wrapper()
                 train_dataset = train_loader.get_dataset_from_loader()
                 if hasattr(train_dataset, "shuffle"):
                     train_dataset.shuffle()
                 training_loss = self.train_step(model_w, train_loader, optimizers, lr_schedulers, rank, scaler)
 
+                if self.attack is not None:
+                    if self.attack_mode == "injection":
+                        graph0.test_mask = graph0.train_mask
+                    else:
+                        graph0.test_mask[torch.where(graph0.train_mask)[0].multinomial(int(num_train * 0.01))] = True
+                    graph_attack = self.attack.attack(model=model_w.model, graph=graph0, adj_norm_func=None)  # todo
+                    adj_attack = graph_attack.to_scipy_csr()
+                    features_attack = graph_attack.x
+                    adj_train = adj_preprocess(adj=adj_attack, adj_norm_func=None, device=rank)  # todo
+                    n_inject = graph_attack.num_nodes - graph.num_nodes
+                    updateGraph(graph, adj_train, features_attack)
+                    graph.edge_weight = torch.ones(graph.num_edges, device=rank)
+                    graph.train_mask = torch.cat((graph.train_mask, torch.zeros(n_inject, dtype=bool, device=rank)), 0)
+                    graph.val_mask = torch.cat((graph.val_mask, torch.zeros(n_inject, dtype=bool, device=rank)), 0)
+                    graph.test_mask = torch.cat((graph.test_mask, torch.zeros(n_inject, dtype=bool, device=rank)), 0)
+                    graph.y = torch.cat((graph.y, torch.zeros(n_inject, device=rank)), 0)
+                    graph.grb_adj = adj_to_tensor(adj_train).to(rank)
                 print_str_dict["Epoch"] = epoch
                 print_str_dict["train_loss"] = training_loss
 
                 val_loader = dataset_w.on_val_wrapper()
-                if val_loader is not None and epoch % self.eval_step == 0:
-                    # inductive setting ..
-                    dataset_w.eval()
-                    # do validation in inference device
-                    val_result = self.validate(model_w, dataset_w, rank)
-                    if val_result is not None:
-                        monitoring = val_result[self.monitor]
-                        if compare_fn(monitoring, best_index):
-                            best_index = monitoring
-                            best_epoch = epoch
-                            patience = 0
-                            best_model_w = copy.deepcopy(model_w)
-                        else:
-                            patience += 1
-                            if self.early_stopping and patience >= self.patience:
-                                break
-                        print_str_dict[f"val_{self.evaluation_metric}"] = monitoring
+                if self.do_valid is True:
+                    if val_loader is not None and epoch % self.eval_step == 0:
+                        # inductive setting ..
+                        dataset_w.eval()
+                        # do validation in inference device
+                        val_result = self.validate(model_w, dataset_w, rank)
+                        if val_result is not None:
+                            monitoring = val_result[self.monitor]
+                            if compare_fn(monitoring, best_index):
+                                best_index = monitoring
+                                best_epoch = epoch
+                                patience = 0
+                                best_model_w = copy.deepcopy(model_w)
+                            else:
+                                patience += 1
+                                if self.early_stopping and patience >= self.patience:
+                                    break
+                            print_str_dict[f"val_{self.evaluation_metric}"] = monitoring
 
                 if self.distributed_training:
                     if rank == 0:
                         epoch_printer(print_str_dict)
                         self.logger.note(print_str_dict, epoch)
                 else:
                     epoch_printer(print_str_dict)
@@ -369,14 +414,16 @@
             with torch.no_grad():
                 model_w.eval()
                 post_stage_out = model_w.post_stage(stage, dataset_w)
                 dataset_w.post_stage(stage, post_stage_out)
 
             if best_model_w is None:
                 best_model_w = copy.deepcopy(model_w)
+            if self.attack is not None:
+                dataset_w.dataset.data = graph_backup
 
         if self.distributed_training:
             if rank == 0:
                 save_model(best_model_w.to("cpu"), self.checkpoint_path, best_epoch)
                 dist.barrier()
             else:
                 dist.barrier()
```

### Comparing `cogdl-0.5.3/cogdl/trainer/trainer_utils.py` & `cogdl-0.6/cogdl/trainer/trainer_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict
 
 import numpy as np
-
+import os
 import torch
 import torch.distributed as dist
 
 
 def merge_batch_indexes(outputs: list):
     assert len(outputs) > 0
     keys = list(outputs[0].keys())
@@ -49,14 +49,25 @@
     else:
         return 0, bigger_than
 
 
 def save_model(model, path, epoch):
     print(f"Saving {epoch}-th model to {path} ...")
     torch.save(model.state_dict(), path)
+    model = model.model
+    emb_path = os.path.dirname(path)
+    if hasattr(model, "entity_embedding"):
+        entity_embedding = model.entity_embedding.detach().numpy()
+        print('Saving entity_embedding to ', path)
+        np.save(os.path.join(emb_path, "entity_embedding"), entity_embedding) 
+
+    if hasattr(model, "relation_embedding"):
+        relation_embedding = model.relation_embedding.detach().numpy()
+        print('Saving entity_embedding to ', path)
+        np.save(os.path.join(emb_path, "relation_embedding"), relation_embedding)
 
 
 def load_model(model, path):
     print(f"Loading model from {path} ...")
     model.load_state_dict(torch.load(path))
     return model
```

### Comparing `cogdl-0.5.3/cogdl/utils/evaluator.py` & `cogdl-0.6/cogdl/utils/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,35 @@
         if len(self.y_pred) > 0:
             y_pred = torch.cat(self.y_pred, dim=0)
             y_true = torch.cat(self.y_true, dim=0)
             self.clear()
             return self.eval_func(y_pred, y_true)
         return 0
 
+class MAE(object):
+    def __init__(self):
+        super(MAE, self).__init__()
+        self.MAE = list()
+
+    def __call__(self, y_pred, y_true):
+
+        d = np.abs(y_true - y_pred)
+        mae = d.tolist()
+        MAE = np.array(mae).mean()
+        self.MAE.append(MAE)
+        return MAE
+
+    def evaluate(self):
+        if len(self.MAE) > 0:
+            return np.sum(self.MAE) / len(self.MAE)
+        warnings.warn("pre-computing list is empty")
+        return 0
+
+    def clear(self):
+        self.MAE = list()
 
 class Accuracy(object):
     def __init__(self, mini_batch=False):
         super(Accuracy, self).__init__()
         self.mini_batch = mini_batch
         self.tp = list()
         self.total = list()
```

### Comparing `cogdl-0.5.3/cogdl/utils/graph_utils.py` & `cogdl-0.6/cogdl/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/utils/index.py` & `cogdl-0.6/cogdl/utils/index.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/utils/link_prediction_utils.py` & `cogdl-0.6/cogdl/utils/link_prediction_utils.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/utils/optimizer.py` & `cogdl-0.6/cogdl/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/utils/ppr_utils.py` & `cogdl-0.6/cogdl/utils/ppr_utils.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/utils/prone_utils.py` & `cogdl-0.6/cogdl/utils/prone_utils.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/utils/rwalk/__init__.py` & `cogdl-0.6/cogdl/utils/rwalk/__init__.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/utils/sampling.py` & `cogdl-0.6/cogdl/utils/sampling.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,33 @@
 import scipy.sparse as sp
 import random
 
 # from cogdl.utils.rwalk import random_walk as c_random_walk
 
 
 @numba.njit(cache=True, parallel=True)
-def random_walk(start, length, indptr, indices, p=0.0):
+def random_walk_parallel(start, length, indptr, indices, p=0.0):
+    """
+    Parameters:
+        start : np.array(dtype=np.int32)
+        length : int
+        indptr : np.array(dtype=np.int32)
+        indices : np.array(dtype=np.int32)
+        p : float
+    Return:
+        list(np.array(dtype=np.int32))
+    """
+    result = [np.zeros(length, dtype=np.int32)] * len(start)
+    for i in numba.prange(len(start)):
+        result[i] = _random_walk(start[i], length, indptr, indices, p)
+    return result
+
+
+@numba.njit(cache=True)
+def random_walk_single(start, length, indptr, indices, p=0.0):
     """
     Parameters:
         start : np.array(dtype=np.int32)
         length : int
         indptr : np.array(dtype=np.int32)
         indices : np.array(dtype=np.int32)
         p : float
@@ -27,23 +45,27 @@
 
 @numba.njit(cache=True)
 def _random_walk(node, length, indptr, indices, p=0.0):
     result = [numba.int32(0)] * length
     result[0] = numba.int32(node)
     i = numba.int32(1)
     _node = node
+    _start = indptr[_node] 
+    _end = indptr[_node + 1]
     while i < length:
-        start = indptr[node]
+        start = indptr[node] 
         end = indptr[node + 1]
         sample = random.randint(start, end - 1)
         node = indices[sample]
         if np.random.uniform(0, 1) > p:
             result[i] = node
         else:
-            result[i] = _node
+            sample = random.randint(_start, _end - 1)
+            node = indices[sample]
+            result[i] = node
         i += 1
     return np.array(result, dtype=np.int32)
 
 
 class RandomWalker(object):
     def __init__(self, adj=None, num_nodes=None):
         if adj is None:
@@ -72,16 +94,19 @@
             data = np.ones(row.shape[0])
             adj = sp.csr_matrix((data, (row, col)), shape=(num_nodes, num_nodes))
         adj = adj.tocsr()
 
         self.indptr = adj.indptr
         self.indices = adj.indices
 
-    def walk(self, start, walk_length, restart_p=0.0):
+    def walk(self, start, walk_length, restart_p=0.0, parallel=True):
         assert self.indptr is not None, "Please build the adj_list first"
         if isinstance(start, torch.Tensor):
             start = start.cpu().numpy()
         if isinstance(start, list):
             start = np.asarray(start, dtype=np.int32)
-        result = random_walk(start, walk_length, self.indptr, self.indices, restart_p)
+        if parallel:
+            result = random_walk_parallel(start, walk_length, self.indptr, self.indices, restart_p)
+        else:
+            result = random_walk_single(start, walk_length, self.indptr, self.indices, restart_p)
         result = np.array(result, dtype=np.int64)
         return result
```

### Comparing `cogdl-0.5.3/cogdl/utils/spmm_utils.py` & `cogdl-0.6/cogdl/utils/spmm_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,20 @@
         self.fast_spmm_cpu = CONFIGS["fast_spmm_cpu"]
 
     def forward(self, graph, x):
         return spmm_cpu(graph, x, self.fast_spmm_cpu)
 
 
 def spmm(graph, x, actnn=False, fast_spmm=None, fast_spmm_cpu=None):
+    if hasattr(graph, "grb_adj") and graph.grb_adj is not None:
+        if graph.grb_adj.is_sparse:
+            x = torch.sparse.mm(graph.grb_adj, x)
+        else:
+            x = torch.mm(graph.grb_adj, x)
+        return x
     if fast_spmm is None:
         initialize_spmm()
         fast_spmm = CONFIGS["fast_spmm"]
     if fast_spmm_cpu is None:
         initialize_spmm_cpu()
         fast_spmm_cpu = CONFIGS["fast_spmm_cpu"]
     if fast_spmm is not None and str(x.device) != "cpu":
```

### Comparing `cogdl-0.5.3/cogdl/utils/srgcn_utils.py` & `cogdl-0.6/cogdl/utils/srgcn_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,19 +144,15 @@
         res = reduce(fn, result)
         return res._indices(), res._values()
 
 
 class HeatKernel(nn.Module):
     def __init__(self, in_feat):
         super(HeatKernel, self).__init__()
-        self.t = nn.Parameter(
-            torch.zeros(
-                1,
-            )
-        )
+        self.t = nn.Parameter(torch.zeros(1,))
 
     def forward(self, x, edge_index, edge_attr):
         row, col = edge_index
         deg = get_degrees(row, col, x.shape[0])
         deg_inv = deg.pow(-1)
         edge_attr_t = self.t * edge_attr * deg_inv[col] - self.t
         return edge_index, edge_attr_t.exp()
```

### Comparing `cogdl-0.5.3/cogdl/utils/transform.py` & `cogdl-0.6/cogdl/utils/transform.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/utils/utils.py` & `cogdl-0.6/cogdl/utils/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -230,18 +230,15 @@
         if isinstance(variant[1], nn.Module):
             variant = (variant[0], variant[1].model_name)
         tab_data.append(
             [variant]
             + list(
                 itertools.starmap(
                     lambda x, y: f"{x:.4f}±{y:.4f}",
-                    zip(
-                        np.mean(results, axis=0).tolist(),
-                        np.std(results, axis=0).tolist(),
-                    ),
+                    zip(np.mean(results, axis=0).tolist(), np.std(results, axis=0).tolist(),),
                 )
             )
         )
     return tab_data
 
 
 def print_result(results, datasets, model_name):
@@ -284,10 +281,41 @@
     reserved = torch.cuda.memory_reserved(0)
     if print_info:
         print("allocated: %.2f MB" % (allocated / 1024 / 1024), flush=True)
         print("reserved:  %.2f MB" % (reserved / 1024 / 1024), flush=True)
     return allocated
 
 
+def build_model_path(args, model_name):
+    if not hasattr(args, "save_model_path"):
+        args.save_model_path = ""
+    if model_name == "gcc":
+        if hasattr(args, "pretrain") and args.pretrain:
+            model_name_path = "{}_{}_{}_layer_{}_lr_{}_decay_{}_bsz_{}_hid_{}_samples_{}_nce_t_{}_nce_k_{}_rw_hops_{}_restart_prob_{}_aug_{}_ft_{}_deg_{}_pos_{}_momentum_{}".format(
+                "Pretrain" if not args.finetune else "FT", 
+                '_'.join([x.replace('gcc_', '').replace('_', '-') for x in args.dataset.split(' ')]),
+                args.gnn_model,
+                args.num_layers,
+                args.lr,
+                args.weight_decay,
+                args.batch_size,
+                args.hidden_size,
+                args.num_samples,
+                args.nce_t,
+                args.nce_k,
+                args.rw_hops,
+                args.restart_prob,
+                args.aug,
+                args.finetune,
+                args.degree_embedding_size,
+                args.positional_embedding_size,
+                args.momentum,
+            )
+
+            args.save_model_path = os.path.join(args.save_model_path, model_name_path)
+            os.makedirs(args.save_model_path, exist_ok=True)
+    return args
+
+
 if __name__ == "__main__":
     args = build_args_from_dict({"a": 1, "b": 2})
     print(args.a, args.b)
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/__init__.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,18 @@
     else:
         raise NotImplementedError(f"Failed to import {name} DataWrapper.")
     class_name = SUPPORTED_DW[name].split(".")[-1]
     return getattr(module, class_name)
 
 
 SUPPORTED_DW = {
+    "triple_link_prediction_dw": "cogdl.wrappers.data_wrapper.link_prediction.TripleDataWrapper",
     "cluster_dw": "cogdl.wrappers.data_wrapper.node_classification.ClusterWrapper",
     "graphsage_dw": "cogdl.wrappers.data_wrapper.node_classification.GraphSAGEDataWrapper",
+    "unsup_graphsage_dw": "cogdl.wrappers.data_wrapper.node_classification.UnsupGraphSAGEDataWrapper",
     "m3s_dw": "cogdl.wrappers.data_wrapper.node_classification.M3SDataWrapper",
     "network_embedding_dw": "cogdl.wrappers.data_wrapper.node_classification.NetworkEmbeddingDataWrapper",
     "node_classification_dw": "cogdl.wrappers.data_wrapper.node_classification.FullBatchNodeClfDataWrapper",
     "pprgo_dw": "cogdl.wrappers.data_wrapper.node_classification.PPRGoDataWrapper",
     "sagn_dw": "cogdl.wrappers.data_wrapper.node_classification.SAGNDataWrapper",
     "gcc_dw": "cogdl.wrappers.data_wrapper.pretraining.GCCDataWrapper",
     "embedding_link_prediction_dw": "cogdl.wrappers.data_wrapper.link_prediction.EmbeddingLinkPredictionDataWrapper",
@@ -45,8 +47,10 @@
     "heterogeneous_embedding_dw": "cogdl.wrappers.data_wrapper.heterogeneous.HeterogeneousEmbeddingDataWrapper",
     "heterogeneous_gnn_dw": "cogdl.wrappers.data_wrapper.heterogeneous.HeterogeneousGNNDataWrapper",
     "multiplex_embedding_dw": "cogdl.wrappers.data_wrapper.heterogeneous.MultiplexEmbeddingDataWrapper",
     "graph_classification_dw": "cogdl.wrappers.data_wrapper.graph_classification.GraphClassificationDataWrapper",
     "graph_embedding_dw": "cogdl.wrappers.data_wrapper.graph_classification.GraphEmbeddingDataWrapper",
     "infograph_dw": "cogdl.wrappers.data_wrapper.graph_classification.InfoGraphDataWrapper",
     "patchy_san_dw": "cogdl.wrappers.data_wrapper.graph_classification.PATCHY_SAN_DataWrapper",
+    "stgcn_dw": "cogdl.wrappers.data_wrapper.traffic_prediction.STGCNDataWrapper",
+    "stgat_dw": "cogdl.wrappers.data_wrapper.traffic_prediction.STGATDataWrapper",
 }
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/base_data_wrapper.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/base_data_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,21 +150,25 @@
 
     def on_test_wrapper(self):
         return self.__test_data
 
     def train(self):
         if self.__dataset__ is None:
             self.__dataset__ = getattr(self, "dataset", None)
-        if self.__dataset__ is not None and isinstance(self.__dataset__.data, Graph):
+        if self.__dataset__ is not None and \
+                (isinstance(self.__dataset__.data, Graph) 
+                    or hasattr(self.__dataset__.data, "graphs")):
             self.__dataset__.data.train()
 
     def eval(self):
         if self.__dataset__ is None:
             self.__dataset__ = getattr(self, "dataset", None)
-        if self.__dataset__ is not None and isinstance(self.__dataset__.data, Graph):
+        if self.__dataset__ is not None and \
+                (isinstance(self.__dataset__.data, Graph) 
+                    or hasattr(self.__dataset__.data, "graphs")):
             self.__dataset__.data.eval()
 
 
 class OnLoadingWrapper(object):
     def __init__(self, data, transform):
         """
         Args:
@@ -258,15 +262,15 @@
             return None
 
         # if isinstance(inputs, tuple):
         #     inputs = list(inputs)
         if isinstance(inputs, list):
             outputs = [0] * len(inputs)
             for i, item in enumerate(inputs):
-                inputs[i] = self.__get_min_len__(item)
+                outputs[i] = self.__get_min_len__(item)
             return np.min(outputs)
         # elif isinstance(inputs, dict):
         #     outputs = {key: 0 for key in inputs.keys()}
         #     for i, val in enumerate(inputs.values()):
         #         outputs[i] = self.__get_min_len__(val)
         #     return np.min(list(outputs.values()))
         else:
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/graph_classification/graph_classification_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/graph_classification/graph_classification_dw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/graph_classification/graph_embedding_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/graph_classification/graph_embedding_dw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/graph_classification/patchy_san_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/graph_classification/patchy_san_dw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/link_prediction/embedding_link_prediction_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/link_prediction/embedding_link_prediction_dw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/link_prediction/gnn_link_prediction_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/link_prediction/gnn_link_prediction_dw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import torch
-
 from .. import DataWrapper
 
 
 class GNNLinkPredictionDataWrapper(DataWrapper):
     def __init__(self, dataset):
         super(GNNLinkPredictionDataWrapper, self).__init__(dataset)
         self.dataset = dataset
@@ -17,18 +16,17 @@
 
     def test_wrapper(self):
         return self.dataset.data
 
     def pre_transform(self):
         data = self.dataset.data
         num_nodes = data.x.shape[0]
-        (
-            (train_edges, val_edges, test_edges),
-            (val_false_edges, test_false_edges),
-        ) = self.train_test_edge_split(data.edge_index, num_nodes)
+        ((train_edges, val_edges, test_edges), (val_false_edges, test_false_edges),) = self.train_test_edge_split(
+            data.edge_index, num_nodes
+        )
         data.train_edges = train_edges
         data.val_edges = val_edges
         data.test_edges = test_edges
         data.val_neg_edges = val_false_edges
         data.test_neg_edges = test_false_edges
         self.dataset.data = data
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/cluster_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/cluster_dw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/graphsage_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/graphsage_dw.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         self.train_dataset = NeighborSamplerDataset(
             dataset, sizes=sample_size, batch_size=batch_size, mask=dataset.data.train_mask
         )
         self.val_dataset = NeighborSamplerDataset(
             dataset, sizes=sample_size, batch_size=batch_size * 2, mask=dataset.data.val_mask
         )
         self.test_dataset = NeighborSamplerDataset(
-            dataset=self.dataset,
-            mask=None,
-            sizes=[-1],
-            batch_size=batch_size * 2,
+            dataset=self.dataset, mask=None, sizes=[-1], batch_size=batch_size * 2,
         )
         self.x = self.dataset.data.x
         self.y = self.dataset.data.y
         self.batch_size = batch_size
         self.sample_size = sample_size
 
     def train_wrapper(self):
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/m3s_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/m3s_dw.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,18 +37,15 @@
             masked = train_nodes[perm[preserve_nnz:]]
             data.train_mask = torch.full((data.train_mask.shape[0],), False, dtype=torch.bool)
             data.train_mask[preserved] = True
             data.test_mask[masked] = True
 
         # Compute absorption probability
         row, col = data.edge_index
-        A = sp.coo_matrix(
-            (np.ones(row.shape[0]), (row.numpy(), col.numpy())),
-            shape=(num_nodes, num_nodes),
-        ).tocsr()
+        A = sp.coo_matrix((np.ones(row.shape[0]), (row.numpy(), col.numpy())), shape=(num_nodes, num_nodes),).tocsr()
         D = A.sum(1).flat
         confidence = np.zeros([num_classes, num_nodes])
         confidence_ranking = np.zeros([num_classes, num_nodes], dtype=int)
 
         if self.approximate:
             eps = 1e-2
             for i in range(num_classes):
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/network_embedding_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/network_embedding_dw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/node_classification_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/node_classification_dw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/pprgo_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/pprgo_dw.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,15 @@
             return self.dataset.data
 
 
 def setup_dataloader(ppr_dataset, batch_size):
     data_loader = torch.utils.data.DataLoader(
         dataset=ppr_dataset,
         sampler=torch.utils.data.BatchSampler(
-            torch.utils.data.SequentialSampler(ppr_dataset),
-            batch_size=batch_size,
-            drop_last=False,
+            torch.utils.data.SequentialSampler(ppr_dataset), batch_size=batch_size, drop_last=False,
         ),
         batch_size=None,
     )
     return data_loader
 
 
 def pre_transform(dataset, topk, alpha, epsilon, normalization, mode="train"):
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/data_wrapper/node_classification/sagn_dw.py` & `cogdl-0.6/cogdl/wrappers/data_wrapper/node_classification/sagn_dw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/default_match.py` & `cogdl-0.6/cogdl/wrappers/default_match.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,14 +75,19 @@
     ]
 
     heterogeneous_emb_models = [
         "metapath2vec",
         "pte",
         "hin2vec",
     ]
+    triple_link_prediction_models=["transe","distmult", "rotate", "complex"]
+    triple_link_prediction_wrappers=dict()
+    for item in triple_link_prediction_models:
+        triple_link_prediction_wrappers[item] = {"mw": "triple_link_prediction_mw", "dw": "triple_link_prediction_dw"}
+
 
     node_classification_wrappers = dict()
     for item in node_classification_models:
         node_classification_wrappers[item] = {"mw": "node_classification_mw", "dw": "node_classification_dw"}
 
     node_classification_wrappers["dgi"]["mw"] = "dgi_mw"
     node_classification_wrappers["m3s"]["mw"] = "m3s_mw"
@@ -93,14 +98,15 @@
     node_classification_wrappers["grand"]["mw"] = "grand_mw"
     node_classification_wrappers["gcnmix"]["mw"] = "gcnmix_mw"
     node_classification_wrappers["grace"]["mw"] = "grace_mw"
     node_classification_wrappers["pprgo"]["mw"] = "pprgo_mw"
 
     node_classification_wrappers["m3s"]["dw"] = "m3s_dw"
     node_classification_wrappers["graphsage"]["dw"] = "graphsage_dw"
+    node_classification_wrappers["unsup_graphsage"]["dw"] = "unsup_graphsage_dw"
     node_classification_wrappers["pprgo"]["dw"] = "pprgo_dw"
     node_classification_wrappers["sagn"]["dw"] = "sagn_dw"
 
     graph_classification_wrappers = dict()
     for item in graph_classification_models:
         graph_classification_wrappers[item] = {"mw": "graph_classification_mw", "dw": "graph_classification_dw"}
 
@@ -130,27 +136,35 @@
     for item in heterogeneous_gnn_models:
         heterogeneous_gnn_wrappers[item] = {"dw": "heterogeneous_gnn_dw", "mw": "heterogeneous_gnn_mw"}
 
     heterogeneous_emb_wrappers = dict()
     for item in heterogeneous_emb_models:
         heterogeneous_emb_wrappers[item] = {"dw": "heterogeneous_embedding_dw", "mw": "heterogeneous_embedding_mw"}
 
+    traffic_prediction_models = ["stgcn", "stgat"]
+    traffic_prediction_wrappers = dict()
+    for item in traffic_prediction_models:
+        traffic_prediction_wrappers[item] = {"dw": "{}_dw".format(item), "mw": "{}_mw".format(item)}
+
     other_wrappers = dict()
     other_wrappers["gatne"] = {"mw": "multiplex_embedding_mw", "dw": "multiplex_embedding_dw"}
+    other_wrappers["gcc"] = {"mw": "gcc_mw", "dw": "gcc_dw"}
 
     merged = dict()
     merged.update(node_classification_wrappers)
     merged.update(graph_embedding_wrappers)
     merged.update(graph_classification_wrappers)
     merged.update(network_embedding_wrappers)
     merged.update(graph_clustering_wrappers)
     merged.update(graph_kg_link_prediction_wrappers)
     merged.update(heterogeneous_gnn_wrappers)
     merged.update(heterogeneous_emb_wrappers)
     merged.update(other_wrappers)
+    merged.update(triple_link_prediction_wrappers)
+    merged.update(traffic_prediction_wrappers)
     return merged
 
 
 default_wrapper_config = set_default_wrapper_config()
 
 
 def get_wrappers(model_name):
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/__init__.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     else:
         raise NotImplementedError(f"Failed to import {name} ModelWrapper.")
     class_name = SUPPORTED_MW[name].split(".")[-1]
     return getattr(module, class_name)
 
 
 SUPPORTED_MW = {
+    "triple_link_prediction_mw": "cogdl.wrappers.model_wrapper.link_prediction.TripleModelWrapper",
     "dgi_mw": "cogdl.wrappers.model_wrapper.node_classification.DGIModelWrapper",
     "gcnmix_mw": "cogdl.wrappers.model_wrapper.node_classification.GCNMixModelWrapper",
     "grace_mw": "cogdl.wrappers.model_wrapper.node_classification.GRACEModelWrapper",
     "grand_mw": "cogdl.wrappers.model_wrapper.node_classification.GrandModelWrapper",
     "mvgrl_mw": "cogdl.wrappers.model_wrapper.node_classification.MVGRLModelWrapper",
     "self_auxiliary_mw": "cogdl.wrappers.model_wrapper.node_classification.SelfAuxiliaryModelWrapper",
     "graphsage_mw": "cogdl.wrappers.model_wrapper.node_classification.GraphSAGEModelWrapper",
@@ -55,8 +56,10 @@
     "multiplex_embedding_mw": "cogdl.wrappers.model_wrapper.heterogeneous.MultiplexEmbeddingModelWrapper",
     "graph_classification_mw": "cogdl.wrappers.model_wrapper.graph_classification.GraphClassificationModelWrapper",
     "graph_embedding_mw": "cogdl.wrappers.model_wrapper.graph_classification.GraphEmbeddingModelWrapper",
     "infograph_mw": "cogdl.wrappers.model_wrapper.graph_classification.InfoGraphModelWrapper",
     "agc_mw": "cogdl.wrappers.model_wrapper.clustering.AGCModelWrapper",
     "daegc_mw": "cogdl.wrappers.model_wrapper.clustering.DAEGCModelWrapper",
     "gae_mw": "cogdl.wrappers.model_wrapper.clustering.GAEModelWrapper",
+    "stgcn_mw": "cogdl.wrappers.model_wrapper.traffic_prediction.STGCNModelWrapper",
+    "stgat_mw": "cogdl.wrappers.model_wrapper.traffic_prediction.STGATModelWrapper",
 }
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/base_model_wrapper.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/base_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/clustering/agc_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/clustering/agc_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/clustering/daegc_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/clustering/daegc_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/clustering/gae_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/clustering/gae_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/graph_classification/graph_classification_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/graph_classification/graph_classification_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/graph_classification/graph_embedding_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/graph_classification/graph_embedding_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/graph_classification/infograph_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/graph_classification/infograph_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/heterogeneous/heterogeneous_embedding_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/heterogeneous/heterogeneous_embedding_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/heterogeneous/heterogeneous_gnn_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/heterogeneous/heterogeneous_gnn_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/heterogeneous/multiplex_embedding_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/heterogeneous/multiplex_embedding_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/link_prediction/embedding_link_prediction_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/link_prediction/embedding_link_prediction_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/link_prediction/gnn_kg_link_prediction_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/link_prediction/gnn_kg_link_prediction_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/link_prediction/gnn_link_prediction_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/link_prediction/gnn_link_prediction_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/__init__.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/correct_smooth_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/correct_smooth_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/dgi_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/dgi_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/gcnmix_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/gcnmix_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/grace_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/grace_mw.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,19 +50,15 @@
         with torch.no_grad():
             pred = self.model(graph)
         y = graph.y
         result = evaluate_node_embeddings_using_logreg(pred, y, graph.train_mask, graph.test_mask)
         self.note("test_acc", result)
 
     def prop(
-        self,
-        graph: Graph,
-        x: torch.Tensor,
-        drop_feature_rate: float = 0.0,
-        drop_edge_rate: float = 0.0,
+        self, graph: Graph, x: torch.Tensor, drop_feature_rate: float = 0.0, drop_edge_rate: float = 0.0,
     ):
         x = dropout_features(x, drop_feature_rate)
         with graph.local_graph():
             graph.edge_index, graph.edge_weight = dropout_adj(graph.edge_index, graph.edge_weight, drop_edge_rate)
             return self.model.forward(graph, x)
 
     def contrastive_loss(self, z1: torch.Tensor, z2: torch.Tensor):
@@ -77,18 +73,15 @@
         intro_scores = score_func(z1, z1)
         inter_scores = score_func(z1, z2)
 
         _loss = -torch.log(intro_scores.diag() / (intro_scores.sum(1) - intro_scores.diag() + inter_scores.sum(1)))
         return torch.mean(_loss)
 
     def batched_loss(
-        self,
-        z1: torch.Tensor,
-        z2: torch.Tensor,
-        batch_size: int,
+        self, z1: torch.Tensor, z2: torch.Tensor, batch_size: int,
     ):
         num_nodes = z1.shape[0]
         num_batches = (num_nodes - 1) // batch_size + 1
 
         losses = []
         indices = torch.arange(num_nodes).to(z1.device)
         for i in range(num_batches):
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/grand_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/grand_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/graphsage_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/graphsage_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/m3s_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/m3s_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/mvgrl_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/mvgrl_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/network_embedding_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/network_embedding_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/node_classification_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/node_classification_mw.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     def test_step(self, batch):
         graph = batch
         pred = self.model(graph)
         test_mask = batch.test_mask
         loss = self.default_loss_fn(pred[test_mask], batch.y[test_mask])
 
         metric = self.evaluate(pred[test_mask], batch.y[test_mask], metric="auto")
-
         self.note("test_loss", loss.item())
         self.note("test_metric", metric)
 
     def setup_optimizer(self):
         cfg = self.optimizer_cfg
         if hasattr(self.model, "setup_optimizer"):
             model_spec_optim = self.model.setup_optimizer(cfg)
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/pprgo_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/pprgo_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/sagn_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/sagn_mw.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/model_wrapper/node_classification/self_auxiliary_mw.py` & `cogdl-0.6/cogdl/wrappers/model_wrapper/node_classification/self_auxiliary_mw.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,20 +63,15 @@
     def generate_virtual_labels(self, data):
         if self.auxiliary_task == "edge_mask":
             self.agent = EdgeMask(self.hidden_size, self.mask_ratio, self.device)
         elif self.auxiliary_task == "attribute_mask":
             self.agent = AttributeMask(data, self.hidden_size, data.train_mask, self.mask_ratio, self.device)
         elif self.auxiliary_task == "pairwise_distance":
             self.agent = PairwiseDistance(
-                self.hidden_size,
-                [(1, 2), (2, 3), (3, 5)],
-                self.sampling,
-                self.dropedge_rate,
-                256,
-                self.device,
+                self.hidden_size, [(1, 2), (2, 3), (3, 5)], self.sampling, self.dropedge_rate, 256, self.device,
             )
         elif self.auxiliary_task == "distance2clusters":
             self.agent = Distance2Clusters(self.hidden_size, 30, self.device)
         elif self.auxiliary_task == "pairwise_attr_sim":
             self.agent = PairwiseAttrSim(self.hidden_size, 5, self.device)
         else:
             raise Exception(
```

### Comparing `cogdl-0.5.3/cogdl/wrappers/tools/memory_moco.py` & `cogdl-0.6/cogdl/wrappers/tools/memory_moco.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl/wrappers/tools/wrapper_utils.py` & `cogdl-0.6/cogdl/wrappers/tools/wrapper_utils.py`

 * *Files identical despite different names*

### Comparing `cogdl-0.5.3/cogdl.egg-info/PKG-INFO` & `cogdl-0.6/cogdl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogdl
-Version: 0.5.3
+Version: 0.6
 Summary: An Extensive Research Toolkit for Deep Learning on Graphs
 Home-page: https://github.com/THUDM/cogdl
 License: MIT
 Keywords: network embedding,graph representation learning,graph neural networks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -19,47 +19,51 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![CogDL](./docs/source/_static/cogdl-logo.png)
 ===
 
 [![PyPI Latest Release](https://badge.fury.io/py/cogdl.svg)](https://pypi.org/project/cogdl/)
-[![Build Status](https://travis-ci.org/THUDM/cogdl.svg?branch=master)](https://travis-ci.org/THUDM/cogdl)
+[![Build Status](https://app.travis-ci.com/THUDM/cogdl.svg?branch=master)](https://app.travis-ci.com/THUDM/cogdl)
 [![Documentation Status](https://readthedocs.org/projects/cogdl/badge/?version=latest)](https://cogdl.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://pepy.tech/badge/cogdl)](https://pepy.tech/project/cogdl)
 [![Coverage Status](https://coveralls.io/repos/github/THUDM/cogdl/badge.svg?branch=master)](https://coveralls.io/github/THUDM/cogdl?branch=master)
 [![License](https://img.shields.io/github/license/thudm/cogdl)](https://github.com/THUDM/cogdl/blob/master/LICENSE)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
-**[Homepage](https://cogdl.ai)** | **[Paper](https://arxiv.org/abs/2103.00959)** | **[100 GNN papers](./gnn_papers.md)** | **[Leaderboards](./results.md)** | **[Documentation](https://cogdl.readthedocs.io)** | **[Datasets](./cogdl/datasets/README.md)** | **[Join our Slack](https://join.slack.com/t/cogdl/shared_invite/zt-b9b4a49j-2aMB035qZKxvjV4vqf0hEg)** | **[中文](./README_CN.md)**
+**[Homepage](https://cogdl.ai)** | **[Paper](https://arxiv.org/abs/2103.00959)** | **[Documentation](https://cogdl.readthedocs.io)** | **[Discussion Forum](https://discuss.cogdl.ai)** | **[Dataset](./cogdl/datasets/README.md)** | **[中文](./README_CN.md)**
 
 CogDL is a graph deep learning toolkit that allows researchers and developers to easily train and compare baseline or customized models for node classification, graph classification, and other important tasks in the graph domain. 
 
 We summarize the contributions of CogDL as follows:
 
 - **Efficiency**: CogDL utilizes well-optimized operators to speed up training and save GPU memory of GNN models.
 - **Ease of Use**: CogDL provides easy-to-use APIs for running experiments with the given models and datasets using hyper-parameter search.
 - **Extensibility**: The design of CogDL makes it easy to apply GNN models to new scenarios based on our framework.
 
 ## ❗ News
 
-- The new **v0.5.3 release** supports mixed-precision training by setting \textit{fp16=True} and provides a basic [example](https://github.com/THUDM/cogdl/blob/master/examples/jittor/gcn.py) written by [Jittor](https://github.com/Jittor/jittor). It also updates the tutorial in the document, fixes downloading links of some datasets, and fixes potential bugs of operators. 
+- [The CogDL paper](https://arxiv.org/abs/2103.00959) was accepted by [WWW 2023](https://www2023.thewebconf.org/). Find us at WWW 2023! We also release the new **v0.6 release** which adds more examples of graph self-supervised learning, including [GraphMAE](https://github.com/THUDM/cogdl/tree/master/examples/graphmae), [GraphMAE2](https://github.com/THUDM/cogdl/tree/master/examples/graphmae2), and [BGRL](https://github.com/THUDM/cogdl/tree/master/examples/bgrl). 
 
-- The new **v0.5.2 release** adds a GNN example for ogbn-products and updates geom datasets. It also fixes some potential bugs including setting devices, using cpu for inference, etc.
+- A free GNN course provided by CogDL Team is present at [this link](https://cogdl.ai/gnn2022/). We also provide a [discussion forum](https://discuss.cogdl.ai) for Chinese users. 
 
-- The new **v0.5.1 release** adds fast operators including SpMM (cpu version) and scatter_max (cuda version). It also adds lots of datasets for node classification which can be found in [this link](./cogdl/datasets/rd2cd_data.py). 🎉
-
-- The new **v0.5.0 release** designs and implements a unified training loop for GNN. It introduces `DataWrapper` to help prepare the training/validation/test data and `ModelWrapper` to define the training/validation/test steps. 🎉
+- The new **v0.5.3 release** supports mixed-precision training by setting \textit{fp16=True} and provides a basic [example](https://github.com/THUDM/cogdl/blob/master/examples/jittor/gcn.py) written by [Jittor](https://github.com/Jittor/jittor). It also updates the tutorial in the document, fixes downloading links of some datasets, and fixes potential bugs of operators. 
 
 <details>
 <summary>
 News History
 </summary>
 <br/>
 
+- The new **v0.5.2 release** adds a GNN example for ogbn-products and updates geom datasets. It also fixes some potential bugs including setting devices, using cpu for inference, etc.
+
+- The new **v0.5.1 release** adds fast operators including SpMM (cpu version) and scatter_max (cuda version). It also adds lots of datasets for node classification which can be found in [this link](./cogdl/datasets/rd2cd_data.py). 🎉
+
+- The new **v0.5.0 release** designs and implements a unified training loop for GNN. It introduces `DataWrapper` to help prepare the training/validation/test data and `ModelWrapper` to define the training/validation/test steps. 🎉
+
 - The new **v0.4.1 release** adds the implementation of Deep GNNs and the recommendation task. It also supports new pipelines for generating embeddings and recommendation. Welcome to join our tutorial on KDD 2021 at 10:30 am - 12:00 am, Aug. 14th (Singapore Time). More details can be found in https://kdd2021graph.github.io/. 🎉
 
 - The new **v0.4.0 release** refactors the data storage (from `Data` to `Graph`) and provides more fast operators to speed up GNN training. It also includes many self-supervised learning methods on graphs. BTW, we are glad to announce that we will give a tutorial on KDD 2021 in August. Please see [this link](https://kdd2021graph.github.io/) for more details. 🎉
 
 - CogDL supports GNN models with Mixture of Experts (MoE). You can install [FastMoE](https://github.com/laekov/fastmoe) and try **[MoE GCN](./cogdl/models/nn/moe_gcn.py)** in CogDL now!
 
 - The new **v0.3.0 release** provides a fast spmm operator to speed up GNN training. We also release the first version of **[CogDL paper](https://arxiv.org/abs/2103.00959)** in arXiv. You can join [our slack](https://join.slack.com/t/cogdl/shared_invite/zt-b9b4a49j-2aMB035qZKxvjV4vqf0hEg) for discussion. 🎉🎉🎉
@@ -127,26 +131,14 @@
         "hidden_size": trial.suggest_categorical("hidden_size", [32, 64, 128]),
         "dropout": trial.suggest_uniform("dropout", 0.5, 0.8),
     }
 
 experiment(dataset="cora", model="gcn", seed=[1, 2], search_space=search_space)
 ```
 
-Some interesting applications can be used through `pipeline` API. An example can be found in the [pipeline.py](https://github.com/THUDM/cogdl/tree/master/examples/pipeline.py). 
-
-```python
-from cogdl import pipeline
-
-# load OAGBert model and perform inference
-oagbert = pipeline("oagbert")
-outputs = oagbert(["CogDL is developed by KEG, Tsinghua.", "OAGBert is developed by KEG, Tsinghua."])
-```
-
-More details of the OAGBert usage can be found [here](./cogdl/oag/README.md).
-
 ### Command-Line Usage
 
 You can also use `python scripts/train.py --dataset example_dataset --model example_model` to run example_model on example_data.
 
 - --dataset, dataset name to run, can be a list of datasets with space like `cora citeseer`. Supported datasets include
 'cora', 'citeseer', 'pumbed', 'ppi', 'wikipedia', 'blogcatalog', 'flickr'. More datasets can be found in the [cogdl/datasets](https://github.com/THUDM/cogdl/tree/master/cogdl/datasets).
 - --model, model name to run, can be a list of models like `gcn gat`. Supported models include
@@ -234,23 +226,23 @@
 
 * Let's say you implement a GNN model in a script `models/nn/abcgnn.py` that does the task of node classification. Then, you need to add a unit test inside the script `tests/tasks/test_node_classification.py` (or whatever relevant task your model does). 
 * To add the unit test, you simply add a function *test_abcgnn_cora()* (just follow the format of the other unit tests already in the script), fill it with required arguments and the last line in the function *'assert 0 <= ret["Acc"] <= 1'* is the very basic sanity check conducted by the unit test. 
 * After modifying `tests/tasks/test_node_classification.py`, commit it together with your `models/nn/abcgnn.py` and your pull request should pass.
 </details>
 
 ## CogDL Team
-CogDL is developed and maintained by [Tsinghua, ZJU, BAAI, DAMO Academy, and ZHIPU.AI](https://cogdl.ai/about/). 
+CogDL is developed and maintained by [Tsinghua, ZJU, DAMO Academy, and ZHIPU.AI](https://cogdl.ai/about/). 
 
 The core development team can be reached at [cogdlteam@gmail.com](mailto:cogdlteam@gmail.com).
 
 ## Citing CogDL
 
 Please cite [our paper](https://arxiv.org/abs/2103.00959) if you find our code or results useful for your research:
 
 ```
-@article{cen2021cogdl,
-    title={CogDL: A Toolkit for Deep Learning on Graphs},
+@inproceedings{cen2023cogdl,
+    title={CogDL: A Comprehensive Library for Graph Deep Learning},
     author={Yukuo Cen and Zhenyu Hou and Yan Wang and Qibin Chen and Yizhen Luo and Zhongming Yu and Hengrui Zhang and Xingcheng Yao and Aohan Zeng and Shiguang Guo and Yuxiao Dong and Yang Yang and Peng Zhang and Guohao Dai and Yu Wang and Chang Zhou and Hongxia Yang and Jie Tang},
-    journal={arXiv preprint arXiv:2103.00959},
-    year={2021}
+    booktitle={Proceedings of the ACM Web Conference 2023 (WWW'23)},
+    year={2023}
 }
 ```
```

### Comparing `cogdl-0.5.3/cogdl.egg-info/SOURCES.txt` & `cogdl-0.6/cogdl.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 cogdl/__init__.py
-cogdl/backend.py
 cogdl/configs.py
 cogdl/experiments.py
 cogdl/options.py
 cogdl/pipelines.py
 cogdl.egg-info/PKG-INFO
 cogdl.egg-info/SOURCES.txt
 cogdl.egg-info/dependency_links.txt
@@ -21,77 +20,89 @@
 cogdl/data/dataset.py
 cogdl/data/sampler.py
 cogdl/datasets/__init__.py
 cogdl/datasets/customized_data.py
 cogdl/datasets/gatne.py
 cogdl/datasets/gcc_data.py
 cogdl/datasets/geom_data.py
+cogdl/datasets/grb_data.py
 cogdl/datasets/gtn_data.py
 cogdl/datasets/han_data.py
 cogdl/datasets/kg_data.py
 cogdl/datasets/matlab_matrix.py
 cogdl/datasets/oagbert_data.py
 cogdl/datasets/ogb.py
 cogdl/datasets/planetoid_data.py
 cogdl/datasets/rd2cd_data.py
 cogdl/datasets/rec_data.py
 cogdl/datasets/saint_data.py
+cogdl/datasets/stgat_data.py
+cogdl/datasets/stgcn_data.py
 cogdl/datasets/tu_data.py
 cogdl/layers/__init__.py
 cogdl/layers/actgcn_layer.py
 cogdl/layers/actgcnii_layer.py
 cogdl/layers/actlinear_layer.py
 cogdl/layers/actmlp_layer.py
 cogdl/layers/actsage_layer.py
 cogdl/layers/base_layer.py
 cogdl/layers/deepergcn_layer.py
 cogdl/layers/disengcn_layer.py
 cogdl/layers/gat_layer.py
+cogdl/layers/gat_layerii.py
 cogdl/layers/gcn_layer.py
+cogdl/layers/gcn_layerii.py
 cogdl/layers/gcnii_layer.py
 cogdl/layers/gin_layer.py
 cogdl/layers/gine_layer.py
 cogdl/layers/han_layer.py
 cogdl/layers/mixhop_layer.py
 cogdl/layers/mlp_layer.py
 cogdl/layers/pprgo_layer.py
 cogdl/layers/reversible_layer.py
 cogdl/layers/rgcn_layer.py
 cogdl/layers/sage_layer.py
 cogdl/layers/saint_layer.py
 cogdl/layers/se_layer.py
 cogdl/layers/set2set.py
 cogdl/layers/sgc_layer.py
+cogdl/layers/stgat_layer.py
+cogdl/layers/stgcn_layer.py
 cogdl/layers/jittor/__init__.py
 cogdl/layers/jittor/gcn_layer.py
 cogdl/loggers/__init__.py
 cogdl/loggers/base_logger.py
 cogdl/loggers/tensorboard_logger.py
 cogdl/loggers/wandb_logger.py
 cogdl/models/__init__.py
 cogdl/models/base_model.py
 cogdl/models/emb/__init__.py
+cogdl/models/emb/complex.py
 cogdl/models/emb/deepwalk.py
 cogdl/models/emb/dgk.py
+cogdl/models/emb/distmult.py
 cogdl/models/emb/dngr.py
 cogdl/models/emb/gatne.py
 cogdl/models/emb/graph2vec.py
 cogdl/models/emb/grarep.py
 cogdl/models/emb/hin2vec.py
 cogdl/models/emb/hope.py
+cogdl/models/emb/knowledge_base.py
 cogdl/models/emb/line.py
 cogdl/models/emb/metapath2vec.py
 cogdl/models/emb/netmf.py
 cogdl/models/emb/netsmf.py
 cogdl/models/emb/node2vec.py
 cogdl/models/emb/prone.py
 cogdl/models/emb/pronepp.py
 cogdl/models/emb/pte.py
+cogdl/models/emb/rotate.py
 cogdl/models/emb/sdne.py
 cogdl/models/emb/spectral.py
+cogdl/models/emb/transe.py
 cogdl/models/nn/__init__.py
 cogdl/models/nn/actgcn.py
 cogdl/models/nn/agc.py
 cogdl/models/nn/autognn.py
 cogdl/models/nn/compgcn.py
 cogdl/models/nn/correct_smooth.py
 cogdl/models/nn/daegc.py
@@ -129,15 +140,16 @@
 cogdl/models/nn/revgcn.py
 cogdl/models/nn/rgcn.py
 cogdl/models/nn/sagn.py
 cogdl/models/nn/sgc.py
 cogdl/models/nn/sign.py
 cogdl/models/nn/sortpool.py
 cogdl/models/nn/srgcn.py
-cogdl/models/nn/unsup_graphsage.py
+cogdl/models/nn/stgat.py
+cogdl/models/nn/stgcn.py
 cogdl/oag/__init__.py
 cogdl/oag/bert_model.py
 cogdl/oag/dual_position_bert_model.py
 cogdl/oag/oagbert.py
 cogdl/oag/oagbert_metainfo.py
 cogdl/oag/utils.py
 cogdl/operators/__init__.py
@@ -173,14 +185,15 @@
 cogdl/trainer/trainer_utils.py
 cogdl/trainer/controller/__init__.py
 cogdl/trainer/controller/data_controller.py
 cogdl/trainer/controller/training_controller.py
 cogdl/utils/__init__.py
 cogdl/utils/evaluator.py
 cogdl/utils/graph_utils.py
+cogdl/utils/grb_utils.py
 cogdl/utils/index.py
 cogdl/utils/link_prediction_utils.py
 cogdl/utils/optimizer.py
 cogdl/utils/ppr_utils.py
 cogdl/utils/prone_utils.py
 cogdl/utils/sampling.py
 cogdl/utils/spmm_utils.py
@@ -201,24 +214,29 @@
 cogdl/wrappers/data_wrapper/heterogeneous/heterogeneous_embedding_dw.py
 cogdl/wrappers/data_wrapper/heterogeneous/heterogeneous_gnn_dw.py
 cogdl/wrappers/data_wrapper/heterogeneous/multiplex_embedding_dw.py
 cogdl/wrappers/data_wrapper/link_prediction/__init__.py
 cogdl/wrappers/data_wrapper/link_prediction/embedding_link_prediction_dw.py
 cogdl/wrappers/data_wrapper/link_prediction/gnn_kg_link_prediction_dw.py
 cogdl/wrappers/data_wrapper/link_prediction/gnn_link_prediction_dw.py
+cogdl/wrappers/data_wrapper/link_prediction/triple_link_prediction_dw.py
 cogdl/wrappers/data_wrapper/node_classification/__init__.py
 cogdl/wrappers/data_wrapper/node_classification/cluster_dw.py
 cogdl/wrappers/data_wrapper/node_classification/graphsage_dw.py
 cogdl/wrappers/data_wrapper/node_classification/m3s_dw.py
 cogdl/wrappers/data_wrapper/node_classification/network_embedding_dw.py
 cogdl/wrappers/data_wrapper/node_classification/node_classification_dw.py
 cogdl/wrappers/data_wrapper/node_classification/pprgo_dw.py
 cogdl/wrappers/data_wrapper/node_classification/sagn_dw.py
+cogdl/wrappers/data_wrapper/node_classification/unsup_graphsage_dw.py
 cogdl/wrappers/data_wrapper/pretraining/__init__.py
 cogdl/wrappers/data_wrapper/pretraining/gcc_dw.py
+cogdl/wrappers/data_wrapper/traffic_prediction/__init__.py
+cogdl/wrappers/data_wrapper/traffic_prediction/stgat_dw.py
+cogdl/wrappers/data_wrapper/traffic_prediction/stgcn_dw.py
 cogdl/wrappers/model_wrapper/__init__.py
 cogdl/wrappers/model_wrapper/base_model_wrapper.py
 cogdl/wrappers/model_wrapper/clustering/__init__.py
 cogdl/wrappers/model_wrapper/clustering/agc_mw.py
 cogdl/wrappers/model_wrapper/clustering/daegc_mw.py
 cogdl/wrappers/model_wrapper/clustering/gae_mw.py
 cogdl/wrappers/model_wrapper/graph_classification/__init__.py
@@ -229,14 +247,15 @@
 cogdl/wrappers/model_wrapper/heterogeneous/heterogeneous_embedding_mw.py
 cogdl/wrappers/model_wrapper/heterogeneous/heterogeneous_gnn_mw.py
 cogdl/wrappers/model_wrapper/heterogeneous/multiplex_embedding_mw.py
 cogdl/wrappers/model_wrapper/link_prediction/__init__.py
 cogdl/wrappers/model_wrapper/link_prediction/embedding_link_prediction_mw.py
 cogdl/wrappers/model_wrapper/link_prediction/gnn_kg_link_prediction_mw.py
 cogdl/wrappers/model_wrapper/link_prediction/gnn_link_prediction_mw.py
+cogdl/wrappers/model_wrapper/link_prediction/triple_link_prediction_mw.py
 cogdl/wrappers/model_wrapper/node_classification/__init__.py
 cogdl/wrappers/model_wrapper/node_classification/correct_smooth_mw.py
 cogdl/wrappers/model_wrapper/node_classification/dgi_mw.py
 cogdl/wrappers/model_wrapper/node_classification/gcnmix_mw.py
 cogdl/wrappers/model_wrapper/node_classification/grace_mw.py
 cogdl/wrappers/model_wrapper/node_classification/grand_mw.py
 cogdl/wrappers/model_wrapper/node_classification/graphsage_mw.py
@@ -246,10 +265,21 @@
 cogdl/wrappers/model_wrapper/node_classification/node_classification_mw.py
 cogdl/wrappers/model_wrapper/node_classification/pprgo_mw.py
 cogdl/wrappers/model_wrapper/node_classification/sagn_mw.py
 cogdl/wrappers/model_wrapper/node_classification/self_auxiliary_mw.py
 cogdl/wrappers/model_wrapper/node_classification/unsup_graphsage_mw.py
 cogdl/wrappers/model_wrapper/pretraining/__init__.py
 cogdl/wrappers/model_wrapper/pretraining/gcc_mw.py
+cogdl/wrappers/model_wrapper/traffic_prediction/__init__.py
+cogdl/wrappers/model_wrapper/traffic_prediction/stgat_mw.py
+cogdl/wrappers/model_wrapper/traffic_prediction/stgcn_mw.py
 cogdl/wrappers/tools/__init__.py
 cogdl/wrappers/tools/memory_moco.py
-cogdl/wrappers/tools/wrapper_utils.py
+cogdl/wrappers/tools/wrapper_utils.py
+tests/test_args.py
+tests/test_experiments.py
+tests/test_layers.py
+tests/test_oag.py
+tests/test_ops.py
+tests/test_options.py
+tests/test_pipelines.py
+tests/test_utils.py
```

### Comparing `cogdl-0.5.3/setup.py` & `cogdl-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,20 +69,21 @@
     #   py_modules=["my_module"],
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=[
         "torch",
+        "importlib-metadata<5.0",
         "networkx",
         "matplotlib",
         "tqdm",
         "numpy>=1.21",
         "scipy",
-        "gensim<4.0",
+        "gensim>=4.0",
         "grave",
         "scikit_learn",
         "tabulate",
         "optuna==2.4.0",
         "ogb",
         "pre-commit",
         "flake8",
```


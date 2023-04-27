# Comparing `tmp/open-metric-learning-0.3.9.tar.gz` & `tmp/open-metric-learning-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/open-metric-learning-0.3.9.tar", last modified: Tue Jan 31 10:40:56 2023, max compression
+gzip compressed data, was "dist/open-metric-learning-0.4.0.tar", last modified: Thu Apr 27 16:36:45 2023, max compression
```

## Comparing `open-metric-learning-0.3.9.tar` & `open-metric-learning-0.4.0.tar`

### file list

```diff
@@ -1,201 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.207877 open-metric-learning-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    36030 2023-01-31 10:40:56.207877 open-metric-learning-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    34606 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.187877 open-metric-learning-0.3.9/oml/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.187877 open-metric-learning-0.3.9/oml/configs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.187877 open-metric-learning-0.3.9/oml/configs/criterion/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/criterion/arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/criterion/mlp_arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/criterion/surrogate_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/criterion/triplet.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/criterion/triplet_plain.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/criterion/triplet_with_miner.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.187877 open-metric-learning-0.3.9/oml/configs/miner/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/miner/all_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/miner/hard_cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/miner/hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/miner/miner_with_bank.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/miner/n_hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/miner/triplets_with_memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.187877 open-metric-learning-0.3.9/oml/configs/model/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/model/extractor_with_mlp.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/model/resnet.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/model/vit.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/model/vit_clip.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.191877 open-metric-learning-0.3.9/oml/configs/optimizer/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/optimizer/adadelta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/optimizer/adagrad.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/optimizer/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/optimizer/adamax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/optimizer/adamw.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/optimizer/asgd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/optimizer/lbfgs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/optimizer/rmsprop.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/optimizer/rprop.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/optimizer/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.191877 open-metric-learning-0.3.9/oml/configs/pairwise_model/
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/pairwise_model/concat_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/pairwise_model/linear_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/pairwise_model/trivial_distance_siamese.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.191877 open-metric-learning-0.3.9/oml/configs/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/postprocessor/pairwise_embeddings.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/postprocessor/pairwise_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.191877 open-metric-learning-0.3.9/oml/configs/sampler/
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/sampler/balance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/sampler/category_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/sampler/distinct_category_balance.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.191877 open-metric-learning-0.3.9/oml/configs/scheduler/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/scheduler/cosine_annealing.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/scheduler/cyclic.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/scheduler/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/scheduler/lambda.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/scheduler/multi_step.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/scheduler/multiplicative.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/scheduler/one_cycle.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/scheduler/reduce_on_plateau.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/scheduler/step.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.191877 open-metric-learning-0.3.9/oml/configs/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/transforms/augs_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/transforms/augs_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/transforms/augs_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/transforms/norm_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/transforms/norm_resize_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/transforms/norm_resize_albu_clip.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/transforms/norm_resize_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/transforms/norm_resize_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/configs/transforms/norm_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/const.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.191877 open-metric-learning-0.3.9/oml/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12300 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4446 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/datasets/list_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     4109 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/datasets/pairs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/datasets/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.195877 open-metric-learning-0.3.9/oml/ddp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/ddp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/ddp/patching.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/ddp/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.195877 open-metric-learning-0.3.9/oml/functional/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/functional/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/functional/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)    25556 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/functional/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.195877 open-metric-learning-0.3.9/oml/inference/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/inference/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)     3054 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/inference/flat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2538 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/inference/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.195877 open-metric-learning-0.3.9/oml/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/interfaces/criterions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/interfaces/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     2362 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/interfaces/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3106 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/interfaces/miners.py
--rw-r--r--   0 runner    (1001) docker     (122)     1187 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/interfaces/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/interfaces/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/interfaces/samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.195877 open-metric-learning-0.3.9/oml/lightning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.195877 open-metric-learning-0.3.9/oml/lightning/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8802 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/callbacks/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.195877 open-metric-learning-0.3.9/oml/lightning/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6263 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/entrypoints/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     5327 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/entrypoints/train.py
--rw-r--r--   0 runner    (1001) docker     (122)     6941 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/entrypoints/train_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/entrypoints/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.195877 open-metric-learning-0.3.9/oml/lightning/modules/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/modules/ddp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/modules/pairwise_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5553 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/lightning/modules/retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.195877 open-metric-learning-0.3.9/oml/losses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/losses/arcface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/losses/surrogate_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     8507 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/losses/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.199877 open-metric-learning-0.3.9/oml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    15995 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/metrics/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/metrics/triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.199877 open-metric-learning-0.3.9/oml/miners/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/miners/cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/miners/inbatch_all_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     6530 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/miners/inbatch_hard_cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/miners/inbatch_hard_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/miners/inbatch_nhard_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/miners/miner_with_bank.py
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/miners/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.199877 open-metric-learning-0.3.9/oml/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/pooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/projection.py
--rw-r--r--   0 runner    (1001) docker     (122)     6827 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     4665 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/siamese.py
--rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.203877 open-metric-learning-0.3.9/oml/models/vit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/vit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6055 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/vit/clip.py
--rw-r--r--   0 runner    (1001) docker     (122)     5696 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/vit/hubconf.py
--rw-r--r--   0 runner    (1001) docker     (122)    13388 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/vit/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/vit/vision_transformer_clip.py
--rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/models/vit/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.203877 open-metric-learning-0.3.9/oml/registry/
--rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/registry/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/registry/miners.py
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/registry/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/registry/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/registry/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/registry/samplers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/registry/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/registry/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.203877 open-metric-learning-0.3.9/oml/retrieval/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/retrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.203877 open-metric-learning-0.3.9/oml/retrieval/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/retrieval/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10866 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/retrieval/postprocessors/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.203877 open-metric-learning-0.3.9/oml/samplers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/samplers/balance.py
--rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/samplers/category_balance.py
--rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/samplers/distinct_category_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.203877 open-metric-learning-0.3.9/oml/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.203877 open-metric-learning-0.3.9/oml/transforms/images/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/transforms/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.203877 open-metric-learning-0.3.9/oml/transforms/images/albumentations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/transforms/images/albumentations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/transforms/images/albumentations/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.207877 open-metric-learning-0.3.9/oml/transforms/images/torchvision/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/transforms/images/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/transforms/images/torchvision/transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/transforms/images/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.207877 open-metric-learning-0.3.9/oml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/utils/dataframe_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/utils/download_mock_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.207877 open-metric-learning-0.3.9/oml/utils/images/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/utils/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3019 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/utils/images/images.py
--rw-r--r--   0 runner    (1001) docker     (122)     6600 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/utils/images/images_resize.py
--rw-r--r--   0 runner    (1001) docker     (122)     4202 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5640 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)    16347 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/utils/misc_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/oml/utils/remote_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 10:40:56.207877 open-metric-learning-0.3.9/open_metric_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    36030 2023-01-31 10:40:56.000000 open-metric-learning-0.3.9/open_metric_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5183 2023-01-31 10:40:56.000000 open-metric-learning-0.3.9/open_metric_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-31 10:40:56.000000 open-metric-learning-0.3.9/open_metric_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-01-31 10:40:56.000000 open-metric-learning-0.3.9/open_metric_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-01-31 10:40:56.000000 open-metric-learning-0.3.9/open_metric_learning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-01-31 10:40:56.207877 open-metric-learning-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-01-31 10:40:38.000000 open-metric-learning-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    25628 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24204 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.512738 open-metric-learning-0.4.0/oml/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.512738 open-metric-learning-0.4.0/oml/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.512738 open-metric-learning-0.4.0/oml/configs/criterion/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/mlp_arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/surrogate_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/triplet.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/triplet_plain.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/triplet_with_miner.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.512738 open-metric-learning-0.4.0/oml/configs/extractor/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/extractor/extractor_with_mlp.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/extractor/resnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/extractor/vit.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/extractor/vit_clip.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.516738 open-metric-learning-0.4.0/oml/configs/miner/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/all_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/hard_cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/miner_with_bank.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/n_hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/triplets_with_memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.516738 open-metric-learning-0.4.0/oml/configs/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/adadelta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/adagrad.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/adamax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/adamw.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/asgd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/lbfgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/rmsprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/rprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.516738 open-metric-learning-0.4.0/oml/configs/pairwise_model/
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/pairwise_model/concat_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/pairwise_model/linear_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/pairwise_model/trivial_distance_siamese.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.516738 open-metric-learning-0.4.0/oml/configs/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/postprocessor/pairwise_embeddings.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/postprocessor/pairwise_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.516738 open-metric-learning-0.4.0/oml/configs/sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/sampler/balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/sampler/category_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/sampler/distinct_category_balance.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/configs/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/cosine_annealing.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/cyclic.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/lambda.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/multi_step.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/multiplicative.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/one_cycle.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/reduce_on_plateau.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/step.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/configs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/augs_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/augs_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/augs_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_resize_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_resize_albu_clip.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_resize_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_resize_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/const.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12302 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4428 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/datasets/list_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/datasets/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3739 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/datasets/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/ddp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/ddp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/ddp/patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/ddp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/functional/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/functional/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/functional/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25034 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/functional/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/inference/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/inference/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/inference/flat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/inference/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/criterions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2354 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3106 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/miners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/lightning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/lightning/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8802 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/callbacks/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/lightning/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/modules/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/modules/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/modules/pairwise_postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/lightning/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/pipelines/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/pipelines/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/pipelines/train_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/pipelines/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/losses/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/losses/arcface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/losses/surrogate_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8578 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/losses/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15976 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/metrics/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/metrics/triplets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/miners/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/inbatch_all_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6530 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/inbatch_hard_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/inbatch_hard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/inbatch_nhard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/miner_with_bank.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/models/meta/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/meta/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5280 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/meta/siamese.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7763 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/models/vit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/clip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5696 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/hubconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13388 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/vision_transformer_clip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8065 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/registry/
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/miners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2679 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/retrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/retrieval/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/retrieval/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/retrieval/postprocessors/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/samplers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/samplers/balance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/samplers/category_balance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/samplers/distinct_category_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/transforms/images/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/transforms/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/transforms/images/albumentations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/transforms/images/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/transforms/images/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/dataframe_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/download_mock_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/utils/images/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3128 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/images/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6600 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/images/images_resize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4202 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5640 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16347 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/misc_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/remote_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/open_metric_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    25628 2023-04-27 16:36:45.000000 open-metric-learning-0.4.0/open_metric_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5159 2023-04-27 16:36:45.000000 open-metric-learning-0.4.0/open_metric_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 16:36:45.000000 open-metric-learning-0.4.0/open_metric_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-04-27 16:36:45.000000 open-metric-learning-0.4.0/open_metric_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-04-27 16:36:45.000000 open-metric-learning-0.4.0/open_metric_learning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/tests/test_build_readme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/tests/test_imports.py
```

### Comparing `open-metric-learning-0.3.9/LICENSE` & `open-metric-learning-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/const.py` & `open-metric-learning-0.4.0/oml/const.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/datasets/base.py` & `open-metric-learning-0.4.0/oml/datasets/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def __init__(
         self,
         df: pd.DataFrame,
         extra_data: Optional[Dict[str, Any]] = None,
         transform: Optional[TTransforms] = None,
         dataset_root: Optional[Union[str, Path]] = None,
         f_imread: Optional[TImReader] = None,
-        cache_size: Optional[int] = 100_000,
+        cache_size: Optional[int] = 0,
         input_tensors_key: str = INPUT_TENSORS_KEY,
         labels_key: str = LABELS_KEY,
         paths_key: str = PATHS_KEY,
         categories_key: Optional[str] = CATEGORIES_KEY,
         x1_key: str = X1_KEY,
         x2_key: str = X2_KEY,
         y1_key: str = Y1_KEY,
@@ -63,19 +63,19 @@
         index_key: str = INDEX_KEY,
     ):
         """
 
         Args:
             df: Table with the following obligatory columns:
 
-                  >>> LABELS_COLUMN, PATHS_COLUMN
+                  ``LABELS_COLUMN``, ``PATHS_COLUMN``
 
                   and the optional ones:
 
-                  >>> X1_COLUMN, X2_COLUMN, Y1_COLUMN, Y2_COLUMN, CATEGORIES_COLUMN
+                  ``X1_COLUMN``, ``X2_COLUMN``, ``Y1_COLUMN``, ``Y2_COLUMN``, ``CATEGORIES_COLUMN``
 
             extra_data: Dictionary with additional information which we want to put into batches. We assume that
                 the length of each record in this structure is the same as dataset's size.
             transform: Augmentations for the images, set ``None`` to perform only normalisation and casting to tensor
             dataset_root: Path to the images' dir, set ``None`` if you provided the absolute paths in your dataframe
             f_imread: Function to read the images, pass ``None`` so we pick it autmatically based on provided transforms
             cache_size: Size of the dataset's cache
@@ -246,15 +246,15 @@
     def __init__(
         self,
         df: pd.DataFrame,
         extra_data: Optional[Dict[str, Any]] = None,
         dataset_root: Optional[Union[str, Path]] = None,
         transform: Optional[albu.Compose] = None,
         f_imread: Optional[TImReader] = None,
-        cache_size: Optional[int] = 100_000,
+        cache_size: Optional[int] = 0,
         input_tensors_key: str = INPUT_TENSORS_KEY,
         labels_key: str = LABELS_KEY,
         paths_key: str = PATHS_KEY,
         categories_key: str = CATEGORIES_KEY,
         x1_key: str = X1_KEY,
         x2_key: str = X2_KEY,
         y1_key: str = Y1_KEY,
@@ -293,15 +293,15 @@
 def get_retrieval_datasets(
     dataset_root: Path,
     transforms_train: Any,
     transforms_val: Any,
     f_imread_train: Optional[TImReader] = None,
     f_imread_val: Optional[TImReader] = None,
     dataframe_name: str = "df.csv",
-    cache_size: Optional[int] = 100_000,
+    cache_size: Optional[int] = 0,
     verbose: bool = True,
 ) -> Tuple[DatasetWithLabels, DatasetQueryGallery]:
     df = pd.read_csv(dataset_root / dataframe_name, index_col=False)
 
     check_retrieval_dataframe_format(df, dataset_root=dataset_root, verbose=verbose)
 
     # first half will consist of "train" split, second one of "val"
```

### Comparing `open-metric-learning-0.3.9/oml/datasets/list_dataset.py` & `open-metric-learning-0.4.0/oml/datasets/list_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import albumentations as albu
 import numpy as np
 from PIL import Image
 from torch.utils.data import Dataset
 
 from oml.const import INDEX_KEY, INPUT_TENSORS_KEY
 from oml.exceptions import InvalidBBoxesException
-from oml.transforms.images.torchvision.transforms import get_normalisation_torch
+from oml.transforms.images.torchvision import get_normalisation_torch
 from oml.transforms.images.utils import TTransforms, get_im_reader_for_transforms
 from oml.utils.images.images import TImReader
 
 TBBox = Tuple[int, int, int, int]
 TBBoxes = Sequence[Optional[TBBox]]
 
 
@@ -23,15 +23,15 @@
     def __init__(
         self,
         filenames_list: Sequence[Path],
         bboxes: Optional[TBBoxes] = None,
         transform: TTransforms = get_normalisation_torch(),
         f_imread: Optional[TImReader] = None,
         input_tensors_key: str = INPUT_TENSORS_KEY,
-        cache_size: Optional[int] = 100_000,
+        cache_size: Optional[int] = 0,
         index_key: str = INDEX_KEY,
     ):
         """
         Args:
             filenames_list: list of paths to images
             bboxes: Should be either ``None`` or a sequence of bboxes.
                 If an image has ``N`` boxes, duplicate its
@@ -58,15 +58,15 @@
 
         self.validate_bboxes(bboxes, filenames_list)
 
     @staticmethod
     def validate_bboxes(bboxes: Optional[TBBoxes], files: Sequence[Path]) -> None:
         if bboxes is not None:
             if len(bboxes) != len(files):
-                raise InvalidBBoxesException(f"Number of boxes and files missmatch: {len(bboxes)=} != {len(files)}")
+                raise InvalidBBoxesException(f"Number of boxes and files missmatch: {len(bboxes)} != {len(files)}")
             for box, file_ in zip(bboxes, files):
                 if box is not None:
                     if len(box) != 4:
                         raise InvalidBBoxesException(f"Bbox size does not equal to 4: {box} for image {file_}")
                     x1, y1, x2, y2 = box
                     if any(coord < 0 for coord in box):
                         raise InvalidBBoxesException(f"Bbox coordintates cannot be negative. File: {file_}")
```

### Comparing `open-metric-learning-0.3.9/oml/datasets/pairs.py` & `open-metric-learning-0.4.0/oml/datasets/pairs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Optional, Union
 
 from torch import Tensor
 
 from oml.const import INDEX_KEY, PAIR_1ST_KEY, PAIR_2ND_KEY
 from oml.datasets.list_dataset import ListDataset, TBBoxes
 from oml.interfaces.datasets import IPairsDataset
-from oml.transforms.images.torchvision.transforms import get_normalisation_torch
+from oml.transforms.images.torchvision import get_normalisation_torch
 from oml.transforms.images.utils import TTransforms
 from oml.utils.images.images import TImReader, imread_pillow
 
 
 class EmbeddingPairsDataset(IPairsDataset):
     """
     Dataset to iterate over pairs of embeddings.
@@ -65,15 +65,15 @@
         bboxes1: Optional[TBBoxes] = None,
         bboxes2: Optional[TBBoxes] = None,
         transform: Optional[TTransforms] = None,
         f_imread: TImReader = imread_pillow,
         pair_1st_key: str = PAIR_1ST_KEY,
         pair_2nd_key: str = PAIR_2ND_KEY,
         index_key: str = INDEX_KEY,
-        cache_size: Optional[int] = 100_000,
+        cache_size: Optional[int] = 0,
     ):
         """
         Args:
             paths1: Paths to the 1st input images
             paths2: Paths to the 2nd input images
             bboxes1: Should be either ``None`` or a sequence of bboxes.
                 If an image has ``N`` boxes, duplicate its
```

### Comparing `open-metric-learning-0.3.9/oml/datasets/triplet.py` & `open-metric-learning-0.4.0/oml/datasets/triplet.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import albumentations as albu
 import numpy as np
 import torch
 from torch.utils.data import Dataset
 
 from oml.const import INDEX_KEY, INPUT_TENSORS_KEY
-from oml.transforms.images.albumentations.transforms import get_normalisation_albu
+from oml.transforms.images.albumentations import get_normalisation_albu
 from oml.utils.images.images import TImReader, imread_cv2
 
 TPath = Union[Path, str]
 TTriplet = Tuple[TPath, TPath, TPath]
 TItem = Dict[str, Any]
 
 
@@ -24,15 +24,15 @@
     def __init__(
         self,
         triplets: List[TTriplet],
         im_root: Path,
         transforms: albu.Compose,
         expand_ratio: float,
         f_imread: TImReader = imread_cv2,
-        cache_size: Optional[int] = 50_000,
+        cache_size: Optional[int] = 0,
         index_key: str = INDEX_KEY,
     ):
         """
 
         Args:
             triplets: List of triplets
             im_root: Images directory
```

### Comparing `open-metric-learning-0.3.9/oml/ddp/patching.py` & `open-metric-learning-0.4.0/oml/ddp/patching.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/ddp/utils.py` & `open-metric-learning-0.4.0/oml/ddp/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/functional/label_smoothing.py` & `open-metric-learning-0.4.0/oml/functional/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/functional/losses.py` & `open-metric-learning-0.4.0/oml/functional/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/functional/metrics.py` & `open-metric-learning-0.4.0/oml/functional/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     mask_gt: Tensor,
     mask_to_ignore: Optional[Tensor] = None,
     cmc_top_k: Tuple[int, ...] = (5,),
     precision_top_k: Tuple[int, ...] = (5,),
     map_top_k: Tuple[int, ...] = (5,),
     fmr_vals: Tuple[int, ...] = (1,),
     reduce: bool = True,
-    check_dataset_validity: bool = False,
 ) -> TMetricsDict:
     """
     Function to count different retrieval metrics.
 
     Args:
         distances: Distance matrix with the shape of ``[query_size, gallery_size]``
         mask_gt: ``(i,j)`` element indicates if for ``i``-th query ``j``-th gallery is the correct prediction
@@ -35,29 +34,24 @@
         cmc_top_k: Values of ``k`` to calculate ``cmc@k`` (`Cumulative Matching Characteristic`)
         precision_top_k: Values of ``k`` to calculate ``precision@k``
         map_top_k: Values of ``k`` to calculate ``map@k`` (`Mean Average Precision`)
         fmr_vals: Values of ``fmr`` (measured in quantiles) to calculate ``fnmr@fmr`` (`False Non Match Rate
                   at the given False Match Rate`).
                   For example, if ``fmr_values`` is (0.2, 0.4) we will calculate ``fnmr@fmr=0.2`` and ``fnmr@fmr=0.4``
         reduce: If ``False`` return metrics for each query without averaging
-        check_dataset_validity: Set ``True`` if you want to check that we have available answers in the gallery for
-         each of the queries
 
     Returns:
         Metrics dictionary.
 
     """
     top_k_args = [cmc_top_k, precision_top_k, map_top_k]
 
     if not any(top_k_args + [fmr_vals]):
         raise ValueError("You must specify arguments for at leas 1 metric to calculate it")
 
-    if check_dataset_validity:
-        validate_dataset(mask_gt=mask_gt, mask_to_ignore=mask_to_ignore)
-
     if distances.shape != mask_gt.shape:
         raise ValueError(
             f"Distances matrix has the shape of {distances.shape}, "
             f"but mask_to_ignore has the shape of {mask_gt.shape}."
         )
 
     if (mask_to_ignore is not None) and (mask_to_ignore.shape != distances.shape):
@@ -366,23 +360,24 @@
 
     Given a list :math:`g=[g_1, \\ldots, g_k]` of ground truth top :math:`k` closest elements from the gallery to
     a given query (:math:`g_i` is 1 if :math:`i`-th element from the gallery is relevant to the query and 0 otherwise),
     and the total number of relevant elements from the gallery :math:`n`, the :math:`\\textrm{map}@k`
     for the query is defined as
 
     .. math::
-        \\begin{split}\\textrm{map}@k &=
-        \\frac{1}{\\min{\\left(k, n\\right)}}\\sum\\limits_{i = 1}^k
-        \\frac{\\textrm{# of relevant elements among top } i\\textrm{ elements}}{i} \\times \\textrm{rel}(i) = \\\\
-        & = \\frac{1}{\\min{\\left(k, n\\right)}}\\sum\\limits_{i = 1}^k
-        \\frac{\\sum\\limits_{j = 1}^{i}g_j}{i} \\times \\textrm{rel}(i)
+        \\begin{split}
+        \\textrm{map}@k &=
+        \\frac{1}{n_k}\\sum\\limits_{i = 1}^k
+        \\frac{n_i}{i} \\times \\textrm{rel}(i)
         \\end{split}
 
     where :math:`\\textrm{rel}(i)` is 1 if :math:`i`-th element from the top :math:`i` closest
-    elements from the gallery to the query is relevant to the query, and 0 otherwise.
+    elements from the gallery to the query is relevant to the query, and 0 otherwise;
+    and :math:`n_i = \\sum\\limits_{j = 1}^{i}g_j`, which is the number of the relevant predictions
+    among the first :math:`i` outputs.
 
     See:
 
         `Evaluation measures (information retrieval). Mean Average Precision`_
 
         `Mean Average Precision (MAP) For Recommender Systems`_
 
@@ -396,24 +391,25 @@
         >>> gt_tops = torch.tensor([
         ...                         [1, 0],
         ...                         [0, 1],
         ...                         [0, 0]
         ... ], dtype=torch.bool)
         >>> n_gt = torch.tensor([2, 3, 5])
         >>> calc_map(gt_tops, n_gt, top_k=(1, 2))
-        [tensor([1., 0., 0.]), tensor([0.5000, 0.2500, 0.0000])]
+        [tensor([1., 0., 0.]), tensor([1.0000, 0.5000, 0.0000])]
     """
     check_if_nonempty_positive_integers(top_k, "top_k")
     top_k = _clip_max_with_warning(top_k, gt_tops.shape[1])
     map = []
     correct_preds = torch.cumsum(gt_tops.float(), dim=1)
     for k in top_k:
-        _n_gt = torch.min(n_gt, torch.tensor(k).unsqueeze(0))
-        positions = torch.arange(1, k + 1).unsqueeze(0)
-        map.append(torch.sum((correct_preds[:, :k] / positions) * gt_tops[:, :k], dim=1) / _n_gt)
+        positions = torch.arange(1, k + 1).unsqueeze(0).to(correct_preds.device)
+        n_k = correct_preds[:, k - 1].clone()
+        n_k[n_k < 1] = torch.inf  # hack to avoid zero division
+        map.append(torch.sum((correct_preds[:, :k] / positions) * gt_tops[:, :k], dim=1) / n_k)
     return map
 
 
 def calc_fnmr_at_fmr(pos_dist: Tensor, neg_dist: Tensor, fmr_vals: Tuple[float, ...] = (0.1,)) -> Tensor:
     """
     Function to compute False Non Match Rate (FNMR) value when False Match Rate (FMR) value
     is equal to ``fmr_vals``.
@@ -563,20 +559,14 @@
         neg_dist = distances[~mask_gt & mask_to_not_ignore]
     else:
         pos_dist = distances[mask_gt]
         neg_dist = distances[~mask_gt]
     return pos_dist, neg_dist
 
 
-def validate_dataset(mask_gt: Tensor, mask_to_ignore: Tensor) -> None:
-    assert (
-        (mask_gt & ~mask_to_ignore).any(1).all()
-    ), "There are queries without available correct answers in the gallery!"
-
-
 def _to_tensor(array: Union[np.ndarray, Tensor]) -> Tensor:
     if isinstance(array, Tensor):
         return array
     elif isinstance(array, np.ndarray):
         return torch.from_numpy(array)
     else:
         raise TypeError("Wrong type")
```

### Comparing `open-metric-learning-0.3.9/oml/inference/abstract.py` & `open-metric-learning-0.4.0/oml/inference/abstract.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/inference/flat.py` & `open-metric-learning-0.4.0/oml/inference/flat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 import torch
 from pandas import DataFrame
 from torch import Tensor, nn
 
 from oml.const import PATHS_COLUMN, SPLIT_COLUMN
@@ -45,31 +45,31 @@
         accumulate_on_cpu=accumulate_on_cpu,
     )
 
     return outputs
 
 
 def inference_on_dataframe(
-    dataset_root: Path,
+    dataset_root: Union[Path, str],
     dataframe_name: str,
-    output_cache_path: Optional[Path],
     extractor: IExtractor,
     transforms_extraction: TTransforms,
-    num_workers: int,
-    batch_size: int,
-    use_fp16: bool,
+    output_cache_path: Optional[Union[str, Path]] = None,
+    num_workers: int = 0,
+    batch_size: int = 128,
+    use_fp16: bool = False,
 ) -> Tuple[Tensor, Tensor, DataFrame, DataFrame]:
-    df = pd.read_csv(dataset_root / dataframe_name)
+    df = pd.read_csv(Path(dataset_root) / dataframe_name)
 
     # it has now affect if paths are global already
     df[PATHS_COLUMN] = df[PATHS_COLUMN].apply(lambda x: Path(dataset_root) / x)
 
     check_retrieval_dataframe_format(df)
 
-    if (output_cache_path is not None) and output_cache_path.is_file():
+    if (output_cache_path is not None) and Path(output_cache_path).is_file():
         embeddings = torch.load(output_cache_path, map_location="cpu")
         print("Embeddings have been loaded from the disk.")
     else:
         embeddings = inference_on_images(
             model=extractor,
             paths=df[PATHS_COLUMN],
             transform=transforms_extraction,
```

### Comparing `open-metric-learning-0.3.9/oml/inference/pairs.py` & `open-metric-learning-0.4.0/oml/inference/pairs.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     def _apply(
         model_: IPairwiseModel,
         batch_: Dict[str, Any],
     ) -> Tensor:
         pair1 = batch_[dataset.pair_1st_key][dataset.dataset1.input_tensors_key].to(device)
         pair2 = batch_[dataset.pair_2nd_key][dataset.dataset2.input_tensors_key].to(device)
-        return model_(pair1, pair2)
+        return model_.predict(pair1, pair2)
 
     output = _inference(
         model=model,
         apply_model=_apply,
         dataset=dataset,
         num_workers=num_workers,
         batch_size=batch_size,
@@ -71,15 +71,15 @@
 
     def _apply(
         model_: IPairwiseModel,
         batch_: Dict[str, Any],
     ) -> Tensor:
         pair1 = batch_[dataset.pair_1st_key].to(device)
         pair2 = batch_[dataset.pair_2nd_key].to(device)
-        return model_(pair1, pair2)
+        return model_.predict(pair1, pair2)
 
     output = _inference(
         model=model,
         apply_model=_apply,
         dataset=dataset,
         num_workers=num_workers,
         batch_size=batch_size,
```

### Comparing `open-metric-learning-0.3.9/oml/interfaces/criterions.py` & `open-metric-learning-0.4.0/oml/interfaces/criterions.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/interfaces/datasets.py` & `open-metric-learning-0.4.0/oml/interfaces/datasets.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 
         Args:
             item: Idx of the sample
 
         Returns:
              Dictionary with the following keys:
 
-            >>> self.input_tensors_key
-            >>> self.labels_key
-            >>> self.index_key
+            ``self.input_tensors_key``
+            ``self.labels_key``
+            ``self.index_key``
 
         """
         raise NotImplementedError()
 
     @abstractmethod
     def get_labels(self) -> np.ndarray:
         raise NotImplementedError()
@@ -65,19 +65,19 @@
         """
         Args:
             item: Idx of the sample
 
         Returns:
              Dictionary with the following keys:
 
-            >>> self.input_tensors_key
-            >>> self.labels_key
-            >>> self.is_query_key
-            >>> self.is_gallery_key
-            >>> self.index_key
+            ``self.input_tensors_key``
+            ``self.labels_key``
+            ``self.is_query_key``
+            ``self.is_gallery_key``
+            ``self.index_key``
 
         """
         raise NotImplementedError()
 
 
 class IPairsDataset(Dataset, ABC):
     """
@@ -94,16 +94,16 @@
         """
         Args:
             item: Idx of the sample
 
         Returns:
              Dictionary with the following keys:
 
-            >>> self.pairs_1st_key
-            >>> self.pairs_2nd_key
-            >>> self.index_key
+            ``self.pairs_1st_key``
+            ``self.pairs_2nd_key``
+            ``self.index_key``
 
         """
         raise NotImplementedError()
 
 
 __all__ = ["IDatasetWithLabels", "IDatasetQueryGallery", "IPairsDataset"]
```

### Comparing `open-metric-learning-0.3.9/oml/interfaces/metrics.py` & `open-metric-learning-0.4.0/oml/interfaces/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,15 @@
     metric_name = "BASE"
     overall_categories_key = OVERALL_CATEGORIES_KEY
 
     @abstractmethod
     def setup(self, *args: Any, **kwargs: Any) -> Any:
         """
         Method for preparing metrics to work: memory allocation, placeholder preparation, etc.
-        Has to be called before the first call of
-
-        >>> self.update_data()
+        Has to be called before the first call of ``self.update_data()``.
 
         """
         raise NotImplementedError()
 
     @abstractmethod
     def update_data(self, *args: Any, **kwargs: Any) -> Any:
         """
```

### Comparing `open-metric-learning-0.3.9/oml/interfaces/miners.py` & `open-metric-learning-0.4.0/oml/interfaces/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/interfaces/retrieval.py` & `open-metric-learning-0.4.0/oml/interfaces/retrieval.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/interfaces/samplers.py` & `open-metric-learning-0.4.0/oml/interfaces/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/lightning/callbacks/metric.py` & `open-metric-learning-0.4.0/oml/lightning/callbacks/metric.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/lightning/entrypoints/parser.py` & `open-metric-learning-0.4.0/oml/lightning/pipelines/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import warnings
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import albumentations as albu
 import torch
 from pytorch_lightning.callbacks import ModelCheckpoint
 from pytorch_lightning.loggers import NeptuneLogger
@@ -64,14 +65,20 @@
     Logger initialisation.
 
     If Neptune Logger is used, we also upload to its cloud some files
     which are good to have for reproducibility.
 
     """
     if ("NEPTUNE_API_TOKEN" in os.environ.keys()) and (cfg["neptune_project"] is not None):
+        warnings.warn(
+            "Unfortunately, in the case of using Neptune, you may experience that long experiments are"
+            "stacked and not responding. It's not an issue on OML's side, so, we cannot fix it. You can use"
+            "Tensorboard logger instead, for this simply leave <NEPTUNE_API_TOKEN> unfilled."
+        )
+
         cwd = Path.cwd()
         logger = NeptuneLogger(
             api_key=os.environ["NEPTUNE_API_TOKEN"],
             project=cfg["neptune_project"],
             tags=list(cfg.get("tags", [])) + [cfg.get("postfix", "")] + [cwd.name],
             log_model_checkpoints=False,
         )
```

### Comparing `open-metric-learning-0.3.9/oml/lightning/entrypoints/train.py` & `open-metric-learning-0.4.0/oml/lightning/pipelines/train.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 import pytorch_lightning as pl
 from torch.utils.data import DataLoader
 
 from oml.const import TCfg
 from oml.datasets.base import get_retrieval_datasets
 from oml.lightning.callbacks.metric import MetricValCallback, MetricValCallbackDDP
-from oml.lightning.entrypoints.parser import (
+from oml.lightning.modules.extractor import ExtractorModule, ExtractorModuleDDP
+from oml.lightning.pipelines.parser import (
     check_is_config_for_ddp,
     initialize_logging,
     parse_ckpt_callback_from_config,
     parse_engine_params_from_config,
     parse_sampler_from_config,
     parse_scheduler_from_config,
 )
-from oml.lightning.modules.retrieval import RetrievalModule, RetrievalModuleDDP
 from oml.metrics.embeddings import EmbeddingMetrics, EmbeddingMetricsDDP
 from oml.registry.losses import get_criterion_by_cfg
 from oml.registry.models import get_extractor_by_cfg
 from oml.registry.optimizers import get_optimizer_by_cfg
 from oml.registry.transforms import get_transforms_by_cfg
 from oml.utils.misc import dictconfig_to_dict, load_dotenv, set_global_seed
 
@@ -53,20 +53,21 @@
         )
 
     loader_val = DataLoader(dataset=valid_dataset, batch_size=cfg["bs_val"], num_workers=cfg["num_workers"])
 
     return loader_train, loader_val
 
 
-def pl_train(cfg: TCfg) -> None:
+def extractor_training_pipeline(cfg: TCfg) -> None:
     """
-    This is an entrypoint for the model training in metric learning setup.
+    This pipeline allows you to train and validate a feature extractor which
+    represents images as feature vectors.
 
     The config can be specified as a dictionary or with hydra: https://hydra.cc/.
-    For more details look at ``examples/README.md``
+    For more details look at ``pipelines/features_extraction/README.md``
 
     """
     # Here we try to load NEPTUNE_API_TOKEN from .env file
     # You can also set it up via `export NEPTUNE_API_TOKEN=...`
     load_dotenv()
 
     set_global_seed(cfg["seed"])
@@ -75,32 +76,32 @@
     pprint(cfg)
     logger = initialize_logging(cfg)
 
     trainer_engine_params = parse_engine_params_from_config(cfg)
     is_ddp = check_is_config_for_ddp(trainer_engine_params)
 
     loader_train, loaders_val = get_retrieval_loaders(cfg)
-    extractor = get_extractor_by_cfg(cfg["model"])
+    extractor = get_extractor_by_cfg(cfg["extractor"])
     criterion = get_criterion_by_cfg(cfg["criterion"], **{"label2category": loader_train.dataset.get_label2category()})
     optimizable_parameters = [
         {"lr": cfg["optimizer"]["args"]["lr"], "params": extractor.parameters()},
         {"lr": cfg["optimizer"]["args"]["lr"], "params": criterion.parameters()},
     ]
     optimizer = get_optimizer_by_cfg(cfg["optimizer"], **{"params": optimizable_parameters})  # type: ignore
 
     module_kwargs = {}
     module_kwargs.update(parse_scheduler_from_config(cfg, optimizer=optimizer))
     if is_ddp:
         module_kwargs.update({"loaders_train": loader_train, "loaders_val": loaders_val})
-        module_constructor = RetrievalModuleDDP
+        module_constructor = ExtractorModuleDDP
     else:
-        module_constructor = RetrievalModule  # type: ignore
+        module_constructor = ExtractorModule  # type: ignore
 
     pl_module = module_constructor(
-        model=extractor,
+        extractor=extractor,
         criterion=criterion,
         optimizer=optimizer,
         input_tensors_key=loader_train.dataset.input_tensors_key,
         labels_key=loader_train.dataset.labels_key,
         freeze_n_epochs=cfg.get("freeze_n_epochs", 0),
         **module_kwargs,
     )
@@ -130,16 +131,17 @@
         enable_checkpointing=True,
         enable_progress_bar=True,
         enable_model_summary=True,
         callbacks=[metrics_clb, parse_ckpt_callback_from_config(cfg)],
         logger=logger,
         precision=cfg.get("precision", 32),
         **trainer_engine_params,
+        **cfg.get("lightning_trainer_extra_args", {}),
     )
 
     if is_ddp:
         trainer.fit(model=pl_module)
     else:
         trainer.fit(model=pl_module, train_dataloaders=loader_train, val_dataloaders=loaders_val)
 
 
-__all__ = ["pl_train"]
+__all__ = ["extractor_training_pipeline"]
```

### Comparing `open-metric-learning-0.3.9/oml/lightning/entrypoints/train_postprocessor.py` & `open-metric-learning-0.4.0/oml/lightning/pipelines/train_postprocessor.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,33 +9,36 @@
 from omegaconf import DictConfig
 from torch import device as tdevice
 from torch.utils.data import DataLoader
 
 from oml.const import BBOXES_COLUMNS, EMBEDDINGS_KEY, TCfg
 from oml.datasets.base import DatasetQueryGallery, DatasetWithLabels
 from oml.inference.flat import inference_on_dataframe
+from oml.interfaces.models import IPairwiseModel
 from oml.lightning.callbacks.metric import MetricValCallback, MetricValCallbackDDP
-from oml.lightning.entrypoints.parser import (
+from oml.lightning.modules.pairwise_postprocessing import (
+    PairwiseModule,
+    PairwiseModuleDDP,
+)
+from oml.lightning.pipelines.parser import (
     check_is_config_for_ddp,
     initialize_logging,
     parse_ckpt_callback_from_config,
     parse_engine_params_from_config,
     parse_sampler_from_config,
     parse_scheduler_from_config,
 )
-from oml.lightning.modules.pairwise_postprocessing import (
-    PairwiseModule,
-    PairwiseModuleDDP,
-)
 from oml.metrics.embeddings import EmbeddingMetrics, EmbeddingMetricsDDP
 from oml.miners.pairs import PairsMiner
-from oml.registry.models import get_extractor_by_cfg, get_pairwise_model_by_cfg
+from oml.registry.models import get_extractor_by_cfg
 from oml.registry.optimizers import get_optimizer_by_cfg
+from oml.registry.postprocessors import get_postprocessor_by_cfg
 from oml.registry.transforms import get_transforms_by_cfg
 from oml.retrieval.postprocessors.pairwise import PairwiseImagesPostprocessor
+from oml.transforms.images.torchvision import get_normalisation_resize_torch
 from oml.utils.misc import (
     dictconfig_to_dict,
     flatten_dict,
     load_dotenv,
     set_global_seed,
 )
 
@@ -75,89 +78,92 @@
     emb_train, emb_val, df_train, df_val = inference_on_dataframe(
         extractor=extractor,
         dataset_root=cfg["dataset_root"],
         output_cache_path=cache_file,
         dataframe_name=cfg["dataframe_name"],
         transforms_extraction=get_transforms_by_cfg(cfg["transforms_extraction"]),
         num_workers=cfg["num_workers"],
-        batch_size=cfg["bs_val"],
+        batch_size=cfg["batch_size_inference"],
         use_fp16=int(cfg.get("precision", 32)) == 16,
     )
 
     train_dataset = DatasetWithLabels(
         df=df_train,
         transform=get_transforms_by_cfg(cfg["transforms_train"]),
         extra_data={EMBEDDINGS_KEY: emb_train},
     )
 
     valid_dataset = DatasetQueryGallery(
         df=df_val,
-        transform=get_transforms_by_cfg(cfg["transforms_val"]),
+        # we don't care about transforms, since the only goal of this dataset is to deliver embeddings
+        transform=get_normalisation_resize_torch(im_size=8),
         extra_data={EMBEDDINGS_KEY: emb_val},
     )
 
     sampler = parse_sampler_from_config(cfg, dataset=train_dataset)
     assert sampler is not None
     loader_train = DataLoader(batch_sampler=sampler, dataset=train_dataset, num_workers=cfg["num_workers"])
 
     loader_val = DataLoader(
-        dataset=valid_dataset, batch_size=cfg["bs_val"], num_workers=cfg["num_workers"], shuffle=False
+        dataset=valid_dataset, batch_size=cfg["batch_size_inference"], num_workers=cfg["num_workers"], shuffle=False
     )
 
     return loader_train, loader_val
 
 
-def pl_train_postprocessor(cfg: DictConfig) -> None:
+def postprocessor_training_pipeline(cfg: DictConfig) -> None:
+    """
+    This pipeline allows you to train and validate a pairwise postprocessor
+    which fixes mistakes of a feature extractor in retrieval setup.
+
+    The config can be specified as a dictionary or with hydra: https://hydra.cc/.
+    For more details look at ``pipelines/postprocessing/pairwise_postprocessing/README.md``
+
+    """
     load_dotenv()
 
     set_global_seed(cfg["seed"])
 
     cfg = dictconfig_to_dict(cfg)
     pprint(cfg)
     logger = initialize_logging(cfg)
 
     trainer_engine_params = parse_engine_params_from_config(cfg)
     is_ddp = check_is_config_for_ddp(trainer_engine_params)
 
     loader_train, loader_val = get_loaders_with_embeddings(cfg)
 
-    siamese = get_pairwise_model_by_cfg(cfg["pairwise_model"])
+    postprocessor = None if not cfg.get("postprocessor", None) else get_postprocessor_by_cfg(cfg["postprocessor"])
+    assert isinstance(postprocessor, PairwiseImagesPostprocessor), "We support only images processing in this pipeline."
+    assert isinstance(postprocessor.model, IPairwiseModel), f"You model must be a child of {IPairwiseModel.__name__}"
+
     criterion = torch.nn.BCEWithLogitsLoss()
     pairs_miner = PairsMiner(hard_mining=cfg["hard_pairs_mining"])
-    optimizer = get_optimizer_by_cfg(cfg["optimizer"], **{"params": siamese.parameters()})
+    optimizer = get_optimizer_by_cfg(cfg["optimizer"], **{"params": postprocessor.model.parameters()})
 
     module_kwargs = {}
     module_kwargs.update(parse_scheduler_from_config(cfg, optimizer=optimizer))
     if is_ddp:
         module_kwargs.update({"loaders_train": loader_train, "loaders_val": loader_val})
         module_constructor = PairwiseModuleDDP
     else:
         module_constructor = PairwiseModule  # type: ignore
 
     pl_module = module_constructor(
-        pairwise_model=siamese,
+        pairwise_model=postprocessor.model,
         pairs_miner=pairs_miner,
         criterion=criterion,
         optimizer=optimizer,
         input_tensors_key=loader_train.dataset.input_tensors_key,
         labels_key=loader_train.dataset.labels_key,
         embeddings_key=EMBEDDINGS_KEY,
         freeze_n_epochs=cfg.get("freeze_n_epochs", 0),
         **module_kwargs,
     )
 
-    postprocessor = PairwiseImagesPostprocessor(
-        pairwise_model=siamese,
-        top_n=cfg["postprocessing_top_n"],
-        transforms=get_transforms_by_cfg(cfg["transforms_val"]),
-        batch_size=cfg["bs_val"],
-        num_workers=cfg["num_workers"],
-        use_fp16=int(cfg.get("precision", 32)) == 16,
-    )
-
     metrics_constructor = EmbeddingMetricsDDP if is_ddp else EmbeddingMetrics
     metrics_calc = metrics_constructor(
         embeddings_key=pl_module.embeddings_key,
         categories_key=loader_val.dataset.categories_key,
         labels_key=loader_val.dataset.labels_key,
         is_query_key=loader_val.dataset.is_query_key,
         is_gallery_key=loader_val.dataset.is_gallery_key,
@@ -185,8 +191,8 @@
 
     if is_ddp:
         trainer.fit(model=pl_module)
     else:
         trainer.fit(model=pl_module, train_dataloaders=loader_train, val_dataloaders=loader_val)
 
 
-__all__ = ["pl_train_postprocessor"]
+__all__ = ["postprocessor_training_pipeline"]
```

### Comparing `open-metric-learning-0.3.9/oml/lightning/modules/ddp.py` & `open-metric-learning-0.4.0/oml/lightning/modules/ddp.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/lightning/modules/pairwise_postprocessing.py` & `open-metric-learning-0.4.0/oml/lightning/modules/pairwise_postprocessing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/lightning/modules/retrieval.py` & `open-metric-learning-0.4.0/oml/lightning/modules/extractor.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 from torch.optim.lr_scheduler import ReduceLROnPlateau, _LRScheduler
 
 from oml.const import EMBEDDINGS_KEY, INPUT_TENSORS_KEY, LABELS_KEY
 from oml.interfaces.models import IExtractor, IFreezable
 from oml.lightning.modules.ddp import ModuleDDP
 
 
-class RetrievalModule(pl.LightningModule):
+class ExtractorModule(pl.LightningModule):
     """
     This is a base module to train your model with Lightning.
 
     """
 
     def __init__(
         self,
-        model: IExtractor,
+        extractor: IExtractor,
         criterion: nn.Module,
         optimizer: torch.optim.Optimizer,
         scheduler: Optional[_LRScheduler] = None,
         scheduler_interval: str = "step",
         scheduler_frequency: int = 1,
         input_tensors_key: str = INPUT_TENSORS_KEY,
         labels_key: str = LABELS_KEY,
         embeddings_key: str = EMBEDDINGS_KEY,
         scheduler_monitor_metric: Optional[str] = None,
         freeze_n_epochs: int = 0,
     ):
         """
 
         Args:
-            model: Model to train
+            extractor: Extractor to train
             criterion: Criterion to optimize
             optimizer: Optimizer
             scheduler: Learning rate scheduler
             scheduler_interval: Interval of calling scheduler (must be ``step`` or ``epoch``)
             scheduler_frequency: Frequency of calling scheduler
             input_tensors_key: Key to get tensors from the batches
             labels_key: Key to get labels from the batches
@@ -47,30 +47,30 @@
             freeze_n_epochs: number of epochs to freeze model (for n > 0 model has to be a successor of ``IFreezable``
                 interface). When ``current_epoch >= freeze_n_epochs`` model is unfreezed. Note that epochs are
                 starting with 0.
 
         """
         pl.LightningModule.__init__(self)
 
-        self.model = model
+        self.model = extractor
         self.criterion = criterion
         self.optimizer = optimizer
 
         self.monitor_metric = scheduler_monitor_metric
         self.scheduler = scheduler
         self.scheduler_interval = scheduler_interval
         self.scheduler_frequency = scheduler_frequency
 
         self.input_tensors_key = input_tensors_key
         self.labels_key = labels_key
         self.embeddings_key = embeddings_key
 
         self.freeze_n_epochs = freeze_n_epochs
         assert freeze_n_epochs == 0 or isinstance(
-            model, IFreezable
+            extractor, IFreezable
         ), f"Model must be {IFreezable.__name__} to use this."
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         embeddings = self.model(x)
         return embeddings
 
     def training_step(self, batch: Dict[str, Any], batch_idx: int) -> torch.Tensor:
@@ -122,25 +122,25 @@
 
             if self.current_epoch >= self.freeze_n_epochs:
                 self.model.unfreeze()
             else:
                 self.model.freeze()
 
 
-class RetrievalModuleDDP(RetrievalModule, ModuleDDP):
+class ExtractorModuleDDP(ExtractorModule, ModuleDDP):
     """
     This is a base module for the training of your model with Lightning in DDP.
 
     """
 
     def __init__(
         self,
         loaders_train: Optional[TRAIN_DATALOADERS] = None,
         loaders_val: Optional[EVAL_DATALOADERS] = None,
         *args: Any,
         **kwargs: Any,
     ):
         ModuleDDP.__init__(self, loaders_train=loaders_train, loaders_val=loaders_val)
-        RetrievalModule.__init__(self, *args, **kwargs)
+        ExtractorModule.__init__(self, *args, **kwargs)
 
 
-__all__ = ["RetrievalModule", "RetrievalModuleDDP"]
+__all__ = ["ExtractorModule", "ExtractorModuleDDP"]
```

### Comparing `open-metric-learning-0.3.9/oml/losses/arcface.py` & `open-metric-learning-0.4.0/oml/losses/arcface.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/losses/surrogate_precision.py` & `open-metric-learning-0.4.0/oml/losses/surrogate_precision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/losses/triplet.py` & `open-metric-learning-0.4.0/oml/losses/triplet.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,18 @@
 
         """
         n = len(features)
         assert n % 3 == 0
 
         anchor_ii, positive_ii, negative_ii = get_tri_ids_in_plain(n)
 
-        return self.criterion(features[anchor_ii], features[positive_ii], features[negative_ii])
+        loss = self.criterion(features[anchor_ii], features[positive_ii], features[negative_ii])
+        self.last_logs = self.criterion.last_logs
+
+        return loss
 
 
 class TripletLossWithMiner(ITripletLossWithMiner):
     """
     This class combines `Miner` and `TripletLoss`.
 
     """
```

### Comparing `open-metric-learning-0.3.9/oml/metrics/accumulation.py` & `open-metric-learning-0.4.0/oml/metrics/accumulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
     def __init__(self, keys_to_accumulate: Sequence[str]):
         """
         Class for accumulating values of different types, for instance,
         torch.Tensor and numpy.array.
 
         Args:
             keys_to_accumulate: List or tuple of keys to be collected.
-                                 We will take values via these keys calling
-                                 >>> self.update_data()
+                                 We will take values via these keys calling ``self.update_data()``.
         """
         assert len(keys_to_accumulate) == len(set(keys_to_accumulate)), "All the keys have to be unique!"
 
         self.keys_to_accumulate = keys_to_accumulate
         self.num_samples = None
 
         self._collected_samples = 0
@@ -75,16 +74,15 @@
             self._storage[key].extend(list(batch_value))  # type: ignore
         else:
             raise TypeError(f"Type '{type(batch_value)}' is not available for accumulating")
 
     def update_data(self, data_dict: Dict[str, Any]) -> None:
         """
         Args:
-            data_dict: We will accumulate data getting values via
-            >>> self.keys_to_accumulate
+            data_dict: We will accumulate data getting values via ``self.keys_to_accumulate``.
 
         """
         bs_values = [len(data_dict[k]) for k in self.keys_to_accumulate]
         bs = bs_values[0]
         assert all(bs == bs_value for bs_value in bs_values), f"Lengths of data are not equal, lengths: {bs_values}"
 
         for k in self.keys_to_accumulate:
```

### Comparing `open-metric-learning-0.3.9/oml/metrics/embeddings.py` & `open-metric-learning-0.4.0/oml/metrics/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from copy import deepcopy
 from pprint import pprint
 from typing import Any, Collection, Dict, Iterable, List, Optional, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
+from torch import Tensor
 
 from oml.const import (
     BLUE,
     EMBEDDINGS_KEY,
     GRAY,
     GREEN,
     IS_GALLERY_KEY,
@@ -41,14 +42,20 @@
 from oml.metrics.accumulation import Accumulator
 from oml.utils.images.images import get_img_with_bbox, square_pad
 from oml.utils.misc import flatten_dict
 
 TMetricsDict_ByLabels = Dict[Union[str, int], TMetricsDict]
 
 
+def validate_dataset(mask_gt: Tensor, mask_to_ignore: Tensor) -> None:
+    assert (
+        (mask_gt & ~mask_to_ignore).any(1).all()
+    ), "There are queries without available correct answers in the gallery!"
+
+
 class EmbeddingMetrics(IMetricVisualisable):
     """
     This class accumulates the information from the batches and embeddings produced by the model
     at every batch in epoch. After all the samples have been stored, you can call the function
     which computes retrievals metrics. To get the needed information from the batches, it uses
     keys which have to be provided as init arguments. Please, check the usage example in
     `Readme`.
@@ -68,15 +75,14 @@
         precision_top_k: Tuple[int, ...] = (5,),
         map_top_k: Tuple[int, ...] = (5,),
         fmr_vals: Tuple[float, ...] = tuple(),
         pfc_variance: Tuple[float, ...] = (0.5,),
         categories_key: Optional[str] = None,
         postprocessor: Optional[IDistancesPostprocessor] = None,
         metrics_to_exclude_from_visualization: Iterable[str] = (),
-        check_dataset_validity: bool = True,
         return_only_main_category: bool = False,
         visualize_only_main_category: bool = True,
         verbose: bool = True,
     ):
         """
 
         Args:
@@ -97,16 +103,14 @@
             pfc_variance: Values in range [0, 1]. Find the number of components such that the amount
                           of variance that needs to be explained is greater than the percentage specified
                           by ``pfc_variance``.
             categories_key: Key to take the samples' categories from the batches (if you have ones)
             postprocessor: Postprocessor which applies some techniques like query reranking
             metrics_to_exclude_from_visualization: Names of the metrics to exclude from the visualization. It will not
              affect calculations.
-            check_dataset_validity: Set ``True`` if you want to check if all the queries have valid answers in the
-             gallery set
             return_only_main_category: Whether you want to return only the main category from ``.compute_metrics()``
             visualize_only_main_category: Whether you want to visualize only the main category with ``.visualize()``
             verbose: Set ``True`` if you want to print metrics
 
         """
         self.embeddings_key = embeddings_key
         self.labels_key = labels_key
@@ -122,17 +126,15 @@
         self.categories_key = categories_key
         self.postprocessor = postprocessor
 
         self.distance_matrix = None
         self.mask_gt = None
         self.metrics = None
         self.metrics_unreduced = None
-        self.mask_to_ignore = None
 
-        self.check_dataset_validity = check_dataset_validity
         self.visualize_only_main_category = visualize_only_main_category
         self.return_only_main_category = return_only_main_category
 
         self.metrics_to_exclude_from_visualization = ["fnmr@fmr", "pcf", *metrics_to_exclude_from_visualization]
         self.verbose = verbose
 
         keys_to_accumulate = [self.embeddings_key, self.is_query_key, self.is_gallery_key, self.labels_key]
@@ -146,32 +148,37 @@
         self.keys_to_accumulate = tuple(set(keys_to_accumulate))
         self.acc = Accumulator(keys_to_accumulate=self.keys_to_accumulate)
 
     def setup(self, num_samples: int) -> None:  # type: ignore
         self.distance_matrix = None
         self.mask_gt = None
         self.metrics = None
-        self.mask_to_ignore = None
 
         self.acc.refresh(num_samples=num_samples)
 
     def update_data(self, data_dict: Dict[str, Any]) -> None:  # type: ignore
         self.acc.update_data(data_dict=data_dict)
 
     def _calc_matrices(self) -> None:
         embeddings = self.acc.storage[self.embeddings_key]
         labels = self.acc.storage[self.labels_key]
         is_query = self.acc.storage[self.is_query_key]
         is_gallery = self.acc.storage[self.is_gallery_key]
 
         # Note, in some datasets part of the samples may appear in both query & gallery.
         # Here we handle this case to avoid picking an item itself as the nearest neighbour for itself
-        self.mask_to_ignore = calc_mask_to_ignore(is_query=is_query, is_gallery=is_gallery)
-        self.mask_gt = calc_gt_mask(labels=labels, is_query=is_query, is_gallery=is_gallery)
-        self.distance_matrix = calc_distance_matrix(embeddings=embeddings, is_query=is_query, is_gallery=is_gallery)
+        mask_to_ignore = calc_mask_to_ignore(is_query=is_query, is_gallery=is_gallery)
+        mask_gt = calc_gt_mask(labels=labels, is_query=is_query, is_gallery=is_gallery)
+        distance_matrix = calc_distance_matrix(embeddings=embeddings, is_query=is_query, is_gallery=is_gallery)
+
+        self.distance_matrix, self.mask_gt = apply_mask_to_ignore(
+            distances=distance_matrix, mask_gt=mask_gt, mask_to_ignore=mask_to_ignore
+        )
+
+        validate_dataset(mask_gt=self.mask_gt, mask_to_ignore=mask_to_ignore)
 
         if self.postprocessor:
             self.distance_matrix = self.postprocessor.process_by_dict(self.distance_matrix, data=self.acc.storage)
 
     def compute_metrics(self) -> TMetricsDict_ByLabels:  # type: ignore
         if not self.acc.is_storage_full():
             raise ValueError(
@@ -192,17 +199,16 @@
 
         metrics: TMetricsDict_ByLabels = dict()
 
         # note, here we do micro averaging
         metrics[self.overall_categories_key] = calc_retrieval_metrics(
             distances=self.distance_matrix,
             mask_gt=self.mask_gt,
-            mask_to_ignore=self.mask_to_ignore,
-            check_dataset_validity=self.check_dataset_validity,
             reduce=False,
+            mask_to_ignore=None,  # we already applied it
             **args_retrieval_metrics,  # type: ignore
         )
 
         embeddings = self.acc.storage[self.embeddings_key]
         metrics[self.overall_categories_key].update(calc_topological_metrics(embeddings, **args_topological_metrics))
 
         if self.categories_key is not None:
@@ -212,16 +218,16 @@
 
             for category in np.unique(query_categories):
                 mask = query_categories == category
 
                 metrics[category] = calc_retrieval_metrics(
                     distances=self.distance_matrix[mask],  # type: ignore
                     mask_gt=self.mask_gt[mask],  # type: ignore
-                    mask_to_ignore=self.mask_to_ignore[mask],  # type: ignore
                     reduce=False,
+                    mask_to_ignore=None,  # we already applied it
                     **args_retrieval_metrics,  # type: ignore
                 )
 
                 mask = categories == category
                 metrics[category].update(calc_topological_metrics(embeddings[mask], **args_topological_metrics))
 
         self.metrics_unreduced = metrics  # type: ignore
@@ -279,16 +285,14 @@
             query_ids: Index of the query
             n_instances: Amount of the predictions to show
             verbose: wether to show image paths or not
 
         """
         assert self.metrics is not None, "We are not ready to plot, because metrics were not calculated yet."
 
-        dist_matrix_with_inf, mask_gt = apply_mask_to_ignore(self.distance_matrix, self.mask_gt, self.mask_to_ignore)
-
         is_query = self.acc.storage[self.is_query_key]
         is_gallery = self.acc.storage[self.is_gallery_key]
 
         query_paths = np.array(self.acc.storage[PATHS_KEY])[is_query]
         gallery_paths = np.array(self.acc.storage[PATHS_KEY])[is_gallery]
 
         if all([k in self.acc.storage for k in [X1_KEY, X2_KEY, Y1_KEY, Y2_KEY]]):
@@ -305,60 +309,62 @@
             bboxes = list(zip(fake_coord, fake_coord, fake_coord, fake_coord))
         else:
             raise KeyError(f"Not all the keys collected in storage! {[*self.acc.storage]}")
 
         query_bboxes = torch.tensor(bboxes)[is_query]
         gallery_bboxes = torch.tensor(bboxes)[is_gallery]
 
-        fig = plt.figure(figsize=(30, 30 / (n_instances + N_GT_SHOW_EMBEDDING_METRICS + 1) * len(query_ids)))
+        fig = plt.figure(figsize=(16, 16 / (n_instances + N_GT_SHOW_EMBEDDING_METRICS + 1) * len(query_ids)))
         for j, query_idx in enumerate(query_ids):
-            ids = torch.argsort(dist_matrix_with_inf[query_idx])[:n_instances]
+            ids = torch.argsort(self.distance_matrix[query_idx])[:n_instances]
 
-            n_gt = mask_gt[query_idx].sum()  # type: ignore
+            n_gt = self.mask_gt[query_idx].sum()  # type: ignore
 
             plt.subplot(
                 len(query_ids),
                 n_instances + 1 + N_GT_SHOW_EMBEDDING_METRICS,
                 j * (n_instances + 1 + N_GT_SHOW_EMBEDDING_METRICS) + 1,
             )
 
             img = get_img_with_bbox(query_paths[query_idx], query_bboxes[query_idx], BLUE)
             img = square_pad(img)
+
             if verbose:
                 print("Q  ", query_paths[query_idx])
+
             plt.imshow(img)
             plt.title(f"Query, #gt = {n_gt}")
             plt.axis("off")
 
             for i, idx in enumerate(ids):
-                color = GREEN if mask_gt[query_idx, idx] else RED  # type: ignore
+                color = GREEN if self.mask_gt[query_idx, idx] else RED  # type: ignore
                 if verbose:
                     print("G", i, gallery_paths[idx])
                 plt.subplot(
                     len(query_ids),
                     n_instances + N_GT_SHOW_EMBEDDING_METRICS + 1,
                     j * (n_instances + 1 + N_GT_SHOW_EMBEDDING_METRICS) + i + 2,
                 )
                 img = get_img_with_bbox(gallery_paths[idx], gallery_bboxes[idx], color)
                 img = square_pad(img)
-                plt.title(f"{i} - {round(dist_matrix_with_inf[query_idx, idx].item(), 3)}")
+                plt.title(f"{i} - {round(self.distance_matrix[query_idx, idx].item(), 3)}")
                 plt.imshow(img)
                 plt.axis("off")
 
-            gt_ids = mask_gt[query_idx].nonzero(as_tuple=True)[0][:N_GT_SHOW_EMBEDDING_METRICS]  # type: ignore
+            gt_ids = self.mask_gt[query_idx].nonzero(as_tuple=True)[0][:N_GT_SHOW_EMBEDDING_METRICS]  # type: ignore
 
             for i, gt_idx in enumerate(gt_ids):
                 plt.subplot(
                     len(query_ids),
                     n_instances + N_GT_SHOW_EMBEDDING_METRICS + 1,
                     j * (n_instances + 1 + N_GT_SHOW_EMBEDDING_METRICS) + i + n_instances + 2,
                 )
                 img = get_img_with_bbox(gallery_paths[gt_idx], gallery_bboxes[gt_idx], GRAY)
                 img = square_pad(img)
-                plt.title("GT " + str(round(dist_matrix_with_inf[query_idx, gt_idx].item(), 3)))
+                plt.title("GT " + str(round(self.distance_matrix[query_idx, gt_idx].item(), 3)))
                 plt.imshow(img)
                 plt.axis("off")
 
         fig.tight_layout()
         return fig
```

### Comparing `open-metric-learning-0.3.9/oml/metrics/triplets.py` & `open-metric-learning-0.4.0/oml/metrics/triplets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/miners/cross_batch.py` & `open-metric-learning-0.4.0/oml/miners/cross_batch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/miners/inbatch_all_tri.py` & `open-metric-learning-0.4.0/oml/miners/inbatch_all_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/miners/inbatch_hard_cluster.py` & `open-metric-learning-0.4.0/oml/miners/inbatch_hard_cluster.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/miners/inbatch_hard_tri.py` & `open-metric-learning-0.4.0/oml/miners/inbatch_hard_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/miners/inbatch_nhard_tri.py` & `open-metric-learning-0.4.0/oml/miners/inbatch_nhard_tri.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     def __init__(
         self,
         n_positive: Union[Tuple[int, int], List[int], int] = 1,
         n_negative: Union[Tuple[int, int], List[int], int] = 1,
     ):
         """
         Args:
-            n_positive: keep ``n_positive`` positive examples with large distances. If the value is a range, minimal
+            n_positive: keep ``n_positive`` positive samples with large distances. If the value is a range, minimal
                 value has to be less than the available amount of labels in batches
-            n_negative: keep ``n_negative`` negative examples with small distances
+            n_negative: keep ``n_negative`` negative pipelines with small distances
 
         Note:
             If both parameters are 1, the miner is equivalent to ``HardTripletsMiner``.
             If both parameters are large enough, the miner can be equivalent to ``AllTripletsMiner``
 
         """
```

### Comparing `open-metric-learning-0.3.9/oml/miners/miner_with_bank.py` & `open-metric-learning-0.4.0/oml/miners/miner_with_bank.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/miners/pairs.py` & `open-metric-learning-0.4.0/oml/miners/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/models/pooling.py` & `open-metric-learning-0.4.0/oml/models/pooling.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/models/projection.py` & `open-metric-learning-0.4.0/oml/models/meta/projection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,99 @@
-from functools import partial
 from pathlib import Path
 from typing import List, Optional, Union
 
 import torch
-from torch import nn
 from torchvision.ops import MLP
 
 from oml.const import STORAGE_CKPTS
 from oml.interfaces.models import IExtractor, IFreezable
 from oml.models.utils import remove_prefix_from_state_dict
 from oml.models.vit.vit import ViTExtractor
 from oml.utils.io import download_checkpoint
 
 
-def get_vit_and_mlp(
-    arch_vit: str,
-    normalise_features_vit: bool,
-    mlp_features: List[int],
-    use_multi_scale_vit: bool = False,
-) -> nn.Module:
-    """
-    Function for creation of ViT model and MLP projection.
-
-    """
-    vit = ViTExtractor(
-        weights=None,
-        arch=arch_vit,
-        normalise_features=normalise_features_vit,
-        use_multi_scale=use_multi_scale_vit,
-    )
-    mlp = MLP(vit.feat_dim, mlp_features)
-    return vit, mlp
-
-
 class ExtractorWithMLP(IExtractor, IFreezable):
     """
-    Class-wrapper for extractors which adds additional MLP (may be useful for classification losses).
+    Class-wrapper for extractors which an additional MLP.
 
     """
 
-    constructors = {
-        "vits16_224_mlp_384": partial(
-            get_vit_and_mlp,
-            arch_vit="vits16",
-            normalise_features_vit=False,
-            use_multi_scale_vit=False,
-            mlp_features=[384],
-        )
-    }
-
     pretrained_models = {
-        "vits16_224_mlp_384_inshop": (
-            f"{STORAGE_CKPTS}/inshop/vits16_224_mlp_384_inshop.ckpt",
-            "35244966",
-            "vits16_224_mlp_384_inshop.ckpt",
-        )
+        "vits16_224_mlp_384_inshop": {  # type: ignore
+            "url": f"{STORAGE_CKPTS}/inshop/vits16_224_mlp_384_inshop.ckpt",
+            "hash": "35244966",
+            "fname": "vits16_224_mlp_384_inshop.ckpt",
+            "init_args": {
+                "extractor_creator": lambda: ViTExtractor(None, "vits16", False, use_multi_scale=False),
+                "mlp_features": [384],
+                "train_backbone": True,
+            },
+        }
     }
 
     def __init__(
         self,
         extractor: IExtractor,
         mlp_features: List[int],
         weights: Optional[Union[str, Path]] = None,
-        strict_load: bool = True,
         train_backbone: bool = False,
     ):
         """
         Args:
             extractor: Instance of ``IExtractor`` (e.g. ``ViTExtractor``)
             mlp_features: Sizes of projection layers
             weights: Path to weights file or ``None`` for random initialization
-            strict_load: Whether to use ``self.load_state_dict`` with strict argument
+            train_backbone: set ``False`` if you want to train only MLP head
 
         """
         IExtractor.__init__(self)
-        self.train_backbone = train_backbone
+
         self.extractor = extractor
-        self.projection = MLP(self.extractor.feat_dim, mlp_features)
+        self.mlp_features = mlp_features
+        self.train_backbone = train_backbone
+
+        self.projection = MLP(self.extractor.feat_dim, self.mlp_features)
+
         if weights:
             if weights in self.pretrained_models:
-                url_or_fid, hash_md5, fname = self.pretrained_models[weights]  # type: ignore
-                weights = download_checkpoint(url_or_fid=url_or_fid, hash_md5=hash_md5, fname=fname)
+                pretrained = self.pretrained_models[weights]  # type: ignore
+                weights = download_checkpoint(
+                    url_or_fid=pretrained["url"],  # type: ignore
+                    hash_md5=pretrained["hash"],  # type: ignore
+                    fname=pretrained["fname"],  # type: ignore
+                )
 
             loaded = torch.load(weights, map_location="cpu")
             loaded = loaded.get("state_dict", loaded)
             loaded = remove_prefix_from_state_dict(loaded, trial_key="extractor.")
-            self.load_state_dict(loaded, strict=strict_load)
+            self.load_state_dict(loaded, strict=True)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         with torch.set_grad_enabled(self.train_backbone):
             features = self.extractor(x)
 
         return self.projection(features)
 
     @property
     def feat_dim(self) -> int:
-        return self.projection.out_features
+        return self.mlp_features[-1]
 
     def freeze(self) -> None:
         self.train_backbone = False
 
     def unfreeze(self) -> None:
         self.train_backbone = True
 
+    @classmethod
+    def from_pretrained(cls, weights: str) -> "IExtractor":
+        # The current class takes another model as a constructor's argument, so, they need to be
+        # in the `self.pretrained_models`. The problem is these models will be instantiated even if we simply
+        # import something from the current module. To avoid it we added the logic of wrapping/unwrapping
+        # constructors into lambda functions.
+
+        ini = cls.pretrained_models[weights]["init_args"]
+        ini["extractor"] = ini.pop("extractor_creator")()  # type: ignore
+
+        return super().from_pretrained(weights)
+
 
-__all__ = ["ExtractorWithMLP", "get_vit_and_mlp"]
+__all__ = ["ExtractorWithMLP"]
```

### Comparing `open-metric-learning-0.3.9/oml/models/resnet.py` & `open-metric-learning-0.4.0/oml/models/resnet.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,193 +1,217 @@
 from pathlib import Path
-from typing import Optional, Union
+from typing import Any, Dict, Optional, Union
 
 import numpy as np
+import PIL.Image
 import torch
+from PIL.Image import Image as TPILImage
 from pytorch_grad_cam import GradCAM
 from pytorch_grad_cam.utils.image import show_cam_on_image
 from torch import nn
 from torchvision.models import resnet18, resnet34, resnet50, resnet101, resnet152
 
 from oml.interfaces.models import IExtractor
 from oml.models.pooling import GEM
 from oml.models.utils import remove_prefix_from_state_dict
-from oml.transforms.images.albumentations.transforms import get_normalisation_albu
+from oml.transforms.images.albumentations import get_normalisation_albu
 from oml.utils.io import download_checkpoint
-from oml.utils.misc_torch import normalise
+from oml.utils.misc_torch import get_device, normalise
+
+
+def resnet50_projector() -> nn.Module:
+    model = resnet50(weights=None, num_classes=128)
+    model.fc = nn.Sequential(
+        nn.Linear(model.fc.weight.shape[1], model.fc.weight.shape[1]),
+        nn.ReLU(),
+        model.fc,
+    )
+    return model
 
 
 class ResnetExtractor(IExtractor):
     """
     The base class for the extractors that follow ResNet architecture.
 
     """
 
     constructors = {
         "resnet18": resnet18,
         "resnet34": resnet34,
         "resnet50": resnet50,
+        "resnet50_projector": resnet50_projector,
         "resnet101": resnet101,
         "resnet152": resnet152,
     }
 
     pretrained_models = {
-        "resnet50_moco_v2": (
-            "https://dl.fbaipublicfiles.com/moco/moco_checkpoints/moco_v2_800ep/moco_v2_800ep_pretrain.pth.tar",
-            "a04e12f8",
-            None,
-        )
+        "resnet50_moco_v2": {
+            "url": "https://dl.fbaipublicfiles.com/moco/moco_checkpoints/moco_v2_800ep/moco_v2_800ep_pretrain.pth.tar",
+            "hash": "a04e12f8",
+            "fname": "moco_v2_800ep_pretrain.pth.tar",
+            "init_args": {"arch": "resnet50_projector", "remove_fc": True, "normalise_features": False, "gem_p": 5.0},
+        },
+        "resnet18_imagenet1k_v1": {
+            "init_args": {"arch": "resnet18", "remove_fc": True, "normalise_features": False, "gem_p": None}
+        },
+        "resnet34_imagenet1k_v1": {
+            "init_args": {"arch": "resnet34", "remove_fc": True, "normalise_features": False, "gem_p": None}
+        },
+        "resnet50_imagenet1k_v1": {
+            "init_args": {"arch": "resnet50", "remove_fc": True, "normalise_features": False, "gem_p": None},
+        },
+        "resnet101_imagenet1k_v1": {
+            "init_args": {"arch": "resnet101", "remove_fc": True, "normalise_features": False, "gem_p": None},
+        },
+        "resnet152_imagenet1k_v1": {
+            "init_args": {"arch": "resnet152", "remove_fc": True, "normalise_features": False, "gem_p": None},
+        },
     }
 
     def __init__(
         self,
         weights: Optional[Union[Path, str]],
         arch: str,
-        normalise_features: bool,
         gem_p: Optional[float],
         remove_fc: bool,
-        strict_load: bool = True,
+        normalise_features: bool,
     ):
         """
 
         Args:
             weights: Path to weights or a special key to download pretrained checkpoint, use ``None`` to randomly
-             initialize model's weights or ``default`` to use the checkpoint pretrained on ImageNet.
-             You can check the available pretrained checkpoints in ``self.pretrained_models``.
+             initialize model's weights. You can check the available pretrained checkpoints
+             in ``self.pretrained_models``.
             arch: Different types of ResNet, please, check ``self.constructors``
-            normalise_features: Set ``True`` to normalise output features
             gem_p: Value of power in `Generalized Mean Pooling` that we use as the replacement for the default one
-             (if ``gem_p == 1`` it's just a normal average pooling and if ``gem_p -> inf`` it's max-pooling)
-            remove_fc: Set ``True`` if you want to remove the last fully connected layer
-            strict_load: Set ``True`` if you want the strict load of the weights from the checkpoint
+             (if ``gem_p == 1`` or ``None`` it's just a normal average pooling and if ``gem_p -> inf`` it's max-pooling)
+            remove_fc: Set ``True`` if you want to remove the last fully connected layer. Note, that having this layer
+              is obligatory for calling ``draw_gradcam()`` method
+            normalise_features: Set ``True`` to normalise output features
 
         """
         assert arch in self.constructors.keys()
-
         super(ResnetExtractor, self).__init__()
 
         self.arch = arch
-        self.normalise_features = normalise_features
+        self.gem_p = gem_p
         self.remove_fc = remove_fc
+        self.normalise_features = normalise_features
 
-        factory_fun = self.constructors[self.arch]
-
-        self.model = factory_fun(weights=None)
-
-        if weights == "resnet50_moco_v2":
-            # todo:
-            # in the next iterations we should use head as a separate entity to change fc
-            self.model.fc = nn.Sequential(
-                nn.Linear(self.model.fc.weight.shape[1], self.model.fc.weight.shape[1]),
-                nn.ReLU(),
-                nn.Linear(self.model.fc.weight.shape[1], 128),  # output size in moco v2
-            )
-
-        self.last_conv_channels = self.calc_last_conv_channels()
+        constructor = self.constructors[self.arch]
+        self.model = constructor()
 
         if gem_p is not None:
             self.model.avgpool = GEM(p=gem_p)
 
         if weights is None:
+            if self.remove_fc:
+                self.model.fc = nn.Identity()
             return
 
-        elif isinstance(weights, str) and weights.lower() == "default":
-            state_dict = factory_fun(weights="DEFAULT").state_dict()
-
-        elif isinstance(weights, str) and weights.lower() == "imagenet_v1":
-            state_dict = factory_fun(weights="IMAGENET1K_V1").state_dict()
+        elif weights == "resnet50_moco_v2":
+            pretrained = self.pretrained_models[weights]  # type: ignore
+            moco_path = download_checkpoint(
+                url_or_fid=pretrained["url"],  # type: ignore
+                hash_md5=pretrained["hash"],  # type: ignore
+                fname=pretrained["fname"],  # type: ignore
+            )
+            state_dict = load_moco_weights(moco_path)
 
-        elif weights in self.pretrained_models:
-            url_or_fid, hash_md5, fname = self.pretrained_models[weights]  # type: ignore
-            path_to_ckpt = download_checkpoint(url_or_fid=url_or_fid, hash_md5=hash_md5, fname=fname)
-            state_dict = load_moco_model(path_to_model=Path(path_to_ckpt)).state_dict()
+        elif str(weights).endswith("_imagenet1k_v1"):
+            state_dict = constructor(weights="IMAGENET1K_V1").state_dict()
 
         else:
             state_dict = torch.load(weights, map_location="cpu")
 
         state_dict = state_dict["state_dict"] if "state_dict" in state_dict.keys() else state_dict
-        state_dict = remove_prefix_from_state_dict(state_dict, "layer4.")
-        self.model.load_state_dict(state_dict, strict=strict_load)
+        state_dict = remove_prefix_from_state_dict(state_dict, "layer4.")  # type: ignore
+        self.model.load_state_dict(state_dict, strict=True)
 
-        if remove_fc:
+        if self.remove_fc:
             self.model.fc = nn.Identity()
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         x = self.model(x)
 
         if self.normalise_features:
             x = normalise(x)
 
         return x
 
-    def calc_last_conv_channels(self) -> int:
+    def get_last_conv_channels(self) -> int:
         last_block = self.model.layer4[-1]
         if self.arch in ("resnet18", "resnet34"):
             n_out_channels = last_block.conv2.out_channels
         else:
             # resnet50, resnet101, resnet152
             n_out_channels = last_block.conv3.out_channels
         return n_out_channels
 
     @property
     def feat_dim(self) -> int:
         if isinstance(self.model.fc, torch.nn.Identity):
-            return self.last_conv_channels
+            return self.get_last_conv_channels()
         elif isinstance(self.model.fc, torch.nn.Linear):
             return self.model.fc.out_features
         else:
             # 2-layer mlp case
             return self.model.fc[-1].out_features
 
-    def draw_gradcam(self, image: np.ndarray) -> np.ndarray:
+    def draw_gradcam(self, image: Union[np.ndarray, TPILImage]) -> Union[np.ndarray, TPILImage]:
         """
+        Args:
+            image: An image with pixel values in the range of ``[0..255]``.
+
+        Returns:
+            An image with drawn gradients.
+
         Visualization of the gradients on a particular image using `GradCam`_.
 
         .. _GradCam: https://arxiv.org/abs/1610.02391
 
         """
-        model_device = str(list(self.model.parameters())[0].device)
-        image_tensor = get_normalisation_albu()(image=image)["image"].to(model_device)
-        cam = GradCAM(model=self.model, target_layer=self.model.layer4[-1], use_cuda=model_device != "cpu")
-        gray_image = cam(image_tensor.unsqueeze(0), "gradcam", None)
+        if self.remove_fc:
+            raise ValueError("This method does not work if there is no FC layer in the model.")
+
+        need_to_convert = not isinstance(image, np.ndarray)
+
+        if need_to_convert:
+            image = np.asarray(image)
+
+        device = get_device(self.model)
+        image_tensor = get_normalisation_albu()(image=image)["image"].to(device)
+        cam = GradCAM(model=self.model, target_layers=[self.model.layer4[-1]], use_cuda=device != "cpu")
+        gray_image = cam(image_tensor.unsqueeze(0), None)[0]
         img_with_grads = show_cam_on_image(image / 255, gray_image)
+
+        if need_to_convert:
+            img_with_grads = PIL.Image.fromarray(img_with_grads)
+
         return img_with_grads
 
 
-def load_moco_model(path_to_model: Path) -> nn.Module:
+def load_moco_weights(path_to_model: Union[str, Path]) -> Dict[str, Any]:
     """
     Args:
         path_to_model: Path to model trained using original
            code from MoCo repository:
            https://github.com/facebookresearch/moco
 
     Returns:
-        Model
+        State dict without weights of student
 
     """
     checkpoint = torch.load(path_to_model, map_location="cpu")
 
     state_dict = checkpoint["state_dict"]
-    for k in list(state_dict.keys()):
+    for key in list(state_dict.keys()):
         # retain only encoder_q up to before the embedding layer
-        if k.startswith("module.encoder_q"):
-            state_dict[k[len("module.encoder_q.") :]] = state_dict[k]
-        del state_dict[k]
-
-    model = resnet50(num_classes=128)  # output size in moco v2
-
-    if "fc.2.weight" in state_dict.keys():
-        print("MOCO V2 architecture was detected!")
-        model.fc = nn.Sequential(
-            nn.Linear(model.fc.weight.shape[1], model.fc.weight.shape[1]),
-            nn.ReLU(),
-            model.fc,
-        )
-    else:
-        print("MOCO V1 architecture will be used")
-
-    model.load_state_dict(state_dict)
+        if key.startswith("module.encoder_q"):
+            new_key = key[len("module.encoder_q.") :]
+            state_dict[new_key] = state_dict[key]
+        del state_dict[key]
 
-    return model
+    return state_dict
 
 
-__all__ = ["ResnetExtractor", "load_moco_model"]
+__all__ = ["ResnetExtractor"]
```

### Comparing `open-metric-learning-0.3.9/oml/models/siamese.py` & `open-metric-learning-0.4.0/oml/models/meta/siamese.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,41 +45,46 @@
 
         """
         x1 = self.proj(x1)
         x2 = self.proj(x2)
         y = elementwise_dist(x1, x2, p=2)
         return y
 
+    def predict(self, x1: Tensor, x2: Tensor) -> Tensor:
+        return self.forward(x1=x1, x2=x2)
+
 
 class ConcatSiamese(IPairwiseModel, IFreezable):
     """
     This model concatenates two inputs and passes them through
     a given backbone and applyies a head after that.
 
     """
 
     pretrained_models: Dict[str, Any] = {}
 
     def __init__(
         self,
         extractor: IExtractor,
         mlp_hidden_dims: List[int],
+        use_tta: bool = False,
         weights: Optional[Union[str, Path]] = None,
-        strict_load: bool = True,
     ) -> None:
         """
         Args:
             extractor: Instance of ``IExtractor`` (e.g. ``ViTExtractor``)
             mlp_hidden_dims: Hidden dimensions of the head
+            use_tta: Set ``True`` if you want to average the results obtained by two different orders of concatenating
+             input images. Affects only ``self.predict()`` method.
             weights: Path to weights file or ``None`` for random initialization
-            strict_load: Whether to use ``self.load_state_dict`` with strict argument
 
         """
         super(ConcatSiamese, self).__init__()
         self.extractor = extractor
+        self.use_tta = use_tta
 
         self.head = MLP(
             in_channels=self.extractor.feat_dim,
             hidden_channels=[*mlp_hidden_dims, 1],
             activation_layer=Sigmoid,
             dropout=0.5,
             inplace=None,
@@ -97,27 +102,38 @@
             if weights in self.pretrained_models:
                 url_or_fid, hash_md5, fname = self.pretrained_models[weights]  # type: ignore
                 weights = download_checkpoint(url_or_fid=url_or_fid, hash_md5=hash_md5, fname=fname)
 
             loaded = torch.load(weights, map_location="cpu")
             loaded = loaded.get("state_dict", loaded)
             loaded = remove_prefix_from_state_dict(loaded, trial_key="extractor.")
-            self.load_state_dict(loaded, strict=strict_load)
+            self.load_state_dict(loaded, strict=True)
 
     def forward(self, x1: Tensor, x2: Tensor) -> Tensor:
         x = torch.concat([x1, x2], dim=2)
 
         with torch.set_grad_enabled(self.train_backbone):
             x = self.extractor(x)
 
         x = self.head(x)
         x = x.view(len(x))
 
         return x
 
+    def predict(self, x1: Tensor, x2: Tensor) -> Tensor:
+        x = self.forward(x1=x1, x2=x2)
+        x = torch.sigmoid(x)
+
+        if self.use_tta:
+            y = self.forward(x1=x2, x2=x1)
+            y = torch.sigmoid(y)
+            return (x + y) / 2
+        else:
+            return x
+
     def freeze(self) -> None:
         self.train_backbone = False
 
     def unfreeze(self) -> None:
         self.train_backbone = True
 
 
@@ -148,9 +164,12 @@
             Distance between inputs.
 
         """
         x1 = self.extractor(x1)
         x2 = self.extractor(x2)
         return elementwise_dist(x1, x2, p=2)
 
+    def predict(self, x1: Tensor, x2: Tensor) -> Tensor:
+        return self.forward(x1=x1, x2=x2)
+
 
 __all__ = ["LinearTrivialDistanceSiamese", "ConcatSiamese", "TrivialDistanceSiamese"]
```

### Comparing `open-metric-learning-0.3.9/oml/models/utils.py` & `open-metric-learning-0.4.0/oml/models/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/models/vit/hubconf.py` & `open-metric-learning-0.4.0/oml/models/vit/hubconf.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/models/vit/vision_transformer.py` & `open-metric-learning-0.4.0/oml/models/vit/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/models/vit/vision_transformer_clip.py` & `open-metric-learning-0.4.0/oml/models/vit/vision_transformer_clip.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/registry/__init__.py` & `open-metric-learning-0.4.0/oml/registry/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 
 from oml.registry.losses import LOSSES_REGISTRY
 from oml.registry.miners import MINERS_REGISTRY
-from oml.registry.models import EXTRACTORS_REGISTRY
+from oml.registry.models import EXTRACTORS_REGISTRY, PAIRWISE_MODELS_REGISTRY
 from oml.registry.optimizers import OPTIMIZERS_REGISTRY
 from oml.registry.samplers import SAMPLERS_REGISTRY
 from oml.registry.schedulers import SCHEDULERS_REGISTRY
 from oml.registry.transforms import TRANSFORMS_REGISTRY
 
 
 def show_registry() -> None:
```

### Comparing `open-metric-learning-0.3.9/oml/registry/losses.py` & `open-metric-learning-0.4.0/oml/registry/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/registry/miners.py` & `open-metric-learning-0.4.0/oml/registry/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/registry/models.py` & `open-metric-learning-0.4.0/oml/registry/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict
 from warnings import warn
 
 from oml.interfaces.models import IExtractor, IPairwiseModel
-from oml.models.projection import ExtractorWithMLP
-from oml.models.resnet import ResnetExtractor
-from oml.models.siamese import (
+from oml.models.meta.projection import ExtractorWithMLP
+from oml.models.meta.siamese import (
     ConcatSiamese,
     LinearTrivialDistanceSiamese,
     TrivialDistanceSiamese,
 )
+from oml.models.resnet import ResnetExtractor
 from oml.models.vit.clip import ViTCLIPExtractor
 from oml.models.vit.vit import ViTExtractor
 from oml.utils.misc import TCfg, dictconfig_to_dict
 
 EXTRACTORS_REGISTRY = {
     "resnet": ResnetExtractor,
     "vit": ViTExtractor,
```

### Comparing `open-metric-learning-0.3.9/oml/registry/optimizers.py` & `open-metric-learning-0.4.0/oml/registry/optimizers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/registry/postprocessors.py` & `open-metric-learning-0.4.0/oml/registry/postprocessors.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/registry/samplers.py` & `open-metric-learning-0.4.0/oml/registry/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/registry/schedulers.py` & `open-metric-learning-0.4.0/oml/registry/schedulers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/retrieval/postprocessors/pairwise.py` & `open-metric-learning-0.4.0/oml/retrieval/postprocessors/pairwise.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,16 +174,16 @@
 
 class PairwiseImagesPostprocessor(PairwisePostprocessor):
     def __init__(
         self,
         top_n: int,
         pairwise_model: IPairwiseModel,
         transforms: TTransforms,
-        num_workers: int,
-        batch_size: int,
+        num_workers: int = 0,
+        batch_size: int = 128,
         verbose: bool = True,
         use_fp16: bool = False,
         is_query_key: str = IS_QUERY_KEY,
         is_gallery_key: str = IS_GALLERY_KEY,
         paths_key: str = PATHS_KEY,
     ):
         """
```

### Comparing `open-metric-learning-0.3.9/oml/samplers/balance.py` & `open-metric-learning-0.4.0/oml/samplers/balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/samplers/category_balance.py` & `open-metric-learning-0.4.0/oml/samplers/category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/samplers/distinct_category_balance.py` & `open-metric-learning-0.4.0/oml/samplers/distinct_category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/transforms/images/albumentations/transforms.py` & `open-metric-learning-0.4.0/oml/transforms/images/albumentations.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/transforms/images/torchvision/transforms.py` & `open-metric-learning-0.4.0/oml/transforms/images/torchvision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/utils/dataframe_format.py` & `open-metric-learning-0.4.0/oml/utils/dataframe_format.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/utils/download_mock_dataset.py` & `open-metric-learning-0.4.0/oml/utils/download_mock_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,17 @@
         raise Exception("Downloaded mock dataset is invalid.")
 
     df = pd.read_csv(Path(dataset_root) / "df.csv")
 
     df_train = df[df["split"] == "train"].reset_index(drop=True)
     df_val = df[df["split"] == "validation"].reset_index(drop=True)
 
+    df_val["is_query"] = df_val["is_query"].astype(bool)
+    df_val["is_gallery"] = df_val["is_gallery"].astype(bool)
+
     return df_train, df_val
 
 
 def main() -> None:
     args = get_argparser().parse_args()
     download_mock_dataset(dataset_root=args.dataset_root)
```

### Comparing `open-metric-learning-0.3.9/oml/utils/images/images.py` & `open-metric-learning-0.4.0/oml/utils/images/images.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,15 +69,17 @@
     if not any(torch.isnan(bbox)):
         x1, y1, x2, y2 = list(map(int, bbox))
     elif all(torch.isnan(bbox)):
         x1, y1, x2, y2 = 0, 0, im_ret.shape[1], im_ret.shape[0]
     else:
         raise ValueError("BBox can only consist of all NaNs or all numbers.")
 
-    im_ret = cv2.rectangle(im_ret, (x1, y1), (x2, y2), thickness=15, color=color)
+    im_avg_sz = (im_ret.shape[0] + im_ret.shape[1]) / 2
+    thickness = max(3, int(0.05 * im_avg_sz))
+    im_ret = cv2.rectangle(im_ret, (x1, y1), (x2, y2), thickness=thickness, color=color)
 
     return im_ret
 
 
 def get_img_with_bbox(im_path: str, bbox: torch.Tensor, color: TColor) -> np.ndarray:
     """
     Reads the image by its name and draws bbox on it.
```

### Comparing `open-metric-learning-0.3.9/oml/utils/images/images_resize.py` & `open-metric-learning-0.4.0/oml/utils/images/images_resize.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/utils/io.py` & `open-metric-learning-0.4.0/oml/utils/io.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/utils/misc.py` & `open-metric-learning-0.4.0/oml/utils/misc.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/utils/misc_torch.py` & `open-metric-learning-0.4.0/oml/utils/misc_torch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/oml/utils/remote_storage.py` & `open-metric-learning-0.4.0/oml/utils/remote_storage.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.3.9/open_metric_learning.egg-info/SOURCES.txt` & `open-metric-learning-0.4.0/open_metric_learning.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 oml/configs/__init__.py
 oml/configs/criterion/arcface.yaml
 oml/configs/criterion/mlp_arcface.yaml
 oml/configs/criterion/surrogate_precision.yaml
 oml/configs/criterion/triplet.yaml
 oml/configs/criterion/triplet_plain.yaml
 oml/configs/criterion/triplet_with_miner.yaml
+oml/configs/extractor/extractor_with_mlp.yaml
+oml/configs/extractor/resnet.yaml
+oml/configs/extractor/vit.yaml
+oml/configs/extractor/vit_clip.yaml
 oml/configs/miner/all_triplets.yaml
 oml/configs/miner/hard_cluster.yaml
 oml/configs/miner/hard_triplets.yaml
 oml/configs/miner/miner_with_bank.yaml
 oml/configs/miner/n_hard_triplets.yaml
 oml/configs/miner/triplets_with_memory.yaml
-oml/configs/model/extractor_with_mlp.yaml
-oml/configs/model/resnet.yaml
-oml/configs/model/vit.yaml
-oml/configs/model/vit_clip.yaml
 oml/configs/optimizer/adadelta.yaml
 oml/configs/optimizer/adagrad.yaml
 oml/configs/optimizer/adam.yaml
 oml/configs/optimizer/adamax.yaml
 oml/configs/optimizer/adamw.yaml
 oml/configs/optimizer/asgd.yaml
 oml/configs/optimizer/lbfgs.yaml
@@ -82,23 +82,23 @@
 oml/interfaces/miners.py
 oml/interfaces/models.py
 oml/interfaces/retrieval.py
 oml/interfaces/samplers.py
 oml/lightning/__init__.py
 oml/lightning/callbacks/__init__.py
 oml/lightning/callbacks/metric.py
-oml/lightning/entrypoints/__init__.py
-oml/lightning/entrypoints/parser.py
-oml/lightning/entrypoints/train.py
-oml/lightning/entrypoints/train_postprocessor.py
-oml/lightning/entrypoints/validate.py
 oml/lightning/modules/__init__.py
 oml/lightning/modules/ddp.py
+oml/lightning/modules/extractor.py
 oml/lightning/modules/pairwise_postprocessing.py
-oml/lightning/modules/retrieval.py
+oml/lightning/pipelines/__init__.py
+oml/lightning/pipelines/parser.py
+oml/lightning/pipelines/train.py
+oml/lightning/pipelines/train_postprocessor.py
+oml/lightning/pipelines/validate.py
 oml/losses/__init__.py
 oml/losses/arcface.py
 oml/losses/surrogate_precision.py
 oml/losses/triplet.py
 oml/metrics/__init__.py
 oml/metrics/accumulation.py
 oml/metrics/embeddings.py
@@ -109,18 +109,19 @@
 oml/miners/inbatch_hard_cluster.py
 oml/miners/inbatch_hard_tri.py
 oml/miners/inbatch_nhard_tri.py
 oml/miners/miner_with_bank.py
 oml/miners/pairs.py
 oml/models/__init__.py
 oml/models/pooling.py
-oml/models/projection.py
 oml/models/resnet.py
-oml/models/siamese.py
 oml/models/utils.py
+oml/models/meta/__init__.py
+oml/models/meta/projection.py
+oml/models/meta/siamese.py
 oml/models/vit/__init__.py
 oml/models/vit/clip.py
 oml/models/vit/hubconf.py
 oml/models/vit/vision_transformer.py
 oml/models/vit/vision_transformer_clip.py
 oml/models/vit/vit.py
 oml/registry/__init__.py
@@ -137,27 +138,27 @@
 oml/retrieval/postprocessors/pairwise.py
 oml/samplers/__init__.py
 oml/samplers/balance.py
 oml/samplers/category_balance.py
 oml/samplers/distinct_category_balance.py
 oml/transforms/__init__.py
 oml/transforms/images/__init__.py
+oml/transforms/images/albumentations.py
+oml/transforms/images/torchvision.py
 oml/transforms/images/utils.py
-oml/transforms/images/albumentations/__init__.py
-oml/transforms/images/albumentations/transforms.py
-oml/transforms/images/torchvision/__init__.py
-oml/transforms/images/torchvision/transforms.py
 oml/utils/__init__.py
 oml/utils/dataframe_format.py
 oml/utils/download_mock_dataset.py
 oml/utils/io.py
 oml/utils/misc.py
 oml/utils/misc_torch.py
 oml/utils/remote_storage.py
 oml/utils/images/__init__.py
 oml/utils/images/images.py
 oml/utils/images/images_resize.py
 open_metric_learning.egg-info/PKG-INFO
 open_metric_learning.egg-info/SOURCES.txt
 open_metric_learning.egg-info/dependency_links.txt
 open_metric_learning.egg-info/requires.txt
-open_metric_learning.egg-info/top_level.txt
+open_metric_learning.egg-info/top_level.txt
+tests/test_build_readme.py
+tests/test_imports.py
```

### Comparing `open-metric-learning-0.3.9/setup.py` & `open-metric-learning-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     with io.open(version_file, encoding="utf-8") as f:
         return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', f.read(), re.M).group(1)
 
 
 setup(
     # technical things
     version=load_version(),
-    packages=find_packages(exclude=["ci", "docs", "examples", "tests*"]),
+    packages=find_packages(exclude=["ci", "docs", "pipelines", "tests*"]),
     python_requires=">=3.7,<4.0",
     install_requires=load_requirements("ci/requirements.txt"),
     include_package_data=True,
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     # general information
     name="open-metric-learning",
```


# Comparing `tmp/causica-0.2.0.tar.gz` & `tmp/causica-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causica-0.2.0.tar", max compression
+gzip compressed data, was "causica-0.3.0.tar", max compression
```

## Comparing `causica-0.2.0.tar` & `causica-0.3.0.tar`

### file list

```diff
@@ -1,62 +1,70 @@
--rw-r--r--   0        0        0     1141 2023-03-29 12:50:34.395911 causica-0.2.0/LICENSE
--rw-r--r--   0        0        0     7149 2023-03-29 13:47:25.234110 causica-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-03-29 12:50:34.395911 causica-0.2.0/examples/__init__.py
--rw-r--r--   0        0        0    76973 2023-03-29 13:47:25.234110 causica-0.2.0/examples/csuite_example.ipynb
--rw-r--r--   0        0        0      682 2023-03-29 13:47:25.244110 causica-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-29 12:50:34.405911 causica-0.2.0/src/causica/__init__.py
--rw-r--r--   0        0        0      152 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/config/lightning/default_data.yaml
--rw-r--r--   0        0        0     1226 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/config/lightning/default_gaussian.yaml
--rw-r--r--   0        0        0     1224 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/config/lightning/default_spline.yaml
--rw-r--r--   0        0        0        0 2023-03-29 12:50:34.405911 causica-0.2.0/src/causica/datasets/__init__.py
--rw-r--r--   0        0        0    12141 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/datasets/causica_dataset_format.py
--rw-r--r--   0        0        0     2665 2023-03-29 12:50:34.405911 causica-0.2.0/src/causica/datasets/interventional_data.py
--rw-r--r--   0        0        0     1230 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/datasets/loaded_expert_graph_container.py
--rw-r--r--   0        0        0     2454 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/datasets/standardizer.py
--rw-r--r--   0        0        0     1965 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/datasets/tensordict_utils.py
--rw-r--r--   0        0        0      306 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/datasets/variable_types.py
--rw-r--r--   0        0        0      860 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/__init__.py
--rw-r--r--   0        0        0      526 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/adjacency/__init__.py
--rw-r--r--   0        0        0     3600 2023-03-29 12:50:34.405911 causica-0.2.0/src/causica/distributions/adjacency/adjacency_distributions.py
--rw-r--r--   0        0        0     8590 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/adjacency/constrained_adjacency_distributions.py
--rw-r--r--   0        0        0     7979 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/adjacency/enco.py
--rw-r--r--   0        0        0     3958 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/adjacency/gibbs_dag_prior.py
--rw-r--r--   0        0        0     4784 2023-03-29 12:50:34.405911 causica-0.2.0/src/causica/distributions/adjacency/three_way.py
--rw-r--r--   0        0        0      773 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/distribution_module.py
--rw-r--r--   0        0        0      649 2023-03-29 12:50:34.415911 causica-0.2.0/src/causica/distributions/gumbel_binary.py
--rw-r--r--   0        0        0      595 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/noise/__init__.py
--rw-r--r--   0        0        0     3356 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/noise/bernoulli.py
--rw-r--r--   0        0        0     3222 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/noise/categorical.py
--rw-r--r--   0        0        0     7589 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/noise/joint.py
--rw-r--r--   0        0        0     3415 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/noise/noise.py
--rw-r--r--   0        0        0      112 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/noise/spline/__init__.py
--rw-r--r--   0        0        0     9952 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/noise/spline/rational_quadratic_transform.py
--rw-r--r--   0        0        0     8037 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/noise/spline/spline.py
--rw-r--r--   0        0        0     1736 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/noise/univariate_normal.py
--rw-r--r--   0        0        0     4089 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/sem_distribution.py
--rw-r--r--   0        0        0     3087 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/distributions/transforms.py
--rw-r--r--   0        0        0      522 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/fsspec_helpers.py
--rw-r--r--   0        0        0      310 2023-03-29 12:50:34.425911 causica-0.2.0/src/causica/functional_relationships/__init__.py
--rw-r--r--   0        0        0     4600 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/functional_relationships/do_functional_relationships.py
--rw-r--r--   0        0        0     2349 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/functional_relationships/functional_relationships.py
--rw-r--r--   0        0        0     9454 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/functional_relationships/icgnn.py
--rw-r--r--   0        0        0     2974 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/functional_relationships/linear_functional_relationships.py
--rw-r--r--   0        0        0        0 2023-03-29 12:50:34.425911 causica-0.2.0/src/causica/graph/__init__.py
--rw-r--r--   0        0        0      375 2023-03-29 12:50:34.425911 causica-0.2.0/src/causica/graph/dag_constraint.py
--rw-r--r--   0        0        0     2737 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/graph/evaluation_metrics.py
--rw-r--r--   0        0        0        0 2023-03-29 12:50:34.425911 causica-0.2.0/src/causica/lightning/__init__.py
--rw-r--r--   0        0        0     3065 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/lightning/callbacks.py
--rw-r--r--   0        0        0      718 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/lightning/cli.py
--rw-r--r--   0        0        0     6555 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/lightning/data_modules.py
--rw-r--r--   0        0        0    12447 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/lightning/deci_module.py
--rw-r--r--   0        0        0      767 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/lightning/main.py
--rw-r--r--   0        0        0     2106 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/lightning/variable_spec_module.py
--rw-r--r--   0        0        0     1289 2023-03-29 12:50:34.425911 causica-0.2.0/src/causica/mlflow_helpers.py
--rw-r--r--   0        0        0        0 2023-03-29 12:50:34.425911 causica-0.2.0/src/causica/sem/__init__.py
--rw-r--r--   0        0        0     3736 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/sem/distribution_parameters_sem.py
--rw-r--r--   0        0        0     6501 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/sem/structural_equation_model.py
--rw-r--r--   0        0        0        0 2023-03-29 12:50:34.435911 causica-0.2.0/src/causica/training/__init__.py
--rw-r--r--   0        0        0    11227 2023-03-29 12:50:34.435911 causica-0.2.0/src/causica/training/auglag.py
--rw-r--r--   0        0        0     9416 2023-03-29 13:47:25.244110 causica-0.2.0/src/causica/training/evaluation.py
--rw-r--r--   0        0        0     1169 2023-03-29 12:50:34.435911 causica-0.2.0/src/causica/training/training_callbacks.py
--rw-r--r--   0        0        0     1725 2023-03-29 12:50:34.435911 causica-0.2.0/src/causica/triangular_transformations.py
--rw-r--r--   0        0        0     7889 1970-01-01 00:00:00.000000 causica-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-04-27 12:56:49.952801 causica-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7092 2023-04-27 13:52:23.840044 causica-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 12:56:49.952801 causica-0.3.0/examples/__init__.py
+-rw-r--r--   0        0        0    76973 2023-04-27 12:56:49.952801 causica-0.3.0/examples/csuite_example.ipynb
+-rw-r--r--   0        0        0   530997 2023-04-27 13:52:23.850044 causica-0.3.0/examples/multi_investment_sales_attribution.ipynb
+-rw-r--r--   0        0        0      760 2023-04-27 13:52:23.860045 causica-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 12:56:49.952801 causica-0.3.0/src/causica/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/config/lightning/default_data.yaml
+-rw-r--r--   0        0        0     1227 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/config/lightning/default_gaussian.yaml
+-rw-r--r--   0        0        0     1225 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/config/lightning/default_spline.yaml
+-rw-r--r--   0        0        0        0 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/datasets/__init__.py
+-rw-r--r--   0        0        0    12768 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/datasets/causica_dataset_format.py
+-rw-r--r--   0        0        0     2642 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/datasets/interventional_data.py
+-rw-r--r--   0        0        0     1230 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/datasets/loaded_expert_graph_container.py
+-rw-r--r--   0        0        0     2454 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/datasets/standardizer.py
+-rw-r--r--   0        0        0     1959 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/datasets/tensordict_utils.py
+-rw-r--r--   0        0        0      307 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/datasets/variable_types.py
+-rw-r--r--   0        0        0      891 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/__init__.py
+-rw-r--r--   0        0        0      613 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/adjacency/__init__.py
+-rw-r--r--   0        0        0     3600 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/adjacency/adjacency_distributions.py
+-rw-r--r--   0        0        0     8583 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/adjacency/constrained_adjacency_distributions.py
+-rw-r--r--   0        0        0     3374 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/adjacency/directed_acyclic.py
+-rw-r--r--   0        0        0     7979 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/adjacency/enco.py
+-rw-r--r--   0        0        0     3952 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/adjacency/gibbs_dag_prior.py
+-rw-r--r--   0        0        0     4784 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/adjacency/three_way.py
+-rw-r--r--   0        0        0      773 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/distribution_module.py
+-rw-r--r--   0        0        0      649 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/gumbel_binary.py
+-rw-r--r--   0        0        0      595 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/noise/__init__.py
+-rw-r--r--   0        0        0     3356 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/noise/bernoulli.py
+-rw-r--r--   0        0        0     3222 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/noise/categorical.py
+-rw-r--r--   0        0        0     7593 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/noise/joint.py
+-rw-r--r--   0        0        0     3389 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/noise/noise.py
+-rw-r--r--   0        0        0      112 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/noise/spline/__init__.py
+-rw-r--r--   0        0        0     6539 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py
+-rw-r--r--   0        0        0     4340 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/noise/spline/rational_quadratic_transform.py
+-rw-r--r--   0        0        0     8024 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/noise/spline/spline.py
+-rw-r--r--   0        0        0     1736 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/noise/univariate_normal.py
+-rw-r--r--   0        0        0     4058 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/sem_distribution.py
+-rw-r--r--   0        0        0     3063 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/transforms.py
+-rw-r--r--   0        0        0      516 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/fsspec_helpers.py
+-rw-r--r--   0        0        0      310 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/functional_relationships/__init__.py
+-rw-r--r--   0        0        0     4574 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/functional_relationships/do_functional_relationships.py
+-rw-r--r--   0        0        0     2330 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/functional_relationships/functional_relationships.py
+-rw-r--r--   0        0        0     9442 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/functional_relationships/icgnn.py
+-rw-r--r--   0        0        0     2949 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/functional_relationships/linear_functional_relationships.py
+-rw-r--r--   0        0        0        0 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/graph/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/graph/dag_constraint.py
+-rw-r--r--   0        0        0     2711 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/graph/evaluation_metrics.py
+-rw-r--r--   0        0        0        0 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/lightning/__init__.py
+-rw-r--r--   0        0        0     3437 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/callbacks.py
+-rw-r--r--   0        0        0      718 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/lightning/cli.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/data_modules/__init__.py
+-rw-r--r--   0        0        0     3052 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/data_modules/basic_data_module.py
+-rw-r--r--   0        0        0     1143 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/data_modules/deci_data_module.py
+-rw-r--r--   0        0        0     7778 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/data_modules/variable_spec_data.py
+-rw-r--r--   0        0        0      776 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/main.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/modules/__init__.py
+-rw-r--r--   0        0        0    12424 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/modules/deci_module.py
+-rw-r--r--   0        0        0     2096 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/modules/variable_spec_module.py
+-rw-r--r--   0        0        0     1289 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/mlflow_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/sem/__init__.py
+-rw-r--r--   0        0        0     3711 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/sem/distribution_parameters_sem.py
+-rw-r--r--   0        0        0     6175 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/sem/structural_equation_model.py
+-rw-r--r--   0        0        0        0 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/training/__init__.py
+-rw-r--r--   0        0        0    10903 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/training/auglag.py
+-rw-r--r--   0        0        0     5286 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/training/evaluation.py
+-rw-r--r--   0        0        0     8958 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/training/per_variable_metrics.py
+-rw-r--r--   0        0        0     1169 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/training/training_callbacks.py
+-rw-r--r--   0        0        0     1725 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/triangular_transformations.py
+-rw-r--r--   0        0        0     7913 1970-01-01 00:00:00.000000 causica-0.3.0/PKG-INFO
```

### Comparing `causica-0.2.0/LICENSE` & `causica-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/README.md` & `causica-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 
 **Simulation-based Causal Inference**
 
 DECI estimates causal quantities (ATE) by applying the relevant interventions to its learnt causal graph (i.e. mutilating incoming edges to intervened variables) and then sampling from the generative model. This process involves first sampling a vector of exogenous noise from the learnt noise distribution and then forward simulating the SEM until an observation vector is obtained. ATE can be computed via estimating an expectation over the effect variable of interest using MonteCarlo samples of the intervened distribution of observations. 
 
 ## How to run
 
-See the notebook `examples/csuite_example.ipynb`, for how to train a DECI model and check the causal discovery.
+The best place to start is the `examples/multi_investment_sales_attribution.ipynb` notebook. This explains how to fit a model using PyTorch Lightning and test ATE and ITE results.
+
+For a more detailed introduction to the components and how they fit together, see the notebook `examples/csuite_example.ipynb`, for how to train a DECI model and check the causal discovery.
 
 This will download the data from the CSuite Azure blob storage and train DECI on it. See [here](https://github.com/microsoft/csuite) for more info about CSuite datasets. The notebook will work on any of the available CSuite datasets.
 
 
 **Specifying a noise model**
 
 The noise exogenous model can be modified by changing the `noise_dist` field within `TrainingConfig`, either Gaussian or Spline are allowed.
@@ -70,18 +72,14 @@
 
 [2], **(DECI)** Tomas Geffner, Javier Antoran, Adam Foster, Wenbo Gong, Chao Ma, Emre Kiciman, Amit Sharma, Angus Lamb, Martin Kukla, Nick Pawlowski, Miltiadis Allamanis, Cheng Zhang. Deep End-to-end Causal Inference. [Arxiv preprint](https://arxiv.org/abs/2202.02195) (2022)
 
 [3], **(DDECI)** Matthew Ashman, Chao Ma, Agrin Hilmkil, Joel Jennings, Cheng Zhang. Causal Reasoning in the Presence of Latent Confounders via Neural ADMG Learning. [ICLR](https://openreview.net/forum?id=dcN0CaXQhT) (2023)
 
 [4], **(Rhino)** Wenbo Gong, Joel Jennings, Cheng Zhang, Nick Pawlowski. Rhino: Deep Causal Temporal Relationship Learning with History-dependent Noise. [ICLR](https://openreview.net/forum?id=i_1rbq8yFWC) (2023)
 
-Other references:
-- Louizos, Christos, et al. "Causal effect inference with deep latent-variable models." Advances in neural information processing systems 30 (2017).
-- Hill, Jennifer L. "Bayesian nonparametric modeling for causal inference." Journal of Computational and Graphical Statistics 20.1 (2011): 217-240.
-
 
 # Development
 
 ## Poetry
 
 We use Poetry to manage the project dependencies, they're specified in the [pyproject.toml](pyproject.toml). To install poetry run:
```

### Comparing `causica-0.2.0/examples/csuite_example.ipynb` & `causica-0.3.0/examples/csuite_example.ipynb`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/pyproject.toml` & `causica-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [tool.poetry]
 name = "causica"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "causica", from = "src" },
     { include = "examples", from = "." },
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "~3.9"
+python = "~3.10"
 azureml-mlflow = "^1.46.0"
 mlflow = "^2.0.0"
 numpy = "^1.22.4"
 pandas = "^1.4.2"
 tensorboard = "^2.9.0"
-pytorch-lightning = {version = "^1.7.7", extras= ["extra"]}
+pytorch-lightning = {version = "^2.0.0", extras= ["extra"]}
+jsonargparse = "<=4.20.0"
 dataclasses-json = "^0.5.7"
 types-PyYAML = "^6.0.12.2"
 tensordict = "^0.1.0"
 torch = "^2.0.0"
+numba = "^0.56.0"  # needed to make the build work
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `causica-0.2.0/src/causica/config/lightning/default_gaussian.yaml` & `causica-0.3.0/src/causica/config/lightning/default_gaussian.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
           noise_dist: 5e-3
         aggregation_period: 20
         lr_factor: 0.1
         penalty_progress_rate: 0.65
         safety_rho: 1e13
         safety_alpha: 1e13
         max_lr_down: 3
-        inner_early_stopping_patience: 500
+        inner_early_stopping_patience: 1500
         max_outer_steps: 100
         patience_penalty_reached: 5
         patience_max_rho: 3
         penalty_tolerance: 1e-5
         max_inner_steps: 6000
 trainer:
   max_epochs: 2000
```

### Comparing `causica-0.2.0/src/causica/config/lightning/default_spline.yaml` & `causica-0.3.0/src/causica/config/lightning/default_spline.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
           noise_dist: 1e-4
         aggregation_period: 20
         lr_factor: 0.1
         penalty_progress_rate: 0.65
         safety_rho: 1e13
         safety_alpha: 1e13
         max_lr_down: 3
-        inner_early_stopping_patience: 500
+        inner_early_stopping_patience: 1500
         max_outer_steps: 100
         patience_penalty_reached: 5
         patience_max_rho: 3
         penalty_tolerance: 1e-5
         max_inner_steps: 6000
 trainer:
   max_epochs: 2000
```

### Comparing `causica-0.2.0/src/causica/datasets/causica_dataset_format.py` & `causica-0.3.0/src/causica/datasets/causica_dataset_format.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 """
 A module to load data from the standard directory structure (i.e. the one followed by csuite)
 """
 import json
+import logging
 import os
 from enum import Enum
 from functools import partial
-from typing import Any, Counter, Dict, List, Optional, Set, Tuple
+from typing import Any, Counter, Optional
 
 import fsspec
 import numpy as np
 import torch
 from tensordict import TensorDict
 
 from causica.datasets.interventional_data import CounterfactualData, InterventionData
 from causica.datasets.tensordict_utils import convert_one_hot
 from causica.datasets.variable_types import DTYPE_MAP, VariableTypeEnum
 
 CSUITE_DATASETS_PATH = "https://azuastoragepublic.blob.core.windows.net/datasets"
 
 
-InterventionWithEffects = Tuple[InterventionData, InterventionData, Set[str]]
-CounterfactualWithEffects = Tuple[CounterfactualData, CounterfactualData, Set[str]]
+InterventionWithEffects = tuple[InterventionData, InterventionData, set[str]]
+CounterfactualWithEffects = tuple[CounterfactualData, Optional[CounterfactualData], set[str]]
+
+logger = logging.getLogger(__name__)
 
 
 class DataEnum(Enum):
     TRAIN = "train.csv"
     TEST = "test.csv"
     INTERVENTIONS = "interventions.json"
     COUNTERFACTUALS = "counterfactuals.json"
     TRUE_ADJACENCY = "adj_matrix.csv"
     VARIABLES_JSON = "variables.json"
 
 
-def convert_variable_types_to_enum(variable_metadata: Dict[str, Any]):
+def convert_variable_types_to_enum(variable_metadata: dict[str, Any]):
     # Convert the types to the enum
     for variable in variable_metadata["variables"]:
         variable["type"] = VariableTypeEnum(variable["type"])
 
     return variable_metadata
 
 
+def convert_enum_to_variable_types(variable_metadata: dict[str, Any]):
+    # Convert enum to types
+    for variable in variable_metadata["variables"]:
+        variable["type"] = VariableTypeEnum(variable["type"]).value
+
+    return variable_metadata
+
+
 def load_data(
     root_path: str,
     data_enum: DataEnum,
-    variables_metadata: Optional[Dict[str, Any]] = None,
-    **storage_options: Dict[str, Any],
+    variables_metadata: Optional[dict[str, Any]] = None,
+    **storage_options: dict[str, Any],
 ):
     """
     Load the Data from the location, dataset name and type of data.
 
     Args:
         root_path: The root path to the Data e.g. `CSUITE_DATASETS_PATH/csuite_linexp_2`
         data_enum: The type of dataset for which to return the path
@@ -58,22 +69,24 @@
         The downloaded data (the type depends on the data requested)
     """
 
     path_name = os.path.join(root_path, data_enum.value)
 
     fsspec_open = partial(fsspec.open, mode="r", encoding="utf-8", **storage_options)
 
+    logger.debug(f"Loading {data_enum} from {path_name} with storage options {storage_options}")
+
     if data_enum == DataEnum.TRUE_ADJACENCY:
         with fsspec_open(path_name) as f:
             return torch.tensor(np.loadtxt(f, dtype=int, delimiter=","))
 
     if data_enum == DataEnum.VARIABLES_JSON:
         if variables_metadata is not None:
             raise ValueError("Variables metadata was supplied and requested")
-        with fsspec_open(path_name, **storage_options) as f:
+        with fsspec_open(path_name) as f:
             return convert_variable_types_to_enum(json.load(f))
 
     if variables_metadata is None:
         variables_metadata = load_data(root_path, data_enum=DataEnum.VARIABLES_JSON)
 
     with fsspec_open(path_name) as f:
         if data_enum in {DataEnum.TRAIN, DataEnum.TEST}:
@@ -87,28 +100,28 @@
             return _load_interventions(json_object=json.load(f), metadata=variables_metadata)
         elif data_enum == DataEnum.COUNTERFACTUALS:
             return _load_counterfactuals(json_object=json.load(f), metadata=variables_metadata)
         else:
             raise RuntimeError("Unrecognized data type")
 
 
-def _load_interventions(json_object: Dict[str, Any], metadata: Dict[str, Any]) -> List[InterventionWithEffects]:
+def _load_interventions(json_object: dict[str, Any], metadata: dict[str, Any]) -> list[InterventionWithEffects]:
     """
     Load the Interventional Datasets as a list of interventions/counterfactuals.
 
     Args:
         json_object: The .json file loaded as a json object.
         metadata: Metadata of the dataset containing names and types.
 
     Returns:
         A list of interventions and the nodes we want to observe for each
     """
     variables_list = metadata["variables"]
 
-    intervened_column_to_group_name: Dict[int, str] = dict(
+    intervened_column_to_group_name: dict[int, str] = dict(
         zip(
             json_object["metadata"]["columns_to_nodes"],
             list(item["group_name"] for item in variables_list),
         )
     )
 
     interventions_list = []
@@ -142,28 +155,28 @@
         # default to all nodes
         if not effect_nodes:
             effect_nodes = set(intervention.sampled_nodes)
         interventions_list.append((intervention, reference, effect_nodes))
     return interventions_list
 
 
-def _load_counterfactuals(json_object: Dict[str, Any], metadata: Dict[str, Any]) -> List[CounterfactualWithEffects]:
+def _load_counterfactuals(json_object: dict[str, Any], metadata: dict[str, Any]) -> list[CounterfactualWithEffects]:
     """
     Load the Interventional Datasets as a list of counterfactuals.
 
     Args:
         json_object: The .json file in loaded as a json object.
         metadata: Metadata of the dataset containing names and types.
 
     Returns:
         A list of counterfactuals and the nodes we want to observe for each
     """
     variables_list = metadata["variables"]
 
-    intervened_column_to_group_name: Dict[int, str] = dict(
+    intervened_column_to_group_name: dict[int, str] = dict(
         zip(
             json_object["metadata"]["columns_to_nodes"],
             list(item["group_name"] for item in variables_list),
         )
     )
 
     cf_list = []
@@ -174,30 +187,34 @@
             np.array(environment["test_data"]),
             factual_data,
             intervention_nodes=intervention_nodes,
             variables_list=variables_list,
         )
         # if the json has reference data create another intervention dataclass
         if (reference_data := environment["reference_data"]) is None:
-            raise RuntimeError()
-        reference = _to_counterfactual(
-            np.array(reference_data), factual_data, intervention_nodes=intervention_nodes, variables_list=variables_list
-        )
+            reference = None
+        else:
+            reference = _to_counterfactual(
+                np.array(reference_data),
+                factual_data,
+                intervention_nodes=intervention_nodes,
+                variables_list=variables_list,
+            )
 
         # store the nodes we're interested in observing
         effect_nodes = set(intervened_column_to_group_name[idx] for idx in environment["effect_idxs"])
         # default to all nodes
         if not effect_nodes:
             effect_nodes = set(intervention.sampled_nodes)
         cf_list.append((intervention, reference, effect_nodes))
     return cf_list
 
 
 def _to_intervention(
-    data: np.ndarray, intervention_nodes: List[str], condition_nodes: List[str], variables_list: List[Dict[str, Any]]
+    data: np.ndarray, intervention_nodes: list[str], condition_nodes: list[str], variables_list: list[dict[str, Any]]
 ) -> InterventionData:
     """Create an `InterventionData` object from the data within the json file."""
     interv_data = tensordict_from_variables_metadata(data, variables_list=variables_list)
 
     # all the intervention values in the dataset should be the same, so we use the first row
     first_row = interv_data[0]
     assert all(torch.allclose(interv_data[node_name], first_row[node_name]) for node_name in intervention_nodes)
@@ -217,15 +234,15 @@
         ),
         intervention_data=convert_one_hot(interv_data, _intersect_dicts_left(categorical_sizes, interv_data)),
         condition_values=convert_one_hot(condition_values, _intersect_dicts_left(categorical_sizes, condition_values)),
     )
 
 
 def _to_counterfactual(
-    data: np.ndarray, base_data: np.ndarray, intervention_nodes: List[str], variables_list: List[Dict[str, Any]]
+    data: np.ndarray, base_data: np.ndarray, intervention_nodes: list[str], variables_list: list[dict[str, Any]]
 ) -> CounterfactualData:
     """Create an `CounterfactualData` object from the data within the json file."""
     interv_data = tensordict_from_variables_metadata(data, variables_list=variables_list)
     # all the intervention values in the dataset should be the same, so we use the first row
     first_row = interv_data[0]
     assert all(torch.allclose(interv_data[node_name], first_row[node_name]) for node_name in intervention_nodes)
     intervention_values = TensorDict(
@@ -240,32 +257,30 @@
             intervention_values, _intersect_dicts_left(categorical_sizes, intervention_values)
         ),
         counterfactual_data=convert_one_hot(interv_data, _intersect_dicts_left(categorical_sizes, interv_data)),
         factual_data=convert_one_hot(factual_data, _intersect_dicts_left(categorical_sizes, factual_data)),
     )
 
 
-def _get_categorical_sizes(variables_list: List[Dict[str, Any]]) -> Dict[str, int]:
+def _get_categorical_sizes(variables_list: list[dict[str, Any]]) -> dict[str, int]:
     categorical_sizes = {}
     for item in variables_list:
         if item["type"] == VariableTypeEnum.CATEGORICAL:
             upper = item.get("upper")
             lower = item.get("lower")
             if upper is not None and lower is not None:
                 categorical_sizes[item["group_name"]] = item["upper"] - item["lower"] + 1
             else:
                 assert upper is None and lower is None, "Please specify either both limits or neither"
                 categorical_sizes[item["group_name"]] = -1
     return categorical_sizes
 
 
-def tensordict_from_variables_metadata(data: np.ndarray, variables_list: List[Dict[str, Any]]) -> TensorDict:
-    """
-    Convert a 2D numpy array and variables information into a `TensorDict`.
-    """
+def tensordict_from_variables_metadata(data: np.ndarray, variables_list: list[dict[str, Any]]) -> TensorDict:
+    """Returns a tensor created by concatenating all values along the last dim."""
     assert data.ndim == 2, "Numpy loading only supported for 2d data"
     batch_size = data.shape[0]
 
     # guaranteed to be ordered correctly in python 3.7+ https://docs.python.org/3/library/collections.html#collections.Counter
     sizes = Counter(d["group_name"] for d in variables_list)  # get the dimensions of each key from the variables
     assert sum(sizes.values()) == data.shape[1], "Variable sizes do not match data shape"
 
@@ -278,10 +293,17 @@
     for key, length in sizes.items():
         d[key] = torch.Tensor(data[:, curr_idx : curr_idx + length]).to(dtype=dtypes[key])
         curr_idx += length
 
     return d
 
 
-def _intersect_dicts_left(dict_1: Dict, dict_2: Dict) -> Dict:
+def tensordict_to_tensor(tensor_dict: TensorDict) -> torch.Tensor:
+    """
+    Convert a `TensorDict` into a 2D `torch.Tensor`.
+    """
+    return torch.cat(tuple(tensor_dict.values()), dim=-1)
+
+
+def _intersect_dicts_left(dict_1: dict, dict_2: dict) -> dict:
     """Select the keys that are in both dictionaries, with values from the first."""
     return {key: dict_1[key] for key in dict_1.keys() & dict_2.keys()}
```

### Comparing `causica-0.2.0/src/causica/datasets/interventional_data.py` & `causica-0.3.0/src/causica/datasets/interventional_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass, field
-from typing import Set
 
 import torch
 from tensordict import TensorDict
 
 
 @dataclass
 class InterventionData:
@@ -19,15 +18,15 @@
         intervention_values: A dictionary of node names to 1D numpy arrays of the intervened values
         condition_values: A dictionary of node names to 1D numpy arrays of the conditioned values
     """
 
     intervention_data: TensorDict
     intervention_values: TensorDict
     condition_values: TensorDict
-    sampled_nodes: Set[str] = field(init=False)  # the nodes that are neither conditioned nor sampled
+    sampled_nodes: set[str] = field(init=False)  # the nodes that are neither conditioned nor sampled
 
     def __post_init__(self):
         assert self.intervention_values.batch_size == torch.Size()
         assert self.condition_values.batch_size == torch.Size()
 
         self.sampled_nodes = (
             set(self.intervention_data.keys())
@@ -53,15 +52,15 @@
             I observed (base observation).
         intervention_values: A dictionary of node names to 1D numpy arrays of the intervened values
     """
 
     counterfactual_data: TensorDict
     intervention_values: TensorDict
     factual_data: TensorDict
-    sampled_nodes: Set[str] = field(init=False)
+    sampled_nodes: set[str] = field(init=False)
 
     def __post_init__(self):
         assert list(self.counterfactual_data.keys()) == list(self.factual_data.keys())
         assert self.counterfactual_data.batch_size == self.factual_data.batch_size
         assert self.intervention_values.batch_size == torch.Size()
 
         self.sampled_nodes = set(self.counterfactual_data.keys()) - set(self.intervention_values.keys())
```

### Comparing `causica-0.2.0/src/causica/datasets/loaded_expert_graph_container.py` & `causica-0.3.0/src/causica/datasets/loaded_expert_graph_container.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/datasets/standardizer.py` & `causica-0.3.0/src/causica/datasets/standardizer.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/datasets/tensordict_utils.py` & `causica-0.3.0/src/causica/datasets/tensordict_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Dict, Optional
+from typing import Optional
 
 import pandas as pd
 import torch
 from tensordict import TensorDict
 
 
 def convert_one_hot(
     data: TensorDict,
-    one_hot_sizes: Optional[Dict[str, int]] = None,
+    one_hot_sizes: Optional[dict[str, int]] = None,
 ):
     """
     Args:
         data: A tensordict representing the underlying data
         one_hot_keys: A list of keys to convert to one hot encodings
     """
     # one hot encode the categorical variables
@@ -22,15 +22,15 @@
     for key, num_classes in one_hot_sizes.items():
         cat_var = new_data[key]
         assert cat_var.shape == new_data.batch_size + (1,), "Only support 1D categorical values"
         new_data[key] = torch.nn.functional.one_hot(cat_var[..., 0].to(torch.long), num_classes=num_classes)
     return new_data
 
 
-def tensordict_shapes(tds: TensorDict) -> Dict[str, torch.Size]:
+def tensordict_shapes(tds: TensorDict) -> dict[str, torch.Size]:
     """Return the shapes within the TensorDict without batch dimensions."""
     return {key: val.shape[len(tds.batch_size) :] for key, val in tds.items()}
 
 
 def tensordict_from_pandas(df: pd.DataFrame) -> TensorDict:
     """
     Create a `TensorDict` from a pandas dataframe.
```

### Comparing `causica-0.2.0/src/causica/distributions/__init__.py` & `causica-0.3.0/src/causica/distributions/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from causica.distributions.adjacency import (
     AdjacencyDistribution,
     ConstrainedAdjacency,
     ConstrainedAdjacencyDistribution,
     ENCOAdjacencyDistribution,
     ENCOAdjacencyDistributionModule,
+    ErdosRenyiDAGDistribution,
     ExpertGraphContainer,
     GibbsDAGPrior,
     ThreeWayAdjacencyDistribution,
 )
 from causica.distributions.distribution_module import DistributionModule
 from causica.distributions.noise import (
     BernoulliNoise,
```

### Comparing `causica-0.2.0/src/causica/distributions/adjacency/__init__.py` & `causica-0.3.0/src/causica/distributions/adjacency/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from causica.distributions.adjacency.adjacency_distributions import AdjacencyDistribution
 from causica.distributions.adjacency.constrained_adjacency_distributions import (
     ConstrainedAdjacency,
     ConstrainedAdjacencyDistribution,
 )
+from causica.distributions.adjacency.directed_acyclic import ErdosRenyiDAGDistribution
 from causica.distributions.adjacency.enco import ENCOAdjacencyDistribution, ENCOAdjacencyDistributionModule
 from causica.distributions.adjacency.gibbs_dag_prior import ExpertGraphContainer, GibbsDAGPrior
 from causica.distributions.adjacency.three_way import ThreeWayAdjacencyDistribution
```

### Comparing `causica-0.2.0/src/causica/distributions/adjacency/adjacency_distributions.py` & `causica-0.3.0/src/causica/distributions/adjacency/adjacency_distributions.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/distributions/adjacency/constrained_adjacency_distributions.py` & `causica-0.3.0/src/causica/distributions/adjacency/constrained_adjacency_distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import partial
-from typing import Callable, Tuple, Type
+from typing import Callable, Type
 
 import torch
 import torch.distributions as td
 
 from causica.distributions.adjacency.adjacency_distributions import AdjacencyDistribution
 from causica.distributions.distribution_module import DistributionModule
 
@@ -109,15 +109,15 @@
         return self.dist.log_prob(value)
 
     def _apply_constraints(self, G: torch.Tensor) -> torch.Tensor:
         """Return G with the positive and negative constraints applied."""
         return 1.0 - (1.0 - G * self.negative_constraints) * (~self.positive_constraints)
 
 
-def get_graph_constraint(graph_constraint_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
+def get_graph_constraint(graph_constraint_matrix: torch.Tensor) -> tuple[torch.Tensor, torch.Tensor]:
     """Converts graph constraint matrix into a positive and negative matrix for easier usage.
 
     Args:
         graph_constraint_matrix: Graph constraints: 0 = no edge, 1 = edge, nan: no constraint. Should be a square matrix
                                  with the lengths matching the number of nodes in the graph.
 
     Returns:
```

### Comparing `causica-0.2.0/src/causica/distributions/adjacency/enco.py` & `causica-0.3.0/src/causica/distributions/adjacency/enco.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/distributions/adjacency/gibbs_dag_prior.py` & `causica-0.3.0/src/causica/distributions/adjacency/gibbs_dag_prior.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional
+from typing import Optional
 
 import torch
 import torch.distributions as td
 
 
 class ExpertGraphContainer(torch.nn.Module):
     def __init__(self, dag: torch.Tensor, mask: torch.Tensor, confidence: float, scale: float) -> None:
@@ -29,15 +29,15 @@
     The prior distribution consists of two terms:
         A sparsity term
         A Expert Graph term that represents some known prior belief about the graph.
 
     Each term has an associated parameter (lambda)
     """
 
-    arg_constraints: Dict = {}
+    arg_constraints: dict = {}
 
     def __init__(
         self,
         num_nodes: int,
         sparsity_lambda: float,
         expert_graph_container: Optional[ExpertGraphContainer] = None,
         **kwargs
```

### Comparing `causica-0.2.0/src/causica/distributions/adjacency/three_way.py` & `causica-0.3.0/src/causica/distributions/adjacency/three_way.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/distributions/distribution_module.py` & `causica-0.3.0/src/causica/distributions/distribution_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/distributions/gumbel_binary.py` & `causica-0.3.0/src/causica/distributions/gumbel_binary.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/distributions/noise/__init__.py` & `causica-0.3.0/src/causica/distributions/noise/__init__.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/distributions/noise/bernoulli.py` & `causica-0.3.0/src/causica/distributions/noise/bernoulli.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/distributions/noise/categorical.py` & `causica-0.3.0/src/causica/distributions/noise/categorical.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/distributions/noise/joint.py` & `causica-0.3.0/src/causica/distributions/noise/joint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from collections import defaultdict
 from enum import Enum
-from typing import Any, Callable, DefaultDict, Dict, Iterable, List, Optional, Tuple, TypeVar
+from typing import Any, Callable, Iterable, Optional, TypeVar
 
 import torch
 from tensordict import TensorDict
 from torch import nn
 
 from causica.datasets.causica_dataset_format import VariableTypeEnum
 from causica.distributions.noise.bernoulli import BernoulliNoiseModule
@@ -17,16 +18,16 @@
 
 class JointNoise(Noise[TensorDict]):
     """Represents an independent joint noise distribution of multiple variables types.
 
     Samples are TensorDicts containining independent variables.
     """
 
-    def __init__(self, independent_noise_dists: Dict[str, Noise[torch.Tensor]]):
-        shapes = DefaultDict[torch.Size, List[str]](list)
+    def __init__(self, independent_noise_dists: dict[str, Noise[torch.Tensor]]):
+        shapes = defaultdict[torch.Size, list[str]](list)
         for name, noise_dist in independent_noise_dists.items():
             shapes[noise_dist.batch_shape].append(name)
         if len(shapes) > 1:
             raise ValueError(f"Incompatible batch shapes: {shapes}")
 
         batch_shape = next(iter(shapes)) if shapes else torch.Size()
         super().__init__(batch_shape=batch_shape, event_shape=torch.Size([len(independent_noise_dists)]))
@@ -66,15 +67,15 @@
             torch.Tensor: The log probability of the given value, of shape
                            `torch.broadcast_shapes(value.batch_size, self.batch_shape)`.
         """
         log_probs = [noise_dist.log_prob(value[name]) for name, noise_dist in self._independent_noise_dists.items()]
         return torch.sum(torch.stack(log_probs, dim=0), dim=0)
 
     @property
-    def support(self) -> Dict[str, Optional[Any]]:
+    def support(self) -> dict[str, Optional[Any]]:
         return {name: noise_dist.support for name, noise_dist in self._independent_noise_dists.items()}
 
     @property
     def mode(self) -> TensorDict:
         return TensorDict(
             {name: noise_dist.mode for name, noise_dist in self._independent_noise_dists.items()},
             batch_size=self.batch_shape,
@@ -94,32 +95,32 @@
 
 class ContinuousNoiseDist(Enum):
     SPLINE = "spline"
     GAUSSIAN = "gaussian"
 
 
 def create_noise_modules(
-    shapes: Dict[str, torch.Size],
-    types: Dict[str, VariableTypeEnum],
+    shapes: dict[str, torch.Size],
+    types: dict[str, VariableTypeEnum],
     continuous_noise_dist: ContinuousNoiseDist,
-) -> Dict[str, NoiseModule[Noise[torch.Tensor]]]:
+) -> dict[str, NoiseModule[Noise[torch.Tensor]]]:
     """Create noise modules for each item of shapes and types.
 
     Args:
         shapes: The shape of each distribution. Currently only the last dimension is used.
         types: Names of variables mapping to the variable type `VariableTypeEnum`.
         continuous_noise_dist: The noise module to use for variable types of `VariableTypeEnum.CONTINUOUS`.
 
     Raises:
         ValueError: If any of the types or the continuous noise distribution is incorrectly specified.
 
     Returns
         Dict of independent noise modules following the shape and type specifications.
     """
-    noise_modules: Dict[str, NoiseModule] = {}
+    noise_modules: dict[str, NoiseModule] = {}
     for key, shape in shapes.items():
         size = shape[-1]
         var_type = types[key]
 
         if var_type == VariableTypeEnum.CATEGORICAL:
             noise_module = CategoricalNoiseModule(size)
         elif var_type == VariableTypeEnum.BINARY:
@@ -139,15 +140,15 @@
 
 class JointNoiseModule(NoiseModule[JointNoise]):
     """Represents JointNoise with learnable parameters.
 
     Each noise module is used independently on their corresponding key of sample TensorDicts.
     """
 
-    def __init__(self, independent_noise_modules: Dict[str, NoiseModule[Noise[torch.Tensor]]]):
+    def __init__(self, independent_noise_modules: dict[str, NoiseModule[Noise[torch.Tensor]]]):
         """
         Args:
             independent_noise_modules: Noise modules to be applied keywise to input TensorDicts. Could e.g. be created
                                        by `create_noise_distributions`.
         """
         super().__init__()
         self.noise_modules = nn.ModuleDict(independent_noise_modules)
@@ -161,10 +162,10 @@
 
     def __getitem__(self, selection: Iterable[str]) -> "JointNoiseModule":
         """Return a JointNoiseModule representing the subset of variables specified in selection."""
         selected_independent_noise_modules = {name: self.noise_modules[name] for name in selection}
         # ModuleDict doesn't allow tracking value types, so ignore the type here.
         return JointNoiseModule(selected_independent_noise_modules)  # type: ignore
 
-    def keys(self) -> Tuple[str, ...]:
+    def keys(self) -> tuple[str, ...]:
         """The keys for the different noise modules in order."""
         return tuple(self.noise_modules)
```

### Comparing `causica-0.2.0/src/causica/distributions/noise/noise.py` & `causica-0.3.0/src/causica/distributions/noise/noise.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,25 @@
         Transform from the sample observations to corresponding noise variables.
 
         Args:
             samples: Tensor of shape sample_shape + batch_shape + event_shape
         Returns:
             The generated samples with shape sample_shape + batch_shape + event_shape
         """
-        pass
 
     @abc.abstractmethod
     def noise_to_sample(self, noise: SampleType) -> SampleType:
         """
         Generate samples using the given exogenous noise.
 
         Args:
             noise: noise variable with shape sample_shape + batch_shape.
         Returns:
             The generated samples with shape sample_shape + batch_shape + event_shape
         """
-        pass
 
 
 BaseNoiseType_co = TypeVar("BaseNoiseType_co", bound=Noise, covariant=True)
 
 
 class IndependentNoise(Generic[BaseNoiseType_co], td.Independent, Noise[torch.Tensor]):
     """Like `td.Idenpendent` but also forwards `Noise` specific methods."""
```

### Comparing `causica-0.2.0/src/causica/distributions/noise/spline/rational_quadratic_transform.py` & `causica-0.3.0/src/causica/functional_relationships/icgnn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,255 +1,228 @@
-"""
-Implementation of the Piecewise Rational Quadratic Transform
+from typing import Optional, Type
 
-This is pretty much a copy-paste of
-    https://github.com/tonyduan/normalizing-flows/blob/master/nf/utils.py
-
-We should consider using the Pyro implementation.
-"""
-from typing import Tuple
-
-import numpy as np
 import torch
-import torch.distributions as td
-from torch.nn import functional as F
+from tensordict import TensorDict
+from torch import nn
 
-DEFAULT_MIN_BIN_WIDTH = 1e-3
-DEFAULT_MIN_BIN_HEIGHT = 1e-3
-DEFAULT_MIN_DERIVATIVE = 1e-3
+from causica.functional_relationships.functional_relationships import (
+    FunctionalRelationships,
+    sample_dict_to_tensor,
+    tensor_to_sample_dict,
+)
 
 
-class PiecewiseRationalQuadraticTransform(td.Transform):
+class ICGNN(FunctionalRelationships):
     """
-    Layer that implements a spline-cdf (https://arxiv.org/abs/1906.04032) transformation.
+    This is a `FunctionalRelationsips` that implements the ICGNN.
 
-    All dimensions of x are treated as independent, no coupling is used. This is needed
-    to ensure invertibility in our additive noise SEM.
+    Details can be found here: https://openreview.net/forum?id=S2pNPZM-w-f
 
-    This is pretty much a copy-paste of
-        https://github.com/tonyduan/normalizing-flows/blob/master/nf/utils.py
+    This wraps the `FGNNI` in a `TensorDict` interface.
     """
 
-    bijective = True
+    def __init__(
+        self,
+        variables: dict[str, torch.Size],
+        embedding_size: Optional[int] = None,
+        out_dim_g: Optional[int] = None,
+        norm_layer: Optional[Type[nn.LayerNorm]] = None,
+        res_connection: bool = False,
+    ) -> None:
+        super().__init__(variables)
 
-    def __init__(self, knot_locations: torch.Tensor, derivatives: torch.Tensor, tail_bound: float = 3.0):
-        """
-        Args:
-            knot_locations: the x, y points of the knots,  shape [dim, num_bins, 2]
-            derivatives: the derivatives at the knots, shape [dim, num_bins - 1]
-            tail_bound: distance of edgemost bins relative to 0,
-        """
-        super().__init__()
-        assert knot_locations.ndim == 3, "Only two dimensional params are supported"
-        assert knot_locations.shape[-1] == 2, "Knot locations are 2-d"
-        self.dim, self.num_bins, *_ = knot_locations.shape
+        # this needs to be a parameter so it is registered to the module
+        self.stacked_variable_masks = torch.nn.Parameter(
+            torch.stack(list(self.variable_masks.values())).float(), requires_grad=False
+        )
 
-        assert derivatives.shape == (self.dim, self.num_bins - 1)
+        self.nn = FGNNI(self.stacked_variable_masks, embedding_size, out_dim_g, norm_layer, res_connection)
 
-        self.tail_bound = tail_bound
-        self._event_dim = 0
+    def forward(self, samples: TensorDict, graphs: torch.Tensor) -> TensorDict:
+        return tensor_to_sample_dict(
+            self.nn(sample_dict_to_tensor(samples, self.variable_masks), graphs), self.variable_masks
+        )
 
-        self.knot_locations = knot_locations
-        self.derivatives = derivatives
 
-    @property
-    def event_dim(self):
-        return self._event_dim
+class FGNNI(nn.Module):
+    """
+    Defines the function f for the SEM. For each variable x_i we use
+    f_i(x) = f(e_i, sum_{k in pa(i)} g(e_k, x_k)), where e_i is a learned embedding
+    for node i.
+    """
 
-    def _piecewise_cdf(self, inputs: torch.Tensor, inverse: bool = False) -> Tuple[torch.Tensor, torch.Tensor]:
+    def __init__(
+        self,
+        group_mask: torch.Tensor,
+        embedding_size: Optional[int] = None,
+        out_dim_g: Optional[int] = None,
+        norm_layer: Optional[Type[nn.LayerNorm]] = None,
+        res_connection: bool = False,
+    ):
         """
-        Evaluate the Cumulative Density function at `inputs`
-
         Args:
-            inputs: the positions at which to evaluate the cdf shape batch_shape + (input_dim)
-            inverse: whether this is forwards or backwards transform
-        Returns:
-            input_evaluations and absolute log determinants, a tuple of tensors of shape batch_shape + (input_dim)
+            group_mask: A mask of shape (num_nodes, num_processed_cols) such that group_mask[i, j] = 1. when col j is in group i.
+            embedding_size: Size of the embeddings used by each node. If none, default is processed_dim_all.
+            out_dim_g: Output dimension of the "inner" NN, g. If none, default is embedding size.
+            layers_g: Size of the layers of NN g. Does not include input not output dim. If none, default
+                      is [a], with a = max(2 * input_dim, embedding_size, 10).
+            layers_f: Size of the layers of NN f. Does not include input nor output dim. If none, default
+                      is [a], with a = max(2 * input_dim, embedding_size, 10)
         """
-        assert len(inputs.shape) == 2  # TODO(JJ) accept 1d inputs
-        batch_shape = inputs.shape[:-1]
-        # shape batch_shape + (dim, 3 * num_bins - 1)
-        expanded_knot_locations = self.knot_locations[None, ...].expand(*batch_shape, -1, -1, -1)
-
-        unnormalized_derivatives = F.pad(
-            self.derivatives[None, ...].expand(*batch_shape, -1, -1),
-            pad=(1, 1),
-            value=np.log(np.expm1(1 - DEFAULT_MIN_DERIVATIVE)),
-        )  # shape batch_shape + (dim, num_bins + 1)
-
-        inside_intvl_mask = torch.abs(inputs) <= self.tail_bound
-        outputs = inputs.clone().detach()  # shape batch_shape + (input_dim)
-        outputs[inside_intvl_mask] = 0
-
-        logabsdet = torch.zeros_like(inputs)  # shape batch_shape + (input_dim)
-
-        if inside_intvl_mask.any():
-            outputs[inside_intvl_mask], logabsdet[inside_intvl_mask] = rational_quadratic_spline(
-                inputs=inputs[inside_intvl_mask],
-                unnormalized_knot_locations=expanded_knot_locations[inside_intvl_mask, :, :],
-                unnormalized_derivatives=unnormalized_derivatives[inside_intvl_mask, :],
-                inverse=inverse,
-                tail_bound=self.tail_bound,
-            )
-        return outputs, logabsdet
-
-    @td.constraints.dependent_property(is_discrete=False)
-    def domain(self):
-        if self.event_dim == 0:
-            return td.constraints.real
-        return td.constraints.independent(td.constraints.real, self.event_dim)
-
-    @td.constraints.dependent_property(is_discrete=False)
-    def codomain(self):
-        if self.event_dim == 0:
-            return td.constraints.real
-        return td.constraints.independent(td.constraints.real, self.event_dim)
+        super().__init__()
+        self.group_mask = group_mask
+        self.num_nodes, self.processed_dim_all = group_mask.shape
+        # Initialize embeddings
+        self.embedding_size = self.processed_dim_all if embedding_size is None else embedding_size
+        aux = torch.randn(self.num_nodes, self.embedding_size) * 0.01
+        self.embeddings = nn.parameter.Parameter(aux, requires_grad=True)  # Shape (input_dim, embedding_size)
+
+        # Set value for out_dim_g
+        out_dim_g = self.embedding_size if out_dim_g is None else out_dim_g
+        # Set NNs sizes
+        a = max(4 * self.processed_dim_all, self.embedding_size, 64)
+        in_dim_g = self.embedding_size + self.processed_dim_all
+        in_dim_f = self.embedding_size + out_dim_g
+        self.g = generate_fully_connected(
+            input_dim=in_dim_g,
+            output_dim=out_dim_g,
+            hidden_dims=[a, a],
+            non_linearity=nn.LeakyReLU,
+            activation=nn.Identity,
+            device=group_mask.device,
+            normalization=norm_layer,
+            res_connection=res_connection,
+        )
+        self.f = generate_fully_connected(
+            input_dim=in_dim_f,
+            output_dim=self.processed_dim_all,
+            hidden_dims=[a, a],
+            non_linearity=nn.LeakyReLU,
+            activation=nn.Identity,
+            device=group_mask.device,
+            normalization=norm_layer,
+            res_connection=res_connection,
+        )
+        self.w = torch.nn.Parameter(torch.zeros((self.num_nodes, self.num_nodes)), requires_grad=True)
 
-    def _call(self, x: torch.Tensor) -> torch.Tensor:
-        """
-        Args:
-            x: batch_shape + (input_dim)
-        Returns:
-            transformed_input batch_shape + (input_dim)
+    def forward(self, samples: torch.Tensor, graphs: torch.Tensor) -> torch.Tensor:
         """
-        return self._piecewise_cdf(x, inverse=False)[0]
+        Computes non-linear function h(X, W) using the given weighted adjacency matrix.
 
-    def _inverse(self, y: torch.Tensor) -> torch.Tensor:
-        """
-        Args:
-            y: batch_shape + (input_dim)
-        Returns:
-            transformed_input, batch_shape + (input_dim)
-        """
-        return self._piecewise_cdf(y, inverse=True)[0]
+        g takes inputs of size batch_shape + (embedding_size + processed_dim_all) and outputs batch_shape + (out_dim_g)
+        the input will be appropriately masked to correspond to one variable group
+
+        f takes inputs of size batch_shape + (embedding_size + out_dim_g) and outputs batch_shape + (processed_dim_all)
+        the ouptut is then masked to correspond to one variable
 
-    def log_abs_det_jacobian(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        """
         Args:
-            input: batch_shape + (input_dim)
+            samples: Batched inputs, size batch_size_x + (processed_dim_all).
+            graphs: Weighted adjacency matrix, size batch_size_g + (n, n)
         Returns:
-            jacobian_log_determinant: batch_shape + (input_dim)
+            A tensor of shape batch_shape_x + batch_shape_g + (processed_dim_all)
         """
-        return self._piecewise_cdf(x, inverse=False)[1]
+        batch_shape_x = samples.shape[:-1]
+        batch_shape_g = graphs.shape[:-2]
 
-
-def rational_quadratic_spline(
-    inputs: torch.Tensor,
-    unnormalized_knot_locations: torch.Tensor,
-    unnormalized_derivatives: torch.Tensor,
-    inverse: bool = False,
-    tail_bound: float = 1.0,
-) -> Tuple[torch.Tensor, torch.Tensor]:
+        # Generate required input for g (concatenate X and embeddings)
+        # Pointwise multiply X
+        # Shape batch_shape_x + (num_nodes, processed_dim_all)
+        masked_samples = torch.einsum("...i,ji->...ji", samples, self.group_mask)
+        E = self.embeddings.expand(*batch_shape_x, -1, -1)  # Shape batch_shape_x + (num_nodes, embedding_size)
+
+        # Shape batch_shape_x + (num_nodes, embedding_size + processed_dim_all)
+        embedded_samples = self.g(
+            torch.cat([masked_samples, E], dim=-1)
+        )  # Shape batch_shape_x + (num_nodes, out_dim_g)
+
+        target_shape = batch_shape_x + batch_shape_g + embedded_samples.shape[-2:]
+        view_shape = batch_shape_x + (1,) * len(batch_shape_g) + embedded_samples.shape[-2:]
+        # Shape batch_shape_x + batch_shape_g + (num_nodes, out_dim_g)
+        embedded_samples_broad = embedded_samples.view(view_shape).expand(target_shape)
+        # Aggregate sum and generate input for f (concatenate X_aggr and embeddings)
+        # Shape batch_shape_x + batch_shape_g + (num_nodes, out_dim_g)
+        samples_aggr_sum = torch.einsum("...jk,...jl->...lk", embedded_samples_broad, graphs * self.w)
+
+        # expand dimensions of E batch_shape_x + batch_shape_g + (num_nodes, embedding_size)
+        E_broad = E.view(view_shape).expand(target_shape)
+        # Run f Shape batch_shape_x + batch_shape_g + (num_nodes, processed_dim_all)
+        samples_rec = self.f(torch.cat([samples_aggr_sum, E_broad], dim=-1))
+        # Mask and aggregate Shape batch_shape_x + batch_shape_g + (processed_dim_all)
+        return torch.einsum("...ij,ij->...j", samples_rec, self.group_mask)
+
+
+def generate_fully_connected(
+    input_dim: int,
+    output_dim: int,
+    hidden_dims: list[int],
+    non_linearity: Optional[Type[nn.Module]],
+    activation: Optional[Type[nn.Module]],
+    device: torch.device,
+    p_dropout: float = 0.0,
+    normalization: Optional[Type[nn.LayerNorm]] = None,
+    res_connection: bool = False,
+) -> nn.Module:
     """
+    Generate a fully connected network.
+
     Args:
-        inputs: shape batch_shape + (input_dim)
-        unnormalized_knot_locations: shape batch_shape + (dim, num_bins, 2)
-        unnormalized_derivatives: shape batch_shape + (dim, num_bins + 1)
-        inverse: whether this is the forward or backward pass
-        tail_bound:
+        input_dim: Int. Size of input to network.
+        output_dim: Int. Size of output of network.
+        hidden_dims: List of int. Sizes of internal hidden layers. i.e. [a, b] is three linear layers with shapes (input_dim, a), (a, b), (b, output_dim)
+        non_linearity: Non linear activation function used between Linear layers.
+        activation: Final layer activation to use.
+        device: torch device to load weights to.
+        p_dropout: Float. Dropout probability at the hidden layers.
+        init_method: initialization method
+        normalization: Normalisation layer to use (batchnorm, layer norm, etc). Will be placed before linear layers, excluding the input layer.
+        res_connection : Whether to use residual connections where possible (if previous layer width matches next layer width)
+
     Returns:
-        the outputs and the absolute log determinant, a tuple of tensors of shape batch_shape + (input_dim)
+        Sequential object containing the desired network.
     """
+    layers: list[nn.Module] = []
 
-    if (torch.abs(inputs) > tail_bound).any():
-        raise ValueError("Input outside domain")
+    prev_dim = input_dim
+    for idx, hidden_dim in enumerate(hidden_dims):
 
-    num_bins = unnormalized_knot_locations.shape[-2]
+        block: list[nn.Module] = []
 
-    if DEFAULT_MIN_BIN_WIDTH * num_bins > 1.0:
-        raise ValueError("Minimal bin width too large for the number of bins")
-    if DEFAULT_MIN_BIN_HEIGHT * num_bins > 1.0:
-        raise ValueError("Minimal bin height too large for the number of bins")
-
-    # create the bins
-    derivatives = DEFAULT_MIN_DERIVATIVE + F.softplus(unnormalized_derivatives)
-    # shape batch_shape + (dim)
-    widths, cumwidths = normalize_bins(
-        unnormalized_knot_locations[..., 0], tail_bound=tail_bound, min_bin_size=DEFAULT_MIN_BIN_WIDTH
-    )
-    heights, cumheights = normalize_bins(
-        unnormalized_knot_locations[..., 1], tail_bound=tail_bound, min_bin_size=DEFAULT_MIN_BIN_HEIGHT
-    )
-
-    # place the input data within the bins
-    bin_idx = torch.searchsorted(cumheights if inverse else cumwidths, inputs[..., None]) - 1
-
-    input_cumwidths = cumwidths.gather(-1, bin_idx)[..., 0]
-    input_bin_widths = widths.gather(-1, bin_idx)[..., 0]
-
-    input_cumheights = cumheights.gather(-1, bin_idx)[..., 0]
-    input_bin_heights = heights.gather(-1, bin_idx)[..., 0]
-
-    delta = heights / widths
-    input_delta = delta.gather(-1, bin_idx)[..., 0]
-
-    input_derivatives = derivatives.gather(-1, bin_idx)[..., 0]
-    input_derivatives_plus_one = derivatives[..., 1:].gather(-1, bin_idx)
-    input_derivatives_plus_one = input_derivatives_plus_one[..., 0]
-
-    # here be dragons
-    if inverse:
-        a = (inputs - input_cumheights) * (
-            input_derivatives + input_derivatives_plus_one - 2 * input_delta
-        ) + input_bin_heights * (input_delta - input_derivatives)
-        b = input_bin_heights * input_derivatives - (inputs - input_cumheights) * (
-            input_derivatives + input_derivatives_plus_one - 2 * input_delta
-        )
-        c = -input_delta * (inputs - input_cumheights)
+        if normalization is not None and idx > 0:
+            block.append(normalization(prev_dim).to(device))
+        block.append(nn.Linear(prev_dim, hidden_dim).to(device))
 
-        discriminant = b * b - 4 * a * c
-        assert (discriminant >= 0).all()
+        if non_linearity is not None:
+            block.append(non_linearity())
+        if p_dropout != 0:
+            block.append(nn.Dropout(p_dropout))
 
-        theta = (2 * c) / (-b - torch.sqrt(discriminant))
-        theta_one_minus_theta = theta * (1 - theta)
+        if res_connection and (prev_dim == hidden_dim):
+            layers.append(_ResBlock(nn.Sequential(*block)))
+        else:
+            layers.append(nn.Sequential(*block))
+        prev_dim = hidden_dim
 
-        outputs = theta * input_bin_widths + input_cumwidths
+    if normalization is not None:
+        layers.append(normalization(prev_dim).to(device))
+    layers.append(nn.Linear(prev_dim, output_dim).to(device))
 
-        denominator = input_delta + (
-            (input_derivatives + input_derivatives_plus_one - 2 * input_delta) * theta_one_minus_theta
-        )
-        derivative_numerator = input_delta.pow(2) * (
-            input_derivatives_plus_one * theta * theta
-            + 2 * input_delta * theta_one_minus_theta
-            + input_derivatives * (1 - theta).pow(2)
-        )
-        logabsdet = torch.log(derivative_numerator) - 2 * torch.log(denominator)
-        return outputs, -logabsdet
-    else:
-        theta = (inputs - input_cumwidths) / input_bin_widths
-        theta_one_minus_theta = theta * (1 - theta)
-
-        numerator = input_bin_heights * (input_delta * theta * theta + input_derivatives * theta_one_minus_theta)
-        denominator = input_delta + (
-            (input_derivatives + input_derivatives_plus_one - 2 * input_delta) * theta_one_minus_theta
-        )
-        outputs = input_cumheights + numerator / denominator
+    if activation is not None:
+        layers.append(activation())
 
-        derivative_numerator = input_delta.pow(2) * (
-            input_derivatives_plus_one * theta.pow(2)
-            + 2 * input_delta * theta_one_minus_theta
-            + input_derivatives * (1 - theta).pow(2)
-        )
-        logabsdet = torch.log(derivative_numerator) - 2 * torch.log(denominator)
-        return outputs, logabsdet
+    return nn.Sequential(*layers)
 
 
-def normalize_bins(
-    bins: torch.Tensor, tail_bound: float, min_bin_size: float = 1e-3
-) -> Tuple[torch.Tensor, torch.Tensor]:
+class _ResBlock(nn.Module):
     """
-    For a tensor of unnormalized bin widths `bins`, create bins in [-tail_bound, tail_bound]
-
-    Args:
-        bins: shape (..., num_bins)
-        tail_bound: the size of interval to project to
-        min_bin_size: the minimum bin size
-    Returns:
-        Tuple of the normalized bin_widths and their locations shape (..., num_bins) and (..., num_bins + 1)
+    Wraps an nn.Module, adding a skip connection to it.
     """
-    num_bins = bins.shape[-1]
-    # shape batch_shape + (dim)
-    norm_bins = min_bin_size + (1 - min_bin_size * num_bins) * F.softmax(bins, dim=-1)
-    cum_norm_bins = F.pad(torch.cumsum(norm_bins, dim=-1), pad=(1, 0), mode="constant", value=0.0)
-    cum_norm_bins = tail_bound * (2 * cum_norm_bins - 1)
-    norm_bins = torch.diff(cum_norm_bins)
-    return norm_bins, cum_norm_bins
+
+    def __init__(self, block: nn.Module):
+        """
+        Args:
+            block: module to which skip connection will be added. The input dimension must match the output dimension.
+        """
+        super().__init__()
+        self.block = block
+
+    def forward(self, x):
+        return x + self.block(x)
```

### Comparing `causica-0.2.0/src/causica/distributions/noise/spline/spline.py` & `causica-0.3.0/src/causica/distributions/noise/spline/spline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import List, Optional, Tuple, Union
+from typing import Optional, Union
 
 import torch
 import torch.distributions as td
 from torch import nn
 
 from causica.distributions.noise.noise import IndependentNoise, Noise, NoiseModule
 from causica.distributions.noise.spline.rational_quadratic_transform import PiecewiseRationalQuadraticTransform
 
 # Ordered inputs to `_create_composite_layer`
-SplineParams = Tuple[torch.Tensor, ...]
+SplineParams = tuple[torch.Tensor, ...]
 
 
 class SplineNoise(td.TransformedDistribution, Noise):
     """A Spline Based Noise Distribution.
 
     Parametrized as in in [Neural Spline Flows](https://arxiv.org/pdf/1906.04032.pdf).
     """
 
     def __init__(
         self,
         base_loc: torch.Tensor,
         base_scale: torch.Tensor,
-        spline_transforms: List[Union[td.AffineTransform, td.ComposeTransform]],
+        spline_transforms: list[Union[td.AffineTransform, td.ComposeTransform]],
     ):
         """
         Args:
             base_loc: Loc of base normal distribution.
             base_scale: Scale of base normal distribution.
             spline_transforms: Spline transforms, where the last transform bijects from noise to samples.
         """
@@ -70,28 +70,28 @@
 
 def create_spline_dist_params(
     dim: int,
     num_bins: int,
     flow_steps: int,
     knot_locations_scale: float,
     derivatives_scale: float,
-) -> List[SplineParams]:
+) -> list[SplineParams]:
     """Create initial values for a spline distribution.
 
     Args:
         dim: Number of dimensions of the represented variable.
         num_bins: Number of spline bins.
         flow_steps: Number of flow steps.
         knot_locations_scale: Scale of random values used for `knot_locations` of `PiecewiseRationalQuadraticTransform`.
         derivatives_scale: Scale of random values for `derivatives` of `PiecewiseRationalQuadraticTransform`.
 
     Returns:
         A list of parameters for `CompositeSplineLayer`s.
     """
-    param_list: List[SplineParams] = []
+    param_list: list[SplineParams] = []
     for i in range(flow_steps + 1):
         log_scale = torch.zeros(dim)  # this will be exponentiated when passed to the spline distribution
         loc = torch.zeros(dim)
         if i == flow_steps:
             param_list.append((loc, log_scale))
         else:
             knot_locations = knot_locations_scale * torch.randn(dim, num_bins, 2)
```

### Comparing `causica-0.2.0/src/causica/distributions/noise/univariate_normal.py` & `causica-0.3.0/src/causica/distributions/noise/univariate_normal.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/distributions/sem_distribution.py` & `causica-0.3.0/src/causica/distributions/sem_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Dict, List
-
 import torch
 import torch.distributions as td
 from torch.distributions.constraints import Constraint
 
 from causica.distributions.adjacency import AdjacencyDistribution
 from causica.distributions.distribution_module import DistributionModule
 from causica.distributions.noise.joint import JointNoiseModule
@@ -17,15 +15,15 @@
     Samples are instances of DistributionParametersSEM.
 
     The distribution is essentially the same as the given adjacency distribution but with samples converted to SEMs.
     Therefore, all distribution properties such as entropy, mean and mode are given by the equivalent properties for the
     adjacency distribution.
     """
 
-    arg_constraints: Dict[str, Constraint] = {}
+    arg_constraints: dict[str, Constraint] = {}
 
     def __init__(
         self,
         adjacency_dist: AdjacencyDistribution,
         noise_module: JointNoiseModule,
         functional_relationships: FunctionalRelationships,
     ):
@@ -36,15 +34,15 @@
             functional_relationships: The functional relationship for any SEM of this distribution.
         """
         super().__init__()
         self._adjacency_dist = adjacency_dist
         self._noise_module = noise_module
         self._functional_relationships = functional_relationships
 
-    def _create_sems(self, graphs: torch.Tensor) -> List[DistributionParametersSEM]:
+    def _create_sems(self, graphs: torch.Tensor) -> list[DistributionParametersSEM]:
         graphs = graphs.reshape(-1, *graphs.shape[-2:])
         return [
             DistributionParametersSEM(
                 graph=graph,
                 noise_dist=self._noise_module,
                 func=self._functional_relationships,
             )
@@ -55,15 +53,15 @@
         graphs = self._adjacency_dist.sample(sample_shape)
         if not sample_shape:
             graphs = graphs[None, ...]
         return self._create_sems(graphs)
 
     def relaxed_sample(
         self, sample_shape: torch.Size = torch.Size(), temperature: float = 0.0
-    ) -> List[DistributionParametersSEM]:
+    ) -> list[DistributionParametersSEM]:
         graphs = self._adjacency_dist.relaxed_sample(sample_shape=sample_shape, temperature=temperature)
         return self._create_sems(graphs)
 
     def entropy(self) -> torch.Tensor:
         return self._adjacency_dist.entropy()
 
     @property
```

### Comparing `causica-0.2.0/src/causica/distributions/transforms.py` & `causica-0.3.0/src/causica/distributions/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 Wrapper around torch.distributions.transforms to allow for joint transforms on TensorDicts.
 """
-from typing import Dict
 
 import torch
 import torch.distributions as td
 from tensordict import TensorDict
 
 
 class JointTransform(td.Transform):
     """A joint transform that applies a different transform to each key in the TensorDict.
 
     This is heavily inspired by the `torch.distributions.transforms.StackTransform` class.
     See https://pytorch.org/docs/stable/distributions.html#torch.distributions.transforms.StackTransform
     """
 
-    def __init__(self, transformations: Dict[str, td.Transform], cache_size: int = 0):
+    def __init__(self, transformations: dict[str, td.Transform], cache_size: int = 0):
         """
         Args:
             transformations: A dictionary of transforms, where the keys are the keys in the TensorDict
             cache_size: Size of cache. If zero, no caching is done. If one, the latest single value is cached.
                 Only 0 and 1 are supported.
         """
         assert all(
```

### Comparing `causica-0.2.0/src/causica/fsspec_helpers.py` & `causica-0.3.0/src/causica/fsspec_helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Any, Dict
+from typing import Any
 
 import fsspec
 
 
-def get_storage_options_for_path(path: str) -> Dict[str, Any]:
+def get_storage_options_for_path(path: str) -> dict[str, Any]:
     """Get storage options for a given path.
 
     This checks whether a path uses the abfs protocol and if so returns storage options for the Azure Blob Storage.
 
     Args:
         path: fsspec compatible path
```

### Comparing `causica-0.2.0/src/causica/functional_relationships/do_functional_relationships.py` & `causica-0.3.0/src/causica/functional_relationships/do_functional_relationships.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Tuple
-
 import torch
 from tensordict import TensorDict
 
 from causica.functional_relationships.functional_relationships import FunctionalRelationships
 
 
 class DoFunctionalRelationships(FunctionalRelationships):
@@ -80,15 +78,15 @@
     assign_mask[..., ~x_mask, :] = 0
     assign_mask[..., :, ~y_mask] = 0
     A[assign_mask] = B.flatten()
 
 
 def create_do_functional_relationship(
     interventions: TensorDict, func: FunctionalRelationships, graph: torch.Tensor
-) -> Tuple[DoFunctionalRelationships, torch.Tensor]:
+) -> tuple[DoFunctionalRelationships, torch.Tensor]:
     """
     Given a set of interventions, `FunctionalRelationships` and a graph, create a `DoFunctionalRelationships` and an intervened graph.
 
     Args:
         interventions: the nodes and their intervention values
         func: the functional relationship of the unintervened SEM
         graph: the unintervened graph shape: [..., num_nodes, num_nodes]
```

### Comparing `causica-0.2.0/src/causica/functional_relationships/functional_relationships.py` & `causica-0.3.0/src/causica/functional_relationships/functional_relationships.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import abc
-from typing import Any, Dict
+from typing import Any
 
 import torch
 from tensordict import TensorDict
 
 
 class FunctionalRelationships(abc.ABC, torch.nn.Module):
-    def __init__(self, variables: Dict[str, torch.Size]) -> None:
+    def __init__(self, variables: dict[str, torch.Size]) -> None:
         """_summary_
 
         Args:
             variables: Dict of node shapes (how many dimensions a variable has)
                 Order corresponds to the order in graph(s).
         """
         super().__init__()
@@ -23,20 +23,20 @@
         for name, shape in variables.items():
             mask = torch.zeros(self.output_shape, dtype=torch.bool)
             mask[last_idx : last_idx + shape.numel()] = True
 
             self.variable_masks[name] = mask
             last_idx += shape.numel()
 
-    def set_extra_state(self, state: Dict[str, Any]):
+    def set_extra_state(self, state: dict[str, Any]):
         self.num_nodes = state.pop("num_nodes")
         self.variables = state.pop("variables")
         self.output_shape = state.pop("output_shape")
 
-    def get_extra_state(self) -> Dict[str, Any]:
+    def get_extra_state(self) -> dict[str, Any]:
         return {
             "num_nodes": self.num_nodes,
             "variables": self.variables,
             "output_shape": self.output_shape,
         }
 
     @abc.abstractmethod
@@ -46,20 +46,19 @@
         Args:
             samples: dictionary of variable samples of shape sample_shape + [node shape]
             graphs: tensor of shape batch_shape + [nodes, nodes]
 
         Returns:
             Dictionary of torch.Tensors of shape sample_shape + batch_shape + [node shape]
         """
-        pass
 
 
-def sample_dict_to_tensor(sample_dict: TensorDict, variable_masks: Dict[str, torch.Tensor]) -> torch.Tensor:
+def sample_dict_to_tensor(sample_dict: TensorDict, variable_masks: dict[str, torch.Tensor]) -> torch.Tensor:
     """Converts a sample dictionary to a tensor."""
     return torch.cat([sample_dict[name] for name in variable_masks.keys()], dim=-1)
 
 
-def tensor_to_sample_dict(sample_tensor: torch.Tensor, variable_masks: Dict[str, torch.Tensor]) -> TensorDict:
+def tensor_to_sample_dict(sample_tensor: torch.Tensor, variable_masks: dict[str, torch.Tensor]) -> TensorDict:
     """Converts a tensor to a sample dictionary."""
     return TensorDict(
         {name: sample_tensor[..., mask] for name, mask in variable_masks.items()}, batch_size=sample_tensor.shape[:-1]
     )
```

### Comparing `causica-0.2.0/src/causica/functional_relationships/linear_functional_relationships.py` & `causica-0.3.0/src/causica/functional_relationships/linear_functional_relationships.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Dict
-
 import torch
 from tensordict import TensorDict
 
 from causica.functional_relationships.functional_relationships import (
     FunctionalRelationships,
     sample_dict_to_tensor,
     tensor_to_sample_dict,
@@ -13,15 +11,15 @@
 class LinearFunctionalRelationships(FunctionalRelationships):
     """
     A simple linear functional relationship.
     """
 
     def __init__(
         self,
-        variables: Dict[str, torch.Size],
+        variables: dict[str, torch.Size],
         initial_linear_coefficient_matrix: torch.Tensor,
         trainable: bool = False,
     ) -> None:
         """
         Args:
             variables: Dict of node shapes (how many dimensions a variable has)
                 Order corresponds to the order in graph(s).
```

### Comparing `causica-0.2.0/src/causica/graph/evaluation_metrics.py` & `causica-0.3.0/src/causica/graph/evaluation_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from typing import Tuple
-
 import torch
 
 from causica.triangular_transformations import unfill_triangular
 
 
-def adjacency_precision_recall(graph1: torch.Tensor, graph2: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
+def adjacency_precision_recall(graph1: torch.Tensor, graph2: torch.Tensor) -> tuple[torch.Tensor, torch.Tensor]:
     """Evaluate the precision and recall of edge existence for two adjacency matrices."""
     vec1 = torch.abs(_to_vector(graph1)) > 0
     vec2 = torch.abs(_to_vector(graph2)) > 0
 
     correspondence = (vec1 & vec2).sum()
 
     if (vec1_sum := vec1.sum()) != 0:
@@ -26,15 +24,15 @@
 
 
 def adjacency_f1(graph1: torch.Tensor, graph2: torch.Tensor) -> torch.Tensor:
     """Evaluate the f1 score of edge existence for two adjacency matrices."""
     return f1_score(*adjacency_precision_recall(graph1, graph2))
 
 
-def orientation_precision_recall(graph1: torch.Tensor, graph2: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
+def orientation_precision_recall(graph1: torch.Tensor, graph2: torch.Tensor) -> tuple[torch.Tensor, torch.Tensor]:
     """Evaluate the precision and recall of edge orientation for two adjacency matrices."""
     vec1 = _to_vector(graph1)
     vec2 = _to_vector(graph2)
     non_zero_vec1 = vec1 != 0
     non_zero_vec2 = vec2 != 0
 
     if (non_zero_vec1_sum := non_zero_vec1.sum()) != 0:
```

### Comparing `causica-0.2.0/src/causica/lightning/callbacks.py` & `causica-0.3.0/src/causica/lightning/callbacks.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,25 @@
         is_converged = self.scheduler.step(
             optimizer=optimizer,
             loss=auglag_loss,
             loss_value=outputs["loss"].item(),
             lagrangian_penalty=outputs["constraint"].item(),
         )
 
+        auglag_logging_attributes = [
+            "num_lr_updates",
+            "outer_opt_counter",
+            "step_counter",
+            "outer_below_penalty_tol",
+            "outer_max_rho",
+            "last_best_step",
+            "last_lr_update_step",
+        ]
+        pl_module.log_dict({f"auglag/{k}": getattr(self.scheduler, k) for k in auglag_logging_attributes}, on_step=True)
+
         # Notify trainer to stop if the auglag algorithm has converged
         if is_converged:
             trainer.should_stop = True
 
 
 class MLFlowSaveConfigCallback(SaveConfigCallback):
     """Logs the config using MLFlow if there is an active run, otherwise saves locally as the superclass."""
@@ -59,15 +70,15 @@
             parser=parser, config=config, config_filename=config_filename, overwrite=True, multifile=multifile
         )
 
     def setup(self, trainer: pl.Trainer, pl_module: pl.LightningModule, stage: TrainerFn) -> None:  # type: ignore
         # Save the file on rank 0
         if trainer.is_global_zero and stage == TrainerFn.FITTING:
             with TemporaryDirectory() as tmpdir:
-                temporary_config_path = str(Path(tmpdir) / (f"{stage.value}_" + self.config_filename))
+                temporary_config_path = str(Path(tmpdir) / self.config_filename)
                 self.parser.save(
                     self.config,
                     temporary_config_path,
                     skip_none=False,
                     overwrite=self.overwrite,
                     multifile=self.multifile,
                 )
```

### Comparing `causica-0.2.0/src/causica/lightning/cli.py` & `causica-0.3.0/src/causica/lightning/cli.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/lightning/deci_module.py` & `causica-0.3.0/src/causica/lightning/modules/deci_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, Dict, List, Optional, Sequence, Union
+from typing import Any, Optional, Sequence, Union
 
 import fsspec
 import numpy as np
 import pytorch_lightning as pl
 import torch
 from pytorch_lightning.trainer.states import TrainerFn
 from pytorch_lightning.utilities.types import STEP_OUTPUT
@@ -23,16 +23,16 @@
 )
 from causica.distributions.noise.joint import ContinuousNoiseDist
 from causica.fsspec_helpers import get_storage_options_for_path
 from causica.functional_relationships import ICGNN
 from causica.graph.dag_constraint import calculate_dagness
 from causica.graph.evaluation_metrics import adjacency_f1, orientation_f1
 from causica.lightning.callbacks import AuglagLRCallback
-from causica.lightning.data_modules import VariableSpecDataModule
-from causica.lightning.variable_spec_module import VariableSpecModule
+from causica.lightning.data_modules.deci_data_module import DECIDataModule
+from causica.lightning.modules.variable_spec_module import VariableSpecModule
 from causica.sem.structural_equation_model import SEM
 from causica.training.auglag import AugLagLossCalculator, AugLagLR, AugLagLRConfig
 from causica.training.evaluation import (
     eval_ate_rmse,
     eval_intervention_likelihoods,
     eval_ite_rmse,
     list_logsumexp,
@@ -109,29 +109,29 @@
             self.num_samples,
             self.variable_group_shapes,
             self.variable_types,
             self.variable_names,
         ]
         if any(member is None for member in dataset_defined_members):
             datamodule = getattr(self.trainer, "datamodule", None)
-            if not isinstance(datamodule, VariableSpecDataModule):
+            if not isinstance(datamodule, DECIDataModule):
                 raise TypeError(
                     f"Incompatible data module {datamodule}, requires a DECIDataModule but is "
                     f"{type(datamodule).mro()}"
                 )
             if self.dataset_name is None:
                 self.dataset_name = datamodule.dataset_name
             if self.num_samples is None:
                 self.num_samples = len(datamodule.dataset_train)
             if self.variable_group_shapes is None:
-                self.variable_group_shapes = datamodule.get_variable_shapes()
+                self.variable_group_shapes = datamodule.variable_shapes
             if self.variable_types is None:
-                self.variable_types = datamodule.get_variable_types()
+                self.variable_types = datamodule.variable_types
             if self.variable_names is None:
-                self.variable_names = datamodule.get_variable_names()
+                self.variable_names = datamodule.column_names
 
     def setup(self, stage: Optional[str] = None):
         if self.is_setup:
             return  # Already setup
         elif stage not in {TrainerFn.TESTING, TrainerFn.FITTING}:
             raise ValueError(f"Model can only be setup during the {TrainerFn.FITTING} and {TrainerFn.TESTING} stages.")
 
@@ -245,23 +245,23 @@
         orient_f1 = list_mean([orientation_f1(true_adj_matrix, graph) for graph in graph_samples]).item()
         self.log("eval/adjacency.f1", adj_f1, add_dataloader_idx=False)
         self.log("eval/orientation.f1", orient_f1, add_dataloader_idx=False)
 
     def test_step_interventions(self, interventions: InterventionWithEffects, *args, **kwargs):
         """Evaluate the ATE and Interventional log prob performance of the model"""
         _, _ = args, kwargs
-        sems_list: List[SEM] = list(self.sem_module().sample(torch.Size([NUM_ATE_ITE_SEMS])))
+        sems_list: list[SEM] = list(self.sem_module().sample(torch.Size([NUM_ATE_ITE_SEMS])))
         interventional_log_prob = eval_intervention_likelihoods(sems_list, interventions)
         self.log("eval/Interventional_LL", torch.mean(interventional_log_prob).item(), add_dataloader_idx=False)
 
         mean_ate_rmse = eval_ate_rmse(sems_list, interventions)
         self.log("eval/ATE_RMSE", list_mean(list(mean_ate_rmse.values())).item(), add_dataloader_idx=False)
 
     def test_step_counterfactuals(self, counterfactuals: CounterfactualWithEffects, *args, **kwargs):
         """Evaluate the ITE performance of the model"""
         _, _ = args, kwargs
         sems_list = list(self.sem_module().sample(torch.Size([NUM_ATE_ITE_SEMS])))
         ite_rmse = eval_ite_rmse(sems_list, counterfactuals)
         self.log("eval/ITE_RMSE", list_mean(list(ite_rmse.values())).item(), add_dataloader_idx=False)
 
-    def on_save_checkpoint(self, checkpoint: Dict[str, Any]) -> None:
+    def on_save_checkpoint(self, checkpoint: dict[str, Any]) -> None:
         checkpoint["sem_module"] = self.sem_module
```

### Comparing `causica-0.2.0/src/causica/lightning/main.py` & `causica-0.3.0/src/causica/lightning/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 
 from causica.lightning.callbacks import MLFlowSaveConfigCallback
 from causica.lightning.cli import LightningCLIWithDefaults
-from causica.lightning.data_modules import VariableSpecDataModule
-from causica.lightning.deci_module import DECIModule
+from causica.lightning.data_modules.deci_data_module import DECIDataModule
+from causica.lightning.modules.deci_module import DECIModule
 
 if __name__ == "__main__":
     # Set Azure logging to warning to prevent spam from HTTP requests
     logging.getLogger("azure").setLevel(logging.WARNING)
 
     cli = LightningCLIWithDefaults(
         DECIModule,
-        VariableSpecDataModule,
+        DECIDataModule,
         run=False,
         save_config_callback=MLFlowSaveConfigCallback,
         subclass_mode_model=True,
         subclass_mode_data=True,
     )
     cli.trainer.fit(cli.model, datamodule=cli.datamodule)
     cli.trainer.test(cli.model, datamodule=cli.datamodule)
```

### Comparing `causica-0.2.0/src/causica/lightning/variable_spec_module.py` & `causica-0.3.0/src/causica/lightning/modules/variable_spec_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,38 +11,37 @@
     """
     An Abstract Base Class for `LightningModule`s that use the VariableSpecDataModule.
 
     This class provides a default implementation of the `test_step` method that
     dispatches to the separate test steps for each dataloader.
     """
 
-    def test_step(self, *args, **kwargs):
+    def test_step(self, batch, batch_idx, dataloader_idx=0):
         """
         Dispatch to the appropriate test step based on the dataloader index.
 
         The dataloader indexing is handled by Lightning and is based on the order
         of the dataloaders in the `test_dataloader` method.
 
         This assumes that the dataloaders are in the following order:
         Test data
         Graph data
         Intervention data
         Counterfactual data
 
         See the superclass for *args and **kwargs conventions.
         """
-        dataloader_idx = args[2]
         if dataloader_idx == 0:
-            return self.test_step_observational(*args, **kwargs)
+            return self.test_step_observational(batch, batch_idx)
         elif dataloader_idx == 1:
-            return self.test_step_graph(*args, **kwargs)
+            return self.test_step_graph(batch, batch_idx)
         elif dataloader_idx == 2:
-            return self.test_step_interventions(*args, **kwargs)
+            return self.test_step_interventions(batch, batch_idx)
         elif dataloader_idx == 3:
-            return self.test_step_counterfactuals(*args, **kwargs)
+            return self.test_step_counterfactuals(batch, batch_idx)
 
     @abc.abstractmethod
     def test_step_observational(self, batch: TensorDict, *args, **kwargs):
         """Test step method for the test data."""
 
     @abc.abstractmethod
     def test_step_graph(self, true_adj_matrix: torch.Tensor, *args, **kwargs):
```

### Comparing `causica-0.2.0/src/causica/mlflow_helpers.py` & `causica-0.3.0/src/causica/mlflow_helpers.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/sem/distribution_parameters_sem.py` & `causica-0.3.0/src/causica/sem/distribution_parameters_sem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Dict
-
 import torch
 from tensordict import TensorDict
 
 from causica.distributions import JointNoiseModule
 from causica.functional_relationships import FunctionalRelationships, create_do_functional_relationship
 from causica.sem.structural_equation_model import SEM
 
@@ -11,15 +9,15 @@
 class DistributionParametersSEM(SEM):
     """
     A Structural Equation Model where the functional forward pass generates the parameters of the distributions to be sampled.
 
     This is more general than the simple additive case.
     """
 
-    arg_constraints: Dict = {}
+    arg_constraints: dict = {}
 
     def __init__(
         self,
         graph: torch.Tensor,
         noise_dist: JointNoiseModule,
         func: FunctionalRelationships,
     ):
```

### Comparing `causica-0.2.0/src/causica/sem/structural_equation_model.py` & `causica-0.3.0/src/causica/sem/structural_equation_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import abc
-from typing import Dict, List, Optional, Sequence
+from typing import Optional, Sequence
 
 import torch
 import torch.distributions as dist
 from tensordict import TensorDict
 
 
 class SEM(dist.Distribution, abc.ABC):
-    arg_constraints: Dict = {}
+    arg_constraints: dict = {}
 
     def __init__(
         self,
         graph: torch.Tensor,
         node_names: Sequence[str],
         event_shape: torch.Size = torch.Size(),
         batch_shape: torch.Size = torch.Size(),
@@ -42,39 +42,36 @@
     @abc.abstractmethod
     def log_prob(self, value: TensorDict) -> torch.Tensor:
         pass
 
     @abc.abstractmethod
     def do(self, interventions: TensorDict) -> "SEM":
         """Return the SEM associated with the interventions"""
-        pass
 
     @abc.abstractmethod
     def noise_to_sample(self, noise: TensorDict) -> TensorDict:
         """
         For a given noise vector, return the corresponding sample values.
 
         Args:
             noise: Dictionary of tensors representing the noise shape sample_shape + batch_shape + noise_shape
         Return:
             Dictionary of samples from the sem corresponding to the noise, shape sample_shape + batch_shape + event_shape
         """
-        pass
 
     @abc.abstractmethod
     def sample_to_noise(self, sample: TensorDict) -> TensorDict:
         """
         For a given sample get the noise vector.
 
         Args:
             sample: samples from the sem each of shape sample_shape + batch_shape + event_shape
         Return:
             Dictionary of tensors representing the noise shape sample_shape + batch_shape + noise_shape
         """
-        pass
 
     @torch.no_grad()
     def sample(self, sample_shape: torch.Size = torch.Size()) -> TensorDict:
         """
         Sample from the SEM
 
         Grads shall not pass through this method (see `Distribution.sample` vs `Distribution.rsample`).
@@ -96,31 +93,30 @@
         Grads shall not pass through implementations of this method.
 
         Args:
             sample_shape: shape of the returned noise samples
         Return:
             Dictionary of samples from the noise distribution for each node, shape sample_shape + batch_shape + event_shape
         """
-        pass
 
 
 def ite(
     sem: SEM,
     factual_data: TensorDict,
     intervention_a: TensorDict,
     intervention_b: TensorDict,
-    effects: Optional[List[str]] = None,
+    effects: Optional[list[str]] = None,
 ) -> TensorDict:
     """Calculate ITE of intervention A and B on some factual data for a list of effects.
 
     Args:
-        factual_data (Dict[str, torch.Tensor]): Factual data to abduct the noise from.
-        intervention_a (Dict[str, torch.Tensor]): Specification of intervention A.
-        intervention_b (Dict[str, torch.Tensor]): Specification of intervention B.
-        effects (Optional[List[str]], optional): List of effect variables. Defaults to None.
+        factual_data: Factual data to abduct the noise from.
+        intervention_a: Specification of intervention A.
+        intervention_b: Specification of intervention B.
+        effects: List of effect variables. Defaults to None.
 
     Returns:
        TensorDict: Dictionary holding the ITEs for the effect variables for all samples.
     """
     if effects is None:
         effects = list(set(sem.node_names) - set(intervention_a.keys()) - set(intervention_b.keys()))
 
@@ -131,39 +127,39 @@
     return {effect: do_a_cfs[effect] - do_b_cfs[effect] for effect in effects}
 
 
 def counterfactual(sem: SEM, factual_data: TensorDict, intervention: TensorDict) -> TensorDict:
     """Calculate Counterfactual of an intervention on some factual data.
 
     Args:
-        factual_data (Dict[str, torch.Tensor]): Factual data to abduct the noise from.
-        intervention (Dict[str, torch.Tensor]): Specification of intervention.
+        factual_data: Factual data to abduct the noise from.
+        intervention: Specification of intervention.
 
     Returns:
        TensorDict: Dictionary holding the counterfactual values for all samples.
     """
     # TODO: do we want to average over multiple "sample_to_noise" values for the discrete variables
     # where this is not a 1:1 mapping?
     return sem.do(interventions=intervention).noise_to_sample(sem.sample_to_noise(factual_data))
 
 
 def ate(
     sem: SEM,
     intervention_a: TensorDict,
     intervention_b: TensorDict,
-    effects: Optional[List[str]] = None,
+    effects: Optional[list[str]] = None,
     num_samples: int = 1000,
 ) -> TensorDict:
     """Calculate the ATE of intervention A and B for a list of effects.
 
     Args:
-        intervention_a (Dict[str, torch.Tensor]): Specification of intervention A.
-        intervention_b (Dict[str, torch.Tensor]): Specification of intervention B.
-        effects (Optional[List[str]], optional): List of effect variables. Defaults to None.
-        num_samples (int, optional): Number of Monte-Carlo samples to estimate the ATE. Defaults to 1000.
+        intervention_a: Specification of intervention A.
+        intervention_b: Specification of intervention B.
+        effects: List of effect variables. Defaults to None.
+        num_samples: Number of Monte-Carlo samples to estimate the ATE. Defaults to 1000.
 
     Returns:
        TensorDict: Dictionary holding the ATEs for the effect variables.
     """
     sample_shape = torch.Size([num_samples])
 
     if effects is None:
```

### Comparing `causica-0.2.0/src/causica/training/auglag.py` & `causica-0.3.0/src/causica/training/auglag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import deque
 from dataclasses import dataclass, field
-from typing import Dict, List, Union
+from typing import Union
 
 import numpy as np
 import torch
 from dataclasses_json import dataclass_json
 from torch.optim import Optimizer
 
 
@@ -19,36 +19,36 @@
 
 @dataclass_json
 @dataclass(frozen=True)
 class AugLagLRConfig:
     """
     Configuration parameters for the AuglagLR scheduler.
 
-    lr_update_lag (int): Number of iterations to wait before updating the learning rate.
-    lr_update_lag_best (int): Number of iterations to wait after the best model before updating the learning rate.
-    lr_init_dict (Dict[str, float]): Dictionary of intitialization parameters for every new inner optimization step.
+    lr_update_lag: Number of iterations to wait before updating the learning rate.
+    lr_update_lag_best: Number of iterations to wait after the best model before updating the learning rate.
+    lr_init_dict: Dictionary of intitialization parameters for every new inner optimization step.
         This must contain all parameter_groups for all optimizers
-    aggregation_period (int): Aggregation period to compare the mean of the loss terms across this period.
-    lr_factor (float): Learning rate update schedule factor (exponential decay).
-    penalty_progress_rate (float): Number of iterations to wait before updating rho based on the dag penalty.
-    safety_rho (float): Maximum rho that could be updated to.
-    safety_alpha (float): Maximum alpha that could be udated to.
-    max_lr_down (int): Maximum number of lr update times to decide inner loop termination.
-    inner_early_stopping_patience (int): Maximum number of iterations to run after the best inner loss to terminate inner loop.
-    max_outer_steps (int): Maximum number of outer update steps.
-    patience_penalty_reached (int): Maximum number of outer iterations to run after the dag penalty has reached a good value.
-    patience_max_rho (int): Maximum number of iterations to run once rho threshold is reached.
-    penalty_tolerance (float): Tolerance of the dag penalty
-    max_inner_steps (int): Maximum number of inner loop steps to run.
+    aggregation_period: Aggregation period to compare the mean of the loss terms across this period.
+    lr_factor: Learning rate update schedule factor (exponential decay).
+    penalty_progress_rate: Number of iterations to wait before updating rho based on the dag penalty.
+    safety_rho: Maximum rho that could be updated to.
+    safety_alpha: Maximum alpha that could be udated to.
+    max_lr_down: Maximum number of lr update times to decide inner loop termination.
+    inner_early_stopping_patience: Maximum number of iterations to run after the best inner loss to terminate inner loop.
+    max_outer_steps: Maximum number of outer update steps.
+    patience_penalty_reached: Maximum number of outer iterations to run after the dag penalty has reached a good value.
+    patience_max_rho: Maximum number of iterations to run once rho threshold is reached.
+    penalty_tolerance: Tolerance of the dag penalty
+    max_inner_steps: Maximum number of inner loop steps to run.
 
     """
 
     lr_update_lag: int = 500
     lr_update_lag_best: int = 250
-    lr_init_dict: Dict[str, float] = field(
+    lr_init_dict: dict[str, float] = field(
         default_factory=lambda: {"vardist": 0.1, "icgnn": 0.0003, "noise_dist": 0.003}
     )
     aggregation_period: int = 20
     lr_factor: float = 0.1
     penalty_progress_rate: float = 0.65
     safety_rho: float = 1e13
     safety_alpha: float = 1e13
@@ -135,36 +135,36 @@
 
         Returns:
             bool: Returns True if last iteration at which learning rate was
             updated and last best loss iteration is less than total steps, else False.
         """
         return self.last_best_step + self.config.lr_update_lag_best <= self.step_counter
 
-    def _update_lr(self, optimizer: Union[Optimizer, List[Optimizer]]):
+    def _update_lr(self, optimizer: Union[Optimizer, list[Optimizer]]):
         """Update the learning rate of the optimizer(s) based on the lr multiplicative factor.
 
         Args:
-            optimizer (Union[Optimizer, List[Optimizer]]): Optimizers of auglag to be updated.
+            optimizer: Optimizers of auglag to be updated.
         """
         self.last_lr_update_step = self.step_counter
         self.num_lr_updates += 1
 
         if isinstance(optimizer, list):
             for opt in optimizer:
                 for param_group in opt.param_groups:
                     param_group["lr"] *= self.config.lr_factor
         else:
             for param_group in optimizer.param_groups:
                 param_group["lr"] *= self.config.lr_factor
 
-    def _reset_lr(self, optimizer: Union[Optimizer, List[Optimizer]]):
+    def _reset_lr(self, optimizer: Union[Optimizer, list[Optimizer]]):
         """Reset the learning rate of individual param groups from lr init dictionary.
 
         Args:
-            optimizer (Union[Optimizer, List[Optimizer]]): Optimizer(s) corresponding to all param groups.
+            optimizer: Optimizer(s) corresponding to all param groups.
         """
         self.last_lr_update_step = self.step_counter
 
         if isinstance(optimizer, list):
             for opt in optimizer:
                 for param_group in opt.param_groups:
                     param_group["lr"] = self.config.lr_init_dict[param_group["name"]]
@@ -173,15 +173,15 @@
             for param_group in optimizer.param_groups:
                 param_group["lr"] = self.config.lr_init_dict[param_group["name"]]
 
     def _update_lagrangian_params(self, loss: AugLagLossCalculator):
         """Update the lagrangian parameters (of the auglag routine) based on the dag constraint values observed.
 
         Args:
-            loss (AugLagLoss): loss with lagrangian attributes rho and alpha to be updated.
+            loss: loss with lagrangian attributes rho and alpha to be updated.
         """
         if self._cur_dag_penalty < self.config.penalty_tolerance:
             self.outer_below_penalty_tol += 1
         else:
             self.outer_below_penalty_tol = 0
 
         if loss.rho > self.config.safety_rho:
@@ -198,21 +198,21 @@
             print(f"Updating alpha to: {loss.alpha}")
         if loss.rho >= self.config.safety_rho:
             loss.alpha *= 5
 
         loss.rho = min([loss.rho, self.config.safety_rho])
         loss.alpha = min([loss.alpha, self.config.safety_alpha])
 
-    def _is_auglag_converged(self, optimizer: Union[Optimizer, List[Optimizer]], loss: AugLagLossCalculator) -> bool:
+    def _is_auglag_converged(self, optimizer: Union[Optimizer, list[Optimizer]], loss: AugLagLossCalculator) -> bool:
         """Checks if the inner and outer loops have converged. If inner loop is converged,
         it initilaizes the optimisation parameters for a new inner loop. If both are converged, it returns True.
 
         Args:
-            optimizer (Union[Optimizer, List[Optimizer]]): Optimizer(s) corresponding to different parameter groups on which auglag is being performed.
-            loss (AugLagLoss): Auglag loss.
+            optimizer: Optimizer(s) corresponding to different parameter groups on which auglag is being performed.
+            loss: Auglag loss.
 
         Returns:
             bool: Returns True if both inner and outer have converged, else False
         """
         if self._is_inner_converged():
             if self._is_outer_converged():
                 return True
@@ -232,26 +232,26 @@
             avg_loss = np.mean(self.loss_tracker)
             if avg_loss < self.best_loss:
                 self.best_loss = avg_loss
                 self.last_best_step = self.step_counter
 
     def step(
         self,
-        optimizer: Union[Optimizer, List[Optimizer]],
+        optimizer: Union[Optimizer, list[Optimizer]],
         loss: AugLagLossCalculator,
         loss_value: float,
         lagrangian_penalty: float,
     ) -> bool:
         """The main update method to take one auglag inner step.
 
         Args:
-            optimizer (Union[Optimizer, List[Optimizer]]): Optimizer(s) corresponding to different param groups.
-            loss (AugLagLoss): auglag loss with lagrangian parameters
-            loss_value (float): the actual value of the elbo for the current update step.
-            lagrangian_penalty (float): Dag penalty for the current update step.
+            optimizer: Optimizer(s) corresponding to different param groups.
+            loss: auglag loss with lagrangian parameters
+            loss_value: the actual value of the elbo for the current update step.
+            lagrangian_penalty: Dag penalty for the current update step.
 
         Returns:
             bool: if the auglag has converged (False) or not (True)
         """
         assert lagrangian_penalty >= 0, "auglag penalty must be non-negative"
         self.loss_tracker.append(loss_value)
         self._cur_dag_penalty = lagrangian_penalty
```

### Comparing `causica-0.2.0/src/causica/training/evaluation.py` & `causica-0.3.0/src/causica/training/per_variable_metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,140 +1,93 @@
-import math
-from collections import defaultdict
-from typing import Dict, Iterable, List, Tuple, Union
+from typing import Iterable, Optional, Union
 
 import torch
 from tensordict import TensorDict
 
-from causica.datasets.causica_dataset_format import CounterfactualWithEffects, InterventionWithEffects
+from causica.datasets.causica_dataset_format import CounterfactualWithEffects
+from causica.distributions.transforms import JointTransform
 from causica.sem.distribution_parameters_sem import DistributionParametersSEM
-from causica.sem.structural_equation_model import SEM, ate, ite
+from causica.sem.structural_equation_model import SEM, counterfactual
 
 
-def eval_intervention_likelihoods(sems: List[SEM], intervention_with_effects: InterventionWithEffects) -> torch.Tensor:
-    """
-    Calculate the average log-prob of interventional data.
-
-    Specifically we calculate 𝔼_sample[log(𝔼_G[p(sample | G)])]
-
-    Args:
-        sems: An iterable of SEMS to evaluate the interventional log prob of
-        interventions: True interventional data to use for evaluation.
-
-    Returns:
-        Log-likelihood of the interventional data for each interventional datapoint
-    """
-    total_log_sum_exp_per_int = []  # this will end up being length number of interventions
-    for intervention in intervention_with_effects[:2]:
-        inner_log_probs = [
-            sem.do(interventions=intervention.intervention_values).log_prob(intervention.intervention_data)
-            for sem in sems
-        ]
-        # calculate log(𝔼_G[p(sample | G)]) for each sample
-        log_prob = list_logsumexp(inner_log_probs) - math.log(len(sems))  # batch_size
-        assert len(log_prob.shape) == 1
-        total_log_sum_exp_per_int.append(log_prob)
-
-    # log(𝔼_G[p(sample | G)]) for each sample in both interventions, shape 2 * batch_size
-    return torch.cat(total_log_sum_exp_per_int, dim=-1)
-
-
-def eval_ate_rmse(
-    sems: Iterable[SEM], intervention: InterventionWithEffects, samples_per_graph: int = 1000
+def eval_counterfactual_outcome_per_variable_rmse(
+    sems: Iterable[SEM],
+    counterfactual_data: CounterfactualWithEffects,
+    grouped_variable_names: Optional[dict[str, list[str]]] = None,
+    standardizer: Optional[JointTransform] = None,
 ) -> TensorDict:
-    """Evaluate the ATEs of a model
-
-    Args:
-        sems: An iterable of structural equation models to evaluate the ATE RMSE of
-        intervention: True interventional data to use for evaluation.
-        samples_per_graph: Number of samples to draw per graph to calculate the ATE.
-
-    Returns:
-        Dict of the RMSE of the ATE for each node we're interested in
-    """
-
-    intervention_a, intervention_b, effects = intervention
-
-    # each node has shape [batch_size, node_dim]
-    true_ates = {
-        effect: intervention_a.intervention_data[effect].mean() - intervention_b.intervention_data[effect].mean()
-        for effect in effects
-    }
-
-    # generate samples from the intervened distribution and the base distribution
-    ates_per_graph: Dict[str, List[torch.Tensor]] = defaultdict(list)
-    for sem in sems:
-        graph_ates = ate(
-            sem, intervention_a.intervention_values, intervention_b.intervention_values, effects, samples_per_graph
-        )
-        for key in effects:
-            ates_per_graph[key].append(graph_ates[key].detach())
-
-    # each node has shape [node_dim]
-    generated_ates = {k: list_mean(v) for k, v in ates_per_graph.items()}
-    return TensorDict(
-        {key: torch.sqrt(torch.mean(torch.sum((generated_ates[key] - true_ates[key]) ** 2, -1))) for key in effects},
-        batch_size=torch.Size([]),
-    )
-
-
-def eval_ite_rmse(sems: Iterable[SEM], counterfactual: CounterfactualWithEffects) -> TensorDict:
-    """Evaluate the ITEs of a model.
+    """Evaluate the counterfacual rmses of a model.
 
     Args:
         sems: An iterable of structural equation models to evaluate the ITE RMSE of
-        counterfactual: Data of true counterfactuals to use for evaluation.
+        counterfactual_data: Data of true counterfactuals to use for evaluation.
+        grouped_variable_names: Optional dictionary that holds the names of the variables in each group. If given,
+            the variables are evaluated individually. Otherwise, the variables are evaluated groupwise.
+        standardizer: Standardizer that is used to invert the predictions and loaded data to convery the metrics into
+            the space of the original data.
 
     Returns:
         Dict of RMSEs for each effect variable we're interested in
     """
-    intervention_a, intervention_b, effects = counterfactual
-    for key, a_val in intervention_a.factual_data.items():
-        b_val = intervention_b.factual_data[key]
-        assert torch.allclose(a_val, b_val), "Base data must be the same for ITEs"
-    # each node has shape [batch_size, node_dim]
-    true_ites = {
-        effect: intervention_a.counterfactual_data[effect] - intervention_b.counterfactual_data[effect]
-        for effect in effects
-    }
+    intervention, _, effects = counterfactual_data
 
     # generate samples from the intervened distribution and the base distribution
-    per_graph_ites: Dict[str, List[torch.Tensor]] = defaultdict(list)
-    for sem in sems:
-        sem_ites = ite(
-            sem,
-            intervention_a.factual_data,
-            intervention_a.intervention_values,
-            intervention_b.intervention_values,
-            effects,
-        )
+    stacked: TensorDict = torch.stack(
+        [counterfactual(sem, intervention.factual_data, intervention.intervention_values) for sem in sems]
+    )
+    generated_cf_outcomes = stacked.apply(
+        lambda v: v.mean(axis=0), batch_size=intervention.factual_data.batch_size, inplace=False
+    )
+    true_counterfactual_outcome = intervention.counterfactual_data
 
-        for key in effects:
-            per_graph_ites[key].append(sem_ites[key].detach())
+    if standardizer is not None:
+        generated_cf_outcomes = standardizer.inv(generated_cf_outcomes)
+        true_counterfactual_outcome = standardizer.inv(true_counterfactual_outcome)
+
+    if grouped_variable_names is None:
+        # calculate the rmse metrics, one for each group
+        rmses = TensorDict(
+            {key: rmse(generated_cf_outcomes[key], true_counterfactual_outcome[key]) for key in effects},
+            batch_size=torch.Size(),
+        )
+    else:
+        # calculate the rmse metrics, one for each column/single variable
+        rmses = TensorDict(
+            {
+                col_name: rmse(generated_cf_outcomes[key][:, idx], true_counterfactual_outcome[key][:, idx])
+                for key in effects
+                for idx, col_name in enumerate(grouped_variable_names[key])
+            },
+            batch_size=torch.Size(),
+        )
 
-    # average the treatment value over all graphs, each node has shape [batch_size, node_dim]
-    generated_ites = {k: list_mean(v) for k, v in per_graph_ites.items()}
-    return TensorDict(
-        {key: torch.sqrt(torch.mean(torch.sum((generated_ites[key] - true_ites[key]) ** 2, -1))) for key in effects},
-        batch_size=torch.Size(),
-    )
+    return rmses
 
 
 def eval_observational_per_variable_rmse_and_accuracy(
-    sems: Union[List[DistributionParametersSEM], Tuple[DistributionParametersSEM]],
+    sems: Union[list[DistributionParametersSEM], tuple[DistributionParametersSEM]],
     observations: TensorDict,
-    continuous_variables: List[str],  # keys to variables to be interpreted as categorical
-    binary_variables: List[str],  # keys to variables to be interpreted as binary
-    categorical_variables: List[str],  # keys to variables to be interpreted as categorical
-) -> Dict[str, torch.Tensor]:
+    continuous_variables: list[str],  # keys to variables to be interpreted as categorical
+    binary_variables: list[str],  # keys to variables to be interpreted as binary
+    categorical_variables: list[str],  # keys to variables to be interpreted as categorical
+    grouped_variable_names: Optional[dict[str, list[str]]] = None,
+    standardizer: Optional[JointTransform] = None,
+) -> tuple[dict[str, torch.Tensor], dict[str, torch.Tensor]]:
     """Calculates the RMSE and accuracy of the predictions of a model.
 
     Args:
         sems: An iterable of structural equation models to evaluate the ITE RMSE of
         observations: Observational data to evaluate
+        continuous_variables: Keys of the continuous variables
+        binary_variables: Keys of the binary variables
+        categorical_variables: Keys of the categorical variables
+        grouped_variable_names: Optional dictionary that holds the names of the variables in each group. If given,
+            the variables are evaluated individually. Otherwise, the variables are evaluated groupwise.
+        standardizer: Standardizer that is used to invert the predictions and loaded data to convery the metrics into
+            the space of the original data.
 
     Returns:
         Dict holding the accuracy metrics for each node
     """
     assert all(
         set(sem.node_names) == set(observations.keys()) for sem in sems
     ), f"observations must be compatible with SEMs: got {set(observations.keys())} but expected {set(list(sems)[0].node_names)}"
@@ -149,27 +102,54 @@
         set(categorical_variables)
     ), f"continuous and categorical variables must be disjoint: got {set(continuous_variables).intersection(set(categorical_variables))}"
     assert set(binary_variables).isdisjoint(
         set(categorical_variables)
     ), f"binary and categorical variables must be disjoint: got {set(binary_variables).intersection(set(categorical_variables))}"
 
     stacked: TensorDict = torch.stack([sem.func(observations, sem.graph) for sem in sems])
-    mean_predictions = stacked.apply(lambda v: v.mean(axis=0), batch_size=(len(sems),), inplace=False)
-
-    metrics = {}
-    for var in continuous_variables:
-        metrics[f"rmse_{var}"] = rmse(mean_predictions.get(var), observations.get(var))
-
-    for var in binary_variables:
-        metrics[f"accuracy_{var}"] = binary_accuracy(mean_predictions.get(var), observations.get(var))
+    mean_predictions = stacked.apply(lambda v: v.mean(axis=0), batch_size=observations.batch_size, inplace=False)
 
-    for var in categorical_variables:
-        metrics[f"accuracy_{var}"] = categorical_accuracy(mean_predictions.get(var), observations.get(var))
+    if standardizer is not None:
+        mean_predictions = standardizer.inv(mean_predictions)
+        observations = standardizer.inv(observations)
+
+    rmses = {}
+    accuraccies = {}
+    if grouped_variable_names is None:
+        # Calculate metrics for each group
+        for var in continuous_variables:
+            rmses[f"{var}"] = rmse(mean_predictions.get(var), observations.get(var))
+
+        for var in binary_variables:
+            accuraccies[f"{var}"] = binary_accuracy(mean_predictions.get(var), observations.get(var))
+
+        for var in categorical_variables:
+            accuraccies[f"{var}"] = categorical_accuracy(mean_predictions.get(var), observations.get(var))
+    else:
+        # Calculate metrics for each variable in each group
+        for group_name in continuous_variables:
+            for i, var in enumerate(grouped_variable_names[group_name]):
+                rmses[f"{var}"] = rmse(
+                    mean_predictions.get(group_name)[:, i][:, None], observations.get(group_name)[:, i][:, None]
+                )
+
+        for group_name in binary_variables:
+            for i, var in enumerate(grouped_variable_names[group_name]):
+                accuraccies[f"{var}"] = binary_accuracy(
+                    mean_predictions.get(group_name)[:, i], observations.get(group_name)[:, i]
+                )
+
+        # Categorical variables are one-hot encoded, so we need to calculate the accuracy for each group as we do not
+        # support grouped categorical variables of shape [batch_size, num_groups, num_dims_for_node]
+        for group_name in categorical_variables:
+            accuraccies[f"{group_name}"] = categorical_accuracy(
+                mean_predictions.get(group_name), observations.get(group_name)
+            )
 
-    return metrics
+    return rmses, accuraccies
 
 
 def binary_accuracy(logits: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
     """Calculate the accuracy of a prediction for a binary variable.
 
     Args:
         logits: Tensor of logits [batch_size] or [batch_size, num_dims_for_node]
@@ -207,17 +187,7 @@
         prediction: Tensor of predictions [batch_size, num_dims_for_node]
         target: Tensor of targets [batch_size, num_dims_for_node]
 
     Returns:
         RMSE of the prediction
     """
     return torch.sqrt(torch.mean(torch.sum((prediction - target) ** 2, -1)))
-
-
-def list_mean(list_of_tensors: List[torch.Tensor]) -> torch.Tensor:
-    """Take the mean of a list of torch tensors, they must all have the same shape"""
-    return torch.stack(list_of_tensors, dim=0).mean(dim=0)
-
-
-def list_logsumexp(list_of_tensors: List[torch.Tensor]) -> torch.Tensor:
-    """Take the logsumexp of a list of torch tensors, they must all have the same shape"""
-    return torch.logsumexp(torch.stack(list_of_tensors, dim=0), dim=0)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `causica-0.2.0/src/causica/training/training_callbacks.py` & `causica-0.3.0/src/causica/training/training_callbacks.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/src/causica/triangular_transformations.py` & `causica-0.3.0/src/causica/triangular_transformations.py`

 * *Files identical despite different names*

### Comparing `causica-0.2.0/PKG-INFO` & `causica-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: causica
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: MIT
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: azureml-mlflow (>=1.46.0,<2.0.0)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
+Requires-Dist: jsonargparse (<=4.20.0)
 Requires-Dist: mlflow (>=2.0.0,<3.0.0)
+Requires-Dist: numba (>=0.56.0,<0.57.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
-Requires-Dist: pytorch-lightning[extra] (>=1.7.7,<2.0.0)
+Requires-Dist: pytorch-lightning[extra] (>=2.0.0,<3.0.0)
 Requires-Dist: tensorboard (>=2.9.0,<3.0.0)
 Requires-Dist: tensordict (>=0.1.0,<0.2.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: types-PyYAML (>=6.0.12.2,<7.0.0.0)
 Description-Content-Type: text/markdown
 
 [![Causica CI Build](https://github.com/microsoft/causica/actions/workflows/ci-build.yml/badge.svg)](https://github.com/microsoft/causica/actions/workflows/ci-build.yml)
@@ -58,15 +60,17 @@
 
 **Simulation-based Causal Inference**
 
 DECI estimates causal quantities (ATE) by applying the relevant interventions to its learnt causal graph (i.e. mutilating incoming edges to intervened variables) and then sampling from the generative model. This process involves first sampling a vector of exogenous noise from the learnt noise distribution and then forward simulating the SEM until an observation vector is obtained. ATE can be computed via estimating an expectation over the effect variable of interest using MonteCarlo samples of the intervened distribution of observations. 
 
 ## How to run
 
-See the notebook `examples/csuite_example.ipynb`, for how to train a DECI model and check the causal discovery.
+The best place to start is the `examples/multi_investment_sales_attribution.ipynb` notebook. This explains how to fit a model using PyTorch Lightning and test ATE and ITE results.
+
+For a more detailed introduction to the components and how they fit together, see the notebook `examples/csuite_example.ipynb`, for how to train a DECI model and check the causal discovery.
 
 This will download the data from the CSuite Azure blob storage and train DECI on it. See [here](https://github.com/microsoft/csuite) for more info about CSuite datasets. The notebook will work on any of the available CSuite datasets.
 
 
 **Specifying a noise model**
 
 The noise exogenous model can be modified by changing the `noise_dist` field within `TrainingConfig`, either Gaussian or Spline are allowed.
@@ -91,18 +95,14 @@
 
 [2], **(DECI)** Tomas Geffner, Javier Antoran, Adam Foster, Wenbo Gong, Chao Ma, Emre Kiciman, Amit Sharma, Angus Lamb, Martin Kukla, Nick Pawlowski, Miltiadis Allamanis, Cheng Zhang. Deep End-to-end Causal Inference. [Arxiv preprint](https://arxiv.org/abs/2202.02195) (2022)
 
 [3], **(DDECI)** Matthew Ashman, Chao Ma, Agrin Hilmkil, Joel Jennings, Cheng Zhang. Causal Reasoning in the Presence of Latent Confounders via Neural ADMG Learning. [ICLR](https://openreview.net/forum?id=dcN0CaXQhT) (2023)
 
 [4], **(Rhino)** Wenbo Gong, Joel Jennings, Cheng Zhang, Nick Pawlowski. Rhino: Deep Causal Temporal Relationship Learning with History-dependent Noise. [ICLR](https://openreview.net/forum?id=i_1rbq8yFWC) (2023)
 
-Other references:
-- Louizos, Christos, et al. "Causal effect inference with deep latent-variable models." Advances in neural information processing systems 30 (2017).
-- Hill, Jennifer L. "Bayesian nonparametric modeling for causal inference." Journal of Computational and Graphical Statistics 20.1 (2011): 217-240.
-
 
 # Development
 
 ## Poetry
 
 We use Poetry to manage the project dependencies, they're specified in the [pyproject.toml](pyproject.toml). To install poetry run:
```


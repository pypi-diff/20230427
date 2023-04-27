# Comparing `tmp/sygnet-0.0.8.tar.gz` & `tmp/sygnet-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sygnet-0.0.8.tar", last modified: Sat Jul  2 17:53:31 2022, max compression
+gzip compressed data, was "sygnet-0.0.9.tar", last modified: Wed Apr 26 15:48:43 2023, max compression
```

## Comparing `sygnet-0.0.8.tar` & `sygnet-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,29 @@
--rw-r--r--   0        0        0      562 2022-07-02 17:53:27.192129 sygnet-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1470 2022-07-02 17:53:27.192129 sygnet-0.0.8/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      100 2022-07-02 17:53:27.192129 sygnet-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2022-07-02 17:53:27.192129 sygnet-0.0.8/LICENSE
--rw-r--r--   0        0        0     2234 2022-07-02 17:53:27.192129 sygnet-0.0.8/README.md
--rw-r--r--   0        0        0  7542748 2022-07-02 17:53:27.244129 sygnet-0.0.8/data/simulation_data_1.csv
--rw-r--r--   0        0        0   560910 2022-07-02 17:53:27.248129 sygnet-0.0.8/data/sygnet_model_30Jun22_1058
--rw-r--r--   0        0        0    20883 2022-07-02 17:53:27.276128 sygnet-0.0.8/examples/basic_example.ipynb
--rw-r--r--   0        0        0     1241 2022-07-02 17:53:27.276128 sygnet-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       67 2022-07-02 17:53:27.276128 sygnet-0.0.8/src/sygnet/__init__.py
--rw-r--r--   0        0        0     5720 2022-07-02 17:53:27.280128 sygnet-0.0.8/src/sygnet/dataloaders.py
--rw-r--r--   0        0        0    19007 2022-07-02 17:53:27.280128 sygnet-0.0.8/src/sygnet/interface.py
--rw-r--r--   0        0        0      533 2022-07-02 17:53:27.280128 sygnet-0.0.8/src/sygnet/loader.py
--rw-r--r--   0        0        0    13199 2022-07-02 17:53:27.280128 sygnet-0.0.8/src/sygnet/models.py
--rw-r--r--   0        0        0      351 2022-07-02 17:53:27.280128 sygnet-0.0.8/src/sygnet/requirements.py
--rw-r--r--   0        0        0    13528 2022-07-02 17:53:27.280128 sygnet-0.0.8/src/sygnet/train.py
--rw-r--r--   0        0        0     5375 2022-07-02 17:53:27.280128 sygnet-0.0.8/src/sygnet/tune.py
--rw-r--r--   0        0        0  1052220 2022-07-02 17:53:27.284129 sygnet-0.0.8/sygnet.png
--rw-r--r--   0        0        0   590639 2022-07-02 17:53:27.292128 sygnet-0.0.8/sygnet1280.png
--rw-r--r--   0        0        0        0 2022-07-02 17:53:27.292128 sygnet-0.0.8/test/__init__.py
--rw-r--r--   0        0        0     2885 2022-07-02 17:53:27.292128 sygnet-0.0.8/test/test_mixed_act.py
--rw-r--r--   0        0        0     1091 2022-07-02 17:53:27.292128 sygnet-0.0.8/test/test_pipeline.py
--rw-r--r--   0        0        0     7649 2022-07-02 17:53:27.292128 sygnet-0.0.8/test/test_sampler.py
--rw-r--r--   0        0        0     1331 2022-07-02 17:53:27.292128 sygnet-0.0.8/test/test_saver.py
--rw-r--r--   0        0        0     1588 2022-07-02 17:53:27.292128 sygnet-0.0.8/test/test_tuner.py
--rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 sygnet-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      562 2023-04-21 14:49:14.426274 sygnet-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1470 2023-04-21 14:49:14.427765 sygnet-0.0.9/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      110 2023-04-26 13:59:04.553854 sygnet-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2023-04-21 14:49:14.431180 sygnet-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2438 2023-04-26 13:59:04.554355 sygnet-0.0.9/README.md
+-rw-r--r--   0        0        0  7542748 2023-04-21 14:49:14.493609 sygnet-0.0.9/data/simulation_data_1.csv
+-rw-r--r--   0        0        0   560910 2023-04-21 14:49:14.506101 sygnet-0.0.9/data/sygnet_model_30Jun22_1058
+-rw-r--r--   0        0        0    20883 2023-04-21 14:49:14.577499 sygnet-0.0.9/examples/basic_example.ipynb
+-rw-r--r--   0        0        0     1241 2023-04-26 13:59:04.555601 sygnet-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-26 13:59:04.556668 sygnet-0.0.9/src/.DS_Store
+-rw-r--r--   0        0        0       66 2023-04-21 14:49:14.584350 sygnet-0.0.9/src/sygnet/__init__.py
+-rw-r--r--   0        0        0     2381 2023-04-26 13:59:04.564459 sygnet-0.0.9/src/sygnet/blocks.py
+-rw-r--r--   0        0        0     5368 2023-04-26 13:59:04.565051 sygnet-0.0.9/src/sygnet/dataloaders.py
+-rw-r--r--   0        0        0     7460 2023-04-21 14:49:34.815258 sygnet-0.0.9/src/sygnet/experimental.py
+-rw-r--r--   0        0        0    19092 2023-04-26 13:59:04.565648 sygnet-0.0.9/src/sygnet/interface.py
+-rw-r--r--   0        0        0      533 2023-04-21 14:49:14.640416 sygnet-0.0.9/src/sygnet/loader.py
+-rw-r--r--   0        0        0     8900 2023-04-26 13:59:04.566133 sygnet-0.0.9/src/sygnet/models.py
+-rw-r--r--   0        0        0      351 2023-04-21 14:49:14.642346 sygnet-0.0.9/src/sygnet/requirements.py
+-rw-r--r--   0        0        0    12407 2023-04-26 13:59:04.566614 sygnet-0.0.9/src/sygnet/train.py
+-rw-r--r--   0        0        0     5834 2023-04-21 14:49:14.645675 sygnet-0.0.9/src/sygnet/tune.py
+-rw-r--r--   0        0        0  1052220 2023-04-21 14:49:14.654663 sygnet-0.0.9/sygnet.png
+-rw-r--r--   0        0        0   590639 2023-04-21 14:49:14.661351 sygnet-0.0.9/sygnet1280.png
+-rw-r--r--   0        0        0        0 2023-04-21 14:49:14.661463 sygnet-0.0.9/test/__init__.py
+-rw-r--r--   0        0        0     3064 2023-04-26 13:59:04.573367 sygnet-0.0.9/test/test_mixed_act.py
+-rw-r--r--   0        0        0      800 2023-04-26 13:59:04.575412 sygnet-0.0.9/test/test_pipeline.py
+-rw-r--r--   0        0        0     7649 2023-04-26 12:12:08.242699 sygnet-0.0.9/test/test_sampler.py
+-rw-r--r--   0        0        0     1327 2023-04-26 13:59:04.580808 sygnet-0.0.9/test/test_saver.py
+-rw-r--r--   0        0        0     1588 2023-04-25 14:26:34.667143 sygnet-0.0.9/test/test_tuner.py
+-rw-r--r--   0        0        0     3552 1970-01-01 00:00:00.000000 sygnet-0.0.9/PKG-INFO
```

### Comparing `sygnet-0.0.8/.github/workflows/publish.yml` & `sygnet-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sygnet-0.0.8/.github/workflows/python-app.yml` & `sygnet-0.0.9/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `sygnet-0.0.8/LICENSE` & `sygnet-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sygnet-0.0.8/README.md` & `sygnet-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,44 +4,54 @@
 
 *Principal Investigator: Dr Thomas Robinson (thomas.robinson@durham.ac.uk)*
 
 *Research team: Artem Nesterov, Maksim Zubok*
 
 ![example workflow](https://github.com/tsrobinson/SyGNet/actions/workflows/python-app.yml/badge.svg)
 
-**sygnet** is a Python package for generating synthetic data within social science contexts. The **sygnet** algorithm uses cutting-edge advances in deep learning methods to learn the underlying relationships between variables in a dataset. Users can then generate brand-new, synthetic observations that mimic the real data.
+**sygnet** ("sig·net") is a Python package for generating 
+synthetic data within 
+social science contexts. The **sygnet** algorithm uses cutting-edge advances in deep learning methods to learn the underlying relationships between variables in a dataset. Users can then generate brand-new, synthetic observations that mimic the real data.
 
 ### Installation
 To install via pip, you can run the following command at the command line:
 `pip install sygnet`
 
 **sygnet** requires:
     
-    numpy>=1.20
+    numpy>=1.21
     torch>=1.10.0
     scikit-learn>=1.0
     pandas>=1.4
     datetime
     tqdm
 
 ### Example implementation
 
 You can find a demonstration of **sygnet** under [examples/basic_example](examples/basic_example.ipynb).
 
-### Current version: 0.0.8 (alpha release)
+### Current version: 0.0.9 (alpha release)
 
-**Alpha release**: You should expect both functionality and pipelines to change (rapidly). Comments and bug reports are very welcome!
+**Alpha release**: You should expect both functionality and pipelines to change (rapidly and without warning). Comments and bug reports are very welcome!
 
 Changes:
 
-* Update `tune()` to provide no k-fold cross validation as default
-* Update numpy dependency to fix pre-processing bug
+* Rewrite of main interface and underlying functions
+* Bulding models now structured in terms of hidden "blocks"
+* Added self-attention mechanism
 
 ### Previous releases
 
+**0.0.8**
+
+Changes:
+
+* Update `tune()` to provide no k-fold cross validation as default
+* Update numpy dependency to fix pre-processing bug
+
 **0.0.7**
 * Update internal `train_*` functions to return losses and improve logging
 * Update `tune()` function
 
 **0.0.6 and 0.0.5**
 * Internal changes to improve code efficiency
 * Removes `sygnet_` from all submodule names
@@ -58,8 +68,8 @@
 * Updates example
 
 **0.0.2**
 * Fixes mixed activation bug where final layer wasn't sent to `device`
 * Adds `SygnetModel.transform()` alias for `SygnetModel.sample()`
 
 **0.0.1**
-Our first release! This version has been lightly tested and the core functionality has been implemented. 
+Our first release! This version has been lightly tested and the core functionality has been implemented.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sygnet-0.0.8/data/simulation_data_1.csv` & `sygnet-0.0.9/data/simulation_data_1.csv`

 * *Files identical despite different names*

### Comparing `sygnet-0.0.8/data/sygnet_model_30Jun22_1058` & `sygnet-0.0.9/data/sygnet_model_30Jun22_1058`

 * *Files identical despite different names*

### Comparing `sygnet-0.0.8/examples/basic_example.ipynb` & `sygnet-0.0.9/examples/basic_example.ipynb`

 * *Files identical despite different names*

### Comparing `sygnet-0.0.8/pyproject.toml` & `sygnet-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 maintainers = [
     {name = "Thomas Robinson", email = "thomas.robinson@durham.ac.uk"},
     {name = "Artem Nesterov"},
     {name = "Maksim Zubok"},
 ]
 
-version = "0.0.8"
+version = "0.0.9"
 description = "Synthetic data using Generative Adversarial Networks"
 keywords = [
     "synthetic data", 
     "neural networks", 
     "GAN",
     "torch",
 ]
@@ -30,15 +30,15 @@
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
     "numpy>=1.21",
     "torch>=1.10.0",
-    "scikit-learn>=1.0",
+    "scikit-learn>=1.2",
     "pandas>=1.4",
     "datetime",
     "tqdm",
 ]
 
 [project.optional-dependencies]
 viz = [
```

### Comparing `sygnet-0.0.8/src/sygnet/dataloaders.py` & `sygnet-0.0.9/src/sygnet/dataloaders.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .requirements import *
-from sklearn.preprocessing import OneHotEncoder
+from sklearn.preprocessing import OneHotEncoder, MinMaxScaler
 
 logger = logging.getLogger(__name__)
 
 class GeneratedData(Dataset):
     """Formats processed data for GAN training, optionally using the conditional infrastructure
 
     Args:
@@ -36,112 +36,100 @@
         if conditional:
 
             # Separate data
             cond_labels = data_in.loc[:,cond_cols]
             data_in.drop(cond_cols, axis = 1, inplace = True)
             
             # Process latent data
-            self.x, self.x_indxs, self.x_funcs, self.x_OHE, self.colnames = _preprocess_df(data_in)
+            self.x, self.x_indxs, self.x_funcs, self.x_transformers, self.colnames = _preprocess_df(data_in)
             self.x = torch.from_numpy(self.x)
 
             # Process conditional labels (no need to save funcs as won't be fed to activation)
-            self.labels,_,_,self.labels_OHE, label_names = _preprocess_df(cond_labels)
+            self.labels,_,_,self.labels_transformers, label_names = _preprocess_df(cond_labels)
             self.labels = torch.from_numpy(self.labels)
             self.colnames += label_names
 
         else:
-            self.x, self.x_indxs, self.x_funcs, self.x_OHE, self.colnames = _preprocess_df(data_in)
+            self.x, self.x_indxs, self.x_funcs, self.x_transformers, self.colnames = _preprocess_df(data_in)
             self.x = torch.from_numpy(self.x)
             self.labels = torch.ones(self.n_samples, 1)
         
     def __getitem__(self, index):
         return self.x[index], self.labels[index]
 
     def __len__(self):
         return self.n_samples
 
 
 def _preprocess_df(df):
     '''
     Sort and arrange columns for managing mixed activation
-
     Args:
         df(pd.Dataframe): The input data
-
     Returns:
         df (np.array)
         col_idx (list): Tuples with 'column name' and list of one-hot indices for that column plus all numeric columns)
         col_fs (list): List of functions for each column in data
-        OHE (Encoder): sklearn OneHotEncoding object that can be used to inverse transform synthetic data
+        transformers (tuple): OHE object and min-max scaler for inverse data transformation
         df_cols (list): List of column names after column sorting but before one-hot encoding
     '''
     # 1. get categorical colum names
     num_type = ['int16', 'int32', 'int64', 'float16', 'float32', 'float64']  # numeric columns
-    str_type = ['O','category','string']  # select desired data type: 'O' - string
+    str_type = 'O'  # select desired data type: 'O' - string
     categorical_cols = []
-    binary_cols = []
-    positive_cols = []
     numeric_cols = []
     dtypes = df.dtypes.to_dict()
 
     for colname, data_type in dtypes.items():
-        if data_type in str_type:
+        if data_type == str_type:
             categorical_cols.append(colname)
         elif data_type in num_type:
-            if set(df[colname].unique()) == {1,0}:
-                binary_cols.append(colname)
-            elif df[colname].min() >= 0:
-                positive_cols.append(colname)
-            else:
-                numeric_cols.append(colname)
+          numeric_cols.append(colname)
         else:
             pass
-
-    # 2. one-hot encoding, puts categorical columns at the end of the df
-    OHE = OneHotEncoder(sparse=False)
-    cat_df = OHE.fit_transform(df[categorical_cols])
-    df.drop(categorical_cols, axis=1, inplace=True)
-
-    df_cols = df.columns.tolist() + categorical_cols
-
+    
+    OHE = OneHotEncoder(sparse_output=False)
+    scaler = MinMaxScaler()
+    # fill missing categorical columns as nan
+    df_cat = df[categorical_cols].fillna('nan')
+    # OHe transform
+    df_cat = OHE.fit_transform(df_cat)
+    df_num = df.drop(categorical_cols, axis=1)
+    # fill missing numeric values
+    df_num = df_num.fillna(df_num.median())
+    
+    # get ordered list of column names
+    df_cols = df_num.columns.tolist() + categorical_cols
+    if df_num.shape[1] > 0:
+        df_num = scaler.fit_transform(df_num)
+    transformers = (OHE, scaler)
+    
     # 3. finding idx for each original categorical column
-    col_idx = []
-    col_fs = []
+    col_idx, col_fs = [], []
     
-    # Numeric cols indx
+    # Numeric cols idx
     if len(numeric_cols) != 0:
-        col_idx_tensor = torch.Tensor([df.columns.get_loc(c) for c in numeric_cols])
+        col_idx_tensor = torch.Tensor([c for c in range(len(numeric_cols))])
         col_idx.append(col_idx_tensor)
         col_fs.append('identity')
 
-    # Positive cols
-    if len(positive_cols) != 0:
-        col_idx_tensor = torch.Tensor([df.columns.get_loc(c) for c in positive_cols])
-        col_idx.append(col_idx_tensor)
-        col_fs.append('relu')
-
-    # Binary cols
-    if len(binary_cols) != 0:
-        col_idx_tensor = torch.Tensor([df.columns.get_loc(c) for c in binary_cols])
-        col_idx.append(col_idx_tensor)
-        col_fs.append('sigmoid')
-
-    # Categorical cols
-    n_numeric = df.shape[1]
+    # Categorical cols idx
+    n_numeric = df_num.shape[1]
     cat_current_count = 0
     for var in OHE.categories_:
         one_hot_cols = var.tolist()
         start_idx = n_numeric + cat_current_count
         col_idx_tensor = torch.Tensor([i for i in range(start_idx, start_idx + len(one_hot_cols))])
         cat_current_count += len(one_hot_cols)
         col_idx.append(col_idx_tensor)
         col_fs.append('softmax')
 
-    df = np.concatenate((df, cat_df), axis = 1, dtype=np.float32)
-    return df, col_idx, col_fs, OHE, df_cols
+    df = np.concatenate((df_num, df_cat), axis = 1, dtype=np.float32) 
+
+    return df, col_idx, col_fs, transformers, df_cols 
 
 def _ohe_colnames(OHE):
     cat_cols = []
     for i in range(OHE.n_features_in_):
         for j in OHE.categories_[i]:
             cat_cols.append(OHE.feature_names_in_[i]+"_"+j)
     return cat_cols
```

### Comparing `sygnet-0.0.8/src/sygnet/interface.py` & `sygnet-0.0.9/src/sygnet/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,145 +1,152 @@
 ## USER INTERFACE
 import logging
 import os.path
 from pathlib import Path
 
 from .requirements import *
-from .models import Generator, Discriminator, Critic, ConditionalWrapper
-from .train import train_basic, train_wgan, train_conditional
+from .models import Generator, Critic, ConditionalWrapper
+from .train import train
 from .dataloaders import GeneratedData, _ohe_colnames
 
 
 logger = logging.getLogger(__name__)
 
 class SygnetModel:
 
     def __init__(
-        self, 
+        self,
+        # Model type 
         mode,
+        attention = True,
 
         # Generator and Discriminator options
-        hidden_nodes = [256,256], 
+        n_blocks = 2,
+        hidden_nodes = 256, 
         dropout_p = 0.2, 
-        layer_norms = True, 
-        relu_leak = 0.1,
+        relu_leak = 0.01,
+        n_heads = None,
         mixed_activation = True
         ):
         """SyGNet model object
 
         Args:
-            mode (str): One of ["basic","wgan","cgan"]. Determines whether to use basic GAN, Wasserstein loss, or Conditional GAN training method (default = "wgan").
-            hidden_nodes (list of ints, or [list of ints, list of ints]): The number of nodes in each hidden layer of the generator/discriminator network (default = [256, 256]). By default, both models are assigned the same hidden structure.         
-            dropout_p, disc_dropout (float, or [float, float]): The proportion of hidden nodes to be dropped randomly during training.
-            layer_norms (boolean, or [boolean, boolean]): Whether to include layer normalization in network (default = True).
-            relu_leak (float, or [float, float]): The negative slope parameter used to construct hidden-layer ReLU activation functions (default = 0.1; note: this default is an order larger than torch default).
+            mode (str): One of ["wgan","cgan"]. Determines whether to use Wasserstein loss or Conditional GAN training method (default = "wgan").
+            attention (bool): Whether to use self-attention within the generator model (default = True).
+            n_blocks (int, or [int, int]): The number of hidden blocks to use in the generator and critic networks (default = 2). See notes for more details.
+            hidden_nodes (int, or [int, int]): The number of nodes in each hidden layer of the generator and critic networks (default = 256). 
+            dropout_p (float, or [float, float]): The proportion of hidden nodes to be dropped randomly during training from the generator and critic respectively (default = 0.2).
+            relu_leak (float, or [float, float]): The negative slope parameters used to construct hidden-layer ReLU activation functions (default = 0.01)
+            n_heads (int): The number of attention heads within the self-attention mechanism (default = None).
             mixed_activation (boolean): Whether to use a mixed activation function final layer for the generator (default = True). If set to false, categorical and binary columns will not be properly transformed in generator output.
 
         Notes: 
-            hidden_nodes, dropout_p, layer_norms, and relu_leak can all accept list arguments of length 2, specifying parameters for the [generator, discriminator] respectively.
+            hidden_nodes, dropout_p, and relu_leak can all accept list arguments of length 2, specifying parameters for the [generator, discriminator] respectively.
             Parameters for the generator and discriminator are set independently (with identical default settings). Both models are modified in-place.
-            Arguments referring to "discriminators" cover both discriminator and critic networks. When mode = "basic" the discriminator model output is the probability of an observation being real. When mode != "basic", the discriminator model is a critic and provides an unbounded score of the observations "realness".
+            The hidden blocks of the network comprise different steps dependent on the architecture. At present, these are fixed by the `attention` argument. When attention = True, a single block comprises self attention -> batch normalisation -> leaky-ReLU activation. If attention = False, a single block comprises a linear layer -> layer normalisation -> leaky-ReLU -> dropout.  
 
         Attributes:
             mode (str):
             input_size (int): The number of input nodes. `None` until .fit() is called.
             label_size (int): The number of additional nodes for label columns when mode = "cgan". `None` until .fit() is called.
             output_size (int): The number of output nodes
             generator (nn.Module): The generator network (`None` until data fit). See `help(Generator)` for more information on internal attributes.
             mixed_activation (bool): Inclusion of a mixed activation layer
             discriminator (nn.Module): The discriminator/critic network (None until data fit). See `help(Discriminator)` or `help(Critic)` for more information on internal attributes.
             gen_hidden(list)
             disc_hidden(list)
             gen_dropout (float)
             disc_dropout (float)
-            gen_ln (bool)
             disc_lin (bool)
             gen_leak (float)
             disc_leak (float)
             data_encoders (list)
             gen_losses (list)
             disc_losses (list)
 
         """
         self.mode = mode
+        self.attention = attention
+        self.n_heads = n_heads
+
         self.input_size = None
         self.label_size = None
         self.output_size = None
         
         self.generator = None
-        self.discriminator = None
+        self.critic = None
 
         self.mixed_activation = mixed_activation
         self.data_encoders = None
         self.colnames = None
 
+        self.num_idx = None
+
         self.gen_losses = []
         self.disc_losses = []
 
         # Check args
-        if self.mode not in ['basic','wgan','cgan']:
-            logger.error("Argument `mode` must be one of 'basic', 'wgan', or 'cgan'")
+        if self.mode not in ['wgan','cgan']:
+            logger.error("Argument `mode` must be one of 'wgan' or 'cgan'")
+
+        if type(n_blocks) is int:
+            self.gen_blocks = self.crit_blocks = n_blocks
+        elif type(n_blocks) is list and len(n_blocks) == 2:
+            self.gen_blocks, self.crit_blocks = n_blocks
+        else:
+            logger.error("Argument `n_blocks` must either be a float or a list/tuple of length 2")
 
         # Get hidden node sizes
-        if type(hidden_nodes[0]) is list:
-            self.gen_hidden, self.disc_hidden = hidden_nodes
-        elif type(hidden_nodes) is list:
-            self.gen_hidden = self.disc_hidden = hidden_nodes
+        if type(hidden_nodes) is int:
+            self.gen_hidden = self.crit_hidden = hidden_nodes
+        elif type(hidden_nodes) is list and len(hidden_nodes) == 2:
+            self.gen_hidden, self.crit_hidden = hidden_nodes
         else:
-            logger.error("Argument `hidden_nodes` must either be a list of hidden layer sizes, or a list/tuple of length 2 where each element is a separate list of hidden layer sizes for the generator and discriminator respectively")
+            logger.warning("Supplying separate lists for each model was removed in v0.0.9")
+            logger.error("Argument `hidden_nodes` must either be a list of hidden layer sizes, or an integer.")
 
         # Get dropout proportions
         if type(dropout_p) is float:
-            self.gen_dropout = self.disc_dropout = dropout_p
-        elif len(dropout_p) == 2:
-            self.gen_dropout, self.disc_dropout = dropout_p
+            self.gen_dropout = self.crit_dropout = dropout_p
+        elif type(dropout_p) is list and len(dropout_p) == 2:
+            self.gen_dropout, self.crit_dropout = dropout_p
         else:
             logger.error("Argument `dropout_p` must either be a float or a list/tuple of length 2")
 
-        # Get layer norm toggles
-        if type(layer_norms) is bool:
-            self.gen_ln = self.disc_ln = layer_norms
-        elif len(layer_norms) == 2:
-            self.gen_ln, self.disc_ln = layer_norms
-        else:
-            logger.error("Argument `layer_norms` must either be a float or a list/tuple of length 2")
-
         # Get leaky alpha values
         if type(relu_leak) is float:
-            self.gen_leak = self.disc_leak = relu_leak
-        elif len(layer_norms) == 2:
-            self.gen_leak, self.disc_leak = relu_leak
+            self.gen_leak = self.crit_leak = relu_leak
+        elif type(relu_leak) is list and len(relu_leak) == 2:
+            self.gen_leak, self.crit_leak = relu_leak
         else:
             logger.error("Argument `relu_leak` must either be a float or a list/tuple of length 2.") 
     
     def fit(
         self, 
         data,
         cond_cols = None,
         epochs=10, 
         device='cpu',
         batch_size = None,
-        learning_rate = 0.0001,
-        adam_betas = (0.0, 0.9),
+        learning_rates = 0.0001,
         lmbda = 10,
         use_tensorboard = False,
         save_model = False,
         save_loc = "",
         save_prefix = "sygnet_model_"
         ):
         """Fit the SyGNet model to the training data
 
         Args:
             data (str or pd.DataFrame): Real data used to train GAN, can be a filepath or Pandas DataFrame
             cond_cols (list of colnames): Column names that indicate conditioning variables
             epochs (int): Number of training epochs
             device (str): Either 'cuda' for GPU training, or 'cpu' (default='cpu')
             batch_size (int): Number of training observations per batch (default = None). If left at default, the batch size is set to 1/20th of the overall length of the data.
-            learning_rate (float): The learning rate for the Adam optimizer (default = 0.0001)
-            adam_betas (tuple): The beta parameters for the Adam optimizer, only used in wgan and cgan modes
+            learning_rates (float or [float, float]): The learning rates for the generator and critic AdamW optimizers
             lmbda (float): Scalar penalty term for applying gradient penalty as part of Wasserstein loss, only used in wgan and cgan modes
             use_tensorboard (boolean): If True, creates tensorboard output capturing key training metrics (default = True)
             save_model (bool): Whether or not to save the model after training (default = False)
             save_loc (str): If save_model is True, the filepath where the directory should be saved (default = current working directory). Note, on Windows users should use raw strings (i.e. r"C:..." to avoid backslash escape issues)
             save_prefix (str): File prefix for the saved model (default = "sygnet_model_"). The full filename will be save_prefix + "DDMMMYY_HHMM"
 
         Note: 
@@ -155,14 +162,21 @@
         # Check args
         if cond_cols is not None and self.mode != "cgan":
             logger.warning(f"Conditional column indices supplied but model mode is set to '{self.mode}'. All columns in 'cond_cols'  will be synthesised.")
         elif cond_cols is None and self.mode == "cgan":
             logger.warning(f"Model mode is set to '{self.mode}' but no columns specified in 'cond_cols'. Switching to WGAN architecture.")
             self.mode = "wgan"
 
+        if type(learning_rates) is float:
+            learning_rates = [learning_rates, learning_rates]
+        elif len(learning_rates) == 2:
+            learning_rates = learning_rates
+        else:
+            logger.error("Learning rates argument must be a float or a list of two floats, for the generator and discriminator respectively.")
+
         # Set file path and static part of filename
         if save_model:
             if not isinstance(save_loc, str):
                 logger.error("Argument `save_loc` must contain a directory path as an 'r' string. For example: save_loc = r'path/to/my/models/'")
                 logger.error("Model will not be saved")
             elif save_loc == None:
                 logger.error("Argument `save_loc` must contain a directory path as an 'r' string. For example: save_loc = r'path/to/my/models/'")
@@ -174,115 +188,93 @@
                 logger.info("Model will be saved to: " + save_loc)
                 filepath = Path(save_loc)
 
         # Convert data dependent on model type
         if self.mode != "cgan":
             torch_data = GeneratedData(real_data = data)
             self.input_size = self.output_size = torch_data.x.shape[1]
-            self.data_encoders = [torch_data.x_OHE]
+            # self.data_encoders = [torch_data.x_OHE]
+            self.data_encoders = torch_data.x_transformers
 
         else:
             torch_data = GeneratedData(real_data = data, conditional = True, cond_cols = cond_cols)
             self.input_size = self.output_size = torch_data.x.shape[1]
             self.label_size = torch_data.labels.shape[1]
-            self.data_encoders = [torch_data.x_OHE, torch_data.labels_OHE]
+            # self.data_encoders = [torch_data.x_OHE, torch_data.labels_OHE]
+            self.data_encoders = torch_data.x_transformers
+            self.label_encoders = torch_data.labels_transformers
 
         self.colnames = torch_data.colnames
+        self.num_idx = torch_data.x_indxs[0].long()
         
         ## Build the models (if not already built)
 
         if self.generator is None:      
 
             self.generator = Generator(
-                input_size = self.input_size,
-                hidden_sizes = self.gen_hidden,
+
+                input_size = self.input_size, 
                 output_size = self.output_size,
+                n_blocks = self.gen_blocks,
+                hidden_nodes = self.gen_hidden,
+                attention = self.attention,
+                n_heads = self.n_heads,
                 mixed_activation = self.mixed_activation,
                 mix_act_indices=torch_data.x_indxs,
                 mix_act_funcs=torch_data.x_funcs,
                 dropout_p = self.gen_dropout,
-                layer_norm = self.gen_ln,
                 relu_alpha=self.gen_leak,
-                device=device
+                device=device,
                 )
 
-            if self.mode == "basic":
-                self.discriminator = Discriminator(
-                    input_size = self.input_size,
-                    hidden_sizes = self.disc_hidden,
-                    dropout_p = self.disc_dropout,
-                    layer_norm = self.disc_ln,
-                    relu_alpha = self.disc_leak
-                    )
-            else:
-                self.discriminator = Critic(
-                    input_size = self.input_size,
-                    hidden_sizes = self.disc_hidden,
-                    dropout_p = self.disc_dropout,
-                    layer_norm = self.disc_ln,
-                    relu_alpha = self.disc_leak
-                    )
+            self.critic = Critic(
+                input_size = self.input_size, 
+                n_blocks = self.crit_blocks, 
+                hidden_nodes = self.crit_hidden, 
+                dropout_p = self.crit_dropout, 
+                relu_alpha = self.crit_leak,
+            )
 
             # Wrap conditional GANs
             if self.mode == "cgan":
                 self.generator = ConditionalWrapper(latent_size = self.input_size, label_size = self.label_size, main_network = self.generator)
-                self.discriminator = ConditionalWrapper(latent_size = self.input_size, label_size = self.label_size, main_network = self.discriminator)
+                self.critic = ConditionalWrapper(latent_size = self.input_size, label_size = self.label_size, main_network = self.critic)
 
         ## Train the models
 
         if batch_size is None:
             batch_size = int(np.floor(data.shape[0]/20))
 
-        if self.mode == "basic":
-            g_loss, d_loss = train_basic(
-                training_data = torch_data, 
-                generator = self.generator, 
-                discriminator = self.discriminator,
-                epochs = epochs, 
-                device = device,
-                batch_size = batch_size,
-                learning_rate = learning_rate,
-                use_tensorboard = use_tensorboard
-            )
-        elif self.mode == "wgan":
-            g_loss, d_loss = train_wgan(
-                training_data = torch_data, 
-                generator = self.generator, 
-                critic = self.discriminator,
-                epochs = epochs, 
-                device = device,
-                batch_size = batch_size,
-                learning_rate = learning_rate,
-                adam_betas = adam_betas,
-                lmbda = lmbda,
-                use_tensorboard = use_tensorboard
-            )
+        train_args = {
+            'training_data' : torch_data, 
+            'generator' : self.generator, 
+            'critic' : self.critic,
+            'epochs' : epochs, 
+            'num_cols' : self.num_idx,
+            'batch_size' : batch_size,
+            'learning_rates' : learning_rates,
+            'lmbda' : lmbda,
+            'device' : device,
+            'use_tensorboard' : use_tensorboard,
+        }
+
+        if self.mode == "wgan":
+            g_loss, d_loss = train(**train_args, conditional = False)
         elif self.mode == "cgan":
-            g_loss, d_loss = train_conditional(
-                training_data = torch_data, 
-                generator = self.generator, 
-                critic = self.discriminator,
-                epochs = epochs, 
-                device = device,
-                batch_size = batch_size,
-                learning_rate = learning_rate,
-                adam_betas = adam_betas,
-                lmbda = lmbda,
-                use_tensorboard = use_tensorboard
-            )
+            g_loss, d_loss = train(**train_args, conditional = True)
         
         self.gen_losses += g_loss
         self.disc_losses += d_loss
             
         if save_model:
             with open(filepath / (save_prefix + datetime.now().strftime("%d%b%y_%H%M")), 'wb') as f:
                 pickle.dump(self, f)
         return None
 
-    def sample(self, nobs, labels = None, file = None, decode = True, as_pandas = True,  **kwargs):
+    def sample(self, nobs, labels = None, file = None, decode = True, as_pandas = True, **kwargs):
         """Generate synthetic data 
 
         Args:
             generator_model (nn.Module): Generator model object
             nobs (nn.Module): Discriminator model object
             labels (pd.Dataframe): Array of labels that should have as many rows as 'nobs' argument. Only used if the Sygnet model has mode = "cgan" (default = None).
             file (str): File path location to save data. If a path is not provided, the data is only returned in memory (default = None).
@@ -308,70 +300,84 @@
                     try:
                         labels = pd.DataFrame(labels)
                     except:
                         logger.error("Labels was not provided as DataFrame: implicit conversion failed.")
                 
                 seed_latent = torch.rand(size=(nobs, self.generator.latent_size))
 
-                labels_colnames_cat = self.data_encoders[1].feature_names_in_ if self.data_encoders[1].categories_ else []
+                labels_colnames_cat = self.label_encoders[0].feature_names_in_ if self.label_encoders[0].categories_ else []
                 labels_cat = labels[labels_colnames_cat]
 
                 labels_num = labels.drop(labels_colnames_cat, axis = 1)
                 labels_colnames_num = labels_num.columns
 
+                seed_labels = []
+                if hasattr(self.label_encoders[1], 'n_features_in_'):
+                    seed_labels.append(self.label_encoders[1].transform(labels_num))
+                if hasattr(self.label_encoders[0], 'categories_'):
+                    seed_labels.append(self.label_encoders[0].transform(labels_cat))
+
                 seed_labels = torch.from_numpy(
-                    np.concatenate((labels_num, self.data_encoders[1].transform(labels_cat)), axis=1)
+                    np.concatenate(
+                        seed_labels, 
+                        axis=1
+                    )
                 ).float()
                 
         else:
             seed_data = torch.rand(size=(nobs, self.generator.output_size))
 
+        self.generator.eval()
         with torch.no_grad():
-            device = 'cuda' if next(self.generator.parameters()).is_cuda else 'cpu'
+            device = next(self.generator.parameters()).device.type
 
             if self.mode == "cgan":
                 seed_latent = seed_latent.to(device)
                 seed_labels = seed_labels.to(device)
                 synth_output = self.generator(seed_latent, seed_labels)                  
             else:
                 seed_data = seed_data.to(device)
                 synth_output = self.generator(seed_data)
 
             synth_output = synth_output.detach().to('cpu').numpy()
         
         logger.debug("Generated data")
         logger.debug(synth_output)
 
+        self.generator.train()
+
         if decode:
             n_cat_vars = self.data_encoders[0].n_features_in_
             cat_names = [val for sublist in self.data_encoders[0].categories_ for val in sublist]
             n_cats = len(cat_names)
             if n_cat_vars > 0:
                 logger.debug(f"{n_cats} categorical columns to transform for {n_cat_vars} categorical variables")
                 synth_output = np.column_stack(
                     (synth_output[:,:-n_cats],
                     self.data_encoders[0].inverse_transform(synth_output[:,-n_cats:]))
                 )
+            else:
+                synth_output = self.data_encoders[1].inverse_transform(synth_output)
+            
             if self.mode == "cgan":
                 synth_output = np.column_stack([synth_output, np.array(labels)])
                 out_col_order = self.colnames[:-len(labels.columns)] + labels.columns.tolist()
         else:
             X_cat_cols = _ohe_colnames(self.data_encoders[0])
             labels_cat_cols =  []
             
             if self.mode == "cgan":
                 synth_output = np.column_stack([synth_output, seed_labels]) 
-                labels_cat_cols = _ohe_colnames(self.data_encoders[1])
+                labels_cat_cols = _ohe_colnames(self.label_encoders[0])
                 X_num_cols = self.colnames[:-(labels.shape[1]+self.data_encoders[0].n_features_in_)]
                 out_col_order = X_num_cols + X_cat_cols + labels_colnames_num.tolist() + labels_cat_cols
             else:
                 X_num_cols = self.colnames[:-self.data_encoders[0].n_features_in_]
                 out_col_order = X_num_cols + X_cat_cols
                 
-        
         # Convert to pandas if required:
         if as_pandas:
             synth_output = pd.DataFrame(synth_output)
             if self.mode == "cgan":
                 if decode:
                     synth_output.columns = out_col_order
                 else:
```

### Comparing `sygnet-0.0.8/src/sygnet/loader.py` & `sygnet-0.0.9/src/sygnet/loader.py`

 * *Files identical despite different names*

### Comparing `sygnet-0.0.8/src/sygnet/train.py` & `sygnet-0.0.9/src/sygnet/train.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,189 @@
 ### TRAINING FUNCTIONS
 from .requirements import *
 
 logger = logging.getLogger(__name__)
 
-def train_basic(
-    training_data, 
-    generator, 
-    discriminator,
-    epochs, 
-    device,
-    batch_size,
-    learning_rate,
-    use_tensorboard
-    ):
-    """Training function for basic GAN method
-
-    Args:
-        training_data (Dataset): Real data used to train GAN
-        generator (nn.Module): Generator model object
-        discriminator (nn.Module): Discriminator model object
-        epochs (int): Number of training epochs
-        device (str): Either 'cuda' for GPU training, or 'cpu'.
-        batch_size (int): Number of training observations per batch
-        learning_rate (float): The learning rate for the Adam optimizer (default = 0.0001)
-        use_tensorboard (boolean): If True, creates tensorboard output capturing key training metrics (default = True)
-
-    Note: 
-        The generator (and discriminator) model is modified in-place so this is not returned by the function
-
-    Returns:
-        generator_losses (list), discriminator_losses (list): lists of losses at the batch-level
-
-    """
-
-    data_loader = DataLoader(dataset = training_data, batch_size=batch_size, shuffle=True)
-
-    if use_tensorboard:
-        from torch.utils.tensorboard import SummaryWriter
-        writer = SummaryWriter(f'outputs/run_gan_{datetime.now()}')
-
-    # Models
-    discriminator_model = discriminator.to(device)
-    generator_model = generator.to(device)
-
-    # Optimizers
-    generator_optimizer = torch.optim.Adam(generator_model.parameters(), lr=learning_rate)
-    discriminator_optimizer = torch.optim.Adam(discriminator_model.parameters(), lr=learning_rate)
-
-    # Loss recording
-    generator_losses = []
-    discriminator_losses = []
-
-    # Define loss function
-    loss = nn.BCELoss()
+# def train_wgan(
+#     training_data, 
+#     generator, 
+#     critic,
+#     epochs, 
+#     num_cols,
+#     batch_size,
+#     learning_rates,
+#     lmbda,
+#     use_tensorboard,
+#     device,
+#     noise_std = 0.01,
+#     ):
+#     """Training function for Wasserstein-GP GAN method
+
+#     Args:
+#         training_data (Dataset): Real data used to train GAN
+#         generator (nn.Module): Generator model object
+#         critic (nn.Module): Critic model object
+#         epochs (int): Number of training epochs
+#         num_cols (list): List indicating which *numeric* columns to apply random noise to
+#         batch_size (int): Number of training observations per batch
+#         learning_rates (list): The learning rates for the generator and critic AdamW optimizers
+#         lmbda (float): Scalar penalty term for applying gradient penalty as part of Wasserstein loss
+#         use_tensorboard (boolean): If True, creates tensorboard output capturing key training metrics (default = True)
+#         device (str): Either 'cuda' for GPU training, or 'cpu'
+
+#     Note: 
+#         The generator and critic models are modified in-place so this is not returned by the function
+
+#     Returns:
+#         generator_losses (list), critic_losses (list): lists of losses at the batch-level
+
+#     """
+
+#     data_loader = DataLoader(dataset = training_data, batch_size=batch_size, shuffle=True)
+
+#     if use_tensorboard:
+#         from torch.utils.tensorboard import SummaryWriter
+#         writer = SummaryWriter(f'outputs/run_wgan_{datetime.now()}')
+#     # Models
+#     critic_model = critic.to(device)
+#     generator_model = generator.to(device)
+
+#     # Optimizers
+#     learning_rate_g = learning_rates[0]
+#     learning_rate_c = learning_rates[1]
+
+#     generator_optimizer = torch.optim.AdamW(generator_model.parameters(),
+#                                             lr=learning_rate_g, weight_decay=0.01)
+#     critic_optimizer = torch.optim.AdamW(critic_model.parameters(), lr=learning_rate_c,
+#                                          weight_decay=0.01)
+    
+#     base_lambda_g = lambda epoch: 0.9995 ** epoch
+#     base_lambda_c = lambda epoch: 0.9995 ** epoch
 
-    # Training loop
-    tbar = trange(epochs, desc="Epoch")
-    for epoch in tbar:
-        logger.debug("Epoch: "+str(epoch))
-         
-        for i, (features, labels) in enumerate(data_loader):
+#     scheduler_g = torch.optim.lr_scheduler.LambdaLR(generator_optimizer, lr_lambda=base_lambda_g)
+#     scheduler_c = torch.optim.lr_scheduler.LambdaLR(critic_optimizer, lr_lambda=base_lambda_c)
 
-            logger.debug("Batch: "+str(i))
+#     # Loss recording
+#     generator_losses = []
+#     critic_losses = []
 
-            generator_optimizer.zero_grad()
+#     num_cols = num_cols.to(device)
 
-            gen_obs = features.size(dim=0)
-            gen_cols = features.size(dim=1)
+#     # Training loop
+#     tbar = trange(epochs, desc="Epoch")
+#     for epoch in tbar:
 
-            noisy_input = torch.rand(size=(gen_obs, gen_cols))
-            noisy_input = noisy_input.to(device)
-            generated_data = generator_model(noisy_input).to(device)
-
-            true_data = features.to(device)
-            true_labels = labels.to(device)
-
-            logger.debug("BATCHSTEP: Training the generator")
-            generator_discriminator_out = discriminator_model(generated_data)
-            generator_loss = loss(generator_discriminator_out, true_labels)
-            generator_loss.backward()
-            generator_optimizer.step()
+#         for i, (features, _) in enumerate(data_loader):
+            
+#             # Get info on batches
+#             gen_obs = features.size(dim=0)
+#             gen_cols = features.size(dim=1)
+
+#             # Add random noise for stability
+#             noise_g = torch.randn(size=(gen_obs, num_cols.shape[0])) * noise_std
+#             noise_c = torch.randn(size=(gen_obs, num_cols.shape[0])) * noise_std
+#             noise_g = noise_g.to(device)
+#             noise_c = noise_c.to(device)
+            
+#             real_data = features.to(device)
+            
+#             # add gausian noise
+#             real_data[:, num_cols] = real_data[:, num_cols] + noise_c
 
-            logger.debug("BATCHSTEP: Training discriminator on true data")
-            discriminator_optimizer.zero_grad()
-            true_discriminator_out = discriminator_model(true_data)
-            true_discriminator_loss = loss(true_discriminator_out, true_labels)
-
-            logger.debug("BATCHSTEP: Training discriminator on fake data")
-            generator_discriminator_out = discriminator_model(generated_data.detach())  #  Detach to break out of grad. calc.
-            generator_discriminator_loss = loss(generator_discriminator_out, torch.zeros(gen_obs, 1).to(device))
-            discriminator_loss = (true_discriminator_loss + generator_discriminator_loss) / 2
-            discriminator_loss.backward()
-            discriminator_optimizer.step()
+#             ## Sort out the critic
+#             # Zero gradients and get critic scores
+#             generator_model.zero_grad()
+#             critic_model.zero_grad()
 
-            generator_losses.append(generator_loss.item())
-            discriminator_losses.append(true_discriminator_loss.item())
+#             critic_score_real = critic_model(real_data)
+            
+#             fake_input = torch.rand(size=(gen_obs, gen_cols))
+#             fake_input = fake_input.to(device)
+#             fake_data = generator_model(fake_input).to(device)
+
+#             critic_score_fake = critic_model(fake_data)
+
+#             # Calculate gradient penalty
+#             eps_shape = [gen_obs] + [1]*(len(features.shape)-1)
+#             eps = torch.rand(eps_shape).to(device)
+#             mixed_data = eps*real_data + (1-eps)*fake_data
+#             mixed_output = critic_model(mixed_data)
+
+#             grad = torch.autograd.grad(
+#                 outputs = mixed_output,
+#                 inputs = mixed_data,
+#                 grad_outputs = torch.ones_like(mixed_output),
+#                 create_graph = True,
+#                 retain_graph = True,
+#                 only_inputs=True,
+#                 allow_unused=True
+#             )[0]
+
+#             critic_grad_penalty = ((grad.norm(2, dim=1) -1)**2)
+
+#             error_critic = (critic_score_fake - critic_score_real).mean() + critic_grad_penalty.mean()*lmbda
+#             error_critic.backward()
+#             critic_optimizer.step()
+#             scheduler_c.step()
+
+#             critic_losses.append(error_critic.item())
+
+#             ## Sort out the generator
+#             # Re-zero gradients
+#             generator_model.zero_grad()
+#             critic_model.zero_grad()
+#             # Refresh random fake data
+#             fake_input2 = torch.rand(size=(gen_obs, gen_cols))
+#             fake_input2 = fake_input2.to(device)
+#             fake_data2 = generator_model(fake_input2).to(device)
+
+#             neg_critic_score_fake = -critic_model(fake_data2)
+#             error_gen = neg_critic_score_fake.mean()
+#             error_gen.backward()
+#             generator_optimizer.step()
+#             scheduler_g.step()
 
-        if use_tensorboard:
-            writer.add_scalar('Generator loss', generator_loss, global_step=epoch)
-            writer.add_scalar('True Discriminator loss', true_discriminator_loss, global_step=epoch)
+#             generator_losses.append(error_gen.item())
+            
+#         if use_tensorboard:
+#             writer.add_scalar('Critic loss', critic_losses[-1], global_step=epoch)
+#             writer.add_scalar('Generator loss', generator_losses[-1], global_step=epoch)
 
-        logger.info(" Epoch %s summary: Generator loss: %s; True discriminator loss = %s; Training loss: %s" % (epoch, round(generator_loss.item(),5), round(true_discriminator_loss.item(),5), round(generator_discriminator_loss.item(),5)))
+#         logger.info("Epoch %s summary: Generator loss: %s; Critic loss = %s" % (epoch, round(generator_losses[-1],5), round(critic_losses[-1],5)))
+#         tbar.set_postfix(loss = critic_losses[-1])
+#     return generator_losses, critic_losses
 
-    return generator_losses, discriminator_losses
 
-def train_wgan(
+def train(
     training_data, 
     generator, 
     critic,
+    conditional,
     epochs, 
-    device,
+    num_cols,
     batch_size,
-    learning_rate,
-    adam_betas,
+    learning_rates,
     lmbda,
-    use_tensorboard
+    use_tensorboard,
+    device,
+    noise_std = 0.01,
     ):
     """Training function for Wasserstein-GP GAN method
 
     Args:
         training_data (Dataset): Real data used to train GAN
         generator (nn.Module): Generator model object
         critic (nn.Module): Critic model object
         epochs (int): Number of training epochs
-        device (str): Either 'cuda' for GPU training, or 'cpu'.
+        num_cols (list): List indicating which *numeric* columns to apply random noise to
         batch_size (int): Number of training observations per batch
-        learning_rate (float): The learning rate for the Adam optimizer
-        adam_betas (tuple): The beta parameters for the Adam optimizer
+        learning_rates (list): The learning rates for the generator and critic AdamW optimizers
         lmbda (float): Scalar penalty term for applying gradient penalty as part of Wasserstein loss
         use_tensorboard (boolean): If True, creates tensorboard output capturing key training metrics (default = True)
+        device (str): Either 'cuda' for GPU training, or 'cpu'
 
     Note: 
         The generator and critic models are modified in-place so this is not returned by the function
 
     Returns:
         generator_losses (list), critic_losses (list): lists of losses at the batch-level
 
@@ -144,178 +195,92 @@
         from torch.utils.tensorboard import SummaryWriter
         writer = SummaryWriter(f'outputs/run_wgan_{datetime.now()}')
     # Models
     critic_model = critic.to(device)
     generator_model = generator.to(device)
 
     # Optimizers
-    generator_optimizer = torch.optim.Adam(generator_model.parameters(), lr=learning_rate, betas=adam_betas)
-    critic_optimizer = torch.optim.Adam(critic_model.parameters(), lr=learning_rate, betas=adam_betas)
-
-    # Loss recording
-    generator_losses = []
-    critic_losses = []
-
-    # Training loop
-    tbar = trange(epochs, desc="Epoch")
-    for epoch in tbar:
-
-        for i, (features, _) in enumerate(data_loader):
-            
-            # Get info on batches
-            gen_obs = features.size(dim=0)
-            gen_cols = features.size(dim=1)
-
-            real_data = features.to(device)
-            # real_labels = labels.to(device)
-
-            ## Sort out the critic
-            # Zero gradients and get critic scores
-            generator_model.zero_grad()
-            critic_model.zero_grad()
-
-            critic_score_real = critic_model(real_data)
-            
-            fake_input = torch.rand(size=(gen_obs, gen_cols))
-            fake_input = fake_input.to(device)
-            fake_data = generator_model(fake_input).to(device)
-
-            critic_score_fake = critic_model(fake_data)
-
-            # Calculate gradient penalty
-            eps_shape = [gen_obs] + [1]*(len(features.shape)-1)
-            eps = torch.rand(eps_shape).to(device)
-            mixed_data = eps*real_data + (1-eps)*fake_data
-            mixed_output = critic_model(mixed_data)
-
-            grad = torch.autograd.grad(
-                outputs = mixed_output,
-                inputs = mixed_data,
-                grad_outputs = torch.ones_like(mixed_output),
-                create_graph = True,
-                retain_graph = True,
-                only_inputs=True,
-                allow_unused=True
-            )[0]
-
-            critic_grad_penalty = ((grad.norm(2, dim=1) -1)**2)
-
-            error_critic = (critic_score_fake - critic_score_real).mean() + critic_grad_penalty.mean()*lmbda
-            error_critic.backward()
-            critic_optimizer.step()
-
-            critic_losses.append(error_critic.item())
-
-            ## Sort out the generator
-            # Re-zero gradients
-            generator_model.zero_grad()
-            critic_model.zero_grad()
-            # Refresh random fake data
-            fake_input2 = torch.rand(size=(gen_obs, gen_cols))
-            fake_input2 = fake_input2.to(device)
-            fake_data2 = generator_model(fake_input2).to(device)
-
-            neg_critic_score_fake = -critic_model(fake_data2)
-            error_gen = neg_critic_score_fake.mean()
-            error_gen.backward()
-            generator_optimizer.step()
-
-            generator_losses.append(error_gen.item())
-        
-        if use_tensorboard:
-            writer.add_scalar('Critic loss', critic_losses[-1], global_step=epoch)
-            writer.add_scalar('Generator loss', generator_losses[-1], global_step=epoch)
-
-        logger.info("Epoch %s summary: Generator loss: %s; Critic loss = %s" % (epoch, round(generator_losses[-1],5), round(critic_losses[-1],5)))
-        tbar.set_postfix(loss = critic_losses[-1])
-    return generator_losses, critic_losses
-
-def train_conditional(
-    training_data, 
-    generator, 
-    critic,
-    epochs, 
-    device,
-    batch_size,
-    learning_rate,
-    adam_betas,
-    lmbda,
-    use_tensorboard
-    ):
-    """Training function for conditional GAN (using Wasserstein loss)
-
-    Args:
-        training_data (Dataset): Real data used to train GAN
-        generator (nn.Module): Generator model object
-        critic (nn.Module): Critic model object
-        epochs (int): Number of training epochs
-        device (str): Either 'cuda' for GPU training, or 'cpu'.
-        batch_size (int): Number of training observations per batch
-        learning_rate (float): The learning rate for the Adam optimizer
-        adam_betas (tuple): The beta parameters for the Adam optimizer
-        lmbda (float): Scalar penalty term for applying gradient penalty as part of Wasserstein loss
-        use_tensorboard (boolean): If True, creates tensorboard output capturing key training metrics (default = True)
-
-    Note: 
-        The generator and critic models are modified in-place so this is not returned by the function
-
-    Returns:
-        generator_losses (list), critic_losses (list): lists of losses at the batch-level
-
-    """
-
-    data_loader = DataLoader(dataset = training_data, batch_size=batch_size, shuffle=True)
+    learning_rate_g = learning_rates[0]
+    learning_rate_c = learning_rates[1]
 
-    if use_tensorboard:
-        from torch.utils.tensorboard import SummaryWriter
-        writer = SummaryWriter(f'outputs/run_cond_wgan_{datetime.now().strftime("%Y-%m-%d_%H%M%S")}')
+    generator_optimizer = torch.optim.AdamW(generator_model.parameters(),
+                                            lr=learning_rate_g, weight_decay=0.01)
+    critic_optimizer = torch.optim.AdamW(critic_model.parameters(), lr=learning_rate_c,
+                                         weight_decay=0.01)
     
-    # Send models to device
-    critic_model = critic.to(device)
-    generator_model = generator.to(device)
+    base_lambda_g = lambda epoch: 0.9995 ** epoch
+    base_lambda_c = lambda epoch: 0.9995 ** epoch
 
-    # Optimizers
-    generator_optimizer = torch.optim.Adam(generator_model.parameters(), lr=learning_rate, betas=adam_betas)
-    critic_optimizer = torch.optim.Adam(critic_model.parameters(), lr=learning_rate, betas=adam_betas)
+    scheduler_g = torch.optim.lr_scheduler.LambdaLR(generator_optimizer, lr_lambda=base_lambda_g)
+    scheduler_c = torch.optim.lr_scheduler.LambdaLR(critic_optimizer, lr_lambda=base_lambda_c)
 
     # Loss recording
     generator_losses = []
     critic_losses = []
 
+    num_cols = num_cols.to(device)
+
     # Training loop
     tbar = trange(epochs, desc="Epoch")
     for epoch in tbar:
-         
+
         for i, (features, labels) in enumerate(data_loader):
             
             # Get info on batches
             gen_obs = features.size(dim=0)
             gen_cols = features.size(dim=1)
 
-            real_data = features.to(device)
-            real_labels = labels.to(device)
+            # Add random noise for stability
+            noise_g = torch.randn(size=(gen_obs, num_cols.shape[0])) * noise_std
+            noise_c = torch.randn(size=(gen_obs, num_cols.shape[0])) * noise_std
+            noise_g = noise_g.to(device)
+            noise_c = noise_c.to(device)
+
+            if conditional:
+                train_args = [
+                    features.to(device),
+                    labels.to(device)
+                ]
+            else:
+                train_args = [
+                    features.to(device)
+                ]
+            
+            
+            # add gausian noise
+            train_args[0][:, num_cols] = train_args[0][:, num_cols] + noise_c
 
             ## Sort out the critic
             # Zero gradients and get critic scores
             generator_model.zero_grad()
             critic_model.zero_grad()
 
-            critic_score_real = critic_model(real_data, real_labels)
+            critic_score_real = critic_model(*train_args)
             
             fake_input = torch.rand(size=(gen_obs, gen_cols))
             fake_input = fake_input.to(device)
-            fake_data = generator_model(fake_input, real_labels).to(device)
+            
+            
 
-            critic_score_fake = critic_model(fake_data, real_labels)
+            if conditional:
+                fake_data = generator_model(fake_input, train_args[1]).to(device)
+                critic_score_fake = critic_model(fake_data, train_args[1])
+            else:
+                fake_data = generator_model(fake_input).to(device)
+                critic_score_fake = critic_model(fake_data)
 
             # Calculate gradient penalty
-            eps_shape = [gen_obs] + [1]*(len(features.shape) -1)
+            eps_shape = [gen_obs] + [1]*(len(features.shape)-1)
             eps = torch.rand(eps_shape).to(device)
-            mixed_data = eps*real_data + (1-eps)*fake_data
-            mixed_output = critic_model(mixed_data, real_labels)
+            mixed_data = eps*train_args[0] + (1-eps)*fake_data
+
+            if conditional:
+                mixed_output = critic_model(mixed_data, train_args[1])
+            else:
+                mixed_output = critic_model(mixed_data)
 
             grad = torch.autograd.grad(
                 outputs = mixed_output,
                 inputs = mixed_data,
                 grad_outputs = torch.ones_like(mixed_output),
                 create_graph = True,
                 retain_graph = True,
@@ -324,34 +289,40 @@
             )[0]
 
             critic_grad_penalty = ((grad.norm(2, dim=1) -1)**2)
 
             error_critic = (critic_score_fake - critic_score_real).mean() + critic_grad_penalty.mean()*lmbda
             error_critic.backward()
             critic_optimizer.step()
+            scheduler_c.step()
 
             critic_losses.append(error_critic.item())
 
             ## Sort out the generator
             # Re-zero gradients
             generator_model.zero_grad()
             critic_model.zero_grad()
+            
             # Refresh random fake data
             fake_input2 = torch.rand(size=(gen_obs, gen_cols))
             fake_input2 = fake_input2.to(device)
-            fake_data2 = generator_model(fake_input2, real_labels).to(device)
+            if conditional:
+                fake_data2 = generator_model(fake_input2, train_args[1]).to(device)
+                neg_critic_score_fake = -critic_model(fake_data2, train_args[1])
+            else:
+                fake_data2 = generator_model(fake_input2).to(device)
+                neg_critic_score_fake = -critic_model(fake_data2)
 
-            neg_critic_score_fake = -critic_model(fake_data2, real_labels)
             error_gen = neg_critic_score_fake.mean()
             error_gen.backward()
             generator_optimizer.step()
+            scheduler_g.step()
 
             generator_losses.append(error_gen.item())
-
+            
         if use_tensorboard:
             writer.add_scalar('Critic loss', critic_losses[-1], global_step=epoch)
             writer.add_scalar('Generator loss', generator_losses[-1], global_step=epoch)
 
         logger.info("Epoch %s summary: Generator loss: %s; Critic loss = %s" % (epoch, round(generator_losses[-1],5), round(critic_losses[-1],5)))
         tbar.set_postfix(loss = critic_losses[-1])
-
-    return generator_losses, critic_losses
+    return generator_losses, critic_losses
```

### Comparing `sygnet-0.0.8/src/sygnet/tune.py` & `sygnet-0.0.9/src/sygnet/tune.py`

 * *Files 15% similar despite different names*

```diff
@@ -56,23 +56,31 @@
 
         Returns:
             pd.DataFrame of hyperparameter tuning results
 
     """
 
     logger.warning(
-        "This function is still in development. Only 'wgan' modelling has been implemented thus far, and all hyperparameter searches will use random sampling rather than an exhaustive grid seach"
+        "This function is still in development. Only 'wgan' and 'cgan' modelling has been implemented thus far, and all hyperparameter searches will use random sampling rather than an exhaustive grid seach"
     )
 
     torch.manual_seed(seed)
     random.seed(seed)
 
-    if mode != "wgan":
+    if mode not in ["wgan", "cgan"]:
         return None
 
+    if mode == "cgan" and 'cond_cols' not in fit_opts:
+        logger.warning(
+            "Since you are using Conditional arcgitecture, you need to specify conditional columns as 'cond_cols' in fit_opts dictionary. Example: fit_opts = {'save_model': False, 'cond_cols' : ['name']}"
+        )
+
+    if mode == "cgan" and not isinstance(fit_opts['cond_cols'],list):
+        raise Exception("Conditional columns 'cond_cols' must be a list!")
+
     if type(parameter_dict) is not dict:
         logger.error("`parameter_dict` must be a dictionary with hyperparameter arguments as keys and lists of options to try as values. \n \
             Tunable hyperparameters across sygnet are currently: \n \
                 \t SygnetModel: `hidden_nodes`, `dropout_p`,`layer_norms`,`relu_leak`, \n \
                 \t .fit(): `batch_size,`learning_rate`, and `adam_betas`"
                 )
 
@@ -94,15 +102,15 @@
             kf.get_n_splits(data)
         else:
             kf = KFold(n_splits =2)
             kf.get_n_splits(data)
         
         k_count = 0
 
-        for train_idx, test_idx in kf.split(data):
+        for train_idx, _ in kf.split(data):
 
             if k == 1 and k_count == 1:
                 continue
             
             sygnet_model = SygnetModel(**model_dict_chosen, **model_opts, mode = mode)
             train_epochs = epochs//checkpoints
```

### Comparing `sygnet-0.0.8/sygnet.png` & `sygnet-0.0.9/sygnet.png`

 * *Files identical despite different names*

### Comparing `sygnet-0.0.8/sygnet1280.png` & `sygnet-0.0.9/sygnet1280.png`

 * *Files identical despite different names*

### Comparing `sygnet-0.0.8/test/test_mixed_act.py` & `sygnet-0.0.9/test/test_mixed_act.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
         self.n_samples = 1000
         csv_input = pd.DataFrame(data = {
                 'x1' : np.random.uniform(low = -2, high = -1, size=self.n_samples),
                 'x2' : np.random.normal(loc = 100, scale = 200, size = self.n_samples),
                 'x3' : np.random.uniform(low = 5, high = 10, size=self.n_samples),
                 'y' : np.random.normal(loc = 0, scale = 10, size = self.n_samples),
-                'pet' : random.choices(['cat','cat','dog','dog','bird'], k = self.n_samples), 
+                'pet' : random.choices(['cat','dog','bird'], k = self.n_samples), 
                 'name' : random.choices(['bob','carl','sam','joe','mike'], k = self.n_samples),
                 'bin' : random.choices([1,0], k = self.n_samples)
                 })
 
         print(csv_input.head())
 
         training_data = GeneratedData(csv_input, conditional = False)
@@ -37,48 +37,53 @@
                 # x = self.lin2(x)
                 x = self.out_mix(x)
                 return x
 
         test_model = test_nn(input_size = training_data.x.shape[1], indices = training_data.x_indxs, funcs = training_data.x_funcs)
 
         self.out_df = test_model(training_data.x)
+
+        print("-----")
+        print(training_data.x[:5,:])
+        print(training_data.x_funcs)
+        print(training_data.x_indxs)
+        print(self.out_df[:2,:])
         
 
     def test_softmax_group1(self):
         """
         Test that 3-category column constrained to 1 (check with 5 obs)
         """
-        
         self.assertEqual(torch.sum(self.out_df[:,5:8]), self.n_samples)
 
     def test_softmax_group2(self):
         """
         Test that 5-category column constrained to 1 (check with 5 obs)
         """
         
         self.assertEqual(torch.sum(self.out_df[:,8:]), self.n_samples)
 
-    def test_bin(self):
-        """
-        Test binary column (check with 5 obs)
-        """
+    # def test_bin(self):
+    #     """
+    #     Test binary column (check with 5 obs)
+    #     """
 
-        # Binary is in col-position 4 since it occurs after categorical, so moved back to before cats
+    #     # Binary is in col-position 4 since it occurs after categorical, so moved back to before cats
         
-        bin_col = self.out_df.detach().numpy()[:,4]
-        less_than_one = sum(bin_col <= 1)
-        greater_than_zero = sum(bin_col >= 0)
+    #     bin_col = self.out_df.detach().numpy()[:,4]
+    #     less_than_one = sum(bin_col <= 1)
+    #     greater_than_zero = sum(bin_col >= 0)
         
-        self.assertEqual(less_than_one + greater_than_zero, self.n_samples*2)
+    #     self.assertEqual(less_than_one + greater_than_zero, self.n_samples*2)
 
-    def test_relu(self):
-        """
-        Test strictly-positive column (check with 5 obs)
-        """
+    # def test_relu(self):
+    #     """
+    #     Test strictly-positive column (check with 5 obs)
+    #     """
         
-        relu_col = self.out_df.detach().numpy()[:,2]
-        greater_than_zero = sum(relu_col >= 0)
+    #     relu_col = self.out_df.detach().numpy()[:,2]
+    #     greater_than_zero = sum(relu_col >= 0)
         
-        self.assertEqual(greater_than_zero, self.n_samples)
+    #     self.assertEqual(greater_than_zero, self.n_samples)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sygnet-0.0.8/test/test_pipeline.py` & `sygnet-0.0.9/test/test_pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,14 @@
 from src.sygnet.interface import *
 
 class TestSum(unittest.TestCase):
 
     def setUp(self):
         self.input_data = pd.read_csv("data/simulation_data_1.csv",delimiter=",").iloc[0:100,:]
 
-    def test_basic(self):
-        """
-        Test without conditional labels or Wasserstein loss
-        """
-
-        model = SygnetModel(mode="basic")
-        model.fit(self.input_data, epochs=1, batch_size=self.input_data.shape[0])
-        self.assertEqual(model.sample(5).shape, (5,4))
-
     def test_wgan(self):
         """
         Test without conditional labels
         """
 
         model = SygnetModel(mode="wgan")
         model.fit(self.input_data, epochs=1, batch_size=self.input_data.shape[0])
```

### Comparing `sygnet-0.0.8/test/test_sampler.py` & `sygnet-0.0.9/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `sygnet-0.0.8/test/test_saver.py` & `sygnet-0.0.9/test/test_saver.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,12 +27,12 @@
         with tempfile.TemporaryDirectory() as tmpdirname:
             model0.fit(self.input_data, epochs = 1, save_model=True, save_loc = r"{}".format(tmpdirname))
             new_file = os.listdir(tmpdirname)[0]
             model1 = load(Path(tmpdirname) / new_file)
 
         self.assertTrue(
             torch.equal(
-                model0.generator.state_dict()['linears.1.weight'],
-                model1.generator.state_dict()['linears.1.weight']
+                model0.generator.state_dict()['lin_out.weight'],
+                model1.generator.state_dict()['lin_out.weight']
             )
         )
```

### Comparing `sygnet-0.0.8/test/test_tuner.py` & `sygnet-0.0.9/test/test_tuner.py`

 * *Files identical despite different names*

### Comparing `sygnet-0.0.8/PKG-INFO` & `sygnet-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sygnet
-Version: 0.0.8
+Version: 0.0.9
 Summary: Synthetic data using Generative Adversarial Networks
 Keywords: synthetic data,neural networks,GAN,torch
 Author-email: Thomas Robinson <thomas.robinson@durham.ac.uk>
 Maintainer: Artem Nesterov, Maksim Zubok
 Maintainer-email: Thomas Robinson <thomas.robinson@durham.ac.uk>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: numpy>=1.21
 Requires-Dist: torch>=1.10.0
-Requires-Dist: scikit-learn>=1.0
+Requires-Dist: scikit-learn>=1.2
 Requires-Dist: pandas>=1.4
 Requires-Dist: datetime
 Requires-Dist: tqdm
 Requires-Dist: pickle ; extra == "save"
 Requires-Dist: tensorboard ; extra == "viz"
 Project-URL: Bugs, https://github.com/tsrobinson/SyGNet/issues
 Project-URL: Source, https://github.com/tsrobinson/SyGNet
@@ -33,44 +33,54 @@
 
 *Principal Investigator: Dr Thomas Robinson (thomas.robinson@durham.ac.uk)*
 
 *Research team: Artem Nesterov, Maksim Zubok*
 
 ![example workflow](https://github.com/tsrobinson/SyGNet/actions/workflows/python-app.yml/badge.svg)
 
-**sygnet** is a Python package for generating synthetic data within social science contexts. The **sygnet** algorithm uses cutting-edge advances in deep learning methods to learn the underlying relationships between variables in a dataset. Users can then generate brand-new, synthetic observations that mimic the real data.
+**sygnet** ("sig·net") is a Python package for generating 
+synthetic data within 
+social science contexts. The **sygnet** algorithm uses cutting-edge advances in deep learning methods to learn the underlying relationships between variables in a dataset. Users can then generate brand-new, synthetic observations that mimic the real data.
 
 ### Installation
 To install via pip, you can run the following command at the command line:
 `pip install sygnet`
 
 **sygnet** requires:
     
-    numpy>=1.20
+    numpy>=1.21
     torch>=1.10.0
     scikit-learn>=1.0
     pandas>=1.4
     datetime
     tqdm
 
 ### Example implementation
 
 You can find a demonstration of **sygnet** under [examples/basic_example](examples/basic_example.ipynb).
 
-### Current version: 0.0.8 (alpha release)
+### Current version: 0.0.9 (alpha release)
 
-**Alpha release**: You should expect both functionality and pipelines to change (rapidly). Comments and bug reports are very welcome!
+**Alpha release**: You should expect both functionality and pipelines to change (rapidly and without warning). Comments and bug reports are very welcome!
 
 Changes:
 
-* Update `tune()` to provide no k-fold cross validation as default
-* Update numpy dependency to fix pre-processing bug
+* Rewrite of main interface and underlying functions
+* Bulding models now structured in terms of hidden "blocks"
+* Added self-attention mechanism
 
 ### Previous releases
 
+**0.0.8**
+
+Changes:
+
+* Update `tune()` to provide no k-fold cross validation as default
+* Update numpy dependency to fix pre-processing bug
+
 **0.0.7**
 * Update internal `train_*` functions to return losses and improve logging
 * Update `tune()` function
 
 **0.0.6 and 0.0.5**
 * Internal changes to improve code efficiency
 * Removes `sygnet_` from all submodule names
@@ -88,7 +98,8 @@
 
 **0.0.2**
 * Fixes mixed activation bug where final layer wasn't sent to `device`
 * Adds `SygnetModel.transform()` alias for `SygnetModel.sample()`
 
 **0.0.1**
 Our first release! This version has been lightly tested and the core functionality has been implemented. 
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


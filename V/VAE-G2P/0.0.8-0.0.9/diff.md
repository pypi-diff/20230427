# Comparing `tmp/VAE_G2P-0.0.8.tar.gz` & `tmp/VAE_G2P-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VAE_G2P-0.0.8.tar", last modified: Thu Apr 27 17:41:32 2023, max compression
+gzip compressed data, was "VAE_G2P-0.0.9.tar", last modified: Thu Apr 27 19:25:47 2023, max compression
```

## Comparing `VAE_G2P-0.0.8.tar` & `VAE_G2P-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 17:41:32.570642 VAE_G2P-0.0.8/
--rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-27 17:41:32.570501 VAE_G2P-0.0.8/PKG-INFO
--rw-r--r--   0 davidblair   (501) staff       (20)      158 2023-03-05 01:23:50.000000 VAE_G2P-0.0.8/README.md
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 17:41:32.569535 VAE_G2P-0.0.8/VAE_G2P/
--rw-r--r--   0 davidblair   (501) staff       (20)      130 2023-04-05 04:44:26.000000 VAE_G2P-0.0.8/VAE_G2P/__init__.py
--rw-r--r--   0 davidblair   (501) staff       (20)    19663 2023-04-27 17:40:52.000000 VAE_G2P-0.0.8/VAE_G2P/basic_g2p.py
--rw-r--r--   0 davidblair   (501) staff       (20)    13488 2023-04-05 04:47:18.000000 VAE_G2P-0.0.8/VAE_G2P/cvae_model.py
--rw-r--r--   0 davidblair   (501) staff       (20)    15935 2023-04-27 17:27:13.000000 VAE_G2P-0.0.8/VAE_G2P/data.py
--rw-r--r--   0 davidblair   (501) staff       (20)     2120 2023-03-30 02:16:44.000000 VAE_G2P-0.0.8/VAE_G2P/data_wrapper.py
--rw-r--r--   0 davidblair   (501) staff       (20)     9624 2023-03-08 05:48:31.000000 VAE_G2P-0.0.8/VAE_G2P/networks.py
--rw-r--r--   0 davidblair   (501) staff       (20)    15046 2023-04-05 04:47:50.000000 VAE_G2P-0.0.8/VAE_G2P/optim.py
--rw-r--r--   0 davidblair   (501) staff       (20)    23311 2023-04-27 17:41:12.000000 VAE_G2P-0.0.8/VAE_G2P/vae_g2p.py
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 17:41:32.570311 VAE_G2P-0.0.8/VAE_G2P.egg-info/
--rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-27 17:41:32.000000 VAE_G2P-0.0.8/VAE_G2P.egg-info/PKG-INFO
--rw-r--r--   0 davidblair   (501) staff       (20)      331 2023-04-27 17:41:32.000000 VAE_G2P-0.0.8/VAE_G2P.egg-info/SOURCES.txt
--rw-r--r--   0 davidblair   (501) staff       (20)        1 2023-04-27 17:41:32.000000 VAE_G2P-0.0.8/VAE_G2P.egg-info/dependency_links.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       34 2023-04-27 17:41:32.000000 VAE_G2P-0.0.8/VAE_G2P.egg-info/requires.txt
--rw-r--r--   0 davidblair   (501) staff       (20)        8 2023-04-27 17:41:32.000000 VAE_G2P-0.0.8/VAE_G2P.egg-info/top_level.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       38 2023-04-27 17:41:32.570687 VAE_G2P-0.0.8/setup.cfg
--rw-r--r--   0 davidblair   (501) staff       (20)      941 2023-04-05 04:37:12.000000 VAE_G2P-0.0.8/setup.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 19:25:47.239858 VAE_G2P-0.0.9/
+-rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-27 19:25:47.239647 VAE_G2P-0.0.9/PKG-INFO
+-rw-r--r--   0 davidblair   (501) staff       (20)      158 2023-03-05 01:23:50.000000 VAE_G2P-0.0.9/README.md
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 19:25:47.238667 VAE_G2P-0.0.9/VAE_G2P/
+-rw-r--r--   0 davidblair   (501) staff       (20)      130 2023-04-05 04:44:26.000000 VAE_G2P-0.0.9/VAE_G2P/__init__.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    19656 2023-04-27 19:24:00.000000 VAE_G2P-0.0.9/VAE_G2P/basic_g2p.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    13488 2023-04-05 04:47:18.000000 VAE_G2P-0.0.9/VAE_G2P/cvae_model.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    15935 2023-04-27 17:27:13.000000 VAE_G2P-0.0.9/VAE_G2P/data.py
+-rw-r--r--   0 davidblair   (501) staff       (20)     2120 2023-03-30 02:16:44.000000 VAE_G2P-0.0.9/VAE_G2P/data_wrapper.py
+-rw-r--r--   0 davidblair   (501) staff       (20)     9624 2023-03-08 05:48:31.000000 VAE_G2P-0.0.9/VAE_G2P/networks.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    15046 2023-04-05 04:47:50.000000 VAE_G2P-0.0.9/VAE_G2P/optim.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    23311 2023-04-27 19:24:46.000000 VAE_G2P-0.0.9/VAE_G2P/vae_g2p.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 19:25:47.239373 VAE_G2P-0.0.9/VAE_G2P.egg-info/
+-rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-27 19:25:47.000000 VAE_G2P-0.0.9/VAE_G2P.egg-info/PKG-INFO
+-rw-r--r--   0 davidblair   (501) staff       (20)      331 2023-04-27 19:25:47.000000 VAE_G2P-0.0.9/VAE_G2P.egg-info/SOURCES.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)        1 2023-04-27 19:25:47.000000 VAE_G2P-0.0.9/VAE_G2P.egg-info/dependency_links.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       34 2023-04-27 19:25:47.000000 VAE_G2P-0.0.9/VAE_G2P.egg-info/requires.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)        8 2023-04-27 19:25:47.000000 VAE_G2P-0.0.9/VAE_G2P.egg-info/top_level.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       38 2023-04-27 19:25:47.239897 VAE_G2P-0.0.9/setup.cfg
+-rw-r--r--   0 davidblair   (501) staff       (20)      941 2023-04-05 04:37:12.000000 VAE_G2P-0.0.9/setup.py
```

### Comparing `VAE_G2P-0.0.8/VAE_G2P/basic_g2p.py` & `VAE_G2P-0.0.9/VAE_G2P/basic_g2p.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,15 +376,15 @@
         else:
             in_training=False
 
         annot_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.n_pred),dtype=torch.float32)
         freq_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.n_pred),dtype=torch.float32)
         for t,hpo_freq_vec in enumerate(hpo_freq_pairs):
             idx_vec=[self.g2p_dataset.symptom_map[x[0]] for x in hpo_freq_vec]
-            freq_vec=[self.g2p_dataset._ProcessSymptomCounts(x[1],self.diseaseGeneDataset.symptom_count_prior) for x in hpo_freq_vec]
+            freq_vec=[self.g2p_dataset._ProcessSymptomCounts(x[1],self.g2p_dataset.symptom_count_prior) for x in hpo_freq_vec]
             annot_array[t,idx_vec]=1
             freq_array[t,idx_vec]=torch.tensor(freq_vec,dtype=torch.float32)
         data_arrays=(annot_array,freq_array,self.g2p_dataset.ReturnGeneDataArrays(gene_list))
 
 
         pred_log_odds=self.basic_net.forward(data_arrays[2])
         if in_training:
```

### Comparing `VAE_G2P-0.0.8/VAE_G2P/cvae_model.py` & `VAE_G2P-0.0.9/VAE_G2P/cvae_model.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.8/VAE_G2P/data.py` & `VAE_G2P-0.0.9/VAE_G2P/data.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.8/VAE_G2P/data_wrapper.py` & `VAE_G2P-0.0.9/VAE_G2P/data_wrapper.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.8/VAE_G2P/networks.py` & `VAE_G2P-0.0.9/VAE_G2P/networks.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.8/VAE_G2P/optim.py` & `VAE_G2P-0.0.9/VAE_G2P/optim.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.8/VAE_G2P/vae_g2p.py` & `VAE_G2P-0.0.9/VAE_G2P/vae_g2p.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import copy
 
 from .cvae_model import DiseaseCondVAE
 from .basic_g2p import BasicG2PModel
 from .data import GeneToPhenotypeDataset
 from .optim import AutoEncoderOptimizer
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 class VAE_G2P:
 
 	def _readModelFromFile(self,fName):
 		with open(fName,'rb') as f:
 			model_dict = torch.load(f,map_location='cpu')
```

### Comparing `VAE_G2P-0.0.8/setup.py` & `VAE_G2P-0.0.9/setup.py`

 * *Files identical despite different names*


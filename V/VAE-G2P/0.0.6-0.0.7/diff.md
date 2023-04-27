# Comparing `tmp/VAE_G2P-0.0.6.tar.gz` & `tmp/VAE_G2P-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VAE_G2P-0.0.6.tar", last modified: Wed Apr 26 05:32:33 2023, max compression
+gzip compressed data, was "VAE_G2P-0.0.7.tar", last modified: Thu Apr 27 17:28:54 2023, max compression
```

## Comparing `VAE_G2P-0.0.6.tar` & `VAE_G2P-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-26 05:32:33.955181 VAE_G2P-0.0.6/
--rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-26 05:32:33.955046 VAE_G2P-0.0.6/PKG-INFO
--rw-r--r--   0 davidblair   (501) staff       (20)      158 2023-03-05 01:23:50.000000 VAE_G2P-0.0.6/README.md
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-26 05:32:33.953983 VAE_G2P-0.0.6/VAE_G2P/
--rw-r--r--   0 davidblair   (501) staff       (20)      130 2023-04-05 04:44:26.000000 VAE_G2P-0.0.6/VAE_G2P/__init__.py
--rw-r--r--   0 davidblair   (501) staff       (20)    19614 2023-04-05 04:47:05.000000 VAE_G2P-0.0.6/VAE_G2P/basic_g2p.py
--rw-r--r--   0 davidblair   (501) staff       (20)    13488 2023-04-05 04:47:18.000000 VAE_G2P-0.0.6/VAE_G2P/cvae_model.py
--rw-r--r--   0 davidblair   (501) staff       (20)    15876 2023-04-26 05:24:52.000000 VAE_G2P-0.0.6/VAE_G2P/data.py
--rw-r--r--   0 davidblair   (501) staff       (20)     2120 2023-03-30 02:16:44.000000 VAE_G2P-0.0.6/VAE_G2P/data_wrapper.py
--rw-r--r--   0 davidblair   (501) staff       (20)     9624 2023-03-08 05:48:31.000000 VAE_G2P-0.0.6/VAE_G2P/networks.py
--rw-r--r--   0 davidblair   (501) staff       (20)    15046 2023-04-05 04:47:50.000000 VAE_G2P-0.0.6/VAE_G2P/optim.py
--rw-r--r--   0 davidblair   (501) staff       (20)    23311 2023-04-26 05:29:45.000000 VAE_G2P-0.0.6/VAE_G2P/vae_g2p.py
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-26 05:32:33.954870 VAE_G2P-0.0.6/VAE_G2P.egg-info/
--rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-26 05:32:33.000000 VAE_G2P-0.0.6/VAE_G2P.egg-info/PKG-INFO
--rw-r--r--   0 davidblair   (501) staff       (20)      331 2023-04-26 05:32:33.000000 VAE_G2P-0.0.6/VAE_G2P.egg-info/SOURCES.txt
--rw-r--r--   0 davidblair   (501) staff       (20)        1 2023-04-26 05:32:33.000000 VAE_G2P-0.0.6/VAE_G2P.egg-info/dependency_links.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       34 2023-04-26 05:32:33.000000 VAE_G2P-0.0.6/VAE_G2P.egg-info/requires.txt
--rw-r--r--   0 davidblair   (501) staff       (20)        8 2023-04-26 05:32:33.000000 VAE_G2P-0.0.6/VAE_G2P.egg-info/top_level.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       38 2023-04-26 05:32:33.955218 VAE_G2P-0.0.6/setup.cfg
--rw-r--r--   0 davidblair   (501) staff       (20)      941 2023-04-05 04:37:12.000000 VAE_G2P-0.0.6/setup.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 17:28:54.017745 VAE_G2P-0.0.7/
+-rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-27 17:28:54.017614 VAE_G2P-0.0.7/PKG-INFO
+-rw-r--r--   0 davidblair   (501) staff       (20)      158 2023-03-05 01:23:50.000000 VAE_G2P-0.0.7/README.md
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 17:28:54.016658 VAE_G2P-0.0.7/VAE_G2P/
+-rw-r--r--   0 davidblair   (501) staff       (20)      130 2023-04-05 04:44:26.000000 VAE_G2P-0.0.7/VAE_G2P/__init__.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    19614 2023-04-05 04:47:05.000000 VAE_G2P-0.0.7/VAE_G2P/basic_g2p.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    13488 2023-04-05 04:47:18.000000 VAE_G2P-0.0.7/VAE_G2P/cvae_model.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    15935 2023-04-27 17:27:13.000000 VAE_G2P-0.0.7/VAE_G2P/data.py
+-rw-r--r--   0 davidblair   (501) staff       (20)     2120 2023-03-30 02:16:44.000000 VAE_G2P-0.0.7/VAE_G2P/data_wrapper.py
+-rw-r--r--   0 davidblair   (501) staff       (20)     9624 2023-03-08 05:48:31.000000 VAE_G2P-0.0.7/VAE_G2P/networks.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    15046 2023-04-05 04:47:50.000000 VAE_G2P-0.0.7/VAE_G2P/optim.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    23311 2023-04-27 17:23:49.000000 VAE_G2P-0.0.7/VAE_G2P/vae_g2p.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 17:28:54.017441 VAE_G2P-0.0.7/VAE_G2P.egg-info/
+-rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-27 17:28:53.000000 VAE_G2P-0.0.7/VAE_G2P.egg-info/PKG-INFO
+-rw-r--r--   0 davidblair   (501) staff       (20)      331 2023-04-27 17:28:53.000000 VAE_G2P-0.0.7/VAE_G2P.egg-info/SOURCES.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)        1 2023-04-27 17:28:53.000000 VAE_G2P-0.0.7/VAE_G2P.egg-info/dependency_links.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       34 2023-04-27 17:28:53.000000 VAE_G2P-0.0.7/VAE_G2P.egg-info/requires.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)        8 2023-04-27 17:28:53.000000 VAE_G2P-0.0.7/VAE_G2P.egg-info/top_level.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       38 2023-04-27 17:28:54.017783 VAE_G2P-0.0.7/setup.cfg
+-rw-r--r--   0 davidblair   (501) staff       (20)      941 2023-04-05 04:37:12.000000 VAE_G2P-0.0.7/setup.py
```

### Comparing `VAE_G2P-0.0.6/VAE_G2P/basic_g2p.py` & `VAE_G2P-0.0.7/VAE_G2P/basic_g2p.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.6/VAE_G2P/cvae_model.py` & `VAE_G2P-0.0.7/VAE_G2P/cvae_model.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.6/VAE_G2P/data.py` & `VAE_G2P-0.0.7/VAE_G2P/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 		all_unique_symptoms=sorted(list(set().union(*orig_symp_values.apply(lambda x:[y[0] for y in x]).values)))
 		self.symptom_map=dict(zip(all_unique_symptoms,range(len(all_unique_symptoms))))
 		self.inverse_symptom_map=dict(zip(self.symptom_map.values(),self.symptom_map.keys()))
 		self.num_symptoms=len(self.symptom_map)
 		
 		self.ordinal_cut_points=np.array(list(ordinal_freq_upperlimits.values()))
 		self.ordinal_freq_map=dict(zip(np.array(list(ordinal_freq_upperlimits.keys()))[np.argsort(self.ordinal_cut_points)],np.arange(self.ordinal_cut_points.shape[0])))
+		self.ordinal_cut_points=np.sort(self.ordinal_cut_points)
 		self.ordinal_freq_map[missing_label]=-1
 		self.num_ordinal_freqs = len(self.ordinal_freq_map)-1
 		self.missing_label=missing_label
 
 		self.gene_info_table=gene_info_table
 		self.symptom_count_prior=symptom_count_prior
```

### Comparing `VAE_G2P-0.0.6/VAE_G2P/data_wrapper.py` & `VAE_G2P-0.0.7/VAE_G2P/data_wrapper.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.6/VAE_G2P/networks.py` & `VAE_G2P-0.0.7/VAE_G2P/networks.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.6/VAE_G2P/optim.py` & `VAE_G2P-0.0.7/VAE_G2P/optim.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.6/VAE_G2P/vae_g2p.py` & `VAE_G2P-0.0.7/VAE_G2P/vae_g2p.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import copy
 
 from .cvae_model import DiseaseCondVAE
 from .basic_g2p import BasicG2PModel
 from .data import GeneToPhenotypeDataset
 from .optim import AutoEncoderOptimizer
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 
 class VAE_G2P:
 
 	def _readModelFromFile(self,fName):
 		with open(fName,'rb') as f:
 			model_dict = torch.load(f,map_location='cpu')
```

### Comparing `VAE_G2P-0.0.6/setup.py` & `VAE_G2P-0.0.7/setup.py`

 * *Files identical despite different names*


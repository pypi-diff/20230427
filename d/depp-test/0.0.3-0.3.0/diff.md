# Comparing `tmp/depp_test-0.0.3.tar.gz` & `tmp/depp_test-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depp_test-0.0.3.tar", last modified: Thu Mar 31 15:15:41 2022, max compression
+gzip compressed data, was "depp_test-0.3.0.tar", last modified: Thu Apr 27 21:38:37 2023, max compression
```

## Comparing `depp_test-0.0.3.tar` & `depp_test-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,48 @@
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2022-03-31 15:15:41.904096 depp_test-0.0.3/
--rw-r--r--   0 yueyu      (501) staff       (20)     1067 2022-03-31 05:54:54.000000 depp_test-0.0.3/LICENSE
--rw-r--r--   0 yueyu      (501) staff       (20)      474 2022-03-31 15:15:41.903874 depp_test-0.0.3/PKG-INFO
--rw-r--r--   0 yueyu      (501) staff       (20)     6292 2022-03-31 05:54:54.000000 depp_test-0.0.3/README.md
--rw-r--r--   0 yueyu      (501) staff       (20)     1941 2022-03-31 06:33:31.000000 depp_test-0.0.3/agg_dist.py
--rw-r--r--   0 yueyu      (501) staff       (20)      577 2022-03-31 06:33:31.000000 depp_test-0.0.3/comb_json.py
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2022-03-31 15:15:41.902743 depp_test-0.0.3/depp/
--rw-r--r--   0 yueyu      (501) staff       (20)     5935 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/Model_new.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5475 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/Model_pl.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5542 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/Model_pl.split.py
--rw-r--r--   0 yueyu      (501) staff       (20)    11426 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/Model_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)        0 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/__init__.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1970 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/data.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2441 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/data.split.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2880 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/data_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1454 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/default_config.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1182 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/depp_distance.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1645 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/distance_correction.py
--rw-r--r--   0 yueyu      (501) staff       (20)     7731 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/submodule.py
--rw-r--r--   0 yueyu      (501) staff       (20)    12237 2022-03-31 06:34:25.000000 depp_test-0.0.3/depp/utils.py
--rw-r--r--   0 yueyu      (501) staff       (20)     4814 2022-03-31 15:13:59.000000 depp_test-0.0.3/depp-place-rRNA-one-type.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     3201 2022-03-31 06:33:17.000000 depp_test-0.0.3/depp-place-rRNA.sh
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2022-03-31 15:15:41.903651 depp_test-0.0.3/depp_test.egg-info/
--rw-r--r--   0 yueyu      (501) staff       (20)      474 2022-03-31 15:15:41.000000 depp_test-0.0.3/depp_test.egg-info/PKG-INFO
--rw-r--r--   0 yueyu      (501) staff       (20)      632 2022-03-31 15:15:41.000000 depp_test-0.0.3/depp_test.egg-info/SOURCES.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        1 2022-03-31 15:15:41.000000 depp_test-0.0.3/depp_test.egg-info/dependency_links.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        1 2022-03-31 15:15:32.000000 depp_test-0.0.3/depp_test.egg-info/not-zip-safe
--rw-r--r--   0 yueyu      (501) staff       (20)      146 2022-03-31 15:15:41.000000 depp_test-0.0.3/depp_test.egg-info/requires.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        5 2022-03-31 15:15:41.000000 depp_test-0.0.3/depp_test.egg-info/top_level.txt
--rw-r--r--   0 yueyu      (501) staff       (20)     1149 2022-03-31 06:33:31.000000 depp_test-0.0.3/merge_json.py
--rwxr-xr-x   0 yueyu      (501) staff       (20)      913 2022-03-31 06:33:17.000000 depp_test-0.0.3/run_upp.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     1346 2022-03-31 06:33:31.000000 depp_test-0.0.3/seq_sep.py
--rw-r--r--   0 yueyu      (501) staff       (20)       38 2022-03-31 15:15:41.904159 depp_test-0.0.3/setup.cfg
--rw-r--r--   0 yueyu      (501) staff       (20)     1634 2022-03-31 15:15:22.000000 depp_test-0.0.3/setup.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2730 2022-03-31 06:33:31.000000 depp_test-0.0.3/train_depp.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2816 2022-03-31 06:33:31.000000 depp_test-0.0.3/train_depp_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5173 2022-03-31 06:33:17.000000 depp_test-0.0.3/wol_placement.sh
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 21:38:37.732454 depp_test-0.3.0/
+-rw-r--r--   0 yueyu      (501) staff       (20)      474 2023-04-27 21:38:37.732217 depp_test-0.3.0/PKG-INFO
+-rw-r--r--   0 yueyu      (501) staff       (20)       15 2022-12-08 05:14:10.000000 depp_test-0.3.0/README.md
+-rw-r--r--   0 yueyu      (501) staff       (20)     1941 2022-12-08 03:54:04.000000 depp_test-0.3.0/agg_dist.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      577 2022-12-08 03:54:04.000000 depp_test-0.3.0/comb_json.py
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 21:38:37.731145 depp_test-0.3.0/depp/
+-rw-r--r--   0 yueyu      (501) staff       (20)     5764 2023-02-01 22:01:10.000000 depp_test-0.3.0/depp/Agg_model.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4909 2023-04-15 21:40:03.000000 depp_test-0.3.0/depp/Agg_model_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     8710 2023-02-01 19:47:27.000000 depp_test-0.3.0/depp/Model_pl.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    11301 2023-04-20 17:57:40.000000 depp_test-0.3.0/depp/Model_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)        0 2022-12-08 03:54:04.000000 depp_test-0.3.0/depp/__init__.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1605 2022-12-23 18:59:14.000000 depp_test-0.3.0/depp/assign_cluster_by_placement.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      526 2022-12-08 09:46:07.000000 depp_test-0.3.0/depp/count_gapped_ratio.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    12673 2023-01-05 06:08:45.000000 depp_test-0.3.0/depp/data.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2431 2022-12-08 03:54:04.000000 depp_test-0.3.0/depp/data.split.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4009 2022-12-08 04:17:46.000000 depp_test-0.3.0/depp/data_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1730 2023-01-05 18:39:30.000000 depp_test-0.3.0/depp/default_config.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2433 2023-04-19 17:27:35.000000 depp_test-0.3.0/depp/depp_distance.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2063 2023-04-19 17:32:01.000000 depp_test-0.3.0/depp/depp_distance_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      766 2022-12-08 09:41:19.000000 depp_test-0.3.0/depp/filter_by_entropy_gap.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)      782 2022-12-08 09:46:07.000000 depp_test-0.3.0/depp/get_names_by_entropy_gap.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      849 2023-04-27 21:34:13.000000 depp_test-0.3.0/depp/get_tree_dist.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      576 2022-12-08 09:46:07.000000 depp_test-0.3.0/depp/grep_jplace.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1008 2022-12-08 09:46:07.000000 depp_test-0.3.0/depp/grep_seq.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      885 2023-04-27 21:33:25.000000 depp_test-0.3.0/depp/grep_seq_group.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      743 2022-12-23 19:57:48.000000 depp_test-0.3.0/depp/select_placement.py
+-rw-------   0 yueyu      (501) staff       (20)      871 2023-04-27 21:32:31.000000 depp_test-0.3.0/depp/select_species_by_distance.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      342 2023-04-27 18:26:24.000000 depp_test-0.3.0/depp/set_bl_one.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     7731 2022-12-08 03:54:04.000000 depp_test-0.3.0/depp/submodule.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    32601 2023-04-19 17:28:16.000000 depp_test-0.3.0/depp/utils.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5802 2023-02-03 22:09:45.000000 depp_test-0.3.0/depp-place-rRNA-one-type.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     6477 2023-02-25 20:07:16.000000 depp_test-0.3.0/depp-place-rRNA.sh
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 21:38:37.731965 depp_test-0.3.0/depp_test.egg-info/
+-rw-r--r--   0 yueyu      (501) staff       (20)      474 2023-04-27 21:38:37.000000 depp_test-0.3.0/depp_test.egg-info/PKG-INFO
+-rw-r--r--   0 yueyu      (501) staff       (20)      934 2023-04-27 21:38:37.000000 depp_test-0.3.0/depp_test.egg-info/SOURCES.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        1 2023-04-27 21:38:37.000000 depp_test-0.3.0/depp_test.egg-info/dependency_links.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        1 2023-04-27 21:37:24.000000 depp_test-0.3.0/depp_test.egg-info/not-zip-safe
+-rw-r--r--   0 yueyu      (501) staff       (20)      154 2023-04-27 21:38:37.000000 depp_test-0.3.0/depp_test.egg-info/requires.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        5 2023-04-27 21:38:37.000000 depp_test-0.3.0/depp_test.egg-info/top_level.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)     1149 2022-12-08 03:54:04.000000 depp_test-0.3.0/merge_json.py
+-rwxr-xr-x   0 yueyu      (501) staff       (20)      912 2022-12-08 03:54:01.000000 depp_test-0.3.0/run_upp.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     2339 2023-02-01 07:34:59.000000 depp_test-0.3.0/seq_sep.py
+-rw-r--r--   0 yueyu      (501) staff       (20)       38 2023-04-27 21:38:37.732530 depp_test-0.3.0/setup.cfg
+-rw-r--r--   0 yueyu      (501) staff       (20)     1994 2023-04-27 21:38:24.000000 depp_test-0.3.0/setup.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     6233 2023-04-27 21:35:33.000000 depp_test-0.3.0/train_cluster_depp.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     4773 2023-02-01 20:15:45.000000 depp_test-0.3.0/train_depp.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5033 2023-04-19 17:48:08.000000 depp_test-0.3.0/train_depp_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5173 2022-12-08 03:54:01.000000 depp_test-0.3.0/wol_placement.sh
```

### Comparing `depp_test-0.0.3/agg_dist.py` & `depp_test-0.3.0/agg_dist.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.0.3/comb_json.py` & `depp_test-0.3.0/comb_json.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.0.3/depp/Model_pl.py` & `depp_test-0.3.0/depp/Model_pl.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from depp import submodule
 from depp import data
 from depp import utils
 from pytorch_lightning.core.lightning import LightningModule
 from torch.utils.data import DataLoader
 from typing import List, Dict, Optional, Callable, Union
 from torch.optim.optimizer import Optimizer
+import numpy as np
 import math
+import omegaconf
 
 
 class encoder(nn.Module):
     def __init__(self, args):
         super(encoder, self).__init__()
         channel = 4
 
@@ -37,116 +39,202 @@
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         bs, channel, seq_length = x.shape
 
         x = self.celu(self.conv(x))
         x = self.resblocks(x)
         x = self.linear(x).squeeze(-1)
-        x = x.view(bs, self.args.embedding_size)
+        x = x.view(bs, -1)
+        return x
+
+class classifier(nn.Module):
+    def __init__(self, args, cluster_num=None):
+        super(classifier, self).__init__()
+        channel = 4
+
+        self.conv = nn.Conv1d(channel, args.h_channel, 1)
+        self.relu = nn.ReLU()
+        self.celu = nn.CELU()
+        resblocks = []
+        for i in range(args.resblock_num):
+            resblocks.append(submodule.resblock(args.h_channel,
+                                                args.h_channel,
+                                                5, 0.3))
+
+        if args.classifier_seqdir is not None:
+            seqdir = args.classifier_seqdir
+        else:
+            seqdir = args.seqdir
+        if cluster_num is None:
+            cluster_num = len([i for i in range(len(os.listdir(seqdir))) if os.path.isfile(f'{seqdir}/{i}.fa')])
+
+        self.resblocks = nn.Sequential(*resblocks)
+
+        self.linear = nn.Conv1d(args.h_channel,
+                                cluster_num,
+                                args.sequence_length)
+        self.args = args
+        self.train_loss = 0
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        bs, channel, seq_length = x.shape
+
+        x = self.celu(self.conv(x))
+        x = self.resblocks(x)
+        x = self.linear(x).squeeze(-1)
+        x = x.view(bs, -1)
         return x
 
 
 class model(LightningModule):
-    def __init__(self, args):
+    def __init__(self, args, current_model):
         super(model, self).__init__()
         self.save_hyperparameters(args)
         if not self.hparams.sequence_length:
             utils.get_seq_length(self.hparams)
-        self.save_hyperparameters(self.hparams)
-        self.encoder = encoder(self.hparams)
+
+        if current_model != -1:
+            embedding_size = self.hparams.embedding_size
+            self.hparams.embedding_size = embedding_size[current_model]
+            self.encoder = encoder(self.hparams)
+            self.hparams.embedding_size = embedding_size
+        else:
+            self.classifier = classifier(self.hparams)
         self.channel = 4
-        self.hparams.distance_ratio = math.sqrt(float(1.0 / float(self.hparams.embedding_size) / 10 * float(self.hparams.distance_alpha)))
+        self.hparams.distance_ratio = math.sqrt(float(1.0 / 128 / 10 * float(self.hparams.distance_alpha)))
 
         self.dis_loss_w = 100
         self.train_loss = []
-        self.val_loss = float('inf') 
+        self.val_loss = float('inf')
 
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        encoding = self.encoder(x)
-        return encoding
+        self.testing = False
+        if current_model == -1:
+            self.training_classifier = True
+        else:
+            self.training_classifier = False
+        self.current_model = current_model
+        self.counting = 0
+
+        self.save_hyperparameters(self.hparams)
+
+    def forward(self, x, model_idx=None) -> torch.Tensor:
+        if self.training_classifier:
+            return self.classifier(x)
+        return self.encoder(x)
 
     def training_step(self, batch, batch_idx):
 
         nodes = batch['nodes']
         seq = batch['seqs'].float()
+        model_idx = batch['cluster_idx'].long()
         device = seq.device
 
-        encoding = self(seq)
-        gt_distance = self.train_data.true_distance(nodes, nodes).to(device)
+        if self.training_classifier:
+            c = self(seq)
+            loss = nn.functional.cross_entropy(c, model_idx)
+            self.val_loss += loss
+            return {'loss': loss}
+        else:
+            encoding = self(seq, model_idx[0])
+            gt_distance = self.train_data.true_distance(nodes, nodes).to(device)
+
+            distance = utils.distance(encoding, encoding.detach(), self.hparams.distance_mode) * self.hparams.distance_ratio
 
-        distance = utils.distance(encoding, encoding.detach(), self.hparams.distance_mode) * self.hparams.distance_ratio
+            not_self = torch.ones_like(distance)
+            not_self[torch.arange(0, len(distance)), torch.arange(0, len(distance))] = 0
 
-        not_self = torch.ones_like(distance)
-        not_self[torch.arange(0, len(distance)), torch.arange(0, len(distance))] = 0
+            dis_loss = utils.mse_loss(distance[not_self == 1], gt_distance[not_self == 1], self.hparams.weighted_method)
+            loss = self.dis_loss_w * dis_loss * self.hparams.dis_loss_ratio
 
-        dis_loss = utils.mse_loss(distance[not_self == 1], gt_distance[not_self == 1], self.hparams.weighted_method)
-        loss = self.dis_loss_w * dis_loss * self.hparams.dis_loss_ratio
-        self.val_loss += loss
+            if loss.isnan().any():
+                breakpoint()
 
-        return {'loss': loss}
+            self.val_loss += loss
+
+            return {'loss': loss}
 
     def training_epoch_end(
             self,
             outputs: Union[List[Dict[str, torch.Tensor]], List[List[Dict[str, torch.Tensor]]]]
     ) -> Dict[str, Dict[str, torch.Tensor]]:
         self.dis_loss_w = 100 + 1e-3 * (self.trainer.current_epoch - 1e4) * (self.trainer.current_epoch > 1e4)
+        self.counting += 1
         if self.trainer.current_epoch % 100 == 0:
-            self.trainer.save_checkpoint(f'{self.hparams.model_dir}/epoch-{self.trainer.current_epoch}.pth')
+            if self.training_classifier:
+                subdir = 'classifier'
+            else:
+                subdir = self.current_model
+            os.makedirs(f'{self.hparams.model_dir}/{subdir}', exist_ok=True)
+            self.trainer.save_checkpoint(f'{self.hparams.model_dir}/{subdir}/epoch-{self.trainer.current_epoch}.pth')
             if self.trainer.current_epoch > 0:
                 try:
-                    os.remove(f'{self.hparams.model_dir}/epoch-{self.trainer.current_epoch - 100}.pth')
+                    os.remove(f'{self.hparams.model_dir}/{subdir}/epoch-{self.trainer.current_epoch - 100}.pth')
                 except:
                     pass
 
     def configure_optimizers(self):
-        return torch.optim.RMSprop(self.parameters(), lr=self.hparams.lr)
+        return torch.optim.Adam(self.parameters(), lr=self.hparams.lr)
 
     def train_dataloader(self) -> DataLoader:
+        # self.train_data = self.train_data_list[0]
         loader = DataLoader(self.train_data,
                             batch_size=self.hparams.batch_size,
                             num_workers=self.hparams.num_worker,
                             shuffle=True,
                             drop_last=True)
         return loader
 
     def validation_step(self, batch, batch_idx):
-        return {}        
+        return {}
 
     def validation_epoch_end(self, outputs):
         val_loss = self.val_loss
         self.val_loss = 0
         self.log('val_loss', val_loss)
 
     def val_dataloader(self):
         # TODO: do a real train/val split
-        self.train_data = data.data(self.hparams, calculate_distance_matrix=True)
+        # self.train_data = data.data(self.hparams, calculate_distance_matrix=True)
+        # self.train_data_list = data.make_datalist(self.hparams)
+        if not self.training_classifier:
+            print(f'training {self.current_model} model...')
+            self.train_data = data.get_data(self.current_model, self.hparams)
+        else:
+            # self.train_data = self.train_data_list[-1]
+            print(f'training classifier...')
+            self.train_data = data.get_data(-1, self.hparams)
         loader = DataLoader(self.train_data,
                             batch_size=self.hparams.batch_size,
                             shuffle=False,
                             num_workers=self.hparams.num_worker,
-                            drop_last=False)
+                            drop_last=True)
         return loader
 
     def optimizer_step(
             self,
             epoch: int,
             batch_idx: int,
             optimizer: Optimizer,
             optimizer_idx: int,
             optimizer_closure: Optional[Callable] = None,
             on_tpu: bool = False,
             using_native_amp: bool = False,
             using_lbfgs: bool = False,
     ) -> None:
 
-        if self.trainer.global_step % self.hparams.lr_update_freq == 0:
-
-            lr = 3e-5 + self.hparams.lr * (0.1 ** (epoch / self.hparams.lr_decay))
+        if self.counting == self.hparams.lr_update_freq:
+            # if (epoch + 1) % self.hparams.lr_decay == 0:
+            # lr = 3e-5 + self.hparams.lr * (0.1 ** ((self.trainer.current_epoch + 1) / self.hparams.lr_decay))
+            # print('lr', lr)
             for param_group in optimizer.param_groups:
-                param_group['lr'] = lr
+                param_group['lr'] = param_group['lr'] * 0.1 + 2e-5
+            print('lr', param_group['lr'])
+            print(self.counting, self.hparams.lr_update_freq)
+            self.counting = 0
+
 
         super(model, self).optimizer_step(
             epoch,
             batch_idx,
             optimizer,
             optimizer_idx,
             optimizer_closure,
```

### Comparing `depp_test-0.0.3/depp/Model_pl.split.py` & `depp_test-0.3.0/depp/Agg_model_recon.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,157 +1,124 @@
 #!/usr/bin/env python3
+import json
 
 import torch
-import os
-import math
 import torch.nn as nn
-from depp import submodule
-from depp import data
 from depp import utils
+from depp import Model_recon
 from pytorch_lightning.core.lightning import LightningModule
 from torch.utils.data import DataLoader
 from typing import List, Dict, Optional, Callable, Union
-from torch.optim.optimizer import Optimizer
+import numpy as np
 import math
-
-
-class encoder(nn.Module):
-    def __init__(self, args):
-        super(encoder, self).__init__()
-        channel = 4
-
-        self.conv = nn.Conv1d(channel, args.h_channel, 1)
-        self.relu = nn.ReLU()
-        self.celu = nn.CELU()
-        resblocks = []
-        for i in range(args.resblock_num):
-            resblocks.append(submodule.resblock(args.h_channel,
-                                                args.h_channel,
-                                                5, 0.3))
-        self.resblocks = nn.Sequential(*resblocks)
-
-        self.linear = nn.Conv1d(args.h_channel,
-                                args.embedding_size,
-                                args.sequence_length)
-        self.args = args
-        self.train_loss = 0
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        bs, channel, seq_length = x.shape
-
-        x = self.celu(self.conv(x))
-        x = self.resblocks(x)
-        x = self.linear(x).squeeze(-1)
-        x = x.view(bs, self.args.embedding_size)
-        return x
+import omegaconf
+import sys
 
 
 class model(LightningModule):
-    def __init__(self, args):
+    def __init__(self, args, load_model=False, classifier_cluster_num=None):
         super(model, self).__init__()
         self.save_hyperparameters(args)
         if not self.hparams.sequence_length:
             utils.get_seq_length(self.hparams)
-        self.save_hyperparameters(self.hparams)
-        self.encoder = encoder(self.hparams)
+        embedding_size = self.hparams.embedding_size
+        self.encoders = []
+        for i in range(self.hparams.cluster_num):
+            if isinstance(self.hparams.embedding_size, omegaconf.listconfig.ListConfig) or \
+                    isinstance(self.hparams.embedding_size, list):
+                self.hparams.embedding_size = embedding_size[i]
+                self.encoders.append(Model_recon.encoder(self.hparams))
+                self.hparams.embedding_size = []
+            else:
+                self.encoders.append(Model_recon.encoder(self.hparams))
+        self.classifier = Model_recon.classifier(self.hparams, cluster_num=classifier_cluster_num)
+
+        if load_model:
+            for i in range(self.hparams.cluster_num):
+                print(f'loading {i} model...')
+                save_epoch_num = self.hparams.epoch - self.hparams.epoch % 100
+                sub_model = Model_recon.model.load_from_checkpoint(
+                    f'{self.hparams.model_dir}/{i}/epoch-{save_epoch_num}.pth', current_model=i)
+                # breakpoint()
+                self.encoders[i].load_state_dict(sub_model.encoder.state_dict(), strict=True)
+            classifier = Model_recon.model.load_from_checkpoint(
+                f'{self.hparams.model_dir}/classifier/epoch-{self.hparams.classifier_epoch - self.hparams.classifier_epoch % 100}.pth', current_model=-1)
+            self.classifier.load_state_dict(classifier.classifier.state_dict(), strict=True)
+
+        self.hparams.embedding_size = embedding_size
+        self.encoders = nn.ModuleList(self.encoders)
         self.channel = 4
-        self.hparams.distance_ratio = math.sqrt(float(1.0 / float(self.hparams.embedding_size) / 10 * float(self.hparams.distance_alpha)))
+        self.hparams.distance_ratio = math.sqrt(float(1.0 / 128 / 10 * float(self.hparams.distance_alpha)))
 
         self.dis_loss_w = 100
         self.train_loss = []
-        self.val_loss = float('inf') 
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        encoding = self.encoder(x)
-        return encoding
-
-    def training_step(self, batch, batch_idx):
+        self.val_loss = float('inf')
 
-        nodes = batch['nodes']
-        seq = batch['seqs'].float()
-        device = seq.device
+        self.testing = False
+        if self.hparams.classifier_epoch == 0:
+            self.training_classifier = False
+            self.current_model = -1
+        else:
+            self.training_classifier = True
+            self.current_model = args.start_model_idx
+        self.counting = 0
+
+        if load_model:
+            with open(args.cluster_corr, 'r') as f:
+                self.hparams.corr_str = f.read()
+        else:
+            corr = json.loads(self.hparams.corr_str)
+            self.corr = {int(i): torch.tensor(corr[i]) for i in corr}
 
-        encoding = self(seq)
-        gt_distance = self.train_data.true_distance(nodes, nodes).to(device)
-
-        distance = utils.distance(encoding, encoding.detach(), self.hparams.distance_mode) * self.hparams.distance_ratio
+        self.save_hyperparameters(self.hparams)
 
-        not_self = torch.ones_like(distance)
-        not_self[torch.arange(0, len(distance)), torch.arange(0, len(distance))] = 0
+    def forward(self, x, model_idx=None, only_class=False) -> torch.Tensor:
+        if self.testing:
+            model_prob = self.classifier(x).softmax(-1)
+            model_prob = torch.stack([model_prob[:, self.corr[i]].max(-1)[0] for i in range(self.hparams.cluster_num)], dim=-1)
+            # model_prob = model_prob / model_prob.sum(-1, keepdims=True)
+            model_idx = model_prob.argmax(-1)
+            if only_class:
+                return model_idx, model_prob
+            result_tmp = [self.encoders[model_idx[i]](x[i].unsqueeze(0)) for i in range(len(x))]
+            result = np.empty(len(result_tmp), dtype=object)
+            result[:] = result_tmp
+            return result, model_idx, model_prob
+        if self.training_classifier:
+            return self.classifier(x)
+        return self.encoders[model_idx](x)
 
-        dis_loss = utils.mse_loss(distance[not_self == 1], gt_distance[not_self == 1], self.hparams.weighted_method)
-        loss = self.dis_loss_w * dis_loss * self.hparams.dis_loss_ratio
-        self.val_loss += loss
+    def configure_optimizers(self):
+        self.trainer.save_checkpoint(
+            f'{self.hparams.model_dir}/cluster-depp.pth')
+        sys.exit()
+
+    def on_epoch_start(self) -> None:
+        # self.trainer.save_checkpoint(
+        #     f'{self.hparams.model_dir}/epoch-agg.pth')
+        sys.exit()
 
-        return {'loss': loss}
+    def training_step(self, batch, batch_idx):
+        pass
 
     def training_epoch_end(
             self,
             outputs: Union[List[Dict[str, torch.Tensor]], List[List[Dict[str, torch.Tensor]]]]
     ) -> Dict[str, Dict[str, torch.Tensor]]:
-        self.dis_loss_w = 100 + 1e-3 * (self.trainer.current_epoch - 1e4) * (self.trainer.current_epoch > 1e4)
-        self.train_data.current_epoch = self.trainer.current_epoch
-        if self.trainer.current_epoch % 100 == 0:
-            self.trainer.save_checkpoint(f'{self.hparams.model_dir}/epoch-{self.trainer.current_epoch}.pth')
-            if self.trainer.current_epoch > 0:
-                try:
-                    os.remove(f'{self.hparams.model_dir}/epoch-{self.trainer.current_epoch - 100}.pth')
-                except:
-                    pass
+        pass
 
     def configure_optimizers(self):
-        return torch.optim.RMSprop(self.parameters(), lr=self.hparams.lr)
+        # self.trainer.save_checkpoint(
+        #     f'{self.hparams.model_dir}/epoch-agg.pth')
+        return None
 
     def train_dataloader(self) -> DataLoader:
-        loader = DataLoader(self.train_data,
-                            batch_size=self.hparams.batch_size,
-                            num_workers=self.hparams.num_worker,
-                            shuffle=True,
-                            drop_last=True)
-        return loader
+        pass
 
     def validation_step(self, batch, batch_idx):
-        return {}        
-
-    def validation_epoch_end(self, outputs):
-        val_loss = self.val_loss
-        self.val_loss = 0
-        self.log('val_loss', val_loss)
+        return {}
 
     def val_dataloader(self):
         # TODO: do a real train/val split
-        self.train_data = data.data(self.hparams, calculate_distance_matrix=True)
-        loader = DataLoader(self.train_data,
-                            batch_size=self.hparams.batch_size,
-                            shuffle=False,
-                            num_workers=self.hparams.num_worker,
-                            drop_last=False)
-        return loader
-
-    def optimizer_step(
-            self,
-            epoch: int,
-            batch_idx: int,
-            optimizer: Optimizer,
-            optimizer_idx: int,
-            optimizer_closure: Optional[Callable] = None,
-            on_tpu: bool = False,
-            using_native_amp: bool = False,
-            using_lbfgs: bool = False,
-    ) -> None:
-
-        if self.trainer.global_step % self.hparams.lr_update_freq == 0:
-
-            lr = 3e-5 + self.hparams.lr * (0.1 ** (epoch / self.hparams.lr_decay))
-            for param_group in optimizer.param_groups:
-                param_group['lr'] = lr
-
-        super(model, self).optimizer_step(
-            epoch,
-            batch_idx,
-            optimizer,
-            optimizer_idx,
-            optimizer_closure,
-            on_tpu,
-            using_native_amp,
-            using_lbfgs,
-        )
+        self.trainer.save_checkpoint(
+            f'{self.hparams.model_dir}/cluster-depp.pth')
+        sys.exit()
```

### Comparing `depp_test-0.0.3/depp/Model_recon.py` & `depp_test-0.3.0/depp/Model_recon.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,53 @@
 #!/usr/bin/env python3
 
 import torch
 import os
 import math
 import torch.nn as nn
 from depp import submodule
-from depp import data_recon
+from depp import data
 from depp import utils
 from pytorch_lightning.core.lightning import LightningModule
 from torch.utils.data import DataLoader
 from typing import List, Dict, Optional, Callable, Union
 from torch.optim.optimizer import Optimizer
 import math
 
+class SeqNet(nn.Module):
+    def __init__(self, args):
+        super(SeqNet, self).__init__()
+        channel = 4
+
+        self.conv = nn.Conv1d(channel, args.h_channel, 1)
+        self.relu = nn.ReLU()
+        self.celu = nn.CELU()
+        resblocks = []
+        for i in range(args.resblock_num):
+            resblocks.append(submodule.resblock(args.h_channel,
+                                                args.h_channel,
+                                                5, 0.3))
+        self.resblocks = nn.Sequential(*resblocks)
+        args.seq_h = int(args.sequence_length * args.seq_h_ratio)
+        self.linear = nn.Conv1d(args.h_channel,
+                                args.seq_h,
+                                args.sequence_length)
+        self.tranconv = nn.ConvTranspose1d(args.seq_h, 4, args.sequence_length)
+        self.args = args
+        self.train_loss = 0
+        print("seq_h", args.seq_h)
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        bs, channel, seq_length = x.shape
+
+        x = self.celu(self.conv(x))
+        x = self.resblocks(x)
+        x = self.celu(self.linear(x))
+        x = self.tranconv(x)
+        return x
 
 class encoder(nn.Module):
     def __init__(self, args):
         super(encoder, self).__init__()
         channel = 4
 
         self.conv = nn.Conv1d(channel, args.h_channel, 1)
@@ -28,258 +59,241 @@
                                                 args.h_channel,
                                                 5, 0.3))
         self.resblocks = nn.Sequential(*resblocks)
 
         self.linear = nn.Conv1d(args.h_channel,
                                 args.embedding_size,
                                 args.sequence_length)
+
+        self.seq_net = SeqNet(args)
+        for param in self.seq_net.parameters():
+            param.requires_grad = False
+
         self.args = args
         self.train_loss = 0
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         bs, channel, seq_length = x.shape
 
+        mask = (x == self.args.gap_encode).all(1).unsqueeze(1).repeat(1, 4, 1)
+        recon_x = self.seq_net(x)
+        softmax_recon_x = torch.softmax(recon_x, dim=1)
+        sorted_softmax = softmax_recon_x.sort(dim=1)[0]
+        valid_sites = ((sorted_softmax[:, -1] / sorted_softmax[:, -2]) > 20).unsqueeze(1).repeat(1, 4, 1)
+        x = x.clone()
+        x[mask & valid_sites] = softmax_recon_x[mask & valid_sites]
+
         x = self.celu(self.conv(x))
         x = self.resblocks(x)
         x = self.linear(x).squeeze(-1)
-        x = x.view(bs, self.args.embedding_size)
+        x = x.view(bs, -1)
         return x
-#
-#
-# class SeqNet(nn.Module):
-#     def __init__(self, args):
-#         super(SeqNet, self).__init__()
-#         self.conv1 = nn.Conv1d(4+1, 8, 1)
-#         self.lstm = nn.LSTM(8, 8, 2, batch_first=True, bidirectional=True)
-#         self.conv2 = nn.Conv1d(16, 4, 1)
-#         self.relu = nn.ReLU()
-#
-#     def forward(self, x):
-#         n, chn, l = x.shape
-#         # idx = torch.zeros(n, l, l).to(x.device)
-#         idx = torch.arange(0, l).to(x.device).view(1, 1, -1).repeat(len(x), 1, 1) * 0.01
-#         # idx[:, torch.arange(0, l), torch.arange(0, l)] = 1
-#         x = torch.cat([x, idx], dim=1)
-#         x = self.relu(self.conv1(x))
-#         x = self.lstm(x.permute(0, 2, 1))
-#         x = self.conv2(x[0].permute(0, 2, 1))
-#         return x
 
-class SeqNet(nn.Module):
-    def __init__(self, args):
-        super(SeqNet, self).__init__()
+class classifier(nn.Module):
+    def __init__(self, args, cluster_num=None):
+        super(classifier, self).__init__()
         channel = 4
 
         self.conv = nn.Conv1d(channel, args.h_channel, 1)
         self.relu = nn.ReLU()
         self.celu = nn.CELU()
         resblocks = []
         for i in range(args.resblock_num):
             resblocks.append(submodule.resblock(args.h_channel,
                                                 args.h_channel,
                                                 5, 0.3))
+
+        if args.classifier_seqdir is not None:
+            seqdir = args.classifier_seqdir
+        else:
+            seqdir = args.seqdir
+        if cluster_num is None:
+            cluster_num = len([i for i in range(len(os.listdir(seqdir))) if os.path.isfile(f'{seqdir}/{i}.fa')])
+
         self.resblocks = nn.Sequential(*resblocks)
-        args.seq_h = int(args.sequence_length * args.seq_h_ratio)
+
         self.linear = nn.Conv1d(args.h_channel,
-                                args.seq_h,
+                                cluster_num,
                                 args.sequence_length)
-        self.tranconv = nn.ConvTranspose1d(args.seq_h, 4, args.sequence_length)
+
+        self.seq_net = SeqNet(args)
+        for param in self.seq_net.parameters():
+            param.requires_grad = False
+
         self.args = args
         self.train_loss = 0
-        print("seq_h", args.seq_h)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         bs, channel, seq_length = x.shape
 
+        mask = (x == self.args.gap_encode).all(1).unsqueeze(1).repeat(1, 4, 1)
+        recon_x = self.seq_net(x)
+        softmax_recon_x = torch.softmax(recon_x, dim=1)
+        sorted_softmax = softmax_recon_x.sort(dim=1)[0]
+        valid_sites = ((sorted_softmax[:, -1] / sorted_softmax[:, -2]) > 20).unsqueeze(1).repeat(1, 4, 1)
+        x = x.clone()
+        x[mask & valid_sites] = softmax_recon_x[mask & valid_sites]
+
         x = self.celu(self.conv(x))
         x = self.resblocks(x)
-        x = self.celu(self.linear(x))
-        x = self.tranconv(x)
+        x = self.linear(x).squeeze(-1)
+        x = x.view(bs, -1)
         return x
 
-# class SeqNet(nn.Module):
-#     def __init__(self, args):
-#         super(SeqNet, self).__init__()
-#         self.encoder = nn.Sequential(
-#             nn.Conv1d(5, 16, 5, stride=2),
-#             nn.ReLU(),
-#             nn.Conv1d(16, 32, 5, stride=2),
-#             nn.ReLU(),
-#             nn.Conv1d(32, 64, 5, stride=2),
-#             nn.ReLU(),
-#             nn.Conv1d(64, 128, 5, stride=2),
-#             nn.ReLU(),
-#             nn.Conv1d(128, 128, 5, stride=2),
-#             nn.ReLU()
-#         )
-#         self.lstm = nn.LSTM(128, 128, 1, batch_first=True, bidirectional=True)
-#         self.decoder = nn.Sequential(
-#             nn.ConvTranspose1d(128*2, 128, 5, stride=2, padding=0, output_padding=0),
-#             nn.ReLU(),
-#             nn.ConvTranspose1d(128, 64, 5, stride=2, padding=0, output_padding=0),
-#             nn.ReLU(),
-#             nn.ConvTranspose1d(64, 32, 5, stride=2, padding=0, output_padding=1),
-#             nn.ReLU(),
-#             nn.ConvTranspose1d(32, 16, 5, stride=2, padding=0, output_padding=0),
-#             nn.ReLU(),
-#             nn.ConvTranspose1d(16, 16, 5, stride=2, padding=0, output_padding=0),
-#             nn.ReLU(),
-#             nn.Conv1d(16, 4, 1)
-#         )
-#         self.L = args.sequence_length
-#
-#     def forward(self, x):
-#         idx = torch.arange(0, self.L).to(x.device).view(1, 1, -1).repeat(len(x), 1, 1) * 0.01
-#                 # idx[:, torch.arange(0, l), torch.arange(0, l)] = 1
-#         x = torch.cat([x, idx], dim=1)
-#         x = self.encoder(x)
-#         x = self.lstm(x.permute(0, 2, 1))
-#         x = self.decoder(x[0].permute(0, 2, 1))
-#         # x = self.decoder(x)
-#         if self.L % 2 == 0:
-#             x = x[:, :, :-1]
-#         return x
-
 class model(LightningModule):
-    def __init__(self, args):
+    def __init__(self, args, current_model):
         super(model, self).__init__()
         self.save_hyperparameters(args)
         if not self.hparams.sequence_length:
             utils.get_seq_length(self.hparams)
-        self.save_hyperparameters(self.hparams)
-        self.encoder = encoder(self.hparams)
+
+        if current_model != -1:
+            embedding_size = self.hparams.embedding_size
+            self.hparams.embedding_size = embedding_size[current_model]
+            self.encoder = encoder(self.hparams)
+            self.hparams.embedding_size = embedding_size
+        else:
+            self.classifier = classifier(self.hparams)
         self.channel = 4
-        self.hparams.distance_ratio = math.sqrt(
-            float(1.0 / float(self.hparams.embedding_size) / 10 * float(self.hparams.distance_alpha)))
+        self.hparams.distance_ratio = math.sqrt(float(1.0 / 128 / 10 * float(self.hparams.distance_alpha)))
 
         self.dis_loss_w = 100
         self.train_loss = []
         self.val_loss = float('inf')
-        self.seq_net = SeqNet(self.hparams)
-        self.running_recon_loss = 0
-        self.reconseq = []
-        self.wrong_site = []
-        self.is_training = True
-        self.cnt = []
 
-    def forward(self, x: torch.Tensor, train_sn=False, mask=None) -> torch.Tensor:
-        recon_x = self.seq_net(x)
-        softmax_recon_x = torch.softmax(recon_x, dim=1)
-        if not train_sn:
-            softmax_recon_x[mask.repeat(1, 4, 1)] = x[mask.repeat(1, 4, 1)]
-        encoding = self.encoder(softmax_recon_x)
-        if self.is_training:
-            return recon_x, encoding
+        self.testing = False
+        if current_model == -1:
+            self.training_classifier = True
         else:
-            return encoding
+            self.training_classifier = False
+        self.current_model = current_model
+        self.counting = 0
+
+        self.save_hyperparameters(self.hparams)
+
+    def forward(self, x, model_idx=None) -> torch.Tensor:
+        if self.training_classifier:
+            return self.classifier(x)
+        return self.encoder(x)
 
     def training_step(self, batch, batch_idx):
+
         nodes = batch['nodes']
         seq = batch['seqs'].float()
-        masked_seq = batch['masked_seqs'].float()
-        mask = batch['mask']
+        model_idx = batch['cluster_idx'].long()
         device = seq.device
 
-        if self.trainer.current_epoch < self.hparams.ae_train_epoch:
-            reconseq, _ = self(masked_seq, train_sn=True)
-            n, chn, l = reconseq.shape
-            reconseq = reconseq.permute(0, 2, 1).reshape(n*l, chn)
-            mask = mask.permute(0, 2, 1).reshape(n*l, -1).squeeze(-1)
-            seq = seq.permute(0, 2, 1).reshape(n*l, chn)
-            loss = nn.functional.cross_entropy(reconseq[mask, :], torch.argmax(seq[mask, :], dim=-1))
-            self.running_recon_loss += loss
-            if self.trainer.current_epoch % 10 == 0:
-                self.reconseq.append(reconseq.flatten())
-                wrong_site = (torch.argmax(reconseq[mask, :], dim=-1) != torch.argmax(seq[mask, :], dim=-1)).sum() / mask.sum()
-                self.wrong_site.append(wrong_site)
+        if self.training_classifier:
+            c = self(seq)
+            loss = nn.functional.cross_entropy(c, model_idx)
+            self.val_loss += loss
+            return {'loss': loss}
         else:
-            _, encoding = self(seq, mask=mask)
+            encoding = self(seq, model_idx[0])
             gt_distance = self.train_data.true_distance(nodes, nodes).to(device)
 
-            distance = utils.distance(encoding, encoding.detach(),
-                                      self.hparams.distance_mode) * self.hparams.distance_ratio
+            distance = utils.distance(encoding, encoding.detach(), self.hparams.distance_mode) * self.hparams.distance_ratio
 
             not_self = torch.ones_like(distance)
             not_self[torch.arange(0, len(distance)), torch.arange(0, len(distance))] = 0
 
             dis_loss = utils.mse_loss(distance[not_self == 1], gt_distance[not_self == 1], self.hparams.weighted_method)
             loss = self.dis_loss_w * dis_loss * self.hparams.dis_loss_ratio
+
+            if loss.isnan().any():
+                breakpoint()
+
             self.val_loss += loss
 
-        return {'loss': loss}
+            return {'loss': loss}
 
     def training_epoch_end(
             self,
             outputs: Union[List[Dict[str, torch.Tensor]], List[List[Dict[str, torch.Tensor]]]]
     ) -> Dict[str, Dict[str, torch.Tensor]]:
         self.dis_loss_w = 100 + 1e-3 * (self.trainer.current_epoch - 1e4) * (self.trainer.current_epoch > 1e4)
+        self.counting += 1
         if self.trainer.current_epoch % 100 == 0:
-            self.trainer.save_checkpoint(f'{self.hparams.model_dir}/epoch-{self.trainer.current_epoch}.pth')
-            #if self.trainer.current_epoch > 0:
-            #    os.remove(f'{self.hparams.model_dir}/epoch-{self.trainer.current_epoch - 100}.pth')
-    def on_train_epoch_start(self):
-        if self.trainer.current_epoch == self.hparams.ae_train_epoch:
-            self.seq_net.requires_grad_(False)
-            self.train_data.train_encoder = False
-
+            if self.training_classifier:
+                subdir = 'classifier'
+            else:
+                subdir = self.current_model
+            os.makedirs(f'{self.hparams.model_dir}/{subdir}', exist_ok=True)
+            self.trainer.save_checkpoint(f'{self.hparams.model_dir}/{subdir}/epoch-{self.trainer.current_epoch}.pth')
+            if self.trainer.current_epoch > 0:
+                try:
+                    os.remove(f'{self.hparams.model_dir}/{subdir}/epoch-{self.trainer.current_epoch - 100}.pth')
+                except:
+                    pass
 
     def configure_optimizers(self):
-        return torch.optim.RMSprop(self.parameters(), lr=self.hparams.lr)
+        if self.current_model == -1:
+            params = list(self.classifier.conv.parameters()) + list(self.classifier.resblocks.parameters()) + list(self.classifier.linear.parameters())
+        else:
+            params = list(self.encoder.conv.parameters()) + list(self.encoder.resblocks.parameters()) + list(self.encoder.linear.parameters())
+        return torch.optim.Adam(params,
+                                lr=self.hparams.lr)
 
     def train_dataloader(self) -> DataLoader:
+        # self.train_data = self.train_data_list[0]
         loader = DataLoader(self.train_data,
                             batch_size=self.hparams.batch_size,
                             num_workers=self.hparams.num_worker,
                             shuffle=True,
                             drop_last=True)
         return loader
 
     def validation_step(self, batch, batch_idx):
         return {}
 
     def validation_epoch_end(self, outputs):
         val_loss = self.val_loss
-        if self.trainer.current_epoch > 0 and self.trainer.current_epoch < self.hparams.ae_train_epoch:
-            # self.logger.experiment.add_scalar('recon_loss', self.running_recon_loss, self.trainer.current_epoch)
-            # self.logger.experiment.add_histogram('recon_seq', torch.sigmoid(torch.cat(self.reconseq)), self.trainer.current_epoch)
-            # self.logger.experiment.add_histogram('wrong_site', torch.tensor(self.wrong_site), self.trainer.current_epoch)
-            self.running_recon_loss = 0
-            self.reconseq = []
-            self.wrong_site = []
-        self.log('val_loss', val_loss)
         self.val_loss = 0
+        self.log('val_loss', val_loss)
 
     def val_dataloader(self):
         # TODO: do a real train/val split
-        self.train_data = data_recon.data(self.hparams, calculate_distance_matrix=True)
+        # self.train_data = data.data(self.hparams, calculate_distance_matrix=True)
+        # self.train_data_list = data.make_datalist(self.hparams)
+        if not self.training_classifier:
+            print(f'training {self.current_model} model...')
+            self.train_data = data.get_data(self.current_model, self.hparams)
+        else:
+            # self.train_data = self.train_data_list[-1]
+            print(f'training classifier...')
+            self.train_data = data.get_data(-1, self.hparams)
         loader = DataLoader(self.train_data,
                             batch_size=self.hparams.batch_size,
                             shuffle=False,
                             num_workers=self.hparams.num_worker,
-                            drop_last=False)
+                            drop_last=True)
         return loader
 
     def optimizer_step(
             self,
             epoch: int,
             batch_idx: int,
             optimizer: Optimizer,
             optimizer_idx: int,
             optimizer_closure: Optional[Callable] = None,
             on_tpu: bool = False,
             using_native_amp: bool = False,
             using_lbfgs: bool = False,
     ) -> None:
 
-        if self.trainer.global_step % self.hparams.lr_update_freq == 0:
-
-            #lr = 3e-5 + self.hparams.lr * (0.1 ** (epoch / self.hparams.lr_decay))
-            lr = 3e-5 + self.hparams.lr * (0.1 ** (epoch / self.hparams.lr_decay))
+        if self.counting == self.hparams.lr_update_freq:
+            # if (epoch + 1) % self.hparams.lr_decay == 0:
+            # lr = 3e-5 + self.hparams.lr * (0.1 ** ((self.trainer.current_epoch + 1) / self.hparams.lr_decay))
+            # print('lr', lr)
             for param_group in optimizer.param_groups:
-                param_group['lr'] = lr
+                param_group['lr'] = param_group['lr'] * 0.1 + 2e-5
+            print('lr', param_group['lr'])
+            print(self.counting, self.hparams.lr_update_freq)
+            self.counting = 0
+
 
         super(model, self).optimizer_step(
             epoch,
             batch_idx,
             optimizer,
             optimizer_idx,
             optimizer_closure,
```

### Comparing `depp_test-0.0.3/depp/data.py` & `depp_test-0.3.0/depp/data.split.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import os
 import torch
 import treeswift
 import numpy as np
 import pandas as pd
-from depp import utils
+import utils
 from torch.utils.data import Dataset
 from operator import itemgetter
 from Bio import SeqIO
 
 class data(Dataset):
     def __init__(self, args, calculate_distance_matrix=False):
         self.args = args
@@ -31,23 +31,33 @@
             self.distance_matrix = tree.distance_matrix(leaf_labels=True)
             for key in self.distance_matrix:
                 self.distance_matrix[key][key] = 0
             self.distance_matrix = pd.DataFrame.from_dict(self.distance_matrix)
             print('Finish distance matrix calculation!')
         self.nodes, self.seq = utils.process_seq(self_seq, args, True)
         self.seq = dict(zip(self.nodes, self.seq))
+        self.split = False
+        self.current_epoch = 0
+        self.cur_idx = 0
+        if len(self.nodes) > 10_000:
+            self.split = True
+            idx = np.random.choice(len(self.nodes), replace=False, size=len(self.nodes))
+            self.all_nodes = np.array(self.nodes)[idx]
+            self.nodes = self.all_nodes[:2000]
 
     def true_distance(self, nodes1, nodes2):
         # gt_distance_list = itemgetter(*nodes1)(self.distance_matrix)
         # gt_distance = [torch.tensor(itemgetter(*nodes2)(item)).view(1, len(nodes2)) for item in gt_distance_list]
         # gt_distance = torch.cat(gt_distance, dim=0)
         gt_distance = self.distance_matrix.loc[nodes1][nodes2]
         return torch.from_numpy(gt_distance.values)
 
     def __getitem__(self, idx):
+        if self.split and (self.current_epoch + 1) % 2000 == 0:
+            self.nodes = self.all_nodes[:self.current_epoch+2000]
         sample = {}
         node_name = self.nodes[idx]
         seq = self.seq[node_name]
         sample['seqs'] = seq
         sample['nodes'] = node_name
         return sample
```

### Comparing `depp_test-0.0.3/depp/data_recon.py` & `depp_test-0.3.0/depp/data_recon.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 from depp import utils
 import numpy as np
 import pandas as pd
 from torch.utils.data import Dataset
 from operator import itemgetter
 from Bio import SeqIO
 
+
 class data(Dataset):
     def __init__(self, args, calculate_distance_matrix=False):
         self.args = args
         print('Loding data...')
         backbone_tree_file = args.backbone_tree_file
         backbone_seq_file = args.backbone_seq_file
         self_seq = SeqIO.to_dict(SeqIO.parse(backbone_seq_file, "fasta"))
         tree = treeswift.read_tree(backbone_tree_file, 'newick')
 
-#        self.nodes = list(self_seq.keys())
+        #        self.nodes = list(self_seq.keys())
 
         print('finish data loading!')
 
         args.sequence_length = len(list(self_seq.values())[0])
         L = args.sequence_length
 
         if calculate_distance_matrix:
@@ -34,14 +35,15 @@
             self.distance_matrix = pd.DataFrame.from_dict(self.distance_matrix)
             print('Finish distance matrix calculation!')
 
         self.nodes, self.seq, self.mask = utils.process_seq(self_seq, args, True, True)
         self.seq = dict(zip(self.nodes, self.seq))
         self.nongaps = dict(zip(self.nodes, self.mask))
         self.num = len(self.nodes)
+        self.train_recon = True
 
     def true_distance(self, nodes1, nodes2):
         # gt_distance_list = itemgetter(*nodes1)(self.distance_matrix)
         # gt_distance = [torch.tensor(itemgetter(*nodes2)(item)).view(1, len(nodes2)) for item in gt_distance_list]
         # gt_distance = torch.cat(gt_distance, dim=0)
         gt_distance = self.distance_matrix.loc[nodes1][nodes2]
         return torch.from_numpy(gt_distance.values)
@@ -50,28 +52,48 @@
         sample = {}
         node_name = self.nodes[idx]
         seq = self.seq[node_name]
         sample['seqs'] = seq
         sample['nodes'] = node_name
         nongap = torch.arange(seq.shape[-1])
         nongap = nongap[self.nongaps[node_name][0]]
-        if len(nongap)/seq.shape[-1] > 0.3:
-            p = np.random.rand() * (len(nongap)/seq.shape[-1] - 0.3)
-            method = np.random.choice([0, 1])
-            size = int(p * seq.shape[-1])
-            if method == 1:
-                start = np.random.choice(nongap)
-                mask = torch.ones(1, seq.shape[-1])
-                mask[:, start: start + size] = 0
-            elif method == 0:
-                mask_site = np.random.choice(nongap, size=size)
-                mask = torch.ones(1, seq.shape[-1])
-                mask[:, mask_site] = 0
+        if self.train_recon:
+            if len(nongap) / seq.shape[-1] > 0.3:
+                p = np.random.rand() * (len(nongap) / seq.shape[-1] - 0.3)
+                method = np.random.choice([0, 1])
+                size = int(p * seq.shape[-1])
+                if method == 1:
+                    start = np.random.choice(nongap)
+                    mask = torch.ones(1, seq.shape[-1])
+                    mask[:, start: start + size] = 0
+                elif method == 0:
+                    mask_site = np.random.choice(nongap, size=size)
+                    mask = torch.ones(1, seq.shape[-1])
+                    mask[:, mask_site] = 0
+            else:
+                mask = torch.ones_like(seq)
+            sample['mask'] = self.nongaps[node_name]
         else:
-            mask = torch.ones_like(seq)
-        sample['masked_seqs'] = mask * seq
-        sample['mask'] = self.nongaps[node_name]
+            if len(nongap) / seq.shape[-1] > 0.3:
+                p = np.random.rand() * (len(nongap) / seq.shape[-1] * 0.4)
+                method = np.random.choice([0, 1, 2], p=[0.6, 0.3, 0.1])
+                size = int(p * seq.shape[-1])
+                if method == 1:
+                    start = np.random.choice(nongap)
+                    mask = torch.ones(1, seq.shape[-1])
+                    mask[:, start: start + size] = 0
+                elif method == 2:
+                    mask_site = np.random.choice(nongap, size=size)
+                    mask = torch.ones(1, seq.shape[-1])
+                    mask[:, mask_site] = 0
+                elif method == 0:
+                    mask = torch.ones(1, seq.shape[-1])
+            else:
+                mask = torch.ones(1, seq.shape[-1])
+            sample['mask'] = self.nongaps[node_name] * (mask != 0)
+        # sample['masked_seqs'] = mask * seq
+        sample['masked_seqs'] = seq
+        sample['masked_seqs'][(mask != 1).repeat(4, 1)] = self.args.gap_encode
         return sample
 
     def __len__(self):
         return self.num
-
```

### Comparing `depp_test-0.0.3/depp/default_config.py` & `depp_test-0.3.0/depp/default_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 default_config = \
 {'exp_name': '',
 'data_dir': '',
 'summary_dir': 'summary',
 'model_dir': 'model',
 'distance_mode': 'L2',
-'embedding_size': -1,
+'embedding_size': None,
 'sequence_length': 0,
 'h_channel': 8,
 'beta_ratio': 50000,
 
 'tau_pres_end_epoch': 5,
 'start_epoch': 0,
 'epoch': 5001,
 'batch_size': 32,
 'cp': 1.0,
 'resblock_num': 1,
 
 'lr': 1e-4,
 'lr_decay': 2000,
-'backbone_tree_file': '',
-'backbone_seq_file': '',
+'backbone_tree_file': None,
+'backbone_seq_file': None,
 'query_seq_file': '',
 'weighted_method': 'square_root_fm',
-'distance_alpha': 1e7,
+'distance_alpha': 1e5,
 'dis_loss_ratio': 1.0,
 'plot_freq': 1000,
 'save_data_freq': 1000,
 'save_model_freq': 3000,
 'print_freq': 1000,
 'stop_par': 200,
 'gpus': [0],
 'plot_all_freqdistance_depp.sh -q ./seq/query_seq/query_seq.fa -b ./seq/backbone_seq/backbone_seq.fa -m model/epoch\=599.ckpt -t tree/backbone_tree/backbone.newick -o dis_mat/': 2000,
-'lr_update_freq': 100,
+'lr_update_freq': 500,
 'bar_update_freq': 1,
 'patience': 500000,
 'model_path': '',
 'outdir': 'depp_distance',
 'num_worker': 4,
 'replicate_seq': False,
 'gap_encode': 0.25,
@@ -45,15 +45,27 @@
 'val_freq': 50000000,
 'ae_train_epoch': 300,
 'seq_h_ratio': 0.5,
 'backbone_emb': None,
 'backbone_gap': None,
 'backbone_id': None,
 'recon_backbone_emb':None,
-'load_model': None
+'load_model': None,
+'add_random_mask': False,
+'get_representative_emb': False,
+'start_model_idx': -1,
+'only_class': False,
+'end_model_idx': None,
+'cluster_num': 1,
+'seqdir': None,
+'use_cluster': None,
+'classifier_seqdir': None,
+'use_multi_class': None,
+'prob_thr': 5,
+'cluster_corr': None
 }
 
 #def get_cfg_defaults():
 #    """Get a yacs CfgNode object with default values for my_project."""
 #    # Return a clone so that the defaults will not be altered
 #    # This is for the "local variable" use pattern
 #    return _C.clone()
```

### Comparing `depp_test-0.0.3/depp/submodule.py` & `depp_test-0.3.0/depp/submodule.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.0.3/merge_json.py` & `depp_test-0.3.0/merge_json.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.0.3/run_upp.sh` & `depp_test-0.3.0/run_upp.sh`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 if [ -z "${4+x}" ]
 then
   run_upp.py -s ${3}/${1}.fa -a ${2}/${1}_a.fasta -t ${3}/${1}/backbone_ml.nwk -A 100 -d ${3}/${1} -d ${3}/${1} -p ${3}/${1}
 else
   run_upp.py -s ${3}/${1}.fa -a ${2}/${1}_a.fasta -t ${3}/${1}/backbone_ml.nwk -A 100 -d ${3}/${1} -x $4 -d ${3}/${1} -p ${3}/${1}
 fi
 grep -w -A 1 -f ${3}/${1}/ref_ids.txt ${3}/${1}/output_alignment_masked.fasta --no-group-separator > ${3}/${1}_aligned.fa
-#rm -rf ${3}/${1}
+rm -rf ${3}/${1}
 fi
```

### Comparing `depp_test-0.0.3/setup.py` & `depp_test-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 from setuptools import setup,find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
 	name='depp_test',    # This is the name of your PyPI-package.
-        version='0.0.3',    # Update the version number for new releases
+        version='0.3.0',    # Update the version number for new releases
         scripts=['train_depp.py',
-                 #'distance_depp.sh',
                  'depp/depp_distance.py',
-                 'depp/distance_correction.py',
                  'agg_dist.py',
                  'wol_placement.sh',
                  'run_upp.sh',
                  'merge_json.py',
 		 'train_depp_recon.py',
                  'depp-place-rRNA.sh',
                  'depp-place-rRNA-one-type.sh',
                  'comb_json.py',
-                 'seq_sep.py'], # The name of your scipt, and also the command you'll be using for calling it
+                 'seq_sep.py',
+                 'depp/filter_by_entropy_gap.sh',
+                 'depp/grep_seq.py',
+                 'depp/get_names_by_entropy_gap.py',
+                 'depp/grep_jplace.py',
+                 'depp/count_gapped_ratio.py',
+                 'depp/set_bl_one.py',
+                 'depp/grep_seq_group.py',
+                 'depp/get_tree_dist.py',
+                 'depp/select_species_by_distance.py',
+                 'train_cluster_depp.sh'], # The name of your scipt, and also the command you'll be using for calling it
         description='DEPP: Deep Learning Enables Extending Species Trees using Single Genes',
         long_description='DEPP is a deep-learning-based tool for phylogenetic placement.'
                          'Output of the tool is the distance matrix between the query sequences and the backbone sequences',
         long_description_content_type='text/plain',
         url='https://github.com/yueyujiang/DEPP',
         author='Yueyu Jiang',
         author_email='y5jiang@ucsd.edu',
         packages=find_packages(),
         zip_safe = False,
-        install_requires=['numpy==1.19.1',
+        install_requires=[
+			'numpy==1.22.3',
 			'treeswift==1.1.19',
-			#'torch==1.7.1',
-			'torch>=1.3,<=1.7.1',
-			'pandas==1.3.0',
-			'pytorch-lightning==1.0.5',
+			'torch==1.11.0',
+			'pandas==1.4.2',
+			'pytorch-lightning==1.5.4',
 			'biopython==1.79',
 			'omegaconf==2.1.0',
 			'apples',
+			'scipy==1.7.3',
 			'dendropy==4.5.2'
 			],
         include_package_data=True
 )
```

### Comparing `depp_test-0.0.3/train_depp.py` & `depp_test-0.3.0/train_depp_recon.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-#!/calab_data/mirarab/home/yueyu/miniconda3/envs/depp_env/bin/python
+#!/usr/bin/env python3
 
 import os
-from depp import Model_pl
+import torch
 from depp import default_config
 import pkg_resources
+from depp import Agg_model_recon
+from depp import Model_recon
 
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 from pytorch_lightning.callbacks import ModelCheckpoint
 
 from pytorch_lightning.loggers import TensorBoardLogger
 from omegaconf import OmegaConf
 
 
-#os.environ['OMP_NUM_THREADS'] = '1'
-#os.environ['MKL_NUM_THREADS'] = '1'
+# os.environ['OMP_NUM_THREADS'] = '1'
+# os.environ['MKL_NUM_THREADS'] = '1'
 
 def main():
     args_base = OmegaConf.create(default_config.default_config)
 
     args_cli = OmegaConf.from_cli()
 
     # if args_cli.config_file is not None:
@@ -28,62 +30,115 @@
     # elif args_cli.exp_name is None:
     #     raise ValueError('exp_name cannot be empty without specifying a config file')
     # del args_cli['config_file']
     args = OmegaConf.merge(args_base, args_cli)
 
     model_dir = args.model_dir
     os.makedirs(model_dir, exist_ok=True)
-
-    if args.load_model is not None:
-        model = Model_pl.model.load_from_checkpoint(args.load_model, args=args)
-    else:
-        model = Model_pl.model(args=args)    
-
     early_stop_callback = EarlyStopping(
         monitor='val_loss',
         min_delta=0.00,
         patience=args.patience,
         verbose=False,
         mode='min'
     )
 
     checkpoint_callback = ModelCheckpoint(
-        filepath=model_dir,
+        dirpath=model_dir,
         save_top_k=1,
         verbose=True,
         monitor='val_loss',
         mode='min',
-        prefix=''
     )
     print(model_dir)
-    if args.gpus == 0:
-        trainer = pl.Trainer(
-            logger=False,
-            gpus=args.gpus,
-            progress_bar_refresh_rate=args.bar_update_freq,
-            check_val_every_n_epoch=args.val_freq,
-            max_epochs=args.epoch,
-            gradient_clip_val=args.cp,
-            benchmark=True,
-            callbacks=[early_stop_callback],
-            checkpoint_callback=checkpoint_callback,
-            # reload_dataloaders_every_epoch=True
-        )
+
+    if args.backbone_tree_file is not None and args.cluster_num == 1:
+        args.start_model_idx = 0
+        args.end_model_idx = 1
+    # trainer.fit(model)
+    if args.end_model_idx is None:
+        args.end_model_idx = args.cluster_num
+    if args.start_model_idx == -1:
+        if args.gpus == 0:
+            classifier_trainer = pl.Trainer(
+                logger=False,
+                gpus=args.gpus,
+                # progress_bar_refresh_rate=args.bar_update_freq,
+                check_val_every_n_epoch=args.val_freq,
+                max_epochs=args.classifier_epoch + 1,
+                gradient_clip_val=args.cp,
+                benchmark=True,
+                callbacks=[early_stop_callback],
+                enable_checkpointing=checkpoint_callback
+            )
+        else:
+            classifier_trainer = pl.Trainer(
+                logger=False,
+                gpus=args.gpus,
+                # progress_bar_refresh_rate=args.bar_update_freq,
+                strategy='ddp',
+                check_val_every_n_epoch=args.val_freq,
+                max_epochs=args.classifier_epoch + 1,
+                gradient_clip_val=args.cp,
+                benchmark=True,
+                callbacks=[early_stop_callback],
+                enable_checkpointing=checkpoint_callback
+            )
+
+        model = Model_recon.model(args=args, current_model=-1)
+        model.classifier.seq_net.load_state_dict(torch.load(f'{args.model_dir}/seq_net_params.pt'), strict=True)
+
+        classifier_trainer.fit(model)
+        args.start_model_idx = 0
+
+    for model_idx in range(args.start_model_idx, args.end_model_idx):
+        if args.gpus == 0:
+            trainer = pl.Trainer(
+                logger=False,
+                gpus=args.gpus,
+                # progress_bar_refresh_rate=args.bar_update_freq,
+                check_val_every_n_epoch=args.val_freq,
+                max_epochs=args.epoch + 1,
+                gradient_clip_val=args.cp,
+                benchmark=True,
+                callbacks=[early_stop_callback],
+                enable_checkpointing=checkpoint_callback
+            )
+        else:
+            trainer = pl.Trainer(
+                logger=False,
+                gpus=args.gpus,
+                # progress_bar_refresh_rate=args.bar_update_freq,
+                strategy='ddp',
+                check_val_every_n_epoch=args.val_freq,
+                max_epochs=args.epoch + 1,
+                gradient_clip_val=args.cp,
+                benchmark=True,
+                callbacks=[early_stop_callback],
+                enable_checkpointing=checkpoint_callback
+            )
+
+        model = Model_recon.model(args=args, current_model=model_idx)
+        model.encoder.seq_net.load_state_dict(torch.load(f'{args.model_dir}/seq_net_params.pt'), strict=True)
+
+        trainer.fit(model)
+
+    if args.backbone_tree_file is not None and args.cluster_num == 1:
+        os.rename(f'{args.model_dir}/0/epoch-{args.epoch - args.epoch % 100}.pth', f'{args.model_dir}/depp-model.pth')
     else:
+        model = Agg_model_recon.model(args=args, load_model=True)
         trainer = pl.Trainer(
             logger=False,
             gpus=args.gpus,
             progress_bar_refresh_rate=args.bar_update_freq,
-            distributed_backend='ddp',
+            # distributed_backend='ddp',
             check_val_every_n_epoch=args.val_freq,
-            max_epochs=args.epoch,
+            max_epochs=1,
             gradient_clip_val=args.cp,
-            benchmark=True,
-            callbacks=[early_stop_callback],
-            checkpoint_callback=checkpoint_callback,
+            benchmark=True
             # reload_dataloaders_every_epoch=True
         )
+        trainer.fit(model)
 
-    trainer.fit(model)
 
 if __name__ == '__main__':
     main()
```

### Comparing `depp_test-0.0.3/wol_placement.sh` & `depp_test-0.3.0/wol_placement.sh`

 * *Files identical despite different names*


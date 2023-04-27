# Comparing `tmp/move-dl-1.4.7.tar.gz` & `tmp/move-dl-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "move-dl-1.4.7.tar", last modified: Tue Mar 14 14:47:28 2023, max compression
+gzip compressed data, was "move-dl-1.4.8.tar", last modified: Thu Apr 27 12:12:26 2023, max compression
```

## Comparing `move-dl-1.4.7.tar` & `move-dl-1.4.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.509054 move-dl-1.4.7/
--rw-rw-rw-   0        0        0     1102 2022-03-24 14:38:38.000000 move-dl-1.4.7/LICENSE
--rw-rw-rw-   0        0        0      118 2022-05-24 08:52:38.000000 move-dl-1.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0      466 2023-03-14 14:47:28.509836 move-dl-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     4208 2023-02-28 16:09:27.000000 move-dl-1.4.7/README.md
--rw-rw-rw-   0        0        0      167 2022-11-22 12:49:29.000000 move-dl-1.4.7/pyproject.toml
--rw-rw-rw-   0        0        0      786 2023-03-14 14:47:28.524638 move-dl-1.4.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.330081 move-dl-1.4.7/src/
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.350612 move-dl-1.4.7/src/move/
--rw-rw-rw-   0        0        0      303 2023-03-14 14:46:43.000000 move-dl-1.4.7/src/move/__init__.py
--rw-rw-rw-   0        0        0     1302 2023-02-01 12:15:14.000000 move-dl-1.4.7/src/move/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.356016 move-dl-1.4.7/src/move/analysis/
--rw-rw-rw-   0        0        0      166 2022-11-22 12:49:29.000000 move-dl-1.4.7/src/move/analysis/__init__.py
--rw-rw-rw-   0        0        0     2846 2023-03-10 10:19:51.000000 move-dl-1.4.7/src/move/analysis/metrics.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.362868 move-dl-1.4.7/src/move/conf/
--rw-rw-rw-   0        0        0       69 2022-11-07 16:12:48.000000 move-dl-1.4.7/src/move/conf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.364870 move-dl-1.4.7/src/move/conf/data/
--rw-rw-rw-   0        0        0     1044 2022-11-22 13:40:00.000000 move-dl-1.4.7/src/move/conf/data/base_data.yaml
--rw-rw-rw-   0        0        0      422 2022-11-22 12:49:29.000000 move-dl-1.4.7/src/move/conf/main.yaml
--rw-rw-rw-   0        0        0     6274 2023-01-05 22:52:18.000000 move-dl-1.4.7/src/move/conf/schema.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.379673 move-dl-1.4.7/src/move/conf/task/
--rw-rw-rw-   0        0        0      524 2022-11-07 16:12:48.000000 move-dl-1.4.7/src/move/conf/task/analyze_latent.yaml
--rw-rw-rw-   0        0        0      580 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/conf/task/identify_associations_bayes.yaml
--rw-rw-rw-   0        0        0      589 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/conf/task/identify_associations_ttest.yaml
--rw-rw-rw-   0        0        0      490 2023-01-05 22:32:25.000000 move-dl-1.4.7/src/move/conf/task/tune_model_reconstruction.yaml
--rw-rw-rw-   0        0        0      500 2023-01-05 22:32:25.000000 move-dl-1.4.7/src/move/conf/task/tune_model_stability.yaml
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.390675 move-dl-1.4.7/src/move/core/
--rw-rw-rw-   0        0        0      137 2022-11-22 12:49:29.000000 move-dl-1.4.7/src/move/core/__init__.py
--rw-rw-rw-   0        0        0     1316 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/core/logging.py
--rw-rw-rw-   0        0        0      530 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/core/seed.py
--rw-rw-rw-   0        0        0      341 2022-11-07 16:12:48.000000 move-dl-1.4.7/src/move/core/typing.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.405262 move-dl-1.4.7/src/move/data/
--rw-rw-rw-   0        0        0       78 2022-11-07 16:12:48.000000 move-dl-1.4.7/src/move/data/__init__.py
--rw-rw-rw-   0        0        0     6949 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/data/dataloaders.py
--rw-rw-rw-   0        0        0     5286 2022-11-22 13:40:00.000000 move-dl-1.4.7/src/move/data/io.py
--rw-rw-rw-   0        0        0     3849 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/data/perturbations.py
--rw-rw-rw-   0        0        0     2646 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/data/preprocessing.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.409778 move-dl-1.4.7/src/move/models/
--rw-rw-rw-   0        0        0       54 2022-05-24 08:52:38.000000 move-dl-1.4.7/src/move/models/__init__.py
--rw-rw-rw-   0        0        0    26994 2023-02-01 12:16:59.000000 move-dl-1.4.7/src/move/models/vae.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.423654 move-dl-1.4.7/src/move/tasks/
--rw-rw-rw-   0        0        0      326 2022-11-09 12:50:46.000000 move-dl-1.4.7/src/move/tasks/__init__.py
--rw-rw-rw-   0        0        0    10027 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/tasks/analyze_latent.py
--rw-rw-rw-   0        0        0     1913 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/tasks/encode_data.py
--rw-rw-rw-   0        0        0    13356 2023-02-24 14:23:45.000000 move-dl-1.4.7/src/move/tasks/identify_associations.py
--rw-rw-rw-   0        0        0     8952 2023-03-14 14:46:43.000000 move-dl-1.4.7/src/move/tasks/tune_model.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.428499 move-dl-1.4.7/src/move/training/
--rw-rw-rw-   0        0        0        0 2023-01-05 22:41:07.000000 move-dl-1.4.7/src/move/training/__init__.py
--rw-rw-rw-   0        0        0     3504 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/training/training_loop.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.446714 move-dl-1.4.7/src/move/visualization/
--rw-rw-rw-   0        0        0      750 2022-11-17 16:27:56.000000 move-dl-1.4.7/src/move/visualization/__init__.py
--rw-rw-rw-   0        0        0     6759 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/visualization/feature_importance.py
--rw-rw-rw-   0        0        0     3689 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/visualization/latent_space.py
--rw-rw-rw-   0        0        0     1279 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/visualization/loss_curves.py
--rw-rw-rw-   0        0        0     1860 2023-01-07 01:19:48.000000 move-dl-1.4.7/src/move/visualization/metrics.py
--rw-rw-rw-   0        0        0     1340 2022-11-07 16:12:48.000000 move-dl-1.4.7/src/move/visualization/style.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:47:28.507190 move-dl-1.4.7/src/move_dl.egg-info/
--rw-rw-rw-   0        0        0      466 2023-03-14 14:47:28.000000 move-dl-1.4.7/src/move_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2023-03-14 14:47:28.000000 move-dl-1.4.7/src/move_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 14:47:28.000000 move-dl-1.4.7/src/move_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-14 14:47:28.000000 move-dl-1.4.7/src/move_dl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2023-03-14 14:47:28.000000 move-dl-1.4.7/src/move_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-14 14:47:28.000000 move-dl-1.4.7/src/move_dl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:26.184743 move-dl-1.4.8/
+-rw-rw-rw-   0        0        0     1102 2022-03-24 14:38:38.000000 move-dl-1.4.8/LICENSE
+-rw-rw-rw-   0        0        0      118 2022-05-24 08:52:38.000000 move-dl-1.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      466 2023-04-27 12:12:26.184958 move-dl-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4208 2023-04-27 10:53:04.000000 move-dl-1.4.8/README.md
+-rw-rw-rw-   0        0        0      167 2022-11-22 12:49:29.000000 move-dl-1.4.8/pyproject.toml
+-rw-rw-rw-   0        0        0      786 2023-04-27 12:12:26.187741 move-dl-1.4.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:25.953396 move-dl-1.4.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:25.986572 move-dl-1.4.8/src/move/
+-rw-rw-rw-   0        0        0      303 2023-04-27 12:11:37.000000 move-dl-1.4.8/src/move/__init__.py
+-rw-rw-rw-   0        0        0     1302 2023-04-26 12:47:53.000000 move-dl-1.4.8/src/move/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:25.991578 move-dl-1.4.8/src/move/analysis/
+-rw-rw-rw-   0        0        0      166 2022-11-22 12:49:29.000000 move-dl-1.4.8/src/move/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2846 2023-04-27 10:53:04.000000 move-dl-1.4.8/src/move/analysis/metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:26.011473 move-dl-1.4.8/src/move/conf/
+-rw-rw-rw-   0        0        0       69 2022-11-07 16:12:48.000000 move-dl-1.4.8/src/move/conf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:26.023437 move-dl-1.4.8/src/move/conf/data/
+-rw-rw-rw-   0        0        0     1044 2022-11-22 13:40:00.000000 move-dl-1.4.8/src/move/conf/data/base_data.yaml
+-rw-rw-rw-   0        0        0      422 2022-11-22 12:49:29.000000 move-dl-1.4.8/src/move/conf/main.yaml
+-rw-rw-rw-   0        0        0     6274 2023-04-26 12:47:53.000000 move-dl-1.4.8/src/move/conf/schema.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:26.076608 move-dl-1.4.8/src/move/conf/task/
+-rw-rw-rw-   0        0        0      524 2023-04-26 12:47:53.000000 move-dl-1.4.8/src/move/conf/task/analyze_latent.yaml
+-rw-rw-rw-   0        0        0      580 2023-04-26 12:47:53.000000 move-dl-1.4.8/src/move/conf/task/identify_associations_bayes.yaml
+-rw-rw-rw-   0        0        0      589 2023-04-26 12:47:53.000000 move-dl-1.4.8/src/move/conf/task/identify_associations_ttest.yaml
+-rw-rw-rw-   0        0        0      490 2023-01-05 22:32:25.000000 move-dl-1.4.8/src/move/conf/task/tune_model_reconstruction.yaml
+-rw-rw-rw-   0        0        0      500 2023-01-05 22:32:25.000000 move-dl-1.4.8/src/move/conf/task/tune_model_stability.yaml
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:26.086449 move-dl-1.4.8/src/move/core/
+-rw-rw-rw-   0        0        0      137 2022-11-22 12:49:29.000000 move-dl-1.4.8/src/move/core/__init__.py
+-rw-rw-rw-   0        0        0     1351 2023-04-27 12:11:37.000000 move-dl-1.4.8/src/move/core/logging.py
+-rw-rw-rw-   0        0        0      530 2023-04-26 12:47:53.000000 move-dl-1.4.8/src/move/core/seed.py
+-rw-rw-rw-   0        0        0      341 2022-11-07 16:12:48.000000 move-dl-1.4.8/src/move/core/typing.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:26.099450 move-dl-1.4.8/src/move/data/
+-rw-rw-rw-   0        0        0       78 2022-11-07 16:12:48.000000 move-dl-1.4.8/src/move/data/__init__.py
+-rw-rw-rw-   0        0        0     6921 2023-04-27 12:11:37.000000 move-dl-1.4.8/src/move/data/dataloaders.py
+-rw-rw-rw-   0        0        0     5286 2022-11-22 13:40:00.000000 move-dl-1.4.8/src/move/data/io.py
+-rw-rw-rw-   0        0        0     3849 2023-04-26 12:47:53.000000 move-dl-1.4.8/src/move/data/perturbations.py
+-rw-rw-rw-   0        0        0     2646 2023-04-27 12:11:28.000000 move-dl-1.4.8/src/move/data/preprocessing.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:26.104454 move-dl-1.4.8/src/move/models/
+-rw-rw-rw-   0        0        0       54 2022-05-24 08:52:38.000000 move-dl-1.4.8/src/move/models/__init__.py
+-rw-rw-rw-   0        0        0    26686 2023-04-27 12:11:37.000000 move-dl-1.4.8/src/move/models/vae.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:26.117449 move-dl-1.4.8/src/move/tasks/
+-rw-rw-rw-   0        0        0      326 2022-11-09 12:50:46.000000 move-dl-1.4.8/src/move/tasks/__init__.py
+-rw-rw-rw-   0        0        0    10680 2023-04-27 12:11:37.000000 move-dl-1.4.8/src/move/tasks/analyze_latent.py
+-rw-rw-rw-   0        0        0     1949 2023-04-27 12:11:37.000000 move-dl-1.4.8/src/move/tasks/encode_data.py
+-rw-rw-rw-   0        0        0    13314 2023-04-27 12:11:37.000000 move-dl-1.4.8/src/move/tasks/identify_associations.py
+-rw-rw-rw-   0        0        0     8952 2023-04-27 12:11:28.000000 move-dl-1.4.8/src/move/tasks/tune_model.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:26.120479 move-dl-1.4.8/src/move/training/
+-rw-rw-rw-   0        0        0        0 2023-01-05 22:41:07.000000 move-dl-1.4.8/src/move/training/__init__.py
+-rw-rw-rw-   0        0        0     3504 2023-04-26 12:47:53.000000 move-dl-1.4.8/src/move/training/training_loop.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:26.134742 move-dl-1.4.8/src/move/visualization/
+-rw-rw-rw-   0        0        0      750 2022-11-17 16:27:56.000000 move-dl-1.4.8/src/move/visualization/__init__.py
+-rw-rw-rw-   0        0        0     6754 2023-04-27 12:11:37.000000 move-dl-1.4.8/src/move/visualization/feature_importance.py
+-rw-rw-rw-   0        0        0     3715 2023-04-27 12:11:37.000000 move-dl-1.4.8/src/move/visualization/latent_space.py
+-rw-rw-rw-   0        0        0     1279 2023-04-26 12:47:53.000000 move-dl-1.4.8/src/move/visualization/loss_curves.py
+-rw-rw-rw-   0        0        0     1860 2023-04-26 12:47:53.000000 move-dl-1.4.8/src/move/visualization/metrics.py
+-rw-rw-rw-   0        0        0     1340 2023-04-27 12:11:28.000000 move-dl-1.4.8/src/move/visualization/style.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:12:26.182742 move-dl-1.4.8/src/move_dl.egg-info/
+-rw-rw-rw-   0        0        0      466 2023-04-27 12:12:25.000000 move-dl-1.4.8/src/move_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-04-27 12:12:25.000000 move-dl-1.4.8/src/move_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 12:12:25.000000 move-dl-1.4.8/src/move_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-27 12:12:25.000000 move-dl-1.4.8/src/move_dl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2023-04-27 12:12:25.000000 move-dl-1.4.8/src/move_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 12:12:25.000000 move-dl-1.4.8/src/move_dl.egg-info/top_level.txt
```

### Comparing `move-dl-1.4.7/LICENSE` & `move-dl-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/README.md` & `move-dl-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/setup.cfg` & `move-dl-1.4.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/__main__.py` & `move-dl-1.4.8/src/move/__main__.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/analysis/metrics.py` & `move-dl-1.4.8/src/move/analysis/metrics.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/conf/data/base_data.yaml` & `move-dl-1.4.8/src/move/conf/data/base_data.yaml`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/conf/schema.py` & `move-dl-1.4.8/src/move/conf/schema.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/conf/task/analyze_latent.yaml` & `move-dl-1.4.8/src/move/conf/task/analyze_latent.yaml`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/conf/task/identify_associations_bayes.yaml` & `move-dl-1.4.8/src/move/conf/task/identify_associations_bayes.yaml`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/conf/task/identify_associations_ttest.yaml` & `move-dl-1.4.8/src/move/conf/task/identify_associations_ttest.yaml`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/core/logging.py` & `move-dl-1.4.8/src/move/core/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Returns:
         Logger
     """
 
     if "." in name:
         name = name.split(".")[-1]
 
+    logging.captureWarnings(True)
     logger = logging.getLogger(name)
 
     if not logger.hasHandlers():
         logger.setLevel(logging.DEBUG)
 
         path = Path.cwd() / "logs"
         path.mkdir(exist_ok=True)
```

### Comparing `move-dl-1.4.7/src/move/core/seed.py` & `move-dl-1.4.8/src/move/core/seed.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/data/dataloaders.py` & `move-dl-1.4.8/src/move/data/dataloaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,19 +57,17 @@
         self.cat_shapes = cat_shapes
         self.con_all = con_all
         self.con_shapes = con_shapes
 
     def __len__(self) -> int:
         return self.num_samples
 
-    def __getitem__(
-        self, idx: int
-    ) -> tuple[Optional[torch.Tensor], Optional[torch.Tensor]]:
-        cat_slice = None if self.cat_all is None else self.cat_all[idx]
-        con_slice = None if self.con_all is None else self.con_all[idx]
+    def __getitem__(self, idx: int) -> tuple[torch.Tensor, torch.Tensor]:
+        cat_slice = torch.empty(0) if self.cat_all is None else self.cat_all[idx]
+        con_slice = torch.empty(0) if self.con_all is None else self.con_all[idx]
         return cat_slice, con_slice
 
 
 def concat_cat_list(
     cat_list: list[FloatArray],
 ) -> tuple[list[tuple[int, ...]], FloatArray]:
     """
@@ -135,22 +133,22 @@
 
     Raises:
         ValueError: If both inputs are None
 
     Returns:
         MOVEDataset
     """
-    if cat_list is None and con_list is None:
+    if not cat_list and not con_list:
         raise ValueError("At least one type of data must be in the input")
 
-    cat_shapes, cat_all = None, None
+    cat_shapes, cat_all = [], None
     if cat_list:
         cat_shapes, cat_all = concat_cat_list(cat_list)
 
-    con_shapes, con_all = None, None
+    con_shapes, con_all = [], None
     if con_list:
         con_shapes, con_all = concat_con_list(con_list)
 
     if cat_all is not None:
         cat_all = torch.from_numpy(cat_all)
         if mask is not None:
             cat_all = cat_all[mask]
```

### Comparing `move-dl-1.4.7/src/move/data/io.py` & `move-dl-1.4.8/src/move/data/io.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/data/perturbations.py` & `move-dl-1.4.8/src/move/data/perturbations.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/data/preprocessing.py` & `move-dl-1.4.8/src/move/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/models/vae.py` & `move-dl-1.4.8/src/move/models/vae.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 __all__ = ["VAE"]
 
 import logging
-from typing import Optional
+from typing import Optional, cast
 
-import numpy as np
 import torch
 from torch import nn, optim
 from torch.utils.data import DataLoader
 
 from move.core.typing import FloatArray, IntArray
 
 logger = logging.getLogger("vae.py")
@@ -36,16 +35,16 @@
             continuous datasets
         ValueError: Number of categorical weights must be the same as number of
             categorical datasets
     """
 
     def __init__(
         self,
-        categorical_shapes: Optional[list[tuple]] = None,
-        continuous_shapes: Optional[list[tuple]] = None,
+        categorical_shapes: Optional[list[tuple[int, ...]]] = None,
+        continuous_shapes: Optional[list[int]] = None,
         categorical_weights: Optional[list[int]] = None,
         continuous_weights: Optional[list[int]] = None,
         num_hidden: list[int] = [200, 200],
         num_latent: int = 20,
         beta: float = 0.01,
         dropout: float = 0.2,
         cuda: bool = False,
@@ -59,47 +58,46 @@
 
         if not (0 <= dropout < 1):
             raise ValueError("Dropout must be between zero and one.")
 
         if continuous_shapes is None and categorical_shapes is None:
             raise ValueError("Shapes of the input data must be provided.")
 
-        num_categorical = sum([int.__mul__(*shape) for shape in categorical_shapes])
-        num_continuous = sum(continuous_shapes)
-
         self.input_size = 0
-        if num_continuous is not None and continuous_shapes is not None:
-            self.num_continuous = num_continuous
+        if continuous_shapes is not None:
+            self.num_continuous = sum(continuous_shapes)
             self.input_size += self.num_continuous
             self.continuous_shapes = continuous_shapes
 
             if continuous_weights is not None:
                 self.continuous_weights = continuous_weights
                 if len(continuous_shapes) != len(continuous_weights):
                     raise ValueError(
                         "Number of continuous weights must be the same as"
                         " number of continuous datasets"
                     )
         else:
-            self.num_continuous = None
+            self.num_continuous = 0
 
-        if num_categorical is not None and categorical_shapes is not None:
-            self.num_categorical = num_categorical
+        if categorical_shapes is not None:
+            self.num_categorical = sum(
+                [int.__mul__(*shape) for shape in categorical_shapes]
+            )
             self.input_size += self.num_categorical
             self.categorical_shapes = categorical_shapes
 
             if categorical_weights is not None:
                 self.categorical_weights = categorical_weights
                 if len(categorical_shapes) != len(categorical_weights):
                     raise ValueError(
                         "Number of categorical weights must be the same as"
                         " number of categorical datasets"
                     )
         else:
-            self.num_categorical = None
+            self.num_categorical = 0
 
         super(VAE, self).__init__()
 
         # Initialize simple attributes
         self.beta = beta
         self.num_hidden = num_hidden
         self.num_latent = num_latent
@@ -203,15 +201,17 @@
             cat_out_tmp = self.log_softmax(cat_out_tmp)
 
             cat_out.append(cat_out_tmp)
             pos += cat_shape[0] * cat_shape[1]
 
         return cat_out
 
-    def decode(self, x: torch.Tensor) -> tuple[list[torch.Tensor], torch.Tensor]:
+    def decode(
+        self, x: torch.Tensor
+    ) -> tuple[Optional[list[torch.Tensor]], Optional[torch.Tensor]]:
         """
         Decode to the input space from the latent space
 
         Args:
             x: sample from latent space distribution
 
         Returns:
@@ -227,31 +227,27 @@
             x = self.dropoutlayer(x)
             x = decodernorm(x)
 
         reconstruction = self.out(x)
 
         # Decompose reconstruction to categorical and continuous variables
         # if both types are in the input
-        if not (self.num_categorical is None or self.num_continuous is None):
+        cat_out, con_out = None, None
+        if self.num_categorical > 0:
             cat_out = self.decompose_categorical(reconstruction)
+        if self.num_continuous > 0:
             con_out = reconstruction.narrow(
                 1, self.num_categorical, self.num_continuous
             )
-        elif self.num_categorical is not None:
-            cat_out = self.decompose_categorical(reconstruction)
-            con_out = None
-        elif self.num_continuous is not None:
-            cat_out = None
-            con_out = reconstruction.narrow(1, 0, self.num_continuous)
 
         return cat_out, con_out
 
     def forward(
         self, tensor: torch.Tensor
-    ) -> tuple[list[torch.Tensor], torch.Tensor, torch.Tensor]:
+    ) -> tuple[list[torch.Tensor], torch.Tensor, torch.Tensor, torch.Tensor]:
         """
         Forward propagate through the VAE network
 
         Args:
             tensor (torch.Tensor): input data
 
         Returns:
@@ -441,42 +437,42 @@
         optimizer = optim.Adam(self.parameters(), lr=lrate)
 
         epoch_loss = 0
         epoch_kldloss = 0
         epoch_sseloss = 0
         epoch_bceloss = 0
 
-        for batch_idx, (cat, con) in enumerate(train_loader):
+        for _, (cat, con) in enumerate(train_loader):
             # Move input to GPU if requested
             cat = cat.to(self.device)
             con = con.to(self.device)
 
-            if self.num_categorical is not None and self.num_continuous is not None:
+            if self.num_categorical > 0 and self.num_continuous > 0:
                 tensor = torch.cat((cat, con), 1)
-            elif self.num_categorical is not None:
+            elif self.num_categorical > 0:
                 tensor = cat
-            elif self.num_continuous is not None:
+            elif self.num_continuous > 0:
                 tensor = con
 
             optimizer.zero_grad()
 
             cat_out, con_out, mu, logvar = self(tensor)
 
             loss, bce, sse, kld = self.loss_function(
                 cat, cat_out, con, con_out, mu, logvar, kld_w
             )
             loss.backward()
 
             epoch_loss += loss.data.item()
             epoch_kldloss += kld.data.item()
 
-            if self.num_continuous is not None:
+            if self.num_continuous > 0:
                 epoch_sseloss += sse.data.item()
 
-            if self.num_categorical is not None:
+            if self.num_categorical > 0:
                 epoch_bceloss += bce.data.item()
 
             optimizer.step()
 
         logger.info(
             "\tEpoch: {}\tLoss: {:.6f}\tCE: {:.7f}\tSSE: {:.6f}\t"
             "KLD: {:.4f}\tBatchsize: {}".format(
@@ -581,17 +577,17 @@
         Returns:
             a formed batch
         """
         cat, con = batch
         cat = cat.to(self.device)
         con = con.to(self.device)
 
-        if self.num_categorical is None:
+        if self.num_categorical == 0:
             return con
-        elif self.num_continuous is None:
+        elif self.num_continuous == 0:
             return cat
         return torch.cat((cat, con), dim=1)
 
     @torch.no_grad()
     def project(self, dataloader: DataLoader) -> FloatArray:
         """Generates an embedding of the data contained in the DataLoader.
 
@@ -626,19 +622,23 @@
         """
         self.eval()
         cat_recons = [[] for _ in range(len(self.categorical_shapes))]
         con_recons = []
         for batch in dataloader:
             batch = self._validate_batch(batch)
             cat_recon, con_recon, *_ = self(batch)
-            for i, cat in enumerate(cat_recon):
-                cat_recons[i].append(torch.argmax(cat, dim=1))
-            con_recons.append(con_recon)
-        cat_recons = [torch.cat(cats, dim=0).cpu().numpy() for cats in cat_recons]
-        con_recons = torch.cat(con_recons, dim=0).cpu().numpy()
+            if cat_recon is not None:
+                for i, cat in enumerate(cat_recon):
+                    cat_recons[i].append(torch.argmax(cat, dim=1))
+            if con_recon is not None:
+                con_recons.append(con_recon)
+        if cat_recons:
+            cat_recons = [torch.cat(cats, dim=0).cpu().numpy() for cats in cat_recons]
+        if con_recons:
+            con_recons = torch.cat(con_recons, dim=0).cpu().numpy()
         return cat_recons, con_recons
 
     @torch.no_grad()
     def latent(
         self, dataloader: DataLoader, kld_weight: float
     ) -> tuple[FloatArray, FloatArray, IntArray, IntArray, FloatArray, float, float]:
         """
@@ -665,37 +665,37 @@
 
         num_samples = dataloader.dataset.num_samples
 
         latent = torch.empty((num_samples, self.num_latent))
         latent_var = torch.empty((num_samples, self.num_latent))
 
         # reconstructed output
-        if self.num_categorical is not None:
+        if self.num_categorical > 0:
             cat_class, cat_recon, cat_total_shape = self.make_cat_recon_out(num_samples)
         else:
             cat_class = None
             cat_recon = None
 
         con_recon = (
             None
-            if self.num_continuous is None
+            if self.num_continuous == 0
             else torch.empty((num_samples, self.num_continuous))
         )
 
         row = 0
         for (cat, con) in dataloader:
             cat = cat.to(self.device)
             con = con.to(self.device)
 
             # get dataset
-            if self.num_categorical is not None and self.num_continuous is not None:
+            if self.num_categorical > 0 and self.num_continuous > 0:
                 tensor = torch.cat((cat, con), 1)
-            elif self.num_categorical is not None:
+            elif self.num_categorical > 0:
                 tensor = cat
-            elif self.num_continuous is not None:
+            elif self.num_continuous > 0:
                 tensor = con
 
             # Evaluate
             cat_out, con_out, mu, logvar = self(tensor)
 
             mu = mu.to(self.device)
             logvar = logvar.to(self.device)
@@ -703,22 +703,22 @@
 
             loss, bce, sse, _ = self.loss_function(
                 cat, cat_out, con, con_out, mu, logvar, kld_weight
             )
             test_likelihood += bce + sse
             test_loss += loss.data.item()
 
-            if self.num_categorical is not None:
+            if self.num_categorical > 0:
                 cat_out_class, cat_target = self.get_cat_recon(
                     batch, cat_total_shape, cat, cat_out
                 )
                 cat_recon[row : row + len(cat_out_class)] = torch.Tensor(cat_out_class)
                 cat_class[row : row + len(cat_target)] = torch.Tensor(cat_target)
 
-            if self.num_continuous is not None:
+            if self.num_continuous > 0:
                 con_recon[row : row + len(con_out)] = con_out
 
             latent_var[row : row + len(logvar)] = logvar
             latent[row : row + len(mu)] = mu
             row += len(mu)
 
         test_loss /= len(dataloader)
```

### Comparing `move-dl-1.4.7/src/move/tasks/analyze_latent.py` & `move-dl-1.4.8/src/move/tasks/analyze_latent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 __all__ = ["analyze_latent"]
 
+import re
 from pathlib import Path
 from typing import Sized, cast
 
 import hydra
 import numpy as np
 import pandas as pd
 import torch
@@ -141,55 +142,70 @@
     model.eval()
 
     logger.info("Projecting into latent space")
     latent_space = model.project(test_dataloader)
     reducer: TransformerMixin = hydra.utils.instantiate(task_config.reducer)
     embedding = reducer.fit_transform(latent_space)
 
-    mappings = io.load_mappings(interim_path / "mappings.json")
+    mappings_path = interim_path / "mappings.json"
+    if mappings_path.exists():
+        mappings = io.load_mappings(mappings_path)
+    else:
+        mappings = {}
+
     fig_df = pd.DataFrame(
         np.take(embedding, [0, 1], axis=1),
         columns=["dim0", "dim1"],
         index=df_index,
     )
+
     for feature_name in task_config.feature_names:
         logger.debug(f"Generating plot: latent space + '{feature_name}'")
         is_categorical = False
         try:
             dataset_index, feature_values = find_feature_values(
                 feature_name, cat_names, cat_list
             )
             is_categorical = True
         except KeyError:
-            dataset_index, feature_values = find_feature_values(
-                feature_name, con_names, con_list
-            )
+            try:
+                dataset_index, feature_values = find_feature_values(
+                    feature_name, con_names, con_list
+                )
+            except KeyError:
+                logger.warning(f"Feature '{feature_name}' not found in any dataset.")
+                continue
 
         if is_categorical:
             # Convert one-hot encoding to category codes
             is_nan = feature_values.sum(axis=1) == 0
             feature_values = np.argmax(feature_values, axis=1)
 
             dataset_name = config.data.categorical_names[dataset_index]
+            feature_mapping = {
+                str(code): category for category, code in mappings[dataset_name].items()
+            }
             fig = viz.plot_latent_space_with_cat(
                 embedding,
                 feature_name,
                 feature_values,
-                mappings[dataset_name],
+                feature_mapping,
                 is_nan,
             )
             fig_df[feature_name] = np.where(is_nan, np.nan, feature_values)
         else:
             feature_values = feature_values
             fig = viz.plot_latent_space_with_con(
                 embedding, feature_name, feature_values
             )
             fig_df[feature_name] = np.where(feature_values == 0, np.nan, feature_values)
 
-        fig_path = str(output_path / f"latent_space_{feature_name}.png")
+        # Remove non-alpha characters
+        safe_feature_name = re.sub(r"[^\w\s]", "", feature_name)
+        fig_path = str(output_path / f"latent_space_{safe_feature_name}.png")
         fig.savefig(fig_path, bbox_inches="tight")
 
     fig_df.to_csv(output_path / "latent_space.tsv", sep="\t")
 
     logger.info("Reconstructing")
     cat_recons, con_recons = model.reconstruct(test_dataloader)
     con_recons = np.split(con_recons, np.cumsum(model.continuous_shapes[:-1]), axis=1)
@@ -220,16 +236,19 @@
         )
         num_features = len(dataloaders)
         z = model.project(test_dataloader)
         diffs = np.empty((num_samples, num_features))
         for j, dataloader in enumerate(dataloaders):
             z_perturb = model.project(dataloader)
             diffs[:, j] = np.sum(z_perturb - z, axis=1)
+        feature_mapping = {
+            str(code): category for category, code in mappings[dataset_name].items()
+        }
         fig = viz.plot_categorical_feature_importance(
-            diffs, cat_list[i], cat_names[i], mappings[dataset_name]
+            diffs, cat_list[i], cat_names[i], feature_mapping
         )
         fig_path = str(output_path / f"feat_importance_{dataset_name}.png")
         fig.savefig(fig_path, bbox_inches="tight")
         fig_df = pd.DataFrame(diffs, columns=cat_names[i], index=df_index)
         fig_df.to_csv(output_path / f"feat_importance_{dataset_name}.tsv", sep="\t")
 
     for i, dataset_name in enumerate(config.data.continuous_names):
```

### Comparing `move-dl-1.4.7/src/move/tasks/encode_data.py` & `move-dl-1.4.8/src/move/tasks/encode_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,28 +19,29 @@
     """
     logger = get_logger(__name__)
     logger.info("Beginning task: encode data")
 
     raw_data_path = Path(config.raw_data_path)
     raw_data_path.mkdir(exist_ok=True)
     interim_data_path = Path(config.interim_data_path)
-    interim_data_path.mkdir(exist_ok=True)
+    interim_data_path.mkdir(exist_ok=True, parents=True)
 
     sample_names = io.read_names(raw_data_path / f"{config.sample_names}.txt")
 
     mappings = {}
     for dataset_name in config.categorical_names:
         logger.info(f"Encoding '{dataset_name}'")
         filepath = raw_data_path / f"{dataset_name}.tsv"
         names, values = io.read_tsv(filepath, sample_names)
         values, mapping = preprocessing.one_hot_encode(values)
         mappings[dataset_name] = mapping
         io.dump_names(interim_data_path / f"{dataset_name}.txt", names)
         np.save(interim_data_path / f"{dataset_name}.npy", values)
-    io.dump_mappings(interim_data_path / "mappings.json", mappings)
+    if mappings:
+        io.dump_mappings(interim_data_path / "mappings.json", mappings)
 
     for dataset_name in config.continuous_names:
         logger.info(f"Encoding '{dataset_name}'")
         filepath = raw_data_path / f"{dataset_name}.tsv"
         names, values = io.read_tsv(filepath, sample_names)
         values, mask_1d = preprocessing.scale(values)
         names = names[mask_1d]
```

### Comparing `move-dl-1.4.7/src/move/tasks/identify_associations.py` & `move-dl-1.4.8/src/move/tasks/identify_associations.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,16 +299,14 @@
         a_df = pd.DataFrame(dict(feature_a_name=cat_names[target_dataset_idx]))
         a_df.index.name = "feature_a_id"
         a_df.reset_index(inplace=True)
         con_names = reduce(list.__add__, con_names)
         b_df = pd.DataFrame(dict(feature_b_name=con_names))
         b_df.index.name = "feature_b_id"
         b_df.reset_index(inplace=True)
-        results = (
-            results
             .merge(a_df, on="feature_a_id", how="left")
             .merge(b_df, on="feature_b_id", how="left")
         )
         results["feature_b_dataset"] = pd.cut(
             cast(IntArray, results["feature_b_id"].values),
             bins=cast(list[int], np.cumsum([0] + con_shapes)),
             right=False,
```

### Comparing `move-dl-1.4.7/src/move/tasks/tune_model.py` & `move-dl-1.4.8/src/move/tasks/tune_model.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/training/training_loop.py` & `move-dl-1.4.8/src/move/training/training_loop.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/visualization/__init__.py` & `move-dl-1.4.8/src/move/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/visualization/feature_importance.py` & `move-dl-1.4.8/src/move/visualization/feature_importance.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,17 @@
     data = pd.DataFrame(
         dict(
             x=diffs.T[top10_ids, :].ravel()[~is_nan],
             y=np.compress(~is_nan, perturbed_features),
             category=feature_values.T[top10_ids, :].ravel()[~is_nan],
         )
     )
-    with style_settings(style), color_cycle(colormap):
+    with style_settings(style):
         fig, ax = plt.subplots(figsize=figsize)
-        sns.swarmplot(data=data, x="x", y="y", hue="category", size=1, ax=ax)
+        sns.stripplot(data=data, x="x", y="y", hue="category", size=1, ax=ax, palette=colormap)
         ax.set(xlabel="Impact on latent space", ylabel="Feature")
         # Fix labels in legend
         legend = ax.get_legend()
         assert legend is not None
         for text in legend.get_texts():
             code = text.get_text()
             if code in feature_mapping:
@@ -169,15 +169,15 @@
     palette = np.empty((25, 4))  # 25 colors x 4 channels
     palette[:13, :] = sm.to_rgba(np.linspace(vmin, 0, 13))  # first slope
     palette[12:, :] = sm.to_rgba(np.linspace(0, vmax, 13))  # second slope
     palette = palette.tolist()  # NDArray not always supported
 
     with style_settings(style):
         fig, ax = plt.subplots(figsize=figsize)
-        sns.swarmplot(
+        sns.stripplot(
             data=data, x="x", y="y", hue="category", ax=ax, palette=palette, size=2
         )
         ax.set(xlabel="Impact on latent space", ylabel="Feature")
         # Add colormap
         legend = ax.get_legend()
         if legend is not None:
             legend.remove()
```

### Comparing `move-dl-1.4.7/src/move/visualization/latent_space.py` & `move-dl-1.4.8/src/move/visualization/latent_space.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 __all__ = ["plot_latent_space_with_cat", "plot_latent_space_with_con"]
 
+from typing import Any
+
 import matplotlib.figure
 import matplotlib.pyplot as plt
 import matplotlib.style
 import numpy as np
 from matplotlib.colors import TwoSlopeNorm
 
 from move.core.typing import BoolArray, FloatArray
@@ -16,15 +18,15 @@
 )
 
 
 def plot_latent_space_with_cat(
     latent_space: FloatArray,
     feature_name: str,
     feature_values: FloatArray,
-    feature_mapping: dict[str, int],
+    feature_mapping: dict[str, Any],
     is_nan: BoolArray,
     style: str = DEFAULT_PLOT_STYLE,
     colormap: str = DEFAULT_QUALITATIVE_PALETTE,
 ) -> matplotlib.figure.Figure:
     """Plot a 2D latent space together with a legend mapping the latent
     space to the values of a discrete feature.
```

### Comparing `move-dl-1.4.7/src/move/visualization/loss_curves.py` & `move-dl-1.4.8/src/move/visualization/loss_curves.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/visualization/metrics.py` & `move-dl-1.4.8/src/move/visualization/metrics.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move/visualization/style.py` & `move-dl-1.4.8/src/move/visualization/style.py`

 * *Files identical despite different names*

### Comparing `move-dl-1.4.7/src/move_dl.egg-info/SOURCES.txt` & `move-dl-1.4.8/src/move_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*


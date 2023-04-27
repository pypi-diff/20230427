# Comparing `tmp/pseudo_labeller-0.0.4.tar.gz` & `tmp/pseudo_labeller-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pseudo_labeller-0.0.4.tar", last modified: Tue Apr  4 07:58:13 2023, max compression
+gzip compressed data, was "pseudo_labeller-0.0.5.tar", last modified: Thu Apr 27 13:50:18 2023, max compression
```

## Comparing `pseudo_labeller-0.0.4.tar` & `pseudo_labeller-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:58:13.057402 pseudo_labeller-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-04 07:57:59.000000 pseudo_labeller-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-04 07:57:59.000000 pseudo_labeller-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-04 07:58:13.053402 pseudo_labeller-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-04 07:57:59.000000 pseudo_labeller-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:58:13.053402 pseudo_labeller-0.0.4/pseudo_labeller/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 07:57:59.000000 pseudo_labeller-0.0.4/pseudo_labeller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:58:13.053402 pseudo_labeller-0.0.4/pseudo_labeller/model/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-04 07:57:59.000000 pseudo_labeller-0.0.4/pseudo_labeller/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-04-04 07:57:59.000000 pseudo_labeller-0.0.4/pseudo_labeller/model/idam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:58:13.053402 pseudo_labeller-0.0.4/pseudo_labeller/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-04 07:57:59.000000 pseudo_labeller-0.0.4/pseudo_labeller/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:58:13.053402 pseudo_labeller-0.0.4/pseudo_labeller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-04 07:58:13.000000 pseudo_labeller-0.0.4/pseudo_labeller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-04 07:58:13.000000 pseudo_labeller-0.0.4/pseudo_labeller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:58:13.000000 pseudo_labeller-0.0.4/pseudo_labeller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-04 07:58:13.000000 pseudo_labeller-0.0.4/pseudo_labeller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-04 07:58:13.000000 pseudo_labeller-0.0.4/pseudo_labeller.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-04 07:57:59.000000 pseudo_labeller-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 07:58:13.057402 pseudo_labeller-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-04 07:57:59.000000 pseudo_labeller-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:50:18.178451 pseudo_labeller-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-27 13:49:57.000000 pseudo_labeller-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 13:49:57.000000 pseudo_labeller-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-27 13:50:18.178451 pseudo_labeller-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-27 13:49:57.000000 pseudo_labeller-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:50:18.174451 pseudo_labeller-0.0.5/pseudo_labeller/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:49:57.000000 pseudo_labeller-0.0.5/pseudo_labeller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:50:18.178451 pseudo_labeller-0.0.5/pseudo_labeller/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 13:49:57.000000 pseudo_labeller-0.0.5/pseudo_labeller/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-27 13:49:57.000000 pseudo_labeller-0.0.5/pseudo_labeller/model/idam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:50:18.178451 pseudo_labeller-0.0.5/pseudo_labeller/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 13:49:57.000000 pseudo_labeller-0.0.5/pseudo_labeller/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:50:18.178451 pseudo_labeller-0.0.5/pseudo_labeller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-27 13:50:18.000000 pseudo_labeller-0.0.5/pseudo_labeller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-27 13:50:18.000000 pseudo_labeller-0.0.5/pseudo_labeller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:50:18.000000 pseudo_labeller-0.0.5/pseudo_labeller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 13:50:18.000000 pseudo_labeller-0.0.5/pseudo_labeller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 13:50:18.000000 pseudo_labeller-0.0.5/pseudo_labeller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 13:49:57.000000 pseudo_labeller-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:50:18.178451 pseudo_labeller-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-27 13:49:57.000000 pseudo_labeller-0.0.5/setup.py
```

### Comparing `pseudo_labeller-0.0.4/LICENSE` & `pseudo_labeller-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pseudo_labeller-0.0.4/pseudo_labeller/model/idam.py` & `pseudo_labeller-0.0.5/pseudo_labeller/model/idam.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,16 @@
                 nn.Conv3d(
                     in_channels=conv3d_channels,
                     out_channels=conv3d_channels,
                     kernel_size=(kernel_size, kernel_size, kernel_size),
                     padding="same",
                 )
             )
+            if i % 2 == 0:
+                self.layers.append(nn.BatchNorm3d(conv3d_channels))
 
         # Map to output latent variables, per timestep
 
         # Map the output to the latent variables
         # Latent head should be number of output steps + latent channels
         self.latent_head = nn.Conv2d(
             in_channels=input_steps * conv3d_channels,
@@ -94,19 +96,21 @@
 
         # Small head model to convert from latent space to PV generation for training
         # Input is per-pixel input data, this will be
         # reshaped to the same output steps as the latent head
         self.pv_meta_input = nn.Conv2d(
             pv_meta_input_channels, out_channels=hidden_dim, kernel_size=(1, 1)
         )
+        self.batch_norm_meta = nn.BatchNorm2d(hidden_dim)
 
         # Output is forecast steps channels, each channel is a timestep
         # For labelling, this should be 1, forecasting the middle
         # timestep, for forecasting, the number of steps
         # This is done by putting the meta inputs to each timestep
+        self.batch_norm_output_meta = nn.BatchNorm2d((output_steps * output_channels) + hidden_dim)
         self.pv_meta_output = nn.Conv2d(
             in_channels=(output_steps * output_channels) + hidden_dim,
             out_channels=output_steps,
             kernel_size=(1, 1),
             padding="same",
         )
 
@@ -127,12 +131,13 @@
         x = einops.rearrange(x, "b c t h w -> b (c t) h w")
         x = self.latent_head(x)
         if output_latents:
             # Rearrange back to timeseries of latent variables
             x = einops.rearrange(x, "b (c t) h w -> b c t h w", c=self.output_channels)
             return x
         pv_meta = self.pv_meta_input(pv_meta)
+        pv_meta = self.batch_norm_meta(pv_meta)
         # Reshape to fit into 3DCNN
         x = torch.cat([x, pv_meta], dim=1)
         # Get pv_meta_output
-        x = F.relu(self.pv_meta_output(x))  # Generation can only be positive or 0, so ReLU
+        x = F.relu(self.pv_meta_output(self.batch_norm_output_meta(x)))  # Generation can only be positive or 0, so ReLU
         return x
```

### Comparing `pseudo_labeller-0.0.4/setup.py` & `pseudo_labeller-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 
 setup(
     name="pseudo_labeller",
-    version="0.0.4",
+    version="0.0.5",
     license="MIT",
     description="Psuedo PV/Irradience Labeller",
     author="Jacob Bieker",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
     long_description=long_description,
```


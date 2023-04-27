# Comparing `tmp/astromartini-2.0.0.tar.gz` & `tmp/astromartini-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromartini-2.0.0.tar", last modified: Sun Mar 26 10:06:58 2023, max compression
+gzip compressed data, was "astromartini-2.0.1.tar", last modified: Thu Apr 27 13:28:06 2023, max compression
```

## Comparing `astromartini-2.0.0.tar` & `astromartini-2.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:06:58.636010 astromartini-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-03-26 10:06:26.000000 astromartini-2.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-26 10:06:26.000000 astromartini-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-03-26 10:06:58.636010 astromartini-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-03-26 10:06:26.000000 astromartini-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:06:58.632010 astromartini-2.0.0/astromartini.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-03-26 10:06:58.000000 astromartini-2.0.0/astromartini.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-26 10:06:58.000000 astromartini-2.0.0/astromartini.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 10:06:58.000000 astromartini-2.0.0/astromartini.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-26 10:06:58.000000 astromartini-2.0.0/astromartini.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-26 10:06:58.000000 astromartini-2.0.0/astromartini.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:06:58.632010 astromartini-2.0.0/martini/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/beams.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/datacube.py
--rw-r--r--   0 runner    (1001) docker     (123)    32216 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/martini.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:06:58.632010 astromartini-2.0.0/martini/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/_L_align.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/_cartesian_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/_illustris_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/colibre_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/eagle_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/magneticum_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/simba_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/so_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/sph_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/swiftgalaxy_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sources/tng_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/spectral_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    46079 2023-03-26 10:06:26.000000 astromartini-2.0.0/martini/sph_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-26 10:06:26.000000 astromartini-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 10:06:58.636010 astromartini-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:06:58.636010 astromartini-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-03-26 10:06:26.000000 astromartini-2.0.0/tests/test_beams.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-03-26 10:06:26.000000 astromartini-2.0.0/tests/test_datacube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-26 10:06:26.000000 astromartini-2.0.0/tests/test_fits_compliant.py
--rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-03-26 10:06:26.000000 astromartini-2.0.0/tests/test_martini.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-26 10:06:26.000000 astromartini-2.0.0/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-03-26 10:06:26.000000 astromartini-2.0.0/tests/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-03-26 10:06:26.000000 astromartini-2.0.0/tests/test_spectral_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-03-26 10:06:26.000000 astromartini-2.0.0/tests/test_sph_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-03-26 10:06:26.000000 astromartini-2.0.0/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:28:06.337108 astromartini-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-27 13:27:32.000000 astromartini-2.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 13:27:32.000000 astromartini-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-04-27 13:28:06.337108 astromartini-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-27 13:27:32.000000 astromartini-2.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:28:06.333108 astromartini-2.0.1/astromartini.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-04-27 13:28:06.000000 astromartini-2.0.1/astromartini.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-27 13:28:06.000000 astromartini-2.0.1/astromartini.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:28:06.000000 astromartini-2.0.1/astromartini.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-27 13:28:06.000000 astromartini-2.0.1/astromartini.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 13:28:06.000000 astromartini-2.0.1/astromartini.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:28:06.333108 astromartini-2.0.1/martini/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/beams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/datacube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32216 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/martini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:28:06.337108 astromartini-2.0.1/martini/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/_L_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/_cartesian_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/_illustris_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/colibre_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/eagle_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/magneticum_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/simba_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/so_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/sph_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/swiftgalaxy_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sources/tng_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/spectral_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46079 2023-04-27 13:27:32.000000 astromartini-2.0.1/martini/sph_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-27 13:27:32.000000 astromartini-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:28:06.337108 astromartini-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:28:06.337108 astromartini-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-27 13:27:32.000000 astromartini-2.0.1/tests/test_beams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-27 13:27:32.000000 astromartini-2.0.1/tests/test_datacube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-27 13:27:32.000000 astromartini-2.0.1/tests/test_fits_compliant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-04-27 13:27:32.000000 astromartini-2.0.1/tests/test_martini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-27 13:27:32.000000 astromartini-2.0.1/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-04-27 13:27:32.000000 astromartini-2.0.1/tests/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-27 13:27:32.000000 astromartini-2.0.1/tests/test_spectral_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-04-27 13:27:32.000000 astromartini-2.0.1/tests/test_sph_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-27 13:27:32.000000 astromartini-2.0.1/tests/test_write.py
```

### Comparing `astromartini-2.0.0/LICENSE.md` & `astromartini-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/PKG-INFO` & `astromartini-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromartini
-Version: 2.0.0
+Version: 2.0.1
 Summary: Synthetic datacube creation from simulations.
 Author-email: Kyle Oman <kyle.a.oman@durham.ac.uk>
 Project-URL: Homepage, https://github.com/kyleaoman/martini
 Project-URL: Bug Tracker, https://github.com/kyleaoman/martini/issues
 Project-URL: Documentation, https://martini.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `astromartini-2.0.0/README.rst` & `astromartini-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/astromartini.egg-info/PKG-INFO` & `astromartini-2.0.1/astromartini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromartini
-Version: 2.0.0
+Version: 2.0.1
 Summary: Synthetic datacube creation from simulations.
 Author-email: Kyle Oman <kyle.a.oman@durham.ac.uk>
 Project-URL: Homepage, https://github.com/kyleaoman/martini
 Project-URL: Bug Tracker, https://github.com/kyleaoman/martini/issues
 Project-URL: Documentation, https://martini.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `astromartini-2.0.0/astromartini.egg-info/SOURCES.txt` & `astromartini-2.0.1/astromartini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/__init__.py` & `astromartini-2.0.1/martini/__init__.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/_demo.py` & `astromartini-2.0.1/martini/_demo.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/beams.py` & `astromartini-2.0.1/martini/beams.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/datacube.py` & `astromartini-2.0.1/martini/datacube.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/martini.py` & `astromartini-2.0.1/martini/martini.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/noise.py` & `astromartini-2.0.1/martini/noise.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sources/_L_align.py` & `astromartini-2.0.1/martini/sources/_L_align.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sources/_cartesian_translation.py` & `astromartini-2.0.1/martini/sources/_cartesian_translation.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sources/_illustris_tools.py` & `astromartini-2.0.1/martini/sources/_illustris_tools.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sources/colibre_source.py` & `astromartini-2.0.1/martini/sources/colibre_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sources/eagle_source.py` & `astromartini-2.0.1/martini/sources/eagle_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sources/magneticum_source.py` & `astromartini-2.0.1/martini/sources/magneticum_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sources/simba_source.py` & `astromartini-2.0.1/martini/sources/simba_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sources/so_source.py` & `astromartini-2.0.1/martini/sources/so_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sources/sph_source.py` & `astromartini-2.0.1/martini/sources/sph_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sources/swiftgalaxy_source.py` & `astromartini-2.0.1/martini/sources/swiftgalaxy_source.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sources/tng_source.py` & `astromartini-2.0.1/martini/sources/tng_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,17 @@
                     cutout = api_get(
                         cutout_api_path, params=cutout_request, api_key=api_key
                     )
                 # hold file in memory
                 cfname = io.BytesIO(cutout.content)
                 if cutout_dir is not None:
                     # write a copy to disk for later use
-                    ofile = cutout_file(simulation, snapNum, haloID)
+                    ofile = os.path.join(
+                        cutout_dir, cutout_file(simulation, snapNum, haloID)
+                    )
                     print(f"Writing downloaded cutout to {ofile}")
                     with open(ofile, "wb") as of:
                         of.write(cutout.content)
                     with h5py.File(ofile, "r+") as of:
                         of.create_group(f"{subID}")
                         of[f"{subID}"].attrs["pos"] = data_sub["SubhaloPos"]
                         of[f"{subID}"].attrs["vel"] = data_sub["SubhaloVel"]
```

### Comparing `astromartini-2.0.0/martini/spectral_models.py` & `astromartini-2.0.1/martini/spectral_models.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/martini/sph_kernels.py` & `astromartini-2.0.1/martini/sph_kernels.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/pyproject.toml` & `astromartini-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astromartini"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
     { name="Kyle Oman", email="kyle.a.oman@durham.ac.uk" },
 ]
 description="Synthetic datacube creation from simulations."
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `astromartini-2.0.0/tests/test_beams.py` & `astromartini-2.0.1/tests/test_beams.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/tests/test_datacube.py` & `astromartini-2.0.1/tests/test_datacube.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/tests/test_fits_compliant.py` & `astromartini-2.0.1/tests/test_fits_compliant.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/tests/test_martini.py` & `astromartini-2.0.1/tests/test_martini.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/tests/test_noise.py` & `astromartini-2.0.1/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/tests/test_sources.py` & `astromartini-2.0.1/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/tests/test_spectral_models.py` & `astromartini-2.0.1/tests/test_spectral_models.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/tests/test_sph_kernels.py` & `astromartini-2.0.1/tests/test_sph_kernels.py`

 * *Files identical despite different names*

### Comparing `astromartini-2.0.0/tests/test_write.py` & `astromartini-2.0.1/tests/test_write.py`

 * *Files identical despite different names*


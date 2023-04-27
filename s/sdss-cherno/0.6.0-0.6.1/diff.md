# Comparing `tmp/sdss_cherno-0.6.0.tar.gz` & `tmp/sdss_cherno-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_cherno-0.6.0.tar", max compression
+gzip compressed data, was "sdss_cherno-0.6.1.tar", max compression
```

## Comparing `sdss_cherno-0.6.0.tar` & `sdss_cherno-0.6.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1504 2023-04-25 16:03:17.263097 sdss_cherno-0.6.0/LICENSE.md
--rw-r--r--   0        0        0     2714 2023-04-25 16:03:17.263503 sdss_cherno-0.6.0/README.md
--rw-r--r--   0        0        0     1251 2023-04-25 16:03:17.263912 sdss_cherno-0.6.0/cherno/__init__.py
--rw-r--r--   0        0        0     2207 2023-04-25 16:03:17.264935 sdss_cherno-0.6.0/cherno/__main__.py
--rw-r--r--   0        0        0      747 2023-04-25 16:03:17.265416 sdss_cherno-0.6.0/cherno/actor/__init__.py
--rw-r--r--   0        0        0     4493 2023-04-25 16:03:17.267569 sdss_cherno-0.6.0/cherno/actor/actor.py
--rw-r--r--   0        0        0        0 2023-04-25 16:03:17.268005 sdss_cherno-0.6.0/cherno/actor/commands/__init__.py
--rw-r--r--   0        0        0     1746 2023-04-25 16:03:17.269274 sdss_cherno-0.6.0/cherno/actor/commands/acquire.py
--rw-r--r--   0        0        0     4938 2023-04-25 16:03:17.269777 sdss_cherno-0.6.0/cherno/actor/commands/config.py
--rw-r--r--   0        0        0     8213 2023-04-25 16:03:17.270233 sdss_cherno-0.6.0/cherno/actor/commands/guide.py
--rw-r--r--   0        0        0     1273 2023-04-25 16:03:17.270821 sdss_cherno-0.6.0/cherno/actor/commands/offset.py
--rw-r--r--   0        0        0     1007 2023-04-25 16:03:17.271351 sdss_cherno-0.6.0/cherno/actor/commands/reprocess.py
--rw-r--r--   0        0        0     2298 2023-04-25 16:03:17.271808 sdss_cherno-0.6.0/cherno/actor/commands/scale.py
--rw-r--r--   0        0        0     3119 2023-04-25 16:03:17.272781 sdss_cherno-0.6.0/cherno/actor/commands/set.py
--rw-r--r--   0        0        0     1049 2023-04-25 16:03:17.273181 sdss_cherno-0.6.0/cherno/actor/commands/show.py
--rw-r--r--   0        0        0     1964 2023-04-25 16:03:17.273587 sdss_cherno-0.6.0/cherno/actor/commands/status.py
--rw-r--r--   0        0        0      778 2023-04-25 16:03:17.274051 sdss_cherno-0.6.0/cherno/actor/commands/stop.py
--rw-r--r--   0        0        0     1148 2023-04-25 16:03:17.274411 sdss_cherno-0.6.0/cherno/actor/commands/version.py
--rw-r--r--   0        0        0    10857 2023-04-25 16:03:17.274768 sdss_cherno-0.6.0/cherno/actor/exposer.py
--rw-r--r--   0        0        0       73 2023-04-25 16:03:17.275193 sdss_cherno-0.6.0/cherno/etc/astrometrynet_APO.cfg
--rw-r--r--   0        0        0       73 2023-04-25 16:03:17.275770 sdss_cherno-0.6.0/cherno/etc/astrometrynet_LCO.cfg
--rw-r--r--   0        0        0     1994 2023-04-25 16:03:17.276124 sdss_cherno-0.6.0/cherno/etc/cherno_APO.yml
--rw-r--r--   0        0        0     1958 2023-04-25 16:03:17.301758 sdss_cherno-0.6.0/cherno/etc/cherno_LCO.yml
--rw-r--r--   0        0        0     5688 2023-04-25 16:03:17.302240 sdss_cherno-0.6.0/cherno/etc/schema.json
--rw-r--r--   0        0        0     1233 2023-04-25 16:03:17.302599 sdss_cherno-0.6.0/cherno/exceptions.py
--rw-r--r--   0        0        0    14028 2023-04-25 16:03:17.303956 sdss_cherno-0.6.0/cherno/extraction.py
--rw-r--r--   0        0        0    40248 2023-04-25 16:03:17.304689 sdss_cherno-0.6.0/cherno/guider.py
--rw-r--r--   0        0        0     4175 2023-04-25 16:03:17.305802 sdss_cherno-0.6.0/cherno/lcotcc.py
--rw-r--r--   0        0        0     1394 2023-04-25 16:03:17.306236 sdss_cherno-0.6.0/cherno/maskbits.py
--rw-r--r--   0        0        0     4738 2023-04-25 16:03:17.306612 sdss_cherno-0.6.0/cherno/tcc.py
--rw-r--r--   0        0        0     6237 2023-04-25 16:03:17.307096 sdss_cherno-0.6.0/cherno/utils.py
--rw-r--r--   0        0        0     2314 2023-04-25 16:03:17.315859 sdss_cherno-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 sdss_cherno-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-27 15:49:06.932924 sdss_cherno-0.6.1/LICENSE.md
+-rw-r--r--   0        0        0     2723 2023-04-27 15:49:06.933270 sdss_cherno-0.6.1/README.md
+-rw-r--r--   0        0        0     1251 2023-04-27 15:49:06.933672 sdss_cherno-0.6.1/cherno/__init__.py
+-rw-r--r--   0        0        0     2207 2023-04-27 15:49:06.934006 sdss_cherno-0.6.1/cherno/__main__.py
+-rw-r--r--   0        0        0      747 2023-04-27 15:49:06.934389 sdss_cherno-0.6.1/cherno/actor/__init__.py
+-rw-r--r--   0        0        0     4493 2023-04-27 15:49:06.934860 sdss_cherno-0.6.1/cherno/actor/actor.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:49:06.935084 sdss_cherno-0.6.1/cherno/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1746 2023-04-27 15:49:06.935760 sdss_cherno-0.6.1/cherno/actor/commands/acquire.py
+-rw-r--r--   0        0        0     4938 2023-04-27 15:49:06.936996 sdss_cherno-0.6.1/cherno/actor/commands/config.py
+-rw-r--r--   0        0        0     8213 2023-04-27 15:49:06.937407 sdss_cherno-0.6.1/cherno/actor/commands/guide.py
+-rw-r--r--   0        0        0     1273 2023-04-27 15:49:06.937813 sdss_cherno-0.6.1/cherno/actor/commands/offset.py
+-rw-r--r--   0        0        0     1007 2023-04-27 15:49:06.938943 sdss_cherno-0.6.1/cherno/actor/commands/reprocess.py
+-rw-r--r--   0        0        0     2298 2023-04-27 15:49:06.939411 sdss_cherno-0.6.1/cherno/actor/commands/scale.py
+-rw-r--r--   0        0        0     3119 2023-04-27 15:49:06.939872 sdss_cherno-0.6.1/cherno/actor/commands/set.py
+-rw-r--r--   0        0        0     1049 2023-04-27 15:49:06.940241 sdss_cherno-0.6.1/cherno/actor/commands/show.py
+-rw-r--r--   0        0        0     1964 2023-04-27 15:49:06.940894 sdss_cherno-0.6.1/cherno/actor/commands/status.py
+-rw-r--r--   0        0        0      778 2023-04-27 15:49:06.941407 sdss_cherno-0.6.1/cherno/actor/commands/stop.py
+-rw-r--r--   0        0        0     1148 2023-04-27 15:49:06.941771 sdss_cherno-0.6.1/cherno/actor/commands/version.py
+-rw-r--r--   0        0        0    10857 2023-04-27 15:49:06.942168 sdss_cherno-0.6.1/cherno/actor/exposer.py
+-rw-r--r--   0        0        0       73 2023-04-27 15:49:06.942579 sdss_cherno-0.6.1/cherno/etc/astrometrynet_APO.cfg
+-rw-r--r--   0        0        0       73 2023-04-27 15:49:06.942896 sdss_cherno-0.6.1/cherno/etc/astrometrynet_LCO.cfg
+-rw-r--r--   0        0        0     1994 2023-04-27 15:49:06.943266 sdss_cherno-0.6.1/cherno/etc/cherno_APO.yml
+-rw-r--r--   0        0        0     1958 2023-04-27 15:49:06.943603 sdss_cherno-0.6.1/cherno/etc/cherno_LCO.yml
+-rw-r--r--   0        0        0     5688 2023-04-27 15:49:06.943938 sdss_cherno-0.6.1/cherno/etc/schema.json
+-rw-r--r--   0        0        0     1233 2023-04-27 15:49:06.944428 sdss_cherno-0.6.1/cherno/exceptions.py
+-rw-r--r--   0        0        0    14028 2023-04-27 15:49:06.945028 sdss_cherno-0.6.1/cherno/extraction.py
+-rw-r--r--   0        0        0    40346 2023-04-27 15:49:06.945681 sdss_cherno-0.6.1/cherno/guider.py
+-rw-r--r--   0        0        0     4175 2023-04-27 15:49:06.946143 sdss_cherno-0.6.1/cherno/lcotcc.py
+-rw-r--r--   0        0        0     1394 2023-04-27 15:49:06.946554 sdss_cherno-0.6.1/cherno/maskbits.py
+-rw-r--r--   0        0        0     4738 2023-04-27 15:49:06.946970 sdss_cherno-0.6.1/cherno/tcc.py
+-rw-r--r--   0        0        0     6237 2023-04-27 15:49:06.947512 sdss_cherno-0.6.1/cherno/utils.py
+-rw-r--r--   0        0        0     2314 2023-04-27 15:49:06.957729 sdss_cherno-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 sdss_cherno-0.6.1/PKG-INFO
```

### Comparing `sdss_cherno-0.6.0/LICENSE.md` & `sdss_cherno-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/README.md` & `sdss_cherno-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cherno
 
 ![Versions](https://img.shields.io/badge/python->3.8-blue)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/sdss-cherno/badge/?version=latest)](https://sdss-cherno.readthedocs.io/en/latest/?badge=latest)
 [![Tests Status](https://github.com/sdss/cherno/workflows/Test/badge.svg)](https://github.com/sdss/cherno/actions)
-[![codecov](https://codecov.io/gh/sdss/cherno/branch/main/graph/badge.svg)](https://codecov.io/gh/sdss/cherno)
+<!-- [![codecov](https://codecov.io/gh/sdss/cherno/branch/main/graph/badge.svg)](https://codecov.io/gh/sdss/cherno) -->
 
 
 SDSS guider actor
 
 ## Installation
 
 In general you should be able to install ``cherno`` by doing
```

### Comparing `sdss_cherno-0.6.0/cherno/__init__.py` & `sdss_cherno-0.6.1/cherno/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/__main__.py` & `sdss_cherno-0.6.1/cherno/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/__init__.py` & `sdss_cherno-0.6.1/cherno/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/actor.py` & `sdss_cherno-0.6.1/cherno/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/commands/acquire.py` & `sdss_cherno-0.6.1/cherno/actor/commands/acquire.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/commands/config.py` & `sdss_cherno-0.6.1/cherno/actor/commands/config.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/commands/guide.py` & `sdss_cherno-0.6.1/cherno/actor/commands/guide.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/commands/offset.py` & `sdss_cherno-0.6.1/cherno/actor/commands/offset.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/commands/reprocess.py` & `sdss_cherno-0.6.1/cherno/actor/commands/reprocess.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/commands/scale.py` & `sdss_cherno-0.6.1/cherno/actor/commands/scale.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/commands/set.py` & `sdss_cherno-0.6.1/cherno/actor/commands/set.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/commands/show.py` & `sdss_cherno-0.6.1/cherno/actor/commands/show.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/commands/status.py` & `sdss_cherno-0.6.1/cherno/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/commands/stop.py` & `sdss_cherno-0.6.1/cherno/actor/commands/stop.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/commands/version.py` & `sdss_cherno-0.6.1/cherno/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/actor/exposer.py` & `sdss_cherno-0.6.1/cherno/actor/exposer.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/etc/cherno_APO.yml` & `sdss_cherno-0.6.1/cherno/etc/cherno_APO.yml`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/etc/cherno_LCO.yml` & `sdss_cherno-0.6.1/cherno/etc/cherno_LCO.yml`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/etc/schema.json` & `sdss_cherno-0.6.1/cherno/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/exceptions.py` & `sdss_cherno-0.6.1/cherno/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/extraction.py` & `sdss_cherno-0.6.1/cherno/extraction.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/guider.py` & `sdss_cherno-0.6.1/cherno/guider.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,14 +438,18 @@
             # just use the previous fit.
             if guider_fit is not None and (fit_rms_sigma <= 0 or not tmp_guider_fit):
                 break
 
             # Update the fit with the previous one.
             guider_fit = tmp_guider_fit
 
+            # If the fit failed, exit.
+            if guider_fit is False:
+                break
+
             # If only 3 cameras remain we exit. We don't want to reject any more.
             if len(fit_cameras) <= 3:
                 break
 
             sc = SigmaClip(fit_rms_sigma)
             rms_clip = sc(guider_fit.fit_rms.loc[fit_cameras, "rms"])
```

### Comparing `sdss_cherno-0.6.0/cherno/lcotcc.py` & `sdss_cherno-0.6.1/cherno/lcotcc.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/maskbits.py` & `sdss_cherno-0.6.1/cherno/maskbits.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/tcc.py` & `sdss_cherno-0.6.1/cherno/tcc.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/cherno/utils.py` & `sdss_cherno-0.6.1/cherno/utils.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.0/pyproject.toml` & `sdss_cherno-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-cherno"
-version = "0.6.0"
+version = "0.6.1"
 description = "SDSS guider actor"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/cherno"
 repository = "https://github.com/sdss/cherno"
 documentation = "https://sdss-cherno.readthedocs.org"
@@ -28,15 +28,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 sdsstools = "^1.0.0"
 sdss-clu = "^1.8.0"
 astropy = "^5.0.0"
 click-default-group = "^1.2.2"
-sdss-coordio = "^1.7.1"
+sdss-coordio = "^1.7.2"
 pandas = "^1.3.4"
 tables = ">=3.6.1"
 simple-pid = "^1.0.1"
 sqlalchemy = "^1.4.45"
 psycopg2-binary = "^2.9.5"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `sdss_cherno-0.6.0/PKG-INFO` & `sdss_cherno-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-cherno
-Version: 0.6.0
+Version: 0.6.1
 Summary: SDSS guider actor
 Home-page: https://github.com/sdss/cherno
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.9,<3.12
@@ -21,30 +21,30 @@
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: astropy (>=5.0.0,<6.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: sdss-clu (>=1.8.0,<2.0.0)
-Requires-Dist: sdss-coordio (>=1.7.1,<2.0.0)
+Requires-Dist: sdss-coordio (>=1.7.2,<2.0.0)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
 Requires-Dist: simple-pid (>=1.0.1,<2.0.0)
 Requires-Dist: sqlalchemy (>=1.4.45,<2.0.0)
 Requires-Dist: tables (>=3.6.1)
 Project-URL: Documentation, https://sdss-cherno.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/cherno
 Description-Content-Type: text/markdown
 
 # cherno
 
 ![Versions](https://img.shields.io/badge/python->3.8-blue)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/sdss-cherno/badge/?version=latest)](https://sdss-cherno.readthedocs.io/en/latest/?badge=latest)
 [![Tests Status](https://github.com/sdss/cherno/workflows/Test/badge.svg)](https://github.com/sdss/cherno/actions)
-[![codecov](https://codecov.io/gh/sdss/cherno/branch/main/graph/badge.svg)](https://codecov.io/gh/sdss/cherno)
+<!-- [![codecov](https://codecov.io/gh/sdss/cherno/branch/main/graph/badge.svg)](https://codecov.io/gh/sdss/cherno) -->
 
 
 SDSS guider actor
 
 ## Installation
 
 In general you should be able to install ``cherno`` by doing
```


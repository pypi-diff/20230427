# Comparing `tmp/sliderule-3.0.6.tar.gz` & `tmp/sliderule-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.0.6.tar", last modified: Mon Apr 17 15:44:36 2023, max compression
+gzip compressed data, was "sliderule-3.1.0.tar", last modified: Thu Apr 27 14:09:53 2023, max compression
```

## Comparing `sliderule-3.0.6.tar` & `sliderule-3.1.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:44:36.568606 sliderule-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-17 15:44:23.000000 sliderule-3.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-17 15:44:23.000000 sliderule-3.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-17 15:44:36.568606 sliderule-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-04-17 15:44:23.000000 sliderule-3.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-17 15:44:23.000000 sliderule-3.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 15:44:36.568606 sliderule-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-04-17 15:44:23.000000 sliderule-3.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:44:36.564606 sliderule-3.0.6/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/arcticdem.py
--rw-r--r--   0 runner    (1001) docker     (122)    24752 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    11492 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    36103 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    36286 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85031 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)    43166 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:44:36.564606 sliderule-3.0.6/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-17 15:44:36.000000 sliderule-3.0.6/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      973 2023-04-17 15:44:36.000000 sliderule-3.0.6/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 15:44:36.000000 sliderule-3.0.6/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-17 15:44:36.000000 sliderule-3.0.6/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-17 15:44:36.000000 sliderule-3.0.6/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:44:36.568606 sliderule-3.0.6/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/_landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/hls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-17 15:44:23.000000 sliderule-3.0.6/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 14:09:53.818036 sliderule-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-27 14:09:41.000000 sliderule-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-27 14:09:41.000000 sliderule-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-27 14:09:53.818036 sliderule-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-27 14:09:41.000000 sliderule-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-27 14:09:41.000000 sliderule-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-27 14:09:53.818036 sliderule-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-04-27 14:09:41.000000 sliderule-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 14:09:53.818036 sliderule-3.1.0/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/arcticdem.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24752 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16811 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36102 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44220 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 14:09:53.818036 sliderule-3.1.0/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-27 14:09:53.000000 sliderule-3.1.0/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-04-27 14:09:53.000000 sliderule-3.1.0/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 14:09:53.000000 sliderule-3.1.0/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-27 14:09:53.000000 sliderule-3.1.0/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-27 14:09:53.000000 sliderule-3.1.0/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 14:09:53.818036 sliderule-3.1.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/_landsat.py
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/hls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/landsat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/lpdaac_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-27 14:09:41.000000 sliderule-3.1.0/version.txt
```

### Comparing `sliderule-3.0.6/LICENSE` & `sliderule-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/PKG-INFO` & `sliderule-3.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.0.6
+Version: 3.1.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.0.6/README.md` & `sliderule-3.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "cnf": icesat2.CNF_SURFACE_HIGH,
     "len": 40.0,
     "res": 20.0,
     "maxi": 1
 }
 
 # make request
-rsps = icesat2.atl06p(parms, "nsidc-s3")
+rsps = icesat2.atl06p(parms, "icesat2")
 print(f"{rsps}")
 ```
 
 More extensive examples in the form of Jupyter Notebooks can be found in the [examples](https://github.com/ICESat2-SlideRule/sliderule-python/tree/main/examples) folder of the [sliderule-python](https://github.com/ICESat2-SlideRule/sliderule-python) repository.
 
 ## III. Reference and User's Guide
```

### Comparing `sliderule-3.0.6/setup.py` & `sliderule-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/sliderule/arcticdem.py` & `sliderule-3.1.0/sliderule/arcticdem.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/sliderule/earthdata.py` & `sliderule-3.1.0/sliderule/earthdata.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/sliderule/gedi.py` & `sliderule-3.1.0/sliderule/gedi.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import time
-import datetime
 import logging
 import numpy
 import geopandas
 import sliderule
 from sliderule import earthdata
 
 ###############################################################################
@@ -41,16 +40,18 @@
 
 # create logger
 logger = logging.getLogger(__name__)
 
 # profiling times for each major function
 profiles = {}
 
-# default asset
-DEFAULT_ASSET="ornl-s3"
+# default assets
+DEFAULT_L1B_ASSET="gedil1b"
+DEFAULT_L2A_ASSET="gedil2a"
+DEFAULT_L4A_ASSET="gedil4a"
 
 # default GEDI standard data product version
 DEFAULT_GEDI_SDP_VERSION = '2'
 
 # gedi parameters
 ALL_BEAMS = -1
 
@@ -205,14 +206,46 @@
 
     # Return Resources
     if kwargs['return_metadata']:
         return (resources,metadata)
     else:
         return resources
 
+#
+#  Perform Processing Request
+#
+def __processing_request(parm, asset, callbacks, resources, keep_id, dataset, api, rec, profile):
+    try:
+        tstart = time.perf_counter()
+
+        # Get List of Resources from CMR (if not supplied)
+        if resources == None:
+            resources = __query_resources(parm, dataset)
+
+        # Build GEDI Request
+        parm["asset"] = asset
+        rqst = {
+            "resources": resources,
+            "parms": parm
+        }
+
+        # Make API Processing Request
+        rsps = sliderule.source(api, rqst, stream=True, callbacks=callbacks)
+
+        # Flatten Responses
+        gdf = __flattenbatches(rsps, rec, 'footprint', parm, keep_id)
+
+        # Return Response
+        profiles[profile] = time.perf_counter() - tstart
+        return gdf
+
+    # Handle Runtime Errors
+    except RuntimeError as e:
+        logger.critical(e)
+        return sliderule.emptyframe()
 
 ###############################################################################
 # APIs
 ###############################################################################
 
 #
 #  Initialize
@@ -234,17 +267,17 @@
     '''
     sliderule.init(url, verbose, loglevel, organization, desired_nodes, time_to_live, bypass_dns, plugins=['gedi'])
     earthdata.set_max_resources(max_resources) # set maximum number of resources allowed per request
 
 #
 #  GEDI L4A
 #
-def gedi04a (parm, resource, asset=DEFAULT_ASSET):
+def gedi04a (parm, resource, asset=DEFAULT_L4A_ASSET):
     '''
-    Performs GEDI L4A subsetting returns gridded elevations
+    Performs GEDI L4A subsetting of elevation footprints
 
     Parameters
     ----------
     parms:      dict
                 parameters used to configure subsetting process
     resource:   str
                 GEDI HDF5 filename
@@ -255,19 +288,19 @@
     -------
     GeoDataFrame
         gridded footrpints
     '''
     return gedi04ap(parm, asset=asset, resources=[resource])
 
 #
-#  Parallel ATL06
+#  Parallel GEDI04A
 #
-def gedi04ap(parm, asset=DEFAULT_ASSET, callbacks={}, resources=None, keep_id=False):
+def gedi04ap(parm, asset=DEFAULT_L4A_ASSET, callbacks={}, resources=None, keep_id=False):
     '''
-    Performs subsetting in parallel on GEDI data and returns gridded footprints.  This function expects that the **parm** argument
+    Performs subsetting in parallel on GEDI data and returns elevation footprints.  This function expects that the **parm** argument
     includes a polygon which is used to fetch all available resources from the CMR system automatically.  If **resources** is specified
     then any polygon or resource filtering options supplied in **parm** are ignored.
 
     Parameters
     ----------
         parms:          dict
                         parameters used to configure subsetting process
@@ -279,15 +312,15 @@
                         a list of granules to process (e.g. ["GEDI04_A_2019229131935_O03846_02_T03642_02_002_02_V002.h5", ...])
         keep_id:        bool
                         whether to retain the "extent_id" column in the GeoDataFrame for future merges
 
     Returns
     -------
     GeoDataFrame
-        gridded footprints
+        geolocated footprints
 
     Examples
     --------
         >>> from sliderule import gedi
         >>> gedi.init()
         >>> region = [ {"lon":-105.82971551223244, "lat": 39.81983728534918},
         ...            {"lon":-105.30742121965137, "lat": 39.81983728534918},
@@ -295,35 +328,140 @@
         ...            {"lon":-105.82971551223244, "lat": 40.164048017973755},
         ...            {"lon":-105.82971551223244, "lat": 39.81983728534918} ]
         >>> parms = { "poly": region }
         >>> resources = ["GEDI04_A_2019229131935_O03846_02_T03642_02_002_02_V002.h5"]
         >>> asset = "ornldaac-s3"
         >>> rsps = gedi.gedi04ap(parms, asset=asset, resources=resources)
     '''
-    try:
-        tstart = time.perf_counter()
+    return __processing_request(parm, asset, callbacks, resources, keep_id, 'GEDI_L4A_AGB_Density_V2_1_2056', 'gedi04ap', 'gedi04arec', gedi04ap.__name__)
 
-        # Get List of Resources from CMR (if not supplied)
-        if resources == None:
-            resources = __query_resources(parm, 'GEDI_L4A_AGB_Density_V2_1_2056')
+#
+#  GEDI L2A
+#
+def gedi02a (parm, resource, asset=DEFAULT_L2A_ASSET):
+    '''
+    Performs GEDI L2A subsetting of elevation footprints
 
-        # Build ATL06 Request
-        parm["asset"] = asset
-        rqst = {
-            "resources": resources,
-            "parms": parm
-        }
+    Parameters
+    ----------
+    parms:      dict
+                parameters used to configure subsetting process
+    resource:   str
+                GEDI HDF5 filename
+    asset:      str
+                data source asset
 
-        # Make API Processing Request
-        rsps = sliderule.source("gedi04ap", rqst, stream=True, callbacks=callbacks)
+    Returns
+    -------
+    GeoDataFrame
+        gridded footrpints
+    '''
+    return gedi02ap(parm, asset=asset, resources=[resource])
 
-        # Flatten Responses
-        gdf = __flattenbatches(rsps, 'gedi04arec', 'footprint', parm, keep_id)
+#
+#  Parallel GEDI02A
+#
+def gedi02ap(parm, asset=DEFAULT_L2A_ASSET, callbacks={}, resources=None, keep_id=False):
+    '''
+    Performs subsetting in parallel on GEDI data and returns geolocated footprints.  This function expects that the **parm** argument
+    includes a polygon which is used to fetch all available resources from the CMR system automatically.  If **resources** is specified
+    then any polygon or resource filtering options supplied in **parm** are ignored.
 
-        # Return Response
-        profiles[gedi04ap.__name__] = time.perf_counter() - tstart
-        return gdf
+    Parameters
+    ----------
+        parms:          dict
+                        parameters used to configure subsetting process
+        asset:          str
+                        data source asset
+        callbacks:      dictionary
+                        a callback function that is called for each result record
+        resources:      list
+                        a list of granules to process (e.g. ["GEDI04_A_2019229131935_O03846_02_T03642_02_002_02_V002.h5", ...])
+        keep_id:        bool
+                        whether to retain the "extent_id" column in the GeoDataFrame for future merges
 
-    # Handle Runtime Errors
-    except RuntimeError as e:
-        logger.critical(e)
-        return sliderule.emptyframe()
+    Returns
+    -------
+    GeoDataFrame
+        geolocated footprints
+
+    Examples
+    --------
+        >>> from sliderule import gedi
+        >>> gedi.init()
+        >>> region = [ {"lon":-105.82971551223244, "lat": 39.81983728534918},
+        ...            {"lon":-105.30742121965137, "lat": 39.81983728534918},
+        ...            {"lon":-105.30742121965137, "lat": 40.164048017973755},
+        ...            {"lon":-105.82971551223244, "lat": 40.164048017973755},
+        ...            {"lon":-105.82971551223244, "lat": 39.81983728534918} ]
+        >>> parms = { "poly": region }
+        >>> resources = ["GEDI02_A_2019229131935_O03846_02_T03642_02_002_02_V002.h5"]
+        >>> asset = "gedi-local"
+        >>> rsps = gedi.gedi02ap(parms, asset=asset, resources=resources)
+    '''
+    return __processing_request(parm, asset, callbacks, resources, keep_id, 'GEDI02_A', 'gedi02ap', 'gedi02arec', gedi02ap.__name__)
+
+#
+#  GEDI L1B
+#
+def gedi01b (parm, resource, asset=DEFAULT_L1B_ASSET):
+    '''
+    Performs GEDI L1B subsetting of elevation waveforms
+
+    Parameters
+    ----------
+    parms:      dict
+                parameters used to configure subsetting process
+    resource:   str
+                GEDI HDF5 filename
+    asset:      str
+                data source asset
+
+    Returns
+    -------
+    GeoDataFrame
+        gridded footrpints
+    '''
+    return gedi01bp(parm, asset=asset, resources=[resource])
+
+#
+#  Parallel GEDI01B
+#
+def gedi01bp(parm, asset=DEFAULT_L1B_ASSET, callbacks={}, resources=None, keep_id=False):
+    '''
+    Performs subsetting in parallel on GEDI data and returns geolocated footprints.  This function expects that the **parm** argument
+    includes a polygon which is used to fetch all available resources from the CMR system automatically.  If **resources** is specified
+    then any polygon or resource filtering options supplied in **parm** are ignored.
+
+    Parameters
+    ----------
+        parms:          dict
+                        parameters used to configure subsetting process
+        asset:          str
+                        data source asset
+        callbacks:      dictionary
+                        a callback function that is called for each result record
+        resources:      list
+                        a list of granules to process (e.g. ["GEDI04_A_2019229131935_O03846_02_T03642_02_002_02_V002.h5", ...])
+        keep_id:        bool
+                        whether to retain the "extent_id" column in the GeoDataFrame for future merges
+
+    Returns
+    -------
+    GeoDataFrame
+        geolocated footprints
+
+    Examples
+    --------
+        >>> from sliderule import gedi
+        >>> gedi.init()
+        >>> region = [ {"lon":-105.82971551223244, "lat": 39.81983728534918},
+        ...            {"lon":-105.30742121965137, "lat": 39.81983728534918},
+        ...            {"lon":-105.30742121965137, "lat": 40.164048017973755},
+        ...            {"lon":-105.82971551223244, "lat": 40.164048017973755},
+        ...            {"lon":-105.82971551223244, "lat": 39.81983728534918} ]
+        >>> parms = { "poly": region }
+        >>> resources = ["GEDI01_B_2019229131935_O03846_02_T03642_02_002_02_V002.h5"]
+        >>> asset = "gedi-local"
+        >>> rsps = gedi.gedi01bp(parms, asset=asset, resources=resources)
+    '''
+    return __processing_request(parm, asset, callbacks, resources, keep_id, 'GEDI01_B', 'gedi01bp', 'gedi01brec', gedi01bp.__name__)
```

### Comparing `sliderule-3.0.6/sliderule/h5.py` & `sliderule-3.1.0/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/sliderule/icesat2.py` & `sliderule-3.1.0/sliderule/icesat2.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 # create logger
 logger = logging.getLogger(__name__)
 
 # profiling times for each major function
 profiles = {}
 
 # default asset
-DEFAULT_ASSET="nsidc-s3"
+DEFAULT_ASSET="icesat2"
 
 # default standard data product version
 DEFAULT_ICESAT2_SDP_VERSION='005'
 
 # icesat2 parameters
 CNF_POSSIBLE_TEP = -2
 CNF_NOT_CONSIDERED = -1
```

### Comparing `sliderule-3.0.6/sliderule/io.py` & `sliderule-3.1.0/sliderule/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -265,14 +265,64 @@
     elif isinstance(attr, (np.bool_)):
         return bool(attr)
     elif isinstance(attr, (np.void)):
         return None
     else:
         return attr
 
+# conversion factors between time units and seconds
+_to_sec = {'microseconds': 1e-6, 'microsecond': 1e-6,
+           'microsec': 1e-6, 'microsecs': 1e-6,
+           'milliseconds': 1e-3, 'millisecond': 1e-3,
+           'millisec': 1e-3, 'millisecs': 1e-3,
+           'msec': 1e-3, 'msecs': 1e-3, 'ms': 1e-3,
+           'seconds': 1.0, 'second': 1.0, 'sec': 1.0,
+           'secs': 1.0, 's': 1.0,
+           'minutes': 60.0, 'minute': 60.0,
+           'min': 60.0, 'mins': 60.0,
+           'hours': 3600.0, 'hour': 3600.0,
+           'hr': 3600.0, 'hrs': 3600.0, 'h': 3600.0,
+           'day': 86400.0, 'days': 86400.0, 'd': 86400.0}
+
+# PURPOSE: split a date string into units and epoch
+def split_date_string(date_string: str):
+    """
+    split a date string into units and epoch
+
+    Parameters
+    ----------
+    date_string: str
+        time-units since yyyy-mm-dd hh:mm:ss
+    """
+    try:
+        units,_,epoch = date_string.split(None, 2)
+    except ValueError:
+        raise ValueError(f'Invalid format: {date_string}')
+    else:
+        return (units.lower(), epoch)
+
+# PURPOSE: convert a numpy datetime array to delta times from the UNIX epoch
+def convert_datetime(date, epoch='2018-01-01T00:00:00'):
+    """
+    Convert a numpy datetime array to seconds since ``epoch``
+
+    Parameters
+    ----------
+    date: obj
+        numpy datetime array
+    epoch: str, default '2018-01-01T00:00:00'
+        epoch for output delta_time
+
+    Returns
+    -------
+    delta_time: float
+        seconds since epoch
+    """
+    return (date - np.datetime64(epoch)) / np.timedelta64(1, 's')
+
 # calculate centroid of polygon
 def centroid(x,y):
     npts = len(x)
     area,cx,cy = (0.0,0.0,0.0)
     for i in range(npts-1):
         SA = x[i]*y[i+1] - x[i+1]*y[i]
         area += SA
@@ -392,30 +442,40 @@
 def to_nc(gdf, filename, **kwargs):
     # set default keyword arguments
     kwargs.setdefault('parameters',None)
     kwargs.setdefault('regions',[])
     kwargs.setdefault('crs','EPSG:4326')
     kwargs.setdefault('lon_key','longitude')
     kwargs.setdefault('lat_key','latitude')
+    kwargs.setdefault('units','seconds since 2018-01-01T00:00:00')
     # get output attributes
     attributes = get_attributes()
     # open netCDF3 file object (64-bit offset format)
     fileID = scipy.io.netcdf.netcdf_file(filename, 'w', version=2)
     warnings.filterwarnings("ignore")
     # convert geodataframe to pandas dataframe
     df = geopandas.pd.DataFrame(gdf.drop(columns='geometry'))
     # append latitude and longitude as columns
     lon_key,lat_key = (kwargs['lon_key'],kwargs['lat_key'])
     df[lat_key] = gdf['geometry'].values.y
     df[lon_key] = gdf['geometry'].values.x
     # get geodataframe coordinate system
     if gdf.crs:
         kwargs['crs'] = gdf.crs
-    # create dimensions
-    fileID.createDimension('delta_time', len(df['delta_time']))
+    # create output delta time dimension and variable
+    fileID.createDimension('delta_time', len(df.index))
+    nc = fileID.createVariable('delta_time', 'f8', ('delta_time',))
+    units, epoch = split_date_string(kwargs['units'])
+    delta_time = convert_datetime(df.index, epoch)/_to_sec[units]
+    nc[:] = delta_time.copy()
+    # set attributes for delta time
+    attributes['delta_time']['units'] = kwargs['units']
+    attributes['delta_time']['long_name'] = "Elapsed GPS time"
+    for att_key,att_val in attributes['delta_time'].items():
+        setattr(nc, att_key, att_val)
     # for each variable in the dataframe
     for key,val in df.items():
         if np.issubdtype(val, np.unsignedinteger):
             nc = fileID.createVariable(key, 'i4', ('delta_time',))
             nc[:] = val.astype(np.int32)
         else:
             nc = fileID.createVariable(key, val.dtype, ('delta_time',))
@@ -514,36 +574,38 @@
     # read each region from list attribute
     regions = []
     # counter variable for reading polygon attributes
     i = 0
     while True:
         # attempt to get x and y coordinates for query polygon
         try:
-            x = json.loads(getattr(fileID, 'poly{0:d}_x'.format(i)))
-            y = json.loads(getattr(fileID, 'poly{0:d}_y'.format(i)))
+            x = json.loads(getattr(fileID, f'poly{i:d}_x'))
+            y = json.loads(getattr(fileID, f'poly{i:d}_y'))
         except:
             break
         else:
             # convert x and y coordinates into sliderule region
             regions.append(to_region(x, y))
             # add to polygon counter
             i += 1
-    # Closing the netCDF file
-    fileID.close()
-    warnings.filterwarnings("default")
     # Generate Time Column
-    delta_time = (nc['delta_time']*1e9).astype('timedelta64[ns]')
-    atlas_sdp_epoch = np.datetime64(datetime.datetime(2018, 1, 1))
-    nc['time'] = geopandas.pd.to_datetime(atlas_sdp_epoch + delta_time)
+    units, epoch = split_date_string(fileID.variables['delta_time'].units.decode('utf-8'))
+    delta_time = (1e9*_to_sec[units]*nc['delta_time']).astype('timedelta64[ns]')
+    nc['time'] = geopandas.pd.to_datetime(np.datetime64(epoch) + delta_time)
+    # remove delta time from dictionary
+    del nc['delta_time']
     # generate geometry column
     lon_key,lat_key = (kwargs['lon_key'],kwargs['lat_key'])
     geometry = geopandas.points_from_xy(nc[lon_key],nc[lat_key])
     # remove coordinates from dictionary
     del nc[lon_key]
     del nc[lat_key]
+    # Closing the netCDF file
+    fileID.close()
+    warnings.filterwarnings("default")
     # create Pandas DataFrame object
     df = geopandas.pd.DataFrame(nc)
     # build GeoDataFrame
     gdf = geopandas.GeoDataFrame(df, geometry=geometry, crs=kwargs['crs'])
     # set index
     gdf.set_index(kwargs['index_key'], inplace=True)
     gdf.sort_index(inplace=True)
@@ -569,14 +631,15 @@
     # set default keyword arguments
     kwargs.setdefault('driver','pytables')
     kwargs.setdefault('parameters',None)
     kwargs.setdefault('regions',[])
     kwargs.setdefault('crs','EPSG:4326')
     kwargs.setdefault('lon_key','longitude')
     kwargs.setdefault('lat_key','latitude')
+    kwargs.setdefault('units','seconds since 2018-01-01T00:00:00')
     # get output attributes
     attributes = get_attributes()
     # convert geodataframe to pandas dataframe
     df = geopandas.pd.DataFrame(gdf.drop(columns='geometry'))
     # append latitude and longitude as columns
     lon_key,lat_key = (kwargs['lon_key'],kwargs['lat_key'])
     df[lat_key] = gdf['geometry'].values.y
@@ -640,44 +703,46 @@
             # if empty or unavailable
             pass
     # save each region as a list attribute
     for i,poly in enumerate(kwargs['regions']):
         lon, lat = from_region(poly)
         lon = attributes_encoder(lon)
         lat = attributes_encoder(lat)
-        setattr(fileID.root._v_attrs, 'poly{0:d}_x'.format(i), json.dumps(lon))
-        setattr(fileID.root._v_attrs, 'poly{0:d}_y'.format(i), json.dumps(lat))
+        setattr(fileID.root._v_attrs, f'poly{i:d}_x', json.dumps(lon))
+        setattr(fileID.root._v_attrs, f'poly{i:d}_y', json.dumps(lat))
     # Output HDF5 structure information
     logging.info(filename)
     logging.info(fileID.get_storer('sliderule_segments').non_index_axes[0][1])
     # Closing the HDF5 file
     fileID.close()
 
 # write pandas dataframe to h5py HDF5
 def write_h5py(df, filename, attributes, **kwargs):
     # set default keyword arguments
     kwargs.setdefault('parameters',None)
     kwargs.setdefault('regions',[])
     kwargs.setdefault('crs','EPSG:4326')
+    kwargs.setdefault('units','seconds since 2018-01-01T00:00:00')
     # open HDF5 file object
     fileID = h5py.File(filename, mode='w')
     # create HDF5 records
     h5 = {}
-    # create dataset for variable
+    # create output delta time variable
     key = 'delta_time'
-    h5[key] = fileID.create_dataset(key, df[key].shape, data=df[key],
-        dtype=df[key].dtype, compression='gzip')
-    # set attributes for variable
+    units, epoch = split_date_string(kwargs['units'])
+    delta_time = convert_datetime(df.index, epoch)/_to_sec[units]
+    h5[key] = fileID.create_dataset(key, delta_time.shape, data=delta_time,
+        dtype=delta_time.dtype, compression='gzip')
+    # set attributes for delta time
+    attributes['delta_time']['units'] = kwargs['units']
+    attributes['delta_time']['long_name'] = "Elapsed GPS time"
     for att_key,att_val in attributes[key].items():
         h5[key].attrs[att_key] = att_val
     # for each variable in the dataframe
     for key,val in df.items():
-        # skip delta time variable
-        if (key == 'delta_time'):
-            continue
         # create dataset for variable
         h5[key] = fileID.create_dataset(key, val.shape, data=val,
             dtype=val.dtype, compression='gzip')
         h5[key].dims[0].attach_scale(h5['delta_time'])
         # set attributes for variable
         for att_key,att_val in attributes[key].items():
             h5[key].attrs[att_key] = att_val
@@ -719,16 +784,16 @@
             # if empty or unavailable
             pass
     # save each region as a list attribute
     for i,poly in enumerate(kwargs['regions']):
         lon, lat = from_region(poly)
         lon = attributes_encoder(lon)
         lat = attributes_encoder(lat)
-        fileID.attrs['poly{0:d}_x'.format(i)] = json.dumps(lon)
-        fileID.attrs['poly{0:d}_y'.format(i)] = json.dumps(lat)
+        fileID.attrs[f'poly{i:d}_x'] = json.dumps(lon)
+        fileID.attrs[f'poly{i:d}_y'] = json.dumps(lat)
     # Output HDF5 structure information
     logging.info(filename)
     logging.info(list(fileID.keys()))
     # Closing the HDF5 file
     fileID.close()
 
 # input geodataframe from HDF5
@@ -781,16 +846,16 @@
     # read each region from list attribute
     regions = []
     # counter variable for reading polygon attributes
     i = 0
     while True:
         # attempt to get x and y coordinates for query polygon
         try:
-            x = json.loads(getattr(fileID.root._v_attrs,'poly{0:d}_x'.format(i)))
-            y = json.loads(getattr(fileID.root._v_attrs,'poly{0:d}_y'.format(i)))
+            x = json.loads(getattr(fileID.root._v_attrs,f'poly{i:d}_x'))
+            y = json.loads(getattr(fileID.root._v_attrs,f'poly{i:d}_y'))
         except:
             break
         else:
             # convert x and y coordinates into sliderule region
             regions.append(to_region(x,y))
             # add to polygon counter
             i += 1
@@ -851,35 +916,37 @@
     # read each region from list attribute
     regions = []
     # counter variable for reading polygon attributes
     i = 0
     while True:
         # attempt to get x and y coordinates for query polygon
         try:
-            x = json.loads(fileID.attrs['poly{0:d}_x'.format(i)])
-            y = json.loads(fileID.attrs['poly{0:d}_y'.format(i)])
+            x = json.loads(fileID.attrs[f'poly{i:d}_x'])
+            y = json.loads(fileID.attrs[f'poly{i:d}_y'])
         except:
             break
         else:
             # convert x and y coordinates into sliderule region
             regions.append(to_region(x,y))
             # add to polygon counter
             i += 1
-    # Closing the HDF5 file
-    fileID.close()
     # Generate Time Column
-    delta_time = (h5['delta_time']*1e9).astype('timedelta64[ns]')
-    atlas_sdp_epoch = np.datetime64(datetime.datetime(2018, 1, 1))
-    h5['time'] = geopandas.pd.to_datetime(atlas_sdp_epoch + delta_time)
+    units, epoch = split_date_string(fileID['delta_time'].attrs['units'])
+    delta_time = (1e9*_to_sec[units]*h5['delta_time']).astype('timedelta64[ns]')
+    h5['time'] = geopandas.pd.to_datetime(np.datetime64(epoch) + delta_time)
+    # remove delta time from dictionary
+    del h5['delta_time']
     # generate geometry column
     lon_key,lat_key = (kwargs['lon_key'],kwargs['lat_key'])
     geometry = geopandas.points_from_xy(h5[lon_key],h5[lat_key])
     # remove coordinates from dictionary
     del h5[lon_key]
     del h5[lat_key]
+    # Closing the HDF5 file
+    fileID.close()
     # create Pandas DataFrame object
     df = geopandas.pd.DataFrame(h5)
     # build GeoDataFrame
     gdf = geopandas.GeoDataFrame(df, geometry=geometry, crs=kwargs['crs'])
     # set index
     gdf.set_index(kwargs['index_key'], inplace=True)
     gdf.sort_index(inplace=True)
```

### Comparing `sliderule-3.0.6/sliderule/ipxapi.py` & `sliderule-3.1.0/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/sliderule/ipysliderule.py` & `sliderule-3.1.0/sliderule/ipysliderule.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,16 +77,16 @@
         # set default keyword options
         kwargs.setdefault('style', {})
         # set style
         self.style = copy.copy(kwargs['style'])
 
         # dropdown menu for setting asset
         self.asset = ipywidgets.Dropdown(
-            options=['atlas-local', 'atlas-s3', 'nsidc-s3'],
-            value='nsidc-s3',
+            options=['atlas-local', 'atlas-s3', 'icesat2'],
+            value='icesat2',
             description='Asset:',
             description_tooltip="Asset: Location for SlideRule to get the data",
             disabled=False,
             style=self.style,
         )
 
         # dropdown menu for ICESat-2 product
```

### Comparing `sliderule-3.0.6/sliderule/sliderule.py` & `sliderule-3.1.0/sliderule/sliderule.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,15 +574,15 @@
                         names of the plugins that need to be available on the server
 
     Examples
     --------
         >>> import sliderule
         >>> sliderule.init()
     '''
-    if verbose:
+    if verbose and loglevel == logging.CRITICAL:
         loglevel = logging.INFO
     logging.basicConfig(level=loglevel)
     set_verbose(verbose)
     set_url(url) # configure domain
     authenticate(organization) # configure credentials (if any) for organization
     scaleout(desired_nodes, time_to_live, bypass_dns) # set cluster to desired number of nodes (if permitted based on credentials)
     check_version(plugins=plugins) # verify compatibility between client and server versions
@@ -805,23 +805,43 @@
         >>> import sliderule
         >>> num_servers, max_workers = sliderule.update_available_servers(10)
     '''
     global service_url, service_org, request_timeout
 
     # Update number of nodes
     if type(desired_nodes) == int:
+        rsps_body = {}
+        requested_nodes = desired_nodes
         headers = __build_auth_header()
-        if type(time_to_live) == int:
-            host = "https://ps." + service_url + "/api/desired_org_num_nodes_ttl/" + service_org + "/" + str(desired_nodes) + "/" + str(time_to_live) + "/"
-            rsps = session.post(host, headers=headers, timeout=request_timeout)
-        else:
-            host = "https://ps." + service_url + "/api/desired_org_num_nodes/" + service_org + "/" + str(desired_nodes) + "/"
-            rsps = session.put(host, headers=headers, timeout=request_timeout)
-        rsps.raise_for_status()
 
+        # Get boundaries of cluster and calculate nodes to request
+        try:
+            host = "https://ps." + service_url + "/api/org_num_nodes/" + service_org + "/"
+            rsps = session.get(host, headers=headers, timeout=request_timeout)
+            rsps_body = rsps.json()
+            rsps.raise_for_status()
+            requested_nodes = max(min(desired_nodes, rsps_body["max_nodes"]), rsps_body["min_nodes"])
+        except requests.exceptions.HTTPError as e:
+            logger.info('{}'.format(e))
+            logger.info('Provisioning system status request returned error => {}'.format(rsps_body["error_msg"]))
+
+        # Request number of nodes in cluster
+        try:
+            if type(time_to_live) == int:
+                host = "https://ps." + service_url + "/api/desired_org_num_nodes_ttl/" + service_org + "/" + str(requested_nodes) + "/" + str(time_to_live) + "/"
+                rsps = session.post(host, headers=headers, timeout=request_timeout)
+            else:
+                host = "https://ps." + service_url + "/api/desired_org_num_nodes/" + service_org + "/" + str(requested_nodes) + "/"
+                rsps = session.put(host, headers=headers, timeout=request_timeout)
+            rsps_body = rsps.json()
+            rsps.raise_for_status()
+        except requests.exceptions.HTTPError as e:
+            logger.info('{}'.format(e))
+            logger.error('Provisioning system update request error => {}'.format(rsps_body["error_msg"]))
+    
     # Get number of nodes currently registered
     try:
         rsps = source("status", parm={"service":"sliderule"}, path="/discovery", silence=True)
         available_servers = rsps["nodes"]
     except FatalError:
         available_servers = 0
     return available_servers, available_servers
```

### Comparing `sliderule-3.0.6/sliderule.egg-info/PKG-INFO` & `sliderule-3.1.0/sliderule.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.0.6
+Version: 3.1.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.0.6/sliderule.egg-info/SOURCES.txt` & `sliderule-3.1.0/sliderule.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 utils/build_arctic_dem_mosaics_index.py
 utils/build_arctic_dem_mosaics_vrt_list.py
 utils/build_arctic_dem_strips_vrt.py
 utils/extract_h5_dataset.py
 utils/hls.py
 utils/icepyx_region.py
 utils/landsat.py
+utils/lpdaac_download.py
 utils/monitor.py
 utils/query_cmr.py
 utils/query_elevations.py
 utils/query_metrics.py
 utils/query_photons.py
 utils/query_stac.py
 utils/query_version.py
```

### Comparing `sliderule-3.0.6/utils/_landsat.py` & `sliderule-3.1.0/utils/_landsat.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/big_query.py` & `sliderule-3.1.0/utils/big_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
  't1': '2019-05-02T03:00:00',
  'poly': [{'lat': -64.5, 'lon': 67.7},
   {'lat': -64.5, 'lon': 59.6},
   {'lat': -76.5, 'lon': 59.6},
   {'lat': -76.5, 'lon': 67.7},
   {'lat': -64.5, 'lon': 67.7}]}
 
-gdf = icesat2.atl03sp(params, asset="nsidc-s3", resources=['ATL03_20190502021224_05160312_005_01.h5'], callbacks = {"atl03rec": atl03rec_cb})
+gdf = icesat2.atl03sp(params, asset="icesat2", resources=['ATL03_20190502021224_05160312_005_01.h5'], callbacks = {"atl03rec": atl03rec_cb})
```

### Comparing `sliderule-3.0.6/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.1.0/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.1.0/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.1.0/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/extract_h5_dataset.py` & `sliderule-3.1.0/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/hls.py` & `sliderule-3.1.0/utils/hls.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/icepyx_region.py` & `sliderule-3.1.0/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/landsat.py` & `sliderule-3.1.0/utils/landsat.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/monitor.py` & `sliderule-3.1.0/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/query_cmr.py` & `sliderule-3.1.0/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/query_elevations.py` & `sliderule-3.1.0/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/query_metrics.py` & `sliderule-3.1.0/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/query_photons.py` & `sliderule-3.1.0/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/query_stac.py` & `sliderule-3.1.0/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/query_version.py` & `sliderule-3.1.0/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/region_of_interest.py` & `sliderule-3.1.0/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/results_to_s3.py` & `sliderule-3.1.0/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/stac.py` & `sliderule-3.1.0/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/stream_events.py` & `sliderule-3.1.0/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/tail_events.py` & `sliderule-3.1.0/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.6/utils/utils.py` & `sliderule-3.1.0/utils/utils.py`

 * *Files identical despite different names*


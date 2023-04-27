# Comparing `tmp/pyrsig-0.2.0.tar.gz` & `tmp/pyrsig-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrsig-0.2.0.tar", last modified: Mon Mar 20 20:58:59 2023, max compression
+gzip compressed data, was "dist/pyrsig-0.2.1.tar", last modified: Thu Apr 27 13:41:21 2023, max compression
```

## Comparing `pyrsig-0.2.0.tar` & `pyrsig-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-03-20 20:58:59.000000 pyrsig-0.2.0/
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.2.0/setup.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-03-20 20:58:59.000000 pyrsig-0.2.0/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.2.0/LICENSE
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-03-20 20:58:59.000000 pyrsig-0.2.0/pyrsig.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)      248 2023-03-20 20:58:58.000000 pyrsig-0.2.0/pyrsig.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-03-20 20:58:58.000000 pyrsig-0.2.0/pyrsig.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-03-20 20:58:58.000000 pyrsig-0.2.0/pyrsig.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-03-20 20:58:58.000000 pyrsig-0.2.0/pyrsig.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-03-20 20:58:58.000000 pyrsig-0.2.0/pyrsig.egg-info/requires.txt
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-03-20 20:58:59.000000 pyrsig-0.2.0/pyrsig/
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-03-20 20:58:59.000000 pyrsig-0.2.0/pyrsig/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.2.0/pyrsig/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2613 2023-03-20 17:04:08.000000 pyrsig-0.2.0/pyrsig/tests/test_overall.py
--rw-r--r--   0 bhenders (83225) romo       (131)    25215 2023-03-20 20:58:39.000000 pyrsig-0.2.0/pyrsig/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-03-20 20:58:59.000000 pyrsig-0.2.0/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-03-20 17:04:08.000000 pyrsig-0.2.0/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-04-27 13:41:21.000000 pyrsig-0.2.1/
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.2.1/setup.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-04-27 13:41:21.000000 pyrsig-0.2.1/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.2.1/LICENSE
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)      357 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/requires.txt
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig/
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)      800 2023-03-29 20:44:48.000000 pyrsig-0.2.1/pyrsig/tests/test_api.py
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.2.1/pyrsig/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2058 2023-03-29 20:31:50.000000 pyrsig-0.2.1/pyrsig/tests/test_ioapi.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-03-29 20:35:02.000000 pyrsig-0.2.1/pyrsig/tests/test_misc.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2460 2023-03-29 20:44:35.000000 pyrsig-0.2.1/pyrsig/tests/test_dataframes.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.2.1/pyrsig/tests/test_coards.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    33171 2023-04-26 13:25:55.000000 pyrsig-0.2.1/pyrsig/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-04-27 13:41:21.000000 pyrsig-0.2.1/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.2.1/README.md
```

### Comparing `pyrsig-0.2.0/setup.py` & `pyrsig-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.2.0/PKG-INFO` & `pyrsig-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.2.0/LICENSE` & `pyrsig-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsig-0.2.0/pyrsig.egg-info/PKG-INFO` & `pyrsig-0.2.1/pyrsig.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.2.0/pyrsig/tests/test_overall.py` & `pyrsig-0.2.1/pyrsig/tests/test_ioapi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-def test_initdef():
-    from .. import RsigApi
-
-    RsigApi()
-
-
-def test_init():
-    from .. import RsigApi
-
-    RsigApi(
-        bdate='2022-03-01T00:00:00', edate='2022-03-01T23:59:59',
-        bbox=(-126, 20, -110, 50)
-    )
-
-
 def test_tropomi():
     from .. import RsigApi
     import tempfile
 
     with tempfile.TemporaryDirectory() as td:
         rsigapi = RsigApi(
             bdate='2022-03-01', workdir=td,
@@ -24,84 +9,64 @@
         )
         ds = rsigapi.to_ioapi(
             'tropomi.offl.no2.nitrogendioxide_tropospheric_column'
         )
         print(ds.dims)
 
 
-def test_tropomi_encoding_remove():
+def test_tropomi_cache():
     from .. import RsigApi
     import tempfile
 
     with tempfile.TemporaryDirectory() as td:
         rsigapi = RsigApi(
-            bdate='2022-03-02', workdir=td,
-            bbox=(-97, 20, -65, 50), encoding={'zlib': True, 'complevel': 1}
+            bdate='2022-03-01', workdir=td,
+            bbox=(-97, 20, -65, 50)
         )
         ds = rsigapi.to_ioapi(
-            'tropomi.offl.no2.nitrogendioxide_tropospheric_column',
-            removegz=True
+            'tropomi.offl.no2.nitrogendioxide_tropospheric_column'
         )
         print(ds.dims)
-
-
-def _test_viirsnoaa():
-    """currently not operational. I don't yet know why"""
-    from .. import RsigApi
-    import tempfile
-
-    with tempfile.TemporaryDirectory() as td:
-        rsigapi = RsigApi(bdate='2022-03-01', workdir=td)
         ds = rsigapi.to_ioapi(
-            'viirsnoaa.jrraod.AOD550'
+            'tropomi.offl.no2.nitrogendioxide_tropospheric_column'
         )
         print(ds.dims)
-
-
-def test_aqs_ozone_cache():
-    from .. import RsigApi
-    import tempfile
-
-    with tempfile.TemporaryDirectory() as td:
         rsigapi = RsigApi(
-            bdate='2022-03-01T00', edate='2022-03-01T01', workdir=td
+            bdate='2022-03-01', workdir=td, overwrite=True,
+            bbox=(-97, 20, -65, 50)
         )
-        df = rsigapi.to_dataframe('aqs.ozone')
-        print(df.shape)
-        df = rsigapi.to_dataframe('aqs.ozone')
-        print(df.shape)
+        ds = rsigapi.to_ioapi(
+            'tropomi.offl.no2.nitrogendioxide_tropospheric_column'
+        )
+        print(ds.dims)
 
 
-def test_aqs_no2_verbose():
+def test_tropomi_encoding_remove():
     from .. import RsigApi
     import tempfile
 
     with tempfile.TemporaryDirectory() as td:
         rsigapi = RsigApi(
-            bdate='2022-03-01T00', edate='2022-03-01T01', workdir=td
+            bdate='2022-03-02', workdir=td,
+            bbox=(-97, 20, -65, 50), encoding={'zlib': True, 'complevel': 1}
         )
-        df = rsigapi.to_dataframe('aqs.no2', verbose=1)
-        print(df.shape)
+        ds = rsigapi.to_ioapi(
+            'tropomi.offl.no2.nitrogendioxide_tropospheric_column',
+            removegz=True
+        )
+        print(ds.dims)
 
 
-def test_aqs_no2_unittime():
+def test_tropomi_withmeta():
     from .. import RsigApi
     import tempfile
 
     with tempfile.TemporaryDirectory() as td:
         rsigapi = RsigApi(
-            bdate='2022-03-01T00', edate='2022-03-01T01', workdir=td
+            bdate='2022-03-02', workdir=td,
+            bbox=(-97, 20, -65, 50), encoding={'zlib': True, 'complevel': 1}
         )
-        df = rsigapi.to_dataframe(
-            'aqs.no2', unit_keys=False, parse_dates=True, verbose=1
+        ds = rsigapi.to_ioapi(
+            'tropomi.offl.no2.nitrogendioxide_tropospheric_column',
+            withmeta=True, removegz=True
         )
-        print(df.shape)
-
-
-def test_capabilities():
-    from .. import RsigApi
-
-    rsigapi = RsigApi()
-    keys = rsigapi.keys()
-    print(len(keys))
-    keys = rsigapi.keys(offline=False)
-    print(len(keys))
+        print(ds.dims, len(ds.attrs['metadata']))
```

### Comparing `pyrsig-0.2.0/pyrsig/__init__.py` & `pyrsig-0.2.1/pyrsig/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __all__ = ['RsigApi', 'open_ioapi']
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 
 import pandas as pd
 
 _def_grid_kw = {
     '12US1': dict(
         GDNAM='12US1', GDTYP=2, NCOLS=459, NROWS=299,
         XORIG=-2556000.0, YORIG=-1728000.0, XCELL=12000., YCELL=12000.,
@@ -81,27 +81,98 @@
     'metar.precip1Hour', 'metar.precip3Hour', 'metar.precip6Hour',
     'metar.precip24Hour', 'metar.pressChange3Hour', 'metar.snowCover'
     'nesdis.pm25', 'nesdis.co', 'nesdis.co2', 'nesdis.ch4', 'nesdis.n2o',
     'nesdis.nh3', 'nesdis.nox', 'nesdis.so2', 'nesdis.tnmhc',
     'pandora.ozone', 'purpleair.pm25_corrected',
     'purpleair.pm25_corrected_hourly', 'purpleair.pm25_corrected_daily',
     'purpleair.pm25_corrected_monthly', 'purpleair.pm25_corrected_yearly',
+    'tempo.proxy_l2.no2.vertical_column_total',
+    'tempo.proxy_l2.no2.vertical_column_total_uncertainty',
+    'tempo.proxy_l2.no2.vertical_column_troposphere',
+    'tempo.proxy_l2.no2.vertical_column_stratosphere',
+    'tempo.proxy_l2.no2.amf_total',
+    'tempo.proxy_l2.no2.amf_total_uncertainty',
+    'tempo.proxy_l2.no2.amf_troposphere',
+    'tempo.proxy_l2.no2.amf_stratosphere',
+    'tempo.proxy_l2.no2.ground_pixel_quality_flag'
+    'tempo.proxy_l2.hcho.vertical_column',
+    'tempo.proxy_l2.hcho.vertical_column_uncertainty',
+    'tempo.proxy_l2.hcho.amf',
+    'tempo.proxy_l2.hcho.amf_uncertainty',
+    'tempo.proxy_l2.o3p.total_ozone_column',
+    'tempo.proxy_l2.o3p.troposphere_ozone_column',
+    'tempo.proxy_l2.o3p.stratosphere_ozone_column',
+    'tempo.proxy_l2.o3p.ozone_information_content',
+    'tempo.proxy_l2.o3p.ground_pixel_quality_flag',
     'tropomi.offl.no2.nitrogendioxide_tropospheric_column',
     'tropomi.offl.no2.air_mass_factor_troposphere',
     'tropomi.offl.hcho.formaldehyde_tropospheric_vertical_column',
     'tropomi.offl.co.carbonmonoxide_total_column',
     'tropomi.offl.ch4.methane_mixing_ratio',
     'tropomi.offl.ch4.methane_mixing_ratio',
     'tropomi.offl.ch4.methane_mixing_ratio_bias_corrected',
     'viirsnoaa.jrraod.AOD550', 'viirsnoaa.vaooo.AerosolOpticalDepth_at_550nm',
 )
 
 _point_prefixes = ('airnow', 'aqs', 'purpleair', 'pandora')
 
 
+def parsexml(root):
+    """Recursive xml parsing:
+    Given a root, return dictionaries for each element and its children.
+    Each element has children, attributes (attr), tag, and text.
+    If any of these has no elements, it will be removed.
+    """
+    out = dict(
+        children=[], attr=root.attrib, text=root.text,
+        tag=root.tag.split('}')[1]
+    )
+    for child in root:
+        childd = parsexml(child)
+        out['children'].append(childd)
+    if len(out['children']) == 0:
+        del out['children']
+    if out['text'] is None:
+        out['text'] = ''
+    out['text'] = out['text'].strip()
+    if len(out['text']) == 0:
+        del out['text']
+    if len(out['attr']) == 0:
+        del out['attr']
+    return out
+
+
+def coverages_from_xml(txt):
+    """Based on xml text, create coverage data"""
+    import xml.etree.ElementTree as ET
+    root = ET.fromstring(txt)
+    xmlout = parsexml(root)
+    out = []
+    for c in xmlout['children']:
+        record = {k: v for k, v in c.items() if k != 'children'}
+        kids = c['children']
+        for e in kids:
+            if 'attr' not in e and len(e.get('children', [])) == 0:
+                record[e['tag']] = e.get('text', '')
+            if e['tag'] == 'lonLatEnvelope':
+                envtxt = ''
+                for p in e['children']:
+                    envtxt += ' ' + p['text']
+                record['bbox_str'] = envtxt
+            if e['tag'] == 'domainSet':
+                for s in e['children']:
+                    if s['tag'] == 'temporalDomain':
+                        for tp in s['children']:
+                            for te in tp['children']:
+                                record[te['tag']] = te['text']
+        out.append(record)
+
+    return out
+
+
 def _progress(blocknum, readsize, totalsize):
     """
     Arguments
     ---------
     blocknum : int
         block number of blocks to be read
     readsize : int
@@ -187,15 +258,15 @@
             print('Failed', url, t1 - t0)
         tries += 1
 
         if verbose > 0:
             print('')
 
 
-def open_ioapi(path, earth_radius=6370000.):
+def open_ioapi(path, metapath=None, earth_radius=6370000.):
     import xarray as xr
     import numpy as np
     f = xr.open_dataset(path, engine='netcdf4')
     lvls = f.attrs['VGLVLS']
     tflag = f['TFLAG'][:, 0, :].astype('i').values
     yyyyjjj = tflag[:, 0]
     yyyyjjj = np.where(yyyyjjj < 1, 1970001, yyyyjjj)
@@ -221,14 +292,27 @@
     if f.attrs['GDTYP'] == 2:
         f.attrs['crs_proj4'] = (
             '+proj=lcc +lat_1={P_ALP} +lat_2={P_BET} +lat_0={YCENT}'
             ' +lon_0={XCENT} +R={earth_radius} +x_0={x_0} +y_0={y_0}'
             ' +to_meter={XCELL} +no_defs'
         ).format(**props)
 
+    if metapath is None:
+        import os
+        if os.path.exists(path + '.txt'):
+            metapath = path + '.txt'
+
+    if metapath is False:
+        metapath = None
+
+    if metapath is not None:
+        with open(metapath, 'r') as metaf:
+            metatxt = metaf.read()
+        f.attrs['metadata'] = metatxt
+
     return f
 
 
 class RsigApi:
     def __init__(
         self, key=None, bdate=None, edate=None, bbox=None, grid_kw=None,
         tropomi_kw=None, purpleair_kw=None, viirsnoaa_kw=None,
@@ -301,20 +385,22 @@
           teh api_key property to their own key. Contact PurpleAir for more
           details.
 
         """
         self._description = {}
         self._keys = None
         self._capabilities = None
+        self._describecoverage = None
         self.server = server
         self.key = key
         self.compress = compress
         self.workdir = workdir
         self.encoding = encoding
         self.overwrite = overwrite
+
         if bbox is None:
             self.bbox = (-126, 24, -66, 50)
         else:
             self.bbox = bbox
         if bdate is None:
             bdate = (
                 pd.to_datetime('now') - pd.to_timedelta('1day')
@@ -325,14 +411,15 @@
             self.edate = edate
         else:
             self.edate = pd.to_datetime(edate)
 
         self.corners = corners
         if grid_kw is None:
             grid_kw = '12US1'
+
         if isinstance(grid_kw, str):
             if grid_kw not in _def_grid_kw:
                 raise KeyError('unknown grid, you must specify properites')
             grid_kw = _def_grid_kw[grid_kw].copy()
 
         self.grid_kw = grid_kw
 
@@ -352,36 +439,130 @@
                 'maximum_difference': 5, 'maximum_ratio': 0.70,
                 'agg_pct': 75, 'api_key': '<your key here>'
             }
 
         self.purpleair_kw = purpleair_kw
 
     def describe(self, key):
+        """
+        Describe is currently unreliable becuase of malformed xml.
+        Use descriptions and query by name.
+        """
         import requests
         if key not in self._description:
             r = requests.get(
                 f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
                 f'1.0.0&REQUEST=DescribeCoverage&COVERAGE={key}&compress=1'
             )
             self._description[key] = r.text
+
         return self._description[key]
 
+    def descriptions(self, as_dataframe=True):
+        """
+        Experimental and may change.
+
+        Currently, parses capabilities using xml.etree.ElementTree and returns
+        coverages from details available in CoverageOffering elements from
+        DescribeCoverage.
+
+        Currently cleaning up data xml elements that are bad and doing a
+        per-coverage parsing to increase fault tolerance in the xml.
+
+        Examples:
+
+            rsigapi = pyrsig.RsigApi()
+            desc = rsigapi.descriptions()
+            desc[desc['name'].str.startswith('tropomi')]
+
+        """
+        import re
+        import pandas as pd
+        import warnings
+
+        c = self.describecoverages()
+        ctext = c.text.replace('<?xml version="1.0" encoding="UTF-8" ?>', '')
+        # Currently correcting information that wasn't working.
+        ctext = ctext.replace('<=', 'less than or equal to')
+        ctext = ctext.replace('<0=', 'less than zero =')
+        ctext = ctext.replace('>0=', 'greater than zero =')
+        ctext = ctext.replace(
+            '<lonLatEnvelope srsName="WGS84(DD)"\n',
+            '<lonLatEnvelope srsName="WGS84(DD)">\n'
+        )
+        cleanre = re.compile(
+            r'\</name\>.+?\</CoverageOffering\>',
+            flags=re.MULTILINE + re.DOTALL
+        )
+        # <CoverageOffering>.+?</CoverageOffering>
+        coverre = re.compile(
+            r'\<CoverageOffering\>.+?\</CoverageOffering\>',
+            flags=re.MULTILINE + re.DOTALL
+        )
+        coverages = []
+        for rex in coverre.finditer(ctext):
+            secttxt = ctext[rex.start():rex.end()]
+            secttxt = (
+                '<CoverageDescription version="1.0.0"'
+                + ' xmlns="http://www.opengeospatial.org/standards/wcs"'
+                + ' xmlns:gml="http://www.opengis.net/gml"'
+                + ' xmlns:xlink="http://www.w3.org/1999/xlink">'
+                + secttxt + '</CoverageDescription>'
+            )
+            try:
+                coverage = coverages_from_xml(secttxt)
+                coverages.extend(coverage)
+            except Exception as e:
+                try:
+                    secttxt = cleanre.sub(
+                        '</name></CoverageOffering>', secttxt
+                    )
+                    coverage = coverages_from_xml(secttxt)
+                    coverages.extend(coverage)
+                    warnings.warn(f'Limited details for {coverage[0]["name"]}')
+                except Exception as e2:
+                    # If a secondary error was raised, print it... but raise
+                    # the original error
+                    print(e)
+                    raise e2
+
+        if as_dataframe:
+            coverages = pd.DataFrame.from_records(coverages)
+
+        return coverages
+
     def capabilities(self):
         """
         At this time, the capabilities does not list cmaq.*
 
         """
         import requests
         if self._capabilities is None:
             self._capabilities = requests.get(
                 f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
                 '1.0.0&REQUEST=GetCapabilities&compress=1'
             )
+
         return self._capabilities
 
+    def describecoverages(self):
+        """
+        DescribeCoverage is a call to the server to get all key contents.
+        Right now, I do not allow specific key requests because they are
+        unreliable. They are unreliable because of malformed xml.
+        """
+        import requests
+        if self._describecoverage is None:
+            self._describecoverage = requests.get(
+                f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
+                '1.0.0&REQUEST=DescribeCoverage&compress=1'
+            )
+
+        return self._describecoverage
+
     def keys(self, offline=True):
         """
         Arguments
         ---------
         offline : bool
             If True, uses small cached set of coverages.
             If False, finds all coverages from capabilities.
@@ -410,15 +591,17 @@
             overwrite = self.overwrite
         url, outpath = self._build_url(
             formatstr, key=key, bdate=bdate, edate=edate, bbox=bbox,
             grid=grid, request=request, compress=compress
         )
         if verbose > 0:
             print(url)
+
         _getfile(url, outpath, verbose=verbose, overwrite=overwrite)
+
         return outpath
 
     def _build_url(
         self, formatstr, key=None, bdate=None, edate=None, bbox=None,
         grid=False, request='GetCoverage',
         compress=1
     ):
@@ -431,14 +614,17 @@
             'GetCoverage' or 'GetMetadata'
         all other keywords see __init__
 
         """
         if key is None:
             key = self.key
 
+        if key is None:
+            raise ValueError('key must be specified')
+
         if bdate is None:
             bdate = self.bdate
         else:
             bdate = pd.to_datetime(bdate)
 
         if edate is None:
             if self.edate is None:
@@ -465,14 +651,15 @@
         corners = self.corners
         grid_kw = self.grid_kw
         purpleair_kw = self.purpleair_kw
         tropomi_kw = self.tropomi_kw
         viirsnoaa_kw = self.viirsnoaa_kw
         if compress is None:
             compress = self.compress
+
         wlon, slat, elon, nlat = bbox
         if grid and request == 'GetCoverage':
             gridstr = self._build_grid(grid_kw)
         else:
             gridstr = ''
 
         if key.startswith('viirsnoaa'):
@@ -554,15 +741,15 @@
 
             return gridstr
         else:
             raise KeyError('GDTYP only implemented for ')
 
     def to_dataframe(
         self, key=None, bdate=None, edate=None, bbox=None, unit_keys=True,
-        parse_dates=False, verbose=0
+        parse_dates=False, withmeta=False, verbose=0
     ):
         """
         All arguments default to those provided during initialization.
 
         Arguments
         ---------
         key : str
@@ -575,14 +762,17 @@
         bbox : tuple
           wlon, slat, elon, nlat in decimal degrees (-180 to 180)
         unit_keys : bool
           If True, keep unit in column name.
           If False, move last parenthetical part of key to attrs of Series.
         parse_dates : bool
           If True, parse Timestamp(UTC)
+        withmeta: bool
+          If True, add 'GetMetadata' results as a "metadata" attribute of the
+          dataframe.
         verbose : int
           level of verbosity
 
         Returns
         -------
         df : pandas.DataFrame
             Results from download
@@ -590,14 +780,23 @@
         """
         outpath = self.get_file(
             'ascii', key=key, bdate=bdate, edate=edate, bbox=bbox,
             grid=False, verbose=verbose,
             compress=1
         )
         df = pd.read_csv(outpath, delimiter='\t', na_values=[-9999., -999])
+        if withmeta:
+            metapath = self.get_file(
+                'ascii', key=key, bdate=bdate, edate=edate, bbox=bbox,
+                grid=False, verbose=verbose, request='GetMetadata',
+                compress=1
+            )
+            metatxt = open(metapath, 'r').read()
+            df.attrs['metadata'] = metatxt
+
         if not unit_keys:
             columns = [k for k in df.columns]
             newcolumns = []
             unit_dict = {}
             for k in columns:
                 if '(' not in k:
                     newk = k
@@ -608,25 +807,26 @@
                     unit = k[idx+1:-1]
                 unit_dict[newk] = unit
                 newcolumns.append(newk)
             df.columns = newcolumns
             for k in newcolumns:
                 if hasattr(df[k], 'attrs'):
                     df[k].attrs.update(dict(units=unit_dict.get(k, 'unknown')))
+
         if parse_dates:
             if 'Timestamp(UTC)' in df:
                 df['time'] = pd.to_datetime(df['Timestamp(UTC)'])
             if 'Timestamp' in df:
                 df['time'] = pd.to_datetime(df['Timestamp'])
 
         return df
 
     def to_ioapi(
-        self, key=None, bdate=None, edate=None, bbox=None, removegz=False,
-        verbose=0
+        self, key=None, bdate=None, edate=None, bbox=None, withmeta=False,
+        removegz=False, verbose=0
     ):
         """
         All arguments default to those provided during initialization.
 
         Arguments
         ---------
         key : str
@@ -634,14 +834,17 @@
           or 'tropomi.offl.no2.nitrogendioxide_tropospheric_column')
         bdate : str or pd.Datetime
           beginning date (inclusive) defaults to yesterday at 0Z
         edate : str or pd.Datetime
           ending date (inclusive) defaults to bdate + 23:59:59
         bbox : tuple
           wlon, slat, elon, nlat in decimal degrees (-180 to 180)
+        withmeta : bool
+          If True, add 'GetMetadata' results at an attribute "metadata" to the
+          netcdf file.
         removegz : bool
           If True, then remove the downloaded gz file. Bad for caching.
 
         Returns
         -------
         ds : xarray.Dataset
             Results from download
@@ -673,23 +876,31 @@
                     tvar = tmpf[key]
                     tvar.encoding.update(self.encoding)
                     if key in ('TFLAG', 'COUNT'):
                         tvar.encoding.pop('_FillValue', '')
 
                 tmpf.to_netcdf(outpath[:-3], format='NETCDF4_CLASSIC')
 
-        f = open_ioapi(outpath[:-3])
+        if withmeta:
+            metapath = self.get_file(
+                'netcdf-ioapi', key=key, bdate=bdate, edate=edate, bbox=bbox,
+                grid=True, compress=1, request='GetMetadata', verbose=verbose
+            )
+        else:
+            metapath = None
+
+        f = open_ioapi(outpath[:-3], metapath=metapath)
         if removegz:
             os.remove(outpath)
 
         return f
 
     def to_netcdf(
         self, key=None, bdate=None, edate=None, bbox=None, grid=False,
-        removegz=False, verbose=0
+        withmeta=False, removegz=False, verbose=0
     ):
         """
         All arguments default to those provided during initialization.
 
         Arguments
         ---------
         key : str
@@ -699,14 +910,17 @@
           beginning date (inclusive) defaults to yesterday at 0Z
         edate : str or pd.Datetime
           ending date (inclusive) defaults to bdate + 23:59:59
         bbox : tuple
           wlon, slat, elon, nlat in decimal degrees (-180 to 180)
         grid : bool
           Add column and row variables with grid assignments.
+        withmeta : bool
+          If True, add 'GetMetadata' results at an attribute "metadata" to the
+          netcdf file.
         removegz : bool
           If True, then remove the downloaded gz file. Bad for caching.
 
         Returns
         -------
         ds : xarray.Dataset
             Results from download
@@ -728,11 +942,21 @@
         else:
             with gzip.open(outpath, 'rb') as f_in:
                 with open(outpath[:-3], 'wb') as f_out:
                     shutil.copyfileobj(f_in, f_out)
                     f_out.flush()
 
         f = xr.open_dataset(outpath[:-3])
+
+        if withmeta:
+            metapath = self.get_file(
+                'netcdf-coards', key=key, bdate=bdate, edate=edate, bbox=bbox,
+                grid=grid, compress=1, request='GetMetadata', verbose=verbose
+            )
+            with open(metapath, 'r') as metaf:
+                metatxt = metaf.read()
+            f.attrs['metadata'] = metatxt
+
         if removegz:
             os.remove(outpath)
 
         return f
```

### Comparing `pyrsig-0.2.0/README.md` & `pyrsig-0.2.1/README.md`

 * *Files identical despite different names*


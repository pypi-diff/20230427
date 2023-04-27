# Comparing `tmp/earthscopestraintools-0.1.4.tar.gz` & `tmp/earthscopestraintools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthscopestraintools-0.1.4.tar", last modified: Fri Mar 31 22:49:45 2023, max compression
+gzip compressed data, was "earthscopestraintools-0.1.5.tar", last modified: Thu Apr 27 18:31:20 2023, max compression
```

## Comparing `earthscopestraintools-0.1.4.tar` & `earthscopestraintools-0.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-03-31 22:49:45.906767 earthscopestraintools-0.1.4/
--rw-r--r--   0 gottlieb   (501) staff       (20)     1042 2023-02-21 23:33:21.000000 earthscopestraintools-0.1.4/LICENSE
--rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-03-31 22:49:45.906312 earthscopestraintools-0.1.4/PKG-INFO
--rw-r--r--   0 gottlieb   (501) staff       (20)     1505 2023-03-07 14:24:27.000000 earthscopestraintools-0.1.4/README.md
--rw-r--r--   0 gottlieb   (501) staff       (20)      955 2023-03-31 22:49:31.000000 earthscopestraintools-0.1.4/pyproject.toml
--rw-r--r--   0 gottlieb   (501) staff       (20)       38 2023-03-31 22:49:45.906900 earthscopestraintools-0.1.4/setup.cfg
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-03-31 22:49:45.886141 earthscopestraintools-0.1.4/src/
--rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.4/src/__init__.py
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-03-31 22:49:45.896164 earthscopestraintools-0.1.4/src/earthscopestraintools/
--rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/__init__.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     6920 2023-03-27 21:01:53.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/ascii2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)    10688 2023-02-08 22:58:57.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/bottle.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1563 2023-03-07 13:59:16.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/bottle2mseed.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     5141 2023-03-27 21:06:16.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/bottle2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     6350 2023-03-07 14:19:55.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/bottletar.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     7409 2023-03-27 17:52:37.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/edid.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1591 2023-03-27 17:31:01.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/event.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     8507 2023-03-27 17:34:50.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/event_processing.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     4929 2021-03-10 22:31:02.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/event_site_terms.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)    18373 2023-03-30 14:01:59.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/gtsm_metadata.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     4353 2023-03-27 19:10:40.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/mseed_tools.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     9700 2023-03-30 16:58:05.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/processing.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     4346 2023-03-07 12:51:32.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/tdb2ascii.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     2063 2023-03-07 12:53:14.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/tdb2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)    29779 2023-03-30 13:59:10.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/tiledbtools.py
--rw-r--r--   0 gottlieb   (501) staff       (20)    25580 2023-03-27 20:59:57.000000 earthscopestraintools-0.1.4/src/earthscopestraintools/timeseries.py
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-03-31 22:49:45.901720 earthscopestraintools-0.1.4/src/earthscopestraintools.egg-info/
--rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-03-31 22:49:45.000000 earthscopestraintools-0.1.4/src/earthscopestraintools.egg-info/PKG-INFO
--rw-r--r--   0 gottlieb   (501) staff       (20)     1174 2023-03-31 22:49:45.000000 earthscopestraintools-0.1.4/src/earthscopestraintools.egg-info/SOURCES.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)        1 2023-03-31 22:49:45.000000 earthscopestraintools-0.1.4/src/earthscopestraintools.egg-info/dependency_links.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)      120 2023-03-31 22:49:45.000000 earthscopestraintools-0.1.4/src/earthscopestraintools.egg-info/requires.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)       22 2023-03-31 22:49:45.000000 earthscopestraintools-0.1.4/src/earthscopestraintools.egg-info/top_level.txt
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-03-31 22:49:45.905762 earthscopestraintools-0.1.4/test/
--rw-r--r--   0 gottlieb   (501) staff       (20)      240 2023-03-29 13:58:10.000000 earthscopestraintools-0.1.4/test/test_ascii2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1295 2023-03-07 13:56:58.000000 earthscopestraintools-0.1.4/test/test_bottle2mseed.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     2533 2023-03-07 19:39:09.000000 earthscopestraintools-0.1.4/test/test_bottle2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1336 2023-03-07 14:11:58.000000 earthscopestraintools-0.1.4/test/test_bottletar.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1044 2023-03-27 18:40:20.000000 earthscopestraintools-0.1.4/test/test_edid.py
--rw-r--r--   0 gottlieb   (501) staff       (20)      373 2023-03-13 12:24:04.000000 earthscopestraintools-0.1.4/test/test_gtsm_metadata.py
--rw-r--r--   0 gottlieb   (501) staff       (20)      470 2023-03-06 23:40:58.000000 earthscopestraintools-0.1.4/test/test_tdb2ascii.py
--rw-r--r--   0 gottlieb   (501) staff       (20)      277 2023-03-07 00:03:02.000000 earthscopestraintools-0.1.4/test/test_tdb2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1818 2023-03-27 22:45:21.000000 earthscopestraintools-0.1.4/test/test_ts2tdb.py
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-04-27 18:31:20.104816 earthscopestraintools-0.1.5/
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1042 2023-02-21 23:33:21.000000 earthscopestraintools-0.1.5/LICENSE
+-rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-04-27 18:31:20.104457 earthscopestraintools-0.1.5/PKG-INFO
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1505 2023-03-07 14:24:27.000000 earthscopestraintools-0.1.5/README.md
+-rw-r--r--   0 gottlieb   (501) staff       (20)      955 2023-04-27 18:30:05.000000 earthscopestraintools-0.1.5/pyproject.toml
+-rw-r--r--   0 gottlieb   (501) staff       (20)       38 2023-04-27 18:31:20.104897 earthscopestraintools-0.1.5/setup.cfg
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-04-27 18:31:19.885566 earthscopestraintools-0.1.5/src/
+-rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.5/src/__init__.py
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-04-27 18:31:20.032575 earthscopestraintools-0.1.5/src/earthscopestraintools/
+-rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/__init__.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     6920 2023-03-27 21:01:53.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/ascii2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)    10688 2023-02-08 22:58:57.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/bottle.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1563 2023-03-07 13:59:16.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/bottle2mseed.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     5141 2023-03-27 21:06:16.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/bottle2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     6350 2023-03-07 14:19:55.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/bottletar.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     7409 2023-03-27 17:52:37.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/edid.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1591 2023-03-27 17:31:01.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/event.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     8507 2023-03-27 17:34:50.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/event_processing.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     4929 2021-03-10 22:31:02.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/event_site_terms.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)    18373 2023-03-30 14:01:59.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/gtsm_metadata.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     4353 2023-03-27 19:10:40.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/mseed_tools.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     9700 2023-03-30 16:58:05.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/processing.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     4346 2023-03-07 12:51:32.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/tdb2ascii.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     2063 2023-03-07 12:53:14.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/tdb2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)    29844 2023-04-27 18:29:14.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/tiledbtools.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)    25726 2023-04-04 14:51:28.000000 earthscopestraintools-0.1.5/src/earthscopestraintools/timeseries.py
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-04-27 18:31:20.036919 earthscopestraintools-0.1.5/src/earthscopestraintools.egg-info/
+-rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-04-27 18:31:19.000000 earthscopestraintools-0.1.5/src/earthscopestraintools.egg-info/PKG-INFO
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1174 2023-04-27 18:31:19.000000 earthscopestraintools-0.1.5/src/earthscopestraintools.egg-info/SOURCES.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)        1 2023-04-27 18:31:19.000000 earthscopestraintools-0.1.5/src/earthscopestraintools.egg-info/dependency_links.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)      120 2023-04-27 18:31:19.000000 earthscopestraintools-0.1.5/src/earthscopestraintools.egg-info/requires.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)       22 2023-04-27 18:31:19.000000 earthscopestraintools-0.1.5/src/earthscopestraintools.egg-info/top_level.txt
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-04-27 18:31:20.103455 earthscopestraintools-0.1.5/test/
+-rw-r--r--   0 gottlieb   (501) staff       (20)      240 2023-03-29 13:58:10.000000 earthscopestraintools-0.1.5/test/test_ascii2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1295 2023-03-07 13:56:58.000000 earthscopestraintools-0.1.5/test/test_bottle2mseed.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     2533 2023-03-07 19:39:09.000000 earthscopestraintools-0.1.5/test/test_bottle2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1336 2023-03-07 14:11:58.000000 earthscopestraintools-0.1.5/test/test_bottletar.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1044 2023-03-27 18:40:20.000000 earthscopestraintools-0.1.5/test/test_edid.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)      373 2023-03-13 12:24:04.000000 earthscopestraintools-0.1.5/test/test_gtsm_metadata.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)      470 2023-03-06 23:40:58.000000 earthscopestraintools-0.1.5/test/test_tdb2ascii.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)      277 2023-03-07 00:03:02.000000 earthscopestraintools-0.1.5/test/test_tdb2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1818 2023-03-27 22:45:21.000000 earthscopestraintools-0.1.5/test/test_ts2tdb.py
```

### Comparing `earthscopestraintools-0.1.4/LICENSE` & `earthscopestraintools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/PKG-INFO` & `earthscopestraintools-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthscopestraintools
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of utilities for working with EarthScope strainmeter data
 Author-email: Mike Gottlieb <mike.gottlieb@eartscope.org>
 License: Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `earthscopestraintools-0.1.4/README.md` & `earthscopestraintools-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/pyproject.toml` & `earthscopestraintools-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "earthscopestraintools"
-version ="0.1.4"
+version ="0.1.5"
 authors = [
   { name="Mike Gottlieb", email="mike.gottlieb@eartscope.org" },
 ]
 description = "A collection of utilities for working with EarthScope strainmeter data"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/ascii2tdb.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/ascii2tdb.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/bottle.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/bottle.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/bottle2mseed.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/bottle2mseed.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/bottle2tdb.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/bottle2tdb.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/bottletar.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/bottletar.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/edid.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/edid.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/event.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/event.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/event_processing.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/event_processing.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/event_site_terms.txt` & `earthscopestraintools-0.1.5/src/earthscopestraintools/event_site_terms.txt`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/gtsm_metadata.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/gtsm_metadata.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/mseed_tools.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/mseed_tools.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/processing.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/processing.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/tdb2ascii.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/tdb2ascii.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/tdb2tdb.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/tdb2tdb.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/tiledbtools.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/tiledbtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         return config
 
     def set_default_ctx(self):
         config = self.default_config()
         self.ctx = tiledb.Ctx(config=config)
 
     def get_schema_from_s3(self, schema_type):
+        bucket = "earthscope-tiledb-schema-dev-us-east-2-ebamji"
         s3_schema_uri = f"s3://tiledb-strain/STRAIN_SCHEMA_{schema_type}.tdb"
         logger.info(f"Using schema {s3_schema_uri}")
         config = tiledb.Config()
         config["vfs.s3.region"] = "us-east-2"
         config["vfs.s3.scheme"] = "https"
         config["vfs.s3.endpoint_override"] = ""
         config["vfs.s3.use_virtual_addressing"] = "true"
```

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools/timeseries.py` & `earthscopestraintools-0.1.5/src/earthscopestraintools/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,16 @@
         data: pd.DataFrame = None,
         quality_df: pd.DataFrame = None,
         series: str = "",
         units: str = "",
         level: str = "",
         period: float = 0,
         name: str = None,
+        network: str = "",
+        station: str = "",
     ):
         if data is not None:
             self.data = data
             self.columns = list(data.columns)
         else:
             self.data = pd.DataFrame()
             self.columns = []
@@ -50,18 +52,20 @@
         else:
             self.quality_df = self.set_initial_quality_flags()
 
         self.series = series
         self.units = units
         self.level = level
         self.period = period
+        self.network = network
+        self.station = station
         if name:
             self.name = name
         else:
-            self.name = ""
+            self.name = f"{self.network}.{self.station}"
         self.check_for_gaps()
 
     def set_data(self, df):
         self.data = df
 
     def set_period(self, period):
         self.period = period
```

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools.egg-info/PKG-INFO` & `earthscopestraintools-0.1.5/src/earthscopestraintools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthscopestraintools
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of utilities for working with EarthScope strainmeter data
 Author-email: Mike Gottlieb <mike.gottlieb@eartscope.org>
 License: Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `earthscopestraintools-0.1.4/src/earthscopestraintools.egg-info/SOURCES.txt` & `earthscopestraintools-0.1.5/src/earthscopestraintools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/test/test_bottle2mseed.py` & `earthscopestraintools-0.1.5/test/test_bottle2mseed.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/test/test_bottle2tdb.py` & `earthscopestraintools-0.1.5/test/test_bottle2tdb.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/test/test_bottletar.py` & `earthscopestraintools-0.1.5/test/test_bottletar.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/test/test_edid.py` & `earthscopestraintools-0.1.5/test/test_edid.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.4/test/test_ts2tdb.py` & `earthscopestraintools-0.1.5/test/test_ts2tdb.py`

 * *Files identical despite different names*


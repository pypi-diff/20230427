# Comparing `tmp/asic-0.0.8.post0.tar.gz` & `tmp/asic-0.0.9.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asic-0.0.8.post0.tar", last modified: Tue Aug 16 00:06:35 2022, max compression
+gzip compressed data, was "asic-0.0.9.post0.tar", last modified: Thu Sep  8 14:00:15 2022, max compression
```

## Comparing `asic-0.0.8.post0.tar` & `asic-0.0.9.post0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:06:35.834785 asic-0.0.8.post0/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-08-16 00:06:32.000000 asic-0.0.8.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-08-16 00:06:35.834785 asic-0.0.8.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2687 2022-08-16 00:06:32.000000 asic-0.0.8.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-16 00:06:35.834785 asic-0.0.8.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8788 2022-08-16 00:06:32.000000 asic-0.0.8.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:06:35.830784 asic-0.0.8.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:06:35.834785 asic-0.0.8.post0/src/asic/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8108 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:06:35.834785 asic-0.0.8.post0/src/asic/data/
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/data/ASIC_FILE_CONFIG.jsonl
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/data/ASIC_FILE_EXTENSION_MAP.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:06:35.834785 asic-0.0.8.post0/src/asic/files/
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/adem.py
--rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/aenc.py
--rw-r--r--   0 runner    (1001) docker     (121)    12007 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/afac.py
--rw-r--r--   0 runner    (1001) docker     (121)     4248 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/dspcttos.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/ldcbmr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/pep.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/pubfc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/pubfc_falla_hurto.py
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/sntie.py
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/tgrl.py
--rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/trsd.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/trsm.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/files/undefined.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:06:35.834785 asic-0.0.8.post0/src/asic/ftp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4641 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/ftp/ftp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     5649 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/publication.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-08-16 00:06:32.000000 asic-0.0.8.post0/src/asic/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:06:35.834785 asic-0.0.8.post0/src/asic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-08-16 00:06:35.000000 asic-0.0.8.post0/src/asic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-08-16 00:06:35.000000 asic-0.0.8.post0/src/asic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 00:06:35.000000 asic-0.0.8.post0/src/asic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-16 00:06:35.000000 asic-0.0.8.post0/src/asic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-16 00:06:35.000000 asic-0.0.8.post0/src/asic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-16 00:06:35.000000 asic-0.0.8.post0/src/asic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 14:00:15.236604 asic-0.0.9.post0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-08 14:00:12.000000 asic-0.0.9.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-09-08 14:00:15.236604 asic-0.0.9.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2687 2022-09-08 14:00:12.000000 asic-0.0.9.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 14:00:15.236604 asic-0.0.9.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     8788 2022-09-08 14:00:12.000000 asic-0.0.9.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 14:00:15.232604 asic-0.0.9.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 14:00:15.232604 asic-0.0.9.post0/src/asic/
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8108 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 14:00:15.232604 asic-0.0.9.post0/src/asic/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/data/ASIC_FILE_CONFIG.jsonl
+-rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/data/ASIC_FILE_EXTENSION_MAP.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 14:00:15.232604 asic-0.0.9.post0/src/asic/files/
+-rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/adem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/aenc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12007 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/afac.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4248 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/dspcttos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/ldcbmr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/pep.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/pubfc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/pubfc_falla_hurto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/sntie.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/tgrl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/trsd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/trsm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/files/undefined.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 14:00:15.236604 asic-0.0.9.post0/src/asic/ftp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4641 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/ftp/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5649 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-09-08 14:00:12.000000 asic-0.0.9.post0/src/asic/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 14:00:15.232604 asic-0.0.9.post0/src/asic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-09-08 14:00:15.000000 asic-0.0.9.post0/src/asic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      873 2022-09-08 14:00:15.000000 asic-0.0.9.post0/src/asic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 14:00:15.000000 asic-0.0.9.post0/src/asic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 14:00:15.000000 asic-0.0.9.post0/src/asic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-09-08 14:00:15.000000 asic-0.0.9.post0/src/asic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-08 14:00:15.000000 asic-0.0.9.post0/src/asic.egg-info/top_level.txt
```

### Comparing `asic-0.0.8.post0/LICENSE` & `asic-0.0.9.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/PKG-INFO` & `asic-0.0.9.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asic
-Version: 0.0.8.post0
+Version: 0.0.9.post0
 Summary: Download and format ASIC files
 Home-page: https://github.com/enerBit/asic
 Author: enerBit
 Author-email: jtamayoh@gmail.com
 Project-URL: Source, https://github.com/enerBit/asic.git
 Keywords: asic xm colombia mem ftp development integration expertos mercados mercado energia mayorista
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `asic-0.0.8.post0/README.md` & `asic-0.0.9.post0/README.md`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/setup.py` & `asic-0.0.9.post0/setup.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/cli.py` & `asic-0.0.9.post0/src/asic/cli.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/config.py` & `asic-0.0.9.post0/src/asic/config.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/data/ASIC_FILE_CONFIG.jsonl` & `asic-0.0.9.post0/src/asic/data/ASIC_FILE_CONFIG.jsonl`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/data/ASIC_FILE_EXTENSION_MAP.jsonl` & `asic-0.0.9.post0/src/asic/data/ASIC_FILE_EXTENSION_MAP.jsonl`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/__init__.py` & `asic-0.0.9.post0/src/asic/files/__init__.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/adem.py` & `asic-0.0.9.post0/src/asic/files/adem.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/aenc.py` & `asic-0.0.9.post0/src/asic/files/aenc.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/afac.py` & `asic-0.0.9.post0/src/asic/files/afac.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/dspcttos.py` & `asic-0.0.9.post0/src/asic/files/dspcttos.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/ldcbmr.py` & `asic-0.0.9.post0/src/asic/files/ldcbmr.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/pep.py` & `asic-0.0.9.post0/src/asic/files/pep.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/pubfc.py` & `asic-0.0.9.post0/src/asic/files/pubfc.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/pubfc_falla_hurto.py` & `asic-0.0.9.post0/src/asic/files/pubfc_falla_hurto.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/sntie.py` & `asic-0.0.9.post0/src/asic/files/sntie.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/tgrl.py` & `asic-0.0.9.post0/src/asic/files/tgrl.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/trsd.py` & `asic-0.0.9.post0/src/asic/files/trsd.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/files/trsm.py` & `asic-0.0.9.post0/src/asic/files/trsm.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/ftp/ftp.py` & `asic-0.0.9.post0/src/asic/ftp/ftp.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/metadata.py` & `asic-0.0.9.post0/src/asic/metadata.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/publication.py` & `asic-0.0.9.post0/src/asic/publication.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic/reader.py` & `asic-0.0.9.post0/src/asic/reader.py`

 * *Files identical despite different names*

### Comparing `asic-0.0.8.post0/src/asic.egg-info/PKG-INFO` & `asic-0.0.9.post0/src/asic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asic
-Version: 0.0.8.post0
+Version: 0.0.9.post0
 Summary: Download and format ASIC files
 Home-page: https://github.com/enerBit/asic
 Author: enerBit
 Author-email: jtamayoh@gmail.com
 Project-URL: Source, https://github.com/enerBit/asic.git
 Keywords: asic xm colombia mem ftp development integration expertos mercados mercado energia mayorista
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `asic-0.0.8.post0/src/asic.egg-info/SOURCES.txt` & `asic-0.0.9.post0/src/asic.egg-info/SOURCES.txt`

 * *Files identical despite different names*


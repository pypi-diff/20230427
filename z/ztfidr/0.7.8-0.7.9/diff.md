# Comparing `tmp/ztfidr-0.7.8.tar.gz` & `tmp/ztfidr-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztfidr-0.7.8.tar", last modified: Thu Nov 10 10:02:33 2022, max compression
+gzip compressed data, was "ztfidr-0.7.9.tar", last modified: Fri Nov 11 13:43:13 2022, max compression
```

## Comparing `ztfidr-0.7.8.tar` & `ztfidr-0.7.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-11-10 10:02:33.985393 ztfidr-0.7.8/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.7.8/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      234 2022-11-10 10:02:33.985273 ztfidr-0.7.8/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.7.8/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2022-11-10 10:02:33.985509 ztfidr-0.7.8/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2022-11-10 09:09:29.000000 ztfidr-0.7.8/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-11-10 10:02:33.984616 ztfidr-0.7.8/ztfidr/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2022-11-10 09:09:25.000000 ztfidr-0.7.8/ztfidr/__init__.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11147 2022-11-05 14:23:12.000000 ztfidr-0.7.8/ztfidr/io.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    21919 2022-10-13 13:52:33.000000 ztfidr-0.7.8/ztfidr/lightcurve.py
--rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.7.8/ztfidr/linefitter.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.7.8/ztfidr/salt2.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    24473 2022-11-07 15:47:37.000000 ztfidr-0.7.8/ztfidr/sample.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.7.8/ztfidr/script.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      950 2022-05-18 13:01:28.000000 ztfidr-0.7.8/ztfidr/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    19194 2022-11-05 13:23:19.000000 ztfidr-0.7.8/ztfidr/spectroscopy.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10144 2022-11-05 13:51:48.000000 ztfidr-0.7.8/ztfidr/target.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    18712 2022-11-10 08:58:11.000000 ztfidr-0.7.8/ztfidr/typing.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1443 2022-04-07 08:06:50.000000 ztfidr-0.7.8/ztfidr/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-11-10 10:02:33.985110 ztfidr-0.7.8/ztfidr.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2022-11-10 10:02:33.000000 ztfidr-0.7.8/ztfidr.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      358 2022-11-10 10:02:33.000000 ztfidr-0.7.8/ztfidr.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2022-11-10 10:02:33.000000 ztfidr-0.7.8/ztfidr.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2022-11-10 10:02:33.000000 ztfidr-0.7.8/ztfidr.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-11-11 13:43:13.874855 ztfidr-0.7.9/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.7.9/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2022-11-11 13:43:13.874728 ztfidr-0.7.9/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.7.9/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2022-11-11 13:43:13.874897 ztfidr-0.7.9/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2022-11-11 13:42:57.000000 ztfidr-0.7.9/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-11-11 13:43:13.874070 ztfidr-0.7.9/ztfidr/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2022-11-11 13:42:53.000000 ztfidr-0.7.9/ztfidr/__init__.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11147 2022-11-05 14:23:12.000000 ztfidr-0.7.9/ztfidr/io.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    21919 2022-10-13 13:52:33.000000 ztfidr-0.7.9/ztfidr/lightcurve.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.7.9/ztfidr/linefitter.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.7.9/ztfidr/salt2.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    24627 2022-11-11 13:41:50.000000 ztfidr-0.7.9/ztfidr/sample.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.7.9/ztfidr/script.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      950 2022-05-18 13:01:28.000000 ztfidr-0.7.9/ztfidr/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    19194 2022-11-05 13:23:19.000000 ztfidr-0.7.9/ztfidr/spectroscopy.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10144 2022-11-05 13:51:48.000000 ztfidr-0.7.9/ztfidr/target.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    18712 2022-11-10 08:58:11.000000 ztfidr-0.7.9/ztfidr/typing.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1443 2022-04-07 08:06:50.000000 ztfidr-0.7.9/ztfidr/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-11-11 13:43:13.874573 ztfidr-0.7.9/ztfidr.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2022-11-11 13:43:13.000000 ztfidr-0.7.9/ztfidr.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      358 2022-11-11 13:43:13.000000 ztfidr-0.7.9/ztfidr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2022-11-11 13:43:13.000000 ztfidr-0.7.9/ztfidr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2022-11-11 13:43:13.000000 ztfidr-0.7.9/ztfidr.egg-info/top_level.txt
```

### Comparing `ztfidr-0.7.8/LICENSE` & `ztfidr-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.8/README.md` & `ztfidr-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.8/setup.py` & `ztfidr-0.7.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.7.8'
+VERSION = '0.7.9'
         
 setup(name='ztfidr',
       version=VERSION,
       description='Tools for ZTF Ia *Internal*DataReleases',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/ztfdr',
```

### Comparing `ztfidr-0.7.8/ztfidr/io.py` & `ztfidr-0.7.9/ztfidr/io.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.8/ztfidr/lightcurve.py` & `ztfidr-0.7.9/ztfidr/lightcurve.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.8/ztfidr/linefitter.py` & `ztfidr-0.7.9/ztfidr/linefitter.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.8/ztfidr/salt2.py` & `ztfidr-0.7.9/ztfidr/salt2.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.8/ztfidr/sample.py` & `ztfidr-0.7.9/ztfidr/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,26 @@
 class Sample():
     
     def __init__(self, data=None):
         """ """
         self.set_data(data)
     
     @classmethod
-    def load(cls, redshift_range=None, target_list=None):
+    def load(cls, redshift_range=None, target_list=None, has_spectra=True):
         """ Load a Sample instance building it from io.get_targets_data() """
         data = io.get_targets_data()
         if redshift_range is not None:
             data = data[data["redshift"].between(*redshift_range)]
 
         if target_list is not None:
             data = data.loc[target_list]
+
+        if has_spectra:
+            specfile = io.get_spectra_datafile()
+            data = data[data.index.isin(specfile["ztfname"])]
             
         return cls(data=data)
 
     # ------- #
     # LOADER  #
     # ------- #
     def load_hostdata(self):
```

### Comparing `ztfidr-0.7.8/ztfidr/script.py` & `ztfidr-0.7.9/ztfidr/script.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.8/ztfidr/snid.py` & `ztfidr-0.7.9/ztfidr/snid.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.8/ztfidr/spectroscopy.py` & `ztfidr-0.7.9/ztfidr/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.8/ztfidr/target.py` & `ztfidr-0.7.9/ztfidr/target.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.8/ztfidr/typing.py` & `ztfidr-0.7.9/ztfidr/typing.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.8/ztfidr/utils.py` & `ztfidr-0.7.9/ztfidr/utils.py`

 * *Files identical despite different names*


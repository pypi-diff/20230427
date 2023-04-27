# Comparing `tmp/prodimopy-2.1.5.tar.gz` & `tmp/prodimopy-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodimopy-2.1.5.tar", last modified: Wed Mar 22 21:16:52 2023, max compression
+gzip compressed data, was "prodimopy-2.1.6.tar", last modified: Thu Apr 27 16:13:06 2023, max compression
```

## Comparing `prodimopy-2.1.5.tar` & `prodimopy-2.1.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-03-22 21:16:52.250707 prodimopy-2.1.5/
--rw-r--r--   0 work       (501) staff       (20)      790 2022-01-20 16:31:16.000000 prodimopy-2.1.5/DESCRIPTION.md
--rw-r--r--   0 work       (501) staff       (20)     1069 2022-01-20 16:31:16.000000 prodimopy-2.1.5/LICENSE
--rw-r--r--   0 work       (501) staff       (20)       23 2023-03-17 07:39:25.000000 prodimopy-2.1.5/MANIFEST.in
--rw-r--r--   0 work       (501) staff       (20)     1392 2023-03-22 21:16:52.251014 prodimopy-2.1.5/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     3249 2023-01-12 08:13:23.000000 prodimopy-2.1.5/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-03-22 21:16:52.234637 prodimopy-2.1.5/prodimopy/
--rw-r--r--   0 work       (501) staff       (20)        0 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/__init__.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-03-22 21:16:52.241378 prodimopy-2.1.5/prodimopy/chemistry/
--rw-r--r--   0 work       (501) staff       (20)        0 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/chemistry/__init__.py
--rw-r--r--   0 work       (501) staff       (20)    25757 2022-11-07 17:13:23.000000 prodimopy-2.1.5/prodimopy/chemistry/network.py
--rw-r--r--   0 work       (501) staff       (20)    30925 2022-06-07 21:45:47.000000 prodimopy-2.1.5/prodimopy/compare.py
--rw-r--r--   0 work       (501) staff       (20)    18647 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/extinction.py
--rw-r--r--   0 work       (501) staff       (20)     8251 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/grid.py
--rw-r--r--   0 work       (501) staff       (20)    36560 2022-11-07 17:21:52.000000 prodimopy-2.1.5/prodimopy/hitran.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-03-22 21:16:52.247746 prodimopy-2.1.5/prodimopy/interface1D/
--rw-r--r--   0 work       (501) staff       (20)        0 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/interface1D/__init__.py
--rw-r--r--   0 work       (501) staff       (20)    19062 2022-03-25 14:35:34.000000 prodimopy-2.1.5/prodimopy/interface1D/infile.py
--rw-r--r--   0 work       (501) staff       (20)     8035 2022-03-25 14:35:34.000000 prodimopy-2.1.5/prodimopy/interface1D/twoppToProDiMo.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-03-22 21:16:52.249518 prodimopy-2.1.5/prodimopy/interface2D/
--rw-r--r--   0 work       (501) staff       (20)        0 2022-09-29 19:40:01.000000 prodimopy-2.1.5/prodimopy/interface2D/__init__.py
--rw-r--r--   0 work       (501) staff       (20)     4385 2023-03-17 07:39:25.000000 prodimopy-2.1.5/prodimopy/interface2D/infile.py
--rw-r--r--   0 work       (501) staff       (20)    14741 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/movie.py
--rw-r--r--   0 work       (501) staff       (20)    89882 2023-03-17 07:44:10.000000 prodimopy-2.1.5/prodimopy/plot.py
--rw-r--r--   0 work       (501) staff       (20)    31709 2022-11-24 09:36:45.000000 prodimopy-2.1.5/prodimopy/plot_casasim.py
--rw-r--r--   0 work       (501) staff       (20)    11783 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/plot_mc.py
--rw-r--r--   0 work       (501) staff       (20)    53680 2023-01-13 14:03:21.000000 prodimopy-2.1.5/prodimopy/plot_models.py
--rw-r--r--   0 work       (501) staff       (20)    22131 2023-03-14 13:22:11.000000 prodimopy-2.1.5/prodimopy/plot_slab.py
--rw-r--r--   0 work       (501) staff       (20)   119601 2023-03-22 21:05:00.000000 prodimopy-2.1.5/prodimopy/read.py
--rw-r--r--   0 work       (501) staff       (20)    20456 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/read_casasim.py
--rw-r--r--   0 work       (501) staff       (20)     8556 2023-03-22 21:05:00.000000 prodimopy-2.1.5/prodimopy/read_mc.py
--rw-r--r--   0 work       (501) staff       (20)    89507 2023-03-16 09:17:21.000000 prodimopy-2.1.5/prodimopy/read_slab.py
--rwxr-xr-x   0 work       (501) staff       (20)     2442 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/script_compare.py
--rwxr-xr-x   0 work       (501) staff       (20)     2803 2022-07-28 12:55:01.000000 prodimopy-2.1.5/prodimopy/script_params.py
--rwxr-xr-x   0 work       (501) staff       (20)     6454 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/script_plot.py
--rw-r--r--   0 work       (501) staff       (20)     6667 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/script_plot_models.py
--rw-r--r--   0 work       (501) staff       (20)     3331 2022-03-25 14:35:34.000000 prodimopy-2.1.5/prodimopy/utils.py
--rw-r--r--   0 work       (501) staff       (20)    22755 2022-01-20 16:31:16.000000 prodimopy-2.1.5/prodimopy/utils_casasim.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-03-22 21:16:52.239995 prodimopy-2.1.5/prodimopy.egg-info/
--rw-r--r--   0 work       (501) staff       (20)     1392 2023-03-22 21:16:52.000000 prodimopy-2.1.5/prodimopy.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      981 2023-03-22 21:16:52.000000 prodimopy-2.1.5/prodimopy.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-03-22 21:16:52.000000 prodimopy-2.1.5/prodimopy.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)      181 2023-03-22 21:16:52.000000 prodimopy-2.1.5/prodimopy.egg-info/entry_points.txt
--rw-r--r--   0 work       (501) staff       (20)       93 2023-03-22 21:16:52.000000 prodimopy-2.1.5/prodimopy.egg-info/requires.txt
--rw-r--r--   0 work       (501) staff       (20)       10 2023-03-22 21:16:52.000000 prodimopy-2.1.5/prodimopy.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       67 2023-03-22 21:16:52.252659 prodimopy-2.1.5/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)     5526 2023-03-22 21:10:18.000000 prodimopy-2.1.5/setup.py
+drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.973666 prodimopy-2.1.6/
+-rw-rw-r--   0 rab      (11485) rab      (11485)      790 2023-01-11 15:23:54.000000 prodimopy-2.1.6/DESCRIPTION.md
+-rw-rw-r--   0 rab      (11485) rab      (11485)     1069 2023-01-11 15:23:54.000000 prodimopy-2.1.6/LICENSE
+-rw-rw-r--   0 rab      (11485) rab      (11485)       23 2023-03-16 13:01:01.000000 prodimopy-2.1.6/MANIFEST.in
+-rw-rw-r--   0 rab      (11485) rab      (11485)     1392 2023-04-27 16:13:06.973666 prodimopy-2.1.6/PKG-INFO
+-rw-rw-r--   0 rab      (11485) rab      (11485)     3002 2023-04-14 12:19:49.000000 prodimopy-2.1.6/README.md
+drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.969666 prodimopy-2.1.6/prodimopy/
+-rw-rw-r--   0 rab      (11485) rab      (11485)        0 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/__init__.py
+drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.969666 prodimopy-2.1.6/prodimopy/chemistry/
+-rw-rw-r--   0 rab      (11485) rab      (11485)        0 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/chemistry/__init__.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    25757 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/chemistry/network.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    30948 2023-04-27 10:53:09.000000 prodimopy-2.1.6/prodimopy/compare.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    18647 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/extinction.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)     8251 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/grid.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    36560 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/hitran.py
+drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.973666 prodimopy-2.1.6/prodimopy/interface1D/
+-rw-rw-r--   0 rab      (11485) rab      (11485)        0 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/interface1D/__init__.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    19062 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/interface1D/infile.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)     8035 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/interface1D/twoppToProDiMo.py
+drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.973666 prodimopy-2.1.6/prodimopy/interface2D/
+-rw-rw-r--   0 rab      (11485) rab      (11485)        0 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/interface2D/__init__.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)     4385 2023-04-27 10:53:09.000000 prodimopy-2.1.6/prodimopy/interface2D/infile.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    14741 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/movie.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    91480 2023-04-27 13:48:22.000000 prodimopy-2.1.6/prodimopy/plot.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    31715 2023-04-14 12:19:49.000000 prodimopy-2.1.6/prodimopy/plot_casasim.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    11783 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/plot_mc.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    53612 2023-04-14 12:19:49.000000 prodimopy-2.1.6/prodimopy/plot_models.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    22534 2023-04-27 10:53:16.000000 prodimopy-2.1.6/prodimopy/plot_slab.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)   119635 2023-04-27 10:53:09.000000 prodimopy-2.1.6/prodimopy/read.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    20456 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/read_casasim.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)     8556 2023-04-14 12:19:49.000000 prodimopy-2.1.6/prodimopy/read_mc.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    88984 2023-04-27 16:00:15.000000 prodimopy-2.1.6/prodimopy/read_slab.py
+-rwxrwxr-x   0 rab      (11485) rab      (11485)     2442 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/script_compare.py
+-rwxrwxr-x   0 rab      (11485) rab      (11485)     2803 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/script_params.py
+-rwxrwxr-x   0 rab      (11485) rab      (11485)     6430 2023-04-14 12:19:49.000000 prodimopy-2.1.6/prodimopy/script_plot.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)     6667 2023-01-11 15:23:54.000000 prodimopy-2.1.6/prodimopy/script_plot_models.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)     3331 2023-01-11 15:23:55.000000 prodimopy-2.1.6/prodimopy/utils.py
+-rw-rw-r--   0 rab      (11485) rab      (11485)    22755 2023-01-11 15:23:55.000000 prodimopy-2.1.6/prodimopy/utils_casasim.py
+drwxrwxr-x   0 rab      (11485) rab      (11485)        0 2023-04-27 16:13:06.969666 prodimopy-2.1.6/prodimopy.egg-info/
+-rw-rw-r--   0 rab      (11485) rab      (11485)     1392 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/PKG-INFO
+-rw-rw-r--   0 rab      (11485) rab      (11485)      981 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/SOURCES.txt
+-rw-rw-r--   0 rab      (11485) rab      (11485)        1 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/dependency_links.txt
+-rw-rw-r--   0 rab      (11485) rab      (11485)      181 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/entry_points.txt
+-rw-rw-r--   0 rab      (11485) rab      (11485)       86 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/requires.txt
+-rw-rw-r--   0 rab      (11485) rab      (11485)       10 2023-04-27 16:13:06.000000 prodimopy-2.1.6/prodimopy.egg-info/top_level.txt
+-rw-rw-r--   0 rab      (11485) rab      (11485)       67 2023-04-27 16:13:06.973666 prodimopy-2.1.6/setup.cfg
+-rw-rw-r--   0 rab      (11485) rab      (11485)     5519 2023-04-27 16:05:12.000000 prodimopy-2.1.6/setup.py
```

### Comparing `prodimopy-2.1.5/DESCRIPTION.md` & `prodimopy-2.1.6/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/LICENSE` & `prodimopy-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/PKG-INFO` & `prodimopy-2.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodimopy
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python tools for ProDiMo.
 Home-page: https://gitlab.astro.rug.nl/prodimo/prodimopy/
 Author: Christian Rab
 Author-email: rab@astro.rug.nl
 License: MIT License
 Keywords: astronomy astrophysics star-formation protoplanetary-disks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `prodimopy-2.1.5/README.md` & `prodimopy-2.1.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,81 +12,71 @@
 If you want to take a look before installing you can try prodimopy
 on the web in a binder environment:
 
 [![prodimopy binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fgitlab.astro.rug.nl%2Fprodimo%2Fprodimopy/HEAD?labpath=notebooks)
 
 On your left hand side you will see the notebooks, just open one and try it!
 
+## Documentation
+Please check out the documentation! Click on the badge!
+
+[![Documentation Status](https://readthedocs.org/projects/prodimopy/badge/?version=latest)](https://prodimopy.readthedocs.io/en/latest/?badge=latest)
+
 ## Requirements
 prodimopy uses several additional python packages which are commonly used in the astronomical community. 
-If you use [anaconda](https://www.anaconda.com/distribution/) all this packages should be available in your python distribution. 
-The following packages are required
+If you use [anaconda](https://www.anaconda.com/distribution/) all this packages should be available in your python distribution. The following packages are required
 
-* *matplotib* required for the plotting part only, version>=2 is recommended  
-* *astropy*     version >=2.0 is recommended
-* *numpy*       no known special requirements
+* *matplotib*   required for the plotting part only, version>3 is recommended  
+* *astropy*     version >4.0 
+* *numpy*       version >=1.17
 * *scipy*       no known special requirements
 
 If you use the setup script (see Installation) those packages will be installed automatically if 
-they are not included in your python distribution. We recommend to use python3 but python2 should
-also still work.
+they are not included in your python distribution. There are other dependencies not listed here, but those are only required for special cases (e.g. slab models), but also those dependencies will be installed automatically if required. We only support python3, but python2 might still work.
 
 ## Installation
 
+### via pip (for Users)
+If you just want a stable version you can also use pip to install the project. Just type in the command line 
+
+```
+pip install prodimopy
+```
+
+to upgrade to a new version you can also use pip. We recommend to do it this way. 
+
+```
+pip install --upgrade --upgrade-strategy only-if-needed prodimopy
+```
+
+
+
 ### from source (for Developers)
 I you always want to have the most recent version or if you plan to change the code (you are very welcome) clone this repository and install the package directly from the source: 
 
 * change into a directory of your choice and 
 * clone the repository (git will create a new directory called prodimopy)
 
   ```
   git clone https://gitlab.astro.rug.nl/prodimo/prodimopy.git
   ```    
  
 * change into the newly created prodimopy directory and type:
 
   ```
-  pip install -e .  
+  pip install -e . 
   ```
 
-This will install the package in your current python environment (should be the one you want to use for ProDiMo). 
-The `-e` options allows to update the python code (e.g. via git) without the need to reinstall the package.
-
-If you do not have root access to install python packages, this should work
+  If you do not have root access to install python packages, try this.
 
   ```
   pip install -e . --user
   ```
 
-##### Code Update
-
-Simply type 
+This will install the package in your current python environment (should be the one you want to use for ProDiMo). The `-e` options allows to update the python code (e.g. via git) without the need to reinstall the package. To update the code simply type
 
 ```
 git pull 
 ```
 
 in the prodimopy directory. You can directly use the updated code (no reinstall required).
 
-### via pip (for Users)
-If you just want a stable version you can also use pip to install the project. Just type in the command line 
-
-```
-pip install prodimopy
-```
-
-to upgrade to a new version you can also use pip. We recommend to do it this way. 
-
-```
-pip install --upgrade --upgrade-strategy only-if-needed prodimopy
-```
-    
-### Windows
-
-We do not really recommend it and also do not test it, but it is also possible to use prodimopy with Windows (at least we know about one succesfull case). It worked with the Anaconda distribution for Windows. With the Anaconda prompt (comes with the installation) the installation procedure is the same as above. However, you most likely need to install git first.  
-
-
-## Documentation
-Please check out the documentation! Click on the badge!
-
-[![Documentation Status](https://readthedocs.org/projects/prodimopy/badge/?version=latest)](https://prodimopy.readthedocs.io/en/latest/?badge=latest)
-
```

### Comparing `prodimopy-2.1.5/prodimopy/chemistry/network.py` & `prodimopy-2.1.6/prodimopy/chemistry/network.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/compare.py` & `prodimopy-2.1.6/prodimopy/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     if (fe^feref): return False,None
 
     # FIXME: in restart.dat this CONVERGENCE keywordk makes problems,
     # I think the KEYWORD name is too long (see the fitsheader of reastart.fits.gz)
     # do not test for MAINIT, so that also models that were rerun can be compared
     try:
       diff=FITSDiff(self.m.directory+"/"+fname,self.mref.directory+"/"+fname,
-                    ignore_keywords=['CONVERGENCE',"MAINIT"],
+                    ignore_keywords=['CONVERGENCE',"MAINIT","TIMESTAMP","REVISION"],
                     numdiffs=3,atol=atol,rtol=rtol)
     except Exception as e:
       print("Exception in FITSDiff: ",e)
       return False,None
 
     if diff.identical:
       return True,None
```

### Comparing `prodimopy-2.1.5/prodimopy/extinction.py` & `prodimopy-2.1.6/prodimopy/extinction.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/grid.py` & `prodimopy-2.1.6/prodimopy/grid.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/hitran.py` & `prodimopy-2.1.6/prodimopy/hitran.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/interface1D/infile.py` & `prodimopy-2.1.6/prodimopy/interface1D/infile.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/interface1D/twoppToProDiMo.py` & `prodimopy-2.1.6/prodimopy/interface1D/twoppToProDiMo.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/interface2D/infile.py` & `prodimopy-2.1.6/prodimopy/interface2D/infile.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/movie.py` & `prodimopy-2.1.6/prodimopy/movie.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/plot.py` & `prodimopy-2.1.6/prodimopy/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import division
 from __future__ import print_function
 
 import copy
 import math
-import prodimopy.extinction
-import prodimopy.plot_models
 
 from matplotlib.ticker import MaxNLocator
 from scipy.interpolate import interp1d
 
 import astropy.units as u
 import matplotlib as mpl
 import matplotlib.colors as mcolors
 import matplotlib.pyplot as plt
 import numpy as np
+import prodimopy.extinction
+import prodimopy.plot_models
 
 
 # has to be this way because of circular imports
 class Plot(object):
   '''
   Plot routines for a single ProDiMo model.
   '''
@@ -576,22 +576,22 @@
   #  print pdata.zetaCR[ix,:]
     y1=model.zetaCR[:,0]
     y2=model.zetaX[:,0]*2.0  # convert to per H2 TODO: maybe do this in ProDiMo already to be consistent
     y3=model.zetaSTCR[:,0]  # convert to per H2 TODO: maybe do this in ProDiMo already to be consistent
 
     fig,ax=self._initfig(ax,**kwargs)
 
-    ax.plot(x,y2,color=cX,label="$\zeta_\mathrm{X}$")
-    ax.plot(x,y3,color=cSP,label="$\zeta_\mathrm{SP}$")
-    ax.plot(x,y1,color=cCR,label="$\zeta_\mathrm{CR}$")
+    ax.plot(x,y2,color=cX,label=r"$\zeta_\mathrm{X}$")
+    ax.plot(x,y3,color=cSP,label=r"$\zeta_\mathrm{SP}$")
+    ax.plot(x,y1,color=cCR,label=r"$\zeta_\mathrm{CR}$")
 
     # print ax.get_xlim()
 
     ax.set_xlabel(r"r [au]")
-    ax.set_ylabel("$\mathrm{\zeta\,per\,H_2\,[s^{-1}]}$")
+    ax.set_ylabel(r"$\mathrm{\zeta\,per\,H_2\,[s^{-1}]}$")
 
     ax.semilogy()
     self._dokwargs(ax,**kwargs)
     self._legend(ax)
     # handles, labels = ax.get_legend_handles_labels()
     # ax.legend(handles, labels, loc="best", fancybox=False)
 
@@ -613,25 +613,25 @@
   #  print pdata.zetaCR[ix,:]
     y1=model.zetaCR[ix,:]
     y2=model.zetaX[ix,:]*2.0  # convert to per H2 TODO: maybe do this in ProDiMo already to be consistent
     y3=model.zetaSTCR[ix,:]
 
     fig,ax=self._initfig(ax,**kwargs)
 
-    ax.plot(nhver,y2,color=cX,label="$\zeta_\mathrm{X}$")
-    ax.plot(nhver,y3,color=cSP,label="$\zeta_\mathrm{SP}$")
-    ax.plot(nhver,y1,color=cCR,label="$\zeta_\mathrm{CR}$")
+    ax.plot(nhver,y2,color=cX,label=r"$\zeta_\mathrm{X}$")
+    ax.plot(nhver,y3,color=cSP,label=r"$\zeta_\mathrm{SP}$")
+    ax.plot(nhver,y1,color=cCR,label=r"$\zeta_\mathrm{CR}$")
 
     # set the limits
 
     ax.set_xlim([17.5,nhver.max()])
     ax.set_ylim([1.e-21,1.e-9])
 
     ax.set_xlabel(r"$\log$ N$_\mathrm{<H>,ver}$ [cm$^{-2}$]")
-    ax.set_ylabel("$\zeta$ per H$_2$ [s$^{-1}$]")
+    ax.set_ylabel(r"$\zeta$ per H$_2$ [s$^{-1}$]")
 
     # do axis style
     ax.semilogy()
 
     # title does not work here
     self._dokwargs(ax,title=None,**kwargs)
 
@@ -665,15 +665,15 @@
       if (spec in model.spnames):
         y=model.cdnmol[:,0,model.spnames[spec]]
         y=y/model.NHver[:,0]
         x=model.x[:,0]
 
         style="-"
         if "#" in spec: style="--"
-        ax.plot(x,y,linestyle=style,marker=None,label="$\mathrm{"+spnToLatex(spec)+"}$")
+        ax.plot(x,y,linestyle=style,marker=None,label=r"$\mathrm{"+spnToLatex(spec)+"}$")
 
         iplot=iplot+1
 
     if iplot==0:
       print("Species "+species+" not found in any model!")
       return
 
@@ -740,15 +740,15 @@
 
     self._dokwargs(ax,**kwargs)
     # self._legend(ax)
 
     return self._closefig(fig)
 
   def plot_cdnmol(self,model,species,colors=None,styles=None,
-                  scalefacs=None,norm=None,normidx=None,ylabel="$\mathrm{N_{ver}\,[cm^{-2}}]$",
+                  scalefacs=None,norm=None,normidx=None,ylabel=r"$\mathrm{N_{ver}\,[cm^{-2}}]$",
                   patches=None,ax=None,**kwargs):
     '''
     Plots the vertical column densities as a function of radius for the
     given species.
 
     Parameters
     ----------
@@ -1513,15 +1513,15 @@
 
       marker=None
       if markers!=None:
         marker=markers[iplot]
 
       lines=ax.plot(x,y,marker=marker,ms=4,markeredgecolor=color,markerfacecolor=color,
               linestyle=style,color=color,
-              label="$\mathrm{"+spnToLatex(spec)+"}$")
+              label=r"$\mathrm{"+spnToLatex(spec)+"}$")
 
       if linewidths!=None:
         if linewidths[iplot]!=None:
           lines[-1].set_linewidth(linewidths[iplot])
 
       iplot=iplot+1
       if min(y)<ymin: ymin=min(y)
@@ -1608,15 +1608,15 @@
 
         marker=None
         if markers!=None:
           marker=markers[iplot]
 
         lines=ax.plot(x,y,marker=marker,ms=4,markeredgecolor=color,markerfacecolor=color,
                 linestyle=style,color=color,
-                label="$\mathrm{"+spnToLatex(spec)+"}$")
+                label=r"$\mathrm{"+spnToLatex(spec)+"}$")
 
         if linewidths!=None:
           if linewidths[iplot]!=None:
             lines[-1].set_linewidth(linewidths[iplot])
 
         iplot=iplot+1
         if min(y)<ymin: ymin=min(y)
@@ -1689,15 +1689,15 @@
         style=styles[iplot]
 
       if colors==None:
         color=None
       else:
         color=colors[iplot]
 
-      ax.plot(x,y,marker=None,linestyle=style,color=color,label="$\mathrm{"+spnToLatex(spec)+"}$")
+      ax.plot(x,y,marker=None,linestyle=style,color=color,label=r"$\mathrm{"+spnToLatex(spec)+"}$")
 
       iplot=iplot+1
 
       if min(x)<xmin: xmin=min(x)
       if max(x)>xmax: xmax=max(x)
       if min(y)<ymin: ymin=min(y)
       if max(y)>ymax: ymax=max(y)
@@ -2159,15 +2159,15 @@
     iplot=0
     for lineIdent in lineIdents:
       x=model.x[:,0]
       lineEstimate=model.getLineEstimate(lineIdent[0],lineIdent[1])
       y=[dum.tauLine for dum in lineEstimate.rInfo]
 
       ax.axhline(y=1.0,linestyle="-",color="black",linewidth=0.5)
-      label=r"$\mathrm{"+spnToLatex(lineEstimate.ident)+"}$ "+"{:.2f}".format(lineEstimate.wl)+" $\mathrm{\mu m}$"
+      label=r"$\mathrm{"+spnToLatex(lineEstimate.ident)+"}$ "+"{:.2f}".format(lineEstimate.wl)+r" $\mathrm{\mu m}$"
 
       line,=ax.plot(x,[dum.tauLine for dum in lineEstimate.rInfo],marker=None,label=label)
 
       if showCont:
         ax.plot(x,[dum.tauDust for dum in lineEstimate.rInfo],
                 marker=None,linestyle="--",color=line.get_color())
 
@@ -2264,27 +2264,27 @@
 
       if zr is True:
         for point in points:
           point[1]=point[1]/point[0]
 
       if showBox:
         if len(points)>1:
-          patch=mpl.patches.Polygon(points,True,fill=False,color=boxcolors[ibox],
+          patch=mpl.patches.Polygon(points,closed=True,fill=False,color=boxcolors[ibox],
                                       linestyle=boxlinestyles[ibox],
                                       zorder=100,linewidth=boxlinewidths[ibox])
 
           patches.append(patch)
         else:
           print("WARN: Unable to calculate a proper region for the line origin: "+str(lesti))
 
       if showContOrigin is True:
         if (model.sed is not None and model.sed.sedAna is not None):
           pointsc=self._getSEDana_boxpoints(lesti.wl,model,zr)
           if len(pointsc)>1:
-            patchc=mpl.patches.Polygon(pointsc,True,fill=False,
+            patchc=mpl.patches.Polygon(pointsc,closed=True,fill=False,
                                          color=boxcolors[ibox],zorder=100,
                                          linewidth=1.0,linestyle="--")
             patches.append(patchc)
           else:
             print("WARN: Unable to calculate a proper region for the continuum origin: "+str(lesti))
 
       ibox+=1
@@ -2418,15 +2418,15 @@
       y=y/np.max(y)
 
     if linetxt is None:
       if ident is not None:
         linetxt=ident
       else:
         linetxt=line.species
-      linetxt=linetxt+"@"+"{:.2f}".format(line.wl)+" $\mathrm{\mu m}$"
+      linetxt=linetxt+"@"+"{:.2f}".format(line.wl)+r" $\mathrm{\mu m}$"
 
     if style=="step":
       ax.sep(x,y,marker=None,label=linetxt,where="mid")
     else:
       ax.plot(x,y,marker=None,label=linetxt)
 
     # plot the line profile if it exists
@@ -2490,22 +2490,44 @@
     ppm=prodimopy.plot_models.PlotModels(None,markers=["x"])
     fig=ppm.plot_lines([model],lineIdents,useLineEstimate=useLineEstimate,jansky=jansky,
                  showBoxes=showBoxes,lineObs=lineObs,lineObsLabel=lineObsLabel,peakFlux=peakFlux,
                  showCont=showCont,xLabelGHz=xLabelGHz,showGrid=showGrid,**kwargs)
 
     return self._closefig(fig)
 
-  def plot_heat_cool(self,model,zr=True,oconts=None,**kwargs):
+  def plot_heat_cool(self,model,zr=True,oconts=None,showidx=(0,0),**kwargs):
     """
     Plots the dominant heating and cooling processes.
 
     The initial python code for this routine is from Frank Backs
 
-    TODO: possibility to have different oconts for the heating and cooling figures
-    TODO: possibility to map certain heating/cooling processes always to the same color
+    Parameters
+    ----------
+
+    model : :class:`~prodimopy.read.Data_ProDiMo`
+      the model data
+
+    zr : boolean
+      use z/r for y axis Default: True
+
+    oconts : array_like(:class:`~prodimopy.plot.Contour`,ndim=1)
+      list of :class:`~prodimopy.plot.Contour` objects which will be drawn
+      contours (like in :func:`~prodimopy.plot.Plot.plot_cont`.
+
+    showidx : tuple(ndim=1)
+      Default is (0,0): will show the most dominant heating and cooling process.
+      For example (1,1) will show the second most dominant heating and cooling process.
+      For example (-1,-1) will show the least dominant heating and cooling process.
+
+
+    .. todo::
+
+      * possibility to have different oconts for the heating and cooling figures
+      * possibility to map certain heating/cooling processes always to the same color
+
     """
     print("PLOT: plot_heat_cool ...")
 
     colors=np.array([(230,25,75),(60,180,75),(255,225,25),(0,130,200),
                         (245,130,48),(145,30,180),(70,240,240),(240,50,230),
                         (210,245,60),(250,190,190),(0,128,128),(230,190,255),
                         (170,110,40),(255,250,200),(128,0,0),(170,255,95),
@@ -2517,26 +2539,52 @@
       z=model.z/model.x
     else:
       z=model.z
 
     # used for plotting
     max_idx=np.zeros(shape=(model.nx,model.nz),dtype='int16')
 
+    # heat_mainidx=model.heat_mainidx
+    # cool_mainidx=model.cool_mainidx
+
+    # sort the heat/cool .. this allows to also plot e.g. the second most
+    # important etc. i.e. differently to using heat_mainidx from ProDiMo.out
+
+    # sortidx is  most important one first +1 to be consistent with
+    # model_heatmainidx from ProDiMo.out ... makes checking easier
+    heat_mainidx=np.flip(np.argsort(model.heat,axis=2),axis=2)[:,:,showidx[0]]+1
+    cool_mainidx=np.flip(np.argsort(model.cool,axis=2),axis=2)[:,:,showidx[1]]+1
+
     # list of all the dominant heating processes
-    idxlisth,idxlisth_counts=np.unique(model.heat_mainidx,return_counts=True)
-    idxlistc,idxlistc_counts=np.unique(model.cool_mainidx,return_counts=True)
+
+    idxlisth,idxlisth_counts=np.unique(heat_mainidx,return_counts=True)
+    idxlistc,idxlistc_counts=np.unique(cool_mainidx,return_counts=True)
 
     # sort it descending
     idxlisth=idxlisth[np.argsort(idxlisth_counts)[::-1]]
     idxlistc=idxlistc[np.argsort(idxlistc_counts)[::-1]]
 
-    # axis equal needs to be done here already ... at least it seems so
     sfigs=[2.0,1.3]
     if "sfigs" in kwargs: sfigs=kwargs["sfigs"]
 
+    # build title strings
+    titles=list()
+    for idx,tit in zip(showidx,["heating processes","cooling processes"]):
+      # FIXME: (somehow) least impo
+      if idx==-1:
+        titles.append("least important "+tit)
+      elif idx==0:
+        titles.append("dominant "+tit)
+      elif idx>0 and idx<3:
+        titles.append(str(idx+1)+"nd most dominant "+tit)
+      elif idx>=3:
+        titles.append(str(idx+1)+"th most dominant "+tit)
+      else:
+        titles.append(str(idx)+" (idx) "+tit)
+
     fig,axarr=plt.subplots(1,2,figsize=self._sfigs(sfigs=sfigs))
     plt.subplots_adjust(bottom=0.3)
     axh=axarr[0]
     axc=axarr[1]
 
     if len(idxlisth)>len(colors):
       print("WARN: too many heating processes, do not show the least important ones:")
@@ -2546,43 +2594,43 @@
     # this if for the labels, and also maps the colors to the names
     for i in range(min(len(idxlisth),len(colors))):
       # -1 because python starts at zero
       axh.scatter(0,0,marker="s",color=colors[i],label=model.heat_names[idxlisth[i]-1])
 
       # this is necessary to have the fields with increasing number without
       # gaps, otherwhise the colormapping in pcolormesh does not work
-      max_idx[model.heat_mainidx==idxlisth[i]]=i
+      max_idx[heat_mainidx==idxlisth[i]]=i
 
     cMap=mpl.colors.ListedColormap(colors[0:len(idxlisth)-1])
     axh.pcolormesh(model.x,z,max_idx,linewidth=0,cmap=cMap,rasterized=True)
     axh.legend(loc='upper center',bbox_to_anchor=(0.5,-0.175),ncol=2,
                frameon=False,fontsize=5.5)
-    axh.set_title("dominant heating processes")
 
-    # now for the cooling
+    axh.set_title(titles[0])
 
+    # now for the cooling
     if len(idxlistc)>len(colors):
       print("WARN: too many cooling processes, do not show the least important ones:")
       for i in range(len(colors),len(idxlistc)):
         print("   ",model.cool_names[idxlistc[i]-1])
 
     # this if for the labels, and also maps the colors to the names
     for i in range(min(len(idxlistc),len(colors))):
       # -1 because python starts at zeror
       axc.scatter(0,0,marker="s",color=colors[i],label=model.cool_names[idxlistc[i]-1])
 
       # this is necessary to have the fields with increasing number without
       # gaps, otherwhise the colormapping in pcolormesh does not work
-      max_idx[model.cool_mainidx==idxlistc[i]]=i
+      max_idx[cool_mainidx==idxlistc[i]]=i
 
     cMap=mpl.colors.ListedColormap(colors[0:len(idxlistc)-1])
     axc.pcolormesh(model.x,z,max_idx,linewidth=0,cmap=cMap,rasterized=True)
     axc.legend(loc='upper center',bbox_to_anchor=(0.5,-0.175),ncol=2,
                frameon=False,fontsize=5.5)
-    axc.set_title("dominant cooling processes")
+    axc.set_title(titles[1])
 
     for ax in [axh,axc]:
       # axis equal needs to be done here already ... at least it seems so
       if "axequal" in kwargs:
         if kwargs["axequal"]: ax.axis('equal')
 
       ax.set_xlim(np.min(model.x),None)
@@ -2778,23 +2826,23 @@
         newname+="_"+c
     # deal with ortho and para (o-, p-) species
     elif c=="-" and not (previous_char=="o" or previous_char=="p" or previous_char=="-"):
       newname+="^-"
     elif c=="+" and not previous_char=="+":
       newname+="^+"
     elif c=="#":
-      newname+="\#"
+      newname+=r"\#"
     else:
       newname+=c
 
     previous_char=c
 
   # for line names (species)
   if "_H" in newname:
-    newname=newname.replace("_H","\_H")
+    newname=newname.replace("_H",r"\_H")
 
   # repair the double ionized case
   if "^++" in newname: newname=newname.replace("^++","^{++}")
   # repair the triple ionized case
   if "^+++" in newname: newname=newname.replace("^+++","^{+++}")
   # repair the double ionized case
   if "^--" in newname: newname=newname.replace("^--","^{--}")
```

### Comparing `prodimopy-2.1.5/prodimopy/plot_casasim.py` & `prodimopy-2.1.6/prodimopy/plot_casasim.py`

 * *Files 0% similar despite different names*

```diff
@@ -936,15 +936,15 @@
     Copied from https://matplotlib.org/mpl_toolkits/axes_grid/api/anchored_artists_api.html
     Adapted it a bit (I think)
 
     Check how to use original class properly.
 
     """
     self._box=AuxTransformBox(transform)
-    self.ellipse=patches.Ellipse((0,0),width,height,angle,color=color)
+    self.ellipse=patches.Ellipse((0,0),width,height,angle=angle,color=color)
     self._box.add_artist(self.ellipse)
 
     AnchoredOffsetbox.__init__(self,loc,pad=pad,borderpad=borderpad,
                                child=self._box,
                                prop=prop,
                                frameon=frameon)
```

### Comparing `prodimopy-2.1.5/prodimopy/plot_mc.py` & `prodimopy-2.1.6/prodimopy/plot_mc.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/plot_models.py` & `prodimopy-2.1.6/prodimopy/plot_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import division
 from __future__ import print_function
 
 from math import pi
+import prodimopy.extinction
+import prodimopy.plot
 
 from matplotlib import lines
 from matplotlib import patches
 
 import astropy.constants as const
 import astropy.units as u
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import matplotlib.ticker as plticker
 import numpy as np
-import prodimopy.extinction
-import prodimopy.plot
 
 
 # has to be this way because of circular imports
 class PlotModels(object):
 
   def __init__(self,pdf,
                colors=None,
@@ -241,16 +241,14 @@
     if len(lineIdents)>10:
       fig,ax=plt.subplots(1,1,figsize=self._sfigs(sfigs=[2.0,1.0]))
     else:
       fig,ax=plt.subplots(1,1,figsize=self._sfigs(**kwargs))
 
     imodel=0
     lticks=list()
-    # for some reason this dummy is require
-    lticks.append("")
 
     ymin=1.e100
     ymax=1.e-100
     for model in models:
       iline=1
       x=list()
       y=list()
@@ -368,15 +366,15 @@
       # takes the x from above
       if showBoxes:
         ax.errorbar(x,ylinesObs,yerr=ylinesObsErr2,fmt=".",ms=0.0,color="lightgrey",linewidth=10)
       ax.errorbar(x,ylinesObs,yerr=ylinesObsErr,uplims=ylinesObsUl,fmt="o",ms=4.0,color="black",capsize=2,label=lineObsLabel,zorder=5)
 
     ax.set_xlim(0.5,iline-0.5)
 
-    loc=plticker.MultipleLocator(base=1.0)  # this locator puts ticks at regular intervals
+    loc=plticker.FixedLocator(np.arange(1,len(lticks)+1,1))
     ax.xaxis.set_major_locator(loc)
 
     if "ylim" in kwargs:
       ax.set_ylim(kwargs["ylim"])
     else:
       ax.set_ylim(ymin/2,ymax*2)
 
@@ -394,16 +392,16 @@
       xgrid=np.array(x)
       # ygrid=ax.get_yticks()
       # print(ygrid)
       ax.vlines(xgrid-0.5,ymin=ax.get_ylim()[0],ymax=ax.get_ylim()[1],linestyle="solid",linewidth=0.5,color="grey",zorder=-100)
       # ax.hlines(ygrid,xmin=ax.get_xlim()[0],xmax=ax.get_xlim()[1],linestyle="solid",linewidth=0.5,color="grey",zorder=100)
       ax.yaxis.grid(color="grey",zorder=-100)
 
-    ax.set_xticklabels(lticks,rotation=70,minor=False)
-    zed=[tick.label.set_fontsize(7) for tick in ax.xaxis.get_major_ticks()]
+    ax.set_xticklabels(lticks,rotation=80,minor=False,fontdict={"fontsize": 7})
+    # zed=[tick.label.set_fontsize(7) for tick in ax.xaxis.get_major_ticks()]
 
     self._legend(ax,**kwargs)
 
     if "title" in kwargs and kwargs["title"]!=None:
       ax.set_title(kwargs["title"])
 
     return self._closefig(fig)
@@ -635,15 +633,15 @@
     if xlog==True: ax.semilogx()
 
     ax.semilogy()
 
     ax.set_xlabel(r"r [au]")
     ax.set_ylabel(r"$\mathrm{\tau_{line}}$")
     if lineEstimate is not None:
-      ax.set_title(lineEstimate.ident+" "+"{:.2f}".format(lineEstimate.wl)+" $\mathrm{\mu m}$")
+      ax.set_title(lineEstimate.ident+" "+"{:.2f}".format(lineEstimate.wl)+r" $\mathrm{\mu m}$")
 
     self._legend(ax)
 
     return self._closefig(fig)
 
   def plot_avgabun(self,models,species,**kwargs):
     '''
@@ -1685,15 +1683,15 @@
     ymax=-1.e100
     for model in models:
       line=model.getLine(wl,ident=ident)
       if line==None: continue
 
       # text for the title
       if iplot==0 and linetxt is None:
-        linetxt=line.species+"@"+"{:.2f}".format(line.wl)+" $\mathrm{\mu m}$"
+        linetxt=line.species+"@"+"{:.2f}".format(line.wl)+r" $\mathrm{\mu m}$"
       x=line.profile.velo
 
       # Remove the continuum
 
       if convolved:
         y=line.profile.flux_conv
         if contsub:
```

### Comparing `prodimopy-2.1.5/prodimopy/plot_slab.py` & `prodimopy-2.1.6/prodimopy/plot_slab.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 
 
 import numpy as np
 import pandas as pd
 from scipy.constants import h,c,k
 from adjustText import adjust_text
 import matplotlib.pyplot as plt
-from prodimopy.read_slab import slab_data,slab,slab1D
+from prodimopy.read_slab import slab_data,slab,slab1D,generate_grid
 import matplotlib.colors as mcolors
 import matplotlib.cm as cm
+import spectres
 sci_c = c*1.00
 
 class default_figsize:
     def __init__(self):
         self.width = 7
         self.height = 5
 
@@ -313,15 +314,15 @@
         y = y/np.amax(y)
     ax.vlines(x, 0.0+offset, y*scaling+offset, label = label, color=color, lw=lw)
     ax.set_xlabel('Wavelength [microns]')
     ax.legend()
     return(fig,ax)
 
 
-def plot_spectra(dat, normalise = False, fig=None, ax=None, overplot=False, add=False, cmap=None, colors=None, style='step', figsize=None, NLTE=False, label='', lw=1, c=None, scaling=1, sampling=1, offset=0, overlap=False):
+def plot_spectra(dat, normalise = False, fig=None, ax=None, overplot=False, add=False, cmap=None, colors=None, style='step', figsize=None, NLTE=False, label='', lw=1, c=None, scaling=1, sampling=None, offset=0, overlap=False, custom_wave=None):
     """
     This function plots convolved spectra (erg/s/cm2/sr)
     """
 
     if isinstance(dat,slab_data):
         dat = dat.models
     elif isinstance(dat,slab):
@@ -406,15 +407,15 @@
                 for i,d in enumerate(dat):
                     add_flux+=d.convOverlapNLTE
             else:
                 for i,d in enumerate(dat):
                     add_flux+=d.convOverlapLTE
             convRR = dat[0].convOverlapR
         fig,ax = _get_set_fig(ax,fig,figsize)
-        fig,ax = _basic_spectra_plot(add_wave, add_flux,convR = convRR, sampling=sampling, scaling=scaling, normalise=normalise, fig=fig, ax=ax, style=style, figsize=figsize, label=label, color=c,lw=lw, where='mid',offset=offset)
+        fig,ax = _basic_spectra_plot(add_wave, add_flux,convR = convRR, sampling=sampling, scaling=scaling, normalise=normalise, fig=fig, ax=ax, style=style, figsize=figsize, label=label, color=c,lw=lw, where='mid',offset=offset,custom_wave=custom_wave)
         return(fig,ax)
     
     if overplot:
         fig,ax = _get_set_fig(ax,fig,figsize)
         values = range(len(dat))
         if cmap is None: cmap = 'jet'
         jet = cmm = plt.get_cmap(cmap) 
@@ -458,15 +459,15 @@
             else:
                 add_wave = sci_c/d.convOverlapFreq*1e-3
                 if NLTE:
                     add_flux=d.convOverlapNLTE
                 else:
                     add_flux=d.convOverlapLTE
                 convRR = dat[i].convOverlapR
-            fig_list[0],ax_list[0] = _basic_spectra_plot(add_wave, add_flux,convR= convRR,sampling=sampling, scaling=scaling_list[i], offset=offset_list[i],  normalise=normalise, fig=fig_list[0], ax=ax_list[0], style=style, figsize=figsize, label=label_list[i], color=color_list[i],lw=lw, where='mid')
+            fig_list[0],ax_list[0] = _basic_spectra_plot(add_wave, add_flux,convR= convRR,sampling=sampling, scaling=scaling_list[i], offset=offset_list[i],  normalise=normalise, fig=fig_list[0], ax=ax_list[0], style=style, figsize=figsize, label=label_list[i], color=color_list[i],lw=lw, where='mid',custom_wave=custom_wave)
         return(fig_list[0],ax_list[0])
     else:
         for i,d in enumerate(dat):
             if not overlap:
                 add_wave = d.convWavelength
                 if NLTE:
                     add_flux=d.convNLTEflux
@@ -476,15 +477,15 @@
             else:
                 add_wave = sci_c/d.convOverlapFreq*1e-3
                 if NLTE:
                     add_flux=d.convOverlapNLTE
                 else:
                     add_flux=d.convOverlapLTE
                 convRR = dat[i].convOverlapR
-            fig_list[i],ax_list[i] = _basic_spectra_plot(add_wave, add_flux,convR= convRR,sampling=sampling, scaling=scaling_list[i], offset=offset_list[i],  normalise=normalise, fig=fig_list[i], ax=ax_list[i], style=style, figsize=figsize, label=label_list[i], color=color_list[i],lw=lw, where='mid')
+            fig_list[i],ax_list[i] = _basic_spectra_plot(add_wave, add_flux,convR= convRR,sampling=sampling, scaling=scaling_list[i], offset=offset_list[i],  normalise=normalise, fig=fig_list[i], ax=ax_list[i], style=style, figsize=figsize, label=label_list[i], color=color_list[i],lw=lw, where='mid',custom_wave=custom_wave)
         if axx_len>1:
             return(fig_list[0],np.array(ax_list))
         else:
             return([(fig,ax) for (fig,ax) in zip(fig_list,ax_list)])
             
 def plot_1D_spectra(dat, convolved = False, R=None, normalise = False, fig=None, ax=None, style='step', figsize=None, label='', lw=1, c=None, scaling=1, sampling=1, offset=0):
     """
@@ -515,15 +516,15 @@
         Flux = dat.conv_flux
         Wavelength = dat.convWavelength
         convR = dat.convR
     else:
         raise ValueError('The model is not convolved, please set convolved=False or use .convolve() method or specify a resolving power to plot')
 
     fig,ax = _get_set_fig(ax,fig,figsize)
-    fig,ax = _basic_spectra_plot(Wavelength, Flux,convR = convR, sampling=sampling, scaling=scaling, normalise=normalise, fig=fig, ax=ax, style=style, figsize=figsize, label=label, color=c,lw=lw, where='mid',offset=offset)
+    fig,ax = _basic_spectra_plot(Wavelength, Flux,convR = convR, sampling=sampling, scaling=scaling, normalise=normalise, fig=fig, ax=ax, style=style, figsize=figsize, label=label, color=c,lw=lw, where='mid',offset=offset,custom_wave=custom_wave)
     return(fig,ax)
 
 def plot_1D_structure(dat, figsize=None,grid_point=False):
     """
     This function plots structure of 1D slab models
     """
     fig,ax = plt.subplots(1,5,figsize=figsize,sharey=True)
@@ -565,24 +566,28 @@
     ax[4].set_xscale('log')
     ax[4].set_xlabel('n [cm$^-3$]')
 
     
 
     return(fig,ax)
         
-def _basic_spectra_plot(x, y, convR,sampling=1,normalise=False, fig=None, ax=None, scaling=1, offset=0.0, figsize=None, label='', color='k', style='step', lw=1, where='post', R=1e6):
+def _basic_spectra_plot(x, y, convR,sampling=None,normalise=False, fig=None, ax=None, scaling=1, offset=0.0, figsize=None, label='', color='k', style='step', lw=1, where='post', R=1e6,custom_wave=None):
     if x is None or y is None:
         raise ValueError('x or y is None, mostly the data is not convolved. Please use .convolve() method first')
     fig,ax = _get_set_fig(ax,fig,figsize)
     if normalise:
         y = y/np.amax(y)
     y = y*scaling+offset
-    ind = int(R/convR/sampling)
-    if ind>len(y): ind = len(y)
-    if ind == 0:   ind = 1
+    if not custom_wave is None:
+        y = spectres.spectres(custom_wave,x,y, verbose=False,fill=0.0)
+        x = custom_wave*1.0
+    if not sampling is None:
+        x_new = sci_c/generate_grid(R=convR,lambda_0=np.amin(x),lambda_n=np.amax(x),sampling=sampling)*1e-3
+        y = spectres.spectres(x_new,x,y, verbose=False,fill=0.0)
+        x = x_new*1.0
     if style=='step':
-        ax.step(x[::ind], y[::ind], lw=lw, label = label, color=color, where=where)
+        ax.step(x, y, lw=lw, label = label, color=color, where=where)
     else:
-        ax.plot(x[::ind], y[::ind], lw=lw, label = label, color=color)
+        ax.plot(x, y, lw=lw, label = label, color=color)
     ax.set_xlabel('Wavelength [microns]')
     # ax.legend()
     return(fig,ax)
```

### Comparing `prodimopy-2.1.5/prodimopy/read.py` & `prodimopy-2.1.6/prodimopy/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -3232,14 +3232,15 @@
       contObs.fnuJy[i]=float(elems[1])
       contObs.fnuJyErr[i]=float(elems[2])
       contObs.flag[i]=str(elems[3])
 
     contObs.nu=(contObs.lam*u.micrometer).to(u.Hz,equivalencies=u.spectral()).value
     contObs.fnuErg=(contObs.fnuJy*u.Jy).cgs.value
     contObs.fnuErgErr=(contObs.fnuJyErr*u.Jy).cgs.value
+    f.close()
 
   # check for the spectrum files
   # types of spectra that are understood, is more of a unofficial naming convention
   types=["Spitzer","ISO","PACS","SPIRE"]
   fnames=list()
   for spectype in types:
     fnames.extend(glob.glob(directory+"/"+spectype+"*spec*.dat"))
@@ -3283,14 +3284,16 @@
     fext=open(fn_ext,"r")
     fext.readline()
     contObs.E_BV=float(fext.readline())
     fext.readline()
     contObs.R_V=float(fext.readline())
     contObs.A_V=contObs.R_V*contObs.E_BV
 
+    fn_ext.close()
+
 #   # check if there is an image.in
 #   fn_images= directory+"/image.in"
 #   if os.path.exists(fn_images):
 #     if contObs is None:
 #       contObs=DataContinuumObs()
 #
 #     fext= open(fn_images,"r")
```

### Comparing `prodimopy-2.1.5/prodimopy/read_casasim.py` & `prodimopy-2.1.6/prodimopy/read_casasim.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/read_mc.py` & `prodimopy-2.1.6/prodimopy/read_mc.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/read_slab.py` & `prodimopy-2.1.6/prodimopy/read_slab.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,5582 +14,5549 @@
 000000d0: 726e 656c 0a66 726f 6d20 6173 7472 6f70  rnel.from astrop
 000000e0: 792e 636f 6e76 6f6c 7574 696f 6e20 696d  y.convolution im
 000000f0: 706f 7274 2063 6f6e 766f 6c76 6520 6173  port convolve as
 00000100: 2061 7079 5f63 6f6e 766f 6c76 650a 6672   apy_convolve.fr
 00000110: 6f6d 2061 7374 726f 7079 2e69 6f20 696d  om astropy.io im
 00000120: 706f 7274 2066 6974 730a 6672 6f6d 2073  port fits.from s
 00000130: 6369 7079 2e63 6f6e 7374 616e 7473 2069  cipy.constants i
-00000140: 6d70 6f72 7420 682c 632c 6b0a 6672 6f6d  mport h,c,k.from
-00000150: 2073 6369 7079 2e73 7065 6369 616c 2069   scipy.special i
-00000160: 6d70 6f72 7420 6572 6620 6173 2073 6572  mport erf as ser
-00000170: 660a 6672 6f6d 2073 6369 7079 2e63 6f6e  f.from scipy.con
-00000180: 7374 616e 7473 2069 6d70 6f72 7420 6173  stants import as
-00000190: 7472 6f6e 6f6d 6963 616c 5f75 6e69 7420  tronomical_unit 
-000001a0: 6173 2061 750a 6672 6f6d 2073 6369 7079  as au.from scipy
-000001b0: 2e63 6f6e 7374 616e 7473 2069 6d70 6f72  .constants impor
-000001c0: 7420 7061 7273 6563 2061 7320 7063 0a69  t parsec as pc.i
-000001d0: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
-000001e0: 700a 696d 706f 7274 2070 616e 6461 7320  p.import pandas 
-000001f0: 6173 2070 640a 696d 706f 7274 2073 7065  as pd.import spe
-00000200: 6374 7265 730a 0a63 6c61 7373 2073 6c61  ctres..class sla
-00000210: 625f 6461 7461 3a0a 2020 2020 2222 220a  b_data:.    """.
-00000220: 2020 2020 5374 7275 6374 7572 6520 6f66      Structure of
-00000230: 2074 6865 206d 6f64 656c 7320 7365 7420   the models set 
-00000240: 7570 2066 726f 6d20 7468 6520 536c 6162  up from the Slab
-00000250: 496e 7075 742e 696e 2066 696c 653a 0a0a  Input.in file:..
-00000260: 2020 2020 5072 6f44 694d 6f20 7275 6e0a      ProDiMo run.
-00000270: 0a20 2020 207c 5f5f 4d6f 6465 6c5f 310a  .    |__Model_1.
-00000280: 2020 2020 2020 2020 7c5f 5f6d 6f6c 6563          |__molec
-00000290: 756c 655f 310a 2020 2020 2020 2020 7c5f  ule_1.        |_
-000002a0: 5f6d 6f6c 6563 756c 655f 320a 2020 2020  _molecule_2.    
-000002b0: 2020 2020 7c5f 5f2e 2e2e 0a20 2020 2020      |__....     
-000002c0: 2020 207c 5f5f 6d6f 6c65 6375 6c65 5f6e     |__molecule_n
-000002d0: 0a20 2020 207c 5f5f 4d6f 6465 6c5f 320a  .    |__Model_2.
-000002e0: 2020 2020 2020 2020 7c5f 5f6d 6f6c 6563          |__molec
-000002f0: 756c 655f 310a 2020 2020 2020 2020 7c5f  ule_1.        |_
-00000300: 5f6d 6f6c 6563 756c 655f 320a 2020 2020  _molecule_2.    
-00000310: 2020 2020 7c5f 5f2e 2e2e 0a20 2020 2020      |__....     
-00000320: 2020 207c 5f5f 6d6f 6c65 6375 6c65 5f6e     |__molecule_n
-00000330: 0a20 2020 207c 5f5f 2e2e 2e0a 2020 2020  .    |__....    
-00000340: 2020 2020 7c5f 5f2e 2e2e 0a20 2020 2020      |__....     
-00000350: 2020 207c 5f5f 2e2e 2e0a 2020 2020 2020     |__....      
-00000360: 2020 7c5f 5f2e 2e2e 0a20 2020 207c 5f5f    |__....    |__
-00000370: 4d6f 6465 6c5f 6e0a 2020 2020 2020 2020  Model_n.        
-00000380: 7c5f 5f6d 6f6c 6563 756c 655f 310a 2020  |__molecule_1.  
-00000390: 2020 2020 2020 7c5f 5f6d 6f6c 6563 756c        |__molecul
-000003a0: 655f 320a 2020 2020 2020 2020 7c5f 5f2e  e_2.        |__.
-000003b0: 2e2e 0a20 2020 2020 2020 207c 5f5f 6d6f  ...        |__mo
-000003c0: 6c65 6375 6c65 5f6e 0a0a 2020 2020 4461  lecule_n..    Da
-000003d0: 7461 2073 7472 7563 7475 7265 2074 6f20  ta structure to 
-000003e0: 686f 6c64 2074 6865 2063 6f72 7265 7370  hold the corresp
-000003f0: 6f6e 6469 6e67 2073 6c61 6220 6d6f 6465  onding slab mode
-00000400: 6c20 6f75 7470 7574 0a20 2020 2073 6c61  l output.    sla
-00000410: 625f 6461 7461 0a0a 2020 2020 7c5f 6469  b_data..    |_di
-00000420: 7265 6374 6f72 790a 0a20 2020 207c 5f6d  rectory..    |_m
-00000430: 6f64 656c 730a 2020 2020 2020 2020 7c5f  odels.        |_
-00000440: 5f6d 6f64 656c 5f31 2028 7479 7065 3a73  _model_1 (type:s
-00000450: 6c61 6229 0a20 2020 2020 2020 2020 2020  lab).           
-00000460: 7c5f 5f70 726f 6469 6d6f 5f4d 6f64 656c  |__prodimo_Model
-00000470: 5f31 5f6d 6f6c 6563 756c 655f 310a 2020  _1_molecule_1.  
-00000480: 2020 2020 2020 7c5f 5f6d 6f64 656c 5f32        |__model_2
-00000490: 2028 7479 7065 3a73 6c61 6229 0a20 2020   (type:slab).   
-000004a0: 2020 2020 2020 2020 7c5f 5f70 726f 6469          |__prodi
-000004b0: 6d6f 5f4d 6f64 656c 5f31 5f6d 6f6c 6563  mo_Model_1_molec
-000004c0: 756c 655f 320a 2020 2020 2020 2020 7c5f  ule_2.        |_
-000004d0: 5f6d 6f64 656c 5f2e 2e2e 2028 7479 7065  _model_... (type
-000004e0: 3a73 6c61 6229 0a20 2020 2020 2020 2020  :slab).         
-000004f0: 2020 7c5f 5f2e 2e2e 0a20 2020 2020 2020    |__....       
-00000500: 207c 5f5f 6d6f 6465 6c5f 6e20 2874 7970   |__model_n (typ
-00000510: 653a 736c 6162 290a 2020 2020 2020 2020  e:slab).        
-00000520: 2020 207c 5f5f 7072 6f64 696d 6f5f 4d6f     |__prodimo_Mo
-00000530: 6465 6c5f 325f 6d6f 6c65 6375 6c65 5f6e  del_2_molecule_n
-00000540: 0a20 2020 2020 2020 207c 5f5f 6d6f 6465  .        |__mode
-00000550: 6c5f 6e2b 3120 2874 7970 653a 736c 6162  l_n+1 (type:slab
-00000560: 290a 2020 2020 2020 2020 2020 207c 5f5f  ).           |__
-00000570: 7072 6f64 696d 6f5f 4d6f 6465 6c5f 325f  prodimo_Model_2_
-00000580: 6d6f 6c65 6375 6c65 5f31 0a20 2020 2020  molecule_1.     
-00000590: 2020 207c 5f5f 6d6f 6465 6c5f 6e2b 3220     |__model_n+2 
-000005a0: 2874 7970 653a 736c 6162 290a 2020 2020  (type:slab).    
-000005b0: 2020 2020 2020 207c 5f5f 7072 6f64 696d         |__prodim
-000005c0: 6f5f 4d6f 6465 6c5f 325f 6d6f 6c65 6375  o_Model_2_molecu
-000005d0: 6c65 5f32 0a20 2020 2020 2020 207c 5f5f  le_2.        |__
-000005e0: 6d6f 6465 6c5f 2e2e 2e20 2874 7970 653a  model_... (type:
-000005f0: 736c 6162 290a 2020 2020 2020 2020 2020  slab).          
-00000600: 207c 5f5f 2e2e 2e0a 2020 2020 2020 2020   |__....        
-00000610: 7c5f 5f6d 6f64 656c 5f6e 2b6e 2028 7479  |__model_n+n (ty
-00000620: 7065 3a73 6c61 6229 0a20 2020 2020 2020  pe:slab).       
-00000630: 2020 2020 7c5f 5f70 726f 6469 6d6f 5f6d      |__prodimo_m
-00000640: 6f64 656c 5f32 5f6d 6f6c 6563 756c 655f  odel_2_molecule_
-00000650: 6e0a 2020 2020 2020 2020 7c5f 5f6d 6f64  n.        |__mod
-00000660: 656c 5f2e 2e2e 2028 7479 7065 3a73 6c61  el_... (type:sla
-00000670: 6229 0a20 2020 2020 2020 2020 2020 7c5f  b).           |_
-00000680: 5f2e 2e2e 0a20 2020 2022 2222 0a0a 2020  _....    """..  
-00000690: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-000006a0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-000006b0: 6c66 2e5f 6e6d 6f64 656c 733d 300a 2020  lf._nmodels=0.  
-000006c0: 2020 2020 2020 2222 2220 696e 7465 6765        """ intege
-000006d0: 7220 3a0a 2020 2020 2020 2020 6e75 6d62  r :.        numb
-000006e0: 6572 206f 6620 6d6f 6465 6c73 2e0a 2020  er of models..  
-000006f0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00000700: 2020 2073 656c 662e 6469 7265 6374 6f72     self.director
-00000710: 793d 4e6f 6e65 0a20 2020 2020 2020 2022  y=None.        "
-00000720: 2222 2073 7472 696e 6720 3a0a 2020 2020  "" string :.    
-00000730: 2020 2020 5468 6520 6469 7265 6374 6f72      The director
-00000740: 7920 6672 6f6d 2077 6869 6368 2074 6865  y from which the
-00000750: 206d 6f64 656c 2077 6173 2072 6561 642e   model was read.
-00000760: 0a20 2020 2020 2020 2043 616e 2062 6520  .        Can be 
-00000770: 6120 7265 6c61 7469 7665 2070 6174 682e  a relative path.
-00000780: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00000790: 2020 2020 2073 656c 662e 6d6f 6465 6c73       self.models
-000007a0: 3d5b 5d0a 2020 2020 2020 2020 2222 2220  =[].        """ 
-000007b0: 6c69 7374 203a 0a20 2020 2020 2020 2054  list :.        T
-000007c0: 6865 206c 6973 7420 636f 6e74 6169 6e69  he list containi
-000007d0: 6e67 2074 6865 206d 6f64 656c 730a 2020  ng the models.  
-000007e0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-000007f0: 2020 2073 656c 662e 5f73 7065 6369 6573     self._species
-00000800: 5f6e 756d 6265 723d 4e6f 6e65 0a20 2020  _number=None.   
-00000810: 2020 2020 2022 2222 206c 6973 743a 0a20       """ list:. 
-00000820: 2020 2020 2020 2049 7420 7374 6f72 6573         It stores
-00000830: 2074 6865 2073 7065 6369 6573 206e 756d   the species num
-00000840: 6265 7220 6163 636f 7264 696e 6720 746f  ber according to
-00000850: 2053 6c61 6249 6e70 7574 2e69 6e20 6f66   SlabInput.in of
-00000860: 2061 6c6c 206d 6f64 656c 730a 2020 2020   all models.    
-00000870: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00000880: 2073 656c 662e 5f6d 6f64 656c 5f6e 756d   self._model_num
-00000890: 6265 723d 4e6f 6e65 0a20 2020 2020 2020  ber=None.       
-000008a0: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
-000008b0: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
-000008c0: 206d 6f64 656c 206e 756d 6265 7220 6163   model number ac
-000008d0: 636f 7264 696e 6720 746f 2053 6c61 6249  cording to SlabI
-000008e0: 6e70 7574 2e69 6e20 6f66 2061 6c6c 206d  nput.in of all m
-000008f0: 6f64 656c 730a 2020 2020 2020 2020 2222  odels.        ""
-00000900: 220a 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00000910: 5f4e 483d 4e6f 6e65 0a20 2020 2020 2020  _NH=None.       
-00000920: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
-00000930: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
-00000940: 2074 6f74 616c 2067 6173 2064 656e 7369   total gas densi
-00000950: 7469 6573 206f 6620 616c 6c20 6d6f 6465  ties of all mode
-00000960: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
-00000970: 2020 2020 2020 2020 7365 6c66 2e5f 6e43          self._nC
-00000980: 6f6c 6c3d 4e6f 6e65 0a20 2020 2020 2020  oll=None.       
-00000990: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
-000009a0: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
-000009b0: 2074 6f74 616c 2063 6f6c 6c69 7369 6f6e   total collision
-000009c0: 2070 6172 746e 6572 2061 6275 6e64 616e   partner abundan
-000009d0: 6365 206f 6620 616c 6c20 6d6f 6465 6c73  ce of all models
-000009e0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-000009f0: 2020 2020 2020 7365 6c66 2e5f 6e65 3d4e        self._ne=N
-00000a00: 6f6e 650a 2020 2020 2020 2020 2222 2220  one.        """ 
-00000a10: 6c69 7374 3a0a 2020 2020 2020 2020 4974  list:.        It
-00000a20: 2073 746f 7265 7320 7468 6520 656c 6563   stores the elec
-00000a30: 7472 6f6e 2061 6275 6e64 616e 6365 206f  tron abundance o
-00000a40: 6620 616c 6c20 6d6f 6465 6c73 0a20 2020  f all models.   
-00000a50: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00000a60: 2020 7365 6c66 2e5f 6e48 653d 4e6f 6e65    self._nHe=None
-00000a70: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
-00000a80: 743a 0a20 2020 2020 2020 2049 7420 7374  t:.        It st
-00000a90: 6f72 6573 2074 6865 2048 6520 6162 756e  ores the He abun
-00000aa0: 6461 6e63 6520 6f66 2061 6c6c 206d 6f64  dance of all mod
-00000ab0: 656c 730a 2020 2020 2020 2020 2222 220a  els.        """.
-00000ac0: 0a20 2020 2020 2020 2073 656c 662e 5f6e  .        self._n
-00000ad0: 4849 493d 4e6f 6e65 0a20 2020 2020 2020  HII=None.       
-00000ae0: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
-00000af0: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
-00000b00: 2048 4949 2061 6275 6e64 616e 6365 206f   HII abundance o
-00000b10: 6620 616c 6c20 6d6f 6465 6c73 0a20 2020  f all models.   
-00000b20: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00000b30: 2020 7365 6c66 2e5f 6e48 493d 4e6f 6e65    self._nHI=None
-00000b40: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
-00000b50: 743a 0a20 2020 2020 2020 2049 7420 7374  t:.        It st
-00000b60: 6f72 6573 2074 6865 2048 4920 6162 756e  ores the HI abun
-00000b70: 6461 6e63 6520 6f66 2061 6c6c 206d 6f64  dance of all mod
-00000b80: 656c 730a 2020 2020 2020 2020 2222 220a  els.        """.
-00000b90: 0a20 2020 2020 2020 2073 656c 662e 5f6e  .        self._n
-00000ba0: 4832 3d4e 6f6e 650a 2020 2020 2020 2020  H2=None.        
-00000bb0: 2222 2220 6c69 7374 3a0a 2020 2020 2020  """ list:.      
-00000bc0: 2020 4974 2073 746f 7265 7320 7468 6520    It stores the 
-00000bd0: 6d6f 6c65 6375 6c61 7220 6879 6472 6f67  molecular hydrog
-00000be0: 656e 2061 6275 6e64 616e 6365 206f 6620  en abundance of 
-00000bf0: 616c 6c20 6d6f 6465 6c73 0a20 2020 2020  all models.     
-00000c00: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00000c10: 7365 6c66 2e5f 6475 7374 5f74 6f5f 6761  self._dust_to_ga
-00000c20: 733d 4e6f 6e65 0a20 2020 2020 2020 2022  s=None.        "
-00000c30: 2222 206c 6973 743a 0a20 2020 2020 2020  "" list:.       
-00000c40: 2049 7420 7374 6f72 6573 2074 6865 2064   It stores the d
-00000c50: 7573 7420 746f 2067 6173 2072 6174 696f  ust to gas ratio
-00000c60: 206f 6620 616c 6c20 6d6f 6465 6c73 0a20   of all models. 
-00000c70: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00000c80: 2020 2020 7365 6c66 2e5f 7674 7572 623d      self._vturb=
-00000c90: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
-00000ca0: 206c 6973 743a 0a20 2020 2020 2020 2049   list:.        I
-00000cb0: 7420 7374 6f72 6573 2074 6865 2074 7572  t stores the tur
-00000cc0: 6275 6c65 6e74 2062 726f 6164 656e 696e  bulent broadenin
-00000cd0: 6720 6f66 2061 6c6c 206d 6f64 656c 730a  g of all models.
-00000ce0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00000cf0: 2020 2020 2073 656c 662e 5f54 673d 4e6f       self._Tg=No
-00000d00: 6e65 0a20 2020 2020 2020 2022 2222 206c  ne.        """ l
-00000d10: 6973 743a 0a20 2020 2020 2020 2049 7420  ist:.        It 
-00000d20: 7374 6f72 6573 2074 6865 2067 6173 2074  stores the gas t
-00000d30: 656d 7065 7261 7475 7265 7320 6f66 2061  emperatures of a
-00000d40: 6c6c 206d 6f64 656c 730a 2020 2020 2020  ll models.      
-00000d50: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
-00000d60: 656c 662e 5f54 643d 4e6f 6e65 0a20 2020  elf._Td=None.   
-00000d70: 2020 2020 2022 2222 206c 6973 743a 0a20       """ list:. 
-00000d80: 2020 2020 2020 2049 7420 7374 6f72 6573         It stores
-00000d90: 2074 6865 2064 7573 7420 7465 6d70 6572   the dust temper
-00000da0: 6174 7572 6573 206f 6620 616c 6c20 6d6f  atures of all mo
-00000db0: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
-00000dc0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00000dd0: 7370 6563 6965 735f 6e61 6d65 3d4e 6f6e  species_name=Non
-00000de0: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
-00000df0: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
-00000e00: 746f 7265 7320 7468 6520 6e61 6d65 206f  tores the name o
-00000e10: 6620 7468 6520 6d6f 6c65 6375 6c65 7320  f the molecules 
-00000e20: 6f66 2061 6c6c 206d 6f64 656c 730a 2020  of all models.  
-00000e30: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00000e40: 2020 2073 656c 662e 5f73 7065 6369 6573     self._species
-00000e50: 5f69 6e64 6578 3d4e 6f6e 650a 2020 2020  _index=None.    
-00000e60: 2020 2020 2222 2220 6c69 7374 3a0a 2020      """ list:.  
-00000e70: 2020 2020 2020 4974 2073 746f 7265 7320        It stores 
-00000e80: 7468 6520 5072 6f44 694d 6f20 7370 6563  the ProDiMo spec
-00000e90: 6965 7320 696e 6465 7820 6f66 2061 6c6c  ies index of all
-00000ea0: 206d 6f64 656c 730a 2020 2020 2020 2020   models.        
-00000eb0: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
-00000ec0: 662e 5f61 6275 6e64 616e 6365 3d4e 6f6e  f._abundance=Non
-00000ed0: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
-00000ee0: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
-00000ef0: 746f 7265 7320 7468 6520 7370 6563 6965  tores the specie
-00000f00: 7320 6162 756e 6461 6e63 6520 6163 636f  s abundance acco
-00000f10: 7264 696e 6720 746f 2053 6c61 6249 6e70  rding to SlabInp
-00000f20: 7574 2e69 6e20 6f66 2061 6c6c 206d 6f64  ut.in of all mod
-00000f30: 656c 730a 2020 2020 2020 2020 2222 220a  els.        """.
-00000f40: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
-00000f50: 763d 4e6f 6e65 0a20 2020 2020 2020 2022  v=None.        "
-00000f60: 2222 206c 6973 743a 0a20 2020 2020 2020  "" list:.       
-00000f70: 2049 7420 7374 6f72 6573 2074 6865 2076   It stores the v
-00000f80: 656c 6f63 6974 7920 7769 6474 6820 6f66  elocity width of
-00000f90: 2061 6c6c 206d 6f64 656c 730a 2020 2020   all models.    
-00000fa0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00000fb0: 2073 656c 662e 5f6e 6c65 7665 6c73 3d4e   self._nlevels=N
-00000fc0: 6f6e 650a 2020 2020 2020 2020 2222 2220  one.        """ 
-00000fd0: 6c69 7374 3a0a 2020 2020 2020 2020 4974  list:.        It
-00000fe0: 2073 746f 7265 7320 7468 6520 6e75 6d62   stores the numb
-00000ff0: 6572 206f 6620 6c65 7665 6c73 206f 6620  er of levels of 
-00001000: 616c 6c20 6d6f 6465 6c73 0a20 2020 2020  all models.     
-00001010: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00001020: 7365 6c66 2e5f 6e6c 696e 6573 3d4e 6f6e  self._nlines=Non
-00001030: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
-00001040: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
-00001050: 746f 7265 7320 7468 6520 6e75 6d62 6572  tores the number
-00001060: 206f 6620 6c69 6e65 7320 6f66 2061 6c6c   of lines of all
-00001070: 206d 6f64 656c 730a 2020 2020 2020 2020   models.        
-00001080: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-00001090: 2e5f 6c69 6e65 6461 7461 3d4e 6f6e 650a  ._linedata=None.
-000010a0: 2020 2020 2020 2020 2222 2220 6c69 7374          """ list
-000010b0: 3a0a 2020 2020 2020 2020 4974 2073 746f  :.        It sto
-000010c0: 7265 7320 7468 6520 6c69 6e65 2064 6174  res the line dat
-000010d0: 6120 6f66 2061 6c6c 206d 6f64 656c 730a  a of all models.
-000010e0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-000010f0: 2020 2020 2073 656c 662e 5f6c 6576 656c       self._level
-00001100: 6461 7461 3d4e 6f6e 650a 2020 2020 2020  data=None.      
-00001110: 2020 2222 2220 6c69 7374 3a0a 2020 2020    """ list:.    
-00001120: 2020 2020 4974 2073 746f 7265 7320 7468      It stores th
-00001130: 6520 6c65 7665 6c20 6461 7461 206f 6620  e level data of 
-00001140: 616c 6c20 6d6f 6465 6c73 0a20 2020 2020  all models.     
-00001150: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00001160: 7365 6c66 2e5f 636f 6e76 5761 7665 6c65  self._convWavele
-00001170: 6e67 7468 3d4e 6f6e 650a 2020 2020 2020  ngth=None.      
-00001180: 2020 2222 2220 6c69 7374 3a0a 2020 2020    """ list:.    
-00001190: 2020 2020 4974 2073 746f 7265 7320 7468      It stores th
-000011a0: 6520 636f 6e76 6f6c 7665 6420 7761 7665  e convolved wave
-000011b0: 6c65 6e67 7468 2067 7269 6420 6f66 2061  length grid of a
-000011c0: 6c6c 206d 6f64 656c 730a 2020 2020 2020  ll models.      
-000011d0: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
-000011e0: 656c 662e 5f63 6f6e 764c 5445 666c 7578  elf._convLTEflux
-000011f0: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
-00001200: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
-00001210: 4974 2073 746f 7265 7320 7468 6520 636f  It stores the co
-00001220: 6e76 6f6c 7665 6420 4c54 4520 666c 7578  nvolved LTE flux
-00001230: 206f 6620 616c 6c20 6d6f 6465 6c73 0a20   of all models. 
-00001240: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00001250: 2020 2020 7365 6c66 2e5f 636f 6e76 4e4c      self._convNL
-00001260: 5445 666c 7578 3d4e 6f6e 650a 2020 2020  TEflux=None.    
-00001270: 2020 2020 2222 2220 6c69 7374 3a0a 2020      """ list:.  
-00001280: 2020 2020 2020 4974 2073 746f 7265 7320        It stores 
-00001290: 7468 6520 636f 6e76 6f6c 7665 6420 4e4c  the convolved NL
-000012a0: 5445 2066 6c75 7820 6f66 2061 6c6c 206d  TE flux of all m
-000012b0: 6f64 656c 730a 2020 2020 2020 2020 2222  odels.        ""
-000012c0: 220a 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-000012d0: 5f63 6f6e 7654 7970 653d 4e6f 6e65 0a20  _convType=None. 
-000012e0: 2020 2020 2020 2022 2222 206c 6973 743a         """ list:
-000012f0: 0a20 2020 2020 2020 2049 7420 7374 6f72  .        It stor
-00001300: 6573 2074 6865 2063 6f6e 766f 6c75 7469  es the convoluti
-00001310: 6f6e 2074 7970 6520 6f66 2061 6c6c 206d  on type of all m
-00001320: 6f64 656c 730a 2020 2020 2020 2020 2222  odels.        ""
-00001330: 220a 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00001340: 5f63 6f6e 7652 3d4e 6f6e 650a 2020 2020  _convR=None.    
-00001350: 2020 2020 2222 2220 6c69 7374 3a0a 2020      """ list:.  
-00001360: 2020 2020 2020 4974 2073 746f 7265 7320        It stores 
-00001370: 7468 6520 636f 6e76 6f6c 7665 6420 7265  the convolved re
-00001380: 736f 6c76 696e 6720 706f 7765 7220 5220  solving power R 
-00001390: 6f66 2061 6c6c 206d 6f64 656c 730a 2020  of all models.  
-000013a0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-000013b0: 2020 2073 656c 662e 5f63 6f6e 764f 7665     self._convOve
-000013c0: 726c 6170 4672 6571 3d4e 6f6e 650a 2020  rlapFreq=None.  
-000013d0: 2020 2020 2020 2222 2220 6c69 7374 3a0a        """ list:.
-000013e0: 2020 2020 2020 2020 4974 2073 746f 7265          It store
-000013f0: 7320 7468 6520 636f 6e76 6f6c 7665 6420  s the convolved 
-00001400: 6672 6571 7565 6e63 7920 6772 6964 206f  frequency grid o
-00001410: 6620 616c 6c20 6c69 6e65 206f 7665 726c  f all line overl
-00001420: 6170 206d 6f64 656c 730a 2020 2020 2020  ap models.      
-00001430: 2020 2222 220a 2020 2020 2020 2020 0a20    """.        . 
-00001440: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
-00001450: 764f 7665 726c 6170 5761 763d 4e6f 6e65  vOverlapWav=None
-00001460: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
-00001470: 743a 0a20 2020 2020 2020 2049 7420 7374  t:.        It st
-00001480: 6f72 6573 2074 6865 2063 6f6e 766f 6c76  ores the convolv
-00001490: 6564 2077 6176 656c 656e 6774 6820 6772  ed wavelength gr
-000014a0: 6964 206f 6620 616c 6c20 6c69 6e65 206f  id of all line o
-000014b0: 7665 726c 6170 206d 6f64 656c 730a 2020  verlap models.  
-000014c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-000014d0: 2020 2073 656c 662e 5f63 6f6e 764f 7665     self._convOve
-000014e0: 726c 6170 4c54 4566 6c75 783d 4e6f 6e65  rlapLTEflux=None
-000014f0: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
-00001500: 743a 0a20 2020 2020 2020 2049 7420 7374  t:.        It st
-00001510: 6f72 6573 2074 6865 2063 6f6e 766f 6c76  ores the convolv
-00001520: 6564 204c 5445 2066 6c75 7820 6f66 2061  ed LTE flux of a
-00001530: 6c6c 206c 696e 6520 6f76 6572 6c61 7020  ll line overlap 
-00001540: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
-00001550: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00001560: 2e5f 636f 6e76 4f76 6572 6c61 704e 4c54  ._convOverlapNLT
-00001570: 4566 6c75 783d 4e6f 6e65 0a20 2020 2020  Eflux=None.     
-00001580: 2020 2022 2222 206c 6973 743a 0a20 2020     """ list:.   
-00001590: 2020 2020 2049 7420 7374 6f72 6573 2074       It stores t
-000015a0: 6865 2063 6f6e 766f 6c76 6564 204e 4c54  he convolved NLT
-000015b0: 4520 666c 7578 206f 6620 616c 6c20 6c69  E flux of all li
-000015c0: 6e65 206f 7665 726c 6170 206d 6f64 656c  ne overlap model
-000015d0: 730a 2020 2020 2020 2020 2222 220a 0a20  s.        """.. 
-000015e0: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
-000015f0: 726c 6170 4672 6571 3d4e 6f6e 650a 2020  rlapFreq=None.  
-00001600: 2020 2020 2020 2222 2220 6c69 7374 3a0a        """ list:.
-00001610: 2020 2020 2020 2020 4974 2073 746f 7265          It store
-00001620: 7320 7468 6520 6672 6571 7565 6e63 7920  s the frequency 
-00001630: 6772 6964 206f 6620 616c 6c20 6c69 6e65  grid of all line
-00001640: 206f 7665 726c 6170 206d 6f64 656c 730a   overlap models.
-00001650: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00001660: 2020 2020 2073 656c 662e 5f6f 7665 726c       self._overl
-00001670: 6170 4c54 453d 4e6f 6e65 0a20 2020 2020  apLTE=None.     
-00001680: 2020 2022 2222 206c 6973 743a 0a20 2020     """ list:.   
-00001690: 2020 2020 2049 7420 7374 6f72 6573 2074       It stores t
-000016a0: 6865 2063 6f6e 766f 6c76 6564 204c 5445  he convolved LTE
-000016b0: 2066 6c75 7820 6f66 2061 6c6c 206c 696e   flux of all lin
-000016c0: 6520 6f76 6572 6c61 7020 6d6f 6465 6c73  e overlap models
-000016d0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-000016e0: 2020 2020 2020 7365 6c66 2e5f 6f76 6572        self._over
-000016f0: 6c61 704e 4c54 453d 4e6f 6e65 0a20 2020  lapNLTE=None.   
-00001700: 2020 2020 2022 2222 206c 6973 743a 0a20       """ list:. 
-00001710: 2020 2020 2020 2049 7420 7374 6f72 6573         It stores
-00001720: 2074 6865 2063 6f6e 766f 6c76 6564 204e   the convolved N
-00001730: 4c54 4520 666c 7578 206f 6620 616c 6c20  LTE flux of all 
-00001740: 6c69 6e65 206f 7665 726c 6170 206d 6f64  line overlap mod
-00001750: 656c 730a 2020 2020 2020 2020 2222 220a  els.        """.
-00001760: 0a20 2020 2020 2020 2073 656c 662e 5f6f  .        self._o
-00001770: 7665 726c 6170 5461 754c 5445 3d4e 6f6e  verlapTauLTE=Non
-00001780: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
-00001790: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
-000017a0: 746f 7265 7320 7468 6520 636f 6e76 6f6c  tores the convol
-000017b0: 7665 6420 4c54 4520 6f70 7469 6361 6c20  ved LTE optical 
-000017c0: 6465 7074 6873 206f 6620 616c 6c20 6c69  depths of all li
-000017d0: 6e65 206f 7665 726c 6170 206d 6f64 656c  ne overlap model
-000017e0: 730a 2020 2020 2020 2020 2222 220a 0a20  s.        """.. 
-000017f0: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
-00001800: 726c 6170 5461 754e 4c54 453d 4e6f 6e65  rlapTauNLTE=None
-00001810: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
-00001820: 743a 0a20 2020 2020 2020 2049 7420 7374  t:.        It st
-00001830: 6f72 6573 2074 6865 2063 6f6e 766f 6c76  ores the convolv
-00001840: 6564 204e 4c54 4520 6f70 7469 6361 6c20  ed NLTE optical 
-00001850: 6465 7074 6873 206f 6620 616c 6c20 6c69  depths of all li
-00001860: 6e65 206f 7665 726c 6170 206d 6f64 656c  ne overlap model
-00001870: 730a 2020 2020 2020 2020 2222 220a 0a20  s.        """.. 
-00001880: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
-00001890: 726c 6170 523d 4e6f 6e65 0a20 2020 2020  rlapR=None.     
-000018a0: 2020 2022 2222 206c 6973 743a 0a20 2020     """ list:.   
-000018b0: 2020 2020 2049 7420 7374 6f72 6573 2074       It stores t
-000018c0: 6865 2072 6573 6f6c 7669 6e67 2070 6f77  he resolving pow
-000018d0: 6572 2052 206f 6620 616c 6c20 6c69 6e65  er R of all line
-000018e0: 206f 7665 726c 6170 206d 6f64 656c 730a   overlap models.
-000018f0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00001900: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
-00001910: 7665 726c 6170 523d 4e6f 6e65 0a20 2020  verlapR=None.   
-00001920: 2020 2020 2022 2222 206c 6973 743a 0a20       """ list:. 
-00001930: 2020 2020 2020 2049 7420 7374 6f72 6573         It stores
-00001940: 2074 6865 2063 6f6e 766f 6c76 6564 2072   the convolved r
-00001950: 6573 6f6c 7669 6e67 2070 6f77 6572 2052  esolving power R
-00001960: 206f 6620 616c 6c20 6c69 6e65 206f 7665   of all line ove
-00001970: 726c 6170 206d 6f64 656c 730a 2020 2020  rlap models.    
-00001980: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
-00001990: 205f 5f73 7472 5f5f 2873 656c 6629 3a0a   __str__(self):.
-000019a0: 2020 2020 2020 2020 6f75 7470 7574 3d22          output="
-000019b0: 496e 666f 3a20 5c6e 220a 2020 2020 2020  Info: \n".      
-000019c0: 2020 6f75 7470 7574 2b3d 225c 6e20 4e4d    output+="\n NM
-000019d0: 6f64 656c 733a 2022 0a20 2020 2020 2020  odels: ".       
-000019e0: 206f 7574 7075 742b 3d73 7472 2873 656c   output+=str(sel
-000019f0: 662e 6e6d 6f64 656c 7329 0a20 2020 2020  f.nmodels).     
-00001a00: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00001a10: 2873 656c 662e 6469 7265 6374 6f72 792c  (self.directory,
-00001a20: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
-00001a30: 2020 2066 6f72 2069 2069 6e20 7365 6c66     for i in self
-00001a40: 2e64 6972 6563 746f 7279 3a0a 2020 2020  .directory:.    
-00001a50: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00001a60: 7574 2b3d 225c 6e5c 6e20 4469 7265 6374  ut+="\n\n Direct
-00001a70: 6f72 793a 2022 2b69 0a20 2020 2020 2020  ory: "+i.       
-00001a80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00001a90: 2020 206f 7574 7075 742b 3d22 5c6e 5c6e     output+="\n\n
-00001aa0: 2044 6972 6563 746f 7279 3a20 222b 7365   Directory: "+se
-00001ab0: 6c66 2e64 6972 6563 746f 7279 0a20 2020  lf.directory.   
-00001ac0: 2020 2020 2072 6574 7572 6e20 6f75 7470       return outp
-00001ad0: 7574 0a0a 2020 2020 6465 6620 7368 6f77  ut..    def show
-00001ae0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00001af0: 7072 696e 7428 7365 6c66 290a 2020 2020  print(self).    
-00001b00: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00001b10: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-00001b20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00001b30: 6c66 2e6d 6f64 656c 735b 695d 2e73 686f  lf.models[i].sho
-00001b40: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
-00001b50: 7072 696e 7428 275c 6e27 290a 0a20 2020  print('\n')..   
-00001b60: 2064 6566 2061 6464 5f6d 6f64 656c 2873   def add_model(s
-00001b70: 656c 662c 6d6f 6465 6c5f 6461 7461 293a  elf,model_data):
-00001b80: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00001b90: 6973 696e 7374 616e 6365 286d 6f64 656c  isinstance(model
-00001ba0: 5f64 6174 612c 736c 6162 293a 0a20 2020  _data,slab):.   
-00001bb0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00001bc0: 7970 6545 7272 6f72 2827 7061 7468 206d  ypeError('path m
-00001bd0: 7573 7420 6265 206f 6620 636c 6173 733a  ust be of class:
-00001be0: 6d6f 6465 6c27 290a 2020 2020 2020 2020  model').        
-00001bf0: 7365 6c66 2e6d 6f64 656c 732e 6170 7065  self.models.appe
-00001c00: 6e64 286d 6f64 656c 5f64 6174 6129 0a0a  nd(model_data)..
-00001c10: 2020 2020 6465 6620 7265 6d6f 7665 5f6d      def remove_m
-00001c20: 6f64 656c 2873 656c 662c 696e 6465 7829  odel(self,index)
-00001c30: 3a0a 2020 2020 2020 2020 6966 2069 6e64  :.        if ind
-00001c40: 6578 3c30 3a0a 2020 2020 2020 2020 2020  ex<0:.          
-00001c50: 2020 696e 6465 782b 3d73 656c 662e 6e6d    index+=self.nm
-00001c60: 6f64 656c 730a 2020 2020 2020 2020 6966  odels.        if
-00001c70: 2069 6e64 6578 2b31 3e73 656c 662e 6e6d   index+1>self.nm
-00001c80: 6f64 656c 7320 6f72 2069 6e64 6578 3c30  odels or index<0
-00001c90: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00001ca0: 6973 6520 496e 6465 7845 7272 6f72 2827  ise IndexError('
-00001cb0: 496e 6465 7820 6f75 7420 6f66 2072 616e  Index out of ran
-00001cc0: 6765 2729 0a20 2020 2020 2020 2065 6c73  ge').        els
-00001cd0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00001ce0: 656c 662e 6e6d 6f64 656c 732d 3d31 0a20  elf.nmodels-=1. 
-00001cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001d00: 6d6f 6465 6c73 2e70 6f70 2869 6e64 6578  models.pop(index
-00001d10: 290a 0a20 2020 2064 6566 205f 5f67 6574  )..    def __get
-00001d20: 6974 656d 5f5f 2873 656c 662c 6172 6729  item__(self,arg)
-00001d30: 3a0a 2020 2020 2020 2020 7265 745f 6461  :.        ret_da
-00001d40: 7461 3d73 6c61 625f 6461 7461 2829 0a20  ta=slab_data(). 
-00001d50: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00001d60: 616e 6365 2861 7267 2c69 6e74 293a 0a20  ance(arg,int):. 
-00001d70: 2020 2020 2020 2020 2020 2069 6620 6172             if ar
-00001d80: 673e 7365 6c66 2e6e 6d6f 6465 6c73 3a0a  g>self.nmodels:.
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00001db0: 2866 2769 6e64 6578 207b 6172 677d 2067  (f'index {arg} g
-00001dc0: 7265 6174 6572 2074 6861 6e20 6e75 6d62  reater than numb
-00001dd0: 6572 206f 6620 6d6f 6465 6c73 207b 7365  er of models {se
-00001de0: 6c66 2e6e 6d6f 6465 6c73 7d27 290a 2020  lf.nmodels}').  
-00001df0: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
-00001e00: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
-00001e10: 662e 6d6f 6465 6c73 5b61 7267 5d29 0a20  f.models[arg]). 
-00001e20: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-00001e30: 7374 616e 6365 2861 7267 2c74 7970 6528  stance(arg,type(
-00001e40: 4e6f 6e65 2929 3a0a 2020 2020 2020 2020  None)):.        
-00001e50: 2020 2020 666f 7220 6d6f 6465 6c20 696e      for model in
-00001e60: 2073 656c 662e 6d6f 6465 6c73 3a0a 2020   self.models:.  
-00001e70: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00001e80: 745f 6461 7461 2e61 6464 5f6d 6f64 656c  t_data.add_model
-00001e90: 286d 6f64 656c 290a 2020 2020 2020 2020  (model).        
-00001ea0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-00001eb0: 6172 672c 736c 6963 6529 3a0a 2020 2020  arg,slice):.    
-00001ec0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00001ed0: 7461 6e63 6528 6172 672e 7374 6172 742c  tance(arg.start,
-00001ee0: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00001ef0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00001f00: 6e63 6528 6172 672e 7374 6f70 2c69 6e74  nce(arg.stop,int
-00001f10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00001f20: 2020 2020 2020 2066 6f72 206d 6f64 656c         for model
-00001f30: 2069 6e20 7365 6c66 2e6d 6f64 656c 735b   in self.models[
-00001f40: 6172 675d 3a0a 2020 2020 2020 2020 2020  arg]:.          
-00001f50: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00001f60: 745f 6461 7461 2e61 6464 5f6d 6f64 656c  t_data.add_model
-00001f70: 286d 6f64 656c 290a 2020 2020 2020 2020  (model).        
-00001f80: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-00001f90: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
-00001fa0: 2c74 7970 6528 4e6f 6e65 2929 3a0a 2020  ,type(None)):.  
-00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fc0: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
-00001fd0: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
-00001fe0: 5b61 7267 2e73 7461 7274 5d29 0a20 2020  [arg.start]).   
-00001ff0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00002000: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00002010: 2020 2020 2020 2072 6169 7365 2049 6e64         raise Ind
-00002020: 6578 4572 726f 7228 6627 736c 6963 696e  exError(f'slicin
-00002030: 6720 6e6f 7420 756e 6465 7273 7461 6e64  g not understand
-00002040: 6162 6c65 207b 6172 677d 2729 0a20 2020  able {arg}').   
-00002050: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
-00002060: 696e 7374 616e 6365 2861 7267 2e73 7461  instance(arg.sta
-00002070: 7274 2c73 7472 293a 0a20 2020 2020 2020  rt,str):.       
-00002080: 2020 2020 2020 2020 2069 6620 6172 672e           if arg.
-00002090: 7374 6172 743d 3d27 7370 6563 6965 735f  start=='species_
-000020a0: 6e61 6d65 273a 0a20 2020 2020 2020 2020  name':.         
-000020b0: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
-000020c0: 7065 6369 6573 3d5b 5d0a 2020 2020 2020  pecies=[].      
-000020d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000020e0: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-000020f0: 7374 6f70 2c73 7472 293a 0a20 2020 2020  stop,str):.     
+00000140: 6d70 6f72 7420 6173 7472 6f6e 6f6d 6963  mport astronomic
+00000150: 616c 5f75 6e69 7420 6173 2061 750a 6672  al_unit as au.fr
+00000160: 6f6d 2073 6369 7079 2e63 6f6e 7374 616e  om scipy.constan
+00000170: 7473 2069 6d70 6f72 7420 682c 632c 6b0a  ts import h,c,k.
+00000180: 6672 6f6d 2073 6369 7079 2e63 6f6e 7374  from scipy.const
+00000190: 616e 7473 2069 6d70 6f72 7420 7061 7273  ants import pars
+000001a0: 6563 2061 7320 7063 0a66 726f 6d20 7363  ec as pc.from sc
+000001b0: 6970 792e 7370 6563 6961 6c20 696d 706f  ipy.special impo
+000001c0: 7274 2065 7266 2061 7320 7365 7266 0a69  rt erf as serf.i
+000001d0: 6d70 6f72 7420 7370 6563 7472 6573 0a0a  mport spectres..
+000001e0: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
+000001f0: 6e70 0a69 6d70 6f72 7420 7061 6e64 6173  np.import pandas
+00000200: 2061 7320 7064 0a0a 0a63 6c61 7373 2073   as pd...class s
+00000210: 6c61 625f 6461 7461 3a0a 2020 2020 2222  lab_data:.    ""
+00000220: 220a 2020 2020 5374 7275 6374 7572 6520  ".    Structure 
+00000230: 6f66 2074 6865 206d 6f64 656c 7320 7365  of the models se
+00000240: 7420 7570 2066 726f 6d20 7468 6520 536c  t up from the Sl
+00000250: 6162 496e 7075 742e 696e 2066 696c 653a  abInput.in file:
+00000260: 0a0a 2020 2020 5072 6f44 694d 6f20 7275  ..    ProDiMo ru
+00000270: 6e0a 0a20 2020 207c 5f5f 4d6f 6465 6c5f  n..    |__Model_
+00000280: 310a 2020 2020 2020 2020 7c5f 5f6d 6f6c  1.        |__mol
+00000290: 6563 756c 655f 310a 0a20 2020 2020 2020  ecule_1..       
+000002a0: 207c 5f5f 6d6f 6c65 6375 6c65 5f32 0a0a   |__molecule_2..
+000002b0: 2020 2020 2020 2020 7c5f 5f2e 2e2e 0a0a          |__.....
+000002c0: 2020 2020 2020 2020 7c5f 5f6d 6f6c 6563          |__molec
+000002d0: 756c 655f 6e0a 2020 2020 7c5f 5f4d 6f64  ule_n.    |__Mod
+000002e0: 656c 5f32 0a20 2020 2020 2020 207c 5f5f  el_2.        |__
+000002f0: 6d6f 6c65 6375 6c65 5f31 0a0a 2020 2020  molecule_1..    
+00000300: 2020 2020 7c5f 5f6d 6f6c 6563 756c 655f      |__molecule_
+00000310: 320a 0a20 2020 2020 2020 207c 5f5f 2e2e  2..        |__..
+00000320: 2e0a 0a20 2020 2020 2020 207c 5f5f 6d6f  ...        |__mo
+00000330: 6c65 6375 6c65 5f6e 0a20 2020 207c 5f5f  lecule_n.    |__
+00000340: 2e2e 2e0a 2020 2020 2020 2020 7c5f 5f2e  ....        |__.
+00000350: 2e2e 0a0a 2020 2020 2020 2020 7c5f 5f2e  ....        |__.
+00000360: 2e2e 0a0a 2020 2020 2020 2020 7c5f 5f2e  ....        |__.
+00000370: 2e2e 0a20 2020 207c 5f5f 4d6f 6465 6c5f  ...    |__Model_
+00000380: 6e0a 2020 2020 2020 2020 7c5f 5f6d 6f6c  n.        |__mol
+00000390: 6563 756c 655f 310a 0a20 2020 2020 2020  ecule_1..       
+000003a0: 207c 5f5f 6d6f 6c65 6375 6c65 5f32 0a0a   |__molecule_2..
+000003b0: 2020 2020 2020 2020 7c5f 5f2e 2e2e 0a0a          |__.....
+000003c0: 2020 2020 2020 2020 7c5f 5f6d 6f6c 6563          |__molec
+000003d0: 756c 655f 6e0a 0a20 2020 2044 6174 6120  ule_n..    Data 
+000003e0: 7374 7275 6374 7572 6520 746f 2068 6f6c  structure to hol
+000003f0: 6420 7468 6520 636f 7272 6573 706f 6e64  d the correspond
+00000400: 696e 6720 736c 6162 206d 6f64 656c 206f  ing slab model o
+00000410: 7574 7075 740a 2020 2020 736c 6162 5f64  utput.    slab_d
+00000420: 6174 610a 0a20 2020 207c 5f64 6972 6563  ata..    |_direc
+00000430: 746f 7279 0a0a 2020 2020 7c5f 6d6f 6465  tory..    |_mode
+00000440: 6c73 0a20 2020 2020 2020 207c 5f5f 6d6f  ls.        |__mo
+00000450: 6465 6c5f 3120 2874 7970 653a 736c 6162  del_1 (type:slab
+00000460: 290a 2020 2020 2020 2020 2020 207c 5f5f  ).           |__
+00000470: 7072 6f64 696d 6f5f 4d6f 6465 6c5f 315f  prodimo_Model_1_
+00000480: 6d6f 6c65 6375 6c65 5f31 0a20 2020 2020  molecule_1.     
+00000490: 2020 207c 5f5f 6d6f 6465 6c5f 3220 2874     |__model_2 (t
+000004a0: 7970 653a 736c 6162 290a 2020 2020 2020  ype:slab).      
+000004b0: 2020 2020 207c 5f5f 7072 6f64 696d 6f5f       |__prodimo_
+000004c0: 4d6f 6465 6c5f 315f 6d6f 6c65 6375 6c65  Model_1_molecule
+000004d0: 5f32 0a20 2020 2020 2020 207c 5f5f 6d6f  _2.        |__mo
+000004e0: 6465 6c5f 2e2e 2e20 2874 7970 653a 736c  del_... (type:sl
+000004f0: 6162 290a 2020 2020 2020 2020 2020 207c  ab).           |
+00000500: 5f5f 2e2e 2e0a 2020 2020 2020 2020 7c5f  __....        |_
+00000510: 5f6d 6f64 656c 5f6e 2028 7479 7065 3a73  _model_n (type:s
+00000520: 6c61 6229 0a20 2020 2020 2020 2020 2020  lab).           
+00000530: 7c5f 5f70 726f 6469 6d6f 5f4d 6f64 656c  |__prodimo_Model
+00000540: 5f32 5f6d 6f6c 6563 756c 655f 6e0a 2020  _2_molecule_n.  
+00000550: 2020 2020 2020 7c5f 5f6d 6f64 656c 5f6e        |__model_n
+00000560: 2b31 2028 7479 7065 3a73 6c61 6229 0a20  +1 (type:slab). 
+00000570: 2020 2020 2020 2020 2020 7c5f 5f70 726f            |__pro
+00000580: 6469 6d6f 5f4d 6f64 656c 5f32 5f6d 6f6c  dimo_Model_2_mol
+00000590: 6563 756c 655f 310a 2020 2020 2020 2020  ecule_1.        
+000005a0: 7c5f 5f6d 6f64 656c 5f6e 2b32 2028 7479  |__model_n+2 (ty
+000005b0: 7065 3a73 6c61 6229 0a20 2020 2020 2020  pe:slab).       
+000005c0: 2020 2020 7c5f 5f70 726f 6469 6d6f 5f4d      |__prodimo_M
+000005d0: 6f64 656c 5f32 5f6d 6f6c 6563 756c 655f  odel_2_molecule_
+000005e0: 320a 2020 2020 2020 2020 7c5f 5f6d 6f64  2.        |__mod
+000005f0: 656c 5f2e 2e2e 2028 7479 7065 3a73 6c61  el_... (type:sla
+00000600: 6229 0a20 2020 2020 2020 2020 2020 7c5f  b).           |_
+00000610: 5f2e 2e2e 0a20 2020 2020 2020 207c 5f5f  _....        |__
+00000620: 6d6f 6465 6c5f 6e2b 6e20 2874 7970 653a  model_n+n (type:
+00000630: 736c 6162 290a 2020 2020 2020 2020 2020  slab).          
+00000640: 207c 5f5f 7072 6f64 696d 6f5f 6d6f 6465   |__prodimo_mode
+00000650: 6c5f 325f 6d6f 6c65 6375 6c65 5f6e 0a20  l_2_molecule_n. 
+00000660: 2020 2020 2020 207c 5f5f 6d6f 6465 6c5f         |__model_
+00000670: 2e2e 2e20 2874 7970 653a 736c 6162 290a  ... (type:slab).
+00000680: 2020 2020 2020 2020 2020 207c 5f5f 2e2e             |__..
+00000690: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+000006a0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+000006b0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000006c0: 5f6e 6d6f 6465 6c73 3d30 0a20 2020 2020  _nmodels=0.     
+000006d0: 2020 2022 2222 2069 6e74 6567 6572 203a     """ integer :
+000006e0: 0a20 2020 2020 2020 206e 756d 6265 7220  .        number 
+000006f0: 6f66 206d 6f64 656c 732e 0a20 2020 2020  of models..     
+00000700: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00000710: 7365 6c66 2e64 6972 6563 746f 7279 3d4e  self.directory=N
+00000720: 6f6e 650a 2020 2020 2020 2020 2222 2220  one.        """ 
+00000730: 7374 7269 6e67 203a 0a20 2020 2020 2020  string :.       
+00000740: 2054 6865 2064 6972 6563 746f 7279 2066   The directory f
+00000750: 726f 6d20 7768 6963 6820 7468 6520 6d6f  rom which the mo
+00000760: 6465 6c20 7761 7320 7265 6164 2e0a 2020  del was read..  
+00000770: 2020 2020 2020 4361 6e20 6265 2061 2072        Can be a r
+00000780: 656c 6174 6976 6520 7061 7468 2e0a 2020  elative path..  
+00000790: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000007a0: 2020 7365 6c66 2e6d 6f64 656c 733d 5b5d    self.models=[]
+000007b0: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
+000007c0: 7420 3a0a 2020 2020 2020 2020 5468 6520  t :.        The 
+000007d0: 6c69 7374 2063 6f6e 7461 696e 696e 6720  list containing 
+000007e0: 7468 6520 6d6f 6465 6c73 0a20 2020 2020  the models.     
+000007f0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00000800: 7365 6c66 2e5f 7370 6563 6965 735f 6e75  self._species_nu
+00000810: 6d62 6572 3d4e 6f6e 650a 2020 2020 2020  mber=None.      
+00000820: 2020 2222 2220 6c69 7374 3a0a 2020 2020    """ list:.    
+00000830: 2020 2020 4974 2073 746f 7265 7320 7468      It stores th
+00000840: 6520 7370 6563 6965 7320 6e75 6d62 6572  e species number
+00000850: 2061 6363 6f72 6469 6e67 2074 6f20 536c   according to Sl
+00000860: 6162 496e 7075 742e 696e 206f 6620 616c  abInput.in of al
+00000870: 6c20 6d6f 6465 6c73 0a20 2020 2020 2020  l models.       
+00000880: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
+00000890: 6c66 2e5f 6d6f 6465 6c5f 6e75 6d62 6572  lf._model_number
+000008a0: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
+000008b0: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
+000008c0: 4974 2073 746f 7265 7320 7468 6520 6d6f  It stores the mo
+000008d0: 6465 6c20 6e75 6d62 6572 2061 6363 6f72  del number accor
+000008e0: 6469 6e67 2074 6f20 536c 6162 496e 7075  ding to SlabInpu
+000008f0: 742e 696e 206f 6620 616c 6c20 6d6f 6465  t.in of all mode
+00000900: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
+00000910: 2020 2020 2020 2020 7365 6c66 2e5f 4e48          self._NH
+00000920: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
+00000930: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
+00000940: 4974 2073 746f 7265 7320 7468 6520 746f  It stores the to
+00000950: 7461 6c20 6761 7320 6465 6e73 6974 6965  tal gas densitie
+00000960: 7320 6f66 2061 6c6c 206d 6f64 656c 730a  s of all models.
+00000970: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00000980: 2020 2020 2073 656c 662e 5f6e 436f 6c6c       self._nColl
+00000990: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
+000009a0: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
+000009b0: 4974 2073 746f 7265 7320 7468 6520 746f  It stores the to
+000009c0: 7461 6c20 636f 6c6c 6973 696f 6e20 7061  tal collision pa
+000009d0: 7274 6e65 7220 6162 756e 6461 6e63 6520  rtner abundance 
+000009e0: 6f66 2061 6c6c 206d 6f64 656c 730a 2020  of all models.  
+000009f0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00000a00: 2020 2073 656c 662e 5f6e 653d 4e6f 6e65     self._ne=None
+00000a10: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
+00000a20: 743a 0a20 2020 2020 2020 2049 7420 7374  t:.        It st
+00000a30: 6f72 6573 2074 6865 2065 6c65 6374 726f  ores the electro
+00000a40: 6e20 6162 756e 6461 6e63 6520 6f66 2061  n abundance of a
+00000a50: 6c6c 206d 6f64 656c 730a 2020 2020 2020  ll models.      
+00000a60: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
+00000a70: 656c 662e 5f6e 4865 3d4e 6f6e 650a 2020  elf._nHe=None.  
+00000a80: 2020 2020 2020 2222 2220 6c69 7374 3a0a        """ list:.
+00000a90: 2020 2020 2020 2020 4974 2073 746f 7265          It store
+00000aa0: 7320 7468 6520 4865 2061 6275 6e64 616e  s the He abundan
+00000ab0: 6365 206f 6620 616c 6c20 6d6f 6465 6c73  ce of all models
+00000ac0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00000ad0: 2020 2020 2020 7365 6c66 2e5f 6e48 4949        self._nHII
+00000ae0: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
+00000af0: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
+00000b00: 4974 2073 746f 7265 7320 7468 6520 4849  It stores the HI
+00000b10: 4920 6162 756e 6461 6e63 6520 6f66 2061  I abundance of a
+00000b20: 6c6c 206d 6f64 656c 730a 2020 2020 2020  ll models.      
+00000b30: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
+00000b40: 656c 662e 5f6e 4849 3d4e 6f6e 650a 2020  elf._nHI=None.  
+00000b50: 2020 2020 2020 2222 2220 6c69 7374 3a0a        """ list:.
+00000b60: 2020 2020 2020 2020 4974 2073 746f 7265          It store
+00000b70: 7320 7468 6520 4849 2061 6275 6e64 616e  s the HI abundan
+00000b80: 6365 206f 6620 616c 6c20 6d6f 6465 6c73  ce of all models
+00000b90: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00000ba0: 2020 2020 2020 7365 6c66 2e5f 6e48 323d        self._nH2=
+00000bb0: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
+00000bc0: 206c 6973 743a 0a20 2020 2020 2020 2049   list:.        I
+00000bd0: 7420 7374 6f72 6573 2074 6865 206d 6f6c  t stores the mol
+00000be0: 6563 756c 6172 2068 7964 726f 6765 6e20  ecular hydrogen 
+00000bf0: 6162 756e 6461 6e63 6520 6f66 2061 6c6c  abundance of all
+00000c00: 206d 6f64 656c 730a 2020 2020 2020 2020   models.        
+00000c10: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
+00000c20: 662e 5f64 7573 745f 746f 5f67 6173 3d4e  f._dust_to_gas=N
+00000c30: 6f6e 650a 2020 2020 2020 2020 2222 2220  one.        """ 
+00000c40: 6c69 7374 3a0a 2020 2020 2020 2020 4974  list:.        It
+00000c50: 2073 746f 7265 7320 7468 6520 6475 7374   stores the dust
+00000c60: 2074 6f20 6761 7320 7261 7469 6f20 6f66   to gas ratio of
+00000c70: 2061 6c6c 206d 6f64 656c 730a 2020 2020   all models.    
+00000c80: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00000c90: 2073 656c 662e 5f76 7475 7262 3d4e 6f6e   self._vturb=Non
+00000ca0: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
+00000cb0: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
+00000cc0: 746f 7265 7320 7468 6520 7475 7262 756c  tores the turbul
+00000cd0: 656e 7420 6272 6f61 6465 6e69 6e67 206f  ent broadening o
+00000ce0: 6620 616c 6c20 6d6f 6465 6c73 0a20 2020  f all models.   
+00000cf0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00000d00: 2020 7365 6c66 2e5f 5467 3d4e 6f6e 650a    self._Tg=None.
+00000d10: 2020 2020 2020 2020 2222 2220 6c69 7374          """ list
+00000d20: 3a0a 2020 2020 2020 2020 4974 2073 746f  :.        It sto
+00000d30: 7265 7320 7468 6520 6761 7320 7465 6d70  res the gas temp
+00000d40: 6572 6174 7572 6573 206f 6620 616c 6c20  eratures of all 
+00000d50: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
+00000d60: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00000d70: 2e5f 5464 3d4e 6f6e 650a 2020 2020 2020  ._Td=None.      
+00000d80: 2020 2222 2220 6c69 7374 3a0a 2020 2020    """ list:.    
+00000d90: 2020 2020 4974 2073 746f 7265 7320 7468      It stores th
+00000da0: 6520 6475 7374 2074 656d 7065 7261 7475  e dust temperatu
+00000db0: 7265 7320 6f66 2061 6c6c 206d 6f64 656c  res of all model
+00000dc0: 730a 2020 2020 2020 2020 2222 220a 0a20  s.        """.. 
+00000dd0: 2020 2020 2020 2073 656c 662e 5f73 7065         self._spe
+00000de0: 6369 6573 5f6e 616d 653d 4e6f 6e65 0a20  cies_name=None. 
+00000df0: 2020 2020 2020 2022 2222 206c 6973 743a         """ list:
+00000e00: 0a20 2020 2020 2020 2049 7420 7374 6f72  .        It stor
+00000e10: 6573 2074 6865 206e 616d 6520 6f66 2074  es the name of t
+00000e20: 6865 206d 6f6c 6563 756c 6573 206f 6620  he molecules of 
+00000e30: 616c 6c20 6d6f 6465 6c73 0a20 2020 2020  all models.     
+00000e40: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00000e50: 7365 6c66 2e5f 7370 6563 6965 735f 696e  self._species_in
+00000e60: 6465 783d 4e6f 6e65 0a20 2020 2020 2020  dex=None.       
+00000e70: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
+00000e80: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
+00000e90: 2050 726f 4469 4d6f 2073 7065 6369 6573   ProDiMo species
+00000ea0: 2069 6e64 6578 206f 6620 616c 6c20 6d6f   index of all mo
+00000eb0: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
+00000ec0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00000ed0: 6162 756e 6461 6e63 653d 4e6f 6e65 0a20  abundance=None. 
+00000ee0: 2020 2020 2020 2022 2222 206c 6973 743a         """ list:
+00000ef0: 0a20 2020 2020 2020 2049 7420 7374 6f72  .        It stor
+00000f00: 6573 2074 6865 2073 7065 6369 6573 2061  es the species a
+00000f10: 6275 6e64 616e 6365 2061 6363 6f72 6469  bundance accordi
+00000f20: 6e67 2074 6f20 536c 6162 496e 7075 742e  ng to SlabInput.
+00000f30: 696e 206f 6620 616c 6c20 6d6f 6465 6c73  in of all models
+00000f40: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00000f50: 2020 2020 2020 7365 6c66 2e5f 6476 3d4e        self._dv=N
+00000f60: 6f6e 650a 2020 2020 2020 2020 2222 2220  one.        """ 
+00000f70: 6c69 7374 3a0a 2020 2020 2020 2020 4974  list:.        It
+00000f80: 2073 746f 7265 7320 7468 6520 7665 6c6f   stores the velo
+00000f90: 6369 7479 2077 6964 7468 206f 6620 616c  city width of al
+00000fa0: 6c20 6d6f 6465 6c73 0a20 2020 2020 2020  l models.       
+00000fb0: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
+00000fc0: 6c66 2e5f 6e6c 6576 656c 733d 4e6f 6e65  lf._nlevels=None
+00000fd0: 0a20 2020 2020 2020 2022 2222 206c 6973  .        """ lis
+00000fe0: 743a 0a20 2020 2020 2020 2049 7420 7374  t:.        It st
+00000ff0: 6f72 6573 2074 6865 206e 756d 6265 7220  ores the number 
+00001000: 6f66 206c 6576 656c 7320 6f66 2061 6c6c  of levels of all
+00001010: 206d 6f64 656c 730a 2020 2020 2020 2020   models.        
+00001020: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
+00001030: 662e 5f6e 6c69 6e65 733d 4e6f 6e65 0a20  f._nlines=None. 
+00001040: 2020 2020 2020 2022 2222 206c 6973 743a         """ list:
+00001050: 0a20 2020 2020 2020 2049 7420 7374 6f72  .        It stor
+00001060: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
+00001070: 206c 696e 6573 206f 6620 616c 6c20 6d6f   lines of all mo
+00001080: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
+00001090: 0a20 2020 2020 2020 2073 656c 662e 5f6c  .        self._l
+000010a0: 696e 6564 6174 613d 4e6f 6e65 0a20 2020  inedata=None.   
+000010b0: 2020 2020 2022 2222 206c 6973 743a 0a20       """ list:. 
+000010c0: 2020 2020 2020 2049 7420 7374 6f72 6573         It stores
+000010d0: 2074 6865 206c 696e 6520 6461 7461 206f   the line data o
+000010e0: 6620 616c 6c20 6d6f 6465 6c73 0a20 2020  f all models.   
+000010f0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00001100: 2020 7365 6c66 2e5f 6c65 7665 6c64 6174    self._leveldat
+00001110: 613d 4e6f 6e65 0a20 2020 2020 2020 2022  a=None.        "
+00001120: 2222 206c 6973 743a 0a20 2020 2020 2020  "" list:.       
+00001130: 2049 7420 7374 6f72 6573 2074 6865 206c   It stores the l
+00001140: 6576 656c 2064 6174 6120 6f66 2061 6c6c  evel data of all
+00001150: 206d 6f64 656c 730a 2020 2020 2020 2020   models.        
+00001160: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
+00001170: 662e 5f63 6f6e 7657 6176 656c 656e 6774  f._convWavelengt
+00001180: 683d 4e6f 6e65 0a20 2020 2020 2020 2022  h=None.        "
+00001190: 2222 206c 6973 743a 0a20 2020 2020 2020  "" list:.       
+000011a0: 2049 7420 7374 6f72 6573 2074 6865 2063   It stores the c
+000011b0: 6f6e 766f 6c76 6564 2077 6176 656c 656e  onvolved wavelen
+000011c0: 6774 6820 6772 6964 206f 6620 616c 6c20  gth grid of all 
+000011d0: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
+000011e0: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+000011f0: 2e5f 636f 6e76 4c54 4566 6c75 783d 4e6f  ._convLTEflux=No
+00001200: 6e65 0a20 2020 2020 2020 2022 2222 206c  ne.        """ l
+00001210: 6973 743a 0a20 2020 2020 2020 2049 7420  ist:.        It 
+00001220: 7374 6f72 6573 2074 6865 2063 6f6e 766f  stores the convo
+00001230: 6c76 6564 204c 5445 2066 6c75 7820 6f66  lved LTE flux of
+00001240: 2061 6c6c 206d 6f64 656c 730a 2020 2020   all models.    
+00001250: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00001260: 2073 656c 662e 5f63 6f6e 764e 4c54 4566   self._convNLTEf
+00001270: 6c75 783d 4e6f 6e65 0a20 2020 2020 2020  lux=None.       
+00001280: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
+00001290: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
+000012a0: 2063 6f6e 766f 6c76 6564 204e 4c54 4520   convolved NLTE 
+000012b0: 666c 7578 206f 6620 616c 6c20 6d6f 6465  flux of all mode
+000012c0: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
+000012d0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+000012e0: 6e76 5479 7065 3d4e 6f6e 650a 2020 2020  nvType=None.    
+000012f0: 2020 2020 2222 2220 6c69 7374 3a0a 2020      """ list:.  
+00001300: 2020 2020 2020 4974 2073 746f 7265 7320        It stores 
+00001310: 7468 6520 636f 6e76 6f6c 7574 696f 6e20  the convolution 
+00001320: 7479 7065 206f 6620 616c 6c20 6d6f 6465  type of all mode
+00001330: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
+00001340: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+00001350: 6e76 523d 4e6f 6e65 0a20 2020 2020 2020  nvR=None.       
+00001360: 2022 2222 206c 6973 743a 0a20 2020 2020   """ list:.     
+00001370: 2020 2049 7420 7374 6f72 6573 2074 6865     It stores the
+00001380: 2063 6f6e 766f 6c76 6564 2072 6573 6f6c   convolved resol
+00001390: 7669 6e67 2070 6f77 6572 2052 206f 6620  ving power R of 
+000013a0: 616c 6c20 6d6f 6465 6c73 0a20 2020 2020  all models.     
+000013b0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+000013c0: 7365 6c66 2e5f 636f 6e76 4f76 6572 6c61  self._convOverla
+000013d0: 7046 7265 713d 4e6f 6e65 0a20 2020 2020  pFreq=None.     
+000013e0: 2020 2022 2222 206c 6973 743a 0a20 2020     """ list:.   
+000013f0: 2020 2020 2049 7420 7374 6f72 6573 2074       It stores t
+00001400: 6865 2063 6f6e 766f 6c76 6564 2066 7265  he convolved fre
+00001410: 7175 656e 6379 2067 7269 6420 6f66 2061  quency grid of a
+00001420: 6c6c 206c 696e 6520 6f76 6572 6c61 7020  ll line overlap 
+00001430: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
+00001440: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00001450: 2e5f 636f 6e76 4f76 6572 6c61 7057 6176  ._convOverlapWav
+00001460: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
+00001470: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
+00001480: 4974 2073 746f 7265 7320 7468 6520 636f  It stores the co
+00001490: 6e76 6f6c 7665 6420 7761 7665 6c65 6e67  nvolved waveleng
+000014a0: 7468 2067 7269 6420 6f66 2061 6c6c 206c  th grid of all l
+000014b0: 696e 6520 6f76 6572 6c61 7020 6d6f 6465  ine overlap mode
+000014c0: 6c73 0a20 2020 2020 2020 2022 2222 0a0a  ls.        """..
+000014d0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+000014e0: 6e76 4f76 6572 6c61 704c 5445 666c 7578  nvOverlapLTEflux
+000014f0: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
+00001500: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
+00001510: 4974 2073 746f 7265 7320 7468 6520 636f  It stores the co
+00001520: 6e76 6f6c 7665 6420 4c54 4520 666c 7578  nvolved LTE flux
+00001530: 206f 6620 616c 6c20 6c69 6e65 206f 7665   of all line ove
+00001540: 726c 6170 206d 6f64 656c 730a 2020 2020  rlap models.    
+00001550: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00001560: 2073 656c 662e 5f63 6f6e 764f 7665 726c   self._convOverl
+00001570: 6170 4e4c 5445 666c 7578 3d4e 6f6e 650a  apNLTEflux=None.
+00001580: 2020 2020 2020 2020 2222 2220 6c69 7374          """ list
+00001590: 3a0a 2020 2020 2020 2020 4974 2073 746f  :.        It sto
+000015a0: 7265 7320 7468 6520 636f 6e76 6f6c 7665  res the convolve
+000015b0: 6420 4e4c 5445 2066 6c75 7820 6f66 2061  d NLTE flux of a
+000015c0: 6c6c 206c 696e 6520 6f76 6572 6c61 7020  ll line overlap 
+000015d0: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
+000015e0: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+000015f0: 2e5f 6f76 6572 6c61 7046 7265 713d 4e6f  ._overlapFreq=No
+00001600: 6e65 0a20 2020 2020 2020 2022 2222 206c  ne.        """ l
+00001610: 6973 743a 0a20 2020 2020 2020 2049 7420  ist:.        It 
+00001620: 7374 6f72 6573 2074 6865 2066 7265 7175  stores the frequ
+00001630: 656e 6379 2067 7269 6420 6f66 2061 6c6c  ency grid of all
+00001640: 206c 696e 6520 6f76 6572 6c61 7020 6d6f   line overlap mo
+00001650: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
+00001660: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00001670: 6f76 6572 6c61 704c 5445 3d4e 6f6e 650a  overlapLTE=None.
+00001680: 2020 2020 2020 2020 2222 2220 6c69 7374          """ list
+00001690: 3a0a 2020 2020 2020 2020 4974 2073 746f  :.        It sto
+000016a0: 7265 7320 7468 6520 636f 6e76 6f6c 7665  res the convolve
+000016b0: 6420 4c54 4520 666c 7578 206f 6620 616c  d LTE flux of al
+000016c0: 6c20 6c69 6e65 206f 7665 726c 6170 206d  l line overlap m
+000016d0: 6f64 656c 730a 2020 2020 2020 2020 2222  odels.        ""
+000016e0: 220a 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+000016f0: 5f6f 7665 726c 6170 4e4c 5445 3d4e 6f6e  _overlapNLTE=Non
+00001700: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
+00001710: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
+00001720: 746f 7265 7320 7468 6520 636f 6e76 6f6c  tores the convol
+00001730: 7665 6420 4e4c 5445 2066 6c75 7820 6f66  ved NLTE flux of
+00001740: 2061 6c6c 206c 696e 6520 6f76 6572 6c61   all line overla
+00001750: 7020 6d6f 6465 6c73 0a20 2020 2020 2020  p models.       
+00001760: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
+00001770: 6c66 2e5f 6f76 6572 6c61 7054 6175 4c54  lf._overlapTauLT
+00001780: 453d 4e6f 6e65 0a20 2020 2020 2020 2022  E=None.        "
+00001790: 2222 206c 6973 743a 0a20 2020 2020 2020  "" list:.       
+000017a0: 2049 7420 7374 6f72 6573 2074 6865 2063   It stores the c
+000017b0: 6f6e 766f 6c76 6564 204c 5445 206f 7074  onvolved LTE opt
+000017c0: 6963 616c 2064 6570 7468 7320 6f66 2061  ical depths of a
+000017d0: 6c6c 206c 696e 6520 6f76 6572 6c61 7020  ll line overlap 
+000017e0: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
+000017f0: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00001800: 2e5f 6f76 6572 6c61 7054 6175 4e4c 5445  ._overlapTauNLTE
+00001810: 3d4e 6f6e 650a 2020 2020 2020 2020 2222  =None.        ""
+00001820: 2220 6c69 7374 3a0a 2020 2020 2020 2020  " list:.        
+00001830: 4974 2073 746f 7265 7320 7468 6520 636f  It stores the co
+00001840: 6e76 6f6c 7665 6420 4e4c 5445 206f 7074  nvolved NLTE opt
+00001850: 6963 616c 2064 6570 7468 7320 6f66 2061  ical depths of a
+00001860: 6c6c 206c 696e 6520 6f76 6572 6c61 7020  ll line overlap 
+00001870: 6d6f 6465 6c73 0a20 2020 2020 2020 2022  models.        "
+00001880: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00001890: 2e5f 6f76 6572 6c61 7052 3d4e 6f6e 650a  ._overlapR=None.
+000018a0: 2020 2020 2020 2020 2222 2220 6c69 7374          """ list
+000018b0: 3a0a 2020 2020 2020 2020 4974 2073 746f  :.        It sto
+000018c0: 7265 7320 7468 6520 7265 736f 6c76 696e  res the resolvin
+000018d0: 6720 706f 7765 7220 5220 6f66 2061 6c6c  g power R of all
+000018e0: 206c 696e 6520 6f76 6572 6c61 7020 6d6f   line overlap mo
+000018f0: 6465 6c73 0a20 2020 2020 2020 2022 2222  dels.        """
+00001900: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00001910: 636f 6e76 4f76 6572 6c61 7052 3d4e 6f6e  convOverlapR=Non
+00001920: 650a 2020 2020 2020 2020 2222 2220 6c69  e.        """ li
+00001930: 7374 3a0a 2020 2020 2020 2020 4974 2073  st:.        It s
+00001940: 746f 7265 7320 7468 6520 636f 6e76 6f6c  tores the convol
+00001950: 7665 6420 7265 736f 6c76 696e 6720 706f  ved resolving po
+00001960: 7765 7220 5220 6f66 2061 6c6c 206c 696e  wer R of all lin
+00001970: 6520 6f76 6572 6c61 7020 6d6f 6465 6c73  e overlap models
+00001980: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00001990: 2020 6465 6620 5f5f 7374 725f 5f28 7365    def __str__(se
+000019a0: 6c66 293a 0a20 2020 2020 2020 206f 7574  lf):.        out
+000019b0: 7075 743d 2249 6e66 6f3a 205c 6e22 0a20  put="Info: \n". 
+000019c0: 2020 2020 2020 206f 7574 7075 742b 3d22         output+="
+000019d0: 5c6e 204e 4d6f 6465 6c73 3a20 220a 2020  \n NModels: ".  
+000019e0: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
+000019f0: 7228 7365 6c66 2e6e 6d6f 6465 6c73 290a  r(self.nmodels).
+00001a00: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00001a10: 7461 6e63 6528 7365 6c66 2e64 6972 6563  tance(self.direc
+00001a20: 746f 7279 2c6c 6973 7429 3a0a 2020 2020  tory,list):.    
+00001a30: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00001a40: 2073 656c 662e 6469 7265 6374 6f72 793a   self.directory:
+00001a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001a60: 206f 7574 7075 742b 3d22 5c6e 5c6e 2044   output+="\n\n D
+00001a70: 6972 6563 746f 7279 3a20 222b 690a 2020  irectory: "+i.  
+00001a80: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00001a90: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+00001aa0: 225c 6e5c 6e20 4469 7265 6374 6f72 793a  "\n\n Directory:
+00001ab0: 2022 2b73 656c 662e 6469 7265 6374 6f72   "+self.director
+00001ac0: 790a 2020 2020 2020 2020 7265 7475 726e  y.        return
+00001ad0: 206f 7574 7075 740a 0a20 2020 2064 6566   output..    def
+00001ae0: 2073 686f 7728 7365 6c66 293a 0a20 2020   show(self):.   
+00001af0: 2020 2020 2070 7269 6e74 2873 656c 6629       print(self)
+00001b00: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+00001b10: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+00001b20: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00001b30: 2020 2073 656c 662e 6d6f 6465 6c73 5b69     self.models[i
+00001b40: 5d2e 7368 6f77 2829 0a20 2020 2020 2020  ].show().       
+00001b50: 2020 2020 2070 7269 6e74 2827 5c6e 2729       print('\n')
+00001b60: 0a0a 2020 2020 6465 6620 6164 645f 6d6f  ..    def add_mo
+00001b70: 6465 6c28 7365 6c66 2c6d 6f64 656c 5f64  del(self,model_d
+00001b80: 6174 6129 3a0a 2020 2020 2020 2020 6966  ata):.        if
+00001b90: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+00001ba0: 6d6f 6465 6c5f 6461 7461 2c73 6c61 6229  model_data,slab)
+00001bb0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00001bc0: 6973 6520 5479 7065 4572 726f 7228 2770  ise TypeError('p
+00001bd0: 6174 6820 6d75 7374 2062 6520 6f66 2063  ath must be of c
+00001be0: 6c61 7373 3a6d 6f64 656c 2729 0a20 2020  lass:model').   
+00001bf0: 2020 2020 2073 656c 662e 6d6f 6465 6c73       self.models
+00001c00: 2e61 7070 656e 6428 6d6f 6465 6c5f 6461  .append(model_da
+00001c10: 7461 290a 0a20 2020 2064 6566 2072 656d  ta)..    def rem
+00001c20: 6f76 655f 6d6f 6465 6c28 7365 6c66 2c69  ove_model(self,i
+00001c30: 6e64 6578 293a 0a20 2020 2020 2020 2069  ndex):.        i
+00001c40: 6620 696e 6465 783c 303a 0a20 2020 2020  f index<0:.     
+00001c50: 2020 2020 2020 2069 6e64 6578 2b3d 7365         index+=se
+00001c60: 6c66 2e6e 6d6f 6465 6c73 0a20 2020 2020  lf.nmodels.     
+00001c70: 2020 2069 6620 696e 6465 782b 313e 7365     if index+1>se
+00001c80: 6c66 2e6e 6d6f 6465 6c73 206f 7220 696e  lf.nmodels or in
+00001c90: 6465 783c 303a 0a20 2020 2020 2020 2020  dex<0:.         
+00001ca0: 2020 2072 6169 7365 2049 6e64 6578 4572     raise IndexEr
+00001cb0: 726f 7228 2749 6e64 6578 206f 7574 206f  ror('Index out o
+00001cc0: 6620 7261 6e67 6527 290a 2020 2020 2020  f range').      
+00001cd0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00001ce0: 2020 2020 7365 6c66 2e6e 6d6f 6465 6c73      self.nmodels
+00001cf0: 2d3d 310a 2020 2020 2020 2020 2020 2020  -=1.            
+00001d00: 7365 6c66 2e6d 6f64 656c 732e 706f 7028  self.models.pop(
+00001d10: 696e 6465 7829 0a0a 2020 2020 6465 6620  index)..    def 
+00001d20: 5f5f 6765 7469 7465 6d5f 5f28 7365 6c66  __getitem__(self
+00001d30: 2c61 7267 293a 0a20 2020 2020 2020 2072  ,arg):.        r
+00001d40: 6574 5f64 6174 613d 736c 6162 5f64 6174  et_data=slab_dat
+00001d50: 6128 290a 2020 2020 2020 2020 6966 2069  a().        if i
+00001d60: 7369 6e73 7461 6e63 6528 6172 672c 696e  sinstance(arg,in
+00001d70: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00001d80: 6966 2061 7267 3e73 656c 662e 6e6d 6f64  if arg>self.nmod
+00001d90: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+00001da0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00001db0: 4572 726f 7228 6627 696e 6465 7820 7b61  Error(f'index {a
+00001dc0: 7267 7d20 6772 6561 7465 7220 7468 616e  rg} greater than
+00001dd0: 206e 756d 6265 7220 6f66 206d 6f64 656c   number of model
+00001de0: 7320 7b73 656c 662e 6e6d 6f64 656c 737d  s {self.nmodels}
+00001df0: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
+00001e00: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
+00001e10: 6c28 7365 6c66 2e6d 6f64 656c 735b 6172  l(self.models[ar
+00001e20: 675d 290a 2020 2020 2020 2020 656c 6966  g]).        elif
+00001e30: 2069 7369 6e73 7461 6e63 6528 6172 672c   isinstance(arg,
+00001e40: 7479 7065 284e 6f6e 6529 293a 0a20 2020  type(None)):.   
+00001e50: 2020 2020 2020 2020 2066 6f72 206d 6f64           for mod
+00001e60: 656c 2069 6e20 7365 6c66 2e6d 6f64 656c  el in self.model
+00001e70: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00001e80: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
+00001e90: 6d6f 6465 6c28 6d6f 6465 6c29 0a20 2020  model(model).   
+00001ea0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00001eb0: 616e 6365 2861 7267 2c73 6c69 6365 293a  ance(arg,slice):
+00001ec0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00001ed0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00001ee0: 7461 7274 2c69 6e74 293a 0a20 2020 2020  tart,int):.     
+00001ef0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00001f00: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
+00001f10: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
+00001f20: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00001f30: 6d6f 6465 6c20 696e 2073 656c 662e 6d6f  model in self.mo
+00001f40: 6465 6c73 5b61 7267 5d3a 0a20 2020 2020  dels[arg]:.     
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f60: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
+00001f70: 6d6f 6465 6c28 6d6f 6465 6c29 0a20 2020  model(model).   
+00001f80: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00001f90: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
+00001fa0: 2e73 746f 702c 7479 7065 284e 6f6e 6529  .stop,type(None)
+00001fb0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00001fc0: 2020 2020 2020 2072 6574 5f64 6174 612e         ret_data.
+00001fd0: 6164 645f 6d6f 6465 6c28 7365 6c66 2e6d  add_model(self.m
+00001fe0: 6f64 656c 735b 6172 672e 7374 6172 745d  odels[arg.start]
+00001ff0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00002000: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00002010: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00002020: 6520 496e 6465 7845 7272 6f72 2866 2773  e IndexError(f's
+00002030: 6c69 6369 6e67 206e 6f74 2075 6e64 6572  licing not under
+00002040: 7374 616e 6461 626c 6520 7b61 7267 7d27  standable {arg}'
+00002050: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00002060: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
+00002070: 672e 7374 6172 742c 7374 7229 3a0a 2020  g.start,str):.  
+00002080: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002090: 2061 7267 2e73 7461 7274 3d3d 2773 7065   arg.start=='spe
+000020a0: 6369 6573 5f6e 616d 6527 3a0a 2020 2020  cies_name':.    
+000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020c0: 7365 6c5f 7370 6563 6965 733d 5b5d 0a20  sel_species=[]. 
+000020d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020e0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+000020f0: 2861 7267 2e73 746f 702c 7374 7229 3a0a  (arg.stop,str):.
 00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002110: 2020 2073 656c 5f73 7065 6369 6573 2e61     sel_species.a
-00002120: 7070 656e 6428 6172 672e 7374 6f70 290a  ppend(arg.stop).
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00002150: 6e63 6528 6172 672e 7374 6f70 2c6c 6973  nce(arg.stop,lis
-00002160: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00002170: 2020 2020 2020 2020 2020 2020 7365 6c5f              sel_
-00002180: 7370 6563 6965 733d 6172 672e 7374 6f70  species=arg.stop
-00002190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021a0: 2020 2020 2069 6620 6c65 6e28 7365 6c5f       if len(sel_
-000021b0: 7370 6563 6965 7329 3e30 3a0a 2020 2020  species)>0:.    
-000021c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021d0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-000021e0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-000021f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002200: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002210: 2073 656c 662e 6d6f 6465 6c73 5b69 5d2e   self.models[i].
-00002220: 7370 6563 6965 735f 6e61 6d65 2069 6e20  species_name in 
-00002230: 7365 6c5f 7370 6563 6965 733a 0a20 2020  sel_species:.   
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00002260: 5f64 6174 612e 6164 645f 6d6f 6465 6c28  _data.add_model(
-00002270: 7365 6c66 2e6d 6f64 656c 735b 695d 290a  self.models[i]).
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 656c 6966 2061 7267 2e73 7461 7274 3d3d  elif arg.start==
-000022a0: 2773 7065 6369 6573 5f6e 756d 6265 7227  'species_number'
-000022b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000022c0: 2020 2020 2020 7365 6c5f 7370 6563 6965        sel_specie
-000022d0: 735f 6e75 6d62 6572 3d5b 5d0a 2020 2020  s_number=[].    
-000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022f0: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
-00002300: 672e 7374 6f70 2c69 6e74 293a 0a20 2020  g.stop,int):.   
-00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00002330: 6365 2861 7267 2e73 7465 702c 696e 7429  ce(arg.step,int)
-00002340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002350: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00002360: 7220 6920 696e 2072 616e 6765 2861 7267  r i in range(arg
-00002370: 2e73 746f 702c 6172 672e 7374 6570 293a  .stop,arg.step):
-00002380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002110: 2020 2020 2020 2020 7365 6c5f 7370 6563          sel_spec
+00002120: 6965 732e 6170 7065 6e64 2861 7267 2e73  ies.append(arg.s
+00002130: 746f 7029 0a20 2020 2020 2020 2020 2020  top).           
+00002140: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
+00002150: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
+00002160: 702c 6c69 7374 293a 0a20 2020 2020 2020  p,list):.       
+00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002180: 2073 656c 5f73 7065 6369 6573 3d61 7267   sel_species=arg
+00002190: 2e73 746f 700a 2020 2020 2020 2020 2020  .stop.          
+000021a0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+000021b0: 2873 656c 5f73 7065 6369 6573 293e 303a  (sel_species)>0:
+000021c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000021d0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+000021e0: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+000021f0: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002210: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
+00002220: 735b 695d 2e73 7065 6369 6573 5f6e 616d  s[i].species_nam
+00002230: 6520 696e 2073 656c 5f73 7065 6369 6573  e in sel_species
+00002240: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002260: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
+00002270: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
+00002280: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+00002290: 2020 2020 2065 6c69 6620 6172 672e 7374       elif arg.st
+000022a0: 6172 743d 3d27 7370 6563 6965 735f 6e75  art=='species_nu
+000022b0: 6d62 6572 273a 0a20 2020 2020 2020 2020  mber':.         
+000022c0: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
+000022d0: 7065 6369 6573 5f6e 756d 6265 723d 5b5d  pecies_number=[]
+000022e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000022f0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00002300: 6365 2861 7267 2e73 746f 702c 696e 7429  ce(arg.stop,int)
+00002310: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002320: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00002330: 6e73 7461 6e63 6528 6172 672e 7374 6570  nstance(arg.step
+00002340: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
+00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002360: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00002370: 6528 6172 672e 7374 6f70 2c61 7267 2e73  e(arg.stop,arg.s
+00002380: 7465 7029 3a0a 2020 2020 2020 2020 2020  tep):.          
 00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023a0: 2073 656c 5f73 7065 6369 6573 5f6e 756d   sel_species_num
-000023b0: 6265 722e 6170 7065 6e64 2869 290a 2020  ber.append(i).  
-000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023f0: 2020 2020 2020 2020 7365 6c5f 7370 6563          sel_spec
-00002400: 6965 735f 6e75 6d62 6572 2e61 7070 656e  ies_number.appen
-00002410: 6428 6172 672e 7374 6f70 290a 2020 2020  d(arg.stop).    
-00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002430: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-00002440: 6172 672e 7374 6f70 2c6c 6973 7429 3a0a  arg.stop,list):.
-00002450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002460: 2020 2020 2020 2020 2020 2020 7365 6c5f              sel_
-00002470: 7370 6563 6965 735f 6e75 6d62 6572 3d61  species_number=a
-00002480: 7267 2e73 746f 700a 2020 2020 2020 2020  rg.stop.        
-00002490: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-000024a0: 656e 2873 656c 5f73 7065 6369 6573 5f6e  en(sel_species_n
-000024b0: 756d 6265 7229 3e30 3a0a 2020 2020 2020  umber)>0:.      
+000023a0: 2020 2020 2020 7365 6c5f 7370 6563 6965        sel_specie
+000023b0: 735f 6e75 6d62 6572 2e61 7070 656e 6428  s_number.append(
+000023c0: 6929 0a20 2020 2020 2020 2020 2020 2020  i).             
+000023d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000023e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000023f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00002400: 5f73 7065 6369 6573 5f6e 756d 6265 722e  _species_number.
+00002410: 6170 7065 6e64 2861 7267 2e73 746f 7029  append(arg.stop)
+00002420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002430: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00002440: 616e 6365 2861 7267 2e73 746f 702c 6c69  ance(arg.stop,li
+00002450: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002470: 2073 656c 5f73 7065 6369 6573 5f6e 756d   sel_species_num
+00002480: 6265 723d 6172 672e 7374 6f70 0a20 2020  ber=arg.stop.   
+00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024a0: 2069 6620 6c65 6e28 7365 6c5f 7370 6563   if len(sel_spec
+000024b0: 6965 735f 6e75 6d62 6572 293e 303a 0a20  ies_number)>0:. 
 000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024d0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-000024e0: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
-000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002500: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00002510: 656c 662e 6d6f 6465 6c73 5b69 5d2e 7370  elf.models[i].sp
-00002520: 6563 6965 735f 6e75 6d62 6572 2069 6e20  ecies_number in 
-00002530: 7365 6c5f 7370 6563 6965 735f 6e75 6d62  sel_species_numb
-00002540: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+000024d0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000024e0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+000024f0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002510: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
+00002520: 695d 2e73 7065 6369 6573 5f6e 756d 6265  i].species_numbe
+00002530: 7220 696e 2073 656c 5f73 7065 6369 6573  r in sel_species
+00002540: 5f6e 756d 6265 723a 0a20 2020 2020 2020  _number:.       
 00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002560: 2020 2020 7265 745f 6461 7461 2e61 6464      ret_data.add
-00002570: 5f6d 6f64 656c 2873 656c 662e 6d6f 6465  _model(self.mode
-00002580: 6c73 5b69 5d29 0a20 2020 2020 2020 2020  ls[i]).         
-00002590: 2020 2020 2020 2065 6c69 6620 6172 672e         elif arg.
-000025a0: 7374 6172 743d 3d27 6d6f 6465 6c5f 6e75  start=='model_nu
-000025b0: 6d62 6572 273a 0a20 2020 2020 2020 2020  mber':.         
-000025c0: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
-000025d0: 7065 6369 6573 5f6e 756d 6265 723d 5b5d  pecies_number=[]
-000025e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000025f0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00002600: 6365 2861 7267 2e73 746f 702c 696e 7429  ce(arg.stop,int)
-00002610: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002620: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00002630: 6e73 7461 6e63 6528 6172 672e 7374 6570  nstance(arg.step
-00002640: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
+00002560: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
+00002570: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
+00002580: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
+00002590: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000025a0: 2061 7267 2e73 7461 7274 3d3d 276d 6f64   arg.start=='mod
+000025b0: 656c 5f6e 756d 6265 7227 3a0a 2020 2020  el_number':.    
+000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025d0: 7365 6c5f 7370 6563 6965 735f 6e75 6d62  sel_species_numb
+000025e0: 6572 3d5b 5d0a 2020 2020 2020 2020 2020  er=[].          
+000025f0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00002600: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
+00002610: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
+00002620: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002630: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
+00002640: 2e73 7465 702c 696e 7429 3a0a 2020 2020  .step,int):.    
 00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00002670: 6528 6172 672e 7374 6f70 2c61 7267 2e73  e(arg.stop,arg.s
-00002680: 7465 7029 3a0a 2020 2020 2020 2020 2020  tep):.          
+00002660: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00002670: 2072 616e 6765 2861 7267 2e73 746f 702c   range(arg.stop,
+00002680: 6172 672e 7374 6570 293a 0a20 2020 2020  arg.step):.     
 00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026a0: 2020 2020 2020 7365 6c5f 7370 6563 6965        sel_specie
-000026b0: 735f 6e75 6d62 6572 2e61 7070 656e 6428  s_number.append(
-000026c0: 6929 0a20 2020 2020 2020 2020 2020 2020  i).             
-000026d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000026e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000026f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002700: 5f73 7065 6369 6573 5f6e 756d 6265 722e  _species_number.
-00002710: 6170 7065 6e64 2861 7267 2e73 746f 7029  append(arg.stop)
-00002720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002730: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-00002740: 616e 6365 2861 7267 2e73 746f 702c 6c69  ance(arg.stop,li
-00002750: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+000026a0: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
+000026b0: 7065 6369 6573 5f6e 756d 6265 722e 6170  pecies_number.ap
+000026c0: 7065 6e64 2869 290a 2020 2020 2020 2020  pend(i).        
+000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002700: 2020 7365 6c5f 7370 6563 6965 735f 6e75    sel_species_nu
+00002710: 6d62 6572 2e61 7070 656e 6428 6172 672e  mber.append(arg.
+00002720: 7374 6f70 290a 2020 2020 2020 2020 2020  stop).          
+00002730: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
+00002740: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+00002750: 6f70 2c6c 6973 7429 3a0a 2020 2020 2020  op,list):.      
 00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002770: 2073 656c 5f73 7065 6369 6573 5f6e 756d   sel_species_num
-00002780: 6265 723d 6172 672e 7374 6f70 0a20 2020  ber=arg.stop.   
-00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027a0: 2069 6620 6c65 6e28 7365 6c5f 7370 6563   if len(sel_spec
-000027b0: 6965 735f 6e75 6d62 6572 293e 303a 0a20  ies_number)>0:. 
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027d0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000027e0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
-000027f0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00002770: 2020 2020 2020 7365 6c5f 7370 6563 6965        sel_specie
+00002780: 735f 6e75 6d62 6572 3d61 7267 2e73 746f  s_number=arg.sto
+00002790: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+000027a0: 2020 2020 2020 6966 206c 656e 2873 656c        if len(sel
+000027b0: 5f73 7065 6369 6573 5f6e 756d 6265 7229  _species_number)
+000027c0: 3e30 3a0a 2020 2020 2020 2020 2020 2020  >0:.            
+000027d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000027e0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+000027f0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
 00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
-00002820: 695d 2e6d 6f64 656c 5f6e 756d 6265 7220  i].model_number 
-00002830: 696e 2073 656c 5f73 7065 6369 6573 5f6e  in sel_species_n
-00002840: 756d 6265 723a 0a20 2020 2020 2020 2020  umber:.         
+00002810: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
+00002820: 6465 6c73 5b69 5d2e 6d6f 6465 6c5f 6e75  dels[i].model_nu
+00002830: 6d62 6572 2069 6e20 7365 6c5f 7370 6563  mber in sel_spec
+00002840: 6965 735f 6e75 6d62 6572 3a0a 2020 2020  ies_number:.    
 00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002860: 2020 2020 2020 2072 6574 5f64 6174 612e         ret_data.
-00002870: 6164 645f 6d6f 6465 6c28 7365 6c66 2e6d  add_model(self.m
-00002880: 6f64 656c 735b 695d 290a 2020 2020 2020  odels[i]).      
-00002890: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
-000028a0: 7267 2e73 7461 7274 3d3d 274e 4827 3a0a  rg.start=='NH':.
-000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028c0: 2020 2020 7570 7065 723d 6e70 2e6e 616e      upper=np.nan
-000028d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028e0: 2020 2020 206c 6f77 6572 3d6e 702e 6e61       lower=np.na
-000028f0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00002900: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00002910: 6e63 6528 6172 672e 7374 6f70 2c66 6c6f  nce(arg.stop,flo
-00002920: 6174 2920 6f72 2069 7369 6e73 7461 6e63  at) or isinstanc
-00002930: 6528 6172 672e 7374 6f70 2c69 6e74 293a  e(arg.stop,int):
-00002940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002950: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-00002960: 7374 616e 6365 2861 7267 2e73 7465 702c  stance(arg.step,
-00002970: 666c 6f61 7429 206f 7220 6973 696e 7374  float) or isinst
-00002980: 616e 6365 2861 7267 2e73 7465 702c 696e  ance(arg.step,in
-00002990: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00002860: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
+00002870: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
+00002880: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
+00002890: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000028a0: 6c69 6620 6172 672e 7374 6172 743d 3d27  lif arg.start=='
+000028b0: 4e48 273a 0a20 2020 2020 2020 2020 2020  NH':.           
+000028c0: 2020 2020 2020 2020 2075 7070 6572 3d6e           upper=n
+000028d0: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
+000028e0: 2020 2020 2020 2020 2020 6c6f 7765 723d            lower=
+000028f0: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
+00002900: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00002910: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
+00002920: 702c 666c 6f61 7429 206f 7220 6973 696e  p,float) or isin
+00002930: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
+00002940: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+00002950: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002960: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00002970: 7374 6570 2c66 6c6f 6174 2920 6f72 2069  step,float) or i
+00002980: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+00002990: 6570 2c69 6e74 293a 0a20 2020 2020 2020  ep,int):.       
 000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029b0: 6c6f 7765 722c 7570 7065 723d 6172 672e  lower,upper=arg.
-000029c0: 7374 6f70 2c61 7267 2e73 7465 700a 2020  stop,arg.step.  
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a00: 2020 2020 2020 2020 7570 7065 723d 6172          upper=ar
-00002a10: 672e 7374 6f70 0a20 2020 2020 2020 2020  g.stop.         
-00002a20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00002a30: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-00002a40: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-00002a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a60: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00002a70: 6e70 2e69 736e 616e 286c 6f77 6572 293a  np.isnan(lower):
-00002a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000029b0: 2020 2020 206c 6f77 6572 2c75 7070 6572       lower,upper
+000029c0: 3d61 7267 2e73 746f 702c 6172 672e 7374  =arg.stop,arg.st
+000029d0: 6570 0a20 2020 2020 2020 2020 2020 2020  ep.             
+000029e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000029f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a00: 2020 2020 2020 2020 2020 2020 2075 7070               upp
+00002a10: 6572 3d61 7267 2e73 746f 700a 2020 2020  er=arg.stop.    
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a30: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00002a40: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+00002a50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002a60: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002a70: 206e 6f74 206e 702e 6973 6e61 6e28 6c6f   not np.isnan(lo
+00002a80: 7765 7229 3a0a 2020 2020 2020 2020 2020  wer):.          
 00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002aa0: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
-00002ab0: 695d 2e4e 483c 7570 7065 7220 616e 6420  i].NH<upper and 
-00002ac0: 7365 6c66 2e6d 6f64 656c 735b 695d 2e4e  self.models[i].N
-00002ad0: 483e 6c6f 7765 723a 0a20 2020 2020 2020  H>lower:.       
+00002aa0: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
+00002ab0: 6465 6c73 5b69 5d2e 4e48 3c75 7070 6572  dels[i].NH<upper
+00002ac0: 2061 6e64 2073 656c 662e 6d6f 6465 6c73   and self.models
+00002ad0: 5b69 5d2e 4e48 3e6c 6f77 6572 3a0a 2020  [i].NH>lower:.  
 00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002af0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00002b00: 5f64 6174 612e 6164 645f 6d6f 6465 6c28  _data.add_model(
-00002b10: 7365 6c66 2e6d 6f64 656c 735b 695d 290a  self.models[i]).
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00002b40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b00: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
+00002b10: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
+00002b20: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
 00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b60: 2020 6966 2073 656c 662e 6d6f 6465 6c73    if self.models
-00002b70: 5b69 5d2e 4e48 3d3d 7570 7065 723a 0a20  [i].NH==upper:. 
-00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b60: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00002b70: 6f64 656c 735b 695d 2e4e 483d 3d75 7070  odels[i].NH==upp
+00002b80: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
 00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ba0: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
-00002bb0: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
-00002bc0: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
-00002bd0: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
-00002be0: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
-00002bf0: 6f70 2c6c 6973 7429 3a0a 2020 2020 2020  op,list):.      
+00002ba0: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
+00002bb0: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
+00002bc0: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
+00002bd0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00002be0: 6c69 6620 6973 696e 7374 616e 6365 2861  lif isinstance(a
+00002bf0: 7267 2e73 746f 702c 6c69 7374 293a 0a20  rg.stop,list):. 
 00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00002c20: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
-00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c40: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00002c50: 656c 662e 6d6f 6465 6c73 5b69 5d2e 4e48  elf.models[i].NH
-00002c60: 2069 6e20 6172 672e 7374 6f70 3a0a 2020   in arg.stop:.  
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00002c90: 745f 6461 7461 2e61 6464 5f6d 6f64 656c  t_data.add_model
-00002ca0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d29  (self.models[i])
-00002cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002cc0: 2065 6c69 6620 6172 672e 7374 6172 743d   elif arg.start=
-00002cd0: 3d27 6e43 6f6c 6c27 3a0a 2020 2020 2020  ='nColl':.      
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 7570                up
-00002cf0: 7065 723d 6e70 2e6e 616e 0a20 2020 2020  per=np.nan.     
-00002d00: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00002d10: 6f77 6572 3d6e 702e 6e61 6e0a 2020 2020  ower=np.nan.    
-00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d30: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
-00002d40: 672e 7374 6f70 2c66 6c6f 6174 2920 6f72  g.stop,float) or
-00002d50: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-00002d60: 7374 6f70 2c69 6e74 293a 0a20 2020 2020  stop,int):.     
+00002c10: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00002c20: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00002c30: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c50: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
+00002c60: 695d 2e4e 4820 696e 2061 7267 2e73 746f  i].NH in arg.sto
+00002c70: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
+00002ca0: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
+00002cb0: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
+00002cc0: 2020 2020 2020 656c 6966 2061 7267 2e73        elif arg.s
+00002cd0: 7461 7274 3d3d 276e 436f 6c6c 273a 0a20  tart=='nColl':. 
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2020 2075 7070 6572 3d6e 702e 6e61 6e0a     upper=np.nan.
+00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d10: 2020 2020 6c6f 7765 723d 6e70 2e6e 616e      lower=np.nan
+00002d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d30: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00002d40: 6365 2861 7267 2e73 746f 702c 666c 6f61  ce(arg.stop,floa
+00002d50: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
+00002d60: 2861 7267 2e73 746f 702c 696e 7429 3a0a  (arg.stop,int):.
 00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d80: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00002d90: 2861 7267 2e73 7465 702c 666c 6f61 7429  (arg.step,float)
-00002da0: 206f 7220 6973 696e 7374 616e 6365 2861   or isinstance(a
-00002db0: 7267 2e73 7465 702c 696e 7429 3a0a 2020  rg.step,int):.  
-00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dd0: 2020 2020 2020 2020 2020 6c6f 7765 722c            lower,
-00002de0: 7570 7065 723d 6172 672e 7374 6f70 2c61  upper=arg.stop,a
-00002df0: 7267 2e73 7465 700a 2020 2020 2020 2020  rg.step.        
+00002d80: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00002d90: 7461 6e63 6528 6172 672e 7374 6570 2c66  tance(arg.step,f
+00002da0: 6c6f 6174 2920 6f72 2069 7369 6e73 7461  loat) or isinsta
+00002db0: 6e63 6528 6172 672e 7374 6570 2c69 6e74  nce(arg.step,int
+00002dc0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00002dd0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00002de0: 6f77 6572 2c75 7070 6572 3d61 7267 2e73  ower,upper=arg.s
+00002df0: 746f 702c 6172 672e 7374 6570 0a20 2020  top,arg.step.   
 00002e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00002e10: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
 00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e30: 2020 7570 7065 723d 6172 672e 7374 6f70    upper=arg.stop
-00002e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002e50: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00002e60: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-00002e70: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00002e30: 2020 2020 2020 2075 7070 6572 3d61 7267         upper=arg
+00002e40: 2e73 746f 700a 2020 2020 2020 2020 2020  .stop.          
+00002e50: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00002e60: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+00002e70: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
 00002e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e90: 2020 2069 6620 6e6f 7420 6e70 2e69 736e     if not np.isn
-00002ea0: 616e 286c 6f77 6572 293a 0a20 2020 2020  an(lower):.     
+00002e90: 2020 2020 2020 2020 6966 206e 6f74 206e          if not n
+00002ea0: 702e 6973 6e61 6e28 6c6f 7765 7229 3a0a  p.isnan(lower):.
 00002eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ec0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00002ed0: 6c66 2e6d 6f64 656c 735b 695d 2e6e 436f  lf.models[i].nCo
-00002ee0: 6c6c 3c75 7070 6572 2061 6e64 2073 656c  ll<upper and sel
-00002ef0: 662e 6d6f 6465 6c73 5b69 5d2e 6e43 6f6c  f.models[i].nCol
-00002f00: 6c3e 6c6f 7765 723a 0a20 2020 2020 2020  l>lower:.       
+00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ed0: 6966 2073 656c 662e 6d6f 6465 6c73 5b69  if self.models[i
+00002ee0: 5d2e 6e43 6f6c 6c3c 7570 7065 7220 616e  ].nColl<upper an
+00002ef0: 6420 7365 6c66 2e6d 6f64 656c 735b 695d  d self.models[i]
+00002f00: 2e6e 436f 6c6c 3e6c 6f77 6572 3a0a 2020  .nColl>lower:.  
 00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f20: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00002f30: 5f64 6174 612e 6164 645f 6d6f 6465 6c28  _data.add_model(
-00002f40: 7365 6c66 2e6d 6f64 656c 735b 695d 290a  self.models[i]).
-00002f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f60: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00002f70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f30: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
+00002f40: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
+00002f50: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
 00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f90: 2020 6966 2073 656c 662e 6d6f 6465 6c73    if self.models
-00002fa0: 5b69 5d2e 6e43 6f6c 6c3d 3d75 7070 6572  [i].nColl==upper
-00002fb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002f90: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00002fa0: 6f64 656c 735b 695d 2e6e 436f 6c6c 3d3d  odels[i].nColl==
+00002fb0: 7570 7065 723a 0a20 2020 2020 2020 2020  upper:.         
 00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fd0: 2020 2020 2020 7265 745f 6461 7461 2e61        ret_data.a
-00002fe0: 6464 5f6d 6f64 656c 2873 656c 662e 6d6f  dd_model(self.mo
-00002ff0: 6465 6c73 5b69 5d29 0a20 2020 2020 2020  dels[i]).       
-00003000: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00003010: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-00003020: 2e73 746f 702c 6c69 7374 293a 0a20 2020  .stop,list):.   
-00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003040: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00003050: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-00003060: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00003070: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003080: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
-00003090: 2e6e 436f 6c6c 2069 6e20 6172 672e 7374  .nColl in arg.st
-000030a0: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
+00002fd0: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
+00002fe0: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
+00002ff0: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
+00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003010: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00003020: 6528 6172 672e 7374 6f70 2c6c 6973 7429  e(arg.stop,list)
+00003030: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003040: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00003050: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
+00003060: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
+00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003080: 2020 2020 6966 2073 656c 662e 6d6f 6465      if self.mode
+00003090: 6c73 5b69 5d2e 6e43 6f6c 6c20 696e 2061  ls[i].nColl in a
+000030a0: 7267 2e73 746f 703a 0a20 2020 2020 2020  rg.stop:.       
 000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030c0: 2020 2020 7265 745f 6461 7461 2e61 6464      ret_data.add
-000030d0: 5f6d 6f64 656c 2873 656c 662e 6d6f 6465  _model(self.mode
-000030e0: 6c73 5b69 5d29 0a20 2020 2020 2020 2020  ls[i]).         
-000030f0: 2020 2020 2020 2065 6c69 6620 6172 672e         elif arg.
-00003100: 7374 6172 743d 3d27 6e65 273a 0a20 2020  start=='ne':.   
-00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003120: 2075 7070 6572 3d6e 702e 6e61 6e0a 2020   upper=np.nan.  
-00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 2020 6c6f 7765 723d 6e70 2e6e 616e 0a20    lower=np.nan. 
-00003150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003160: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00003170: 2861 7267 2e73 746f 702c 666c 6f61 7429  (arg.stop,float)
-00003180: 206f 7220 6973 696e 7374 616e 6365 2861   or isinstance(a
-00003190: 7267 2e73 746f 702c 696e 7429 3a0a 2020  rg.stop,int):.  
-000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031b0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-000031c0: 6e63 6528 6172 672e 7374 6570 2c66 6c6f  nce(arg.step,flo
-000031d0: 6174 2920 6f72 2069 7369 6e73 7461 6e63  at) or isinstanc
-000031e0: 6528 6172 672e 7374 6570 2c69 6e74 293a  e(arg.step,int):
-000031f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003200: 2020 2020 2020 2020 2020 2020 206c 6f77               low
-00003210: 6572 2c75 7070 6572 3d61 7267 2e73 746f  er,upper=arg.sto
-00003220: 702c 6172 672e 7374 6570 0a20 2020 2020  p,arg.step.     
+000030c0: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
+000030d0: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
+000030e0: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
+000030f0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00003100: 2061 7267 2e73 7461 7274 3d3d 276e 6527   arg.start=='ne'
+00003110: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003120: 2020 2020 2020 7570 7065 723d 6e70 2e6e        upper=np.n
+00003130: 616e 0a20 2020 2020 2020 2020 2020 2020  an.             
+00003140: 2020 2020 2020 206c 6f77 6572 3d6e 702e         lower=np.
+00003150: 6e61 6e0a 2020 2020 2020 2020 2020 2020  nan.            
+00003160: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00003170: 7461 6e63 6528 6172 672e 7374 6f70 2c66  tance(arg.stop,f
+00003180: 6c6f 6174 2920 6f72 2069 7369 6e73 7461  loat) or isinsta
+00003190: 6e63 6528 6172 672e 7374 6f70 2c69 6e74  nce(arg.stop,int
+000031a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000031b0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+000031c0: 696e 7374 616e 6365 2861 7267 2e73 7465  instance(arg.ste
+000031d0: 702c 666c 6f61 7429 206f 7220 6973 696e  p,float) or isin
+000031e0: 7374 616e 6365 2861 7267 2e73 7465 702c  stance(arg.step,
+000031f0: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003210: 2020 6c6f 7765 722c 7570 7065 723d 6172    lower,upper=ar
+00003220: 672e 7374 6f70 2c61 7267 2e73 7465 700a  g.stop,arg.step.
 00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003240: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00003240: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
 00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003260: 2020 2020 2075 7070 6572 3d61 7267 2e73       upper=arg.s
-00003270: 746f 700a 2020 2020 2020 2020 2020 2020  top.            
-00003280: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00003290: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-000032a0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00003260: 2020 2020 2020 2020 2020 7570 7065 723d            upper=
+00003270: 6172 672e 7374 6f70 0a20 2020 2020 2020  arg.stop.       
+00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003290: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+000032a0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
 000032b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032c0: 2020 2020 2020 6966 206e 6f74 206e 702e        if not np.
-000032d0: 6973 6e61 6e28 6c6f 7765 7229 3a0a 2020  isnan(lower):.  
-000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00003300: 2073 656c 662e 6d6f 6465 6c73 5b69 5d2e   self.models[i].
-00003310: 6e65 3c75 7070 6572 2061 6e64 2073 656c  ne<upper and sel
-00003320: 662e 6d6f 6465 6c73 5b69 5d2e 6e65 3e6c  f.models[i].ne>l
-00003330: 6f77 6572 3a0a 2020 2020 2020 2020 2020  ower:.          
+000032c0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+000032d0: 7420 6e70 2e69 736e 616e 286c 6f77 6572  t np.isnan(lower
+000032e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003300: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
+00003310: 735b 695d 2e6e 653c 7570 7065 7220 616e  s[i].ne<upper an
+00003320: 6420 7365 6c66 2e6d 6f64 656c 735b 695d  d self.models[i]
+00003330: 2e6e 653e 6c6f 7765 723a 0a20 2020 2020  .ne>lower:.     
 00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
-00003360: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
-00003370: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
-00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003390: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000033c0: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
-000033d0: 2e6e 653d 3d75 7070 6572 3a0a 2020 2020  .ne==upper:.    
-000033e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003350: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00003360: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
+00003370: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
+00003380: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003390: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000033a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000033b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033c0: 2020 2020 6966 2073 656c 662e 6d6f 6465      if self.mode
+000033d0: 6c73 5b69 5d2e 6e65 3d3d 7570 7065 723a  ls[i].ne==upper:
+000033e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 7265 745f 6461 7461 2e61 6464 5f6d 6f64  ret_data.add_mod
-00003410: 656c 2873 656c 662e 6d6f 6465 6c73 5b69  el(self.models[i
-00003420: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00003430: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-00003440: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
-00003450: 6c69 7374 293a 0a0a 2020 2020 2020 2020  list):..        
+00003400: 2020 2020 2072 6574 5f64 6174 612e 6164       ret_data.ad
+00003410: 645f 6d6f 6465 6c28 7365 6c66 2e6d 6f64  d_model(self.mod
+00003420: 656c 735b 695d 290a 2020 2020 2020 2020  els[i]).        
+00003430: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00003440: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00003450: 7374 6f70 2c6c 6973 7429 3a0a 0a20 2020  stop,list):..   
 00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00003480: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00003490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034a0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000034b0: 662e 6d6f 6465 6c73 5b69 5d2e 6e65 2069  f.models[i].ne i
-000034c0: 6e20 6172 672e 7374 6f70 3a0a 2020 2020  n arg.stop:.    
-000034d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034e0: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
-000034f0: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
-00003500: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
-00003510: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00003520: 6c69 6620 6172 672e 7374 6172 743d 3d27  lif arg.start=='
-00003530: 6e48 6527 3a0a 2020 2020 2020 2020 2020  nHe':.          
-00003540: 2020 2020 2020 2020 2020 7570 7065 723d            upper=
-00003550: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
-00003560: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
-00003570: 3d6e 702e 6e61 6e0a 2020 2020 2020 2020  =np.nan.        
-00003580: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00003590: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
-000035a0: 6f70 2c66 6c6f 6174 2920 6f72 2069 7369  op,float) or isi
-000035b0: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
-000035c0: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
-000035d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000035e0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-000035f0: 2e73 7465 702c 666c 6f61 7429 206f 7220  .step,float) or 
-00003600: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00003610: 7465 702c 696e 7429 3a0a 2020 2020 2020  tep,int):.      
+00003470: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00003480: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
+00003490: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000034a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000034b0: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
+000034c0: 2e6e 6520 696e 2061 7267 2e73 746f 703a  .ne in arg.stop:
+000034d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034f0: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
+00003500: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
+00003510: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+00003520: 2020 2020 656c 6966 2061 7267 2e73 7461      elif arg.sta
+00003530: 7274 3d3d 276e 4865 273a 0a20 2020 2020  rt=='nHe':.     
+00003540: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00003550: 7070 6572 3d6e 702e 6e61 6e0a 2020 2020  pper=np.nan.    
+00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003570: 6c6f 7765 723d 6e70 2e6e 616e 0a20 2020  lower=np.nan.   
+00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003590: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
+000035a0: 7267 2e73 746f 702c 666c 6f61 7429 206f  rg.stop,float) o
+000035b0: 7220 6973 696e 7374 616e 6365 2861 7267  r isinstance(arg
+000035c0: 2e73 746f 702c 696e 7429 3a0a 2020 2020  .stop,int):.    
+000035d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035e0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000035f0: 6528 6172 672e 7374 6570 2c66 6c6f 6174  e(arg.step,float
+00003600: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
+00003610: 6172 672e 7374 6570 2c69 6e74 293a 0a20  arg.step,int):. 
 00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 2020 2020 2020 6c6f 7765 722c 7570 7065        lower,uppe
-00003640: 723d 6172 672e 7374 6f70 2c61 7267 2e73  r=arg.stop,arg.s
-00003650: 7465 700a 2020 2020 2020 2020 2020 2020  tep.            
-00003660: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00003670: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003680: 2020 2020 2020 2020 2020 2020 2020 7570                up
-00003690: 7065 723d 6172 672e 7374 6f70 0a20 2020  per=arg.stop.   
-000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036b0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-000036c0: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-000036d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000036e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000036f0: 6620 6e6f 7420 6e70 2e69 736e 616e 286c  f not np.isnan(l
-00003700: 6f77 6572 293a 0a20 2020 2020 2020 2020  ower):.         
+00003630: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
+00003640: 2c75 7070 6572 3d61 7267 2e73 746f 702c  ,upper=arg.stop,
+00003650: 6172 672e 7374 6570 0a20 2020 2020 2020  arg.step.       
+00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003670: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00003680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003690: 2020 2075 7070 6572 3d61 7267 2e73 746f     upper=arg.sto
+000036a0: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+000036b0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+000036c0: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
+000036d0: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
+000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036f0: 2020 2020 6966 206e 6f74 206e 702e 6973      if not np.is
+00003700: 6e61 6e28 6c6f 7765 7229 3a0a 2020 2020  nan(lower):.    
 00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003720: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00003730: 6f64 656c 735b 695d 2e6e 4865 3c75 7070  odels[i].nHe<upp
-00003740: 6572 2061 6e64 2073 656c 662e 6d6f 6465  er and self.mode
-00003750: 6c73 5b69 5d2e 6e48 653e 6c6f 7765 723a  ls[i].nHe>lower:
-00003760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003720: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00003730: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6e48  elf.models[i].nH
+00003740: 653c 7570 7065 7220 616e 6420 7365 6c66  e<upper and self
+00003750: 2e6d 6f64 656c 735b 695d 2e6e 4865 3e6c  .models[i].nHe>l
+00003760: 6f77 6572 3a0a 2020 2020 2020 2020 2020  ower:.          
 00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2020 2072 6574 5f64 6174 612e 6164       ret_data.ad
-00003790: 645f 6d6f 6465 6c28 7365 6c66 2e6d 6f64  d_model(self.mod
-000037a0: 656c 735b 695d 290a 2020 2020 2020 2020  els[i]).        
+00003780: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
+00003790: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
+000037a0: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
 000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000037c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 000037d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000037f0: 662e 6d6f 6465 6c73 5b69 5d2e 6e48 653d  f.models[i].nHe=
-00003800: 3d75 7070 6572 3a0a 2020 2020 2020 2020  =upper:.        
+000037e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000037f0: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
+00003800: 2e6e 4865 3d3d 7570 7065 723a 0a20 2020  .nHe==upper:.   
 00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003820: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
-00003830: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
-00003840: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
-00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00003870: 6365 2861 7267 2e73 746f 702c 6c69 7374  ce(arg.stop,list
-00003880: 293a 0a0a 2020 2020 2020 2020 2020 2020  ):..            
-00003890: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000038a0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-000038b0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003830: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
+00003840: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
+00003850: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+00003860: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+00003870: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
+00003880: 2c6c 6973 7429 3a0a 0a20 2020 2020 2020  ,list):..       
+00003890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038a0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+000038b0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
 000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038d0: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
-000038e0: 6465 6c73 5b69 5d2e 6e48 6520 696e 2061  dels[i].nHe in a
-000038f0: 7267 2e73 746f 703a 0a20 2020 2020 2020  rg.stop:.       
+000038d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000038e0: 6c66 2e6d 6f64 656c 735b 695d 2e6e 4865  lf.models[i].nHe
+000038f0: 2069 6e20 6172 672e 7374 6f70 3a0a 2020   in arg.stop:.  
 00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003910: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
-00003920: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
-00003930: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
-00003940: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00003950: 2061 7267 2e73 7461 7274 3d3d 276e 4849   arg.start=='nHI
-00003960: 4927 3a0a 2020 2020 2020 2020 2020 2020  I':.            
-00003970: 2020 2020 2020 2020 7570 7065 723d 6e70          upper=np
-00003980: 2e6e 616e 0a20 2020 2020 2020 2020 2020  .nan.           
-00003990: 2020 2020 2020 2020 206c 6f77 6572 3d6e           lower=n
-000039a0: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
-000039b0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-000039c0: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
-000039d0: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
-000039e0: 7461 6e63 6528 6172 672e 7374 6f70 2c69  tance(arg.stop,i
-000039f0: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-00003a00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00003a10: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00003a20: 7465 702c 666c 6f61 7429 206f 7220 6973  tep,float) or is
-00003a30: 696e 7374 616e 6365 2861 7267 2e73 7465  instance(arg.ste
-00003a40: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
+00003910: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00003920: 745f 6461 7461 2e61 6464 5f6d 6f64 656c  t_data.add_model
+00003930: 2873 656c 662e 6d6f 6465 6c73 5b69 5d29  (self.models[i])
+00003940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003950: 2065 6c69 6620 6172 672e 7374 6172 743d   elif arg.start=
+00003960: 3d27 6e48 4949 273a 0a20 2020 2020 2020  ='nHII':.       
+00003970: 2020 2020 2020 2020 2020 2020 2075 7070               upp
+00003980: 6572 3d6e 702e 6e61 6e0a 2020 2020 2020  er=np.nan.      
+00003990: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000039a0: 7765 723d 6e70 2e6e 616e 0a20 2020 2020  wer=np.nan.     
+000039b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000039c0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
+000039d0: 2e73 746f 702c 666c 6f61 7429 206f 7220  .stop,float) or 
+000039e0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+000039f0: 746f 702c 696e 7429 3a0a 2020 2020 2020  top,int):.      
+00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a10: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00003a20: 6172 672e 7374 6570 2c66 6c6f 6174 2920  arg.step,float) 
+00003a30: 6f72 2069 7369 6e73 7461 6e63 6528 6172  or isinstance(ar
+00003a40: 672e 7374 6570 2c69 6e74 293a 0a20 2020  g.step,int):.   
 00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 2020 2020 6c6f 7765 722c 7570 7065 723d      lower,upper=
-00003a70: 6172 672e 7374 6f70 2c61 7267 2e73 7465  arg.stop,arg.ste
-00003a80: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-00003a90: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ab0: 2020 2020 2020 2020 2020 2020 7570 7065              uppe
-00003ac0: 723d 6172 672e 7374 6f70 0a20 2020 2020  r=arg.stop.     
+00003a60: 2020 2020 2020 2020 206c 6f77 6572 2c75           lower,u
+00003a70: 7070 6572 3d61 7267 2e73 746f 702c 6172  pper=arg.stop,ar
+00003a80: 672e 7374 6570 0a20 2020 2020 2020 2020  g.step.         
+00003a90: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003aa0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ac0: 2075 7070 6572 3d61 7267 2e73 746f 700a   upper=arg.stop.
 00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ae0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00003af0: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-00003b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003b10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00003b20: 6e6f 7420 6e70 2e69 736e 616e 286c 6f77  not np.isnan(low
-00003b30: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
+00003ae0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00003af0: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
+00003b00: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2020 6966 206e 6f74 206e 702e 6973 6e61    if not np.isna
+00003b30: 6e28 6c6f 7765 7229 3a0a 2020 2020 2020  n(lower):.      
 00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b50: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
-00003b60: 656c 735b 695d 2e6e 4849 493c 7570 7065  els[i].nHII<uppe
-00003b70: 7220 616e 6420 7365 6c66 2e6d 6f64 656c  r and self.model
-00003b80: 735b 695d 2e6e 4849 493e 6c6f 7765 723a  s[i].nHII>lower:
-00003b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b50: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00003b60: 662e 6d6f 6465 6c73 5b69 5d2e 6e48 4949  f.models[i].nHII
+00003b70: 3c75 7070 6572 2061 6e64 2073 656c 662e  <upper and self.
+00003b80: 6d6f 6465 6c73 5b69 5d2e 6e48 4949 3e6c  models[i].nHII>l
+00003b90: 6f77 6572 3a0a 2020 2020 2020 2020 2020  ower:.          
 00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bb0: 2020 2020 2072 6574 5f64 6174 612e 6164       ret_data.ad
-00003bc0: 645f 6d6f 6465 6c28 7365 6c66 2e6d 6f64  d_model(self.mod
-00003bd0: 656c 735b 695d 290a 2020 2020 2020 2020  els[i]).        
+00003bb0: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
+00003bc0: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
+00003bd0: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
 00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bf0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00003bf0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c10: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00003c20: 662e 6d6f 6465 6c73 5b69 5d2e 6e48 4949  f.models[i].nHII
-00003c30: 3d3d 7570 7065 723a 0a20 2020 2020 2020  ==upper:.       
+00003c10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003c20: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
+00003c30: 2e6e 4849 493d 3d75 7070 6572 3a0a 2020  .nHII==upper:.  
 00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c50: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00003c60: 5f64 6174 612e 6164 645f 6d6f 6465 6c28  _data.add_model(
-00003c70: 7365 6c66 2e6d 6f64 656c 735b 695d 290a  self.models[i]).
-00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c90: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00003ca0: 6e63 6528 6172 672e 7374 6f70 2c6c 6973  nce(arg.stop,lis
-00003cb0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00003cc0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00003cd0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-00003ce0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00003c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c60: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
+00003c70: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
+00003c80: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+00003c90: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
+00003ca0: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
+00003cb0: 702c 6c69 7374 293a 0a20 2020 2020 2020  p,list):.       
+00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cd0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00003ce0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
 00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d00: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
-00003d10: 6465 6c73 5b69 5d2e 6e48 4949 2069 6e20  dels[i].nHII in 
-00003d20: 6172 672e 7374 6f70 3a0a 2020 2020 2020  arg.stop:.      
+00003d00: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00003d10: 6c66 2e6d 6f64 656c 735b 695d 2e6e 4849  lf.models[i].nHI
+00003d20: 4920 696e 2061 7267 2e73 746f 703a 0a20  I in arg.stop:. 
 00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d40: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
-00003d50: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
-00003d60: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
-00003d70: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00003d80: 6620 6172 672e 7374 6172 743d 3d27 6e48  f arg.start=='nH
-00003d90: 4927 3a0a 2020 2020 2020 2020 2020 2020  I':.            
-00003da0: 2020 2020 2020 2020 7570 7065 723d 6e70          upper=np
-00003db0: 2e6e 616e 0a20 2020 2020 2020 2020 2020  .nan.           
-00003dc0: 2020 2020 2020 2020 206c 6f77 6572 3d6e           lower=n
-00003dd0: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
-00003de0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00003df0: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
-00003e00: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
-00003e10: 7461 6e63 6528 6172 672e 7374 6f70 2c69  tance(arg.stop,i
-00003e20: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-00003e30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00003e40: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00003e50: 7465 702c 666c 6f61 7429 206f 7220 6973  tep,float) or is
-00003e60: 696e 7374 616e 6365 2861 7267 2e73 7465  instance(arg.ste
-00003e70: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
+00003d40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00003d50: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
+00003d60: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
+00003d70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003d80: 2020 656c 6966 2061 7267 2e73 7461 7274    elif arg.start
+00003d90: 3d3d 276e 4849 273a 0a20 2020 2020 2020  =='nHI':.       
+00003da0: 2020 2020 2020 2020 2020 2020 2075 7070               upp
+00003db0: 6572 3d6e 702e 6e61 6e0a 2020 2020 2020  er=np.nan.      
+00003dc0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00003dd0: 7765 723d 6e70 2e6e 616e 0a20 2020 2020  wer=np.nan.     
+00003de0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003df0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
+00003e00: 2e73 746f 702c 666c 6f61 7429 206f 7220  .stop,float) or 
+00003e10: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00003e20: 746f 702c 696e 7429 3a0a 2020 2020 2020  top,int):.      
+00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e40: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00003e50: 6172 672e 7374 6570 2c66 6c6f 6174 2920  arg.step,float) 
+00003e60: 6f72 2069 7369 6e73 7461 6e63 6528 6172  or isinstance(ar
+00003e70: 672e 7374 6570 2c69 6e74 293a 0a20 2020  g.step,int):.   
 00003e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e90: 2020 2020 6c6f 7765 722c 7570 7065 723d      lower,upper=
-00003ea0: 6172 672e 7374 6f70 2c61 7267 2e73 7465  arg.stop,arg.ste
-00003eb0: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-00003ec0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00003ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ee0: 2020 2020 2020 2020 2020 2020 7570 7065              uppe
-00003ef0: 723d 6172 672e 7374 6f70 0a20 2020 2020  r=arg.stop.     
+00003e90: 2020 2020 2020 2020 206c 6f77 6572 2c75           lower,u
+00003ea0: 7070 6572 3d61 7267 2e73 746f 702c 6172  pper=arg.stop,ar
+00003eb0: 672e 7374 6570 0a20 2020 2020 2020 2020  g.step.         
+00003ec0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003ed0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00003ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ef0: 2075 7070 6572 3d61 7267 2e73 746f 700a   upper=arg.stop.
 00003f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f10: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00003f20: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-00003f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003f40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00003f50: 6e6f 7420 6e70 2e69 736e 616e 286c 6f77  not np.isnan(low
-00003f60: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
+00003f10: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00003f20: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
+00003f30: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+00003f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f50: 2020 6966 206e 6f74 206e 702e 6973 6e61    if not np.isna
+00003f60: 6e28 6c6f 7765 7229 3a0a 2020 2020 2020  n(lower):.      
 00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f80: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
-00003f90: 656c 735b 695d 2e6e 4849 3c75 7070 6572  els[i].nHI<upper
-00003fa0: 2061 6e64 2073 656c 662e 6d6f 6465 6c73   and self.models
-00003fb0: 5b69 5d2e 6e48 493e 6c6f 7765 723a 0a20  [i].nHI>lower:. 
-00003fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f80: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00003f90: 662e 6d6f 6465 6c73 5b69 5d2e 6e48 493c  f.models[i].nHI<
+00003fa0: 7570 7065 7220 616e 6420 7365 6c66 2e6d  upper and self.m
+00003fb0: 6f64 656c 735b 695d 2e6e 4849 3e6c 6f77  odels[i].nHI>low
+00003fc0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
 00003fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fe0: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
-00003ff0: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
-00004000: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
+00003fe0: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
+00003ff0: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
+00004000: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
 00004010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004020: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00004020: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
 00004030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004040: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00004050: 6d6f 6465 6c73 5b69 5d2e 6e48 493d 3d75  models[i].nHI==u
-00004060: 7070 6572 3a0a 2020 2020 2020 2020 2020  pper:.          
+00004040: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004050: 7365 6c66 2e6d 6f64 656c 735b 695d 2e6e  self.models[i].n
+00004060: 4849 3d3d 7570 7065 723a 0a20 2020 2020  HI==upper:.     
 00004070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004080: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
-00004090: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
-000040a0: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
-000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040c0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-000040d0: 2861 7267 2e73 746f 702c 6c69 7374 293a  (arg.stop,list):
-000040e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000040f0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00004100: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-00004110: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00004080: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004090: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
+000040a0: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
+000040b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000040c0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+000040d0: 7461 6e63 6528 6172 672e 7374 6f70 2c6c  tance(arg.stop,l
+000040e0: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
+000040f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00004100: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+00004110: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
 00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004130: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
-00004140: 735b 695d 2e6e 4849 2069 6e20 6172 672e  s[i].nHI in arg.
-00004150: 7374 6f70 3a0a 2020 2020 2020 2020 2020  stop:.          
+00004130: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00004140: 6d6f 6465 6c73 5b69 5d2e 6e48 4920 696e  models[i].nHI in
+00004150: 2061 7267 2e73 746f 703a 0a20 2020 2020   arg.stop:.     
 00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004170: 2020 2020 2020 7265 745f 6461 7461 2e61        ret_data.a
-00004180: 6464 5f6d 6f64 656c 2873 656c 662e 6d6f  dd_model(self.mo
-00004190: 6465 6c73 5b69 5d29 0a20 2020 2020 2020  dels[i]).       
-000041a0: 2020 2020 2020 2020 2065 6c69 6620 6172           elif ar
-000041b0: 672e 7374 6172 743d 3d27 6e48 3227 3a0a  g.start=='nH2':.
-000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041d0: 2020 2020 7570 7065 723d 6e70 2e6e 616e      upper=np.nan
-000041e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000041f0: 2020 2020 206c 6f77 6572 3d6e 702e 6e61       lower=np.na
-00004200: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00004210: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00004220: 6e63 6528 6172 672e 7374 6f70 2c66 6c6f  nce(arg.stop,flo
-00004230: 6174 2920 6f72 2069 7369 6e73 7461 6e63  at) or isinstanc
-00004240: 6528 6172 672e 7374 6f70 2c69 6e74 293a  e(arg.stop,int):
-00004250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004260: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-00004270: 7374 616e 6365 2861 7267 2e73 7465 702c  stance(arg.step,
-00004280: 666c 6f61 7429 206f 7220 6973 696e 7374  float) or isinst
-00004290: 616e 6365 2861 7267 2e73 7465 702c 696e  ance(arg.step,in
-000042a0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00004170: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
+00004180: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
+00004190: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
+000041a0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000041b0: 6966 2061 7267 2e73 7461 7274 3d3d 276e  if arg.start=='n
+000041c0: 4832 273a 0a20 2020 2020 2020 2020 2020  H2':.           
+000041d0: 2020 2020 2020 2020 2075 7070 6572 3d6e           upper=n
+000041e0: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
+000041f0: 2020 2020 2020 2020 2020 6c6f 7765 723d            lower=
+00004200: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
+00004210: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00004220: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
+00004230: 702c 666c 6f61 7429 206f 7220 6973 696e  p,float) or isin
+00004240: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
+00004250: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+00004260: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004270: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00004280: 7374 6570 2c66 6c6f 6174 2920 6f72 2069  step,float) or i
+00004290: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+000042a0: 6570 2c69 6e74 293a 0a20 2020 2020 2020  ep,int):.       
 000042b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042c0: 6c6f 7765 722c 7570 7065 723d 6172 672e  lower,upper=arg.
-000042d0: 7374 6f70 2c61 7267 2e73 7465 700a 2020  stop,arg.step.  
-000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00004300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004310: 2020 2020 2020 2020 7570 7065 723d 6172          upper=ar
-00004320: 672e 7374 6f70 0a20 2020 2020 2020 2020  g.stop.         
-00004330: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00004340: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-00004350: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004370: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00004380: 6e70 2e69 736e 616e 286c 6f77 6572 293a  np.isnan(lower):
-00004390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000042c0: 2020 2020 206c 6f77 6572 2c75 7070 6572       lower,upper
+000042d0: 3d61 7267 2e73 746f 702c 6172 672e 7374  =arg.stop,arg.st
+000042e0: 6570 0a20 2020 2020 2020 2020 2020 2020  ep.             
+000042f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00004300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004310: 2020 2020 2020 2020 2020 2020 2075 7070               upp
+00004320: 6572 3d61 7267 2e73 746f 700a 2020 2020  er=arg.stop.    
+00004330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004340: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00004350: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+00004360: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004370: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004380: 206e 6f74 206e 702e 6973 6e61 6e28 6c6f   not np.isnan(lo
+00004390: 7765 7229 3a0a 2020 2020 2020 2020 2020  wer):.          
 000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043b0: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
-000043c0: 695d 2e6e 4832 3c75 7070 6572 2061 6e64  i].nH2<upper and
-000043d0: 2073 656c 662e 6d6f 6465 6c73 5b69 5d2e   self.models[i].
-000043e0: 6e48 323e 6c6f 7765 723a 0a20 2020 2020  nH2>lower:.     
+000043b0: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
+000043c0: 6465 6c73 5b69 5d2e 6e48 323c 7570 7065  dels[i].nH2<uppe
+000043d0: 7220 616e 6420 7365 6c66 2e6d 6f64 656c  r and self.model
+000043e0: 735b 695d 2e6e 4832 3e6c 6f77 6572 3a0a  s[i].nH2>lower:.
 000043f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004400: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004410: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
-00004420: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
-00004430: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004440: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00004450: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00004400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004410: 2020 2020 7265 745f 6461 7461 2e61 6464      ret_data.add
+00004420: 5f6d 6f64 656c 2873 656c 662e 6d6f 6465  _model(self.mode
+00004430: 6c73 5b69 5d29 0a20 2020 2020 2020 2020  ls[i]).         
+00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004450: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
 00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004470: 2020 2020 6966 2073 656c 662e 6d6f 6465      if self.mode
-00004480: 6c73 5b69 5d2e 6e48 323d 3d75 7070 6572  ls[i].nH2==upper
-00004490: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004470: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00004480: 2e6d 6f64 656c 735b 695d 2e6e 4832 3d3d  .models[i].nH2==
+00004490: 7570 7065 723a 0a20 2020 2020 2020 2020  upper:.         
 000044a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044b0: 2020 2020 2020 7265 745f 6461 7461 2e61        ret_data.a
-000044c0: 6464 5f6d 6f64 656c 2873 656c 662e 6d6f  dd_model(self.mo
-000044d0: 6465 6c73 5b69 5d29 0a20 2020 2020 2020  dels[i]).       
-000044e0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-000044f0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-00004500: 2e73 746f 702c 6c69 7374 293a 0a0a 2020  .stop,list):..  
-00004510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004520: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00004530: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
-00004540: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+000044b0: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
+000044c0: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
+000044d0: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
+000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044f0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00004500: 6528 6172 672e 7374 6f70 2c6c 6973 7429  e(arg.stop,list)
+00004510: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004520: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00004530: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+00004540: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
 00004550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004560: 6966 2073 656c 662e 6d6f 6465 6c73 5b69  if self.models[i
-00004570: 5d2e 6e48 3220 696e 2061 7267 2e73 746f  ].nH2 in arg.sto
-00004580: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+00004560: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
+00004570: 656c 735b 695d 2e6e 4832 2069 6e20 6172  els[i].nH2 in ar
+00004580: 672e 7374 6f70 3a0a 2020 2020 2020 2020  g.stop:.        
 00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045a0: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
-000045b0: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
-000045c0: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
-000045d0: 2020 2020 2020 656c 6966 2061 7267 2e73        elif arg.s
-000045e0: 7461 7274 3d3d 2764 7573 745f 746f 5f67  tart=='dust_to_g
-000045f0: 6173 273a 0a20 2020 2020 2020 2020 2020  as':.           
-00004600: 2020 2020 2020 2020 2075 7070 6572 3d6e           upper=n
-00004610: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
-00004620: 2020 2020 2020 2020 2020 6c6f 7765 723d            lower=
-00004630: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
-00004640: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00004650: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
-00004660: 702c 666c 6f61 7429 206f 7220 6973 696e  p,float) or isin
-00004670: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
-00004680: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00004690: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000046a0: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-000046b0: 7374 6570 2c66 6c6f 6174 2920 6f72 2069  step,float) or i
-000046c0: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
-000046d0: 6570 2c69 6e74 293a 0a20 2020 2020 2020  ep,int):.       
+000045a0: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
+000045b0: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
+000045c0: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
+000045d0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000045e0: 6172 672e 7374 6172 743d 3d27 6475 7374  arg.start=='dust
+000045f0: 5f74 6f5f 6761 7327 3a0a 2020 2020 2020  _to_gas':.      
+00004600: 2020 2020 2020 2020 2020 2020 2020 7570                up
+00004610: 7065 723d 6e70 2e6e 616e 0a20 2020 2020  per=np.nan.     
+00004620: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00004630: 6f77 6572 3d6e 702e 6e61 6e0a 2020 2020  ower=np.nan.    
+00004640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004650: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
+00004660: 672e 7374 6f70 2c66 6c6f 6174 2920 6f72  g.stop,float) or
+00004670: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00004680: 7374 6f70 2c69 6e74 293a 0a20 2020 2020  stop,int):.     
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+000046b0: 2861 7267 2e73 7465 702c 666c 6f61 7429  (arg.step,float)
+000046c0: 206f 7220 6973 696e 7374 616e 6365 2861   or isinstance(a
+000046d0: 7267 2e73 7465 702c 696e 7429 3a0a 2020  rg.step,int):.  
 000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046f0: 2020 2020 206c 6f77 6572 2c75 7070 6572       lower,upper
-00004700: 3d61 7267 2e73 746f 702c 6172 672e 7374  =arg.stop,arg.st
-00004710: 6570 0a20 2020 2020 2020 2020 2020 2020  ep.             
-00004720: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00004730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004740: 2020 2020 2020 2020 2020 2020 2075 7070               upp
-00004750: 6572 3d61 7267 2e73 746f 700a 2020 2020  er=arg.stop.    
-00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004770: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00004780: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-00004790: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000047a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000047b0: 206e 6f74 206e 702e 6973 6e61 6e28 6c6f   not np.isnan(lo
-000047c0: 7765 7229 3a0a 2020 2020 2020 2020 2020  wer):.          
+000046f0: 2020 2020 2020 2020 2020 6c6f 7765 722c            lower,
+00004700: 7570 7065 723d 6172 672e 7374 6f70 2c61  upper=arg.stop,a
+00004710: 7267 2e73 7465 700a 2020 2020 2020 2020  rg.step.        
+00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004730: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00004740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004750: 2020 7570 7065 723d 6172 672e 7374 6f70    upper=arg.stop
+00004760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004770: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00004780: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+00004790: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 2020 2069 6620 6e6f 7420 6e70 2e69 736e     if not np.isn
+000047c0: 616e 286c 6f77 6572 293a 0a20 2020 2020  an(lower):.     
 000047d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047e0: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
-000047f0: 6465 6c73 5b69 5d2e 6475 7374 5f74 6f5f  dels[i].dust_to_
-00004800: 6761 733c 7570 7065 7220 616e 6420 7365  gas<upper and se
-00004810: 6c66 2e6d 6f64 656c 735b 695d 2e64 7573  lf.models[i].dus
-00004820: 745f 746f 5f67 6173 3e6c 6f77 6572 3a0a  t_to_gas>lower:.
-00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000047f0: 6c66 2e6d 6f64 656c 735b 695d 2e64 7573  lf.models[i].dus
+00004800: 745f 746f 5f67 6173 3c75 7070 6572 2061  t_to_gas<upper a
+00004810: 6e64 2073 656c 662e 6d6f 6465 6c73 5b69  nd self.models[i
+00004820: 5d2e 6475 7374 5f74 6f5f 6761 733e 6c6f  ].dust_to_gas>lo
+00004830: 7765 723a 0a20 2020 2020 2020 2020 2020  wer:.           
 00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004850: 2020 2020 7265 745f 6461 7461 2e61 6464      ret_data.add
-00004860: 5f6d 6f64 656c 2873 656c 662e 6d6f 6465  _model(self.mode
-00004870: 6c73 5b69 5d29 0a20 2020 2020 2020 2020  ls[i]).         
+00004850: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
+00004860: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
+00004870: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
 00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004890: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00004890: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
 000048a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048b0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000048c0: 2e6d 6f64 656c 735b 695d 2e64 7573 745f  .models[i].dust_
-000048d0: 746f 5f67 6173 3d3d 7570 7065 723a 0a20  to_gas==upper:. 
-000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000048c0: 2073 656c 662e 6d6f 6465 6c73 5b69 5d2e   self.models[i].
+000048d0: 6475 7374 5f74 6f5f 6761 733d 3d75 7070  dust_to_gas==upp
+000048e0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
 000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004900: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
-00004910: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
-00004920: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
-00004930: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
-00004940: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
-00004950: 6f70 2c6c 6973 7429 3a0a 0a20 2020 2020  op,list):..     
+00004900: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
+00004910: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
+00004920: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
+00004930: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00004940: 6c69 6620 6973 696e 7374 616e 6365 2861  lif isinstance(a
+00004950: 7267 2e73 746f 702c 6c69 7374 293a 0a0a  rg.stop,list):..
 00004960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004970: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00004980: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-00004990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000049a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000049b0: 7365 6c66 2e6d 6f64 656c 735b 695d 2e64  self.models[i].d
-000049c0: 7573 745f 746f 5f67 6173 2069 6e20 6172  ust_to_gas in ar
-000049d0: 672e 7374 6f70 3a0a 2020 2020 2020 2020  g.stop:.        
+00004970: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00004980: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
+00004990: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+000049a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049b0: 2020 6966 2073 656c 662e 6d6f 6465 6c73    if self.models
+000049c0: 5b69 5d2e 6475 7374 5f74 6f5f 6761 7320  [i].dust_to_gas 
+000049d0: 696e 2061 7267 2e73 746f 703a 0a20 2020  in arg.stop:.   
 000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049f0: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
-00004a00: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
-00004a10: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
-00004a20: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00004a30: 6172 672e 7374 6172 743d 3d27 7674 7572  arg.start=='vtur
-00004a40: 6227 3a0a 2020 2020 2020 2020 2020 2020  b':.            
-00004a50: 2020 2020 2020 2020 7570 7065 723d 6e70          upper=np
-00004a60: 2e6e 616e 0a20 2020 2020 2020 2020 2020  .nan.           
-00004a70: 2020 2020 2020 2020 206c 6f77 6572 3d6e           lower=n
-00004a80: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
-00004a90: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00004aa0: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
-00004ab0: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
-00004ac0: 7461 6e63 6528 6172 672e 7374 6f70 2c69  tance(arg.stop,i
-00004ad0: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-00004ae0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004af0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00004b00: 7465 702c 666c 6f61 7429 206f 7220 6973  tep,float) or is
-00004b10: 696e 7374 616e 6365 2861 7267 2e73 7465  instance(arg.ste
-00004b20: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
+000049f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00004a00: 5f64 6174 612e 6164 645f 6d6f 6465 6c28  _data.add_model(
+00004a10: 7365 6c66 2e6d 6f64 656c 735b 695d 290a  self.models[i]).
+00004a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a30: 656c 6966 2061 7267 2e73 7461 7274 3d3d  elif arg.start==
+00004a40: 2776 7475 7262 273a 0a20 2020 2020 2020  'vturb':.       
+00004a50: 2020 2020 2020 2020 2020 2020 2075 7070               upp
+00004a60: 6572 3d6e 702e 6e61 6e0a 2020 2020 2020  er=np.nan.      
+00004a70: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00004a80: 7765 723d 6e70 2e6e 616e 0a20 2020 2020  wer=np.nan.     
+00004a90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004aa0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
+00004ab0: 2e73 746f 702c 666c 6f61 7429 206f 7220  .stop,float) or 
+00004ac0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00004ad0: 746f 702c 696e 7429 3a0a 2020 2020 2020  top,int):.      
+00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004af0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00004b00: 6172 672e 7374 6570 2c66 6c6f 6174 2920  arg.step,float) 
+00004b10: 6f72 2069 7369 6e73 7461 6e63 6528 6172  or isinstance(ar
+00004b20: 672e 7374 6570 2c69 6e74 293a 0a20 2020  g.step,int):.   
 00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 2020 2020 6c6f 7765 722c 7570 7065 723d      lower,upper=
-00004b50: 6172 672e 7374 6f70 2c61 7267 2e73 7465  arg.stop,arg.ste
-00004b60: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-00004b70: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b90: 2020 2020 2020 2020 2020 2020 7570 7065              uppe
-00004ba0: 723d 6172 672e 7374 6f70 0a20 2020 2020  r=arg.stop.     
+00004b40: 2020 2020 2020 2020 206c 6f77 6572 2c75           lower,u
+00004b50: 7070 6572 3d61 7267 2e73 746f 702c 6172  pper=arg.stop,ar
+00004b60: 672e 7374 6570 0a20 2020 2020 2020 2020  g.step.         
+00004b70: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00004b80: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ba0: 2075 7070 6572 3d61 7267 2e73 746f 700a   upper=arg.stop.
 00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00004bd0: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-00004be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004bf0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004c00: 6e6f 7420 6e70 2e69 736e 616e 286c 6f77  not np.isnan(low
-00004c10: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
+00004bc0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00004bd0: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
+00004be0: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c00: 2020 6966 206e 6f74 206e 702e 6973 6e61    if not np.isna
+00004c10: 6e28 6c6f 7765 7229 3a0a 2020 2020 2020  n(lower):.      
 00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
-00004c40: 656c 735b 695d 2e76 7475 7262 3c75 7070  els[i].vturb<upp
-00004c50: 6572 2061 6e64 2073 656c 662e 6d6f 6465  er and self.mode
-00004c60: 6c73 5b69 5d2e 7674 7572 623e 6c6f 7765  ls[i].vturb>lowe
-00004c70: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+00004c30: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00004c40: 662e 6d6f 6465 6c73 5b69 5d2e 7674 7572  f.models[i].vtur
+00004c50: 623c 7570 7065 7220 616e 6420 7365 6c66  b<upper and self
+00004c60: 2e6d 6f64 656c 735b 695d 2e76 7475 7262  .models[i].vturb
+00004c70: 3e6c 6f77 6572 3a0a 2020 2020 2020 2020  >lower:.        
 00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c90: 2020 2020 2020 2072 6574 5f64 6174 612e         ret_data.
-00004ca0: 6164 645f 6d6f 6465 6c28 7365 6c66 2e6d  add_model(self.m
-00004cb0: 6f64 656c 735b 695d 290a 2020 2020 2020  odels[i]).      
+00004c90: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
+00004ca0: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
+00004cb0: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
 00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cf0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00004d00: 656c 662e 6d6f 6465 6c73 5b69 5d2e 7674  elf.models[i].vt
-00004d10: 7572 623d 3d75 7070 6572 3a0a 2020 2020  urb==upper:.    
-00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cd0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00004ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d00: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
+00004d10: 695d 2e76 7475 7262 3d3d 7570 7065 723a  i].vturb==upper:
+00004d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d40: 7265 745f 6461 7461 2e61 6464 5f6d 6f64  ret_data.add_mod
-00004d50: 656c 2873 656c 662e 6d6f 6465 6c73 5b69  el(self.models[i
-00004d60: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00004d70: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-00004d80: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
-00004d90: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
-00004da0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00004db0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-00004dc0: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004de0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00004df0: 2e6d 6f64 656c 735b 695d 2e76 7475 7262  .models[i].vturb
-00004e00: 2069 6e20 6172 672e 7374 6f70 3a0a 2020   in arg.stop:.  
-00004e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e20: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00004e30: 745f 6461 7461 2e61 6464 5f6d 6f64 656c  t_data.add_model
-00004e40: 2873 656c 662e 6d6f 6465 6c73 5b69 5d29  (self.models[i])
-00004e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e60: 2065 6c69 6620 6172 672e 7374 6172 743d   elif arg.start=
-00004e70: 3d27 5467 273a 0a20 2020 2020 2020 2020  ='Tg':.         
-00004e80: 2020 2020 2020 2020 2020 2075 7070 6572             upper
-00004e90: 3d6e 702e 6e61 6e0a 2020 2020 2020 2020  =np.nan.        
-00004ea0: 2020 2020 2020 2020 2020 2020 6c6f 7765              lowe
-00004eb0: 723d 6e70 2e6e 616e 0a20 2020 2020 2020  r=np.nan.       
-00004ec0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004ed0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00004ee0: 746f 702c 666c 6f61 7429 206f 7220 6973  top,float) or is
-00004ef0: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
-00004f00: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
+00004d40: 2020 2020 2072 6574 5f64 6174 612e 6164       ret_data.ad
+00004d50: 645f 6d6f 6465 6c28 7365 6c66 2e6d 6f64  d_model(self.mod
+00004d60: 656c 735b 695d 290a 2020 2020 2020 2020  els[i]).        
+00004d70: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00004d80: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00004d90: 7374 6f70 2c6c 6973 7429 3a0a 2020 2020  stop,list):.    
+00004da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004db0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00004dc0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+00004dd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004de0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004df0: 2073 656c 662e 6d6f 6465 6c73 5b69 5d2e   self.models[i].
+00004e00: 7674 7572 6220 696e 2061 7267 2e73 746f  vturb in arg.sto
+00004e10: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+00004e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e30: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
+00004e40: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
+00004e50: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
+00004e60: 2020 2020 2020 656c 6966 2061 7267 2e73        elif arg.s
+00004e70: 7461 7274 3d3d 2754 6727 3a0a 2020 2020  tart=='Tg':.    
+00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e90: 7570 7065 723d 6e70 2e6e 616e 0a20 2020  upper=np.nan.   
+00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004eb0: 206c 6f77 6572 3d6e 702e 6e61 6e0a 2020   lower=np.nan.  
+00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ed0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00004ee0: 6172 672e 7374 6f70 2c66 6c6f 6174 2920  arg.stop,float) 
+00004ef0: 6f72 2069 7369 6e73 7461 6e63 6528 6172  or isinstance(ar
+00004f00: 672e 7374 6f70 2c69 6e74 293a 0a20 2020  g.stop,int):.   
 00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f20: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
-00004f30: 672e 7374 6570 2c66 6c6f 6174 2920 6f72  g.step,float) or
-00004f40: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-00004f50: 7374 6570 2c69 6e74 293a 0a20 2020 2020  step,int):.     
+00004f20: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00004f30: 6365 2861 7267 2e73 7465 702c 666c 6f61  ce(arg.step,floa
+00004f40: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
+00004f50: 2861 7267 2e73 7465 702c 696e 7429 3a0a  (arg.step,int):.
 00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f70: 2020 2020 2020 206c 6f77 6572 2c75 7070         lower,upp
-00004f80: 6572 3d61 7267 2e73 746f 702c 6172 672e  er=arg.stop,arg.
-00004f90: 7374 6570 0a20 2020 2020 2020 2020 2020  step.           
-00004fa0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00004fb0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00004fc0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00004fd0: 7070 6572 3d61 7267 2e73 746f 700a 2020  pper=arg.stop.  
-00004fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ff0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00005000: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
-00005010: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00004f70: 2020 2020 2020 2020 2020 2020 6c6f 7765              lowe
+00004f80: 722c 7570 7065 723d 6172 672e 7374 6f70  r,upper=arg.stop
+00004f90: 2c61 7267 2e73 7465 700a 2020 2020 2020  ,arg.step.      
+00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fd0: 2020 2020 7570 7065 723d 6172 672e 7374      upper=arg.st
+00004fe0: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
+00004ff0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00005000: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+00005010: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
 00005020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005030: 6966 206e 6f74 206e 702e 6973 6e61 6e28  if not np.isnan(
-00005040: 6c6f 7765 7229 3a0a 2020 2020 2020 2020  lower):.        
+00005030: 2020 2020 2069 6620 6e6f 7420 6e70 2e69       if not np.i
+00005040: 736e 616e 286c 6f77 6572 293a 0a20 2020  snan(lower):.   
 00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005060: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00005070: 6d6f 6465 6c73 5b69 5d2e 5467 3c75 7070  models[i].Tg<upp
-00005080: 6572 2061 6e64 2073 656c 662e 6d6f 6465  er and self.mode
-00005090: 6c73 5b69 5d2e 5467 3e6c 6f77 6572 3a0a  ls[i].Tg>lower:.
-000050a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005060: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00005070: 7365 6c66 2e6d 6f64 656c 735b 695d 2e54  self.models[i].T
+00005080: 673c 7570 7065 7220 616e 6420 7365 6c66  g<upper and self
+00005090: 2e6d 6f64 656c 735b 695d 2e54 673e 6c6f  .models[i].Tg>lo
+000050a0: 7765 723a 0a20 2020 2020 2020 2020 2020  wer:.           
 000050b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050c0: 2020 2020 7265 745f 6461 7461 2e61 6464      ret_data.add
-000050d0: 5f6d 6f64 656c 2873 656c 662e 6d6f 6465  _model(self.mode
-000050e0: 6c73 5b69 5d29 0a20 2020 2020 2020 2020  ls[i]).         
+000050c0: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
+000050d0: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
+000050e0: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
 000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005100: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00005100: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
 00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005120: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00005130: 2e6d 6f64 656c 735b 695d 2e54 673d 3d75  .models[i].Tg==u
-00005140: 7070 6572 3a0a 2020 2020 2020 2020 2020  pper:.          
+00005120: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005130: 2073 656c 662e 6d6f 6465 6c73 5b69 5d2e   self.models[i].
+00005140: 5467 3d3d 7570 7065 723a 0a20 2020 2020  Tg==upper:.     
 00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005160: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
-00005170: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
-00005180: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
-00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051a0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-000051b0: 2861 7267 2e73 746f 702c 6c69 7374 293a  (arg.stop,list):
-000051c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000051d0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-000051e0: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-000051f0: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00005160: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00005170: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
+00005180: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
+00005190: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000051a0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+000051b0: 7461 6e63 6528 6172 672e 7374 6f70 2c6c  tance(arg.stop,l
+000051c0: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
+000051d0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000051e0: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+000051f0: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
 00005200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005210: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
-00005220: 735b 695d 2e54 6720 696e 2061 7267 2e73  s[i].Tg in arg.s
-00005230: 746f 703a 0a20 2020 2020 2020 2020 2020  top:.           
+00005210: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00005220: 6d6f 6465 6c73 5b69 5d2e 5467 2069 6e20  models[i].Tg in 
+00005230: 6172 672e 7374 6f70 3a0a 2020 2020 2020  arg.stop:.      
 00005240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005250: 2020 2020 2072 6574 5f64 6174 612e 6164       ret_data.ad
-00005260: 645f 6d6f 6465 6c28 7365 6c66 2e6d 6f64  d_model(self.mod
-00005270: 656c 735b 695d 290a 2020 2020 2020 2020  els[i]).        
-00005280: 2020 2020 2020 2020 656c 6966 2061 7267          elif arg
-00005290: 2e73 7461 7274 3d3d 2754 6427 3a0a 2020  .start=='Td':.  
-000052a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052b0: 2020 7570 7065 723d 6e70 2e6e 616e 0a20    upper=np.nan. 
-000052c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052d0: 2020 206c 6f77 6572 3d6e 702e 6e61 6e0a     lower=np.nan.
-000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052f0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00005300: 6528 6172 672e 7374 6f70 2c66 6c6f 6174  e(arg.stop,float
-00005310: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
-00005320: 6172 672e 7374 6f70 2c69 6e74 293a 0a20  arg.stop,int):. 
-00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005340: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00005350: 616e 6365 2861 7267 2e73 7465 702c 666c  ance(arg.step,fl
-00005360: 6f61 7429 206f 7220 6973 696e 7374 616e  oat) or isinstan
-00005370: 6365 2861 7267 2e73 7465 702c 696e 7429  ce(arg.step,int)
-00005380: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005390: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000053a0: 7765 722c 7570 7065 723d 6172 672e 7374  wer,upper=arg.st
-000053b0: 6f70 2c61 7267 2e73 7465 700a 2020 2020  op,arg.step.    
-000053c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00005250: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
+00005260: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
+00005270: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
+00005280: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00005290: 6620 6172 672e 7374 6172 743d 3d27 5464  f arg.start=='Td
+000052a0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+000052b0: 2020 2020 2020 2075 7070 6572 3d6e 702e         upper=np.
+000052c0: 6e61 6e0a 2020 2020 2020 2020 2020 2020  nan.            
+000052d0: 2020 2020 2020 2020 6c6f 7765 723d 6e70          lower=np
+000052e0: 2e6e 616e 0a20 2020 2020 2020 2020 2020  .nan.           
+000052f0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00005300: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
+00005310: 666c 6f61 7429 206f 7220 6973 696e 7374  float) or isinst
+00005320: 616e 6365 2861 7267 2e73 746f 702c 696e  ance(arg.stop,in
+00005330: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00005340: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00005350: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+00005360: 6570 2c66 6c6f 6174 2920 6f72 2069 7369  ep,float) or isi
+00005370: 6e73 7461 6e63 6528 6172 672e 7374 6570  nstance(arg.step
+00005380: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
+00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053a0: 2020 206c 6f77 6572 2c75 7070 6572 3d61     lower,upper=a
+000053b0: 7267 2e73 746f 702c 6172 672e 7374 6570  rg.stop,arg.step
+000053c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000053d0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 000053e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053f0: 2020 2020 2020 7570 7065 723d 6172 672e        upper=arg.
-00005400: 7374 6f70 0a20 2020 2020 2020 2020 2020  stop.           
-00005410: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00005420: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-00005430: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+000053f0: 2020 2020 2020 2020 2020 2075 7070 6572             upper
+00005400: 3d61 7267 2e73 746f 700a 2020 2020 2020  =arg.stop.      
+00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005420: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00005430: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
 00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005450: 2020 2020 2020 2069 6620 6e6f 7420 6e70         if not np
-00005460: 2e69 736e 616e 286c 6f77 6572 293a 0a20  .isnan(lower):. 
-00005470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005480: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005490: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
-000054a0: 2e54 643c 7570 7065 7220 616e 6420 7365  .Td<upper and se
-000054b0: 6c66 2e6d 6f64 656c 735b 695d 2e54 643e  lf.models[i].Td>
-000054c0: 6c6f 7765 723a 0a20 2020 2020 2020 2020  lower:.         
+00005450: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00005460: 6f74 206e 702e 6973 6e61 6e28 6c6f 7765  ot np.isnan(lowe
+00005470: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005490: 2020 2020 6966 2073 656c 662e 6d6f 6465      if self.mode
+000054a0: 6c73 5b69 5d2e 5464 3c75 7070 6572 2061  ls[i].Td<upper a
+000054b0: 6e64 2073 656c 662e 6d6f 6465 6c73 5b69  nd self.models[i
+000054c0: 5d2e 5464 3e6c 6f77 6572 3a0a 2020 2020  ].Td>lower:.    
 000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054e0: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
-000054f0: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
-00005500: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
-00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054f0: 7265 745f 6461 7461 2e61 6464 5f6d 6f64  ret_data.add_mod
+00005500: 656c 2873 656c 662e 6d6f 6465 6c73 5b69  el(self.models[i
+00005510: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00005520: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00005530: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
 00005540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005550: 6966 2073 656c 662e 6d6f 6465 6c73 5b69  if self.models[i
-00005560: 5d2e 5464 3d3d 7570 7065 723a 0a20 2020  ].Td==upper:.   
-00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005550: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
+00005560: 656c 735b 695d 2e54 643d 3d75 7070 6572  els[i].Td==upper
+00005570: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005590: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
-000055a0: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
-000055b0: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-000055c0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-000055d0: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
-000055e0: 2c6c 6973 7429 3a0a 2020 2020 2020 2020  ,list):.        
+00005590: 2020 2020 2020 7265 745f 6461 7461 2e61        ret_data.a
+000055a0: 6464 5f6d 6f64 656c 2873 656c 662e 6d6f  dd_model(self.mo
+000055b0: 6465 6c73 5b69 5d29 0a20 2020 2020 2020  dels[i]).       
+000055c0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+000055d0: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
+000055e0: 2e73 746f 702c 6c69 7374 293a 0a20 2020  .stop,list):.   
 000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005600: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00005610: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005630: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00005640: 662e 6d6f 6465 6c73 5b69 5d2e 5464 2069  f.models[i].Td i
-00005650: 6e20 6172 672e 7374 6f70 3a0a 2020 2020  n arg.stop:.    
-00005660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005670: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
-00005680: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
-00005690: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
-000056a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000056b0: 6c69 6620 6172 672e 7374 6172 743d 3d27  lif arg.start=='
-000056c0: 7370 6563 6965 735f 696e 6465 7827 3a0a  species_index':.
-000056d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056e0: 2020 2020 7365 6c5f 7370 6563 6965 735f      sel_species_
-000056f0: 6e75 6d62 6572 3d5b 5d0a 2020 2020 2020  number=[].      
-00005700: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005710: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-00005720: 7374 6f70 2c69 6e74 293a 0a20 2020 2020  stop,int):.     
+00005600: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00005610: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
+00005620: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00005630: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005640: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
+00005650: 2e54 6420 696e 2061 7267 2e73 746f 703a  .Td in arg.stop:
+00005660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005680: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
+00005690: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
+000056a0: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+000056b0: 2020 2020 656c 6966 2061 7267 2e73 7461      elif arg.sta
+000056c0: 7274 3d3d 2773 7065 6369 6573 5f69 6e64  rt=='species_ind
+000056d0: 6578 273a 0a20 2020 2020 2020 2020 2020  ex':.           
+000056e0: 2020 2020 2020 2020 2073 656c 5f73 7065           sel_spe
+000056f0: 6369 6573 5f6e 756d 6265 723d 5b5d 0a20  cies_number=[]. 
+00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005710: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00005720: 2861 7267 2e73 746f 702c 696e 7429 3a0a  (arg.stop,int):.
 00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00005750: 2861 7267 2e73 7465 702c 696e 7429 3a0a  (arg.step,int):.
-00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005770: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00005780: 6920 696e 2072 616e 6765 2861 7267 2e73  i in range(arg.s
-00005790: 746f 702c 6172 672e 7374 6570 293a 0a20  top,arg.step):. 
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000057c0: 656c 5f73 7065 6369 6573 5f6e 756d 6265  el_species_numbe
-000057d0: 722e 6170 7065 6e64 2869 290a 2020 2020  r.append(i).    
-000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00005740: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00005750: 7461 6e63 6528 6172 672e 7374 6570 2c69  tance(arg.step,i
+00005760: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005780: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00005790: 6172 672e 7374 6f70 2c61 7267 2e73 7465  arg.stop,arg.ste
+000057a0: 7029 3a0a 2020 2020 2020 2020 2020 2020  p):.            
+000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057c0: 2020 2020 7365 6c5f 7370 6563 6965 735f      sel_species_
+000057d0: 6e75 6d62 6572 2e61 7070 656e 6428 6929  number.append(i)
+000057e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000057f0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005810: 2020 2020 2020 7365 6c5f 7370 6563 6965        sel_specie
-00005820: 735f 6e75 6d62 6572 2e61 7070 656e 6428  s_number.append(
-00005830: 6172 672e 7374 6f70 290a 2020 2020 2020  arg.stop).      
-00005840: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00005850: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
-00005860: 672e 7374 6f70 2c6c 6973 7429 3a0a 2020  g.stop,list):.  
-00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005880: 2020 2020 2020 2020 2020 7365 6c5f 7370            sel_sp
-00005890: 6563 6965 735f 6e75 6d62 6572 3d61 7267  ecies_number=arg
-000058a0: 2e73 746f 700a 2020 2020 2020 2020 2020  .stop.          
-000058b0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-000058c0: 2873 656c 5f73 7065 6369 6573 5f6e 756d  (sel_species_num
-000058d0: 6265 7229 3e30 3a0a 2020 2020 2020 2020  ber)>0:.        
+00005810: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
+00005820: 7065 6369 6573 5f6e 756d 6265 722e 6170  pecies_number.ap
+00005830: 7065 6e64 2861 7267 2e73 746f 7029 0a20  pend(arg.stop). 
+00005840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005850: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00005860: 6365 2861 7267 2e73 746f 702c 6c69 7374  ce(arg.stop,list
+00005870: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00005880: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005890: 656c 5f73 7065 6369 6573 5f6e 756d 6265  el_species_numbe
+000058a0: 723d 6172 672e 7374 6f70 0a20 2020 2020  r=arg.stop.     
+000058b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000058c0: 6620 6c65 6e28 7365 6c5f 7370 6563 6965  f len(sel_specie
+000058d0: 735f 6e75 6d62 6572 293e 303a 0a20 2020  s_number)>0:.   
 000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058f0: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00005900: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005920: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00005930: 662e 6d6f 6465 6c73 5b69 5d2e 7370 6563  f.models[i].spec
-00005940: 6965 735f 696e 6465 7820 696e 2073 656c  ies_index in sel
-00005950: 5f73 7065 6369 6573 5f6e 756d 6265 723a  _species_number:
-00005960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000058f0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00005900: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
+00005910: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00005920: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005930: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
+00005940: 2e73 7065 6369 6573 5f69 6e64 6578 2069  .species_index i
+00005950: 6e20 7365 6c5f 7370 6563 6965 735f 6e75  n sel_species_nu
+00005960: 6d62 6572 3a0a 2020 2020 2020 2020 2020  mber:.          
 00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005980: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
-00005990: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
-000059a0: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-000059b0: 2020 2020 656c 6966 2061 7267 2e73 7461      elif arg.sta
-000059c0: 7274 3d3d 2761 6275 6e64 616e 6365 273a  rt=='abundance':
-000059d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000059e0: 2020 2020 2075 7070 6572 3d6e 702e 6e61       upper=np.na
-000059f0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00005a00: 2020 2020 2020 6c6f 7765 723d 6e70 2e6e        lower=np.n
-00005a10: 616e 0a20 2020 2020 2020 2020 2020 2020  an.             
-00005a20: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00005a30: 616e 6365 2861 7267 2e73 746f 702c 666c  ance(arg.stop,fl
-00005a40: 6f61 7429 206f 7220 6973 696e 7374 616e  oat) or isinstan
-00005a50: 6365 2861 7267 2e73 746f 702c 696e 7429  ce(arg.stop,int)
-00005a60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005a70: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00005a80: 6e73 7461 6e63 6528 6172 672e 7374 6570  nstance(arg.step
-00005a90: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
-00005aa0: 7461 6e63 6528 6172 672e 7374 6570 2c69  tance(arg.step,i
-00005ab0: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+00005980: 2020 2020 2020 7265 745f 6461 7461 2e61        ret_data.a
+00005990: 6464 5f6d 6f64 656c 2873 656c 662e 6d6f  dd_model(self.mo
+000059a0: 6465 6c73 5b69 5d29 0a20 2020 2020 2020  dels[i]).       
+000059b0: 2020 2020 2020 2020 2065 6c69 6620 6172           elif ar
+000059c0: 672e 7374 6172 743d 3d27 6162 756e 6461  g.start=='abunda
+000059d0: 6e63 6527 3a0a 2020 2020 2020 2020 2020  nce':.          
+000059e0: 2020 2020 2020 2020 2020 7570 7065 723d            upper=
+000059f0: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
+00005a00: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
+00005a10: 3d6e 702e 6e61 6e0a 2020 2020 2020 2020  =np.nan.        
+00005a20: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00005a30: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+00005a40: 6f70 2c66 6c6f 6174 2920 6f72 2069 7369  op,float) or isi
+00005a50: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
+00005a60: 2c69 6e74 293a 0a20 2020 2020 2020 2020  ,int):.         
+00005a70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005a80: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
+00005a90: 2e73 7465 702c 666c 6f61 7429 206f 7220  .step,float) or 
+00005aa0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00005ab0: 7465 702c 696e 7429 3a0a 2020 2020 2020  tep,int):.      
 00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ad0: 206c 6f77 6572 2c75 7070 6572 3d61 7267   lower,upper=arg
-00005ae0: 2e73 746f 702c 6172 672e 7374 6570 0a20  .stop,arg.step. 
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b20: 2020 2020 2020 2020 2075 7070 6572 3d61           upper=a
-00005b30: 7267 2e73 746f 700a 2020 2020 2020 2020  rg.stop.        
+00005ad0: 2020 2020 2020 6c6f 7765 722c 7570 7065        lower,uppe
+00005ae0: 723d 6172 672e 7374 6f70 2c61 7267 2e73  r=arg.stop,arg.s
+00005af0: 7465 700a 2020 2020 2020 2020 2020 2020  tep.            
+00005b00: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00005b10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005b20: 2020 2020 2020 2020 2020 2020 2020 7570                up
+00005b30: 7065 723d 6172 672e 7374 6f70 0a20 2020  per=arg.stop.   
 00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b50: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00005b60: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b80: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00005b90: 206e 702e 6973 6e61 6e28 6c6f 7765 7229   np.isnan(lower)
-00005ba0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005b50: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00005b60: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
+00005b70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00005b80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005b90: 6620 6e6f 7420 6e70 2e69 736e 616e 286c  f not np.isnan(l
+00005ba0: 6f77 6572 293a 0a20 2020 2020 2020 2020  ower):.         
 00005bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bc0: 2020 6966 2073 656c 662e 6d6f 6465 6c73    if self.models
-00005bd0: 5b69 5d2e 6162 756e 6461 6e63 653c 7570  [i].abundance<up
-00005be0: 7065 7220 616e 6420 7365 6c66 2e6d 6f64  per and self.mod
-00005bf0: 656c 735b 695d 2e61 6275 6e64 616e 6365  els[i].abundance
-00005c00: 3e6c 6f77 6572 3a0a 2020 2020 2020 2020  >lower:.        
+00005bc0: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00005bd0: 6f64 656c 735b 695d 2e61 6275 6e64 616e  odels[i].abundan
+00005be0: 6365 3c75 7070 6572 2061 6e64 2073 656c  ce<upper and sel
+00005bf0: 662e 6d6f 6465 6c73 5b69 5d2e 6162 756e  f.models[i].abun
+00005c00: 6461 6e63 653e 6c6f 7765 723a 0a20 2020  dance>lower:.   
 00005c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c20: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
-00005c30: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
-00005c40: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
-00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c60: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00005c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c30: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
+00005c40: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
+00005c50: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
 00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c90: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
-00005ca0: 695d 2e61 6275 6e64 616e 6365 3d3d 7570  i].abundance==up
-00005cb0: 7065 723a 0a20 2020 2020 2020 2020 2020  per:.           
+00005c90: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
+00005ca0: 6465 6c73 5b69 5d2e 6162 756e 6461 6e63  dels[i].abundanc
+00005cb0: 653d 3d75 7070 6572 3a0a 2020 2020 2020  e==upper:.      
 00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cd0: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
-00005ce0: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
-00005cf0: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-00005d20: 6172 672e 7374 6f70 2c6c 6973 7429 3a0a  arg.stop,list):.
-00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d40: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00005d50: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00005d60: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+00005cd0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00005ce0: 745f 6461 7461 2e61 6464 5f6d 6f64 656c  t_data.add_model
+00005cf0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d29  (self.models[i])
+00005d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d10: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00005d20: 616e 6365 2861 7267 2e73 746f 702c 6c69  ance(arg.stop,li
+00005d30: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00005d40: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00005d50: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+00005d60: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
 00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d80: 2020 6966 2073 656c 662e 6d6f 6465 6c73    if self.models
-00005d90: 5b69 5d2e 6162 756e 6461 6e63 6520 696e  [i].abundance in
-00005da0: 2061 7267 2e73 746f 703a 0a20 2020 2020   arg.stop:.     
+00005d80: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00005d90: 6f64 656c 735b 695d 2e61 6275 6e64 616e  odels[i].abundan
+00005da0: 6365 2069 6e20 6172 672e 7374 6f70 3a0a  ce in arg.stop:.
 00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
-00005dd0: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
-00005de0: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
-00005df0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00005e00: 6966 2061 7267 2e73 7461 7274 3d3d 2764  if arg.start=='d
-00005e10: 7627 3a0a 2020 2020 2020 2020 2020 2020  v':.            
-00005e20: 2020 2020 2020 2020 7570 7065 723d 6e70          upper=np
-00005e30: 2e6e 616e 0a20 2020 2020 2020 2020 2020  .nan.           
-00005e40: 2020 2020 2020 2020 206c 6f77 6572 3d6e           lower=n
-00005e50: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
-00005e60: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00005e70: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
-00005e80: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
-00005e90: 7461 6e63 6528 6172 672e 7374 6f70 2c69  tance(arg.stop,i
-00005ea0: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-00005eb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005ec0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
-00005ed0: 7465 702c 666c 6f61 7429 206f 7220 6973  tep,float) or is
-00005ee0: 696e 7374 616e 6365 2861 7267 2e73 7465  instance(arg.ste
-00005ef0: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
+00005dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005dd0: 7265 745f 6461 7461 2e61 6464 5f6d 6f64  ret_data.add_mod
+00005de0: 656c 2873 656c 662e 6d6f 6465 6c73 5b69  el(self.models[i
+00005df0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00005e00: 2020 2065 6c69 6620 6172 672e 7374 6172     elif arg.star
+00005e10: 743d 3d27 6476 273a 0a20 2020 2020 2020  t=='dv':.       
+00005e20: 2020 2020 2020 2020 2020 2020 2075 7070               upp
+00005e30: 6572 3d6e 702e 6e61 6e0a 2020 2020 2020  er=np.nan.      
+00005e40: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00005e50: 7765 723d 6e70 2e6e 616e 0a20 2020 2020  wer=np.nan.     
+00005e60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005e70: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
+00005e80: 2e73 746f 702c 666c 6f61 7429 206f 7220  .stop,float) or 
+00005e90: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00005ea0: 746f 702c 696e 7429 3a0a 2020 2020 2020  top,int):.      
+00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ec0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00005ed0: 6172 672e 7374 6570 2c66 6c6f 6174 2920  arg.step,float) 
+00005ee0: 6f72 2069 7369 6e73 7461 6e63 6528 6172  or isinstance(ar
+00005ef0: 672e 7374 6570 2c69 6e74 293a 0a20 2020  g.step,int):.   
 00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f10: 2020 2020 6c6f 7765 722c 7570 7065 723d      lower,upper=
-00005f20: 6172 672e 7374 6f70 2c61 7267 2e73 7465  arg.stop,arg.ste
-00005f30: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-00005f40: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f60: 2020 2020 2020 2020 2020 2020 7570 7065              uppe
-00005f70: 723d 6172 672e 7374 6f70 0a20 2020 2020  r=arg.stop.     
+00005f10: 2020 2020 2020 2020 206c 6f77 6572 2c75           lower,u
+00005f20: 7070 6572 3d61 7267 2e73 746f 702c 6172  pper=arg.stop,ar
+00005f30: 672e 7374 6570 0a20 2020 2020 2020 2020  g.step.         
+00005f40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00005f50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f70: 2075 7070 6572 3d61 7267 2e73 746f 700a   upper=arg.stop.
 00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00005fa0: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-00005fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005fc0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005fd0: 6e6f 7420 6e70 2e69 736e 616e 286c 6f77  not np.isnan(low
-00005fe0: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
+00005f90: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00005fa0: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
+00005fb0: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fd0: 2020 6966 206e 6f74 206e 702e 6973 6e61    if not np.isna
+00005fe0: 6e28 6c6f 7765 7229 3a0a 2020 2020 2020  n(lower):.      
 00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006000: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
-00006010: 656c 735b 695d 2e64 763c 7570 7065 7220  els[i].dv<upper 
-00006020: 616e 6420 7365 6c66 2e6d 6f64 656c 735b  and self.models[
-00006030: 695d 2e64 763e 6c6f 7765 723a 0a20 2020  i].dv>lower:.   
-00006040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006000: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00006010: 662e 6d6f 6465 6c73 5b69 5d2e 6476 3c75  f.models[i].dv<u
+00006020: 7070 6572 2061 6e64 2073 656c 662e 6d6f  pper and self.mo
+00006030: 6465 6c73 5b69 5d2e 6476 3e6c 6f77 6572  dels[i].dv>lower
+00006040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 00006050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006060: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
-00006070: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
-00006080: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+00006060: 2020 2020 2020 7265 745f 6461 7461 2e61        ret_data.a
+00006070: 6464 5f6d 6f64 656c 2873 656c 662e 6d6f  dd_model(self.mo
+00006080: 6465 6c73 5b69 5d29 0a20 2020 2020 2020  dels[i]).       
 00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000060a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
 000060b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060c0: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
-000060d0: 6465 6c73 5b69 5d2e 6476 3d3d 7570 7065  dels[i].dv==uppe
-000060e0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+000060c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000060d0: 6c66 2e6d 6f64 656c 735b 695d 2e64 763d  lf.models[i].dv=
+000060e0: 3d75 7070 6572 3a0a 2020 2020 2020 2020  =upper:.        
 000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006100: 2020 2020 2020 2072 6574 5f64 6174 612e         ret_data.
-00006110: 6164 645f 6d6f 6465 6c28 7365 6c66 2e6d  add_model(self.m
-00006120: 6f64 656c 735b 695d 290a 2020 2020 2020  odels[i]).      
-00006130: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00006140: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
-00006150: 672e 7374 6f70 2c6c 6973 7429 3a0a 2020  g.stop,list):.  
-00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006170: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00006180: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
-00006190: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00006100: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
+00006110: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
+00006120: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
+00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006140: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00006150: 6365 2861 7267 2e73 746f 702c 6c69 7374  ce(arg.stop,list
+00006160: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00006170: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00006180: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+00006190: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
 000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061b0: 6966 2073 656c 662e 6d6f 6465 6c73 5b69  if self.models[i
-000061c0: 5d2e 6476 2069 6e20 6172 672e 7374 6f70  ].dv in arg.stop
-000061d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000061b0: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
+000061c0: 656c 735b 695d 2e64 7620 696e 2061 7267  els[i].dv in arg
+000061d0: 2e73 746f 703a 0a20 2020 2020 2020 2020  .stop:.         
 000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061f0: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
-00006200: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
-00006210: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
-00006220: 2020 2020 2065 6c69 6620 6172 672e 7374       elif arg.st
-00006230: 6172 743d 3d27 6e6c 6576 656c 7327 3a0a  art=='nlevels':.
-00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006250: 2020 2020 7365 6c5f 7370 6563 6965 735f      sel_species_
-00006260: 6e75 6d62 6572 3d5b 5d0a 2020 2020 2020  number=[].      
-00006270: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00006280: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
-00006290: 7374 6f70 2c69 6e74 293a 0a20 2020 2020  stop,int):.     
+000061f0: 2020 2020 2020 2072 6574 5f64 6174 612e         ret_data.
+00006200: 6164 645f 6d6f 6465 6c28 7365 6c66 2e6d  add_model(self.m
+00006210: 6f64 656c 735b 695d 290a 2020 2020 2020  odels[i]).      
+00006220: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
+00006230: 7267 2e73 7461 7274 3d3d 276e 6c65 7665  rg.start=='nleve
+00006240: 6c73 273a 0a20 2020 2020 2020 2020 2020  ls':.           
+00006250: 2020 2020 2020 2020 2073 656c 5f73 7065           sel_spe
+00006260: 6369 6573 5f6e 756d 6265 723d 5b5d 0a20  cies_number=[]. 
+00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006280: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00006290: 2861 7267 2e73 746f 702c 696e 7429 3a0a  (arg.stop,int):.
 000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000062c0: 2861 7267 2e73 7465 702c 696e 7429 3a0a  (arg.step,int):.
-000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000062f0: 6920 696e 2072 616e 6765 2861 7267 2e73  i in range(arg.s
-00006300: 746f 702c 6172 672e 7374 6570 293a 0a20  top,arg.step):. 
-00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006320: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006330: 656c 5f73 7065 6369 6573 5f6e 756d 6265  el_species_numbe
-00006340: 722e 6170 7065 6e64 2869 290a 2020 2020  r.append(i).    
-00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006360: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000062b0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+000062c0: 7461 6e63 6528 6172 672e 7374 6570 2c69  tance(arg.step,i
+000062d0: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062f0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00006300: 6172 672e 7374 6f70 2c61 7267 2e73 7465  arg.stop,arg.ste
+00006310: 7029 3a0a 2020 2020 2020 2020 2020 2020  p):.            
+00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006330: 2020 2020 7365 6c5f 7370 6563 6965 735f      sel_species_
+00006340: 6e75 6d62 6572 2e61 7070 656e 6428 6929  number.append(i)
+00006350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006360: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006380: 2020 2020 2020 7365 6c5f 7370 6563 6965        sel_specie
-00006390: 735f 6e75 6d62 6572 2e61 7070 656e 6428  s_number.append(
-000063a0: 6172 672e 7374 6f70 290a 2020 2020 2020  arg.stop).      
-000063b0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000063c0: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
-000063d0: 672e 7374 6f70 2c6c 6973 7429 3a0a 2020  g.stop,list):.  
-000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063f0: 2020 2020 2020 2020 2020 7365 6c5f 7370            sel_sp
-00006400: 6563 6965 735f 6e75 6d62 6572 3d61 7267  ecies_number=arg
-00006410: 2e73 746f 700a 2020 2020 2020 2020 2020  .stop.          
-00006420: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00006430: 2873 656c 5f73 7065 6369 6573 5f6e 756d  (sel_species_num
-00006440: 6265 7229 3e30 3a0a 2020 2020 2020 2020  ber)>0:.        
+00006380: 2020 2020 2020 2020 2020 2073 656c 5f73             sel_s
+00006390: 7065 6369 6573 5f6e 756d 6265 722e 6170  pecies_number.ap
+000063a0: 7065 6e64 2861 7267 2e73 746f 7029 0a20  pend(arg.stop). 
+000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063c0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+000063d0: 6365 2861 7267 2e73 746f 702c 6c69 7374  ce(arg.stop,list
+000063e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000063f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006400: 656c 5f73 7065 6369 6573 5f6e 756d 6265  el_species_numbe
+00006410: 723d 6172 672e 7374 6f70 0a20 2020 2020  r=arg.stop.     
+00006420: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00006430: 6620 6c65 6e28 7365 6c5f 7370 6563 6965  f len(sel_specie
+00006440: 735f 6e75 6d62 6572 293e 303a 0a20 2020  s_number)>0:.   
 00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00006470: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006490: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000064a0: 662e 6d6f 6465 6c73 5b69 5d2e 6e6c 6576  f.models[i].nlev
-000064b0: 656c 7320 696e 2073 656c 5f73 7065 6369  els in sel_speci
-000064c0: 6573 5f6e 756d 6265 723a 0a20 2020 2020  es_number:.     
+00006460: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00006470: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
+00006480: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00006490: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000064a0: 6620 7365 6c66 2e6d 6f64 656c 735b 695d  f self.models[i]
+000064b0: 2e6e 6c65 7665 6c73 2069 6e20 7365 6c5f  .nlevels in sel_
+000064c0: 7370 6563 6965 735f 6e75 6d62 6572 3a0a  species_number:.
 000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064e0: 2020 2020 2020 2020 2020 2072 6574 5f64             ret_d
-000064f0: 6174 612e 6164 645f 6d6f 6465 6c28 7365  ata.add_model(se
-00006500: 6c66 2e6d 6f64 656c 735b 695d 290a 2020  lf.models[i]).  
-00006510: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00006520: 6966 2061 7267 2e73 7461 7274 3d3d 276e  if arg.start=='n
-00006530: 6c69 6e65 7327 3a0a 2020 2020 2020 2020  lines':.        
-00006540: 2020 2020 2020 2020 2020 2020 7365 6c5f              sel_
-00006550: 7370 6563 6965 735f 6e75 6d62 6572 3d5b  species_number=[
-00006560: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00006570: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00006580: 6e63 6528 6172 672e 7374 6f70 2c69 6e74  nce(arg.stop,int
-00006590: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000065a0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-000065b0: 696e 7374 616e 6365 2861 7267 2e73 7465  instance(arg.ste
-000065c0: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
+000064e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064f0: 7265 745f 6461 7461 2e61 6464 5f6d 6f64  ret_data.add_mod
+00006500: 656c 2873 656c 662e 6d6f 6465 6c73 5b69  el(self.models[i
+00006510: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00006520: 2020 2065 6c69 6620 6172 672e 7374 6172     elif arg.star
+00006530: 743d 3d27 6e6c 696e 6573 273a 0a20 2020  t=='nlines':.   
+00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006550: 2073 656c 5f73 7065 6369 6573 5f6e 756d   sel_species_num
+00006560: 6265 723d 5b5d 0a20 2020 2020 2020 2020  ber=[].         
+00006570: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00006580: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
+00006590: 702c 696e 7429 3a0a 2020 2020 2020 2020  p,int):.        
+000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065b0: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
+000065c0: 672e 7374 6570 2c69 6e74 293a 0a20 2020  g.step,int):.   
 000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065e0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-000065f0: 6765 2861 7267 2e73 746f 702c 6172 672e  ge(arg.stop,arg.
-00006600: 7374 6570 293a 0a20 2020 2020 2020 2020  step):.         
+000065e0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+000065f0: 6e20 7261 6e67 6528 6172 672e 7374 6f70  n range(arg.stop
+00006600: 2c61 7267 2e73 7465 7029 3a0a 2020 2020  ,arg.step):.    
 00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006620: 2020 2020 2020 2073 656c 5f73 7065 6369         sel_speci
-00006630: 6573 5f6e 756d 6265 722e 6170 7065 6e64  es_number.append
-00006640: 2869 290a 2020 2020 2020 2020 2020 2020  (i).            
-00006650: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00006660: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006670: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006680: 6c5f 7370 6563 6965 735f 6e75 6d62 6572  l_species_number
-00006690: 2e61 7070 656e 6428 6172 672e 7374 6f70  .append(arg.stop
-000066a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000066b0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-000066c0: 7461 6e63 6528 6172 672e 7374 6f70 2c6c  tance(arg.stop,l
-000066d0: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
+00006620: 2020 2020 2020 2020 2020 2020 7365 6c5f              sel_
+00006630: 7370 6563 6965 735f 6e75 6d62 6572 2e61  species_number.a
+00006640: 7070 656e 6428 6929 0a20 2020 2020 2020  ppend(i).       
+00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006660: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006680: 2020 2073 656c 5f73 7065 6369 6573 5f6e     sel_species_n
+00006690: 756d 6265 722e 6170 7065 6e64 2861 7267  umber.append(arg
+000066a0: 2e73 746f 7029 0a20 2020 2020 2020 2020  .stop).         
+000066b0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000066c0: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+000066d0: 746f 702c 6c69 7374 293a 0a20 2020 2020  top,list):.     
 000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066f0: 2020 7365 6c5f 7370 6563 6965 735f 6e75    sel_species_nu
-00006700: 6d62 6572 3d61 7267 2e73 746f 700a 2020  mber=arg.stop.  
-00006710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006720: 2020 6966 206c 656e 2873 656c 5f73 7065    if len(sel_spe
-00006730: 6369 6573 5f6e 756d 6265 7229 3e30 3a0a  cies_number)>0:.
-00006740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006750: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00006760: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00006770: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+000066f0: 2020 2020 2020 2073 656c 5f73 7065 6369         sel_speci
+00006700: 6573 5f6e 756d 6265 723d 6172 672e 7374  es_number=arg.st
+00006710: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
+00006720: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
+00006730: 6c5f 7370 6563 6965 735f 6e75 6d62 6572  l_species_number
+00006740: 293e 303a 0a20 2020 2020 2020 2020 2020  )>0:.           
+00006750: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00006760: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+00006770: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
 00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006790: 2020 6966 2073 656c 662e 6d6f 6465 6c73    if self.models
-000067a0: 5b69 5d2e 6e6c 696e 6573 2069 6e20 7365  [i].nlines in se
-000067b0: 6c5f 7370 6563 6965 735f 6e75 6d62 6572  l_species_number
-000067c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006790: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+000067a0: 6f64 656c 735b 695d 2e6e 6c69 6e65 7320  odels[i].nlines 
+000067b0: 696e 2073 656c 5f73 7065 6369 6573 5f6e  in sel_species_n
+000067c0: 756d 6265 723a 0a20 2020 2020 2020 2020  umber:.         
 000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067e0: 2020 7265 745f 6461 7461 2e61 6464 5f6d    ret_data.add_m
-000067f0: 6f64 656c 2873 656c 662e 6d6f 6465 6c73  odel(self.models
-00006800: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
-00006810: 2020 2020 2065 6c69 6620 6172 672e 7374       elif arg.st
-00006820: 6172 743d 3d27 636f 6e76 5479 7065 273a  art=='convType':
-00006830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006840: 2020 2020 2073 656c 5f73 7065 6369 6573       sel_species
-00006850: 5f6e 756d 6265 723d 5b5d 0a20 2020 2020  _number=[].     
-00006860: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00006870: 6620 6973 696e 7374 616e 6365 2861 7267  f isinstance(arg
-00006880: 2e73 746f 702c 696e 7429 3a0a 2020 2020  .stop,int):.    
-00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068a0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000068b0: 6528 6172 672e 7374 6570 2c69 6e74 293a  e(arg.step,int):
-000068c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000068d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000068e0: 5f73 7065 6369 6573 5f6e 756d 6265 723d  _species_number=
-000068f0: 5b61 7267 2e73 746f 702c 6172 672e 7374  [arg.stop,arg.st
-00006900: 6570 5d0a 2020 2020 2020 2020 2020 2020  ep].            
-00006910: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00006920: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006930: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006940: 6c5f 7370 6563 6965 735f 6e75 6d62 6572  l_species_number
-00006950: 2e61 7070 656e 6428 6172 672e 7374 6f70  .append(arg.stop
-00006960: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00006970: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00006980: 7461 6e63 6528 6172 672e 7374 6f70 2c6c  tance(arg.stop,l
-00006990: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
+000067e0: 2020 2020 2020 2072 6574 5f64 6174 612e         ret_data.
+000067f0: 6164 645f 6d6f 6465 6c28 7365 6c66 2e6d  add_model(self.m
+00006800: 6f64 656c 735b 695d 290a 2020 2020 2020  odels[i]).      
+00006810: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
+00006820: 7267 2e73 7461 7274 3d3d 2763 6f6e 7654  rg.start=='convT
+00006830: 7970 6527 3a0a 2020 2020 2020 2020 2020  ype':.          
+00006840: 2020 2020 2020 2020 2020 7365 6c5f 7370            sel_sp
+00006850: 6563 6965 735f 6e75 6d62 6572 3d5b 5d0a  ecies_number=[].
+00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006870: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00006880: 6528 6172 672e 7374 6f70 2c69 6e74 293a  e(arg.stop,int):
+00006890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000068a0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+000068b0: 7374 616e 6365 2861 7267 2e73 7465 702c  stance(arg.step,
+000068c0: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068e0: 2020 7365 6c5f 7370 6563 6965 735f 6e75    sel_species_nu
+000068f0: 6d62 6572 3d5b 6172 672e 7374 6f70 2c61  mber=[arg.stop,a
+00006900: 7267 2e73 7465 705d 0a20 2020 2020 2020  rg.step].       
+00006910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006920: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006940: 2020 2073 656c 5f73 7065 6369 6573 5f6e     sel_species_n
+00006950: 756d 6265 722e 6170 7065 6e64 2861 7267  umber.append(arg
+00006960: 2e73 746f 7029 0a20 2020 2020 2020 2020  .stop).         
+00006970: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00006980: 6973 696e 7374 616e 6365 2861 7267 2e73  isinstance(arg.s
+00006990: 746f 702c 6c69 7374 293a 0a20 2020 2020  top,list):.     
 000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069b0: 2020 7365 6c5f 7370 6563 6965 735f 6e75    sel_species_nu
-000069c0: 6d62 6572 3d61 7267 2e73 746f 700a 2020  mber=arg.stop.  
-000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069e0: 2020 6966 206c 656e 2873 656c 5f73 7065    if len(sel_spe
-000069f0: 6369 6573 5f6e 756d 6265 7229 3e30 3a0a  cies_number)>0:.
-00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a10: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00006a20: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00006a30: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+000069b0: 2020 2020 2020 2073 656c 5f73 7065 6369         sel_speci
+000069c0: 6573 5f6e 756d 6265 723d 6172 672e 7374  es_number=arg.st
+000069d0: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
+000069e0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
+000069f0: 6c5f 7370 6563 6965 735f 6e75 6d62 6572  l_species_number
+00006a00: 293e 303a 0a20 2020 2020 2020 2020 2020  )>0:.           
+00006a10: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00006a20: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+00006a30: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
 00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a50: 2020 6966 2073 656c 662e 6d6f 6465 6c73    if self.models
-00006a60: 5b69 5d2e 636f 6e76 5479 7065 2069 6e20  [i].convType in 
-00006a70: 7365 6c5f 7370 6563 6965 735f 6e75 6d62  sel_species_numb
-00006a80: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+00006a50: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00006a60: 6f64 656c 735b 695d 2e63 6f6e 7654 7970  odels[i].convTyp
+00006a70: 6520 696e 2073 656c 5f73 7065 6369 6573  e in sel_species
+00006a80: 5f6e 756d 6265 723a 0a20 2020 2020 2020  _number:.       
 00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006aa0: 2020 2020 7265 745f 6461 7461 2e61 6464      ret_data.add
-00006ab0: 5f6d 6f64 656c 2873 656c 662e 6d6f 6465  _model(self.mode
-00006ac0: 6c73 5b69 5d29 0a20 2020 2020 2020 2020  ls[i]).         
-00006ad0: 2020 2020 2020 2065 6c69 6620 6172 672e         elif arg.
-00006ae0: 7374 6172 743d 3d27 636f 6e76 5227 3a0a  start=='convR':.
-00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b00: 2020 2020 7570 7065 723d 6e70 2e6e 616e      upper=np.nan
-00006b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006b20: 2020 2020 206c 6f77 6572 3d6e 702e 6e61       lower=np.na
-00006b30: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00006b40: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00006b50: 6e63 6528 6172 672e 7374 6f70 2c66 6c6f  nce(arg.stop,flo
-00006b60: 6174 2920 6f72 2069 7369 6e73 7461 6e63  at) or isinstanc
-00006b70: 6528 6172 672e 7374 6f70 2c69 6e74 293a  e(arg.stop,int):
-00006b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006b90: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-00006ba0: 7374 616e 6365 2861 7267 2e73 7465 702c  stance(arg.step,
-00006bb0: 666c 6f61 7429 206f 7220 6973 696e 7374  float) or isinst
-00006bc0: 616e 6365 2861 7267 2e73 7465 702c 696e  ance(arg.step,in
-00006bd0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00006aa0: 2020 2020 2020 2020 2072 6574 5f64 6174           ret_dat
+00006ab0: 612e 6164 645f 6d6f 6465 6c28 7365 6c66  a.add_model(self
+00006ac0: 2e6d 6f64 656c 735b 695d 290a 2020 2020  .models[i]).    
+00006ad0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00006ae0: 2061 7267 2e73 7461 7274 3d3d 2763 6f6e   arg.start=='con
+00006af0: 7652 273a 0a20 2020 2020 2020 2020 2020  vR':.           
+00006b00: 2020 2020 2020 2020 2075 7070 6572 3d6e           upper=n
+00006b10: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
+00006b20: 2020 2020 2020 2020 2020 6c6f 7765 723d            lower=
+00006b30: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
+00006b40: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00006b50: 696e 7374 616e 6365 2861 7267 2e73 746f  instance(arg.sto
+00006b60: 702c 666c 6f61 7429 206f 7220 6973 696e  p,float) or isin
+00006b70: 7374 616e 6365 2861 7267 2e73 746f 702c  stance(arg.stop,
+00006b80: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+00006b90: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00006ba0: 2069 7369 6e73 7461 6e63 6528 6172 672e   isinstance(arg.
+00006bb0: 7374 6570 2c66 6c6f 6174 2920 6f72 2069  step,float) or i
+00006bc0: 7369 6e73 7461 6e63 6528 6172 672e 7374  sinstance(arg.st
+00006bd0: 6570 2c69 6e74 293a 0a20 2020 2020 2020  ep,int):.       
 00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bf0: 6c6f 7765 722c 7570 7065 723d 6172 672e  lower,upper=arg.
-00006c00: 7374 6f70 2c61 7267 2e73 7465 700a 2020  stop,arg.step.  
-00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c40: 2020 2020 2020 2020 7570 7065 723d 6172          upper=ar
-00006c50: 672e 7374 6f70 0a20 2020 2020 2020 2020  g.stop.         
-00006c60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00006c70: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-00006c80: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-00006c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ca0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00006cb0: 6e70 2e69 736e 616e 286c 6f77 6572 293a  np.isnan(lower):
-00006cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006bf0: 2020 2020 206c 6f77 6572 2c75 7070 6572       lower,upper
+00006c00: 3d61 7267 2e73 746f 702c 6172 672e 7374  =arg.stop,arg.st
+00006c10: 6570 0a20 2020 2020 2020 2020 2020 2020  ep.             
+00006c20: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00006c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c40: 2020 2020 2020 2020 2020 2020 2075 7070               upp
+00006c50: 6572 3d61 7267 2e73 746f 700a 2020 2020  er=arg.stop.    
+00006c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c70: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00006c80: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+00006c90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006ca0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00006cb0: 206e 6f74 206e 702e 6973 6e61 6e28 6c6f   not np.isnan(lo
+00006cc0: 7765 7229 3a0a 2020 2020 2020 2020 2020  wer):.          
 00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 2069 6620 7365 6c66 2e6d 6f64 656c 735b   if self.models[
-00006cf0: 695d 2e63 6f6e 7652 3c75 7070 6572 2061  i].convR<upper a
-00006d00: 6e64 2073 656c 662e 6d6f 6465 6c73 5b69  nd self.models[i
-00006d10: 5d2e 636f 6e76 523e 6c6f 7765 723a 0a20  ].convR>lower:. 
-00006d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ce0: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
+00006cf0: 6465 6c73 5b69 5d2e 636f 6e76 523c 7570  dels[i].convR<up
+00006d00: 7065 7220 616e 6420 7365 6c66 2e6d 6f64  per and self.mod
+00006d10: 656c 735b 695d 2e63 6f6e 7652 3e6c 6f77  els[i].convR>low
+00006d20: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
 00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2072 6574 5f64 6174 612e 6164 645f     ret_data.add_
-00006d50: 6d6f 6465 6c28 7365 6c66 2e6d 6f64 656c  model(self.model
-00006d60: 735b 695d 290a 2020 2020 2020 2020 2020  s[i]).          
+00006d40: 2020 2020 2020 2020 7265 745f 6461 7461          ret_data
+00006d50: 2e61 6464 5f6d 6f64 656c 2873 656c 662e  .add_model(self.
+00006d60: 6d6f 6465 6c73 5b69 5d29 0a20 2020 2020  models[i]).     
 00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00006d80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
 00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006da0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00006db0: 6d6f 6465 6c73 5b69 5d2e 636f 6e76 523d  models[i].convR=
-00006dc0: 3d75 7070 6572 3a0a 2020 2020 2020 2020  =upper:.        
+00006da0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00006db0: 7365 6c66 2e6d 6f64 656c 735b 695d 2e63  self.models[i].c
+00006dc0: 6f6e 7652 3d3d 7570 7065 723a 0a20 2020  onvR==upper:.   
 00006dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006de0: 2020 2020 2020 2020 2020 2020 7265 745f              ret_
-00006df0: 6461 7461 2e61 6464 5f6d 6f64 656c 2873  data.add_model(s
-00006e00: 656c 662e 6d6f 6465 6c73 5b69 5d29 0a20  elf.models[i]). 
-00006e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e20: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00006e30: 6365 2861 7267 2e73 746f 702c 6c69 7374  ce(arg.stop,list
-00006e40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00006e50: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00006e60: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-00006e70: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+00006de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006df0: 2072 6574 5f64 6174 612e 6164 645f 6d6f   ret_data.add_mo
+00006e00: 6465 6c28 7365 6c66 2e6d 6f64 656c 735b  del(self.models[
+00006e10: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+00006e20: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+00006e30: 6e73 7461 6e63 6528 6172 672e 7374 6f70  nstance(arg.stop
+00006e40: 2c6c 6973 7429 3a0a 2020 2020 2020 2020  ,list):.        
+00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e60: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+00006e70: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
 00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e90: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
-00006ea0: 656c 735b 695d 2e63 6f6e 7652 2069 6e20  els[i].convR in 
-00006eb0: 6172 672e 7374 6f70 3a0a 2020 2020 2020  arg.stop:.      
+00006e90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00006ea0: 662e 6d6f 6465 6c73 5b69 5d2e 636f 6e76  f.models[i].conv
+00006eb0: 5220 696e 2061 7267 2e73 746f 703a 0a20  R in arg.stop:. 
 00006ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ed0: 2020 2020 2020 2020 2020 7265 745f 6461            ret_da
-00006ee0: 7461 2e61 6464 5f6d 6f64 656c 2873 656c  ta.add_model(sel
-00006ef0: 662e 6d6f 6465 6c73 5b69 5d29 0a20 2020  f.models[i]).   
-00006f00: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00006f10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00006f20: 2020 2020 2020 2072 6169 7365 204b 6579         raise Key
-00006f30: 4572 726f 7228 2755 6e72 6563 6f67 6e69  Error('Unrecogni
-00006f40: 7365 6420 7061 7261 6d65 7465 7220 666f  sed parameter fo
-00006f50: 7220 736c 6963 696e 6727 290a 2020 2020  r slicing').    
-00006f60: 2020 2020 7265 7475 726e 2072 6574 5f64      return ret_d
-00006f70: 6174 610a 0a20 2020 2064 6566 2063 6f6e  ata..    def con
-00006f80: 766f 6c76 6528 7365 6c66 2c66 7265 715f  volve(self,freq_
-00006f90: 6269 6e73 3d4e 6f6e 652c 523d 312c 6c61  bins=None,R=1,la
-00006fa0: 6d62 6461 5f30 3d31 2c6c 616d 6264 615f  mbda_0=1,lambda_
-00006fb0: 6e3d 312c 7672 3d31 3330 302c 4e4c 5445  n=1,vr=1300,NLTE
-00006fc0: 3d46 616c 7365 2c63 6f6e 765f 7479 7065  =False,conv_type
-00006fd0: 3d31 2c76 6572 626f 7365 3d54 7275 6529  =1,verbose=True)
-00006fe0: 3a0a 2020 2020 2020 2020 666f 7220 692c  :.        for i,
-00006ff0: 6420 696e 2065 6e75 6d65 7261 7465 2873  d in enumerate(s
-00007000: 656c 662e 6d6f 6465 6c73 293a 0a20 2020  elf.models):.   
-00007010: 2020 2020 2020 2020 2069 6620 7665 7262           if verb
-00007020: 6f73 653a 2070 7269 6e74 2827 5c6e 272c  ose: print('\n',
-00007030: 692b 312c 273b 204d 6f64 656c 206e 756d  i+1,'; Model num
-00007040: 6265 7220 272c 7365 6c66 2e6d 6f64 656c  ber ',self.model
-00007050: 735b 695d 2e6d 6f64 656c 5f6e 756d 6265  s[i].model_numbe
-00007060: 722c 273b 2053 7065 6369 6573 206e 756d  r,'; Species num
-00007070: 6265 7220 272c 7365 6c66 2e6d 6f64 656c  ber ',self.model
-00007080: 735b 695d 2e73 7065 6369 6573 5f6e 756d  s[i].species_num
-00007090: 6265 7229 0a20 2020 2020 2020 2020 2020  ber).           
-000070a0: 2064 2e63 6f6e 766f 6c76 6528 6672 6571   d.convolve(freq
-000070b0: 5f62 696e 733d 6672 6571 5f62 696e 732c  _bins=freq_bins,
-000070c0: 523d 522c 6c61 6d62 6461 5f30 3d6c 616d  R=R,lambda_0=lam
-000070d0: 6264 615f 302c 6c61 6d62 6461 5f6e 3d6c  bda_0,lambda_n=l
-000070e0: 616d 6264 615f 6e2c 7672 3d76 722c 4e4c  ambda_n,vr=vr,NL
-000070f0: 5445 3d4e 4c54 452c 636f 6e76 5f74 7970  TE=NLTE,conv_typ
-00007100: 653d 636f 6e76 5f74 7970 6529 0a0a 2020  e=conv_type)..  
-00007110: 2020 6465 6620 636f 6e76 6f6c 7665 5f6f    def convolve_o
-00007120: 7665 726c 6170 2873 656c 662c 523d 312c  verlap(self,R=1,
-00007130: 6c61 6d62 6461 5f30 3d31 2c6c 616d 6264  lambda_0=1,lambd
-00007140: 615f 6e3d 312c 7665 7262 6f73 653d 5472  a_n=1,verbose=Tr
-00007150: 7565 293a 0a20 2020 2020 2020 2066 6f72  ue):.        for
-00007160: 2069 2c64 2069 6e20 656e 756d 6572 6174   i,d in enumerat
-00007170: 6528 7365 6c66 2e6d 6f64 656c 7329 3a0a  e(self.models):.
-00007180: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00007190: 6572 626f 7365 3a20 7072 696e 7428 275c  erbose: print('\
-000071a0: 6e27 2c69 2b31 2c27 3b20 4d6f 6465 6c20  n',i+1,'; Model 
-000071b0: 6e75 6d62 6572 2027 2c73 656c 662e 6d6f  number ',self.mo
-000071c0: 6465 6c73 5b69 5d2e 6d6f 6465 6c5f 6e75  dels[i].model_nu
-000071d0: 6d62 6572 290a 2020 2020 2020 2020 2020  mber).          
-000071e0: 2020 642e 636f 6e76 6f6c 7665 5f6f 7665    d.convolve_ove
-000071f0: 726c 6170 2852 3d52 2c6c 616d 6264 615f  rlap(R=R,lambda_
-00007200: 303d 6c61 6d62 6461 5f30 2c6c 616d 6264  0=lambda_0,lambd
-00007210: 615f 6e3d 6c61 6d62 6461 5f6e 290a 0a0a  a_n=lambda_n)...
-00007220: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00007230: 2020 6465 6620 6e6d 6f64 656c 7328 7365    def nmodels(se
-00007240: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00007250: 662e 5f6e 6d6f 6465 6c73 3d6c 656e 2873  f._nmodels=len(s
-00007260: 656c 662e 6d6f 6465 6c73 290a 2020 2020  elf.models).    
-00007270: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00007280: 5f6e 6d6f 6465 6c73 0a0a 2020 2020 406e  _nmodels..    @n
-00007290: 6d6f 6465 6c73 2e73 6574 7465 720a 2020  models.setter.  
-000072a0: 2020 6465 6620 6e6d 6f64 656c 7328 7365    def nmodels(se
-000072b0: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
-000072c0: 2020 2073 656c 662e 5f6e 6d6f 6465 6c73     self._nmodels
-000072d0: 3d76 616c 7565 0a0a 2020 2020 4070 726f  =value..    @pro
-000072e0: 7065 7274 790a 2020 2020 6465 6620 7370  perty.    def sp
-000072f0: 6563 6965 735f 6e75 6d62 6572 2873 656c  ecies_number(sel
-00007300: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00007310: 656c 662e 6e6d 6f64 656c 733e 313a 0a20  elf.nmodels>1:. 
-00007320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007330: 5f73 7065 6369 6573 5f6e 756d 6265 723d  _species_number=
-00007340: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-00007350: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-00007360: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-00007370: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007380: 662e 5f73 7065 6369 6573 5f6e 756d 6265  f._species_numbe
-00007390: 722e 6170 7065 6e64 2873 656c 662e 6d6f  r.append(self.mo
-000073a0: 6465 6c73 5b69 5d2e 7370 6563 6965 735f  dels[i].species_
-000073b0: 6e75 6d62 6572 290a 2020 2020 2020 2020  number).        
-000073c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000073d0: 2020 7365 6c66 2e5f 7370 6563 6965 735f    self._species_
-000073e0: 6e75 6d62 6572 3d73 656c 662e 6d6f 6465  number=self.mode
-000073f0: 6c73 5b30 5d2e 7370 6563 6965 735f 6e75  ls[0].species_nu
-00007400: 6d62 6572 0a20 2020 2020 2020 2072 6574  mber.        ret
-00007410: 7572 6e20 7365 6c66 2e5f 7370 6563 6965  urn self._specie
-00007420: 735f 6e75 6d62 6572 0a0a 2020 2020 4073  s_number..    @s
-00007430: 7065 6369 6573 5f6e 756d 6265 722e 7365  pecies_number.se
-00007440: 7474 6572 0a20 2020 2064 6566 2073 7065  tter.    def spe
-00007450: 6369 6573 5f6e 756d 6265 7228 7365 6c66  cies_number(self
-00007460: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
-00007470: 2073 656c 662e 5f73 7065 6369 6573 5f6e   self._species_n
-00007480: 756d 6265 723d 7661 6c75 650a 0a20 2020  umber=value..   
-00007490: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000074a0: 6566 206d 6f64 656c 5f6e 756d 6265 7228  ef model_number(
-000074b0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-000074c0: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
-000074d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000074e0: 6c66 2e5f 6d6f 6465 6c5f 6e75 6d62 6572  lf._model_number
-000074f0: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
-00007500: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00007510: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00007520: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007530: 6c66 2e5f 6d6f 6465 6c5f 6e75 6d62 6572  lf._model_number
-00007540: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
-00007550: 656c 735b 695d 2e6d 6f64 656c 5f6e 756d  els[i].model_num
-00007560: 6265 7229 0a20 2020 2020 2020 2065 6c73  ber).        els
-00007570: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00007580: 656c 662e 5f6d 6f64 656c 5f6e 756d 6265  elf._model_numbe
-00007590: 723d 7365 6c66 2e6d 6f64 656c 735b 305d  r=self.models[0]
-000075a0: 2e6d 6f64 656c 5f6e 756d 6265 720a 2020  .model_number.  
-000075b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000075c0: 662e 5f6d 6f64 656c 5f6e 756d 6265 720a  f._model_number.
-000075d0: 0a20 2020 2040 6d6f 6465 6c5f 6e75 6d62  .    @model_numb
-000075e0: 6572 2e73 6574 7465 720a 2020 2020 6465  er.setter.    de
-000075f0: 6620 6d6f 6465 6c5f 6e75 6d62 6572 2873  f model_number(s
-00007600: 656c 662c 7661 6c75 6529 3a0a 2020 2020  elf,value):.    
-00007610: 2020 2020 7365 6c66 2e5f 6d6f 6465 6c5f      self._model_
-00007620: 6e75 6d62 6572 3d76 616c 7565 0a0a 2020  number=value..  
-00007630: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00007640: 6465 6620 4e48 2873 656c 6629 3a0a 2020  def NH(self):.  
-00007650: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
-00007660: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
-00007670: 2020 2020 2073 656c 662e 5f4e 483d 5b5d       self._NH=[]
-00007680: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00007690: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-000076a0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-000076b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000076c0: 5f4e 482e 6170 7065 6e64 2873 656c 662e  _NH.append(self.
-000076d0: 6d6f 6465 6c73 5b69 5d2e 4e48 290a 2020  models[i].NH).  
-000076e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000076f0: 2020 2020 2020 2020 7365 6c66 2e5f 4e48          self._NH
-00007700: 3d73 656c 662e 6d6f 6465 6c73 5b30 5d2e  =self.models[0].
-00007710: 4e48 0a20 2020 2020 2020 2072 6574 7572  NH.        retur
-00007720: 6e20 7365 6c66 2e5f 4e48 0a0a 2020 2020  n self._NH..    
-00007730: 404e 482e 7365 7474 6572 0a20 2020 2064  @NH.setter.    d
-00007740: 6566 204e 4828 7365 6c66 2c76 616c 7565  ef NH(self,value
-00007750: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00007760: 5f4e 483d 7661 6c75 650a 0a20 2020 2040  _NH=value..    @
-00007770: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00007780: 206e 436f 6c6c 2873 656c 6629 3a0a 2020   nColl(self):.  
-00007790: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
-000077a0: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
-000077b0: 2020 2020 2073 656c 662e 5f6e 436f 6c6c       self._nColl
-000077c0: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
-000077d0: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-000077e0: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-000077f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007800: 6c66 2e5f 6e43 6f6c 6c2e 6170 7065 6e64  lf._nColl.append
-00007810: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
-00007820: 6e43 6f6c 6c29 0a20 2020 2020 2020 2065  nColl).        e
-00007830: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00007840: 2073 656c 662e 5f6e 436f 6c6c 3d73 656c   self._nColl=sel
-00007850: 662e 6d6f 6465 6c73 5b30 5d2e 6e43 6f6c  f.models[0].nCol
-00007860: 6c0a 2020 2020 2020 2020 7265 7475 726e  l.        return
-00007870: 2073 656c 662e 5f6e 436f 6c6c 0a0a 2020   self._nColl..  
-00007880: 2020 406e 436f 6c6c 2e73 6574 7465 720a    @nColl.setter.
-00007890: 2020 2020 6465 6620 6e43 6f6c 6c28 7365      def nColl(se
-000078a0: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
-000078b0: 2020 2073 656c 662e 5f6e 436f 6c6c 3d76     self._nColl=v
-000078c0: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
-000078d0: 7274 790a 2020 2020 6465 6620 6e65 2873  rty.    def ne(s
-000078e0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-000078f0: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
-00007900: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007910: 662e 5f6e 653d 5b5d 0a20 2020 2020 2020  f._ne=[].       
-00007920: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00007930: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-00007940: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00007950: 2020 2073 656c 662e 5f6e 652e 6170 7065     self._ne.appe
-00007960: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
-00007970: 5d2e 6e65 290a 2020 2020 2020 2020 656c  ].ne).        el
-00007980: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00007990: 7365 6c66 2e5f 6e65 3d73 656c 662e 6d6f  self._ne=self.mo
-000079a0: 6465 6c73 5b30 5d2e 6e65 0a20 2020 2020  dels[0].ne.     
-000079b0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000079c0: 6e65 0a0a 2020 2020 406e 652e 7365 7474  ne..    @ne.sett
-000079d0: 6572 0a20 2020 2064 6566 206e 6528 7365  er.    def ne(se
-000079e0: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
-000079f0: 2020 2073 656c 662e 5f6e 653d 7661 6c75     self._ne=valu
-00007a00: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-00007a10: 0a20 2020 2064 6566 206e 4865 2873 656c  .    def nHe(sel
-00007a20: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00007a30: 656c 662e 6e6d 6f64 656c 733e 313a 0a20  elf.nmodels>1:. 
-00007a40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007a50: 5f6e 4865 3d5b 5d0a 2020 2020 2020 2020  _nHe=[].        
-00007a60: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00007a70: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-00007a80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007a90: 2020 7365 6c66 2e5f 6e48 652e 6170 7065    self._nHe.appe
-00007aa0: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
-00007ab0: 5d2e 6e48 6529 0a20 2020 2020 2020 2065  ].nHe).        e
-00007ac0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00007ad0: 2073 656c 662e 5f6e 4865 3d73 656c 662e   self._nHe=self.
-00007ae0: 6d6f 6465 6c73 5b30 5d2e 6e48 650a 2020  models[0].nHe.  
-00007af0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00007b00: 662e 5f6e 4865 0a0a 2020 2020 406e 4865  f._nHe..    @nHe
-00007b10: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00007b20: 6e48 6528 7365 6c66 2c76 616c 7565 293a  nHe(self,value):
-00007b30: 0a20 2020 2020 2020 2073 656c 662e 5f6e  .        self._n
-00007b40: 4865 3d76 616c 7565 0a0a 2020 2020 4070  He=value..    @p
-00007b50: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00007b60: 6e48 4949 2873 656c 6629 3a0a 2020 2020  nHII(self):.    
-00007b70: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
-00007b80: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
-00007b90: 2020 2073 656c 662e 5f6e 4849 493d 5b5d     self._nHII=[]
-00007ba0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00007bb0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-00007bc0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-00007bd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007be0: 5f6e 4849 492e 6170 7065 6e64 2873 656c  _nHII.append(sel
-00007bf0: 662e 6d6f 6465 6c73 5b69 5d2e 6e48 4949  f.models[i].nHII
-00007c00: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00007c10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007c20: 2e5f 6e48 4949 3d73 656c 662e 6d6f 6465  ._nHII=self.mode
-00007c30: 6c73 5b30 5d2e 6e48 4949 0a20 2020 2020  ls[0].nHII.     
-00007c40: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00007c50: 6e48 4949 0a0a 2020 2020 406e 4849 492e  nHII..    @nHII.
-00007c60: 7365 7474 6572 0a20 2020 2064 6566 206e  setter.    def n
-00007c70: 4849 4928 7365 6c66 2c76 616c 7565 293a  HII(self,value):
-00007c80: 0a20 2020 2020 2020 2073 656c 662e 5f6e  .        self._n
-00007c90: 4849 493d 7661 6c75 650a 0a20 2020 2040  HII=value..    @
-00007ca0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00007cb0: 206e 4849 2873 656c 6629 3a0a 2020 2020   nHI(self):.    
-00007cc0: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
-00007cd0: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
-00007ce0: 2020 2073 656c 662e 5f6e 4849 3d5b 5d0a     self._nHI=[].
-00007cf0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00007d00: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-00007d10: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-00007d20: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00007d30: 6e48 492e 6170 7065 6e64 2873 656c 662e  nHI.append(self.
-00007d40: 6d6f 6465 6c73 5b69 5d2e 6e48 4929 0a20  models[i].nHI). 
-00007d50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00007d60: 2020 2020 2020 2020 2073 656c 662e 5f6e           self._n
-00007d70: 4849 3d73 656c 662e 6d6f 6465 6c73 5b30  HI=self.models[0
-00007d80: 5d2e 6e48 490a 2020 2020 2020 2020 7265  ].nHI.        re
-00007d90: 7475 726e 2073 656c 662e 5f6e 4849 0a0a  turn self._nHI..
-00007da0: 2020 2020 406e 4849 2e73 6574 7465 720a      @nHI.setter.
-00007db0: 2020 2020 6465 6620 6e48 4928 7365 6c66      def nHI(self
-00007dc0: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
-00007dd0: 2073 656c 662e 5f6e 4849 3d76 616c 7565   self._nHI=value
-00007de0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00007df0: 2020 2020 6465 6620 6e48 3228 7365 6c66      def nH2(self
-00007e00: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00007e10: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
-00007e20: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00007e30: 6e48 323d 5b5d 0a20 2020 2020 2020 2020  nH2=[].         
-00007e40: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00007e50: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-00007e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007e70: 2073 656c 662e 5f6e 4832 2e61 7070 656e   self._nH2.appen
-00007e80: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
-00007e90: 2e6e 4832 290a 2020 2020 2020 2020 656c  .nH2).        el
-00007ea0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00007eb0: 7365 6c66 2e5f 6e48 323d 7365 6c66 2e6d  self._nH2=self.m
-00007ec0: 6f64 656c 735b 305d 2e6e 4832 0a20 2020  odels[0].nH2.   
-00007ed0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00007ee0: 2e5f 6e48 320a 0a20 2020 2040 6e48 322e  ._nH2..    @nH2.
-00007ef0: 7365 7474 6572 0a20 2020 2064 6566 206e  setter.    def n
-00007f00: 4832 2873 656c 662c 7661 6c75 6529 3a0a  H2(self,value):.
-00007f10: 2020 2020 2020 2020 7365 6c66 2e5f 6e48          self._nH
-00007f20: 323d 7661 6c75 650a 0a20 2020 2040 7072  2=value..    @pr
-00007f30: 6f70 6572 7479 0a20 2020 2064 6566 2064  operty.    def d
-00007f40: 7573 745f 746f 5f67 6173 2873 656c 6629  ust_to_gas(self)
-00007f50: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00007f60: 662e 6e6d 6f64 656c 733e 313a 0a20 2020  f.nmodels>1:.   
-00007f70: 2020 2020 2020 2020 2073 656c 662e 5f64           self._d
-00007f80: 7573 745f 746f 5f67 6173 3d5b 5d0a 2020  ust_to_gas=[].  
-00007f90: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00007fa0: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
-00007fb0: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
-00007fc0: 2020 2020 2020 2020 7365 6c66 2e5f 6475          self._du
-00007fd0: 7374 5f74 6f5f 6761 732e 6170 7065 6e64  st_to_gas.append
-00007fe0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
-00007ff0: 6475 7374 5f74 6f5f 6761 7329 0a20 2020  dust_to_gas).   
-00008000: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00008010: 2020 2020 2020 2073 656c 662e 5f64 7573         self._dus
-00008020: 745f 746f 5f67 6173 3d73 656c 662e 6d6f  t_to_gas=self.mo
-00008030: 6465 6c73 5b30 5d2e 6475 7374 5f74 6f5f  dels[0].dust_to_
-00008040: 6761 730a 2020 2020 2020 2020 7265 7475  gas.        retu
-00008050: 726e 2073 656c 662e 5f64 7573 745f 746f  rn self._dust_to
-00008060: 5f67 6173 0a0a 2020 2020 4064 7573 745f  _gas..    @dust_
-00008070: 746f 5f67 6173 2e73 6574 7465 720a 2020  to_gas.setter.  
-00008080: 2020 6465 6620 6475 7374 5f74 6f5f 6761    def dust_to_ga
-00008090: 7328 7365 6c66 2c76 616c 7565 293a 0a20  s(self,value):. 
-000080a0: 2020 2020 2020 2073 656c 662e 5f64 7573         self._dus
-000080b0: 745f 746f 5f67 6173 3d76 616c 7565 0a0a  t_to_gas=value..
-000080c0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-000080d0: 2020 6465 6620 7674 7572 6228 7365 6c66    def vturb(self
-000080e0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-000080f0: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
-00008100: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00008110: 7674 7572 623d 5b5d 0a20 2020 2020 2020  vturb=[].       
-00008120: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00008130: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
-00008140: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00008150: 2020 2073 656c 662e 5f76 7475 7262 2e61     self._vturb.a
-00008160: 7070 656e 6428 7365 6c66 2e6d 6f64 656c  ppend(self.model
-00008170: 735b 695d 2e76 7475 7262 290a 2020 2020  s[i].vturb).    
-00008180: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008190: 2020 2020 2020 7365 6c66 2e5f 7674 7572        self._vtur
-000081a0: 623d 7365 6c66 2e6d 6f64 656c 735b 305d  b=self.models[0]
-000081b0: 2e76 7475 7262 0a20 2020 2020 2020 2072  .vturb.        r
-000081c0: 6574 7572 6e20 7365 6c66 2e5f 7674 7572  eturn self._vtur
-000081d0: 620a 0a20 2020 2040 7674 7572 622e 7365  b..    @vturb.se
-000081e0: 7474 6572 0a20 2020 2064 6566 2076 7475  tter.    def vtu
-000081f0: 7262 2873 656c 662c 7661 6c75 6529 3a0a  rb(self,value):.
-00008200: 2020 2020 2020 2020 7365 6c66 2e5f 7674          self._vt
-00008210: 7572 623d 7661 6c75 650a 0a20 2020 2040  urb=value..    @
-00008220: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00008230: 2054 6728 7365 6c66 293a 0a20 2020 2020   Tg(self):.     
-00008240: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
-00008250: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
-00008260: 2020 7365 6c66 2e5f 5467 3d5b 5d0a 2020    self._Tg=[].  
-00008270: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00008280: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
-00008290: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
-000082a0: 2020 2020 2020 2020 7365 6c66 2e5f 5467          self._Tg
-000082b0: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
-000082c0: 656c 735b 695d 2e54 6729 0a20 2020 2020  els[i].Tg).     
-000082d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000082e0: 2020 2020 2073 656c 662e 5f54 673d 7365       self._Tg=se
-000082f0: 6c66 2e6d 6f64 656c 735b 305d 2e54 670a  lf.models[0].Tg.
-00008300: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00008310: 656c 662e 5f54 670a 0a20 2020 2040 5467  elf._Tg..    @Tg
-00008320: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00008330: 5467 2873 656c 662c 7661 6c75 6529 3a0a  Tg(self,value):.
-00008340: 2020 2020 2020 2020 7365 6c66 2e5f 5467          self._Tg
-00008350: 3d76 616c 7565 0a0a 2020 2020 4070 726f  =value..    @pro
-00008360: 7065 7274 790a 2020 2020 6465 6620 5464  perty.    def Td
-00008370: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008380: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-00008390: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-000083a0: 656c 662e 5f54 643d 5b5d 0a20 2020 2020  elf._Td=[].     
-000083b0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000083c0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
-000083d0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-000083e0: 2020 2020 2073 656c 662e 5f54 642e 6170       self._Td.ap
-000083f0: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
-00008400: 5b69 5d2e 5464 290a 2020 2020 2020 2020  [i].Td).        
-00008410: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00008420: 2020 7365 6c66 2e5f 5464 3d73 656c 662e    self._Td=self.
-00008430: 6d6f 6465 6c73 5b30 5d2e 5464 0a20 2020  models[0].Td.   
-00008440: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00008450: 2e5f 5464 0a0a 2020 2020 4054 642e 7365  ._Td..    @Td.se
-00008460: 7474 6572 0a20 2020 2064 6566 2054 6428  tter.    def Td(
-00008470: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-00008480: 2020 2020 2073 656c 662e 5f54 643d 7661       self._Td=va
-00008490: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
-000084a0: 7479 0a20 2020 2064 6566 2073 7065 6369  ty.    def speci
-000084b0: 6573 5f6e 616d 6528 7365 6c66 293a 0a20  es_name(self):. 
-000084c0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-000084d0: 6d6f 6465 6c73 3e31 3a0a 2020 2020 2020  models>1:.      
-000084e0: 2020 2020 2020 7365 6c66 2e5f 7370 6563        self._spec
-000084f0: 6965 735f 6e61 6d65 3d5b 5d0a 2020 2020  ies_name=[].    
-00008500: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00008510: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00008520: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
-00008530: 2020 2020 2020 7365 6c66 2e5f 7370 6563        self._spec
-00008540: 6965 735f 6e61 6d65 2e61 7070 656e 6428  ies_name.append(
-00008550: 7365 6c66 2e6d 6f64 656c 735b 695d 2e73  self.models[i].s
-00008560: 7065 6369 6573 5f6e 616d 6529 0a20 2020  pecies_name).   
-00008570: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00008580: 2020 2020 2020 2073 656c 662e 5f73 7065         self._spe
-00008590: 6369 6573 5f6e 616d 653d 7365 6c66 2e6d  cies_name=self.m
-000085a0: 6f64 656c 735b 305d 2e73 7065 6369 6573  odels[0].species
-000085b0: 5f6e 616d 650a 2020 2020 2020 2020 7265  _name.        re
-000085c0: 7475 726e 2073 656c 662e 5f73 7065 6369  turn self._speci
-000085d0: 6573 5f6e 616d 650a 0a20 2020 2040 7370  es_name..    @sp
-000085e0: 6563 6965 735f 6e61 6d65 2e73 6574 7465  ecies_name.sette
-000085f0: 720a 2020 2020 6465 6620 7370 6563 6965  r.    def specie
-00008600: 735f 6e61 6d65 2873 656c 662c 7661 6c75  s_name(self,valu
-00008610: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00008620: 2e5f 7370 6563 6965 735f 6e61 6d65 3d76  ._species_name=v
-00008630: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
-00008640: 7274 790a 2020 2020 6465 6620 7370 6563  rty.    def spec
-00008650: 6965 735f 696e 6465 7828 7365 6c66 293a  ies_index(self):
-00008660: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00008670: 2e6e 6d6f 6465 6c73 3e31 3a0a 2020 2020  .nmodels>1:.    
-00008680: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
-00008690: 6563 6965 735f 696e 6465 783d 5b5d 0a20  ecies_index=[]. 
-000086a0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-000086b0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-000086c0: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
-000086d0: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
-000086e0: 7065 6369 6573 5f69 6e64 6578 2e61 7070  pecies_index.app
-000086f0: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
-00008700: 695d 2e73 7065 6369 6573 5f69 6e64 6578  i].species_index
-00008710: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00008720: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008730: 2e5f 7370 6563 6965 735f 696e 6465 783d  ._species_index=
-00008740: 7365 6c66 2e6d 6f64 656c 735b 305d 2e73  self.models[0].s
-00008750: 7065 6369 6573 5f69 6e64 6578 0a20 2020  pecies_index.   
-00008760: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00008770: 2e5f 7370 6563 6965 735f 696e 6465 780a  ._species_index.
-00008780: 0a20 2020 2040 7370 6563 6965 735f 696e  .    @species_in
-00008790: 6465 782e 7365 7474 6572 0a20 2020 2064  dex.setter.    d
-000087a0: 6566 2073 7065 6369 6573 5f69 6e64 6578  ef species_index
-000087b0: 2873 656c 662c 7661 6c75 6529 3a0a 2020  (self,value):.  
-000087c0: 2020 2020 2020 7365 6c66 2e5f 7370 6563        self._spec
-000087d0: 6965 735f 696e 6465 783d 7661 6c75 650a  ies_index=value.
-000087e0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000087f0: 2020 2064 6566 2061 6275 6e64 616e 6365     def abundance
-00008800: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008810: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-00008820: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-00008830: 656c 662e 5f61 6275 6e64 616e 6365 3d5b  elf._abundance=[
-00008840: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00008850: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
-00008860: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
-00008870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008880: 2e5f 6162 756e 6461 6e63 652e 6170 7065  ._abundance.appe
-00008890: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
-000088a0: 5d2e 6162 756e 6461 6e63 6529 0a20 2020  ].abundance).   
-000088b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000088c0: 2020 2020 2020 2073 656c 662e 5f61 6275         self._abu
-000088d0: 6e64 616e 6365 3d73 656c 662e 6d6f 6465  ndance=self.mode
-000088e0: 6c73 5b30 5d2e 6162 756e 6461 6e63 650a  ls[0].abundance.
-000088f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00008900: 656c 662e 5f61 6275 6e64 616e 6365 0a0a  elf._abundance..
-00008910: 2020 2020 4061 6275 6e64 616e 6365 2e73      @abundance.s
-00008920: 6574 7465 720a 2020 2020 6465 6620 6162  etter.    def ab
-00008930: 756e 6461 6e63 6528 7365 6c66 2c76 616c  undance(self,val
-00008940: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
-00008950: 662e 5f61 6275 6e64 616e 6365 3d76 616c  f._abundance=val
-00008960: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
-00008970: 790a 2020 2020 6465 6620 6476 2873 656c  y.    def dv(sel
-00008980: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00008990: 656c 662e 6e6d 6f64 656c 733e 313a 0a20  elf.nmodels>1:. 
-000089a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000089b0: 5f64 763d 5b5d 0a20 2020 2020 2020 2020  _dv=[].         
-000089c0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-000089d0: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-000089e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000089f0: 2073 656c 662e 5f64 762e 6170 7065 6e64   self._dv.append
-00008a00: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
-00008a10: 6476 290a 2020 2020 2020 2020 656c 7365  dv).        else
-00008a20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00008a30: 6c66 2e5f 6476 3d73 656c 662e 6d6f 6465  lf._dv=self.mode
-00008a40: 6c73 5b30 5d2e 6476 0a20 2020 2020 2020  ls[0].dv.       
-00008a50: 2072 6574 7572 6e20 7365 6c66 2e5f 6476   return self._dv
-00008a60: 0a0a 2020 2020 4064 762e 7365 7474 6572  ..    @dv.setter
-00008a70: 0a20 2020 2064 6566 2064 7628 7365 6c66  .    def dv(self
-00008a80: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
-00008a90: 2073 656c 662e 5f64 763d 7661 6c75 650a   self._dv=value.
-00008aa0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00008ab0: 2020 2064 6566 206e 6c65 7665 6c73 2873     def nlevels(s
-00008ac0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00008ad0: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
-00008ae0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008af0: 662e 5f6e 6c65 7665 6c73 3d5b 5d0a 2020  f._nlevels=[].  
-00008b00: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00008b10: 696e 2072 616e 6765 2873 656c 662e 6e6d  in range(self.nm
-00008b20: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
-00008b30: 2020 2020 2020 2020 7365 6c66 2e5f 6e6c          self._nl
-00008b40: 6576 656c 732e 6170 7065 6e64 2873 656c  evels.append(sel
-00008b50: 662e 6d6f 6465 6c73 5b69 5d2e 6e6c 6576  f.models[i].nlev
-00008b60: 656c 7329 0a20 2020 2020 2020 2065 6c73  els).        els
-00008b70: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00008b80: 656c 662e 5f6e 6c65 7665 6c73 3d73 656c  elf._nlevels=sel
-00008b90: 662e 6d6f 6465 6c73 5b30 5d2e 6e6c 6576  f.models[0].nlev
-00008ba0: 656c 730a 2020 2020 2020 2020 7265 7475  els.        retu
-00008bb0: 726e 2073 656c 662e 5f6e 6c65 7665 6c73  rn self._nlevels
-00008bc0: 0a0a 2020 2020 406e 6c65 7665 6c73 2e73  ..    @nlevels.s
-00008bd0: 6574 7465 720a 2020 2020 6465 6620 6e6c  etter.    def nl
-00008be0: 6576 656c 7328 7365 6c66 2c76 616c 7565  evels(self,value
-00008bf0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00008c00: 5f6e 6c65 7665 6c73 3d76 616c 7565 0a0a  _nlevels=value..
-00008c10: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00008c20: 2020 6465 6620 6e6c 696e 6573 2873 656c    def nlines(sel
-00008c30: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00008c40: 656c 662e 6e6d 6f64 656c 733e 313a 0a20  elf.nmodels>1:. 
-00008c50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008c60: 5f6e 6c69 6e65 733d 5b5d 0a20 2020 2020  _nlines=[].     
-00008c70: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00008c80: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
-00008c90: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-00008ca0: 2020 2020 2073 656c 662e 5f6e 6c69 6e65       self._nline
-00008cb0: 732e 6170 7065 6e64 2873 656c 662e 6d6f  s.append(self.mo
-00008cc0: 6465 6c73 5b69 5d2e 6e6c 696e 6573 290a  dels[i].nlines).
-00008cd0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00008ce0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00008cf0: 6e6c 696e 6573 3d73 656c 662e 6d6f 6465  nlines=self.mode
-00008d00: 6c73 5b30 5d2e 6e6c 696e 6573 0a20 2020  ls[0].nlines.   
-00008d10: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00008d20: 2e5f 6e6c 696e 6573 0a0a 2020 2020 406e  ._nlines..    @n
-00008d30: 6c69 6e65 732e 7365 7474 6572 0a20 2020  lines.setter.   
-00008d40: 2064 6566 206e 6c69 6e65 7328 7365 6c66   def nlines(self
-00008d50: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
-00008d60: 2073 656c 662e 5f6e 6c69 6e65 733d 7661   self._nlines=va
-00008d70: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
-00008d80: 7479 0a20 2020 2064 6566 206c 696e 6564  ty.    def lined
-00008d90: 6174 6128 7365 6c66 293a 0a20 2020 2020  ata(self):.     
-00008da0: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
-00008db0: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
-00008dc0: 2020 7365 6c66 2e5f 6c69 6e65 6461 7461    self._linedata
-00008dd0: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
-00008de0: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00008df0: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00008e00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00008e10: 6c66 2e5f 6c69 6e65 6461 7461 2e61 7070  lf._linedata.app
-00008e20: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
-00008e30: 695d 2e6c 696e 6564 6174 6129 0a20 2020  i].linedata).   
-00008e40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00008e50: 2020 2020 2020 2073 656c 662e 5f6c 696e         self._lin
-00008e60: 6564 6174 613d 7365 6c66 2e6d 6f64 656c  edata=self.model
-00008e70: 735b 305d 2e6c 696e 6564 6174 610a 2020  s[0].linedata.  
-00008e80: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00008e90: 662e 5f6c 696e 6564 6174 610a 0a20 2020  f._linedata..   
-00008ea0: 2040 6c69 6e65 6461 7461 2e73 6574 7465   @linedata.sette
-00008eb0: 720a 2020 2020 6465 6620 6c69 6e65 6461  r.    def lineda
-00008ec0: 7461 2873 656c 662c 7661 6c75 6529 3a0a  ta(self,value):.
-00008ed0: 2020 2020 2020 2020 7365 6c66 2e5f 6c69          self._li
-00008ee0: 6e65 6461 7461 3d76 616c 7565 0a0a 2020  nedata=value..  
-00008ef0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00008f00: 6465 6620 6c65 7665 6c64 6174 6128 7365  def leveldata(se
-00008f10: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00008f20: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
-00008f30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008f40: 2e5f 6c65 7665 6c64 6174 613d 5b5d 0a20  ._leveldata=[]. 
-00008f50: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00008f60: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-00008f70: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
-00008f80: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-00008f90: 6576 656c 6461 7461 2e61 7070 656e 6428  eveldata.append(
-00008fa0: 7365 6c66 2e6d 6f64 656c 735b 695d 2e6c  self.models[i].l
-00008fb0: 6576 656c 6461 7461 290a 2020 2020 2020  eveldata).      
-00008fc0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00008fd0: 2020 2020 7365 6c66 2e5f 6c65 7665 6c64      self._leveld
-00008fe0: 6174 613d 7365 6c66 2e6d 6f64 656c 735b  ata=self.models[
-00008ff0: 305d 2e6c 6576 656c 6461 7461 0a20 2020  0].leveldata.   
-00009000: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00009010: 2e5f 6c65 7665 6c64 6174 610a 0a20 2020  ._leveldata..   
-00009020: 2040 6c65 7665 6c64 6174 612e 7365 7474   @leveldata.sett
-00009030: 6572 0a20 2020 2064 6566 206c 6576 656c  er.    def level
-00009040: 6461 7461 2873 656c 662c 7661 6c75 6529  data(self,value)
-00009050: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00009060: 6c65 7665 6c64 6174 613d 7661 6c75 650a  leveldata=value.
-00009070: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00009080: 2020 2064 6566 2063 6f6e 7657 6176 656c     def convWavel
-00009090: 656e 6774 6828 7365 6c66 293a 0a20 2020  ength(self):.   
-000090a0: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
-000090b0: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
-000090c0: 2020 2020 7365 6c66 2e5f 636f 6e76 5761      self._convWa
-000090d0: 7665 6c65 6e67 7468 3d5b 5d0a 2020 2020  velength=[].    
-000090e0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-000090f0: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00009100: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
-00009110: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
-00009120: 5761 7665 6c65 6e67 7468 2e61 7070 656e  Wavelength.appen
-00009130: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
-00009140: 2e63 6f6e 7657 6176 656c 656e 6774 6829  .convWavelength)
-00009150: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00009160: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009170: 5f63 6f6e 7657 6176 656c 656e 6774 683d  _convWavelength=
-00009180: 7365 6c66 2e6d 6f64 656c 735b 305d 2e63  self.models[0].c
-00009190: 6f6e 7657 6176 656c 656e 6774 680a 2020  onvWavelength.  
-000091a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000091b0: 662e 5f63 6f6e 7657 6176 656c 656e 6774  f._convWavelengt
-000091c0: 680a 0a20 2020 2040 636f 6e76 5761 7665  h..    @convWave
-000091d0: 6c65 6e67 7468 2e73 6574 7465 720a 2020  length.setter.  
-000091e0: 2020 6465 6620 636f 6e76 5761 7665 6c65    def convWavele
-000091f0: 6e67 7468 2873 656c 662c 7661 6c75 6529  ngth(self,value)
-00009200: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00009210: 636f 6e76 5761 7665 6c65 6e67 7468 3d76  convWavelength=v
-00009220: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
-00009230: 7274 790a 2020 2020 6465 6620 636f 6e76  rty.    def conv
-00009240: 4c54 4566 6c75 7828 7365 6c66 293a 0a20  LTEflux(self):. 
-00009250: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-00009260: 6d6f 6465 6c73 3e31 3a0a 2020 2020 2020  models>1:.      
-00009270: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
-00009280: 4c54 4566 6c75 783d 5b5d 0a20 2020 2020  LTEflux=[].     
-00009290: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000092a0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
-000092b0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-000092c0: 2020 2020 2073 656c 662e 5f63 6f6e 764c       self._convL
-000092d0: 5445 666c 7578 2e61 7070 656e 6428 7365  TEflux.append(se
-000092e0: 6c66 2e6d 6f64 656c 735b 695d 2e63 6f6e  lf.models[i].con
-000092f0: 764c 5445 666c 7578 290a 2020 2020 2020  vLTEflux).      
-00009300: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00009310: 2020 2020 7365 6c66 2e5f 636f 6e76 4c54      self._convLT
-00009320: 4566 6c75 783d 7365 6c66 2e6d 6f64 656c  Eflux=self.model
-00009330: 735b 305d 2e63 6f6e 764c 5445 666c 7578  s[0].convLTEflux
-00009340: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009350: 7365 6c66 2e5f 636f 6e76 4c54 4566 6c75  self._convLTEflu
-00009360: 780a 0a20 2020 2040 636f 6e76 4c54 4566  x..    @convLTEf
-00009370: 6c75 782e 7365 7474 6572 0a20 2020 2064  lux.setter.    d
-00009380: 6566 2063 6f6e 764c 5445 666c 7578 2873  ef convLTEflux(s
-00009390: 656c 662c 7661 6c75 6529 3a0a 2020 2020  elf,value):.    
-000093a0: 2020 2020 7365 6c66 2e5f 636f 6e76 4c54      self._convLT
-000093b0: 4566 6c75 783d 7661 6c75 650a 0a20 2020  Eflux=value..   
-000093c0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000093d0: 6566 2063 6f6e 764e 4c54 4566 6c75 7828  ef convNLTEflux(
-000093e0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-000093f0: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
-00009400: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00009410: 6c66 2e5f 636f 6e76 4e4c 5445 666c 7578  lf._convNLTEflux
-00009420: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
-00009430: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00009440: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
-00009450: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00009460: 6c66 2e5f 636f 6e76 4e4c 5445 666c 7578  lf._convNLTEflux
-00009470: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
-00009480: 656c 735b 695d 2e63 6f6e 764e 4c54 4566  els[i].convNLTEf
-00009490: 6c75 7829 0a20 2020 2020 2020 2065 6c73  lux).        els
-000094a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000094b0: 656c 662e 5f63 6f6e 764e 4c54 4566 6c75  elf._convNLTEflu
-000094c0: 783d 7365 6c66 2e6d 6f64 656c 735b 305d  x=self.models[0]
-000094d0: 2e63 6f6e 764e 4c54 4566 6c75 780a 2020  .convNLTEflux.  
-000094e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000094f0: 662e 5f63 6f6e 764e 4c54 4566 6c75 780a  f._convNLTEflux.
-00009500: 0a20 2020 2040 636f 6e76 4e4c 5445 666c  .    @convNLTEfl
-00009510: 7578 2e73 6574 7465 720a 2020 2020 6465  ux.setter.    de
-00009520: 6620 636f 6e76 4e4c 5445 666c 7578 2873  f convNLTEflux(s
-00009530: 656c 662c 7661 6c75 6529 3a0a 2020 2020  elf,value):.    
-00009540: 2020 2020 7365 6c66 2e5f 636f 6e76 4e4c      self._convNL
-00009550: 5445 666c 7578 3d76 616c 7565 0a0a 2020  TEflux=value..  
-00009560: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00009570: 6465 6620 636f 6e76 5479 7065 2873 656c  def convType(sel
-00009580: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00009590: 656c 662e 6e6d 6f64 656c 733e 313a 0a20  elf.nmodels>1:. 
-000095a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000095b0: 5f63 6f6e 7654 7970 653d 5b5d 0a20 2020  _convType=[].   
-000095c0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-000095d0: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
-000095e0: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
-000095f0: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
-00009600: 7654 7970 652e 6170 7065 6e64 2873 656c  vType.append(sel
-00009610: 662e 6d6f 6465 6c73 5b69 5d2e 636f 6e76  f.models[i].conv
-00009620: 5479 7065 290a 2020 2020 2020 2020 656c  Type).        el
-00009630: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00009640: 7365 6c66 2e5f 636f 6e76 5479 7065 3d73  self._convType=s
-00009650: 656c 662e 6d6f 6465 6c73 5b30 5d2e 636f  elf.models[0].co
-00009660: 6e76 5479 7065 0a20 2020 2020 2020 2072  nvType.        r
-00009670: 6574 7572 6e20 7365 6c66 2e5f 636f 6e76  eturn self._conv
-00009680: 5479 7065 0a0a 2020 2020 4063 6f6e 7654  Type..    @convT
-00009690: 7970 652e 7365 7474 6572 0a20 2020 2064  ype.setter.    d
-000096a0: 6566 2063 6f6e 7654 7970 6528 7365 6c66  ef convType(self
-000096b0: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
-000096c0: 2073 656c 662e 5f63 6f6e 7654 7970 653d   self._convType=
-000096d0: 7661 6c75 650a 0a20 2020 2040 7072 6f70  value..    @prop
-000096e0: 6572 7479 0a20 2020 2064 6566 2063 6f6e  erty.    def con
-000096f0: 7652 2873 656c 6629 3a0a 2020 2020 2020  vR(self):.      
-00009700: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
-00009710: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
-00009720: 2073 656c 662e 5f63 6f6e 7652 3d5b 5d0a   self._convR=[].
-00009730: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00009740: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-00009750: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-00009760: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009770: 636f 6e76 522e 6170 7065 6e64 2873 656c  convR.append(sel
-00009780: 662e 6d6f 6465 6c73 5b69 5d2e 636f 6e76  f.models[i].conv
-00009790: 5229 0a20 2020 2020 2020 2065 6c73 653a  R).        else:
-000097a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000097b0: 662e 5f63 6f6e 7652 3d73 656c 662e 6d6f  f._convR=self.mo
-000097c0: 6465 6c73 5b30 5d2e 636f 6e76 520a 2020  dels[0].convR.  
-000097d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000097e0: 662e 5f63 6f6e 7652 0a0a 2020 2020 4063  f._convR..    @c
-000097f0: 6f6e 7652 2e73 6574 7465 720a 2020 2020  onvR.setter.    
-00009800: 6465 6620 636f 6e76 5228 7365 6c66 2c76  def convR(self,v
-00009810: 616c 7565 293a 0a20 2020 2020 2020 2073  alue):.        s
-00009820: 656c 662e 5f63 6f6e 7652 3d76 616c 7565  elf._convR=value
-00009830: 0a0a 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00009840: 0a20 2020 2064 6566 2063 6f6e 764f 7665  .    def convOve
-00009850: 726c 6170 4672 6571 2873 656c 6629 3a0a  rlapFreq(self):.
-00009860: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00009870: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
-00009880: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
-00009890: 764f 7665 726c 6170 4672 6571 3d5b 5d0a  vOverlapFreq=[].
-000098a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000098b0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-000098c0: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-000098d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000098e0: 636f 6e76 4f76 6572 6c61 7046 7265 712e  convOverlapFreq.
-000098f0: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
-00009900: 6c73 5b69 5d2e 636f 6e76 4f76 6572 6c61  ls[i].convOverla
-00009910: 7046 7265 7129 0a20 2020 2020 2020 2065  pFreq).        e
-00009920: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00009930: 2073 656c 662e 5f63 6f6e 764f 7665 726c   self._convOverl
-00009940: 6170 4672 6571 3d73 656c 662e 6d6f 6465  apFreq=self.mode
-00009950: 6c73 5b30 5d2e 636f 6e76 4f76 6572 6c61  ls[0].convOverla
-00009960: 7046 7265 710a 2020 2020 2020 2020 7265  pFreq.        re
-00009970: 7475 726e 2073 656c 662e 5f63 6f6e 764f  turn self._convO
-00009980: 7665 726c 6170 4672 6571 0a0a 2020 2020  verlapFreq..    
-00009990: 4063 6f6e 764f 7665 726c 6170 4672 6571  @convOverlapFreq
-000099a0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-000099b0: 636f 6e76 4f76 6572 6c61 7046 7265 7128  convOverlapFreq(
-000099c0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-000099d0: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
-000099e0: 7665 726c 6170 4672 6571 3d76 616c 7565  verlapFreq=value
-000099f0: 0a0a 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00009a00: 0a20 2020 2064 6566 2063 6f6e 764f 7665  .    def convOve
-00009a10: 726c 6170 5761 7665 2873 656c 6629 3a0a  rlapWave(self):.
-00009a20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00009a30: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
-00009a40: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
-00009a50: 764f 7665 726c 6170 5761 7665 3d5b 5d0a  vOverlapWave=[].
-00009a60: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00009a70: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-00009a80: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
-00009a90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009aa0: 636f 6e76 4f76 6572 6c61 7057 6176 652e  convOverlapWave.
-00009ab0: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
-00009ac0: 6c73 5b69 5d2e 636f 6e76 4f76 6572 6c61  ls[i].convOverla
-00009ad0: 7057 6176 6529 0a20 2020 2020 2020 2065  pWave).        e
-00009ae0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00009af0: 2073 656c 662e 5f63 6f6e 764f 7665 726c   self._convOverl
-00009b00: 6170 5761 7665 3d73 656c 662e 6d6f 6465  apWave=self.mode
-00009b10: 6c73 5b30 5d2e 636f 6e76 4f76 6572 6c61  ls[0].convOverla
-00009b20: 7057 6176 650a 2020 2020 2020 2020 7265  pWave.        re
-00009b30: 7475 726e 2073 656c 662e 5f63 6f6e 764f  turn self._convO
-00009b40: 7665 726c 6170 5761 7665 0a0a 2020 2020  verlapWave..    
-00009b50: 4063 6f6e 764f 7665 726c 6170 5761 7665  @convOverlapWave
-00009b60: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00009b70: 636f 6e76 4f76 6572 6c61 7057 6176 6528  convOverlapWave(
-00009b80: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-00009b90: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
-00009ba0: 7665 726c 6170 5761 7665 3d76 616c 7565  verlapWave=value
-00009bb0: 0a20 2020 2020 2020 200a 2020 2020 4070  .        .    @p
-00009bc0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00009bd0: 6f76 6572 6c61 7046 7265 7128 7365 6c66  overlapFreq(self
-00009be0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00009bf0: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
-00009c00: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009c10: 6f76 6572 6c61 7046 7265 713d 5b5d 0a20  overlapFreq=[]. 
-00009c20: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00009c30: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-00009c40: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
-00009c50: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
-00009c60: 7665 726c 6170 4672 6571 2e61 7070 656e  verlapFreq.appen
-00009c70: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
-00009c80: 2e6f 7665 726c 6170 4672 6571 290a 2020  .overlapFreq).  
-00009c90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00009ca0: 2020 2020 2020 2020 7365 6c66 2e5f 6f76          self._ov
-00009cb0: 6572 6c61 7046 7265 713d 7365 6c66 2e6d  erlapFreq=self.m
-00009cc0: 6f64 656c 735b 305d 2e6f 7665 726c 6170  odels[0].overlap
-00009cd0: 4672 6571 0a20 2020 2020 2020 2072 6574  Freq.        ret
-00009ce0: 7572 6e20 7365 6c66 2e5f 6f76 6572 6c61  urn self._overla
-00009cf0: 7046 7265 710a 0a20 2020 2040 6f76 6572  pFreq..    @over
-00009d00: 6c61 7046 7265 712e 7365 7474 6572 0a20  lapFreq.setter. 
-00009d10: 2020 2064 6566 206f 7665 726c 6170 4672     def overlapFr
-00009d20: 6571 2873 656c 662c 7661 6c75 6529 3a0a  eq(self,value):.
-00009d30: 2020 2020 2020 2020 7365 6c66 2e5f 6f76          self._ov
-00009d40: 6572 6c61 7046 7265 713d 7661 6c75 650a  erlapFreq=value.
-00009d50: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00009d60: 2020 2064 6566 2063 6f6e 764f 7665 726c     def convOverl
-00009d70: 6170 4c54 4528 7365 6c66 293a 0a20 2020  apLTE(self):.   
-00009d80: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
-00009d90: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
-00009da0: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
-00009db0: 6572 6c61 704c 5445 3d5b 5d0a 2020 2020  erlapLTE=[].    
-00009dc0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00009dd0: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
-00009de0: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
-00009df0: 2020 2020 2020 7365 6c66 2e5f 636f 6e76        self._conv
-00009e00: 4f76 6572 6c61 704c 5445 2e61 7070 656e  OverlapLTE.appen
-00009e10: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
-00009e20: 2e63 6f6e 764f 7665 726c 6170 4c54 4529  .convOverlapLTE)
-00009e30: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00009e40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009e50: 5f63 6f6e 764f 7665 726c 6170 4c54 453d  _convOverlapLTE=
-00009e60: 7365 6c66 2e6d 6f64 656c 735b 305d 2e63  self.models[0].c
-00009e70: 6f6e 764f 7665 726c 6170 4c54 450a 2020  onvOverlapLTE.  
-00009e80: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00009e90: 662e 5f63 6f6e 764f 7665 726c 6170 4c54  f._convOverlapLT
-00009ea0: 450a 0a20 2020 2040 636f 6e76 4f76 6572  E..    @convOver
-00009eb0: 6c61 704c 5445 2e73 6574 7465 720a 2020  lapLTE.setter.  
-00009ec0: 2020 6465 6620 636f 6e76 4f76 6572 6c61    def convOverla
-00009ed0: 704c 5445 2873 656c 662c 7661 6c75 6529  pLTE(self,value)
-00009ee0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00009ef0: 636f 6e76 4f76 6572 6c61 704c 5445 3d76  convOverlapLTE=v
-00009f00: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
-00009f10: 7274 790a 2020 2020 6465 6620 636f 6e76  rty.    def conv
-00009f20: 4f76 6572 6c61 704e 4c54 4528 7365 6c66  OverlapNLTE(self
-00009f30: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00009f40: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
-00009f50: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009f60: 636f 6e76 4f76 6572 6c61 704e 4c54 453d  convOverlapNLTE=
-00009f70: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-00009f80: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-00009f90: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
-00009fa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00009fb0: 662e 5f63 6f6e 764f 7665 726c 6170 4e4c  f._convOverlapNL
-00009fc0: 5445 2e61 7070 656e 6428 7365 6c66 2e6d  TE.append(self.m
-00009fd0: 6f64 656c 735b 695d 2e63 6f6e 764f 7665  odels[i].convOve
-00009fe0: 726c 6170 4e4c 5445 290a 2020 2020 2020  rlapNLTE).      
-00009ff0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000a000: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
-0000a010: 6572 6c61 704e 4c54 453d 7365 6c66 2e6d  erlapNLTE=self.m
-0000a020: 6f64 656c 735b 305d 2e63 6f6e 764f 7665  odels[0].convOve
-0000a030: 726c 6170 4e4c 5445 0a20 2020 2020 2020  rlapNLTE.       
-0000a040: 2072 6574 7572 6e20 7365 6c66 2e5f 636f   return self._co
-0000a050: 6e76 4f76 6572 6c61 704e 4c54 450a 0a20  nvOverlapNLTE.. 
-0000a060: 2020 2040 636f 6e76 4f76 6572 6c61 704e     @convOverlapN
-0000a070: 4c54 452e 7365 7474 6572 0a20 2020 2064  LTE.setter.    d
-0000a080: 6566 2063 6f6e 764f 7665 726c 6170 4e4c  ef convOverlapNL
-0000a090: 5445 2873 656c 662c 7661 6c75 6529 3a0a  TE(self,value):.
-0000a0a0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-0000a0b0: 6e76 4f76 6572 6c61 704e 4c54 453d 7661  nvOverlapNLTE=va
-0000a0c0: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
-0000a0d0: 7479 0a20 2020 2064 6566 206f 7665 726c  ty.    def overl
-0000a0e0: 6170 4c54 4528 7365 6c66 293a 0a20 2020  apLTE(self):.   
-0000a0f0: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
-0000a100: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
-0000a110: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
-0000a120: 704c 5445 3d5b 5d0a 2020 2020 2020 2020  pLTE=[].        
-0000a130: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000a140: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-0000a150: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a160: 2020 7365 6c66 2e5f 6f76 6572 6c61 704c    self._overlapL
-0000a170: 5445 2e61 7070 656e 6428 7365 6c66 2e6d  TE.append(self.m
-0000a180: 6f64 656c 735b 695d 2e6f 7665 726c 6170  odels[i].overlap
-0000a190: 4c54 4529 0a20 2020 2020 2020 2065 6c73  LTE).        els
-0000a1a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000a1b0: 656c 662e 5f6f 7665 726c 6170 4c54 453d  elf._overlapLTE=
-0000a1c0: 7365 6c66 2e6d 6f64 656c 735b 305d 2e6f  self.models[0].o
-0000a1d0: 7665 726c 6170 4c54 450a 2020 2020 2020  verlapLTE.      
-0000a1e0: 2020 7265 7475 726e 2073 656c 662e 5f6f    return self._o
-0000a1f0: 7665 726c 6170 4c54 450a 0a20 2020 2040  verlapLTE..    @
-0000a200: 6f76 6572 6c61 704c 5445 2e73 6574 7465  overlapLTE.sette
-0000a210: 720a 2020 2020 6465 6620 6f76 6572 6c61  r.    def overla
-0000a220: 704c 5445 2873 656c 662c 7661 6c75 6529  pLTE(self,value)
-0000a230: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-0000a240: 6f76 6572 6c61 704c 5445 3d76 616c 7565  overlapLTE=value
-0000a250: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000a260: 2020 2020 6465 6620 6f76 6572 6c61 704e      def overlapN
-0000a270: 4c54 4528 7365 6c66 293a 0a20 2020 2020  LTE(self):.     
-0000a280: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
-0000a290: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
-0000a2a0: 2020 7365 6c66 2e5f 6f76 6572 6c61 704e    self._overlapN
-0000a2b0: 4c54 453d 5b5d 0a20 2020 2020 2020 2020  LTE=[].         
-0000a2c0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000a2d0: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-0000a2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a2f0: 2073 656c 662e 5f6f 7665 726c 6170 4e4c   self._overlapNL
-0000a300: 5445 2e61 7070 656e 6428 7365 6c66 2e6d  TE.append(self.m
-0000a310: 6f64 656c 735b 695d 2e6f 7665 726c 6170  odels[i].overlap
-0000a320: 4e4c 5445 290a 2020 2020 2020 2020 656c  NLTE).        el
-0000a330: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000a340: 7365 6c66 2e5f 6f76 6572 6c61 704e 4c54  self._overlapNLT
-0000a350: 453d 7365 6c66 2e6d 6f64 656c 735b 305d  E=self.models[0]
-0000a360: 2e6f 7665 726c 6170 4e4c 5445 0a20 2020  .overlapNLTE.   
-0000a370: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000a380: 2e5f 6f76 6572 6c61 704e 4c54 450a 0a20  ._overlapNLTE.. 
-0000a390: 2020 2040 6f76 6572 6c61 704e 4c54 452e     @overlapNLTE.
-0000a3a0: 7365 7474 6572 0a20 2020 2064 6566 206f  setter.    def o
-0000a3b0: 7665 726c 6170 4e4c 5445 2873 656c 662c  verlapNLTE(self,
-0000a3c0: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
-0000a3d0: 7365 6c66 2e5f 6f76 6572 6c61 704e 4c54  self._overlapNLT
-0000a3e0: 453d 7661 6c75 650a 2020 2020 2020 2020  E=value.        
-0000a3f0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000a400: 2020 2064 6566 206f 7665 726c 6170 5461     def overlapTa
-0000a410: 754c 5445 2873 656c 6629 3a0a 2020 2020  uLTE(self):.    
-0000a420: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
-0000a430: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
-0000a440: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
-0000a450: 5461 754c 5445 3d5b 5d0a 2020 2020 2020  TauLTE=[].      
-0000a460: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0000a470: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
-0000a480: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000a490: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
-0000a4a0: 7054 6175 4c54 452e 6170 7065 6e64 2873  pTauLTE.append(s
-0000a4b0: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6f76  elf.models[i].ov
-0000a4c0: 6572 6c61 7054 6175 4c54 4529 0a20 2020  erlapTauLTE).   
-0000a4d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a4e0: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
-0000a4f0: 726c 6170 5461 754c 5445 3d73 656c 662e  rlapTauLTE=self.
-0000a500: 6d6f 6465 6c73 5b30 5d2e 6f76 6572 6c61  models[0].overla
-0000a510: 7054 6175 4c54 450a 2020 2020 2020 2020  pTauLTE.        
-0000a520: 7265 7475 726e 2073 656c 662e 5f6f 7665  return self._ove
-0000a530: 726c 6170 5461 754c 5445 0a0a 2020 2020  rlapTauLTE..    
-0000a540: 406f 7665 726c 6170 5461 754c 5445 2e73  @overlapTauLTE.s
-0000a550: 6574 7465 720a 2020 2020 6465 6620 6f76  etter.    def ov
-0000a560: 6572 6c61 7054 6175 4c54 4528 7365 6c66  erlapTauLTE(self
-0000a570: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
-0000a580: 2073 656c 662e 5f6f 7665 726c 6170 5461   self._overlapTa
-0000a590: 754c 5445 3d76 616c 7565 0a0a 2020 2020  uLTE=value..    
-0000a5a0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000a5b0: 6620 6f76 6572 6c61 7054 6175 4e4c 5445  f overlapTauNLTE
-0000a5c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000a5d0: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-0000a5e0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-0000a5f0: 656c 662e 5f6f 7665 726c 6170 5461 754e  elf._overlapTauN
-0000a600: 4c54 453d 5b5d 0a20 2020 2020 2020 2020  LTE=[].         
-0000a610: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000a620: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
-0000a630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a640: 2073 656c 662e 5f6f 7665 726c 6170 5461   self._overlapTa
-0000a650: 754e 4c54 452e 6170 7065 6e64 2873 656c  uNLTE.append(sel
-0000a660: 662e 6d6f 6465 6c73 5b69 5d2e 6f76 6572  f.models[i].over
-0000a670: 6c61 7054 6175 4e4c 5445 290a 2020 2020  lapTauNLTE).    
-0000a680: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000a690: 2020 2020 2020 7365 6c66 2e5f 6f76 6572        self._over
-0000a6a0: 6c61 7054 6175 4e4c 5445 3d73 656c 662e  lapTauNLTE=self.
-0000a6b0: 6d6f 6465 6c73 5b30 5d2e 6f76 6572 6c61  models[0].overla
-0000a6c0: 7054 6175 4e4c 5445 0a20 2020 2020 2020  pTauNLTE.       
-0000a6d0: 2072 6574 7572 6e20 7365 6c66 2e5f 6f76   return self._ov
-0000a6e0: 6572 6c61 7054 6175 4e4c 5445 0a0a 2020  erlapTauNLTE..  
-0000a6f0: 2020 406f 7665 726c 6170 5461 754e 4c54    @overlapTauNLT
-0000a700: 452e 7365 7474 6572 0a20 2020 2064 6566  E.setter.    def
-0000a710: 206f 7665 726c 6170 5461 754e 4c54 4528   overlapTauNLTE(
-0000a720: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-0000a730: 2020 2020 2073 656c 662e 5f6f 7665 726c       self._overl
-0000a740: 6170 5461 754e 4c54 453d 7661 6c75 650a  apTauNLTE=value.
-0000a750: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000a760: 2020 2064 6566 2063 6f6e 764f 7665 726c     def convOverl
-0000a770: 6170 5228 7365 6c66 293a 0a20 2020 2020  apR(self):.     
-0000a780: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
-0000a790: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
-0000a7a0: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
-0000a7b0: 6c61 7052 3d5b 5d0a 2020 2020 2020 2020  lapR=[].        
-0000a7c0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000a7d0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
-0000a7e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a7f0: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
-0000a800: 6c61 7052 2e61 7070 656e 6428 7365 6c66  lapR.append(self
-0000a810: 2e6d 6f64 656c 735b 695d 2e63 6f6e 764f  .models[i].convO
-0000a820: 7665 726c 6170 5229 0a20 2020 2020 2020  verlapR).       
-0000a830: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000a840: 2020 2073 656c 662e 5f63 6f6e 764f 7665     self._convOve
-0000a850: 726c 6170 523d 7365 6c66 2e6d 6f64 656c  rlapR=self.model
-0000a860: 735b 305d 2e63 6f6e 764f 7665 726c 6170  s[0].convOverlap
-0000a870: 520a 2020 2020 2020 2020 7265 7475 726e  R.        return
-0000a880: 2073 656c 662e 5f63 6f6e 764f 7665 726c   self._convOverl
-0000a890: 6170 520a 0a20 2020 2040 636f 6e76 4f76  apR..    @convOv
-0000a8a0: 6572 6c61 7052 2e73 6574 7465 720a 2020  erlapR.setter.  
-0000a8b0: 2020 6465 6620 636f 6e76 4f76 6572 6c61    def convOverla
-0000a8c0: 7052 2873 656c 662c 7661 6c75 6529 3a0a  pR(self,value):.
-0000a8d0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-0000a8e0: 6e76 4f76 6572 6c61 7052 3d76 616c 7565  nvOverlapR=value
-0000a8f0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000a900: 2020 2020 6465 6620 6f76 6572 6c61 7052      def overlapR
-0000a910: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000a920: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
-0000a930: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-0000a940: 656c 662e 5f6f 7665 726c 6170 523d 5b5d  elf._overlapR=[]
-0000a950: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000a960: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-0000a970: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
-0000a980: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a990: 5f6f 7665 726c 6170 522e 6170 7065 6e64  _overlapR.append
-0000a9a0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
-0000a9b0: 6f76 6572 6c61 7052 290a 2020 2020 2020  overlapR).      
-0000a9c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000a9d0: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
-0000a9e0: 7052 3d73 656c 662e 6d6f 6465 6c73 5b30  pR=self.models[0
-0000a9f0: 5d2e 6f76 6572 6c61 7052 0a20 2020 2020  ].overlapR.     
-0000aa00: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000aa10: 6f76 6572 6c61 7052 0a0a 2020 2020 406f  overlapR..    @o
-0000aa20: 7665 726c 6170 522e 7365 7474 6572 0a20  verlapR.setter. 
-0000aa30: 2020 2064 6566 206f 7665 726c 6170 5228     def overlapR(
-0000aa40: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-0000aa50: 2020 2020 2073 656c 662e 5f6f 7665 726c       self._overl
-0000aa60: 6170 523d 7661 6c75 650a 0a63 6c61 7373  apR=value..class
-0000aa70: 2073 6c61 623a 0a20 2020 2022 2222 0a20   slab:.    """. 
-0000aa80: 2020 2063 6c61 7373 3a3a 2073 6c61 620a     class:: slab.
-0000aa90: 2020 2020 436c 6173 7320 746f 2068 6f6c      Class to hol
-0000aaa0: 6420 7468 6520 6461 7461 206f 6620 696e  d the data of in
-0000aab0: 6469 7669 6475 616c 2073 6c61 6220 6d6f  dividual slab mo
-0000aac0: 6465 6c73 0a20 2020 2022 2222 0a0a 2020  dels.    """..  
-0000aad0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0000aae0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-0000aaf0: 6c66 2e73 7065 6369 6573 5f6e 756d 6265  lf.species_numbe
-0000ab00: 723d 4e6f 6e65 0a20 2020 2020 2020 2073  r=None.        s
-0000ab10: 656c 662e 6d6f 6465 6c5f 6e75 6d62 6572  elf.model_number
-0000ab20: 3d4e 6f6e 650a 2020 2020 2020 2020 7365  =None.        se
-0000ab30: 6c66 2e4e 483d 4e6f 6e65 0a20 2020 2020  lf.NH=None.     
-0000ab40: 2020 2073 656c 662e 6e43 6f6c 6c3d 4e6f     self.nColl=No
-0000ab50: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-0000ab60: 6e65 3d4e 6f6e 650a 2020 2020 2020 2020  ne=None.        
-0000ab70: 7365 6c66 2e6e 4865 3d4e 6f6e 650a 2020  self.nHe=None.  
-0000ab80: 2020 2020 2020 7365 6c66 2e6e 4849 493d        self.nHII=
-0000ab90: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000aba0: 662e 6e48 493d 4e6f 6e65 0a20 2020 2020  f.nHI=None.     
-0000abb0: 2020 2073 656c 662e 6e48 323d 4e6f 6e65     self.nH2=None
-0000abc0: 0a20 2020 2020 2020 2073 656c 662e 6475  .        self.du
-0000abd0: 7374 5f74 6f5f 6761 733d 4e6f 6e65 0a20  st_to_gas=None. 
-0000abe0: 2020 2020 2020 2073 656c 662e 7674 7572         self.vtur
-0000abf0: 623d 4e6f 6e65 0a20 2020 2020 2020 2073  b=None.        s
-0000ac00: 656c 662e 5467 3d4e 6f6e 650a 2020 2020  elf.Tg=None.    
-0000ac10: 2020 2020 7365 6c66 2e54 643d 4e6f 6e65      self.Td=None
-0000ac20: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
-0000ac30: 6563 6965 735f 6e61 6d65 3d4e 6f6e 650a  ecies_name=None.
-0000ac40: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
-0000ac50: 6369 6573 5f69 6e64 6578 3d4e 6f6e 650a  cies_index=None.
-0000ac60: 2020 2020 2020 2020 7365 6c66 2e61 6275          self.abu
-0000ac70: 6e64 616e 6365 3d4e 6f6e 650a 2020 2020  ndance=None.    
-0000ac80: 2020 2020 7365 6c66 2e64 763d 4e6f 6e65      self.dv=None
-0000ac90: 0a20 2020 2020 2020 2073 656c 662e 6e6c  .        self.nl
-0000aca0: 6576 656c 733d 4e6f 6e65 0a20 2020 2020  evels=None.     
-0000acb0: 2020 2073 656c 662e 6e6c 696e 6573 3d4e     self.nlines=N
-0000acc0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000acd0: 2e6c 696e 6564 6174 613d 4e6f 6e65 0a20  .linedata=None. 
-0000ace0: 2020 2020 2020 2073 656c 662e 6c65 7665         self.leve
-0000acf0: 6c64 6174 613d 4e6f 6e65 0a20 2020 2020  ldata=None.     
-0000ad00: 2020 2073 656c 662e 636f 6e76 5761 7665     self.convWave
-0000ad10: 6c65 6e67 7468 3d4e 6f6e 650a 2020 2020  length=None.    
-0000ad20: 2020 2020 7365 6c66 2e63 6f6e 764c 5445      self.convLTE
-0000ad30: 666c 7578 3d4e 6f6e 650a 2020 2020 2020  flux=None.      
-0000ad40: 2020 7365 6c66 2e63 6f6e 764e 4c54 4566    self.convNLTEf
-0000ad50: 6c75 783d 4e6f 6e65 0a20 2020 2020 2020  lux=None.       
-0000ad60: 2073 656c 662e 636f 6e76 5479 7065 3d4e   self.convType=N
-0000ad70: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000ad80: 2e63 6f6e 7652 3d4e 6f6e 650a 2020 2020  .convR=None.    
-0000ad90: 2020 2020 7365 6c66 2e6f 7665 726c 6170      self.overlap
-0000ada0: 4c54 453d 4e6f 6e65 0a20 2020 2020 2020  LTE=None.       
-0000adb0: 2073 656c 662e 6f76 6572 6c61 704e 4c54   self.overlapNLT
-0000adc0: 453d 4e6f 6e65 0a20 2020 2020 2020 2073  E=None.        s
-0000add0: 656c 662e 6f76 6572 6c61 7054 6175 4c54  elf.overlapTauLT
-0000ade0: 453d 4e6f 6e65 0a20 2020 2020 2020 2073  E=None.        s
-0000adf0: 656c 662e 6f76 6572 6c61 7054 6175 4e4c  elf.overlapTauNL
-0000ae00: 5445 3d4e 6f6e 650a 2020 2020 2020 2020  TE=None.        
-0000ae10: 7365 6c66 2e6f 7665 726c 6170 4672 6571  self.overlapFreq
-0000ae20: 3d4e 6f6e 650a 2020 2020 2020 2020 7365  =None.        se
-0000ae30: 6c66 2e63 6f6e 764f 7665 726c 6170 4c54  lf.convOverlapLT
-0000ae40: 453d 4e6f 6e65 0a20 2020 2020 2020 2073  E=None.        s
-0000ae50: 656c 662e 636f 6e76 4f76 6572 6c61 704e  elf.convOverlapN
-0000ae60: 4c54 453d 4e6f 6e65 0a20 2020 2020 2020  LTE=None.       
-0000ae70: 2073 656c 662e 636f 6e76 4f76 6572 6c61   self.convOverla
-0000ae80: 7046 7265 713d 4e6f 6e65 0a20 2020 2020  pFreq=None.     
-0000ae90: 2020 2073 656c 662e 636f 6e76 4f76 6572     self.convOver
-0000aea0: 6c61 7057 6176 653d 4e6f 6e65 0a20 2020  lapWave=None.   
-0000aeb0: 2020 2020 2073 656c 662e 636f 6e76 4f76       self.convOv
-0000aec0: 6572 6c61 7052 3d31 6535 0a20 2020 2020  erlapR=1e5.     
-0000aed0: 2020 2073 656c 662e 6f76 6572 6c61 7052     self.overlapR
-0000aee0: 3d31 6535 0a0a 2020 2020 6465 6620 5f5f  =1e5..    def __
-0000aef0: 7374 725f 5f28 7365 6c66 293a 0a20 2020  str__(self):.   
-0000af00: 2020 2020 206f 7574 7075 743d 2249 6e66       output="Inf
-0000af10: 6f20 4d6f 6465 6c3a 205c 6e22 0a20 2020  o Model: \n".   
-0000af20: 2020 2020 206f 7574 7075 742b 3d27 7370       output+='sp
-0000af30: 6563 6965 735f 6e75 6d62 6572 3d20 270a  ecies_number= '.
-0000af40: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-0000af50: 7374 7228 7365 6c66 2e73 7065 6369 6573  str(self.species
-0000af60: 5f6e 756d 6265 7229 2b27 5c6e 5c6e 270a  _number)+'\n\n'.
-0000af70: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-0000af80: 276d 6f64 656c 5f6e 756d 6265 7220 203d  'model_number  =
-0000af90: 2027 0a20 2020 2020 2020 206f 7574 7075   '.        outpu
-0000afa0: 742b 3d73 7472 2873 656c 662e 6d6f 6465  t+=str(self.mode
-0000afb0: 6c5f 6e75 6d62 6572 292b 275c 6e5c 6e27  l_number)+'\n\n'
-0000afc0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000afd0: 3d27 4e48 2020 2020 2020 2020 2020 2020  ='NH            
-0000afe0: 3d20 270a 2020 2020 2020 2020 6f75 7470  = '.        outp
-0000aff0: 7574 2b3d 7374 7228 7365 6c66 2e4e 4829  ut+=str(self.NH)
-0000b000: 2b27 5c6e 5c6e 270a 2020 2020 2020 2020  +'\n\n'.        
-0000b010: 6f75 7470 7574 2b3d 276e 436f 6c6c 2020  output+='nColl  
-0000b020: 2020 2020 2020 203d 2027 0a20 2020 2020         = '.     
-0000b030: 2020 206f 7574 7075 742b 3d73 7472 2873     output+=str(s
-0000b040: 656c 662e 6e43 6f6c 6c29 2b27 5c6e 5c6e  elf.nColl)+'\n\n
-0000b050: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
-0000b060: 2b3d 276e 6520 2020 2020 2020 2020 2020  +='ne           
-0000b070: 203d 2027 0a20 2020 2020 2020 206f 7574   = '.        out
-0000b080: 7075 742b 3d73 7472 2873 656c 662e 6e65  put+=str(self.ne
-0000b090: 292b 275c 6e5c 6e27 0a20 2020 2020 2020  )+'\n\n'.       
-0000b0a0: 206f 7574 7075 742b 3d27 6e48 6520 2020   output+='nHe   
-0000b0b0: 2020 2020 2020 2020 3d20 270a 2020 2020          = '.    
-0000b0c0: 2020 2020 6f75 7470 7574 2b3d 7374 7228      output+=str(
-0000b0d0: 7365 6c66 2e6e 4865 292b 275c 6e5c 6e27  self.nHe)+'\n\n'
-0000b0e0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000b0f0: 3d27 6e48 4949 2020 2020 2020 2020 2020  ='nHII          
-0000b100: 3d20 270a 2020 2020 2020 2020 6f75 7470  = '.        outp
-0000b110: 7574 2b3d 7374 7228 7365 6c66 2e6e 4849  ut+=str(self.nHI
-0000b120: 4929 2b27 5c6e 5c6e 270a 2020 2020 2020  I)+'\n\n'.      
-0000b130: 2020 6f75 7470 7574 2b3d 276e 4849 2020    output+='nHI  
-0000b140: 2020 2020 2020 2020 203d 2027 0a20 2020           = '.   
-0000b150: 2020 2020 206f 7574 7075 742b 3d73 7472       output+=str
-0000b160: 2873 656c 662e 6e48 4929 2b27 5c6e 5c6e  (self.nHI)+'\n\n
-0000b170: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
-0000b180: 2b3d 276e 4832 2020 2020 2020 2020 2020  +='nH2          
-0000b190: 203d 2027 0a20 2020 2020 2020 206f 7574   = '.        out
-0000b1a0: 7075 742b 3d73 7472 2873 656c 662e 6e48  put+=str(self.nH
-0000b1b0: 3229 2b27 5c6e 5c6e 270a 2020 2020 2020  2)+'\n\n'.      
-0000b1c0: 2020 6f75 7470 7574 2b3d 2764 7573 745f    output+='dust_
-0000b1d0: 746f 5f67 6173 2020 203d 2027 0a20 2020  to_gas   = '.   
-0000b1e0: 2020 2020 206f 7574 7075 742b 3d73 7472       output+=str
-0000b1f0: 2873 656c 662e 6475 7374 5f74 6f5f 6761  (self.dust_to_ga
-0000b200: 7329 2b27 5c6e 5c6e 270a 2020 2020 2020  s)+'\n\n'.      
-0000b210: 2020 6f75 7470 7574 2b3d 2776 7475 7262    output+='vturb
-0000b220: 2020 2020 2020 2020 203d 2027 0a20 2020           = '.   
-0000b230: 2020 2020 206f 7574 7075 742b 3d73 7472       output+=str
-0000b240: 2873 656c 662e 7674 7572 6229 2b27 5c6e  (self.vturb)+'\n
-0000b250: 5c6e 270a 2020 2020 2020 2020 6f75 7470  \n'.        outp
-0000b260: 7574 2b3d 2754 6720 2020 2020 2020 2020  ut+='Tg         
-0000b270: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
-0000b280: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
-0000b290: 5467 292b 275c 6e5c 6e27 0a20 2020 2020  Tg)+'\n\n'.     
-0000b2a0: 2020 206f 7574 7075 742b 3d27 5464 2020     output+='Td  
-0000b2b0: 2020 2020 2020 2020 2020 3d20 270a 2020            = '.  
-0000b2c0: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
-0000b2d0: 7228 7365 6c66 2e54 6429 2b27 5c6e 5c6e  r(self.Td)+'\n\n
-0000b2e0: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
-0000b2f0: 2b3d 2773 7065 6369 6573 5f6e 616d 6520  +='species_name 
-0000b300: 2020 3d20 270a 2020 2020 2020 2020 6f75    = '.        ou
-0000b310: 7470 7574 2b3d 7365 6c66 2e73 7065 6369  tput+=self.speci
-0000b320: 6573 5f6e 616d 652b 275c 6e5c 6e27 0a20  es_name+'\n\n'. 
-0000b330: 2020 2020 2020 206f 7574 7075 742b 3d27         output+='
-0000b340: 6162 756e 6461 6e63 6520 2020 2020 3d20  abundance     = 
-0000b350: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
-0000b360: 2b3d 7374 7228 7365 6c66 2e61 6275 6e64  +=str(self.abund
-0000b370: 616e 6365 292b 275c 6e5c 6e27 0a20 2020  ance)+'\n\n'.   
-0000b380: 2020 2020 206f 7574 7075 742b 3d27 6476       output+='dv
-0000b390: 2020 2020 2020 2020 2020 2020 3d20 270a              = '.
-0000b3a0: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-0000b3b0: 7374 7228 7365 6c66 2e64 7629 2b27 5c6e  str(self.dv)+'\n
-0000b3c0: 5c6e 270a 2020 2020 2020 2020 6f75 7470  \n'.        outp
-0000b3d0: 7574 2b3d 276e 6c65 7665 6c73 2020 2020  ut+='nlevels    
-0000b3e0: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
-0000b3f0: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
-0000b400: 6e6c 6576 656c 7329 2b27 5c6e 5c6e 270a  nlevels)+'\n\n'.
-0000b410: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
-0000b420: 276e 6c69 6e65 7320 2020 2020 2020 203d  'nlines        =
-0000b430: 2027 0a20 2020 2020 2020 206f 7574 7075   '.        outpu
-0000b440: 742b 3d73 7472 2873 656c 662e 6e6c 696e  t+=str(self.nlin
-0000b450: 6573 292b 275c 6e5c 6e27 0a20 2020 2020  es)+'\n\n'.     
-0000b460: 2020 206f 7574 7075 742b 3d27 636f 6e76     output+='conv
-0000b470: 5479 7065 2020 2020 2020 203d 2027 0a20  Type       = '. 
-0000b480: 2020 2020 2020 206f 7574 7075 742b 3d73         output+=s
-0000b490: 7472 2873 656c 662e 636f 6e76 5479 7065  tr(self.convType
-0000b4a0: 292b 275c 6e5c 6e27 0a20 2020 2020 2020  )+'\n\n'.       
-0000b4b0: 206f 7574 7075 742b 3d27 636f 6e76 5220   output+='convR 
-0000b4c0: 2020 2020 2020 203d 2027 0a20 2020 2020         = '.     
-0000b4d0: 2020 206f 7574 7075 742b 3d73 7472 2873     output+=str(s
-0000b4e0: 656c 662e 636f 6e76 5229 2b27 5c6e 5c6e  elf.convR)+'\n\n
-0000b4f0: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
-0000b500: 206f 7574 7075 740a 0a20 2020 2064 6566   output..    def
-0000b510: 2063 6f6e 766f 6c76 6528 7365 6c66 2c66   convolve(self,f
-0000b520: 7265 715f 6269 6e73 3d4e 6f6e 652c 523d  req_bins=None,R=
-0000b530: 312c 6c61 6d62 6461 5f30 3d31 2c6c 616d  1,lambda_0=1,lam
-0000b540: 6264 615f 6e3d 312c 7672 3d31 3330 302c  bda_n=1,vr=1300,
-0000b550: 4e4c 5445 3d46 616c 7365 2c63 6f6e 765f  NLTE=False,conv_
-0000b560: 7479 7065 3d31 293a 0a20 2020 2020 2020  type=1):.       
-0000b570: 2074 3d27 464c 5445 270a 2020 2020 2020   t='FLTE'.      
-0000b580: 2020 6966 204e 4c54 453a 0a20 2020 2020    if NLTE:.     
-0000b590: 2020 2020 2020 2074 3d27 464e 4c54 4527         t='FNLTE'
-0000b5a0: 0a20 2020 2020 2020 2064 613d 7365 6c66  .        da=self
-0000b5b0: 2e6c 696e 6564 6174 610a 2020 2020 2020  .linedata.      
-0000b5c0: 2020 6966 206c 616d 6264 615f 303d 3d6c    if lambda_0==l
-0000b5d0: 616d 6264 615f 6e3a 0a20 2020 2020 2020  ambda_n:.       
-0000b5e0: 2020 2020 206c 616d 6264 615f 303d 6e70       lambda_0=np
-0000b5f0: 2e61 6d69 6e28 6461 5b27 4748 7a27 5d3e  .amin(da['GHz']>
-0000b600: 632f 6c61 6d62 6461 5f6e 2a31 652d 3329  c/lambda_n*1e-3)
-0000b610: 0a20 2020 2020 2020 2020 2020 206c 616d  .            lam
-0000b620: 6264 615f 6e3d 6e70 2e61 6d61 7828 6461  bda_n=np.amax(da
-0000b630: 5b27 4748 7a27 5d3e 632f 6c61 6d62 6461  ['GHz']>c/lambda
-0000b640: 5f6e 2a31 652d 3329 0a20 2020 2020 2020  _n*1e-3).       
-0000b650: 2020 2020 206c 616d 6264 615f 303d 6c61       lambda_0=la
-0000b660: 6d62 6461 5f30 2a31 302a 2a2d 302e 3035  mbda_0*10**-0.05
-0000b670: 0a20 2020 2020 2020 2020 2020 206c 616d  .            lam
-0000b680: 6264 615f 6e3d 6c61 6d62 6461 5f6e 2a31  bda_n=lambda_n*1
-0000b690: 302a 2a30 2e30 350a 2020 2020 2020 2020  0**0.05.        
-0000b6a0: 6461 5f72 6571 3d64 615b 2864 615b 2747  da_req=da[(da['G
-0000b6b0: 487a 275d 3e63 2f6c 616d 6264 615f 6e2a  Hz']>c/lambda_n*
-0000b6c0: 3165 2d33 2926 2864 615b 2747 487a 275d  1e-3)&(da['GHz']
-0000b6d0: 3c63 2f6c 616d 6264 615f 302a 3165 2d33  <c/lambda_0*1e-3
-0000b6e0: 295d 0a20 2020 2020 2020 2064 615f 7265  )].        da_re
-0000b6f0: 712e 7265 7365 745f 696e 6465 7828 6472  q.reset_index(dr
-0000b700: 6f70 3d54 7275 652c 696e 706c 6163 653d  op=True,inplace=
-0000b710: 5472 7565 290a 2020 2020 2020 2020 6966  True).        if
-0000b720: 2063 6f6e 765f 7479 7065 3d3d 313a 0a20   conv_type==1:. 
-0000b730: 2020 2020 2020 2020 2020 206c 2c66 3d67             l,f=g
-0000b740: 656e 6572 616c 436f 6e76 6f6c 7665 2864  eneralConvolve(d
-0000b750: 615f 7265 715b 745d 2c64 615f 7265 715b  a_req[t],da_req[
-0000b760: 2747 487a 275d 2c52 3d52 2c6c 616d 6264  'GHz'],R=R,lambd
-0000b770: 615f 303d 6c61 6d62 6461 5f30 2c6c 616d  a_0=lambda_0,lam
-0000b780: 6264 615f 6e3d 6c61 6d62 6461 5f6e 290a  bda_n=lambda_n).
-0000b790: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000b7a0: 2020 2020 2020 2020 2020 6c2c 663d 7370            l,f=sp
-0000b7b0: 6563 436f 6e76 6f6c 7665 2864 615f 7265  ecConvolve(da_re
-0000b7c0: 715b 745d 2c64 615f 7265 715b 2747 487a  q[t],da_req['GHz
-0000b7d0: 275d 2c66 7265 715f 6269 6e73 3d66 7265  '],freq_bins=fre
-0000b7e0: 715f 6269 6e73 2c52 3d52 2c6c 616d 6264  q_bins,R=R,lambd
-0000b7f0: 615f 303d 6c61 6d62 6461 5f30 2c6c 616d  a_0=lambda_0,lam
-0000b800: 6264 615f 6e3d 6c61 6d62 6461 5f6e 2c76  bda_n=lambda_n,v
-0000b810: 723d 7672 290a 2020 2020 2020 2020 7365  r=vr).        se
-0000b820: 6c66 2e63 6f6e 7657 6176 656c 656e 6774  lf.convWavelengt
-0000b830: 683d 6c0a 2020 2020 2020 2020 7365 6c66  h=l.        self
-0000b840: 2e63 6f6e 7654 7970 653d 636f 6e76 5f74  .convType=conv_t
-0000b850: 7970 650a 2020 2020 2020 2020 7365 6c66  ype.        self
-0000b860: 2e63 6f6e 7652 3d52 0a20 2020 2020 2020  .convR=R.       
-0000b870: 2069 6620 4e4c 5445 3a0a 2020 2020 2020   if NLTE:.      
-0000b880: 2020 2020 2020 7365 6c66 2e63 6f6e 764e        self.convN
-0000b890: 4c54 4566 6c75 783d 660a 2020 2020 2020  LTEflux=f.      
-0000b8a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000b8b0: 2020 2020 7365 6c66 2e63 6f6e 764c 5445      self.convLTE
-0000b8c0: 666c 7578 3d66 0a0a 2020 2020 6465 6620  flux=f..    def 
-0000b8d0: 636f 6e76 6f6c 7665 5f6f 7665 726c 6170  convolve_overlap
-0000b8e0: 2873 656c 662c 523d 312c 6c61 6d62 6461  (self,R=1,lambda
-0000b8f0: 5f30 3d31 2c6c 616d 6264 615f 6e3d 3129  _0=1,lambda_n=1)
-0000b900: 3a0a 2020 2020 2020 2020 6966 206c 616d  :.        if lam
-0000b910: 6264 615f 303d 3d6c 616d 6264 615f 6e3a  bda_0==lambda_n:
-0000b920: 0a20 2020 2020 2020 2020 2020 206c 616d  .            lam
-0000b930: 6264 615f 303d 6e70 2e61 6d69 6e28 632f  bda_0=np.amin(c/
-0000b940: 7365 6c66 2e6f 7665 726c 6170 4672 6571  self.overlapFreq
-0000b950: 2a31 652d 3329 0a20 2020 2020 2020 2020  *1e-3).         
-0000b960: 2020 206c 616d 6264 615f 6e3d 6e70 2e61     lambda_n=np.a
-0000b970: 6d61 7828 632f 7365 6c66 2e6f 7665 726c  max(c/self.overl
-0000b980: 6170 4672 6571 2a31 652d 3329 0a20 2020  apFreq*1e-3).   
-0000b990: 2020 2020 2020 2020 206c 616d 6264 615f           lambda_
-0000b9a0: 303d 6c61 6d62 6461 5f30 2a31 302a 2a2d  0=lambda_0*10**-
-0000b9b0: 302e 3035 0a20 2020 2020 2020 2020 2020  0.05.           
-0000b9c0: 206c 616d 6264 615f 6e3d 6c61 6d62 6461   lambda_n=lambda
-0000b9d0: 5f6e 2a31 302a 2a30 2e30 350a 2020 2020  _n*10**0.05.    
-0000b9e0: 2020 2020 6d61 736b 3d28 7365 6c66 2e6f      mask=(self.o
-0000b9f0: 7665 726c 6170 4672 6571 3e63 2f6c 616d  verlapFreq>c/lam
-0000ba00: 6264 615f 6e2a 3165 2d33 2926 2873 656c  bda_n*1e-3)&(sel
-0000ba10: 662e 6f76 6572 6c61 7046 7265 713c 632f  f.overlapFreq<c/
-0000ba20: 6c61 6d62 6461 5f30 2a31 652d 3329 0a20  lambda_0*1e-3). 
-0000ba30: 2020 2020 2020 2046 5748 4d3d 7365 6c66         FWHM=self
-0000ba40: 2e6f 7665 726c 6170 522f 522f 322e 3335  .overlapR/R/2.35
-0000ba50: 350a 2020 2020 2020 2020 673d 4761 7573  5.        g=Gaus
-0000ba60: 7369 616e 3144 4b65 726e 656c 2873 7464  sian1DKernel(std
-0000ba70: 6465 763d 4657 484d 2c66 6163 746f 723d  dev=FWHM,factor=
-0000ba80: 3729 0a20 2020 2020 2020 2073 656c 662e  7).        self.
-0000ba90: 636f 6e76 4f76 6572 6c61 704c 5445 3d61  convOverlapLTE=a
-0000baa0: 7079 5f63 6f6e 766f 6c76 6528 7365 6c66  py_convolve(self
-0000bab0: 2e6f 7665 726c 6170 4c54 455b 6d61 736b  .overlapLTE[mask
-0000bac0: 5d2c 6729 0a20 2020 2020 2020 2023 2073  ],g).        # s
-0000bad0: 656c 662e 636f 6e76 4f76 6572 6c61 704e  elf.convOverlapN
-0000bae0: 4c54 453d 6170 795f 636f 6e76 6f6c 7665  LTE=apy_convolve
-0000baf0: 2873 656c 662e 6f76 6572 6c61 704e 4c54  (self.overlapNLT
-0000bb00: 455b 6d61 736b 5d2c 6729 0a20 2020 2020  E[mask],g).     
-0000bb10: 2020 2073 656c 662e 636f 6e76 4f76 6572     self.convOver
-0000bb20: 6c61 7046 7265 713d 7365 6c66 2e6f 7665  lapFreq=self.ove
-0000bb30: 726c 6170 4672 6571 5b6d 6173 6b5d 2a31  rlapFreq[mask]*1
-0000bb40: 2e30 0a20 2020 2020 2020 2073 656c 662e  .0.        self.
-0000bb50: 636f 6e76 4f76 6572 6c61 7057 6176 653d  convOverlapWave=
-0000bb60: 632f 7365 6c66 2e63 6f6e 764f 7665 726c  c/self.convOverl
-0000bb70: 6170 4672 6571 2a31 652d 330a 2020 2020  apFreq*1e-3.    
-0000bb80: 2020 2020 7365 6c66 2e63 6f6e 764f 7665      self.convOve
-0000bb90: 726c 6170 5220 3d20 520a 0a20 2020 2064  rlapR = R..    d
-0000bba0: 6566 2073 686f 7728 7365 6c66 293a 0a20  ef show(self):. 
-0000bbb0: 2020 2020 2020 2070 7269 6e74 2873 656c         print(sel
-0000bbc0: 6629 0a20 2020 2020 2020 2070 7269 6e74  f).        print
-0000bbd0: 2827 6c69 6e65 4461 7461 2020 2020 3d20  ('lineData    = 
-0000bbe0: 2729 0a20 2020 2020 2020 2070 7269 6e74  ').        print
-0000bbf0: 2873 656c 662e 6c69 6e65 6461 7461 290a  (self.linedata).
-0000bc00: 2020 2020 2020 2020 7072 696e 7428 276c          print('l
-0000bc10: 6576 656c 4461 7461 2020 203d 2027 290a  evelData   = ').
-0000bc20: 2020 2020 2020 2020 7072 696e 7428 7365          print(se
-0000bc30: 6c66 2e6c 6576 656c 6461 7461 290a 0a0a  lf.leveldata)...
-0000bc40: 636c 6173 7320 736c 6162 3144 3a0a 2020  class slab1D:.  
-0000bc50: 2020 2222 220a 2020 2020 636c 6173 733a    """.    class:
-0000bc60: 3a20 736c 6162 3144 0a20 2020 2043 6c61  : slab1D.    Cla
-0000bc70: 7373 2074 6f20 686f 6c64 2074 6865 2064  ss to hold the d
-0000bc80: 6174 6120 6f66 2031 4420 736c 6162 206d  ata of 1D slab m
-0000bc90: 6f64 656c 730a 2020 2020 2222 220a 0a20  odels.    """.. 
-0000bca0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0000bcb0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-0000bcc0: 656c 662e 6469 7265 6374 6f72 7920 2020  elf.directory   
-0000bcd0: 2020 2020 2020 2020 3d20 4e6f 6e65 0a20          = None. 
-0000bce0: 2020 2020 2020 2073 656c 662e 666c 7578         self.flux
-0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd00: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-0000bd10: 656c 662e 6672 6571 7565 6e63 7920 2020  elf.frequency   
-0000bd20: 2020 2020 2020 2020 3d20 4e6f 6e65 0a20          = None. 
-0000bd30: 2020 2020 2020 2073 656c 662e 4e73 7065         self.Nspe
-0000bd40: 6369 6573 2020 2020 2020 2020 2020 2020  cies            
-0000bd50: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-0000bd60: 656c 662e 7370 6563 6965 7320 2020 2020  elf.species     
-0000bd70: 2020 2020 2020 2020 3d20 5b5d 0a20 2020          = [].   
-0000bd80: 2020 2020 2073 656c 662e 4e67 7269 6420       self.Ngrid 
-0000bd90: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
-0000bda0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000bdb0: 662e 5220 2020 2020 2020 2020 2020 2020  f.R             
-0000bdc0: 2020 2020 2020 3d20 4e6f 6e65 0a20 2020        = None.   
-0000bdd0: 2020 2020 2073 656c 662e 6772 6964 2020       self.grid  
-0000bde0: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
-0000bdf0: 7064 2e44 6174 6146 7261 6d65 2829 0a20  pd.DataFrame(). 
-0000be00: 2020 2020 2020 2073 656c 662e 736f 7572         self.sour
-0000be10: 6365 5f66 756e 6374 696f 6e20 2020 2020  ce_function     
-0000be20: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-0000be30: 656c 662e 736f 7572 6365 5f66 756e 6374  elf.source_funct
-0000be40: 696f 6e5f 6761 7320 3d20 4e6f 6e65 0a20  ion_gas = None. 
-0000be50: 2020 2020 2020 2073 656c 662e 7461 755f         self.tau_
-0000be60: 6475 7374 2020 2020 2020 2020 2020 2020  dust            
-0000be70: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-0000be80: 656c 662e 7461 755f 6761 7320 2020 2020  elf.tau_gas     
-0000be90: 2020 2020 2020 2020 3d20 4e6f 6e65 0a20          = None. 
-0000bea0: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-0000beb0: 5761 7665 6c65 6e67 7468 2020 2020 2020  Wavelength      
-0000bec0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-0000bed0: 656c 662e 636f 6e76 4672 6571 7565 6e63  elf.convFrequenc
-0000bee0: 7920 2020 2020 2020 3d20 4e6f 6e65 0a20  y       = None. 
-0000bef0: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-0000bf00: 5f66 6c75 7820 2020 2020 2020 2020 2020  _flux           
-0000bf10: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-0000bf20: 656c 662e 636f 6e76 5220 2020 2020 2020  elf.convR       
-0000bf30: 2020 2020 2020 2020 3d20 4e6f 6e65 0a0a          = None..
-0000bf40: 2020 2020 6465 6620 5f5f 7374 725f 5f28      def __str__(
-0000bf50: 7365 6c66 293a 0a20 2020 2020 2020 206f  self):.        o
-0000bf60: 7574 7075 743d 2249 6e66 6f20 4d6f 6465  utput="Info Mode
-0000bf70: 6c3a 205c 6e22 0a20 2020 2020 2020 206f  l: \n".        o
-0000bf80: 7574 7075 742b 3d27 4e75 6d62 6572 206f  utput+='Number o
-0000bf90: 6620 7370 6563 6965 7320 2020 2020 2020  f species       
-0000bfa0: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
-0000bfb0: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
-0000bfc0: 4e73 7065 6369 6573 292b 275c 6e5c 6e27  Nspecies)+'\n\n'
-0000bfd0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000bfe0: 3d27 4772 6964 2073 697a 6520 2020 2020  ='Grid size     
-0000bff0: 2020 2020 2020 2020 2020 2020 203d 2027               = '
-0000c000: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000c010: 3d73 7472 2873 656c 662e 4e67 7269 6429  =str(self.Ngrid)
-0000c020: 2b27 5c6e 5c6e 270a 2020 2020 2020 2020  +'\n\n'.        
-0000c030: 6f75 7470 7574 2b3d 2752 6573 6f6c 7669  output+='Resolvi
-0000c040: 6e67 2070 6f77 6572 206f 6620 7370 6563  ng power of spec
-0000c050: 7472 6120 3d20 270a 2020 2020 2020 2020  tra = '.        
-0000c060: 6f75 7470 7574 2b3d 7374 7228 7365 6c66  output+=str(self
-0000c070: 2e52 292b 275c 6e5c 6e27 0a20 2020 2020  .R)+'\n\n'.     
-0000c080: 2020 206f 7574 7075 742b 3d27 4f75 7470     output+='Outp
-0000c090: 7574 2066 696c 6520 7061 7468 203d 2027  ut file path = '
-0000c0a0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
-0000c0b0: 3d73 7472 2873 656c 662e 6469 7265 6374  =str(self.direct
-0000c0c0: 6f72 7929 2b27 5c6e 5c6e 270a 2020 2020  ory)+'\n\n'.    
-0000c0d0: 2020 2020 7265 7475 726e 206f 7574 7075      return outpu
-0000c0e0: 740a 0a20 2020 2064 6566 2063 6f6e 766f  t..    def convo
-0000c0f0: 6c76 6528 7365 6c66 2c52 3d31 2c6c 616d  lve(self,R=1,lam
-0000c100: 6264 615f 303d 312c 6c61 6d62 6461 5f6e  bda_0=1,lambda_n
-0000c110: 3d31 2c76 6572 626f 7365 3d54 7275 6529  =1,verbose=True)
-0000c120: 3a0a 2020 2020 2020 2020 6966 2076 6572  :.        if ver
-0000c130: 626f 7365 3a20 7072 696e 7428 2243 6f6e  bose: print("Con
-0000c140: 766f 6c76 696e 6720 746f 2022 2c52 290a  volving to ",R).
-0000c150: 2020 2020 2020 2020 6966 206c 616d 6264          if lambd
-0000c160: 615f 303d 3d6c 616d 6264 615f 6e3a 0a20  a_0==lambda_n:. 
-0000c170: 2020 2020 2020 2020 2020 206c 616d 6264             lambd
-0000c180: 615f 303d 6e70 2e61 6d69 6e28 632f 7365  a_0=np.amin(c/se
-0000c190: 6c66 2e66 7265 7175 656e 6379 2a31 652d  lf.frequency*1e-
-0000c1a0: 3329 0a20 2020 2020 2020 2020 2020 206c  3).            l
-0000c1b0: 616d 6264 615f 6e3d 6e70 2e61 6d61 7828  ambda_n=np.amax(
-0000c1c0: 632f 7365 6c66 2e66 7265 7175 656e 6379  c/self.frequency
-0000c1d0: 2a31 652d 3329 0a20 2020 2020 2020 2020  *1e-3).         
-0000c1e0: 2020 206c 616d 6264 615f 303d 6c61 6d62     lambda_0=lamb
-0000c1f0: 6461 5f30 2a31 302a 2a2d 302e 3035 0a20  da_0*10**-0.05. 
-0000c200: 2020 2020 2020 2020 2020 206c 616d 6264             lambd
-0000c210: 615f 6e3d 6c61 6d62 6461 5f6e 2a31 302a  a_n=lambda_n*10*
-0000c220: 2a30 2e30 350a 2020 2020 2020 2020 6d61  *0.05.        ma
-0000c230: 736b 3d28 7365 6c66 2e66 7265 7175 656e  sk=(self.frequen
-0000c240: 6379 3e63 2f6c 616d 6264 615f 6e2a 3165  cy>c/lambda_n*1e
-0000c250: 2d33 2926 2873 656c 662e 6672 6571 7565  -3)&(self.freque
-0000c260: 6e63 793c 632f 6c61 6d62 6461 5f30 2a31  ncy<c/lambda_0*1
-0000c270: 652d 3329 0a20 2020 2020 2020 2046 5748  e-3).        FWH
-0000c280: 4d3d 7365 6c66 2e52 2f52 2f32 2e33 3535  M=self.R/R/2.355
-0000c290: 0a20 2020 2020 2020 2067 3d47 6175 7373  .        g=Gauss
-0000c2a0: 6961 6e31 444b 6572 6e65 6c28 7374 6464  ian1DKernel(stdd
-0000c2b0: 6576 3d46 5748 4d2c 6661 6374 6f72 3d37  ev=FWHM,factor=7
-0000c2c0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-0000c2d0: 6f6e 765f 666c 7578 3d61 7079 5f63 6f6e  onv_flux=apy_con
-0000c2e0: 766f 6c76 6528 7365 6c66 2e66 6c75 785b  volve(self.flux[
-0000c2f0: 6d61 736b 5d2c 6729 0a20 2020 2020 2020  mask],g).       
-0000c300: 2073 656c 662e 636f 6e76 4672 6571 7565   self.convFreque
-0000c310: 6e63 793d 7365 6c66 2e66 7265 7175 656e  ncy=self.frequen
-0000c320: 6379 5b6d 6173 6b5d 2a31 2e30 0a20 2020  cy[mask]*1.0.   
-0000c330: 2020 2020 2073 656c 662e 636f 6e76 5220       self.convR 
-0000c340: 3d20 520a 2020 2020 2020 2020 7365 6c66  = R.        self
-0000c350: 2e63 6f6e 7657 6176 656c 656e 6774 683d  .convWavelength=
-0000c360: 632f 7365 6c66 2e63 6f6e 7646 7265 7175  c/self.convFrequ
-0000c370: 656e 6379 2a31 652d 330a 0a20 2020 2064  ency*1e-3..    d
-0000c380: 6566 2073 686f 7728 7365 6c66 293a 0a20  ef show(self):. 
-0000c390: 2020 2020 2020 2070 7269 6e74 2873 656c         print(sel
-0000c3a0: 6629 0a20 2020 2020 2020 2070 7269 6e74  f).        print
-0000c3b0: 2827 4772 6964 2020 2020 3d20 2729 0a20  ('Grid    = '). 
-0000c3c0: 2020 2020 2020 2070 7269 6e74 2873 656c         print(sel
-0000c3d0: 662e 6772 6964 290a 2020 2020 2020 2020  f.grid).        
-0000c3e0: 7072 696e 7428 2753 6f75 7263 6520 6675  print('Source fu
-0000c3f0: 6e63 7469 6f6e 2020 203d 2027 290a 2020  nction   = ').  
-0000c400: 2020 2020 2020 7072 696e 7428 7365 6c66        print(self
-0000c410: 2e73 6f75 7263 655f 6675 6e63 7469 6f6e  .source_function
-0000c420: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-0000c430: 2747 6173 206f 6e6c 7920 736f 7572 6365  'Gas only source
-0000c440: 2066 756e 6374 696f 6e20 2020 3d20 2729   function   = ')
-0000c450: 0a20 2020 2020 2020 2070 7269 6e74 2873  .        print(s
-0000c460: 656c 662e 736f 7572 6365 5f66 756e 6374  elf.source_funct
-0000c470: 696f 6e5f 6761 7329 0a20 2020 2020 2020  ion_gas).       
-0000c480: 2070 7269 6e74 2827 4475 7374 206f 7074   print('Dust opt
-0000c490: 6963 616c 2064 6570 7468 2020 203d 2027  ical depth   = '
-0000c4a0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-0000c4b0: 7365 6c66 2e74 6175 5f64 7573 7429 0a20  self.tau_dust). 
-0000c4c0: 2020 2020 2020 2070 7269 6e74 2827 4761         print('Ga
-0000c4d0: 7320 6f70 7469 6361 6c20 6465 7074 6820  s optical depth 
-0000c4e0: 2020 3d20 2729 0a20 2020 2020 2020 2070    = ').        p
-0000c4f0: 7269 6e74 2873 656c 662e 7461 755f 6761  rint(self.tau_ga
-0000c500: 7329 0a0a 6465 6620 7265 6164 5f31 445f  s)..def read_1D_
-0000c510: 736c 6162 286d 6f64 656c 5f70 6174 683d  slab(model_path=
-0000c520: 2753 6c61 6252 6573 756c 7473 2e66 6974  'SlabResults.fit
-0000c530: 732e 677a 272c 7665 7262 6f73 653d 5472  s.gz',verbose=Tr
-0000c540: 7565 293a 0a20 2020 2022 2222 0a20 2020  ue):.    """.   
-0000c550: 2046 756e 6374 696f 6e20 746f 2072 6561   Function to rea
-0000c560: 6420 3144 2070 726f 6469 6d6f 2073 6c61  d 1D prodimo sla
-0000c570: 6220 6d6f 6465 6c20 6f75 7470 7574 0a20  b model output. 
-0000c580: 2020 2022 2222 0a20 2020 2069 6620 7665     """.    if ve
-0000c590: 7262 6f73 653a 2070 7269 6e74 2822 5265  rbose: print("Re
-0000c5a0: 6164 696e 6720 3144 2073 6c61 6220 6d6f  ading 1D slab mo
-0000c5b0: 6465 6c20 6f75 7470 7574 2066 726f 6d3a  del output from:
-0000c5c0: 2022 2c6d 6f64 656c 5f70 6174 6829 0a20   ",model_path). 
-0000c5d0: 2020 2069 6620 272e 6669 7473 2e67 7a27     if '.fits.gz'
-0000c5e0: 2069 6e20 6d6f 6465 6c5f 7061 7468 3a0a   in model_path:.
-0000c5f0: 2020 2020 2020 2020 6864 756c 2020 2020          hdul    
-0000c600: 2020 2020 2020 203d 2066 6974 732e 6f70         = fits.op
-0000c610: 656e 286d 6f64 656c 5f70 6174 6829 0a20  en(model_path). 
-0000c620: 2020 2020 2020 2064 6174 6120 2020 2020         data     
-0000c630: 2020 2020 2020 3d20 736c 6162 3144 2829        = slab1D()
-0000c640: 0a20 2020 2020 2020 2064 6174 612e 6469  .        data.di
-0000c650: 7265 6374 6f72 7920 3d20 6d6f 6465 6c5f  rectory = model_
-0000c660: 7061 7468 0a20 2020 2020 2020 2064 6174  path.        dat
-0000c670: 612e 666c 7578 2020 2020 2020 3d20 6864  a.flux      = hd
-0000c680: 756c 5b30 5d2e 6461 7461 2e54 5b3a 2c31  ul[0].data.T[:,1
-0000c690: 5d0a 2020 2020 2020 2020 6461 7461 2e66  ].        data.f
-0000c6a0: 7265 7175 656e 6379 203d 2068 6475 6c5b  requency = hdul[
-0000c6b0: 305d 2e64 6174 612e 545b 3a2c 305d 0a20  0].data.T[:,0]. 
-0000c6c0: 2020 2020 2020 2064 6174 612e 4e73 7065         data.Nspe
-0000c6d0: 6369 6573 2020 3d20 6864 756c 5b30 5d2e  cies  = hdul[0].
-0000c6e0: 6865 6164 6572 5b27 4e53 5045 4349 4553  header['NSPECIES
-0000c6f0: 275d 0a20 2020 2020 2020 2064 6174 612e  '].        data.
-0000c700: 7370 6563 6965 7320 2020 3d20 6864 756c  species   = hdul
-0000c710: 5b30 5d2e 6865 6164 6572 2e63 6f6d 6d65  [0].header.comme
-0000c720: 6e74 735b 274e 5350 4543 4945 5327 5d2e  nts['NSPECIES'].
-0000c730: 7370 6c69 7428 272c 2729 0a20 2020 2020  split(',').     
-0000c740: 2020 2064 6174 612e 4e67 7269 6420 2020     data.Ngrid   
-0000c750: 2020 3d20 6864 756c 5b30 5d2e 6865 6164    = hdul[0].head
-0000c760: 6572 5b27 4e47 5249 4427 5d0a 2020 2020  er['NGRID'].    
-0000c770: 2020 2020 6461 7461 2e52 2020 2020 2020      data.R      
-0000c780: 2020 203d 2068 6475 6c5b 305d 2e68 6561     = hdul[0].hea
-0000c790: 6465 725b 2752 5f4f 564c 5027 5d0a 2020  der['R_OVLP'].  
-0000c7a0: 2020 2020 2020 6966 2028 2839 2b64 6174        if ((9+dat
-0000c7b0: 612e 4e73 7065 6369 6573 2a32 292c 6461  a.Nspecies*2),da
-0000c7c0: 7461 2e4e 6772 6964 2920 3d3d 2068 6475  ta.Ngrid) == hdu
-0000c7d0: 6c5b 315d 2e64 6174 612e 542e 7368 6170  l[1].data.T.shap
-0000c7e0: 653a 0a20 2020 2020 2020 2020 2020 2067  e:.            g
-0000c7f0: 7269 6420 3d20 6864 756c 5b31 5d2e 6461  rid = hdul[1].da
-0000c800: 7461 0a20 2020 2020 2020 2020 2020 2064  ta.            d
-0000c810: 6174 612e 6772 6964 5b27 647a 275d 2020  ata.grid['dz']  
-0000c820: 2020 3d20 6772 6964 5b3a 2c30 5d0a 2020    = grid[:,0].  
-0000c830: 2020 2020 2020 2020 2020 6461 7461 2e67            data.g
-0000c840: 7269 645b 2776 7475 7262 275d 203d 2067  rid['vturb'] = g
-0000c850: 7269 645b 3a2c 315d 0a20 2020 2020 2020  rid[:,1].       
-0000c860: 2020 2020 2064 6174 612e 6772 6964 5b27       data.grid['
-0000c870: 6e64 275d 2020 2020 3d20 6772 6964 5b3a  nd']    = grid[:
-0000c880: 2c32 5d0a 2020 2020 2020 2020 2020 2020  ,2].            
-0000c890: 6461 7461 2e67 7269 645b 2754 6427 5d20  data.grid['Td'] 
-0000c8a0: 2020 203d 2067 7269 645b 3a2c 335d 0a20     = grid[:,3]. 
-0000c8b0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-0000c8c0: 6772 6964 5b27 6e48 3227 5d20 2020 3d20  grid['nH2']   = 
-0000c8d0: 6772 6964 5b3a 2c34 5d0a 2020 2020 2020  grid[:,4].      
-0000c8e0: 2020 2020 2020 6461 7461 2e67 7269 645b        data.grid[
-0000c8f0: 276e 4849 275d 2020 203d 2067 7269 645b  'nHI']   = grid[
-0000c900: 3a2c 355d 0a20 2020 2020 2020 2020 2020  :,5].           
-0000c910: 2064 6174 612e 6772 6964 5b27 6e48 4949   data.grid['nHII
-0000c920: 275d 2020 3d20 6772 6964 5b3a 2c36 5d0a  ']  = grid[:,6].
-0000c930: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000c940: 2e67 7269 645b 276e 4865 275d 2020 203d  .grid['nHe']   =
-0000c950: 2067 7269 645b 3a2c 375d 0a20 2020 2020   grid[:,7].     
-0000c960: 2020 2020 2020 2064 6174 612e 6772 6964         data.grid
-0000c970: 5b27 6e65 6c65 6327 5d20 3d20 6772 6964  ['nelec'] = grid
-0000c980: 5b3a 2c38 5d0a 2020 2020 2020 2020 2020  [:,8].          
-0000c990: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-0000c9a0: 2864 6174 612e 4e73 7065 6369 6573 293a  (data.Nspecies):
-0000c9b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c9c0: 206b 6579 203d 2027 6e27 2b64 6174 612e   key = 'n'+data.
-0000c9d0: 7370 6563 6965 735b 695d 0a20 2020 2020  species[i].     
-0000c9e0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-0000c9f0: 6772 6964 5b6b 6579 5d20 3d20 6772 6964  grid[key] = grid
-0000ca00: 5b3a 2c39 2b69 5d0a 2020 2020 2020 2020  [:,9+i].        
-0000ca10: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000ca20: 6765 2864 6174 612e 4e73 7065 6369 6573  ge(data.Nspecies
-0000ca30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000ca40: 2020 206b 6579 203d 2027 5467 5f27 2b64     key = 'Tg_'+d
-0000ca50: 6174 612e 7370 6563 6965 735b 695d 0a20  ata.species[i]. 
-0000ca60: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000ca70: 6174 612e 6772 6964 5b6b 6579 5d20 3d20  ata.grid[key] = 
-0000ca80: 6772 6964 5b3a 2c39 2b64 6174 612e 4e73  grid[:,9+data.Ns
-0000ca90: 7065 6369 6573 2b69 5d0a 2020 2020 2020  pecies+i].      
-0000caa0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000cab0: 2020 2020 7261 6973 6520 4173 7365 7274      raise Assert
-0000cac0: 696f 6e45 7272 6f72 2827 4772 6964 2069  ionError('Grid i
-0000cad0: 6e20 6f75 7470 7574 2066 696c 6520 646f  n output file do
-0000cae0: 6573 206e 6f74 206d 6174 6368 2074 6865  es not match the
-0000caf0: 2061 6374 7561 6c20 6772 6964 206f 7574   actual grid out
-0000cb00: 7075 7420 6172 7261 7927 290a 2020 2020  put array').    
-0000cb10: 2020 2020 0a20 2020 2020 2020 2069 6620      .        if 
-0000cb20: 286c 656e 2864 6174 612e 6672 6571 7565  (len(data.freque
-0000cb30: 6e63 7929 2c64 6174 612e 4e67 7269 6429  ncy),data.Ngrid)
-0000cb40: 203d 3d20 6864 756c 5b32 5d2e 6461 7461   == hdul[2].data
-0000cb50: 2e54 2e73 6861 7065 3a0a 2020 2020 2020  .T.shape:.      
-0000cb60: 2020 2020 2020 6461 7461 2e73 6f75 7263        data.sourc
-0000cb70: 655f 6675 6e63 7469 6f6e 203d 2068 6475  e_function = hdu
-0000cb80: 6c5b 325d 2e64 6174 610a 2020 2020 2020  l[2].data.      
-0000cb90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000cba0: 2020 2020 7261 6973 6520 4173 7365 7274      raise Assert
-0000cbb0: 696f 6e45 7272 6f72 2827 536f 7572 6365  ionError('Source
-0000cbc0: 2066 756e 6374 696f 6e20 6772 6964 2069   function grid i
-0000cbd0: 6e20 6f75 7470 7574 2066 696c 6520 646f  n output file do
-0000cbe0: 6573 206e 6f74 206d 6174 6368 2074 6865  es not match the
-0000cbf0: 2073 7061 7469 616c 2061 6e64 2066 7265   spatial and fre
-0000cc00: 7175 656e 6379 2067 7269 6420 7369 7a65  quency grid size
-0000cc10: 2729 0a20 2020 2020 2020 200a 2020 2020  ').        .    
-0000cc20: 2020 2020 6966 2028 6c65 6e28 6461 7461      if (len(data
-0000cc30: 2e66 7265 7175 656e 6379 292c 6461 7461  .frequency),data
-0000cc40: 2e4e 6772 6964 2920 3d3d 2068 6475 6c5b  .Ngrid) == hdul[
-0000cc50: 335d 2e64 6174 612e 542e 7368 6170 653a  3].data.T.shape:
-0000cc60: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000cc70: 612e 736f 7572 6365 5f66 756e 6374 696f  a.source_functio
-0000cc80: 6e5f 6761 7320 3d20 6864 756c 5b33 5d2e  n_gas = hdul[3].
-0000cc90: 6461 7461 0a20 2020 2020 2020 2065 6c73  data.        els
-0000cca0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000ccb0: 6169 7365 2041 7373 6572 7469 6f6e 4572  aise AssertionEr
-0000ccc0: 726f 7228 2747 6173 2073 6f75 7263 6520  ror('Gas source 
-0000ccd0: 6675 6e63 7469 6f6e 2067 7269 6420 696e  function grid in
-0000cce0: 206f 7574 7075 7420 6669 6c65 2064 6f65   output file doe
-0000ccf0: 7320 6e6f 7420 6d61 7463 6820 7468 6520  s not match the 
-0000cd00: 7370 6174 6961 6c20 616e 6420 6672 6571  spatial and freq
-0000cd10: 7565 6e63 7920 6772 6964 2073 697a 6527  uency grid size'
-0000cd20: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-0000cd30: 2020 2069 6620 286c 656e 2864 6174 612e     if (len(data.
-0000cd40: 6672 6571 7565 6e63 7929 2c64 6174 612e  frequency),data.
-0000cd50: 4e67 7269 6429 203d 3d20 6864 756c 5b34  Ngrid) == hdul[4
-0000cd60: 5d2e 6461 7461 2e54 2e73 6861 7065 3a0a  ].data.T.shape:.
-0000cd70: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000cd80: 2e74 6175 5f64 7573 7420 3d20 6864 756c  .tau_dust = hdul
-0000cd90: 5b34 5d2e 6461 7461 0a20 2020 2020 2020  [4].data.       
-0000cda0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000cdb0: 2020 2072 6169 7365 2041 7373 6572 7469     raise Asserti
-0000cdc0: 6f6e 4572 726f 7228 2744 7573 7420 6f70  onError('Dust op
-0000cdd0: 7469 6361 6c20 6465 7074 6820 6772 6964  tical depth grid
-0000cde0: 2069 6e20 6f75 7470 7574 2066 696c 6520   in output file 
-0000cdf0: 646f 6573 206e 6f74 206d 6174 6368 2074  does not match t
-0000ce00: 6865 2073 7061 7469 616c 2061 6e64 2066  he spatial and f
-0000ce10: 7265 7175 656e 6379 2067 7269 6420 7369  requency grid si
-0000ce20: 7a65 2729 0a20 2020 2020 2020 200a 2020  ze').        .  
-0000ce30: 2020 2020 2020 6966 2028 6c65 6e28 6461        if (len(da
-0000ce40: 7461 2e66 7265 7175 656e 6379 292c 6461  ta.frequency),da
-0000ce50: 7461 2e4e 6772 6964 2920 3d3d 2068 6475  ta.Ngrid) == hdu
-0000ce60: 6c5b 355d 2e64 6174 612e 542e 7368 6170  l[5].data.T.shap
-0000ce70: 653a 0a20 2020 2020 2020 2020 2020 2064  e:.            d
-0000ce80: 6174 612e 7461 755f 6761 7320 3d20 6864  ata.tau_gas = hd
-0000ce90: 756c 5b35 5d2e 6461 7461 0a20 2020 2020  ul[5].data.     
-0000cea0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000ceb0: 2020 2020 2072 6169 7365 2041 7373 6572       raise Asser
-0000cec0: 7469 6f6e 4572 726f 7228 2747 6173 206f  tionError('Gas o
-0000ced0: 7074 6963 616c 2064 6570 7468 2067 7269  ptical depth gri
-0000cee0: 6420 696e 206f 7574 7075 7420 6669 6c65  d in output file
-0000cef0: 2064 6f65 7320 6e6f 7420 6d61 7463 6820   does not match 
-0000cf00: 7468 6520 7370 6174 6961 6c20 616e 6420  the spatial and 
-0000cf10: 6672 6571 7565 6e63 7920 6772 6964 2073  frequency grid s
-0000cf20: 697a 6527 290a 2020 2020 656c 7365 3a0a  ize').    else:.
-0000cf30: 2020 2020 2020 2020 6461 7461 5f72 6561          data_rea
-0000cf40: 6420 3d20 6e70 2e6c 6f61 6474 7874 286d  d = np.loadtxt(m
-0000cf50: 6f64 656c 5f70 6174 682c 736b 6970 726f  odel_path,skipro
-0000cf60: 7773 3d31 290a 2020 2020 2020 2020 6461  ws=1).        da
-0000cf70: 7461 2020 2020 2020 2020 2020 203d 2073  ta           = s
-0000cf80: 6c61 6231 4428 290a 2020 2020 2020 2020  lab1D().        
-0000cf90: 6461 7461 2e64 6972 6563 746f 7279 203d  data.directory =
-0000cfa0: 206d 6f64 656c 5f70 6174 680a 2020 2020   model_path.    
-0000cfb0: 2020 2020 6461 7461 2e66 6c75 7820 2020      data.flux   
-0000cfc0: 2020 203d 2064 6174 615f 7265 6164 5b3a     = data_read[:
-0000cfd0: 2c31 5d0a 2020 2020 2020 2020 6461 7461  ,1].        data
-0000cfe0: 2e66 7265 7175 656e 6379 203d 2064 6174  .frequency = dat
-0000cff0: 615f 7265 6164 5b3a 2c30 5d0a 2020 2020  a_read[:,0].    
-0000d000: 7265 7475 726e 2864 6174 6129 0a0a 6465  return(data)..de
-0000d010: 6620 7265 6164 5f73 6c61 6228 6d6f 6465  f read_slab(mode
-0000d020: 6c5f 7061 7468 3d27 536c 6162 5265 7375  l_path='SlabResu
-0000d030: 6c74 732e 6f75 7427 2c76 6572 626f 7365  lts.out',verbose
-0000d040: 3d54 7275 652c 7368 6f72 745f 666f 726d  =True,short_form
-0000d050: 6174 3d46 616c 7365 293a 0a20 2020 2022  at=False):.    "
-0000d060: 2222 0a20 2020 2046 756e 6374 696f 6e20  "".    Function 
-0000d070: 746f 2072 6561 6420 736c 6162 206d 6f64  to read slab mod
-0000d080: 656c 206f 7574 7075 740a 2020 2020 2222  el output.    ""
-0000d090: 220a 2020 2020 6966 2069 7369 6e73 7461  ".    if isinsta
-0000d0a0: 6e63 6528 6d6f 6465 6c5f 7061 7468 2c6c  nce(model_path,l
-0000d0b0: 6973 7429 3a0a 2020 2020 2020 2020 6461  ist):.        da
-0000d0c0: 7461 3d73 6c61 625f 6461 7461 2829 0a20  ta=slab_data(). 
-0000d0d0: 2020 2020 2020 2064 6174 612e 6469 7265         data.dire
-0000d0e0: 6374 6f72 793d 6d6f 6465 6c5f 7061 7468  ctory=model_path
-0000d0f0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-0000d100: 6e20 6d6f 6465 6c5f 7061 7468 3a0a 2020  n model_path:.  
-0000d110: 2020 2020 2020 2020 2020 7264 6174 613d            rdata=
-0000d120: 7265 6164 5f73 6c61 6228 692c 7665 7262  read_slab(i,verb
-0000d130: 6f73 653d 7665 7262 6f73 652c 7368 6f72  ose=verbose,shor
-0000d140: 745f 666f 726d 6174 3d73 686f 7274 5f66  t_format=short_f
-0000d150: 6f72 6d61 7429 0a20 2020 2020 2020 2020  ormat).         
-0000d160: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-0000d170: 6528 7264 6174 612e 6e6d 6f64 656c 7329  e(rdata.nmodels)
-0000d180: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d190: 2020 6461 7461 2e61 6464 5f6d 6f64 656c    data.add_model
-0000d1a0: 2872 6461 7461 2e6d 6f64 656c 735b 6a5d  (rdata.models[j]
-0000d1b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000d1c0: 2864 6174 6129 0a0a 2020 2020 6966 2076  (data)..    if v
-0000d1d0: 6572 626f 7365 3a20 7072 696e 7428 2252  erbose: print("R
-0000d1e0: 6561 6469 6e67 2073 6c61 6220 6d6f 6465  eading slab mode
-0000d1f0: 6c20 6f75 7470 7574 2066 726f 6d3a 2022  l output from: "
-0000d200: 2c6d 6f64 656c 5f70 6174 6829 0a20 2020  ,model_path).   
-0000d210: 2066 3d6f 7065 6e28 6d6f 6465 6c5f 7061   f=open(model_pa
-0000d220: 7468 290a 2020 2020 6461 7461 3d73 6c61  th).    data=sla
-0000d230: 625f 6461 7461 2829 0a20 2020 206e 6d6f  b_data().    nmo
-0000d240: 6465 6c73 3d69 6e74 2866 2e72 6561 646c  dels=int(f.readl
-0000d250: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
-0000d260: 290a 2020 2020 6461 7461 2e64 6972 6563  ).    data.direc
-0000d270: 746f 7279 3d6d 6f64 656c 5f70 6174 680a  tory=model_path.
-0000d280: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000d290: 6765 286e 6d6f 6465 6c73 293a 0a23 2020  ge(nmodels):.#  
-0000d2a0: 2020 2020 2020 2074 656d 706f 2020 2020         tempo    
-0000d2b0: 2020 2020 2020 2020 2020 2020 3d20 2020              =   
-0000d2c0: 736c 6162 2829 0a20 2020 2020 2020 2074  slab().        t
-0000d2d0: 656d 706f 5f6d 6f64 656c 5f6e 756d 6265  empo_model_numbe
-0000d2e0: 723d 696e 7428 662e 7265 6164 6c69 6e65  r=int(f.readline
-0000d2f0: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
-0000d300: 2020 2020 2020 206e 7370 6563 6965 733d         nspecies=
-0000d310: 696e 7428 662e 7265 6164 6c69 6e65 2829  int(f.readline()
-0000d320: 2e73 706c 6974 2829 5b30 5d29 0a23 2020  .split()[0]).#  
-0000d330: 2020 2020 2020 2074 656d 706f 2e73 7065         tempo.spe
-0000d340: 6369 6573 5f6e 756d 6265 7220 3d20 2020  cies_number =   
-0000d350: 696e 7428 662e 7265 6164 6c69 6e65 2829  int(f.readline()
-0000d360: 2e73 706c 6974 2829 5b30 5d29 0a20 2020  .split()[0]).   
-0000d370: 2020 2020 2074 656d 706f 5f6e 4874 6f74       tempo_nHtot
-0000d380: 3d66 6c6f 6174 2866 2e72 6561 646c 696e  =float(f.readlin
-0000d390: 6528 292e 7370 6c69 7428 295b 305d 290a  e().split()[0]).
-0000d3a0: 2020 2020 2020 2020 7465 6d70 6f5f 6761          tempo_ga
-0000d3b0: 7344 656e 733d 666c 6f61 7428 662e 7265  sDens=float(f.re
-0000d3c0: 6164 6c69 6e65 2829 2e73 706c 6974 2829  adline().split()
-0000d3d0: 5b30 5d29 0a20 2020 2020 2020 2074 656d  [0]).        tem
-0000d3e0: 706f 5f6e 656c 6563 3d66 6c6f 6174 2866  po_nelec=float(f
-0000d3f0: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
-0000d400: 7428 295b 305d 290a 2020 2020 2020 2020  t()[0]).        
-0000d410: 7465 6d70 6f5f 6e48 653d 666c 6f61 7428  tempo_nHe=float(
-0000d420: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
-0000d430: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
-0000d440: 2074 656d 706f 5f6e 4849 493d 666c 6f61   tempo_nHII=floa
-0000d450: 7428 662e 7265 6164 6c69 6e65 2829 2e73  t(f.readline().s
-0000d460: 706c 6974 2829 5b30 5d29 0a20 2020 2020  plit()[0]).     
-0000d470: 2020 2074 656d 706f 5f6e 4849 3d66 6c6f     tempo_nHI=flo
-0000d480: 6174 2866 2e72 6561 646c 696e 6528 292e  at(f.readline().
-0000d490: 7370 6c69 7428 295b 305d 290a 2020 2020  split()[0]).    
-0000d4a0: 2020 2020 7465 6d70 6f5f 6e48 323d 666c      tempo_nH2=fl
-0000d4b0: 6f61 7428 662e 7265 6164 6c69 6e65 2829  oat(f.readline()
-0000d4c0: 2e73 706c 6974 2829 5b30 5d29 0a20 2020  .split()[0]).   
-0000d4d0: 2020 2020 2074 656d 706f 5f64 7573 745f       tempo_dust_
-0000d4e0: 746f 5f67 6173 3d66 6c6f 6174 2866 2e72  to_gas=float(f.r
-0000d4f0: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
-0000d500: 295b 305d 290a 2020 2020 2020 2020 7465  )[0]).        te
-0000d510: 6d70 6f5f 7674 7572 623d 666c 6f61 7428  mpo_vturb=float(
-0000d520: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
-0000d530: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
-0000d540: 2074 656d 706f 5f54 673d 666c 6f61 7428   tempo_Tg=float(
-0000d550: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
-0000d560: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
-0000d570: 2074 656d 706f 5f54 643d 666c 6f61 7428   tempo_Td=float(
-0000d580: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
-0000d590: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
-0000d5a0: 2069 6620 7368 6f72 745f 666f 726d 6174   if short_format
-0000d5b0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0000d5c0: 7220 6a20 696e 2072 616e 6765 286e 7370  r j in range(nsp
-0000d5d0: 6563 6965 7329 3a0a 2020 2020 2020 2020  ecies):.        
-0000d5e0: 2020 2020 2020 2020 7465 6d70 6f3d 736c          tempo=sl
-0000d5f0: 6162 2829 0a20 2020 2020 2020 2020 2020  ab().           
-0000d600: 2020 2020 2074 656d 706f 2e6d 6f64 656c       tempo.model
-0000d610: 5f6e 756d 6265 723d 7465 6d70 6f5f 6d6f  _number=tempo_mo
-0000d620: 6465 6c5f 6e75 6d62 6572 0a20 2020 2020  del_number.     
-0000d630: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000d640: 2e4e 483d 7465 6d70 6f5f 6e48 746f 740a  .NH=tempo_nHtot.
-0000d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d660: 7465 6d70 6f2e 6e43 6f6c 6c3d 7465 6d70  tempo.nColl=temp
-0000d670: 6f5f 6761 7344 656e 730a 2020 2020 2020  o_gasDens.      
-0000d680: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000d690: 6e65 3d74 656d 706f 5f6e 656c 6563 0a20  ne=tempo_nelec. 
-0000d6a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000d6b0: 656d 706f 2e6e 4865 3d74 656d 706f 5f6e  empo.nHe=tempo_n
-0000d6c0: 4865 0a20 2020 2020 2020 2020 2020 2020  He.             
-0000d6d0: 2020 2074 656d 706f 2e6e 4849 493d 7465     tempo.nHII=te
-0000d6e0: 6d70 6f5f 6e48 4949 0a20 2020 2020 2020  mpo_nHII.       
-0000d6f0: 2020 2020 2020 2020 2074 656d 706f 2e6e           tempo.n
-0000d700: 4849 3d74 656d 706f 5f6e 4849 0a20 2020  HI=tempo_nHI.   
-0000d710: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0000d720: 706f 2e6e 4832 3d74 656d 706f 5f6e 4832  po.nH2=tempo_nH2
-0000d730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d740: 2074 656d 706f 2e64 7573 745f 746f 5f67   tempo.dust_to_g
-0000d750: 6173 3d74 656d 706f 5f64 7573 745f 746f  as=tempo_dust_to
-0000d760: 5f67 6173 0a20 2020 2020 2020 2020 2020  _gas.           
-0000d770: 2020 2020 2074 656d 706f 2e76 7475 7262       tempo.vturb
-0000d780: 3d74 656d 706f 5f76 7475 7262 0a20 2020  =tempo_vturb.   
-0000d790: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0000d7a0: 706f 2e54 673d 7465 6d70 6f5f 5467 0a20  po.Tg=tempo_Tg. 
-0000d7b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000d7c0: 656d 706f 2e54 643d 7465 6d70 6f5f 5464  empo.Td=tempo_Td
-0000d7d0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d7e0: 2020 7465 6d70 6f2e 7370 6563 6965 735f    tempo.species_
-0000d7f0: 696e 6465 783d 696e 7428 662e 7265 6164  index=int(f.read
-0000d800: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
-0000d810: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0000d820: 2020 2074 656d 706f 2e73 7065 6369 6573     tempo.species
-0000d830: 5f6e 756d 6265 723d 6a2b 310a 2020 2020  _number=j+1.    
-0000d840: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000d850: 6f2e 7370 6563 6965 735f 6e61 6d65 3d66  o.species_name=f
-0000d860: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
-0000d870: 7428 295b 305d 0a20 2020 2020 2020 2020  t()[0].         
-0000d880: 2020 2020 2020 2074 656d 706f 2e61 6275         tempo.abu
-0000d890: 6e64 616e 6365 3d66 6c6f 6174 2866 2e72  ndance=float(f.r
-0000d8a0: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
-0000d8b0: 295b 305d 290a 2020 2020 2020 2020 2020  )[0]).          
-0000d8c0: 2020 2020 2020 7465 6d70 6f2e 6476 3d66        tempo.dv=f
-0000d8d0: 6c6f 6174 2866 2e72 6561 646c 696e 6528  loat(f.readline(
-0000d8e0: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
-0000d8f0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000d900: 6d70 6f2e 6e6c 696e 6573 3d69 6e74 2866  mpo.nlines=int(f
-0000d910: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
-0000d920: 7428 295b 305d 290a 2020 2020 2020 2020  t()[0]).        
-0000d930: 2020 2020 2020 2020 6c69 6e65 733d 662e          lines=f.
-0000d940: 7265 6164 6c69 6e65 2829 0a0a 2020 2020  readline()..    
-0000d950: 2020 2020 2020 2020 2020 2020 2320 7465              # te
-0000d960: 6d70 6f2e 6e6c 696e 6573 3d4e 6f6e 650a  mpo.nlines=None.
-0000d970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d980: 7465 6d70 6f2e 6c69 6e65 6461 7461 3d4e  tempo.linedata=N
-0000d990: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000d9a0: 2020 2020 7465 6d70 6f2e 6c65 7665 6c64      tempo.leveld
-0000d9b0: 6174 613d 4e6f 6e65 0a20 2020 2020 2020  ata=None.       
-0000d9c0: 2020 2020 2020 2020 2074 656d 706f 2e63           tempo.c
-0000d9d0: 6f6e 7657 6176 656c 656e 6774 683d 4e6f  onvWavelength=No
-0000d9e0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-0000d9f0: 2020 2074 656d 706f 2e63 6f6e 764c 5445     tempo.convLTE
-0000da00: 666c 7578 3d4e 6f6e 650a 2020 2020 2020  flux=None.      
-0000da10: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000da20: 636f 6e76 4e4c 5445 666c 7578 3d4e 6f6e  convNLTEflux=Non
-0000da30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000da40: 2020 7465 6d70 6f2e 636f 6e76 5479 7065    tempo.convType
-0000da50: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
-0000da60: 2020 2020 2020 7465 6d70 6f2e 636f 6e76        tempo.conv
-0000da70: 523d 4e6f 6e65 0a0a 2020 2020 2020 2020  R=None..        
-0000da80: 2020 2020 2020 2020 6461 743d 5b5d 0a20          dat=[]. 
-0000da90: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000daa0: 2066 6f72 206b 2069 6e20 7261 6e67 6528   for k in range(
-0000dab0: 7465 6d70 6f2e 6e6c 6576 656c 7329 3a0a  tempo.nlevels):.
-0000dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dad0: 2320 2020 2020 6461 745b 305d 5b6b 2c3a  #     dat[0][k,:
-0000dae0: 5d3d 6e70 2e61 7361 7272 6179 285b 666c  ]=np.asarray([fl
-0000daf0: 6f61 7428 7829 2066 6f72 2078 2069 6e20  oat(x) for x in 
-0000db00: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
-0000db10: 6974 2829 5d29 0a20 2020 2020 2020 2020  it()]).         
-0000db20: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0000db30: 2020 2020 2020 2020 2320 6c69 6e65 733d          # lines=
-0000db40: 662e 7265 6164 6c69 6e65 2829 0a20 2020  f.readline().   
-0000db50: 2020 2020 2020 2020 2020 2020 2023 206c               # l
-0000db60: 696e 6573 3d66 2e72 6561 646c 696e 6528  ines=f.readline(
-0000db70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000db80: 2020 6461 743d 6e70 2e7a 6572 6f73 2828    dat=np.zeros((
-0000db90: 7465 6d70 6f2e 6e6c 696e 6573 2c34 2929  tempo.nlines,4))
-0000dba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dbb0: 2073 6c61 624f 7574 466f 726d 6174 3d5b   slabOutFormat=[
-0000dbc0: 382c 3134 2c31 352c 3135 5d0a 2020 2020  8,14,15,15].    
-0000dbd0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000dbe0: 6b20 696e 2072 616e 6765 2874 656d 706f  k in range(tempo
-0000dbf0: 2e6e 6c69 6e65 7329 3a0a 2020 2020 2020  .nlines):.      
-0000dc00: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000dc10: 6e65 5265 6164 3d5b 5d0a 2020 2020 2020  neRead=[].      
-0000dc20: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000dc30: 6e65 733d 662e 7265 6164 6c69 6e65 2829  nes=f.readline()
-0000dc40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dc50: 2020 2020 206c 3d30 0a20 2020 2020 2020       l=0.       
-0000dc60: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000dc70: 206c 656e 6774 6820 696e 2073 6c61 624f   length in slabO
-0000dc80: 7574 466f 726d 6174 3a0a 2020 2020 2020  utFormat:.      
-0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dca0: 2020 6c69 6e65 5265 6164 2e61 7070 656e    lineRead.appen
-0000dcb0: 6428 6c69 6e65 735b 6c3a 6c2b 6c65 6e67  d(lines[l:l+leng
-0000dcc0: 7468 5d29 0a20 2020 2020 2020 2020 2020  th]).           
-0000dcd0: 2020 2020 2020 2020 2020 2020 206c 2b3d               l+=
-0000dce0: 6c65 6e67 7468 0a20 2020 2020 2020 2020  length.         
-0000dcf0: 2020 2020 2020 2020 2020 2064 6174 5b6b             dat[k
-0000dd00: 2c3a 5d3d 6e70 2e61 7361 7272 6179 285b  ,:]=np.asarray([
-0000dd10: 666c 6f61 7428 7829 2066 6f72 2078 2069  float(x) for x i
-0000dd20: 6e20 6c69 6e65 5265 6164 5d29 0a20 2020  n lineRead]).   
-0000dd30: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-0000dd40: 6544 6174 613d 7064 2e44 6174 6146 7261  eData=pd.DataFra
-0000dd50: 6d65 2864 6174 2c63 6f6c 756d 6e73 3d5b  me(dat,columns=[
-0000dd60: 2769 272c 2747 487a 272c 2746 4e4c 5445  'i','GHz','FNLTE
-0000dd70: 272c 2746 4c54 4527 5d29 0a20 2020 2020  ','FLTE']).     
-0000dd80: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000dd90: 2e6c 696e 6564 6174 613d 6c69 6e65 4461  .linedata=lineDa
-0000dda0: 7461 0a20 2020 2020 2020 2020 2020 2020  ta.             
-0000ddb0: 2020 2064 6174 612e 6164 645f 6d6f 6465     data.add_mode
-0000ddc0: 6c28 7465 6d70 6f29 0a20 2020 2020 2020  l(tempo).       
-0000ddd0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000dde0: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-0000ddf0: 6528 6e73 7065 6369 6573 293a 0a20 2020  e(nspecies):.   
-0000de00: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0000de10: 706f 3d73 6c61 6228 290a 2020 2020 2020  po=slab().      
-0000de20: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000de30: 6d6f 6465 6c5f 6e75 6d62 6572 3d74 656d  model_number=tem
-0000de40: 706f 5f6d 6f64 656c 5f6e 756d 6265 720a  po_model_number.
-0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de60: 7465 6d70 6f2e 4e48 3d74 656d 706f 5f6e  tempo.NH=tempo_n
-0000de70: 4874 6f74 0a20 2020 2020 2020 2020 2020  Htot.           
-0000de80: 2020 2020 2074 656d 706f 2e6e 436f 6c6c       tempo.nColl
-0000de90: 3d74 656d 706f 5f67 6173 4465 6e73 0a20  =tempo_gasDens. 
-0000dea0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000deb0: 656d 706f 2e6e 653d 7465 6d70 6f5f 6e65  empo.ne=tempo_ne
-0000dec0: 6c65 630a 2020 2020 2020 2020 2020 2020  lec.            
-0000ded0: 2020 2020 7465 6d70 6f2e 6e48 653d 7465      tempo.nHe=te
-0000dee0: 6d70 6f5f 6e48 650a 2020 2020 2020 2020  mpo_nHe.        
-0000def0: 2020 2020 2020 2020 7465 6d70 6f2e 6e48          tempo.nH
-0000df00: 4949 3d74 656d 706f 5f6e 4849 490a 2020  II=tempo_nHII.  
-0000df10: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000df20: 6d70 6f2e 6e48 493d 7465 6d70 6f5f 6e48  mpo.nHI=tempo_nH
-0000df30: 490a 2020 2020 2020 2020 2020 2020 2020  I.              
-0000df40: 2020 7465 6d70 6f2e 6e48 323d 7465 6d70    tempo.nH2=temp
-0000df50: 6f5f 6e48 320a 2020 2020 2020 2020 2020  o_nH2.          
-0000df60: 2020 2020 2020 7465 6d70 6f2e 6475 7374        tempo.dust
-0000df70: 5f74 6f5f 6761 733d 7465 6d70 6f5f 6475  _to_gas=tempo_du
-0000df80: 7374 5f74 6f5f 6761 730a 2020 2020 2020  st_to_gas.      
-0000df90: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000dfa0: 7674 7572 623d 7465 6d70 6f5f 7674 7572  vturb=tempo_vtur
-0000dfb0: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
-0000dfc0: 2020 7465 6d70 6f2e 5467 3d74 656d 706f    tempo.Tg=tempo
-0000dfd0: 5f54 670a 2020 2020 2020 2020 2020 2020  _Tg.            
-0000dfe0: 2020 2020 7465 6d70 6f2e 5464 3d74 656d      tempo.Td=tem
-0000dff0: 706f 5f54 640a 0a20 2020 2020 2020 2020  po_Td..         
-0000e000: 2020 2020 2020 2074 656d 706f 2e73 7065         tempo.spe
-0000e010: 6369 6573 5f69 6e64 6578 3d69 6e74 2866  cies_index=int(f
-0000e020: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
-0000e030: 7428 295b 305d 290a 2020 2020 2020 2020  t()[0]).        
-0000e040: 2020 2020 2020 2020 7465 6d70 6f2e 7370          tempo.sp
-0000e050: 6563 6965 735f 6e75 6d62 6572 3d6a 2b31  ecies_number=j+1
-0000e060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e070: 2074 656d 706f 2e73 7065 6369 6573 5f6e   tempo.species_n
-0000e080: 616d 653d 662e 7265 6164 6c69 6e65 2829  ame=f.readline()
-0000e090: 2e73 706c 6974 2829 5b30 5d0a 2020 2020  .split()[0].    
-0000e0a0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000e0b0: 6f2e 6162 756e 6461 6e63 653d 666c 6f61  o.abundance=floa
-0000e0c0: 7428 662e 7265 6164 6c69 6e65 2829 2e73  t(f.readline().s
-0000e0d0: 706c 6974 2829 5b30 5d29 0a20 2020 2020  plit()[0]).     
-0000e0e0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
-0000e0f0: 2e64 763d 666c 6f61 7428 662e 7265 6164  .dv=float(f.read
-0000e100: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
-0000e110: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0000e120: 2020 2074 656d 706f 2e6e 6c65 7665 6c73     tempo.nlevels
-0000e130: 3d69 6e74 2866 2e72 6561 646c 696e 6528  =int(f.readline(
-0000e140: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
-0000e150: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000e160: 6e65 733d 662e 7265 6164 6c69 6e65 2829  nes=f.readline()
-0000e170: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e180: 2020 7465 6d70 6f2e 6e6c 696e 6573 3d4e    tempo.nlines=N
-0000e190: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000e1a0: 2020 2020 7465 6d70 6f2e 6c69 6e65 6461      tempo.lineda
-0000e1b0: 7461 3d4e 6f6e 650a 2020 2020 2020 2020  ta=None.        
-0000e1c0: 2020 2020 2020 2020 7465 6d70 6f2e 6c65          tempo.le
-0000e1d0: 7665 6c64 6174 613d 4e6f 6e65 0a20 2020  veldata=None.   
-0000e1e0: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0000e1f0: 706f 2e63 6f6e 7657 6176 656c 656e 6774  po.convWavelengt
-0000e200: 683d 4e6f 6e65 0a20 2020 2020 2020 2020  h=None.         
-0000e210: 2020 2020 2020 2074 656d 706f 2e63 6f6e         tempo.con
-0000e220: 764c 5445 666c 7578 3d4e 6f6e 650a 2020  vLTEflux=None.  
-0000e230: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000e240: 6d70 6f2e 636f 6e76 4e4c 5445 666c 7578  mpo.convNLTEflux
-0000e250: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
-0000e260: 2020 2020 2020 7465 6d70 6f2e 636f 6e76        tempo.conv
-0000e270: 5479 7065 3d4e 6f6e 650a 2020 2020 2020  Type=None.      
-0000e280: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000e290: 636f 6e76 523d 4e6f 6e65 0a0a 2020 2020  convR=None..    
-0000e2a0: 2020 2020 2020 2020 2020 2020 6461 743d              dat=
-0000e2b0: 5b6e 702e 7a65 726f 7328 2874 656d 706f  [np.zeros((tempo
-0000e2c0: 2e6e 6c65 7665 6c73 2c38 2929 2c5b 5d2c  .nlevels,8)),[],
-0000e2d0: 5b5d 5d0a 2020 2020 2020 2020 2020 2020  []].            
-0000e2e0: 2020 2020 666f 7220 6b20 696e 2072 616e      for k in ran
-0000e2f0: 6765 2874 656d 706f 2e6e 6c65 7665 6c73  ge(tempo.nlevels
-0000e300: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000e310: 2020 2020 2020 2064 6174 5b30 5d5b 6b2c         dat[0][k,
-0000e320: 3a5d 3d6e 702e 6173 6172 7261 7928 5b66  :]=np.asarray([f
-0000e330: 6c6f 6174 2878 2920 666f 7220 7820 696e  loat(x) for x in
-0000e340: 2066 2e72 6561 646c 696e 6528 292e 7370   f.readline().sp
-0000e350: 6c69 7428 295d 290a 2020 2020 2020 2020  lit()]).        
-0000e360: 2020 2020 2020 2020 7465 6d70 6f2e 6e6c          tempo.nl
-0000e370: 696e 6573 3d69 6e74 2866 2e72 6561 646c  ines=int(f.readl
-0000e380: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
-0000e390: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e3a0: 2020 6c69 6e65 733d 662e 7265 6164 6c69    lines=f.readli
-0000e3b0: 6e65 2829 0a20 2020 2020 2020 2020 2020  ne().           
-0000e3c0: 2020 2020 206c 696e 6573 3d66 2e72 6561       lines=f.rea
-0000e3d0: 646c 696e 6528 290a 2020 2020 2020 2020  dline().        
-0000e3e0: 2020 2020 2020 2020 6461 745b 315d 3d6e          dat[1]=n
-0000e3f0: 702e 7a65 726f 7328 2874 656d 706f 2e6e  p.zeros((tempo.n
-0000e400: 6c69 6e65 732c 3233 2929 0a20 2020 2020  lines,23)).     
-0000e410: 2020 2020 2020 2020 2020 2073 6c61 624f             slabO
-0000e420: 7574 466f 726d 6174 3d5b 392c 392c 392c  utFormat=[9,9,9,
-0000e430: 352c 352c 352c 3135 2c31 352c 3135 2c31  5,5,5,15,15,15,1
-0000e440: 352c 3135 2c31 352c 3135 2c31 352c 3135  5,15,15,15,15,15
-0000e450: 2c31 352c 3135 2c31 352c 3135 2c31 352c  ,15,15,15,15,15,
-0000e460: 3135 2c31 352c 3135 2c32 312c 3231 2c32  15,15,15,21,21,2
-0000e470: 312c 3231 5d0a 2020 2020 2020 2020 2020  1,21].          
-0000e480: 2020 2020 2020 666f 7220 6b20 696e 2072        for k in r
-0000e490: 616e 6765 2874 656d 706f 2e6e 6c69 6e65  ange(tempo.nline
-0000e4a0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000e4b0: 2020 2020 2020 2020 6c69 6e65 5265 6164          lineRead
-0000e4c0: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
-0000e4d0: 2020 2020 2020 2020 6c69 6e65 733d 662e          lines=f.
-0000e4e0: 7265 6164 6c69 6e65 2829 0a20 2020 2020  readline().     
-0000e4f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000e500: 3d30 0a20 2020 2020 2020 2020 2020 2020  =0.             
-0000e510: 2020 2020 2020 2066 6f72 206c 656e 6774         for lengt
-0000e520: 6820 696e 2073 6c61 624f 7574 466f 726d  h in slabOutForm
-0000e530: 6174 3a0a 2020 2020 2020 2020 2020 2020  at:.            
-0000e540: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-0000e550: 5265 6164 2e61 7070 656e 6428 6c69 6e65  Read.append(line
-0000e560: 735b 6c3a 6c2b 6c65 6e67 7468 5d29 0a20  s[l:l+length]). 
-0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e580: 2020 2020 2020 206c 2b3d 6c65 6e67 7468         l+=length
-0000e590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e5a0: 2020 2020 2064 6174 5b31 5d5b 6b2c 3a5d       dat[1][k,:]
-0000e5b0: 3d6e 702e 6173 6172 7261 7928 5b66 6c6f  =np.asarray([flo
-0000e5c0: 6174 2878 2920 666f 7220 7820 696e 206c  at(x) for x in l
-0000e5d0: 696e 6552 6561 645b 303a 2d34 5d5d 290a  ineRead[0:-4]]).
-0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5f0: 2020 2020 6461 745b 325d 2e61 7070 656e      dat[2].appen
-0000e600: 6428 5b61 2e73 7472 6970 2829 2066 6f72  d([a.strip() for
-0000e610: 2061 2069 6e20 6c69 6e65 5265 6164 5b2d   a in lineRead[-
-0000e620: 343a 5d5d 290a 0a20 2020 2020 2020 2020  4:]])..         
-0000e630: 2020 2020 2020 206c 696e 6544 6174 613d         lineData=
-0000e640: 7064 2e44 6174 6146 7261 6d65 2864 6174  pd.DataFrame(dat
-0000e650: 5b31 5d2c 636f 6c75 6d6e 733d 5b27 6927  [1],columns=['i'
-0000e660: 2c27 7527 2c27 6c27 2c27 6527 2c27 7627  ,'u','l','e','v'
-0000e670: 2c27 4a27 2c27 6775 272c 2745 7527 2c27  ,'J','gu','Eu','
-0000e680: 4127 2c27 4227 2c27 4748 7a27 2c27 7461  A','B','GHz','ta
-0000e690: 7544 272c 274a 6261 636b 272c 2770 6f70  uD','Jback','pop
-0000e6a0: 272c 276c 7465 706f 7027 2c27 7461 754e  ','ltepop','tauN
-0000e6b0: 4c54 4527 2c27 7461 754c 5445 272c 2762  LTE','tauLTE','b
-0000e6c0: 4e4c 5445 272c 2762 4c54 4527 2c27 704e  NLTE','bLTE','pN
-0000e6d0: 4c54 4527 2c27 704c 5445 272c 2746 4e4c  LTE','pLTE','FNL
-0000e6e0: 5445 272c 2746 4c54 4527 5d29 0a20 2020  TE','FLTE']).   
-0000e6f0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-0000e700: 6544 6174 615b 2767 6c6f 6261 6c5f 7527  eData['global_u'
-0000e710: 5d3d 5b61 5b30 5d20 666f 7220 6120 696e  ]=[a[0] for a in
-0000e720: 2064 6174 5b32 5d5d 0a20 2020 2020 2020   dat[2]].       
-0000e730: 2020 2020 2020 2020 206c 696e 6544 6174           lineDat
-0000e740: 615b 2767 6c6f 6261 6c5f 6c27 5d3d 5b61  a['global_l']=[a
-0000e750: 5b31 5d20 666f 7220 6120 696e 2064 6174  [1] for a in dat
-0000e760: 5b32 5d5d 0a20 2020 2020 2020 2020 2020  [2]].           
-0000e770: 2020 2020 206c 696e 6544 6174 615b 276c       lineData['l
-0000e780: 6f63 616c 5f75 275d 3d5b 615b 325d 2066  ocal_u']=[a[2] f
-0000e790: 6f72 2061 2069 6e20 6461 745b 325d 5d0a  or a in dat[2]].
-0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7b0: 6c69 6e65 4461 7461 5b27 6c6f 6361 6c5f  lineData['local_
-0000e7c0: 6c27 5d3d 5b61 5b33 5d20 666f 7220 6120  l']=[a[3] for a 
-0000e7d0: 696e 2064 6174 5b32 5d5d 0a20 2020 2020  in dat[2]].     
-0000e7e0: 2020 2020 2020 2020 2020 206c 6576 4461             levDa
-0000e7f0: 7461 3d70 642e 4461 7461 4672 616d 6528  ta=pd.DataFrame(
-0000e800: 6461 745b 305d 2c63 6f6c 756d 6e73 3d5b  dat[0],columns=[
-0000e810: 2769 272c 2767 272c 2745 272c 2770 6f70  'i','g','E','pop
-0000e820: 272c 276c 7465 706f 7027 2c27 6527 2c27  ','ltepop','e','
-0000e830: 7627 2c27 4a27 5d29 0a20 2020 2020 2020  v','J']).       
-0000e840: 2020 2020 2020 2020 2074 656d 706f 2e6c           tempo.l
-0000e850: 696e 6564 6174 613d 6c69 6e65 4461 7461  inedata=lineData
-0000e860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e870: 2074 656d 706f 2e6c 6576 656c 6461 7461   tempo.leveldata
-0000e880: 3d6c 6576 4461 7461 0a20 2020 2020 2020  =levData.       
-0000e890: 2020 2020 2020 2020 2064 6174 612e 6164           data.ad
-0000e8a0: 645f 6d6f 6465 6c28 7465 6d70 6f29 0a20  d_model(tempo). 
-0000e8b0: 2020 2072 6574 7572 6e28 6461 7461 290a     return(data).
-0000e8c0: 0a64 6566 2072 6561 645f 6f76 6572 6c61  .def read_overla
-0000e8d0: 705f 7370 6563 7472 6128 7061 7468 3d27  p_spectra(path='
-0000e8e0: 536c 6162 4f76 6572 6c61 702e 6f75 7427  SlabOverlap.out'
-0000e8f0: 2c76 6572 626f 7365 3d54 7275 6529 3a0a  ,verbose=True):.
-0000e900: 2020 2020 0a20 2020 2069 6620 6973 696e      .    if isin
-0000e910: 7374 616e 6365 2870 6174 682c 6c69 7374  stance(path,list
-0000e920: 293a 0a20 2020 2020 2020 2064 6174 613d  ):.        data=
-0000e930: 736c 6162 5f64 6174 6128 290a 2020 2020  slab_data().    
-0000e940: 2020 2020 6461 7461 2e64 6972 6563 746f      data.directo
-0000e950: 7279 3d70 6174 680a 2020 2020 2020 2020  ry=path.        
-0000e960: 666f 7220 6920 696e 2070 6174 683a 0a20  for i in path:. 
-0000e970: 2020 2020 2020 2020 2020 2072 6461 7461             rdata
-0000e980: 3d72 6561 645f 6f76 6572 6c61 705f 7370  =read_overlap_sp
-0000e990: 6563 7472 6128 692c 7665 7262 6f73 653d  ectra(i,verbose=
-0000e9a0: 7665 7262 6f73 6529 0a20 2020 2020 2020  verbose).       
-0000e9b0: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
-0000e9c0: 6e67 6528 7264 6174 612e 6e6d 6f64 656c  nge(rdata.nmodel
-0000e9d0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000e9e0: 2020 2020 6461 7461 2e61 6464 5f6d 6f64      data.add_mod
-0000e9f0: 656c 2872 6461 7461 2e6d 6f64 656c 735b  el(rdata.models[
-0000ea00: 6a5d 290a 2020 2020 2020 2020 7265 7475  j]).        retu
-0000ea10: 726e 2864 6174 6129 0a20 2020 200a 2020  rn(data).    .  
-0000ea20: 2020 6966 2076 6572 626f 7365 3a20 7072    if verbose: pr
-0000ea30: 696e 7428 2252 6561 6469 6e67 2073 6c61  int("Reading sla
-0000ea40: 6220 6c69 6e65 206f 7665 726c 6170 206d  b line overlap m
-0000ea50: 6f64 656c 206f 7574 7075 7420 6672 6f6d  odel output from
-0000ea60: 3a20 222c 7061 7468 290a 2020 2020 6966  : ",path).    if
-0000ea70: 2027 2e66 6974 732e 677a 2720 696e 2070   '.fits.gz' in p
-0000ea80: 6174 683a 0a20 2020 2020 2020 2068 6475  ath:.        hdu
-0000ea90: 6c20 3d20 6669 7473 2e6f 7065 6e28 7061  l = fits.open(pa
-0000eaa0: 7468 290a 2020 2020 2020 2020 6461 7461  th).        data
-0000eab0: 3d73 6c61 625f 6461 7461 2829 0a20 2020  =slab_data().   
-0000eac0: 2020 2020 206e 6d6f 6465 6c73 3d68 6475       nmodels=hdu
-0000ead0: 6c5b 305d 2e68 6561 6465 725b 274e 4d4f  l[0].header['NMO
-0000eae0: 4445 4c53 275d 0a20 2020 2020 2020 2064  DELS'].        d
-0000eaf0: 6174 612e 6469 7265 6374 6f72 793d 7061  ata.directory=pa
-0000eb00: 7468 0a20 2020 2020 2020 2066 6f72 2069  th.        for i
-0000eb10: 2069 6e20 7261 6e67 6528 6e6d 6f64 656c   in range(nmodel
-0000eb20: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000eb30: 7465 6d70 6f20 2020 2020 2020 2020 2020  tempo           
-0000eb40: 2020 2020 203d 2020 2073 6c61 6228 290a       =   slab().
-0000eb50: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000eb60: 6f5f 6d6f 6465 6c5f 6e75 6d62 6572 3d68  o_model_number=h
-0000eb70: 6475 6c5b 692b 315d 2e68 6561 6465 725b  dul[i+1].header[
-0000eb80: 274d 4f44 454c 275d 0a20 2020 2020 2020  'MODEL'].       
-0000eb90: 2020 2020 2074 656d 706f 5f4e 6c69 6e65       tempo_Nline
-0000eba0: 3d68 6475 6c5b 692b 315d 2e68 6561 6465  =hdul[i+1].heade
-0000ebb0: 725b 274e 4c49 4e45 275d 2020 2020 200a  r['NLINE']     .
-0000ebc0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000ebd0: 6f5f 523d 6864 756c 5b69 2b31 5d2e 6865  o_R=hdul[i+1].he
-0000ebe0: 6164 6572 5b27 525f 4f56 4c50 275d 0a20  ader['R_OVLP']. 
-0000ebf0: 2020 2020 2020 2020 2020 2064 6174 7461             datta
-0000ec00: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-0000ec10: 2020 7465 6d70 6f2e 6f76 6572 6c61 7046    tempo.overlapF
-0000ec20: 7265 7120 2020 203d 2068 6475 6c5b 692b  req    = hdul[i+
-0000ec30: 315d 2e64 6174 615b 3a2c 2d31 5d0a 2020  1].data[:,-1].  
-0000ec40: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000ec50: 6f76 6572 6c61 704c 5445 2020 2020 203d  overlapLTE     =
-0000ec60: 2068 6475 6c5b 692b 315d 2e64 6174 615b   hdul[i+1].data[
-0000ec70: 3a2c 305d 0a20 2020 2020 2020 2020 2020  :,0].           
-0000ec80: 2074 656d 706f 2e6f 7665 726c 6170 5461   tempo.overlapTa
-0000ec90: 754c 5445 2020 3d20 6864 756c 5b69 2b31  uLTE  = hdul[i+1
-0000eca0: 5d2e 6461 7461 5b3a 2c31 5d0a 2020 2020  ].data[:,1].    
-0000ecb0: 2020 2020 2020 2020 7465 6d70 6f2e 6f76          tempo.ov
-0000ecc0: 6572 6c61 704e 4c54 4520 2020 203d 2068  erlapNLTE    = h
-0000ecd0: 6475 6c5b 692b 315d 2e64 6174 615b 3a2c  dul[i+1].data[:,
-0000ece0: 325d 0a20 2020 2020 2020 2020 2020 2074  2].            t
-0000ecf0: 656d 706f 2e6f 7665 726c 6170 5461 754e  empo.overlapTauN
-0000ed00: 4c54 4520 3d20 6864 756c 5b69 2b31 5d2e  LTE = hdul[i+1].
-0000ed10: 6461 7461 5b3a 2c33 5d0a 2020 2020 2020  data[:,3].      
-0000ed20: 2020 2020 2020 7465 6d70 6f2e 6f76 6572        tempo.over
-0000ed30: 6c61 7052 2020 2020 2020 203d 2074 656d  lapR       = tem
-0000ed40: 706f 5f52 0a20 2020 2020 2020 2020 2020  po_R.           
-0000ed50: 2074 656d 706f 2e6d 6f64 656c 5f6e 756d   tempo.model_num
-0000ed60: 6265 7220 2020 3d20 6864 756c 5b69 2b31  ber   = hdul[i+1
-0000ed70: 5d2e 6865 6164 6572 5b27 4d4f 4445 4c27  ].header['MODEL'
-0000ed80: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
-0000ed90: 6d70 6f2e 5467 2020 2020 2020 2020 2020  mpo.Tg          
-0000eda0: 2020 203d 2068 6475 6c5b 692b 315d 2e68     = hdul[i+1].h
-0000edb0: 6561 6465 725b 2754 4727 5d0a 2020 2020  eader['TG'].    
-0000edc0: 2020 2020 2020 2020 7465 6d70 6f2e 5464          tempo.Td
-0000edd0: 2020 2020 2020 2020 2020 2020 203d 2068               = h
-0000ede0: 6475 6c5b 692b 315d 2e68 6561 6465 725b  dul[i+1].header[
-0000edf0: 2754 4427 5d0a 2020 2020 2020 2020 2020  'TD'].          
-0000ee00: 2020 7465 6d70 6f2e 7674 7572 6220 2020    tempo.vturb   
-0000ee10: 2020 2020 2020 203d 2068 6475 6c5b 692b         = hdul[i+
-0000ee20: 315d 2e68 6561 6465 725b 2756 5455 5242  1].header['VTURB
-0000ee30: 275d 0a20 2020 2020 2020 2020 2020 2074  '].            t
-0000ee40: 656d 706f 2e4e 4820 2020 2020 2020 2020  empo.NH         
-0000ee50: 2020 2020 3d20 6864 756c 5b69 2b31 5d2e      = hdul[i+1].
-0000ee60: 6865 6164 6572 5b27 4e48 544f 5427 5d0a  header['NHTOT'].
-0000ee70: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000ee80: 2e61 6464 5f6d 6f64 656c 2874 656d 706f  .add_model(tempo
-0000ee90: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-0000eea0: 7072 696e 7428 2772 6561 6420 272c 692c  print('read ',i,
-0000eeb0: 2720 6d6f 6465 6c27 290a 2020 2020 656c  ' model').    el
-0000eec0: 7365 3a0a 2020 2020 2020 2020 663d 6f70  se:.        f=op
-0000eed0: 656e 2870 6174 6829 0a20 2020 2020 2020  en(path).       
-0000eee0: 2064 6174 613d 736c 6162 5f64 6174 6128   data=slab_data(
-0000eef0: 290a 2020 2020 2020 2020 6e6d 6f64 656c  ).        nmodel
-0000ef00: 733d 696e 7428 662e 7265 6164 6c69 6e65  s=int(f.readline
-0000ef10: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
-0000ef20: 2020 2020 2020 2064 6174 612e 6469 7265         data.dire
-0000ef30: 6374 6f72 793d 7061 7468 0a20 2020 2020  ctory=path.     
-0000ef40: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000ef50: 6528 6e6d 6f64 656c 7329 3a0a 2020 2020  e(nmodels):.    
-0000ef60: 2020 2020 2020 2020 7465 6d70 6f20 2020          tempo   
-0000ef70: 2020 2020 2020 2020 2020 2020 203d 2020               =  
-0000ef80: 2073 6c61 6228 290a 2020 2020 2020 2020   slab().        
-0000ef90: 2020 2020 7465 6d70 6f5f 6d6f 6465 6c5f      tempo_model_
-0000efa0: 6e75 6d62 6572 3d69 6e74 2866 2e72 6561  number=int(f.rea
-0000efb0: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
-0000efc0: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-0000efd0: 7465 6d70 6f5f 4e6c 696e 653d 696e 7428  tempo_Nline=int(
-0000efe0: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
-0000eff0: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
-0000f000: 2020 2020 2074 656d 706f 5f52 3d66 6c6f       tempo_R=flo
-0000f010: 6174 2866 2e72 6561 646c 696e 6528 292e  at(f.readline().
-0000f020: 7370 6c69 7428 295b 305d 290a 2020 2020  split()[0]).    
-0000f030: 2020 2020 2020 2020 6461 7474 6120 3d20          datta = 
-0000f040: 5b5d 0a20 2020 2020 2020 2020 2020 206c  [].            l
-0000f050: 696e 6573 3d66 2e72 6561 646c 696e 6528  ines=f.readline(
-0000f060: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-0000f070: 7220 6a20 696e 2072 616e 6765 2874 656d  r j in range(tem
-0000f080: 706f 5f4e 6c69 6e65 293a 0a20 2020 2020  po_Nline):.     
-0000f090: 2020 2020 2020 2020 2020 206c 696e 6573             lines
-0000f0a0: 3d66 2e72 6561 646c 696e 6528 290a 2020  =f.readline().  
-0000f0b0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000f0c0: 7474 612e 6170 7065 6e64 286e 702e 6172  tta.append(np.ar
-0000f0d0: 7261 7928 6c69 6e65 732e 7370 6c69 7428  ray(lines.split(
-0000f0e0: 292c 6474 7970 653d 666c 6f61 7429 290a  ),dtype=float)).
-0000f0f0: 2020 2020 2020 2020 2020 2020 6461 7474              datt
-0000f100: 6120 3d20 6e70 2e61 7272 6179 2864 6174  a = np.array(dat
-0000f110: 7461 290a 2020 2020 2020 2020 2020 2020  ta).            
-0000f120: 7465 6d70 6f2e 6f76 6572 6c61 7046 7265  tempo.overlapFre
-0000f130: 7120 2020 203d 2064 6174 7461 5b3a 2c30  q    = datta[:,0
-0000f140: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
-0000f150: 6d70 6f2e 6f76 6572 6c61 704c 5445 2020  mpo.overlapLTE  
-0000f160: 2020 203d 2064 6174 7461 5b3a 2c31 5d0a     = datta[:,1].
-0000f170: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000f180: 6f2e 6f76 6572 6c61 7054 6175 4c54 4520  o.overlapTauLTE 
-0000f190: 203d 2064 6174 7461 5b3a 2c32 5d0a 2020   = datta[:,2].  
-0000f1a0: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
-0000f1b0: 6f76 6572 6c61 704e 4c54 4520 2020 203d  overlapNLTE    =
-0000f1c0: 2064 6174 7461 5b3a 2c33 5d0a 2020 2020   datta[:,3].    
-0000f1d0: 2020 2020 2020 2020 7465 6d70 6f2e 6f76          tempo.ov
-0000f1e0: 6572 6c61 7054 6175 4e4c 5445 203d 2064  erlapTauNLTE = d
-0000f1f0: 6174 7461 5b3a 2c34 5d0a 2020 2020 2020  atta[:,4].      
-0000f200: 2020 2020 2020 7465 6d70 6f2e 6f76 6572        tempo.over
-0000f210: 6c61 7052 2020 2020 2020 203d 2074 656d  lapR       = tem
-0000f220: 706f 5f52 0a20 2020 2020 2020 2020 2020  po_R.           
-0000f230: 2064 6174 612e 6164 645f 6d6f 6465 6c28   data.add_model(
-0000f240: 7465 6d70 6f29 0a20 2020 2020 2020 2020  tempo).         
-0000f250: 2020 206c 696e 6573 3d66 2e72 6561 646c     lines=f.readl
-0000f260: 696e 6528 290a 2020 2020 2020 2020 2020  ine().          
-0000f270: 2020 2320 7072 696e 7428 2772 6561 6420    # print('read 
-0000f280: 272c 692c 2720 6d6f 6465 6c27 290a 0a20  ',i,' model').. 
-0000f290: 2020 2072 6574 7572 6e28 6461 7461 290a     return(data).
-0000f2a0: 0a64 6566 2073 7065 6343 6f6e 766f 6c76  .def specConvolv
-0000f2b0: 6528 6c69 6e65 5374 7265 6e67 7468 732c  e(lineStrengths,
-0000f2c0: 6c69 6e65 4672 6571 2c66 7265 715f 6269  lineFreq,freq_bi
-0000f2d0: 6e73 3d4e 6f6e 652c 523d 312c 6c61 6d62  ns=None,R=1,lamb
-0000f2e0: 6461 5f30 3d31 2c6c 616d 6264 615f 6e3d  da_0=1,lambda_n=
-0000f2f0: 312c 7672 3d31 3330 3029 3a0a 2020 2020  1,vr=1300):.    
-0000f300: 6750 6572 633d 6c61 6d62 6461 2078 2c6d  gPerc=lambda x,m
-0000f310: 2c73 3a20 7365 7266 2828 782d 6d29 2f73  ,s: serf((x-m)/s
-0000f320: 292a 302e 352b 302e 350a 2020 2020 6e75  )*0.5+0.5.    nu
-0000f330: 5f69 6a3d 6c69 6e65 4672 6571 2a31 6539  _ij=lineFreq*1e9
-0000f340: 0a20 2020 2069 6620 6c61 6d62 6461 5f6e  .    if lambda_n
-0000f350: 3d3d 6c61 6d62 6461 5f30 3a0a 2020 2020  ==lambda_0:.    
-0000f360: 2020 2020 6c61 6d62 6461 5f6e 3d6e 702e      lambda_n=np.
-0000f370: 616d 6178 2863 2f6e 755f 696a 2a31 6536  amax(c/nu_ij*1e6
-0000f380: 292a 320a 2020 2020 6966 2074 7970 6528  )*2.    if type(
-0000f390: 6672 6571 5f62 696e 7329 3d3d 7479 7065  freq_bins)==type
-0000f3a0: 284e 6f6e 6529 3a0a 2020 2020 2020 2020  (None):.        
-0000f3b0: 6e75 3d67 656e 6572 6174 655f 6772 6964  nu=generate_grid
-0000f3c0: 2852 3d52 2c6c 616d 6264 615f 303d 6c61  (R=R,lambda_0=la
-0000f3d0: 6d62 6461 5f30 2c6c 616d 6264 615f 6e3d  mbda_0,lambda_n=
-0000f3e0: 6c61 6d62 6461 5f6e 292a 3165 390a 2020  lambda_n)*1e9.  
-0000f3f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000f400: 6672 6571 5f62 696e 733d 6e70 2e63 6f6e  freq_bins=np.con
-0000f410: 6361 7465 6e61 7465 2828 6672 6571 5f62  catenate((freq_b
-0000f420: 696e 732c 6e70 2e61 7272 6179 285b 2866  ins,np.array([(f
-0000f430: 7265 715f 6269 6e73 5b2d 315d 2d66 7265  req_bins[-1]-fre
-0000f440: 715f 6269 6e73 5b2d 325d 292b 6672 6571  q_bins[-2])+freq
-0000f450: 5f62 696e 735b 2d31 5d5d 2929 290a 2020  _bins[-1]]))).  
-0000f460: 2020 2020 2020 6e75 3d66 7265 715f 6269        nu=freq_bi
-0000f470: 6e73 2a31 6539 0a20 2020 206e 755f 696a  ns*1e9.    nu_ij
-0000f480: 5f74 696c 653d 6e70 2e74 696c 6528 6e75  _tile=np.tile(nu
-0000f490: 5f69 6a2c 5b6c 656e 286e 7529 2c31 5d29  _ij,[len(nu),1])
-0000f4a0: 0a20 2020 206e 755f 7469 6c65 3d6e 702e  .    nu_tile=np.
-0000f4b0: 7469 6c65 286e 752c 5b6c 656e 286e 755f  tile(nu,[len(nu_
-0000f4c0: 696a 292c 315d 290a 2020 2020 6c69 6e65  ij),1]).    line
-0000f4d0: 5374 7265 6e67 7468 735f 7469 6c65 3d6e  Strengths_tile=n
-0000f4e0: 702e 7469 6c65 286c 696e 6553 7472 656e  p.tile(lineStren
-0000f4f0: 6774 6873 2c5b 6c65 6e28 6e75 292c 315d  gths,[len(nu),1]
-0000f500: 290a 2020 2020 7065 7263 5f74 696c 653d  ).    perc_tile=
-0000f510: 6750 6572 6328 6e75 5f74 696c 652c 6e75  gPerc(nu_tile,nu
-0000f520: 5f69 6a5f 7469 6c65 2e54 2c6e 755f 696a  _ij_tile.T,nu_ij
-0000f530: 5f74 696c 652e 542f 632a 7672 290a 2020  _tile.T/c*vr).  
-0000f540: 2020 783d 7065 7263 5f74 696c 655b 3a2c    x=perc_tile[:,
-0000f550: 3a2d 315d 2d70 6572 635f 7469 6c65 5b3a  :-1]-perc_tile[:
-0000f560: 2c31 3a5d 0a20 2020 2077 6176 656c 656e  ,1:].    wavelen
-0000f570: 6774 682c 666c 7578 3d63 2f6e 755b 3a2d  gth,flux=c/nu[:-
-0000f580: 315d 2a31 6536 2c6e 702e 7375 6d28 782a  1]*1e6,np.sum(x*
-0000f590: 6c69 6e65 5374 7265 6e67 7468 735f 7469  lineStrengths_ti
-0000f5a0: 6c65 5b3a 2d31 2c3a 5d2e 542c 6178 6973  le[:-1,:].T,axis
-0000f5b0: 3d30 292f 286e 755b 3a2d 315d 2d6e 755b  =0)/(nu[:-1]-nu[
-0000f5c0: 313a 5d29 0a20 2020 2072 6574 7572 6e20  1:]).    return 
-0000f5d0: 7761 7665 6c65 6e67 7468 2c66 6c75 780a  wavelength,flux.
-0000f5e0: 0a0a 6465 6620 6765 6e65 7261 6c43 6f6e  ..def generalCon
-0000f5f0: 766f 6c76 6528 6c69 6e65 5374 7265 6e67  volve(lineStreng
-0000f600: 7468 732c 6c69 6e65 4672 6571 2c52 3d31  ths,lineFreq,R=1
-0000f610: 2c6c 616d 6264 615f 303d 312c 6c61 6d62  ,lambda_0=1,lamb
-0000f620: 6461 5f6e 3d31 2c52 5f62 6163 6b3d 3165  da_n=1,R_back=1e
-0000f630: 3629 3a0a 2020 2020 6966 206c 616d 6264  6):.    if lambd
-0000f640: 615f 6e3d 3d6c 616d 6264 615f 303a 0a20  a_n==lambda_0:. 
-0000f650: 2020 2020 2020 206c 616d 6264 615f 6e3d         lambda_n=
-0000f660: 632f 6e70 2e61 6d69 6e28 6c69 6e65 4672  c/np.amin(lineFr
-0000f670: 6571 292a 3165 2d33 2a32 0a0a 2020 2020  eq)*1e-3*2..    
-0000f680: 2320 525f 6261 636b 3d31 6536 0a20 2020  # R_back=1e6.   
-0000f690: 2066 7265 715f 6269 6e73 3d67 656e 6572   freq_bins=gener
-0000f6a0: 6174 655f 6772 6964 2852 5f62 6163 6b2c  ate_grid(R_back,
-0000f6b0: 6c61 6d62 6461 5f30 2c6c 616d 6264 615f  lambda_0,lambda_
-0000f6c0: 6e29 0a20 2020 2077 6176 655f 6269 6e73  n).    wave_bins
-0000f6d0: 3d63 2f66 7265 715f 6269 6e73 2a31 652d  =c/freq_bins*1e-
-0000f6e0: 330a 2020 2020 666c 7578 5f62 696e 733d  3.    flux_bins=
-0000f6f0: 7761 7665 5f62 696e 732a 302e 300a 2020  wave_bins*0.0.  
-0000f700: 2020 693d 360a 2020 2020 533d 6c69 6e65    i=6.    S=line
-0000f710: 5374 7265 6e67 7468 730a 2020 2020 463d  Strengths.    F=
-0000f720: 6c69 6e65 4672 6571 0a20 2020 2069 6e64  lineFreq.    ind
-0000f730: 3d6e 702e 6469 6769 7469 7a65 2846 2c6e  =np.digitize(F,n
-0000f740: 702e 666c 6970 2866 7265 715f 6269 6e73  p.flip(freq_bins
-0000f750: 295b 3a2d 315d 290a 2020 2020 666f 7220  )[:-1]).    for 
-0000f760: 692c 6964 7820 696e 2065 6e75 6d65 7261  i,idx in enumera
-0000f770: 7465 2869 6e64 293a 0a20 2020 2020 2020  te(ind):.       
-0000f780: 2066 6c75 785f 6269 6e73 5b69 6478 5d2b   flux_bins[idx]+
-0000f790: 3d53 5b69 5d0a 0a20 2020 2046 5748 4d3d  =S[i]..    FWHM=
-0000f7a0: 525f 6261 636b 2f52 2f32 2e33 3535 0a20  R_back/R/2.355. 
-0000f7b0: 2020 2067 3d47 6175 7373 6961 6e31 444b     g=Gaussian1DK
-0000f7c0: 6572 6e65 6c28 7374 6464 6576 3d46 5748  ernel(stddev=FWH
-0000f7d0: 4d2c 6661 6374 6f72 3d37 290a 2020 2020  M,factor=7).    
-0000f7e0: 413d 6170 795f 636f 6e76 6f6c 7665 2866  A=apy_convolve(f
-0000f7f0: 6c75 785f 6269 6e73 2c67 290a 2020 2020  lux_bins,g).    
-0000f800: 413d 415b 313a 5d2f 286e 702e 666c 6970  A=A[1:]/(np.flip
-0000f810: 2866 7265 715f 6269 6e73 295b 313a 5d2d  (freq_bins)[1:]-
-0000f820: 6e70 2e66 6c69 7028 6672 6571 5f62 696e  np.flip(freq_bin
-0000f830: 7329 5b3a 2d31 5d29 2a31 652d 390a 2020  s)[:-1])*1e-9.  
-0000f840: 2020 573d 6e70 2e66 6c69 7028 7761 7665    W=np.flip(wave
-0000f850: 5f62 696e 735b 313a 5d29 0a20 2020 2072  _bins[1:]).    r
-0000f860: 6574 7572 6e20 6e70 2e66 6c69 7028 5729  eturn np.flip(W)
-0000f870: 2c6e 702e 666c 6970 2841 290a 0a0a 6465  ,np.flip(A)...de
-0000f880: 6620 6765 6e65 7261 7465 5f67 7269 6428  f generate_grid(
-0000f890: 523d 312c 6c61 6d62 6461 5f30 3d31 2c6c  R=1,lambda_0=1,l
-0000f8a0: 616d 6264 615f 6e3d 3129 3a0a 2020 2020  ambda_n=1):.    
-0000f8b0: 6465 6c5f 6c6f 676c 616d 3d6e 702e 6c6f  del_loglam=np.lo
-0000f8c0: 6731 3028 312e 302b 312e 302f 5229 0a20  g10(1.0+1.0/R). 
-0000f8d0: 2020 204e 3d31 2b69 6e74 286e 702e 6c6f     N=1+int(np.lo
-0000f8e0: 6731 3028 6c61 6d62 6461 5f6e 2f6c 616d  g10(lambda_n/lam
-0000f8f0: 6264 615f 3029 2f64 656c 5f6c 6f67 6c61  bda_0)/del_logla
-0000f900: 6d29 0a20 2020 206d 776c 736c 696e 653d  m).    mwlsline=
-0000f910: 6e70 2e6c 6f67 7370 6163 6528 6e70 2e6c  np.logspace(np.l
-0000f920: 6f67 3130 286c 616d 6264 615f 3029 2c6e  og10(lambda_0),n
-0000f930: 702e 6c6f 6731 3028 6c61 6d62 6461 5f6e  p.log10(lambda_n
-0000f940: 292c 4e29 0a20 2020 206e 753d 632f 6d77  ),N).    nu=c/mw
-0000f950: 6c73 6c69 6e65 2a31 6536 0a20 2020 2072  lsline*1e6.    r
-0000f960: 6574 7572 6e28 6e75 2a31 652d 3929 0a0a  eturn(nu*1e-9)..
-0000f970: 0a64 6566 2063 6f6e 766f 6c76 6528 6d6f  .def convolve(mo
-0000f980: 6465 6c73 2c66 7265 715f 6269 6e73 3d4e  dels,freq_bins=N
-0000f990: 6f6e 652c 523d 312c 6c61 6d62 6461 5f30  one,R=1,lambda_0
-0000f9a0: 3d31 2c6c 616d 6264 615f 6e3d 312c 7672  =1,lambda_n=1,vr
-0000f9b0: 3d31 3330 302c 4e4c 5445 3d46 616c 7365  =1300,NLTE=False
-0000f9c0: 2c63 6f6e 765f 7479 7065 3d31 2c76 6572  ,conv_type=1,ver
-0000f9d0: 626f 7365 3d54 7275 6529 3a0a 2020 2020  bose=True):.    
-0000f9e0: 666f 7220 692c 6420 696e 2065 6e75 6d65  for i,d in enume
-0000f9f0: 7261 7465 286d 6f64 656c 7329 3a0a 2020  rate(models):.  
-0000fa00: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
-0000fa10: 3a20 7072 696e 7428 275c 6e5c 6e4d 6f64  : print('\n\nMod
-0000fa20: 656c 2027 2c69 2b31 290a 2020 2020 2020  el ',i+1).      
-0000fa30: 2020 642e 636f 6e76 6f6c 7665 2866 7265    d.convolve(fre
-0000fa40: 715f 6269 6e73 3d66 7265 715f 6269 6e73  q_bins=freq_bins
-0000fa50: 2c52 3d52 2c6c 616d 6264 615f 303d 6c61  ,R=R,lambda_0=la
-0000fa60: 6d62 6461 5f30 2c6c 616d 6264 615f 6e3d  mbda_0,lambda_n=
-0000fa70: 6c61 6d62 6461 5f6e 2c76 723d 7672 2c4e  lambda_n,vr=vr,N
-0000fa80: 4c54 453d 4e4c 5445 2c63 6f6e 765f 7479  LTE=NLTE,conv_ty
-0000fa90: 7065 3d63 6f6e 765f 7479 7065 290a 2020  pe=conv_type).  
-0000faa0: 2020 7265 7475 726e 206d 6f64 656c 730a    return models.
-0000fab0: 0a0a 6465 6620 6765 6e65 7261 7465 5f73  ..def generate_s
-0000fac0: 6c61 625f 6772 6964 2864 6972 6563 746f  lab_grid(directo
-0000fad0: 7279 3d27 2e27 2c20 6772 6964 5f70 6172  ry='.', grid_par
-0000fae0: 616d 6574 6572 733d 7b7d 2c20 636f 6d62  ameters={}, comb
-0000faf0: 696e 6174 696f 6e3d 4661 6c73 652c 204e  ination=False, N
-0000fb00: 746f 743d 4e6f 6e65 2c20 5467 3d4e 6f6e  tot=None, Tg=Non
-0000fb10: 652c 206e 4870 6c75 733d 4e6f 6e65 2c20  e, nHplus=None, 
-0000fb20: 6e48 313d 4e6f 6e65 2c20 6e48 323d 4e6f  nH1=None, nH2=No
-0000fb30: 6e65 2c20 6e48 653d 4e6f 6e65 2c20 6e65  ne, nHe=None, ne
-0000fb40: 6c65 633d 4e6f 6e65 2c20 5464 3d4e 6f6e  lec=None, Td=Non
-0000fb50: 652c 2076 7475 7262 3d4e 6f6e 652c 2064  e, vturb=None, d
-0000fb60: 7573 745f 746f 5f67 6173 3d4e 6f6e 652c  ust_to_gas=None,
-0000fb70: 2052 5f6f 7665 726c 6170 3d4e 6f6e 652c   R_overlap=None,
-0000fb80: 206c 696e 655f 6f76 6572 6c61 703d 4e6f   line_overlap=No
-0000fb90: 6e65 2c20 7370 6563 6965 735f 6c69 7374  ne, species_list
-0000fba0: 3d7b 7d2c 206f 7574 7075 745f 6669 6c65  ={}, output_file
-0000fbb0: 6e61 6d65 3d27 536c 6162 5265 7375 6c74  name='SlabResult
-0000fbc0: 732e 6f75 7427 2c20 6f76 6572 6c61 705f  s.out', overlap_
-0000fbd0: 6669 6c65 6e61 6d65 3d27 536c 6162 4f76  filename='SlabOv
-0000fbe0: 6572 6c61 702e 6f75 7427 2c20 7365 7061  erlap.out', sepa
-0000fbf0: 7261 7465 5f6f 705f 6669 6c65 733d 5472  rate_op_files=Tr
-0000fc00: 7565 2c20 736c 6162 5f52 543d 5472 7565  ue, slab_RT=True
-0000fc10: 2c20 7368 6f72 745f 666f 726d 6174 3d46  , short_format=F
-0000fc20: 616c 7365 2c20 6e6f 5f69 6e64 6976 6964  alse, no_individ
-0000fc30: 7561 6c5f 6c69 6e65 7320 3d20 4661 6c73  ual_lines = Fals
-0000fc40: 652c 2066 6974 735f 6f70 5f66 696c 6573  e, fits_op_files
-0000fc50: 203d 2046 616c 7365 293a 0a20 2020 2022   = False):.    "
-0000fc60: 2222 0a20 2020 2046 756e 6374 696f 6e20  "".    Function 
-0000fc70: 746f 2067 656e 6572 6174 6520 536c 6162  to generate Slab
-0000fc80: 496e 7075 742e 696e 2069 6e70 7574 2066  Input.in input f
-0000fc90: 696c 6520 636f 6e74 6169 6e69 6e67 2074  ile containing t
-0000fca0: 6865 2064 6574 6169 6c73 206f 6620 7468  he details of th
-0000fcb0: 6520 736c 6162 206d 6f64 656c 2067 7269  e slab model gri
-0000fcc0: 640a 2020 2020 2222 220a 2020 2020 6e6d  d.    """.    nm
-0000fcd0: 6f64 656c 733d 310a 2020 2020 636f 6d62  odels=1.    comb
-0000fce0: 696e 6174 696f 6e3d 4661 6c73 650a 2020  ination=False.  
-0000fcf0: 2020 6966 206c 656e 2867 7269 645f 7061    if len(grid_pa
-0000fd00: 7261 6d65 7465 7273 293e 303a 0a20 2020  rameters)>0:.   
-0000fd10: 2020 2020 2069 6620 6e6f 7420 636f 6d62       if not comb
-0000fd20: 696e 6174 696f 6e3a 0a20 2020 2020 2020  ination:.       
-0000fd30: 2020 2020 206e 6d6f 6465 6c73 3d6c 656e       nmodels=len
-0000fd40: 2867 7269 645f 7061 7261 6d65 7465 7273  (grid_parameters
-0000fd50: 5b6c 6973 7428 6772 6964 5f70 6172 616d  [list(grid_param
-0000fd60: 6574 6572 732e 6b65 7973 2829 295b 305d  eters.keys())[0]
-0000fd70: 5d29 0a20 2020 2020 2020 2065 6c73 653a  ]).        else:
-0000fd80: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000fd90: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-0000fda0: 6772 6964 5f70 6172 616d 6574 6572 7329  grid_parameters)
-0000fdb0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000fdc0: 2020 206e 6d6f 6465 6c73 2a3d 6c65 6e28     nmodels*=len(
-0000fdd0: 6772 6964 5f70 6172 616d 6574 6572 735b  grid_parameters[
-0000fde0: 6c69 7374 2867 7269 645f 7061 7261 6d65  list(grid_parame
-0000fdf0: 7465 7273 2e6b 6579 7328 2929 5b69 5d5d  ters.keys())[i]]
-0000fe00: 290a 0a20 2020 204e 746f 745f 6c69 7374  )..    Ntot_list
-0000fe10: 3d6e 702e 6f6e 6573 2828 6e6d 6f64 656c  =np.ones((nmodel
-0000fe20: 7329 290a 2020 2020 5467 5f6c 6973 743d  s)).    Tg_list=
-0000fe30: 6e70 2e6f 6e65 7328 286e 6d6f 6465 6c73  np.ones((nmodels
-0000fe40: 2929 0a20 2020 206e 4870 6c75 735f 6c69  )).    nHplus_li
-0000fe50: 7374 3d6e 702e 6f6e 6573 2828 6e6d 6f64  st=np.ones((nmod
-0000fe60: 656c 7329 290a 2020 2020 6e48 315f 6c69  els)).    nH1_li
-0000fe70: 7374 3d6e 702e 6f6e 6573 2828 6e6d 6f64  st=np.ones((nmod
-0000fe80: 656c 7329 290a 2020 2020 6e48 325f 6c69  els)).    nH2_li
-0000fe90: 7374 3d6e 702e 6f6e 6573 2828 6e6d 6f64  st=np.ones((nmod
-0000fea0: 656c 7329 290a 2020 2020 6e48 655f 6c69  els)).    nHe_li
-0000feb0: 7374 3d6e 702e 6f6e 6573 2828 6e6d 6f64  st=np.ones((nmod
-0000fec0: 656c 7329 290a 2020 2020 6e65 6c65 635f  els)).    nelec_
-0000fed0: 6c69 7374 3d6e 702e 6f6e 6573 2828 6e6d  list=np.ones((nm
-0000fee0: 6f64 656c 7329 290a 2020 2020 5464 5f6c  odels)).    Td_l
-0000fef0: 6973 743d 6e70 2e6f 6e65 7328 286e 6d6f  ist=np.ones((nmo
-0000ff00: 6465 6c73 2929 0a20 2020 2076 7475 7262  dels)).    vturb
-0000ff10: 5f6c 6973 743d 6e70 2e6f 6e65 7328 286e  _list=np.ones((n
-0000ff20: 6d6f 6465 6c73 2929 0a20 2020 2064 7573  models)).    dus
-0000ff30: 745f 746f 5f67 6173 5f6c 6973 743d 6e70  t_to_gas_list=np
-0000ff40: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
-0000ff50: 0a20 2020 2052 5f6f 7665 726c 6170 5f6c  .    R_overlap_l
-0000ff60: 6973 743d 6e70 2e6f 6e65 7328 286e 6d6f  ist=np.ones((nmo
-0000ff70: 6465 6c73 2929 0a20 2020 206c 696e 655f  dels)).    line_
-0000ff80: 6f76 6572 6c61 705f 6c69 7374 3d6e 702e  overlap_list=np.
-0000ff90: 6f6e 6573 2828 6e6d 6f64 656c 732c 3229  ones((nmodels,2)
-0000ffa0: 290a 2020 2020 6966 206c 656e 2873 7065  ).    if len(spe
-0000ffb0: 6369 6573 5f6c 6973 7429 3c31 3a20 7261  cies_list)<1: ra
-0000ffc0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-0000ffd0: 5468 6520 7370 6563 6965 735f 6c69 7374  The species_list
-0000ffe0: 2063 616e 6e6f 7420 6265 2065 6d70 7479   cannot be empty
-0000fff0: 2729 0a0a 2020 2020 6966 206e 6f74 2063  ')..    if not c
-00010000: 6f6d 6269 6e61 7469 6f6e 3a0a 2020 2020  ombination:.    
-00010010: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00010020: 6765 286c 656e 2867 7269 645f 7061 7261  ge(len(grid_para
-00010030: 6d65 7465 7273 2929 3a0a 2020 2020 2020  meters)):.      
-00010040: 2020 2020 2020 6966 206c 6973 7428 6772        if list(gr
-00010050: 6964 5f70 6172 616d 6574 6572 732e 6b65  id_parameters.ke
-00010060: 7973 2829 295b 695d 3d3d 274e 746f 7427  ys())[i]=='Ntot'
-00010070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010080: 2020 4e74 6f74 5f6c 6973 742a 3d67 7269    Ntot_list*=gri
-00010090: 645f 7061 7261 6d65 7465 7273 5b27 4e74  d_parameters['Nt
-000100a0: 6f74 275d 0a20 2020 2020 2020 2020 2020  ot'].           
-000100b0: 2065 6c69 6620 6c69 7374 2867 7269 645f   elif list(grid_
-000100c0: 7061 7261 6d65 7465 7273 2e6b 6579 7328  parameters.keys(
-000100d0: 2929 5b69 5d3d 3d27 5467 273a 0a20 2020  ))[i]=='Tg':.   
-000100e0: 2020 2020 2020 2020 2020 2020 2054 675f               Tg_
-000100f0: 6c69 7374 2a3d 6772 6964 5f70 6172 616d  list*=grid_param
-00010100: 6574 6572 735b 2754 6727 5d0a 2020 2020  eters['Tg'].    
-00010110: 2020 2020 2020 2020 656c 6966 206c 6973          elif lis
-00010120: 7428 6772 6964 5f70 6172 616d 6574 6572  t(grid_parameter
-00010130: 732e 6b65 7973 2829 295b 695d 3d3d 276e  s.keys())[i]=='n
-00010140: 4870 6c75 7327 3a0a 2020 2020 2020 2020  Hplus':.        
-00010150: 2020 2020 2020 2020 6e48 706c 7573 5f6c          nHplus_l
-00010160: 6973 742a 3d67 7269 645f 7061 7261 6d65  ist*=grid_parame
-00010170: 7465 7273 5b27 6e48 706c 7573 275d 0a20  ters['nHplus']. 
-00010180: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00010190: 6c69 7374 2867 7269 645f 7061 7261 6d65  list(grid_parame
-000101a0: 7465 7273 2e6b 6579 7328 2929 5b69 5d3d  ters.keys())[i]=
-000101b0: 3d27 6e48 3127 3a0a 2020 2020 2020 2020  ='nH1':.        
-000101c0: 2020 2020 2020 2020 6e48 315f 6c69 7374          nH1_list
-000101d0: 2a3d 6772 6964 5f70 6172 616d 6574 6572  *=grid_parameter
-000101e0: 735b 276e 4831 275d 0a20 2020 2020 2020  s['nH1'].       
-000101f0: 2020 2020 2065 6c69 6620 6c69 7374 2867       elif list(g
-00010200: 7269 645f 7061 7261 6d65 7465 7273 2e6b  rid_parameters.k
-00010210: 6579 7328 2929 5b69 5d3d 3d27 6e48 3227  eys())[i]=='nH2'
-00010220: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010230: 2020 6e48 325f 6c69 7374 2a3d 6772 6964    nH2_list*=grid
-00010240: 5f70 6172 616d 6574 6572 735b 276e 4832  _parameters['nH2
-00010250: 275d 0a20 2020 2020 2020 2020 2020 2065  '].            e
-00010260: 6c69 6620 6c69 7374 2867 7269 645f 7061  lif list(grid_pa
-00010270: 7261 6d65 7465 7273 2e6b 6579 7328 2929  rameters.keys())
-00010280: 5b69 5d3d 3d27 6e48 6527 3a0a 2020 2020  [i]=='nHe':.    
-00010290: 2020 2020 2020 2020 2020 2020 6e48 655f              nHe_
-000102a0: 6c69 7374 2a3d 6772 6964 5f70 6172 616d  list*=grid_param
-000102b0: 6574 6572 735b 276e 4865 275d 0a20 2020  eters['nHe'].   
-000102c0: 2020 2020 2020 2020 2065 6c69 6620 6c69           elif li
-000102d0: 7374 2867 7269 645f 7061 7261 6d65 7465  st(grid_paramete
-000102e0: 7273 2e6b 6579 7328 2929 5b69 5d3d 3d27  rs.keys())[i]=='
-000102f0: 6e65 6c65 6327 3a0a 2020 2020 2020 2020  nelec':.        
-00010300: 2020 2020 2020 2020 6e65 6c65 635f 6c69          nelec_li
-00010310: 7374 2a3d 6772 6964 5f70 6172 616d 6574  st*=grid_paramet
-00010320: 6572 735b 276e 656c 6563 275d 0a20 2020  ers['nelec'].   
-00010330: 2020 2020 2020 2020 2065 6c69 6620 6c69           elif li
-00010340: 7374 2867 7269 645f 7061 7261 6d65 7465  st(grid_paramete
-00010350: 7273 2e6b 6579 7328 2929 5b69 5d3d 3d27  rs.keys())[i]=='
-00010360: 5464 273a 0a20 2020 2020 2020 2020 2020  Td':.           
-00010370: 2020 2020 2054 645f 6c69 7374 2a3d 6772       Td_list*=gr
-00010380: 6964 5f70 6172 616d 6574 6572 735b 2754  id_parameters['T
-00010390: 6427 5d0a 2020 2020 2020 2020 2020 2020  d'].            
-000103a0: 656c 6966 206c 6973 7428 6772 6964 5f70  elif list(grid_p
-000103b0: 6172 616d 6574 6572 732e 6b65 7973 2829  arameters.keys()
-000103c0: 295b 695d 3d3d 2776 7475 7262 273a 0a20  )[i]=='vturb':. 
-000103d0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-000103e0: 7475 7262 5f6c 6973 742a 3d67 7269 645f  turb_list*=grid_
-000103f0: 7061 7261 6d65 7465 7273 5b27 7674 7572  parameters['vtur
-00010400: 6227 5d0a 2020 2020 2020 2020 2020 2020  b'].            
-00010410: 656c 6966 206c 6973 7428 6772 6964 5f70  elif list(grid_p
-00010420: 6172 616d 6574 6572 732e 6b65 7973 2829  arameters.keys()
-00010430: 295b 695d 3d3d 2764 7573 745f 746f 5f67  )[i]=='dust_to_g
-00010440: 6173 273a 0a20 2020 2020 2020 2020 2020  as':.           
-00010450: 2020 2020 2064 7573 745f 746f 5f67 6173       dust_to_gas
-00010460: 5f6c 6973 742a 3d67 7269 645f 7061 7261  _list*=grid_para
-00010470: 6d65 7465 7273 5b27 6475 7374 5f74 6f5f  meters['dust_to_
-00010480: 6761 7327 5d0a 2020 2020 2020 2020 2020  gas'].          
-00010490: 2020 656c 6966 206c 6973 7428 6772 6964    elif list(grid
-000104a0: 5f70 6172 616d 6574 6572 732e 6b65 7973  _parameters.keys
-000104b0: 2829 295b 695d 3d3d 2752 5f6f 7665 726c  ())[i]=='R_overl
-000104c0: 6170 273a 0a20 2020 2020 2020 2020 2020  ap':.           
-000104d0: 2020 2020 2052 5f6f 7665 726c 6170 5f6c       R_overlap_l
-000104e0: 6973 742a 3d67 7269 645f 7061 7261 6d65  ist*=grid_parame
-000104f0: 7465 7273 5b27 525f 6f76 6572 6c61 7027  ters['R_overlap'
-00010500: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
-00010510: 6966 206c 6973 7428 6772 6964 5f70 6172  if list(grid_par
-00010520: 616d 6574 6572 732e 6b65 7973 2829 295b  ameters.keys())[
-00010530: 695d 3d3d 276c 696e 655f 6f76 6572 6c61  i]=='line_overla
-00010540: 7027 3a0a 2020 2020 2020 2020 2020 2020  p':.            
-00010550: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
-00010560: 6765 286c 656e 2867 7269 645f 7061 7261  ge(len(grid_para
-00010570: 6d65 7465 7273 5b27 6c69 6e65 5f6f 7665  meters['line_ove
-00010580: 726c 6170 275d 2929 3a0a 2020 2020 2020  rlap'])):.      
-00010590: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-000105a0: 6e65 5f6f 7665 726c 6170 5f6c 6973 745b  ne_overlap_list[
-000105b0: 6a2c 3a5d 3d6e 702e 6172 7261 7928 6772  j,:]=np.array(gr
-000105c0: 6964 5f70 6172 616d 6574 6572 735b 276c  id_parameters['l
-000105d0: 696e 655f 6f76 6572 6c61 7027 5d5b 6a5d  ine_overlap'][j]
-000105e0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000105f0: 7365 3a20 7261 6973 6520 4b65 7945 7272  se: raise KeyErr
-00010600: 6f72 2866 2755 6e69 6465 6e74 6966 6965  or(f'Unidentifie
-00010610: 6420 6772 6964 2070 6172 616d 6574 6572  d grid parameter
-00010620: 207b 6c69 7374 2867 7269 645f 7061 7261   {list(grid_para
-00010630: 6d65 7465 7273 2e6b 6579 7328 2929 5b69  meters.keys())[i
-00010640: 5d7d 2729 0a20 2020 2065 6c73 653a 0a20  ]}').    else:. 
-00010650: 2020 2020 2020 2072 6169 7365 204b 6579         raise Key
-00010660: 4572 726f 7228 2743 6f6d 6269 6e61 7469  Error('Combinati
-00010670: 6f6e 2069 7320 7374 696c 6c20 6e6f 7420  on is still not 
-00010680: 7375 7070 6f72 7465 6427 290a 0a20 2020  supported')..   
-00010690: 2069 6620 6e70 2e73 756d 284e 746f 745f   if np.sum(Ntot_
-000106a0: 6c69 7374 293d 3d6e 6d6f 6465 6c73 3a0a  list)==nmodels:.
-000106b0: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
-000106c0: 4e74 6f74 2020 2020 2020 2020 6973 204e  Ntot        is N
-000106d0: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
-000106e0: 2020 4e74 6f74 5f6c 6973 742a 3d4e 746f    Ntot_list*=Nto
-000106f0: 740a 2020 2020 2020 2020 2320 656c 7365  t.        # else
-00010700: 3a0a 2020 2020 2020 2020 2320 2020 2020  :.        #     
-00010710: 4e74 6f74 5f6c 6973 742a 3d31 6531 350a  Ntot_list*=1e15.
-00010720: 2020 2020 6966 206e 702e 7375 6d28 5467      if np.sum(Tg
-00010730: 5f6c 6973 7429 3d3d 6e6d 6f64 656c 733a  _list)==nmodels:
-00010740: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00010750: 2854 6720 2020 2020 2020 2020 2069 7320  (Tg          is 
-00010760: 4e6f 6e65 293a 0a20 2020 2020 2020 2020  None):.         
-00010770: 2020 2054 675f 6c69 7374 2a3d 5467 0a20     Tg_list*=Tg. 
-00010780: 2020 2020 2020 2023 2065 6c73 653a 0a20         # else:. 
-00010790: 2020 2020 2020 2023 2020 2020 2054 675f         #     Tg_
-000107a0: 6c69 7374 2a3d 3130 300a 2020 2020 6966  list*=100.    if
-000107b0: 206e 702e 7375 6d28 6e48 706c 7573 5f6c   np.sum(nHplus_l
-000107c0: 6973 7429 3d3d 6e6d 6f64 656c 733a 0a20  ist)==nmodels:. 
-000107d0: 2020 2020 2020 2069 6620 6e6f 7420 286e         if not (n
-000107e0: 4870 6c75 7320 2020 2020 2069 7320 4e6f  Hplus      is No
-000107f0: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
-00010800: 206e 4870 6c75 735f 6c69 7374 2a3d 6e48   nHplus_list*=nH
-00010810: 706c 7573 0a20 2020 2020 2020 2023 2065  plus.        # e
-00010820: 6c73 653a 0a20 2020 2020 2020 2023 2020  lse:.        #  
-00010830: 2020 206e 4870 6c75 735f 6c69 7374 2a3d     nHplus_list*=
-00010840: 3165 310a 2020 2020 6966 206e 702e 7375  1e1.    if np.su
-00010850: 6d28 6e48 315f 6c69 7374 293d 3d6e 6d6f  m(nH1_list)==nmo
-00010860: 6465 6c73 3a0a 2020 2020 2020 2020 6966  dels:.        if
-00010870: 206e 6f74 2028 6e48 3120 2020 2020 2020   not (nH1       
-00010880: 2020 6973 204e 6f6e 6529 3a0a 2020 2020    is None):.    
-00010890: 2020 2020 2020 2020 6e48 315f 6c69 7374          nH1_list
-000108a0: 2a3d 6e48 310a 2020 2020 2020 2020 2320  *=nH1.        # 
-000108b0: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
-000108c0: 2020 2020 6e48 315f 6c69 7374 2a3d 3165      nH1_list*=1e
-000108d0: 3132 0a20 2020 2069 6620 6e70 2e73 756d  12.    if np.sum
-000108e0: 286e 4832 5f6c 6973 7429 3d3d 6e6d 6f64  (nH2_list)==nmod
-000108f0: 656c 733a 0a20 2020 2020 2020 2069 6620  els:.        if 
-00010900: 6e6f 7420 286e 4832 2020 2020 2020 2020  not (nH2        
-00010910: 2069 7320 4e6f 6e65 293a 0a20 2020 2020   is None):.     
-00010920: 2020 2020 2020 206e 4832 5f6c 6973 742a         nH2_list*
-00010930: 3d6e 4832 0a20 2020 2020 2020 2023 2065  =nH2.        # e
-00010940: 6c73 653a 0a20 2020 2020 2020 2023 2020  lse:.        #  
-00010950: 2020 206e 4832 5f6c 6973 742a 3d31 6531     nH2_list*=1e1
-00010960: 320a 2020 2020 6966 206e 702e 7375 6d28  2.    if np.sum(
-00010970: 6e48 655f 6c69 7374 293d 3d6e 6d6f 6465  nHe_list)==nmode
-00010980: 6c73 3a0a 2020 2020 2020 2020 6966 206e  ls:.        if n
-00010990: 6f74 2028 6e48 6520 2020 2020 2020 2020  ot (nHe         
-000109a0: 6973 204e 6f6e 6529 3a0a 2020 2020 2020  is None):.      
-000109b0: 2020 2020 2020 6e48 655f 6c69 7374 2a3d        nHe_list*=
-000109c0: 6e48 650a 2020 2020 2020 2020 2320 656c  nHe.        # el
-000109d0: 7365 3a0a 2020 2020 2020 2020 2320 2020  se:.        #   
-000109e0: 2020 6e48 655f 6c69 7374 2a3d 3165 3131    nHe_list*=1e11
-000109f0: 0a20 2020 2069 6620 6e70 2e73 756d 286e  .    if np.sum(n
-00010a00: 656c 6563 5f6c 6973 7429 3d3d 6e6d 6f64  elec_list)==nmod
-00010a10: 656c 733a 0a20 2020 2020 2020 2069 6620  els:.        if 
-00010a20: 6e6f 7420 286e 656c 6563 2020 2020 2020  not (nelec      
-00010a30: 2069 7320 4e6f 6e65 293a 0a20 2020 2020   is None):.     
-00010a40: 2020 2020 2020 206e 656c 6563 5f6c 6973         nelec_lis
-00010a50: 742a 3d6e 656c 6563 0a20 2020 2020 2020  t*=nelec.       
-00010a60: 2023 2065 6c73 653a 0a20 2020 2020 2020   # else:.       
-00010a70: 2023 2020 2020 206e 656c 6563 5f6c 6973   #     nelec_lis
-00010a80: 742a 3d31 6538 0a20 2020 2069 6620 6e70  t*=1e8.    if np
-00010a90: 2e73 756d 2854 645f 6c69 7374 293d 3d6e  .sum(Td_list)==n
-00010aa0: 6d6f 6465 6c73 3a0a 2020 2020 2020 2020  models:.        
-00010ab0: 6966 206e 6f74 2028 5464 2020 2020 2020  if not (Td      
-00010ac0: 2020 2020 6973 204e 6f6e 6529 3a0a 2020      is None):.  
-00010ad0: 2020 2020 2020 2020 2020 5464 5f6c 6973            Td_lis
-00010ae0: 742a 3d54 640a 2020 2020 2020 2020 2320  t*=Td.        # 
-00010af0: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
-00010b00: 2020 2020 5464 5f6c 6973 742a 3d31 300a      Td_list*=10.
-00010b10: 2020 2020 6966 206e 702e 7375 6d28 7674      if np.sum(vt
-00010b20: 7572 625f 6c69 7374 293d 3d6e 6d6f 6465  urb_list)==nmode
-00010b30: 6c73 3a0a 2020 2020 2020 2020 6966 206e  ls:.        if n
-00010b40: 6f74 2028 7674 7572 6220 2020 2020 2020  ot (vturb       
-00010b50: 6973 204e 6f6e 6529 3a0a 2020 2020 2020  is None):.      
-00010b60: 2020 2020 2020 7674 7572 625f 6c69 7374        vturb_list
-00010b70: 2a3d 7674 7572 620a 2020 2020 2020 2020  *=vturb.        
-00010b80: 2320 656c 7365 3a0a 2020 2020 2020 2020  # else:.        
-00010b90: 2320 2020 2020 7674 7572 625f 6c69 7374  #     vturb_list
-00010ba0: 2a3d 312e 340a 2020 2020 6966 206e 702e  *=1.4.    if np.
-00010bb0: 7375 6d28 6475 7374 5f74 6f5f 6761 735f  sum(dust_to_gas_
-00010bc0: 6c69 7374 293d 3d6e 6d6f 6465 6c73 3a0a  list)==nmodels:.
-00010bd0: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
-00010be0: 6475 7374 5f74 6f5f 6761 7320 6973 204e  dust_to_gas is N
-00010bf0: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
-00010c00: 2020 6475 7374 5f74 6f5f 6761 735f 6c69    dust_to_gas_li
-00010c10: 7374 2a3d 6475 7374 5f74 6f5f 6761 730a  st*=dust_to_gas.
-00010c20: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
-00010c30: 2020 2020 2020 2020 2320 2020 2020 6475          #     du
-00010c40: 7374 5f74 6f5f 6761 735f 6c69 7374 2a3d  st_to_gas_list*=
-00010c50: 3165 2d32 310a 2020 2020 6966 206e 702e  1e-21.    if np.
-00010c60: 7375 6d28 525f 6f76 6572 6c61 705f 6c69  sum(R_overlap_li
-00010c70: 7374 293d 3d6e 6d6f 6465 6c73 3a0a 2020  st)==nmodels:.  
-00010c80: 2020 2020 2020 6966 206e 6f74 2028 525f        if not (R_
-00010c90: 6f76 6572 6c61 7020 6973 204e 6f6e 6529  overlap is None)
-00010ca0: 3a0a 2020 2020 2020 2020 2020 2020 525f  :.            R_
-00010cb0: 6f76 6572 6c61 705f 6c69 7374 2a3d 525f  overlap_list*=R_
-00010cc0: 6f76 6572 6c61 700a 2020 2020 2020 2020  overlap.        
-00010cd0: 2320 656c 7365 3a0a 2020 2020 2020 2020  # else:.        
-00010ce0: 2320 2020 2020 525f 6f76 6572 6c61 705f  #     R_overlap_
-00010cf0: 6c69 7374 2a3d 3165 350a 2020 2020 6966  list*=1e5.    if
-00010d00: 206e 702e 7375 6d28 6c69 6e65 5f6f 7665   np.sum(line_ove
-00010d10: 726c 6170 5f6c 6973 7429 3d3d 322a 6e6d  rlap_list)==2*nm
-00010d20: 6f64 656c 733a 0a20 2020 2020 2020 2069  odels:.        i
-00010d30: 6620 6e6f 7420 286c 696e 655f 6f76 6572  f not (line_over
-00010d40: 6c61 7020 6973 204e 6f6e 6529 3a0a 2020  lap is None):.  
-00010d50: 2020 2020 2020 2020 2020 6c69 6e65 5f6f            line_o
-00010d60: 7665 726c 6170 5f6c 6973 742a 3d6e 702e  verlap_list*=np.
-00010d70: 6172 7261 7928 6c69 6e65 5f6f 7665 726c  array(line_overl
-00010d80: 6170 290a 2020 2020 2020 2020 2320 656c  ap).        # el
-00010d90: 7365 3a0a 2020 2020 2020 2020 2320 2020  se:.        #   
-00010da0: 2020 6c69 6e65 5f6f 7665 726c 6170 5f6c    line_overlap_l
-00010db0: 6973 742a 3d6e 702e 6172 7261 7928 2834  ist*=np.array((4
-00010dc0: 2c33 3029 290a 0a20 2020 206f 732e 7379  ,30))..    os.sy
-00010dd0: 7374 656d 2866 2774 6f75 6368 207b 6469  stem(f'touch {di
-00010de0: 7265 6374 6f72 792b 222f 536c 6162 496e  rectory+"/SlabIn
-00010df0: 7075 742e 696e 227d 2729 0a20 2020 2066  put.in"}').    f
-00010e00: 3d6f 7065 6e28 6469 7265 6374 6f72 792b  =open(directory+
-00010e10: 272f 536c 6162 496e 7075 742e 696e 272c  '/SlabInput.in',
-00010e20: 2777 2729 0a20 2020 2066 2e77 7269 7465  'w').    f.write
-00010e30: 2822 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ("**************
+00006ed0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00006ee0: 6574 5f64 6174 612e 6164 645f 6d6f 6465  et_data.add_mode
+00006ef0: 6c28 7365 6c66 2e6d 6f64 656c 735b 695d  l(self.models[i]
+00006f00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006f10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00006f20: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00006f30: 6520 4b65 7945 7272 6f72 2827 556e 7265  e KeyError('Unre
+00006f40: 636f 676e 6973 6564 2070 6172 616d 6574  cognised paramet
+00006f50: 6572 2066 6f72 2073 6c69 6369 6e67 2729  er for slicing')
+00006f60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00006f70: 7265 745f 6461 7461 0a0a 2020 2020 6465  ret_data..    de
+00006f80: 6620 636f 6e76 6f6c 7665 2873 656c 662c  f convolve(self,
+00006f90: 6672 6571 5f62 696e 733d 4e6f 6e65 2c52  freq_bins=None,R
+00006fa0: 3d31 2c6c 616d 6264 615f 303d 312c 6c61  =1,lambda_0=1,la
+00006fb0: 6d62 6461 5f6e 3d31 2c76 723d 3133 3030  mbda_n=1,vr=1300
+00006fc0: 2c4e 4c54 453d 4661 6c73 652c 636f 6e76  ,NLTE=False,conv
+00006fd0: 5f74 7970 653d 312c 7665 7262 6f73 653d  _type=1,verbose=
+00006fe0: 5472 7565 293a 0a20 2020 2020 2020 2066  True):.        f
+00006ff0: 6f72 2069 2c64 2069 6e20 656e 756d 6572  or i,d in enumer
+00007000: 6174 6528 7365 6c66 2e6d 6f64 656c 7329  ate(self.models)
+00007010: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00007020: 2076 6572 626f 7365 3a20 7072 696e 7428   verbose: print(
+00007030: 275c 6e27 2c69 2b31 2c27 3b20 4d6f 6465  '\n',i+1,'; Mode
+00007040: 6c20 6e75 6d62 6572 2027 2c73 656c 662e  l number ',self.
+00007050: 6d6f 6465 6c73 5b69 5d2e 6d6f 6465 6c5f  models[i].model_
+00007060: 6e75 6d62 6572 2c27 3b20 5370 6563 6965  number,'; Specie
+00007070: 7320 6e75 6d62 6572 2027 2c73 656c 662e  s number ',self.
+00007080: 6d6f 6465 6c73 5b69 5d2e 7370 6563 6965  models[i].specie
+00007090: 735f 6e75 6d62 6572 290a 2020 2020 2020  s_number).      
+000070a0: 2020 2020 2020 642e 636f 6e76 6f6c 7665        d.convolve
+000070b0: 2866 7265 715f 6269 6e73 3d66 7265 715f  (freq_bins=freq_
+000070c0: 6269 6e73 2c52 3d52 2c6c 616d 6264 615f  bins,R=R,lambda_
+000070d0: 303d 6c61 6d62 6461 5f30 2c6c 616d 6264  0=lambda_0,lambd
+000070e0: 615f 6e3d 6c61 6d62 6461 5f6e 2c76 723d  a_n=lambda_n,vr=
+000070f0: 7672 2c4e 4c54 453d 4e4c 5445 2c63 6f6e  vr,NLTE=NLTE,con
+00007100: 765f 7479 7065 3d63 6f6e 765f 7479 7065  v_type=conv_type
+00007110: 290a 0a20 2020 2064 6566 2063 6f6e 766f  )..    def convo
+00007120: 6c76 655f 6f76 6572 6c61 7028 7365 6c66  lve_overlap(self
+00007130: 2c52 3d31 2c6c 616d 6264 615f 303d 312c  ,R=1,lambda_0=1,
+00007140: 6c61 6d62 6461 5f6e 3d31 2c76 6572 626f  lambda_n=1,verbo
+00007150: 7365 3d54 7275 6529 3a0a 2020 2020 2020  se=True):.      
+00007160: 2020 666f 7220 692c 6420 696e 2065 6e75    for i,d in enu
+00007170: 6d65 7261 7465 2873 656c 662e 6d6f 6465  merate(self.mode
+00007180: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00007190: 2069 6620 7665 7262 6f73 653a 2070 7269   if verbose: pri
+000071a0: 6e74 2827 5c6e 272c 692b 312c 273b 204d  nt('\n',i+1,'; M
+000071b0: 6f64 656c 206e 756d 6265 7220 272c 7365  odel number ',se
+000071c0: 6c66 2e6d 6f64 656c 735b 695d 2e6d 6f64  lf.models[i].mod
+000071d0: 656c 5f6e 756d 6265 7229 0a20 2020 2020  el_number).     
+000071e0: 2020 2020 2020 2064 2e63 6f6e 766f 6c76         d.convolv
+000071f0: 655f 6f76 6572 6c61 7028 523d 522c 6c61  e_overlap(R=R,la
+00007200: 6d62 6461 5f30 3d6c 616d 6264 615f 302c  mbda_0=lambda_0,
+00007210: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
+00007220: 6e29 0a0a 2020 2020 4070 726f 7065 7274  n)..    @propert
+00007230: 790a 2020 2020 6465 6620 6e6d 6f64 656c  y.    def nmodel
+00007240: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00007250: 2073 656c 662e 5f6e 6d6f 6465 6c73 3d6c   self._nmodels=l
+00007260: 656e 2873 656c 662e 6d6f 6465 6c73 290a  en(self.models).
+00007270: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00007280: 656c 662e 5f6e 6d6f 6465 6c73 0a0a 2020  elf._nmodels..  
+00007290: 2020 406e 6d6f 6465 6c73 2e73 6574 7465    @nmodels.sette
+000072a0: 720a 2020 2020 6465 6620 6e6d 6f64 656c  r.    def nmodel
+000072b0: 7328 7365 6c66 2c76 616c 7565 293a 0a20  s(self,value):. 
+000072c0: 2020 2020 2020 2073 656c 662e 5f6e 6d6f         self._nmo
+000072d0: 6465 6c73 3d76 616c 7565 0a0a 2020 2020  dels=value..    
+000072e0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+000072f0: 6620 7370 6563 6965 735f 6e75 6d62 6572  f species_number
+00007300: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007310: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+00007320: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+00007330: 656c 662e 5f73 7065 6369 6573 5f6e 756d  elf._species_num
+00007340: 6265 723d 5b5d 0a20 2020 2020 2020 2020  ber=[].         
+00007350: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00007360: 6528 7365 6c66 2e6e 6d6f 6465 6c73 293a  e(self.nmodels):
+00007370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007380: 2073 656c 662e 5f73 7065 6369 6573 5f6e   self._species_n
+00007390: 756d 6265 722e 6170 7065 6e64 2873 656c  umber.append(sel
+000073a0: 662e 6d6f 6465 6c73 5b69 5d2e 7370 6563  f.models[i].spec
+000073b0: 6965 735f 6e75 6d62 6572 290a 2020 2020  ies_number).    
+000073c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000073d0: 2020 2020 2020 7365 6c66 2e5f 7370 6563        self._spec
+000073e0: 6965 735f 6e75 6d62 6572 3d73 656c 662e  ies_number=self.
+000073f0: 6d6f 6465 6c73 5b30 5d2e 7370 6563 6965  models[0].specie
+00007400: 735f 6e75 6d62 6572 0a20 2020 2020 2020  s_number.       
+00007410: 2072 6574 7572 6e20 7365 6c66 2e5f 7370   return self._sp
+00007420: 6563 6965 735f 6e75 6d62 6572 0a0a 2020  ecies_number..  
+00007430: 2020 4073 7065 6369 6573 5f6e 756d 6265    @species_numbe
+00007440: 722e 7365 7474 6572 0a20 2020 2064 6566  r.setter.    def
+00007450: 2073 7065 6369 6573 5f6e 756d 6265 7228   species_number(
+00007460: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+00007470: 2020 2020 2073 656c 662e 5f73 7065 6369       self._speci
+00007480: 6573 5f6e 756d 6265 723d 7661 6c75 650a  es_number=value.
+00007490: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+000074a0: 2020 2064 6566 206d 6f64 656c 5f6e 756d     def model_num
+000074b0: 6265 7228 7365 6c66 293a 0a20 2020 2020  ber(self):.     
+000074c0: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
+000074d0: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
+000074e0: 2020 7365 6c66 2e5f 6d6f 6465 6c5f 6e75    self._model_nu
+000074f0: 6d62 6572 3d5b 5d0a 2020 2020 2020 2020  mber=[].        
+00007500: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00007510: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+00007520: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007530: 2020 7365 6c66 2e5f 6d6f 6465 6c5f 6e75    self._model_nu
+00007540: 6d62 6572 2e61 7070 656e 6428 7365 6c66  mber.append(self
+00007550: 2e6d 6f64 656c 735b 695d 2e6d 6f64 656c  .models[i].model
+00007560: 5f6e 756d 6265 7229 0a20 2020 2020 2020  _number).       
+00007570: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00007580: 2020 2073 656c 662e 5f6d 6f64 656c 5f6e     self._model_n
+00007590: 756d 6265 723d 7365 6c66 2e6d 6f64 656c  umber=self.model
+000075a0: 735b 305d 2e6d 6f64 656c 5f6e 756d 6265  s[0].model_numbe
+000075b0: 720a 2020 2020 2020 2020 7265 7475 726e  r.        return
+000075c0: 2073 656c 662e 5f6d 6f64 656c 5f6e 756d   self._model_num
+000075d0: 6265 720a 0a20 2020 2040 6d6f 6465 6c5f  ber..    @model_
+000075e0: 6e75 6d62 6572 2e73 6574 7465 720a 2020  number.setter.  
+000075f0: 2020 6465 6620 6d6f 6465 6c5f 6e75 6d62    def model_numb
+00007600: 6572 2873 656c 662c 7661 6c75 6529 3a0a  er(self,value):.
+00007610: 2020 2020 2020 2020 7365 6c66 2e5f 6d6f          self._mo
+00007620: 6465 6c5f 6e75 6d62 6572 3d76 616c 7565  del_number=value
+00007630: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00007640: 2020 2020 6465 6620 4e48 2873 656c 6629      def NH(self)
+00007650: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00007660: 662e 6e6d 6f64 656c 733e 313a 0a20 2020  f.nmodels>1:.   
+00007670: 2020 2020 2020 2020 2073 656c 662e 5f4e           self._N
+00007680: 483d 5b5d 0a20 2020 2020 2020 2020 2020  H=[].           
+00007690: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+000076a0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
+000076b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000076c0: 656c 662e 5f4e 482e 6170 7065 6e64 2873  elf._NH.append(s
+000076d0: 656c 662e 6d6f 6465 6c73 5b69 5d2e 4e48  elf.models[i].NH
+000076e0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+000076f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007700: 2e5f 4e48 3d73 656c 662e 6d6f 6465 6c73  ._NH=self.models
+00007710: 5b30 5d2e 4e48 0a20 2020 2020 2020 2072  [0].NH.        r
+00007720: 6574 7572 6e20 7365 6c66 2e5f 4e48 0a0a  eturn self._NH..
+00007730: 2020 2020 404e 482e 7365 7474 6572 0a20      @NH.setter. 
+00007740: 2020 2064 6566 204e 4828 7365 6c66 2c76     def NH(self,v
+00007750: 616c 7565 293a 0a20 2020 2020 2020 2073  alue):.        s
+00007760: 656c 662e 5f4e 483d 7661 6c75 650a 0a20  elf._NH=value.. 
+00007770: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00007780: 2064 6566 206e 436f 6c6c 2873 656c 6629   def nColl(self)
+00007790: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+000077a0: 662e 6e6d 6f64 656c 733e 313a 0a20 2020  f.nmodels>1:.   
+000077b0: 2020 2020 2020 2020 2073 656c 662e 5f6e           self._n
+000077c0: 436f 6c6c 3d5b 5d0a 2020 2020 2020 2020  Coll=[].        
+000077d0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+000077e0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+000077f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007800: 2020 7365 6c66 2e5f 6e43 6f6c 6c2e 6170    self._nColl.ap
+00007810: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
+00007820: 5b69 5d2e 6e43 6f6c 6c29 0a20 2020 2020  [i].nColl).     
+00007830: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00007840: 2020 2020 2073 656c 662e 5f6e 436f 6c6c       self._nColl
+00007850: 3d73 656c 662e 6d6f 6465 6c73 5b30 5d2e  =self.models[0].
+00007860: 6e43 6f6c 6c0a 2020 2020 2020 2020 7265  nColl.        re
+00007870: 7475 726e 2073 656c 662e 5f6e 436f 6c6c  turn self._nColl
+00007880: 0a0a 2020 2020 406e 436f 6c6c 2e73 6574  ..    @nColl.set
+00007890: 7465 720a 2020 2020 6465 6620 6e43 6f6c  ter.    def nCol
+000078a0: 6c28 7365 6c66 2c76 616c 7565 293a 0a20  l(self,value):. 
+000078b0: 2020 2020 2020 2073 656c 662e 5f6e 436f         self._nCo
+000078c0: 6c6c 3d76 616c 7565 0a0a 2020 2020 4070  ll=value..    @p
+000078d0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+000078e0: 6e65 2873 656c 6629 3a0a 2020 2020 2020  ne(self):.      
+000078f0: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
+00007900: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
+00007910: 2073 656c 662e 5f6e 653d 5b5d 0a20 2020   self._ne=[].   
+00007920: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00007930: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+00007940: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00007950: 2020 2020 2020 2073 656c 662e 5f6e 652e         self._ne.
+00007960: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
+00007970: 6c73 5b69 5d2e 6e65 290a 2020 2020 2020  ls[i].ne).      
+00007980: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00007990: 2020 2020 7365 6c66 2e5f 6e65 3d73 656c      self._ne=sel
+000079a0: 662e 6d6f 6465 6c73 5b30 5d2e 6e65 0a20  f.models[0].ne. 
+000079b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000079c0: 6c66 2e5f 6e65 0a0a 2020 2020 406e 652e  lf._ne..    @ne.
+000079d0: 7365 7474 6572 0a20 2020 2064 6566 206e  setter.    def n
+000079e0: 6528 7365 6c66 2c76 616c 7565 293a 0a20  e(self,value):. 
+000079f0: 2020 2020 2020 2073 656c 662e 5f6e 653d         self._ne=
+00007a00: 7661 6c75 650a 0a20 2020 2040 7072 6f70  value..    @prop
+00007a10: 6572 7479 0a20 2020 2064 6566 206e 4865  erty.    def nHe
+00007a20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007a30: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+00007a40: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+00007a50: 656c 662e 5f6e 4865 3d5b 5d0a 2020 2020  elf._nHe=[].    
+00007a60: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00007a70: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
+00007a80: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+00007a90: 2020 2020 2020 7365 6c66 2e5f 6e48 652e        self._nHe.
+00007aa0: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
+00007ab0: 6c73 5b69 5d2e 6e48 6529 0a20 2020 2020  ls[i].nHe).     
+00007ac0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00007ad0: 2020 2020 2073 656c 662e 5f6e 4865 3d73       self._nHe=s
+00007ae0: 656c 662e 6d6f 6465 6c73 5b30 5d2e 6e48  elf.models[0].nH
+00007af0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+00007b00: 2073 656c 662e 5f6e 4865 0a0a 2020 2020   self._nHe..    
+00007b10: 406e 4865 2e73 6574 7465 720a 2020 2020  @nHe.setter.    
+00007b20: 6465 6620 6e48 6528 7365 6c66 2c76 616c  def nHe(self,val
+00007b30: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
+00007b40: 662e 5f6e 4865 3d76 616c 7565 0a0a 2020  f._nHe=value..  
+00007b50: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00007b60: 6465 6620 6e48 4949 2873 656c 6629 3a0a  def nHII(self):.
+00007b70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00007b80: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
+00007b90: 2020 2020 2020 2073 656c 662e 5f6e 4849         self._nHI
+00007ba0: 493d 5b5d 0a20 2020 2020 2020 2020 2020  I=[].           
+00007bb0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00007bc0: 7365 6c66 2e6e 6d6f 6465 6c73 293a 0a20  self.nmodels):. 
+00007bd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007be0: 656c 662e 5f6e 4849 492e 6170 7065 6e64  elf._nHII.append
+00007bf0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
+00007c00: 6e48 4949 290a 2020 2020 2020 2020 656c  nHII).        el
+00007c10: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00007c20: 7365 6c66 2e5f 6e48 4949 3d73 656c 662e  self._nHII=self.
+00007c30: 6d6f 6465 6c73 5b30 5d2e 6e48 4949 0a20  models[0].nHII. 
+00007c40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00007c50: 6c66 2e5f 6e48 4949 0a0a 2020 2020 406e  lf._nHII..    @n
+00007c60: 4849 492e 7365 7474 6572 0a20 2020 2064  HII.setter.    d
+00007c70: 6566 206e 4849 4928 7365 6c66 2c76 616c  ef nHII(self,val
+00007c80: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
+00007c90: 662e 5f6e 4849 493d 7661 6c75 650a 0a20  f._nHII=value.. 
+00007ca0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00007cb0: 2064 6566 206e 4849 2873 656c 6629 3a0a   def nHI(self):.
+00007cc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00007cd0: 6e6d 6f64 656c 733e 313a 0a20 2020 2020  nmodels>1:.     
+00007ce0: 2020 2020 2020 2073 656c 662e 5f6e 4849         self._nHI
+00007cf0: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
+00007d00: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+00007d10: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
+00007d20: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00007d30: 6c66 2e5f 6e48 492e 6170 7065 6e64 2873  lf._nHI.append(s
+00007d40: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6e48  elf.models[i].nH
+00007d50: 4929 0a20 2020 2020 2020 2065 6c73 653a  I).        else:
+00007d60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007d70: 662e 5f6e 4849 3d73 656c 662e 6d6f 6465  f._nHI=self.mode
+00007d80: 6c73 5b30 5d2e 6e48 490a 2020 2020 2020  ls[0].nHI.      
+00007d90: 2020 7265 7475 726e 2073 656c 662e 5f6e    return self._n
+00007da0: 4849 0a0a 2020 2020 406e 4849 2e73 6574  HI..    @nHI.set
+00007db0: 7465 720a 2020 2020 6465 6620 6e48 4928  ter.    def nHI(
+00007dc0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+00007dd0: 2020 2020 2073 656c 662e 5f6e 4849 3d76       self._nHI=v
+00007de0: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
+00007df0: 7274 790a 2020 2020 6465 6620 6e48 3228  rty.    def nH2(
+00007e00: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00007e10: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
+00007e20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00007e30: 6c66 2e5f 6e48 323d 5b5d 0a20 2020 2020  lf._nH2=[].     
+00007e40: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00007e50: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+00007e60: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00007e70: 2020 2020 2073 656c 662e 5f6e 4832 2e61       self._nH2.a
+00007e80: 7070 656e 6428 7365 6c66 2e6d 6f64 656c  ppend(self.model
+00007e90: 735b 695d 2e6e 4832 290a 2020 2020 2020  s[i].nH2).      
+00007ea0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00007eb0: 2020 2020 7365 6c66 2e5f 6e48 323d 7365      self._nH2=se
+00007ec0: 6c66 2e6d 6f64 656c 735b 305d 2e6e 4832  lf.models[0].nH2
+00007ed0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007ee0: 7365 6c66 2e5f 6e48 320a 0a20 2020 2040  self._nH2..    @
+00007ef0: 6e48 322e 7365 7474 6572 0a20 2020 2064  nH2.setter.    d
+00007f00: 6566 206e 4832 2873 656c 662c 7661 6c75  ef nH2(self,valu
+00007f10: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00007f20: 2e5f 6e48 323d 7661 6c75 650a 0a20 2020  ._nH2=value..   
+00007f30: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00007f40: 6566 2064 7573 745f 746f 5f67 6173 2873  ef dust_to_gas(s
+00007f50: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+00007f60: 2073 656c 662e 6e6d 6f64 656c 733e 313a   self.nmodels>1:
+00007f70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007f80: 662e 5f64 7573 745f 746f 5f67 6173 3d5b  f._dust_to_gas=[
+00007f90: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00007fa0: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+00007fb0: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+00007fc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007fd0: 2e5f 6475 7374 5f74 6f5f 6761 732e 6170  ._dust_to_gas.ap
+00007fe0: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
+00007ff0: 5b69 5d2e 6475 7374 5f74 6f5f 6761 7329  [i].dust_to_gas)
+00008000: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00008010: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008020: 5f64 7573 745f 746f 5f67 6173 3d73 656c  _dust_to_gas=sel
+00008030: 662e 6d6f 6465 6c73 5b30 5d2e 6475 7374  f.models[0].dust
+00008040: 5f74 6f5f 6761 730a 2020 2020 2020 2020  _to_gas.        
+00008050: 7265 7475 726e 2073 656c 662e 5f64 7573  return self._dus
+00008060: 745f 746f 5f67 6173 0a0a 2020 2020 4064  t_to_gas..    @d
+00008070: 7573 745f 746f 5f67 6173 2e73 6574 7465  ust_to_gas.sette
+00008080: 720a 2020 2020 6465 6620 6475 7374 5f74  r.    def dust_t
+00008090: 6f5f 6761 7328 7365 6c66 2c76 616c 7565  o_gas(self,value
+000080a0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000080b0: 5f64 7573 745f 746f 5f67 6173 3d76 616c  _dust_to_gas=val
+000080c0: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
+000080d0: 790a 2020 2020 6465 6620 7674 7572 6228  y.    def vturb(
+000080e0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+000080f0: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
+00008100: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00008110: 6c66 2e5f 7674 7572 623d 5b5d 0a20 2020  lf._vturb=[].   
+00008120: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00008130: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+00008140: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00008150: 2020 2020 2020 2073 656c 662e 5f76 7475         self._vtu
+00008160: 7262 2e61 7070 656e 6428 7365 6c66 2e6d  rb.append(self.m
+00008170: 6f64 656c 735b 695d 2e76 7475 7262 290a  odels[i].vturb).
+00008180: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00008190: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000081a0: 7674 7572 623d 7365 6c66 2e6d 6f64 656c  vturb=self.model
+000081b0: 735b 305d 2e76 7475 7262 0a20 2020 2020  s[0].vturb.     
+000081c0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000081d0: 7674 7572 620a 0a20 2020 2040 7674 7572  vturb..    @vtur
+000081e0: 622e 7365 7474 6572 0a20 2020 2064 6566  b.setter.    def
+000081f0: 2076 7475 7262 2873 656c 662c 7661 6c75   vturb(self,valu
+00008200: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00008210: 2e5f 7674 7572 623d 7661 6c75 650a 0a20  ._vturb=value.. 
+00008220: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00008230: 2064 6566 2054 6728 7365 6c66 293a 0a20   def Tg(self):. 
+00008240: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+00008250: 6d6f 6465 6c73 3e31 3a0a 2020 2020 2020  models>1:.      
+00008260: 2020 2020 2020 7365 6c66 2e5f 5467 3d5b        self._Tg=[
+00008270: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00008280: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+00008290: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+000082a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000082b0: 2e5f 5467 2e61 7070 656e 6428 7365 6c66  ._Tg.append(self
+000082c0: 2e6d 6f64 656c 735b 695d 2e54 6729 0a20  .models[i].Tg). 
+000082d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000082e0: 2020 2020 2020 2020 2073 656c 662e 5f54           self._T
+000082f0: 673d 7365 6c66 2e6d 6f64 656c 735b 305d  g=self.models[0]
+00008300: 2e54 670a 2020 2020 2020 2020 7265 7475  .Tg.        retu
+00008310: 726e 2073 656c 662e 5f54 670a 0a20 2020  rn self._Tg..   
+00008320: 2040 5467 2e73 6574 7465 720a 2020 2020   @Tg.setter.    
+00008330: 6465 6620 5467 2873 656c 662c 7661 6c75  def Tg(self,valu
+00008340: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00008350: 2e5f 5467 3d76 616c 7565 0a0a 2020 2020  ._Tg=value..    
+00008360: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00008370: 6620 5464 2873 656c 6629 3a0a 2020 2020  f Td(self):.    
+00008380: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
+00008390: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
+000083a0: 2020 2073 656c 662e 5f54 643d 5b5d 0a20     self._Td=[]. 
+000083b0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000083c0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+000083d0: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+000083e0: 2020 2020 2020 2020 2073 656c 662e 5f54           self._T
+000083f0: 642e 6170 7065 6e64 2873 656c 662e 6d6f  d.append(self.mo
+00008400: 6465 6c73 5b69 5d2e 5464 290a 2020 2020  dels[i].Td).    
+00008410: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008420: 2020 2020 2020 7365 6c66 2e5f 5464 3d73        self._Td=s
+00008430: 656c 662e 6d6f 6465 6c73 5b30 5d2e 5464  elf.models[0].Td
+00008440: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008450: 7365 6c66 2e5f 5464 0a0a 2020 2020 4054  self._Td..    @T
+00008460: 642e 7365 7474 6572 0a20 2020 2064 6566  d.setter.    def
+00008470: 2054 6428 7365 6c66 2c76 616c 7565 293a   Td(self,value):
+00008480: 0a20 2020 2020 2020 2073 656c 662e 5f54  .        self._T
+00008490: 643d 7661 6c75 650a 0a20 2020 2040 7072  d=value..    @pr
+000084a0: 6f70 6572 7479 0a20 2020 2064 6566 2073  operty.    def s
+000084b0: 7065 6369 6573 5f6e 616d 6528 7365 6c66  pecies_name(self
+000084c0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+000084d0: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
+000084e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000084f0: 7370 6563 6965 735f 6e61 6d65 3d5b 5d0a  species_name=[].
+00008500: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00008510: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+00008520: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00008530: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00008540: 7370 6563 6965 735f 6e61 6d65 2e61 7070  species_name.app
+00008550: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+00008560: 695d 2e73 7065 6369 6573 5f6e 616d 6529  i].species_name)
+00008570: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00008580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008590: 5f73 7065 6369 6573 5f6e 616d 653d 7365  _species_name=se
+000085a0: 6c66 2e6d 6f64 656c 735b 305d 2e73 7065  lf.models[0].spe
+000085b0: 6369 6573 5f6e 616d 650a 2020 2020 2020  cies_name.      
+000085c0: 2020 7265 7475 726e 2073 656c 662e 5f73    return self._s
+000085d0: 7065 6369 6573 5f6e 616d 650a 0a20 2020  pecies_name..   
+000085e0: 2040 7370 6563 6965 735f 6e61 6d65 2e73   @species_name.s
+000085f0: 6574 7465 720a 2020 2020 6465 6620 7370  etter.    def sp
+00008600: 6563 6965 735f 6e61 6d65 2873 656c 662c  ecies_name(self,
+00008610: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
+00008620: 7365 6c66 2e5f 7370 6563 6965 735f 6e61  self._species_na
+00008630: 6d65 3d76 616c 7565 0a0a 2020 2020 4070  me=value..    @p
+00008640: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00008650: 7370 6563 6965 735f 696e 6465 7828 7365  species_index(se
+00008660: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+00008670: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
+00008680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008690: 2e5f 7370 6563 6965 735f 696e 6465 783d  ._species_index=
+000086a0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+000086b0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+000086c0: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+000086d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000086e0: 662e 5f73 7065 6369 6573 5f69 6e64 6578  f._species_index
+000086f0: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
+00008700: 656c 735b 695d 2e73 7065 6369 6573 5f69  els[i].species_i
+00008710: 6e64 6578 290a 2020 2020 2020 2020 656c  ndex).        el
+00008720: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00008730: 7365 6c66 2e5f 7370 6563 6965 735f 696e  self._species_in
+00008740: 6465 783d 7365 6c66 2e6d 6f64 656c 735b  dex=self.models[
+00008750: 305d 2e73 7065 6369 6573 5f69 6e64 6578  0].species_index
+00008760: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008770: 7365 6c66 2e5f 7370 6563 6965 735f 696e  self._species_in
+00008780: 6465 780a 0a20 2020 2040 7370 6563 6965  dex..    @specie
+00008790: 735f 696e 6465 782e 7365 7474 6572 0a20  s_index.setter. 
+000087a0: 2020 2064 6566 2073 7065 6369 6573 5f69     def species_i
+000087b0: 6e64 6578 2873 656c 662c 7661 6c75 6529  ndex(self,value)
+000087c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+000087d0: 7370 6563 6965 735f 696e 6465 783d 7661  species_index=va
+000087e0: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
+000087f0: 7479 0a20 2020 2064 6566 2061 6275 6e64  ty.    def abund
+00008800: 616e 6365 2873 656c 6629 3a0a 2020 2020  ance(self):.    
+00008810: 2020 2020 6966 2073 656c 662e 6e6d 6f64      if self.nmod
+00008820: 656c 733e 313a 0a20 2020 2020 2020 2020  els>1:.         
+00008830: 2020 2073 656c 662e 5f61 6275 6e64 616e     self._abundan
+00008840: 6365 3d5b 5d0a 2020 2020 2020 2020 2020  ce=[].          
+00008850: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00008860: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
+00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008880: 7365 6c66 2e5f 6162 756e 6461 6e63 652e  self._abundance.
+00008890: 6170 7065 6e64 2873 656c 662e 6d6f 6465  append(self.mode
+000088a0: 6c73 5b69 5d2e 6162 756e 6461 6e63 6529  ls[i].abundance)
+000088b0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000088c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000088d0: 5f61 6275 6e64 616e 6365 3d73 656c 662e  _abundance=self.
+000088e0: 6d6f 6465 6c73 5b30 5d2e 6162 756e 6461  models[0].abunda
+000088f0: 6e63 650a 2020 2020 2020 2020 7265 7475  nce.        retu
+00008900: 726e 2073 656c 662e 5f61 6275 6e64 616e  rn self._abundan
+00008910: 6365 0a0a 2020 2020 4061 6275 6e64 616e  ce..    @abundan
+00008920: 6365 2e73 6574 7465 720a 2020 2020 6465  ce.setter.    de
+00008930: 6620 6162 756e 6461 6e63 6528 7365 6c66  f abundance(self
+00008940: 2c76 616c 7565 293a 0a20 2020 2020 2020  ,value):.       
+00008950: 2073 656c 662e 5f61 6275 6e64 616e 6365   self._abundance
+00008960: 3d76 616c 7565 0a0a 2020 2020 4070 726f  =value..    @pro
+00008970: 7065 7274 790a 2020 2020 6465 6620 6476  perty.    def dv
+00008980: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00008990: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+000089a0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+000089b0: 656c 662e 5f64 763d 5b5d 0a20 2020 2020  elf._dv=[].     
+000089c0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000089d0: 7261 6e67 6528 7365 6c66 2e6e 6d6f 6465  range(self.nmode
+000089e0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+000089f0: 2020 2020 2073 656c 662e 5f64 762e 6170       self._dv.ap
+00008a00: 7065 6e64 2873 656c 662e 6d6f 6465 6c73  pend(self.models
+00008a10: 5b69 5d2e 6476 290a 2020 2020 2020 2020  [i].dv).        
+00008a20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00008a30: 2020 7365 6c66 2e5f 6476 3d73 656c 662e    self._dv=self.
+00008a40: 6d6f 6465 6c73 5b30 5d2e 6476 0a20 2020  models[0].dv.   
+00008a50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00008a60: 2e5f 6476 0a0a 2020 2020 4064 762e 7365  ._dv..    @dv.se
+00008a70: 7474 6572 0a20 2020 2064 6566 2064 7628  tter.    def dv(
+00008a80: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+00008a90: 2020 2020 2073 656c 662e 5f64 763d 7661       self._dv=va
+00008aa0: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
+00008ab0: 7479 0a20 2020 2064 6566 206e 6c65 7665  ty.    def nleve
+00008ac0: 6c73 2873 656c 6629 3a0a 2020 2020 2020  ls(self):.      
+00008ad0: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
+00008ae0: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
+00008af0: 2073 656c 662e 5f6e 6c65 7665 6c73 3d5b   self._nlevels=[
+00008b00: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00008b10: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+00008b20: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+00008b30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008b40: 2e5f 6e6c 6576 656c 732e 6170 7065 6e64  ._nlevels.append
+00008b50: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
+00008b60: 6e6c 6576 656c 7329 0a20 2020 2020 2020  nlevels).       
+00008b70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00008b80: 2020 2073 656c 662e 5f6e 6c65 7665 6c73     self._nlevels
+00008b90: 3d73 656c 662e 6d6f 6465 6c73 5b30 5d2e  =self.models[0].
+00008ba0: 6e6c 6576 656c 730a 2020 2020 2020 2020  nlevels.        
+00008bb0: 7265 7475 726e 2073 656c 662e 5f6e 6c65  return self._nle
+00008bc0: 7665 6c73 0a0a 2020 2020 406e 6c65 7665  vels..    @nleve
+00008bd0: 6c73 2e73 6574 7465 720a 2020 2020 6465  ls.setter.    de
+00008be0: 6620 6e6c 6576 656c 7328 7365 6c66 2c76  f nlevels(self,v
+00008bf0: 616c 7565 293a 0a20 2020 2020 2020 2073  alue):.        s
+00008c00: 656c 662e 5f6e 6c65 7665 6c73 3d76 616c  elf._nlevels=val
+00008c10: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
+00008c20: 790a 2020 2020 6465 6620 6e6c 696e 6573  y.    def nlines
+00008c30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00008c40: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+00008c50: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+00008c60: 656c 662e 5f6e 6c69 6e65 733d 5b5d 0a20  elf._nlines=[]. 
+00008c70: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00008c80: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+00008c90: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+00008ca0: 2020 2020 2020 2020 2073 656c 662e 5f6e           self._n
+00008cb0: 6c69 6e65 732e 6170 7065 6e64 2873 656c  lines.append(sel
+00008cc0: 662e 6d6f 6465 6c73 5b69 5d2e 6e6c 696e  f.models[i].nlin
+00008cd0: 6573 290a 2020 2020 2020 2020 656c 7365  es).        else
+00008ce0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00008cf0: 6c66 2e5f 6e6c 696e 6573 3d73 656c 662e  lf._nlines=self.
+00008d00: 6d6f 6465 6c73 5b30 5d2e 6e6c 696e 6573  models[0].nlines
+00008d10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008d20: 7365 6c66 2e5f 6e6c 696e 6573 0a0a 2020  self._nlines..  
+00008d30: 2020 406e 6c69 6e65 732e 7365 7474 6572    @nlines.setter
+00008d40: 0a20 2020 2064 6566 206e 6c69 6e65 7328  .    def nlines(
+00008d50: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+00008d60: 2020 2020 2073 656c 662e 5f6e 6c69 6e65       self._nline
+00008d70: 733d 7661 6c75 650a 0a20 2020 2040 7072  s=value..    @pr
+00008d80: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
+00008d90: 696e 6564 6174 6128 7365 6c66 293a 0a20  inedata(self):. 
+00008da0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+00008db0: 6d6f 6465 6c73 3e31 3a0a 2020 2020 2020  models>1:.      
+00008dc0: 2020 2020 2020 7365 6c66 2e5f 6c69 6e65        self._line
+00008dd0: 6461 7461 3d5b 5d0a 2020 2020 2020 2020  data=[].        
+00008de0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00008df0: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+00008e00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008e10: 2020 7365 6c66 2e5f 6c69 6e65 6461 7461    self._linedata
+00008e20: 2e61 7070 656e 6428 7365 6c66 2e6d 6f64  .append(self.mod
+00008e30: 656c 735b 695d 2e6c 696e 6564 6174 6129  els[i].linedata)
+00008e40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00008e50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008e60: 5f6c 696e 6564 6174 613d 7365 6c66 2e6d  _linedata=self.m
+00008e70: 6f64 656c 735b 305d 2e6c 696e 6564 6174  odels[0].linedat
+00008e80: 610a 2020 2020 2020 2020 7265 7475 726e  a.        return
+00008e90: 2073 656c 662e 5f6c 696e 6564 6174 610a   self._linedata.
+00008ea0: 0a20 2020 2040 6c69 6e65 6461 7461 2e73  .    @linedata.s
+00008eb0: 6574 7465 720a 2020 2020 6465 6620 6c69  etter.    def li
+00008ec0: 6e65 6461 7461 2873 656c 662c 7661 6c75  nedata(self,valu
+00008ed0: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00008ee0: 2e5f 6c69 6e65 6461 7461 3d76 616c 7565  ._linedata=value
+00008ef0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00008f00: 2020 2020 6465 6620 6c65 7665 6c64 6174      def leveldat
+00008f10: 6128 7365 6c66 293a 0a20 2020 2020 2020  a(self):.       
+00008f20: 2069 6620 7365 6c66 2e6e 6d6f 6465 6c73   if self.nmodels
+00008f30: 3e31 3a0a 2020 2020 2020 2020 2020 2020  >1:.            
+00008f40: 7365 6c66 2e5f 6c65 7665 6c64 6174 613d  self._leveldata=
+00008f50: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+00008f60: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+00008f70: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+00008f80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00008f90: 662e 5f6c 6576 656c 6461 7461 2e61 7070  f._leveldata.app
+00008fa0: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+00008fb0: 695d 2e6c 6576 656c 6461 7461 290a 2020  i].leveldata).  
+00008fc0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00008fd0: 2020 2020 2020 2020 7365 6c66 2e5f 6c65          self._le
+00008fe0: 7665 6c64 6174 613d 7365 6c66 2e6d 6f64  veldata=self.mod
+00008ff0: 656c 735b 305d 2e6c 6576 656c 6461 7461  els[0].leveldata
+00009000: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009010: 7365 6c66 2e5f 6c65 7665 6c64 6174 610a  self._leveldata.
+00009020: 0a20 2020 2040 6c65 7665 6c64 6174 612e  .    @leveldata.
+00009030: 7365 7474 6572 0a20 2020 2064 6566 206c  setter.    def l
+00009040: 6576 656c 6461 7461 2873 656c 662c 7661  eveldata(self,va
+00009050: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
+00009060: 6c66 2e5f 6c65 7665 6c64 6174 613d 7661  lf._leveldata=va
+00009070: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
+00009080: 7479 0a20 2020 2064 6566 2063 6f6e 7657  ty.    def convW
+00009090: 6176 656c 656e 6774 6828 7365 6c66 293a  avelength(self):
+000090a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000090b0: 2e6e 6d6f 6465 6c73 3e31 3a0a 2020 2020  .nmodels>1:.    
+000090c0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+000090d0: 6e76 5761 7665 6c65 6e67 7468 3d5b 5d0a  nvWavelength=[].
+000090e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000090f0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+00009100: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00009110: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00009120: 636f 6e76 5761 7665 6c65 6e67 7468 2e61  convWavelength.a
+00009130: 7070 656e 6428 7365 6c66 2e6d 6f64 656c  ppend(self.model
+00009140: 735b 695d 2e63 6f6e 7657 6176 656c 656e  s[i].convWavelen
+00009150: 6774 6829 0a20 2020 2020 2020 2065 6c73  gth).        els
+00009160: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00009170: 656c 662e 5f63 6f6e 7657 6176 656c 656e  elf._convWavelen
+00009180: 6774 683d 7365 6c66 2e6d 6f64 656c 735b  gth=self.models[
+00009190: 305d 2e63 6f6e 7657 6176 656c 656e 6774  0].convWavelengt
+000091a0: 680a 2020 2020 2020 2020 7265 7475 726e  h.        return
+000091b0: 2073 656c 662e 5f63 6f6e 7657 6176 656c   self._convWavel
+000091c0: 656e 6774 680a 0a20 2020 2040 636f 6e76  ength..    @conv
+000091d0: 5761 7665 6c65 6e67 7468 2e73 6574 7465  Wavelength.sette
+000091e0: 720a 2020 2020 6465 6620 636f 6e76 5761  r.    def convWa
+000091f0: 7665 6c65 6e67 7468 2873 656c 662c 7661  velength(self,va
+00009200: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
+00009210: 6c66 2e5f 636f 6e76 5761 7665 6c65 6e67  lf._convWaveleng
+00009220: 7468 3d76 616c 7565 0a0a 2020 2020 4070  th=value..    @p
+00009230: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00009240: 636f 6e76 4c54 4566 6c75 7828 7365 6c66  convLTEflux(self
+00009250: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00009260: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
+00009270: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00009280: 636f 6e76 4c54 4566 6c75 783d 5b5d 0a20  convLTEflux=[]. 
+00009290: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000092a0: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+000092b0: 6d6f 6465 6c73 293a 0a20 2020 2020 2020  models):.       
+000092c0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+000092d0: 6f6e 764c 5445 666c 7578 2e61 7070 656e  onvLTEflux.appen
+000092e0: 6428 7365 6c66 2e6d 6f64 656c 735b 695d  d(self.models[i]
+000092f0: 2e63 6f6e 764c 5445 666c 7578 290a 2020  .convLTEflux).  
+00009300: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00009310: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+00009320: 6e76 4c54 4566 6c75 783d 7365 6c66 2e6d  nvLTEflux=self.m
+00009330: 6f64 656c 735b 305d 2e63 6f6e 764c 5445  odels[0].convLTE
+00009340: 666c 7578 0a20 2020 2020 2020 2072 6574  flux.        ret
+00009350: 7572 6e20 7365 6c66 2e5f 636f 6e76 4c54  urn self._convLT
+00009360: 4566 6c75 780a 0a20 2020 2040 636f 6e76  Eflux..    @conv
+00009370: 4c54 4566 6c75 782e 7365 7474 6572 0a20  LTEflux.setter. 
+00009380: 2020 2064 6566 2063 6f6e 764c 5445 666c     def convLTEfl
+00009390: 7578 2873 656c 662c 7661 6c75 6529 3a0a  ux(self,value):.
+000093a0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+000093b0: 6e76 4c54 4566 6c75 783d 7661 6c75 650a  nvLTEflux=value.
+000093c0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+000093d0: 2020 2064 6566 2063 6f6e 764e 4c54 4566     def convNLTEf
+000093e0: 6c75 7828 7365 6c66 293a 0a20 2020 2020  lux(self):.     
+000093f0: 2020 2069 6620 7365 6c66 2e6e 6d6f 6465     if self.nmode
+00009400: 6c73 3e31 3a0a 2020 2020 2020 2020 2020  ls>1:.          
+00009410: 2020 7365 6c66 2e5f 636f 6e76 4e4c 5445    self._convNLTE
+00009420: 666c 7578 3d5b 5d0a 2020 2020 2020 2020  flux=[].        
+00009430: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00009440: 6765 2873 656c 662e 6e6d 6f64 656c 7329  ge(self.nmodels)
+00009450: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009460: 2020 7365 6c66 2e5f 636f 6e76 4e4c 5445    self._convNLTE
+00009470: 666c 7578 2e61 7070 656e 6428 7365 6c66  flux.append(self
+00009480: 2e6d 6f64 656c 735b 695d 2e63 6f6e 764e  .models[i].convN
+00009490: 4c54 4566 6c75 7829 0a20 2020 2020 2020  LTEflux).       
+000094a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000094b0: 2020 2073 656c 662e 5f63 6f6e 764e 4c54     self._convNLT
+000094c0: 4566 6c75 783d 7365 6c66 2e6d 6f64 656c  Eflux=self.model
+000094d0: 735b 305d 2e63 6f6e 764e 4c54 4566 6c75  s[0].convNLTEflu
+000094e0: 780a 2020 2020 2020 2020 7265 7475 726e  x.        return
+000094f0: 2073 656c 662e 5f63 6f6e 764e 4c54 4566   self._convNLTEf
+00009500: 6c75 780a 0a20 2020 2040 636f 6e76 4e4c  lux..    @convNL
+00009510: 5445 666c 7578 2e73 6574 7465 720a 2020  TEflux.setter.  
+00009520: 2020 6465 6620 636f 6e76 4e4c 5445 666c    def convNLTEfl
+00009530: 7578 2873 656c 662c 7661 6c75 6529 3a0a  ux(self,value):.
+00009540: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+00009550: 6e76 4e4c 5445 666c 7578 3d76 616c 7565  nvNLTEflux=value
+00009560: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00009570: 2020 2020 6465 6620 636f 6e76 5479 7065      def convType
+00009580: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00009590: 6966 2073 656c 662e 6e6d 6f64 656c 733e  if self.nmodels>
+000095a0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+000095b0: 656c 662e 5f63 6f6e 7654 7970 653d 5b5d  elf._convType=[]
+000095c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000095d0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+000095e0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+000095f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009600: 5f63 6f6e 7654 7970 652e 6170 7065 6e64  _convType.append
+00009610: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
+00009620: 636f 6e76 5479 7065 290a 2020 2020 2020  convType).      
+00009630: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00009640: 2020 2020 7365 6c66 2e5f 636f 6e76 5479      self._convTy
+00009650: 7065 3d73 656c 662e 6d6f 6465 6c73 5b30  pe=self.models[0
+00009660: 5d2e 636f 6e76 5479 7065 0a20 2020 2020  ].convType.     
+00009670: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00009680: 636f 6e76 5479 7065 0a0a 2020 2020 4063  convType..    @c
+00009690: 6f6e 7654 7970 652e 7365 7474 6572 0a20  onvType.setter. 
+000096a0: 2020 2064 6566 2063 6f6e 7654 7970 6528     def convType(
+000096b0: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
+000096c0: 2020 2020 2073 656c 662e 5f63 6f6e 7654       self._convT
+000096d0: 7970 653d 7661 6c75 650a 0a20 2020 2040  ype=value..    @
+000096e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000096f0: 2063 6f6e 7652 2873 656c 6629 3a0a 2020   convR(self):.  
+00009700: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
+00009710: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
+00009720: 2020 2020 2073 656c 662e 5f63 6f6e 7652       self._convR
+00009730: 3d5b 5d0a 2020 2020 2020 2020 2020 2020  =[].            
+00009740: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+00009750: 656c 662e 6e6d 6f64 656c 7329 3a0a 2020  elf.nmodels):.  
+00009760: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00009770: 6c66 2e5f 636f 6e76 522e 6170 7065 6e64  lf._convR.append
+00009780: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
+00009790: 636f 6e76 5229 0a20 2020 2020 2020 2065  convR).        e
+000097a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000097b0: 2073 656c 662e 5f63 6f6e 7652 3d73 656c   self._convR=sel
+000097c0: 662e 6d6f 6465 6c73 5b30 5d2e 636f 6e76  f.models[0].conv
+000097d0: 520a 2020 2020 2020 2020 7265 7475 726e  R.        return
+000097e0: 2073 656c 662e 5f63 6f6e 7652 0a0a 2020   self._convR..  
+000097f0: 2020 4063 6f6e 7652 2e73 6574 7465 720a    @convR.setter.
+00009800: 2020 2020 6465 6620 636f 6e76 5228 7365      def convR(se
+00009810: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
+00009820: 2020 2073 656c 662e 5f63 6f6e 7652 3d76     self._convR=v
+00009830: 616c 7565 0a0a 2020 2020 4070 726f 7065  alue..    @prope
+00009840: 7274 790a 2020 2020 6465 6620 636f 6e76  rty.    def conv
+00009850: 4f76 6572 6c61 7046 7265 7128 7365 6c66  OverlapFreq(self
+00009860: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00009870: 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a 2020  lf.nmodels>1:.  
+00009880: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00009890: 636f 6e76 4f76 6572 6c61 7046 7265 713d  convOverlapFreq=
+000098a0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+000098b0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+000098c0: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+000098d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000098e0: 662e 5f63 6f6e 764f 7665 726c 6170 4672  f._convOverlapFr
+000098f0: 6571 2e61 7070 656e 6428 7365 6c66 2e6d  eq.append(self.m
+00009900: 6f64 656c 735b 695d 2e63 6f6e 764f 7665  odels[i].convOve
+00009910: 726c 6170 4672 6571 290a 2020 2020 2020  rlapFreq).      
+00009920: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00009930: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
+00009940: 6572 6c61 7046 7265 713d 7365 6c66 2e6d  erlapFreq=self.m
+00009950: 6f64 656c 735b 305d 2e63 6f6e 764f 7665  odels[0].convOve
+00009960: 726c 6170 4672 6571 0a20 2020 2020 2020  rlapFreq.       
+00009970: 2072 6574 7572 6e20 7365 6c66 2e5f 636f   return self._co
+00009980: 6e76 4f76 6572 6c61 7046 7265 710a 0a20  nvOverlapFreq.. 
+00009990: 2020 2040 636f 6e76 4f76 6572 6c61 7046     @convOverlapF
+000099a0: 7265 712e 7365 7474 6572 0a20 2020 2064  req.setter.    d
+000099b0: 6566 2063 6f6e 764f 7665 726c 6170 4672  ef convOverlapFr
+000099c0: 6571 2873 656c 662c 7661 6c75 6529 3a0a  eq(self,value):.
+000099d0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+000099e0: 6e76 4f76 6572 6c61 7046 7265 713d 7661  nvOverlapFreq=va
+000099f0: 6c75 650a 0a20 2020 2040 7072 6f70 6572  lue..    @proper
+00009a00: 7479 0a20 2020 2064 6566 2063 6f6e 764f  ty.    def convO
+00009a10: 7665 726c 6170 5761 7665 2873 656c 6629  verlapWave(self)
+00009a20: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00009a30: 662e 6e6d 6f64 656c 733e 313a 0a20 2020  f.nmodels>1:.   
+00009a40: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00009a50: 6f6e 764f 7665 726c 6170 5761 7665 3d5b  onvOverlapWave=[
+00009a60: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00009a70: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+00009a80: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+00009a90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009aa0: 2e5f 636f 6e76 4f76 6572 6c61 7057 6176  ._convOverlapWav
+00009ab0: 652e 6170 7065 6e64 2873 656c 662e 6d6f  e.append(self.mo
+00009ac0: 6465 6c73 5b69 5d2e 636f 6e76 4f76 6572  dels[i].convOver
+00009ad0: 6c61 7057 6176 6529 0a20 2020 2020 2020  lapWave).       
+00009ae0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00009af0: 2020 2073 656c 662e 5f63 6f6e 764f 7665     self._convOve
+00009b00: 726c 6170 5761 7665 3d73 656c 662e 6d6f  rlapWave=self.mo
+00009b10: 6465 6c73 5b30 5d2e 636f 6e76 4f76 6572  dels[0].convOver
+00009b20: 6c61 7057 6176 650a 2020 2020 2020 2020  lapWave.        
+00009b30: 7265 7475 726e 2073 656c 662e 5f63 6f6e  return self._con
+00009b40: 764f 7665 726c 6170 5761 7665 0a0a 2020  vOverlapWave..  
+00009b50: 2020 4063 6f6e 764f 7665 726c 6170 5761    @convOverlapWa
+00009b60: 7665 2e73 6574 7465 720a 2020 2020 6465  ve.setter.    de
+00009b70: 6620 636f 6e76 4f76 6572 6c61 7057 6176  f convOverlapWav
+00009b80: 6528 7365 6c66 2c76 616c 7565 293a 0a20  e(self,value):. 
+00009b90: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
+00009ba0: 764f 7665 726c 6170 5761 7665 3d76 616c  vOverlapWave=val
+00009bb0: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
+00009bc0: 790a 2020 2020 6465 6620 6f76 6572 6c61  y.    def overla
+00009bd0: 7046 7265 7128 7365 6c66 293a 0a20 2020  pFreq(self):.   
+00009be0: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
+00009bf0: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
+00009c00: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
+00009c10: 7046 7265 713d 5b5d 0a20 2020 2020 2020  pFreq=[].       
+00009c20: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00009c30: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
+00009c40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00009c50: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
+00009c60: 4672 6571 2e61 7070 656e 6428 7365 6c66  Freq.append(self
+00009c70: 2e6d 6f64 656c 735b 695d 2e6f 7665 726c  .models[i].overl
+00009c80: 6170 4672 6571 290a 2020 2020 2020 2020  apFreq).        
+00009c90: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00009ca0: 2020 7365 6c66 2e5f 6f76 6572 6c61 7046    self._overlapF
+00009cb0: 7265 713d 7365 6c66 2e6d 6f64 656c 735b  req=self.models[
+00009cc0: 305d 2e6f 7665 726c 6170 4672 6571 0a20  0].overlapFreq. 
+00009cd0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00009ce0: 6c66 2e5f 6f76 6572 6c61 7046 7265 710a  lf._overlapFreq.
+00009cf0: 0a20 2020 2040 6f76 6572 6c61 7046 7265  .    @overlapFre
+00009d00: 712e 7365 7474 6572 0a20 2020 2064 6566  q.setter.    def
+00009d10: 206f 7665 726c 6170 4672 6571 2873 656c   overlapFreq(sel
+00009d20: 662c 7661 6c75 6529 3a0a 2020 2020 2020  f,value):.      
+00009d30: 2020 7365 6c66 2e5f 6f76 6572 6c61 7046    self._overlapF
+00009d40: 7265 713d 7661 6c75 650a 0a20 2020 2040  req=value..    @
+00009d50: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00009d60: 2063 6f6e 764f 7665 726c 6170 4c54 4528   convOverlapLTE(
+00009d70: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00009d80: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
+00009d90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00009da0: 6c66 2e5f 636f 6e76 4f76 6572 6c61 704c  lf._convOverlapL
+00009db0: 5445 3d5b 5d0a 2020 2020 2020 2020 2020  TE=[].          
+00009dc0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00009dd0: 2873 656c 662e 6e6d 6f64 656c 7329 3a0a  (self.nmodels):.
+00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009df0: 7365 6c66 2e5f 636f 6e76 4f76 6572 6c61  self._convOverla
+00009e00: 704c 5445 2e61 7070 656e 6428 7365 6c66  pLTE.append(self
+00009e10: 2e6d 6f64 656c 735b 695d 2e63 6f6e 764f  .models[i].convO
+00009e20: 7665 726c 6170 4c54 4529 0a20 2020 2020  verlapLTE).     
+00009e30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00009e40: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
+00009e50: 7665 726c 6170 4c54 453d 7365 6c66 2e6d  verlapLTE=self.m
+00009e60: 6f64 656c 735b 305d 2e63 6f6e 764f 7665  odels[0].convOve
+00009e70: 726c 6170 4c54 450a 2020 2020 2020 2020  rlapLTE.        
+00009e80: 7265 7475 726e 2073 656c 662e 5f63 6f6e  return self._con
+00009e90: 764f 7665 726c 6170 4c54 450a 0a20 2020  vOverlapLTE..   
+00009ea0: 2040 636f 6e76 4f76 6572 6c61 704c 5445   @convOverlapLTE
+00009eb0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+00009ec0: 636f 6e76 4f76 6572 6c61 704c 5445 2873  convOverlapLTE(s
+00009ed0: 656c 662c 7661 6c75 6529 3a0a 2020 2020  elf,value):.    
+00009ee0: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
+00009ef0: 6572 6c61 704c 5445 3d76 616c 7565 0a0a  erlapLTE=value..
+00009f00: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00009f10: 2020 6465 6620 636f 6e76 4f76 6572 6c61    def convOverla
+00009f20: 704e 4c54 4528 7365 6c66 293a 0a20 2020  pNLTE(self):.   
+00009f30: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
+00009f40: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
+00009f50: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
+00009f60: 6572 6c61 704e 4c54 453d 5b5d 0a20 2020  erlapNLTE=[].   
+00009f70: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00009f80: 6e20 7261 6e67 6528 7365 6c66 2e6e 6d6f  n range(self.nmo
+00009f90: 6465 6c73 293a 0a20 2020 2020 2020 2020  dels):.         
+00009fa0: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
+00009fb0: 764f 7665 726c 6170 4e4c 5445 2e61 7070  vOverlapNLTE.app
+00009fc0: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+00009fd0: 695d 2e63 6f6e 764f 7665 726c 6170 4e4c  i].convOverlapNL
+00009fe0: 5445 290a 2020 2020 2020 2020 656c 7365  TE).        else
+00009ff0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000a000: 6c66 2e5f 636f 6e76 4f76 6572 6c61 704e  lf._convOverlapN
+0000a010: 4c54 453d 7365 6c66 2e6d 6f64 656c 735b  LTE=self.models[
+0000a020: 305d 2e63 6f6e 764f 7665 726c 6170 4e4c  0].convOverlapNL
+0000a030: 5445 0a20 2020 2020 2020 2072 6574 7572  TE.        retur
+0000a040: 6e20 7365 6c66 2e5f 636f 6e76 4f76 6572  n self._convOver
+0000a050: 6c61 704e 4c54 450a 0a20 2020 2040 636f  lapNLTE..    @co
+0000a060: 6e76 4f76 6572 6c61 704e 4c54 452e 7365  nvOverlapNLTE.se
+0000a070: 7474 6572 0a20 2020 2064 6566 2063 6f6e  tter.    def con
+0000a080: 764f 7665 726c 6170 4e4c 5445 2873 656c  vOverlapNLTE(sel
+0000a090: 662c 7661 6c75 6529 3a0a 2020 2020 2020  f,value):.      
+0000a0a0: 2020 7365 6c66 2e5f 636f 6e76 4f76 6572    self._convOver
+0000a0b0: 6c61 704e 4c54 453d 7661 6c75 650a 0a20  lapNLTE=value.. 
+0000a0c0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000a0d0: 2064 6566 206f 7665 726c 6170 4c54 4528   def overlapLTE(
+0000a0e0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+0000a0f0: 6620 7365 6c66 2e6e 6d6f 6465 6c73 3e31  f self.nmodels>1
+0000a100: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000a110: 6c66 2e5f 6f76 6572 6c61 704c 5445 3d5b  lf._overlapLTE=[
+0000a120: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+0000a130: 7220 6920 696e 2072 616e 6765 2873 656c  r i in range(sel
+0000a140: 662e 6e6d 6f64 656c 7329 3a0a 2020 2020  f.nmodels):.    
+0000a150: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a160: 2e5f 6f76 6572 6c61 704c 5445 2e61 7070  ._overlapLTE.app
+0000a170: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+0000a180: 695d 2e6f 7665 726c 6170 4c54 4529 0a20  i].overlapLTE). 
+0000a190: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000a1a0: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
+0000a1b0: 7665 726c 6170 4c54 453d 7365 6c66 2e6d  verlapLTE=self.m
+0000a1c0: 6f64 656c 735b 305d 2e6f 7665 726c 6170  odels[0].overlap
+0000a1d0: 4c54 450a 2020 2020 2020 2020 7265 7475  LTE.        retu
+0000a1e0: 726e 2073 656c 662e 5f6f 7665 726c 6170  rn self._overlap
+0000a1f0: 4c54 450a 0a20 2020 2040 6f76 6572 6c61  LTE..    @overla
+0000a200: 704c 5445 2e73 6574 7465 720a 2020 2020  pLTE.setter.    
+0000a210: 6465 6620 6f76 6572 6c61 704c 5445 2873  def overlapLTE(s
+0000a220: 656c 662c 7661 6c75 6529 3a0a 2020 2020  elf,value):.    
+0000a230: 2020 2020 7365 6c66 2e5f 6f76 6572 6c61      self._overla
+0000a240: 704c 5445 3d76 616c 7565 0a0a 2020 2020  pLTE=value..    
+0000a250: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000a260: 6620 6f76 6572 6c61 704e 4c54 4528 7365  f overlapNLTE(se
+0000a270: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+0000a280: 7365 6c66 2e6e 6d6f 6465 6c73 3e31 3a0a  self.nmodels>1:.
+0000a290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a2a0: 2e5f 6f76 6572 6c61 704e 4c54 453d 5b5d  ._overlapNLTE=[]
+0000a2b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000a2c0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+0000a2d0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+0000a2e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a2f0: 5f6f 7665 726c 6170 4e4c 5445 2e61 7070  _overlapNLTE.app
+0000a300: 656e 6428 7365 6c66 2e6d 6f64 656c 735b  end(self.models[
+0000a310: 695d 2e6f 7665 726c 6170 4e4c 5445 290a  i].overlapNLTE).
+0000a320: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000a330: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000a340: 6f76 6572 6c61 704e 4c54 453d 7365 6c66  overlapNLTE=self
+0000a350: 2e6d 6f64 656c 735b 305d 2e6f 7665 726c  .models[0].overl
+0000a360: 6170 4e4c 5445 0a20 2020 2020 2020 2072  apNLTE.        r
+0000a370: 6574 7572 6e20 7365 6c66 2e5f 6f76 6572  eturn self._over
+0000a380: 6c61 704e 4c54 450a 0a20 2020 2040 6f76  lapNLTE..    @ov
+0000a390: 6572 6c61 704e 4c54 452e 7365 7474 6572  erlapNLTE.setter
+0000a3a0: 0a20 2020 2064 6566 206f 7665 726c 6170  .    def overlap
+0000a3b0: 4e4c 5445 2873 656c 662c 7661 6c75 6529  NLTE(self,value)
+0000a3c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+0000a3d0: 6f76 6572 6c61 704e 4c54 453d 7661 6c75  overlapNLTE=valu
+0000a3e0: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+0000a3f0: 0a20 2020 2064 6566 206f 7665 726c 6170  .    def overlap
+0000a400: 5461 754c 5445 2873 656c 6629 3a0a 2020  TauLTE(self):.  
+0000a410: 2020 2020 2020 6966 2073 656c 662e 6e6d        if self.nm
+0000a420: 6f64 656c 733e 313a 0a20 2020 2020 2020  odels>1:.       
+0000a430: 2020 2020 2073 656c 662e 5f6f 7665 726c       self._overl
+0000a440: 6170 5461 754c 5445 3d5b 5d0a 2020 2020  apTauLTE=[].    
+0000a450: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0000a460: 2072 616e 6765 2873 656c 662e 6e6d 6f64   range(self.nmod
+0000a470: 656c 7329 3a0a 2020 2020 2020 2020 2020  els):.          
+0000a480: 2020 2020 2020 7365 6c66 2e5f 6f76 6572        self._over
+0000a490: 6c61 7054 6175 4c54 452e 6170 7065 6e64  lapTauLTE.append
+0000a4a0: 2873 656c 662e 6d6f 6465 6c73 5b69 5d2e  (self.models[i].
+0000a4b0: 6f76 6572 6c61 7054 6175 4c54 4529 0a20  overlapTauLTE). 
+0000a4c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000a4d0: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
+0000a4e0: 7665 726c 6170 5461 754c 5445 3d73 656c  verlapTauLTE=sel
+0000a4f0: 662e 6d6f 6465 6c73 5b30 5d2e 6f76 6572  f.models[0].over
+0000a500: 6c61 7054 6175 4c54 450a 2020 2020 2020  lapTauLTE.      
+0000a510: 2020 7265 7475 726e 2073 656c 662e 5f6f    return self._o
+0000a520: 7665 726c 6170 5461 754c 5445 0a0a 2020  verlapTauLTE..  
+0000a530: 2020 406f 7665 726c 6170 5461 754c 5445    @overlapTauLTE
+0000a540: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+0000a550: 6f76 6572 6c61 7054 6175 4c54 4528 7365  overlapTauLTE(se
+0000a560: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
+0000a570: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
+0000a580: 5461 754c 5445 3d76 616c 7565 0a0a 2020  TauLTE=value..  
+0000a590: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000a5a0: 6465 6620 6f76 6572 6c61 7054 6175 4e4c  def overlapTauNL
+0000a5b0: 5445 2873 656c 6629 3a0a 2020 2020 2020  TE(self):.      
+0000a5c0: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
+0000a5d0: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
+0000a5e0: 2073 656c 662e 5f6f 7665 726c 6170 5461   self._overlapTa
+0000a5f0: 754e 4c54 453d 5b5d 0a20 2020 2020 2020  uNLTE=[].       
+0000a600: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+0000a610: 6e67 6528 7365 6c66 2e6e 6d6f 6465 6c73  nge(self.nmodels
+0000a620: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000a630: 2020 2073 656c 662e 5f6f 7665 726c 6170     self._overlap
+0000a640: 5461 754e 4c54 452e 6170 7065 6e64 2873  TauNLTE.append(s
+0000a650: 656c 662e 6d6f 6465 6c73 5b69 5d2e 6f76  elf.models[i].ov
+0000a660: 6572 6c61 7054 6175 4e4c 5445 290a 2020  erlapTauNLTE).  
+0000a670: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000a680: 2020 2020 2020 2020 7365 6c66 2e5f 6f76          self._ov
+0000a690: 6572 6c61 7054 6175 4e4c 5445 3d73 656c  erlapTauNLTE=sel
+0000a6a0: 662e 6d6f 6465 6c73 5b30 5d2e 6f76 6572  f.models[0].over
+0000a6b0: 6c61 7054 6175 4e4c 5445 0a20 2020 2020  lapTauNLTE.     
+0000a6c0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000a6d0: 6f76 6572 6c61 7054 6175 4e4c 5445 0a0a  overlapTauNLTE..
+0000a6e0: 2020 2020 406f 7665 726c 6170 5461 754e      @overlapTauN
+0000a6f0: 4c54 452e 7365 7474 6572 0a20 2020 2064  LTE.setter.    d
+0000a700: 6566 206f 7665 726c 6170 5461 754e 4c54  ef overlapTauNLT
+0000a710: 4528 7365 6c66 2c76 616c 7565 293a 0a20  E(self,value):. 
+0000a720: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
+0000a730: 726c 6170 5461 754e 4c54 453d 7661 6c75  rlapTauNLTE=valu
+0000a740: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+0000a750: 0a20 2020 2064 6566 2063 6f6e 764f 7665  .    def convOve
+0000a760: 726c 6170 5228 7365 6c66 293a 0a20 2020  rlapR(self):.   
+0000a770: 2020 2020 2069 6620 7365 6c66 2e6e 6d6f       if self.nmo
+0000a780: 6465 6c73 3e31 3a0a 2020 2020 2020 2020  dels>1:.        
+0000a790: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
+0000a7a0: 6572 6c61 7052 3d5b 5d0a 2020 2020 2020  erlapR=[].      
+0000a7b0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0000a7c0: 616e 6765 2873 656c 662e 6e6d 6f64 656c  ange(self.nmodel
+0000a7d0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0000a7e0: 2020 2020 7365 6c66 2e5f 636f 6e76 4f76      self._convOv
+0000a7f0: 6572 6c61 7052 2e61 7070 656e 6428 7365  erlapR.append(se
+0000a800: 6c66 2e6d 6f64 656c 735b 695d 2e63 6f6e  lf.models[i].con
+0000a810: 764f 7665 726c 6170 5229 0a20 2020 2020  vOverlapR).     
+0000a820: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a830: 2020 2020 2073 656c 662e 5f63 6f6e 764f       self._convO
+0000a840: 7665 726c 6170 523d 7365 6c66 2e6d 6f64  verlapR=self.mod
+0000a850: 656c 735b 305d 2e63 6f6e 764f 7665 726c  els[0].convOverl
+0000a860: 6170 520a 2020 2020 2020 2020 7265 7475  apR.        retu
+0000a870: 726e 2073 656c 662e 5f63 6f6e 764f 7665  rn self._convOve
+0000a880: 726c 6170 520a 0a20 2020 2040 636f 6e76  rlapR..    @conv
+0000a890: 4f76 6572 6c61 7052 2e73 6574 7465 720a  OverlapR.setter.
+0000a8a0: 2020 2020 6465 6620 636f 6e76 4f76 6572      def convOver
+0000a8b0: 6c61 7052 2873 656c 662c 7661 6c75 6529  lapR(self,value)
+0000a8c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+0000a8d0: 636f 6e76 4f76 6572 6c61 7052 3d76 616c  convOverlapR=val
+0000a8e0: 7565 0a0a 2020 2020 4070 726f 7065 7274  ue..    @propert
+0000a8f0: 790a 2020 2020 6465 6620 6f76 6572 6c61  y.    def overla
+0000a900: 7052 2873 656c 6629 3a0a 2020 2020 2020  pR(self):.      
+0000a910: 2020 6966 2073 656c 662e 6e6d 6f64 656c    if self.nmodel
+0000a920: 733e 313a 0a20 2020 2020 2020 2020 2020  s>1:.           
+0000a930: 2073 656c 662e 5f6f 7665 726c 6170 523d   self._overlapR=
+0000a940: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+0000a950: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+0000a960: 6c66 2e6e 6d6f 6465 6c73 293a 0a20 2020  lf.nmodels):.   
+0000a970: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a980: 662e 5f6f 7665 726c 6170 522e 6170 7065  f._overlapR.appe
+0000a990: 6e64 2873 656c 662e 6d6f 6465 6c73 5b69  nd(self.models[i
+0000a9a0: 5d2e 6f76 6572 6c61 7052 290a 2020 2020  ].overlapR).    
+0000a9b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000a9c0: 2020 2020 2020 7365 6c66 2e5f 6f76 6572        self._over
+0000a9d0: 6c61 7052 3d73 656c 662e 6d6f 6465 6c73  lapR=self.models
+0000a9e0: 5b30 5d2e 6f76 6572 6c61 7052 0a20 2020  [0].overlapR.   
+0000a9f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000aa00: 2e5f 6f76 6572 6c61 7052 0a0a 2020 2020  ._overlapR..    
+0000aa10: 406f 7665 726c 6170 522e 7365 7474 6572  @overlapR.setter
+0000aa20: 0a20 2020 2064 6566 206f 7665 726c 6170  .    def overlap
+0000aa30: 5228 7365 6c66 2c76 616c 7565 293a 0a20  R(self,value):. 
+0000aa40: 2020 2020 2020 2073 656c 662e 5f6f 7665         self._ove
+0000aa50: 726c 6170 523d 7661 6c75 650a 0a0a 636c  rlapR=value...cl
+0000aa60: 6173 7320 736c 6162 3a0a 2020 2020 2222  ass slab:.    ""
+0000aa70: 220a 2020 2020 636c 6173 733a 3a20 736c  ".    class:: sl
+0000aa80: 6162 0a20 2020 2043 6c61 7373 2074 6f20  ab.    Class to 
+0000aa90: 686f 6c64 2074 6865 2064 6174 6120 6f66  hold the data of
+0000aaa0: 2069 6e64 6976 6964 7561 6c20 736c 6162   individual slab
+0000aab0: 206d 6f64 656c 730a 2020 2020 2222 220a   models.    """.
+0000aac0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000aad0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+0000aae0: 2073 656c 662e 7370 6563 6965 735f 6e75   self.species_nu
+0000aaf0: 6d62 6572 3d4e 6f6e 650a 2020 2020 2020  mber=None.      
+0000ab00: 2020 7365 6c66 2e6d 6f64 656c 5f6e 756d    self.model_num
+0000ab10: 6265 723d 4e6f 6e65 0a20 2020 2020 2020  ber=None.       
+0000ab20: 2073 656c 662e 4e48 3d4e 6f6e 650a 2020   self.NH=None.  
+0000ab30: 2020 2020 2020 7365 6c66 2e6e 436f 6c6c        self.nColl
+0000ab40: 3d4e 6f6e 650a 2020 2020 2020 2020 7365  =None.        se
+0000ab50: 6c66 2e6e 653d 4e6f 6e65 0a20 2020 2020  lf.ne=None.     
+0000ab60: 2020 2073 656c 662e 6e48 653d 4e6f 6e65     self.nHe=None
+0000ab70: 0a20 2020 2020 2020 2073 656c 662e 6e48  .        self.nH
+0000ab80: 4949 3d4e 6f6e 650a 2020 2020 2020 2020  II=None.        
+0000ab90: 7365 6c66 2e6e 4849 3d4e 6f6e 650a 2020  self.nHI=None.  
+0000aba0: 2020 2020 2020 7365 6c66 2e6e 4832 3d4e        self.nH2=N
+0000abb0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000abc0: 2e64 7573 745f 746f 5f67 6173 3d4e 6f6e  .dust_to_gas=Non
+0000abd0: 650a 2020 2020 2020 2020 7365 6c66 2e76  e.        self.v
+0000abe0: 7475 7262 3d4e 6f6e 650a 2020 2020 2020  turb=None.      
+0000abf0: 2020 7365 6c66 2e54 673d 4e6f 6e65 0a20    self.Tg=None. 
+0000ac00: 2020 2020 2020 2073 656c 662e 5464 3d4e         self.Td=N
+0000ac10: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000ac20: 2e73 7065 6369 6573 5f6e 616d 653d 4e6f  .species_name=No
+0000ac30: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+0000ac40: 7370 6563 6965 735f 696e 6465 783d 4e6f  species_index=No
+0000ac50: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+0000ac60: 6162 756e 6461 6e63 653d 4e6f 6e65 0a20  abundance=None. 
+0000ac70: 2020 2020 2020 2073 656c 662e 6476 3d4e         self.dv=N
+0000ac80: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000ac90: 2e6e 6c65 7665 6c73 3d4e 6f6e 650a 2020  .nlevels=None.  
+0000aca0: 2020 2020 2020 7365 6c66 2e6e 6c69 6e65        self.nline
+0000acb0: 733d 4e6f 6e65 0a20 2020 2020 2020 2073  s=None.        s
+0000acc0: 656c 662e 6c69 6e65 6461 7461 3d4e 6f6e  elf.linedata=Non
+0000acd0: 650a 2020 2020 2020 2020 7365 6c66 2e6c  e.        self.l
+0000ace0: 6576 656c 6461 7461 3d4e 6f6e 650a 2020  eveldata=None.  
+0000acf0: 2020 2020 2020 7365 6c66 2e63 6f6e 7657        self.convW
+0000ad00: 6176 656c 656e 6774 683d 4e6f 6e65 0a20  avelength=None. 
+0000ad10: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
+0000ad20: 4c54 4566 6c75 783d 4e6f 6e65 0a20 2020  LTEflux=None.   
+0000ad30: 2020 2020 2073 656c 662e 636f 6e76 4e4c       self.convNL
+0000ad40: 5445 666c 7578 3d4e 6f6e 650a 2020 2020  TEflux=None.    
+0000ad50: 2020 2020 7365 6c66 2e63 6f6e 7654 7970      self.convTyp
+0000ad60: 653d 4e6f 6e65 0a20 2020 2020 2020 2073  e=None.        s
+0000ad70: 656c 662e 636f 6e76 523d 4e6f 6e65 0a20  elf.convR=None. 
+0000ad80: 2020 2020 2020 2073 656c 662e 6f76 6572         self.over
+0000ad90: 6c61 704c 5445 3d4e 6f6e 650a 2020 2020  lapLTE=None.    
+0000ada0: 2020 2020 7365 6c66 2e6f 7665 726c 6170      self.overlap
+0000adb0: 4e4c 5445 3d4e 6f6e 650a 2020 2020 2020  NLTE=None.      
+0000adc0: 2020 7365 6c66 2e6f 7665 726c 6170 5461    self.overlapTa
+0000add0: 754c 5445 3d4e 6f6e 650a 2020 2020 2020  uLTE=None.      
+0000ade0: 2020 7365 6c66 2e6f 7665 726c 6170 5461    self.overlapTa
+0000adf0: 754e 4c54 453d 4e6f 6e65 0a20 2020 2020  uNLTE=None.     
+0000ae00: 2020 2073 656c 662e 6f76 6572 6c61 7046     self.overlapF
+0000ae10: 7265 713d 4e6f 6e65 0a20 2020 2020 2020  req=None.       
+0000ae20: 2073 656c 662e 636f 6e76 4f76 6572 6c61   self.convOverla
+0000ae30: 704c 5445 3d4e 6f6e 650a 2020 2020 2020  pLTE=None.      
+0000ae40: 2020 7365 6c66 2e63 6f6e 764f 7665 726c    self.convOverl
+0000ae50: 6170 4e4c 5445 3d4e 6f6e 650a 2020 2020  apNLTE=None.    
+0000ae60: 2020 2020 7365 6c66 2e63 6f6e 764f 7665      self.convOve
+0000ae70: 726c 6170 4672 6571 3d4e 6f6e 650a 2020  rlapFreq=None.  
+0000ae80: 2020 2020 2020 7365 6c66 2e63 6f6e 764f        self.convO
+0000ae90: 7665 726c 6170 5761 7665 3d4e 6f6e 650a  verlapWave=None.
+0000aea0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0000aeb0: 764f 7665 726c 6170 523d 3165 350a 2020  vOverlapR=1e5.  
+0000aec0: 2020 2020 2020 7365 6c66 2e6f 7665 726c        self.overl
+0000aed0: 6170 523d 3165 350a 0a20 2020 2064 6566  apR=1e5..    def
+0000aee0: 205f 5f73 7472 5f5f 2873 656c 6629 3a0a   __str__(self):.
+0000aef0: 2020 2020 2020 2020 6f75 7470 7574 3d22          output="
+0000af00: 496e 666f 204d 6f64 656c 3a20 5c6e 220a  Info Model: \n".
+0000af10: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000af20: 2773 7065 6369 6573 5f6e 756d 6265 723d  'species_number=
+0000af30: 2027 0a20 2020 2020 2020 206f 7574 7075   '.        outpu
+0000af40: 742b 3d73 7472 2873 656c 662e 7370 6563  t+=str(self.spec
+0000af50: 6965 735f 6e75 6d62 6572 292b 275c 6e5c  ies_number)+'\n\
+0000af60: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
+0000af70: 742b 3d27 6d6f 6465 6c5f 6e75 6d62 6572  t+='model_number
+0000af80: 2020 3d20 270a 2020 2020 2020 2020 6f75    = '.        ou
+0000af90: 7470 7574 2b3d 7374 7228 7365 6c66 2e6d  tput+=str(self.m
+0000afa0: 6f64 656c 5f6e 756d 6265 7229 2b27 5c6e  odel_number)+'\n
+0000afb0: 5c6e 270a 2020 2020 2020 2020 6f75 7470  \n'.        outp
+0000afc0: 7574 2b3d 274e 4820 2020 2020 2020 2020  ut+='NH         
+0000afd0: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
+0000afe0: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
+0000aff0: 4e48 292b 275c 6e5c 6e27 0a20 2020 2020  NH)+'\n\n'.     
+0000b000: 2020 206f 7574 7075 742b 3d27 6e43 6f6c     output+='nCol
+0000b010: 6c20 2020 2020 2020 2020 3d20 270a 2020  l         = '.  
+0000b020: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
+0000b030: 7228 7365 6c66 2e6e 436f 6c6c 292b 275c  r(self.nColl)+'\
+0000b040: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
+0000b050: 7075 742b 3d27 6e65 2020 2020 2020 2020  put+='ne        
+0000b060: 2020 2020 3d20 270a 2020 2020 2020 2020      = '.        
+0000b070: 6f75 7470 7574 2b3d 7374 7228 7365 6c66  output+=str(self
+0000b080: 2e6e 6529 2b27 5c6e 5c6e 270a 2020 2020  .ne)+'\n\n'.    
+0000b090: 2020 2020 6f75 7470 7574 2b3d 276e 4865      output+='nHe
+0000b0a0: 2020 2020 2020 2020 2020 203d 2027 0a20             = '. 
+0000b0b0: 2020 2020 2020 206f 7574 7075 742b 3d73         output+=s
+0000b0c0: 7472 2873 656c 662e 6e48 6529 2b27 5c6e  tr(self.nHe)+'\n
+0000b0d0: 5c6e 270a 2020 2020 2020 2020 6f75 7470  \n'.        outp
+0000b0e0: 7574 2b3d 276e 4849 4920 2020 2020 2020  ut+='nHII       
+0000b0f0: 2020 203d 2027 0a20 2020 2020 2020 206f     = '.        o
+0000b100: 7574 7075 742b 3d73 7472 2873 656c 662e  utput+=str(self.
+0000b110: 6e48 4949 292b 275c 6e5c 6e27 0a20 2020  nHII)+'\n\n'.   
+0000b120: 2020 2020 206f 7574 7075 742b 3d27 6e48       output+='nH
+0000b130: 4920 2020 2020 2020 2020 2020 3d20 270a  I           = '.
+0000b140: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000b150: 7374 7228 7365 6c66 2e6e 4849 292b 275c  str(self.nHI)+'\
+0000b160: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
+0000b170: 7075 742b 3d27 6e48 3220 2020 2020 2020  put+='nH2       
+0000b180: 2020 2020 3d20 270a 2020 2020 2020 2020      = '.        
+0000b190: 6f75 7470 7574 2b3d 7374 7228 7365 6c66  output+=str(self
+0000b1a0: 2e6e 4832 292b 275c 6e5c 6e27 0a20 2020  .nH2)+'\n\n'.   
+0000b1b0: 2020 2020 206f 7574 7075 742b 3d27 6475       output+='du
+0000b1c0: 7374 5f74 6f5f 6761 7320 2020 3d20 270a  st_to_gas   = '.
+0000b1d0: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000b1e0: 7374 7228 7365 6c66 2e64 7573 745f 746f  str(self.dust_to
+0000b1f0: 5f67 6173 292b 275c 6e5c 6e27 0a20 2020  _gas)+'\n\n'.   
+0000b200: 2020 2020 206f 7574 7075 742b 3d27 7674       output+='vt
+0000b210: 7572 6220 2020 2020 2020 2020 3d20 270a  urb         = '.
+0000b220: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000b230: 7374 7228 7365 6c66 2e76 7475 7262 292b  str(self.vturb)+
+0000b240: 275c 6e5c 6e27 0a20 2020 2020 2020 206f  '\n\n'.        o
+0000b250: 7574 7075 742b 3d27 5467 2020 2020 2020  utput+='Tg      
+0000b260: 2020 2020 2020 3d20 270a 2020 2020 2020        = '.      
+0000b270: 2020 6f75 7470 7574 2b3d 7374 7228 7365    output+=str(se
+0000b280: 6c66 2e54 6729 2b27 5c6e 5c6e 270a 2020  lf.Tg)+'\n\n'.  
+0000b290: 2020 2020 2020 6f75 7470 7574 2b3d 2754        output+='T
+0000b2a0: 6420 2020 2020 2020 2020 2020 203d 2027  d            = '
+0000b2b0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
+0000b2c0: 3d73 7472 2873 656c 662e 5464 292b 275c  =str(self.Td)+'\
+0000b2d0: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
+0000b2e0: 7075 742b 3d27 7370 6563 6965 735f 6e61  put+='species_na
+0000b2f0: 6d65 2020 203d 2027 0a20 2020 2020 2020  me   = '.       
+0000b300: 206f 7574 7075 742b 3d73 656c 662e 7370   output+=self.sp
+0000b310: 6563 6965 735f 6e61 6d65 2b27 5c6e 5c6e  ecies_name+'\n\n
+0000b320: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
+0000b330: 2b3d 2761 6275 6e64 616e 6365 2020 2020  +='abundance    
+0000b340: 203d 2027 0a20 2020 2020 2020 206f 7574   = '.        out
+0000b350: 7075 742b 3d73 7472 2873 656c 662e 6162  put+=str(self.ab
+0000b360: 756e 6461 6e63 6529 2b27 5c6e 5c6e 270a  undance)+'\n\n'.
+0000b370: 2020 2020 2020 2020 6f75 7470 7574 2b3d          output+=
+0000b380: 2764 7620 2020 2020 2020 2020 2020 203d  'dv            =
+0000b390: 2027 0a20 2020 2020 2020 206f 7574 7075   '.        outpu
+0000b3a0: 742b 3d73 7472 2873 656c 662e 6476 292b  t+=str(self.dv)+
+0000b3b0: 275c 6e5c 6e27 0a20 2020 2020 2020 206f  '\n\n'.        o
+0000b3c0: 7574 7075 742b 3d27 6e6c 6576 656c 7320  utput+='nlevels 
+0000b3d0: 2020 2020 2020 3d20 270a 2020 2020 2020        = '.      
+0000b3e0: 2020 6f75 7470 7574 2b3d 7374 7228 7365    output+=str(se
+0000b3f0: 6c66 2e6e 6c65 7665 6c73 292b 275c 6e5c  lf.nlevels)+'\n\
+0000b400: 6e27 0a20 2020 2020 2020 206f 7574 7075  n'.        outpu
+0000b410: 742b 3d27 6e6c 696e 6573 2020 2020 2020  t+='nlines      
+0000b420: 2020 3d20 270a 2020 2020 2020 2020 6f75    = '.        ou
+0000b430: 7470 7574 2b3d 7374 7228 7365 6c66 2e6e  tput+=str(self.n
+0000b440: 6c69 6e65 7329 2b27 5c6e 5c6e 270a 2020  lines)+'\n\n'.  
+0000b450: 2020 2020 2020 6f75 7470 7574 2b3d 2763        output+='c
+0000b460: 6f6e 7654 7970 6520 2020 2020 2020 3d20  onvType       = 
+0000b470: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
+0000b480: 2b3d 7374 7228 7365 6c66 2e63 6f6e 7654  +=str(self.convT
+0000b490: 7970 6529 2b27 5c6e 5c6e 270a 2020 2020  ype)+'\n\n'.    
+0000b4a0: 2020 2020 6f75 7470 7574 2b3d 2763 6f6e      output+='con
+0000b4b0: 7652 2020 2020 2020 2020 3d20 270a 2020  vR        = '.  
+0000b4c0: 2020 2020 2020 6f75 7470 7574 2b3d 7374        output+=st
+0000b4d0: 7228 7365 6c66 2e63 6f6e 7652 292b 275c  r(self.convR)+'\
+0000b4e0: 6e5c 6e27 0a20 2020 2020 2020 2072 6574  n\n'.        ret
+0000b4f0: 7572 6e20 6f75 7470 7574 0a0a 2020 2020  urn output..    
+0000b500: 6465 6620 636f 6e76 6f6c 7665 2873 656c  def convolve(sel
+0000b510: 662c 6672 6571 5f62 696e 733d 4e6f 6e65  f,freq_bins=None
+0000b520: 2c52 3d31 2c6c 616d 6264 615f 303d 312c  ,R=1,lambda_0=1,
+0000b530: 6c61 6d62 6461 5f6e 3d31 2c76 723d 3133  lambda_n=1,vr=13
+0000b540: 3030 2c4e 4c54 453d 4661 6c73 652c 636f  00,NLTE=False,co
+0000b550: 6e76 5f74 7970 653d 3129 3a0a 2020 2020  nv_type=1):.    
+0000b560: 2020 2020 743d 2746 4c54 4527 0a20 2020      t='FLTE'.   
+0000b570: 2020 2020 2069 6620 4e4c 5445 3a0a 2020       if NLTE:.  
+0000b580: 2020 2020 2020 2020 2020 743d 2746 4e4c            t='FNL
+0000b590: 5445 270a 2020 2020 2020 2020 6461 3d73  TE'.        da=s
+0000b5a0: 656c 662e 6c69 6e65 6461 7461 0a20 2020  elf.linedata.   
+0000b5b0: 2020 2020 2069 6620 6c61 6d62 6461 5f30       if lambda_0
+0000b5c0: 3d3d 6c61 6d62 6461 5f6e 3a0a 2020 2020  ==lambda_n:.    
+0000b5d0: 2020 2020 2020 2020 6c61 6d62 6461 5f30          lambda_0
+0000b5e0: 3d6e 702e 616d 696e 2864 615b 2747 487a  =np.amin(da['GHz
+0000b5f0: 275d 3e63 2f6c 616d 6264 615f 6e2a 3165  ']>c/lambda_n*1e
+0000b600: 2d33 290a 2020 2020 2020 2020 2020 2020  -3).            
+0000b610: 6c61 6d62 6461 5f6e 3d6e 702e 616d 6178  lambda_n=np.amax
+0000b620: 2864 615b 2747 487a 275d 3e63 2f6c 616d  (da['GHz']>c/lam
+0000b630: 6264 615f 6e2a 3165 2d33 290a 2020 2020  bda_n*1e-3).    
+0000b640: 2020 2020 2020 2020 6c61 6d62 6461 5f30          lambda_0
+0000b650: 3d6c 616d 6264 615f 302a 3130 2a2a 2d30  =lambda_0*10**-0
+0000b660: 2e30 350a 2020 2020 2020 2020 2020 2020  .05.            
+0000b670: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
+0000b680: 6e2a 3130 2a2a 302e 3035 0a20 2020 2020  n*10**0.05.     
+0000b690: 2020 2064 615f 7265 713d 6461 5b28 6461     da_req=da[(da
+0000b6a0: 5b27 4748 7a27 5d3e 632f 6c61 6d62 6461  ['GHz']>c/lambda
+0000b6b0: 5f6e 2a31 652d 3329 2628 6461 5b27 4748  _n*1e-3)&(da['GH
+0000b6c0: 7a27 5d3c 632f 6c61 6d62 6461 5f30 2a31  z']<c/lambda_0*1
+0000b6d0: 652d 3329 5d0a 2020 2020 2020 2020 6461  e-3)].        da
+0000b6e0: 5f72 6571 2e72 6573 6574 5f69 6e64 6578  _req.reset_index
+0000b6f0: 2864 726f 703d 5472 7565 2c69 6e70 6c61  (drop=True,inpla
+0000b700: 6365 3d54 7275 6529 0a20 2020 2020 2020  ce=True).       
+0000b710: 2069 6620 636f 6e76 5f74 7970 653d 3d31   if conv_type==1
+0000b720: 3a0a 2020 2020 2020 2020 2020 2020 6c2c  :.            l,
+0000b730: 663d 6765 6e65 7261 6c43 6f6e 766f 6c76  f=generalConvolv
+0000b740: 6528 6461 5f72 6571 5b74 5d2c 6461 5f72  e(da_req[t],da_r
+0000b750: 6571 5b27 4748 7a27 5d2c 523d 522c 6c61  eq['GHz'],R=R,la
+0000b760: 6d62 6461 5f30 3d6c 616d 6264 615f 302c  mbda_0=lambda_0,
+0000b770: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
+0000b780: 6e29 0a20 2020 2020 2020 2065 6c73 653a  n).        else:
+0000b790: 0a20 2020 2020 2020 2020 2020 206c 2c66  .            l,f
+0000b7a0: 3d73 7065 6343 6f6e 766f 6c76 6528 6461  =specConvolve(da
+0000b7b0: 5f72 6571 5b74 5d2c 6461 5f72 6571 5b27  _req[t],da_req['
+0000b7c0: 4748 7a27 5d2c 6672 6571 5f62 696e 733d  GHz'],freq_bins=
+0000b7d0: 6672 6571 5f62 696e 732c 523d 522c 6c61  freq_bins,R=R,la
+0000b7e0: 6d62 6461 5f30 3d6c 616d 6264 615f 302c  mbda_0=lambda_0,
+0000b7f0: 6c61 6d62 6461 5f6e 3d6c 616d 6264 615f  lambda_n=lambda_
+0000b800: 6e2c 7672 3d76 7229 0a20 2020 2020 2020  n,vr=vr).       
+0000b810: 2073 656c 662e 636f 6e76 5761 7665 6c65   self.convWavele
+0000b820: 6e67 7468 3d6c 0a20 2020 2020 2020 2073  ngth=l.        s
+0000b830: 656c 662e 636f 6e76 5479 7065 3d63 6f6e  elf.convType=con
+0000b840: 765f 7479 7065 0a20 2020 2020 2020 2073  v_type.        s
+0000b850: 656c 662e 636f 6e76 523d 520a 2020 2020  elf.convR=R.    
+0000b860: 2020 2020 6966 204e 4c54 453a 0a20 2020      if NLTE:.   
+0000b870: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000b880: 6e76 4e4c 5445 666c 7578 3d66 0a20 2020  nvNLTEflux=f.   
+0000b890: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000b8a0: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
+0000b8b0: 4c54 4566 6c75 783d 660a 0a20 2020 2064  LTEflux=f..    d
+0000b8c0: 6566 2063 6f6e 766f 6c76 655f 6f76 6572  ef convolve_over
+0000b8d0: 6c61 7028 7365 6c66 2c52 3d31 2c6c 616d  lap(self,R=1,lam
+0000b8e0: 6264 615f 303d 312c 6c61 6d62 6461 5f6e  bda_0=1,lambda_n
+0000b8f0: 3d31 293a 0a20 2020 2020 2020 2069 6620  =1):.        if 
+0000b900: 6c61 6d62 6461 5f30 3d3d 6c61 6d62 6461  lambda_0==lambda
+0000b910: 5f6e 3a0a 2020 2020 2020 2020 2020 2020  _n:.            
+0000b920: 6c61 6d62 6461 5f30 3d6e 702e 616d 696e  lambda_0=np.amin
+0000b930: 2863 2f73 656c 662e 6f76 6572 6c61 7046  (c/self.overlapF
+0000b940: 7265 712a 3165 2d33 290a 2020 2020 2020  req*1e-3).      
+0000b950: 2020 2020 2020 6c61 6d62 6461 5f6e 3d6e        lambda_n=n
+0000b960: 702e 616d 6178 2863 2f73 656c 662e 6f76  p.amax(c/self.ov
+0000b970: 6572 6c61 7046 7265 712a 3165 2d33 290a  erlapFreq*1e-3).
+0000b980: 2020 2020 2020 2020 2020 2020 6c61 6d62              lamb
+0000b990: 6461 5f30 3d6c 616d 6264 615f 302a 3130  da_0=lambda_0*10
+0000b9a0: 2a2a 2d30 2e30 350a 2020 2020 2020 2020  **-0.05.        
+0000b9b0: 2020 2020 6c61 6d62 6461 5f6e 3d6c 616d      lambda_n=lam
+0000b9c0: 6264 615f 6e2a 3130 2a2a 302e 3035 0a20  bda_n*10**0.05. 
+0000b9d0: 2020 2020 2020 206d 6173 6b3d 2873 656c         mask=(sel
+0000b9e0: 662e 6f76 6572 6c61 7046 7265 713e 632f  f.overlapFreq>c/
+0000b9f0: 6c61 6d62 6461 5f6e 2a31 652d 3329 2628  lambda_n*1e-3)&(
+0000ba00: 7365 6c66 2e6f 7665 726c 6170 4672 6571  self.overlapFreq
+0000ba10: 3c63 2f6c 616d 6264 615f 302a 3165 2d33  <c/lambda_0*1e-3
+0000ba20: 290a 2020 2020 2020 2020 4657 484d 3d73  ).        FWHM=s
+0000ba30: 656c 662e 6f76 6572 6c61 7052 2f52 2f32  elf.overlapR/R/2
+0000ba40: 2e33 3535 0a20 2020 2020 2020 2067 3d47  .355.        g=G
+0000ba50: 6175 7373 6961 6e31 444b 6572 6e65 6c28  aussian1DKernel(
+0000ba60: 7374 6464 6576 3d46 5748 4d2c 6661 6374  stddev=FWHM,fact
+0000ba70: 6f72 3d37 290a 2020 2020 2020 2020 7365  or=7).        se
+0000ba80: 6c66 2e63 6f6e 764f 7665 726c 6170 4c54  lf.convOverlapLT
+0000ba90: 453d 6170 795f 636f 6e76 6f6c 7665 2873  E=apy_convolve(s
+0000baa0: 656c 662e 6f76 6572 6c61 704c 5445 5b6d  elf.overlapLTE[m
+0000bab0: 6173 6b5d 2c67 290a 2020 2020 2020 2020  ask],g).        
+0000bac0: 2320 7365 6c66 2e63 6f6e 764f 7665 726c  # self.convOverl
+0000bad0: 6170 4e4c 5445 3d61 7079 5f63 6f6e 766f  apNLTE=apy_convo
+0000bae0: 6c76 6528 7365 6c66 2e6f 7665 726c 6170  lve(self.overlap
+0000baf0: 4e4c 5445 5b6d 6173 6b5d 2c67 290a 2020  NLTE[mask],g).  
+0000bb00: 2020 2020 2020 7365 6c66 2e63 6f6e 764f        self.convO
+0000bb10: 7665 726c 6170 4672 6571 3d73 656c 662e  verlapFreq=self.
+0000bb20: 6f76 6572 6c61 7046 7265 715b 6d61 736b  overlapFreq[mask
+0000bb30: 5d2a 312e 300a 2020 2020 2020 2020 7365  ]*1.0.        se
+0000bb40: 6c66 2e63 6f6e 764f 7665 726c 6170 5761  lf.convOverlapWa
+0000bb50: 7665 3d63 2f73 656c 662e 636f 6e76 4f76  ve=c/self.convOv
+0000bb60: 6572 6c61 7046 7265 712a 3165 2d33 0a20  erlapFreq*1e-3. 
+0000bb70: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
+0000bb80: 4f76 6572 6c61 7052 3d52 0a0a 2020 2020  OverlapR=R..    
+0000bb90: 6465 6620 7368 6f77 2873 656c 6629 3a0a  def show(self):.
+0000bba0: 2020 2020 2020 2020 7072 696e 7428 7365          print(se
+0000bbb0: 6c66 290a 2020 2020 2020 2020 7072 696e  lf).        prin
+0000bbc0: 7428 276c 696e 6544 6174 6120 2020 203d  t('lineData    =
+0000bbd0: 2027 290a 2020 2020 2020 2020 7072 696e   ').        prin
+0000bbe0: 7428 7365 6c66 2e6c 696e 6564 6174 6129  t(self.linedata)
+0000bbf0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+0000bc00: 6c65 7665 6c44 6174 6120 2020 3d20 2729  levelData   = ')
+0000bc10: 0a20 2020 2020 2020 2070 7269 6e74 2873  .        print(s
+0000bc20: 656c 662e 6c65 7665 6c64 6174 6129 0a0a  elf.leveldata)..
+0000bc30: 0a63 6c61 7373 2073 6c61 6231 443a 0a20  .class slab1D:. 
+0000bc40: 2020 2022 2222 0a20 2020 2063 6c61 7373     """.    class
+0000bc50: 3a3a 2073 6c61 6231 440a 2020 2020 436c  :: slab1D.    Cl
+0000bc60: 6173 7320 746f 2068 6f6c 6420 7468 6520  ass to hold the 
+0000bc70: 6461 7461 206f 6620 3144 2073 6c61 6220  data of 1D slab 
+0000bc80: 6d6f 6465 6c73 0a20 2020 2022 2222 0a0a  models.    """..
+0000bc90: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000bca0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000bcb0: 7365 6c66 2e64 6972 6563 746f 7279 3d4e  self.directory=N
+0000bcc0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000bcd0: 2e66 6c75 783d 4e6f 6e65 0a20 2020 2020  .flux=None.     
+0000bce0: 2020 2073 656c 662e 6672 6571 7565 6e63     self.frequenc
+0000bcf0: 793d 4e6f 6e65 0a20 2020 2020 2020 2073  y=None.        s
+0000bd00: 656c 662e 4e73 7065 6369 6573 3d4e 6f6e  elf.Nspecies=Non
+0000bd10: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
+0000bd20: 7065 6369 6573 3d5b 5d0a 2020 2020 2020  pecies=[].      
+0000bd30: 2020 7365 6c66 2e4e 6772 6964 3d4e 6f6e    self.Ngrid=Non
+0000bd40: 650a 2020 2020 2020 2020 7365 6c66 2e52  e.        self.R
+0000bd50: 3d4e 6f6e 650a 2020 2020 2020 2020 7365  =None.        se
+0000bd60: 6c66 2e67 7269 643d 7064 2e44 6174 6146  lf.grid=pd.DataF
+0000bd70: 7261 6d65 2829 0a20 2020 2020 2020 2073  rame().        s
+0000bd80: 656c 662e 736f 7572 6365 5f66 756e 6374  elf.source_funct
+0000bd90: 696f 6e3d 4e6f 6e65 0a20 2020 2020 2020  ion=None.       
+0000bda0: 2073 656c 662e 736f 7572 6365 5f66 756e   self.source_fun
+0000bdb0: 6374 696f 6e5f 6761 733d 4e6f 6e65 0a20  ction_gas=None. 
+0000bdc0: 2020 2020 2020 2073 656c 662e 7461 755f         self.tau_
+0000bdd0: 6475 7374 3d4e 6f6e 650a 2020 2020 2020  dust=None.      
+0000bde0: 2020 7365 6c66 2e74 6175 5f67 6173 3d4e    self.tau_gas=N
+0000bdf0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000be00: 2e63 6f6e 7657 6176 656c 656e 6774 683d  .convWavelength=
+0000be10: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000be20: 662e 636f 6e76 4672 6571 7565 6e63 793d  f.convFrequency=
+0000be30: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000be40: 662e 636f 6e76 5f66 6c75 783d 4e6f 6e65  f.conv_flux=None
+0000be50: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0000be60: 6e76 523d 4e6f 6e65 0a0a 2020 2020 6465  nvR=None..    de
+0000be70: 6620 5f5f 7374 725f 5f28 7365 6c66 293a  f __str__(self):
+0000be80: 0a20 2020 2020 2020 206f 7574 7075 743d  .        output=
+0000be90: 2249 6e66 6f20 4d6f 6465 6c3a 205c 6e22  "Info Model: \n"
+0000bea0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
+0000beb0: 3d27 4e75 6d62 6572 206f 6620 7370 6563  ='Number of spec
+0000bec0: 6965 7320 2020 2020 2020 2020 203d 2027  ies          = '
+0000bed0: 0a20 2020 2020 2020 206f 7574 7075 742b  .        output+
+0000bee0: 3d73 7472 2873 656c 662e 4e73 7065 6369  =str(self.Nspeci
+0000bef0: 6573 292b 275c 6e5c 6e27 0a20 2020 2020  es)+'\n\n'.     
+0000bf00: 2020 206f 7574 7075 742b 3d27 4772 6964     output+='Grid
+0000bf10: 2073 697a 6520 2020 2020 2020 2020 2020   size           
+0000bf20: 2020 2020 2020 203d 2027 0a20 2020 2020         = '.     
+0000bf30: 2020 206f 7574 7075 742b 3d73 7472 2873     output+=str(s
+0000bf40: 656c 662e 4e67 7269 6429 2b27 5c6e 5c6e  elf.Ngrid)+'\n\n
+0000bf50: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
+0000bf60: 2b3d 2752 6573 6f6c 7669 6e67 2070 6f77  +='Resolving pow
+0000bf70: 6572 206f 6620 7370 6563 7472 6120 3d20  er of spectra = 
+0000bf80: 270a 2020 2020 2020 2020 6f75 7470 7574  '.        output
+0000bf90: 2b3d 7374 7228 7365 6c66 2e52 292b 275c  +=str(self.R)+'\
+0000bfa0: 6e5c 6e27 0a20 2020 2020 2020 206f 7574  n\n'.        out
+0000bfb0: 7075 742b 3d27 4f75 7470 7574 2066 696c  put+='Output fil
+0000bfc0: 6520 7061 7468 203d 2027 0a20 2020 2020  e path = '.     
+0000bfd0: 2020 206f 7574 7075 742b 3d73 7472 2873     output+=str(s
+0000bfe0: 656c 662e 6469 7265 6374 6f72 7929 2b27  elf.directory)+'
+0000bff0: 5c6e 5c6e 270a 2020 2020 2020 2020 7265  \n\n'.        re
+0000c000: 7475 726e 206f 7574 7075 740a 0a20 2020  turn output..   
+0000c010: 2064 6566 2063 6f6e 766f 6c76 6528 7365   def convolve(se
+0000c020: 6c66 2c52 3d31 2c6c 616d 6264 615f 303d  lf,R=1,lambda_0=
+0000c030: 312c 6c61 6d62 6461 5f6e 3d31 2c76 6572  1,lambda_n=1,ver
+0000c040: 626f 7365 3d54 7275 6529 3a0a 2020 2020  bose=True):.    
+0000c050: 2020 2020 6966 2076 6572 626f 7365 3a20      if verbose: 
+0000c060: 7072 696e 7428 2243 6f6e 766f 6c76 696e  print("Convolvin
+0000c070: 6720 746f 2022 2c52 290a 2020 2020 2020  g to ",R).      
+0000c080: 2020 6966 206c 616d 6264 615f 303d 3d6c    if lambda_0==l
+0000c090: 616d 6264 615f 6e3a 0a20 2020 2020 2020  ambda_n:.       
+0000c0a0: 2020 2020 206c 616d 6264 615f 303d 6e70       lambda_0=np
+0000c0b0: 2e61 6d69 6e28 632f 7365 6c66 2e66 7265  .amin(c/self.fre
+0000c0c0: 7175 656e 6379 2a31 652d 3329 0a20 2020  quency*1e-3).   
+0000c0d0: 2020 2020 2020 2020 206c 616d 6264 615f           lambda_
+0000c0e0: 6e3d 6e70 2e61 6d61 7828 632f 7365 6c66  n=np.amax(c/self
+0000c0f0: 2e66 7265 7175 656e 6379 2a31 652d 3329  .frequency*1e-3)
+0000c100: 0a20 2020 2020 2020 2020 2020 206c 616d  .            lam
+0000c110: 6264 615f 303d 6c61 6d62 6461 5f30 2a31  bda_0=lambda_0*1
+0000c120: 302a 2a2d 302e 3035 0a20 2020 2020 2020  0**-0.05.       
+0000c130: 2020 2020 206c 616d 6264 615f 6e3d 6c61       lambda_n=la
+0000c140: 6d62 6461 5f6e 2a31 302a 2a30 2e30 350a  mbda_n*10**0.05.
+0000c150: 2020 2020 2020 2020 6d61 736b 3d28 7365          mask=(se
+0000c160: 6c66 2e66 7265 7175 656e 6379 3e63 2f6c  lf.frequency>c/l
+0000c170: 616d 6264 615f 6e2a 3165 2d33 2926 2873  ambda_n*1e-3)&(s
+0000c180: 656c 662e 6672 6571 7565 6e63 793c 632f  elf.frequency<c/
+0000c190: 6c61 6d62 6461 5f30 2a31 652d 3329 0a20  lambda_0*1e-3). 
+0000c1a0: 2020 2020 2020 2046 5748 4d3d 7365 6c66         FWHM=self
+0000c1b0: 2e52 2f52 2f32 2e33 3535 0a20 2020 2020  .R/R/2.355.     
+0000c1c0: 2020 2067 3d47 6175 7373 6961 6e31 444b     g=Gaussian1DK
+0000c1d0: 6572 6e65 6c28 7374 6464 6576 3d46 5748  ernel(stddev=FWH
+0000c1e0: 4d2c 6661 6374 6f72 3d37 290a 2020 2020  M,factor=7).    
+0000c1f0: 2020 2020 7365 6c66 2e63 6f6e 765f 666c      self.conv_fl
+0000c200: 7578 3d61 7079 5f63 6f6e 766f 6c76 6528  ux=apy_convolve(
+0000c210: 7365 6c66 2e66 6c75 785b 6d61 736b 5d2c  self.flux[mask],
+0000c220: 6729 0a20 2020 2020 2020 2073 656c 662e  g).        self.
+0000c230: 636f 6e76 4672 6571 7565 6e63 793d 7365  convFrequency=se
+0000c240: 6c66 2e66 7265 7175 656e 6379 5b6d 6173  lf.frequency[mas
+0000c250: 6b5d 2a31 2e30 0a20 2020 2020 2020 2073  k]*1.0.        s
+0000c260: 656c 662e 636f 6e76 523d 520a 2020 2020  elf.convR=R.    
+0000c270: 2020 2020 7365 6c66 2e63 6f6e 7657 6176      self.convWav
+0000c280: 656c 656e 6774 683d 632f 7365 6c66 2e63  elength=c/self.c
+0000c290: 6f6e 7646 7265 7175 656e 6379 2a31 652d  onvFrequency*1e-
+0000c2a0: 330a 0a20 2020 2064 6566 2073 686f 7728  3..    def show(
+0000c2b0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+0000c2c0: 7269 6e74 2873 656c 6629 0a20 2020 2020  rint(self).     
+0000c2d0: 2020 2070 7269 6e74 2827 4772 6964 2020     print('Grid  
+0000c2e0: 2020 3d20 2729 0a20 2020 2020 2020 2070    = ').        p
+0000c2f0: 7269 6e74 2873 656c 662e 6772 6964 290a  rint(self.grid).
+0000c300: 2020 2020 2020 2020 7072 696e 7428 2753          print('S
+0000c310: 6f75 7263 6520 6675 6e63 7469 6f6e 2020  ource function  
+0000c320: 203d 2027 290a 2020 2020 2020 2020 7072   = ').        pr
+0000c330: 696e 7428 7365 6c66 2e73 6f75 7263 655f  int(self.source_
+0000c340: 6675 6e63 7469 6f6e 290a 2020 2020 2020  function).      
+0000c350: 2020 7072 696e 7428 2747 6173 206f 6e6c    print('Gas onl
+0000c360: 7920 736f 7572 6365 2066 756e 6374 696f  y source functio
+0000c370: 6e20 2020 3d20 2729 0a20 2020 2020 2020  n   = ').       
+0000c380: 2070 7269 6e74 2873 656c 662e 736f 7572   print(self.sour
+0000c390: 6365 5f66 756e 6374 696f 6e5f 6761 7329  ce_function_gas)
+0000c3a0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+0000c3b0: 4475 7374 206f 7074 6963 616c 2064 6570  Dust optical dep
+0000c3c0: 7468 2020 203d 2027 290a 2020 2020 2020  th   = ').      
+0000c3d0: 2020 7072 696e 7428 7365 6c66 2e74 6175    print(self.tau
+0000c3e0: 5f64 7573 7429 0a20 2020 2020 2020 2070  _dust).        p
+0000c3f0: 7269 6e74 2827 4761 7320 6f70 7469 6361  rint('Gas optica
+0000c400: 6c20 6465 7074 6820 2020 3d20 2729 0a20  l depth   = '). 
+0000c410: 2020 2020 2020 2070 7269 6e74 2873 656c         print(sel
+0000c420: 662e 7461 755f 6761 7329 0a0a 0a64 6566  f.tau_gas)...def
+0000c430: 2072 6561 645f 3144 5f73 6c61 6228 6d6f   read_1D_slab(mo
+0000c440: 6465 6c5f 7061 7468 3d27 536c 6162 5265  del_path='SlabRe
+0000c450: 7375 6c74 732e 6669 7473 2e67 7a27 2c76  sults.fits.gz',v
+0000c460: 6572 626f 7365 3d54 7275 6529 3a0a 2020  erbose=True):.  
+0000c470: 2020 2222 220a 2020 2020 4675 6e63 7469    """.    Functi
+0000c480: 6f6e 2074 6f20 7265 6164 2031 4420 7072  on to read 1D pr
+0000c490: 6f64 696d 6f20 736c 6162 206d 6f64 656c  odimo slab model
+0000c4a0: 206f 7574 7075 740a 2020 2020 2222 220a   output.    """.
+0000c4b0: 2020 2020 6966 2076 6572 626f 7365 3a20      if verbose: 
+0000c4c0: 7072 696e 7428 2252 6561 6469 6e67 2031  print("Reading 1
+0000c4d0: 4420 736c 6162 206d 6f64 656c 206f 7574  D slab model out
+0000c4e0: 7075 7420 6672 6f6d 3a20 222c 6d6f 6465  put from: ",mode
+0000c4f0: 6c5f 7061 7468 290a 2020 2020 6966 2027  l_path).    if '
+0000c500: 2e66 6974 732e 677a 2720 696e 206d 6f64  .fits.gz' in mod
+0000c510: 656c 5f70 6174 683a 0a20 2020 2020 2020  el_path:.       
+0000c520: 2068 6475 6c3d 6669 7473 2e6f 7065 6e28   hdul=fits.open(
+0000c530: 6d6f 6465 6c5f 7061 7468 290a 2020 2020  model_path).    
+0000c540: 2020 2020 6461 7461 3d73 6c61 6231 4428      data=slab1D(
+0000c550: 290a 2020 2020 2020 2020 6461 7461 2e64  ).        data.d
+0000c560: 6972 6563 746f 7279 3d6d 6f64 656c 5f70  irectory=model_p
+0000c570: 6174 680a 2020 2020 2020 2020 6461 7461  ath.        data
+0000c580: 2e66 6c75 783d 6864 756c 5b30 5d2e 6461  .flux=hdul[0].da
+0000c590: 7461 2e54 5b3a 2c31 5d0a 2020 2020 2020  ta.T[:,1].      
+0000c5a0: 2020 6461 7461 2e66 7265 7175 656e 6379    data.frequency
+0000c5b0: 3d68 6475 6c5b 305d 2e64 6174 612e 545b  =hdul[0].data.T[
+0000c5c0: 3a2c 305d 0a20 2020 2020 2020 2064 6174  :,0].        dat
+0000c5d0: 612e 4e73 7065 6369 6573 3d68 6475 6c5b  a.Nspecies=hdul[
+0000c5e0: 305d 2e68 6561 6465 725b 274e 5350 4543  0].header['NSPEC
+0000c5f0: 4945 5327 5d0a 2020 2020 2020 2020 6461  IES'].        da
+0000c600: 7461 2e73 7065 6369 6573 3d68 6475 6c5b  ta.species=hdul[
+0000c610: 305d 2e68 6561 6465 722e 636f 6d6d 656e  0].header.commen
+0000c620: 7473 5b27 4e53 5045 4349 4553 275d 2e73  ts['NSPECIES'].s
+0000c630: 706c 6974 2827 2c27 290a 2020 2020 2020  plit(',').      
+0000c640: 2020 6461 7461 2e4e 6772 6964 3d68 6475    data.Ngrid=hdu
+0000c650: 6c5b 305d 2e68 6561 6465 725b 274e 4752  l[0].header['NGR
+0000c660: 4944 275d 0a20 2020 2020 2020 2064 6174  ID'].        dat
+0000c670: 612e 523d 6864 756c 5b30 5d2e 6865 6164  a.R=hdul[0].head
+0000c680: 6572 5b27 525f 4f56 4c50 275d 0a20 2020  er['R_OVLP'].   
+0000c690: 2020 2020 2069 6620 2828 392b 6461 7461       if ((9+data
+0000c6a0: 2e4e 7370 6563 6965 732a 3229 2c64 6174  .Nspecies*2),dat
+0000c6b0: 612e 4e67 7269 6429 3d3d 6864 756c 5b31  a.Ngrid)==hdul[1
+0000c6c0: 5d2e 6461 7461 2e54 2e73 6861 7065 3a0a  ].data.T.shape:.
+0000c6d0: 2020 2020 2020 2020 2020 2020 6772 6964              grid
+0000c6e0: 3d68 6475 6c5b 315d 2e64 6174 610a 2020  =hdul[1].data.  
+0000c6f0: 2020 2020 2020 2020 2020 6461 7461 2e67            data.g
+0000c700: 7269 645b 2764 7a27 5d3d 6772 6964 5b3a  rid['dz']=grid[:
+0000c710: 2c30 5d0a 2020 2020 2020 2020 2020 2020  ,0].            
+0000c720: 6461 7461 2e67 7269 645b 2776 7475 7262  data.grid['vturb
+0000c730: 275d 3d67 7269 645b 3a2c 315d 0a20 2020  ']=grid[:,1].   
+0000c740: 2020 2020 2020 2020 2064 6174 612e 6772           data.gr
+0000c750: 6964 5b27 6e64 275d 3d67 7269 645b 3a2c  id['nd']=grid[:,
+0000c760: 325d 0a20 2020 2020 2020 2020 2020 2064  2].            d
+0000c770: 6174 612e 6772 6964 5b27 5464 275d 3d67  ata.grid['Td']=g
+0000c780: 7269 645b 3a2c 335d 0a20 2020 2020 2020  rid[:,3].       
+0000c790: 2020 2020 2064 6174 612e 6772 6964 5b27       data.grid['
+0000c7a0: 6e48 3227 5d3d 6772 6964 5b3a 2c34 5d0a  nH2']=grid[:,4].
+0000c7b0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000c7c0: 2e67 7269 645b 276e 4849 275d 3d67 7269  .grid['nHI']=gri
+0000c7d0: 645b 3a2c 355d 0a20 2020 2020 2020 2020  d[:,5].         
+0000c7e0: 2020 2064 6174 612e 6772 6964 5b27 6e48     data.grid['nH
+0000c7f0: 4949 275d 3d67 7269 645b 3a2c 365d 0a20  II']=grid[:,6]. 
+0000c800: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+0000c810: 6772 6964 5b27 6e48 6527 5d3d 6772 6964  grid['nHe']=grid
+0000c820: 5b3a 2c37 5d0a 2020 2020 2020 2020 2020  [:,7].          
+0000c830: 2020 6461 7461 2e67 7269 645b 276e 656c    data.grid['nel
+0000c840: 6563 275d 3d67 7269 645b 3a2c 385d 0a20  ec']=grid[:,8]. 
+0000c850: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0000c860: 2069 6e20 7261 6e67 6528 6461 7461 2e4e   in range(data.N
+0000c870: 7370 6563 6965 7329 3a0a 2020 2020 2020  species):.      
+0000c880: 2020 2020 2020 2020 2020 6b65 793d 276e            key='n
+0000c890: 272b 6461 7461 2e73 7065 6369 6573 5b69  '+data.species[i
+0000c8a0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000c8b0: 2020 6461 7461 2e67 7269 645b 6b65 795d    data.grid[key]
+0000c8c0: 3d67 7269 645b 3a2c 392b 695d 0a20 2020  =grid[:,9+i].   
+0000c8d0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+0000c8e0: 6e20 7261 6e67 6528 6461 7461 2e4e 7370  n range(data.Nsp
+0000c8f0: 6563 6965 7329 3a0a 2020 2020 2020 2020  ecies):.        
+0000c900: 2020 2020 2020 2020 6b65 793d 2754 675f          key='Tg_
+0000c910: 272b 6461 7461 2e73 7065 6369 6573 5b69  '+data.species[i
+0000c920: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000c930: 2020 6461 7461 2e67 7269 645b 6b65 795d    data.grid[key]
+0000c940: 3d67 7269 645b 3a2c 392b 6461 7461 2e4e  =grid[:,9+data.N
+0000c950: 7370 6563 6965 732b 695d 0a20 2020 2020  species+i].     
+0000c960: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000c970: 2020 2020 2072 6169 7365 2041 7373 6572       raise Asser
+0000c980: 7469 6f6e 4572 726f 7228 2747 7269 6420  tionError('Grid 
+0000c990: 696e 206f 7574 7075 7420 6669 6c65 2064  in output file d
+0000c9a0: 6f65 7320 6e6f 7420 6d61 7463 6820 7468  oes not match th
+0000c9b0: 6520 6163 7475 616c 2067 7269 6420 6f75  e actual grid ou
+0000c9c0: 7470 7574 2061 7272 6179 2729 0a0a 2020  tput array')..  
+0000c9d0: 2020 2020 2020 6966 2028 6c65 6e28 6461        if (len(da
+0000c9e0: 7461 2e66 7265 7175 656e 6379 292c 6461  ta.frequency),da
+0000c9f0: 7461 2e4e 6772 6964 293d 3d68 6475 6c5b  ta.Ngrid)==hdul[
+0000ca00: 325d 2e64 6174 612e 542e 7368 6170 653a  2].data.T.shape:
+0000ca10: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000ca20: 612e 736f 7572 6365 5f66 756e 6374 696f  a.source_functio
+0000ca30: 6e3d 6864 756c 5b32 5d2e 6461 7461 0a20  n=hdul[2].data. 
+0000ca40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000ca50: 2020 2020 2020 2020 2072 6169 7365 2041           raise A
+0000ca60: 7373 6572 7469 6f6e 4572 726f 7228 2753  ssertionError('S
+0000ca70: 6f75 7263 6520 6675 6e63 7469 6f6e 2067  ource function g
+0000ca80: 7269 6420 696e 206f 7574 7075 7420 6669  rid in output fi
+0000ca90: 6c65 2064 6f65 7320 6e6f 7420 6d61 7463  le does not matc
+0000caa0: 6820 7468 6520 7370 6174 6961 6c20 616e  h the spatial an
+0000cab0: 6420 6672 6571 7565 6e63 7920 6772 6964  d frequency grid
+0000cac0: 2073 697a 6527 290a 0a20 2020 2020 2020   size')..       
+0000cad0: 2069 6620 286c 656e 2864 6174 612e 6672   if (len(data.fr
+0000cae0: 6571 7565 6e63 7929 2c64 6174 612e 4e67  equency),data.Ng
+0000caf0: 7269 6429 3d3d 6864 756c 5b33 5d2e 6461  rid)==hdul[3].da
+0000cb00: 7461 2e54 2e73 6861 7065 3a0a 2020 2020  ta.T.shape:.    
+0000cb10: 2020 2020 2020 2020 6461 7461 2e73 6f75          data.sou
+0000cb20: 7263 655f 6675 6e63 7469 6f6e 5f67 6173  rce_function_gas
+0000cb30: 3d68 6475 6c5b 335d 2e64 6174 610a 2020  =hdul[3].data.  
+0000cb40: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000cb50: 2020 2020 2020 2020 7261 6973 6520 4173          raise As
+0000cb60: 7365 7274 696f 6e45 7272 6f72 2827 4761  sertionError('Ga
+0000cb70: 7320 736f 7572 6365 2066 756e 6374 696f  s source functio
+0000cb80: 6e20 6772 6964 2069 6e20 6f75 7470 7574  n grid in output
+0000cb90: 2066 696c 6520 646f 6573 206e 6f74 206d   file does not m
+0000cba0: 6174 6368 2074 6865 2073 7061 7469 616c  atch the spatial
+0000cbb0: 2061 6e64 2066 7265 7175 656e 6379 2067   and frequency g
+0000cbc0: 7269 6420 7369 7a65 2729 0a0a 2020 2020  rid size')..    
+0000cbd0: 2020 2020 6966 2028 6c65 6e28 6461 7461      if (len(data
+0000cbe0: 2e66 7265 7175 656e 6379 292c 6461 7461  .frequency),data
+0000cbf0: 2e4e 6772 6964 293d 3d68 6475 6c5b 345d  .Ngrid)==hdul[4]
+0000cc00: 2e64 6174 612e 542e 7368 6170 653a 0a20  .data.T.shape:. 
+0000cc10: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+0000cc20: 7461 755f 6475 7374 3d68 6475 6c5b 345d  tau_dust=hdul[4]
+0000cc30: 2e64 6174 610a 2020 2020 2020 2020 656c  .data.        el
+0000cc40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000cc50: 7261 6973 6520 4173 7365 7274 696f 6e45  raise AssertionE
+0000cc60: 7272 6f72 2827 4475 7374 206f 7074 6963  rror('Dust optic
+0000cc70: 616c 2064 6570 7468 2067 7269 6420 696e  al depth grid in
+0000cc80: 206f 7574 7075 7420 6669 6c65 2064 6f65   output file doe
+0000cc90: 7320 6e6f 7420 6d61 7463 6820 7468 6520  s not match the 
+0000cca0: 7370 6174 6961 6c20 616e 6420 6672 6571  spatial and freq
+0000ccb0: 7565 6e63 7920 6772 6964 2073 697a 6527  uency grid size'
+0000ccc0: 290a 0a20 2020 2020 2020 2069 6620 286c  )..        if (l
+0000ccd0: 656e 2864 6174 612e 6672 6571 7565 6e63  en(data.frequenc
+0000cce0: 7929 2c64 6174 612e 4e67 7269 6429 3d3d  y),data.Ngrid)==
+0000ccf0: 6864 756c 5b35 5d2e 6461 7461 2e54 2e73  hdul[5].data.T.s
+0000cd00: 6861 7065 3a0a 2020 2020 2020 2020 2020  hape:.          
+0000cd10: 2020 6461 7461 2e74 6175 5f67 6173 3d68    data.tau_gas=h
+0000cd20: 6475 6c5b 355d 2e64 6174 610a 2020 2020  dul[5].data.    
+0000cd30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000cd40: 2020 2020 2020 7261 6973 6520 4173 7365        raise Asse
+0000cd50: 7274 696f 6e45 7272 6f72 2827 4761 7320  rtionError('Gas 
+0000cd60: 6f70 7469 6361 6c20 6465 7074 6820 6772  optical depth gr
+0000cd70: 6964 2069 6e20 6f75 7470 7574 2066 696c  id in output fil
+0000cd80: 6520 646f 6573 206e 6f74 206d 6174 6368  e does not match
+0000cd90: 2074 6865 2073 7061 7469 616c 2061 6e64   the spatial and
+0000cda0: 2066 7265 7175 656e 6379 2067 7269 6420   frequency grid 
+0000cdb0: 7369 7a65 2729 0a20 2020 2065 6c73 653a  size').    else:
+0000cdc0: 0a20 2020 2020 2020 2064 6174 615f 7265  .        data_re
+0000cdd0: 6164 3d6e 702e 6c6f 6164 7478 7428 6d6f  ad=np.loadtxt(mo
+0000cde0: 6465 6c5f 7061 7468 2c73 6b69 7072 6f77  del_path,skiprow
+0000cdf0: 733d 3129 0a20 2020 2020 2020 2064 6174  s=1).        dat
+0000ce00: 613d 736c 6162 3144 2829 0a20 2020 2020  a=slab1D().     
+0000ce10: 2020 2064 6174 612e 6469 7265 6374 6f72     data.director
+0000ce20: 793d 6d6f 6465 6c5f 7061 7468 0a20 2020  y=model_path.   
+0000ce30: 2020 2020 2064 6174 612e 666c 7578 3d64       data.flux=d
+0000ce40: 6174 615f 7265 6164 5b3a 2c31 5d0a 2020  ata_read[:,1].  
+0000ce50: 2020 2020 2020 6461 7461 2e66 7265 7175        data.frequ
+0000ce60: 656e 6379 3d64 6174 615f 7265 6164 5b3a  ency=data_read[:
+0000ce70: 2c30 5d0a 2020 2020 7265 7475 726e 2864  ,0].    return(d
+0000ce80: 6174 6129 0a0a 0a64 6566 2072 6561 645f  ata)...def read_
+0000ce90: 736c 6162 286d 6f64 656c 5f70 6174 683d  slab(model_path=
+0000cea0: 2753 6c61 6252 6573 756c 7473 2e6f 7574  'SlabResults.out
+0000ceb0: 272c 7665 7262 6f73 653d 5472 7565 2c73  ',verbose=True,s
+0000cec0: 686f 7274 5f66 6f72 6d61 743d 4661 6c73  hort_format=Fals
+0000ced0: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+0000cee0: 4675 6e63 7469 6f6e 2074 6f20 7265 6164  Function to read
+0000cef0: 2073 6c61 6220 6d6f 6465 6c20 6f75 7470   slab model outp
+0000cf00: 7574 0a20 2020 2022 2222 0a20 2020 2069  ut.    """.    i
+0000cf10: 6620 6973 696e 7374 616e 6365 286d 6f64  f isinstance(mod
+0000cf20: 656c 5f70 6174 682c 6c69 7374 293a 0a20  el_path,list):. 
+0000cf30: 2020 2020 2020 2064 6174 613d 736c 6162         data=slab
+0000cf40: 5f64 6174 6128 290a 2020 2020 2020 2020  _data().        
+0000cf50: 6461 7461 2e64 6972 6563 746f 7279 3d6d  data.directory=m
+0000cf60: 6f64 656c 5f70 6174 680a 2020 2020 2020  odel_path.      
+0000cf70: 2020 666f 7220 6920 696e 206d 6f64 656c    for i in model
+0000cf80: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
+0000cf90: 2020 2072 6461 7461 3d72 6561 645f 736c     rdata=read_sl
+0000cfa0: 6162 2869 2c76 6572 626f 7365 3d76 6572  ab(i,verbose=ver
+0000cfb0: 626f 7365 2c73 686f 7274 5f66 6f72 6d61  bose,short_forma
+0000cfc0: 743d 7368 6f72 745f 666f 726d 6174 290a  t=short_format).
+0000cfd0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000cfe0: 6a20 696e 2072 616e 6765 2872 6461 7461  j in range(rdata
+0000cff0: 2e6e 6d6f 6465 6c73 293a 0a20 2020 2020  .nmodels):.     
+0000d000: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+0000d010: 6164 645f 6d6f 6465 6c28 7264 6174 612e  add_model(rdata.
+0000d020: 6d6f 6465 6c73 5b6a 5d29 0a20 2020 2020  models[j]).     
+0000d030: 2020 2072 6574 7572 6e28 6461 7461 290a     return(data).
+0000d040: 0a20 2020 2069 6620 7665 7262 6f73 653a  .    if verbose:
+0000d050: 2070 7269 6e74 2822 5265 6164 696e 6720   print("Reading 
+0000d060: 736c 6162 206d 6f64 656c 206f 7574 7075  slab model outpu
+0000d070: 7420 6672 6f6d 3a20 222c 6d6f 6465 6c5f  t from: ",model_
+0000d080: 7061 7468 290a 2020 2020 663d 6f70 656e  path).    f=open
+0000d090: 286d 6f64 656c 5f70 6174 6829 0a20 2020  (model_path).   
+0000d0a0: 2064 6174 613d 736c 6162 5f64 6174 6128   data=slab_data(
+0000d0b0: 290a 2020 2020 6e6d 6f64 656c 733d 696e  ).    nmodels=in
+0000d0c0: 7428 662e 7265 6164 6c69 6e65 2829 2e73  t(f.readline().s
+0000d0d0: 706c 6974 2829 5b30 5d29 0a20 2020 2064  plit()[0]).    d
+0000d0e0: 6174 612e 6469 7265 6374 6f72 793d 6d6f  ata.directory=mo
+0000d0f0: 6465 6c5f 7061 7468 0a20 2020 2066 6f72  del_path.    for
+0000d100: 2069 2069 6e20 7261 6e67 6528 6e6d 6f64   i in range(nmod
+0000d110: 656c 7329 3a0a 2320 2020 2020 2020 2020  els):.#         
+0000d120: 7465 6d70 6f20 2020 2020 2020 2020 2020  tempo           
+0000d130: 2020 2020 203d 2020 2073 6c61 6228 290a       =   slab().
+0000d140: 2020 2020 2020 2020 7465 6d70 6f5f 6d6f          tempo_mo
+0000d150: 6465 6c5f 6e75 6d62 6572 3d69 6e74 2866  del_number=int(f
+0000d160: 2e72 6561 646c 696e 6528 292e 7370 6c69  .readline().spli
+0000d170: 7428 295b 305d 290a 2020 2020 2020 2020  t()[0]).        
+0000d180: 6e73 7065 6369 6573 3d69 6e74 2866 2e72  nspecies=int(f.r
+0000d190: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
+0000d1a0: 295b 305d 290a 2320 2020 2020 2020 2020  )[0]).#         
+0000d1b0: 7465 6d70 6f2e 7370 6563 6965 735f 6e75  tempo.species_nu
+0000d1c0: 6d62 6572 203d 2020 2069 6e74 2866 2e72  mber =   int(f.r
+0000d1d0: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
+0000d1e0: 295b 305d 290a 2020 2020 2020 2020 7465  )[0]).        te
+0000d1f0: 6d70 6f5f 6e48 746f 743d 666c 6f61 7428  mpo_nHtot=float(
+0000d200: 662e 7265 6164 6c69 6e65 2829 2e73 706c  f.readline().spl
+0000d210: 6974 2829 5b30 5d29 0a20 2020 2020 2020  it()[0]).       
+0000d220: 2074 656d 706f 5f67 6173 4465 6e73 3d66   tempo_gasDens=f
+0000d230: 6c6f 6174 2866 2e72 6561 646c 696e 6528  loat(f.readline(
+0000d240: 292e 7370 6c69 7428 295b 305d 290a 2020  ).split()[0]).  
+0000d250: 2020 2020 2020 7465 6d70 6f5f 6e65 6c65        tempo_nele
+0000d260: 633d 666c 6f61 7428 662e 7265 6164 6c69  c=float(f.readli
+0000d270: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
+0000d280: 0a20 2020 2020 2020 2074 656d 706f 5f6e  .        tempo_n
+0000d290: 4865 3d66 6c6f 6174 2866 2e72 6561 646c  He=float(f.readl
+0000d2a0: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
+0000d2b0: 290a 2020 2020 2020 2020 7465 6d70 6f5f  ).        tempo_
+0000d2c0: 6e48 4949 3d66 6c6f 6174 2866 2e72 6561  nHII=float(f.rea
+0000d2d0: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
+0000d2e0: 305d 290a 2020 2020 2020 2020 7465 6d70  0]).        temp
+0000d2f0: 6f5f 6e48 493d 666c 6f61 7428 662e 7265  o_nHI=float(f.re
+0000d300: 6164 6c69 6e65 2829 2e73 706c 6974 2829  adline().split()
+0000d310: 5b30 5d29 0a20 2020 2020 2020 2074 656d  [0]).        tem
+0000d320: 706f 5f6e 4832 3d66 6c6f 6174 2866 2e72  po_nH2=float(f.r
+0000d330: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
+0000d340: 295b 305d 290a 2020 2020 2020 2020 7465  )[0]).        te
+0000d350: 6d70 6f5f 6475 7374 5f74 6f5f 6761 733d  mpo_dust_to_gas=
+0000d360: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
+0000d370: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
+0000d380: 2020 2020 2020 2074 656d 706f 5f76 7475         tempo_vtu
+0000d390: 7262 3d66 6c6f 6174 2866 2e72 6561 646c  rb=float(f.readl
+0000d3a0: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
+0000d3b0: 290a 2020 2020 2020 2020 7465 6d70 6f5f  ).        tempo_
+0000d3c0: 5467 3d66 6c6f 6174 2866 2e72 6561 646c  Tg=float(f.readl
+0000d3d0: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
+0000d3e0: 290a 2020 2020 2020 2020 7465 6d70 6f5f  ).        tempo_
+0000d3f0: 5464 3d66 6c6f 6174 2866 2e72 6561 646c  Td=float(f.readl
+0000d400: 696e 6528 292e 7370 6c69 7428 295b 305d  ine().split()[0]
+0000d410: 290a 2020 2020 2020 2020 6966 2073 686f  ).        if sho
+0000d420: 7274 5f66 6f72 6d61 743a 0a20 2020 2020  rt_format:.     
+0000d430: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+0000d440: 7261 6e67 6528 6e73 7065 6369 6573 293a  range(nspecies):
+0000d450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d460: 2074 656d 706f 3d73 6c61 6228 290a 2020   tempo=slab().  
+0000d470: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000d480: 6d70 6f2e 6d6f 6465 6c5f 6e75 6d62 6572  mpo.model_number
+0000d490: 3d74 656d 706f 5f6d 6f64 656c 5f6e 756d  =tempo_model_num
+0000d4a0: 6265 720a 2020 2020 2020 2020 2020 2020  ber.            
+0000d4b0: 2020 2020 7465 6d70 6f2e 4e48 3d74 656d      tempo.NH=tem
+0000d4c0: 706f 5f6e 4874 6f74 0a20 2020 2020 2020  po_nHtot.       
+0000d4d0: 2020 2020 2020 2020 2074 656d 706f 2e6e           tempo.n
+0000d4e0: 436f 6c6c 3d74 656d 706f 5f67 6173 4465  Coll=tempo_gasDe
+0000d4f0: 6e73 0a20 2020 2020 2020 2020 2020 2020  ns.             
+0000d500: 2020 2074 656d 706f 2e6e 653d 7465 6d70     tempo.ne=temp
+0000d510: 6f5f 6e65 6c65 630a 2020 2020 2020 2020  o_nelec.        
+0000d520: 2020 2020 2020 2020 7465 6d70 6f2e 6e48          tempo.nH
+0000d530: 653d 7465 6d70 6f5f 6e48 650a 2020 2020  e=tempo_nHe.    
+0000d540: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000d550: 6f2e 6e48 4949 3d74 656d 706f 5f6e 4849  o.nHII=tempo_nHI
+0000d560: 490a 2020 2020 2020 2020 2020 2020 2020  I.              
+0000d570: 2020 7465 6d70 6f2e 6e48 493d 7465 6d70    tempo.nHI=temp
+0000d580: 6f5f 6e48 490a 2020 2020 2020 2020 2020  o_nHI.          
+0000d590: 2020 2020 2020 7465 6d70 6f2e 6e48 323d        tempo.nH2=
+0000d5a0: 7465 6d70 6f5f 6e48 320a 2020 2020 2020  tempo_nH2.      
+0000d5b0: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
+0000d5c0: 6475 7374 5f74 6f5f 6761 733d 7465 6d70  dust_to_gas=temp
+0000d5d0: 6f5f 6475 7374 5f74 6f5f 6761 730a 2020  o_dust_to_gas.  
+0000d5e0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000d5f0: 6d70 6f2e 7674 7572 623d 7465 6d70 6f5f  mpo.vturb=tempo_
+0000d600: 7674 7572 620a 2020 2020 2020 2020 2020  vturb.          
+0000d610: 2020 2020 2020 7465 6d70 6f2e 5467 3d74        tempo.Tg=t
+0000d620: 656d 706f 5f54 670a 2020 2020 2020 2020  empo_Tg.        
+0000d630: 2020 2020 2020 2020 7465 6d70 6f2e 5464          tempo.Td
+0000d640: 3d74 656d 706f 5f54 640a 0a20 2020 2020  =tempo_Td..     
+0000d650: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000d660: 2e73 7065 6369 6573 5f69 6e64 6578 3d69  .species_index=i
+0000d670: 6e74 2866 2e72 6561 646c 696e 6528 292e  nt(f.readline().
+0000d680: 7370 6c69 7428 295b 305d 290a 2020 2020  split()[0]).    
+0000d690: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000d6a0: 6f2e 7370 6563 6965 735f 6e75 6d62 6572  o.species_number
+0000d6b0: 3d6a 2b31 0a20 2020 2020 2020 2020 2020  =j+1.           
+0000d6c0: 2020 2020 2074 656d 706f 2e73 7065 6369       tempo.speci
+0000d6d0: 6573 5f6e 616d 653d 662e 7265 6164 6c69  es_name=f.readli
+0000d6e0: 6e65 2829 2e73 706c 6974 2829 5b30 5d0a  ne().split()[0].
+0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d700: 7465 6d70 6f2e 6162 756e 6461 6e63 653d  tempo.abundance=
+0000d710: 666c 6f61 7428 662e 7265 6164 6c69 6e65  float(f.readline
+0000d720: 2829 2e73 706c 6974 2829 5b30 5d29 0a20  ().split()[0]). 
+0000d730: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000d740: 656d 706f 2e64 763d 666c 6f61 7428 662e  empo.dv=float(f.
+0000d750: 7265 6164 6c69 6e65 2829 2e73 706c 6974  readline().split
+0000d760: 2829 5b30 5d29 0a20 2020 2020 2020 2020  ()[0]).         
+0000d770: 2020 2020 2020 2074 656d 706f 2e6e 6c69         tempo.nli
+0000d780: 6e65 733d 696e 7428 662e 7265 6164 6c69  nes=int(f.readli
+0000d790: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
+0000d7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d7b0: 206c 696e 6573 3d66 2e72 6561 646c 696e   lines=f.readlin
+0000d7c0: 6528 290a 0a20 2020 2020 2020 2020 2020  e()..           
+0000d7d0: 2020 2020 2023 2074 656d 706f 2e6e 6c69       # tempo.nli
+0000d7e0: 6e65 733d 4e6f 6e65 0a20 2020 2020 2020  nes=None.       
+0000d7f0: 2020 2020 2020 2020 2074 656d 706f 2e6c           tempo.l
+0000d800: 696e 6564 6174 613d 4e6f 6e65 0a20 2020  inedata=None.   
+0000d810: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000d820: 706f 2e6c 6576 656c 6461 7461 3d4e 6f6e  po.leveldata=Non
+0000d830: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000d840: 2020 7465 6d70 6f2e 636f 6e76 5761 7665    tempo.convWave
+0000d850: 6c65 6e67 7468 3d4e 6f6e 650a 2020 2020  length=None.    
+0000d860: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000d870: 6f2e 636f 6e76 4c54 4566 6c75 783d 4e6f  o.convLTEflux=No
+0000d880: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0000d890: 2020 2074 656d 706f 2e63 6f6e 764e 4c54     tempo.convNLT
+0000d8a0: 4566 6c75 783d 4e6f 6e65 0a20 2020 2020  Eflux=None.     
+0000d8b0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000d8c0: 2e63 6f6e 7654 7970 653d 4e6f 6e65 0a20  .convType=None. 
+0000d8d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000d8e0: 656d 706f 2e63 6f6e 7652 3d4e 6f6e 650a  empo.convR=None.
+0000d8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d900: 2064 6174 3d5b 5d0a 2020 2020 2020 2020   dat=[].        
+0000d910: 2020 2020 2020 2020 2320 666f 7220 6b20          # for k 
+0000d920: 696e 2072 616e 6765 2874 656d 706f 2e6e  in range(tempo.n
+0000d930: 6c65 7665 6c73 293a 0a20 2020 2020 2020  levels):.       
+0000d940: 2020 2020 2020 2020 2023 2020 2020 2064           #     d
+0000d950: 6174 5b30 5d5b 6b2c 3a5d 3d6e 702e 6173  at[0][k,:]=np.as
+0000d960: 6172 7261 7928 5b66 6c6f 6174 2878 2920  array([float(x) 
+0000d970: 666f 7220 7820 696e 2066 2e72 6561 646c  for x in f.readl
+0000d980: 696e 6528 292e 7370 6c69 7428 295d 290a  ine().split()]).
+0000d990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d9a0: 2023 206c 696e 6573 3d66 2e72 6561 646c   # lines=f.readl
+0000d9b0: 696e 6528 290a 2020 2020 2020 2020 2020  ine().          
+0000d9c0: 2020 2020 2020 2320 6c69 6e65 733d 662e        # lines=f.
+0000d9d0: 7265 6164 6c69 6e65 2829 0a20 2020 2020  readline().     
+0000d9e0: 2020 2020 2020 2020 2020 2064 6174 3d6e             dat=n
+0000d9f0: 702e 7a65 726f 7328 2874 656d 706f 2e6e  p.zeros((tempo.n
+0000da00: 6c69 6e65 732c 3429 290a 2020 2020 2020  lines,4)).      
+0000da10: 2020 2020 2020 2020 2020 736c 6162 4f75            slabOu
+0000da20: 7446 6f72 6d61 743d 5b38 2c31 342c 3135  tFormat=[8,14,15
+0000da30: 2c31 355d 0a20 2020 2020 2020 2020 2020  ,15].           
+0000da40: 2020 2020 2066 6f72 206b 2069 6e20 7261       for k in ra
+0000da50: 6e67 6528 7465 6d70 6f2e 6e6c 696e 6573  nge(tempo.nlines
+0000da60: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000da70: 2020 2020 2020 206c 696e 6552 6561 643d         lineRead=
+0000da80: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
+0000da90: 2020 2020 2020 206c 696e 6573 3d66 2e72         lines=f.r
+0000daa0: 6561 646c 696e 6528 290a 2020 2020 2020  eadline().      
+0000dab0: 2020 2020 2020 2020 2020 2020 2020 6c3d                l=
+0000dac0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+0000dad0: 2020 2020 2020 666f 7220 6c65 6e67 7468        for length
+0000dae0: 2069 6e20 736c 6162 4f75 7446 6f72 6d61   in slabOutForma
+0000daf0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0000db00: 2020 2020 2020 2020 2020 206c 696e 6552             lineR
+0000db10: 6561 642e 6170 7065 6e64 286c 696e 6573  ead.append(lines
+0000db20: 5b6c 3a6c 2b6c 656e 6774 685d 290a 2020  [l:l+length]).  
+0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db40: 2020 2020 2020 6c2b 3d6c 656e 6774 680a        l+=length.
+0000db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db60: 2020 2020 6461 745b 6b2c 3a5d 3d6e 702e      dat[k,:]=np.
+0000db70: 6173 6172 7261 7928 5b66 6c6f 6174 2878  asarray([float(x
+0000db80: 2920 666f 7220 7820 696e 206c 696e 6552  ) for x in lineR
+0000db90: 6561 645d 290a 2020 2020 2020 2020 2020  ead]).          
+0000dba0: 2020 2020 2020 6c69 6e65 4461 7461 3d70        lineData=p
+0000dbb0: 642e 4461 7461 4672 616d 6528 6461 742c  d.DataFrame(dat,
+0000dbc0: 636f 6c75 6d6e 733d 5b27 6927 2c27 4748  columns=['i','GH
+0000dbd0: 7a27 2c27 464e 4c54 4527 2c27 464c 5445  z','FNLTE','FLTE
+0000dbe0: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
+0000dbf0: 2020 2020 7465 6d70 6f2e 6c69 6e65 6461      tempo.lineda
+0000dc00: 7461 3d6c 696e 6544 6174 610a 2020 2020  ta=lineData.    
+0000dc10: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000dc20: 2e61 6464 5f6d 6f64 656c 2874 656d 706f  .add_model(tempo
+0000dc30: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000dc40: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000dc50: 6a20 696e 2072 616e 6765 286e 7370 6563  j in range(nspec
+0000dc60: 6965 7329 3a0a 2020 2020 2020 2020 2020  ies):.          
+0000dc70: 2020 2020 2020 7465 6d70 6f3d 736c 6162        tempo=slab
+0000dc80: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000dc90: 2020 2074 656d 706f 2e6d 6f64 656c 5f6e     tempo.model_n
+0000dca0: 756d 6265 723d 7465 6d70 6f5f 6d6f 6465  umber=tempo_mode
+0000dcb0: 6c5f 6e75 6d62 6572 0a20 2020 2020 2020  l_number.       
+0000dcc0: 2020 2020 2020 2020 2074 656d 706f 2e4e           tempo.N
+0000dcd0: 483d 7465 6d70 6f5f 6e48 746f 740a 2020  H=tempo_nHtot.  
+0000dce0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000dcf0: 6d70 6f2e 6e43 6f6c 6c3d 7465 6d70 6f5f  mpo.nColl=tempo_
+0000dd00: 6761 7344 656e 730a 2020 2020 2020 2020  gasDens.        
+0000dd10: 2020 2020 2020 2020 7465 6d70 6f2e 6e65          tempo.ne
+0000dd20: 3d74 656d 706f 5f6e 656c 6563 0a20 2020  =tempo_nelec.   
+0000dd30: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000dd40: 706f 2e6e 4865 3d74 656d 706f 5f6e 4865  po.nHe=tempo_nHe
+0000dd50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dd60: 2074 656d 706f 2e6e 4849 493d 7465 6d70   tempo.nHII=temp
+0000dd70: 6f5f 6e48 4949 0a20 2020 2020 2020 2020  o_nHII.         
+0000dd80: 2020 2020 2020 2074 656d 706f 2e6e 4849         tempo.nHI
+0000dd90: 3d74 656d 706f 5f6e 4849 0a20 2020 2020  =tempo_nHI.     
+0000dda0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000ddb0: 2e6e 4832 3d74 656d 706f 5f6e 4832 0a20  .nH2=tempo_nH2. 
+0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000ddd0: 656d 706f 2e64 7573 745f 746f 5f67 6173  empo.dust_to_gas
+0000dde0: 3d74 656d 706f 5f64 7573 745f 746f 5f67  =tempo_dust_to_g
+0000ddf0: 6173 0a20 2020 2020 2020 2020 2020 2020  as.             
+0000de00: 2020 2074 656d 706f 2e76 7475 7262 3d74     tempo.vturb=t
+0000de10: 656d 706f 5f76 7475 7262 0a20 2020 2020  empo_vturb.     
+0000de20: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000de30: 2e54 673d 7465 6d70 6f5f 5467 0a20 2020  .Tg=tempo_Tg.   
+0000de40: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000de50: 706f 2e54 643d 7465 6d70 6f5f 5464 0a0a  po.Td=tempo_Td..
+0000de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de70: 7465 6d70 6f2e 7370 6563 6965 735f 696e  tempo.species_in
+0000de80: 6465 783d 696e 7428 662e 7265 6164 6c69  dex=int(f.readli
+0000de90: 6e65 2829 2e73 706c 6974 2829 5b30 5d29  ne().split()[0])
+0000dea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000deb0: 2074 656d 706f 2e73 7065 6369 6573 5f6e   tempo.species_n
+0000dec0: 756d 6265 723d 6a2b 310a 2020 2020 2020  umber=j+1.      
+0000ded0: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
+0000dee0: 7370 6563 6965 735f 6e61 6d65 3d66 2e72  species_name=f.r
+0000def0: 6561 646c 696e 6528 292e 7370 6c69 7428  eadline().split(
+0000df00: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
+0000df10: 2020 2020 2074 656d 706f 2e61 6275 6e64       tempo.abund
+0000df20: 616e 6365 3d66 6c6f 6174 2866 2e72 6561  ance=float(f.rea
+0000df30: 646c 696e 6528 292e 7370 6c69 7428 295b  dline().split()[
+0000df40: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
+0000df50: 2020 2020 7465 6d70 6f2e 6476 3d66 6c6f      tempo.dv=flo
+0000df60: 6174 2866 2e72 6561 646c 696e 6528 292e  at(f.readline().
+0000df70: 7370 6c69 7428 295b 305d 290a 2020 2020  split()[0]).    
+0000df80: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000df90: 6f2e 6e6c 6576 656c 733d 696e 7428 662e  o.nlevels=int(f.
+0000dfa0: 7265 6164 6c69 6e65 2829 2e73 706c 6974  readline().split
+0000dfb0: 2829 5b30 5d29 0a20 2020 2020 2020 2020  ()[0]).         
+0000dfc0: 2020 2020 2020 206c 696e 6573 3d66 2e72         lines=f.r
+0000dfd0: 6561 646c 696e 6528 290a 0a20 2020 2020  eadline()..     
+0000dfe0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000dff0: 2e6e 6c69 6e65 733d 4e6f 6e65 0a20 2020  .nlines=None.   
+0000e000: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000e010: 706f 2e6c 696e 6564 6174 613d 4e6f 6e65  po.linedata=None
+0000e020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e030: 2074 656d 706f 2e6c 6576 656c 6461 7461   tempo.leveldata
+0000e040: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
+0000e050: 2020 2020 2020 7465 6d70 6f2e 636f 6e76        tempo.conv
+0000e060: 5761 7665 6c65 6e67 7468 3d4e 6f6e 650a  Wavelength=None.
+0000e070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e080: 7465 6d70 6f2e 636f 6e76 4c54 4566 6c75  tempo.convLTEflu
+0000e090: 783d 4e6f 6e65 0a20 2020 2020 2020 2020  x=None.         
+0000e0a0: 2020 2020 2020 2074 656d 706f 2e63 6f6e         tempo.con
+0000e0b0: 764e 4c54 4566 6c75 783d 4e6f 6e65 0a20  vNLTEflux=None. 
+0000e0c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e0d0: 656d 706f 2e63 6f6e 7654 7970 653d 4e6f  empo.convType=No
+0000e0e0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0000e0f0: 2020 2074 656d 706f 2e63 6f6e 7652 3d4e     tempo.convR=N
+0000e100: 6f6e 650a 0a20 2020 2020 2020 2020 2020  one..           
+0000e110: 2020 2020 2064 6174 3d5b 6e70 2e7a 6572       dat=[np.zer
+0000e120: 6f73 2828 7465 6d70 6f2e 6e6c 6576 656c  os((tempo.nlevel
+0000e130: 732c 3829 292c 5b5d 2c5b 5d5d 0a20 2020  s,8)),[],[]].   
+0000e140: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000e150: 206b 2069 6e20 7261 6e67 6528 7465 6d70   k in range(temp
+0000e160: 6f2e 6e6c 6576 656c 7329 3a0a 2020 2020  o.nlevels):.    
+0000e170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e180: 6461 745b 305d 5b6b 2c3a 5d3d 6e70 2e61  dat[0][k,:]=np.a
+0000e190: 7361 7272 6179 285b 666c 6f61 7428 7829  sarray([float(x)
+0000e1a0: 2066 6f72 2078 2069 6e20 662e 7265 6164   for x in f.read
+0000e1b0: 6c69 6e65 2829 2e73 706c 6974 2829 5d29  line().split()])
+0000e1c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e1d0: 2074 656d 706f 2e6e 6c69 6e65 733d 696e   tempo.nlines=in
+0000e1e0: 7428 662e 7265 6164 6c69 6e65 2829 2e73  t(f.readline().s
+0000e1f0: 706c 6974 2829 5b30 5d29 0a20 2020 2020  plit()[0]).     
+0000e200: 2020 2020 2020 2020 2020 206c 696e 6573             lines
+0000e210: 3d66 2e72 6561 646c 696e 6528 290a 2020  =f.readline().  
+0000e220: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000e230: 6e65 733d 662e 7265 6164 6c69 6e65 2829  nes=f.readline()
+0000e240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e250: 2064 6174 5b31 5d3d 6e70 2e7a 6572 6f73   dat[1]=np.zeros
+0000e260: 2828 7465 6d70 6f2e 6e6c 696e 6573 2c32  ((tempo.nlines,2
+0000e270: 3329 290a 2020 2020 2020 2020 2020 2020  3)).            
+0000e280: 2020 2020 736c 6162 4f75 7446 6f72 6d61      slabOutForma
+0000e290: 743d 5b39 2c39 2c39 2c35 2c35 2c35 2c31  t=[9,9,9,5,5,5,1
+0000e2a0: 352c 3135 2c31 352c 3135 2c31 352c 3135  5,15,15,15,15,15
+0000e2b0: 2c31 352c 3135 2c31 352c 3135 2c31 352c  ,15,15,15,15,15,
+0000e2c0: 3135 2c31 352c 3135 2c31 352c 3135 2c31  15,15,15,15,15,1
+0000e2d0: 352c 3231 2c32 312c 3231 2c32 315d 0a20  5,21,21,21,21]. 
+0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000e2f0: 6f72 206b 2069 6e20 7261 6e67 6528 7465  or k in range(te
+0000e300: 6d70 6f2e 6e6c 696e 6573 293a 0a20 2020  mpo.nlines):.   
+0000e310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e320: 206c 696e 6552 6561 643d 5b5d 0a20 2020   lineRead=[].   
+0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e340: 206c 696e 6573 3d66 2e72 6561 646c 696e   lines=f.readlin
+0000e350: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0000e360: 2020 2020 2020 2020 6c3d 300a 2020 2020          l=0.    
+0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e380: 666f 7220 6c65 6e67 7468 2069 6e20 736c  for length in sl
+0000e390: 6162 4f75 7446 6f72 6d61 743a 0a20 2020  abOutFormat:.   
+0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3b0: 2020 2020 206c 696e 6552 6561 642e 6170       lineRead.ap
+0000e3c0: 7065 6e64 286c 696e 6573 5b6c 3a6c 2b6c  pend(lines[l:l+l
+0000e3d0: 656e 6774 685d 290a 2020 2020 2020 2020  ength]).        
+0000e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3f0: 6c2b 3d6c 656e 6774 680a 2020 2020 2020  l+=length.      
+0000e400: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000e410: 745b 315d 5b6b 2c3a 5d3d 6e70 2e61 7361  t[1][k,:]=np.asa
+0000e420: 7272 6179 285b 666c 6f61 7428 7829 2066  rray([float(x) f
+0000e430: 6f72 2078 2069 6e20 6c69 6e65 5265 6164  or x in lineRead
+0000e440: 5b30 3a2d 345d 5d29 0a20 2020 2020 2020  [0:-4]]).       
+0000e450: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+0000e460: 5b32 5d2e 6170 7065 6e64 285b 612e 7374  [2].append([a.st
+0000e470: 7269 7028 2920 666f 7220 6120 696e 206c  rip() for a in l
+0000e480: 696e 6552 6561 645b 2d34 3a5d 5d29 0a0a  ineRead[-4:]])..
+0000e490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4a0: 6c69 6e65 4461 7461 3d70 642e 4461 7461  lineData=pd.Data
+0000e4b0: 4672 616d 6528 6461 745b 315d 2c63 6f6c  Frame(dat[1],col
+0000e4c0: 756d 6e73 3d5b 2769 272c 2775 272c 276c  umns=['i','u','l
+0000e4d0: 272c 2765 272c 2776 272c 274a 272c 2767  ','e','v','J','g
+0000e4e0: 7527 2c27 4575 272c 2741 272c 2742 272c  u','Eu','A','B',
+0000e4f0: 2747 487a 272c 2774 6175 4427 2c27 4a62  'GHz','tauD','Jb
+0000e500: 6163 6b27 2c27 706f 7027 2c27 6c74 6570  ack','pop','ltep
+0000e510: 6f70 272c 2774 6175 4e4c 5445 272c 2774  op','tauNLTE','t
+0000e520: 6175 4c54 4527 2c27 624e 4c54 4527 2c27  auLTE','bNLTE','
+0000e530: 624c 5445 272c 2770 4e4c 5445 272c 2770  bLTE','pNLTE','p
+0000e540: 4c54 4527 2c27 464e 4c54 4527 2c27 464c  LTE','FNLTE','FL
+0000e550: 5445 275d 290a 2020 2020 2020 2020 2020  TE']).          
+0000e560: 2020 2020 2020 6c69 6e65 4461 7461 5b27        lineData['
+0000e570: 676c 6f62 616c 5f75 275d 3d5b 615b 305d  global_u']=[a[0]
+0000e580: 2066 6f72 2061 2069 6e20 6461 745b 325d   for a in dat[2]
+0000e590: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000e5a0: 2020 6c69 6e65 4461 7461 5b27 676c 6f62    lineData['glob
+0000e5b0: 616c 5f6c 275d 3d5b 615b 315d 2066 6f72  al_l']=[a[1] for
+0000e5c0: 2061 2069 6e20 6461 745b 325d 5d0a 2020   a in dat[2]].  
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000e5e0: 6e65 4461 7461 5b27 6c6f 6361 6c5f 7527  neData['local_u'
+0000e5f0: 5d3d 5b61 5b32 5d20 666f 7220 6120 696e  ]=[a[2] for a in
+0000e600: 2064 6174 5b32 5d5d 0a20 2020 2020 2020   dat[2]].       
+0000e610: 2020 2020 2020 2020 206c 696e 6544 6174           lineDat
+0000e620: 615b 276c 6f63 616c 5f6c 275d 3d5b 615b  a['local_l']=[a[
+0000e630: 335d 2066 6f72 2061 2069 6e20 6461 745b  3] for a in dat[
+0000e640: 325d 5d0a 2020 2020 2020 2020 2020 2020  2]].            
+0000e650: 2020 2020 6c65 7644 6174 613d 7064 2e44      levData=pd.D
+0000e660: 6174 6146 7261 6d65 2864 6174 5b30 5d2c  ataFrame(dat[0],
+0000e670: 636f 6c75 6d6e 733d 5b27 6927 2c27 6727  columns=['i','g'
+0000e680: 2c27 4527 2c27 706f 7027 2c27 6c74 6570  ,'E','pop','ltep
+0000e690: 6f70 272c 2765 272c 2776 272c 274a 275d  op','e','v','J']
+0000e6a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e6b0: 2020 7465 6d70 6f2e 6c69 6e65 6461 7461    tempo.linedata
+0000e6c0: 3d6c 696e 6544 6174 610a 2020 2020 2020  =lineData.      
+0000e6d0: 2020 2020 2020 2020 2020 7465 6d70 6f2e            tempo.
+0000e6e0: 6c65 7665 6c64 6174 613d 6c65 7644 6174  leveldata=levDat
+0000e6f0: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+0000e700: 2020 6461 7461 2e61 6464 5f6d 6f64 656c    data.add_model
+0000e710: 2874 656d 706f 290a 2020 2020 7265 7475  (tempo).    retu
+0000e720: 726e 2864 6174 6129 0a0a 0a64 6566 2072  rn(data)...def r
+0000e730: 6561 645f 6f76 6572 6c61 705f 7370 6563  ead_overlap_spec
+0000e740: 7472 6128 7061 7468 3d27 536c 6162 4f76  tra(path='SlabOv
+0000e750: 6572 6c61 702e 6f75 7427 2c76 6572 626f  erlap.out',verbo
+0000e760: 7365 3d54 7275 6529 3a0a 2020 2020 2222  se=True):.    ""
+0000e770: 220a 2020 2020 4675 6e63 7469 6f6e 2074  ".    Function t
+0000e780: 6f20 7265 6164 206f 4420 7072 6f64 696d  o read oD prodim
+0000e790: 6f20 736c 6162 206d 6f64 656c 206f 7574  o slab model out
+0000e7a0: 7075 7420 7769 7468 206c 696e 6520 6f76  put with line ov
+0000e7b0: 6572 6c61 700a 2020 2020 2222 220a 0a20  erlap.    """.. 
+0000e7c0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000e7d0: 2870 6174 682c 6c69 7374 293a 0a20 2020  (path,list):.   
+0000e7e0: 2020 2020 2064 6174 613d 736c 6162 5f64       data=slab_d
+0000e7f0: 6174 6128 290a 2020 2020 2020 2020 6461  ata().        da
+0000e800: 7461 2e64 6972 6563 746f 7279 3d70 6174  ta.directory=pat
+0000e810: 680a 2020 2020 2020 2020 666f 7220 6920  h.        for i 
+0000e820: 696e 2070 6174 683a 0a20 2020 2020 2020  in path:.       
+0000e830: 2020 2020 2072 6461 7461 3d72 6561 645f       rdata=read_
+0000e840: 6f76 6572 6c61 705f 7370 6563 7472 6128  overlap_spectra(
+0000e850: 692c 7665 7262 6f73 653d 7665 7262 6f73  i,verbose=verbos
+0000e860: 6529 0a20 2020 2020 2020 2020 2020 2066  e).            f
+0000e870: 6f72 206a 2069 6e20 7261 6e67 6528 7264  or j in range(rd
+0000e880: 6174 612e 6e6d 6f64 656c 7329 3a0a 2020  ata.nmodels):.  
+0000e890: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000e8a0: 7461 2e61 6464 5f6d 6f64 656c 2872 6461  ta.add_model(rda
+0000e8b0: 7461 2e6d 6f64 656c 735b 6a5d 290a 2020  ta.models[j]).  
+0000e8c0: 2020 2020 2020 7265 7475 726e 2864 6174        return(dat
+0000e8d0: 6129 0a0a 2020 2020 6966 2076 6572 626f  a)..    if verbo
+0000e8e0: 7365 3a20 7072 696e 7428 2252 6561 6469  se: print("Readi
+0000e8f0: 6e67 2073 6c61 6220 6c69 6e65 206f 7665  ng slab line ove
+0000e900: 726c 6170 206d 6f64 656c 206f 7574 7075  rlap model outpu
+0000e910: 7420 6672 6f6d 3a20 222c 7061 7468 290a  t from: ",path).
+0000e920: 2020 2020 6966 2027 2e66 6974 732e 677a      if '.fits.gz
+0000e930: 2720 696e 2070 6174 683a 0a20 2020 2020  ' in path:.     
+0000e940: 2020 2068 6475 6c3d 6669 7473 2e6f 7065     hdul=fits.ope
+0000e950: 6e28 7061 7468 290a 2020 2020 2020 2020  n(path).        
+0000e960: 6461 7461 3d73 6c61 625f 6461 7461 2829  data=slab_data()
+0000e970: 0a20 2020 2020 2020 206e 6d6f 6465 6c73  .        nmodels
+0000e980: 3d68 6475 6c5b 305d 2e68 6561 6465 725b  =hdul[0].header[
+0000e990: 274e 4d4f 4445 4c53 275d 0a20 2020 2020  'NMODELS'].     
+0000e9a0: 2020 2064 6174 612e 6469 7265 6374 6f72     data.director
+0000e9b0: 793d 7061 7468 0a20 2020 2020 2020 2066  y=path.        f
+0000e9c0: 6f72 2069 2069 6e20 7261 6e67 6528 6e6d  or i in range(nm
+0000e9d0: 6f64 656c 7329 3a0a 2020 2020 2020 2020  odels):.        
+0000e9e0: 2020 2020 7465 6d70 6f3d 736c 6162 2829      tempo=slab()
+0000e9f0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+0000ea00: 706f 5f6d 6f64 656c 5f6e 756d 6265 723d  po_model_number=
+0000ea10: 6864 756c 5b69 2b31 5d2e 6865 6164 6572  hdul[i+1].header
+0000ea20: 5b27 4d4f 4445 4c27 5d0a 2020 2020 2020  ['MODEL'].      
+0000ea30: 2020 2020 2020 7465 6d70 6f5f 4e6c 696e        tempo_Nlin
+0000ea40: 653d 6864 756c 5b69 2b31 5d2e 6865 6164  e=hdul[i+1].head
+0000ea50: 6572 5b27 4e4c 494e 4527 5d0a 2020 2020  er['NLINE'].    
+0000ea60: 2020 2020 2020 2020 7465 6d70 6f5f 523d          tempo_R=
+0000ea70: 6864 756c 5b69 2b31 5d2e 6865 6164 6572  hdul[i+1].header
+0000ea80: 5b27 525f 4f56 4c50 275d 0a20 2020 2020  ['R_OVLP'].     
+0000ea90: 2020 2020 2020 2064 6174 7461 3d5b 5d0a         datta=[].
+0000eaa0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000eab0: 6f2e 6f76 6572 6c61 7046 7265 713d 6864  o.overlapFreq=hd
+0000eac0: 756c 5b69 2b31 5d2e 6461 7461 5b3a 2c2d  ul[i+1].data[:,-
+0000ead0: 315d 0a20 2020 2020 2020 2020 2020 2074  1].            t
+0000eae0: 656d 706f 2e6f 7665 726c 6170 4c54 453d  empo.overlapLTE=
+0000eaf0: 6864 756c 5b69 2b31 5d2e 6461 7461 5b3a  hdul[i+1].data[:
+0000eb00: 2c30 5d0a 2020 2020 2020 2020 2020 2020  ,0].            
+0000eb10: 7465 6d70 6f2e 6f76 6572 6c61 7054 6175  tempo.overlapTau
+0000eb20: 4c54 453d 6864 756c 5b69 2b31 5d2e 6461  LTE=hdul[i+1].da
+0000eb30: 7461 5b3a 2c31 5d0a 2020 2020 2020 2020  ta[:,1].        
+0000eb40: 2020 2020 7465 6d70 6f2e 6f76 6572 6c61      tempo.overla
+0000eb50: 704e 4c54 453d 6864 756c 5b69 2b31 5d2e  pNLTE=hdul[i+1].
+0000eb60: 6461 7461 5b3a 2c32 5d0a 2020 2020 2020  data[:,2].      
+0000eb70: 2020 2020 2020 7465 6d70 6f2e 6f76 6572        tempo.over
+0000eb80: 6c61 7054 6175 4e4c 5445 3d68 6475 6c5b  lapTauNLTE=hdul[
+0000eb90: 692b 315d 2e64 6174 615b 3a2c 335d 0a20  i+1].data[:,3]. 
+0000eba0: 2020 2020 2020 2020 2020 2074 656d 706f             tempo
+0000ebb0: 2e6f 7665 726c 6170 523d 7465 6d70 6f5f  .overlapR=tempo_
+0000ebc0: 520a 2020 2020 2020 2020 2020 2020 7465  R.            te
+0000ebd0: 6d70 6f2e 6d6f 6465 6c5f 6e75 6d62 6572  mpo.model_number
+0000ebe0: 3d68 6475 6c5b 692b 315d 2e68 6561 6465  =hdul[i+1].heade
+0000ebf0: 725b 274d 4f44 454c 275d 0a20 2020 2020  r['MODEL'].     
+0000ec00: 2020 2020 2020 2074 656d 706f 2e54 673d         tempo.Tg=
+0000ec10: 6864 756c 5b69 2b31 5d2e 6865 6164 6572  hdul[i+1].header
+0000ec20: 5b27 5447 275d 0a20 2020 2020 2020 2020  ['TG'].         
+0000ec30: 2020 2074 656d 706f 2e54 643d 6864 756c     tempo.Td=hdul
+0000ec40: 5b69 2b31 5d2e 6865 6164 6572 5b27 5444  [i+1].header['TD
+0000ec50: 275d 0a20 2020 2020 2020 2020 2020 2074  '].            t
+0000ec60: 656d 706f 2e76 7475 7262 3d68 6475 6c5b  empo.vturb=hdul[
+0000ec70: 692b 315d 2e68 6561 6465 725b 2756 5455  i+1].header['VTU
+0000ec80: 5242 275d 0a20 2020 2020 2020 2020 2020  RB'].           
+0000ec90: 2074 656d 706f 2e4e 483d 6864 756c 5b69   tempo.NH=hdul[i
+0000eca0: 2b31 5d2e 6865 6164 6572 5b27 4e48 544f  +1].header['NHTO
+0000ecb0: 5427 5d0a 2020 2020 2020 2020 2020 2020  T'].            
+0000ecc0: 6461 7461 2e61 6464 5f6d 6f64 656c 2874  data.add_model(t
+0000ecd0: 656d 706f 290a 2020 2020 2020 2020 2020  empo).          
+0000ece0: 2020 2320 7072 696e 7428 2772 6561 6420    # print('read 
+0000ecf0: 272c 692c 2720 6d6f 6465 6c27 290a 2020  ',i,' model').  
+0000ed00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000ed10: 663d 6f70 656e 2870 6174 6829 0a20 2020  f=open(path).   
+0000ed20: 2020 2020 2064 6174 613d 736c 6162 5f64       data=slab_d
+0000ed30: 6174 6128 290a 2020 2020 2020 2020 6e6d  ata().        nm
+0000ed40: 6f64 656c 733d 696e 7428 662e 7265 6164  odels=int(f.read
+0000ed50: 6c69 6e65 2829 2e73 706c 6974 2829 5b30  line().split()[0
+0000ed60: 5d29 0a20 2020 2020 2020 2064 6174 612e  ]).        data.
+0000ed70: 6469 7265 6374 6f72 793d 7061 7468 0a20  directory=path. 
+0000ed80: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+0000ed90: 7261 6e67 6528 6e6d 6f64 656c 7329 3a0a  range(nmodels):.
+0000eda0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000edb0: 6f3d 736c 6162 2829 0a20 2020 2020 2020  o=slab().       
+0000edc0: 2020 2020 2074 656d 706f 5f6d 6f64 656c       tempo_model
+0000edd0: 5f6e 756d 6265 723d 696e 7428 662e 7265  _number=int(f.re
+0000ede0: 6164 6c69 6e65 2829 2e73 706c 6974 2829  adline().split()
+0000edf0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+0000ee00: 2074 656d 706f 5f4e 6c69 6e65 3d69 6e74   tempo_Nline=int
+0000ee10: 2866 2e72 6561 646c 696e 6528 292e 7370  (f.readline().sp
+0000ee20: 6c69 7428 295b 305d 290a 2020 2020 2020  lit()[0]).      
+0000ee30: 2020 2020 2020 7465 6d70 6f5f 523d 666c        tempo_R=fl
+0000ee40: 6f61 7428 662e 7265 6164 6c69 6e65 2829  oat(f.readline()
+0000ee50: 2e73 706c 6974 2829 5b30 5d29 0a20 2020  .split()[0]).   
+0000ee60: 2020 2020 2020 2020 2064 6174 7461 3d5b           datta=[
+0000ee70: 5d0a 2020 2020 2020 2020 2020 2020 6c69  ].            li
+0000ee80: 6e65 733d 662e 7265 6164 6c69 6e65 2829  nes=f.readline()
+0000ee90: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000eea0: 206a 2069 6e20 7261 6e67 6528 7465 6d70   j in range(temp
+0000eeb0: 6f5f 4e6c 696e 6529 3a0a 2020 2020 2020  o_Nline):.      
+0000eec0: 2020 2020 2020 2020 2020 6c69 6e65 733d            lines=
+0000eed0: 662e 7265 6164 6c69 6e65 2829 0a20 2020  f.readline().   
+0000eee0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+0000eef0: 7461 2e61 7070 656e 6428 6e70 2e61 7272  ta.append(np.arr
+0000ef00: 6179 286c 696e 6573 2e73 706c 6974 2829  ay(lines.split()
+0000ef10: 2c64 7479 7065 3d66 6c6f 6174 2929 0a20  ,dtype=float)). 
+0000ef20: 2020 2020 2020 2020 2020 2064 6174 7461             datta
+0000ef30: 3d6e 702e 6172 7261 7928 6461 7474 6129  =np.array(datta)
+0000ef40: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+0000ef50: 706f 2e6f 7665 726c 6170 4672 6571 3d64  po.overlapFreq=d
+0000ef60: 6174 7461 5b3a 2c30 5d0a 2020 2020 2020  atta[:,0].      
+0000ef70: 2020 2020 2020 7465 6d70 6f2e 6f76 6572        tempo.over
+0000ef80: 6c61 704c 5445 3d64 6174 7461 5b3a 2c31  lapLTE=datta[:,1
+0000ef90: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
+0000efa0: 6d70 6f2e 6f76 6572 6c61 7054 6175 4c54  mpo.overlapTauLT
+0000efb0: 453d 6461 7474 615b 3a2c 325d 0a20 2020  E=datta[:,2].   
+0000efc0: 2020 2020 2020 2020 2074 656d 706f 2e6f           tempo.o
+0000efd0: 7665 726c 6170 4e4c 5445 3d64 6174 7461  verlapNLTE=datta
+0000efe0: 5b3a 2c33 5d0a 2020 2020 2020 2020 2020  [:,3].          
+0000eff0: 2020 7465 6d70 6f2e 6f76 6572 6c61 7054    tempo.overlapT
+0000f000: 6175 4e4c 5445 3d64 6174 7461 5b3a 2c34  auNLTE=datta[:,4
+0000f010: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
+0000f020: 6d70 6f2e 6f76 6572 6c61 7052 3d74 656d  mpo.overlapR=tem
+0000f030: 706f 5f52 0a20 2020 2020 2020 2020 2020  po_R.           
+0000f040: 2064 6174 612e 6164 645f 6d6f 6465 6c28   data.add_model(
+0000f050: 7465 6d70 6f29 0a20 2020 2020 2020 2020  tempo).         
+0000f060: 2020 206c 696e 6573 3d66 2e72 6561 646c     lines=f.readl
+0000f070: 696e 6528 290a 2020 2020 2020 2020 2020  ine().          
+0000f080: 2020 2320 7072 696e 7428 2772 6561 6420    # print('read 
+0000f090: 272c 692c 2720 6d6f 6465 6c27 290a 0a20  ',i,' model').. 
+0000f0a0: 2020 2072 6574 7572 6e28 6461 7461 290a     return(data).
+0000f0b0: 0a0a 6465 6620 7370 6563 436f 6e76 6f6c  ..def specConvol
+0000f0c0: 7665 286c 696e 6553 7472 656e 6774 6873  ve(lineStrengths
+0000f0d0: 2c6c 696e 6546 7265 712c 6672 6571 5f62  ,lineFreq,freq_b
+0000f0e0: 696e 733d 4e6f 6e65 2c52 3d31 2c6c 616d  ins=None,R=1,lam
+0000f0f0: 6264 615f 303d 312c 6c61 6d62 6461 5f6e  bda_0=1,lambda_n
+0000f100: 3d31 2c76 723d 3133 3030 293a 0a20 2020  =1,vr=1300):.   
+0000f110: 2022 2222 0a20 2020 204e 4f54 2055 5345   """.    NOT USE
+0000f120: 4420 414e 594d 4f52 450a 2020 2020 4675  D ANYMORE.    Fu
+0000f130: 6e63 7469 6f6e 2074 6f20 636f 6e76 6f6c  nction to convol
+0000f140: 7665 206c 696e 6573 2069 6e74 6f20 7370  ve lines into sp
+0000f150: 6563 7472 6120 6279 2073 696d 706c 7920  ectra by simply 
+0000f160: 6269 6e6e 696e 6720 7468 656d 2069 6e74  binning them int
+0000f170: 6f20 6120 7761 7665 6c65 6e67 7468 2067  o a wavelength g
+0000f180: 7269 640a 2020 2020 2222 220a 2020 2020  rid.    """.    
+0000f190: 6750 6572 633d 6c61 6d62 6461 2078 2c6d  gPerc=lambda x,m
+0000f1a0: 2c73 3a20 7365 7266 2828 782d 6d29 2f73  ,s: serf((x-m)/s
+0000f1b0: 292a 302e 352b 302e 350a 2020 2020 6e75  )*0.5+0.5.    nu
+0000f1c0: 5f69 6a3d 6c69 6e65 4672 6571 2a31 6539  _ij=lineFreq*1e9
+0000f1d0: 0a20 2020 2069 6620 6c61 6d62 6461 5f6e  .    if lambda_n
+0000f1e0: 3d3d 6c61 6d62 6461 5f30 3a0a 2020 2020  ==lambda_0:.    
+0000f1f0: 2020 2020 6c61 6d62 6461 5f6e 3d6e 702e      lambda_n=np.
+0000f200: 616d 6178 2863 2f6e 755f 696a 2a31 6536  amax(c/nu_ij*1e6
+0000f210: 292a 320a 2020 2020 6966 2074 7970 6528  )*2.    if type(
+0000f220: 6672 6571 5f62 696e 7329 3d3d 7479 7065  freq_bins)==type
+0000f230: 284e 6f6e 6529 3a0a 2020 2020 2020 2020  (None):.        
+0000f240: 6e75 3d67 656e 6572 6174 655f 6772 6964  nu=generate_grid
+0000f250: 2852 3d52 2c6c 616d 6264 615f 303d 6c61  (R=R,lambda_0=la
+0000f260: 6d62 6461 5f30 2c6c 616d 6264 615f 6e3d  mbda_0,lambda_n=
+0000f270: 6c61 6d62 6461 5f6e 292a 3165 390a 2020  lambda_n)*1e9.  
+0000f280: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000f290: 6672 6571 5f62 696e 733d 6e70 2e63 6f6e  freq_bins=np.con
+0000f2a0: 6361 7465 6e61 7465 2828 6672 6571 5f62  catenate((freq_b
+0000f2b0: 696e 732c 6e70 2e61 7272 6179 285b 2866  ins,np.array([(f
+0000f2c0: 7265 715f 6269 6e73 5b2d 315d 2d66 7265  req_bins[-1]-fre
+0000f2d0: 715f 6269 6e73 5b2d 325d 292b 6672 6571  q_bins[-2])+freq
+0000f2e0: 5f62 696e 735b 2d31 5d5d 2929 290a 2020  _bins[-1]]))).  
+0000f2f0: 2020 2020 2020 6e75 3d66 7265 715f 6269        nu=freq_bi
+0000f300: 6e73 2a31 6539 0a20 2020 206e 755f 696a  ns*1e9.    nu_ij
+0000f310: 5f74 696c 653d 6e70 2e74 696c 6528 6e75  _tile=np.tile(nu
+0000f320: 5f69 6a2c 5b6c 656e 286e 7529 2c31 5d29  _ij,[len(nu),1])
+0000f330: 0a20 2020 206e 755f 7469 6c65 3d6e 702e  .    nu_tile=np.
+0000f340: 7469 6c65 286e 752c 5b6c 656e 286e 755f  tile(nu,[len(nu_
+0000f350: 696a 292c 315d 290a 2020 2020 6c69 6e65  ij),1]).    line
+0000f360: 5374 7265 6e67 7468 735f 7469 6c65 3d6e  Strengths_tile=n
+0000f370: 702e 7469 6c65 286c 696e 6553 7472 656e  p.tile(lineStren
+0000f380: 6774 6873 2c5b 6c65 6e28 6e75 292c 315d  gths,[len(nu),1]
+0000f390: 290a 2020 2020 7065 7263 5f74 696c 653d  ).    perc_tile=
+0000f3a0: 6750 6572 6328 6e75 5f74 696c 652c 6e75  gPerc(nu_tile,nu
+0000f3b0: 5f69 6a5f 7469 6c65 2e54 2c6e 755f 696a  _ij_tile.T,nu_ij
+0000f3c0: 5f74 696c 652e 542f 632a 7672 290a 2020  _tile.T/c*vr).  
+0000f3d0: 2020 783d 7065 7263 5f74 696c 655b 3a2c    x=perc_tile[:,
+0000f3e0: 3a2d 315d 2d70 6572 635f 7469 6c65 5b3a  :-1]-perc_tile[:
+0000f3f0: 2c31 3a5d 0a20 2020 2077 6176 656c 656e  ,1:].    wavelen
+0000f400: 6774 682c 666c 7578 3d63 2f6e 755b 3a2d  gth,flux=c/nu[:-
+0000f410: 315d 2a31 6536 2c6e 702e 7375 6d28 782a  1]*1e6,np.sum(x*
+0000f420: 6c69 6e65 5374 7265 6e67 7468 735f 7469  lineStrengths_ti
+0000f430: 6c65 5b3a 2d31 2c3a 5d2e 542c 6178 6973  le[:-1,:].T,axis
+0000f440: 3d30 292f 286e 755b 3a2d 315d 2d6e 755b  =0)/(nu[:-1]-nu[
+0000f450: 313a 5d29 0a20 2020 2072 6574 7572 6e20  1:]).    return 
+0000f460: 7761 7665 6c65 6e67 7468 2c66 6c75 780a  wavelength,flux.
+0000f470: 0a0a 6465 6620 6765 6e65 7261 6c43 6f6e  ..def generalCon
+0000f480: 766f 6c76 6528 6c69 6e65 5374 7265 6e67  volve(lineStreng
+0000f490: 7468 732c 6c69 6e65 4672 6571 2c52 3d31  ths,lineFreq,R=1
+0000f4a0: 2c6c 616d 6264 615f 303d 312c 6c61 6d62  ,lambda_0=1,lamb
+0000f4b0: 6461 5f6e 3d31 2c52 5f62 6163 6b3d 3165  da_n=1,R_back=1e
+0000f4c0: 3629 3a0a 2020 2020 2222 220a 2020 2020  6):.    """.    
+0000f4d0: 4675 6e63 7469 6f6e 2074 6f20 636f 6e76  Function to conv
+0000f4e0: 6f6c 7665 206c 696e 6520 666c 7578 6573  olve line fluxes
+0000f4f0: 2069 6e74 6f20 6c69 6e65 2073 7065 6374   into line spect
+0000f500: 7261 2062 6173 6564 206f 6e20 6120 7573  ra based on a us
+0000f510: 6572 2064 6566 696e 6564 2073 7065 6374  er defined spect
+0000f520: 7261 6c20 7265 736f 6c76 696e 6720 706f  ral resolving po
+0000f530: 7765 7220 520a 2020 2020 2222 220a 2020  wer R.    """.  
+0000f540: 2020 6966 206c 616d 6264 615f 6e3d 3d6c    if lambda_n==l
+0000f550: 616d 6264 615f 303a 0a20 2020 2020 2020  ambda_0:.       
+0000f560: 206c 616d 6264 615f 6e3d 632f 6e70 2e61   lambda_n=c/np.a
+0000f570: 6d69 6e28 6c69 6e65 4672 6571 292a 3165  min(lineFreq)*1e
+0000f580: 2d33 2a32 0a20 2020 2066 7265 715f 6269  -3*2.    freq_bi
+0000f590: 6e73 3d67 656e 6572 6174 655f 6772 6964  ns=generate_grid
+0000f5a0: 2852 5f62 6163 6b2c 6c61 6d62 6461 5f30  (R_back,lambda_0
+0000f5b0: 2c6c 616d 6264 615f 6e29 0a20 2020 2077  ,lambda_n).    w
+0000f5c0: 6176 655f 6269 6e73 3d63 2f66 7265 715f  ave_bins=c/freq_
+0000f5d0: 6269 6e73 2a31 652d 330a 2020 2020 666c  bins*1e-3.    fl
+0000f5e0: 7578 5f62 696e 733d 7761 7665 5f62 696e  ux_bins=wave_bin
+0000f5f0: 732a 302e 300a 2020 2020 693d 360a 2020  s*0.0.    i=6.  
+0000f600: 2020 533d 6c69 6e65 5374 7265 6e67 7468    S=lineStrength
+0000f610: 730a 2020 2020 463d 6c69 6e65 4672 6571  s.    F=lineFreq
+0000f620: 0a20 2020 2069 6e64 3d6e 702e 6469 6769  .    ind=np.digi
+0000f630: 7469 7a65 2846 2c6e 702e 666c 6970 2866  tize(F,np.flip(f
+0000f640: 7265 715f 6269 6e73 295b 3a2d 315d 290a  req_bins)[:-1]).
+0000f650: 2020 2020 666f 7220 692c 6964 7820 696e      for i,idx in
+0000f660: 2065 6e75 6d65 7261 7465 2869 6e64 293a   enumerate(ind):
+0000f670: 0a20 2020 2020 2020 2066 6c75 785f 6269  .        flux_bi
+0000f680: 6e73 5b69 6478 5d2b 3d53 5b69 5d0a 0a20  ns[idx]+=S[i].. 
+0000f690: 2020 2046 5748 4d3d 525f 6261 636b 2f52     FWHM=R_back/R
+0000f6a0: 2f32 2e33 3535 0a20 2020 2067 3d47 6175  /2.355.    g=Gau
+0000f6b0: 7373 6961 6e31 444b 6572 6e65 6c28 7374  ssian1DKernel(st
+0000f6c0: 6464 6576 3d46 5748 4d2c 6661 6374 6f72  ddev=FWHM,factor
+0000f6d0: 3d37 290a 2020 2020 413d 6170 795f 636f  =7).    A=apy_co
+0000f6e0: 6e76 6f6c 7665 2866 6c75 785f 6269 6e73  nvolve(flux_bins
+0000f6f0: 2c67 290a 2020 2020 413d 415b 313a 5d2f  ,g).    A=A[1:]/
+0000f700: 286e 702e 666c 6970 2866 7265 715f 6269  (np.flip(freq_bi
+0000f710: 6e73 295b 313a 5d2d 6e70 2e66 6c69 7028  ns)[1:]-np.flip(
+0000f720: 6672 6571 5f62 696e 7329 5b3a 2d31 5d29  freq_bins)[:-1])
+0000f730: 2a31 652d 390a 2020 2020 573d 6e70 2e66  *1e-9.    W=np.f
+0000f740: 6c69 7028 7761 7665 5f62 696e 735b 313a  lip(wave_bins[1:
+0000f750: 5d29 0a20 2020 2072 6574 7572 6e20 6e70  ]).    return np
+0000f760: 2e66 6c69 7028 5729 2c6e 702e 666c 6970  .flip(W),np.flip
+0000f770: 2841 290a 0a0a 6465 6620 6765 6e65 7261  (A)...def genera
+0000f780: 7465 5f67 7269 6428 523d 312c 6c61 6d62  te_grid(R=1,lamb
+0000f790: 6461 5f30 3d31 2c6c 616d 6264 615f 6e3d  da_0=1,lambda_n=
+0000f7a0: 312c 7361 6d70 6c69 6e67 3d31 293a 0a20  1,sampling=1):. 
+0000f7b0: 2020 2022 2222 0a20 2020 2047 656e 6572     """.    Gener
+0000f7c0: 6174 6520 6120 7370 6563 7472 616c 2067  ate a spectral g
+0000f7d0: 7269 6420 696e 2047 487a 0a20 2020 2022  rid in GHz.    "
+0000f7e0: 2222 0a20 2020 2064 656c 5f6c 6f67 6c61  "".    del_logla
+0000f7f0: 6d3d 6e70 2e6c 6f67 3130 2831 2e30 2b31  m=np.log10(1.0+1
+0000f800: 2e30 2f52 290a 2020 2020 4e3d 312b 696e  .0/R).    N=1+in
+0000f810: 7428 6e70 2e6c 6f67 3130 286c 616d 6264  t(np.log10(lambd
+0000f820: 615f 6e2f 6c61 6d62 6461 5f30 292f 6465  a_n/lambda_0)/de
+0000f830: 6c5f 6c6f 676c 616d 290a 2020 2020 6d77  l_loglam).    mw
+0000f840: 6c73 6c69 6e65 3d6e 702e 6c6f 6773 7061  lsline=np.logspa
+0000f850: 6365 286e 702e 6c6f 6731 3028 6c61 6d62  ce(np.log10(lamb
+0000f860: 6461 5f30 292c 6e70 2e6c 6f67 3130 286c  da_0),np.log10(l
+0000f870: 616d 6264 615f 6e29 2c69 6e74 284e 2a73  ambda_n),int(N*s
+0000f880: 616d 706c 696e 6729 290a 2020 2020 6e75  ampling)).    nu
+0000f890: 3d63 2f6d 776c 736c 696e 652a 3165 360a  =c/mwlsline*1e6.
+0000f8a0: 2020 2020 7265 7475 726e 286e 752a 3165      return(nu*1e
+0000f8b0: 2d39 290a 0a0a 6465 6620 636f 6e76 6f6c  -9)...def convol
+0000f8c0: 7665 286d 6f64 656c 732c 6672 6571 5f62  ve(models,freq_b
+0000f8d0: 696e 733d 4e6f 6e65 2c52 3d31 2c6c 616d  ins=None,R=1,lam
+0000f8e0: 6264 615f 303d 312c 6c61 6d62 6461 5f6e  bda_0=1,lambda_n
+0000f8f0: 3d31 2c76 723d 3133 3030 2c4e 4c54 453d  =1,vr=1300,NLTE=
+0000f900: 4661 6c73 652c 636f 6e76 5f74 7970 653d  False,conv_type=
+0000f910: 312c 7665 7262 6f73 653d 5472 7565 293a  1,verbose=True):
+0000f920: 0a20 2020 2022 2222 0a20 2020 2053 616d  .    """.    Sam
+0000f930: 6520 6173 202e 636f 6e76 6f6c 7665 2829  e as .convolve()
+0000f940: 206d 6574 686f 640a 2020 2020 2222 220a   method.    """.
+0000f950: 2020 2020 666f 7220 692c 6420 696e 2065      for i,d in e
+0000f960: 6e75 6d65 7261 7465 286d 6f64 656c 7329  numerate(models)
+0000f970: 3a0a 2020 2020 2020 2020 6966 2076 6572  :.        if ver
+0000f980: 626f 7365 3a20 7072 696e 7428 275c 6e5c  bose: print('\n\
+0000f990: 6e4d 6f64 656c 2027 2c69 2b31 290a 2020  nModel ',i+1).  
+0000f9a0: 2020 2020 2020 642e 636f 6e76 6f6c 7665        d.convolve
+0000f9b0: 2866 7265 715f 6269 6e73 3d66 7265 715f  (freq_bins=freq_
+0000f9c0: 6269 6e73 2c52 3d52 2c6c 616d 6264 615f  bins,R=R,lambda_
+0000f9d0: 303d 6c61 6d62 6461 5f30 2c6c 616d 6264  0=lambda_0,lambd
+0000f9e0: 615f 6e3d 6c61 6d62 6461 5f6e 2c76 723d  a_n=lambda_n,vr=
+0000f9f0: 7672 2c4e 4c54 453d 4e4c 5445 2c63 6f6e  vr,NLTE=NLTE,con
+0000fa00: 765f 7479 7065 3d63 6f6e 765f 7479 7065  v_type=conv_type
+0000fa10: 290a 2020 2020 7265 7475 726e 206d 6f64  ).    return mod
+0000fa20: 656c 730a 0a0a 6465 6620 6765 6e65 7261  els...def genera
+0000fa30: 7465 5f73 6c61 625f 6772 6964 2864 6972  te_slab_grid(dir
+0000fa40: 6563 746f 7279 3d27 2e27 2c67 7269 645f  ectory='.',grid_
+0000fa50: 7061 7261 6d65 7465 7273 3d7b 7d2c 636f  parameters={},co
+0000fa60: 6d62 696e 6174 696f 6e3d 4661 6c73 652c  mbination=False,
+0000fa70: 4e74 6f74 3d4e 6f6e 652c 5467 3d4e 6f6e  Ntot=None,Tg=Non
+0000fa80: 652c 6e48 706c 7573 3d4e 6f6e 652c 6e48  e,nHplus=None,nH
+0000fa90: 313d 4e6f 6e65 2c6e 4832 3d4e 6f6e 652c  1=None,nH2=None,
+0000faa0: 6e48 653d 4e6f 6e65 2c6e 656c 6563 3d4e  nHe=None,nelec=N
+0000fab0: 6f6e 652c 5464 3d4e 6f6e 652c 7674 7572  one,Td=None,vtur
+0000fac0: 623d 4e6f 6e65 2c64 7573 745f 746f 5f67  b=None,dust_to_g
+0000fad0: 6173 3d4e 6f6e 652c 525f 6f76 6572 6c61  as=None,R_overla
+0000fae0: 703d 4e6f 6e65 2c6c 696e 655f 6f76 6572  p=None,line_over
+0000faf0: 6c61 703d 4e6f 6e65 2c73 7065 6369 6573  lap=None,species
+0000fb00: 5f6c 6973 743d 7b7d 2c6f 7574 7075 745f  _list={},output_
+0000fb10: 6669 6c65 6e61 6d65 3d27 536c 6162 5265  filename='SlabRe
+0000fb20: 7375 6c74 732e 6f75 7427 2c6f 7665 726c  sults.out',overl
+0000fb30: 6170 5f66 696c 656e 616d 653d 2753 6c61  ap_filename='Sla
+0000fb40: 624f 7665 726c 6170 2e6f 7574 272c 7365  bOverlap.out',se
+0000fb50: 7061 7261 7465 5f6f 705f 6669 6c65 733d  parate_op_files=
+0000fb60: 5472 7565 2c73 6c61 625f 5254 3d54 7275  True,slab_RT=Tru
+0000fb70: 652c 7368 6f72 745f 666f 726d 6174 3d46  e,short_format=F
+0000fb80: 616c 7365 2c6e 6f5f 696e 6469 7669 6475  alse,no_individu
+0000fb90: 616c 5f6c 696e 6573 3d46 616c 7365 2c66  al_lines=False,f
+0000fba0: 6974 735f 6f70 5f66 696c 6573 3d46 616c  its_op_files=Fal
+0000fbb0: 7365 293a 0a20 2020 2022 2222 0a20 2020  se):.    """.   
+0000fbc0: 2046 756e 6374 696f 6e20 746f 2067 656e   Function to gen
+0000fbd0: 6572 6174 6520 536c 6162 496e 7075 742e  erate SlabInput.
+0000fbe0: 696e 2069 6e70 7574 2066 696c 6520 636f  in input file co
+0000fbf0: 6e74 6169 6e69 6e67 2074 6865 2064 6574  ntaining the det
+0000fc00: 6169 6c73 206f 6620 7468 6520 736c 6162  ails of the slab
+0000fc10: 206d 6f64 656c 2067 7269 640a 2020 2020   model grid.    
+0000fc20: 2222 220a 2020 2020 6e6d 6f64 656c 733d  """.    nmodels=
+0000fc30: 310a 2020 2020 636f 6d62 696e 6174 696f  1.    combinatio
+0000fc40: 6e3d 4661 6c73 650a 2020 2020 6966 206c  n=False.    if l
+0000fc50: 656e 2867 7269 645f 7061 7261 6d65 7465  en(grid_paramete
+0000fc60: 7273 293e 303a 0a20 2020 2020 2020 2069  rs)>0:.        i
+0000fc70: 6620 6e6f 7420 636f 6d62 696e 6174 696f  f not combinatio
+0000fc80: 6e3a 0a20 2020 2020 2020 2020 2020 206e  n:.            n
+0000fc90: 6d6f 6465 6c73 3d6c 656e 2867 7269 645f  models=len(grid_
+0000fca0: 7061 7261 6d65 7465 7273 5b6c 6973 7428  parameters[list(
+0000fcb0: 6772 6964 5f70 6172 616d 6574 6572 732e  grid_parameters.
+0000fcc0: 6b65 7973 2829 295b 305d 5d29 0a20 2020  keys())[0]]).   
+0000fcd0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000fce0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+0000fcf0: 7261 6e67 6528 6c65 6e28 6772 6964 5f70  range(len(grid_p
+0000fd00: 6172 616d 6574 6572 7329 293a 0a20 2020  arameters)):.   
+0000fd10: 2020 2020 2020 2020 2020 2020 206e 6d6f               nmo
+0000fd20: 6465 6c73 2a3d 6c65 6e28 6772 6964 5f70  dels*=len(grid_p
+0000fd30: 6172 616d 6574 6572 735b 6c69 7374 2867  arameters[list(g
+0000fd40: 7269 645f 7061 7261 6d65 7465 7273 2e6b  rid_parameters.k
+0000fd50: 6579 7328 2929 5b69 5d5d 290a 0a20 2020  eys())[i]])..   
+0000fd60: 204e 746f 745f 6c69 7374 3d6e 702e 6f6e   Ntot_list=np.on
+0000fd70: 6573 2828 6e6d 6f64 656c 7329 290a 2020  es((nmodels)).  
+0000fd80: 2020 5467 5f6c 6973 743d 6e70 2e6f 6e65    Tg_list=np.one
+0000fd90: 7328 286e 6d6f 6465 6c73 2929 0a20 2020  s((nmodels)).   
+0000fda0: 206e 4870 6c75 735f 6c69 7374 3d6e 702e   nHplus_list=np.
+0000fdb0: 6f6e 6573 2828 6e6d 6f64 656c 7329 290a  ones((nmodels)).
+0000fdc0: 2020 2020 6e48 315f 6c69 7374 3d6e 702e      nH1_list=np.
+0000fdd0: 6f6e 6573 2828 6e6d 6f64 656c 7329 290a  ones((nmodels)).
+0000fde0: 2020 2020 6e48 325f 6c69 7374 3d6e 702e      nH2_list=np.
+0000fdf0: 6f6e 6573 2828 6e6d 6f64 656c 7329 290a  ones((nmodels)).
+0000fe00: 2020 2020 6e48 655f 6c69 7374 3d6e 702e      nHe_list=np.
+0000fe10: 6f6e 6573 2828 6e6d 6f64 656c 7329 290a  ones((nmodels)).
+0000fe20: 2020 2020 6e65 6c65 635f 6c69 7374 3d6e      nelec_list=n
+0000fe30: 702e 6f6e 6573 2828 6e6d 6f64 656c 7329  p.ones((nmodels)
+0000fe40: 290a 2020 2020 5464 5f6c 6973 743d 6e70  ).    Td_list=np
+0000fe50: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
+0000fe60: 0a20 2020 2076 7475 7262 5f6c 6973 743d  .    vturb_list=
+0000fe70: 6e70 2e6f 6e65 7328 286e 6d6f 6465 6c73  np.ones((nmodels
+0000fe80: 2929 0a20 2020 2064 7573 745f 746f 5f67  )).    dust_to_g
+0000fe90: 6173 5f6c 6973 743d 6e70 2e6f 6e65 7328  as_list=np.ones(
+0000fea0: 286e 6d6f 6465 6c73 2929 0a20 2020 2052  (nmodels)).    R
+0000feb0: 5f6f 7665 726c 6170 5f6c 6973 743d 6e70  _overlap_list=np
+0000fec0: 2e6f 6e65 7328 286e 6d6f 6465 6c73 2929  .ones((nmodels))
+0000fed0: 0a20 2020 206c 696e 655f 6f76 6572 6c61  .    line_overla
+0000fee0: 705f 6c69 7374 3d6e 702e 6f6e 6573 2828  p_list=np.ones((
+0000fef0: 6e6d 6f64 656c 732c 3229 290a 2020 2020  nmodels,2)).    
+0000ff00: 6966 206c 656e 2873 7065 6369 6573 5f6c  if len(species_l
+0000ff10: 6973 7429 3c31 3a20 7261 6973 6520 5661  ist)<1: raise Va
+0000ff20: 6c75 6545 7272 6f72 2827 5468 6520 7370  lueError('The sp
+0000ff30: 6563 6965 735f 6c69 7374 2063 616e 6e6f  ecies_list canno
+0000ff40: 7420 6265 2065 6d70 7479 2729 0a0a 2020  t be empty')..  
+0000ff50: 2020 6966 206e 6f74 2063 6f6d 6269 6e61    if not combina
+0000ff60: 7469 6f6e 3a0a 2020 2020 2020 2020 666f  tion:.        fo
+0000ff70: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+0000ff80: 2867 7269 645f 7061 7261 6d65 7465 7273  (grid_parameters
+0000ff90: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000ffa0: 6966 206c 6973 7428 6772 6964 5f70 6172  if list(grid_par
+0000ffb0: 616d 6574 6572 732e 6b65 7973 2829 295b  ameters.keys())[
+0000ffc0: 695d 3d3d 274e 746f 7427 3a0a 2020 2020  i]=='Ntot':.    
+0000ffd0: 2020 2020 2020 2020 2020 2020 4e74 6f74              Ntot
+0000ffe0: 5f6c 6973 742a 3d67 7269 645f 7061 7261  _list*=grid_para
+0000fff0: 6d65 7465 7273 5b27 4e74 6f74 275d 0a20  meters['Ntot']. 
+00010000: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00010010: 6c69 7374 2867 7269 645f 7061 7261 6d65  list(grid_parame
+00010020: 7465 7273 2e6b 6579 7328 2929 5b69 5d3d  ters.keys())[i]=
+00010030: 3d27 5467 273a 0a20 2020 2020 2020 2020  ='Tg':.         
+00010040: 2020 2020 2020 2054 675f 6c69 7374 2a3d         Tg_list*=
+00010050: 6772 6964 5f70 6172 616d 6574 6572 735b  grid_parameters[
+00010060: 2754 6727 5d0a 2020 2020 2020 2020 2020  'Tg'].          
+00010070: 2020 656c 6966 206c 6973 7428 6772 6964    elif list(grid
+00010080: 5f70 6172 616d 6574 6572 732e 6b65 7973  _parameters.keys
+00010090: 2829 295b 695d 3d3d 276e 4870 6c75 7327  ())[i]=='nHplus'
+000100a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000100b0: 2020 6e48 706c 7573 5f6c 6973 742a 3d67    nHplus_list*=g
+000100c0: 7269 645f 7061 7261 6d65 7465 7273 5b27  rid_parameters['
+000100d0: 6e48 706c 7573 275d 0a20 2020 2020 2020  nHplus'].       
+000100e0: 2020 2020 2065 6c69 6620 6c69 7374 2867       elif list(g
+000100f0: 7269 645f 7061 7261 6d65 7465 7273 2e6b  rid_parameters.k
+00010100: 6579 7328 2929 5b69 5d3d 3d27 6e48 3127  eys())[i]=='nH1'
+00010110: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010120: 2020 6e48 315f 6c69 7374 2a3d 6772 6964    nH1_list*=grid
+00010130: 5f70 6172 616d 6574 6572 735b 276e 4831  _parameters['nH1
+00010140: 275d 0a20 2020 2020 2020 2020 2020 2065  '].            e
+00010150: 6c69 6620 6c69 7374 2867 7269 645f 7061  lif list(grid_pa
+00010160: 7261 6d65 7465 7273 2e6b 6579 7328 2929  rameters.keys())
+00010170: 5b69 5d3d 3d27 6e48 3227 3a0a 2020 2020  [i]=='nH2':.    
+00010180: 2020 2020 2020 2020 2020 2020 6e48 325f              nH2_
+00010190: 6c69 7374 2a3d 6772 6964 5f70 6172 616d  list*=grid_param
+000101a0: 6574 6572 735b 276e 4832 275d 0a20 2020  eters['nH2'].   
+000101b0: 2020 2020 2020 2020 2065 6c69 6620 6c69           elif li
+000101c0: 7374 2867 7269 645f 7061 7261 6d65 7465  st(grid_paramete
+000101d0: 7273 2e6b 6579 7328 2929 5b69 5d3d 3d27  rs.keys())[i]=='
+000101e0: 6e48 6527 3a0a 2020 2020 2020 2020 2020  nHe':.          
+000101f0: 2020 2020 2020 6e48 655f 6c69 7374 2a3d        nHe_list*=
+00010200: 6772 6964 5f70 6172 616d 6574 6572 735b  grid_parameters[
+00010210: 276e 4865 275d 0a20 2020 2020 2020 2020  'nHe'].         
+00010220: 2020 2065 6c69 6620 6c69 7374 2867 7269     elif list(gri
+00010230: 645f 7061 7261 6d65 7465 7273 2e6b 6579  d_parameters.key
+00010240: 7328 2929 5b69 5d3d 3d27 6e65 6c65 6327  s())[i]=='nelec'
+00010250: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010260: 2020 6e65 6c65 635f 6c69 7374 2a3d 6772    nelec_list*=gr
+00010270: 6964 5f70 6172 616d 6574 6572 735b 276e  id_parameters['n
+00010280: 656c 6563 275d 0a20 2020 2020 2020 2020  elec'].         
+00010290: 2020 2065 6c69 6620 6c69 7374 2867 7269     elif list(gri
+000102a0: 645f 7061 7261 6d65 7465 7273 2e6b 6579  d_parameters.key
+000102b0: 7328 2929 5b69 5d3d 3d27 5464 273a 0a20  s())[i]=='Td':. 
+000102c0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+000102d0: 645f 6c69 7374 2a3d 6772 6964 5f70 6172  d_list*=grid_par
+000102e0: 616d 6574 6572 735b 2754 6427 5d0a 2020  ameters['Td'].  
+000102f0: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
+00010300: 6973 7428 6772 6964 5f70 6172 616d 6574  ist(grid_paramet
+00010310: 6572 732e 6b65 7973 2829 295b 695d 3d3d  ers.keys())[i]==
+00010320: 2776 7475 7262 273a 0a20 2020 2020 2020  'vturb':.       
+00010330: 2020 2020 2020 2020 2076 7475 7262 5f6c           vturb_l
+00010340: 6973 742a 3d67 7269 645f 7061 7261 6d65  ist*=grid_parame
+00010350: 7465 7273 5b27 7674 7572 6227 5d0a 2020  ters['vturb'].  
+00010360: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
+00010370: 6973 7428 6772 6964 5f70 6172 616d 6574  ist(grid_paramet
+00010380: 6572 732e 6b65 7973 2829 295b 695d 3d3d  ers.keys())[i]==
+00010390: 2764 7573 745f 746f 5f67 6173 273a 0a20  'dust_to_gas':. 
+000103a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000103b0: 7573 745f 746f 5f67 6173 5f6c 6973 742a  ust_to_gas_list*
+000103c0: 3d67 7269 645f 7061 7261 6d65 7465 7273  =grid_parameters
+000103d0: 5b27 6475 7374 5f74 6f5f 6761 7327 5d0a  ['dust_to_gas'].
+000103e0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000103f0: 206c 6973 7428 6772 6964 5f70 6172 616d   list(grid_param
+00010400: 6574 6572 732e 6b65 7973 2829 295b 695d  eters.keys())[i]
+00010410: 3d3d 2752 5f6f 7665 726c 6170 273a 0a20  =='R_overlap':. 
+00010420: 2020 2020 2020 2020 2020 2020 2020 2052                 R
+00010430: 5f6f 7665 726c 6170 5f6c 6973 742a 3d67  _overlap_list*=g
+00010440: 7269 645f 7061 7261 6d65 7465 7273 5b27  rid_parameters['
+00010450: 525f 6f76 6572 6c61 7027 5d0a 2020 2020  R_overlap'].    
+00010460: 2020 2020 2020 2020 656c 6966 206c 6973          elif lis
+00010470: 7428 6772 6964 5f70 6172 616d 6574 6572  t(grid_parameter
+00010480: 732e 6b65 7973 2829 295b 695d 3d3d 276c  s.keys())[i]=='l
+00010490: 696e 655f 6f76 6572 6c61 7027 3a0a 2020  ine_overlap':.  
+000104a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000104b0: 7220 6a20 696e 2072 616e 6765 286c 656e  r j in range(len
+000104c0: 2867 7269 645f 7061 7261 6d65 7465 7273  (grid_parameters
+000104d0: 5b27 6c69 6e65 5f6f 7665 726c 6170 275d  ['line_overlap']
+000104e0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+000104f0: 2020 2020 2020 2020 6c69 6e65 5f6f 7665          line_ove
+00010500: 726c 6170 5f6c 6973 745b 6a2c 3a5d 3d6e  rlap_list[j,:]=n
+00010510: 702e 6172 7261 7928 6772 6964 5f70 6172  p.array(grid_par
+00010520: 616d 6574 6572 735b 276c 696e 655f 6f76  ameters['line_ov
+00010530: 6572 6c61 7027 5d5b 6a5d 290a 2020 2020  erlap'][j]).    
+00010540: 2020 2020 2020 2020 656c 7365 3a20 7261          else: ra
+00010550: 6973 6520 4b65 7945 7272 6f72 2866 2755  ise KeyError(f'U
+00010560: 6e69 6465 6e74 6966 6965 6420 6772 6964  nidentified grid
+00010570: 2070 6172 616d 6574 6572 207b 6c69 7374   parameter {list
+00010580: 2867 7269 645f 7061 7261 6d65 7465 7273  (grid_parameters
+00010590: 2e6b 6579 7328 2929 5b69 5d7d 2729 0a20  .keys())[i]}'). 
+000105a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000105b0: 2072 6169 7365 204b 6579 4572 726f 7228   raise KeyError(
+000105c0: 2743 6f6d 6269 6e61 7469 6f6e 2069 7320  'Combination is 
+000105d0: 7374 696c 6c20 6e6f 7420 7375 7070 6f72  still not suppor
+000105e0: 7465 6427 290a 0a20 2020 2069 6620 6e70  ted')..    if np
+000105f0: 2e73 756d 284e 746f 745f 6c69 7374 293d  .sum(Ntot_list)=
+00010600: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
+00010610: 2020 6966 206e 6f74 2028 4e74 6f74 2020    if not (Ntot  
+00010620: 2020 2020 2020 6973 204e 6f6e 6529 3a0a        is None):.
+00010630: 2020 2020 2020 2020 2020 2020 4e74 6f74              Ntot
+00010640: 5f6c 6973 742a 3d4e 746f 740a 2020 2020  _list*=Ntot.    
+00010650: 2020 2020 2320 656c 7365 3a0a 2020 2020      # else:.    
+00010660: 2020 2020 2320 2020 2020 4e74 6f74 5f6c      #     Ntot_l
+00010670: 6973 742a 3d31 6531 350a 2020 2020 6966  ist*=1e15.    if
+00010680: 206e 702e 7375 6d28 5467 5f6c 6973 7429   np.sum(Tg_list)
+00010690: 3d3d 6e6d 6f64 656c 733a 0a20 2020 2020  ==nmodels:.     
+000106a0: 2020 2069 6620 6e6f 7420 2854 6720 2020     if not (Tg   
+000106b0: 2020 2020 2020 2069 7320 4e6f 6e65 293a         is None):
+000106c0: 0a20 2020 2020 2020 2020 2020 2054 675f  .            Tg_
+000106d0: 6c69 7374 2a3d 5467 0a20 2020 2020 2020  list*=Tg.       
+000106e0: 2023 2065 6c73 653a 0a20 2020 2020 2020   # else:.       
+000106f0: 2023 2020 2020 2054 675f 6c69 7374 2a3d   #     Tg_list*=
+00010700: 3130 300a 2020 2020 6966 206e 702e 7375  100.    if np.su
+00010710: 6d28 6e48 706c 7573 5f6c 6973 7429 3d3d  m(nHplus_list)==
+00010720: 6e6d 6f64 656c 733a 0a20 2020 2020 2020  nmodels:.       
+00010730: 2069 6620 6e6f 7420 286e 4870 6c75 7320   if not (nHplus 
+00010740: 2020 2020 2069 7320 4e6f 6e65 293a 0a20       is None):. 
+00010750: 2020 2020 2020 2020 2020 206e 4870 6c75             nHplu
+00010760: 735f 6c69 7374 2a3d 6e48 706c 7573 0a20  s_list*=nHplus. 
+00010770: 2020 2020 2020 2023 2065 6c73 653a 0a20         # else:. 
+00010780: 2020 2020 2020 2023 2020 2020 206e 4870         #     nHp
+00010790: 6c75 735f 6c69 7374 2a3d 3165 310a 2020  lus_list*=1e1.  
+000107a0: 2020 6966 206e 702e 7375 6d28 6e48 315f    if np.sum(nH1_
+000107b0: 6c69 7374 293d 3d6e 6d6f 6465 6c73 3a0a  list)==nmodels:.
+000107c0: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
+000107d0: 6e48 3120 2020 2020 2020 2020 6973 204e  nH1         is N
+000107e0: 6f6e 6529 3a0a 2020 2020 2020 2020 2020  one):.          
+000107f0: 2020 6e48 315f 6c69 7374 2a3d 6e48 310a    nH1_list*=nH1.
+00010800: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
+00010810: 2020 2020 2020 2020 2320 2020 2020 6e48          #     nH
+00010820: 315f 6c69 7374 2a3d 3165 3132 0a20 2020  1_list*=1e12.   
+00010830: 2069 6620 6e70 2e73 756d 286e 4832 5f6c   if np.sum(nH2_l
+00010840: 6973 7429 3d3d 6e6d 6f64 656c 733a 0a20  ist)==nmodels:. 
+00010850: 2020 2020 2020 2069 6620 6e6f 7420 286e         if not (n
+00010860: 4832 2020 2020 2020 2020 2069 7320 4e6f  H2         is No
+00010870: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
+00010880: 206e 4832 5f6c 6973 742a 3d6e 4832 0a20   nH2_list*=nH2. 
+00010890: 2020 2020 2020 2023 2065 6c73 653a 0a20         # else:. 
+000108a0: 2020 2020 2020 2023 2020 2020 206e 4832         #     nH2
+000108b0: 5f6c 6973 742a 3d31 6531 320a 2020 2020  _list*=1e12.    
+000108c0: 6966 206e 702e 7375 6d28 6e48 655f 6c69  if np.sum(nHe_li
+000108d0: 7374 293d 3d6e 6d6f 6465 6c73 3a0a 2020  st)==nmodels:.  
+000108e0: 2020 2020 2020 6966 206e 6f74 2028 6e48        if not (nH
+000108f0: 6520 2020 2020 2020 2020 6973 204e 6f6e  e         is Non
+00010900: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00010910: 6e48 655f 6c69 7374 2a3d 6e48 650a 2020  nHe_list*=nHe.  
+00010920: 2020 2020 2020 2320 656c 7365 3a0a 2020        # else:.  
+00010930: 2020 2020 2020 2320 2020 2020 6e48 655f        #     nHe_
+00010940: 6c69 7374 2a3d 3165 3131 0a20 2020 2069  list*=1e11.    i
+00010950: 6620 6e70 2e73 756d 286e 656c 6563 5f6c  f np.sum(nelec_l
+00010960: 6973 7429 3d3d 6e6d 6f64 656c 733a 0a20  ist)==nmodels:. 
+00010970: 2020 2020 2020 2069 6620 6e6f 7420 286e         if not (n
+00010980: 656c 6563 2020 2020 2020 2069 7320 4e6f  elec       is No
+00010990: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
+000109a0: 206e 656c 6563 5f6c 6973 742a 3d6e 656c   nelec_list*=nel
+000109b0: 6563 0a20 2020 2020 2020 2023 2065 6c73  ec.        # els
+000109c0: 653a 0a20 2020 2020 2020 2023 2020 2020  e:.        #    
+000109d0: 206e 656c 6563 5f6c 6973 742a 3d31 6538   nelec_list*=1e8
+000109e0: 0a20 2020 2069 6620 6e70 2e73 756d 2854  .    if np.sum(T
+000109f0: 645f 6c69 7374 293d 3d6e 6d6f 6465 6c73  d_list)==nmodels
+00010a00: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+00010a10: 2028 5464 2020 2020 2020 2020 2020 6973   (Td          is
+00010a20: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00010a30: 2020 2020 5464 5f6c 6973 742a 3d54 640a      Td_list*=Td.
+00010a40: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
+00010a50: 2020 2020 2020 2020 2320 2020 2020 5464          #     Td
+00010a60: 5f6c 6973 742a 3d31 300a 2020 2020 6966  _list*=10.    if
+00010a70: 206e 702e 7375 6d28 7674 7572 625f 6c69   np.sum(vturb_li
+00010a80: 7374 293d 3d6e 6d6f 6465 6c73 3a0a 2020  st)==nmodels:.  
+00010a90: 2020 2020 2020 6966 206e 6f74 2028 7674        if not (vt
+00010aa0: 7572 6220 2020 2020 2020 6973 204e 6f6e  urb       is Non
+00010ab0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00010ac0: 7674 7572 625f 6c69 7374 2a3d 7674 7572  vturb_list*=vtur
+00010ad0: 620a 2020 2020 2020 2020 2320 656c 7365  b.        # else
+00010ae0: 3a0a 2020 2020 2020 2020 2320 2020 2020  :.        #     
+00010af0: 7674 7572 625f 6c69 7374 2a3d 312e 340a  vturb_list*=1.4.
+00010b00: 2020 2020 6966 206e 702e 7375 6d28 6475      if np.sum(du
+00010b10: 7374 5f74 6f5f 6761 735f 6c69 7374 293d  st_to_gas_list)=
+00010b20: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
+00010b30: 2020 6966 206e 6f74 2028 6475 7374 5f74    if not (dust_t
+00010b40: 6f5f 6761 7320 6973 204e 6f6e 6529 3a0a  o_gas is None):.
+00010b50: 2020 2020 2020 2020 2020 2020 6475 7374              dust
+00010b60: 5f74 6f5f 6761 735f 6c69 7374 2a3d 6475  _to_gas_list*=du
+00010b70: 7374 5f74 6f5f 6761 730a 2020 2020 2020  st_to_gas.      
+00010b80: 2020 2320 656c 7365 3a0a 2020 2020 2020    # else:.      
+00010b90: 2020 2320 2020 2020 6475 7374 5f74 6f5f    #     dust_to_
+00010ba0: 6761 735f 6c69 7374 2a3d 3165 2d32 310a  gas_list*=1e-21.
+00010bb0: 2020 2020 6966 206e 702e 7375 6d28 525f      if np.sum(R_
+00010bc0: 6f76 6572 6c61 705f 6c69 7374 293d 3d6e  overlap_list)==n
+00010bd0: 6d6f 6465 6c73 3a0a 2020 2020 2020 2020  models:.        
+00010be0: 6966 206e 6f74 2028 525f 6f76 6572 6c61  if not (R_overla
+00010bf0: 7020 6973 204e 6f6e 6529 3a0a 2020 2020  p is None):.    
+00010c00: 2020 2020 2020 2020 525f 6f76 6572 6c61          R_overla
+00010c10: 705f 6c69 7374 2a3d 525f 6f76 6572 6c61  p_list*=R_overla
+00010c20: 700a 2020 2020 2020 2020 2320 656c 7365  p.        # else
+00010c30: 3a0a 2020 2020 2020 2020 2320 2020 2020  :.        #     
+00010c40: 525f 6f76 6572 6c61 705f 6c69 7374 2a3d  R_overlap_list*=
+00010c50: 3165 350a 2020 2020 6966 206e 702e 7375  1e5.    if np.su
+00010c60: 6d28 6c69 6e65 5f6f 7665 726c 6170 5f6c  m(line_overlap_l
+00010c70: 6973 7429 3d3d 322a 6e6d 6f64 656c 733a  ist)==2*nmodels:
+00010c80: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00010c90: 286c 696e 655f 6f76 6572 6c61 7020 6973  (line_overlap is
+00010ca0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00010cb0: 2020 2020 6c69 6e65 5f6f 7665 726c 6170      line_overlap
+00010cc0: 5f6c 6973 742a 3d6e 702e 6172 7261 7928  _list*=np.array(
+00010cd0: 6c69 6e65 5f6f 7665 726c 6170 290a 2020  line_overlap).  
+00010ce0: 2020 2020 2020 2320 656c 7365 3a0a 2020        # else:.  
+00010cf0: 2020 2020 2020 2320 2020 2020 6c69 6e65        #     line
+00010d00: 5f6f 7665 726c 6170 5f6c 6973 742a 3d6e  _overlap_list*=n
+00010d10: 702e 6172 7261 7928 2834 2c33 3029 290a  p.array((4,30)).
+00010d20: 0a20 2020 206f 732e 7379 7374 656d 2866  .    os.system(f
+00010d30: 2774 6f75 6368 207b 6469 7265 6374 6f72  'touch {director
+00010d40: 792b 222f 536c 6162 496e 7075 742e 696e  y+"/SlabInput.in
+00010d50: 227d 2729 0a20 2020 2066 3d6f 7065 6e28  "}').    f=open(
+00010d60: 6469 7265 6374 6f72 792b 272f 536c 6162  directory+'/Slab
+00010d70: 496e 7075 742e 696e 272c 2777 2729 0a20  Input.in','w'). 
+00010d80: 2020 2066 2e77 7269 7465 2822 2a2a 2a2a     f.write("****
+00010d90: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010da0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010db0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00010dc0: 2a2a 2a2a 2a2a 2a5c 6e22 290a 2020 2020  *******\n").    
+00010dd0: 662e 7772 6974 6528 222a 2a2a 2049 6e70  f.write("*** Inp
+00010de0: 7574 2066 696c 6520 666f 7220 736c 6162  ut file for slab
+00010df0: 2065 7363 6170 6520 7072 6f62 6162 696c   escape probabil
+00010e00: 6974 7920 7769 7468 2050 726f 4469 4d6f  ity with ProDiMo
+00010e10: 202a 2a2a 5c6e 2229 0a20 2020 2066 2e77   ***\n").    f.w
+00010e20: 7269 7465 2822 2a2a 2a2a 2a2a 2a2a 2a2a  rite("**********
+00010e30: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 00010e40: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 00010e50: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010e60: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a5c 6e22  *************\n"
-00010e70: 290a 2020 2020 662e 7772 6974 6528 222a  ).    f.write("*
-00010e80: 2a2a 2049 6e70 7574 2066 696c 6520 666f  ** Input file fo
-00010e90: 7220 736c 6162 2065 7363 6170 6520 7072  r slab escape pr
-00010ea0: 6f62 6162 696c 6974 7920 7769 7468 2050  obability with P
-00010eb0: 726f 4469 4d6f 202a 2a2a 5c6e 2229 0a20  roDiMo ***\n"). 
-00010ec0: 2020 2066 2e77 7269 7465 2822 2a2a 2a2a     f.write("****
-00010ed0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010ee0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010ef0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00010f00: 2a2a 2a2a 2a2a 2a5c 6e22 290a 2020 2020  *******\n").    
-00010f10: 662e 7772 6974 6528 222a 2a2a 206e 6d6f  f.write("*** nmo
-00010f20: 6465 6c73 2073 686f 756c 6420 666f 6c6c  dels should foll
-00010f30: 6f77 206f 7574 7075 745f 6669 6c65 6e61  ow output_filena
-00010f40: 6d65 202a 2a2a 5c6e 2229 0a20 2020 2066  me ***\n").    f
-00010f50: 2e77 7269 7465 2866 277b 6f75 7470 7574  .write(f'{output
-00010f60: 5f66 696c 656e 616d 657d 2021 206f 7574  _filename} ! out
-00010f70: 7075 745f 6669 6c65 6e61 6d65 5c6e 2729  put_filename\n')
-00010f80: 0a20 2020 2066 2e77 7269 7465 2866 277b  .    f.write(f'{
-00010f90: 6f76 6572 6c61 705f 6669 6c65 6e61 6d65  overlap_filename
-00010fa0: 7d20 2120 6f76 6572 6c61 705f 6669 6c65  } ! overlap_file
-00010fb0: 6e61 6d65 5c6e 2729 0a20 2020 2069 6620  name\n').    if 
-00010fc0: 7365 7061 7261 7465 5f6f 705f 6669 6c65  separate_op_file
-00010fd0: 733a 0a20 2020 2020 2020 2066 2e77 7269  s:.        f.wri
-00010fe0: 7465 2827 2e74 7275 652e 2020 2020 2120  te('.true.    ! 
-00010ff0: 7365 7061 7261 7465 5f6f 705f 6669 6c65  separate_op_file
-00011000: 735c 6e27 290a 2020 2020 656c 7365 3a0a  s\n').    else:.
-00011010: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00011020: 272e 6661 6c73 652e 2020 2021 2073 6570  '.false.   ! sep
-00011030: 6172 6174 655f 6f70 5f66 696c 6573 5c6e  arate_op_files\n
-00011040: 2729 0a20 2020 2069 6620 6669 7473 5f6f  ').    if fits_o
-00011050: 705f 6669 6c65 733a 0a20 2020 2020 2020  p_files:.       
-00011060: 2066 2e77 7269 7465 2827 2e74 7275 652e   f.write('.true.
-00011070: 2020 2020 2120 6669 7473 5f6f 705f 6669      ! fits_op_fi
-00011080: 6c65 735c 6e27 290a 2020 2020 656c 7365  les\n').    else
-00011090: 3a0a 2020 2020 2020 2020 662e 7772 6974  :.        f.writ
-000110a0: 6528 272e 6661 6c73 652e 2020 2021 2066  e('.false.   ! f
-000110b0: 6974 735f 6f70 5f66 696c 6573 5c6e 2729  its_op_files\n')
-000110c0: 0a20 2020 2069 6620 6e6f 5f69 6e64 6976  .    if no_indiv
-000110d0: 6964 7561 6c5f 6c69 6e65 733a 0a20 2020  idual_lines:.   
-000110e0: 2020 2020 2066 2e77 7269 7465 2827 2e74       f.write('.t
-000110f0: 7275 652e 2020 2020 2120 6e6f 5f69 6e64  rue.    ! no_ind
-00011100: 6976 6964 7561 6c5f 6c69 6e65 735c 6e27  ividual_lines\n'
-00011110: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00011120: 2020 2020 662e 7772 6974 6528 272e 6661      f.write('.fa
-00011130: 6c73 652e 2020 2021 206e 6f5f 696e 6469  lse.   ! no_indi
-00011140: 7669 6475 616c 5f6c 696e 6573 5c6e 2729  vidual_lines\n')
-00011150: 0a20 2020 2069 6620 736c 6162 5f52 543a  .    if slab_RT:
-00011160: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
-00011170: 2827 2e74 7275 652e 2020 2020 2120 736c  ('.true.    ! sl
-00011180: 6162 5f52 5420 5c6e 2729 0a20 2020 2065  ab_RT \n').    e
-00011190: 6c73 653a 0a20 2020 2020 2020 2066 2e77  lse:.        f.w
-000111a0: 7269 7465 2827 2e66 616c 7365 2e20 2020  rite('.false.   
-000111b0: 2120 736c 6162 5f52 5420 5c6e 2729 0a20  ! slab_RT \n'). 
-000111c0: 2020 2069 6620 7368 6f72 745f 666f 726d     if short_form
-000111d0: 6174 3a0a 2020 2020 2020 2020 662e 7772  at:.        f.wr
-000111e0: 6974 6528 272e 7472 7565 2e20 2020 2021  ite('.true.    !
-000111f0: 2073 686f 7274 5f66 6f72 6d61 745c 6e27   short_format\n'
-00011200: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00011210: 2020 2020 662e 7772 6974 6528 272e 6661      f.write('.fa
-00011220: 6c73 652e 2020 2021 2073 686f 7274 5f66  lse.   ! short_f
-00011230: 6f72 6d61 745c 6e27 290a 2020 2020 662e  ormat\n').    f.
-00011240: 7772 6974 6528 6627 7b6e 6d6f 6465 6c73  write(f'{nmodels
-00011250: 7d20 2020 2020 2020 2020 2020 2020 2120  }             ! 
-00011260: 6e6d 6f64 656c 735c 6e27 290a 2020 2020  nmodels\n').    
-00011270: 662e 7772 6974 6528 272d 2d2d 2d2d 2d2d  f.write('-------
-00011280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000112a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000112b0: 2729 0a20 2020 2066 6f72 2069 2069 6e20  ').    for i in 
-000112c0: 7261 6e67 6528 6e6d 6f64 656c 7329 3a0a  range(nmodels):.
-000112d0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-000112e0: 6627 5c6e 2a2a 2a20 6d6f 6465 6c20 7b69  f'\n*** model {i
-000112f0: 2b31 7d20 2a2a 2a5c 6e27 290a 2020 2020  +1} ***\n').    
-00011300: 2020 2020 6966 206e 702e 7375 6d28 4e74      if np.sum(Nt
-00011310: 6f74 5f6c 6973 7429 213d 6e6d 6f64 656c  ot_list)!=nmodel
-00011320: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-00011330: 2e77 7269 7465 2866 6d74 2e66 6f72 6d61  .write(fmt.forma
-00011340: 7428 277b 3a2e 336d 7d27 2c4e 746f 745f  t('{:.3m}',Ntot_
-00011350: 6c69 7374 5b69 5d29 290a 2020 2020 2020  list[i])).      
-00011360: 2020 2020 2020 662e 7772 6974 6528 2709        f.write('.
-00011370: 2020 2021 204e 4874 6f74 2020 5b63 6d5e     ! NHtot  [cm^
-00011380: 2d32 5d20 746f 7461 6c20 6761 7320 636f  -2] total gas co
-00011390: 6c75 6d6e 2064 656e 7369 7479 5c6e 2729  lumn density\n')
-000113a0: 0a20 2020 2020 2020 2069 6620 6e70 2e73  .        if np.s
-000113b0: 756d 286e 4870 6c75 735f 6c69 7374 2921  um(nHplus_list)!
-000113c0: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
-000113d0: 2020 2020 2020 662e 7772 6974 6528 666d        f.write(fm
-000113e0: 742e 666f 726d 6174 2827 7b3a 2e33 6d7d  t.format('{:.3m}
-000113f0: 272c 6e48 706c 7573 5f6c 6973 745b 695d  ',nHplus_list[i]
-00011400: 2929 0a20 2020 2020 2020 2020 2020 2066  )).            f
-00011410: 2e77 7269 7465 2827 0920 2020 2120 6e48  .write('.   ! nH
-00011420: 2b20 2020 205b 636d 5e2d 335d 2020 7072  +    [cm^-3]  pr
-00011430: 6f74 6f6e 206e 756d 6265 7220 6465 6e73  oton number dens
-00011440: 6974 795c 6e27 290a 2020 2020 2020 2020  ity\n').        
-00011450: 6966 206e 702e 7375 6d28 6e48 315f 6c69  if np.sum(nH1_li
-00011460: 7374 2921 3d6e 6d6f 6465 6c73 3a0a 2020  st)!=nmodels:.  
-00011470: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-00011480: 6528 666d 742e 666f 726d 6174 2827 7b3a  e(fmt.format('{:
-00011490: 2e33 6d7d 272c 6e48 315f 6c69 7374 5b69  .3m}',nH1_list[i
-000114a0: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-000114b0: 662e 7772 6974 6528 2709 2020 2021 206e  f.write('.   ! n
-000114c0: 4849 0920 5b63 6d5e 2d33 5d20 6174 6f6d  HI. [cm^-3] atom
-000114d0: 6963 2068 7964 726f 6765 6e5c 6e27 290a  ic hydrogen\n').
-000114e0: 2020 2020 2020 2020 6966 206e 702e 7375          if np.su
-000114f0: 6d28 6e48 325f 6c69 7374 2921 3d6e 6d6f  m(nH2_list)!=nmo
-00011500: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
-00011510: 2020 662e 7772 6974 6528 666d 742e 666f    f.write(fmt.fo
-00011520: 726d 6174 2827 7b3a 2e33 6d7d 272c 6e48  rmat('{:.3m}',nH
-00011530: 325f 6c69 7374 5b69 5d29 290a 2020 2020  2_list[i])).    
-00011540: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00011550: 2709 2020 2021 206e 4832 2020 2020 5b63  '.   ! nH2    [c
-00011560: 6d5e 2d33 5d20 2020 6d6f 6c65 6375 6c61  m^-3]   molecula
-00011570: 7220 6879 6472 6f67 656e 5c6e 2729 0a20  r hydrogen\n'). 
-00011580: 2020 2020 2020 2069 6620 6e70 2e73 756d         if np.sum
-00011590: 286e 4865 5f6c 6973 7429 213d 6e6d 6f64  (nHe_list)!=nmod
-000115a0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
-000115b0: 2066 2e77 7269 7465 2866 6d74 2e66 6f72   f.write(fmt.for
-000115c0: 6d61 7428 277b 3a2e 336d 7d27 2c6e 4865  mat('{:.3m}',nHe
-000115d0: 5f6c 6973 745b 695d 2929 0a20 2020 2020  _list[i])).     
-000115e0: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
-000115f0: 0920 2020 2120 6e48 6520 2020 205b 636d  .   ! nHe    [cm
-00011600: 5e2d 335d 2020 2048 656c 6975 6d5c 6e27  ^-3]   Helium\n'
-00011610: 290a 2020 2020 2020 2020 6966 206e 702e  ).        if np.
-00011620: 7375 6d28 6e65 6c65 635f 6c69 7374 2921  sum(nelec_list)!
-00011630: 3d6e 6d6f 6465 6c73 3a0a 2020 2020 2020  =nmodels:.      
-00011640: 2020 2020 2020 662e 7772 6974 6528 666d        f.write(fm
-00011650: 742e 666f 726d 6174 2827 7b3a 2e33 6d7d  t.format('{:.3m}
-00011660: 272c 6e65 6c65 635f 6c69 7374 5b69 5d29  ',nelec_list[i])
-00011670: 290a 2020 2020 2020 2020 2020 2020 662e  ).            f.
-00011680: 7772 6974 6528 2709 2020 2021 206e 656c  write('.   ! nel
-00011690: 6563 2020 5b63 6d5e 2d33 5d20 2020 656c  ec  [cm^-3]   el
-000116a0: 6563 7472 6f6e 206e 756d 6265 7220 6465  ectron number de
-000116b0: 6e73 6974 795c 6e27 290a 2020 2020 2020  nsity\n').      
-000116c0: 2020 6966 206e 702e 7375 6d28 5467 5f6c    if np.sum(Tg_l
-000116d0: 6973 7429 213d 6e6d 6f64 656c 733a 0a20  ist)!=nmodels:. 
-000116e0: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
-000116f0: 7465 2866 6d74 2e66 6f72 6d61 7428 277b  te(fmt.format('{
-00011700: 3a2e 336d 7d27 2c54 675f 6c69 7374 5b69  :.3m}',Tg_list[i
-00011710: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-00011720: 662e 7772 6974 6528 2709 2020 2021 2054  f.write('.   ! T
-00011730: 6761 7320 5b4b 5d20 2020 2020 2020 2020  gas [K]         
-00011740: 2020 6761 7320 7465 6d70 6572 6174 7572    gas temperatur
-00011750: 655c 6e27 290a 2020 2020 2020 2020 6966  e\n').        if
-00011760: 206e 702e 7375 6d28 5464 5f6c 6973 7429   np.sum(Td_list)
-00011770: 213d 6e6d 6f64 656c 733a 0a20 2020 2020  !=nmodels:.     
-00011780: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
-00011790: 6d74 2e66 6f72 6d61 7428 277b 3a2e 336d  mt.format('{:.3m
-000117a0: 7d27 2c54 645f 6c69 7374 5b69 5d29 290a  }',Td_list[i])).
-000117b0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-000117c0: 6974 6528 2709 2020 2021 2054 6475 7374  ite('.   ! Tdust
-000117d0: 205b 4b5d 2020 2020 2020 2020 2020 2064   [K]           d
-000117e0: 7573 7420 7465 6d70 6572 6174 7572 655c  ust temperature\
-000117f0: 6e27 290a 2020 2020 2020 2020 6966 206e  n').        if n
-00011800: 702e 7375 6d28 7674 7572 625f 6c69 7374  p.sum(vturb_list
-00011810: 2921 3d6e 6d6f 6465 6c73 3a0a 2020 2020  )!=nmodels:.    
-00011820: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00011830: 666d 742e 666f 726d 6174 2827 7b3a 2e33  fmt.format('{:.3
-00011840: 6d7d 272c 7674 7572 625f 6c69 7374 5b69  m}',vturb_list[i
-00011850: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-00011860: 662e 7772 6974 6528 2709 2020 2021 2076  f.write('.   ! v
-00011870: 7475 7262 2020 5b6b 6d73 2f73 5d20 2020  turb  [kms/s]   
-00011880: 2074 7572 6275 6c65 6e74 2076 656c 6f63   turbulent veloc
-00011890: 6974 795c 6e27 290a 2020 2020 2020 2020  ity\n').        
-000118a0: 6966 206e 702e 7375 6d28 6475 7374 5f74  if np.sum(dust_t
-000118b0: 6f5f 6761 735f 6c69 7374 2921 3d6e 6d6f  o_gas_list)!=nmo
-000118c0: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
-000118d0: 2020 662e 7772 6974 6528 666d 742e 666f    f.write(fmt.fo
-000118e0: 726d 6174 2827 7b3a 2e33 6d7d 272c 6475  rmat('{:.3m}',du
-000118f0: 7374 5f74 6f5f 6761 735f 6c69 7374 5b69  st_to_gas_list[i
-00011900: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-00011910: 662e 7772 6974 6528 2709 2020 2021 2064  f.write('.   ! d
-00011920: 7573 745f 746f 5f67 6173 5c6e 2729 0a20  ust_to_gas\n'). 
-00011930: 2020 2020 2020 2069 6620 6e70 2e73 756d         if np.sum
-00011940: 286c 696e 655f 6f76 6572 6c61 705f 6c69  (line_overlap_li
-00011950: 7374 2921 3d32 2a6e 6d6f 6465 6c73 3a0a  st)!=2*nmodels:.
-00011960: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00011970: 6974 6528 666d 742e 666f 726d 6174 2827  ite(fmt.format('
-00011980: 7b3a 2e33 667d 272c 6c69 6e65 5f6f 7665  {:.3f}',line_ove
-00011990: 726c 6170 5f6c 6973 745b 692c 305d 292b  rlap_list[i,0])+
-000119a0: 2720 272b 666d 742e 666f 726d 6174 2827  ' '+fmt.format('
-000119b0: 7b3a 2e33 667d 272c 6c69 6e65 5f6f 7665  {:.3f}',line_ove
-000119c0: 726c 6170 5f6c 6973 745b 692c 315d 2929  rlap_list[i,1]))
-000119d0: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
-000119e0: 7269 7465 2827 0920 2020 2120 6c69 6e65  rite('.   ! line
-000119f0: 5f6f 7665 726c 6170 2020 5b6d 6963 726f  _overlap  [micro
-00011a00: 6e73 5d20 206d 696e 696d 756d 2061 6e64  ns]  minimum and
-00011a10: 206d 6178 696d 756d 2077 6176 656c 656e   maximum wavelen
-00011a20: 6774 6873 2066 6f72 206c 696e 6520 6f76  gths for line ov
-00011a30: 6572 6c61 705c 6e27 290a 2020 2020 2020  erlap\n').      
-00011a40: 2020 6966 206e 702e 7375 6d28 525f 6f76    if np.sum(R_ov
-00011a50: 6572 6c61 705f 6c69 7374 2921 3d6e 6d6f  erlap_list)!=nmo
-00011a60: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
-00011a70: 2020 662e 7772 6974 6528 666d 742e 666f    f.write(fmt.fo
-00011a80: 726d 6174 2827 7b3a 2e33 6d7d 272c 525f  rmat('{:.3m}',R_
-00011a90: 6f76 6572 6c61 705f 6c69 7374 5b69 5d29  overlap_list[i])
-00011aa0: 290a 2020 2020 2020 2020 2020 2020 662e  ).            f.
-00011ab0: 7772 6974 6528 2709 2020 2021 2052 5f6f  write('.   ! R_o
-00011ac0: 7665 726c 6170 2020 7361 6d70 6c69 6e67  verlap  sampling
-00011ad0: 2067 7269 6420 7265 736f 6c75 7469 6f6e   grid resolution
-00011ae0: 2066 6f72 206c 696e 6520 6f76 6572 6c61   for line overla
-00011af0: 705c 6e27 290a 2020 2020 2020 2020 662e  p\n').        f.
-00011b00: 7772 6974 6528 6627 7b6c 656e 2873 7065  write(f'{len(spe
-00011b10: 6369 6573 5f6c 6973 7429 7d09 2020 2021  cies_list)}.   !
-00011b20: 204e 7370 6563 6965 7320 2020 2020 2020   Nspecies       
-00011b30: 2020 2020 206e 756d 6265 7220 6f66 2073       number of s
-00011b40: 7065 6369 6573 2066 6f72 2074 6861 7420  pecies for that 
-00011b50: 6d6f 6465 6c5c 6e27 290a 2020 2020 2020  model\n').      
-00011b60: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
-00011b70: 286c 656e 2873 7065 6369 6573 5f6c 6973  (len(species_lis
-00011b80: 7429 293a 0a20 2020 2020 2020 2020 2020  t)):.           
-00011b90: 2066 2e77 7269 7465 2866 277b 6c69 7374   f.write(f'{list
-00011ba0: 2873 7065 6369 6573 5f6c 6973 742e 6b65  (species_list.ke
-00011bb0: 7973 2829 295b 6a5d 7d20 2020 2020 207b  ys())[j]}      {
-00011bc0: 7370 6563 6965 735f 6c69 7374 5b6c 6973  species_list[lis
-00011bd0: 7428 7370 6563 6965 735f 6c69 7374 2e6b  t(species_list.k
-00011be0: 6579 7328 2929 5b6a 5d5d 7d5c 6e27 290a  eys())[j]]}\n').
-00011bf0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00011c00: 2720 2020 2020 2020 2020 2020 2120 656e  '           ! en
-00011c10: 645c 6e27 290a 2020 2020 2020 2020 662e  d\n').        f.
-00011c20: 7772 6974 6528 272d 2d2d 2d2d 2d2d 2d2d  write('---------
-00011c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2729  --------------')
-00011c60: 0a20 2020 2066 2e63 6c6f 7365 2829 0a20  .    f.close(). 
-00011c70: 2020 2072 6574 7572 6e0a 0a64 6566 2067     return..def g
-00011c80: 656e 6572 6174 655f 3144 5f73 7472 7563  enerate_1D_struc
-00011c90: 7475 7265 2864 7a2c 7370 6563 6965 735f  ture(dz,species_
-00011ca0: 6c69 7374 2c76 7475 7262 2c6e 642c 5464  list,vturb,nd,Td
-00011cb0: 2c6e 5f73 7065 6369 6573 2c54 5f73 7065  ,n_species,T_spe
-00011cc0: 6369 6573 2c6e 4832 3d30 2c6e 4849 3d30  cies,nH2=0,nHI=0
-00011cd0: 2c6e 4849 493d 302c 6e48 653d 302c 6e65  ,nHII=0,nHe=0,ne
-00011ce0: 6c65 633d 302c 6669 6c65 6e61 6d65 3d27  lec=0,filename='
-00011cf0: 3144 5f73 7472 7563 7475 7265 2729 3a0a  1D_structure'):.
-00011d00: 2020 2020 2222 220a 2020 2020 4765 6e65      """.    Gene
-00011d10: 7261 7465 7320 3144 2073 7472 7563 7475  rates 1D structu
-00011d20: 7265 2066 696c 6520 7265 7175 6972 6564  re file required
-00011d30: 2066 6f72 2031 4420 736c 6162 206d 6f64   for 1D slab mod
-00011d40: 656c 730a 2020 2020 2222 220a 2020 2020  els.    """.    
-00011d50: 6966 2069 7369 6e73 7461 6e63 6528 647a  if isinstance(dz
-00011d60: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
-00011d70: 7461 6e63 6528 647a 2c69 6e74 293a 2020  tance(dz,int):  
-00011d80: 2020 2020 2020 2020 2020 2020 2064 7a20               dz 
-00011d90: 3d20 6e70 2e61 7272 6179 285b 647a 5d29  = np.array([dz])
-00011da0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-00011db0: 6365 2864 7a2c 6c69 7374 293a 2020 2020  ce(dz,list):    
-00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011de0: 2020 647a 203d 206e 702e 6172 7261 7928    dz = np.array(
-00011df0: 647a 290a 2020 2020 6966 2069 7369 6e73  dz).    if isins
-00011e00: 7461 6e63 6528 7370 6563 6965 735f 6c69  tance(species_li
-00011e10: 7374 2c73 7472 293a 2020 2020 2020 2020  st,str):        
-00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e30: 2020 2020 2073 7065 6369 6573 5f6c 6973       species_lis
-00011e40: 743d 5b73 7065 6369 6573 5f6c 6973 745d  t=[species_list]
-00011e50: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-00011e60: 6365 2876 7475 7262 2c66 6c6f 6174 2920  ce(vturb,float) 
-00011e70: 6f72 2069 7369 6e73 7461 6e63 6528 7674  or isinstance(vt
-00011e80: 7572 622c 696e 7429 3a20 2020 2020 2020  urb,int):       
-00011e90: 2020 7674 7572 6220 3d20 6e70 2e6f 6e65    vturb = np.one
-00011ea0: 735f 6c69 6b65 2864 7a29 2a76 7475 7262  s_like(dz)*vturb
-00011eb0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-00011ec0: 6365 286e 642c 666c 6f61 7429 206f 7220  ce(nd,float) or 
-00011ed0: 6973 696e 7374 616e 6365 286e 642c 696e  isinstance(nd,in
-00011ee0: 7429 3a20 2020 2020 2020 2020 2020 2020  t):             
-00011ef0: 2020 6e64 203d 206e 702e 6f6e 6573 5f6c    nd = np.ones_l
-00011f00: 696b 6528 647a 292a 6e64 0a20 2020 2069  ike(dz)*nd.    i
-00011f10: 6620 6973 696e 7374 616e 6365 2854 642c  f isinstance(Td,
-00011f20: 666c 6f61 7429 206f 7220 6973 696e 7374  float) or isinst
-00011f30: 616e 6365 2854 642c 696e 7429 3a20 2020  ance(Td,int):   
-00011f40: 2020 2020 2020 2020 2020 2020 5464 203d              Td =
-00011f50: 206e 702e 6f6e 6573 5f6c 696b 6528 647a   np.ones_like(dz
-00011f60: 292a 5464 0a20 2020 2069 6620 6973 696e  )*Td.    if isin
-00011f70: 7374 616e 6365 286e 4832 2c66 6c6f 6174  stance(nH2,float
-00011f80: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
-00011f90: 6e48 322c 696e 7429 3a20 2020 2020 2020  nH2,int):       
-00011fa0: 2020 2020 2020 6e48 3220 3d20 6e70 2e6f        nH2 = np.o
-00011fb0: 6e65 735f 6c69 6b65 2864 7a29 2a6e 4832  nes_like(dz)*nH2
-00011fc0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-00011fd0: 6365 286e 4849 2c66 6c6f 6174 2920 6f72  ce(nHI,float) or
-00011fe0: 2069 7369 6e73 7461 6e63 6528 6e48 492c   isinstance(nHI,
-00011ff0: 696e 7429 3a20 2020 2020 2020 2020 2020  int):           
-00012000: 2020 6e48 4920 3d20 6e70 2e6f 6e65 735f    nHI = np.ones_
-00012010: 6c69 6b65 2864 7a29 2a6e 4849 0a20 2020  like(dz)*nHI.   
-00012020: 2069 6620 6973 696e 7374 616e 6365 286e   if isinstance(n
-00012030: 4849 492c 666c 6f61 7429 206f 7220 6973  HII,float) or is
-00012040: 696e 7374 616e 6365 286e 4849 492c 696e  instance(nHII,in
-00012050: 7429 3a20 2020 2020 2020 2020 2020 6e48  t):           nH
-00012060: 4949 203d 206e 702e 6f6e 6573 5f6c 696b  II = np.ones_lik
-00012070: 6528 647a 292a 6e48 4949 0a20 2020 2069  e(dz)*nHII.    i
-00012080: 6620 6973 696e 7374 616e 6365 286e 4865  f isinstance(nHe
-00012090: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
-000120a0: 7461 6e63 6528 6e48 652c 696e 7429 3a20  tance(nHe,int): 
-000120b0: 2020 2020 2020 2020 2020 2020 6e48 6520              nHe 
-000120c0: 3d20 6e70 2e6f 6e65 735f 6c69 6b65 2864  = np.ones_like(d
-000120d0: 7a29 2a6e 4865 0a20 2020 2069 6620 6973  z)*nHe.    if is
-000120e0: 696e 7374 616e 6365 286e 656c 6563 2c66  instance(nelec,f
-000120f0: 6c6f 6174 2920 6f72 2069 7369 6e73 7461  loat) or isinsta
-00012100: 6e63 6528 6e65 6c65 632c 696e 7429 3a20  nce(nelec,int): 
-00012110: 2020 2020 2020 2020 6e65 6c65 6320 3d20          nelec = 
-00012120: 6e70 2e6f 6e65 735f 6c69 6b65 2864 7a29  np.ones_like(dz)
-00012130: 2a6e 656c 6563 0a20 2020 2069 6620 6973  *nelec.    if is
-00012140: 696e 7374 616e 6365 286e 5f73 7065 6369  instance(n_speci
-00012150: 6573 2c66 6c6f 6174 2920 6f72 2069 7369  es,float) or isi
-00012160: 6e73 7461 6e63 6528 6e5f 7370 6563 6965  nstance(n_specie
-00012170: 732c 696e 7429 3a20 6e5f 7370 6563 6965  s,int): n_specie
-00012180: 7320 3d20 6e70 2e6f 6e65 7328 2864 7a2e  s = np.ones((dz.
-00012190: 7368 6170 655b 305d 2c6c 656e 2873 7065  shape[0],len(spe
-000121a0: 6369 6573 5f6c 6973 7429 2929 2a6e 5f73  cies_list)))*n_s
-000121b0: 7065 6369 6573 0a20 2020 2069 6620 6973  pecies.    if is
-000121c0: 696e 7374 616e 6365 2854 5f73 7065 6369  instance(T_speci
-000121d0: 6573 2c66 6c6f 6174 2920 6f72 2069 7369  es,float) or isi
-000121e0: 6e73 7461 6e63 6528 545f 7370 6563 6965  nstance(T_specie
-000121f0: 732c 696e 7429 3a20 545f 7370 6563 6965  s,int): T_specie
-00012200: 7320 3d20 6e70 2e6f 6e65 7328 2864 7a2e  s = np.ones((dz.
-00012210: 7368 6170 655b 305d 2c6c 656e 2873 7065  shape[0],len(spe
-00012220: 6369 6573 5f6c 6973 7429 2929 2a54 5f73  cies_list)))*T_s
-00012230: 7065 6369 6573 0a20 2020 2069 6620 6973  pecies.    if is
-00012240: 696e 7374 616e 6365 2854 5f73 7065 6369  instance(T_speci
-00012250: 6573 2c6c 6973 7429 3a20 2020 2020 2020  es,list):       
-00012260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012270: 2020 2020 2020 2020 545f 7370 6563 6965          T_specie
-00012280: 7320 3d20 6e70 2e61 7272 6179 2854 5f73  s = np.array(T_s
-00012290: 7065 6369 6573 290a 2020 2020 6966 2069  pecies).    if i
-000122a0: 7369 6e73 7461 6e63 6528 6e5f 7370 6563  sinstance(n_spec
-000122b0: 6965 732c 6c69 7374 293a 2020 2020 2020  ies,list):      
-000122c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122d0: 2020 2020 2020 2020 206e 5f73 7065 6369           n_speci
-000122e0: 6573 203d 206e 702e 6172 7261 7928 6e5f  es = np.array(n_
-000122f0: 7370 6563 6965 7329 0a20 2020 2069 6620  species).    if 
-00012300: 6e70 2e61 7272 6179 2854 5f73 7065 6369  np.array(T_speci
-00012310: 6573 292e 7369 7a65 3d3d 6c65 6e28 7370  es).size==len(sp
-00012320: 6563 6965 735f 6c69 7374 293a 0a20 2020  ecies_list):.   
-00012330: 2020 2020 2054 5f73 7065 6369 6573 5f74       T_species_t
-00012340: 656d 7020 3d20 6e70 2e6f 6e65 7328 2864  emp = np.ones((d
-00012350: 7a2e 7368 6170 655b 305d 2c6c 656e 2873  z.shape[0],len(s
-00012360: 7065 6369 6573 5f6c 6973 7429 2929 0a20  pecies_list))). 
-00012370: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00012380: 7261 6e67 6528 6c65 6e28 7370 6563 6965  range(len(specie
-00012390: 735f 6c69 7374 2929 3a0a 2020 2020 2020  s_list)):.      
-000123a0: 2020 2020 2020 545f 7370 6563 6965 735f        T_species_
-000123b0: 7465 6d70 5b3a 2c69 5d20 3d20 545f 7370  temp[:,i] = T_sp
-000123c0: 6563 6965 735b 695d 0a20 2020 2020 2020  ecies[i].       
-000123d0: 2054 5f73 7065 6369 6573 203d 2054 5f73   T_species = T_s
-000123e0: 7065 6369 6573 5f74 656d 702a 312e 3030  pecies_temp*1.00
-000123f0: 0a20 2020 2069 6620 6e70 2e61 7272 6179  .    if np.array
-00012400: 286e 5f73 7065 6369 6573 292e 7369 7a65  (n_species).size
-00012410: 3d3d 6c65 6e28 7370 6563 6965 735f 6c69  ==len(species_li
-00012420: 7374 293a 0a20 2020 2020 2020 206e 5f73  st):.        n_s
-00012430: 7065 6369 6573 5f74 656d 7020 3d20 6e70  pecies_temp = np
-00012440: 2e6f 6e65 7328 2864 7a2e 7368 6170 655b  .ones((dz.shape[
-00012450: 305d 2c6c 656e 2873 7065 6369 6573 5f6c  0],len(species_l
-00012460: 6973 7429 2929 0a20 2020 2020 2020 2066  ist))).        f
-00012470: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00012480: 6e28 7370 6563 6965 735f 6c69 7374 2929  n(species_list))
-00012490: 3a0a 2020 2020 2020 2020 2020 2020 6e5f  :.            n_
-000124a0: 7370 6563 6965 735f 7465 6d70 5b3a 2c69  species_temp[:,i
-000124b0: 5d20 3d20 6e5f 7370 6563 6965 735b 695d  ] = n_species[i]
-000124c0: 0a20 2020 2020 2020 206e 5f73 7065 6369  .        n_speci
-000124d0: 6573 203d 206e 5f73 7065 6369 6573 5f74  es = n_species_t
-000124e0: 656d 702a 312e 3030 0a0a 2020 2020 7769  emp*1.00..    wi
-000124f0: 7468 206f 7065 6e28 6669 6c65 6e61 6d65  th open(filename
-00012500: 2c27 7727 2920 6173 2066 3a0a 2020 2020  ,'w') as f:.    
-00012510: 2020 2020 662e 7772 6974 6528 6627 7b6c      f.write(f'{l
-00012520: 656e 2864 7a29 3a64 7d5c 6e27 290a 2020  en(dz):d}\n').  
-00012530: 2020 2020 2020 662e 7772 6974 6528 6627        f.write(f'
-00012540: 7b6c 656e 2873 7065 6369 6573 5f6c 6973  {len(species_lis
-00012550: 7429 3a64 7d5c 6e27 290a 2020 2020 2020  t):d}\n').      
-00012560: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00012570: 286c 656e 2873 7065 6369 6573 5f6c 6973  (len(species_lis
-00012580: 7429 293a 0a20 2020 2020 2020 2020 2020  t)):.           
-00012590: 2066 2e77 7269 7465 2873 7065 6369 6573   f.write(species
-000125a0: 5f6c 6973 745b 695d 2b27 5c6e 2729 0a20  _list[i]+'\n'). 
-000125b0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000125c0: 7261 6e67 6528 6c65 6e28 647a 2929 3a0a  range(len(dz)):.
-000125d0: 2020 2020 2020 2020 2020 2020 7374 7269              stri
-000125e0: 6e67 203d 2027 270a 2020 2020 2020 2020  ng = ''.        
-000125f0: 2020 2020 7374 7269 6e67 202b 3d20 6627      string += f'
-00012600: 7b69 2b31 3a64 7d20 2027 0a20 2020 2020  {i+1:d}  '.     
-00012610: 2020 2020 2020 2073 7472 696e 6720 2b3d         string +=
-00012620: 2066 277b 647a 5b69 5d3a 2e33 657d 2020   f'{dz[i]:.3e}  
-00012630: 270a 2020 2020 2020 2020 2020 2020 7374  '.            st
-00012640: 7269 6e67 202b 3d20 6627 7b76 7475 7262  ring += f'{vturb
-00012650: 5b69 5d3a 2e33 667d 2020 270a 2020 2020  [i]:.3f}  '.    
-00012660: 2020 2020 2020 2020 7374 7269 6e67 202b          string +
-00012670: 3d20 6627 7b6e 645b 695d 3a2e 3365 7d20  = f'{nd[i]:.3e} 
-00012680: 2027 0a20 2020 2020 2020 2020 2020 2073   '.            s
-00012690: 7472 696e 6720 2b3d 2066 277b 5464 5b69  tring += f'{Td[i
-000126a0: 5d3a 2e33 667d 2020 270a 2020 2020 2020  ]:.3f}  '.      
-000126b0: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
-000126c0: 616e 6765 286c 656e 2873 7065 6369 6573  ange(len(species
-000126d0: 5f6c 6973 7429 293a 0a20 2020 2020 2020  _list)):.       
-000126e0: 2020 2020 2020 2020 2073 7472 696e 6720           string 
-000126f0: 2b3d 2066 277b 6e5f 7370 6563 6965 735b  += f'{n_species[
-00012700: 692c 6a5d 3a2e 3365 7d20 2027 0a20 2020  i,j]:.3e}  '.   
-00012710: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-00012720: 6e20 7261 6e67 6528 6c65 6e28 7370 6563  n range(len(spec
-00012730: 6965 735f 6c69 7374 2929 3a0a 2020 2020  ies_list)):.    
-00012740: 2020 2020 2020 2020 2020 2020 7374 7269              stri
-00012750: 6e67 202b 3d20 6627 7b54 5f73 7065 6369  ng += f'{T_speci
-00012760: 6573 5b69 2c6a 5d3a 2e33 667d 2020 270a  es[i,j]:.3f}  '.
-00012770: 2020 2020 2020 2020 2020 2020 7374 7269              stri
-00012780: 6e67 202b 3d20 6627 7b6e 4832 5b69 5d3a  ng += f'{nH2[i]:
-00012790: 2e33 657d 2020 270a 2020 2020 2020 2020  .3e}  '.        
-000127a0: 2020 2020 7374 7269 6e67 202b 3d20 6627      string += f'
-000127b0: 7b6e 4849 5b69 5d3a 2e33 657d 2020 270a  {nHI[i]:.3e}  '.
-000127c0: 2020 2020 2020 2020 2020 2020 7374 7269              stri
-000127d0: 6e67 202b 3d20 6627 7b6e 4849 495b 695d  ng += f'{nHII[i]
-000127e0: 3a2e 3365 7d20 2027 0a20 2020 2020 2020  :.3e}  '.       
-000127f0: 2020 2020 2073 7472 696e 6720 2b3d 2066       string += f
-00012800: 277b 6e48 655b 695d 3a2e 3365 7d20 2027  '{nHe[i]:.3e}  '
-00012810: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00012820: 696e 6720 2b3d 2066 277b 6e65 6c65 635b  ing += f'{nelec[
-00012830: 695d 3a2e 3365 7d20 2027 0a20 2020 2020  i]:.3e}  '.     
-00012840: 2020 2020 2020 2066 2e77 7269 7465 2873         f.write(s
-00012850: 7472 696e 672b 275c 6e27 290a 2020 2020  tring+'\n').    
-00012860: 2020 2020 662e 636c 6f73 6528 290a 0a0a      f.close()...
-00012870: 2020 2020 2020 2020 0a0a 2020 2020 0a0a          ..    ..
-00012880: 0a63 6c61 7373 204d 7946 6f72 6d61 7474  .class MyFormatt
-00012890: 6572 2873 7472 696e 672e 466f 726d 6174  er(string.Format
-000128a0: 7465 7229 3a0a 2020 2020 2222 220a 2020  ter):.    """.  
-000128b0: 2020 5374 7269 6e67 2066 6f72 6d61 7474    String formatt
-000128c0: 6572 2066 6f72 2070 726f 6475 6369 6e67  er for producing
-000128d0: 2069 6e70 7574 2066 696c 6573 0a20 2020   input files.   
-000128e0: 2022 2222 0a0a 2020 2020 6465 6620 666f   """..    def fo
-000128f0: 726d 6174 5f66 6965 6c64 2873 656c 662c  rmat_field(self,
-00012900: 7661 6c75 652c 666f 726d 6174 5f73 7065  value,format_spe
-00012910: 6329 3a0a 2020 2020 2020 2020 6966 2066  c):.        if f
-00012920: 6f72 6d61 745f 7370 6563 5b2d 315d 3d3d  ormat_spec[-1]==
-00012930: 276d 273a 0a20 2020 2020 2020 2020 2020  'm':.           
-00012940: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00012950: 666f 726d 6174 5f66 6965 6c64 2876 616c  format_field(val
-00012960: 7565 2c66 6f72 6d61 745f 7370 6563 5b3a  ue,format_spec[:
-00012970: 2d31 5d2b 2765 2729 2e72 6570 6c61 6365  -1]+'e').replace
-00012980: 2827 652b 272c 2765 2729 0a20 2020 2020  ('e+','e').     
-00012990: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000129a0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-000129b0: 7228 292e 666f 726d 6174 5f66 6965 6c64  r().format_field
-000129c0: 2876 616c 7565 2c66 6f72 6d61 745f 7370  (value,format_sp
-000129d0: 6563 290a 0a0a 666d 743d 4d79 466f 726d  ec)...fmt=MyForm
-000129e0: 6174 7465 7228 290a 0a64 6566 206c 696e  atter()..def lin
-000129f0: 655f 666c 7578 286c 312c 6c32 2c77 6176  e_flux(l1,l2,wav
-00012a00: 656c 656e 6774 682c 666c 7578 293a 0a20  elength,flux):. 
-00012a10: 2020 2027 2727 0a20 2020 2052 6574 7572     '''.    Retur
-00012a20: 6e3a 2053 756d 206f 6620 696e 7465 6772  n: Sum of integr
-00012a30: 6174 6564 206c 696e 6520 666c 7578 2062  ated line flux b
-00012a40: 6574 7765 656e 2077 6176 656c 656e 6774  etween wavelengt
-00012a50: 6873 206c 3120 616e 6420 6c32 2e20 0a20  hs l1 and l2. . 
-00012a60: 2020 2055 6e69 7473 3a20 5265 7475 726e     Units: Return
-00012a70: 2069 7320 696e 2074 6865 2073 616d 6520   is in the same 
-00012a80: 756e 6974 2061 7320 696e 7075 742e 205b  unit as input. [
-00012a90: 4173 7375 6d65 6420 746f 2062 6520 696e  Assumed to be in
-00012aa0: 2065 7267 2f73 2f63 6d32 2f73 725d 0a20   erg/s/cm2/sr]. 
-00012ab0: 2020 2020 2020 2020 2020 6c31 2061 6e64            l1 and
-00012ac0: 206c 3220 7361 6d65 2075 6e69 7420 6173   l2 same unit as
-00012ad0: 2077 6176 656c 656e 6774 680a 2020 2020   wavelength.    
-00012ae0: 2727 270a 2020 2020 6d61 736b 203d 2028  '''.    mask = (
-00012af0: 7761 7665 6c65 6e67 7468 3e6c 3129 2026  wavelength>l1) &
-00012b00: 2028 7761 7665 6c65 6e67 7468 3c3d 6c32   (wavelength<=l2
-00012b10: 290a 2020 2020 7265 7475 726e 206e 702e  ).    return np.
-00012b20: 7375 6d28 666c 7578 5b6d 6173 6b5d 290a  sum(flux[mask]).
-00012b30: 0a64 6566 206c 696e 655f 666c 7578 6573  .def line_fluxes
-00012b40: 2877 696e 646f 7773 2c77 6176 656c 656e  (windows,wavelen
-00012b50: 6774 682c 666c 7578 293a 0a20 2020 2027  gth,flux):.    '
-00012b60: 2727 0a20 2020 2052 6574 7572 6e3a 2061  ''.    Return: a
-00012b70: 7272 6179 206f 6620 7375 6d20 6f66 2069  rray of sum of i
-00012b80: 6e74 6567 7261 7465 6420 6c69 6e65 2066  ntegrated line f
-00012b90: 6c75 7820 696e 2077 6176 656c 656e 6774  lux in wavelengt
-00012ba0: 6820 7769 6e64 6f77 732e 200a 2020 2020  h windows. .    
-00012bb0: 556e 6974 733a 2052 6574 7572 6e20 6973  Units: Return is
-00012bc0: 2069 6e20 7468 6520 7361 6d65 2075 6e69   in the same uni
-00012bd0: 7420 6173 2069 6e70 7574 2e20 5b41 7373  t as input. [Ass
-00012be0: 756d 6564 2074 6f20 6265 2069 6e20 6572  umed to be in er
-00012bf0: 672f 732f 636d 322f 7372 5d0a 2020 2020  g/s/cm2/sr].    
-00012c00: 7769 6e64 6f77 733a 206c 6973 7420 6f66  windows: list of
-00012c10: 2077 6176 656c 656e 6774 6820 6c69 6d69   wavelength limi
-00012c20: 7473 206f 6620 7769 6e64 6f77 732e 2045  ts of windows. E
-00012c30: 7861 6d70 6c65 3a20 5b5b 3134 2c31 342e  xample: [[14,14.
-00012c40: 355d 2c5b 3135 2c31 362e 325d 2c5b 3132  5],[15,16.2],[12
-00012c50: 2e35 2c31 342e 315d 5d0a 2020 2020 2727  .5,14.1]].    ''
-00012c60: 270a 2020 2020 4620 3d20 5b5d 0a20 2020  '.    F = [].   
-00012c70: 2066 6f72 2057 2069 6e20 7769 6e64 6f77   for W in window
-00012c80: 733a 0a20 2020 2020 2020 2046 2e61 7070  s:.        F.app
-00012c90: 656e 6428 6c69 6e65 5f66 6c75 7828 575b  end(line_flux(W[
-00012ca0: 305d 2c57 5b31 5d2c 7761 7665 6c65 6e67  0],W[1],waveleng
-00012cb0: 7468 2c66 6c75 7829 290a 2020 2020 7265  th,flux)).    re
-00012cc0: 7475 726e 286e 702e 6172 7261 7928 4629  turn(np.array(F)
-00012cd0: 290a 0a64 6566 206c 696e 655f 666c 7578  )..def line_flux
-00012ce0: 5f72 6174 696f 7328 7261 7469 6f5f 7769  _ratios(ratio_wi
-00012cf0: 6e64 6f77 732c 7761 7665 6c65 6e67 7468  ndows,wavelength
-00012d00: 2c66 6c75 7829 3a0a 2020 2020 2727 270a  ,flux):.    '''.
-00012d10: 2020 2020 5265 7475 726e 3a20 496e 7465      Return: Inte
-00012d20: 6772 6174 6564 206c 696e 6520 666c 7578  grated line flux
-00012d30: 2072 6174 696f 7320 6265 7477 6565 6e20   ratios between 
-00012d40: 7761 7665 6c65 6e67 7468 7320 6c31 2061  wavelengths l1 a
-00012d50: 6e64 206c 322e 0a20 2020 2055 6e69 743a  nd l2..    Unit:
-00012d60: 2052 6574 7572 6e20 6861 7320 6e6f 2075   Return has no u
-00012d70: 6e69 742e 205b 496e 7075 7420 6973 2061  nit. [Input is a
-00012d80: 7373 756d 6564 2074 6f20 6265 2069 6e20  ssumed to be in 
-00012d90: 6572 672f 732f 636d 322f 7372 5d0a 2020  erg/s/cm2/sr].  
-00012da0: 2020 7261 7469 6f5f 7769 6e64 6f77 733a    ratio_windows:
-00012db0: 206c 6973 7420 6f66 2077 6176 656c 656e   list of wavelen
-00012dc0: 6774 6820 7769 6e64 6f77 732e 2045 7861  gth windows. Exa
-00012dd0: 6d70 6c65 3a20 5b5b 5b31 342c 3134 2e35  mple: [[[14,14.5
-00012de0: 5d2c 5b31 352c 3136 2e32 5d5d 2c5b 5b31  ],[15,16.2]],[[1
-00012df0: 322e 352c 3134 2e31 5d2c 5b31 332e 342c  2.5,14.1],[13.4,
-00012e00: 3133 2e38 5d5d 5d0a 2020 2020 2727 270a  13.8]]].    '''.
-00012e10: 2020 2020 5220 3d20 5b5d 0a20 2020 2066      R = [].    f
-00012e20: 6f72 2077 696e 646f 7720 696e 2072 6174  or window in rat
-00012e30: 696f 5f77 696e 646f 7773 3a0a 2020 2020  io_windows:.    
-00012e40: 2020 2020 4620 3d20 6c69 6e65 5f66 6c75      F = line_flu
-00012e50: 7865 7328 5b77 696e 646f 775b 305d 2c77  xes([window[0],w
-00012e60: 696e 646f 775b 315d 5d2c 7761 7665 6c65  indow[1]],wavele
-00012e70: 6e67 7468 2c66 6c75 7829 0a20 2020 2020  ngth,flux).     
-00012e80: 2020 2052 2e61 7070 656e 6428 465b 315d     R.append(F[1]
-00012e90: 2f46 5b30 5d29 0a20 2020 2072 6574 7572  /F[0]).    retur
-00012ea0: 6e28 6e70 2e61 7272 6179 2852 2929 0a0a  n(np.array(R))..
-00012eb0: 6465 6620 6c69 6e65 5f66 6c75 785f 7072  def line_flux_pr
-00012ec0: 6f64 7563 7473 2870 726f 6475 6374 5f77  oducts(product_w
-00012ed0: 696e 646f 7773 2c77 6176 656c 656e 6774  indows,wavelengt
-00012ee0: 682c 666c 7578 293a 0a20 2020 2027 2727  h,flux):.    '''
-00012ef0: 0a20 2020 2052 6574 7572 6e3a 2049 6e74  .    Return: Int
-00012f00: 6567 7261 7465 6420 6c69 6e65 2066 6c75  egrated line flu
-00012f10: 7820 7072 6f64 7563 7473 2062 6574 7765  x products betwe
-00012f20: 656e 2077 6176 656c 656e 6774 6873 206c  en wavelengths l
-00012f30: 3120 616e 6420 6c32 2e0a 2020 2020 556e  1 and l2..    Un
-00012f40: 6974 3a20 5265 7475 726e 2075 6e69 7420  it: Return unit 
-00012f50: 6973 206f 7574 7075 7420 756e 6974 7320  is output units 
-00012f60: 7371 7561 7265 642e 205b 496e 7075 7420  squared. [Input 
-00012f70: 6973 2061 7373 756d 6564 2074 6f20 6265  is assumed to be
-00012f80: 2069 6e20 6572 672f 732f 636d 322f 7372   in erg/s/cm2/sr
-00012f90: 5d0a 2020 2020 7072 6f64 7563 745f 7769  ].    product_wi
-00012fa0: 6e64 6f77 733a 206c 6973 7420 6f66 2077  ndows: list of w
-00012fb0: 6176 656c 656e 6774 6820 7769 6e64 6f77  avelength window
-00012fc0: 732e 2045 7861 6d70 6c65 3a20 5b5b 5b31  s. Example: [[[1
-00012fd0: 342c 3134 2e35 5d2c 5b31 352c 3136 2e32  4,14.5],[15,16.2
-00012fe0: 5d5d 2c5b 5b31 322e 352c 3134 2e31 5d2c  ]],[[12.5,14.1],
-00012ff0: 5b31 332e 342c 3133 2e38 5d5d 5d0a 2020  [13.4,13.8]]].  
-00013000: 2020 2727 270a 2020 2020 5220 3d20 5b5d    '''.    R = []
-00013010: 0a20 2020 2066 6f72 2077 696e 646f 7720  .    for window 
-00013020: 696e 2070 726f 6475 6374 5f77 696e 646f  in product_windo
-00013030: 7773 3a0a 2020 2020 2020 2020 4620 3d20  ws:.        F = 
-00013040: 6c69 6e65 5f66 6c75 7865 7328 5b77 696e  line_fluxes([win
-00013050: 646f 775b 305d 2c77 696e 646f 775b 315d  dow[0],window[1]
-00013060: 5d2c 7761 7665 6c65 6e67 7468 2c66 6c75  ],wavelength,flu
-00013070: 7829 0a20 2020 2020 2020 2052 2e61 7070  x).        R.app
-00013080: 656e 6428 465b 315d 2a46 5b30 5d29 0a20  end(F[1]*F[0]). 
-00013090: 2020 2072 6574 7572 6e28 6e70 2e61 7272     return(np.arr
-000130a0: 6179 2852 2929 0a0a 6465 6620 7370 6563  ay(R))..def spec
-000130b0: 7472 616c 5f66 6c75 7828 6c31 2c6c 322c  tral_flux(l1,l2,
-000130c0: 7761 7665 6c65 6e67 7468 2c66 6c75 7829  wavelength,flux)
-000130d0: 3a0a 2020 2020 2727 270a 2020 2020 5265  :.    '''.    Re
-000130e0: 7475 726e 3a20 5375 6d20 6f66 2069 6e74  turn: Sum of int
-000130f0: 6567 7261 7465 6420 6c69 6e65 2066 6c75  egrated line flu
-00013100: 7820 6265 7477 6565 6e20 7761 7665 6c65  x between wavele
-00013110: 6e67 7468 7320 6c31 2061 6e64 206c 322e  ngths l1 and l2.
-00013120: 200a 2020 2020 556e 6974 3a20 5265 7475   .    Unit: Retu
-00013130: 726e 2069 6e20 5b65 7267 2f73 2f63 6d32  rn in [erg/s/cm2
-00013140: 5d20 616e 6420 696e 7075 7420 6973 2069  ] and input is i
-00013150: 6e20 5b4a 795d 0a20 2020 2020 2020 2020  n [Jy].         
-00013160: 206c 312c 206c 322c 2061 6e64 2077 6176   l1, l2, and wav
-00013170: 656c 656e 6774 6820 696e 206d 6963 726f  elength in micro
-00013180: 6e73 0a20 2020 2027 2727 0a20 2020 2066  ns.    '''.    f
-00013190: 6c75 7820 2020 2020 2020 3d20 666c 7578  lux       = flux
-000131a0: 2a31 652d 3233 2023 436f 6e76 6572 7469  *1e-23 #Converti
-000131b0: 6e67 204a 7920 746f 2065 7267 2e73 e288  ng Jy to erg.s..
-000131c0: 9231 2e63 6de2 8892 322e 487a e288 9231  .1.cm...2.Hz...1
-000131d0: 0a20 2020 2077 6176 656c 656e 6774 6820  .    wavelength 
-000131e0: 3d20 7761 7665 6c65 6e67 7468 2a31 652d  = wavelength*1e-
-000131f0: 3420 2343 6f6e 7665 7274 696e 6720 6d69  4 #Converting mi
-00013200: 6372 6f6e 7320 746f 2063 6d0a 2020 2020  crons to cm.    
-00013210: 666c 7578 2020 2020 2020 203d 2066 6c75  flux       = flu
-00013220: 785b 6e70 2e61 7267 736f 7274 2877 6176  x[np.argsort(wav
-00013230: 656c 656e 6774 6829 5d0a 2020 2020 7761  elength)].    wa
-00013240: 7665 6c65 6e67 7468 203d 2077 6176 656c  velength = wavel
-00013250: 656e 6774 685b 6e70 2e61 7267 736f 7274  ength[np.argsort
-00013260: 2877 6176 656c 656e 6774 6829 5d0a 2020  (wavelength)].  
-00013270: 2020 6c31 2020 2020 2020 2020 203d 206c    l1         = l
-00013280: 312a 3165 2d34 2023 436f 6e76 6572 7469  1*1e-4 #Converti
-00013290: 6e67 206d 6963 726f 6e73 2074 6f20 636d  ng microns to cm
-000132a0: 0a20 2020 206c 3220 2020 2020 2020 2020  .    l2         
-000132b0: 3d20 6c32 2a31 652d 3420 2343 6f6e 7665  = l2*1e-4 #Conve
-000132c0: 7274 696e 6720 6d69 6372 6f6e 7320 746f  rting microns to
-000132d0: 2063 6d0a 2020 2020 635f 636d 7320 2020   cm.    c_cms   
-000132e0: 2020 203d 2063 2a31 6532 2023 436f 6e76     = c*1e2 #Conv
-000132f0: 6572 7469 6e67 206d 2f73 2074 6f20 636d  erting m/s to cm
-00013300: 2f73 0a20 2020 206d 6173 6b20 2020 2020  /s.    mask     
-00013310: 2020 3d20 2877 6176 656c 656e 6774 683e    = (wavelength>
-00013320: 6c31 2920 2620 2877 6176 656c 656e 6774  l1) & (wavelengt
-00013330: 683c 3d6c 3229 0a20 2020 2077 6176 6520  h<=l2).    wave 
-00013340: 2020 2020 2020 3d20 7761 7665 6c65 6e67        = waveleng
-00013350: 7468 5b6d 6173 6b5d 0a20 2020 2023 2077  th[mask].    # w
-00013360: 6176 6531 2020 2020 2020 3d20 6e70 2e72  ave1      = np.r
-00013370: 6f6c 6c28 7761 7665 6c65 6e67 7468 2c31  oll(wavelength,1
-00013380: 295b 6d61 736b 5d0a 2020 2020 2320 7761  )[mask].    # wa
-00013390: 7665 3120 2020 2020 203d 2031 302a 2a28  ve1      = 10**(
-000133a0: 286e 702e 6c6f 6731 3028 7761 7665 292b  (np.log10(wave)+
-000133b0: 6e70 2e6c 6f67 3130 2877 6176 6531 2929  np.log10(wave1))
-000133c0: 2f32 290a 2020 2020 2320 7761 7665 3220  /2).    # wave2 
-000133d0: 2020 2020 203d 206e 702e 726f 6c6c 2877       = np.roll(w
-000133e0: 6176 656c 656e 6774 682c 2d31 295b 6d61  avelength,-1)[ma
-000133f0: 736b 5d0a 2020 2020 2320 7761 7665 3220  sk].    # wave2 
-00013400: 2020 2020 203d 2031 302a 2a28 286e 702e       = 10**((np.
-00013410: 6c6f 6731 3028 7761 7665 292b 6e70 2e6c  log10(wave)+np.l
-00013420: 6f67 3130 2877 6176 6532 2929 2f32 290a  og10(wave2))/2).
-00013430: 2020 2020 2320 646e 7520 2020 2020 2020      # dnu       
-00013440: 203d 2063 2a28 7761 7665 322d 7761 7665   = c*(wave2-wave
-00013450: 3129 2f77 6176 652a 2a32 2a31 6532 0a20  1)/wave**2*1e2. 
-00013460: 2020 2077 6176 6531 2020 2020 2020 3d20     wave1      = 
-00013470: 6e70 2e72 6f6c 6c28 7761 7665 6c65 6e67  np.roll(waveleng
-00013480: 7468 2c31 295b 6d61 736b 5d0a 2020 2020  th,1)[mask].    
-00013490: 7761 7665 3220 2020 2020 203d 206e 702e  wave2      = np.
-000134a0: 726f 6c6c 2877 6176 656c 656e 6774 682c  roll(wavelength,
-000134b0: 2d31 295b 6d61 736b 5d0a 2020 2020 646e  -1)[mask].    dn
-000134c0: 7520 2020 2020 2020 203d 2028 635f 636d  u        = (c_cm
-000134d0: 732a 2831 2f77 6176 6531 2d31 2f77 6176  s*(1/wave1-1/wav
-000134e0: 6532 292f 3229 0a20 2020 2072 6574 7572  e2)/2).    retur
-000134f0: 6e28 6e70 2e73 756d 2866 6c75 785b 6d61  n(np.sum(flux[ma
-00013500: 736b 5d2a 646e 7529 290a 0a64 6566 2073  sk]*dnu))..def s
-00013510: 7065 6374 7261 6c5f 666c 7578 6573 2877  pectral_fluxes(w
-00013520: 696e 646f 7773 2c77 6176 656c 656e 6774  indows,wavelengt
-00013530: 682c 666c 7578 293a 0a20 2020 2027 2727  h,flux):.    '''
-00013540: 0a20 2020 2052 6574 7572 6e3a 2053 756d  .    Return: Sum
-00013550: 206f 6620 696e 7465 6772 6174 6564 206c   of integrated l
-00013560: 696e 6520 666c 7578 2062 6574 7765 656e  ine flux between
-00013570: 2077 6176 656c 656e 6774 6820 7769 6e64   wavelength wind
-00013580: 6f77 732e 0a20 2020 2055 6e69 743a 2072  ows..    Unit: r
-00013590: 6574 7572 6e20 6973 2069 6e20 5b65 7267  eturn is in [erg
-000135a0: 2f73 2f63 6d32 5d20 616e 6420 696e 7075  /s/cm2] and inpu
-000135b0: 7420 6973 2069 6e20 5b4a 795d 0a20 2020  t is in [Jy].   
-000135c0: 2077 696e 646f 7773 3a20 6c69 7374 206f   windows: list o
-000135d0: 6620 7761 7665 6c65 6e67 7468 206c 696d  f wavelength lim
-000135e0: 6974 7320 286d 6963 726f 6e73 2920 6f66  its (microns) of
-000135f0: 2077 696e 646f 7773 2e20 4578 616d 706c   windows. Exampl
-00013600: 653a 205b 5b31 342c 3134 2e35 5d2c 5b31  e: [[14,14.5],[1
-00013610: 352c 3136 2e32 5d2c 5b31 322e 352c 3134  5,16.2],[12.5,14
-00013620: 2e31 5d5d 0a20 2020 2027 2727 0a20 2020  .1]].    '''.   
-00013630: 2046 203d 205b 5d0a 2020 2020 666f 7220   F = [].    for 
-00013640: 5720 696e 2077 696e 646f 7773 3a0a 2020  W in windows:.  
-00013650: 2020 2020 2020 462e 6170 7065 6e64 2873        F.append(s
-00013660: 7065 6374 7261 6c5f 666c 7578 2857 5b30  pectral_flux(W[0
-00013670: 5d2c 575b 315d 2c77 6176 656c 656e 6774  ],W[1],wavelengt
-00013680: 682c 666c 7578 2929 0a20 2020 2072 6574  h,flux)).    ret
-00013690: 7572 6e28 6e70 2e61 7272 6179 2846 2929  urn(np.array(F))
-000136a0: 0a0a 6465 6620 7370 6563 7472 616c 5f66  ..def spectral_f
-000136b0: 6c75 785f 7261 7469 6f73 2872 6174 696f  lux_ratios(ratio
-000136c0: 5f77 696e 646f 7773 2c77 6176 656c 656e  _windows,wavelen
-000136d0: 6774 682c 666c 7578 293a 0a20 2020 2027  gth,flux):.    '
-000136e0: 2727 0a20 2020 2052 6574 7572 6e3a 2053  ''.    Return: S
-000136f0: 7065 6374 7261 6c20 696e 7465 6772 6174  pectral integrat
-00013700: 6564 2066 6c75 7820 7261 7469 6f73 2062  ed flux ratios b
-00013710: 6574 7765 656e 2077 6176 656c 656e 6774  etween wavelengt
-00013720: 6820 7769 6e64 6f77 732e 200a 2020 2020  h windows. .    
-00013730: 556e 6974 733a 2052 6574 7572 6e20 6973  Units: Return is
-00013740: 2077 6974 686f 7574 2075 6e69 7473 2061   without units a
-00013750: 6e64 2069 6e70 7574 2069 7320 696e 205b  nd input is in [
-00013760: 4a79 5d0a 2020 2020 7261 7469 6f5f 7769  Jy].    ratio_wi
-00013770: 6e64 6f77 733a 206c 6973 7420 6f66 2077  ndows: list of w
-00013780: 6176 656c 656e 6774 6820 286d 6963 726f  avelength (micro
-00013790: 6e73 2920 7769 6e64 6f77 732e 2045 7861  ns) windows. Exa
-000137a0: 6d70 6c65 3a20 5b5b 5b31 342c 3134 2e35  mple: [[[14,14.5
-000137b0: 5d2c 5b31 352c 3136 2e32 5d5d 2c5b 5b31  ],[15,16.2]],[[1
-000137c0: 322e 352c 3134 2e31 5d2c 5b31 332e 342c  2.5,14.1],[13.4,
-000137d0: 3133 2e38 5d5d 5d0a 2020 2020 2727 270a  13.8]]].    '''.
-000137e0: 2020 2020 5220 3d20 5b5d 0a20 2020 2066      R = [].    f
-000137f0: 6f72 2077 696e 646f 7720 696e 2072 6174  or window in rat
-00013800: 696f 5f77 696e 646f 7773 3a0a 2020 2020  io_windows:.    
-00013810: 2020 2020 4620 3d20 7370 6563 7472 616c      F = spectral
-00013820: 5f66 6c75 7865 7328 5b77 696e 646f 775b  _fluxes([window[
-00013830: 305d 2c77 696e 646f 775b 315d 5d2c 7761  0],window[1]],wa
-00013840: 7665 6c65 6e67 7468 2c66 6c75 7829 0a20  velength,flux). 
-00013850: 2020 2020 2020 2052 2e61 7070 656e 6428         R.append(
-00013860: 465b 315d 2f46 5b30 5d29 0a20 2020 2072  F[1]/F[0]).    r
-00013870: 6574 7572 6e28 6e70 2e61 7272 6179 2852  eturn(np.array(R
-00013880: 2929 0a0a 6465 6620 7370 6563 7472 616c  ))..def spectral
-00013890: 5f66 6c75 785f 7072 6f64 7563 7473 2870  _flux_products(p
-000138a0: 726f 6475 6374 5f77 696e 646f 7773 2c77  roduct_windows,w
-000138b0: 6176 656c 656e 6774 682c 666c 7578 293a  avelength,flux):
-000138c0: 0a20 2020 2027 2727 0a20 2020 2052 6574  .    '''.    Ret
-000138d0: 7572 6e3a 2050 726f 6475 6374 7320 6f66  urn: Products of
-000138e0: 2073 7065 6374 7261 6c20 696e 7465 6772   spectral integr
-000138f0: 6174 6564 2066 6c75 7865 7320 6265 7477  ated fluxes betw
-00013900: 6565 6e20 7761 7665 6c65 6e67 7468 2077  een wavelength w
-00013910: 696e 646f 7773 2e20 0a20 2020 2055 6e69  indows. .    Uni
-00013920: 7473 3a20 5265 7475 726e 2075 6e69 7420  ts: Return unit 
-00013930: 6973 206f 7574 7075 7420 756e 6974 7320  is output units 
-00013940: 7371 7561 7265 6420 616e 6420 696e 7075  squared and inpu
-00013950: 7420 6973 2069 6e20 5b4a 795d 0a20 2020  t is in [Jy].   
-00013960: 2070 726f 6475 6374 5f77 696e 646f 7773   product_windows
-00013970: 3a20 6c69 7374 206f 6620 7761 7665 6c65  : list of wavele
-00013980: 6e67 7468 2028 6d69 6372 6f6e 7329 2077  ngth (microns) w
-00013990: 696e 646f 7773 2e20 4578 616d 706c 653a  indows. Example:
-000139a0: 205b 5b5b 3134 2c31 342e 355d 2c5b 3135   [[[14,14.5],[15
-000139b0: 2c31 362e 325d 5d2c 5b5b 3132 2e35 2c31  ,16.2]],[[12.5,1
-000139c0: 342e 315d 2c5b 3133 2e34 2c31 332e 385d  4.1],[13.4,13.8]
-000139d0: 5d5d 0a20 2020 2027 2727 0a20 2020 2052  ]].    '''.    R
-000139e0: 203d 205b 5d0a 2020 2020 666f 7220 7769   = [].    for wi
-000139f0: 6e64 6f77 2069 6e20 7072 6f64 7563 745f  ndow in product_
-00013a00: 7769 6e64 6f77 733a 0a20 2020 2020 2020  windows:.       
-00013a10: 2046 203d 2073 7065 6374 7261 6c5f 666c   F = spectral_fl
-00013a20: 7578 6573 285b 7769 6e64 6f77 5b30 5d2c  uxes([window[0],
-00013a30: 7769 6e64 6f77 5b31 5d5d 2c77 6176 656c  window[1]],wavel
-00013a40: 656e 6774 682c 666c 7578 290a 2020 2020  ength,flux).    
-00013a50: 2020 2020 522e 6170 7065 6e64 2846 5b31      R.append(F[1
-00013a60: 5d2a 465b 305d 290a 2020 2020 7265 7475  ]*F[0]).    retu
-00013a70: 726e 286e 702e 6172 7261 7928 5229 290a  rn(np.array(R)).
-00013a80: 0a64 6566 2063 6869 325f 736c 6162 2873  .def chi2_slab(s
-00013a90: 6c61 625f 6461 7461 2c73 7065 6374 7261  lab_data,spectra
-00013aa0: 2c77 696e 646f 7773 3d5b 5d2c 7261 7469  ,windows=[],rati
-00013ab0: 6f5f 7769 6e64 6f77 733d 5b5d 2c70 726f  o_windows=[],pro
-00013ac0: 6475 6374 5f77 696e 646f 7773 3d5b 5d2c  duct_windows=[],
-00013ad0: 5264 6973 6b3d 6e70 2e6c 6f67 7370 6163  Rdisk=np.logspac
-00013ae0: 6528 2d32 2c32 2c31 3029 2c64 6973 7461  e(-2,2,10),dista
-00013af0: 6e63 653d 3132 302c 636f 6e76 6f6c 7665  nce=120,convolve
-00013b00: 3d46 616c 7365 2c4e 4c54 453d 4661 6c73  =False,NLTE=Fals
-00013b10: 652c 7368 6f72 745f 666f 726d 6174 3d46  e,short_format=F
-00013b20: 616c 7365 293a 0a20 2020 2027 2727 0a20  alse):.    '''. 
-00013b30: 2020 2052 6574 7572 6e73 2063 6869 3220     Returns chi2 
-00013b40: 6261 7365 6420 6f6e 2073 656c 6563 7465  based on selecte
-00013b50: 6420 7370 6563 7472 616c 2077 696e 646f  d spectral windo
-00013b60: 7773 2061 6372 6f73 7320 6469 6666 6572  ws across differ
-00013b70: 656e 7420 656d 6974 7469 6e67 2064 6973  ent emitting dis
-00013b80: 6b20 7261 6469 7573 0a20 2020 2073 6c61  k radius.    sla
-00013b90: 625f 6461 7461 3a20 7061 7468 2063 6f72  b_data: path cor
-00013ba0: 7265 7370 6f6e 6469 6e67 2074 6f20 6120  responding to a 
-00013bb0: 7369 6e67 6c65 2073 6c61 6220 6d6f 6465  single slab mode
-00013bc0: 6c20 6f72 2061 2073 696e 676c 6520 736c  l or a single sl
-00013bd0: 6162 5f6d 6f64 656c 2069 6e73 7461 6e63  ab_model instanc
-00013be0: 650a 2020 2020 7370 6563 7472 613a 206e  e.    spectra: n
-00013bf0: 756d 7079 2061 7272 6179 2077 6974 6820  umpy array with 
-00013c00: 6669 7273 7420 636f 6c75 6d6e 2074 6865  first column the
-00013c10: 2077 6176 656c 656e 6774 6820 696e 205b   wavelength in [
-00013c20: 6d69 6372 6f6e 735d 2061 6e64 2073 6563  microns] and sec
-00013c30: 6f6e 6420 636f 6c75 6d6e 2066 6c75 7820  ond column flux 
-00013c40: 696e 205b 4a79 5d0a 2020 2020 7769 6e64  in [Jy].    wind
-00013c50: 6f77 733a 204c 6973 7420 6f66 2073 7065  ows: List of spe
-00013c60: 6374 7261 6c20 7769 6e64 6f77 7320 666f  ctral windows fo
-00013c70: 7220 6368 6932 2063 616c 6375 6c61 7469  r chi2 calculati
-00013c80: 6f6e 2028 7765 6967 6874 7320 6f70 7469  on (weights opti
-00013c90: 6f6e 616c 290a 2020 2020 2020 2020 2020  onal).          
-00013ca0: 2020 2046 6f72 6d61 743a 205b 7769 6e64     Format: [wind
-00013cb0: 6f77 312c 7769 6e64 6f77 322c 2e2e 2e2e  ow1,window2,....
-00013cc0: 5d0a 2020 2020 2020 2020 2020 2020 2057  ].             W
-00013cd0: 696e 646f 7720 666f 726d 6174 3a20 5b6c  indow format: [l
-00013ce0: 616d 6264 615f 302c 206c 616d 6264 615f  ambda_0, lambda_
-00013cf0: 312c 2077 6569 6768 745d 0a20 2020 2020  1, weight].     
-00013d00: 2020 2020 2020 2020 7765 6967 6874 2069          weight i
-00013d10: 7320 6f70 7469 6f6e 616c 2c20 7573 6564  s optional, used
-00013d20: 2066 6f72 2077 6569 6768 7465 6420 6368   for weighted ch
-00013d30: 6932 0a20 2020 2020 2020 2020 2020 2020  i2.             
-00013d40: 4578 616d 706c 6520 7769 7468 6f75 7420  Example without 
-00013d50: 7765 6967 6874 3a20 5b5b 3134 2c31 342e  weight: [[14,14.
-00013d60: 355d 2c5b 3135 2c31 362e 325d 2c5b 3132  5],[15,16.2],[12
-00013d70: 2e35 2c31 342e 315d 5d0a 2020 2020 2020  .5,14.1]].      
-00013d80: 2020 2020 2020 2045 7861 6d70 6c65 2077         Example w
-00013d90: 6974 6820 7765 6967 6874 3a20 5b5b 3134  ith weight: [[14
-00013da0: 2c31 342e 352c 325d 2c5b 3135 2c31 362e  ,14.5,2],[15,16.
-00013db0: 322c 355d 2c5b 3132 2e35 2c31 342e 312c  2,5],[12.5,14.1,
-00013dc0: 315d 5d0a 2020 2020 2020 2020 2020 2020  1]].            
-00013dd0: 2057 6569 6768 7473 2061 7265 2061 7574   Weights are aut
-00013de0: 6f6d 6174 6963 616c 6c79 206e 6f72 6d61  omatically norma
-00013df0: 6c69 7365 642c 2073 6f20 7375 6d20 6f66  lised, so sum of
-00013e00: 2077 6569 6768 7473 206e 6565 6420 6e6f   weights need no
-00013e10: 7420 6265 2031 0a20 2020 2052 6469 736b  t be 1.    Rdisk
-00013e20: 3a20 5261 6469 7573 2063 6f72 7265 7370  : Radius corresp
-00013e30: 6f6e 6469 6e67 2074 6f20 656d 6974 7469  onding to emitti
-00013e40: 6e67 2061 7265 6120 696e 2061 7374 726f  ng area in astro
-00013e50: 6e6f 6d69 6361 6c20 756e 6974 730a 2020  nomical units.  
-00013e60: 2020 6469 7374 616e 6365 3a20 6469 7374    distance: dist
-00013e70: 616e 6365 206f 6620 6469 736b 2069 6e20  ance of disk in 
-00013e80: 7061 7273 6563 0a20 2020 2063 6f6e 766f  parsec.    convo
-00013e90: 6c76 653a 2049 6620 5472 7565 2c20 7468  lve: If True, th
-00013ea0: 6520 6368 6932 2069 7320 7065 7266 6f72  e chi2 is perfor
-00013eb0: 6d65 6420 6f6e 2063 6f6e 766f 6c76 6564  med on convolved
-00013ec0: 2073 7065 6374 7261 2061 6e64 206e 6f74   spectra and not
-00013ed0: 206f 6e20 696e 6469 7669 6475 616c 206c   on individual l
-00013ee0: 696e 6573 0a20 2020 204e 4c54 453a 2069  ines.    NLTE: i
-00013ef0: 6620 5472 7565 2c20 4e4c 5445 2066 6c75  f True, NLTE flu
-00013f00: 7820 6973 2074 616b 656e 2066 726f 6d20  x is taken from 
-00013f10: 7468 6520 736c 6162 206d 6f64 656c 2e0a  the slab model..
-00013f20: 2020 2020 2727 270a 2020 2020 6172 6561      '''.    area
-00013f30: 203d 206e 702e 7069 2a28 5264 6973 6b2a   = np.pi*(Rdisk*
-00013f40: 6175 2f64 6973 7461 6e63 652f 7063 292a  au/distance/pc)*
-00013f50: 2a32 0a20 2020 2063 6869 5f61 7265 6120  *2.    chi_area 
-00013f60: 3d20 6e70 2e7a 6572 6f73 2828 6c65 6e28  = np.zeros((len(
-00013f70: 6172 6561 2929 290a 2020 2020 6966 2069  area))).    if i
-00013f80: 7369 6e73 7461 6e63 6528 736c 6162 5f64  sinstance(slab_d
-00013f90: 6174 612c 7374 7229 3a20 736c 6162 5f64  ata,str): slab_d
-00013fa0: 6174 6120 3d20 7265 6164 5f73 6c61 6228  ata = read_slab(
-00013fb0: 736c 6162 5f64 6174 612c 7665 7262 6f73  slab_data,verbos
-00013fc0: 653d 4661 6c73 652c 7368 6f72 745f 666f  e=False,short_fo
-00013fd0: 726d 6174 3d73 686f 7274 5f66 6f72 6d61  rmat=short_forma
-00013fe0: 7429 0a20 2020 2069 6620 6c65 6e28 7769  t).    if len(wi
-00013ff0: 6e64 6f77 7329 3c30 2061 6e64 206c 656e  ndows)<0 and len
-00014000: 2872 6174 696f 5f77 696e 646f 7773 293c  (ratio_windows)<
-00014010: 3020 616e 6420 6c65 6e28 7072 6f64 7563  0 and len(produc
-00014020: 745f 7769 6e64 6f77 7329 3c30 3a20 7265  t_windows)<0: re
-00014030: 7475 726e 2063 6869 5f61 7265 610a 2020  turn chi_area.  
-00014040: 2020 6966 2063 6f6e 766f 6c76 653a 2020    if convolve:  
-00014050: 2320 746f 2065 7374 696d 6174 6520 666c  # to estimate fl
-00014060: 7578 2066 726f 6d20 636f 6e76 6f6c 7665  ux from convolve
-00014070: 6420 7370 6563 7472 610a 2020 2020 2020  d spectra.      
-00014080: 2020 6c6d 696e 2c6c 6d61 7820 3d20 5b5d    lmin,lmax = []
-00014090: 2c5b 5d0a 2020 2020 2020 2020 6966 206c  ,[].        if l
-000140a0: 656e 2877 696e 646f 7773 293e 303a 0a20  en(windows)>0:. 
-000140b0: 2020 2020 2020 2020 2020 206c 6d69 6e2e             lmin.
-000140c0: 6170 7065 6e64 286e 702e 616d 696e 286e  append(np.amin(n
-000140d0: 702e 6172 7261 7928 5b5b 695b 305d 2c69  p.array([[i[0],i
-000140e0: 5b31 5d5d 2066 6f72 2069 2069 6e20 7769  [1]] for i in wi
-000140f0: 6e64 6f77 735d 292e 666c 6174 7465 6e28  ndows]).flatten(
-00014100: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-00014110: 6c6d 6178 2e61 7070 656e 6428 6e70 2e61  lmax.append(np.a
-00014120: 6d61 7828 6e70 2e61 7272 6179 285b 5b69  max(np.array([[i
-00014130: 5b30 5d2c 695b 315d 5d20 666f 7220 6920  [0],i[1]] for i 
-00014140: 696e 2077 696e 646f 7773 5d29 2e66 6c61  in windows]).fla
-00014150: 7474 656e 2829 2929 0a20 2020 2020 2020  tten())).       
-00014160: 2069 6620 6c65 6e28 7261 7469 6f5f 7769   if len(ratio_wi
-00014170: 6e64 6f77 7329 3e30 3a0a 2020 2020 2020  ndows)>0:.      
-00014180: 2020 2020 2020 6c6d 696e 2e61 7070 656e        lmin.appen
-00014190: 6428 6e70 2e61 6d69 6e28 6e70 2e61 7272  d(np.amin(np.arr
-000141a0: 6179 285b 5b69 5b30 5d2c 695b 315d 5d20  ay([[i[0],i[1]] 
-000141b0: 666f 7220 6920 696e 2072 6174 696f 5f77  for i in ratio_w
-000141c0: 696e 646f 7773 5d29 2e66 6c61 7474 656e  indows]).flatten
-000141d0: 2829 2929 0a20 2020 2020 2020 2020 2020  ())).           
-000141e0: 206c 6d61 782e 6170 7065 6e64 286e 702e   lmax.append(np.
-000141f0: 616d 6178 286e 702e 6172 7261 7928 5b5b  amax(np.array([[
-00014200: 695b 305d 2c69 5b31 5d5d 2066 6f72 2069  i[0],i[1]] for i
-00014210: 2069 6e20 7261 7469 6f5f 7769 6e64 6f77   in ratio_window
-00014220: 735d 292e 666c 6174 7465 6e28 2929 290a  s]).flatten())).
-00014230: 2020 2020 2020 2020 6966 206c 656e 2870          if len(p
-00014240: 726f 6475 6374 5f77 696e 646f 7773 293e  roduct_windows)>
-00014250: 303a 0a20 2020 2020 2020 2020 2020 206c  0:.            l
-00014260: 6d69 6e2e 6170 7065 6e64 286e 702e 616d  min.append(np.am
-00014270: 696e 286e 702e 6172 7261 7928 5b5b 695b  in(np.array([[i[
-00014280: 305d 2c69 5b31 5d5d 2066 6f72 2069 2069  0],i[1]] for i i
-00014290: 6e20 7072 6f64 7563 745f 7769 6e64 6f77  n product_window
-000142a0: 735d 292e 666c 6174 7465 6e28 2929 290a  s]).flatten())).
-000142b0: 2020 2020 2020 2020 2020 2020 6c6d 6178              lmax
-000142c0: 2e61 7070 656e 6428 6e70 2e61 6d61 7828  .append(np.amax(
-000142d0: 6e70 2e61 7272 6179 285b 5b69 5b30 5d2c  np.array([[i[0],
-000142e0: 695b 315d 5d20 666f 7220 6920 696e 2070  i[1]] for i in p
-000142f0: 726f 6475 6374 5f77 696e 646f 7773 5d29  roduct_windows])
-00014300: 2e66 6c61 7474 656e 2829 2929 0a20 2020  .flatten())).   
-00014310: 2020 2020 206c 6d69 6e20 3d20 6e70 2e61       lmin = np.a
-00014320: 6d69 6e28 6c6d 696e 290a 2020 2020 2020  min(lmin).      
-00014330: 2020 6c6d 6178 203d 206e 702e 616d 6178    lmax = np.amax
-00014340: 286c 6d61 7829 0a20 2020 2020 2020 2073  (lmax).        s
-00014350: 6c61 625f 6461 7461 2e63 6f6e 766f 6c76  lab_data.convolv
-00014360: 6528 523d 3230 3030 2c6c 616d 6264 615f  e(R=2000,lambda_
-00014370: 303d 6c6d 696e 2a30 2e39 2c6c 616d 6264  0=lmin*0.9,lambd
-00014380: 615f 6e3d 6c6d 6178 2a31 2e31 2c4e 4c54  a_n=lmax*1.1,NLT
-00014390: 453d 4e4c 5445 2c76 6572 626f 7365 3d46  E=NLTE,verbose=F
-000143a0: 616c 7365 290a 2020 2020 2020 2020 6966  alse).        if
-000143b0: 204e 4c54 453a 0a20 2020 2020 2020 2020   NLTE:.         
-000143c0: 2020 2046 6d6f 6465 6c20 3d20 7370 6563     Fmodel = spec
-000143d0: 7472 616c 5f66 6c75 7865 7328 7769 6e64  tral_fluxes(wind
-000143e0: 6f77 732c 736c 6162 5f64 6174 612e 636f  ows,slab_data.co
-000143f0: 6e76 5761 7665 6c65 6e67 7468 2c73 6c61  nvWavelength,sla
-00014400: 625f 6461 7461 2e63 6f6e 764e 4c54 4566  b_data.convNLTEf
-00014410: 6c75 782a 3165 3233 290a 2020 2020 2020  lux*1e23).      
-00014420: 2020 2020 2020 526d 6f64 656c 203d 2073        Rmodel = s
-00014430: 7065 6374 7261 6c5f 666c 7578 5f72 6174  pectral_flux_rat
-00014440: 696f 7328 7261 7469 6f5f 7769 6e64 6f77  ios(ratio_window
-00014450: 732c 736c 6162 5f64 6174 612e 636f 6e76  s,slab_data.conv
-00014460: 5761 7665 6c65 6e67 7468 2c73 6c61 625f  Wavelength,slab_
-00014470: 6461 7461 2e63 6f6e 764e 4c54 4566 6c75  data.convNLTEflu
-00014480: 782a 3165 3233 290a 2020 2020 2020 2020  x*1e23).        
-00014490: 2020 2020 506d 6f64 656c 203d 2073 7065      Pmodel = spe
-000144a0: 6374 7261 6c5f 666c 7578 5f70 726f 6475  ctral_flux_produ
-000144b0: 6374 7328 7072 6f64 7563 745f 7769 6e64  cts(product_wind
-000144c0: 6f77 732c 736c 6162 5f64 6174 612e 636f  ows,slab_data.co
-000144d0: 6e76 5761 7665 6c65 6e67 7468 2c73 6c61  nvWavelength,sla
-000144e0: 625f 6461 7461 2e63 6f6e 764e 4c54 4566  b_data.convNLTEf
-000144f0: 6c75 782a 3165 3233 290a 2020 2020 2020  lux*1e23).      
-00014500: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00014510: 2020 2020 466d 6f64 656c 203d 2073 7065      Fmodel = spe
-00014520: 6374 7261 6c5f 666c 7578 6573 2877 696e  ctral_fluxes(win
-00014530: 646f 7773 2c73 6c61 625f 6461 7461 2e63  dows,slab_data.c
-00014540: 6f6e 7657 6176 656c 656e 6774 682c 736c  onvWavelength,sl
-00014550: 6162 5f64 6174 612e 636f 6e76 4c54 4566  ab_data.convLTEf
-00014560: 6c75 782a 3165 3233 290a 2020 2020 2020  lux*1e23).      
-00014570: 2020 2020 2020 526d 6f64 656c 203d 2073        Rmodel = s
-00014580: 7065 6374 7261 6c5f 666c 7578 5f72 6174  pectral_flux_rat
-00014590: 696f 7328 7261 7469 6f5f 7769 6e64 6f77  ios(ratio_window
-000145a0: 732c 736c 6162 5f64 6174 612e 636f 6e76  s,slab_data.conv
-000145b0: 5761 7665 6c65 6e67 7468 2c73 6c61 625f  Wavelength,slab_
-000145c0: 6461 7461 2e63 6f6e 764c 5445 666c 7578  data.convLTEflux
-000145d0: 2a31 6532 3329 0a20 2020 2020 2020 2020  *1e23).         
-000145e0: 2020 2050 6d6f 6465 6c20 3d20 7370 6563     Pmodel = spec
-000145f0: 7472 616c 5f66 6c75 785f 7072 6f64 7563  tral_flux_produc
-00014600: 7473 2870 726f 6475 6374 5f77 696e 646f  ts(product_windo
-00014610: 7773 2c73 6c61 625f 6461 7461 2e63 6f6e  ws,slab_data.con
-00014620: 7657 6176 656c 656e 6774 682c 736c 6162  vWavelength,slab
-00014630: 5f64 6174 612e 636f 6e76 4c54 4566 6c75  _data.convLTEflu
-00014640: 782a 3165 3233 290a 2020 2020 656c 7365  x*1e23).    else
-00014650: 3a20 2023 2074 6f20 6573 7469 6d61 7465  :  # to estimate
-00014660: 2066 6c75 7820 6672 6f6d 206c 696e 6520   flux from line 
-00014670: 6c69 7374 0a20 2020 2020 2020 2069 6620  list.        if 
-00014680: 4e4c 5445 3a0a 2020 2020 2020 2020 2020  NLTE:.          
-00014690: 2020 7420 3d20 2746 4e4c 5445 270a 2020    t = 'FNLTE'.  
-000146a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000146b0: 2020 2020 2020 2020 7420 3d20 2746 4c54          t = 'FLT
-000146c0: 4527 0a20 2020 2020 2020 206c 696e 6564  E'.        lined
-000146d0: 6174 6120 3d20 736c 6162 5f64 6174 612e  ata = slab_data.
-000146e0: 6c69 6e65 6461 7461 0a20 2020 2020 2020  linedata.       
-000146f0: 206c 696e 6564 6174 612e 736f 7274 5f76   linedata.sort_v
-00014700: 616c 7565 7328 6279 3d5b 2747 487a 275d  alues(by=['GHz']
-00014710: 2c20 6173 6365 6e64 696e 673d 4661 6c73  , ascending=Fals
-00014720: 652c 2069 6e70 6c61 6365 3d54 7275 652c  e, inplace=True,
-00014730: 2069 676e 6f72 655f 696e 6465 783d 5472   ignore_index=Tr
-00014740: 7565 290a 2020 2020 2020 2020 466d 6f64  ue).        Fmod
-00014750: 656c 203d 206c 696e 655f 666c 7578 6573  el = line_fluxes
-00014760: 2877 696e 646f 7773 2c63 2f6c 696e 6564  (windows,c/lined
-00014770: 6174 615b 2747 487a 275d 2a31 652d 332c  ata['GHz']*1e-3,
-00014780: 6c69 6e65 6461 7461 5b74 5d29 0a20 2020  linedata[t]).   
-00014790: 2020 2020 2052 6d6f 6465 6c20 3d20 6c69       Rmodel = li
-000147a0: 6e65 5f66 6c75 785f 7261 7469 6f73 2872  ne_flux_ratios(r
-000147b0: 6174 696f 5f77 696e 646f 7773 2c63 2f6c  atio_windows,c/l
-000147c0: 696e 6564 6174 615b 2747 487a 275d 2a31  inedata['GHz']*1
-000147d0: 652d 332c 6c69 6e65 6461 7461 5b74 5d29  e-3,linedata[t])
-000147e0: 0a20 2020 2020 2020 2050 6d6f 6465 6c20  .        Pmodel 
-000147f0: 3d20 6c69 6e65 5f66 6c75 785f 7261 7469  = line_flux_rati
-00014800: 6f73 2870 726f 6475 6374 5f77 696e 646f  os(product_windo
-00014810: 7773 2c63 2f6c 696e 6564 6174 615b 2747  ws,c/linedata['G
-00014820: 487a 275d 2a31 652d 332c 6c69 6e65 6461  Hz']*1e-3,lineda
-00014830: 7461 5b74 5d29 0a20 2020 2046 6f62 7365  ta[t]).    Fobse
-00014840: 7276 6564 203d 2073 7065 6374 7261 6c5f  rved = spectral_
-00014850: 666c 7578 6573 2877 696e 646f 7773 2c73  fluxes(windows,s
-00014860: 7065 6374 7261 5b3a 2c30 5d2c 7370 6563  pectra[:,0],spec
-00014870: 7472 615b 3a2c 315d 290a 2020 2020 526f  tra[:,1]).    Ro
-00014880: 6273 6572 7665 6420 3d20 7370 6563 7472  bserved = spectr
-00014890: 616c 5f66 6c75 785f 7261 7469 6f73 2872  al_flux_ratios(r
-000148a0: 6174 696f 5f77 696e 646f 7773 2c73 7065  atio_windows,spe
-000148b0: 6374 7261 5b3a 2c30 5d2c 7370 6563 7472  ctra[:,0],spectr
-000148c0: 615b 3a2c 315d 290a 2020 2020 506f 6273  a[:,1]).    Pobs
-000148d0: 6572 7665 6420 3d20 7370 6563 7472 616c  erved = spectral
-000148e0: 5f66 6c75 785f 7072 6f64 7563 7473 2870  _flux_products(p
-000148f0: 726f 6475 6374 5f77 696e 646f 7773 2c73  roduct_windows,s
-00014900: 7065 6374 7261 5b3a 2c30 5d2c 7370 6563  pectra[:,0],spec
-00014910: 7472 615b 3a2c 315d 290a 2020 2020 6e6f  tra[:,1]).    no
-00014920: 726d 5f66 6163 746f 7220 3d20 300a 2020  rm_factor = 0.  
-00014930: 2020 6966 206c 656e 2877 696e 646f 7773    if len(windows
-00014940: 293e 303a 0a20 2020 2020 2020 2061 7265  )>0:.        are
-00014950: 615f 3264 2020 2020 2020 3d20 6e70 2e64  a_2d      = np.d
-00014960: 7374 6163 6b28 5b61 7265 6120 666f 7220  stack([area for 
-00014970: 6920 696e 2072 616e 6765 286c 656e 2877  i in range(len(w
-00014980: 696e 646f 7773 2929 5d29 2e73 7175 6565  indows))]).squee
-00014990: 7a65 2829 2e72 6573 6861 7065 2828 6c65  ze().reshape((le
-000149a0: 6e28 6172 6561 292c 6c65 6e28 7769 6e64  n(area),len(wind
-000149b0: 6f77 7329 2929 0a20 2020 2020 2020 2046  ows))).        F
-000149c0: 6d6f 6465 6c5f 3264 2020 2020 3d20 6e70  model_2d    = np
-000149d0: 2e64 7374 6163 6b28 5b46 6d6f 6465 6c20  .dstack([Fmodel 
-000149e0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-000149f0: 656e 2861 7265 6129 295d 292e 7371 7565  en(area))]).sque
-00014a00: 657a 6528 292e 542e 7265 7368 6170 6528  eze().T.reshape(
-00014a10: 286c 656e 2861 7265 6129 2c6c 656e 2877  (len(area),len(w
-00014a20: 696e 646f 7773 2929 290a 2020 2020 2020  indows))).      
-00014a30: 2020 466f 6273 6572 7665 645f 3264 203d    Fobserved_2d =
-00014a40: 206e 702e 6473 7461 636b 285b 466f 6273   np.dstack([Fobs
-00014a50: 6572 7665 6420 666f 7220 6920 696e 2072  erved for i in r
-00014a60: 616e 6765 286c 656e 2861 7265 6129 295d  ange(len(area))]
-00014a70: 292e 7371 7565 657a 6528 292e 542e 7265  ).squeeze().T.re
-00014a80: 7368 6170 6528 286c 656e 2861 7265 6129  shape((len(area)
-00014a90: 2c6c 656e 2877 696e 646f 7773 2929 290a  ,len(windows))).
-00014aa0: 2020 2020 2020 2020 6966 206c 656e 2877          if len(w
-00014ab0: 696e 646f 7773 5b30 5d29 3d3d 333a 2023  indows[0])==3: #
-00014ac0: 7765 6967 6874 6564 2063 6869 320a 2020  weighted chi2.  
-00014ad0: 2020 2020 2020 2020 2020 7769 6e64 6f77            window
-00014ae0: 735f 7765 6967 6874 7320 2020 203d 206e  s_weights    = n
-00014af0: 702e 6172 7261 7928 5b77 696e 646f 7773  p.array([windows
-00014b00: 5b6b 5d5b 325d 2066 6f72 206b 2069 6e20  [k][2] for k in 
-00014b10: 7261 6e67 6528 6c65 6e28 7769 6e64 6f77  range(len(window
-00014b20: 7329 295d 290a 2020 2020 2020 2020 2020  s))]).          
-00014b30: 2020 7769 6e64 6f77 735f 7765 6967 6874    windows_weight
-00014b40: 735f 3264 203d 206e 702e 6473 7461 636b  s_2d = np.dstack
-00014b50: 285b 7769 6e64 6f77 735f 7765 6967 6874  ([windows_weight
-00014b60: 7320 666f 7220 6920 696e 2072 616e 6765  s for i in range
-00014b70: 286c 656e 2861 7265 6129 295d 292e 7371  (len(area))]).sq
-00014b80: 7565 657a 6528 292e 542e 7265 7368 6170  ueeze().T.reshap
-00014b90: 6528 286c 656e 2861 7265 6129 2c6c 656e  e((len(area),len
-00014ba0: 2877 696e 646f 7773 5f77 6569 6768 7473  (windows_weights
-00014bb0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-00014bc0: 6368 695f 6172 6561 2020 2020 2020 2020  chi_area        
-00014bd0: 2020 2b3d 206e 702e 7375 6d28 2828 466d    += np.sum(((Fm
-00014be0: 6f64 656c 5f32 642a 6172 6561 5f32 642d  odel_2d*area_2d-
-00014bf0: 466f 6273 6572 7665 645f 3264 292f 466f  Fobserved_2d)/Fo
-00014c00: 6273 6572 7665 645f 3264 292a 2a32 2a77  bserved_2d)**2*w
-00014c10: 696e 646f 7773 5f77 6569 6768 7473 5f32  indows_weights_2
-00014c20: 642c 6178 6973 3d31 290a 2020 2020 2020  d,axis=1).      
-00014c30: 2020 2020 2020 6e6f 726d 5f66 6163 746f        norm_facto
-00014c40: 7220 2020 2020 2020 2b3d 206e 702e 7375  r       += np.su
-00014c50: 6d28 7769 6e64 6f77 735f 7765 6967 6874  m(windows_weight
-00014c60: 7329 0a20 2020 2020 2020 2065 6c73 653a  s).        else:
-00014c70: 0a20 2020 2020 2020 2020 2020 2063 6869  .            chi
-00014c80: 5f61 7265 6120 2020 2020 202b 3d20 6e70  _area      += np
-00014c90: 2e73 756d 2828 2846 6d6f 6465 6c5f 3264  .sum(((Fmodel_2d
-00014ca0: 2a61 7265 615f 3264 2d46 6f62 7365 7276  *area_2d-Fobserv
-00014cb0: 6564 5f32 6429 2f46 6f62 7365 7276 6564  ed_2d)/Fobserved
-00014cc0: 5f32 6429 2a2a 322c 6178 6973 3d31 290a  _2d)**2,axis=1).
-00014cd0: 2020 2020 2020 2020 2020 2020 6e6f 726d              norm
-00014ce0: 5f66 6163 746f 7220 2020 2b3d 206c 656e  _factor   += len
-00014cf0: 2877 696e 646f 7773 290a 2020 2020 6966  (windows).    if
-00014d00: 206c 656e 2872 6174 696f 5f77 696e 646f   len(ratio_windo
-00014d10: 7773 293e 303a 200a 2020 2020 2020 2020  ws)>0: .        
-00014d20: 526d 6f64 656c 5f32 6420 2020 203d 206e  Rmodel_2d    = n
-00014d30: 702e 6473 7461 636b 285b 526d 6f64 656c  p.dstack([Rmodel
-00014d40: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00014d50: 6c65 6e28 6172 6561 2929 5d29 2e73 7175  len(area))]).squ
-00014d60: 6565 7a65 2829 2e54 2e72 6573 6861 7065  eeze().T.reshape
-00014d70: 2828 6c65 6e28 6172 6561 292c 6c65 6e28  ((len(area),len(
-00014d80: 7261 7469 6f5f 7769 6e64 6f77 7329 2929  ratio_windows)))
-00014d90: 0a20 2020 2020 2020 2052 6f62 7365 7276  .        Robserv
-00014da0: 6564 5f32 6420 3d20 6e70 2e64 7374 6163  ed_2d = np.dstac
-00014db0: 6b28 5b52 6f62 7365 7276 6564 2066 6f72  k([Robserved for
-00014dc0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00014dd0: 6172 6561 2929 5d29 2e73 7175 6565 7a65  area))]).squeeze
-00014de0: 2829 2e54 2e72 6573 6861 7065 2828 6c65  ().T.reshape((le
-00014df0: 6e28 6172 6561 292c 6c65 6e28 7261 7469  n(area),len(rati
-00014e00: 6f5f 7769 6e64 6f77 7329 2929 0a20 2020  o_windows))).   
-00014e10: 2020 2020 2069 6620 286c 656e 2872 6174       if (len(rat
-00014e20: 696f 5f77 696e 646f 7773 5b30 5d29 3d3d  io_windows[0])==
-00014e30: 3329 3a20 2377 6569 6768 7465 6420 6368  3): #weighted ch
-00014e40: 6932 0a20 2020 2020 2020 2020 2020 2072  i2.            r
-00014e50: 6174 696f 5f77 696e 646f 7773 5f77 6569  atio_windows_wei
-00014e60: 6768 7473 2020 2020 3d20 6e70 2e61 7272  ghts    = np.arr
-00014e70: 6179 285b 7261 7469 6f5f 7769 6e64 6f77  ay([ratio_window
-00014e80: 735b 6b5d 5b32 5d20 666f 7220 6b20 696e  s[k][2] for k in
-00014e90: 2072 616e 6765 286c 656e 2872 6174 696f   range(len(ratio
-00014ea0: 5f77 696e 646f 7773 2929 5d29 0a20 2020  _windows))]).   
-00014eb0: 2020 2020 2020 2020 2072 6174 696f 5f77           ratio_w
-00014ec0: 696e 646f 7773 5f77 6569 6768 7473 5f32  indows_weights_2
-00014ed0: 6420 3d20 6e70 2e64 7374 6163 6b28 5b72  d = np.dstack([r
-00014ee0: 6174 696f 5f77 696e 646f 7773 5f77 6569  atio_windows_wei
-00014ef0: 6768 7473 2066 6f72 2069 2069 6e20 7261  ghts for i in ra
-00014f00: 6e67 6528 6c65 6e28 6172 6561 2929 5d29  nge(len(area))])
-00014f10: 2e73 7175 6565 7a65 2829 2e54 2e72 6573  .squeeze().T.res
-00014f20: 6861 7065 2828 6c65 6e28 6172 6561 292c  hape((len(area),
-00014f30: 6c65 6e28 7261 7469 6f5f 7769 6e64 6f77  len(ratio_window
-00014f40: 735f 7765 6967 6874 7329 2929 0a20 2020  s_weights))).   
-00014f50: 2020 2020 2020 2020 2063 6869 5f61 7265           chi_are
-00014f60: 6120 2020 2020 2020 2020 2020 2020 2020  a               
-00014f70: 202b 3d20 6e70 2e73 756d 2828 2852 6d6f   += np.sum(((Rmo
-00014f80: 6465 6c5f 3264 2d52 6f62 7365 7276 6564  del_2d-Robserved
-00014f90: 5f32 6429 2f52 6f62 7365 7276 6564 5f32  _2d)/Robserved_2
-00014fa0: 6429 2a2a 322a 7261 7469 6f5f 7769 6e64  d)**2*ratio_wind
-00014fb0: 6f77 735f 7765 6967 6874 735f 3264 2c61  ows_weights_2d,a
-00014fc0: 7869 733d 3129 0a20 2020 2020 2020 2020  xis=1).         
-00014fd0: 2020 206e 6f72 6d5f 6661 6374 6f72 2020     norm_factor  
-00014fe0: 2020 2020 2020 2020 2020 202b 3d20 6e70             += np
-00014ff0: 2e73 756d 2872 6174 696f 5f77 696e 646f  .sum(ratio_windo
-00015000: 7773 5f77 6569 6768 7473 290a 2020 2020  ws_weights).    
-00015010: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00015020: 2020 2020 2020 6368 695f 6172 6561 2020        chi_area  
-00015030: 2020 2020 2b3d 206e 702e 7375 6d28 2828      += np.sum(((
-00015040: 526d 6f64 656c 5f32 642d 526f 6273 6572  Rmodel_2d-Robser
-00015050: 7665 645f 3264 292f 526f 6273 6572 7665  ved_2d)/Robserve
-00015060: 645f 3264 292a 2a32 2c61 7869 733d 3129  d_2d)**2,axis=1)
-00015070: 0a20 2020 2020 2020 2020 2020 206e 6f72  .            nor
-00015080: 6d5f 6661 6374 6f72 2020 202b 3d20 6c65  m_factor   += le
-00015090: 6e28 7261 7469 6f5f 7769 6e64 6f77 7329  n(ratio_windows)
-000150a0: 0a20 2020 2069 6620 6c65 6e28 7072 6f64  .    if len(prod
-000150b0: 7563 745f 7769 6e64 6f77 7329 3e30 3a20  uct_windows)>0: 
-000150c0: 0a20 2020 2020 2020 2061 7265 615f 3264  .        area_2d
-000150d0: 2020 2020 2020 3d20 6e70 2e64 7374 6163        = np.dstac
-000150e0: 6b28 5b61 7265 6120 666f 7220 6920 696e  k([area for i in
-000150f0: 2072 616e 6765 286c 656e 2870 726f 6475   range(len(produ
-00015100: 6374 5f77 696e 646f 7773 2929 5d29 2e73  ct_windows))]).s
-00015110: 7175 6565 7a65 2829 2e72 6573 6861 7065  queeze().reshape
-00015120: 2828 6c65 6e28 6172 6561 292c 6c65 6e28  ((len(area),len(
-00015130: 7072 6f64 7563 745f 7769 6e64 6f77 7329  product_windows)
-00015140: 2929 0a20 2020 2020 2020 2050 6d6f 6465  )).        Pmode
-00015150: 6c5f 3264 2020 2020 3d20 6e70 2e64 7374  l_2d    = np.dst
-00015160: 6163 6b28 5b50 6d6f 6465 6c20 666f 7220  ack([Pmodel for 
-00015170: 6920 696e 2072 616e 6765 286c 656e 2861  i in range(len(a
-00015180: 7265 6129 295d 292e 7371 7565 657a 6528  rea))]).squeeze(
-00015190: 292e 542e 7265 7368 6170 6528 286c 656e  ).T.reshape((len
-000151a0: 2861 7265 6129 2c6c 656e 2870 726f 6475  (area),len(produ
-000151b0: 6374 5f77 696e 646f 7773 2929 290a 2020  ct_windows))).  
-000151c0: 2020 2020 2020 506f 6273 6572 7665 645f        Pobserved_
-000151d0: 3264 203d 206e 702e 6473 7461 636b 285b  2d = np.dstack([
-000151e0: 506f 6273 6572 7665 6420 666f 7220 6920  Pobserved for i 
-000151f0: 696e 2072 616e 6765 286c 656e 2861 7265  in range(len(are
-00015200: 6129 295d 292e 7371 7565 657a 6528 292e  a))]).squeeze().
-00015210: 542e 7265 7368 6170 6528 286c 656e 2861  T.reshape((len(a
-00015220: 7265 6129 2c6c 656e 2870 726f 6475 6374  rea),len(product
-00015230: 5f77 696e 646f 7773 2929 290a 2020 2020  _windows))).    
-00015240: 2020 2020 6966 2028 6c65 6e28 7072 6f64      if (len(prod
-00015250: 7563 745f 7769 6e64 6f77 735b 305d 293d  uct_windows[0])=
-00015260: 3d33 293a 2023 7765 6967 6874 6564 2063  =3): #weighted c
-00015270: 6869 320a 2020 2020 2020 2020 2020 2020  hi2.            
-00015280: 7072 6f64 7563 745f 7769 6e64 6f77 735f  product_windows_
-00015290: 7765 6967 6874 7320 2020 203d 206e 702e  weights    = np.
-000152a0: 6172 7261 7928 5b70 726f 6475 6374 5f77  array([product_w
-000152b0: 696e 646f 7773 5b6b 5d5b 325d 2066 6f72  indows[k][2] for
-000152c0: 206b 2069 6e20 7261 6e67 6528 6c65 6e28   k in range(len(
-000152d0: 7072 6f64 7563 745f 7769 6e64 6f77 7329  product_windows)
-000152e0: 295d 290a 2020 2020 2020 2020 2020 2020  )]).            
-000152f0: 7072 6f64 7563 745f 7769 6e64 6f77 735f  product_windows_
-00015300: 7765 6967 6874 735f 3264 203d 206e 702e  weights_2d = np.
-00015310: 6473 7461 636b 285b 7072 6f64 7563 745f  dstack([product_
-00015320: 7769 6e64 6f77 735f 7765 6967 6874 7320  windows_weights 
-00015330: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00015340: 656e 2861 7265 6129 295d 292e 7371 7565  en(area))]).sque
-00015350: 657a 6528 292e 542e 7265 7368 6170 6528  eze().T.reshape(
-00015360: 286c 656e 2861 7265 6129 2c6c 656e 2870  (len(area),len(p
-00015370: 726f 6475 6374 5f77 696e 646f 7773 5f77  roduct_windows_w
-00015380: 6569 6768 7473 2929 290a 2020 2020 2020  eights))).      
-00015390: 2020 2020 2020 6368 695f 6172 6561 2020        chi_area  
-000153a0: 2020 2020 2020 2020 2020 2020 2020 2b3d                +=
-000153b0: 206e 702e 7375 6d28 2828 2850 6d6f 6465   np.sum((((Pmode
-000153c0: 6c5f 3264 2a61 7265 615f 3264 2a2a 3229  l_2d*area_2d**2)
-000153d0: 2a2a 302e 352d 2850 6f62 7365 7276 6564  **0.5-(Pobserved
-000153e0: 5f32 6429 2a2a 302e 3529 2f28 506f 6273  _2d)**0.5)/(Pobs
-000153f0: 6572 7665 645f 3264 292a 2a30 2e35 292a  erved_2d)**0.5)*
-00015400: 2a32 2a70 726f 6475 6374 5f77 696e 646f  *2*product_windo
-00015410: 7773 5f77 6569 6768 7473 5f32 642c 6178  ws_weights_2d,ax
-00015420: 6973 3d31 290a 2020 2020 2020 2020 2020  is=1).          
-00015430: 2020 6e6f 726d 5f66 6163 746f 7220 2020    norm_factor   
-00015440: 2020 2020 2020 2020 2020 2b3d 206e 702e            += np.
-00015450: 7375 6d28 7072 6f64 7563 745f 7769 6e64  sum(product_wind
-00015460: 6f77 735f 7765 6967 6874 7329 0a20 2020  ows_weights).   
-00015470: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00015480: 2020 2020 2020 2063 6869 5f61 7265 6120         chi_area 
-00015490: 2020 2020 202b 3d20 6e70 2e73 756d 2828       += np.sum((
-000154a0: 2828 506d 6f64 656c 5f32 642a 6172 6561  ((Pmodel_2d*area
-000154b0: 5f32 642a 2a32 292a 2a30 2e35 2d28 506f  _2d**2)**0.5-(Po
-000154c0: 6273 6572 7665 645f 3264 292a 2a30 2e35  bserved_2d)**0.5
-000154d0: 292f 2850 6f62 7365 7276 6564 5f32 6429  )/(Pobserved_2d)
-000154e0: 2a2a 302e 3529 2a2a 322c 6178 6973 3d31  **0.5)**2,axis=1
-000154f0: 290a 2020 2020 2020 2020 2020 2020 6e6f  ).            no
-00015500: 726d 5f66 6163 746f 7220 2020 2b3d 206c  rm_factor   += l
-00015510: 656e 2870 726f 6475 6374 5f77 696e 646f  en(product_windo
-00015520: 7773 290a 2020 2020 6966 206e 6f72 6d5f  ws).    if norm_
-00015530: 6661 6374 6f72 3e30 3a20 6368 695f 6172  factor>0: chi_ar
-00015540: 6561 2f3d 6e6f 726d 5f66 6163 746f 720a  ea/=norm_factor.
-00015550: 2020 2020 7265 7475 726e 2863 6869 5f61      return(chi_a
-00015560: 7265 6129 0a0a 0a64 6566 2072 6564 5f63  rea)...def red_c
-00015570: 6869 325f 736c 6162 2873 6c61 625f 6461  hi2_slab(slab_da
-00015580: 7461 2c20 7370 6563 7472 612c 206d 6173  ta, spectra, mas
-00015590: 6b2c 2052 6469 736b 3d6e 702e 6c6f 6773  k, Rdisk=np.logs
-000155a0: 7061 6365 282d 322c 322c 3130 292c 2064  pace(-2,2,10), d
-000155b0: 6973 7461 6e63 653d 3132 302c 204e 4c54  istance=120, NLT
-000155c0: 453d 4661 6c73 652c 2052 3d33 3030 302c  E=False, R=3000,
-000155d0: 2073 686f 7274 5f66 6f72 6d61 743d 4661   short_format=Fa
-000155e0: 6c73 652c 206f 7665 726c 6170 3d46 616c  lse, overlap=Fal
-000155f0: 7365 2c20 6e6f 6973 655f 6c65 7665 6c3d  se, noise_level=
-00015600: 3129 3a0a 2020 2020 2727 270a 2020 2020  1):.    '''.    
-00015610: 5265 7475 726e 7320 7265 6475 6365 6420  Returns reduced 
-00015620: 6368 6932 2062 6173 6564 206f 6e20 7365  chi2 based on se
-00015630: 6c65 6374 6564 2073 7065 6374 7261 6c20  lected spectral 
-00015640: 7769 6e64 6f77 7320 6163 726f 7373 2064  windows across d
-00015650: 6966 6665 7265 6e74 2065 6d69 7474 696e  ifferent emittin
-00015660: 6720 6469 736b 2072 6164 6975 730a 2020  g disk radius.  
-00015670: 2020 736c 6162 5f64 6174 613a 2070 6174    slab_data: pat
-00015680: 6820 636f 7272 6573 706f 6e64 696e 6720  h corresponding 
-00015690: 746f 2061 2073 696e 676c 6520 736c 6162  to a single slab
-000156a0: 206d 6f64 656c 206f 7220 6120 7369 6e67   model or a sing
-000156b0: 6c65 2073 6c61 625f 6d6f 6465 6c20 696e  le slab_model in
-000156c0: 7374 616e 6365 0a20 2020 2073 7065 6374  stance.    spect
-000156d0: 7261 3a20 6e75 6d70 7920 6172 7261 7920  ra: numpy array 
-000156e0: 7769 7468 2066 6972 7374 2063 6f6c 756d  with first colum
-000156f0: 6e20 7468 6520 7761 7665 6c65 6e67 7468  n the wavelength
-00015700: 2069 6e20 5b6d 6963 726f 6e73 5d20 616e   in [microns] an
-00015710: 6420 7365 636f 6e64 2063 6f6c 756d 6e20  d second column 
-00015720: 666c 7578 2069 6e20 5b4a 795d 0a20 2020  flux in [Jy].   
-00015730: 2052 6469 736b 3a20 5261 6469 7573 2063   Rdisk: Radius c
-00015740: 6f72 7265 7370 6f6e 6469 6e67 2074 6f20  orresponding to 
-00015750: 656d 6974 7469 6e67 2061 7265 6120 696e  emitting area in
-00015760: 2061 7374 726f 6e6f 6d69 6361 6c20 756e   astronomical un
-00015770: 6974 730a 2020 2020 6469 7374 616e 6365  its.    distance
-00015780: 3a20 6469 7374 616e 6365 206f 6620 6469  : distance of di
-00015790: 736b 2069 6e20 7061 7273 6563 0a20 2020  sk in parsec.   
-000157a0: 204e 4c54 453a 2069 6620 5472 7565 2c20   NLTE: if True, 
-000157b0: 4e4c 5445 2066 6c75 7820 6973 2074 616b  NLTE flux is tak
-000157c0: 656e 2066 726f 6d20 7468 6520 736c 6162  en from the slab
-000157d0: 206d 6f64 656c 2069 6e20 6361 7365 206f   model in case o
-000157e0: 6620 6f76 6572 6c61 703d 4661 6c73 652e  f overlap=False.
-000157f0: 0a20 2020 2027 2727 0a20 2020 2061 7265  .    '''.    are
-00015800: 6120 3d20 286e 702e 7069 2a28 5264 6973  a = (np.pi*(Rdis
-00015810: 6b2a 6175 2f64 6973 7461 6e63 652f 7063  k*au/distance/pc
-00015820: 292a 2a32 292e 7265 7368 6170 6528 5264  )**2).reshape(Rd
-00015830: 6973 6b2e 7368 6170 655b 305d 2c31 290a  isk.shape[0],1).
-00015840: 0a20 2020 2069 6620 6e6f 7420 6f76 6572  .    if not over
-00015850: 6c61 703a 0a20 2020 2020 2020 2069 6620  lap:.        if 
-00015860: 6973 696e 7374 616e 6365 2873 6c61 625f  isinstance(slab_
-00015870: 6461 7461 2c73 7472 293a 2073 6c61 625f  data,str): slab_
-00015880: 6461 7461 203d 2072 6561 645f 736c 6162  data = read_slab
-00015890: 2873 6c61 625f 6461 7461 2c76 6572 626f  (slab_data,verbo
-000158a0: 7365 3d46 616c 7365 2c73 686f 7274 5f66  se=False,short_f
-000158b0: 6f72 6d61 743d 7368 6f72 745f 666f 726d  ormat=short_form
-000158c0: 6174 290a 2020 2020 2020 2020 6c6d 696e  at).        lmin
-000158d0: 203d 206e 702e 616d 696e 2873 7065 6374   = np.amin(spect
-000158e0: 7261 5b3a 2c30 5d29 0a20 2020 2020 2020  ra[:,0]).       
-000158f0: 206c 6d61 7820 3d20 6e70 2e61 6d61 7828   lmax = np.amax(
-00015900: 7370 6563 7472 615b 3a2c 305d 290a 2020  spectra[:,0]).  
-00015910: 2020 2020 2020 736c 6162 5f64 6174 612e        slab_data.
-00015920: 636f 6e76 6f6c 7665 2852 3d52 2c6c 616d  convolve(R=R,lam
-00015930: 6264 615f 303d 6c6d 696e 2a30 2e39 2c6c  bda_0=lmin*0.9,l
-00015940: 616d 6264 615f 6e3d 6c6d 6178 2a31 2e31  ambda_n=lmax*1.1
-00015950: 2c4e 4c54 453d 4e4c 5445 2c76 6572 626f  ,NLTE=NLTE,verbo
-00015960: 7365 3d46 616c 7365 290a 2020 2020 2020  se=False).      
-00015970: 2020 6966 204e 4c54 453a 0a20 2020 2020    if NLTE:.     
-00015980: 2020 2020 2020 206d 6f64 656c 5370 6563         modelSpec
-00015990: 203d 2073 7065 6374 7265 732e 7370 6563   = spectres.spec
-000159a0: 7472 6573 2873 7065 6374 7261 5b3a 2c30  tres(spectra[:,0
-000159b0: 5d2c 2073 6c61 625f 6461 7461 2e63 6f6e  ], slab_data.con
-000159c0: 7657 6176 656c 656e 6774 682c 736c 6162  vWavelength,slab
-000159d0: 5f64 6174 612e 636f 6e76 4e4c 5445 666c  _data.convNLTEfl
-000159e0: 7578 2a31 6532 332c 2076 6572 626f 7365  ux*1e23, verbose
-000159f0: 3d46 616c 7365 2c66 696c 6c3d 302e 3029  =False,fill=0.0)
-00015a00: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00015a10: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00015a20: 5370 6563 203d 2073 7065 6374 7265 732e  Spec = spectres.
-00015a30: 7370 6563 7472 6573 2873 7065 6374 7261  spectres(spectra
-00015a40: 5b3a 2c30 5d2c 2073 6c61 625f 6461 7461  [:,0], slab_data
-00015a50: 2e63 6f6e 7657 6176 656c 656e 6774 682c  .convWavelength,
-00015a60: 736c 6162 5f64 6174 612e 636f 6e76 4c54  slab_data.convLT
-00015a70: 4566 6c75 782a 3165 3233 2c20 7665 7262  Eflux*1e23, verb
-00015a80: 6f73 653d 4661 6c73 652c 6669 6c6c 3d30  ose=False,fill=0
-00015a90: 2e30 2920 2020 0a20 2020 2065 6c73 653a  .0)   .    else:
-00015aa0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00015ab0: 7374 616e 6365 2873 6c61 625f 6461 7461  stance(slab_data
-00015ac0: 2c73 7472 293a 2073 6c61 625f 6461 7461  ,str): slab_data
-00015ad0: 203d 2072 6561 645f 6f76 6572 6c61 705f   = read_overlap_
-00015ae0: 7370 6563 7472 6128 736c 6162 5f64 6174  spectra(slab_dat
-00015af0: 612c 7665 7262 6f73 653d 4661 6c73 6529  a,verbose=False)
-00015b00: 0a20 2020 2020 2020 206c 6d69 6e20 3d20  .        lmin = 
-00015b10: 6e70 2e61 6d69 6e28 7370 6563 7472 615b  np.amin(spectra[
-00015b20: 3a2c 305d 290a 2020 2020 2020 2020 6c6d  :,0]).        lm
-00015b30: 6178 203d 206e 702e 616d 6178 2873 7065  ax = np.amax(spe
-00015b40: 6374 7261 5b3a 2c30 5d29 0a20 2020 2020  ctra[:,0]).     
-00015b50: 2020 2073 6c61 625f 6461 7461 2e63 6f6e     slab_data.con
-00015b60: 766f 6c76 655f 6f76 6572 6c61 7028 523d  volve_overlap(R=
-00015b70: 522c 6c61 6d62 6461 5f30 3d6c 6d69 6e2a  R,lambda_0=lmin*
-00015b80: 302e 392c 6c61 6d62 6461 5f6e 3d6c 6d61  0.9,lambda_n=lma
-00015b90: 782a 312e 312c 7665 7262 6f73 653d 4661  x*1.1,verbose=Fa
-00015ba0: 6c73 6529 0a20 2020 2020 2020 206d 6f64  lse).        mod
-00015bb0: 656c 5370 6563 203d 2073 7065 6374 7265  elSpec = spectre
-00015bc0: 732e 7370 6563 7472 6573 2873 7065 6374  s.spectres(spect
-00015bd0: 7261 5b3a 2c30 5d2c 2063 2f73 6c61 625f  ra[:,0], c/slab_
-00015be0: 6461 7461 2e63 6f6e 764f 7665 726c 6170  data.convOverlap
-00015bf0: 4672 6571 5b3a 3a2d 315d 2a31 652d 332c  Freq[::-1]*1e-3,
-00015c00: 2073 6c61 625f 6461 7461 2e63 6f6e 764f   slab_data.convO
-00015c10: 7665 726c 6170 4c54 455b 3a3a 2d31 5d2a  verlapLTE[::-1]*
-00015c20: 3165 3233 2c20 7665 7262 6f73 653d 4661  1e23, verbose=Fa
-00015c30: 6c73 652c 2066 696c 6c3d 302e 3029 0a20  lse, fill=0.0). 
-00015c40: 2020 2073 7065 6374 7261 5f32 6420 3d20     spectra_2d = 
-00015c50: 7370 6563 7472 615b 6d61 736b 2c31 5d2e  spectra[mask,1].
-00015c60: 7265 7368 6170 6528 312c 7370 6563 7472  reshape(1,spectr
-00015c70: 615b 6d61 736b 2c2d 315d 2e73 6861 7065  a[mask,-1].shape
-00015c80: 5b30 5d29 2a6e 702e 6f6e 6573 5f6c 696b  [0])*np.ones_lik
-00015c90: 6528 6172 6561 290a 2020 2020 6d6f 6465  e(area).    mode
-00015ca0: 6c53 7065 635f 3264 203d 206d 6f64 656c  lSpec_2d = model
-00015cb0: 5370 6563 5b6d 6173 6b5d 2e72 6573 6861  Spec[mask].resha
-00015cc0: 7065 2831 2c6d 6f64 656c 5370 6563 5b6d  pe(1,modelSpec[m
-00015cd0: 6173 6b5d 2e73 6861 7065 5b30 5d29 2a6e  ask].shape[0])*n
-00015ce0: 702e 6f6e 6573 5f6c 696b 6528 6172 6561  p.ones_like(area
-00015cf0: 290a 2020 2020 6172 6561 5f32 6420 3d20  ).    area_2d = 
-00015d00: 6172 6561 2e72 6573 6861 7065 2861 7265  area.reshape(are
-00015d10: 612e 7368 6170 655b 305d 2c31 290a 2020  a.shape[0],1).  
-00015d20: 2020 6368 695f 6172 6561 203d 206e 702e    chi_area = np.
-00015d30: 7375 6d28 2873 7065 6374 7261 5f32 642d  sum((spectra_2d-
-00015d40: 6d6f 6465 6c53 7065 635f 3264 2a61 7265  modelSpec_2d*are
-00015d50: 615f 3264 292a 2a32 2c61 7869 733d 3129  a_2d)**2,axis=1)
-00015d60: 2f6c 656e 2873 7065 6374 7261 5b6d 6173  /len(spectra[mas
-00015d70: 6b2c 305d 292f 6e6f 6973 655f 6c65 7665  k,0])/noise_leve
-00015d80: 6c0a 0a20 2020 2020 2020 2020 2020 0a20  l..           . 
-00015d90: 2020 2072 6574 7572 6e28 6368 695f 6172     return(chi_ar
-00015da0: 6561 29                                  ea)
+00010e60: 2a5c 6e22 290a 2020 2020 662e 7772 6974  *\n").    f.writ
+00010e70: 6528 222a 2a2a 206e 6d6f 6465 6c73 2073  e("*** nmodels s
+00010e80: 686f 756c 6420 666f 6c6c 6f77 206f 7574  hould follow out
+00010e90: 7075 745f 6669 6c65 6e61 6d65 202a 2a2a  put_filename ***
+00010ea0: 5c6e 2229 0a20 2020 2066 2e77 7269 7465  \n").    f.write
+00010eb0: 2866 277b 6f75 7470 7574 5f66 696c 656e  (f'{output_filen
+00010ec0: 616d 657d 2021 206f 7574 7075 745f 6669  ame} ! output_fi
+00010ed0: 6c65 6e61 6d65 5c6e 2729 0a20 2020 2066  lename\n').    f
+00010ee0: 2e77 7269 7465 2866 277b 6f76 6572 6c61  .write(f'{overla
+00010ef0: 705f 6669 6c65 6e61 6d65 7d20 2120 6f76  p_filename} ! ov
+00010f00: 6572 6c61 705f 6669 6c65 6e61 6d65 5c6e  erlap_filename\n
+00010f10: 2729 0a20 2020 2069 6620 7365 7061 7261  ').    if separa
+00010f20: 7465 5f6f 705f 6669 6c65 733a 0a20 2020  te_op_files:.   
+00010f30: 2020 2020 2066 2e77 7269 7465 2827 2e74       f.write('.t
+00010f40: 7275 652e 2020 2020 2120 7365 7061 7261  rue.    ! separa
+00010f50: 7465 5f6f 705f 6669 6c65 735c 6e27 290a  te_op_files\n').
+00010f60: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00010f70: 2020 662e 7772 6974 6528 272e 6661 6c73    f.write('.fals
+00010f80: 652e 2020 2021 2073 6570 6172 6174 655f  e.   ! separate_
+00010f90: 6f70 5f66 696c 6573 5c6e 2729 0a20 2020  op_files\n').   
+00010fa0: 2069 6620 6669 7473 5f6f 705f 6669 6c65   if fits_op_file
+00010fb0: 733a 0a20 2020 2020 2020 2066 2e77 7269  s:.        f.wri
+00010fc0: 7465 2827 2e74 7275 652e 2020 2020 2120  te('.true.    ! 
+00010fd0: 6669 7473 5f6f 705f 6669 6c65 735c 6e27  fits_op_files\n'
+00010fe0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00010ff0: 2020 2020 662e 7772 6974 6528 272e 6661      f.write('.fa
+00011000: 6c73 652e 2020 2021 2066 6974 735f 6f70  lse.   ! fits_op
+00011010: 5f66 696c 6573 5c6e 2729 0a20 2020 2069  _files\n').    i
+00011020: 6620 6e6f 5f69 6e64 6976 6964 7561 6c5f  f no_individual_
+00011030: 6c69 6e65 733a 0a20 2020 2020 2020 2066  lines:.        f
+00011040: 2e77 7269 7465 2827 2e74 7275 652e 2020  .write('.true.  
+00011050: 2020 2120 6e6f 5f69 6e64 6976 6964 7561    ! no_individua
+00011060: 6c5f 6c69 6e65 735c 6e27 290a 2020 2020  l_lines\n').    
+00011070: 656c 7365 3a0a 2020 2020 2020 2020 662e  else:.        f.
+00011080: 7772 6974 6528 272e 6661 6c73 652e 2020  write('.false.  
+00011090: 2021 206e 6f5f 696e 6469 7669 6475 616c   ! no_individual
+000110a0: 5f6c 696e 6573 5c6e 2729 0a20 2020 2069  _lines\n').    i
+000110b0: 6620 736c 6162 5f52 543a 0a20 2020 2020  f slab_RT:.     
+000110c0: 2020 2066 2e77 7269 7465 2827 2e74 7275     f.write('.tru
+000110d0: 652e 2020 2020 2120 736c 6162 5f52 5420  e.    ! slab_RT 
+000110e0: 5c6e 2729 0a20 2020 2065 6c73 653a 0a20  \n').    else:. 
+000110f0: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
+00011100: 2e66 616c 7365 2e20 2020 2120 736c 6162  .false.   ! slab
+00011110: 5f52 5420 5c6e 2729 0a20 2020 2069 6620  _RT \n').    if 
+00011120: 7368 6f72 745f 666f 726d 6174 3a0a 2020  short_format:.  
+00011130: 2020 2020 2020 662e 7772 6974 6528 272e        f.write('.
+00011140: 7472 7565 2e20 2020 2021 2073 686f 7274  true.    ! short
+00011150: 5f66 6f72 6d61 745c 6e27 290a 2020 2020  _format\n').    
+00011160: 656c 7365 3a0a 2020 2020 2020 2020 662e  else:.        f.
+00011170: 7772 6974 6528 272e 6661 6c73 652e 2020  write('.false.  
+00011180: 2021 2073 686f 7274 5f66 6f72 6d61 745c   ! short_format\
+00011190: 6e27 290a 2020 2020 662e 7772 6974 6528  n').    f.write(
+000111a0: 6627 7b6e 6d6f 6465 6c73 7d20 2020 2020  f'{nmodels}     
+000111b0: 2020 2020 2020 2020 2120 6e6d 6f64 656c          ! nmodel
+000111c0: 735c 6e27 290a 2020 2020 662e 7772 6974  s\n').    f.writ
+000111d0: 6528 272d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  e('-------------
+000111e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000111f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011200: 2d2d 2d2d 2d2d 2d2d 2d2d 2729 0a20 2020  ----------').   
+00011210: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00011220: 6e6d 6f64 656c 7329 3a0a 2020 2020 2020  nmodels):.      
+00011230: 2020 662e 7772 6974 6528 6627 5c6e 2a2a    f.write(f'\n**
+00011240: 2a20 6d6f 6465 6c20 7b69 2b31 7d20 2a2a  * model {i+1} **
+00011250: 2a5c 6e27 290a 2020 2020 2020 2020 6966  *\n').        if
+00011260: 206e 702e 7375 6d28 4e74 6f74 5f6c 6973   np.sum(Ntot_lis
+00011270: 7429 213d 6e6d 6f64 656c 733a 0a20 2020  t)!=nmodels:.   
+00011280: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
+00011290: 2866 6d74 2e66 6f72 6d61 7428 277b 3a2e  (fmt.format('{:.
+000112a0: 336d 7d27 2c4e 746f 745f 6c69 7374 5b69  3m}',Ntot_list[i
+000112b0: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
+000112c0: 662e 7772 6974 6528 2709 2020 2021 204e  f.write('.   ! N
+000112d0: 4874 6f74 2020 5b63 6d5e 2d32 5d20 746f  Htot  [cm^-2] to
+000112e0: 7461 6c20 6761 7320 636f 6c75 6d6e 2064  tal gas column d
+000112f0: 656e 7369 7479 5c6e 2729 0a20 2020 2020  ensity\n').     
+00011300: 2020 2069 6620 6e70 2e73 756d 286e 4870     if np.sum(nHp
+00011310: 6c75 735f 6c69 7374 2921 3d6e 6d6f 6465  lus_list)!=nmode
+00011320: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
+00011330: 662e 7772 6974 6528 666d 742e 666f 726d  f.write(fmt.form
+00011340: 6174 2827 7b3a 2e33 6d7d 272c 6e48 706c  at('{:.3m}',nHpl
+00011350: 7573 5f6c 6973 745b 695d 2929 0a20 2020  us_list[i])).   
+00011360: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
+00011370: 2827 0920 2020 2120 6e48 2b20 2020 205b  ('.   ! nH+    [
+00011380: 636d 5e2d 335d 2020 7072 6f74 6f6e 206e  cm^-3]  proton n
+00011390: 756d 6265 7220 6465 6e73 6974 795c 6e27  umber density\n'
+000113a0: 290a 2020 2020 2020 2020 6966 206e 702e  ).        if np.
+000113b0: 7375 6d28 6e48 315f 6c69 7374 2921 3d6e  sum(nH1_list)!=n
+000113c0: 6d6f 6465 6c73 3a0a 2020 2020 2020 2020  models:.        
+000113d0: 2020 2020 662e 7772 6974 6528 666d 742e      f.write(fmt.
+000113e0: 666f 726d 6174 2827 7b3a 2e33 6d7d 272c  format('{:.3m}',
+000113f0: 6e48 315f 6c69 7374 5b69 5d29 290a 2020  nH1_list[i])).  
+00011400: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00011410: 6528 2709 2020 2021 206e 4849 0920 5b63  e('.   ! nHI. [c
+00011420: 6d5e 2d33 5d20 6174 6f6d 6963 2068 7964  m^-3] atomic hyd
+00011430: 726f 6765 6e5c 6e27 290a 2020 2020 2020  rogen\n').      
+00011440: 2020 6966 206e 702e 7375 6d28 6e48 325f    if np.sum(nH2_
+00011450: 6c69 7374 2921 3d6e 6d6f 6465 6c73 3a0a  list)!=nmodels:.
+00011460: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+00011470: 6974 6528 666d 742e 666f 726d 6174 2827  ite(fmt.format('
+00011480: 7b3a 2e33 6d7d 272c 6e48 325f 6c69 7374  {:.3m}',nH2_list
+00011490: 5b69 5d29 290a 2020 2020 2020 2020 2020  [i])).          
+000114a0: 2020 662e 7772 6974 6528 2709 2020 2021    f.write('.   !
+000114b0: 206e 4832 2020 2020 5b63 6d5e 2d33 5d20   nH2    [cm^-3] 
+000114c0: 2020 6d6f 6c65 6375 6c61 7220 6879 6472    molecular hydr
+000114d0: 6f67 656e 5c6e 2729 0a20 2020 2020 2020  ogen\n').       
+000114e0: 2069 6620 6e70 2e73 756d 286e 4865 5f6c   if np.sum(nHe_l
+000114f0: 6973 7429 213d 6e6d 6f64 656c 733a 0a20  ist)!=nmodels:. 
+00011500: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+00011510: 7465 2866 6d74 2e66 6f72 6d61 7428 277b  te(fmt.format('{
+00011520: 3a2e 336d 7d27 2c6e 4865 5f6c 6973 745b  :.3m}',nHe_list[
+00011530: 695d 2929 0a20 2020 2020 2020 2020 2020  i])).           
+00011540: 2066 2e77 7269 7465 2827 0920 2020 2120   f.write('.   ! 
+00011550: 6e48 6520 2020 205b 636d 5e2d 335d 2020  nHe    [cm^-3]  
+00011560: 2048 656c 6975 6d5c 6e27 290a 2020 2020   Helium\n').    
+00011570: 2020 2020 6966 206e 702e 7375 6d28 6e65      if np.sum(ne
+00011580: 6c65 635f 6c69 7374 2921 3d6e 6d6f 6465  lec_list)!=nmode
+00011590: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
+000115a0: 662e 7772 6974 6528 666d 742e 666f 726d  f.write(fmt.form
+000115b0: 6174 2827 7b3a 2e33 6d7d 272c 6e65 6c65  at('{:.3m}',nele
+000115c0: 635f 6c69 7374 5b69 5d29 290a 2020 2020  c_list[i])).    
+000115d0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+000115e0: 2709 2020 2021 206e 656c 6563 2020 5b63  '.   ! nelec  [c
+000115f0: 6d5e 2d33 5d20 2020 656c 6563 7472 6f6e  m^-3]   electron
+00011600: 206e 756d 6265 7220 6465 6e73 6974 795c   number density\
+00011610: 6e27 290a 2020 2020 2020 2020 6966 206e  n').        if n
+00011620: 702e 7375 6d28 5467 5f6c 6973 7429 213d  p.sum(Tg_list)!=
+00011630: 6e6d 6f64 656c 733a 0a20 2020 2020 2020  nmodels:.       
+00011640: 2020 2020 2066 2e77 7269 7465 2866 6d74       f.write(fmt
+00011650: 2e66 6f72 6d61 7428 277b 3a2e 336d 7d27  .format('{:.3m}'
+00011660: 2c54 675f 6c69 7374 5b69 5d29 290a 2020  ,Tg_list[i])).  
+00011670: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00011680: 6528 2709 2020 2021 2054 6761 7320 5b4b  e('.   ! Tgas [K
+00011690: 5d20 2020 2020 2020 2020 2020 6761 7320  ]           gas 
+000116a0: 7465 6d70 6572 6174 7572 655c 6e27 290a  temperature\n').
+000116b0: 2020 2020 2020 2020 6966 206e 702e 7375          if np.su
+000116c0: 6d28 5464 5f6c 6973 7429 213d 6e6d 6f64  m(Td_list)!=nmod
+000116d0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+000116e0: 2066 2e77 7269 7465 2866 6d74 2e66 6f72   f.write(fmt.for
+000116f0: 6d61 7428 277b 3a2e 336d 7d27 2c54 645f  mat('{:.3m}',Td_
+00011700: 6c69 7374 5b69 5d29 290a 2020 2020 2020  list[i])).      
+00011710: 2020 2020 2020 662e 7772 6974 6528 2709        f.write('.
+00011720: 2020 2021 2054 6475 7374 205b 4b5d 2020     ! Tdust [K]  
+00011730: 2020 2020 2020 2020 2064 7573 7420 7465           dust te
+00011740: 6d70 6572 6174 7572 655c 6e27 290a 2020  mperature\n').  
+00011750: 2020 2020 2020 6966 206e 702e 7375 6d28        if np.sum(
+00011760: 7674 7572 625f 6c69 7374 2921 3d6e 6d6f  vturb_list)!=nmo
+00011770: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
+00011780: 2020 662e 7772 6974 6528 666d 742e 666f    f.write(fmt.fo
+00011790: 726d 6174 2827 7b3a 2e33 6d7d 272c 7674  rmat('{:.3m}',vt
+000117a0: 7572 625f 6c69 7374 5b69 5d29 290a 2020  urb_list[i])).  
+000117b0: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+000117c0: 6528 2709 2020 2021 2076 7475 7262 2020  e('.   ! vturb  
+000117d0: 5b6b 6d73 2f73 5d20 2020 2074 7572 6275  [kms/s]    turbu
+000117e0: 6c65 6e74 2076 656c 6f63 6974 795c 6e27  lent velocity\n'
+000117f0: 290a 2020 2020 2020 2020 6966 206e 702e  ).        if np.
+00011800: 7375 6d28 6475 7374 5f74 6f5f 6761 735f  sum(dust_to_gas_
+00011810: 6c69 7374 2921 3d6e 6d6f 6465 6c73 3a0a  list)!=nmodels:.
+00011820: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+00011830: 6974 6528 666d 742e 666f 726d 6174 2827  ite(fmt.format('
+00011840: 7b3a 2e33 6d7d 272c 6475 7374 5f74 6f5f  {:.3m}',dust_to_
+00011850: 6761 735f 6c69 7374 5b69 5d29 290a 2020  gas_list[i])).  
+00011860: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00011870: 6528 2709 2020 2021 2064 7573 745f 746f  e('.   ! dust_to
+00011880: 5f67 6173 5c6e 2729 0a20 2020 2020 2020  _gas\n').       
+00011890: 2069 6620 6e70 2e73 756d 286c 696e 655f   if np.sum(line_
+000118a0: 6f76 6572 6c61 705f 6c69 7374 2921 3d32  overlap_list)!=2
+000118b0: 2a6e 6d6f 6465 6c73 3a0a 2020 2020 2020  *nmodels:.      
+000118c0: 2020 2020 2020 662e 7772 6974 6528 666d        f.write(fm
+000118d0: 742e 666f 726d 6174 2827 7b3a 2e33 667d  t.format('{:.3f}
+000118e0: 272c 6c69 6e65 5f6f 7665 726c 6170 5f6c  ',line_overlap_l
+000118f0: 6973 745b 692c 305d 292b 2720 272b 666d  ist[i,0])+' '+fm
+00011900: 742e 666f 726d 6174 2827 7b3a 2e33 667d  t.format('{:.3f}
+00011910: 272c 6c69 6e65 5f6f 7665 726c 6170 5f6c  ',line_overlap_l
+00011920: 6973 745b 692c 315d 2929 0a20 2020 2020  ist[i,1])).     
+00011930: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
+00011940: 0920 2020 2120 6c69 6e65 5f6f 7665 726c  .   ! line_overl
+00011950: 6170 2020 5b6d 6963 726f 6e73 5d20 206d  ap  [microns]  m
+00011960: 696e 696d 756d 2061 6e64 206d 6178 696d  inimum and maxim
+00011970: 756d 2077 6176 656c 656e 6774 6873 2066  um wavelengths f
+00011980: 6f72 206c 696e 6520 6f76 6572 6c61 705c  or line overlap\
+00011990: 6e27 290a 2020 2020 2020 2020 6966 206e  n').        if n
+000119a0: 702e 7375 6d28 525f 6f76 6572 6c61 705f  p.sum(R_overlap_
+000119b0: 6c69 7374 2921 3d6e 6d6f 6465 6c73 3a0a  list)!=nmodels:.
+000119c0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+000119d0: 6974 6528 666d 742e 666f 726d 6174 2827  ite(fmt.format('
+000119e0: 7b3a 2e33 6d7d 272c 525f 6f76 6572 6c61  {:.3m}',R_overla
+000119f0: 705f 6c69 7374 5b69 5d29 290a 2020 2020  p_list[i])).    
+00011a00: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00011a10: 2709 2020 2021 2052 5f6f 7665 726c 6170  '.   ! R_overlap
+00011a20: 2020 7361 6d70 6c69 6e67 2067 7269 6420    sampling grid 
+00011a30: 7265 736f 6c75 7469 6f6e 2066 6f72 206c  resolution for l
+00011a40: 696e 6520 6f76 6572 6c61 705c 6e27 290a  ine overlap\n').
+00011a50: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00011a60: 6627 7b6c 656e 2873 7065 6369 6573 5f6c  f'{len(species_l
+00011a70: 6973 7429 7d09 2020 2021 204e 7370 6563  ist)}.   ! Nspec
+00011a80: 6965 7320 2020 2020 2020 2020 2020 206e  ies            n
+00011a90: 756d 6265 7220 6f66 2073 7065 6369 6573  umber of species
+00011aa0: 2066 6f72 2074 6861 7420 6d6f 6465 6c5c   for that model\
+00011ab0: 6e27 290a 2020 2020 2020 2020 666f 7220  n').        for 
+00011ac0: 6a20 696e 2072 616e 6765 286c 656e 2873  j in range(len(s
+00011ad0: 7065 6369 6573 5f6c 6973 7429 293a 0a20  pecies_list)):. 
+00011ae0: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+00011af0: 7465 2866 277b 6c69 7374 2873 7065 6369  te(f'{list(speci
+00011b00: 6573 5f6c 6973 742e 6b65 7973 2829 295b  es_list.keys())[
+00011b10: 6a5d 7d20 2020 2020 207b 7370 6563 6965  j]}      {specie
+00011b20: 735f 6c69 7374 5b6c 6973 7428 7370 6563  s_list[list(spec
+00011b30: 6965 735f 6c69 7374 2e6b 6579 7328 2929  ies_list.keys())
+00011b40: 5b6a 5d5d 7d5c 6e27 290a 2020 2020 2020  [j]]}\n').      
+00011b50: 2020 662e 7772 6974 6528 2720 2020 2020    f.write('     
+00011b60: 2020 2020 2020 2120 656e 645c 6e27 290a        ! end\n').
+00011b70: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00011b80: 272d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  '---------------
+00011b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011bb0: 2d2d 2d2d 2d2d 2d2d 2729 0a20 2020 2066  --------').    f
+00011bc0: 2e63 6c6f 7365 2829 0a20 2020 2072 6574  .close().    ret
+00011bd0: 7572 6e0a 0a0a 6465 6620 6765 6e65 7261  urn...def genera
+00011be0: 7465 5f31 445f 7374 7275 6374 7572 6528  te_1D_structure(
+00011bf0: 647a 2c73 7065 6369 6573 5f6c 6973 742c  dz,species_list,
+00011c00: 7674 7572 622c 6e64 2c54 642c 6e5f 7370  vturb,nd,Td,n_sp
+00011c10: 6563 6965 732c 545f 7370 6563 6965 732c  ecies,T_species,
+00011c20: 6e48 323d 302c 6e48 493d 302c 6e48 4949  nH2=0,nHI=0,nHII
+00011c30: 3d30 2c6e 4865 3d30 2c6e 656c 6563 3d30  =0,nHe=0,nelec=0
+00011c40: 2c66 696c 656e 616d 653d 2731 445f 7374  ,filename='1D_st
+00011c50: 7275 6374 7572 6527 293a 0a20 2020 2022  ructure'):.    "
+00011c60: 2222 0a20 2020 2047 656e 6572 6174 6573  "".    Generates
+00011c70: 2031 4420 7374 7275 6374 7572 6520 6669   1D structure fi
+00011c80: 6c65 2072 6571 7569 7265 6420 666f 7220  le required for 
+00011c90: 3144 2073 6c61 6220 6d6f 6465 6c73 0a20  1D slab models. 
+00011ca0: 2020 2022 2222 0a20 2020 2069 6620 6973     """.    if is
+00011cb0: 696e 7374 616e 6365 2864 7a2c 666c 6f61  instance(dz,floa
+00011cc0: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
+00011cd0: 2864 7a2c 696e 7429 3a20 647a 3d6e 702e  (dz,int): dz=np.
+00011ce0: 6172 7261 7928 5b64 7a5d 290a 2020 2020  array([dz]).    
+00011cf0: 6966 2069 7369 6e73 7461 6e63 6528 647a  if isinstance(dz
+00011d00: 2c6c 6973 7429 3a20 647a 3d6e 702e 6172  ,list): dz=np.ar
+00011d10: 7261 7928 647a 290a 2020 2020 6966 2069  ray(dz).    if i
+00011d20: 7369 6e73 7461 6e63 6528 7370 6563 6965  sinstance(specie
+00011d30: 735f 6c69 7374 2c73 7472 293a 2073 7065  s_list,str): spe
+00011d40: 6369 6573 5f6c 6973 743d 5b73 7065 6369  cies_list=[speci
+00011d50: 6573 5f6c 6973 745d 0a20 2020 2069 6620  es_list].    if 
+00011d60: 6973 696e 7374 616e 6365 2876 7475 7262  isinstance(vturb
+00011d70: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
+00011d80: 7461 6e63 6528 7674 7572 622c 696e 7429  tance(vturb,int)
+00011d90: 3a20 7674 7572 623d 6e70 2e6f 6e65 735f  : vturb=np.ones_
+00011da0: 6c69 6b65 2864 7a29 2a76 7475 7262 0a20  like(dz)*vturb. 
+00011db0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00011dc0: 286e 642c 666c 6f61 7429 206f 7220 6973  (nd,float) or is
+00011dd0: 696e 7374 616e 6365 286e 642c 696e 7429  instance(nd,int)
+00011de0: 3a20 6e64 3d6e 702e 6f6e 6573 5f6c 696b  : nd=np.ones_lik
+00011df0: 6528 647a 292a 6e64 0a20 2020 2069 6620  e(dz)*nd.    if 
+00011e00: 6973 696e 7374 616e 6365 2854 642c 666c  isinstance(Td,fl
+00011e10: 6f61 7429 206f 7220 6973 696e 7374 616e  oat) or isinstan
+00011e20: 6365 2854 642c 696e 7429 3a20 5464 3d6e  ce(Td,int): Td=n
+00011e30: 702e 6f6e 6573 5f6c 696b 6528 647a 292a  p.ones_like(dz)*
+00011e40: 5464 0a20 2020 2069 6620 6973 696e 7374  Td.    if isinst
+00011e50: 616e 6365 286e 4832 2c66 6c6f 6174 2920  ance(nH2,float) 
+00011e60: 6f72 2069 7369 6e73 7461 6e63 6528 6e48  or isinstance(nH
+00011e70: 322c 696e 7429 3a20 6e48 323d 6e70 2e6f  2,int): nH2=np.o
+00011e80: 6e65 735f 6c69 6b65 2864 7a29 2a6e 4832  nes_like(dz)*nH2
+00011e90: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+00011ea0: 6365 286e 4849 2c66 6c6f 6174 2920 6f72  ce(nHI,float) or
+00011eb0: 2069 7369 6e73 7461 6e63 6528 6e48 492c   isinstance(nHI,
+00011ec0: 696e 7429 3a20 6e48 493d 6e70 2e6f 6e65  int): nHI=np.one
+00011ed0: 735f 6c69 6b65 2864 7a29 2a6e 4849 0a20  s_like(dz)*nHI. 
+00011ee0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00011ef0: 286e 4849 492c 666c 6f61 7429 206f 7220  (nHII,float) or 
+00011f00: 6973 696e 7374 616e 6365 286e 4849 492c  isinstance(nHII,
+00011f10: 696e 7429 3a20 6e48 4949 3d6e 702e 6f6e  int): nHII=np.on
+00011f20: 6573 5f6c 696b 6528 647a 292a 6e48 4949  es_like(dz)*nHII
+00011f30: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+00011f40: 6365 286e 4865 2c66 6c6f 6174 2920 6f72  ce(nHe,float) or
+00011f50: 2069 7369 6e73 7461 6e63 6528 6e48 652c   isinstance(nHe,
+00011f60: 696e 7429 3a20 6e48 653d 6e70 2e6f 6e65  int): nHe=np.one
+00011f70: 735f 6c69 6b65 2864 7a29 2a6e 4865 0a20  s_like(dz)*nHe. 
+00011f80: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00011f90: 286e 656c 6563 2c66 6c6f 6174 2920 6f72  (nelec,float) or
+00011fa0: 2069 7369 6e73 7461 6e63 6528 6e65 6c65   isinstance(nele
+00011fb0: 632c 696e 7429 3a20 6e65 6c65 633d 6e70  c,int): nelec=np
+00011fc0: 2e6f 6e65 735f 6c69 6b65 2864 7a29 2a6e  .ones_like(dz)*n
+00011fd0: 656c 6563 0a20 2020 2069 6620 6973 696e  elec.    if isin
+00011fe0: 7374 616e 6365 286e 5f73 7065 6369 6573  stance(n_species
+00011ff0: 2c66 6c6f 6174 2920 6f72 2069 7369 6e73  ,float) or isins
+00012000: 7461 6e63 6528 6e5f 7370 6563 6965 732c  tance(n_species,
+00012010: 696e 7429 3a20 6e5f 7370 6563 6965 733d  int): n_species=
+00012020: 6e70 2e6f 6e65 7328 2864 7a2e 7368 6170  np.ones((dz.shap
+00012030: 655b 305d 2c6c 656e 2873 7065 6369 6573  e[0],len(species
+00012040: 5f6c 6973 7429 2929 2a6e 5f73 7065 6369  _list)))*n_speci
+00012050: 6573 0a20 2020 2069 6620 6973 696e 7374  es.    if isinst
+00012060: 616e 6365 2854 5f73 7065 6369 6573 2c66  ance(T_species,f
+00012070: 6c6f 6174 2920 6f72 2069 7369 6e73 7461  loat) or isinsta
+00012080: 6e63 6528 545f 7370 6563 6965 732c 696e  nce(T_species,in
+00012090: 7429 3a20 545f 7370 6563 6965 733d 6e70  t): T_species=np
+000120a0: 2e6f 6e65 7328 2864 7a2e 7368 6170 655b  .ones((dz.shape[
+000120b0: 305d 2c6c 656e 2873 7065 6369 6573 5f6c  0],len(species_l
+000120c0: 6973 7429 2929 2a54 5f73 7065 6369 6573  ist)))*T_species
+000120d0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+000120e0: 6365 2854 5f73 7065 6369 6573 2c6c 6973  ce(T_species,lis
+000120f0: 7429 3a20 545f 7370 6563 6965 733d 6e70  t): T_species=np
+00012100: 2e61 7272 6179 2854 5f73 7065 6369 6573  .array(T_species
+00012110: 290a 2020 2020 6966 2069 7369 6e73 7461  ).    if isinsta
+00012120: 6e63 6528 6e5f 7370 6563 6965 732c 6c69  nce(n_species,li
+00012130: 7374 293a 206e 5f73 7065 6369 6573 3d6e  st): n_species=n
+00012140: 702e 6172 7261 7928 6e5f 7370 6563 6965  p.array(n_specie
+00012150: 7329 0a20 2020 2069 6620 6e70 2e61 7272  s).    if np.arr
+00012160: 6179 2854 5f73 7065 6369 6573 292e 7369  ay(T_species).si
+00012170: 7a65 3d3d 6c65 6e28 7370 6563 6965 735f  ze==len(species_
+00012180: 6c69 7374 293a 0a20 2020 2020 2020 2054  list):.        T
+00012190: 5f73 7065 6369 6573 5f74 656d 703d 6e70  _species_temp=np
+000121a0: 2e6f 6e65 7328 2864 7a2e 7368 6170 655b  .ones((dz.shape[
+000121b0: 305d 2c6c 656e 2873 7065 6369 6573 5f6c  0],len(species_l
+000121c0: 6973 7429 2929 0a20 2020 2020 2020 2066  ist))).        f
+000121d0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+000121e0: 6e28 7370 6563 6965 735f 6c69 7374 2929  n(species_list))
+000121f0: 3a0a 2020 2020 2020 2020 2020 2020 545f  :.            T_
+00012200: 7370 6563 6965 735f 7465 6d70 5b3a 2c69  species_temp[:,i
+00012210: 5d3d 545f 7370 6563 6965 735b 695d 0a20  ]=T_species[i]. 
+00012220: 2020 2020 2020 2054 5f73 7065 6369 6573         T_species
+00012230: 3d54 5f73 7065 6369 6573 5f74 656d 702a  =T_species_temp*
+00012240: 312e 3030 0a20 2020 2069 6620 6e70 2e61  1.00.    if np.a
+00012250: 7272 6179 286e 5f73 7065 6369 6573 292e  rray(n_species).
+00012260: 7369 7a65 3d3d 6c65 6e28 7370 6563 6965  size==len(specie
+00012270: 735f 6c69 7374 293a 0a20 2020 2020 2020  s_list):.       
+00012280: 206e 5f73 7065 6369 6573 5f74 656d 703d   n_species_temp=
+00012290: 6e70 2e6f 6e65 7328 2864 7a2e 7368 6170  np.ones((dz.shap
+000122a0: 655b 305d 2c6c 656e 2873 7065 6369 6573  e[0],len(species
+000122b0: 5f6c 6973 7429 2929 0a20 2020 2020 2020  _list))).       
+000122c0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+000122d0: 6c65 6e28 7370 6563 6965 735f 6c69 7374  len(species_list
+000122e0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+000122f0: 6e5f 7370 6563 6965 735f 7465 6d70 5b3a  n_species_temp[:
+00012300: 2c69 5d3d 6e5f 7370 6563 6965 735b 695d  ,i]=n_species[i]
+00012310: 0a20 2020 2020 2020 206e 5f73 7065 6369  .        n_speci
+00012320: 6573 3d6e 5f73 7065 6369 6573 5f74 656d  es=n_species_tem
+00012330: 702a 312e 3030 0a0a 2020 2020 7769 7468  p*1.00..    with
+00012340: 206f 7065 6e28 6669 6c65 6e61 6d65 2c27   open(filename,'
+00012350: 7727 2920 6173 2066 3a0a 2020 2020 2020  w') as f:.      
+00012360: 2020 662e 7772 6974 6528 6627 7b6c 656e    f.write(f'{len
+00012370: 2864 7a29 3a64 7d5c 6e27 290a 2020 2020  (dz):d}\n').    
+00012380: 2020 2020 662e 7772 6974 6528 6627 7b6c      f.write(f'{l
+00012390: 656e 2873 7065 6369 6573 5f6c 6973 7429  en(species_list)
+000123a0: 3a64 7d5c 6e27 290a 2020 2020 2020 2020  :d}\n').        
+000123b0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+000123c0: 656e 2873 7065 6369 6573 5f6c 6973 7429  en(species_list)
+000123d0: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+000123e0: 2e77 7269 7465 2873 7065 6369 6573 5f6c  .write(species_l
+000123f0: 6973 745b 695d 2b27 5c6e 2729 0a20 2020  ist[i]+'\n').   
+00012400: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00012410: 6e67 6528 6c65 6e28 647a 2929 3a0a 2020  nge(len(dz)):.  
+00012420: 2020 2020 2020 2020 2020 7374 7269 6e67            string
+00012430: 3d27 270a 2020 2020 2020 2020 2020 2020  =''.            
+00012440: 7374 7269 6e67 2b3d 6627 7b69 2b31 3a64  string+=f'{i+1:d
+00012450: 7d20 2027 0a20 2020 2020 2020 2020 2020  }  '.           
+00012460: 2073 7472 696e 672b 3d66 277b 647a 5b69   string+=f'{dz[i
+00012470: 5d3a 2e33 657d 2020 270a 2020 2020 2020  ]:.3e}  '.      
+00012480: 2020 2020 2020 7374 7269 6e67 2b3d 6627        string+=f'
+00012490: 7b76 7475 7262 5b69 5d3a 2e33 667d 2020  {vturb[i]:.3f}  
+000124a0: 270a 2020 2020 2020 2020 2020 2020 7374  '.            st
+000124b0: 7269 6e67 2b3d 6627 7b6e 645b 695d 3a2e  ring+=f'{nd[i]:.
+000124c0: 3365 7d20 2027 0a20 2020 2020 2020 2020  3e}  '.         
+000124d0: 2020 2073 7472 696e 672b 3d66 277b 5464     string+=f'{Td
+000124e0: 5b69 5d3a 2e33 667d 2020 270a 2020 2020  [i]:.3f}  '.    
+000124f0: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
+00012500: 2072 616e 6765 286c 656e 2873 7065 6369   range(len(speci
+00012510: 6573 5f6c 6973 7429 293a 0a20 2020 2020  es_list)):.     
+00012520: 2020 2020 2020 2020 2020 2073 7472 696e             strin
+00012530: 672b 3d66 277b 6e5f 7370 6563 6965 735b  g+=f'{n_species[
+00012540: 692c 6a5d 3a2e 3365 7d20 2027 0a20 2020  i,j]:.3e}  '.   
+00012550: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+00012560: 6e20 7261 6e67 6528 6c65 6e28 7370 6563  n range(len(spec
+00012570: 6965 735f 6c69 7374 2929 3a0a 2020 2020  ies_list)):.    
+00012580: 2020 2020 2020 2020 2020 2020 7374 7269              stri
+00012590: 6e67 2b3d 6627 7b54 5f73 7065 6369 6573  ng+=f'{T_species
+000125a0: 5b69 2c6a 5d3a 2e33 667d 2020 270a 2020  [i,j]:.3f}  '.  
+000125b0: 2020 2020 2020 2020 2020 7374 7269 6e67            string
+000125c0: 2b3d 6627 7b6e 4832 5b69 5d3a 2e33 657d  +=f'{nH2[i]:.3e}
+000125d0: 2020 270a 2020 2020 2020 2020 2020 2020    '.            
+000125e0: 7374 7269 6e67 2b3d 6627 7b6e 4849 5b69  string+=f'{nHI[i
+000125f0: 5d3a 2e33 657d 2020 270a 2020 2020 2020  ]:.3e}  '.      
+00012600: 2020 2020 2020 7374 7269 6e67 2b3d 6627        string+=f'
+00012610: 7b6e 4849 495b 695d 3a2e 3365 7d20 2027  {nHII[i]:.3e}  '
+00012620: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00012630: 696e 672b 3d66 277b 6e48 655b 695d 3a2e  ing+=f'{nHe[i]:.
+00012640: 3365 7d20 2027 0a20 2020 2020 2020 2020  3e}  '.         
+00012650: 2020 2073 7472 696e 672b 3d66 277b 6e65     string+=f'{ne
+00012660: 6c65 635b 695d 3a2e 3365 7d20 2027 0a20  lec[i]:.3e}  '. 
+00012670: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+00012680: 7465 2873 7472 696e 672b 275c 6e27 290a  te(string+'\n').
+00012690: 2020 2020 2020 2020 662e 636c 6f73 6528          f.close(
+000126a0: 290a 0a0a 636c 6173 7320 4d79 466f 726d  )...class MyForm
+000126b0: 6174 7465 7228 7374 7269 6e67 2e46 6f72  atter(string.For
+000126c0: 6d61 7474 6572 293a 0a20 2020 2022 2222  matter):.    """
+000126d0: 0a20 2020 2053 7472 696e 6720 666f 726d  .    String form
+000126e0: 6174 7465 7220 666f 7220 7072 6f64 7563  atter for produc
+000126f0: 696e 6720 696e 7075 7420 6669 6c65 730a  ing input files.
+00012700: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
+00012710: 2066 6f72 6d61 745f 6669 656c 6428 7365   format_field(se
+00012720: 6c66 2c76 616c 7565 2c66 6f72 6d61 745f  lf,value,format_
+00012730: 7370 6563 293a 0a20 2020 2020 2020 2069  spec):.        i
+00012740: 6620 666f 726d 6174 5f73 7065 635b 2d31  f format_spec[-1
+00012750: 5d3d 3d27 6d27 3a0a 2020 2020 2020 2020  ]=='m':.        
+00012760: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+00012770: 2829 2e66 6f72 6d61 745f 6669 656c 6428  ().format_field(
+00012780: 7661 6c75 652c 666f 726d 6174 5f73 7065  value,format_spe
+00012790: 635b 3a2d 315d 2b27 6527 292e 7265 706c  c[:-1]+'e').repl
+000127a0: 6163 6528 2765 2b27 2c27 6527 290a 2020  ace('e+','e').  
+000127b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000127c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000127d0: 7570 6572 2829 2e66 6f72 6d61 745f 6669  uper().format_fi
+000127e0: 656c 6428 7661 6c75 652c 666f 726d 6174  eld(value,format
+000127f0: 5f73 7065 6329 0a0a 0a66 6d74 3d4d 7946  _spec)...fmt=MyF
+00012800: 6f72 6d61 7474 6572 2829 0a0a 0a64 6566  ormatter()...def
+00012810: 206c 696e 655f 666c 7578 286c 312c 6c32   line_flux(l1,l2
+00012820: 2c77 6176 656c 656e 6774 682c 666c 7578  ,wavelength,flux
+00012830: 293a 0a20 2020 2027 2727 0a20 2020 2055  ):.    '''.    U
+00012840: 6e69 7473 3a20 5265 7475 726e 2069 7320  nits: Return is 
+00012850: 696e 2074 6865 2073 616d 6520 756e 6974  in the same unit
+00012860: 2061 7320 696e 7075 742e 205b 4173 7375   as input. [Assu
+00012870: 6d65 6420 746f 2062 6520 696e 2065 7267  med to be in erg
+00012880: 2f73 2f63 6d32 2f73 725d 206c 3120 616e  /s/cm2/sr] l1 an
+00012890: 6420 6c32 2073 616d 6520 756e 6974 2061  d l2 same unit a
+000128a0: 7320 7761 7665 6c65 6e67 7468 0a0a 2020  s wavelength..  
+000128b0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+000128c0: 2d2d 2d2d 2d0a 2020 2020 666c 6f61 743a  -----.    float:
+000128d0: 0a20 2020 2020 2053 756d 206f 6620 696e  .      Sum of in
+000128e0: 7465 6772 6174 6564 206c 696e 6520 666c  tegrated line fl
+000128f0: 7578 2062 6574 7765 656e 2077 6176 656c  ux between wavel
+00012900: 656e 6774 6873 206c 3120 616e 6420 6c32  engths l1 and l2
+00012910: 2e0a 0a20 2020 2027 2727 0a20 2020 206d  ...    '''.    m
+00012920: 6173 6b3d 2877 6176 656c 656e 6774 683e  ask=(wavelength>
+00012930: 6c31 2926 2877 6176 656c 656e 6774 683c  l1)&(wavelength<
+00012940: 3d6c 3229 0a20 2020 2072 6574 7572 6e20  =l2).    return 
+00012950: 6e70 2e73 756d 2866 6c75 785b 6d61 736b  np.sum(flux[mask
+00012960: 5d29 0a0a 0a64 6566 206c 696e 655f 666c  ])...def line_fl
+00012970: 7578 6573 2877 696e 646f 7773 2c77 6176  uxes(windows,wav
+00012980: 656c 656e 6774 682c 666c 7578 293a 0a20  elength,flux):. 
+00012990: 2020 2027 2727 0a20 2020 2052 6574 7572     '''.    Retur
+000129a0: 6e3a 2061 7272 6179 206f 6620 7375 6d20  n: array of sum 
+000129b0: 6f66 2069 6e74 6567 7261 7465 6420 6c69  of integrated li
+000129c0: 6e65 2066 6c75 7820 696e 2077 6176 656c  ne flux in wavel
+000129d0: 656e 6774 6820 7769 6e64 6f77 732e 0a0a  ength windows...
+000129e0: 2020 2020 556e 6974 733a 2052 6574 7572      Units: Retur
+000129f0: 6e20 6973 2069 6e20 7468 6520 7361 6d65  n is in the same
+00012a00: 2075 6e69 7420 6173 2069 6e70 7574 2e20   unit as input. 
+00012a10: 5b41 7373 756d 6564 2074 6f20 6265 2069  [Assumed to be i
+00012a20: 6e20 6572 672f 732f 636d 322f 7372 5d0a  n erg/s/cm2/sr].
+00012a30: 0a20 2020 2077 696e 646f 7773 3a20 6c69  .    windows: li
+00012a40: 7374 206f 6620 7761 7665 6c65 6e67 7468  st of wavelength
+00012a50: 206c 696d 6974 7320 6f66 2077 696e 646f   limits of windo
+00012a60: 7773 2e20 4578 616d 706c 653a 205b 5b31  ws. Example: [[1
+00012a70: 342c 3134 2e35 5d2c 5b31 352c 3136 2e32  4,14.5],[15,16.2
+00012a80: 5d2c 5b31 322e 352c 3134 2e31 5d5d 0a20  ],[12.5,14.1]]. 
+00012a90: 2020 2027 2727 0a20 2020 2046 3d5b 5d0a     '''.    F=[].
+00012aa0: 2020 2020 666f 7220 5720 696e 2077 696e      for W in win
+00012ab0: 646f 7773 3a0a 2020 2020 2020 2020 462e  dows:.        F.
+00012ac0: 6170 7065 6e64 286c 696e 655f 666c 7578  append(line_flux
+00012ad0: 2857 5b30 5d2c 575b 315d 2c77 6176 656c  (W[0],W[1],wavel
+00012ae0: 656e 6774 682c 666c 7578 2929 0a20 2020  ength,flux)).   
+00012af0: 2072 6574 7572 6e28 6e70 2e61 7272 6179   return(np.array
+00012b00: 2846 2929 0a0a 0a64 6566 206c 696e 655f  (F))...def line_
+00012b10: 666c 7578 5f72 6174 696f 7328 7261 7469  flux_ratios(rati
+00012b20: 6f5f 7769 6e64 6f77 732c 7761 7665 6c65  o_windows,wavele
+00012b30: 6e67 7468 2c66 6c75 7829 3a0a 2020 2020  ngth,flux):.    
+00012b40: 2727 270a 2020 2020 5265 7475 726e 3a20  '''.    Return: 
+00012b50: 496e 7465 6772 6174 6564 206c 696e 6520  Integrated line 
+00012b60: 666c 7578 2072 6174 696f 7320 6265 7477  flux ratios betw
+00012b70: 6565 6e20 7761 7665 6c65 6e67 7468 7320  een wavelengths 
+00012b80: 6c31 2061 6e64 206c 322e 0a0a 2020 2020  l1 and l2...    
+00012b90: 556e 6974 3a20 5265 7475 726e 2068 6173  Unit: Return has
+00012ba0: 206e 6f20 756e 6974 2e20 5b49 6e70 7574   no unit. [Input
+00012bb0: 2069 7320 6173 7375 6d65 6420 746f 2062   is assumed to b
+00012bc0: 6520 696e 2065 7267 2f73 2f63 6d32 2f73  e in erg/s/cm2/s
+00012bd0: 725d 0a0a 2020 2020 7261 7469 6f5f 7769  r]..    ratio_wi
+00012be0: 6e64 6f77 733a 206c 6973 7420 6f66 2077  ndows: list of w
+00012bf0: 6176 656c 656e 6774 6820 7769 6e64 6f77  avelength window
+00012c00: 732e 2045 7861 6d70 6c65 3a20 5b5b 5b31  s. Example: [[[1
+00012c10: 342c 3134 2e35 5d2c 5b31 352c 3136 2e32  4,14.5],[15,16.2
+00012c20: 5d5d 2c5b 5b31 322e 352c 3134 2e31 5d2c  ]],[[12.5,14.1],
+00012c30: 5b31 332e 342c 3133 2e38 5d5d 5d0a 2020  [13.4,13.8]]].  
+00012c40: 2020 2727 270a 2020 2020 523d 5b5d 0a20    '''.    R=[]. 
+00012c50: 2020 2066 6f72 2077 696e 646f 7720 696e     for window in
+00012c60: 2072 6174 696f 5f77 696e 646f 7773 3a0a   ratio_windows:.
+00012c70: 2020 2020 2020 2020 463d 6c69 6e65 5f66          F=line_f
+00012c80: 6c75 7865 7328 5b77 696e 646f 775b 305d  luxes([window[0]
+00012c90: 2c77 696e 646f 775b 315d 5d2c 7761 7665  ,window[1]],wave
+00012ca0: 6c65 6e67 7468 2c66 6c75 7829 0a20 2020  length,flux).   
+00012cb0: 2020 2020 2052 2e61 7070 656e 6428 465b       R.append(F[
+00012cc0: 315d 2f46 5b30 5d29 0a20 2020 2072 6574  1]/F[0]).    ret
+00012cd0: 7572 6e28 6e70 2e61 7272 6179 2852 2929  urn(np.array(R))
+00012ce0: 0a0a 0a64 6566 206c 696e 655f 666c 7578  ...def line_flux
+00012cf0: 5f70 726f 6475 6374 7328 7072 6f64 7563  _products(produc
+00012d00: 745f 7769 6e64 6f77 732c 7761 7665 6c65  t_windows,wavele
+00012d10: 6e67 7468 2c66 6c75 7829 3a0a 2020 2020  ngth,flux):.    
+00012d20: 2727 270a 2020 2020 5265 7475 726e 3a20  '''.    Return: 
+00012d30: 496e 7465 6772 6174 6564 206c 696e 6520  Integrated line 
+00012d40: 666c 7578 2070 726f 6475 6374 7320 6265  flux products be
+00012d50: 7477 6565 6e20 7761 7665 6c65 6e67 7468  tween wavelength
+00012d60: 7320 6c31 2061 6e64 206c 322e 0a0a 2020  s l1 and l2...  
+00012d70: 2020 556e 6974 3a20 5265 7475 726e 2075    Unit: Return u
+00012d80: 6e69 7420 6973 206f 7574 7075 7420 756e  nit is output un
+00012d90: 6974 7320 7371 7561 7265 642e 205b 496e  its squared. [In
+00012da0: 7075 7420 6973 2061 7373 756d 6564 2074  put is assumed t
+00012db0: 6f20 6265 2069 6e20 6572 672f 732f 636d  o be in erg/s/cm
+00012dc0: 322f 7372 5d0a 0a20 2020 2070 726f 6475  2/sr]..    produ
+00012dd0: 6374 5f77 696e 646f 7773 3a20 6c69 7374  ct_windows: list
+00012de0: 206f 6620 7761 7665 6c65 6e67 7468 2077   of wavelength w
+00012df0: 696e 646f 7773 2e20 4578 616d 706c 653a  indows. Example:
+00012e00: 205b 5b5b 3134 2c31 342e 355d 2c5b 3135   [[[14,14.5],[15
+00012e10: 2c31 362e 325d 5d2c 5b5b 3132 2e35 2c31  ,16.2]],[[12.5,1
+00012e20: 342e 315d 2c5b 3133 2e34 2c31 332e 385d  4.1],[13.4,13.8]
+00012e30: 5d5d 0a20 2020 2027 2727 0a20 2020 2052  ]].    '''.    R
+00012e40: 3d5b 5d0a 2020 2020 666f 7220 7769 6e64  =[].    for wind
+00012e50: 6f77 2069 6e20 7072 6f64 7563 745f 7769  ow in product_wi
+00012e60: 6e64 6f77 733a 0a20 2020 2020 2020 2046  ndows:.        F
+00012e70: 3d6c 696e 655f 666c 7578 6573 285b 7769  =line_fluxes([wi
+00012e80: 6e64 6f77 5b30 5d2c 7769 6e64 6f77 5b31  ndow[0],window[1
+00012e90: 5d5d 2c77 6176 656c 656e 6774 682c 666c  ]],wavelength,fl
+00012ea0: 7578 290a 2020 2020 2020 2020 522e 6170  ux).        R.ap
+00012eb0: 7065 6e64 2846 5b31 5d2a 465b 305d 290a  pend(F[1]*F[0]).
+00012ec0: 2020 2020 7265 7475 726e 286e 702e 6172      return(np.ar
+00012ed0: 7261 7928 5229 290a 0a0a 6465 6620 7370  ray(R))...def sp
+00012ee0: 6563 7472 616c 5f66 6c75 7828 6c31 2c6c  ectral_flux(l1,l
+00012ef0: 322c 7761 7665 6c65 6e67 7468 2c66 6c75  2,wavelength,flu
+00012f00: 7829 3a0a 2020 2020 2727 270a 2020 2020  x):.    '''.    
+00012f10: 556e 6974 3a20 5265 7475 726e 2069 6e20  Unit: Return in 
+00012f20: 5b65 7267 2f73 2f63 6d32 5d20 616e 6420  [erg/s/cm2] and 
+00012f30: 696e 7075 7420 6973 2069 6e20 5b4a 795d  input is in [Jy]
+00012f40: 206c 312c 206c 322c 2061 6e64 2077 6176   l1, l2, and wav
+00012f50: 656c 656e 6774 6820 696e 206d 6963 726f  elength in micro
+00012f60: 6e73 0a0a 2020 2020 5265 7475 726e 730a  ns..    Returns.
+00012f70: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00012f80: 666c 6f61 743a 0a20 2020 2020 2053 756d  float:.      Sum
+00012f90: 206f 6620 696e 7465 6772 6174 6564 206c   of integrated l
+00012fa0: 696e 6520 666c 7578 2062 6574 7765 656e  ine flux between
+00012fb0: 2077 6176 656c 656e 6774 6873 206c 3120   wavelengths l1 
+00012fc0: 616e 6420 6c32 2e0a 0a20 2020 2027 2727  and l2...    '''
+00012fd0: 0a20 2020 2066 6c75 783d 666c 7578 2a31  .    flux=flux*1
+00012fe0: 652d 3233 2020 2320 436f 6e76 6572 7469  e-23  # Converti
+00012ff0: 6e67 204a 7920 746f 2065 7267 2e73 e288  ng Jy to erg.s..
+00013000: 9231 2e63 6de2 8892 322e 487a e288 9231  .1.cm...2.Hz...1
+00013010: 0a20 2020 2077 6176 656c 656e 6774 683d  .    wavelength=
+00013020: 7761 7665 6c65 6e67 7468 2a31 652d 3420  wavelength*1e-4 
+00013030: 2023 2043 6f6e 7665 7274 696e 6720 6d69   # Converting mi
+00013040: 6372 6f6e 7320 746f 2063 6d0a 2020 2020  crons to cm.    
+00013050: 666c 7578 3d66 6c75 785b 6e70 2e61 7267  flux=flux[np.arg
+00013060: 736f 7274 2877 6176 656c 656e 6774 6829  sort(wavelength)
+00013070: 5d0a 2020 2020 7761 7665 6c65 6e67 7468  ].    wavelength
+00013080: 3d77 6176 656c 656e 6774 685b 6e70 2e61  =wavelength[np.a
+00013090: 7267 736f 7274 2877 6176 656c 656e 6774  rgsort(wavelengt
+000130a0: 6829 5d0a 2020 2020 6c31 3d6c 312a 3165  h)].    l1=l1*1e
+000130b0: 2d34 2020 2320 436f 6e76 6572 7469 6e67  -4  # Converting
+000130c0: 206d 6963 726f 6e73 2074 6f20 636d 0a20   microns to cm. 
+000130d0: 2020 206c 323d 6c32 2a31 652d 3420 2023     l2=l2*1e-4  #
+000130e0: 2043 6f6e 7665 7274 696e 6720 6d69 6372   Converting micr
+000130f0: 6f6e 7320 746f 2063 6d0a 2020 2020 635f  ons to cm.    c_
+00013100: 636d 733d 632a 3165 3220 2023 2043 6f6e  cms=c*1e2  # Con
+00013110: 7665 7274 696e 6720 6d2f 7320 746f 2063  verting m/s to c
+00013120: 6d2f 730a 2020 2020 6d61 736b 3d28 7761  m/s.    mask=(wa
+00013130: 7665 6c65 6e67 7468 3e6c 3129 2628 7761  velength>l1)&(wa
+00013140: 7665 6c65 6e67 7468 3c3d 6c32 290a 2020  velength<=l2).  
+00013150: 2020 7761 7665 3d77 6176 656c 656e 6774    wave=wavelengt
+00013160: 685b 6d61 736b 5d0a 2020 2020 2320 7761  h[mask].    # wa
+00013170: 7665 3120 2020 2020 203d 206e 702e 726f  ve1      = np.ro
+00013180: 6c6c 2877 6176 656c 656e 6774 682c 3129  ll(wavelength,1)
+00013190: 5b6d 6173 6b5d 0a20 2020 2023 2077 6176  [mask].    # wav
+000131a0: 6531 2020 2020 2020 3d20 3130 2a2a 2828  e1      = 10**((
+000131b0: 6e70 2e6c 6f67 3130 2877 6176 6529 2b6e  np.log10(wave)+n
+000131c0: 702e 6c6f 6731 3028 7761 7665 3129 292f  p.log10(wave1))/
+000131d0: 3229 0a20 2020 2023 2077 6176 6532 2020  2).    # wave2  
+000131e0: 2020 2020 3d20 6e70 2e72 6f6c 6c28 7761      = np.roll(wa
+000131f0: 7665 6c65 6e67 7468 2c2d 3129 5b6d 6173  velength,-1)[mas
+00013200: 6b5d 0a20 2020 2023 2077 6176 6532 2020  k].    # wave2  
+00013210: 2020 2020 3d20 3130 2a2a 2828 6e70 2e6c      = 10**((np.l
+00013220: 6f67 3130 2877 6176 6529 2b6e 702e 6c6f  og10(wave)+np.lo
+00013230: 6731 3028 7761 7665 3229 292f 3229 0a20  g10(wave2))/2). 
+00013240: 2020 2023 2064 6e75 2020 2020 2020 2020     # dnu        
+00013250: 3d20 632a 2877 6176 6532 2d77 6176 6531  = c*(wave2-wave1
+00013260: 292f 7761 7665 2a2a 322a 3165 320a 2020  )/wave**2*1e2.  
+00013270: 2020 7761 7665 313d 6e70 2e72 6f6c 6c28    wave1=np.roll(
+00013280: 7761 7665 6c65 6e67 7468 2c31 295b 6d61  wavelength,1)[ma
+00013290: 736b 5d0a 2020 2020 7761 7665 323d 6e70  sk].    wave2=np
+000132a0: 2e72 6f6c 6c28 7761 7665 6c65 6e67 7468  .roll(wavelength
+000132b0: 2c2d 3129 5b6d 6173 6b5d 0a20 2020 2064  ,-1)[mask].    d
+000132c0: 6e75 3d28 635f 636d 732a 2831 2f77 6176  nu=(c_cms*(1/wav
+000132d0: 6531 2d31 2f77 6176 6532 292f 3229 0a20  e1-1/wave2)/2). 
+000132e0: 2020 2072 6574 7572 6e28 6e70 2e73 756d     return(np.sum
+000132f0: 2866 6c75 785b 6d61 736b 5d2a 646e 7529  (flux[mask]*dnu)
+00013300: 290a 0a0a 6465 6620 7370 6563 7472 616c  )...def spectral
+00013310: 5f66 6c75 7865 7328 7769 6e64 6f77 732c  _fluxes(windows,
+00013320: 7761 7665 6c65 6e67 7468 2c66 6c75 7829  wavelength,flux)
+00013330: 3a0a 2020 2020 2727 270a 2020 2020 5265  :.    '''.    Re
+00013340: 7475 726e 3a20 5375 6d20 6f66 2069 6e74  turn: Sum of int
+00013350: 6567 7261 7465 6420 6c69 6e65 2066 6c75  egrated line flu
+00013360: 7820 6265 7477 6565 6e20 7761 7665 6c65  x between wavele
+00013370: 6e67 7468 2077 696e 646f 7773 2e0a 0a20  ngth windows... 
+00013380: 2020 2055 6e69 743a 2072 6574 7572 6e20     Unit: return 
+00013390: 6973 2069 6e20 5b65 7267 2f73 2f63 6d32  is in [erg/s/cm2
+000133a0: 5d20 616e 6420 696e 7075 7420 6973 2069  ] and input is i
+000133b0: 6e20 5b4a 795d 0a0a 2020 2020 7769 6e64  n [Jy]..    wind
+000133c0: 6f77 733a 206c 6973 7420 6f66 2077 6176  ows: list of wav
+000133d0: 656c 656e 6774 6820 6c69 6d69 7473 2028  elength limits (
+000133e0: 6d69 6372 6f6e 7329 206f 6620 7769 6e64  microns) of wind
+000133f0: 6f77 732e 2045 7861 6d70 6c65 3a20 5b5b  ows. Example: [[
+00013400: 3134 2c31 342e 355d 2c5b 3135 2c31 362e  14,14.5],[15,16.
+00013410: 325d 2c5b 3132 2e35 2c31 342e 315d 5d0a  2],[12.5,14.1]].
+00013420: 2020 2020 2727 270a 2020 2020 463d 5b5d      '''.    F=[]
+00013430: 0a20 2020 2066 6f72 2057 2069 6e20 7769  .    for W in wi
+00013440: 6e64 6f77 733a 0a20 2020 2020 2020 2046  ndows:.        F
+00013450: 2e61 7070 656e 6428 7370 6563 7472 616c  .append(spectral
+00013460: 5f66 6c75 7828 575b 305d 2c57 5b31 5d2c  _flux(W[0],W[1],
+00013470: 7761 7665 6c65 6e67 7468 2c66 6c75 7829  wavelength,flux)
+00013480: 290a 2020 2020 7265 7475 726e 286e 702e  ).    return(np.
+00013490: 6172 7261 7928 4629 290a 0a0a 6465 6620  array(F))...def 
+000134a0: 7370 6563 7472 616c 5f66 6c75 785f 7261  spectral_flux_ra
+000134b0: 7469 6f73 2872 6174 696f 5f77 696e 646f  tios(ratio_windo
+000134c0: 7773 2c77 6176 656c 656e 6774 682c 666c  ws,wavelength,fl
+000134d0: 7578 293a 0a20 2020 2027 2727 0a20 2020  ux):.    '''.   
+000134e0: 2052 6574 7572 6e3a 2053 7065 6374 7261   Return: Spectra
+000134f0: 6c20 696e 7465 6772 6174 6564 2066 6c75  l integrated flu
+00013500: 7820 7261 7469 6f73 2062 6574 7765 656e  x ratios between
+00013510: 2077 6176 656c 656e 6774 6820 7769 6e64   wavelength wind
+00013520: 6f77 732e 0a0a 2020 2020 556e 6974 733a  ows...    Units:
+00013530: 2052 6574 7572 6e20 6973 2077 6974 686f   Return is witho
+00013540: 7574 2075 6e69 7473 2061 6e64 2069 6e70  ut units and inp
+00013550: 7574 2069 7320 696e 205b 4a79 5d0a 0a20  ut is in [Jy].. 
+00013560: 2020 2072 6174 696f 5f77 696e 646f 7773     ratio_windows
+00013570: 3a20 6c69 7374 206f 6620 7761 7665 6c65  : list of wavele
+00013580: 6e67 7468 2028 6d69 6372 6f6e 7329 2077  ngth (microns) w
+00013590: 696e 646f 7773 2e20 4578 616d 706c 653a  indows. Example:
+000135a0: 205b 5b5b 3134 2c31 342e 355d 2c5b 3135   [[[14,14.5],[15
+000135b0: 2c31 362e 325d 5d2c 5b5b 3132 2e35 2c31  ,16.2]],[[12.5,1
+000135c0: 342e 315d 2c5b 3133 2e34 2c31 332e 385d  4.1],[13.4,13.8]
+000135d0: 5d5d 0a20 2020 2027 2727 0a20 2020 2052  ]].    '''.    R
+000135e0: 3d5b 5d0a 2020 2020 666f 7220 7769 6e64  =[].    for wind
+000135f0: 6f77 2069 6e20 7261 7469 6f5f 7769 6e64  ow in ratio_wind
+00013600: 6f77 733a 0a20 2020 2020 2020 2046 3d73  ows:.        F=s
+00013610: 7065 6374 7261 6c5f 666c 7578 6573 285b  pectral_fluxes([
+00013620: 7769 6e64 6f77 5b30 5d2c 7769 6e64 6f77  window[0],window
+00013630: 5b31 5d5d 2c77 6176 656c 656e 6774 682c  [1]],wavelength,
+00013640: 666c 7578 290a 2020 2020 2020 2020 522e  flux).        R.
+00013650: 6170 7065 6e64 2846 5b31 5d2f 465b 305d  append(F[1]/F[0]
+00013660: 290a 2020 2020 7265 7475 726e 286e 702e  ).    return(np.
+00013670: 6172 7261 7928 5229 290a 0a0a 6465 6620  array(R))...def 
+00013680: 7370 6563 7472 616c 5f66 6c75 785f 7072  spectral_flux_pr
+00013690: 6f64 7563 7473 2870 726f 6475 6374 5f77  oducts(product_w
+000136a0: 696e 646f 7773 2c77 6176 656c 656e 6774  indows,wavelengt
+000136b0: 682c 666c 7578 293a 0a20 2020 2027 2727  h,flux):.    '''
+000136c0: 0a20 2020 2052 6574 7572 6e3a 2050 726f  .    Return: Pro
+000136d0: 6475 6374 7320 6f66 2073 7065 6374 7261  ducts of spectra
+000136e0: 6c20 696e 7465 6772 6174 6564 2066 6c75  l integrated flu
+000136f0: 7865 7320 6265 7477 6565 6e20 7761 7665  xes between wave
+00013700: 6c65 6e67 7468 2077 696e 646f 7773 2e0a  length windows..
+00013710: 0a20 2020 2055 6e69 7473 3a20 5265 7475  .    Units: Retu
+00013720: 726e 2075 6e69 7420 6973 206f 7574 7075  rn unit is outpu
+00013730: 7420 756e 6974 7320 7371 7561 7265 6420  t units squared 
+00013740: 616e 6420 696e 7075 7420 6973 2069 6e20  and input is in 
+00013750: 5b4a 795d 0a0a 2020 2020 7072 6f64 7563  [Jy]..    produc
+00013760: 745f 7769 6e64 6f77 733a 206c 6973 7420  t_windows: list 
+00013770: 6f66 2077 6176 656c 656e 6774 6820 286d  of wavelength (m
+00013780: 6963 726f 6e73 2920 7769 6e64 6f77 732e  icrons) windows.
+00013790: 2045 7861 6d70 6c65 3a20 5b5b 5b31 342c   Example: [[[14,
+000137a0: 3134 2e35 5d2c 5b31 352c 3136 2e32 5d5d  14.5],[15,16.2]]
+000137b0: 2c5b 5b31 322e 352c 3134 2e31 5d2c 5b31  ,[[12.5,14.1],[1
+000137c0: 332e 342c 3133 2e38 5d5d 5d0a 2020 2020  3.4,13.8]]].    
+000137d0: 2727 270a 2020 2020 523d 5b5d 0a20 2020  '''.    R=[].   
+000137e0: 2066 6f72 2077 696e 646f 7720 696e 2070   for window in p
+000137f0: 726f 6475 6374 5f77 696e 646f 7773 3a0a  roduct_windows:.
+00013800: 2020 2020 2020 2020 463d 7370 6563 7472          F=spectr
+00013810: 616c 5f66 6c75 7865 7328 5b77 696e 646f  al_fluxes([windo
+00013820: 775b 305d 2c77 696e 646f 775b 315d 5d2c  w[0],window[1]],
+00013830: 7761 7665 6c65 6e67 7468 2c66 6c75 7829  wavelength,flux)
+00013840: 0a20 2020 2020 2020 2052 2e61 7070 656e  .        R.appen
+00013850: 6428 465b 315d 2a46 5b30 5d29 0a20 2020  d(F[1]*F[0]).   
+00013860: 2072 6574 7572 6e28 6e70 2e61 7272 6179   return(np.array
+00013870: 2852 2929 0a0a 0a64 6566 2063 6869 325f  (R))...def chi2_
+00013880: 736c 6162 2873 6c61 625f 6461 7461 2c73  slab(slab_data,s
+00013890: 7065 6374 7261 2c77 696e 646f 7773 3d5b  pectra,windows=[
+000138a0: 5d2c 7261 7469 6f5f 7769 6e64 6f77 733d  ],ratio_windows=
+000138b0: 5b5d 2c70 726f 6475 6374 5f77 696e 646f  [],product_windo
+000138c0: 7773 3d5b 5d2c 5264 6973 6b3d 6e70 2e6c  ws=[],Rdisk=np.l
+000138d0: 6f67 7370 6163 6528 2d32 2c32 2c31 3029  ogspace(-2,2,10)
+000138e0: 2c64 6973 7461 6e63 653d 3132 302c 636f  ,distance=120,co
+000138f0: 6e76 6f6c 7665 3d46 616c 7365 2c4e 4c54  nvolve=False,NLT
+00013900: 453d 4661 6c73 652c 7368 6f72 745f 666f  E=False,short_fo
+00013910: 726d 6174 3d46 616c 7365 293a 0a20 2020  rmat=False):.   
+00013920: 2027 2727 0a20 2020 2052 6574 7572 6e73   '''.    Returns
+00013930: 2063 6869 3220 6261 7365 6420 6f6e 2073   chi2 based on s
+00013940: 656c 6563 7465 6420 7370 6563 7472 616c  elected spectral
+00013950: 2077 696e 646f 7773 2061 6372 6f73 7320   windows across 
+00013960: 6469 6666 6572 656e 7420 656d 6974 7469  different emitti
+00013970: 6e67 2064 6973 6b20 7261 6469 7573 0a0a  ng disk radius..
+00013980: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00013990: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000139a0: 2020 736c 6162 5f64 6174 6120 3a20 7374    slab_data : st
+000139b0: 7269 6e67 206f 7220 736c 6162 5f6d 6f64  ring or slab_mod
+000139c0: 656c 2069 6e73 7461 6e63 650a 2020 2020  el instance.    
+000139d0: 2020 7061 7468 2063 6f72 7265 7370 6f6e    path correspon
+000139e0: 6469 6e67 2074 6f20 6120 7369 6e67 6c65  ding to a single
+000139f0: 2073 6c61 6220 6d6f 6465 6c20 6f72 2061   slab model or a
+00013a00: 2073 696e 676c 6520 736c 6162 5f6d 6f64   single slab_mod
+00013a10: 656c 2069 6e73 7461 6e63 650a 0a20 2020  el instance..   
+00013a20: 2073 7065 6374 7261 203a 206e 756d 7079   spectra : numpy
+00013a30: 2e61 7272 6179 0a20 2020 2020 206e 756d  .array.      num
+00013a40: 7079 2061 7272 6179 2077 6974 6820 6669  py array with fi
+00013a50: 7273 7420 636f 6c75 6d6e 2074 6865 2077  rst column the w
+00013a60: 6176 656c 656e 6774 6820 696e 205b 6d69  avelength in [mi
+00013a70: 6372 6f6e 735d 2061 6e64 2073 6563 6f6e  crons] and secon
+00013a80: 6420 636f 6c75 6d6e 2066 6c75 7820 696e  d column flux in
+00013a90: 205b 4a79 5d0a 0a20 2020 2077 696e 646f   [Jy]..    windo
+00013aa0: 7773 203a 2061 7272 6179 5f6c 696b 650a  ws : array_like.
+00013ab0: 2020 2020 2020 4c69 7374 206f 6620 7370        List of sp
+00013ac0: 6563 7472 616c 2077 696e 646f 7773 2066  ectral windows f
+00013ad0: 6f72 2063 6869 3220 6361 6c63 756c 6174  or chi2 calculat
+00013ae0: 696f 6e20 2877 6569 6768 7473 206f 7074  ion (weights opt
+00013af0: 696f 6e61 6c29 2e20 466f 726d 6174 203a  ional). Format :
+00013b00: 205b 7769 6e64 6f77 312c 7769 6e64 6f77   [window1,window
+00013b10: 322c 2e2e 2e2e 5d0a 2020 2020 2020 5769  2,....].      Wi
+00013b20: 6e64 6f77 2066 6f72 6d61 743a 205b 6c61  ndow format: [la
+00013b30: 6d62 6461 5f30 2c20 6c61 6d62 6461 5f31  mbda_0, lambda_1
+00013b40: 2c20 7765 6967 6874 5d20 7765 6967 6874  , weight] weight
+00013b50: 2069 7320 6f70 7469 6f6e 616c 2c20 7573   is optional, us
+00013b60: 6564 2066 6f72 2077 6569 6768 7465 6420  ed for weighted 
+00013b70: 6368 6932 0a20 2020 2020 2045 7861 6d70  chi2.      Examp
+00013b80: 6c65 2077 6974 686f 7574 2077 6569 6768  le without weigh
+00013b90: 743a 205b 5b31 342c 3134 2e35 5d2c 5b31  t: [[14,14.5],[1
+00013ba0: 352c 3136 2e32 5d2c 5b31 322e 352c 3134  5,16.2],[12.5,14
+00013bb0: 2e31 5d5d 0a20 2020 2020 2045 7861 6d70  .1]].      Examp
+00013bc0: 6c65 2077 6974 6820 7765 6967 6874 3a20  le with weight: 
+00013bd0: 5b5b 3134 2c31 342e 352c 325d 2c5b 3135  [[14,14.5,2],[15
+00013be0: 2c31 362e 322c 355d 2c5b 3132 2e35 2c31  ,16.2,5],[12.5,1
+00013bf0: 342e 312c 315d 5d0a 2020 2020 2020 5765  4.1,1]].      We
+00013c00: 6967 6874 7320 6172 6520 6175 746f 6d61  ights are automa
+00013c10: 7469 6361 6c6c 7920 6e6f 726d 616c 6973  tically normalis
+00013c20: 6564 2c20 736f 2073 756d 206f 6620 7765  ed, so sum of we
+00013c30: 6967 6874 7320 6e65 6564 206e 6f74 2062  ights need not b
+00013c40: 6520 310a 0a20 2020 2052 6469 736b 203a  e 1..    Rdisk :
+00013c50: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
+00013c60: 2020 5261 6469 7573 2063 6f72 7265 7370    Radius corresp
+00013c70: 6f6e 6469 6e67 2074 6f20 656d 6974 7469  onding to emitti
+00013c80: 6e67 2061 7265 6120 696e 2061 7374 726f  ng area in astro
+00013c90: 6e6f 6d69 6361 6c20 756e 6974 730a 0a20  nomical units.. 
+00013ca0: 2020 2064 6973 7461 6e63 6520 3a20 666c     distance : fl
+00013cb0: 6f61 740a 2020 2020 2020 6469 7374 616e  oat.      distan
+00013cc0: 6365 206f 6620 6469 736b 2069 6e20 7061  ce of disk in pa
+00013cd0: 7273 6563 0a0a 2020 2020 636f 6e76 6f6c  rsec..    convol
+00013ce0: 7665 203a 2062 6f6f 6c65 616e 0a20 2020  ve : boolean.   
+00013cf0: 2020 2049 6620 5472 7565 2c20 7468 6520     If True, the 
+00013d00: 6368 6932 2069 7320 7065 7266 6f72 6d65  chi2 is performe
+00013d10: 6420 6f6e 2063 6f6e 766f 6c76 6564 2073  d on convolved s
+00013d20: 7065 6374 7261 2061 6e64 206e 6f74 206f  pectra and not o
+00013d30: 6e20 696e 6469 7669 6475 616c 206c 696e  n individual lin
+00013d40: 6573 0a0a 2020 2020 4e4c 5445 203a 2062  es..    NLTE : b
+00013d50: 6f6f 6c65 616e 0a20 2020 2020 2069 6620  oolean.      if 
+00013d60: 5472 7565 2c20 4e4c 5445 2066 6c75 7820  True, NLTE flux 
+00013d70: 6973 2074 616b 656e 2066 726f 6d20 7468  is taken from th
+00013d80: 6520 736c 6162 206d 6f64 656c 2e0a 2020  e slab model..  
+00013d90: 2020 2727 270a 2020 2020 6172 6561 3d6e    '''.    area=n
+00013da0: 702e 7069 2a28 5264 6973 6b2a 6175 2f64  p.pi*(Rdisk*au/d
+00013db0: 6973 7461 6e63 652f 7063 292a 2a32 0a20  istance/pc)**2. 
+00013dc0: 2020 2063 6869 5f61 7265 613d 6e70 2e7a     chi_area=np.z
+00013dd0: 6572 6f73 2828 6c65 6e28 6172 6561 2929  eros((len(area))
+00013de0: 290a 2020 2020 6966 2069 7369 6e73 7461  ).    if isinsta
+00013df0: 6e63 6528 736c 6162 5f64 6174 612c 7374  nce(slab_data,st
+00013e00: 7229 3a20 736c 6162 5f64 6174 613d 7265  r): slab_data=re
+00013e10: 6164 5f73 6c61 6228 736c 6162 5f64 6174  ad_slab(slab_dat
+00013e20: 612c 7665 7262 6f73 653d 4661 6c73 652c  a,verbose=False,
+00013e30: 7368 6f72 745f 666f 726d 6174 3d73 686f  short_format=sho
+00013e40: 7274 5f66 6f72 6d61 7429 0a20 2020 2069  rt_format).    i
+00013e50: 6620 6c65 6e28 7769 6e64 6f77 7329 3c30  f len(windows)<0
+00013e60: 2061 6e64 206c 656e 2872 6174 696f 5f77   and len(ratio_w
+00013e70: 696e 646f 7773 293c 3020 616e 6420 6c65  indows)<0 and le
+00013e80: 6e28 7072 6f64 7563 745f 7769 6e64 6f77  n(product_window
+00013e90: 7329 3c30 3a20 7265 7475 726e 2063 6869  s)<0: return chi
+00013ea0: 5f61 7265 610a 2020 2020 6966 2063 6f6e  _area.    if con
+00013eb0: 766f 6c76 653a 2020 2320 746f 2065 7374  volve:  # to est
+00013ec0: 696d 6174 6520 666c 7578 2066 726f 6d20  imate flux from 
+00013ed0: 636f 6e76 6f6c 7665 6420 7370 6563 7472  convolved spectr
+00013ee0: 610a 2020 2020 2020 2020 6c6d 696e 2c6c  a.        lmin,l
+00013ef0: 6d61 783d 5b5d 2c5b 5d0a 2020 2020 2020  max=[],[].      
+00013f00: 2020 6966 206c 656e 2877 696e 646f 7773    if len(windows
+00013f10: 293e 303a 0a20 2020 2020 2020 2020 2020  )>0:.           
+00013f20: 206c 6d69 6e2e 6170 7065 6e64 286e 702e   lmin.append(np.
+00013f30: 616d 696e 286e 702e 6172 7261 7928 5b5b  amin(np.array([[
+00013f40: 695b 305d 2c69 5b31 5d5d 2066 6f72 2069  i[0],i[1]] for i
+00013f50: 2069 6e20 7769 6e64 6f77 735d 292e 666c   in windows]).fl
+00013f60: 6174 7465 6e28 2929 290a 2020 2020 2020  atten())).      
+00013f70: 2020 2020 2020 6c6d 6178 2e61 7070 656e        lmax.appen
+00013f80: 6428 6e70 2e61 6d61 7828 6e70 2e61 7272  d(np.amax(np.arr
+00013f90: 6179 285b 5b69 5b30 5d2c 695b 315d 5d20  ay([[i[0],i[1]] 
+00013fa0: 666f 7220 6920 696e 2077 696e 646f 7773  for i in windows
+00013fb0: 5d29 2e66 6c61 7474 656e 2829 2929 0a20  ]).flatten())). 
+00013fc0: 2020 2020 2020 2069 6620 6c65 6e28 7261         if len(ra
+00013fd0: 7469 6f5f 7769 6e64 6f77 7329 3e30 3a0a  tio_windows)>0:.
+00013fe0: 2020 2020 2020 2020 2020 2020 6c6d 696e              lmin
+00013ff0: 2e61 7070 656e 6428 6e70 2e61 6d69 6e28  .append(np.amin(
+00014000: 6e70 2e61 7272 6179 285b 5b69 5b30 5d2c  np.array([[i[0],
+00014010: 695b 315d 5d20 666f 7220 6920 696e 2072  i[1]] for i in r
+00014020: 6174 696f 5f77 696e 646f 7773 5d29 2e66  atio_windows]).f
+00014030: 6c61 7474 656e 2829 2929 0a20 2020 2020  latten())).     
+00014040: 2020 2020 2020 206c 6d61 782e 6170 7065         lmax.appe
+00014050: 6e64 286e 702e 616d 6178 286e 702e 6172  nd(np.amax(np.ar
+00014060: 7261 7928 5b5b 695b 305d 2c69 5b31 5d5d  ray([[i[0],i[1]]
+00014070: 2066 6f72 2069 2069 6e20 7261 7469 6f5f   for i in ratio_
+00014080: 7769 6e64 6f77 735d 292e 666c 6174 7465  windows]).flatte
+00014090: 6e28 2929 290a 2020 2020 2020 2020 6966  n())).        if
+000140a0: 206c 656e 2870 726f 6475 6374 5f77 696e   len(product_win
+000140b0: 646f 7773 293e 303a 0a20 2020 2020 2020  dows)>0:.       
+000140c0: 2020 2020 206c 6d69 6e2e 6170 7065 6e64       lmin.append
+000140d0: 286e 702e 616d 696e 286e 702e 6172 7261  (np.amin(np.arra
+000140e0: 7928 5b5b 695b 305d 2c69 5b31 5d5d 2066  y([[i[0],i[1]] f
+000140f0: 6f72 2069 2069 6e20 7072 6f64 7563 745f  or i in product_
+00014100: 7769 6e64 6f77 735d 292e 666c 6174 7465  windows]).flatte
+00014110: 6e28 2929 290a 2020 2020 2020 2020 2020  n())).          
+00014120: 2020 6c6d 6178 2e61 7070 656e 6428 6e70    lmax.append(np
+00014130: 2e61 6d61 7828 6e70 2e61 7272 6179 285b  .amax(np.array([
+00014140: 5b69 5b30 5d2c 695b 315d 5d20 666f 7220  [i[0],i[1]] for 
+00014150: 6920 696e 2070 726f 6475 6374 5f77 696e  i in product_win
+00014160: 646f 7773 5d29 2e66 6c61 7474 656e 2829  dows]).flatten()
+00014170: 2929 0a20 2020 2020 2020 206c 6d69 6e3d  )).        lmin=
+00014180: 6e70 2e61 6d69 6e28 6c6d 696e 290a 2020  np.amin(lmin).  
+00014190: 2020 2020 2020 6c6d 6178 3d6e 702e 616d        lmax=np.am
+000141a0: 6178 286c 6d61 7829 0a20 2020 2020 2020  ax(lmax).       
+000141b0: 2073 6c61 625f 6461 7461 2e63 6f6e 766f   slab_data.convo
+000141c0: 6c76 6528 523d 3230 3030 2c6c 616d 6264  lve(R=2000,lambd
+000141d0: 615f 303d 6c6d 696e 2a30 2e39 2c6c 616d  a_0=lmin*0.9,lam
+000141e0: 6264 615f 6e3d 6c6d 6178 2a31 2e31 2c4e  bda_n=lmax*1.1,N
+000141f0: 4c54 453d 4e4c 5445 2c76 6572 626f 7365  LTE=NLTE,verbose
+00014200: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00014210: 6966 204e 4c54 453a 0a20 2020 2020 2020  if NLTE:.       
+00014220: 2020 2020 2046 6d6f 6465 6c3d 7370 6563       Fmodel=spec
+00014230: 7472 616c 5f66 6c75 7865 7328 7769 6e64  tral_fluxes(wind
+00014240: 6f77 732c 736c 6162 5f64 6174 612e 636f  ows,slab_data.co
+00014250: 6e76 5761 7665 6c65 6e67 7468 2c73 6c61  nvWavelength,sla
+00014260: 625f 6461 7461 2e63 6f6e 764e 4c54 4566  b_data.convNLTEf
+00014270: 6c75 782a 3165 3233 290a 2020 2020 2020  lux*1e23).      
+00014280: 2020 2020 2020 526d 6f64 656c 3d73 7065        Rmodel=spe
+00014290: 6374 7261 6c5f 666c 7578 5f72 6174 696f  ctral_flux_ratio
+000142a0: 7328 7261 7469 6f5f 7769 6e64 6f77 732c  s(ratio_windows,
+000142b0: 736c 6162 5f64 6174 612e 636f 6e76 5761  slab_data.convWa
+000142c0: 7665 6c65 6e67 7468 2c73 6c61 625f 6461  velength,slab_da
+000142d0: 7461 2e63 6f6e 764e 4c54 4566 6c75 782a  ta.convNLTEflux*
+000142e0: 3165 3233 290a 2020 2020 2020 2020 2020  1e23).          
+000142f0: 2020 506d 6f64 656c 3d73 7065 6374 7261    Pmodel=spectra
+00014300: 6c5f 666c 7578 5f70 726f 6475 6374 7328  l_flux_products(
+00014310: 7072 6f64 7563 745f 7769 6e64 6f77 732c  product_windows,
+00014320: 736c 6162 5f64 6174 612e 636f 6e76 5761  slab_data.convWa
+00014330: 7665 6c65 6e67 7468 2c73 6c61 625f 6461  velength,slab_da
+00014340: 7461 2e63 6f6e 764e 4c54 4566 6c75 782a  ta.convNLTEflux*
+00014350: 3165 3233 290a 2020 2020 2020 2020 656c  1e23).        el
+00014360: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00014370: 466d 6f64 656c 3d73 7065 6374 7261 6c5f  Fmodel=spectral_
+00014380: 666c 7578 6573 2877 696e 646f 7773 2c73  fluxes(windows,s
+00014390: 6c61 625f 6461 7461 2e63 6f6e 7657 6176  lab_data.convWav
+000143a0: 656c 656e 6774 682c 736c 6162 5f64 6174  elength,slab_dat
+000143b0: 612e 636f 6e76 4c54 4566 6c75 782a 3165  a.convLTEflux*1e
+000143c0: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
+000143d0: 526d 6f64 656c 3d73 7065 6374 7261 6c5f  Rmodel=spectral_
+000143e0: 666c 7578 5f72 6174 696f 7328 7261 7469  flux_ratios(rati
+000143f0: 6f5f 7769 6e64 6f77 732c 736c 6162 5f64  o_windows,slab_d
+00014400: 6174 612e 636f 6e76 5761 7665 6c65 6e67  ata.convWaveleng
+00014410: 7468 2c73 6c61 625f 6461 7461 2e63 6f6e  th,slab_data.con
+00014420: 764c 5445 666c 7578 2a31 6532 3329 0a20  vLTEflux*1e23). 
+00014430: 2020 2020 2020 2020 2020 2050 6d6f 6465             Pmode
+00014440: 6c3d 7370 6563 7472 616c 5f66 6c75 785f  l=spectral_flux_
+00014450: 7072 6f64 7563 7473 2870 726f 6475 6374  products(product
+00014460: 5f77 696e 646f 7773 2c73 6c61 625f 6461  _windows,slab_da
+00014470: 7461 2e63 6f6e 7657 6176 656c 656e 6774  ta.convWavelengt
+00014480: 682c 736c 6162 5f64 6174 612e 636f 6e76  h,slab_data.conv
+00014490: 4c54 4566 6c75 782a 3165 3233 290a 2020  LTEflux*1e23).  
+000144a0: 2020 656c 7365 3a20 2023 2074 6f20 6573    else:  # to es
+000144b0: 7469 6d61 7465 2066 6c75 7820 6672 6f6d  timate flux from
+000144c0: 206c 696e 6520 6c69 7374 0a20 2020 2020   line list.     
+000144d0: 2020 2069 6620 4e4c 5445 3a0a 2020 2020     if NLTE:.    
+000144e0: 2020 2020 2020 2020 743d 2746 4e4c 5445          t='FNLTE
+000144f0: 270a 2020 2020 2020 2020 656c 7365 3a0a  '.        else:.
+00014500: 2020 2020 2020 2020 2020 2020 743d 2746              t='F
+00014510: 4c54 4527 0a20 2020 2020 2020 206c 696e  LTE'.        lin
+00014520: 6564 6174 613d 736c 6162 5f64 6174 612e  edata=slab_data.
+00014530: 6c69 6e65 6461 7461 0a20 2020 2020 2020  linedata.       
+00014540: 206c 696e 6564 6174 612e 736f 7274 5f76   linedata.sort_v
+00014550: 616c 7565 7328 6279 3d5b 2747 487a 275d  alues(by=['GHz']
+00014560: 2c61 7363 656e 6469 6e67 3d46 616c 7365  ,ascending=False
+00014570: 2c69 6e70 6c61 6365 3d54 7275 652c 6967  ,inplace=True,ig
+00014580: 6e6f 7265 5f69 6e64 6578 3d54 7275 6529  nore_index=True)
+00014590: 0a20 2020 2020 2020 2046 6d6f 6465 6c3d  .        Fmodel=
+000145a0: 6c69 6e65 5f66 6c75 7865 7328 7769 6e64  line_fluxes(wind
+000145b0: 6f77 732c 632f 6c69 6e65 6461 7461 5b27  ows,c/linedata['
+000145c0: 4748 7a27 5d2a 3165 2d33 2c6c 696e 6564  GHz']*1e-3,lined
+000145d0: 6174 615b 745d 290a 2020 2020 2020 2020  ata[t]).        
+000145e0: 526d 6f64 656c 3d6c 696e 655f 666c 7578  Rmodel=line_flux
+000145f0: 5f72 6174 696f 7328 7261 7469 6f5f 7769  _ratios(ratio_wi
+00014600: 6e64 6f77 732c 632f 6c69 6e65 6461 7461  ndows,c/linedata
+00014610: 5b27 4748 7a27 5d2a 3165 2d33 2c6c 696e  ['GHz']*1e-3,lin
+00014620: 6564 6174 615b 745d 290a 2020 2020 2020  edata[t]).      
+00014630: 2020 506d 6f64 656c 3d6c 696e 655f 666c    Pmodel=line_fl
+00014640: 7578 5f72 6174 696f 7328 7072 6f64 7563  ux_ratios(produc
+00014650: 745f 7769 6e64 6f77 732c 632f 6c69 6e65  t_windows,c/line
+00014660: 6461 7461 5b27 4748 7a27 5d2a 3165 2d33  data['GHz']*1e-3
+00014670: 2c6c 696e 6564 6174 615b 745d 290a 2020  ,linedata[t]).  
+00014680: 2020 466f 6273 6572 7665 643d 7370 6563    Fobserved=spec
+00014690: 7472 616c 5f66 6c75 7865 7328 7769 6e64  tral_fluxes(wind
+000146a0: 6f77 732c 7370 6563 7472 615b 3a2c 305d  ows,spectra[:,0]
+000146b0: 2c73 7065 6374 7261 5b3a 2c31 5d29 0a20  ,spectra[:,1]). 
+000146c0: 2020 2052 6f62 7365 7276 6564 3d73 7065     Robserved=spe
+000146d0: 6374 7261 6c5f 666c 7578 5f72 6174 696f  ctral_flux_ratio
+000146e0: 7328 7261 7469 6f5f 7769 6e64 6f77 732c  s(ratio_windows,
+000146f0: 7370 6563 7472 615b 3a2c 305d 2c73 7065  spectra[:,0],spe
+00014700: 6374 7261 5b3a 2c31 5d29 0a20 2020 2050  ctra[:,1]).    P
+00014710: 6f62 7365 7276 6564 3d73 7065 6374 7261  observed=spectra
+00014720: 6c5f 666c 7578 5f70 726f 6475 6374 7328  l_flux_products(
+00014730: 7072 6f64 7563 745f 7769 6e64 6f77 732c  product_windows,
+00014740: 7370 6563 7472 615b 3a2c 305d 2c73 7065  spectra[:,0],spe
+00014750: 6374 7261 5b3a 2c31 5d29 0a20 2020 206e  ctra[:,1]).    n
+00014760: 6f72 6d5f 6661 6374 6f72 3d30 0a20 2020  orm_factor=0.   
+00014770: 2069 6620 6c65 6e28 7769 6e64 6f77 7329   if len(windows)
+00014780: 3e30 3a0a 2020 2020 2020 2020 6172 6561  >0:.        area
+00014790: 5f32 643d 6e70 2e64 7374 6163 6b28 5b61  _2d=np.dstack([a
+000147a0: 7265 6120 666f 7220 6920 696e 2072 616e  rea for i in ran
+000147b0: 6765 286c 656e 2877 696e 646f 7773 2929  ge(len(windows))
+000147c0: 5d29 2e73 7175 6565 7a65 2829 2e72 6573  ]).squeeze().res
+000147d0: 6861 7065 2828 6c65 6e28 6172 6561 292c  hape((len(area),
+000147e0: 6c65 6e28 7769 6e64 6f77 7329 2929 0a20  len(windows))). 
+000147f0: 2020 2020 2020 2046 6d6f 6465 6c5f 3264         Fmodel_2d
+00014800: 3d6e 702e 6473 7461 636b 285b 466d 6f64  =np.dstack([Fmod
+00014810: 656c 2066 6f72 2069 2069 6e20 7261 6e67  el for i in rang
+00014820: 6528 6c65 6e28 6172 6561 2929 5d29 2e73  e(len(area))]).s
+00014830: 7175 6565 7a65 2829 2e54 2e72 6573 6861  queeze().T.resha
+00014840: 7065 2828 6c65 6e28 6172 6561 292c 6c65  pe((len(area),le
+00014850: 6e28 7769 6e64 6f77 7329 2929 0a20 2020  n(windows))).   
+00014860: 2020 2020 2046 6f62 7365 7276 6564 5f32       Fobserved_2
+00014870: 643d 6e70 2e64 7374 6163 6b28 5b46 6f62  d=np.dstack([Fob
+00014880: 7365 7276 6564 2066 6f72 2069 2069 6e20  served for i in 
+00014890: 7261 6e67 6528 6c65 6e28 6172 6561 2929  range(len(area))
+000148a0: 5d29 2e73 7175 6565 7a65 2829 2e54 2e72  ]).squeeze().T.r
+000148b0: 6573 6861 7065 2828 6c65 6e28 6172 6561  eshape((len(area
+000148c0: 292c 6c65 6e28 7769 6e64 6f77 7329 2929  ),len(windows)))
+000148d0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+000148e0: 7769 6e64 6f77 735b 305d 293d 3d33 3a20  windows[0])==3: 
+000148f0: 2023 2077 6569 6768 7465 6420 6368 6932   # weighted chi2
+00014900: 0a20 2020 2020 2020 2020 2020 2077 696e  .            win
+00014910: 646f 7773 5f77 6569 6768 7473 3d6e 702e  dows_weights=np.
+00014920: 6172 7261 7928 5b77 696e 646f 7773 5b6b  array([windows[k
+00014930: 5d5b 325d 2066 6f72 206b 2069 6e20 7261  ][2] for k in ra
+00014940: 6e67 6528 6c65 6e28 7769 6e64 6f77 7329  nge(len(windows)
+00014950: 295d 290a 2020 2020 2020 2020 2020 2020  )]).            
+00014960: 7769 6e64 6f77 735f 7765 6967 6874 735f  windows_weights_
+00014970: 3264 3d6e 702e 6473 7461 636b 285b 7769  2d=np.dstack([wi
+00014980: 6e64 6f77 735f 7765 6967 6874 7320 666f  ndows_weights fo
+00014990: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+000149a0: 2861 7265 6129 295d 292e 7371 7565 657a  (area))]).squeez
+000149b0: 6528 292e 542e 7265 7368 6170 6528 286c  e().T.reshape((l
+000149c0: 656e 2861 7265 6129 2c6c 656e 2877 696e  en(area),len(win
+000149d0: 646f 7773 5f77 6569 6768 7473 2929 290a  dows_weights))).
+000149e0: 2020 2020 2020 2020 2020 2020 6368 695f              chi_
+000149f0: 6172 6561 2b3d 6e70 2e73 756d 2828 2846  area+=np.sum(((F
+00014a00: 6d6f 6465 6c5f 3264 2a61 7265 615f 3264  model_2d*area_2d
+00014a10: 2d46 6f62 7365 7276 6564 5f32 6429 2f46  -Fobserved_2d)/F
+00014a20: 6f62 7365 7276 6564 5f32 6429 2a2a 322a  observed_2d)**2*
+00014a30: 7769 6e64 6f77 735f 7765 6967 6874 735f  windows_weights_
+00014a40: 3264 2c61 7869 733d 3129 0a20 2020 2020  2d,axis=1).     
+00014a50: 2020 2020 2020 206e 6f72 6d5f 6661 6374         norm_fact
+00014a60: 6f72 2b3d 6e70 2e73 756d 2877 696e 646f  or+=np.sum(windo
+00014a70: 7773 5f77 6569 6768 7473 290a 2020 2020  ws_weights).    
+00014a80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00014a90: 2020 2020 2020 6368 695f 6172 6561 2b3d        chi_area+=
+00014aa0: 6e70 2e73 756d 2828 2846 6d6f 6465 6c5f  np.sum(((Fmodel_
+00014ab0: 3264 2a61 7265 615f 3264 2d46 6f62 7365  2d*area_2d-Fobse
+00014ac0: 7276 6564 5f32 6429 2f46 6f62 7365 7276  rved_2d)/Fobserv
+00014ad0: 6564 5f32 6429 2a2a 322c 6178 6973 3d31  ed_2d)**2,axis=1
+00014ae0: 290a 2020 2020 2020 2020 2020 2020 6e6f  ).            no
+00014af0: 726d 5f66 6163 746f 722b 3d6c 656e 2877  rm_factor+=len(w
+00014b00: 696e 646f 7773 290a 2020 2020 6966 206c  indows).    if l
+00014b10: 656e 2872 6174 696f 5f77 696e 646f 7773  en(ratio_windows
+00014b20: 293e 303a 0a20 2020 2020 2020 2052 6d6f  )>0:.        Rmo
+00014b30: 6465 6c5f 3264 3d6e 702e 6473 7461 636b  del_2d=np.dstack
+00014b40: 285b 526d 6f64 656c 2066 6f72 2069 2069  ([Rmodel for i i
+00014b50: 6e20 7261 6e67 6528 6c65 6e28 6172 6561  n range(len(area
+00014b60: 2929 5d29 2e73 7175 6565 7a65 2829 2e54  ))]).squeeze().T
+00014b70: 2e72 6573 6861 7065 2828 6c65 6e28 6172  .reshape((len(ar
+00014b80: 6561 292c 6c65 6e28 7261 7469 6f5f 7769  ea),len(ratio_wi
+00014b90: 6e64 6f77 7329 2929 0a20 2020 2020 2020  ndows))).       
+00014ba0: 2052 6f62 7365 7276 6564 5f32 643d 6e70   Robserved_2d=np
+00014bb0: 2e64 7374 6163 6b28 5b52 6f62 7365 7276  .dstack([Robserv
+00014bc0: 6564 2066 6f72 2069 2069 6e20 7261 6e67  ed for i in rang
+00014bd0: 6528 6c65 6e28 6172 6561 2929 5d29 2e73  e(len(area))]).s
+00014be0: 7175 6565 7a65 2829 2e54 2e72 6573 6861  queeze().T.resha
+00014bf0: 7065 2828 6c65 6e28 6172 6561 292c 6c65  pe((len(area),le
+00014c00: 6e28 7261 7469 6f5f 7769 6e64 6f77 7329  n(ratio_windows)
+00014c10: 2929 0a20 2020 2020 2020 2069 6620 286c  )).        if (l
+00014c20: 656e 2872 6174 696f 5f77 696e 646f 7773  en(ratio_windows
+00014c30: 5b30 5d29 3d3d 3329 3a20 2023 2077 6569  [0])==3):  # wei
+00014c40: 6768 7465 6420 6368 6932 0a20 2020 2020  ghted chi2.     
+00014c50: 2020 2020 2020 2072 6174 696f 5f77 696e         ratio_win
+00014c60: 646f 7773 5f77 6569 6768 7473 3d6e 702e  dows_weights=np.
+00014c70: 6172 7261 7928 5b72 6174 696f 5f77 696e  array([ratio_win
+00014c80: 646f 7773 5b6b 5d5b 325d 2066 6f72 206b  dows[k][2] for k
+00014c90: 2069 6e20 7261 6e67 6528 6c65 6e28 7261   in range(len(ra
+00014ca0: 7469 6f5f 7769 6e64 6f77 7329 295d 290a  tio_windows))]).
+00014cb0: 2020 2020 2020 2020 2020 2020 7261 7469              rati
+00014cc0: 6f5f 7769 6e64 6f77 735f 7765 6967 6874  o_windows_weight
+00014cd0: 735f 3264 3d6e 702e 6473 7461 636b 285b  s_2d=np.dstack([
+00014ce0: 7261 7469 6f5f 7769 6e64 6f77 735f 7765  ratio_windows_we
+00014cf0: 6967 6874 7320 666f 7220 6920 696e 2072  ights for i in r
+00014d00: 616e 6765 286c 656e 2861 7265 6129 295d  ange(len(area))]
+00014d10: 292e 7371 7565 657a 6528 292e 542e 7265  ).squeeze().T.re
+00014d20: 7368 6170 6528 286c 656e 2861 7265 6129  shape((len(area)
+00014d30: 2c6c 656e 2872 6174 696f 5f77 696e 646f  ,len(ratio_windo
+00014d40: 7773 5f77 6569 6768 7473 2929 290a 2020  ws_weights))).  
+00014d50: 2020 2020 2020 2020 2020 6368 695f 6172            chi_ar
+00014d60: 6561 2b3d 6e70 2e73 756d 2828 2852 6d6f  ea+=np.sum(((Rmo
+00014d70: 6465 6c5f 3264 2d52 6f62 7365 7276 6564  del_2d-Robserved
+00014d80: 5f32 6429 2f52 6f62 7365 7276 6564 5f32  _2d)/Robserved_2
+00014d90: 6429 2a2a 322a 7261 7469 6f5f 7769 6e64  d)**2*ratio_wind
+00014da0: 6f77 735f 7765 6967 6874 735f 3264 2c61  ows_weights_2d,a
+00014db0: 7869 733d 3129 0a20 2020 2020 2020 2020  xis=1).         
+00014dc0: 2020 206e 6f72 6d5f 6661 6374 6f72 2b3d     norm_factor+=
+00014dd0: 6e70 2e73 756d 2872 6174 696f 5f77 696e  np.sum(ratio_win
+00014de0: 646f 7773 5f77 6569 6768 7473 290a 2020  dows_weights).  
+00014df0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00014e00: 2020 2020 2020 2020 6368 695f 6172 6561          chi_area
+00014e10: 2b3d 6e70 2e73 756d 2828 2852 6d6f 6465  +=np.sum(((Rmode
+00014e20: 6c5f 3264 2d52 6f62 7365 7276 6564 5f32  l_2d-Robserved_2
+00014e30: 6429 2f52 6f62 7365 7276 6564 5f32 6429  d)/Robserved_2d)
+00014e40: 2a2a 322c 6178 6973 3d31 290a 2020 2020  **2,axis=1).    
+00014e50: 2020 2020 2020 2020 6e6f 726d 5f66 6163          norm_fac
+00014e60: 746f 722b 3d6c 656e 2872 6174 696f 5f77  tor+=len(ratio_w
+00014e70: 696e 646f 7773 290a 2020 2020 6966 206c  indows).    if l
+00014e80: 656e 2870 726f 6475 6374 5f77 696e 646f  en(product_windo
+00014e90: 7773 293e 303a 0a20 2020 2020 2020 2061  ws)>0:.        a
+00014ea0: 7265 615f 3264 3d6e 702e 6473 7461 636b  rea_2d=np.dstack
+00014eb0: 285b 6172 6561 2066 6f72 2069 2069 6e20  ([area for i in 
+00014ec0: 7261 6e67 6528 6c65 6e28 7072 6f64 7563  range(len(produc
+00014ed0: 745f 7769 6e64 6f77 7329 295d 292e 7371  t_windows))]).sq
+00014ee0: 7565 657a 6528 292e 7265 7368 6170 6528  ueeze().reshape(
+00014ef0: 286c 656e 2861 7265 6129 2c6c 656e 2870  (len(area),len(p
+00014f00: 726f 6475 6374 5f77 696e 646f 7773 2929  roduct_windows))
+00014f10: 290a 2020 2020 2020 2020 506d 6f64 656c  ).        Pmodel
+00014f20: 5f32 643d 6e70 2e64 7374 6163 6b28 5b50  _2d=np.dstack([P
+00014f30: 6d6f 6465 6c20 666f 7220 6920 696e 2072  model for i in r
+00014f40: 616e 6765 286c 656e 2861 7265 6129 295d  ange(len(area))]
+00014f50: 292e 7371 7565 657a 6528 292e 542e 7265  ).squeeze().T.re
+00014f60: 7368 6170 6528 286c 656e 2861 7265 6129  shape((len(area)
+00014f70: 2c6c 656e 2870 726f 6475 6374 5f77 696e  ,len(product_win
+00014f80: 646f 7773 2929 290a 2020 2020 2020 2020  dows))).        
+00014f90: 506f 6273 6572 7665 645f 3264 3d6e 702e  Pobserved_2d=np.
+00014fa0: 6473 7461 636b 285b 506f 6273 6572 7665  dstack([Pobserve
+00014fb0: 6420 666f 7220 6920 696e 2072 616e 6765  d for i in range
+00014fc0: 286c 656e 2861 7265 6129 295d 292e 7371  (len(area))]).sq
+00014fd0: 7565 657a 6528 292e 542e 7265 7368 6170  ueeze().T.reshap
+00014fe0: 6528 286c 656e 2861 7265 6129 2c6c 656e  e((len(area),len
+00014ff0: 2870 726f 6475 6374 5f77 696e 646f 7773  (product_windows
+00015000: 2929 290a 2020 2020 2020 2020 6966 2028  ))).        if (
+00015010: 6c65 6e28 7072 6f64 7563 745f 7769 6e64  len(product_wind
+00015020: 6f77 735b 305d 293d 3d33 293a 2020 2320  ows[0])==3):  # 
+00015030: 7765 6967 6874 6564 2063 6869 320a 2020  weighted chi2.  
+00015040: 2020 2020 2020 2020 2020 7072 6f64 7563            produc
+00015050: 745f 7769 6e64 6f77 735f 7765 6967 6874  t_windows_weight
+00015060: 733d 6e70 2e61 7272 6179 285b 7072 6f64  s=np.array([prod
+00015070: 7563 745f 7769 6e64 6f77 735b 6b5d 5b32  uct_windows[k][2
+00015080: 5d20 666f 7220 6b20 696e 2072 616e 6765  ] for k in range
+00015090: 286c 656e 2870 726f 6475 6374 5f77 696e  (len(product_win
+000150a0: 646f 7773 2929 5d29 0a20 2020 2020 2020  dows))]).       
+000150b0: 2020 2020 2070 726f 6475 6374 5f77 696e       product_win
+000150c0: 646f 7773 5f77 6569 6768 7473 5f32 643d  dows_weights_2d=
+000150d0: 6e70 2e64 7374 6163 6b28 5b70 726f 6475  np.dstack([produ
+000150e0: 6374 5f77 696e 646f 7773 5f77 6569 6768  ct_windows_weigh
+000150f0: 7473 2066 6f72 2069 2069 6e20 7261 6e67  ts for i in rang
+00015100: 6528 6c65 6e28 6172 6561 2929 5d29 2e73  e(len(area))]).s
+00015110: 7175 6565 7a65 2829 2e54 2e72 6573 6861  queeze().T.resha
+00015120: 7065 2828 6c65 6e28 6172 6561 292c 6c65  pe((len(area),le
+00015130: 6e28 7072 6f64 7563 745f 7769 6e64 6f77  n(product_window
+00015140: 735f 7765 6967 6874 7329 2929 0a20 2020  s_weights))).   
+00015150: 2020 2020 2020 2020 2063 6869 5f61 7265           chi_are
+00015160: 612b 3d6e 702e 7375 6d28 2828 2850 6d6f  a+=np.sum((((Pmo
+00015170: 6465 6c5f 3264 2a61 7265 615f 3264 2a2a  del_2d*area_2d**
+00015180: 3229 2a2a 302e 352d 2850 6f62 7365 7276  2)**0.5-(Pobserv
+00015190: 6564 5f32 6429 2a2a 302e 3529 2f28 506f  ed_2d)**0.5)/(Po
+000151a0: 6273 6572 7665 645f 3264 292a 2a30 2e35  bserved_2d)**0.5
+000151b0: 292a 2a32 2a70 726f 6475 6374 5f77 696e  )**2*product_win
+000151c0: 646f 7773 5f77 6569 6768 7473 5f32 642c  dows_weights_2d,
+000151d0: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
+000151e0: 2020 2020 6e6f 726d 5f66 6163 746f 722b      norm_factor+
+000151f0: 3d6e 702e 7375 6d28 7072 6f64 7563 745f  =np.sum(product_
+00015200: 7769 6e64 6f77 735f 7765 6967 6874 7329  windows_weights)
+00015210: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00015220: 2020 2020 2020 2020 2020 2063 6869 5f61             chi_a
+00015230: 7265 612b 3d6e 702e 7375 6d28 2828 2850  rea+=np.sum((((P
+00015240: 6d6f 6465 6c5f 3264 2a61 7265 615f 3264  model_2d*area_2d
+00015250: 2a2a 3229 2a2a 302e 352d 2850 6f62 7365  **2)**0.5-(Pobse
+00015260: 7276 6564 5f32 6429 2a2a 302e 3529 2f28  rved_2d)**0.5)/(
+00015270: 506f 6273 6572 7665 645f 3264 292a 2a30  Pobserved_2d)**0
+00015280: 2e35 292a 2a32 2c61 7869 733d 3129 0a20  .5)**2,axis=1). 
+00015290: 2020 2020 2020 2020 2020 206e 6f72 6d5f             norm_
+000152a0: 6661 6374 6f72 2b3d 6c65 6e28 7072 6f64  factor+=len(prod
+000152b0: 7563 745f 7769 6e64 6f77 7329 0a20 2020  uct_windows).   
+000152c0: 2069 6620 6e6f 726d 5f66 6163 746f 723e   if norm_factor>
+000152d0: 303a 2063 6869 5f61 7265 612f 3d6e 6f72  0: chi_area/=nor
+000152e0: 6d5f 6661 6374 6f72 0a20 2020 2072 6574  m_factor.    ret
+000152f0: 7572 6e28 6368 695f 6172 6561 290a 0a0a  urn(chi_area)...
+00015300: 6465 6620 7265 645f 6368 6932 5f73 6c61  def red_chi2_sla
+00015310: 6228 736c 6162 5f64 6174 612c 7370 6563  b(slab_data,spec
+00015320: 7472 612c 6d61 736b 2c52 6469 736b 3d6e  tra,mask,Rdisk=n
+00015330: 702e 6c6f 6773 7061 6365 282d 322c 322c  p.logspace(-2,2,
+00015340: 3130 292c 6469 7374 616e 6365 3d31 3230  10),distance=120
+00015350: 2c4e 4c54 453d 4661 6c73 652c 523d 3330  ,NLTE=False,R=30
+00015360: 3030 2c73 686f 7274 5f66 6f72 6d61 743d  00,short_format=
+00015370: 4661 6c73 652c 6f76 6572 6c61 703d 4661  False,overlap=Fa
+00015380: 6c73 652c 6e6f 6973 655f 6c65 7665 6c3d  lse,noise_level=
+00015390: 3129 3a0a 2020 2020 2727 270a 2020 2020  1):.    '''.    
+000153a0: 5265 7475 726e 7320 7265 6475 6365 6420  Returns reduced 
+000153b0: 6368 6932 2062 6173 6564 206f 6e20 7365  chi2 based on se
+000153c0: 6c65 6374 6564 2073 7065 6374 7261 6c20  lected spectral 
+000153d0: 7769 6e64 6f77 7320 6163 726f 7373 2064  windows across d
+000153e0: 6966 6665 7265 6e74 2065 6d69 7474 696e  ifferent emittin
+000153f0: 6720 6469 736b 2072 6164 6975 730a 0a20  g disk radius.. 
+00015400: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00015410: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00015420: 2073 6c61 625f 6461 7461 203a 2073 7472   slab_data : str
+00015430: 696e 6720 6f72 2073 6c61 625f 6d6f 6465  ing or slab_mode
+00015440: 6c20 696e 7374 616e 6365 0a20 2020 2020  l instance.     
+00015450: 2070 6174 6820 636f 7272 6573 706f 6e64   path correspond
+00015460: 696e 6720 746f 2061 2073 696e 676c 6520  ing to a single 
+00015470: 736c 6162 206d 6f64 656c 206f 7220 6120  slab model or a 
+00015480: 7369 6e67 6c65 2073 6c61 625f 6d6f 6465  single slab_mode
+00015490: 6c20 696e 7374 616e 6365 0a20 2020 200a  l instance.    .
+000154a0: 2020 2020 7370 6563 7472 6120 3a20 6e75      spectra : nu
+000154b0: 6d70 792e 6172 7261 790a 2020 2020 2020  mpy.array.      
+000154c0: 6e75 6d70 7920 6172 7261 7920 7769 7468  numpy array with
+000154d0: 2066 6972 7374 2063 6f6c 756d 6e20 7468   first column th
+000154e0: 6520 7761 7665 6c65 6e67 7468 2069 6e20  e wavelength in 
+000154f0: 5b6d 6963 726f 6e73 5d20 616e 6420 7365  [microns] and se
+00015500: 636f 6e64 2063 6f6c 756d 6e20 666c 7578  cond column flux
+00015510: 2069 6e20 5b4a 795d 0a20 2020 200a 2020   in [Jy].    .  
+00015520: 2020 5264 6973 6b20 3a20 666c 6f61 740a    Rdisk : float.
+00015530: 2020 2020 2020 5261 6469 7573 2063 6f72        Radius cor
+00015540: 7265 7370 6f6e 6469 6e67 2074 6f20 656d  responding to em
+00015550: 6974 7469 6e67 2061 7265 6120 696e 2061  itting area in a
+00015560: 7374 726f 6e6f 6d69 6361 6c20 756e 6974  stronomical unit
+00015570: 730a 2020 2020 0a20 2020 2064 6973 7461  s.    .    dista
+00015580: 6e63 6520 3a20 666c 6f61 740a 2020 2020  nce : float.    
+00015590: 2020 6469 7374 616e 6365 206f 6620 6469    distance of di
+000155a0: 736b 2069 6e20 7061 7273 6563 0a20 2020  sk in parsec.   
+000155b0: 200a 2020 2020 4e4c 5445 203a 2062 6f6f   .    NLTE : boo
+000155c0: 6c65 616e 0a20 2020 2020 2069 6620 5472  lean.      if Tr
+000155d0: 7565 2c20 4e4c 5445 2066 6c75 7820 6973  ue, NLTE flux is
+000155e0: 2074 616b 656e 2066 726f 6d20 7468 6520   taken from the 
+000155f0: 736c 6162 206d 6f64 656c 2069 6e20 6361  slab model in ca
+00015600: 7365 206f 6620 6f76 6572 6c61 703d 4661  se of overlap=Fa
+00015610: 6c73 652e 0a20 2020 2027 2727 0a20 2020  lse..    '''.   
+00015620: 2061 7265 613d 286e 702e 7069 2a28 5264   area=(np.pi*(Rd
+00015630: 6973 6b2a 6175 2f64 6973 7461 6e63 652f  isk*au/distance/
+00015640: 7063 292a 2a32 292e 7265 7368 6170 6528  pc)**2).reshape(
+00015650: 5264 6973 6b2e 7368 6170 655b 305d 2c31  Rdisk.shape[0],1
+00015660: 290a 0a20 2020 2069 6620 6e6f 7420 6f76  )..    if not ov
+00015670: 6572 6c61 703a 0a20 2020 2020 2020 2069  erlap:.        i
+00015680: 6620 6973 696e 7374 616e 6365 2873 6c61  f isinstance(sla
+00015690: 625f 6461 7461 2c73 7472 293a 2073 6c61  b_data,str): sla
+000156a0: 625f 6461 7461 3d72 6561 645f 736c 6162  b_data=read_slab
+000156b0: 2873 6c61 625f 6461 7461 2c76 6572 626f  (slab_data,verbo
+000156c0: 7365 3d46 616c 7365 2c73 686f 7274 5f66  se=False,short_f
+000156d0: 6f72 6d61 743d 7368 6f72 745f 666f 726d  ormat=short_form
+000156e0: 6174 290a 2020 2020 2020 2020 6c6d 696e  at).        lmin
+000156f0: 3d6e 702e 616d 696e 2873 7065 6374 7261  =np.amin(spectra
+00015700: 5b3a 2c30 5d29 0a20 2020 2020 2020 206c  [:,0]).        l
+00015710: 6d61 783d 6e70 2e61 6d61 7828 7370 6563  max=np.amax(spec
+00015720: 7472 615b 3a2c 305d 290a 2020 2020 2020  tra[:,0]).      
+00015730: 2020 736c 6162 5f64 6174 612e 636f 6e76    slab_data.conv
+00015740: 6f6c 7665 2852 3d52 2c6c 616d 6264 615f  olve(R=R,lambda_
+00015750: 303d 6c6d 696e 2a30 2e39 2c6c 616d 6264  0=lmin*0.9,lambd
+00015760: 615f 6e3d 6c6d 6178 2a31 2e31 2c4e 4c54  a_n=lmax*1.1,NLT
+00015770: 453d 4e4c 5445 2c76 6572 626f 7365 3d46  E=NLTE,verbose=F
+00015780: 616c 7365 290a 2020 2020 2020 2020 6966  alse).        if
+00015790: 204e 4c54 453a 0a20 2020 2020 2020 2020   NLTE:.         
+000157a0: 2020 206d 6f64 656c 5370 6563 3d73 7065     modelSpec=spe
+000157b0: 6374 7265 732e 7370 6563 7472 6573 2873  ctres.spectres(s
+000157c0: 7065 6374 7261 5b3a 2c30 5d2c 736c 6162  pectra[:,0],slab
+000157d0: 5f64 6174 612e 636f 6e76 5761 7665 6c65  _data.convWavele
+000157e0: 6e67 7468 2c73 6c61 625f 6461 7461 2e63  ngth,slab_data.c
+000157f0: 6f6e 764e 4c54 4566 6c75 782a 3165 3233  onvNLTEflux*1e23
+00015800: 2c76 6572 626f 7365 3d46 616c 7365 2c66  ,verbose=False,f
+00015810: 696c 6c3d 302e 3029 0a20 2020 2020 2020  ill=0.0).       
+00015820: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00015830: 2020 206d 6f64 656c 5370 6563 3d73 7065     modelSpec=spe
+00015840: 6374 7265 732e 7370 6563 7472 6573 2873  ctres.spectres(s
+00015850: 7065 6374 7261 5b3a 2c30 5d2c 736c 6162  pectra[:,0],slab
+00015860: 5f64 6174 612e 636f 6e76 5761 7665 6c65  _data.convWavele
+00015870: 6e67 7468 2c73 6c61 625f 6461 7461 2e63  ngth,slab_data.c
+00015880: 6f6e 764c 5445 666c 7578 2a31 6532 332c  onvLTEflux*1e23,
+00015890: 7665 7262 6f73 653d 4661 6c73 652c 6669  verbose=False,fi
+000158a0: 6c6c 3d30 2e30 290a 2020 2020 656c 7365  ll=0.0).    else
+000158b0: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
+000158c0: 6e73 7461 6e63 6528 736c 6162 5f64 6174  nstance(slab_dat
+000158d0: 612c 7374 7229 3a20 736c 6162 5f64 6174  a,str): slab_dat
+000158e0: 613d 7265 6164 5f6f 7665 726c 6170 5f73  a=read_overlap_s
+000158f0: 7065 6374 7261 2873 6c61 625f 6461 7461  pectra(slab_data
+00015900: 2c76 6572 626f 7365 3d46 616c 7365 290a  ,verbose=False).
+00015910: 2020 2020 2020 2020 6c6d 696e 3d6e 702e          lmin=np.
+00015920: 616d 696e 2873 7065 6374 7261 5b3a 2c30  amin(spectra[:,0
+00015930: 5d29 0a20 2020 2020 2020 206c 6d61 783d  ]).        lmax=
+00015940: 6e70 2e61 6d61 7828 7370 6563 7472 615b  np.amax(spectra[
+00015950: 3a2c 305d 290a 2020 2020 2020 2020 736c  :,0]).        sl
+00015960: 6162 5f64 6174 612e 636f 6e76 6f6c 7665  ab_data.convolve
+00015970: 5f6f 7665 726c 6170 2852 3d52 2c6c 616d  _overlap(R=R,lam
+00015980: 6264 615f 303d 6c6d 696e 2a30 2e39 2c6c  bda_0=lmin*0.9,l
+00015990: 616d 6264 615f 6e3d 6c6d 6178 2a31 2e31  ambda_n=lmax*1.1
+000159a0: 2c76 6572 626f 7365 3d46 616c 7365 290a  ,verbose=False).
+000159b0: 2020 2020 2020 2020 6d6f 6465 6c53 7065          modelSpe
+000159c0: 633d 7370 6563 7472 6573 2e73 7065 6374  c=spectres.spect
+000159d0: 7265 7328 7370 6563 7472 615b 3a2c 305d  res(spectra[:,0]
+000159e0: 2c63 2f73 6c61 625f 6461 7461 2e63 6f6e  ,c/slab_data.con
+000159f0: 764f 7665 726c 6170 4672 6571 5b3a 3a2d  vOverlapFreq[::-
+00015a00: 315d 2a31 652d 332c 736c 6162 5f64 6174  1]*1e-3,slab_dat
+00015a10: 612e 636f 6e76 4f76 6572 6c61 704c 5445  a.convOverlapLTE
+00015a20: 5b3a 3a2d 315d 2a31 6532 332c 7665 7262  [::-1]*1e23,verb
+00015a30: 6f73 653d 4661 6c73 652c 6669 6c6c 3d30  ose=False,fill=0
+00015a40: 2e30 290a 2020 2020 7370 6563 7472 615f  .0).    spectra_
+00015a50: 3264 3d73 7065 6374 7261 5b6d 6173 6b2c  2d=spectra[mask,
+00015a60: 315d 2e72 6573 6861 7065 2831 2c73 7065  1].reshape(1,spe
+00015a70: 6374 7261 5b6d 6173 6b2c 2d31 5d2e 7368  ctra[mask,-1].sh
+00015a80: 6170 655b 305d 292a 6e70 2e6f 6e65 735f  ape[0])*np.ones_
+00015a90: 6c69 6b65 2861 7265 6129 0a20 2020 206d  like(area).    m
+00015aa0: 6f64 656c 5370 6563 5f32 643d 6d6f 6465  odelSpec_2d=mode
+00015ab0: 6c53 7065 635b 6d61 736b 5d2e 7265 7368  lSpec[mask].resh
+00015ac0: 6170 6528 312c 6d6f 6465 6c53 7065 635b  ape(1,modelSpec[
+00015ad0: 6d61 736b 5d2e 7368 6170 655b 305d 292a  mask].shape[0])*
+00015ae0: 6e70 2e6f 6e65 735f 6c69 6b65 2861 7265  np.ones_like(are
+00015af0: 6129 0a20 2020 2061 7265 615f 3264 3d61  a).    area_2d=a
+00015b00: 7265 612e 7265 7368 6170 6528 6172 6561  rea.reshape(area
+00015b10: 2e73 6861 7065 5b30 5d2c 3129 0a20 2020  .shape[0],1).   
+00015b20: 2063 6869 5f61 7265 613d 6e70 2e73 756d   chi_area=np.sum
+00015b30: 2828 7370 6563 7472 615f 3264 2d6d 6f64  ((spectra_2d-mod
+00015b40: 656c 5370 6563 5f32 642a 6172 6561 5f32  elSpec_2d*area_2
+00015b50: 6429 2a2a 322c 6178 6973 3d31 292f 6c65  d)**2,axis=1)/le
+00015b60: 6e28 7370 6563 7472 615b 6d61 736b 2c30  n(spectra[mask,0
+00015b70: 5d29 2f6e 6f69 7365 5f6c 6576 656c 2a2a  ])/noise_level**
+00015b80: 320a 0a20 2020 2072 6574 7572 6e28 6368  2..    return(ch
+00015b90: 695f 6172 6561 290a                      i_area).
```

### Comparing `prodimopy-2.1.5/prodimopy/script_compare.py` & `prodimopy-2.1.6/prodimopy/script_compare.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/script_params.py` & `prodimopy-2.1.6/prodimopy/script_params.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/script_plot.py` & `prodimopy-2.1.6/prodimopy/script_plot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,160 +1,155 @@
 """
-Default script for the plotting the results of a single ProDiMo model. 
+Default script for the plotting the results of a single ProDiMo model.
 
-A script called `pplot`, which can directly by called from the command line, 
-will be installed automatically during the installation process.  
+A script called `pplot`, which can directly by called from the command line,
+will be installed automatically during the installation process.
 """
-from __future__ import print_function
 from __future__ import division
+from __future__ import print_function
 from __future__ import unicode_literals
 
-# the above two statement are for phyton2 pyhton3 compatibility.
-# With this statmens you can write python3 code and it should also work
-# in python2 (depends on your code) 
-
-# this is for the argument parser included in python
 import argparse
 
-# this is for the PDF output
 from matplotlib.backends.backend_pdf import PdfPages
+import numpy as np
 
-# Thats the prodimpy modules 
-# The first one is for reading a ProDiMo Model 
-# The second one is for plotting
-import prodimopy.read as pread
 import prodimopy.plot as pplot
+import prodimopy.read as pread
 import prodimopy.utils as putils
-import numpy
 
-# The main routine is require to have an entry point. 
+
+# the above two statement are for phyton2 pyhton3 compatibility.
+# With this statmens you can write python3 code and it should also work
+# in python2 (depends on your code)
+# this is for the argument parser included in python
+# this is for the PDF output
+# Thats the prodimpy modules
+# The first one is for reading a ProDiMo Model
+# The second one is for plotting
+# The main routine is require to have an entry point.
 # It is not necessary if you want to write your own script.
 def main(args=None):
   ###############################################################################
   # Command line parsing
-  # this is optional you do not have to do it this way. 
+  # this is optional you do not have to do it this way.
   # You can use the prodimopy module in any way you want
-  parser = argparse.ArgumentParser(description='prodimopy simple example for plotting ')
-  parser.add_argument('-dir', required=False, default=".", help='The directory of the input files DEFAULT: "."')
-  parser.add_argument('-output', required=False, default="./out.pdf", help='The output filename, DEFAULT: "./out.pdf"')
-  parser.add_argument('-td_fileIdx', required=False, default=None, help='The index for the time dependent output file e.g. "01", DEFAULT: None')
-  parser.add_argument('-mplstyle', required=False, default="prodimopy", help='Use a mpl style file, DEFAULT: prodimopy')
-  args = parser.parse_args()
-  
-  print("-dir: ", args.dir)
-  print("-output: ", args.output)
-  print("-td_fileIdx: ", args.td_fileIdx)
-  
+  parser=argparse.ArgumentParser(description='prodimopy simple example for plotting ')
+  parser.add_argument('-dir',required=False,default=".",help='The directory of the input files DEFAULT: "."')
+  parser.add_argument('-output',required=False,default="./out.pdf",help='The output filename, DEFAULT: "./out.pdf"')
+  parser.add_argument('-td_fileIdx',required=False,default=None,help='The index for the time dependent output file e.g. "01", DEFAULT: None')
+  parser.add_argument('-mplstyle',required=False,default="prodimopy",help='Use a mpl style file, DEFAULT: prodimopy')
+  args=parser.parse_args()
+
+  print("-dir: ",args.dir)
+  print("-output: ",args.output)
+  print("-td_fileIdx: ",args.td_fileIdx)
+
   # thats for time dependent models, also optional
   outfile=args.output
-  if args.td_fileIdx != None:
+  if args.td_fileIdx!=None:
     outfile=outfile.replace(".pdf","_"+args.td_fileIdx+".pdf")
-  
+
   # This reads the output of a ProDiMo model
-  # there are more optional arguments 
-  model = pread.read_prodimo(args.dir,td_fileIdx=args.td_fileIdx)
-  
+  # there are more optional arguments
+  model=pread.read_prodimo(args.dir,td_fileIdx=args.td_fileIdx)
+
   # loads the prodimopy style
   putils.load_mplstyle(args.mplstyle)
-  
+
   # Here the plotting happens. This produces one pdf file
   with PdfPages(outfile) as pdf:
     # Init the prodimo plotting module for one model and an optional title
-    # it is required to pass a PdfPages object  
+    # it is required to pass a PdfPages object
     pp=pplot.Plot(pdf,title=model.name)
-    
+
     zr=True
     xlog=True
     ylog=False
 
     pp.plot_grid(model)
-    # This plots the Stellar spectrum  
-    pp.plot_starspec(model)  
+    # This plots the Stellar spectrum
+    pp.plot_starspec(model)
     pp.plot_dust_opac(model)
-    
-    
-    #pp.plot_NH(model,sdscale=True,ylim=[5.e27,5.e29])
-    pp.plot_NH(model,sdscale=True,ylim=[1.e20,None],xlog=True)
 
+    # pp.plot_NH(model,sdscale=True,ylim=[5.e27,5.e29])
+    pp.plot_NH(model,sdscale=True,ylim=[1.e20,None],xlog=True)
 
-    # here the default contour plots are used not very fancy currently. 
+    # here the default contour plots are used not very fancy currently.
     # you can use latex for the labels!
     # note most of the parameters are optional
 
     contAV=pplot.Contour(model.AV,[1.0],showlabels=True,label_fmt=r" $A_V$=%.0f ",colors=pp.pcolors["red"])
-    pp.plot_cont(model, model.nHtot, r"$\mathrm{n_{<H>} [cm^{-3}]}$",oconts=[contAV],zlim=[1.e4,None],extend="min",
-                 zr=zr,xlog=xlog,ylog=ylog)  
-    
-    pp.plot_cont(model, model.rhod, r"$\mathsf{\rho_{dust} [g\;cm^{-3}]}$",
+    pp.plot_cont(model,model.nHtot,r"$\mathrm{n_{<H>} [cm^{-3}]}$",oconts=[contAV],zlim=[1.e4,None],extend="min",
+                 zr=zr,xlog=xlog,ylog=ylog)
+
+    pp.plot_cont(model,model.rhod,r"$\mathsf{\rho_{dust} [g\;cm^{-3}]}$",
                 zlim=[1.e-25,None],extend="both",
                 zr=zr,xlog=xlog,ylog=ylog)
 
-
-
     levels=[10,20,50,100,300,1000]
-    pp.plot_cont(model, model.td, r"$\mathrm{T_{dust} [K]}$",
+    pp.plot_cont(model,model.td,r"$\mathrm{T_{dust} [K]}$",
                    zlim=[10,3500],extend="both",clevels=levels,clabels=map(str,levels),
                    zr=zr,xlog=xlog,ylog=ylog)
 
-    levels=[10,20,50,100,300,1000,3000]   
-    pp.plot_cont(model, model.tg, r"$\mathrm{T_{gas} [K]}$",
+    levels=[10,20,50,100,300,1000,3000]
+    pp.plot_cont(model,model.tg,r"$\mathrm{T_{gas} [K]}$",
                    zlim=[10,3500],extend="both",clevels=levels,clabels=map(str,levels),
                    zr=zr,xlog=xlog,ylog=ylog)
 
-    pp.plot_cont(model, model.chiRT, r"log $\mathrm{\chi\,[Draine\,field]}$",contour=True,
+    pp.plot_cont(model,model.chiRT,r"log $\mathrm{\chi\,[Draine\,field]}$",contour=True,
                     zlim=[1.e-6,1.e6],extend="both",cb_format="%.0f",
                     zr=zr,xlog=xlog,ylog=ylog)
 
-    if numpy.max(model.zetaX)>1.e-99:
-      pp.plot_cont(model, model.zetaX, r"$\mathrm{\zeta_{X}\,per\,H\,[s^{-1}]}$",contour=True,
+    if np.max(model.zetaX)>1.e-99:
+      pp.plot_cont(model,model.zetaX,r"$\mathrm{\zeta_{X}\,per\,H\,[s^{-1}]}$",contour=True,
                    zlim=[1.e-19,1.e-13],extend="both",
                    zr=zr,xlog=xlog,ylog=ylog)
 
-
     pp.plot_heat_cool(model)
     pp.plot_cont(model,model.taucool,r"log $\tau_\mathrm{cool}\,[yr]$",zlim=[1.e-2,None],extend="min",
                  zr=zr,xlog=xlog,ylog=ylog)
-    
-    
-    
+
     pp.plot_cont(model,model.tauchem,r"log $\tau_\mathrm{chem}\,[yr]$",zlim=[1.e-2,1.e7],extend="both",
                  zr=zr,xlog=xlog,ylog=ylog)
-    
+
     for spname in model.spnames:
-      maxabun=numpy.max(model.getAbun(spname))
+      maxabun=np.max(model.getAbun(spname))
       zlim=[maxabun/1.e6,maxabun]
-      pp.plot_abuncont(model, spname,zlim=zlim ,extend="both",rasterized=True,
+      pp.plot_abuncont(model,spname,zlim=zlim ,extend="both",rasterized=True,
                        zr=True,xlog=True,ylog=False,nbins=40)
 
     # observables if available
-    if model.sed is not None: 
+    if model.sed is not None:
       pp.plot_sed(model,sedObs=model.sedObs)
       # model.rhod, r"$\mathsf{\rho_{dust} [g\;cm^{-3}]}$
       pp.plot_sedAna(model,zr=True,xlog=True,ylog=False)
-    
-    # line fluxes stuff 
-    if model.lines is not None:  
-      lineidents=[[line.ident,line.wl] for line in model.lines]            
+
+    # line fluxes stuff
+    if model.lines is not None:
+      lineidents=[[line.ident,line.wl] for line in model.lines]
       pp.plot_lines(model,lineidents,showBoxes=False,lineObs=model.lineObs,useLineEstimate=False)
-      
+
       for line in model.lines:
-        pp.plot_lineprofile(model,line.wl, line.ident,lineObs=model.lineObs)
+        pp.plot_lineprofile(model,line.wl,line.ident,lineObs=model.lineObs)
 
       for line in model.lines:
+        ident=line.ident
+        # this is likely not complete
+        if ident=="OI": ident="O"
+        if ident=="CII": ident="C+"
+
         if line.species in model.spnames:
-          nspmol=model.nmol[:,:,model.spnames[line.species]] 
+          nspmol=model.nmol[:,:,model.spnames[line.species]]
           label=line.species
         else:
           nspmol=model.nmol[:,:,model.spnames["H2"]]
           label="H2"
-        max=numpy.max(nspmol)
-        zlim=[max/1.e11,max/1000] 
-        pp.plot_line_origin(model,[[line.ident,line.wl]],nspmol,
-                        label=r"log $n_{"+pplot.spnToLatex(label)+"}\,[cm^{-3}]$",
+        max=np.max(nspmol)
+        zlim=[max/1.e11,max/1000]
+        pp.plot_line_origin(model,[[ident,line.wl]],nspmol,
+                        label=r"log $n_{"+pplot.spnToLatex(label)+r"}\,[cm^{-3}]$",
                         zlim=zlim,extend="both",showContOrigin=True)
 
-
-       
     # Plot radiation field at certain wavelengths (here simply done with the index)
     # pp.plot_cont(model,model.radFields[:,:,0],zr=False,xlog=False,label="lam="+str(model.lams[0]))
-    # pp.plot_cont(model,model.radFields[:,:,5],zr=False,xlog=False,label="lam="+str(model.lams[5]))     
-  
+    # pp.plot_cont(model,model.radFields[:,:,5],zr=False,xlog=False,label="lam="+str(model.lams[5]))
```

### Comparing `prodimopy-2.1.5/prodimopy/script_plot_models.py` & `prodimopy-2.1.6/prodimopy/script_plot_models.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/utils.py` & `prodimopy-2.1.6/prodimopy/utils.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy/utils_casasim.py` & `prodimopy-2.1.6/prodimopy/utils_casasim.py`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/prodimopy.egg-info/PKG-INFO` & `prodimopy-2.1.6/prodimopy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodimopy
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python tools for ProDiMo.
 Home-page: https://gitlab.astro.rug.nl/prodimo/prodimopy/
 Author: Christian Rab
 Author-email: rab@astro.rug.nl
 License: MIT License
 Keywords: astronomy astrophysics star-formation protoplanetary-disks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `prodimopy-2.1.5/prodimopy.egg-info/SOURCES.txt` & `prodimopy-2.1.6/prodimopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prodimopy-2.1.5/setup.py` & `prodimopy-2.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 setup(
     name='prodimopy',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.1.5',
+    version='2.1.6',
 
     description='Python tools for ProDiMo.',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://gitlab.astro.rug.nl/prodimo/prodimopy/',
@@ -106,21 +106,21 @@
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     # FIXME: include proper version numbers
     # for astropy often dev versoin are automatically install avoid that.
     install_requires=[
-                      'astropy>4.0,<5.2',
+                      'astropy>4',
                       'matplotlib>3',
                       'numpy>=1.17',  # no special requirements, but astropy has some
                       'scipy>1',
                       'pandas>1.4',  # the last three are only for slab models.
-                      'adjustText<=0.8',  # just to avoid the beta version, need to switch to pip install also for local stuff
-                      'spectres<=2.2.0'
+                      'adjustText>=0.8',  # just to avoid the beta version, need to switch to pip install also for local stuff
+                      'spectres>=2.2.0'
                       ],
     cmdclass={'install': new_install},
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
```


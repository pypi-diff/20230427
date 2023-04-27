# Comparing `tmp/solarmach-0.1.6.tar.gz` & `tmp/solarmach-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarmach-0.1.6.tar", last modified: Mon Mar 27 11:54:33 2023, max compression
+gzip compressed data, was "solarmach-0.1.7.tar", last modified: Thu Apr 27 13:55:43 2023, max compression
```

## Comparing `solarmach-0.1.6.tar` & `solarmach-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-03-27 11:54:33.438382 solarmach-0.1.6/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.1.6/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.1.6/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6001 2023-03-27 11:54:33.438382 solarmach-0.1.6/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     5152 2023-03-07 14:33:01.000000 solarmach-0.1.6/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.1.6/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-03-27 11:54:33.426382 solarmach-0.1.6/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solarmach-0.1.6/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2300 2022-03-14 11:55:52.000000 solarmach-0.1.6/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      300 2022-03-14 11:56:45.000000 solarmach-0.1.6/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solarmach-0.1.6/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-03-27 11:54:33.434382 solarmach-0.1.6/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   476228 2022-09-26 07:56:42.000000 solarmach-0.1.6/examples/example.ipynb
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.1.6/examples/solarmach.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-03-27 11:54:33.434382 solarmach-0.1.6/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.1.6/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.1.6/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-01-10 16:26:49.000000 solarmach-0.1.6/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       61 2022-07-06 11:55:56.000000 solarmach-0.1.6/requirements.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2077 2023-03-27 11:54:33.442382 solarmach-0.1.6/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.1.6/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-03-27 11:54:33.438382 solarmach-0.1.6/solarmach/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    30635 2023-03-27 09:38:54.000000 solarmach-0.1.6/solarmach/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-03-27 11:54:33.438382 solarmach-0.1.6/solarmach/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.1.6/solarmach/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1695 2022-11-09 14:33:28.000000 solarmach-0.1.6/solarmach/tests/test.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-03-27 11:54:33.000000 solarmach-0.1.6/solarmach/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-03-27 11:54:33.438382 solarmach-0.1.6/solarmach.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6001 2023-03-27 11:54:33.000000 solarmach-0.1.6/solarmach.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      556 2023-03-27 11:54:33.000000 solarmach-0.1.6/solarmach.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-03-27 11:54:33.000000 solarmach-0.1.6/solarmach.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.1.6/solarmach.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      147 2023-03-27 11:54:33.000000 solarmach-0.1.6/solarmach.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       10 2023-03-27 11:54:33.000000 solarmach-0.1.6/solarmach.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1292 2022-03-14 12:48:29.000000 solarmach-0.1.6/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.048822 solarmach-0.1.7/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.1.7/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.1.7/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-04-27 13:55:43.048822 solarmach-0.1.7/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     5268 2023-04-27 13:45:25.000000 solarmach-0.1.7/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.1.7/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.040822 solarmach-0.1.7/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solarmach-0.1.7/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2300 2022-03-14 11:55:52.000000 solarmach-0.1.7/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      300 2022-03-14 11:56:45.000000 solarmach-0.1.7/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solarmach-0.1.7/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.044823 solarmach-0.1.7/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)  1915936 2023-04-27 13:41:04.000000 solarmach-0.1.7/examples/example.ipynb
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.1.7/examples/solarmach.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.044823 solarmach-0.1.7/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.1.7/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.1.7/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-01-10 16:26:49.000000 solarmach-0.1.7/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       61 2022-07-06 11:55:56.000000 solarmach-0.1.7/requirements.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2077 2023-04-27 13:55:43.048822 solarmach-0.1.7/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.1.7/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.044823 solarmach-0.1.7/solarmach/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    30813 2023-04-27 13:35:33.000000 solarmach-0.1.7/solarmach/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.044823 solarmach-0.1.7/solarmach/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.1.7/solarmach/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1695 2022-11-09 14:33:28.000000 solarmach-0.1.7/solarmach/tests/test.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-04-27 13:55:42.000000 solarmach-0.1.7/solarmach/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.044823 solarmach-0.1.7/solarmach.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-04-27 13:55:42.000000 solarmach-0.1.7/solarmach.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      556 2023-04-27 13:55:43.000000 solarmach-0.1.7/solarmach.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-04-27 13:55:42.000000 solarmach-0.1.7/solarmach.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.1.7/solarmach.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      147 2023-04-27 13:55:42.000000 solarmach-0.1.7/solarmach.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       10 2023-04-27 13:55:42.000000 solarmach-0.1.7/solarmach.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1292 2022-03-14 12:48:29.000000 solarmach-0.1.7/tox.ini
```

### Comparing `solarmach-0.1.6/LICENSE.rst` & `solarmach-0.1.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/PKG-INFO` & `solarmach-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.1.6
+Version: 0.1.7
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -86,16 +86,14 @@
    transparent = False                              # make output figure background transparent
    numbered_markers = True                          # plot each body with a numbered marker
    filename = 'Solar-MACH_'+date.replace(' ', '_')  # define filename of output figure
 
    # initialize
    sm = SolarMACH(date, body_list, vsw_list, reference_long, reference_lat, coord_sys)
 
-
-
    # make plot
    sm.plot(
       plot_spirals=plot_spirals,
       plot_sun_body_line=plot_sun_body_line,
       reference_vsw=reference_vsw,
       transparent=transparent,
       numbered_markers=numbered_markers,
@@ -106,14 +104,16 @@
    
    # obtain data as Pandas DataFrame
    display(sm.coord_table)
 
 .. image:: https://github.com/jgieseler/solarmach/raw/main/examples/solarmach.png
   :alt: Example output figure
   
+See `example notebook <https://github.com/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ for all options!
+  
 Example Notebook
 ----------------
 
 **solarmach** can easily be run in a Jupyter Notebook. 
 
 - `Download example notebook <https://github.com/jgieseler/solarmach/raw/main/examples/example.ipynb>`_
```

### Comparing `solarmach-0.1.6/README.rst` & `solarmach-0.1.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -62,16 +62,14 @@
    transparent = False                              # make output figure background transparent
    numbered_markers = True                          # plot each body with a numbered marker
    filename = 'Solar-MACH_'+date.replace(' ', '_')  # define filename of output figure
 
    # initialize
    sm = SolarMACH(date, body_list, vsw_list, reference_long, reference_lat, coord_sys)
 
-
-
    # make plot
    sm.plot(
       plot_spirals=plot_spirals,
       plot_sun_body_line=plot_sun_body_line,
       reference_vsw=reference_vsw,
       transparent=transparent,
       numbered_markers=numbered_markers,
@@ -82,14 +80,16 @@
    
    # obtain data as Pandas DataFrame
    display(sm.coord_table)
 
 .. image:: https://github.com/jgieseler/solarmach/raw/main/examples/solarmach.png
   :alt: Example output figure
   
+See `example notebook <https://github.com/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ for all options!
+  
 Example Notebook
 ----------------
 
 **solarmach** can easily be run in a Jupyter Notebook. 
 
 - `Download example notebook <https://github.com/jgieseler/solarmach/raw/main/examples/example.ipynb>`_
```

### Comparing `solarmach-0.1.6/code_of_conduct.md` & `solarmach-0.1.7/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/docs/Makefile` & `solarmach-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/docs/conf.py` & `solarmach-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/docs/make.bat` & `solarmach-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/examples/solarmach.png` & `solarmach-0.1.7/examples/solarmach.png`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/licenses/LICENSE.rst` & `solarmach-0.1.7/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/licenses/TEMPLATE_LICENSE.rst` & `solarmach-0.1.7/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/setup.cfg` & `solarmach-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/setup.py` & `solarmach-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/solarmach/__init__.py` & `solarmach-0.1.7/solarmach/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,24 +35,26 @@
 body_dict = dict.fromkeys(['Mercury', 199], [199, 'Mercury', 'darkturquoise'])
 body_dict.update(dict.fromkeys(['Venus', 299], [299, 'Venus', 'darkorchid']))
 body_dict.update(dict.fromkeys(['Earth', 'EARTH', 'earth', 399], [399, 'Earth', 'green']))
 body_dict.update(dict.fromkeys(['Mars', 499], [499, 'Mars', 'maroon']))
 body_dict.update(dict.fromkeys(['Jupiter', 599], [599, 'Jupiter', 'navy']))
 
 body_dict.update(dict.fromkeys(['L1', 31], [31, 'SEMB-L1', 'black']))
+body_dict.update(dict.fromkeys(['ACE', 'Advanced Composition Explorer', -92], [-92, 'ACE', 'dimgrey']))
 
 body_dict.update(dict.fromkeys(['STEREO B', 'STEREO-B', 'STB', 'stb', -235], [-235, 'STEREO B', 'b']))
 body_dict.update(dict.fromkeys(['STEREO A', 'STEREO-A', 'STA', 'sta', -234], [-234, 'STEREO A', 'red']))
 body_dict.update(dict.fromkeys(['SOHO', 'soho', -21], [-21, 'SOHO', 'darkgreen']))
 body_dict.update(dict.fromkeys(['Solar Orbiter', 'SolO', 'solarorbiter', 'SolarOrbiter', -144], [-144, 'Solar Orbiter', 'dodgerblue']))
 body_dict.update(dict.fromkeys(['PSP', 'Parker Solar Probe', 'parkersolarprobe', 'ParkerSolarProbe', -96], [-96, 'Parker Solar Probe', 'purple']))
 body_dict.update(dict.fromkeys(['BepiColombo', 'Bepi Colombo', 'Bepi', 'MPO', -121], [-121, 'BepiColombo', 'orange']))
 body_dict.update(dict.fromkeys(['MAVEN', -202], [-202, 'MAVEN', 'brown']))
 body_dict.update(dict.fromkeys(['Mars Express', -41], [-41, 'Mars Express', 'darkorange']))
 body_dict.update(dict.fromkeys(['MESSENGER', -236], [-236, 'MESSENGER', 'olivedrab']))
+body_dict.update(dict.fromkeys(['JUICE', -28], [-28, 'JUICE', 'violet']))
 body_dict.update(dict.fromkeys(['Juno', -61], [-61, 'Juno', 'orangered']))
 body_dict.update(dict.fromkeys(['Cassini', -82], [-82, 'Cassini', 'mediumvioletred']))
 body_dict.update(dict.fromkeys(['Rosetta', -226], [-226, 'Rosetta', 'blueviolet']))
 body_dict.update(dict.fromkeys(['Pioneer10', -23], [-23, 'Pioneer 10', 'teal']))
 body_dict.update(dict.fromkeys(['Pioneer11', -24], [-24, 'Pioneer 11', 'darkblue']))
 body_dict.update(dict.fromkeys(['Ulysses', -55], [-55, 'Ulysses', 'dimgray']))
 body_dict.update(dict.fromkeys(['Voyager1', -31], [-31, 'Voyager 1', 'darkred']))
```

### Comparing `solarmach-0.1.6/solarmach/tests/test.py` & `solarmach-0.1.7/solarmach/tests/test.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/solarmach.egg-info/PKG-INFO` & `solarmach-0.1.7/solarmach.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.1.6
+Version: 0.1.7
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -86,16 +86,14 @@
    transparent = False                              # make output figure background transparent
    numbered_markers = True                          # plot each body with a numbered marker
    filename = 'Solar-MACH_'+date.replace(' ', '_')  # define filename of output figure
 
    # initialize
    sm = SolarMACH(date, body_list, vsw_list, reference_long, reference_lat, coord_sys)
 
-
-
    # make plot
    sm.plot(
       plot_spirals=plot_spirals,
       plot_sun_body_line=plot_sun_body_line,
       reference_vsw=reference_vsw,
       transparent=transparent,
       numbered_markers=numbered_markers,
@@ -106,14 +104,16 @@
    
    # obtain data as Pandas DataFrame
    display(sm.coord_table)
 
 .. image:: https://github.com/jgieseler/solarmach/raw/main/examples/solarmach.png
   :alt: Example output figure
   
+See `example notebook <https://github.com/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ for all options!
+  
 Example Notebook
 ----------------
 
 **solarmach** can easily be run in a Jupyter Notebook. 
 
 - `Download example notebook <https://github.com/jgieseler/solarmach/raw/main/examples/example.ipynb>`_
```

### Comparing `solarmach-0.1.6/solarmach.egg-info/SOURCES.txt` & `solarmach-0.1.7/solarmach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.6/tox.ini` & `solarmach-0.1.7/tox.ini`

 * *Files identical despite different names*


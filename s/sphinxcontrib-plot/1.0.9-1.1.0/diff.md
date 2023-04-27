# Comparing `tmp/sphinxcontrib-plot-1.0.9.tar.gz` & `tmp/sphinxcontrib-plot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-plot-1.0.9.tar", last modified: Mon Sep  6 06:50:45 2021, max compression
+gzip compressed data, was "sphinxcontrib-plot-1.1.0.tar", last modified: Thu Apr 27 07:30:13 2023, max compression
```

## Comparing `sphinxcontrib-plot-1.0.9.tar` & `sphinxcontrib-plot-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Sangfor  (197608) None     (197121)        0 2021-09-06 06:50:45.963867 sphinxcontrib-plot-1.0.9/
--rw-r--r--   0 Sangfor  (197608) None     (197121)     1418 2021-09-03 01:08:52.000000 sphinxcontrib-plot-1.0.9/LICENSE
--rw-r--r--   0 Sangfor  (197608) None     (197121)       51 2021-09-03 01:08:52.000000 sphinxcontrib-plot-1.0.9/MANIFEST.in
--rw-r--r--   0 Sangfor  (197608) None     (197121)    12397 2021-09-06 06:50:45.963867 sphinxcontrib-plot-1.0.9/PKG-INFO
--rw-r--r--   0 Sangfor  (197608) None     (197121)     9671 2021-09-04 06:59:07.000000 sphinxcontrib-plot-1.0.9/README.rst
--rw-r--r--   0 Sangfor  (197608) None     (197121)       76 2021-09-06 06:50:45.965820 sphinxcontrib-plot-1.0.9/setup.cfg
--rw-r--r--   0 Sangfor  (197608) None     (197121)      625 2021-09-06 06:31:34.000000 sphinxcontrib-plot-1.0.9/setup.py
-drwxr-xr-x   0 Sangfor  (197608) None     (197121)        0 2021-09-06 06:50:45.945312 sphinxcontrib-plot-1.0.9/sphinxcontrib/
--rw-r--r--   0 Sangfor  (197608) None     (197121)      269 2021-09-03 01:08:52.000000 sphinxcontrib-plot-1.0.9/sphinxcontrib/__init__.py
--rw-r--r--   0 Sangfor  (197608) None     (197121)    12798 2021-09-06 06:16:47.000000 sphinxcontrib-plot-1.0.9/sphinxcontrib/plot.py
-drwxr-xr-x   0 Sangfor  (197608) None     (197121)        0 2021-09-06 06:50:45.961914 sphinxcontrib-plot-1.0.9/sphinxcontrib_plot.egg-info/
--rw-r--r--   0 Sangfor  (197608) None     (197121)    12397 2021-09-06 06:50:45.000000 sphinxcontrib-plot-1.0.9/sphinxcontrib_plot.egg-info/PKG-INFO
--rw-r--r--   0 Sangfor  (197608) None     (197121)      357 2021-09-06 06:50:45.000000 sphinxcontrib-plot-1.0.9/sphinxcontrib_plot.egg-info/SOURCES.txt
--rw-r--r--   0 Sangfor  (197608) None     (197121)        1 2021-09-06 06:50:45.000000 sphinxcontrib-plot-1.0.9/sphinxcontrib_plot.egg-info/dependency_links.txt
--rw-r--r--   0 Sangfor  (197608) None     (197121)       14 2021-09-06 06:50:45.000000 sphinxcontrib-plot-1.0.9/sphinxcontrib_plot.egg-info/namespace_packages.txt
--rw-r--r--   0 Sangfor  (197608) None     (197121)       12 2021-09-06 06:50:45.000000 sphinxcontrib-plot-1.0.9/sphinxcontrib_plot.egg-info/requires.txt
--rw-r--r--   0 Sangfor  (197608) None     (197121)       14 2021-09-06 06:50:45.000000 sphinxcontrib-plot-1.0.9/sphinxcontrib_plot.egg-info/top_level.txt
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-04-27 07:30:13.898770 sphinxcontrib-plot-1.1.0/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)     1418 2021-07-29 23:39:29.000000 sphinxcontrib-plot-1.1.0/LICENSE
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       51 2021-07-29 23:39:29.000000 sphinxcontrib-plot-1.1.0/MANIFEST.in
+-rw-rw-r--   0 ypguo    (19391612) Domain Users (1049089)    10498 2023-04-27 07:30:13.899777 sphinxcontrib-plot-1.1.0/PKG-INFO
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    10171 2023-04-27 07:18:45.000000 sphinxcontrib-plot-1.1.0/README.rst
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       76 2023-04-27 07:30:13.900776 sphinxcontrib-plot-1.1.0/setup.cfg
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      625 2023-04-27 07:18:07.000000 sphinxcontrib-plot-1.1.0/setup.py
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-04-27 07:30:13.876563 sphinxcontrib-plot-1.1.0/sphinxcontrib/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      269 2021-07-29 23:39:29.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib/__init__.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    17855 2023-04-27 07:16:01.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib/plot.py
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-04-27 07:30:13.883588 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    10498 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/PKG-INFO
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      357 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)        1 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       14 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/namespace_packages.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       12 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/requires.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       14 2023-04-27 07:30:13.000000 sphinxcontrib-plot-1.1.0/sphinxcontrib_plot.egg-info/top_level.txt
```

### Comparing `sphinxcontrib-plot-1.0.9/LICENSE` & `sphinxcontrib-plot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-plot-1.0.9/README.rst` & `sphinxcontrib-plot-1.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -92,15 +92,16 @@
         |Document|   |!magic!|    |       |
         |     {d}|   |       |    |       |
         +---+----+   +-------+    +-------+
             :                         ^
             |       Lots of work      |
             +-------------------------+
 
-Or plot it with parameters::
+To support vector image you can add --svg parameter, it could be converted to
+.pdf in latex automatically::
 
     .. plot:: ditaa --svg
        :caption: figure 2. illustration for ditaa with option
 
           +--------+   +-------+    +-------+
           |        | --+ ditaa +--> |       |
           |  Text  |   +-------+    |diagram|
@@ -192,27 +193,26 @@
 
     convert rose:  -fill none -stroke white -draw 'line 5,40 65,5'  rose_raw.png
 
 This is the output:
 
 .. image:: https://legacy.imagemagick.org/Usage/draw/rose_raw.png
 
-or you can write most of the command line in the body::
+or you can write a magick script as the following::
 
-    .. plot::
+    .. plot:: magick
         :caption: illustration for convert
 
-        convert -size 140x130 xc:white -stroke black \
-        -fill red   -draw "path 'M 60,70 L   60,20   A 50,50 0 0,1 68.7,20.8 Z'" \
-        -fill green -draw "path 'M 60,70 L 68.7,20.8 A 50,50 0 0,1 77.1,23.0 Z'" \
-        -fill blue  -draw "path 'M 68,65 L 85.1,18.0 A 50,50 0 0,1  118,65   Z'" \
-        -fill gold  -draw "path 'M 60,70 L  110,70   A 50,50 0 1,1   60,20   Z'" \
-        -fill black -stroke none  -pointsize 10 \
-        -draw "text 57,19 '10' text 70,20 '10' text 90,19 '70' text 113,78 '270'" \
-        piechart.jpg
+        -size 140x130 xc:white -stroke black
+        -fill red   -draw "path 'M 60,70 L   60,20   A 50,50 0 0,1 68.7,20.8 Z'"
+        -fill green -draw "path 'M 60,70 L 68.7,20.8 A 50,50 0 0,1 77.1,23.0 Z'"
+        -fill blue  -draw "path 'M 68,65 L 85.1,18.0 A 50,50 0 0,1  118,65   Z'"
+        -fill gold  -draw "path 'M 60,70 L  110,70   A 50,50 0 1,1   60,20   Z'"
+        -fill black -stroke none  -pointsize 10
+        -draw "text 57,19 '10' text 70,20 '10' text 90,19 '70' text 113,78 '270'"
 
 .. image:: https://legacy.imagemagick.org/Usage/draw/piechart.jpg
 
 2.6 Other applications
 ----------------------
 
 In theory, All the command which could generate graph could be used after the
@@ -293,9 +293,15 @@
 .. _ditaa: http://ditaa.sourceforge.net/
 .. _image: http://docutils.sourceforge.net/docs/ref/rst/directives.html#image
 .. _figure: http://docutils.sourceforge.net/docs/ref/rst/directives.html#figure
 
 5. Changelog
 ============
 
-1.0 Initial upload.
-1.0.8 Bug fix: When there is no :size: in gnuplot plot, it might crash.
+| 1.0 Initial upload.
+| 1.0.8 Bug fix: When there is no :size: in gnuplot plot, it might crash.
+| 1.0.10 Bug fix: fix the issue that convert doesn't work.
+| 1.0.13 Support magick script
+| 1.0.17 bug fix: convert can has no body.
+| 1.0.18 New feature: 1) Support montage command; 2) Support including .gif image into html and pdf. If it's html, play the .gif, or else if it's pdf, convert the .gif to a list of frame.
+| 1.0.19 Support lines starting with # in the convert/montage body.
+| 1.1.0 Bug fix: It doesn't work for ditaa with convert parameters.
```

### Comparing `sphinxcontrib-plot-1.0.9/setup.py` & `sphinxcontrib-plot-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 requires = ['Sphinx>=0.6',
         ]
 
 setup(
     name='sphinxcontrib-plot',
-    version='1.0.9',
+    version='1.1.0',
     url='https://github.com/stathissideris/sphinxcontrib-plot',
     license='GPLv3',
     author='Yongping Guo',
     author_email='guoyoooping@163.com',
     description='Embed gnuplot, ditaa, pyplot, DOT, etc. diagrams in your Sphinx-based documentation.',
     long_description=open('README.rst').read(),
     platforms='any',
```


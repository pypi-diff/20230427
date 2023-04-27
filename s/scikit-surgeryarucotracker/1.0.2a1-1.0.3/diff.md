# Comparing `tmp/scikit-surgeryarucotracker-1.0.2a1.tar.gz` & `tmp/scikit-surgeryarucotracker-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-surgeryarucotracker-1.0.2a1.tar", last modified: Fri Mar 31 12:42:25 2023, max compression
+gzip compressed data, was "scikit-surgeryarucotracker-1.0.3.tar", last modified: Thu Apr 27 15:00:56 2023, max compression
```

## Comparing `scikit-surgeryarucotracker-1.0.2a1.tar` & `scikit-surgeryarucotracker-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/scikit_surgeryarucotracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/scikit_surgeryarucotracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/scikit_surgeryarucotracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/scikit_surgeryarucotracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/scikit_surgeryarucotracker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/scikit_surgeryarucotracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/scikit_surgeryarucotracker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/
--rwxr-xr-x   0 runner    (1001) docker     (123)      141 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/algorithms/bitmap_to_photo_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/algorithms/compare_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/algorithms/registration_2d3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/algorithms/rigid_bodies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/arucotracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/debugger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/markerpatterns/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/markerpatterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/markerpatterns/makemarkerpatterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/tests/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/tests/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/tests/algorithms/test_compare_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/tests/algorithms/test_rigid_body.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:25.000000 scikit-surgeryarucotracker-1.0.2a1/tests/markerpatterns/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/tests/markerpatterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/tests/markerpatterns/test_makemarkerpatterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-31 12:42:16.000000 scikit-surgeryarucotracker-1.0.2a1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:56.152882 scikit-surgeryarucotracker-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-04-27 15:00:56.152882 scikit-surgeryarucotracker-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:56.152882 scikit-surgeryarucotracker-1.0.3/scikit_surgeryarucotracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-04-27 15:00:56.000000 scikit-surgeryarucotracker-1.0.3/scikit_surgeryarucotracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-27 15:00:56.000000 scikit-surgeryarucotracker-1.0.3/scikit_surgeryarucotracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:00:56.000000 scikit-surgeryarucotracker-1.0.3/scikit_surgeryarucotracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-27 15:00:56.000000 scikit-surgeryarucotracker-1.0.3/scikit_surgeryarucotracker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 15:00:56.000000 scikit-surgeryarucotracker-1.0.3/scikit_surgeryarucotracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 15:00:56.000000 scikit-surgeryarucotracker-1.0.3/scikit_surgeryarucotracker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 15:00:56.152882 scikit-surgeryarucotracker-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:56.152882 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      141 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 15:00:56.152882 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:56.152882 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/algorithms/compare_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/algorithms/registration_2d3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/algorithms/rigid_bodies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/arucotracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:56.152882 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/markerpatterns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/markerpatterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/markerpatterns/makemarkerpatterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:56.148882 scikit-surgeryarucotracker-1.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:56.152882 scikit-surgeryarucotracker-1.0.3/tests/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/tests/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/tests/algorithms/test_compare_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/tests/algorithms/test_rigid_body.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:56.152882 scikit-surgeryarucotracker-1.0.3/tests/markerpatterns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/tests/markerpatterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/tests/markerpatterns/test_makemarkerpatterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-27 15:00:42.000000 scikit-surgeryarucotracker-1.0.3/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scikit-surgeryarucotracker-1.0.2a1/PKG-INFO` & `scikit-surgeryarucotracker-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-surgeryarucotracker
-Version: 1.0.2a1
+Version: 1.0.3
 Summary: scikit-surgeryarucotracker is a simple tracking interface using ARuCo markers
 Home-page: https://github.com/SciKit-Surgery/scikit-surgeryarucotracker
 Author: Stephen Thompson
 Author-email: s.thompson@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgeryarucotracker
         ===============================
@@ -29,22 +29,29 @@
             :target: https://coveralls.io/github/SciKit-Surgery/scikit-surgeryarucotracker?branch=master
             :alt: Test coverage
         
         .. image:: https://readthedocs.org/projects/scikit-surgeryarucotracker/badge/?version=latest
             :target: http://scikit-surgeryarucotracker.readthedocs.io/en/latest/?badge=latest
             :alt: Documentation Status
         
+        .. image:: https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg
+           :target: CODE_OF_CONDUCT.md
+        
         .. image:: https://img.shields.io/badge/Cite-SciKit--Surgery-informational
            :target: https://doi.org/10.1007/s11548-020-02180-5
            :alt: The SciKit-Surgery paper
         
         .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3971640.svg
            :target: https://doi.org/10.5281/zenodo.3971640
            :alt: Software DOI
         
+        .. image:: https://img.shields.io/twitter/follow/scikit_surgery?style=social
+           :target: https://twitter.com/scikit_surgery?ref_src=twsrc%5Etfw
+           :alt: Follow scikit_surgery on twitter
+        
         Author: Stephen Thompson
         
         scikit-surgeryarucotracker provides a simple Python interface between OpenCV's ARuCo marker tracking libraries and other Python packages designed around scikit-surgerytrackers. It allows you to treat an object tracked using ARuCo markers in the same way as an object tracked using other tracking hardware (e.g. aruco - scikit-surgerynditracker). 
         
         scikit-surgeryarucotracker is part of the `SciKit-Surgery`_ software project, developed at the `Wellcome EPSRC Centre for Interventional and Surgical Sciences`_, part of `University College London (UCL)`_.
         
         scikit-surgeryarucotracker is tested with Python 3.6 and may support other Python versions.
```

### Comparing `scikit-surgeryarucotracker-1.0.2a1/README.rst` & `scikit-surgeryarucotracker-1.0.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,29 @@
     :target: https://coveralls.io/github/SciKit-Surgery/scikit-surgeryarucotracker?branch=master
     :alt: Test coverage
 
 .. image:: https://readthedocs.org/projects/scikit-surgeryarucotracker/badge/?version=latest
     :target: http://scikit-surgeryarucotracker.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
+.. image:: https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg
+   :target: CODE_OF_CONDUCT.md
+
 .. image:: https://img.shields.io/badge/Cite-SciKit--Surgery-informational
    :target: https://doi.org/10.1007/s11548-020-02180-5
    :alt: The SciKit-Surgery paper
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3971640.svg
    :target: https://doi.org/10.5281/zenodo.3971640
    :alt: Software DOI
 
+.. image:: https://img.shields.io/twitter/follow/scikit_surgery?style=social
+   :target: https://twitter.com/scikit_surgery?ref_src=twsrc%5Etfw
+   :alt: Follow scikit_surgery on twitter
+
 Author: Stephen Thompson
 
 scikit-surgeryarucotracker provides a simple Python interface between OpenCV's ARuCo marker tracking libraries and other Python packages designed around scikit-surgerytrackers. It allows you to treat an object tracked using ARuCo markers in the same way as an object tracked using other tracking hardware (e.g. aruco - scikit-surgerynditracker). 
 
 scikit-surgeryarucotracker is part of the `SciKit-Surgery`_ software project, developed at the `Wellcome EPSRC Centre for Interventional and Surgical Sciences`_, part of `University College London (UCL)`_.
 
 scikit-surgeryarucotracker is tested with Python 3.6 and may support other Python versions.
```

### Comparing `scikit-surgeryarucotracker-1.0.2a1/scikit_surgeryarucotracker.egg-info/PKG-INFO` & `scikit-surgeryarucotracker-1.0.3/scikit_surgeryarucotracker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-surgeryarucotracker
-Version: 1.0.2a1
+Version: 1.0.3
 Summary: scikit-surgeryarucotracker is a simple tracking interface using ARuCo markers
 Home-page: https://github.com/SciKit-Surgery/scikit-surgeryarucotracker
 Author: Stephen Thompson
 Author-email: s.thompson@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgeryarucotracker
         ===============================
@@ -29,22 +29,29 @@
             :target: https://coveralls.io/github/SciKit-Surgery/scikit-surgeryarucotracker?branch=master
             :alt: Test coverage
         
         .. image:: https://readthedocs.org/projects/scikit-surgeryarucotracker/badge/?version=latest
             :target: http://scikit-surgeryarucotracker.readthedocs.io/en/latest/?badge=latest
             :alt: Documentation Status
         
+        .. image:: https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg
+           :target: CODE_OF_CONDUCT.md
+        
         .. image:: https://img.shields.io/badge/Cite-SciKit--Surgery-informational
            :target: https://doi.org/10.1007/s11548-020-02180-5
            :alt: The SciKit-Surgery paper
         
         .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3971640.svg
            :target: https://doi.org/10.5281/zenodo.3971640
            :alt: Software DOI
         
+        .. image:: https://img.shields.io/twitter/follow/scikit_surgery?style=social
+           :target: https://twitter.com/scikit_surgery?ref_src=twsrc%5Etfw
+           :alt: Follow scikit_surgery on twitter
+        
         Author: Stephen Thompson
         
         scikit-surgeryarucotracker provides a simple Python interface between OpenCV's ARuCo marker tracking libraries and other Python packages designed around scikit-surgerytrackers. It allows you to treat an object tracked using ARuCo markers in the same way as an object tracked using other tracking hardware (e.g. aruco - scikit-surgerynditracker). 
         
         scikit-surgeryarucotracker is part of the `SciKit-Surgery`_ software project, developed at the `Wellcome EPSRC Centre for Interventional and Surgical Sciences`_, part of `University College London (UCL)`_.
         
         scikit-surgeryarucotracker is tested with Python 3.6 and may support other Python versions.
```

### Comparing `scikit-surgeryarucotracker-1.0.2a1/scikit_surgeryarucotracker.egg-info/SOURCES.txt` & `scikit-surgeryarucotracker-1.0.3/scikit_surgeryarucotracker.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 versioneer.py
 scikit_surgeryarucotracker.egg-info/PKG-INFO
 scikit_surgeryarucotracker.egg-info/SOURCES.txt
@@ -9,17 +10,15 @@
 scikit_surgeryarucotracker.egg-info/entry_points.txt
 scikit_surgeryarucotracker.egg-info/requires.txt
 scikit_surgeryarucotracker.egg-info/top_level.txt
 sksurgeryarucotracker/__init__.py
 sksurgeryarucotracker/__main__.py
 sksurgeryarucotracker/_version.py
 sksurgeryarucotracker/arucotracker.py
-sksurgeryarucotracker/debugger.py
 sksurgeryarucotracker/algorithms/__init__.py
-sksurgeryarucotracker/algorithms/bitmap_to_photo_image.py
 sksurgeryarucotracker/algorithms/compare_matrices.py
 sksurgeryarucotracker/algorithms/registration_2d3d.py
 sksurgeryarucotracker/algorithms/rigid_bodies.py
 sksurgeryarucotracker/markerpatterns/__init__.py
 sksurgeryarucotracker/markerpatterns/makemarkerpatterns.py
 tests/algorithms/__init__.py
 tests/algorithms/test_compare_matrices.py
```

### Comparing `scikit-surgeryarucotracker-1.0.2a1/setup.py` & `scikit-surgeryarucotracker-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
             'data',
         ]
     ),
 
     install_requires=[
         'numpy',
         'opencv-contrib-python-headless',
+        'imshowTk',
         'scikit-surgerycore>=0.6.9'
     ],
 
     entry_points={
         'console_scripts': [
             'scikit-surgeryarucotracker=sksurgeryarucotracker.__main__:main',
         ],
```

### Comparing `scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/algorithms/compare_matrices.py` & `scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/algorithms/compare_matrices.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/algorithms/registration_2d3d.py` & `scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/algorithms/registration_2d3d.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/algorithms/rigid_bodies.py` & `scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/algorithms/rigid_bodies.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/arucotracker.py` & `scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/arucotracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 """A class for straightforward tracking with an ARuCo
 """
 from time import time
 from numpy import array, float32, loadtxt, ravel, float64
 from cv2 import aruco
 import cv2
+from imshowtk.imshowtk import ImshowTk as Debugger
 
 from sksurgerycore.baseclasses.tracker import SKSBaseTracker
 from sksurgeryarucotracker.algorithms.rigid_bodies import ArUcoRigidBody, \
                 configure_rigid_bodies
-from sksurgeryarucotracker.debugger import Debugger
 
 def _load_calibration(textfile):
     """
     loads a calibration from a text file
     """
     projection_matrix = loadtxt(textfile, dtype=float32, max_rows=3)
     distortion = loadtxt(textfile, dtype=float32, skiprows=3, max_rows=1)
@@ -168,20 +168,20 @@
 
 
         temporary_rigid_bodies = []
         for dict_index, ar_dict in enumerate(self._ar_dicts):
             marker_corners, marker_ids, _ = \
                     aruco.detectMarkers(frame, ar_dict)
             if not marker_corners:
-                self._debug.update(frame)
+                self._debug.imshow(frame)
                 continue
 
             if self._debug.in_use:
                 aruco.drawDetectedMarkers(frame, marker_corners)
-                self._debug.update(frame)
+                self._debug.imshow(frame)
 
             assigned_marker_ids = []
             for rigid_body in self._rigid_bodies:
                 if rigid_body.get_dictionary_name() == \
                                 self._ar_dict_names[dict_index]:
                     assigned_marker_ids.extend(rigid_body.set_2d_points(
                                     marker_corners, marker_ids))
```

### Comparing `scikit-surgeryarucotracker-1.0.2a1/sksurgeryarucotracker/markerpatterns/makemarkerpatterns.py` & `scikit-surgeryarucotracker-1.0.3/sksurgeryarucotracker/markerpatterns/makemarkerpatterns.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryarucotracker-1.0.2a1/tests/algorithms/test_rigid_body.py` & `scikit-surgeryarucotracker-1.0.3/tests/algorithms/test_rigid_body.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryarucotracker-1.0.2a1/tests/markerpatterns/test_makemarkerpatterns.py` & `scikit-surgeryarucotracker-1.0.3/tests/markerpatterns/test_makemarkerpatterns.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryarucotracker-1.0.2a1/versioneer.py` & `scikit-surgeryarucotracker-1.0.3/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/intronIC-1.3.7.tar.gz` & `tmp/intronIC-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intronIC-1.3.7.tar", last modified: Fri Jun 10 06:26:20 2022, max compression
+gzip compressed data, was "intronIC-1.4.0.tar", last modified: Thu Apr 27 18:37:02 2023, max compression
```

## Comparing `intronIC-1.3.7.tar` & `intronIC-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 glarue    (1000) glarue    (1000)        0 2022-06-10 06:26:20.257292 intronIC-1.3.7/
--rw-r--r--   0 glarue    (1000) glarue    (1000)       34 2020-06-19 17:27:01.000000 intronIC-1.3.7/.gitattributes
--rw-r--r--   0 glarue    (1000) glarue    (1000)    35149 2020-05-25 16:07:32.000000 intronIC-1.3.7/LICENSE
--rw-r--r--   0 glarue    (1000) glarue    (1000)      130 2020-06-19 17:27:01.000000 intronIC-1.3.7/MANIFEST.in
--rw-r--r--   0 glarue    (1000) glarue    (1000)     9169 2022-06-10 06:26:20.257292 intronIC-1.3.7/PKG-INFO
--rw-r--r--   0 glarue    (1000) glarue    (1000)     8806 2022-06-09 22:35:34.000000 intronIC-1.3.7/README.md
--rw-r--r--   0 glarue    (1000) glarue    (1000)       25 2020-06-05 19:09:23.000000 intronIC-1.3.7/_config.yml
-drwxr-xr-x   0 glarue    (1000) glarue    (1000)        0 2022-06-10 06:26:20.247292 intronIC-1.3.7/images/
--rw-r--r--   0 glarue    (1000) glarue    (1000)   273943 2020-06-06 04:38:22.000000 intronIC-1.3.7/images/caenorhabditis_elegans.example.plot.scatter.iic.png
--rw-r--r--   0 glarue    (1000) glarue    (1000)   261002 2020-06-06 04:40:33.000000 intronIC-1.3.7/images/drosophila_melanogaster.cds.example.plot.scatter.iic.png
--rw-r--r--   0 glarue    (1000) glarue    (1000)   293640 2020-06-06 04:39:55.000000 intronIC-1.3.7/images/homo_sapiens.cds.example.plot.scatter.iic.png
-drwxr-xr-x   0 glarue    (1000) glarue    (1000)        0 2022-06-10 06:26:20.257292 intronIC-1.3.7/intronIC/
--rw-r--r--   0 glarue    (1000) glarue    (1000)       93 2020-06-19 17:27:01.000000 intronIC-1.3.7/intronIC/__init__.py
--rw-r--r--   0 glarue    (1000) glarue    (1000)      498 2022-06-10 06:26:20.257292 intronIC-1.3.7/intronIC/_version.py
-drwxr-xr-x   0 glarue    (1000) glarue    (1000)        0 2022-06-10 06:26:20.250625 intronIC-1.3.7/intronIC/data/
--rw-r--r--   0 glarue    (1000) glarue    (1000)     7872 2020-10-31 00:19:42.000000 intronIC-1.3.7/intronIC/data/empirical.u12s.2+.pub_required.matrices
--rw-r--r--   0 glarue    (1000) glarue    (1000)    20322 2020-11-01 16:10:26.000000 intronIC-1.3.7/intronIC/data/scoring_matrices.2+.pub_required.fasta.iic
--rw-r--r--   0 glarue    (1000) glarue    (1000)    20357 2020-11-01 16:10:26.000000 intronIC-1.3.7/intronIC/data/scoring_matrices.2+_pubs.fasta.iic
--rw-r--r--   0 glarue    (1000) glarue    (1000)    20322 2020-11-01 16:10:26.000000 intronIC-1.3.7/intronIC/data/scoring_matrices.fasta.iic
--rw-r--r--   0 glarue    (1000) glarue    (1000)   144116 2020-06-01 16:14:10.000000 intronIC-1.3.7/intronIC/data/u12_reference.introns.iic.gz
--rw-r--r--   0 glarue    (1000) glarue    (1000)      988 2020-09-07 22:11:35.000000 intronIC-1.3.7/intronIC/data/u2.conserved_empirical_bp_pwm.iic
--rw-r--r--   0 glarue    (1000) glarue    (1000)  5379865 2020-06-01 16:14:10.000000 intronIC-1.3.7/intronIC/data/u2_reference.introns.iic.gz
--rwxr-xr-x   0 glarue    (1000) glarue    (1000)   206527 2022-06-10 06:25:05.000000 intronIC-1.3.7/intronIC/intronIC.py
--rw-r--r--   0 glarue    (1000) glarue    (1000)     6989 2020-10-31 00:19:42.000000 intronIC-1.3.7/intronIC/matrices_from_seqs.py
--rw-r--r--   0 glarue    (1000) glarue    (1000)     7008 2020-10-31 00:19:42.000000 intronIC-1.3.7/intronIC/pwms_from_seqs.py
-drwxr-xr-x   0 glarue    (1000) glarue    (1000)        0 2022-06-10 06:26:20.247292 intronIC-1.3.7/intronIC.egg-info/
--rw-r--r--   0 glarue    (1000) glarue    (1000)     9169 2022-06-10 06:26:19.000000 intronIC-1.3.7/intronIC.egg-info/PKG-INFO
--rw-r--r--   0 glarue    (1000) glarue    (1000)      914 2022-06-10 06:26:20.000000 intronIC-1.3.7/intronIC.egg-info/SOURCES.txt
--rw-r--r--   0 glarue    (1000) glarue    (1000)        1 2022-06-10 06:26:19.000000 intronIC-1.3.7/intronIC.egg-info/dependency_links.txt
--rw-r--r--   0 glarue    (1000) glarue    (1000)       52 2022-06-10 06:26:19.000000 intronIC-1.3.7/intronIC.egg-info/entry_points.txt
--rw-r--r--   0 glarue    (1000) glarue    (1000)       48 2022-06-10 06:26:19.000000 intronIC-1.3.7/intronIC.egg-info/requires.txt
--rw-r--r--   0 glarue    (1000) glarue    (1000)        9 2022-06-10 06:26:19.000000 intronIC-1.3.7/intronIC.egg-info/top_level.txt
--rw-r--r--   0 glarue    (1000) glarue    (1000)      839 2022-06-10 06:26:20.257292 intronIC-1.3.7/setup.cfg
--rw-r--r--   0 glarue    (1000) glarue    (1000)      134 2020-06-19 17:28:57.000000 intronIC-1.3.7/setup.py
--rw-r--r--   0 glarue    (1000) glarue    (1000)    68611 2020-06-19 17:30:49.000000 intronIC-1.3.7/versioneer.py
+drwxr-xr-x   0 glarue    (1000) glarue    (1000)        0 2023-04-27 18:37:02.673888 intronIC-1.4.0/
+-rw-r--r--   0 glarue    (1000) glarue    (1000)       34 2020-06-19 17:27:01.000000 intronIC-1.4.0/.gitattributes
+-rw-r--r--   0 glarue    (1000) glarue    (1000)    35149 2020-05-25 16:07:32.000000 intronIC-1.4.0/LICENSE
+-rw-r--r--   0 glarue    (1000) glarue    (1000)      130 2020-06-19 17:27:01.000000 intronIC-1.4.0/MANIFEST.in
+-rw-r--r--   0 glarue    (1000) glarue    (1000)     9169 2023-04-27 18:37:02.673888 intronIC-1.4.0/PKG-INFO
+-rw-r--r--   0 glarue    (1000) glarue    (1000)     8806 2022-06-09 22:35:34.000000 intronIC-1.4.0/README.md
+-rw-r--r--   0 glarue    (1000) glarue    (1000)       25 2020-06-05 19:09:23.000000 intronIC-1.4.0/_config.yml
+drwxr-xr-x   0 glarue    (1000) glarue    (1000)        0 2023-04-27 18:37:02.663888 intronIC-1.4.0/images/
+-rw-r--r--   0 glarue    (1000) glarue    (1000)   273943 2020-06-06 04:38:22.000000 intronIC-1.4.0/images/caenorhabditis_elegans.example.plot.scatter.iic.png
+-rw-r--r--   0 glarue    (1000) glarue    (1000)   261002 2020-06-06 04:40:33.000000 intronIC-1.4.0/images/drosophila_melanogaster.cds.example.plot.scatter.iic.png
+-rw-r--r--   0 glarue    (1000) glarue    (1000)   293640 2020-06-06 04:39:55.000000 intronIC-1.4.0/images/homo_sapiens.cds.example.plot.scatter.iic.png
+drwxr-xr-x   0 glarue    (1000) glarue    (1000)        0 2023-04-27 18:37:02.673888 intronIC-1.4.0/intronIC/
+-rw-r--r--   0 glarue    (1000) glarue    (1000)       93 2020-06-19 17:27:01.000000 intronIC-1.4.0/intronIC/__init__.py
+-rw-r--r--   0 glarue    (1000) glarue    (1000)      498 2023-04-27 18:37:02.673888 intronIC-1.4.0/intronIC/_version.py
+drwxr-xr-x   0 glarue    (1000) glarue    (1000)        0 2023-04-27 18:37:02.667222 intronIC-1.4.0/intronIC/data/
+-rw-r--r--   0 glarue    (1000) glarue    (1000)     7872 2020-10-31 00:19:42.000000 intronIC-1.4.0/intronIC/data/empirical.u12s.2+.pub_required.matrices
+-rw-r--r--   0 glarue    (1000) glarue    (1000)    20322 2020-11-01 16:10:26.000000 intronIC-1.4.0/intronIC/data/scoring_matrices.2+.pub_required.fasta.iic
+-rw-r--r--   0 glarue    (1000) glarue    (1000)    20357 2020-11-01 16:10:26.000000 intronIC-1.4.0/intronIC/data/scoring_matrices.2+_pubs.fasta.iic
+-rw-r--r--   0 glarue    (1000) glarue    (1000)    20322 2020-11-01 16:10:26.000000 intronIC-1.4.0/intronIC/data/scoring_matrices.fasta.iic
+-rw-r--r--   0 glarue    (1000) glarue    (1000)   144116 2020-06-01 16:14:10.000000 intronIC-1.4.0/intronIC/data/u12_reference.introns.iic.gz
+-rw-r--r--   0 glarue    (1000) glarue    (1000)      988 2020-09-07 22:11:35.000000 intronIC-1.4.0/intronIC/data/u2.conserved_empirical_bp_pwm.iic
+-rw-r--r--   0 glarue    (1000) glarue    (1000)  5379865 2020-06-01 16:14:10.000000 intronIC-1.4.0/intronIC/data/u2_reference.introns.iic.gz
+-rwxr-xr-x   0 glarue    (1000) glarue    (1000)   206527 2023-04-27 18:11:53.000000 intronIC-1.4.0/intronIC/intronIC.py
+-rw-r--r--   0 glarue    (1000) glarue    (1000)     6989 2020-10-31 00:19:42.000000 intronIC-1.4.0/intronIC/matrices_from_seqs.py
+-rw-r--r--   0 glarue    (1000) glarue    (1000)     7008 2020-10-31 00:19:42.000000 intronIC-1.4.0/intronIC/pwms_from_seqs.py
+drwxr-xr-x   0 glarue    (1000) glarue    (1000)        0 2023-04-27 18:37:02.667222 intronIC-1.4.0/intronIC.egg-info/
+-rw-r--r--   0 glarue    (1000) glarue    (1000)     9169 2023-04-27 18:37:02.000000 intronIC-1.4.0/intronIC.egg-info/PKG-INFO
+-rw-r--r--   0 glarue    (1000) glarue    (1000)      914 2023-04-27 18:37:02.000000 intronIC-1.4.0/intronIC.egg-info/SOURCES.txt
+-rw-r--r--   0 glarue    (1000) glarue    (1000)        1 2023-04-27 18:37:02.000000 intronIC-1.4.0/intronIC.egg-info/dependency_links.txt
+-rw-r--r--   0 glarue    (1000) glarue    (1000)       52 2023-04-27 18:37:02.000000 intronIC-1.4.0/intronIC.egg-info/entry_points.txt
+-rw-r--r--   0 glarue    (1000) glarue    (1000)       64 2023-04-27 18:37:02.000000 intronIC-1.4.0/intronIC.egg-info/requires.txt
+-rw-r--r--   0 glarue    (1000) glarue    (1000)        9 2023-04-27 18:37:02.000000 intronIC-1.4.0/intronIC.egg-info/top_level.txt
+-rw-r--r--   0 glarue    (1000) glarue    (1000)      857 2023-04-27 18:37:02.673888 intronIC-1.4.0/setup.cfg
+-rw-r--r--   0 glarue    (1000) glarue    (1000)      134 2020-06-19 17:28:57.000000 intronIC-1.4.0/setup.py
+-rw-r--r--   0 glarue    (1000) glarue    (1000)    68611 2020-06-19 17:30:49.000000 intronIC-1.4.0/versioneer.py
```

### Comparing `intronIC-1.3.7/LICENSE` & `intronIC-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/PKG-INFO` & `intronIC-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intronIC
-Version: 1.3.7
+Version: 1.4.0
 Summary: Retrieve annotated intron sequences and classify them as minor (U12-type) or major (U2-type)
 Home-page: https://github.com/glarue/intronIC/
 Author: Graham Larue
 Author-email: egrahamlarue@gmail.com
 License: GPL v3.0
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
```

### Comparing `intronIC-1.3.7/README.md` & `intronIC-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/images/caenorhabditis_elegans.example.plot.scatter.iic.png` & `intronIC-1.4.0/images/caenorhabditis_elegans.example.plot.scatter.iic.png`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/images/drosophila_melanogaster.cds.example.plot.scatter.iic.png` & `intronIC-1.4.0/images/drosophila_melanogaster.cds.example.plot.scatter.iic.png`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/images/homo_sapiens.cds.example.plot.scatter.iic.png` & `intronIC-1.4.0/images/homo_sapiens.cds.example.plot.scatter.iic.png`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/intronIC/data/empirical.u12s.2+.pub_required.matrices` & `intronIC-1.4.0/intronIC/data/empirical.u12s.2+.pub_required.matrices`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/intronIC/data/scoring_matrices.2+.pub_required.fasta.iic` & `intronIC-1.4.0/intronIC/data/scoring_matrices.2+.pub_required.fasta.iic`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/intronIC/data/scoring_matrices.2+_pubs.fasta.iic` & `intronIC-1.4.0/intronIC/data/scoring_matrices.2+_pubs.fasta.iic`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/intronIC/data/scoring_matrices.fasta.iic` & `intronIC-1.4.0/intronIC/data/scoring_matrices.fasta.iic`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/intronIC/data/u12_reference.introns.iic.gz` & `intronIC-1.4.0/intronIC/data/u12_reference.introns.iic.gz`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/intronIC/data/u2.conserved_empirical_bp_pwm.iic` & `intronIC-1.4.0/intronIC/data/u2.conserved_empirical_bp_pwm.iic`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/intronIC/data/u2_reference.introns.iic.gz` & `intronIC-1.4.0/intronIC/data/u2_reference.introns.iic.gz`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/intronIC/intronIC.py` & `intronIC-1.4.0/intronIC/intronIC.py`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/intronIC/matrices_from_seqs.py` & `intronIC-1.4.0/intronIC/matrices_from_seqs.py`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/intronIC/pwms_from_seqs.py` & `intronIC-1.4.0/intronIC/pwms_from_seqs.py`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/intronIC.egg-info/PKG-INFO` & `intronIC-1.4.0/intronIC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intronIC
-Version: 1.3.7
+Version: 1.4.0
 Summary: Retrieve annotated intron sequences and classify them as minor (U12-type) or major (U2-type)
 Home-page: https://github.com/glarue/intronIC/
 Author: Graham Larue
 Author-email: egrahamlarue@gmail.com
 License: GPL v3.0
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
```

### Comparing `intronIC-1.3.7/intronIC.egg-info/SOURCES.txt` & `intronIC-1.4.0/intronIC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intronIC-1.3.7/setup.cfg` & `intronIC-1.4.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = intronIC
-version = 1.3.1
+version = 1.4.0
 license = GPL v3.0
 description = Retrieve annotated intron sequences and classify them as minor (U12-type) or major (U2-type)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/glarue/intronIC/
 author = Graham Larue
 author_email = egrahamlarue@gmail.com
@@ -14,14 +14,15 @@
 include_package_data = True
 install_requires = 
 	numpy
 	scipy
 	scikit-learn >=0.22
 	biogl
 	matplotlib
+	networkx >=2.5.1
 python_requires = >=3.3
 
 [options.package_data]
 intronIC = intronIC/data/*
 
 [options.entry_points]
 console_scripts =
```

### Comparing `intronIC-1.3.7/versioneer.py` & `intronIC-1.4.0/versioneer.py`

 * *Files identical despite different names*


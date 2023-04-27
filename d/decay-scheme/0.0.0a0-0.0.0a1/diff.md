# Comparing `tmp/decay_scheme-0.0.0a0.tar.gz` & `tmp/decay_scheme-0.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decay_scheme-0.0.0a0.tar", max compression
+gzip compressed data, was "decay_scheme-0.0.0a1.tar", max compression
```

## Comparing `decay_scheme-0.0.0a0.tar` & `decay_scheme-0.0.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      134 2023-04-27 07:48:18.102851 decay_scheme-0.0.0a0/data/arrowhead_codes.dat
--rw-r--r--   0        0        0     1078 2023-04-27 07:48:18.107848 decay_scheme-0.0.0a0/data/arrowhead_vertices.dat
--rw-r--r--   0        0        0      251 2023-04-27 11:24:31.788437 decay_scheme-0.0.0a0/decay_scheme/__init__.py
--rw-r--r--   0        0        0     4353 2023-04-27 11:24:31.791445 decay_scheme-0.0.0a0/decay_scheme/decay_scheme_classes.py
--rw-r--r--   0        0        0     7840 2023-04-27 11:24:31.794417 decay_scheme-0.0.0a0/decay_scheme/decay_scheme_drawer.py
--rw-r--r--   0        0        0        0 2023-04-27 11:20:20.477888 decay_scheme-0.0.0a0/LICENSE
--rw-r--r--   0        0        0      503 2023-04-27 11:24:31.796415 decay_scheme-0.0.0a0/pyproject.toml
--rw-r--r--   0        0        0      142 2023-04-27 07:48:18.102851 decay_scheme-0.0.0a0/README.md
--rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 decay_scheme-0.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0      251 2023-04-27 11:24:31.788437 decay_scheme-0.0.0a1/decay_scheme/__init__.py
+-rw-r--r--   0        0        0      134 2023-04-27 07:48:18.102851 decay_scheme-0.0.0a1/decay_scheme/data/arrowhead_codes.dat
+-rw-r--r--   0        0        0     1078 2023-04-27 07:48:18.107848 decay_scheme-0.0.0a1/decay_scheme/data/arrowhead_vertices.dat
+-rw-r--r--   0        0        0     4353 2023-04-27 11:24:31.791445 decay_scheme-0.0.0a1/decay_scheme/decay_scheme_classes.py
+-rw-r--r--   0        0        0     7833 2023-04-27 11:38:12.008057 decay_scheme-0.0.0a1/decay_scheme/decay_scheme_drawer.py
+-rw-r--r--   0        0        0        0 2023-04-27 11:20:20.477888 decay_scheme-0.0.0a1/LICENSE
+-rw-r--r--   0        0        0      516 2023-04-27 11:39:07.286778 decay_scheme-0.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-04-27 07:48:18.102851 decay_scheme-0.0.0a1/README.md
+-rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 decay_scheme-0.0.0a1/PKG-INFO
```

### Comparing `decay_scheme-0.0.0a0/data/arrowhead_vertices.dat` & `decay_scheme-0.0.0a1/decay_scheme/data/arrowhead_vertices.dat`

 * *Files identical despite different names*

### Comparing `decay_scheme-0.0.0a0/decay_scheme/decay_scheme_classes.py` & `decay_scheme-0.0.0a1/decay_scheme/decay_scheme_classes.py`

 * *Files identical despite different names*

### Comparing `decay_scheme-0.0.0a0/decay_scheme/decay_scheme_drawer.py` & `decay_scheme-0.0.0a1/decay_scheme/decay_scheme_drawer.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     QEC_text_offset = 0.2
     below_text_offset = 0.07
     above_text_offset = 0.
     mec2 = 0.51099895000
     energy_format_string = "2.3f"
 
     def __init__(self):
-        data_dir = Path(__file__).parent.parent / "data"
+        data_dir = Path(__file__).parent / "data"
         arrowhead_vertices = np.loadtxt(data_dir / 'arrowhead_vertices.dat')
         arrowhead_vertices[:, 0] = arrowhead_vertices[:, 0] - np.min(arrowhead_vertices[:, 0])
         arrowhead_vertices[:, 1] = arrowhead_vertices[:, 1] - np.mean(arrowhead_vertices[:, 1]) - 0.05
         arrowhead_codes = np.loadtxt(data_dir / 'arrowhead_codes.dat')
         self.arrowhead = mpl_path(arrowhead_vertices, arrowhead_codes)
 
     class UnsizedMarker(MarkerStyle):
```

### Comparing `decay_scheme-0.0.0a0/PKG-INFO` & `decay_scheme-0.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decay-scheme
-Version: 0.0.0a0
+Version: 0.0.0a1
 Summary: A python package to draw nuclear decay schemas
 Author: Erik Asbjørn Mikkelsen Jensen
 Author-email: ej@phys.au.dk
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


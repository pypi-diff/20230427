# Comparing `tmp/DGet-0.5.tar.gz` & `tmp/DGet-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DGet-0.5.tar", last modified: Mon Apr 24 07:20:00 2023, max compression
+gzip compressed data, was "DGet-0.6.tar", last modified: Thu Apr 27 05:31:05 2023, max compression
```

## Comparing `DGet-0.5.tar` & `DGet-0.6.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:20:00.135157 DGet-0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:20:00.135157 DGet-0.5/DGet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 07:19:39.000000 DGet-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-24 07:20:00.135157 DGet-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 07:19:39.000000 DGet-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:20:00.135157 DGet-0.5/dget/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 07:19:39.000000 DGet-0.5/dget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-24 07:19:39.000000 DGet-0.5/dget/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-24 07:19:39.000000 DGet-0.5/dget/adduct.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-24 07:19:39.000000 DGet-0.5/dget/convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-04-24 07:19:39.000000 DGet-0.5/dget/dget.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 07:20:00.135157 DGet-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-24 07:19:39.000000 DGet-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:20:00.135157 DGet-0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-24 07:19:39.000000 DGet-0.5/tests/test_adduct.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-24 07:19:39.000000 DGet-0.5/tests/test_dget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:31:05.559666 DGet-0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:31:05.559666 DGet-0.6/DGet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 05:30:55.000000 DGet-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-27 05:31:05.559666 DGet-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 05:30:55.000000 DGet-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:31:05.559666 DGet-0.6/dget/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 05:30:55.000000 DGet-0.6/dget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-27 05:30:55.000000 DGet-0.6/dget/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-27 05:30:55.000000 DGet-0.6/dget/adduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-27 05:30:55.000000 DGet-0.6/dget/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-04-27 05:30:55.000000 DGet-0.6/dget/dget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-27 05:30:55.000000 DGet-0.6/dget/formula.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 05:31:05.559666 DGet-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 05:30:55.000000 DGet-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:31:05.559666 DGet-0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-27 05:30:55.000000 DGet-0.6/tests/test_adduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-27 05:30:55.000000 DGet-0.6/tests/test_dget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-27 05:30:55.000000 DGet-0.6/tests/test_formula.py
```

### Comparing `DGet-0.5/DGet.egg-info/PKG-INFO` & `DGet-0.6/DGet.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: DGet
-Version: 0.5
+Version: 0.6
 Summary: Calculates compound deuteration from ToF-MS data.
 Home-page: https://github.com/djdt/dget
 Author: djdt
 License: GPL3
+Project-URL: Documentation, https://dget.readthedocs.io
 Project-URL: Source, https://github.com/djdt/dget
 Project-URL: Web App, https://djdt.github.io/dget
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # DGet
```

### Comparing `DGet-0.5/LICENSE` & `DGet-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `DGet-0.5/PKG-INFO` & `DGet-0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: DGet
-Version: 0.5
+Version: 0.6
 Summary: Calculates compound deuteration from ToF-MS data.
 Home-page: https://github.com/djdt/dget
 Author: djdt
 License: GPL3
+Project-URL: Documentation, https://dget.readthedocs.io
 Project-URL: Source, https://github.com/djdt/dget
 Project-URL: Web App, https://djdt.github.io/dget
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # DGet
```

### Comparing `DGet-0.5/dget/__main__.py` & `DGet-0.6/dget/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 from pathlib import Path
 
 from dget import DGet, __version__
 
 
-def parse_args() -> argparse.Namespace:
+def generate_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser("dget")
     parser.add_argument(
         "formula", help="Molecular formula of the compound, see molmass."
     )
     parser.add_argument(
         "--adduct",
         default="[M]+",
@@ -34,16 +34,18 @@
         "--skiprows",
         type=int,
         default=1,
         help="Number of header rows to skip in data file.",
     )
     parser.add_argument(
         "--plot",
-        action="store_true",
-        help="Plot the convolved match against the MS data.",
+        nargs="?",
+        const="targets",
+        help="Plot the convolved match against the MS data, "
+        "use '--plot full' to show the entire mass range..",
     )
     parser.add_argument(
         "--masswidth",
         type=float,
         default=0.5,
         help="Window for integration of MS data.",
     )
@@ -51,41 +53,41 @@
         "--realign",
         action="store_true",
         help="Force alignment of MS data with predicted spectra, "
         "please just calibrate your MS.",
     )
     parser.add_argument("--version", action="version", version=__version__)
 
+    return parser
+
+
+def main():
+    parser = generate_parser()
     args = parser.parse_args()
 
     if args.autoadduct:
         args.adduct = "[M]+"
 
     if "D" not in args.formula:
         parser.error("--formula, must contain at least one D atom.")
 
-    return args
-
-
-def main():
-    args = parse_args()
     loadtxt_kws = {
         "delimiter": args.delimiter,
         "skiprows": args.skiprows,
         "usecols": args.columns,
     }
     dget = DGet(
         args.formula,
         args.tofdata,
         adduct=args.adduct,
         loadtxt_kws=loadtxt_kws,
     )
     if args.autoadduct:
         adduct, diff = dget.guess_adduct_from_base_peak()
-        dget.formula = adduct
+        dget.adduct = adduct
         print(f"Adduct difference from base peak m/z: {diff:.4f}")
         print()
 
     dget.mass_width = args.masswidth
     if args.realign:
         dget.align_tof_with_spectra()
         print(f"Re-aligned ToF data by shifting {dget.offset_mz:.2f} m/z")
@@ -93,13 +95,13 @@
 
     dget.print_results()
 
     if args.plot:
         import matplotlib.pyplot as plt
 
         fig, axes = plt.subplots(1, 1)
-        dget.plot_predicted_spectra(axes)
+        dget.plot_predicted_spectra(axes, mass_range=args.plot)
         plt.show()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DGet-0.5/dget/convolve.py` & `DGet-0.6/dget/convolve.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""Convolution implementations.
+
+Deconvolution is used by DGet to recover the original deuteration
+pattern from a given mass spectrum.
+"""
 from typing import Tuple
 
 import numpy as np
 
 
 def deconvolve(x: np.ndarray, psf: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
     """Inverse of convolution.
```

### Comparing `DGet-0.5/setup.py` & `DGet-0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["dget"],
     license="GPL3",
     author="djdt",
     url="https://github.com/djdt/dget",
     project_urls={
+        "Documentation": "https://dget.readthedocs.io",
         "Source": "https://github.com/djdt/dget",
         "Web App": "https://djdt.github.io/dget",
     },
     install_requires=["numpy>=1.22", "molmass"],
     extras_require={"tests": ["pytest"]},
     entry_points={"console_scripts": ["dget=dget.__main__:main"]},
 )
```


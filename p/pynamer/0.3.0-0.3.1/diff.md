# Comparing `tmp/pynamer-0.3.0.tar.gz` & `tmp/pynamer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-0.3.0.tar", last modified: Tue Apr 25 12:44:42 2023, max compression
+gzip compressed data, was "pynamer-0.3.1.tar", last modified: Wed Apr 26 19:28:36 2023, max compression
```

## Comparing `pynamer-0.3.0.tar` & `pynamer-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 12:44:42.000337 pynamer-0.3.0/
--rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-0.3.0/AUTHORS.md
--rw-rw-rw-   0        0        0     2395 2023-04-25 12:44:30.000000 pynamer-0.3.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0    10951 2023-04-25 12:44:42.001337 pynamer-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     9886 2023-04-24 17:58:35.000000 pynamer-0.3.0/README.md
--rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0     1713 2023-04-25 12:44:42.003334 pynamer-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 17:08:24.000000 pynamer-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 12:44:41.912338 pynamer-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 12:44:41.974335 pynamer-0.3.0/src/pynamer/
--rw-rw-rw-   0        0        0       10 2023-04-25 12:29:58.000000 pynamer-0.3.0/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1185 2023-04-25 12:44:30.000000 pynamer-0.3.0/src/pynamer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 12:44:41.993334 pynamer-0.3.0/src/pynamer/project_name/
--rw-rw-rw-   0        0        0       37 2023-04-14 21:59:18.000000 pynamer-0.3.0/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0     9854 2023-04-25 12:41:44.000000 pynamer-0.3.0/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      395 2023-04-16 15:45:19.000000 pynamer-0.3.0/src/pynamer/setup.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 12:44:41.991336 pynamer-0.3.0/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    10951 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      475 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 12:44:41.997335 pynamer-0.3.0/tests/
--rw-rw-rw-   0        0        0      781 2023-04-21 18:16:35.000000 pynamer-0.3.0/tests/test_pynamer.py
--rw-rw-rw-   0        0        0     1165 2023-04-21 18:15:58.000000 pynamer-0.3.0/tests/test_pynamer_cli.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:28:36.851787 pynamer-0.3.1/
+-rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-0.3.1/AUTHORS.md
+-rw-rw-rw-   0        0        0     2578 2023-04-26 19:28:21.000000 pynamer-0.3.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    10951 2023-04-26 19:28:36.852789 pynamer-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9886 2023-04-24 17:58:35.000000 pynamer-0.3.1/README.md
+-rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1737 2023-04-26 19:28:36.854790 pynamer-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 19:28:36.772624 pynamer-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 19:28:36.807626 pynamer-0.3.1/src/pynamer/
+-rw-rw-rw-   0        0        0       10 2023-04-25 12:29:58.000000 pynamer-0.3.1/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1390 2023-04-26 19:28:21.000000 pynamer-0.3.1/src/pynamer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:28:36.824622 pynamer-0.3.1/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0       37 2023-04-14 21:59:18.000000 pynamer-0.3.1/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0    10947 2023-04-26 19:26:45.000000 pynamer-0.3.1/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      411 2023-04-26 19:24:01.000000 pynamer-0.3.1/src/pynamer/setup.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 19:28:36.822623 pynamer-0.3.1/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    10951 2023-04-26 19:28:36.000000 pynamer-0.3.1/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-04-26 19:28:36.000000 pynamer-0.3.1/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 19:28:36.000000 pynamer-0.3.1/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-26 19:28:36.000000 pynamer-0.3.1/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-04-26 19:28:36.000000 pynamer-0.3.1/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 19:28:36.000000 pynamer-0.3.1/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 19:28:36.849787 pynamer-0.3.1/tests/
+-rw-rw-rw-   0        0        0      781 2023-04-21 18:16:35.000000 pynamer-0.3.1/tests/test_pynamer.py
+-rw-rw-rw-   0        0        0     1165 2023-04-21 18:15:58.000000 pynamer-0.3.1/tests/test_pynamer_cli.py
```

### Comparing `pynamer-0.3.0/CHANGELOG.md` & `pynamer-0.3.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.1 (2023-04-26)
+### Fix
+* Numerous fixes to get a working script ([`5fb56cc`](https://github.com/Stephen-RA-King/pynamer/commit/5fb56cc77c5d6a5552dbf381abbb3100ded29f76))
+
 ## v0.3.0 (2023-04-25)
 ### Feature
 * Add main function ([`15a10c2`](https://github.com/Stephen-RA-King/pynamer/commit/15a10c24d45d529049ebf4fec21d95d28964de1e))
 * Add input and output file processing functions ([`0f56b9f`](https://github.com/Stephen-RA-King/pynamer/commit/0f56b9fecb405cac96fbf0fbe435d2a8e574a875))
 * Add generate_pypi_index function ([`262de6e`](https://github.com/Stephen-RA-King/pynamer/commit/262de6e78be67263e991324e4c127a43a97a2249))
 * Add cleanup function ([`8fa933a`](https://github.com/Stephen-RA-King/pynamer/commit/8fa933a7a6fc12d03e18d181b715fa7e6d9819e3))
 * Add pypi build and upload functions ([`c83378e`](https://github.com/Stephen-RA-King/pynamer/commit/c83378e6b296f66a497757ee402c90b28467c888))
```

### Comparing `pynamer-0.3.0/LICENSE` & `pynamer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-0.3.0/PKG-INFO` & `pynamer-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 0.3.0
+Version: 0.3.1
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -17,15 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # pynamer
 
 _**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
```

### Comparing `pynamer-0.3.0/README.md` & `pynamer-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pynamer-0.3.0/pyproject.toml` & `pynamer-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-0.3.0/setup.cfg` & `pynamer-0.3.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -61,48 +61,49 @@
 000003c0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
 000003d0: 6167 655f 6469 7220 3d20 0d0a 093d 7372  age_dir = ...=sr
 000003e0: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
 000003f0: 6e64 3a0d 0a70 726f 6a65 6374 5f75 726c  nd:..project_url
 00000400: 7320 3d20 0d0a 696e 636c 7564 655f 7061  s = ..include_pa
 00000410: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
 00000420: 650d 0a70 7974 686f 6e5f 7265 7175 6972  e..python_requir
-00000430: 6573 203d 203e 3d33 2e38 0d0a 696e 7374  es = >=3.8..inst
+00000430: 6573 203d 203e 3d33 2e39 0d0a 696e 7374  es = >=3.9..inst
 00000440: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
-00000450: 0a09 7079 7961 6d6c 0d0a 0972 6571 7565  ..pyyaml...reque
-00000460: 7374 730d 0a09 6a69 6e6a 6132 0d0a 0d0a  sts...jinja2....
-00000470: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000480: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-00000490: 2073 7263 0d0a 0d0a 5b6f 7074 696f 6e73   src....[options
-000004a0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
-000004b0: 7079 6e61 6d65 7220 3d20 0d0a 0973 6574  pynamer = ...set
-000004c0: 7570 2e74 7874 0d0a 0952 4541 444d 452e  up.txt...README.
-000004d0: 6d64 0d0a 0970 726f 6a65 6374 5f6e 616d  md...project_nam
-000004e0: 650d 0a09 7072 6f6a 6563 745f 6e61 6d65  e...project_name
-000004f0: 2f5f 5f69 6e69 745f 5f2e 7079 0d0a 0d0a  /__init__.py....
-00000500: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
-00000510: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
-00000520: 7363 7269 7074 7320 3d20 0d0a 0970 796e  scripts = ...pyn
-00000530: 616d 6572 203d 2070 796e 616d 6572 2e70  amer = pynamer.p
-00000540: 796e 616d 6572 3a6d 6169 6e0d 0a0d 0a5b  ynamer:main....[
-00000550: 666c 616b 6538 5d0d 0a64 6f63 7374 7269  flake8]..docstri
-00000560: 6e67 2d63 6f6e 7665 6e74 696f 6e20 3d20  ng-convention = 
-00000570: 6e75 6d70 790d 0a6d 6178 2d63 6f6d 706c  numpy..max-compl
-00000580: 6578 6974 7920 3d20 3138 0d0a 6d61 782d  exity = 18..max-
-00000590: 6c69 6e65 2d6c 656e 6774 6820 3d20 3838  line-length = 88
-000005a0: 0d0a 7365 6c65 6374 203d 2042 2c20 4239  ..select = B, B9
-000005b0: 2c20 432c 2044 2c20 452c 2046 2c20 4e2c  , C, D, E, F, N,
-000005c0: 2057 0d0a 6578 636c 7564 6520 3d20 7465   W..exclude = te
-000005d0: 7374 732f 2a2c 2e74 6f78 2f2a 2c2e 6e6f  sts/*,.tox/*,.no
-000005e0: 782f 2a2c 646f 6373 2f2a 2c2e 6769 742f  x/*,docs/*,.git/
-000005f0: 2a2c 2e67 6974 6875 622f 2a0d 0a69 676e  *,.github/*..ign
-00000600: 6f72 6520 3d20 0d0a 0945 3230 332c 0d0a  ore = ...E203,..
-00000610: 0957 3530 332c 0d0a 0946 3430 312c 0d0a  .W503,...F401,..
-00000620: 7065 722d 6669 6c65 2d69 676e 6f72 6573  per-file-ignores
-00000630: 203d 200d 0a09 5f5f 696e 6974 5f5f 2e70   = ...__init__.p
-00000640: 793a 4634 3031 0d0a 0970 6174 686d 6167  y:F401...pathmag
-00000650: 6963 2e70 793a 4634 3031 0d0a 0974 6573  ic.py:F401...tes
-00000660: 745f 7079 6e61 6d65 722e 7079 3a46 3430  t_pynamer.py:F40
-00000670: 310d 0a09 7079 6e61 6d65 722e 7079 3a46  1...pynamer.py:F
-00000680: 3430 310d 0a0d 0a5b 6567 675f 696e 666f  401....[egg_info
-00000690: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-000006a0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000006b0: 0a                                       .
+00000450: 0a09 6a69 6e6a 6132 0d0a 0962 7569 6c64  ..jinja2...build
+00000460: 0d0a 0970 7979 616d 6c0d 0a09 7265 7175  ...pyyaml...requ
+00000470: 6573 7473 0d0a 0974 7769 6e65 0d0a 0977  ests...twine...w
+00000480: 6865 656c 0d0a 0d0a 5b6f 7074 696f 6e73  heel....[options
+00000490: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+000004a0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
+000004b0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+000004c0: 5f64 6174 615d 0d0a 7079 6e61 6d65 7220  _data]..pynamer 
+000004d0: 3d20 0d0a 0973 6574 7570 2e74 7874 0d0a  = ...setup.txt..
+000004e0: 0952 4541 444d 452e 6d64 0d0a 0970 726f  .README.md...pro
+000004f0: 6a65 6374 5f6e 616d 650d 0a09 7072 6f6a  ject_name...proj
+00000500: 6563 745f 6e61 6d65 2f5f 5f69 6e69 745f  ect_name/__init_
+00000510: 5f2e 7079 0d0a 0d0a 5b6f 7074 696f 6e73  _.py....[options
+00000520: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
+00000530: 636f 6e73 6f6c 655f 7363 7269 7074 7320  console_scripts 
+00000540: 3d20 0d0a 0970 796e 616d 6572 203d 2070  = ...pynamer = p
+00000550: 796e 616d 6572 2e70 796e 616d 6572 3a6d  ynamer.pynamer:m
+00000560: 6169 6e0d 0a0d 0a5b 666c 616b 6538 5d0d  ain....[flake8].
+00000570: 0a64 6f63 7374 7269 6e67 2d63 6f6e 7665  .docstring-conve
+00000580: 6e74 696f 6e20 3d20 6e75 6d70 790d 0a6d  ntion = numpy..m
+00000590: 6178 2d63 6f6d 706c 6578 6974 7920 3d20  ax-complexity = 
+000005a0: 3138 0d0a 6d61 782d 6c69 6e65 2d6c 656e  18..max-line-len
+000005b0: 6774 6820 3d20 3838 0d0a 7365 6c65 6374  gth = 88..select
+000005c0: 203d 2042 2c20 4239 2c20 432c 2044 2c20   = B, B9, C, D, 
+000005d0: 452c 2046 2c20 4e2c 2057 0d0a 6578 636c  E, F, N, W..excl
+000005e0: 7564 6520 3d20 7465 7374 732f 2a2c 2e74  ude = tests/*,.t
+000005f0: 6f78 2f2a 2c2e 6e6f 782f 2a2c 646f 6373  ox/*,.nox/*,docs
+00000600: 2f2a 2c2e 6769 742f 2a2c 2e67 6974 6875  /*,.git/*,.githu
+00000610: 622f 2a0d 0a69 676e 6f72 6520 3d20 0d0a  b/*..ignore = ..
+00000620: 0945 3230 332c 0d0a 0957 3530 332c 0d0a  .E203,...W503,..
+00000630: 0946 3430 312c 0d0a 7065 722d 6669 6c65  .F401,..per-file
+00000640: 2d69 676e 6f72 6573 203d 200d 0a09 5f5f  -ignores = ...__
+00000650: 696e 6974 5f5f 2e70 793a 4634 3031 0d0a  init__.py:F401..
+00000660: 0970 6174 686d 6167 6963 2e70 793a 4634  .pathmagic.py:F4
+00000670: 3031 0d0a 0974 6573 745f 7079 6e61 6d65  01...test_pyname
+00000680: 722e 7079 3a46 3430 310d 0a09 7079 6e61  r.py:F401...pyna
+00000690: 6d65 722e 7079 3a46 3430 310d 0a0d 0a5b  mer.py:F401....[
+000006a0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000006b0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000006c0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `pynamer-0.3.0/src/pynamer/__init__.py` & `pynamer-0.3.1/src/pynamer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 """Top-level package for pynamer."""
 # Core Library modules
 import logging.config
+from importlib.resources import as_file, files
 
 # Third party modules
 import yaml  # type: ignore
 
 __title__ = "pynamer"
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name on the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
@@ -33,21 +34,27 @@
     mode: w
     encoding: utf-8
     formatter: timestamp
 
 formatters:
   basic:
     style: "{"
-    format: "{levelname:s}:{name:s}:{message:s}"
+    format: "{message:s}"
   timestamp:
     style: "{"
     format: "{asctime} - {levelname} - {name} - {message}"
 
 loggers:
   init:
     handlers: [console, file]
     level: DEBUG
     propagate: False
 """
 
 logging.config.dictConfig(yaml.safe_load(LOGGING_CONFIG))
 logger = logging.getLogger("init")
+
+
+project_path = files("pynamer")
+setup_file_path = project_path.joinpath("setup.txt")
+with as_file(setup_file_path) as _setup_path:
+    setup_text = _setup_path.read_text()
```

### Comparing `pynamer-0.3.0/src/pynamer/pynamer.py` & `pynamer-0.3.1/src/pynamer/pynamer.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,63 +7,66 @@
 import re
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 
 # Third party modules
+import build
 import requests  # type: ignore
 import yaml  # type: ignore
-from jinja2 import Environment, FileSystemLoader
+from jinja2 import Template
 
 # Local modules
-from . import logger
+from . import logger, project_path, setup_text
 
 
 class Config:
     PYPIRC = None
     ROOT_DIR = Path.cwd()
     ORIGINAL_PROJECT_NAME = "project_name"
+    NO_CLEANUP: bool = False
 
 
 config = Config()
 
 
 def find_pypirc_file():
     filename = ".pypirc"
     system_path = os.getenv("PATH")
     path_directories = list()
     path_directories.append(os.getcwd())
     path_directories.extend(system_path.split(os.pathsep))
     for directory in path_directories:
-        print(directory)
         file_path = Path(directory) / filename
         if file_path.exists():
-            print(f"{filename} is present in the system's PATH at {directory}")
+            logger.debug(
+                "%s is present in the system's PATH at %s", filename, directory
+            )
             config.PYPIRC = file_path
             break
     else:
-        print(f"{filename} is not present in the system's PATH.")
+        logger.debug("%s is not present in the system's PATH.", filename)
 
 
 def rename_project_dir(old_name: str, new_name: str) -> None:
     old_directory_path = Path(old_name)
     new_directory_path = Path(new_name)
     logger.debug("renaming project directory from %s to %s", old_name, new_name)
     try:
         old_directory_path.rename(new_directory_path)
     except FileNotFoundError:
         logger.error("directory %s cannot be found:", old_directory_path)
 
 
 def create_setup(new_project_name: str) -> None:
-    environment = Environment(autoescape=True, loader=FileSystemLoader("."))
-    template = environment.get_template("setup.txt")
+    template = Template(setup_text)
     content = template.render(PROJECT_NAME=new_project_name)
-    with open("setup.py", mode="w", encoding="utf-8") as message:
+    setup_file = project_path.joinpath("setup.py")
+    with open(setup_file, mode="w", encoding="utf-8") as message:
         logger.debug("creating new setup.py with the following: \n %s", content)
         message.write(content)
 
 
 def delete_director(items_to_delete: list) -> None:
     """Utility function to delete files or directories"""
     for item in items_to_delete:
@@ -74,15 +77,15 @@
             logger.debug("Deleting Directory: %s", item)
             shutil.rmtree(item, ignore_errors=True)
         else:
             logger.debug("Deleting File: %s", item)
             Path.unlink(item, missing_ok=True)
 
 
-def run_command(*arguments: str, shell=False, working_dir=None, project=None) -> None:
+def run_command(*arguments: str, shell=True, working_dir=None, project=None) -> None:
     working_dir = os.getcwd() if working_dir is None else working_dir
     try:
         process = subprocess.Popen(
             arguments,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             shell=shell,
@@ -135,42 +138,52 @@
         logger.info("Latest Version: %s", project_json["info"]["version"])
         return True
     else:
         logger.info("No response from JSON URL")
         return False
 
 
-def build_dist(project_name):
+def build_dist():
     logger.info("Building the distribution... ")
-    run_command(
-        sys.executable, "-m", "build", "--sdist", "--wheel", ".", project=project_name
-    )
+    builder = build.ProjectBuilder(project_path)
+    builder.build("wheel", project_path / "dist")
+    builder.build("sdist", project_path / "dist")
 
 
 def upload_dist(project_name):
     logger.info("Uploading the distribution... ")
+    dir_path = os.fspath(project_path / "dist" / "*")
+    pypirc_path = os.fspath(config.PYPIRC)
     run_command(
         sys.executable,
         "-m",
         "twine",
         "upload",
         "--config-file",
-        ".pypirc",
-        "dist/*",
+        pypirc_path,
+        dir_path,
         project=project_name,
     )
 
 
 def cleanup(new_project_name):
-    rename_project_dir(new_project_name, config.ORIGINAL_PROJECT_NAME)
+    if config.NO_CLEANUP is True:
+        return
+
+    rename_project_dir(
+        project_path.joinpath(new_project_name),
+        project_path.joinpath(config.ORIGINAL_PROJECT_NAME),
+    )
     build_artifacts = [
-        config.ROOT_DIR / "build",
-        config.ROOT_DIR / "dist",
-        config.ROOT_DIR / "".join([new_project_name, ".egg-info"]),
-        config.ROOT_DIR / "setup.py",
+        project_path / "build",
+        project_path / "dist",
+        project_path / "".join([new_project_name, ".egg-info"]),
+        project_path / "setup.py",
+        project_path / "".join([new_project_name, "-0.0.0.tar.gz"]),
+        project_path / "".join([new_project_name, "-0.0.0-py3-none-any.whl"]),
     ]
     logger.debug("cleaning build artifacts %s", build_artifacts)
     delete_director(build_artifacts)
 
 
 # TODO: complete pypi simple search
 def pypi_simple_index():
@@ -249,14 +262,20 @@
     )
     parser.add_argument(
         "-n",
         "--nocleanup",
         action="store_true",
         help="Debug option to bypass deletion of build artifacts",
     )
+    parser.add_argument(
+        "-a",
+        "--alltests",
+        action="store_true",
+        help="Perform all tests",
+    )
 
     args = parser.parse_args()
     logger.debug(
         "arguments collected from the command line: "
         "\n projects: %s, \n register: %s, \n dryrun: %s, \n file: %s, \n output: %s "
         "\n nocleanup: %s",
         args.projects,
@@ -267,14 +286,17 @@
         args.nocleanup,
     )
 
     if args.projects == "None" and args.file == "None":
         raise SystemExit("No projects to analyse")
 
     project_list = []
+    find_pypirc_file()
+    if args.nocleanup is True:
+        config.NO_CLEANUP = True
 
     if args.projects != "None":
         logger.debug("adding project names from command line %s", args.projects)
         project_list.extend(list(set(args.projects)))
         logger.debug("project_list = %s", project_list)
 
     if args.file != "None":
@@ -282,22 +304,36 @@
         project_list.extend(process_input_file(args.file))
         logger.debug("project_list = %s", project_list)
 
     for new_project in project_list:
         if ping := ping_project(new_project):
             ping_json(new_project)
 
-        if not ping and args.register is True:
-            rename_project_dir(config.ORIGINAL_PROJECT_NAME, new_project)
+        if (
+            args.alltests is True
+            and args.register is True
+            and config.PYPIRC is not None
+            or not ping
+            and args.register is True
+            and config.PYPIRC is not None
+        ):
+            rename_project_dir(
+                project_path.joinpath(config.ORIGINAL_PROJECT_NAME),
+                project_path.joinpath(new_project),
+            )
             create_setup(new_project)
-            build_dist(new_project)
+            build_dist()
             if args.dryrun is False:
                 upload_dist(new_project)
             else:
                 logger.info("Dryrun .... bypassing upload to PyPI..")
             cleanup(new_project)
+        elif config.PYPIRC is None:
+            logger.infog(
+                ".pypirc file cannot be located ... wont attempt to 'register'"
+            )
         elif ping and args.register is True:
             logger.info("Project already exists ... wont attempt to 'register'")
 
 
 if __name__ == "__main__":
     SystemExit(main())
```

### Comparing `pynamer-0.3.0/src/pynamer.egg-info/PKG-INFO` & `pynamer-0.3.1/src/pynamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 0.3.0
+Version: 0.3.1
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -17,15 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # pynamer
 
 _**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
```

### Comparing `pynamer-0.3.0/tests/test_pynamer.py` & `pynamer-0.3.1/tests/test_pynamer.py`

 * *Files identical despite different names*

### Comparing `pynamer-0.3.0/tests/test_pynamer_cli.py` & `pynamer-0.3.1/tests/test_pynamer_cli.py`

 * *Files identical despite different names*


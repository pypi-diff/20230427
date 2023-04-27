# Comparing `tmp/fpcross-0.5.3.tar.gz` & `tmp/fpcross-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpcross-0.5.3.tar", last modified: Mon Feb 27 20:19:44 2023, max compression
+gzip compressed data, was "fpcross-0.5.4.tar", last modified: Thu Apr 27 18:52:47 2023, max compression
```

## Comparing `fpcross-0.5.3.tar` & `fpcross-0.5.4.tar`

### file list

```diff
@@ -1,43 +1,27 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-02-27 20:19:44.511227 fpcross-0.5.3/
--rw-r--r--   0 andrei     (501) staff       (20)     1080 2023-02-27 20:13:29.000000 fpcross-0.5.3/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       63 2022-04-04 15:16:57.000000 fpcross-0.5.3/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     3947 2023-02-27 20:19:44.511367 fpcross-0.5.3/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2632 2022-09-26 14:43:46.000000 fpcross-0.5.3/README.md
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-02-27 20:19:44.492001 fpcross-0.5.3/demo/
--rw-r--r--   0 andrei     (501) staff       (20)     6148 2022-09-26 12:05:29.000000 fpcross-0.5.3/demo/.DS_Store
--rw-r--r--   0 andrei     (501) staff       (20)     4518 2022-10-07 08:05:09.000000 fpcross-0.5.3/demo/check.py
--rw-r--r--   0 andrei     (501) staff       (20)     4717 2023-02-27 20:18:02.000000 fpcross-0.5.3/demo/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)      935 2022-10-07 08:05:11.000000 fpcross-0.5.3/demo/demo_oup_spec.py
--rw-r--r--   0 andrei     (501) staff       (20)    53215 2023-02-27 20:18:34.000000 fpcross-0.5.3/demo/demo_result.png
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-02-27 20:19:44.502239 fpcross-0.5.3/demo/result/
--rw-r--r--   0 andrei     (501) staff       (20)    53215 2022-10-07 07:59:40.000000 fpcross-0.5.3/demo/result/dif_3d.png
--rw-r--r--   0 andrei     (501) staff       (20)    36049 2022-09-26 16:03:56.000000 fpcross-0.5.3/demo/result/dif_3d_np.png
--rw-r--r--   0 andrei     (501) staff       (20)    56125 2022-10-07 08:02:18.000000 fpcross-0.5.3/demo/result/dum_3d.png
--rw-r--r--   0 andrei     (501) staff       (20)    47645 2022-09-26 16:03:56.000000 fpcross-0.5.3/demo/result/oup_1d_np.png
--rw-r--r--   0 andrei     (501) staff       (20)    35075 2022-09-26 16:03:59.000000 fpcross-0.5.3/demo/result/oup_2d_np.png
--rw-r--r--   0 andrei     (501) staff       (20)    61453 2022-10-07 07:59:51.000000 fpcross-0.5.3/demo/result/oup_3d.png
--rw-r--r--   0 andrei     (501) staff       (20)    33273 2022-09-26 16:07:18.000000 fpcross-0.5.3/demo/result/oup_3d_np.png
--rw-r--r--   0 andrei     (501) staff       (20)    55175 2022-10-10 15:58:55.000000 fpcross-0.5.3/demo/result/oup_3d_test_new.png
--rw-r--r--   0 andrei     (501) staff       (20)    54518 2022-10-07 07:58:03.000000 fpcross-0.5.3/demo/result/oup_3d_test_old.png
--rw-r--r--   0 andrei     (501) staff       (20)    66393 2022-10-07 08:00:37.000000 fpcross-0.5.3/demo/result/oup_5d.png
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-02-27 20:19:44.506110 fpcross-0.5.3/fpcross/
--rw-r--r--   0 andrei     (501) staff       (20)      158 2023-02-27 20:19:24.000000 fpcross-0.5.3/fpcross/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)    12100 2023-02-27 20:16:59.000000 fpcross-0.5.3/fpcross/equation.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-02-27 20:19:44.510674 fpcross-0.5.3/fpcross/equation_demo/
--rw-r--r--   0 andrei     (501) staff       (20)      161 2022-10-06 11:03:59.000000 fpcross-0.5.3/fpcross/equation_demo/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)      714 2022-08-31 11:41:49.000000 fpcross-0.5.3/fpcross/equation_demo/equation_dif.py
--rw-r--r--   0 andrei     (501) staff       (20)     2608 2022-09-26 15:16:04.000000 fpcross-0.5.3/fpcross/equation_demo/equation_dum.py
--rw-r--r--   0 andrei     (501) staff       (20)     1783 2022-10-06 11:29:48.000000 fpcross-0.5.3/fpcross/equation_demo/equation_oup.py
--rw-r--r--   0 andrei     (501) staff       (20)     1628 2022-10-06 11:46:55.000000 fpcross-0.5.3/fpcross/equation_demo/equation_oup_univ.py
--rw-r--r--   0 andrei     (501) staff       (20)     8688 2022-10-06 11:51:27.000000 fpcross-0.5.3/fpcross/fpcross.py
--rw-r--r--   0 andrei     (501) staff       (20)     1131 2022-10-07 07:57:34.000000 fpcross-0.5.3/fpcross/fpcross_oup_diag.py
--rw-r--r--   0 andrei     (501) staff       (20)     3167 2022-08-31 11:42:47.000000 fpcross-0.5.3/fpcross/plot.py
--rw-r--r--   0 andrei     (501) staff       (20)      283 2022-10-06 11:27:07.000000 fpcross-0.5.3/fpcross/utils.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-02-27 20:19:44.507822 fpcross-0.5.3/fpcross.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     3947 2023-02-27 20:19:44.000000 fpcross-0.5.3/fpcross.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      862 2023-02-27 20:19:44.000000 fpcross-0.5.3/fpcross.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-02-27 20:19:44.000000 fpcross-0.5.3/fpcross.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       28 2023-02-27 20:19:44.000000 fpcross-0.5.3/fpcross.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)        8 2023-02-27 20:19:44.000000 fpcross-0.5.3/fpcross.egg-info/top_level.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-02-27 20:19:44.511842 fpcross-0.5.3/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2543 2022-09-26 14:16:53.000000 fpcross-0.5.3/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-04-27 18:52:47.476634 fpcross-0.5.4/
+-rw-r--r--   0 andrei     (501) staff       (20)     1080 2023-02-27 20:13:29.000000 fpcross-0.5.4/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       63 2022-04-04 15:16:57.000000 fpcross-0.5.4/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     4334 2023-04-27 18:52:47.476840 fpcross-0.5.4/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     3040 2023-04-26 06:25:58.000000 fpcross-0.5.4/README.md
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-04-27 18:52:47.471599 fpcross-0.5.4/demo/
+-rw-r--r--   0 andrei     (501) staff       (20)     6148 2022-09-26 12:05:29.000000 fpcross-0.5.4/demo/.DS_Store
+-rw-r--r--   0 andrei     (501) staff       (20)     4718 2023-04-27 18:51:00.000000 fpcross-0.5.4/demo/check.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4809 2023-04-27 18:45:05.000000 fpcross-0.5.4/demo/demo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-04-27 18:52:47.472923 fpcross-0.5.4/fpcross/
+-rw-r--r--   0 andrei     (501) staff       (20)      113 2023-04-27 18:52:10.000000 fpcross-0.5.4/fpcross/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)    12608 2023-04-27 18:05:36.000000 fpcross-0.5.4/fpcross/equation.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-04-27 18:52:47.476269 fpcross-0.5.4/fpcross/equation_demo/
+-rw-r--r--   0 andrei     (501) staff       (20)      114 2023-04-27 18:40:43.000000 fpcross-0.5.4/fpcross/equation_demo/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1009 2023-04-27 11:21:32.000000 fpcross-0.5.4/fpcross/equation_demo/equation_dif.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3186 2023-04-27 18:38:30.000000 fpcross-0.5.4/fpcross/equation_demo/equation_dum.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2082 2023-04-27 11:25:01.000000 fpcross-0.5.4/fpcross/equation_demo/equation_oup.py
+-rw-r--r--   0 andrei     (501) staff       (20)     8506 2023-04-27 18:32:49.000000 fpcross-0.5.4/fpcross/fpcross.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3528 2023-04-27 17:51:33.000000 fpcross-0.5.4/fpcross/plot.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-04-27 18:52:47.474635 fpcross-0.5.4/fpcross.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     4334 2023-04-27 18:52:47.000000 fpcross-0.5.4/fpcross.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)      471 2023-04-27 18:52:47.000000 fpcross-0.5.4/fpcross.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-04-27 18:52:47.000000 fpcross-0.5.4/fpcross.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       46 2023-04-27 18:52:47.000000 fpcross-0.5.4/fpcross.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        8 2023-04-27 18:52:47.000000 fpcross-0.5.4/fpcross.egg-info/top_level.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-04-27 18:52:47.477564 fpcross-0.5.4/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2543 2023-04-24 22:04:51.000000 fpcross-0.5.4/setup.py
```

### Comparing `fpcross-0.5.3/LICENSE.txt` & `fpcross-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fpcross-0.5.3/PKG-INFO` & `fpcross-0.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: fpcross
-Version: 0.5.3
+Version: 0.5.4
 Summary: Solver in the low-rank tensor-train format with cross approximation approach for solution of the multidimensional Fokker-Planck equation
 Home-page: https://github.com/AndreiChertkov/fpcross
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/fpcross
 Keywords: Fokker-Planck equation low-rank representation tensor train format TT-decomposition cross approximation probability density estimation
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
@@ -41,14 +40,16 @@
 The function f(x, t), its diagonal partial derivatives d f_i (x, t) / d x_i, initial condition r0(x) and scalar diffusion coefficient D should be known. The equation is solved from the initial moment (t = 0) to the user-specified moment (t), while the solutions obtained at each time step can be used if necessary. The resulting solution r(x, t) represents both the TT-tensor on the multidimensional Chebyshev grid and the Chebyshev interpolation coefficients in the TT-format, and therefore it can be quickly calculated at an arbitrary spatial point.
 
 
 ## Installation
 
 The package can be installed via pip: `pip install fpcross` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [fpcross](https://github.com/AndreiChertkov/fpcross) and installed by `python setup.py install` command from the root folder of the project.
 
+> Required python packages [teneva](https://github.com/AndreiChertkov/teneva) (0.14.1+), [matplotlib](https://matplotlib.org/) (3.7.0+) and [tqdm](https://github.com/tqdm/tqdm) (4.64.0+) will be automatically installed during the installation of the main software product.
+
 
 ## Usage
 
 A compact example of using the solver for a user-defined FPE is provided in the script `demo/demo.py` (run it as `python demo/demo.py` from the root of the project).
 
 The software product also implements classes for the model FPEs:
 1. multidimensional simple diffusion problem (see `fpcross/equation_demo/equation_dif.py`);
@@ -59,14 +60,16 @@
 
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Ivan Oseledets](https://github.com/oseledets)
 
+> ✭__🚂  The stars that you give to **fpcross**, motivate us to develop faster and add new interesting features to the code 😃
+
 
 ## Citation
 
 If you find this approach and/or code useful in your research, please consider citing:
 
 ```bibtex
 @article{chertkov2021solution,
@@ -76,9 +79,7 @@
     journal   = {Frontiers in Artificial Intelligence},
     volume    = {4},
     issn      = {2624-8212},
     doi       = {10.3389/frai.2021.668215},
     url       = {https://www.frontiersin.org/article/10.3389/frai.2021.668215}
 }
 ```
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fpcross-0.5.3/README.md` & `fpcross-0.5.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 The function f(x, t), its diagonal partial derivatives d f_i (x, t) / d x_i, initial condition r0(x) and scalar diffusion coefficient D should be known. The equation is solved from the initial moment (t = 0) to the user-specified moment (t), while the solutions obtained at each time step can be used if necessary. The resulting solution r(x, t) represents both the TT-tensor on the multidimensional Chebyshev grid and the Chebyshev interpolation coefficients in the TT-format, and therefore it can be quickly calculated at an arbitrary spatial point.
 
 
 ## Installation
 
 The package can be installed via pip: `pip install fpcross` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [fpcross](https://github.com/AndreiChertkov/fpcross) and installed by `python setup.py install` command from the root folder of the project.
 
+> Required python packages [teneva](https://github.com/AndreiChertkov/teneva) (0.14.1+), [matplotlib](https://matplotlib.org/) (3.7.0+) and [tqdm](https://github.com/tqdm/tqdm) (4.64.0+) will be automatically installed during the installation of the main software product.
+
 
 ## Usage
 
 A compact example of using the solver for a user-defined FPE is provided in the script `demo/demo.py` (run it as `python demo/demo.py` from the root of the project).
 
 The software product also implements classes for the model FPEs:
 1. multidimensional simple diffusion problem (see `fpcross/equation_demo/equation_dif.py`);
@@ -31,14 +33,16 @@
 
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Ivan Oseledets](https://github.com/oseledets)
 
+> ✭__🚂  The stars that you give to **fpcross**, motivate us to develop faster and add new interesting features to the code 😃
+
 
 ## Citation
 
 If you find this approach and/or code useful in your research, please consider citing:
 
 ```bibtex
 @article{chertkov2021solution,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fpcross-0.5.3/demo/.DS_Store` & `fpcross-0.5.4/demo/.DS_Store`

 * *Files identical despite different names*

### Comparing `fpcross-0.5.3/demo/check.py` & `fpcross-0.5.4/demo/check.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-"""Apply the Fokker-Planck solver for different model problems.
+"""Package fpcross, module demo.check: usage of the solver for various problems.
 
-Run it from the root of the project as "clear && python demo/check.py". The
-output should look like this (see also the folder "demo/result" with plots):
+Script, which demonstrates how to apply the Fokker-Planck solver based on the
+cross approximation method for different model problems. Run it from the root
+of the project as "clear && python demo/check.py". The output should looks like
+this (see also the folder "demo/result" with auto-generated plots):
 "
 >>>>>  DIF-3D
 Solve: 100step [00:06, 15.47step/s,  | t=2.50 | r=1.0 | e_t=1.50e-02]
 -----  Solved > Time :   7.0189 sec
 
 >>>>>  OUP-3D
 Solve: 100step [00:08, 11.91step/s,  | t=5.00 | r=4.0 | e_s=1.57e-03]
@@ -47,138 +49,138 @@
 from fpcross import EquationOUP
 from fpcross import FPCross
 
 
 def run():
     print(f'>>>>>  DIF-3D')
     t = tpc()
-    run_dif_3d()
+    _calc_dif_3d()
     print(f'-----  Solved > Time : {tpc()-t:-8.4f} sec\n')
 
     print(f'>>>>>  OUP-3D')
     t = tpc()
-    run_oup_3d()
+    _calc_oup_3d()
     print(f'-----  Solved > Time : {tpc()-t:-8.4f} sec\n')
 
     print(f'>>>>>  OUP-5D')
     t = tpc()
-    run_oup_5d()
+    _calc_oup_5d()
     print(f'-----  Solved > Time : {tpc()-t:-8.4f} sec\n')
 
 
 def run_np():
     print(f'>>>>>  DIF-3D (Numpy format)')
     t = tpc()
-    run_dif_3d_np()
+    _calc_dif_3d_np()
     print(f'-----  Solved > Time : {tpc()-t:-8.4f} sec\n')
 
     print(f'>>>>>  OUP-1D (Numpy format)')
     t = tpc()
-    run_oup_1d_np()
+    _calc_oup_1d_np()
     print(f'-----  Solved > Time : {tpc()-t:-8.4f} sec\n')
 
     print(f'>>>>>  OUP-2D (Numpy format)')
     t = tpc()
-    run_oup_2d_np()
+    _calc_oup_2d_np()
     print(f'-----  Solved > Time : {tpc()-t:-8.4f} sec\n')
 
     print(f'>>>>>  OUP-3D (Numpy format)')
     t = tpc()
-    run_oup_3d_np()
+    _calc_oup_3d_np()
     print(f'-----  Solved > Time : {tpc()-t:-8.4f} sec\n')
 
 
 def run_spec():
     print(f'>>>>>  DUM-3D')
     t = tpc()
-    run_dum_3d()
+    _calc_dum_3d()
     print(f'-----  Solved > Time : {tpc()-t:-8.4f} sec\n')
 
 
-def run_dif_3d():
+def _calc_dif_3d():
     eq = EquationDif(d=3)
     eq.init()
 
     fpc = FPCross(eq, with_hist=True)
     fpc.solve()
     fpc.plot('./demo/result/dif_3d')
 
 
-def run_dif_3d_np():
+def _calc_dif_3d_np():
     eq = EquationDif(d=3, is_full=True)
     eq.init()
 
     fpc = FPCross(eq, with_hist=True)
     fpc.solve()
     fpc.plot('./demo/result/dif_3d_np')
 
 
-def run_dum_3d():
+def _calc_dum_3d():
     eq = EquationDum(d=3)
     eq.init()
 
     fpc = FPCross(eq, with_hist=True)
     fpc.solve()
     fpc.plot('./demo/result/dum_3d', is_spec=True)
 
 
-def run_oup_1d_np():
+def _calc_oup_1d_np():
     eq = EquationOUP(d=1, is_full=True)
     eq.set_coef_rhs(np.array([
         [1.]
     ]))
     eq.init()
 
     fpc = FPCross(eq, with_hist=True)
     fpc.solve()
     fpc.plot('./demo/result/oup_1d_np')
 
 
-def run_oup_2d_np():
+def _calc_oup_2d_np():
     eq = EquationOUP(d=2, is_full=True)
     eq.set_coef_rhs(np.array([
         [1.0, 0.5],
         [0.0, 1.0],
     ]))
     eq.init()
 
     fpc = FPCross(eq, with_hist=True)
     fpc.solve()
     fpc.plot('./demo/result/oup_2d_np')
 
 
-def run_oup_3d():
+def _calc_oup_3d():
     eq = EquationOUP(d=3)
     eq.set_coef_rhs(np.array([
         [1.5, 0.0, 0.0],
         [0.0, 1.0, 0.0],
         [0.5, 0.3, 1.0],
     ]))
     eq.init()
 
     fpc = FPCross(eq, with_hist=True)
     fpc.solve()
     fpc.plot('./demo/result/oup_3d')
 
 
-def run_oup_3d_np():
+def _calc_oup_3d_np():
     eq = EquationOUP(d=3, is_full=True)
     eq.set_coef_rhs(np.array([
         [1.5, 0.0, 0.0],
         [0.0, 1.0, 0.0],
         [0.5, 0.3, 1.0],
     ]))
     eq.init()
 
     fpc = FPCross(eq, with_hist=True)
     fpc.solve()
     fpc.plot('./demo/result/oup_3d_np')
 
 
-def run_oup_5d():
+def _calc_oup_5d():
     eq = EquationOUP(d=5)
     eq.set_coef_rhs(np.array([
         [1.5, 0.0, 0.0, 0.0, 0.0],
         [0.0, 1.0, 0.0, 0.0, 0.0],
         [0.0, 0.0, 1.0, 0.0, 0.0],
         [0.0, 0.0, 0.0, 1.0, 0.0],
         [0.5, 0.3, 0.2, 0.0, 1.0],
```

### Comparing `fpcross-0.5.3/demo/demo.py` & `fpcross-0.5.4/demo/demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-"""Demo script that shows how to use the Fokker-Planck solver.
+"""Package fpcross, module demo.demo: script that shows how to use the solver.
 
-Run it from the root of the project as "clear && python demo/demo.py". The
-output should look like this (see also the plot "demo/demo_result.png"):
+Demo script that shows how to use the Fokker-Planck solver. Run it from the
+root of the project as "clear && python demo/demo.py". The output should looks
+like this (see also the auto-generated plot "demo/demo_result.png"):
 "
 Solve: 100step [00:06, 15.92step/s,  | t=2.50 | r=1.0 | e_t=1.51e-02]
 
 The value of PDF at poi=[0, 0, 0] for different time moments:
 Time   0.0250 | Value   0.0433
 Time   0.0500 | Value   0.0422
 Time   0.0750 | Value   0.0413
```

### Comparing `fpcross-0.5.3/fpcross/equation.py` & `fpcross-0.5.4/fpcross/equation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Package fpcross, module equation: general representation of the target.
+
+This module contains the class Equation, which provides a set of methods for
+setting the parameters of the multidimensional Fokker-Planck equation and
+calculating auxiliary quantities.
+
+"""
 import numpy as np
 import teneva
 
 
 class Equation:
     def __init__(self, d, e, is_full=False, name='Equation'):
         """Class that represents the Fokker-Planck equation.
@@ -60,28 +67,34 @@
         self.cross_info = {}
         self.cross_cache = {} if self.cross_with_cache else None
 
         if Y0 is None:
             Y0 = teneva.rand(self.n, self.cross_r)
 
         if self.is_full:
-            Y = teneva.cheb_bld_full(func, self.a, self.b, self.n)
+            I = teneva.grid_flat(self.n)
+            X = teneva.ind_to_poi(I, self.a, self.b, self.n, 'cheb')
+            Y = func(X).reshape(self.n, order='F')
+
         else:
             e = e or self.e
-            Y = teneva.cheb_bld(func, self.a, self.b, self.n, eps=e, Y0=Y0,
+            f = lambda I: func(
+                teneva.ind_to_poi(I, self.a, self.b, self.n, 'cheb'))
+            Y = teneva.cross(f, Y0,
                 m=self.cross_m,
                 e=e,
                 nswp=self.cross_nswp,
                 tau=self.cross_tau,
                 dr_min=self.cross_dr_min,
                 dr_max=self.cross_dr_max,
                 tau0=self.cross_tau0,
                 k0=self.cross_k0,
                 info=self.cross_info,
                 cache=self.cross_cache)
+            Y = teneva.truncate(Y, e)
 
         return Y
 
     def build_r0(self):
         """Build the initial PDF r(x, 0) on the Chebyshev grid.
 
         Returns:
@@ -151,16 +164,16 @@
 
         Args:
             X (np.ndarray): the set of spatial points. It is np.ndarray of the
                 shape [samples, dimensions].
             t (float): the current value of time.
 
         Returns:
-            np.ndarray: the values of the vector-values rhs for all samples (it
-            is 2D array of the shape [samples, dimensions]).
+            np.ndarray: the values of the vector rhs for all samples (it is 2D
+            array of the shape [samples, dimensions]).
 
         """
         return np.zeros(X.shape)
 
     def f1(self, X, t):
         """The function computes the derivatives for rhs of equation.
 
@@ -176,16 +189,16 @@
 
         """
         return np.zeros(X.shape)
 
     def init(self):
         """The function is used to initialize the equation parameters.
 
-        Run it before the solution by FPCross solver but after the setting all
-        equation parameters ("set_coef", "set_grid", etc.).
+        Run it before the computations with FPCross solver but after the
+        setting all equation parameters (by "set_coef", "set_grid", etc.).
 
         """
         self.with_rs = False
         self.with_rt = False
 
     def r0(self, X):
         """The function computes initial PDF r(x, 0).
@@ -220,15 +233,15 @@
             np.ndarray: the values of the stationary PDF r0(x) for all samples
             (it is 1D array of the shape [samples]).
 
         Note:
             This function can be defined in a child class. In this case, the
             flag "self.with_rs" must also be set manually to True value (e.g.,
             inside the "init" function). In this case, the Fokker-Planck solver
-            will automatically check the accuracy of the received solution.
+            will automatically check the accuracy of the computed solution.
 
         """
         return
 
     def rt(self, X, t):
         """The function computes time-dependent PDF r(x, t).
 
@@ -241,15 +254,15 @@
             np.ndarray: the values of the time-dependent PDF r(x, t) for all
             samples (it is 1D array of the shape [samples]).
 
         Note:
             This function can be defined in a child class. In this case, the
             flag "self.with_rt" must also be set manually to True value (e.g.,
             inside the "init" function). In this case, the Fokker-Planck solver
-            will automatically check the accuracy of the received solution.
+            will automatically check the accuracy of the computed solution.
 
         """
         return
 
     def set_coef(self, coef=0.5):
         """Set diffusion coefficient.
 
@@ -264,21 +277,23 @@
 
         Args:
             coef_pdf (float): coefficient for initial PDF.
 
         """
         self.coef_pdf = coef_pdf
 
-    def set_cross_opts(self, m=None, e=None, nswp=10, tau=1.1, dr_min=1, dr_max=1, tau0=1.05, k0=100, with_cache=True, r=1):
+    def set_cross_opts(self, m=None, e=None, nswp=10, tau=1.1, dr_min=1,
+                       dr_max=1, tau0=1.05, k0=100, with_cache=True, r=1):
         """Set parameters for the TT-cross method.
 
-        See "https://teneva.readthedocs.io/code/core/cross.html" with a
-        detailed description of the parameters. In addition to this parameters,
-        function also accepts "with_cache" (if flag is True, then cache for
-        TT-cross will be used) and "r" (TT-rank for initial approximation).
+        See "https://teneva.readthedocs.io/code/cross.html#teneva.cross.cross"
+        with a detailed description of the parameters. In addition to this
+        parameters, function also accepts "with_cache" (if flag is True, then
+        cache for TT-cross will be used) and "r" (TT-rank for initial
+        approximation).
 
         """
         self.cross_m = m
         self.cross_e = e
         self.cross_nswp = nswp
         self.cross_tau = tau
         self.cross_dr_min = dr_min
```

### Comparing `fpcross-0.5.3/fpcross/equation_demo/equation_oup.py` & `fpcross-0.5.4/fpcross/equation_demo/equation_oup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Package fpcross, module equation_demo.equation_oup: OUP problem.
+
+This module contains the class EquationOUP, which extends the base class
+Equation and provides a description of the multidimensional Ornstein-Uhlenbeck
+process, which is a case of the Fokker-Planck equation with linear term.
+
+"""
 import numpy as np
 from scipy.linalg import solve_lyapunov
 
 
 from ..equation import Equation
```

### Comparing `fpcross-0.5.3/fpcross/fpcross.py` & `fpcross-0.5.4/fpcross/fpcross.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,28 @@
+"""Package fpcross, module fpcross: the solver for the Fokker-Planck equation.
+
+This module contains the class FPCross, which represents the Fokker-Planck
+solver based on the cross approximation method in the tensor train format.
+
+"""
 import numpy as np
 from scipy.linalg import expm
 from scipy.linalg import toeplitz
 import teneva
 from time import perf_counter as tpc
 from tqdm import tqdm
 
 
 from .plot import plot
 from .plot import plot_spec
 
 
 class FPCross:
-    def __init__(self, eq, with_hist=False, with_y_list=False, with_a_list=False):
+    def __init__(self, eq, with_hist=False, with_y_list=False,
+                 with_a_list=False):
         """Class that represents the solver for the Fokker-Planck equation.
 
         Args:
             eq (Equation): equation class instance.
             with_hist (bool): if flag is set, then accuracy of the result will
                 be checked after each time step. Otherwise, the accuracy check
                 will be performed only after the solver has finished running.
@@ -35,22 +42,22 @@
         self.Y = None  # Current solution r(x, t); it is tensor on the grid
         self.Z = None  # Matrix exponent for the finite difference matrices
         self.m = 0     # Current time-step
         self.s = None  # Current value of Y integral over the spatial domain
         self.t = 0.    # Current value of the time variable
         self.tc = 0.   # Computation time (duration of solver work)
 
-        # Special varuables:
+        # Special variables:
         self.is_last = False
 
         # History for errors, ranks ant integral while computation proccess:
-        self.es_list = []
-        self.et_list = []
-        self.r_list = []
-        self.s_list = []
+        self.es_list = []  # Errors vs stationary exact solution
+        self.et_list = []  # Errors vs time dependent exact solution
+        self.r_list = []   # TT-ranks of the TT-tensor Y
+        self.s_list = []   # Y integrals over the spatial domain
 
         # History for solutions from each time step:
         self.with_y_list = bool(with_y_list)
         self.Y_list = []
         self.with_a_list = bool(with_a_list)
         self.A_list = []
 
@@ -70,15 +77,15 @@
             will be np.ndarray of the shape [samples].
 
         """
         is_one = len(X.shape) == 1
         if is_one:
             X = X.reshape(1, -1)
 
-        func = teneva.cheb_get_full if self.is_full else teneva.cheb_get
+        func = teneva.func_get_full if self.is_full else teneva.func_get
         y = func(X, self.A, self.eq.a, self.eq.b)
 
         return y[0] if is_one else y
 
     def plot(self, fpath=None, is_spec=False):
         """Plot the computation result.
 
@@ -100,14 +107,15 @@
 
         for m in range(1, self.eq.m + 1):
             self.m = m
             self.t = self.eq.h * self.m
             self.is_last = (m == self.eq.m)
 
             self._step()
+            self._step_hist()
             self._step_proc()
             self.text += self.eq.callback(self) or ''
 
             tqdm_.set_postfix_str(self.text, refresh=True)
             tqdm_.update(1)
 
         tqdm_.close()
@@ -133,40 +141,30 @@
 
         e = teneva.accuracy(self.Y, self.eq.Yt)
         self.et_list.append(e)
 
         self.text += f' | e_t={e:-8.2e}'
         return e
 
-    def _conv_apply(self, n_fine_fact=None):
-        if n_fine_fact is not None and not self.is_full:
-            # Experimental option!! Should be "None" in actual code
-            n_fine = self.eq.n * n_fine_fact
-            Z = teneva.cheb_gets(self.A, self.eq.a, self.eq.b, n_fine)
-
+    def _conv_apply(self):
         def func(y, t):
             X, r = y[:, :-1], y[:, -1]
             f0 = self.eq.f(X, self.t)
             f1 = self.eq.f1(X, self.t)
             f1_mult = - np.sum(f1, axis=1) * r
             f1_mult = f1_mult.reshape(-1, 1)
             return np.hstack([f0, f1_mult])
 
         def step_conv(X):
             X0 = ode_solve(self.eq.f, X, self.t, 2, -self.eq.h)
 
             if self.is_full:
-                w0 = teneva.cheb_get_full(X0, self.A, self.eq.a, self.eq.b)
+                w0 = teneva.func_get_full(X0, self.A, self.eq.a, self.eq.b)
             else:
-                if n_fine_fact is None:
-                    w0 = teneva.cheb_get(X0, self.A, self.eq.a, self.eq.b)
-                else:
-                    I0 = teneva.poi_to_ind(X0,
-                        self.eq.a, self.eq.b, n_fine, 'cheb')
-                    w0 = teneva.get_many(Z, I0)
+                w0 = teneva.func_get(X0, self.A, self.eq.a, self.eq.b)
 
             y0 = np.hstack([X0, w0.reshape(-1, 1)])
 
             y1 = ode_solve(func, y0, self.t-self.eq.h, 2, self.eq.h)
 
             w1 = y1[:, -1]
 
@@ -183,74 +181,68 @@
             for k in range(self.eq.d):
                 self.Y[k] = np.einsum('ij,kjm->kim', self.Z, self.Y[k])
             # TODO. Do we need truncation here (?):
             self.Y = teneva.truncate(self.Y, self.eq.e)
 
     def _diff_init(self):
         n = self.eq.n[0]
-        D1, D2 = teneva.cheb_diff_matrix(self.eq.a[0], self.eq.b[0], n, 2)
+        D1, D2 = teneva.func_diff_matrix(self.eq.a[0], self.eq.b[0], n, 2)
         h0 = self.eq.h / 2
         J0 = np.eye(n)
         J0[+0, +0] = 0.
         J0[-1, -1] = 0.
         self.Z = expm(h0 * self.eq.coef * J0 @ D2)
 
         if self.is_full:
             Z0 = self.Z.copy()
             for k in range(1, self.eq.d):
                 self.Z = np.kron(self.Z, Z0)
 
     def _interpolate(self):
         if self.is_full:
-            self.A = teneva.cheb_int_full(self.Y)
+            self.A = teneva.func_int_full(self.Y)
         else:
-            self.A = teneva.cheb_int(self.Y)
+            self.A = teneva.func_int(self.Y)
             # TODO. Do we need truncation here (?):
             self.A = teneva.truncate(self.A, self.eq.e)
 
     def _renormalize(self):
         if self.is_full:
-            self.s = teneva.cheb_sum_full(self.A, self.eq.a, self.eq.b)
+            self.s = teneva.func_sum_full(self.A, self.eq.a, self.eq.b)
             self.Y = (1. / self.s) * self.Y
         else:
-            self.s = teneva.cheb_sum(self.A, self.eq.a, self.eq.b)
+            self.s = teneva.func_sum(self.A, self.eq.a, self.eq.b)
             self.Y = teneva.mul(1. / self.s, self.Y)
 
     def _step(self):
         tc = tpc()
         self._diff_apply()
         self._interpolate()
         self._conv_apply()
         #self._interpolate()
         #self._renormalize()
         self.W = teneva.copy(self.Y)
         self._diff_apply()
         self._interpolate()
         self.tc += tpc() - tc
 
-        self._step_hist()
-
     def _step_hist(self):
         if self.with_y_list:
-            Y = self.Y.copy() if self.is_full else teneva.copy(self.Y)
-            self.Y_list.append(Y)
+            self.Y_list.append(teneva.copy(self.Y))
         if self.with_a_list:
-            A = self.A.copy() if self.is_full else teneva.copy(self.A)
-            self.A_list.append(A)
+            self.A_list.append(teneva.copy(self.A))
 
     def _step_init(self):
         tc = tpc()
         self._diff_init()
         self.Y = self.eq.build_r0()
 
         self._interpolate()
         self._renormalize()
 
-
-
         self.W = teneva.copy(self.Y)
         self.tc += tpc() - tc
 
     def _step_proc(self):
         self.text = f' | t={self.t:-4.2f}'
 
         if not self.is_full:
```

### Comparing `fpcross-0.5.3/fpcross.egg-info/PKG-INFO` & `fpcross-0.5.4/fpcross.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: fpcross
-Version: 0.5.3
+Version: 0.5.4
 Summary: Solver in the low-rank tensor-train format with cross approximation approach for solution of the multidimensional Fokker-Planck equation
 Home-page: https://github.com/AndreiChertkov/fpcross
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/fpcross
 Keywords: Fokker-Planck equation low-rank representation tensor train format TT-decomposition cross approximation probability density estimation
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
@@ -41,14 +40,16 @@
 The function f(x, t), its diagonal partial derivatives d f_i (x, t) / d x_i, initial condition r0(x) and scalar diffusion coefficient D should be known. The equation is solved from the initial moment (t = 0) to the user-specified moment (t), while the solutions obtained at each time step can be used if necessary. The resulting solution r(x, t) represents both the TT-tensor on the multidimensional Chebyshev grid and the Chebyshev interpolation coefficients in the TT-format, and therefore it can be quickly calculated at an arbitrary spatial point.
 
 
 ## Installation
 
 The package can be installed via pip: `pip install fpcross` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [fpcross](https://github.com/AndreiChertkov/fpcross) and installed by `python setup.py install` command from the root folder of the project.
 
+> Required python packages [teneva](https://github.com/AndreiChertkov/teneva) (0.14.1+), [matplotlib](https://matplotlib.org/) (3.7.0+) and [tqdm](https://github.com/tqdm/tqdm) (4.64.0+) will be automatically installed during the installation of the main software product.
+
 
 ## Usage
 
 A compact example of using the solver for a user-defined FPE is provided in the script `demo/demo.py` (run it as `python demo/demo.py` from the root of the project).
 
 The software product also implements classes for the model FPEs:
 1. multidimensional simple diffusion problem (see `fpcross/equation_demo/equation_dif.py`);
@@ -59,14 +60,16 @@
 
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Ivan Oseledets](https://github.com/oseledets)
 
+> ✭__🚂  The stars that you give to **fpcross**, motivate us to develop faster and add new interesting features to the code 😃
+
 
 ## Citation
 
 If you find this approach and/or code useful in your research, please consider citing:
 
 ```bibtex
 @article{chertkov2021solution,
@@ -76,9 +79,7 @@
     journal   = {Frontiers in Artificial Intelligence},
     volume    = {4},
     issn      = {2624-8212},
     doi       = {10.3389/frai.2021.668215},
     url       = {https://www.frontiersin.org/article/10.3389/frai.2021.668215}
 }
 ```
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fpcross-0.5.3/setup.py` & `fpcross-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     description=desc,
     long_description=desc_long,
     long_description_content_type='text/markdown',
     author='Andrei Chertkov',
     author_email='andre.chertkov@gmail.com',
     url='https://github.com/AndreiChertkov/fpcross',
     classifiers=[
-        'Development Status :: 3 - Alpha', # 4 - Beta, 5 - Production/Stable
+        'Development Status :: 4 - Beta', # 3 - Alpha, 5 - Production/Stable
         'License :: OSI Approved :: MIT License',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Intended Audience :: Science/Research',
         'Operating System :: OS Independent',
```


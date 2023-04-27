# Comparing `tmp/xyz_py-5.4.2.tar.gz` & `tmp/xyz_py-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyz_py-5.4.2.tar", last modified: Mon Apr 24 13:21:47 2023, max compression
+gzip compressed data, was "xyz_py-5.5.0.tar", last modified: Thu Apr 27 16:01:59 2023, max compression
```

## Comparing `xyz_py-5.4.2.tar` & `xyz_py-5.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:21:47.325545 xyz_py-5.4.2/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-24 13:21:19.000000 xyz_py-5.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-24 13:21:47.325545 xyz_py-5.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-24 13:21:19.000000 xyz_py-5.4.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-24 13:21:19.000000 xyz_py-5.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 13:21:47.325545 xyz_py-5.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-24 13:21:43.000000 xyz_py-5.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:21:47.320545 xyz_py-5.4.2/xyz_py/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-24 13:21:19.000000 xyz_py-5.4.2/xyz_py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7424 2023-04-24 13:21:19.000000 xyz_py-5.4.2/xyz_py/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     9876 2023-04-24 13:21:19.000000 xyz_py-5.4.2/xyz_py/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-24 13:21:43.000000 xyz_py-5.4.2/xyz_py/version.py
--rw-rw-rw-   0 root         (0) root         (0)    37858 2023-04-24 13:21:19.000000 xyz_py-5.4.2/xyz_py/xyz_py.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:21:47.323545 xyz_py-5.4.2/xyz_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:01:59.982057 xyz_py-5.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-27 16:01:31.000000 xyz_py-5.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-27 16:01:59.980056 xyz_py-5.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-27 16:01:31.000000 xyz_py-5.5.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-27 16:01:31.000000 xyz_py-5.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 16:01:59.982057 xyz_py-5.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-27 16:01:55.000000 xyz_py-5.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:01:59.974056 xyz_py-5.5.0/xyz_py/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-27 16:01:31.000000 xyz_py-5.5.0/xyz_py/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7424 2023-04-27 16:01:31.000000 xyz_py-5.5.0/xyz_py/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10677 2023-04-27 16:01:31.000000 xyz_py-5.5.0/xyz_py/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-27 16:01:55.000000 xyz_py-5.5.0/xyz_py/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    37858 2023-04-27 16:01:31.000000 xyz_py-5.5.0/xyz_py/xyz_py.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:01:59.980056 xyz_py-5.5.0/xyz_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/top_level.txt
```

### Comparing `xyz_py-5.4.2/LICENSE` & `xyz_py-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xyz_py-5.4.2/PKG-INFO` & `xyz_py-5.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz_py
-Version: 5.4.2
+Version: 5.5.0
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyz_py-5.4.2/README.md` & `xyz_py-5.5.0/README.md`

 * *Files identical despite different names*

### Comparing `xyz_py-5.4.2/setup.py` & `xyz_py-5.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "5.4.2"
+__version__ = "5.5.0"
 
 setuptools.setup(
     name="xyz_py",
     version=__version__,
     author="Jon Kragskow",
     author_email="jonkragskow@gmail.com",
     description="A package for manipulating xyz files and chemical structures",
```

### Comparing `xyz_py-5.4.2/xyz_py/atomic.py` & `xyz_py-5.5.0/xyz_py/atomic.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.4.2/xyz_py/cli.py` & `xyz_py-5.5.0/xyz_py/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,14 +248,25 @@
 
     for key, val in entities_dict.items():
         print('{} : {:d}'.format(key, len(val)))
 
     return
 
 
+def renumber_func(uargs):
+
+    l, c = xyz_py.load_xyz(uargs.xyz_file)
+
+    l = xyz_py.add_label_indices(l, style=uargs.style)
+
+    xyz_py.save_xyz(uargs.xyz_file, l, c)
+
+    return
+
+
 def parse_cutoffs(cutoffs):
 
     if len(cutoffs) % 2:
         raise argparse.ArgumentTypeError('Error, cutoffs should come in pairs')
 
     for it in range(1, len(cutoffs), 2):
         try:
@@ -432,14 +443,39 @@
         '--cutoffs',
         type=str,
         nargs='+',
         metavar='symbol number',
         help='Modify cutoff used to define bonds'
     )
 
+    renumber = subparsers.add_parser(
+        'renumber',
+        description=(
+            '(Re)numbers atom labels in file'
+        )
+    )
+    renumber.set_defaults(func=renumber_func)
+
+    renumber.add_argument(
+        'xyz_file',
+        type=str,
+        help='File containing xyz coordinates in .xyz format'
+    )
+
+    renumber.add_argument(
+        '--style',
+        type=str,
+        default='per_element',
+        choices=['per_element', 'sequential'],
+        help=(
+            'per_element : Index by element e.g. Dy1, Dy2, N1, N2, etc.'
+            'sequential : Index the atoms 1->N'
+        )
+    )
+
     # If arg_list==None, i.e. normal cli usage, parse_args() reads from
     # 'sys.argv'. The arg_list can be used to call the argparser from the
     # back end.
 
     # read sub-parser
     parser.set_defaults(func=lambda args: parser.print_help())
     args = parser.parse_args(arg_list)
```

### Comparing `xyz_py-5.4.2/xyz_py/xyz_py.py` & `xyz_py-5.5.0/xyz_py/xyz_py.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.4.2/xyz_py.egg-info/PKG-INFO` & `xyz_py-5.5.0/xyz_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz-py
-Version: 5.4.2
+Version: 5.5.0
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```


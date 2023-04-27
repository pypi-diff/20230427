# Comparing `tmp/anutils-0.4.0.tar.gz` & `tmp/anutils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anutils-0.4.0.tar", last modified: Thu Apr 27 06:44:15 2023, max compression
+gzip compressed data, was "anutils-0.4.1.tar", last modified: Thu Apr 27 06:46:41 2023, max compression
```

## Comparing `anutils-0.4.0.tar` & `anutils-0.4.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:44:15.275430 anutils-0.4.0/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1799 2022-06-15 05:53:11.000000 anutils-0.4.0/.gitignore
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      248 2023-04-27 06:44:15.275430 anutils-0.4.0/PKG-INFO
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1710 2023-03-18 08:13:48.000000 anutils-0.4.0/README.md
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-04-27 06:44:15.275430 anutils-0.4.0/setup.cfg
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      850 2023-04-27 06:43:45.000000 anutils-0.4.0/setup.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:44:15.267430 anutils-0.4.0/src/
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:44:15.271430 anutils-0.4.0/src/anutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       67 2023-03-03 09:18:56.000000 anutils-0.4.0/src/anutils/__init__.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:44:15.271430 anutils-0.4.0/src/anutils/mlutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       70 2022-07-20 14:02:32.000000 anutils-0.4.0/src/anutils/mlutils/__init__.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2457 2022-07-20 14:06:26.000000 anutils-0.4.0/src/anutils/mlutils/mlutils.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:44:15.271430 anutils-0.4.0/src/anutils/scutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      145 2023-04-19 08:30:07.000000 anutils-0.4.0/src/anutils/scutils/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4822 2023-04-26 13:10:33.000000 anutils-0.4.0/src/anutils/scutils/annotation.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:44:15.271430 anutils-0.4.0/src/anutils/scutils/data/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       19 2023-04-18 12:39:59.000000 anutils-0.4.0/src/anutils/scutils/data/__init__.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     3922 2023-04-10 19:26:09.000000 anutils-0.4.0/src/anutils/scutils/data/data.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1539 2023-04-18 21:48:37.000000 anutils-0.4.0/src/anutils/scutils/data/h5ad2mtx.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1211 2023-04-10 19:26:07.000000 anutils-0.4.0/src/anutils/scutils/data/mtx2rds.R
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:44:15.271430 anutils-0.4.0/src/anutils/scutils/external/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       45 2023-04-19 06:02:41.000000 anutils-0.4.0/src/anutils/scutils/external/__init__.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:44:15.271430 anutils-0.4.0/src/anutils/scutils/external/integration/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      102 2023-04-19 06:30:26.000000 anutils-0.4.0/src/anutils/scutils/external/integration/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1945 2023-04-23 09:52:44.000000 anutils-0.4.0/src/anutils/scutils/external/integration/harmony.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2809 2023-04-20 06:33:17.000000 anutils-0.4.0/src/anutils/scutils/external/integration/harmony_matrix.R
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     3812 2023-04-19 08:24:33.000000 anutils-0.4.0/src/anutils/scutils/external/integration/seurat.R
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1668 2023-04-26 13:02:47.000000 anutils-0.4.0/src/anutils/scutils/external/integration/seurat.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    11085 2023-04-26 13:43:46.000000 anutils-0.4.0/src/anutils/scutils/plotting.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     3926 2023-04-23 14:56:13.000000 anutils-0.4.0/src/anutils/scutils/preprocessing.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:44:15.275430 anutils-0.4.0/src/anutils/scutils/sc_cuda/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       72 2023-03-12 12:35:54.000000 anutils-0.4.0/src/anutils/scutils/sc_cuda/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    29119 2023-04-20 13:48:41.000000 anutils-0.4.0/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2503 2023-04-20 13:50:49.000000 anutils-0.4.0/src/anutils/scutils/sc_cuda/scanpy_cuda.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4564 2023-03-12 12:33:33.000000 anutils-0.4.0/src/anutils/scutils/sc_cuda/scib_cuda.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      687 2023-04-20 12:49:32.000000 anutils-0.4.0/src/anutils/scutils/utils.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     9029 2023-04-23 04:03:59.000000 anutils-0.4.0/src/anutils/utils.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:44:15.271430 anutils-0.4.0/src/anutils.egg-info/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      248 2023-04-27 06:44:14.000000 anutils-0.4.0/src/anutils.egg-info/PKG-INFO
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1116 2023-04-27 06:44:15.000000 anutils-0.4.0/src/anutils.egg-info/SOURCES.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)        1 2023-04-27 06:44:14.000000 anutils-0.4.0/src/anutils.egg-info/dependency_links.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       57 2023-04-27 06:44:15.000000 anutils-0.4.0/src/anutils.egg-info/requires.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)        8 2023-04-27 06:44:15.000000 anutils-0.4.0/src/anutils.egg-info/top_level.txt
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:44:15.275430 anutils-0.4.0/tests/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      581 2022-06-17 11:20:29.000000 anutils-0.4.0/tests/run_tests.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1799 2022-06-15 05:53:11.000000 anutils-0.4.1/.gitignore
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2164 2023-04-27 06:46:41.375658 anutils-0.4.1/PKG-INFO
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1710 2023-03-18 08:13:48.000000 anutils-0.4.1/README.md
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-04-27 06:46:41.375658 anutils-0.4.1/setup.cfg
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      850 2023-04-27 06:46:30.000000 anutils-0.4.1/setup.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.371658 anutils-0.4.1/src/
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       67 2023-03-03 09:18:56.000000 anutils-0.4.1/src/anutils/__init__.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/mlutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       70 2022-07-20 14:02:32.000000 anutils-0.4.1/src/anutils/mlutils/__init__.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2457 2022-07-20 14:06:26.000000 anutils-0.4.1/src/anutils/mlutils/mlutils.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/scutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      145 2023-04-19 08:30:07.000000 anutils-0.4.1/src/anutils/scutils/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4822 2023-04-26 13:10:33.000000 anutils-0.4.1/src/anutils/scutils/annotation.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/scutils/data/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       19 2023-04-18 12:39:59.000000 anutils-0.4.1/src/anutils/scutils/data/__init__.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     3922 2023-04-10 19:26:09.000000 anutils-0.4.1/src/anutils/scutils/data/data.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1539 2023-04-18 21:48:37.000000 anutils-0.4.1/src/anutils/scutils/data/h5ad2mtx.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1211 2023-04-10 19:26:07.000000 anutils-0.4.1/src/anutils/scutils/data/mtx2rds.R
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/scutils/external/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       45 2023-04-19 06:02:41.000000 anutils-0.4.1/src/anutils/scutils/external/__init__.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/scutils/external/integration/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      102 2023-04-19 06:30:26.000000 anutils-0.4.1/src/anutils/scutils/external/integration/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1945 2023-04-23 09:52:44.000000 anutils-0.4.1/src/anutils/scutils/external/integration/harmony.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2809 2023-04-20 06:33:17.000000 anutils-0.4.1/src/anutils/scutils/external/integration/harmony_matrix.R
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     3812 2023-04-19 08:24:33.000000 anutils-0.4.1/src/anutils/scutils/external/integration/seurat.R
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1668 2023-04-26 13:02:47.000000 anutils-0.4.1/src/anutils/scutils/external/integration/seurat.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    11085 2023-04-26 13:43:46.000000 anutils-0.4.1/src/anutils/scutils/plotting.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     3926 2023-04-23 14:56:13.000000 anutils-0.4.1/src/anutils/scutils/preprocessing.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/scutils/sc_cuda/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       72 2023-03-12 12:35:54.000000 anutils-0.4.1/src/anutils/scutils/sc_cuda/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    29119 2023-04-20 13:48:41.000000 anutils-0.4.1/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2503 2023-04-20 13:50:49.000000 anutils-0.4.1/src/anutils/scutils/sc_cuda/scanpy_cuda.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4564 2023-03-12 12:33:33.000000 anutils-0.4.1/src/anutils/scutils/sc_cuda/scib_cuda.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      687 2023-04-20 12:49:32.000000 anutils-0.4.1/src/anutils/scutils/utils.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     9029 2023-04-23 04:03:59.000000 anutils-0.4.1/src/anutils/utils.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils.egg-info/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2164 2023-04-27 06:46:41.000000 anutils-0.4.1/src/anutils.egg-info/PKG-INFO
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1116 2023-04-27 06:46:41.000000 anutils-0.4.1/src/anutils.egg-info/SOURCES.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)        1 2023-04-27 06:46:41.000000 anutils-0.4.1/src/anutils.egg-info/dependency_links.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       57 2023-04-27 06:46:41.000000 anutils-0.4.1/src/anutils.egg-info/requires.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)        8 2023-04-27 06:46:41.000000 anutils-0.4.1/src/anutils.egg-info/top_level.txt
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/tests/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      581 2022-06-17 11:20:29.000000 anutils-0.4.1/tests/run_tests.py
```

### Comparing `anutils-0.4.0/.gitignore` & `anutils-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/README.md` & `anutils-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/setup.py` & `anutils-0.4.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from pypandoc import convert_file
     long_description = convert_file('README.md', 'rst')
 except:
     long_description = ''
 
 setup(
     name='anutils',
-    version='0.4.0',
+    version='0.4.1',
     license='MIT',
     author="Aaron Ning",
     author_email='aaronning98@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     
     # If any package contains *.r files, include them:
```

### Comparing `anutils-0.4.0/src/anutils/mlutils/mlutils.py` & `anutils-0.4.1/src/anutils/mlutils/mlutils.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/annotation.py` & `anutils-0.4.1/src/anutils/scutils/annotation.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/data/data.py` & `anutils-0.4.1/src/anutils/scutils/data/data.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/data/h5ad2mtx.py` & `anutils-0.4.1/src/anutils/scutils/data/h5ad2mtx.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/data/mtx2rds.R` & `anutils-0.4.1/src/anutils/scutils/data/mtx2rds.R`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/external/integration/harmony.py` & `anutils-0.4.1/src/anutils/scutils/external/integration/harmony.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/external/integration/harmony_matrix.R` & `anutils-0.4.1/src/anutils/scutils/external/integration/harmony_matrix.R`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/external/integration/seurat.R` & `anutils-0.4.1/src/anutils/scutils/external/integration/seurat.R`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/external/integration/seurat.py` & `anutils-0.4.1/src/anutils/scutils/external/integration/seurat.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/plotting.py` & `anutils-0.4.1/src/anutils/scutils/plotting.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/preprocessing.py` & `anutils-0.4.1/src/anutils/scutils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py` & `anutils-0.4.1/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/sc_cuda/scanpy_cuda.py` & `anutils-0.4.1/src/anutils/scutils/sc_cuda/scanpy_cuda.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/sc_cuda/scib_cuda.py` & `anutils-0.4.1/src/anutils/scutils/sc_cuda/scib_cuda.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/scutils/utils.py` & `anutils-0.4.1/src/anutils/scutils/utils.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils/utils.py` & `anutils-0.4.1/src/anutils/utils.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/src/anutils.egg-info/SOURCES.txt` & `anutils-0.4.1/src/anutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anutils-0.4.0/tests/run_tests.py` & `anutils-0.4.1/tests/run_tests.py`

 * *Files identical despite different names*


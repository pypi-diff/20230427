# Comparing `tmp/preshed-3.0.8.tar.gz` & `tmp/preshed-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preshed-3.0.8.tar", last modified: Fri Oct 14 14:44:52 2022, max compression
+gzip compressed data, was "preshed-4.0.0.tar", last modified: Thu Apr 27 13:54:33 2023, max compression
```

## Comparing `preshed-3.0.8.tar` & `preshed-4.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-14 14:44:52.370880 preshed-3.0.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     1106 2022-10-14 14:44:45.000000 preshed-3.0.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)       96 2022-10-14 14:44:45.000000 preshed-3.0.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     2109 2022-10-14 14:44:52.370880 preshed-3.0.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1077 2022-10-14 14:44:45.000000 preshed-3.0.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-14 14:44:52.370880 preshed-3.0.8/include/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-14 14:44:52.370880 preshed-3.0.8/include/msvc9/
--rw-r--r--   0 vsts      (1001) docker     (121)     8101 2022-10-14 14:44:45.000000 preshed-3.0.8/include/msvc9/stdint.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-14 14:44:52.370880 preshed-3.0.8/preshed/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (121)       21 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      262 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/about.py
--rw-r--r--   0 vsts      (1001) docker     (121)      657 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/bloom.pxd
--rw-r--r--   0 vsts      (1001) docker     (121)     4529 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/bloom.pyx
--rw-r--r--   0 vsts      (1001) docker     (121)      396 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/counter.pxd
--rw-r--r--   0 vsts      (1001) docker     (121)     6116 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/counter.pyx
--rw-r--r--   0 vsts      (1001) docker     (121)     1334 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/maps.pxd
--rw-r--r--   0 vsts      (1001) docker     (121)     8723 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/maps.pyx
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-14 14:44:52.370880 preshed-3.0.8/preshed/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1256 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/tests/test_bloom.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/tests/test_counter.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1404 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/tests/test_hashing.py
--rw-r--r--   0 vsts      (1001) docker     (121)      207 2022-10-14 14:44:45.000000 preshed-3.0.8/preshed/tests/test_pop.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-14 14:44:52.370880 preshed-3.0.8/preshed.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     2109 2022-10-14 14:44:52.000000 preshed-3.0.8/preshed.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      568 2022-10-14 14:44:52.000000 preshed-3.0.8/preshed.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-14 14:44:52.000000 preshed-3.0.8/preshed.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-14 14:44:52.000000 preshed-3.0.8/preshed.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       46 2022-10-14 14:44:52.000000 preshed-3.0.8/preshed.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-10-14 14:44:52.000000 preshed-3.0.8/preshed.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      168 2022-10-14 14:44:45.000000 preshed-3.0.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-10-14 14:44:52.370880 preshed-3.0.8/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4260 2022-10-14 14:44:45.000000 preshed-3.0.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 13:54:33.114960 preshed-4.0.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1106 2023-04-27 13:54:19.000000 preshed-4.0.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)       96 2023-04-27 13:54:19.000000 preshed-4.0.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     2061 2023-04-27 13:54:33.114960 preshed-4.0.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1029 2023-04-27 13:54:19.000000 preshed-4.0.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 13:54:33.110960 preshed-4.0.0/include/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 13:54:33.114960 preshed-4.0.0/include/msvc9/
+-rw-r--r--   0 vsts      (1001) docker     (122)     8101 2023-04-27 13:54:19.000000 preshed-4.0.0/include/msvc9/stdint.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 13:54:33.114960 preshed-4.0.0/preshed/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/about.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      301 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/bloom.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     8907 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/bloom.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      427 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/counter.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     6189 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/counter.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     1118 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/maps.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     8192 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/maps.pyx
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 13:54:33.114960 preshed-4.0.0/preshed/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2623 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/tests/test_bloom.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2000 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/tests/test_counter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1404 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/tests/test_hashing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      207 2023-04-27 13:54:19.000000 preshed-4.0.0/preshed/tests/test_pop.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 13:54:33.114960 preshed-4.0.0/preshed.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2061 2023-04-27 13:54:33.000000 preshed-4.0.0/preshed.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-04-27 13:54:33.000000 preshed-4.0.0/preshed.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-27 13:54:33.000000 preshed-4.0.0/preshed.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-27 13:54:32.000000 preshed-4.0.0/preshed.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       46 2023-04-27 13:54:33.000000 preshed-4.0.0/preshed.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        8 2023-04-27 13:54:33.000000 preshed-4.0.0/preshed.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      168 2023-04-27 13:54:19.000000 preshed-4.0.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-04-27 13:54:33.114960 preshed-4.0.0/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     4288 2023-04-27 13:54:19.000000 preshed-4.0.0/setup.py
```

### Comparing `preshed-3.0.8/LICENSE` & `preshed-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `preshed-3.0.8/PKG-INFO` & `preshed-4.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preshed
-Version: 3.0.8
+Version: 4.0.0
 Summary: Cython hash table that trusts the keys are pre-hashed
 Home-page: https://github.com/explosion/preshed
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -25,13 +25,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # preshed: Cython Hash Table for Pre-Hashed Keys
 
-Simple but high performance Cython hash table mapping pre-randomized keys to `void*` values. Inspired by [Jeff Preshing](http://preshing.com/20130107/this-hash-table-is-faster-than-a-judy-array/).
+Simple but high performance Cython hash table mapping pre-randomized keys to
+`void*` values. Inspired by
+[Jeff Preshing](http://preshing.com/20130107/this-hash-table-is-faster-than-a-judy-array/).
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/3/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=3)
+[![tests](https://github.com/explosion/preshed/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/preshed/actions/workflows/tests.yml)
 [![pypi Version](https://img.shields.io/pypi/v/preshed.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/preshed)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/preshed.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/preshed)
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: preshed Version: 3.0.8 Summary: Cython hash table
+Metadata-Version: 2.1 Name: preshed Version: 4.0.0 Summary: Cython hash table
 that trusts the keys are pre-hashed Home-page: https://github.com/explosion/
 preshed Author: Explosion Author-email: contact@explosion.ai License: MIT
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: Programming Language :: Cython Classifier:
@@ -11,18 +11,17 @@
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE [https://explosion.ai/assets/img/
 logo.svg] # preshed: Cython Hash Table for Pre-Hashed Keys Simple but high
 performance Cython hash table mapping pre-randomized keys to `void*` values.
 Inspired by [Jeff Preshing](http://preshing.com/20130107/this-hash-table-is-
-faster-than-a-judy-array/). [![Azure Pipelines](https://img.shields.io/azure-
-devops/build/explosion-ai/public/3/master.svg?logo=azure-pipelines&style=flat-
-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=3) [!
-[pypi Version](https://img.shields.io/pypi/v/preshed.svg?style=flat-
-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/preshed) [!
-[conda Version](https://img.shields.io/conda/vn/conda-forge/
-preshed.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://
-anaconda.org/conda-forge/preshed) [![Python wheels](https://img.shields.io/
-badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-
+faster-than-a-judy-array/). [![tests](https://github.com/explosion/preshed/
+actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/preshed/
+actions/workflows/tests.yml) [![pypi Version](https://img.shields.io/pypi/v/
+preshed.svg?style=flat-square&logo=pypi&logoColor=white)](https://
+pypi.python.org/pypi/preshed) [![conda Version](https://img.shields.io/conda/
+vn/conda-forge/preshed.svg?style=flat-square&logo=conda-forge&logoColor=white)]
+(https://anaconda.org/conda-forge/preshed) [![Python wheels](https://
+img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-
 square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/
 releases)
```

### Comparing `preshed-3.0.8/README.md` & `preshed-4.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # preshed: Cython Hash Table for Pre-Hashed Keys
 
-Simple but high performance Cython hash table mapping pre-randomized keys to `void*` values. Inspired by [Jeff Preshing](http://preshing.com/20130107/this-hash-table-is-faster-than-a-judy-array/).
+Simple but high performance Cython hash table mapping pre-randomized keys to
+`void*` values. Inspired by
+[Jeff Preshing](http://preshing.com/20130107/this-hash-table-is-faster-than-a-judy-array/).
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/3/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=3)
+[![tests](https://github.com/explosion/preshed/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/preshed/actions/workflows/tests.yml)
 [![pypi Version](https://img.shields.io/pypi/v/preshed.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/preshed)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/preshed.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/preshed)
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 [https://explosion.ai/assets/img/logo.svg] # preshed: Cython Hash Table for
 Pre-Hashed Keys Simple but high performance Cython hash table mapping pre-
 randomized keys to `void*` values. Inspired by [Jeff Preshing](http://
-preshing.com/20130107/this-hash-table-is-faster-than-a-judy-array/). [![Azure
-Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/3/
-master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/
-explosion-ai/public/_build?definitionId=3) [![pypi Version](https://
-img.shields.io/pypi/v/preshed.svg?style=flat-square&logo=pypi&logoColor=white)]
-(https://pypi.python.org/pypi/preshed) [![conda Version](https://
-img.shields.io/conda/vn/conda-forge/preshed.svg?style=flat-square&logo=conda-
-forge&logoColor=white)](https://anaconda.org/conda-forge/preshed) [![Python
-wheels](https://img.shields.io/badge/wheels-%E2%9C%93-
-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://
-github.com/explosion/wheelwright/releases)
+preshing.com/20130107/this-hash-table-is-faster-than-a-judy-array/). [![tests]
+(https://github.com/explosion/preshed/actions/workflows/tests.yml/badge.svg)]
+(https://github.com/explosion/preshed/actions/workflows/tests.yml) [![pypi
+Version](https://img.shields.io/pypi/v/preshed.svg?style=flat-
+square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/preshed) [!
+[conda Version](https://img.shields.io/conda/vn/conda-forge/
+preshed.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://
+anaconda.org/conda-forge/preshed) [![Python wheels](https://img.shields.io/
+badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-
+square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/
+releases)
```

### Comparing `preshed-3.0.8/include/msvc9/stdint.h` & `preshed-4.0.0/include/msvc9/stdint.h`

 * *Files identical despite different names*

### Comparing `preshed-3.0.8/preshed/counter.pyx` & `preshed-4.0.0/preshed/counter.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 """Count occurrences of uint64-valued keys."""
 from __future__ import division
 cimport cython
+from cython.operator cimport dereference as deref
 from libc.math cimport log, exp, sqrt
+from libcpp.memory cimport make_unique
 
 
 cdef class PreshCounter:
     def __init__(self, initial_size=8):
         assert initial_size != 0
         assert initial_size & (initial_size - 1) == 0
-        self.mem = Pool()
-        self.c_map = <MapStruct*>self.mem.alloc(1, sizeof(MapStruct))
-        map_init(self.mem, self.c_map, initial_size)
+        self.c_map = make_unique[MapStruct]()
+        map_init(self.c_map.get(), initial_size)
         self.smoother = None
         self.total = 0
 
     property length:
         def __get__(self):
-            return self.c_map.length
+            return deref(self.c_map).cells.size()
 
     def __len__(self):
-        return self.c_map.length
+        return deref(self.c_map).cells.size()
 
     def __iter__(self):
         cdef int i = 0
         cdef key_t key
         cdef void* value
-        while map_iter(self.c_map, &i, &key, &value):
+        while map_iter(self.c_map.get(), &i, &key, &value):
             yield key, <size_t>value
 
     def __getitem__(self, key_t key):
-        return <count_t>map_get(self.c_map, key)
+        return <count_t>map_get(self.c_map.get(), key)
 
     cpdef int inc(self, key_t key, count_t inc) except -1:
-        cdef count_t c = <count_t>map_get(self.c_map, key)
+        cdef count_t c = <count_t>map_get(self.c_map.get(), key)
         c += inc
-        map_set(self.mem, self.c_map, key, <void*>c)
+        map_set(self.c_map.get(), key, <void*>c)
         self.total += inc
         return c
 
     def prob(self, key_t key):
         cdef GaleSmoother smoother
-        cdef void* value = map_get(self.c_map, key)
+        cdef void* value = map_get(self.c_map.get(), key)
         if self.smoother is not None:
             smoother = self.smoother
             r_star = self.smoother(<count_t>value)
             return r_star / self.smoother.total
         elif value == NULL:
             return 0
         else:
@@ -77,15 +78,15 @@
         self.mem = Pool()
 
         cdef double[2] mb
 
         cdef int n_counts = 0
         for _ in count_counts:
             n_counts += 1
-        sorted_r = <count_t*>count_counts.mem.alloc(n_counts, sizeof(count_t))
+        sorted_r = <count_t*>self.mem.alloc(n_counts, sizeof(count_t))
         self.Nr = <count_t*>self.mem.alloc(n_counts, sizeof(count_t))
         for i, (count, count_count) in enumerate(sorted(count_counts)):
             sorted_r[i] = count
             self.Nr[i] = count_count
 
         _fit_loglinear_model(mb, sorted_r, self.Nr, n_counts)
```

### Comparing `preshed-3.0.8/preshed/maps.pxd` & `preshed-4.0.0/preshed/maps.pxd`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from libc.stdint cimport uint64_t
-from cymem.cymem cimport Pool
+from libcpp.memory cimport unique_ptr
+from libcpp.vector cimport vector
 
 
 ctypedef uint64_t key_t
 
 
 cdef struct Cell:
     key_t key
@@ -12,48 +13,37 @@
 
 cdef struct Result:
     int found
     void* value
 
 
 cdef struct MapStruct:
-    Cell* cells
+    vector[Cell] cells
     void* value_for_empty_key
     void* value_for_del_key
-    key_t length
     key_t filled
     bint is_empty_key_set
     bint is_del_key_set
 
 
 cdef void* map_bulk_get(const MapStruct* map_, const key_t* keys, void** values,
                         int n) nogil
 
 
 cdef Result map_get_unless_missing(const MapStruct* map_, const key_t key) nogil
 
 cdef void* map_get(const MapStruct* map_, const key_t key) nogil
 
-cdef void map_set(Pool mem, MapStruct* map_, key_t key, void* value) except *
+cdef void map_set(MapStruct* map_, key_t key, void* value) except *
 
-cdef void map_init(Pool mem, MapStruct* pmap, size_t length) except *
+cdef void map_init(MapStruct* pmap, size_t length) except *
 
 cdef bint map_iter(const MapStruct* map_, int* i, key_t* key, void** value) nogil
 
 cdef void* map_clear(MapStruct* map_, const key_t key) nogil
 
 
 cdef class PreshMap:
-    cdef MapStruct* c_map
-    cdef Pool mem
+    cdef unique_ptr[MapStruct] c_map
 
     cdef inline void* get(self, key_t key) nogil
     cdef void set(self, key_t key, void* value) except *
-
-
-cdef class PreshMapArray:
-    cdef Pool mem
-    cdef MapStruct* maps
-    cdef size_t length
-
-    cdef inline void* get(self, size_t i, key_t key) nogil
-    cdef void set(self, size_t i, key_t key, void* value) except *
```

### Comparing `preshed-3.0.8/preshed/maps.pyx` & `preshed-4.0.0/preshed/maps.pyx`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # cython: infer_types=True
 # cython: cdivision=True
 #
 cimport cython
+from cython.operator import dereference as deref
+from libcpp.memory cimport make_unique
 
 
 DEF EMPTY_KEY = 0
 DEF DELETED_KEY = 1
 
 
+# Note: will not be needed with Cython 3.
+cdef extern from "<utility>" namespace "std" nogil:
+    void swap[T](T& a, T& b)
+
+
 cdef class PreshMap:
     """Hash map that assumes keys come pre-hashed. Maps uint64_t --> uint64_t.
     Uses open addressing with linear probing.
 
     Usage
         map = PreshMap() # Create a table
         map = PreshMap(initial_size=1024) # Create with initial size (efficiency)
@@ -25,142 +32,122 @@
         if initial_size == 0:
             initial_size = 8
         if initial_size & (initial_size - 1) != 0:
             power = 1
             while power < initial_size:
                 power *= 2
             initial_size = power
-        self.mem = Pool()
-        self.c_map = <MapStruct*>self.mem.alloc(1, sizeof(MapStruct))
-        map_init(self.mem, self.c_map, initial_size)
+        self.c_map = make_unique[MapStruct]()
+        map_init(self.c_map.get(), initial_size)
 
     property capacity:
         def __get__(self):
-            return self.c_map.length
+            return deref(self.c_map).cells.size()
 
     def items(self):
         cdef key_t key
         cdef void* value
         cdef int i = 0
-        while map_iter(self.c_map, &i, &key, &value):
+        while map_iter(self.c_map.get(), &i, &key, &value):
             yield key, <size_t>value
 
     def keys(self):
         for key, _ in self.items():
             yield key
 
     def values(self):
         for _, value in self.items():
             yield value
 
     def pop(self, key_t key, default=None):
-        cdef Result result = map_get_unless_missing(self.c_map, key)
-        map_clear(self.c_map, key)
+        cdef Result result = map_get_unless_missing(self.c_map.get(), key)
+        map_clear(self.c_map.get(), key)
         if result.found:
             return <size_t>result.value
         else:
             return default
 
     def __getitem__(self, key_t key):
-        cdef Result result = map_get_unless_missing(self.c_map, key)
+        cdef Result result = map_get_unless_missing(self.c_map.get(), key)
         if result.found:
             return <size_t>result.value
         else:
             return None
 
     def __setitem__(self, key_t key, size_t value):
-        map_set(self.mem, self.c_map, key, <void*>value)
+        map_set(self.c_map.get(), key, <void*>value)
 
     def __delitem__(self, key_t key):
-        map_clear(self.c_map, key)
+        map_clear(self.c_map.get(), key)
 
     def __len__(self):
-        return self.c_map.filled
+        return deref(self.c_map).filled
 
     def __contains__(self, key_t key):
-        cdef Result result = map_get_unless_missing(self.c_map, key)
+        cdef Result result = map_get_unless_missing(self.c_map.get(), key)
         return True if result.found else False
 
     def __iter__(self):
         for key in self.keys():
             yield key
 
     cdef inline void* get(self, key_t key) nogil:
-        return map_get(self.c_map, key)
+        return map_get(self.c_map.get(), key)
 
     cdef void set(self, key_t key, void* value) except *:
-        map_set(self.mem, self.c_map, key, <void*>value)
-
-
-cdef class PreshMapArray:
-    """An array of hash tables that assume keys come pre-hashed.  Each table
-    uses open addressing with linear probing.
-    """
-    def __init__(self, size_t length, size_t initial_size=8):
-        self.mem = Pool()
-        self.length = length
-        self.maps = <MapStruct*>self.mem.alloc(length, sizeof(MapStruct))
-        for i in range(length):
-            map_init(self.mem, &self.maps[i], initial_size)
-
-    cdef inline void* get(self, size_t i, key_t key) nogil:
-        return map_get(&self.maps[i], key)
-
-    cdef void set(self, size_t i, key_t key, void* value) except *:
-        map_set(self.mem, &self.maps[i], key, <void*>value)
+        map_set(self.c_map.get(), key, <void*>value)
 
 
-cdef void map_init(Pool mem, MapStruct* map_, size_t length) except *:
-    map_.length = length
+cdef void map_init(MapStruct* map_, size_t length) except *:
     map_.filled = 0
-    map_.cells = <Cell*>mem.alloc(length, sizeof(Cell))
+    map_.cells.resize(length)
 
 
-cdef void map_set(Pool mem, MapStruct* map_, key_t key, void* value) except *:
-    cdef Cell* cell
+cdef void map_set(MapStruct* map_, key_t key, void* value) except *:
+    cdef vector[Cell].iterator cell
     if key == EMPTY_KEY:
         map_.value_for_empty_key = value
         map_.is_empty_key_set = True
     elif key == DELETED_KEY:
         map_.value_for_del_key = value
         map_.is_del_key_set = True
     else:
-        cell = _find_cell_for_insertion(map_.cells, map_.length, key)
-        if cell.key == EMPTY_KEY:
+        cell = _find_cell_for_insertion(&map_.cells, key)
+        if deref(cell).key == EMPTY_KEY:
             map_.filled += 1
-        cell.key = key
-        cell.value = value
-        if (map_.filled + 1) * 5 >= (map_.length * 3):
-            _resize(mem, map_)
+        deref(cell).key = key
+        deref(cell).value = value
+        if (map_.filled + 1) * 5 >= (map_.cells.size() * 3):
+            _resize(map_)
 
 
 cdef void* map_get(const MapStruct* map_, const key_t key) nogil:
     if key == EMPTY_KEY:
         return map_.value_for_empty_key
     elif key == DELETED_KEY:
         return map_.value_for_del_key
-    cdef Cell* cell = _find_cell(map_.cells, map_.length, key)
+    cdef Cell cell = _find_cell(map_.cells, key)
     return cell.value
 
 
 cdef Result map_get_unless_missing(const MapStruct* map_, const key_t key) nogil:
     cdef Result result
-    cdef Cell* cell
+    cdef Cell cell
     result.found = 0
     result.value = NULL
     if key == EMPTY_KEY:
         if map_.is_empty_key_set:
             result.found = 1
             result.value = map_.value_for_empty_key
     elif key == DELETED_KEY:
         if map_.is_del_key_set:
             result.found = 1
             result.value = map_.value_for_del_key
     else:
-        cell = _find_cell(map_.cells, map_.length, key)
+        cell = _find_cell(map_.cells, key)
         if cell.key == key:
             result.found = 1
             result.value = cell.value
     return result
 
 
 cdef void* map_clear(MapStruct* map_, const key_t key) nogil:
@@ -169,15 +156,15 @@
         map_.is_empty_key_set = False
         return value
     elif key == DELETED_KEY:
         value = map_.value_for_del_key if map_.is_del_key_set else NULL
         map_.is_del_key_set = False
         return value
     else:
-        cell = _find_cell(map_.cells, map_.length, key)
+        cell = _find_cell(map_.cells, key)
         cell.key = DELETED_KEY
         # We shouldn't decrement the "filled" value here, as we're not actually
         # making "empty" values -- deleted values aren't quite the same.
         # Instead if we manage to insert into a deleted slot, we don't increment
         # the fill rate.
         return cell.value
 
@@ -190,76 +177,72 @@
 
 
 cdef bint map_iter(const MapStruct* map_, int* i, key_t* key, void** value) nogil:
     '''Iterate over the filled items, setting the current place in i, and the
     key and value.  Return False when iteration finishes.
     '''
     cdef const Cell* cell
-    while i[0] < map_.length:
+    while i[0] < map_.cells.size():
         cell = &map_.cells[i[0]]
         i[0] += 1
         if cell[0].key != EMPTY_KEY and cell[0].key != DELETED_KEY:
             key[0] = cell[0].key
             value[0] = cell[0].value
             return True
     # Remember to check for cells keyed by the special empty and deleted keys
-    if i[0] == map_.length:
+    if i[0] == map_.cells.size():
         i[0] += 1
         if map_.is_empty_key_set:
             key[0] = EMPTY_KEY
             value[0] = map_.value_for_empty_key
             return True
-    if i[0] == map_.length + 1:
+    if i[0] == map_.cells.size() + 1:
         i[0] += 1
         if map_.is_del_key_set:
             key[0] = DELETED_KEY
             value[0] = map_.value_for_del_key
             return True
     return False
 
 
 @cython.cdivision
-cdef inline Cell* _find_cell(Cell* cells, const key_t size, const key_t key) nogil:
+cdef inline Cell _find_cell(const vector[Cell]& cells, const key_t key) nogil:
     # Modulo for powers-of-two via bitwise &
-    cdef key_t i = (key & (size - 1))
+    cdef key_t i = (key & (cells.size() - 1))
     while cells[i].key != EMPTY_KEY and cells[i].key != key:
-        i = (i + 1) & (size - 1)
-    return &cells[i]
+        i = (i + 1) & (cells.size() - 1)
+    return cells[i]
 
 
 @cython.cdivision
-cdef inline Cell* _find_cell_for_insertion(Cell* cells, const key_t size, const key_t key) nogil:
+cdef inline vector[Cell].iterator _find_cell_for_insertion(vector[Cell]* cells, const key_t key) nogil:
     """Find the correct cell to insert a value, which could be a previously
     deleted cell. If we cross a deleted cell and the key is in the table, we
     mark the later cell as deleted, and return the earlier one."""
-    cdef Cell* deleted = NULL
+    cdef vector[Cell].iterator deleted = cells.end()
     # Modulo for powers-of-two via bitwise &
-    cdef key_t i = (key & (size - 1))
-    while cells[i].key != EMPTY_KEY and cells[i].key != key:
-        if cells[i].key == DELETED_KEY:
-            deleted = &cells[i]
-        i = (i + 1) & (size - 1)
-    if deleted is not NULL:
-        if cells[i].key == key:
+    cdef key_t i = (key & (cells.size() - 1))
+    while deref(cells)[i].key != EMPTY_KEY and deref(cells)[i].key != key:
+        if deref(cells)[i].key == DELETED_KEY:
+            deleted = cells.begin() + i
+        i = (i + 1) & (cells.size() - 1)
+    if deleted != cells.end():
+        if deref(deleted).key == key:
             # We need to ensure we don't end up with the key in the table twice.
             # If we're using a deleted cell and we also have the key, we mark
             # the later cell as deleted.
-            cells[i].key = DELETED_KEY
+            deref(cells)[i].key = DELETED_KEY
         return deleted
-    return &cells[i]
+    return cells.begin() + i
 
 
-cdef void _resize(Pool mem, MapStruct* map_) except *:
-    cdef size_t new_size = map_.length * 2
-    cdef Cell* old_cells = map_.cells
-    cdef size_t old_size = map_.length
+cdef void _resize(MapStruct* map_) except *:
+    # Allocate memory for new cells and swap out.
+    cdef vector[Cell] old_cells = vector[Cell](map_.cells.size() * 2)
+    swap(old_cells, map_.cells)
 
-    map_.length = new_size
     map_.filled = 0
-    map_.cells = <Cell*>mem.alloc(new_size, sizeof(Cell))
-    
+
     cdef size_t i
-    cdef size_t slot
-    for i in range(old_size):
+    for i in range(old_cells.size()):
         if old_cells[i].key != EMPTY_KEY and old_cells[i].key != DELETED_KEY:
-            map_set(mem, map_, old_cells[i].key, old_cells[i].value)
-    mem.free(old_cells)
+            map_set(map_, old_cells[i].key, old_cells[i].value)
```

### Comparing `preshed-3.0.8/preshed/tests/test_counter.py` & `preshed-4.0.0/preshed/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `preshed-3.0.8/preshed/tests/test_hashing.py` & `preshed-4.0.0/preshed/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `preshed-3.0.8/preshed.egg-info/PKG-INFO` & `preshed-4.0.0/preshed.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preshed
-Version: 3.0.8
+Version: 4.0.0
 Summary: Cython hash table that trusts the keys are pre-hashed
 Home-page: https://github.com/explosion/preshed
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -25,13 +25,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # preshed: Cython Hash Table for Pre-Hashed Keys
 
-Simple but high performance Cython hash table mapping pre-randomized keys to `void*` values. Inspired by [Jeff Preshing](http://preshing.com/20130107/this-hash-table-is-faster-than-a-judy-array/).
+Simple but high performance Cython hash table mapping pre-randomized keys to
+`void*` values. Inspired by
+[Jeff Preshing](http://preshing.com/20130107/this-hash-table-is-faster-than-a-judy-array/).
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/3/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=3)
+[![tests](https://github.com/explosion/preshed/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/preshed/actions/workflows/tests.yml)
 [![pypi Version](https://img.shields.io/pypi/v/preshed.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/preshed)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/preshed.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/preshed)
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: preshed Version: 3.0.8 Summary: Cython hash table
+Metadata-Version: 2.1 Name: preshed Version: 4.0.0 Summary: Cython hash table
 that trusts the keys are pre-hashed Home-page: https://github.com/explosion/
 preshed Author: Explosion Author-email: contact@explosion.ai License: MIT
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: Programming Language :: Cython Classifier:
@@ -11,18 +11,17 @@
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE [https://explosion.ai/assets/img/
 logo.svg] # preshed: Cython Hash Table for Pre-Hashed Keys Simple but high
 performance Cython hash table mapping pre-randomized keys to `void*` values.
 Inspired by [Jeff Preshing](http://preshing.com/20130107/this-hash-table-is-
-faster-than-a-judy-array/). [![Azure Pipelines](https://img.shields.io/azure-
-devops/build/explosion-ai/public/3/master.svg?logo=azure-pipelines&style=flat-
-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=3) [!
-[pypi Version](https://img.shields.io/pypi/v/preshed.svg?style=flat-
-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/preshed) [!
-[conda Version](https://img.shields.io/conda/vn/conda-forge/
-preshed.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://
-anaconda.org/conda-forge/preshed) [![Python wheels](https://img.shields.io/
-badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-
+faster-than-a-judy-array/). [![tests](https://github.com/explosion/preshed/
+actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/preshed/
+actions/workflows/tests.yml) [![pypi Version](https://img.shields.io/pypi/v/
+preshed.svg?style=flat-square&logo=pypi&logoColor=white)](https://
+pypi.python.org/pypi/preshed) [![conda Version](https://img.shields.io/conda/
+vn/conda-forge/preshed.svg?style=flat-square&logo=conda-forge&logoColor=white)]
+(https://anaconda.org/conda-forge/preshed) [![Python wheels](https://
+img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-
 square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/
 releases)
```

### Comparing `preshed-3.0.8/preshed.egg-info/SOURCES.txt` & `preshed-4.0.0/preshed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preshed-3.0.8/setup.py` & `preshed-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 PACKAGES = ["preshed", "preshed.tests"]
 MOD_NAMES = ["preshed.maps", "preshed.counter", "preshed.bloom"]
 
 
 # By subclassing build_extensions we have the actual compiler that will be used which is really known only after finalize_options
 # http://stackoverflow.com/questions/724664/python-distutils-how-to-get-a-compiler-that-is-going-to-be-used
 compile_options = {
-    "msvc": ["/Ox", "/EHsc"],
-    "other": ["-O3", "-Wno-strict-prototypes", "-Wno-unused-function"],
+    "msvc": ["/Ox", "/EHsc", "/std:c++14"],
+    "other": ["-O3", "-Wno-strict-prototypes", "-Wno-unused-function", "-std=c++14"],
 }
 link_options = {"msvc": [], "other": []}
 
 
 class build_ext_options:
     def build_options(self):
         for e in self.extensions:
```


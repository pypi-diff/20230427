# Comparing `tmp/yogger-0.0.6.tar.gz` & `tmp/yogger-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yogger-0.0.6.tar", last modified: Thu Apr 27 02:46:51 2023, max compression
+gzip compressed data, was "yogger-0.0.6a0.tar", last modified: Thu Apr 27 03:08:03 2023, max compression
```

## Comparing `yogger-0.0.6.tar` & `yogger-0.0.6a0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 02:46:51.903638 yogger-0.0.6/
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    35149 2023-02-14 07:17:38.000000 yogger-0.0.6/LICENSE
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    52817 2023-04-27 02:46:51.903638 yogger-0.0.6/PKG-INFO
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    10950 2023-04-27 02:46:09.000000 yogger-0.0.6/README.md
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     4192 2023-03-12 04:35:06.000000 yogger-0.0.6/pyproject.toml
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       38 2023-04-27 02:46:51.903638 yogger-0.0.6/setup.cfg
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      566 2023-02-23 04:23:13.000000 yogger-0.0.6/setup.py
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 02:46:51.903638 yogger-0.0.6/src/
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 02:46:51.903638 yogger-0.0.6/src/yogger/
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      284 2023-03-15 01:09:39.000000 yogger-0.0.6/src/yogger/__init__.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    11323 2023-03-15 01:09:39.000000 yogger-0.0.6/src/yogger/base.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      540 2023-03-15 01:09:39.000000 yogger-0.0.6/src/yogger/compat.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      751 2023-03-15 01:09:39.000000 yogger-0.0.6/src/yogger/constants.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     8369 2023-04-27 02:46:03.000000 yogger-0.0.6/src/yogger/pformat.py
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 02:46:51.903638 yogger-0.0.6/src/yogger.egg-info/
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    52817 2023-04-27 02:46:51.000000 yogger-0.0.6/src/yogger.egg-info/PKG-INFO
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      341 2023-04-27 02:46:51.000000 yogger-0.0.6/src/yogger.egg-info/SOURCES.txt
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)        1 2023-04-27 02:46:51.000000 yogger-0.0.6/src/yogger.egg-info/dependency_links.txt
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       37 2023-04-27 02:46:51.000000 yogger-0.0.6/src/yogger.egg-info/requires.txt
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)        7 2023-04-27 02:46:51.000000 yogger-0.0.6/src/yogger.egg-info/top_level.txt
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 02:46:51.903638 yogger-0.0.6/tests/
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    16096 2023-03-15 01:09:39.000000 yogger-0.0.6/tests/test_pformat.py
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 03:08:03.246879 yogger-0.0.6a0/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    35149 2023-02-14 07:17:38.000000 yogger-0.0.6a0/LICENSE
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    52835 2023-04-27 03:08:03.246879 yogger-0.0.6a0/PKG-INFO
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    10966 2023-04-27 03:07:47.000000 yogger-0.0.6a0/README.md
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     4192 2023-03-12 04:35:06.000000 yogger-0.0.6a0/pyproject.toml
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       38 2023-04-27 03:08:03.246879 yogger-0.0.6a0/setup.cfg
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      566 2023-02-23 04:23:13.000000 yogger-0.0.6a0/setup.py
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 03:08:03.246879 yogger-0.0.6a0/src/
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 03:08:03.246879 yogger-0.0.6a0/src/yogger/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      285 2023-04-27 03:07:47.000000 yogger-0.0.6a0/src/yogger/__init__.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    11323 2023-04-27 03:07:47.000000 yogger-0.0.6a0/src/yogger/base.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      540 2023-04-27 03:07:47.000000 yogger-0.0.6a0/src/yogger/compat.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      751 2023-04-27 03:07:47.000000 yogger-0.0.6a0/src/yogger/constants.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     8369 2023-04-27 03:07:47.000000 yogger-0.0.6a0/src/yogger/pformat.py
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 03:08:03.246879 yogger-0.0.6a0/src/yogger.egg-info/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    52835 2023-04-27 03:08:03.000000 yogger-0.0.6a0/src/yogger.egg-info/PKG-INFO
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      341 2023-04-27 03:08:03.000000 yogger-0.0.6a0/src/yogger.egg-info/SOURCES.txt
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)        1 2023-04-27 03:08:03.000000 yogger-0.0.6a0/src/yogger.egg-info/dependency_links.txt
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       37 2023-04-27 03:08:03.000000 yogger-0.0.6a0/src/yogger.egg-info/requires.txt
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)        7 2023-04-27 03:08:03.000000 yogger-0.0.6a0/src/yogger.egg-info/top_level.txt
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 03:08:03.246879 yogger-0.0.6a0/tests/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    16096 2023-04-27 03:07:47.000000 yogger-0.0.6a0/tests/test_pformat.py
```

### Comparing `yogger-0.0.6/LICENSE` & `yogger-0.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `yogger-0.0.6/PKG-INFO` & `yogger-0.0.6a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yogger
-Version: 0.0.6
+Version: 0.0.6a0
 Summary: Minimal logging setup with utilities to represent interpreter stacks.
 Author-email: The Phosmic Development Team <dev@phosmic.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -743,18 +743,18 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see https://www.gnu.org/licenses/.
 
 ---
 
-[Requirements](#requirements)
-[Installing](#installing)
-[Usage](#usage)
-[Library](#library)
+-   [Requirements](#requirements)
+-   [Installing](#installing)
+-   [Usage](#usage)
+-   [Library](#library)
 
 ## Installing
 
 Most stable version from [**PyPi**](https://pypi.org/project/yogger/):
 
 [![PyPI](https://img.shields.io/pypi/v/yogger?style=flat-square)](https://pypi.org/project/yogger/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yogger?style=flat-square)](https://pypi.org/project/yogger/)
```

### Comparing `yogger-0.0.6/README.md` & `yogger-0.0.6a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see https://www.gnu.org/licenses/.
 
 ---
 
-[Requirements](#requirements)
-[Installing](#installing)
-[Usage](#usage)
-[Library](#library)
+-   [Requirements](#requirements)
+-   [Installing](#installing)
+-   [Usage](#usage)
+-   [Library](#library)
 
 ## Installing
 
 Most stable version from [**PyPi**](https://pypi.org/project/yogger/):
 
 [![PyPI](https://img.shields.io/pypi/v/yogger?style=flat-square)](https://pypi.org/project/yogger/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yogger?style=flat-square)](https://pypi.org/project/yogger/)
```

### Comparing `yogger-0.0.6/pyproject.toml` & `yogger-0.0.6a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yogger-0.0.6/setup.py` & `yogger-0.0.6a0/setup.py`

 * *Files identical despite different names*

### Comparing `yogger-0.0.6/src/yogger/base.py` & `yogger-0.0.6a0/src/yogger/base.py`

 * *Files identical despite different names*

### Comparing `yogger-0.0.6/src/yogger/compat.py` & `yogger-0.0.6a0/src/yogger/compat.py`

 * *Files identical despite different names*

### Comparing `yogger-0.0.6/src/yogger/constants.py` & `yogger-0.0.6a0/src/yogger/constants.py`

 * *Files identical despite different names*

### Comparing `yogger-0.0.6/src/yogger/pformat.py` & `yogger-0.0.6a0/src/yogger/pformat.py`

 * *Files identical despite different names*

### Comparing `yogger-0.0.6/src/yogger.egg-info/PKG-INFO` & `yogger-0.0.6a0/src/yogger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yogger
-Version: 0.0.6
+Version: 0.0.6a0
 Summary: Minimal logging setup with utilities to represent interpreter stacks.
 Author-email: The Phosmic Development Team <dev@phosmic.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -743,18 +743,18 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see https://www.gnu.org/licenses/.
 
 ---
 
-[Requirements](#requirements)
-[Installing](#installing)
-[Usage](#usage)
-[Library](#library)
+-   [Requirements](#requirements)
+-   [Installing](#installing)
+-   [Usage](#usage)
+-   [Library](#library)
 
 ## Installing
 
 Most stable version from [**PyPi**](https://pypi.org/project/yogger/):
 
 [![PyPI](https://img.shields.io/pypi/v/yogger?style=flat-square)](https://pypi.org/project/yogger/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yogger?style=flat-square)](https://pypi.org/project/yogger/)
```

### Comparing `yogger-0.0.6/tests/test_pformat.py` & `yogger-0.0.6a0/tests/test_pformat.py`

 * *Files identical despite different names*


# Comparing `tmp/kaiju_files-2.0.1-py3-none-any.whl.zip` & `tmp/kaiju_files-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 15291 bytes, number of entries: 16
--rw-r--r--  2.0 unx      137 b- defN 23-Jan-24 14:24 kaiju_files/__init__.py
--rw-r--r--  2.0 unx    11909 b- defN 23-Jan-24 14:24 kaiju_files/abc.py
--rw-r--r--  2.0 unx     8657 b- defN 23-Jan-24 14:24 kaiju_files/converters.py
--rw-r--r--  2.0 unx      165 b- defN 23-Jan-24 14:24 kaiju_files/etc.py
--rw-r--r--  2.0 unx    10933 b- defN 23-Jan-24 14:24 kaiju_files/files.py
--rw-r--r--  2.0 unx       88 b- defN 23-Jan-24 14:24 kaiju_files/services.py
--rw-r--r--  2.0 unx     2423 b- defN 23-Jan-24 14:24 kaiju_files/tables.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-24 14:24 kaiju_files/tests/__init__.py
--rw-r--r--  2.0 unx      703 b- defN 23-Jan-24 14:24 kaiju_files/tests/fixtures.py
--rw-r--r--  2.0 unx     2376 b- defN 23-Jan-24 14:24 kaiju_files/tests/test_converters.py
--rw-r--r--  2.0 unx     1010 b- defN 23-Jan-24 14:24 kaiju_files/tests/test_files.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jan-24 14:25 kaiju_files-2.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2937 b- defN 23-Jan-24 14:25 kaiju_files-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-24 14:25 kaiju_files-2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jan-24 14:25 kaiju_files-2.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1299 b- defN 23-Jan-24 14:25 kaiju_files-2.0.1.dist-info/RECORD
-16 files, 43351 bytes uncompressed, 13149 bytes compressed:  69.7%
+Zip file size: 15294 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      137 b- defN 23-Apr-27 12:20 kaiju_files/__init__.py
+-rw-r--r--  2.0 unx    11909 b- defN 23-Apr-27 12:20 kaiju_files/abc.py
+-rw-r--r--  2.0 unx     8657 b- defN 23-Apr-27 12:20 kaiju_files/converters.py
+-rw-r--r--  2.0 unx      165 b- defN 23-Apr-27 12:20 kaiju_files/etc.py
+-rw-r--r--  2.0 unx    10933 b- defN 23-Apr-27 12:20 kaiju_files/files.py
+-rw-r--r--  2.0 unx       88 b- defN 23-Apr-27 12:20 kaiju_files/services.py
+-rw-r--r--  2.0 unx     2423 b- defN 23-Apr-27 12:20 kaiju_files/tables.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-27 12:20 kaiju_files/tests/__init__.py
+-rw-r--r--  2.0 unx      703 b- defN 23-Apr-27 12:20 kaiju_files/tests/fixtures.py
+-rw-r--r--  2.0 unx     2376 b- defN 23-Apr-27 12:20 kaiju_files/tests/test_converters.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-Apr-27 12:20 kaiju_files/tests/test_files.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Apr-27 12:20 kaiju_files-2.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2901 b- defN 23-Apr-27 12:20 kaiju_files-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 12:20 kaiju_files-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-27 12:20 kaiju_files-2.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1299 b- defN 23-Apr-27 12:20 kaiju_files-2.0.2.dist-info/RECORD
+16 files, 43315 bytes uncompressed, 13152 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: kaiju_files/tests/test_converters.py
 Comment: 
 
 Filename: kaiju_files/tests/test_files.py
 Comment: 
 
-Filename: kaiju_files-2.0.1.dist-info/LICENSE
+Filename: kaiju_files-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_files-2.0.1.dist-info/METADATA
+Filename: kaiju_files-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_files-2.0.1.dist-info/WHEEL
+Filename: kaiju_files-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_files-2.0.1.dist-info/top_level.txt
+Filename: kaiju_files-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_files-2.0.1.dist-info/RECORD
+Filename: kaiju_files-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_files/__init__.py

```diff
@@ -1,6 +1,6 @@
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
 __service_package__ = True
 
 from .services import *
```

## Comparing `kaiju_files-2.0.1.dist-info/LICENSE` & `kaiju_files-2.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_files-2.0.1.dist-info/METADATA` & `kaiju_files-2.0.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-files
-Version: 2.0.1
+Version: 2.0.2
 Summary: File management services.
 Home-page: https://gitlab.com/kaiju-python/kaiju-files
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,39 +14,39 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: aiofiles (==22.1.*)
-Requires-Dist: kaiju-tools (==2.0.*)
-Requires-Dist: kaiju-db (==2.0.*)
+Requires-Dist: aiofiles (>=23.1)
+Requires-Dist: kaiju-tools (<3,>=2)
+Requires-Dist: kaiju-db (<3,>=2)
 Provides-Extra: dev
-Requires-Dist: bump2version (==1.0.*) ; extra == 'dev'
-Requires-Dist: pyroma (==4.1) ; extra == 'dev'
-Requires-Dist: bandit (==1.7.*) ; extra == 'dev'
-Requires-Dist: black (==22.12.*) ; extra == 'dev'
-Requires-Dist: flake8 (==6.0.*) ; extra == 'dev'
+Requires-Dist: bump2version (>=1.0) ; extra == 'dev'
+Requires-Dist: pyroma (>=4.1) ; extra == 'dev'
+Requires-Dist: bandit (>=1.7) ; extra == 'dev'
+Requires-Dist: black (>=22.12) ; extra == 'dev'
+Requires-Dist: flake8 (>=6.0) ; extra == 'dev'
 Requires-Dist: pyproject-flake8 ; extra == 'dev'
-Requires-Dist: pre-commit (==2.21.*) ; extra == 'dev'
-Requires-Dist: pydocstyle (==6.2.*) ; extra == 'dev'
-Requires-Dist: setup-cfg-fmt (==2.2.*) ; extra == 'dev'
-Requires-Dist: restructuredtext-lint (==1.4.*) ; extra == 'dev'
-Requires-Dist: tox (==3.28.*) ; extra == 'dev'
-Requires-Dist: tox-pyenv (==1.1.*) ; extra == 'dev'
+Requires-Dist: pre-commit (>=3.1) ; extra == 'dev'
+Requires-Dist: pydocstyle (>=6.3) ; extra == 'dev'
+Requires-Dist: setup-cfg-fmt (>=2.2) ; extra == 'dev'
+Requires-Dist: restructuredtext-lint (>=1.4) ; extra == 'dev'
+Requires-Dist: tox (>=3.28) ; extra == 'dev'
+Requires-Dist: tox-pyenv (>=1.1) ; extra == 'dev'
+Requires-Dist: pip-tools (>=6.13) ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: pytest (==7.2.*) ; extra == 'test'
-Requires-Dist: pytest-asyncio (==0.20) ; extra == 'test'
-Requires-Dist: docker (==6.0) ; extra == 'test'
-Requires-Dist: pytest-timeout (==2.1.*) ; extra == 'test'
-Requires-Dist: pytest-aiohttp (==1.0.*) ; extra == 'test'
+Requires-Dist: pytest (>=7.2) ; extra == 'test'
+Requires-Dist: pytest-asyncio (>=0.20) ; extra == 'test'
+Requires-Dist: docker (>=6.0) ; extra == 'test'
+Requires-Dist: pytest-timeout (>=2.1) ; extra == 'test'
 
 
 .. image:: https://badge.fury.io/py/kaiju-files.svg
     :target: https://pypi.org/project/kaiju-files
     :alt: Latest package version
 
 .. image:: https://readthedocs.org/projects/kaiju-files/badge/?version=latest
```

## Comparing `kaiju_files-2.0.1.dist-info/RECORD` & `kaiju_files-2.0.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-kaiju_files/__init__.py,sha256=SuCFR5FfrRz0IUOe6x5DTZUh0jRNR0STbV7FML4fM4g,137
+kaiju_files/__init__.py,sha256=JdYCSMsnlNOsCarRRciHbB5VlzeUAfMPu3Nzxfhqvbo,137
 kaiju_files/abc.py,sha256=K-amb1JtYZVFJr2W4jVW52vAKQbOhG3shXCNdLtfXiM,11909
 kaiju_files/converters.py,sha256=eQ4k1e_r6yvwHrluyXUXHzMMkl14czWU-7cz389146A,8657
 kaiju_files/etc.py,sha256=qhzJlV_nc5mRYxD77jgQETFSWqUopmNC4vQOMQCn6JA,165
 kaiju_files/files.py,sha256=_EEKgxOY-Onhsyy_WJDzqS50fqFHAIUziJsHnB2V8jA,10933
 kaiju_files/services.py,sha256=cSTDGUa0_cr7mNNNv8CPY_aRj0wFzGAFctEAdK5rYTw,88
 kaiju_files/tables.py,sha256=oODR2hS1gA2awsUQjKmVntS93DZV-K8eqYJ9eA9Qb8M,2423
 kaiju_files/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kaiju_files/tests/fixtures.py,sha256=-tnA9XcaHHDUuP_CYGuRDxgTxonGOsuN-zKy15H8P_E,703
 kaiju_files/tests/test_converters.py,sha256=63Kucljf-tEONsE0Fe3X1OXYR5YyfW5mEpFq6P6hKnI,2376
 kaiju_files/tests/test_files.py,sha256=Q10dmfpa20ljFEFdI2R1E1_AWYb6n7SPCExPpT-wt3E,1010
-kaiju_files-2.0.1.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_files-2.0.1.dist-info/METADATA,sha256=q5KWzm3AUWQzm7mi5rKJBqJ14O2MgnGZuKapCyWhjKA,2937
-kaiju_files-2.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-kaiju_files-2.0.1.dist-info/top_level.txt,sha256=SnVfqkSRIWJ7yYfmROjUcTT19yK_rWaO5lMJkMnM8fM,12
-kaiju_files-2.0.1.dist-info/RECORD,,
+kaiju_files-2.0.2.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_files-2.0.2.dist-info/METADATA,sha256=DUQRCFBUdk4bPLkYiERee6getXTdk2WnwUfwpeAvHzI,2901
+kaiju_files-2.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_files-2.0.2.dist-info/top_level.txt,sha256=SnVfqkSRIWJ7yYfmROjUcTT19yK_rWaO5lMJkMnM8fM,12
+kaiju_files-2.0.2.dist-info/RECORD,,
```


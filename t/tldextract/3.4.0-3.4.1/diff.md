# Comparing `tmp/tldextract-3.4.0.tar.gz` & `tmp/tldextract-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldextract-3.4.0.tar", last modified: Tue Oct  4 20:21:16 2022, max compression
+gzip compressed data, was "tldextract-3.4.1.tar", last modified: Wed Apr 26 23:31:34 2023, max compression
```

## Comparing `tldextract-3.4.0.tar` & `tldextract-3.4.1.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-10-04 20:21:16.650571 tldextract-3.4.0/
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-10-04 20:21:16.641015 tldextract-3.4.0/.github/
--rw-r--r--   0 john       (501) staff       (20)       25 2022-06-05 23:30:19.000000 tldextract-3.4.0/.github/FUNDING.yml
--rw-r--r--   0 john       (501) staff       (20)      129 2022-05-03 19:53:33.000000 tldextract-3.4.0/.gitignore
--rw-r--r--   0 john       (501) staff       (20)      424 2022-05-03 19:53:33.000000 tldextract-3.4.0/.travis.yml
--rw-r--r--   0 john       (501) staff       (20)    12579 2022-10-04 20:20:45.000000 tldextract-3.4.0/CHANGELOG.md
--rw-r--r--   0 john       (501) staff       (20)     1522 2022-05-03 19:53:33.000000 tldextract-3.4.0/LICENSE
--rw-r--r--   0 john       (501) staff       (20)      116 2022-05-03 19:53:33.000000 tldextract-3.4.0/MANIFEST.in
--rw-r--r--   0 john       (501) staff       (20)     2125 2022-10-04 20:21:16.650842 tldextract-3.4.0/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)     9639 2022-10-04 20:01:32.000000 tldextract-3.4.0/README.md
--rw-r--r--   0 john       (501) staff       (20)       68 2022-05-03 19:53:33.000000 tldextract-3.4.0/conftest.py
--rw-r--r--   0 john       (501) staff       (20)    18121 2022-06-05 22:55:01.000000 tldextract-3.4.0/pylintrc
--rw-r--r--   0 john       (501) staff       (20)       37 2022-05-03 19:53:33.000000 tldextract-3.4.0/pytest.ini
--rw-r--r--   0 john       (501) staff       (20)      219 2022-10-04 20:21:16.651707 tldextract-3.4.0/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)     2691 2022-09-17 08:16:28.000000 tldextract-3.4.0/setup.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-10-04 20:21:16.643380 tldextract-3.4.0/tests/
--rw-r--r--   0 john       (501) staff       (20)        0 2021-01-11 20:42:27.000000 tldextract-3.4.0/tests/__init__.py
--rw-r--r--   0 john       (501) staff       (20)      783 2022-06-05 23:30:19.000000 tldextract-3.4.0/tests/cli_test.py
--rw-r--r--   0 john       (501) staff       (20)      428 2022-05-03 19:53:33.000000 tldextract-3.4.0/tests/conftest.py
--rw-r--r--   0 john       (501) staff       (20)     1935 2022-09-20 19:51:12.000000 tldextract-3.4.0/tests/custom_suffix_test.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-10-04 20:21:16.643759 tldextract-3.4.0/tests/fixtures/
--rw-r--r--   0 john       (501) staff       (20)       31 2021-01-11 20:42:27.000000 tldextract-3.4.0/tests/fixtures/fake_suffix_list_fixture.dat
--rw-r--r--   0 john       (501) staff       (20)      248 2022-06-05 23:30:19.000000 tldextract-3.4.0/tests/integration_test.py
--rw-r--r--   0 john       (501) staff       (20)    10760 2022-09-20 19:51:12.000000 tldextract-3.4.0/tests/main_test.py
--rw-r--r--   0 john       (501) staff       (20)     3419 2022-06-05 23:30:19.000000 tldextract-3.4.0/tests/test_cache.py
--rw-r--r--   0 john       (501) staff       (20)     1539 2022-09-17 08:16:28.000000 tldextract-3.4.0/tests/test_parallel.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-10-04 20:21:16.647682 tldextract-3.4.0/tldextract/
--rw-r--r--   0 john       (501) staff       (20)   240783 2022-06-05 23:30:19.000000 tldextract-3.4.0/tldextract/.tld_set_snapshot
--rw-r--r--   0 john       (501) staff       (20)      149 2022-05-03 19:53:33.000000 tldextract-3.4.0/tldextract/__init__.py
--rw-r--r--   0 john       (501) staff       (20)       90 2022-06-05 23:36:58.000000 tldextract-3.4.0/tldextract/__main__.py
--rw-r--r--   0 john       (501) staff       (20)      176 2022-10-04 20:21:16.000000 tldextract-3.4.0/tldextract/_version.py
--rw-r--r--   0 john       (501) staff       (20)     8712 2022-10-04 19:21:53.000000 tldextract-3.4.0/tldextract/cache.py
--rw-r--r--   0 john       (501) staff       (20)     2430 2022-09-20 19:51:12.000000 tldextract-3.4.0/tldextract/cli.py
--rw-r--r--   0 john       (501) staff       (20)        0 2022-05-03 19:53:33.000000 tldextract-3.4.0/tldextract/py.typed
--rw-r--r--   0 john       (501) staff       (20)     1182 2022-10-03 18:20:48.000000 tldextract-3.4.0/tldextract/remote.py
--rw-r--r--   0 john       (501) staff       (20)     3399 2022-10-03 18:40:04.000000 tldextract-3.4.0/tldextract/suffix_list.py
--rw-r--r--   0 john       (501) staff       (20)    14443 2022-10-03 18:30:43.000000 tldextract-3.4.0/tldextract/tldextract.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-10-04 20:21:16.650177 tldextract-3.4.0/tldextract.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     2125 2022-10-04 20:21:16.000000 tldextract-3.4.0/tldextract.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      792 2022-10-04 20:21:16.000000 tldextract-3.4.0/tldextract.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2022-10-04 20:21:16.000000 tldextract-3.4.0/tldextract.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       51 2022-10-04 20:21:16.000000 tldextract-3.4.0/tldextract.egg-info/entry_points.txt
--rw-r--r--   0 john       (501) staff       (20)       56 2022-10-04 20:21:16.000000 tldextract-3.4.0/tldextract.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)       11 2022-10-04 20:21:16.000000 tldextract-3.4.0/tldextract.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)      950 2022-06-05 23:36:58.000000 tldextract-3.4.0/tox.ini
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.373156 tldextract-3.4.1/
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.360626 tldextract-3.4.1/.github/
+-rw-r--r--   0 john       (501) staff       (20)       25 2022-06-01 21:35:53.000000 tldextract-3.4.1/.github/FUNDING.yml
+-rw-r--r--   0 john       (501) staff       (20)      129 2020-10-23 23:38:03.000000 tldextract-3.4.1/.gitignore
+-rw-r--r--   0 john       (501) staff       (20)      469 2023-04-26 23:28:14.000000 tldextract-3.4.1/.travis.yml
+-rw-r--r--   0 john       (501) staff       (20)    12995 2023-04-26 23:26:27.000000 tldextract-3.4.1/CHANGELOG.md
+-rw-r--r--   0 john       (501) staff       (20)     1522 2020-10-11 21:23:20.000000 tldextract-3.4.1/LICENSE
+-rw-r--r--   0 john       (501) staff       (20)      116 2022-04-01 00:16:04.000000 tldextract-3.4.1/MANIFEST.in
+-rw-r--r--   0 john       (501) staff       (20)     2177 2023-04-26 23:31:34.373349 tldextract-3.4.1/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)     9874 2023-04-26 23:08:06.000000 tldextract-3.4.1/README.md
+-rw-r--r--   0 john       (501) staff       (20)       68 2022-04-01 00:16:04.000000 tldextract-3.4.1/conftest.py
+-rw-r--r--   0 john       (501) staff       (20)       37 2022-04-01 00:16:04.000000 tldextract-3.4.1/pytest.ini
+-rw-r--r--   0 john       (501) staff       (20)      327 2023-04-26 23:31:34.373990 tldextract-3.4.1/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)     2769 2023-04-26 23:28:16.000000 tldextract-3.4.1/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.364137 tldextract-3.4.1/tests/
+-rw-r--r--   0 john       (501) staff       (20)        0 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)      783 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/cli_test.py
+-rw-r--r--   0 john       (501) staff       (20)      428 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/conftest.py
+-rw-r--r--   0 john       (501) staff       (20)     1935 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/custom_suffix_test.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.364951 tldextract-3.4.1/tests/fixtures/
+-rw-r--r--   0 john       (501) staff       (20)       31 2020-10-11 21:23:20.000000 tldextract-3.4.1/tests/fixtures/fake_suffix_list_fixture.dat
+-rw-r--r--   0 john       (501) staff       (20)      248 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/integration_test.py
+-rw-r--r--   0 john       (501) staff       (20)    10790 2023-04-10 01:08:44.000000 tldextract-3.4.1/tests/main_test.py
+-rw-r--r--   0 john       (501) staff       (20)     3419 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/test_cache.py
+-rw-r--r--   0 john       (501) staff       (20)     1539 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/test_parallel.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.370515 tldextract-3.4.1/tldextract/
+-rw-r--r--   0 john       (501) staff       (20)   238022 2023-04-26 18:51:17.000000 tldextract-3.4.1/tldextract/.tld_set_snapshot
+-rw-r--r--   0 john       (501) staff       (20)      216 2023-04-10 01:08:44.000000 tldextract-3.4.1/tldextract/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)       90 2023-01-12 01:07:59.000000 tldextract-3.4.1/tldextract/__main__.py
+-rw-r--r--   0 john       (501) staff       (20)      160 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract/_version.py
+-rw-r--r--   0 john       (501) staff       (20)     8717 2023-04-10 01:08:44.000000 tldextract-3.4.1/tldextract/cache.py
+-rw-r--r--   0 john       (501) staff       (20)     2415 2023-04-10 01:15:19.000000 tldextract-3.4.1/tldextract/cli.py
+-rw-r--r--   0 john       (501) staff       (20)        0 2022-04-01 00:16:04.000000 tldextract-3.4.1/tldextract/py.typed
+-rw-r--r--   0 john       (501) staff       (20)     1182 2023-01-12 01:07:59.000000 tldextract-3.4.1/tldextract/remote.py
+-rw-r--r--   0 john       (501) staff       (20)     3399 2023-01-12 01:48:06.000000 tldextract-3.4.1/tldextract/suffix_list.py
+-rw-r--r--   0 john       (501) staff       (20)    14443 2023-01-12 01:48:06.000000 tldextract-3.4.1/tldextract/tldextract.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.372819 tldextract-3.4.1/tldextract.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     2177 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      783 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       51 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/entry_points.txt
+-rw-r--r--   0 john       (501) staff       (20)       56 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)       11 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)      676 2023-04-26 23:28:17.000000 tldextract-3.4.1/tox.ini
```

### Comparing `tldextract-3.4.0/CHANGELOG.md` & `tldextract-3.4.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 # tldextract Changelog
 
 After upgrading, update your cache file by deleting it or via `tldextract
 --update`.
 
+## 3.4.1 (2023-04-26)
+
+* Bugfixes
+  * Fix Pyright not finding tldextract public interface ([#279](https://github.com/john-kurkowski/tldextract/issues/279))
+  * Fix various Pyright checks
+  * Use SPDX license identifier ([#280](https://github.com/john-kurkowski/tldextract/issues/280))
+  * Support Python 3.11
+* Docs
+  * Add FAQ about private domains
+* Misc.
+  * Update bundled snapshot
+  * Fix lint in newer pylint
+
 ## 3.4.0 (2022-10-04)
 
 * Features
   * Add method `extract_urllib` to extract from a `urllib.parse.{ParseResult,SplitResult}` ([#274](https://github.com/john-kurkowski/tldextract/issues/274))
 * Bugfixes
   * Fix internal type-var error, in newer versions of mypy ([#275](https://github.com/john-kurkowski/tldextract/issues/275))
```

### Comparing `tldextract-3.4.0/LICENSE` & `tldextract-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.0/PKG-INFO` & `tldextract-3.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: tldextract
-Version: 3.4.0
+Version: 3.4.1
 Summary: Accurately separates a URL's subdomain, domain, and public suffix, using the Public Suffix List (PSL). By default, this includes the public ICANN TLDs and their exceptions. You can optionally support the Public Suffix List's private domains as well.
 Home-page: https://github.com/john-kurkowski/tldextract
 Author: John Kurkowski
 Author-email: john.kurkowski@gmail.com
-License: BSD License
+License: BSD-3-Clause
 Keywords: tld domain subdomain url parse extract urlparse urlsplit public suffix list publicsuffix publicsuffixlist
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  `tldextract` accurately separates a URL's subdomain, domain, and public suffix,
 using the Public Suffix List (PSL).
```

### Comparing `tldextract-3.4.0/README.md` & `tldextract-3.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -227,14 +227,19 @@
 This project doesn't contain an actual list of public suffixes. That comes from
 [the Public Suffix List (PSL)](https://publicsuffix.org/). Submit amendments there.
 
 (In the meantime, you can tell tldextract about your exception by either
 forking the PSL and using your fork in the `suffix_list_urls` param, or adding
 your suffix piecemeal with the `extra_suffixes` param.)
 
+### I see my suffix in [the Public Suffix List (PSL)](https://publicsuffix.org/), but this library doesn't extract it.
+
+Check if your suffix is in the private section of the list. See [this
+documentation](#public-vs-private-domains).
+
 ### If I pass an invalid URL, I still get a result, no error. What gives?
 
 To keep `tldextract` light in LoC & overhead, and because there are plenty of
 URL validators out there, this library is very lenient with input. If valid
 URLs are important to you, validate them before calling `tldextract`.
 
 To avoid parsing a string twice, you can pass `tldextract` the output of
```

### Comparing `tldextract-3.4.0/setup.py` & `tldextract-3.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,19 @@
     description=(
         "Accurately separates a URL's subdomain, domain, and public suffix, "
         "using the Public Suffix List (PSL). By "
         "default, this includes the public ICANN TLDs and their "
         "exceptions. You can optionally support the Public Suffix "
         "List's private domains as well."
     ),
-    license="BSD License",
-    keywords="tld domain subdomain url parse extract urlparse urlsplit public suffix list publicsuffix publicsuffixlist",
+    license="BSD-3-Clause",
+    keywords=(
+        "tld domain subdomain url parse extract urlparse urlsplit public suffix list"
+        " publicsuffix publicsuffixlist"
+    ),
     url="https://github.com/john-kurkowski/tldextract",
     packages=["tldextract"],
     include_package_data=True,
     python_requires=">=3.7",
     long_description=__doc__,
     long_description_content_type="text/markdown",
     classifiers=[
@@ -53,14 +56,15 @@
         "Topic :: Utilities",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     entry_points={
         "console_scripts": [
             "tldextract = tldextract.cli:main",
         ]
     },
     setup_requires=["setuptools_scm"],
```

### Comparing `tldextract-3.4.0/tests/cli_test.py` & `tldextract-3.4.1/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.0/tests/custom_suffix_test.py` & `tldextract-3.4.1/tests/custom_suffix_test.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.0/tests/main_test.py` & `tldextract-3.4.1/tests/main_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import tempfile
 from typing import Sequence, Tuple
 
 import pytest
 import responses
 import tldextract
+import tldextract.suffix_list
 from tldextract.cache import DiskCache
 from tldextract.suffix_list import SuffixListNotFound
 from tldextract.tldextract import ExtractResult
 
 extract = tldextract.TLDExtract(cache_dir=tempfile.mkdtemp())
 extract_no_cache = tldextract.TLDExtract(cache_dir=None)
 extract_using_real_local_suffix_list = tldextract.TLDExtract(
```

### Comparing `tldextract-3.4.0/tests/test_cache.py` & `tldextract-3.4.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.0/tests/test_parallel.py` & `tldextract-3.4.1/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.0/tldextract/.tld_set_snapshot` & `tldextract-3.4.1/tldextract/.tld_set_snapshot`

 * *Files 6% similar despite different names*

```diff
@@ -376,19 +376,37 @@
 edu.bi
 or.bi
 org.bi
 
 // biz : https://en.wikipedia.org/wiki/.biz
 biz
 
-// bj : https://en.wikipedia.org/wiki/.bj
+// bj : https://nic.bj/bj-suffixes.txt
+// submitted by registry <contact@nic.bj>
 bj
-asso.bj
-barreau.bj
-gouv.bj
+africa.bj
+agro.bj
+architectes.bj
+assur.bj
+avocats.bj
+co.bj
+com.bj
+eco.bj
+econo.bj
+edu.bj
+info.bj
+loisirs.bj
+money.bj
+net.bj
+org.bj
+ote.bj
+resto.bj
+restaurant.bj
+tourism.bj
+univ.bj
 
 // bm : http://www.bermudanic.bm/dnr-text.txt
 bm
 com.bm
 edu.bm
 gov.bm
 net.bm
@@ -1029,24 +1047,23 @@
 net.fm
 org.fm
 fm
 
 // fo : https://en.wikipedia.org/wiki/.fo
 fo
 
-// fr : http://www.afnic.fr/
-// domaines descriptifs : https://www.afnic.fr/medias/documents/Cadre_legal/Afnic_Naming_Policy_12122016_VEN.pdf
+// fr : https://www.afnic.fr/ https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 fr
 asso.fr
 com.fr
 gouv.fr
 nom.fr
 prd.fr
 tm.fr
-// domaines sectoriels : https://www.afnic.fr/en/products-and-services/the-fr-tld/sector-based-fr-domains-4.html
+// Former "domaines sectoriels", still registration suffixes
 aeroport.fr
 avocat.fr
 avoues.fr
 cci.fr
 chambagri.fr
 chirurgiens-dentistes.fr
 experts-comptables.fr
@@ -1311,24 +1328,36 @@
 sch.id
 web.id
 
 // ie : https://en.wikipedia.org/wiki/.ie
 ie
 gov.ie
 
-// il : http://www.isoc.org.il/domains/
+// il :         http://www.isoc.org.il/domains/
+// see also:    https://en.isoc.org.il/il-cctld/registration-rules
+// ISOC-IL      (operated by .il Registry)
 il
 ac.il
 co.il
 gov.il
 idf.il
 k12.il
 muni.il
 net.il
 org.il
+// xn--4dbrk0ce ("Israel", Hebrew) : IL
+ישראל
+// xn--4dbgdty6c.xn--4dbrk0ce.
+אקדמיה.ישראל
+// xn--5dbhl8d.xn--4dbrk0ce.
+ישוב.ישראל
+// xn--8dbq2a.xn--4dbrk0ce.
+צהל.ישראל
+// xn--hebda8b.xn--4dbrk0ce.
+ממשל.ישראל
 
 // im : https://www.nic.im/
 // Submitted by registry <info@nic.im>
 im
 ac.im
 co.im
 com.im
@@ -1336,30 +1365,59 @@
 net.im
 org.im
 plc.co.im
 tt.im
 tv.im
 
 // in : https://en.wikipedia.org/wiki/.in
-// see also: https://registry.in/Policies
+// see also: https://registry.in/policies
 // Please note, that nic.in is not an official eTLD, but used by most
 // government institutions.
 in
+5g.in
+6g.in
+ac.in
+ai.in
+am.in
+bihar.in
+biz.in
+business.in
+ca.in
+cn.in
 co.in
+com.in
+coop.in
+cs.in
+delhi.in
+dr.in
+edu.in
+er.in
 firm.in
-net.in
-org.in
 gen.in
+gov.in
+gujarat.in
 ind.in
+info.in
+int.in
+internet.in
+io.in
+me.in
+mil.in
+net.in
 nic.in
-ac.in
-edu.in
+org.in
+pg.in
+post.in
+pro.in
 res.in
-gov.in
-mil.in
+travel.in
+tv.in
+uk.in
+up.in
+us.in
 
 // info : https://en.wikipedia.org/wiki/.info
 info
 
 // int : https://en.wikipedia.org/wiki/.int
 // Confirmed by registry <iana-questions@icann.org> 2008-06-18
 int
@@ -4007,563 +4065,16 @@
 net.mu
 org.mu
 gov.mu
 ac.mu
 co.mu
 or.mu
 
-// museum : http://about.museum/naming/
-// http://index.museum/
+// museum : https://welcome.museum/wp-content/uploads/2018/05/20180525-Registration-Policy-MUSEUM-EN_VF-2.pdf https://welcome.museum/buy-your-dot-museum-2/
 museum
-academy.museum
-agriculture.museum
-air.museum
-airguard.museum
-alabama.museum
-alaska.museum
-amber.museum
-ambulance.museum
-american.museum
-americana.museum
-americanantiques.museum
-americanart.museum
-amsterdam.museum
-and.museum
-annefrank.museum
-anthro.museum
-anthropology.museum
-antiques.museum
-aquarium.museum
-arboretum.museum
-archaeological.museum
-archaeology.museum
-architecture.museum
-art.museum
-artanddesign.museum
-artcenter.museum
-artdeco.museum
-arteducation.museum
-artgallery.museum
-arts.museum
-artsandcrafts.museum
-asmatart.museum
-assassination.museum
-assisi.museum
-association.museum
-astronomy.museum
-atlanta.museum
-austin.museum
-australia.museum
-automotive.museum
-aviation.museum
-axis.museum
-badajoz.museum
-baghdad.museum
-bahn.museum
-bale.museum
-baltimore.museum
-barcelona.museum
-baseball.museum
-basel.museum
-baths.museum
-bauern.museum
-beauxarts.museum
-beeldengeluid.museum
-bellevue.museum
-bergbau.museum
-berkeley.museum
-berlin.museum
-bern.museum
-bible.museum
-bilbao.museum
-bill.museum
-birdart.museum
-birthplace.museum
-bonn.museum
-boston.museum
-botanical.museum
-botanicalgarden.museum
-botanicgarden.museum
-botany.museum
-brandywinevalley.museum
-brasil.museum
-bristol.museum
-british.museum
-britishcolumbia.museum
-broadcast.museum
-brunel.museum
-brussel.museum
-brussels.museum
-bruxelles.museum
-building.museum
-burghof.museum
-bus.museum
-bushey.museum
-cadaques.museum
-california.museum
-cambridge.museum
-can.museum
-canada.museum
-capebreton.museum
-carrier.museum
-cartoonart.museum
-casadelamoneda.museum
-castle.museum
-castres.museum
-celtic.museum
-center.museum
-chattanooga.museum
-cheltenham.museum
-chesapeakebay.museum
-chicago.museum
-children.museum
-childrens.museum
-childrensgarden.museum
-chiropractic.museum
-chocolate.museum
-christiansburg.museum
-cincinnati.museum
-cinema.museum
-circus.museum
-civilisation.museum
-civilization.museum
-civilwar.museum
-clinton.museum
-clock.museum
-coal.museum
-coastaldefence.museum
-cody.museum
-coldwar.museum
-collection.museum
-colonialwilliamsburg.museum
-coloradoplateau.museum
-columbia.museum
-columbus.museum
-communication.museum
-communications.museum
-community.museum
-computer.museum
-computerhistory.museum
-comunicações.museum
-contemporary.museum
-contemporaryart.museum
-convent.museum
-copenhagen.museum
-corporation.museum
-correios-e-telecomunicações.museum
-corvette.museum
-costume.museum
-countryestate.museum
-county.museum
-crafts.museum
-cranbrook.museum
-creation.museum
-cultural.museum
-culturalcenter.museum
-culture.museum
-cyber.museum
-cymru.museum
-dali.museum
-dallas.museum
-database.museum
-ddr.museum
-decorativearts.museum
-delaware.museum
-delmenhorst.museum
-denmark.museum
-depot.museum
-design.museum
-detroit.museum
-dinosaur.museum
-discovery.museum
-dolls.museum
-donostia.museum
-durham.museum
-eastafrica.museum
-eastcoast.museum
-education.museum
-educational.museum
-egyptian.museum
-eisenbahn.museum
-elburg.museum
-elvendrell.museum
-embroidery.museum
-encyclopedic.museum
-england.museum
-entomology.museum
-environment.museum
-environmentalconservation.museum
-epilepsy.museum
-essex.museum
-estate.museum
-ethnology.museum
-exeter.museum
-exhibition.museum
-family.museum
-farm.museum
-farmequipment.museum
-farmers.museum
-farmstead.museum
-field.museum
-figueres.museum
-filatelia.museum
-film.museum
-fineart.museum
-finearts.museum
-finland.museum
-flanders.museum
-florida.museum
-force.museum
-fortmissoula.museum
-fortworth.museum
-foundation.museum
-francaise.museum
-frankfurt.museum
-franziskaner.museum
-freemasonry.museum
-freiburg.museum
-fribourg.museum
-frog.museum
-fundacio.museum
-furniture.museum
-gallery.museum
-garden.museum
-gateway.museum
-geelvinck.museum
-gemological.museum
-geology.museum
-georgia.museum
-giessen.museum
-glas.museum
-glass.museum
-gorge.museum
-grandrapids.museum
-graz.museum
-guernsey.museum
-halloffame.museum
-hamburg.museum
-handson.museum
-harvestcelebration.museum
-hawaii.museum
-health.museum
-heimatunduhren.museum
-hellas.museum
-helsinki.museum
-hembygdsforbund.museum
-heritage.museum
-histoire.museum
-historical.museum
-historicalsociety.museum
-historichouses.museum
-historisch.museum
-historisches.museum
-history.museum
-historyofscience.museum
-horology.museum
-house.museum
-humanities.museum
-illustration.museum
-imageandsound.museum
-indian.museum
-indiana.museum
-indianapolis.museum
-indianmarket.museum
-intelligence.museum
-interactive.museum
-iraq.museum
-iron.museum
-isleofman.museum
-jamison.museum
-jefferson.museum
-jerusalem.museum
-jewelry.museum
-jewish.museum
-jewishart.museum
-jfk.museum
-journalism.museum
-judaica.museum
-judygarland.museum
-juedisches.museum
-juif.museum
-karate.museum
-karikatur.museum
-kids.museum
-koebenhavn.museum
-koeln.museum
-kunst.museum
-kunstsammlung.museum
-kunstunddesign.museum
-labor.museum
-labour.museum
-lajolla.museum
-lancashire.museum
-landes.museum
-lans.museum
-läns.museum
-larsson.museum
-lewismiller.museum
-lincoln.museum
-linz.museum
-living.museum
-livinghistory.museum
-localhistory.museum
-london.museum
-losangeles.museum
-louvre.museum
-loyalist.museum
-lucerne.museum
-luxembourg.museum
-luzern.museum
-mad.museum
-madrid.museum
-mallorca.museum
-manchester.museum
-mansion.museum
-mansions.museum
-manx.museum
-marburg.museum
-maritime.museum
-maritimo.museum
-maryland.museum
-marylhurst.museum
-media.museum
-medical.museum
-medizinhistorisches.museum
-meeres.museum
-memorial.museum
-mesaverde.museum
-michigan.museum
-midatlantic.museum
-military.museum
-mill.museum
-miners.museum
-mining.museum
-minnesota.museum
-missile.museum
-missoula.museum
-modern.museum
-moma.museum
-money.museum
-monmouth.museum
-monticello.museum
-montreal.museum
-moscow.museum
-motorcycle.museum
-muenchen.museum
-muenster.museum
-mulhouse.museum
-muncie.museum
-museet.museum
-museumcenter.museum
-museumvereniging.museum
-music.museum
-national.museum
-nationalfirearms.museum
-nationalheritage.museum
-nativeamerican.museum
-naturalhistory.museum
-naturalhistorymuseum.museum
-naturalsciences.museum
-nature.museum
-naturhistorisches.museum
-natuurwetenschappen.museum
-naumburg.museum
-naval.museum
-nebraska.museum
-neues.museum
-newhampshire.museum
-newjersey.museum
-newmexico.museum
-newport.museum
-newspaper.museum
-newyork.museum
-niepce.museum
-norfolk.museum
-north.museum
-nrw.museum
-nyc.museum
-nyny.museum
-oceanographic.museum
-oceanographique.museum
-omaha.museum
-online.museum
-ontario.museum
-openair.museum
-oregon.museum
-oregontrail.museum
-otago.museum
-oxford.museum
-pacific.museum
-paderborn.museum
-palace.museum
-paleo.museum
-palmsprings.museum
-panama.museum
-paris.museum
-pasadena.museum
-pharmacy.museum
-philadelphia.museum
-philadelphiaarea.museum
-philately.museum
-phoenix.museum
-photography.museum
-pilots.museum
-pittsburgh.museum
-planetarium.museum
-plantation.museum
-plants.museum
-plaza.museum
-portal.museum
-portland.museum
-portlligat.museum
-posts-and-telecommunications.museum
-preservation.museum
-presidio.museum
-press.museum
-project.museum
-public.museum
-pubol.museum
-quebec.museum
-railroad.museum
-railway.museum
-research.museum
-resistance.museum
-riodejaneiro.museum
-rochester.museum
-rockart.museum
-roma.museum
-russia.museum
-saintlouis.museum
-salem.museum
-salvadordali.museum
-salzburg.museum
-sandiego.museum
-sanfrancisco.museum
-santabarbara.museum
-santacruz.museum
-santafe.museum
-saskatchewan.museum
-satx.museum
-savannahga.museum
-schlesisches.museum
-schoenbrunn.museum
-schokoladen.museum
-school.museum
-schweiz.museum
-science.museum
-scienceandhistory.museum
-scienceandindustry.museum
-sciencecenter.museum
-sciencecenters.museum
-science-fiction.museum
-sciencehistory.museum
-sciences.museum
-sciencesnaturelles.museum
-scotland.museum
-seaport.museum
-settlement.museum
-settlers.museum
-shell.museum
-sherbrooke.museum
-sibenik.museum
-silk.museum
-ski.museum
-skole.museum
-society.museum
-sologne.museum
-soundandvision.museum
-southcarolina.museum
-southwest.museum
-space.museum
-spy.museum
-square.museum
-stadt.museum
-stalbans.museum
-starnberg.museum
-state.museum
-stateofdelaware.museum
-station.museum
-steam.museum
-steiermark.museum
-stjohn.museum
-stockholm.museum
-stpetersburg.museum
-stuttgart.museum
-suisse.museum
-surgeonshall.museum
-surrey.museum
-svizzera.museum
-sweden.museum
-sydney.museum
-tank.museum
-tcm.museum
-technology.museum
-telekommunikation.museum
-television.museum
-texas.museum
-textile.museum
-theater.museum
-time.museum
-timekeeping.museum
-topology.museum
-torino.museum
-touch.museum
-town.museum
-transport.museum
-tree.museum
-trolley.museum
-trust.museum
-trustee.museum
-uhren.museum
-ulm.museum
-undersea.museum
-university.museum
-usa.museum
-usantiques.museum
-usarts.museum
-uscountryestate.museum
-usculture.museum
-usdecorativearts.museum
-usgarden.museum
-ushistory.museum
-ushuaia.museum
-uslivinghistory.museum
-utah.museum
-uvic.museum
-valley.museum
-vantaa.museum
-versailles.museum
-viking.museum
-village.museum
-virginia.museum
-virtual.museum
-virtuel.museum
-vlaanderen.museum
-volkenkunde.museum
-wales.museum
-wallonie.museum
-war.museum
-washingtondc.museum
-watchandclock.museum
-watch-and-clock.museum
-western.museum
-westfalen.museum
-whaling.museum
-wildlife.museum
-williamsburg.museum
-windmill.museum
-workshop.museum
-york.museum
-yorkshire.museum
-yosemite.museum
-youth.museum
-zoological.museum
-zoology.museum
-ירושלים.museum
-иком.museum
 
 // mv : https://en.wikipedia.org/wiki/.mv
 // "mv" included because, contra Wikipedia, google.mv exists.
 mv
 aero.mv
 biz.mv
 com.mv
@@ -5798,15 +5309,15 @@
 wroclaw.pl
 zachpomor.pl
 zagan.pl
 zarow.pl
 zgora.pl
 zgorzelec.pl
 
-// pm : http://www.afnic.fr/medias/documents/AFNIC-naming-policy2012.pdf
+// pm : https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 pm
 
 // pn : http://www.government.pn/PnRegistry/policies.htm
 pn
 gov.pn
 co.pn
 org.pn
@@ -5896,15 +5407,15 @@
 gov.qa
 mil.qa
 name.qa
 net.qa
 org.qa
 sch.qa
 
-// re : http://www.afnic.re/obtenir/chartes/nommage-re/annexe-descriptifs
+// re : https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 re
 asso.re
 com.re
 nom.re
 
 // ro : http://www.rotld.ro/
 ro
@@ -6153,15 +5664,15 @@
 // td : https://en.wikipedia.org/wiki/.td
 td
 
 // tel: https://en.wikipedia.org/wiki/.tel
 // http://www.telnic.org/
 tel
 
-// tf : https://en.wikipedia.org/wiki/.tf
+// tf : https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 tf
 
 // tg : https://en.wikipedia.org/wiki/.tg
 // http://www.nic.tg/
 tg
 
 // th : https://en.wikipedia.org/wiki/.th
@@ -6361,14 +5872,15 @@
 kherson.ua
 khmelnitskiy.ua
 khmelnytskyi.ua
 kiev.ua
 kirovograd.ua
 km.ua
 kr.ua
+kropyvnytskyi.ua
 krym.ua
 ks.ua
 kv.ua
 kyiv.ua
 lg.ua
 lt.ua
 lugansk.ua
@@ -6772,27 +6284,27 @@
 // http://www.vunic.vu/
 vu
 com.vu
 edu.vu
 net.vu
 org.vu
 
-// wf : http://www.afnic.fr/medias/documents/AFNIC-naming-policy2012.pdf
+// wf : https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 wf
 
 // ws : https://en.wikipedia.org/wiki/.ws
 // http://samoanic.ws/index.dhtml
 ws
 com.ws
 net.ws
 org.ws
 gov.ws
 edu.ws
 
-// yt : http://www.afnic.fr/medias/documents/AFNIC-naming-policy2012.pdf
+// yt : https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 yt
 
 // IDN ccTLDs
 // When submitting patches, please maintain a sort by ISO 3166 ccTLD, then
 // U-label, and follow this format:
 // // A-Label ("<Latin renderings>", <language name>[, variant info]) : <ISO 3166 ccTLD>
 // // [sponsoring org]
@@ -7126,15 +6638,15 @@
 gov.zw
 mil.zw
 org.zw
 
 
 // newGTLDs
 
-// List of new gTLDs imported from https://www.icann.org/resources/registries/gtlds/v2/gtlds.json on 2022-04-30T15:14:46Z
+// List of new gTLDs imported from https://www.icann.org/resources/registries/gtlds/v2/gtlds.json on 2023-04-14T15:13:16Z
 // This list is auto-generated, don't edit it manually.
 // aaa : 2015-02-26 American Automobile Association, Inc.
 aaa
 
 // aarp : 2015-05-21 AARP
 aarp
 
@@ -7176,17 +6688,14 @@
 
 // aco : 2015-01-08 ACO Severin Ahlmann GmbH & Co. KG
 aco
 
 // actor : 2013-12-12 Dog Beach, LLC
 actor
 
-// adac : 2015-07-16 Allgemeiner Deutscher Automobil-Club e.V. (ADAC)
-adac
-
 // ads : 2014-12-04 Charleston Road Registry Inc.
 ads
 
 // adult : 2014-10-16 ICM Registry AD LLC
 adult
 
 // aeg : 2015-03-19 Aktiebolaget Electrolux
@@ -7296,15 +6805,15 @@
 
 // arab : 2015-11-12 League of Arab States
 arab
 
 // aramco : 2014-11-20 Aramco Services Company
 aramco
 
-// archi : 2014-02-06 Afilias Limited
+// archi : 2014-02-06 Identity Digital Limited
 archi
 
 // army : 2014-03-06 Dog Beach, LLC
 army
 
 // art : 2016-03-24 UK Creative Ideas Limited
 art
@@ -7344,15 +6853,15 @@
 
 // auto : 2014-11-13 XYZ.COM LLC
 auto
 
 // autos : 2014-01-09 XYZ.COM LLC
 autos
 
-// avianca : 2015-01-08 Avianca Holdings S.A.
+// avianca : 2015-01-08 Avianca Inc.
 avianca
 
 // aws : 2015-06-25 AWS Registry LLC
 aws
 
 // axa : 2013-12-19 AXA Group Operations SAS
 axa
@@ -7440,15 +6949,15 @@
 
 // best : 2013-12-19 BestTLD Pty Ltd
 best
 
 // bestbuy : 2015-07-31 BBY Solutions, Inc.
 bestbuy
 
-// bet : 2015-05-07 Afilias Limited
+// bet : 2015-05-07 Identity Digital Limited
 bet
 
 // bharti : 2014-01-09 Bharti Enterprises (Holding) Private Limited
 bharti
 
 // bible : 2014-06-19 American Bible Society
 bible
@@ -7461,33 +6970,33 @@
 
 // bing : 2014-12-18 Microsoft Corporation
 bing
 
 // bingo : 2014-12-04 Binky Moon, LLC
 bingo
 
-// bio : 2014-03-06 Afilias Limited
+// bio : 2014-03-06 Identity Digital Limited
 bio
 
-// black : 2014-01-16 Afilias Limited
+// black : 2014-01-16 Identity Digital Limited
 black
 
 // blackfriday : 2014-01-16 Registry Services, LLC
 blackfriday
 
 // blockbuster : 2015-07-30 Dish DBS Corporation
 blockbuster
 
 // blog : 2015-05-14 Knock Knock WHOIS There, LLC
 blog
 
 // bloomberg : 2014-07-17 Bloomberg IP Holdings LLC
 bloomberg
 
-// blue : 2013-11-07 Afilias Limited
+// blue : 2013-11-07 Identity Digital Limited
 blue
 
 // bms : 2014-10-30 Bristol-Myers Squibb Company
 bms
 
 // bmw : 2014-01-09 Bayerische Motoren Werke Aktiengesellschaft
 bmw
@@ -7551,17 +7060,14 @@
 
 // brother : 2015-01-29 Brother Industries, Ltd.
 brother
 
 // brussels : 2014-02-06 DNS.be vzw
 brussels
 
-// bugatti : 2015-07-23 Bugatti International SA
-bugatti
-
 // build : 2013-11-07 Plan Bee LLC
 build
 
 // builders : 2013-11-07 Binky Moon, LLC
 builders
 
 // business : 2013-11-07 Binky Moon, LLC
@@ -7596,17 +7102,14 @@
 
 // camera : 2013-08-27 Binky Moon, LLC
 camera
 
 // camp : 2013-11-07 Binky Moon, LLC
 camp
 
-// cancerresearch : 2014-05-15 Australian Cancer Research Foundation
-cancerresearch
-
 // canon : 2014-09-12 Canon Inc.
 canon
 
 // capetown : 2014-03-24 ZA Central Registry NPC trading as ZA Central Registry
 capetown
 
 // capital : 2014-03-06 Binky Moon, LLC
@@ -7635,15 +7138,15 @@
 
 // cars : 2014-11-13 XYZ.COM LLC
 cars
 
 // casa : 2013-11-21 Registry Services, LLC
 casa
 
-// case : 2015-09-03 Helium TLDs Ltd
+// case : 2015-09-03 Digity, LLC
 case
 
 // cash : 2014-03-06 Binky Moon, LLC
 cash
 
 // casino : 2014-12-18 Binky Moon, LLC
 casino
@@ -7683,15 +7186,15 @@
 
 // chanel : 2015-04-09 Chanel International B.V.
 chanel
 
 // channel : 2014-05-08 Charleston Road Registry Inc.
 channel
 
-// charity : 2018-04-11 Binky Moon, LLC
+// charity : 2018-04-11 Public Interest Registry
 charity
 
 // chase : 2015-04-30 JPMorgan Chase Bank, National Association
 chase
 
 // chat : 2014-12-04 Binky Moon, LLC
 chat
@@ -7737,15 +7240,15 @@
 
 // claims : 2014-03-20 Binky Moon, LLC
 claims
 
 // cleaning : 2013-12-05 Binky Moon, LLC
 cleaning
 
-// click : 2014-06-05 UNR Corp.
+// click : 2014-06-05 Internet Naming Company LLC
 click
 
 // clinic : 2014-03-20 Binky Moon, LLC
 clinic
 
 // clinique : 2015-10-01 The Estée Lauder Companies Inc.
 clinique
@@ -7821,24 +7324,24 @@
 
 // cool : 2013-11-14 Binky Moon, LLC
 cool
 
 // corsica : 2014-09-25 Collectivité de Corse
 corsica
 
-// country : 2013-12-19 DotCountry LLC
+// country : 2013-12-19 Internet Naming Company LLC
 country
 
 // coupon : 2015-02-26 Amazon Registry Services, Inc.
 coupon
 
 // coupons : 2015-03-26 Binky Moon, LLC
 coupons
 
-// courses : 2014-12-04 OPEN UNIVERSITIES AUSTRALIA PTY LTD
+// courses : 2014-12-04 Registry Services, LLC
 courses
 
 // cpa : 2019-06-10 American Institute of Certified Public Accountants
 cpa
 
 // credit : 2014-03-20 Binky Moon, LLC
 credit
@@ -8016,15 +7519,15 @@
 
 // dvag : 2014-06-23 Deutsche Vermögensberatung Aktiengesellschaft DVAG
 dvag
 
 // dvr : 2016-05-26 DISH Technologies L.L.C.
 dvr
 
-// earth : 2014-12-04 Interlink Co., Ltd.
+// earth : 2014-12-04 Interlink Systems Innovation Institute K.K.
 earth
 
 // eat : 2014-01-23 Charleston Road Registry Inc.
 eat
 
 // eco : 2016-07-08 Big Room Inc.
 eco
@@ -8223,15 +7726,15 @@
 
 // forsale : 2014-05-22 Dog Beach, LLC
 forsale
 
 // forum : 2015-04-02 Fegistry, LLC
 forum
 
-// foundation : 2013-12-05 Binky Moon, LLC
+// foundation : 2013-12-05 Public Interest Registry
 foundation
 
 // fox : 2015-09-11 FOX Registry, LLC
 fox
 
 // free : 2015-12-10 Amazon Registry Services, Inc.
 free
@@ -8322,27 +7825,27 @@
 
 // gift : 2013-10-17 DotGift, LLC
 gift
 
 // gifts : 2014-07-03 Binky Moon, LLC
 gifts
 
-// gives : 2014-03-06 Dog Beach, LLC
+// gives : 2014-03-06 Public Interest Registry
 gives
 
-// giving : 2014-11-13 Giving Limited
+// giving : 2014-11-13 Public Interest Registry
 giving
 
 // glass : 2013-11-07 Binky Moon, LLC
 glass
 
 // gle : 2014-07-24 Charleston Road Registry Inc.
 gle
 
-// global : 2014-04-17 Dot Global Domain Registry Limited
+// global : 2014-04-17 Identity Digital Limited
 global
 
 // globo : 2013-12-19 Globo Comunicação e Participações S.A
 globo
 
 // gmail : 2014-05-01 Charleston Road Registry Inc.
 gmail
@@ -8391,15 +7894,15 @@
 
 // graphics : 2013-09-13 Binky Moon, LLC
 graphics
 
 // gratis : 2014-03-20 Binky Moon, LLC
 gratis
 
-// green : 2014-05-08 Afilias Limited
+// green : 2014-05-08 Identity Digital Limited
 green
 
 // gripe : 2014-03-06 Binky Moon, LLC
 gripe
 
 // grocery : 2016-06-16 Wal-Mart Stores, Inc.
 grocery
@@ -8448,15 +7951,15 @@
 
 // health : 2015-02-11 DotHealth, LLC
 health
 
 // healthcare : 2014-06-12 Binky Moon, LLC
 healthcare
 
-// help : 2014-06-26 UNR Corp.
+// help : 2014-06-26 Innovation service Limited
 help
 
 // helsinki : 2015-02-05 City of Helsinki
 helsinki
 
 // here : 2014-02-06 Charleston Road Registry Inc.
 here
@@ -8472,15 +7975,15 @@
 
 // hisamitsu : 2015-07-16 Hisamitsu Pharmaceutical Co.,Inc.
 hisamitsu
 
 // hitachi : 2014-10-31 Hitachi, Ltd.
 hitachi
 
-// hiv : 2014-03-13 UNR Corp.
+// hiv : 2014-03-13 Internet Naming Company LLC
 hiv
 
 // hkt : 2015-05-14 PCCW-HKT DataCom Services Limited
 hkt
 
 // hockey : 2015-03-19 Binky Moon, LLC
 hockey
@@ -8676,15 +8179,15 @@
 
 // jpmorgan : 2015-04-30 JPMorgan Chase Bank, National Association
 jpmorgan
 
 // jprs : 2014-09-18 Japan Registry Services Co., Ltd.
 jprs
 
-// juegos : 2014-03-20 UNR Corp.
+// juegos : 2014-03-20 Internet Naming Company LLC
 juegos
 
 // juniper : 2015-07-30 JUNIPER NETWORKS, INC.
 juniper
 
 // kaufen : 2013-11-07 Dog Beach, LLC
 kaufen
@@ -8706,15 +8209,15 @@
 
 // kia : 2015-07-09 KIA MOTORS CORPORATION
 kia
 
 // kids : 2021-08-13 DotKids Foundation Limited
 kids
 
-// kim : 2013-09-23 Afilias Limited
+// kim : 2013-09-23 Identity Digital Limited
 kim
 
 // kinder : 2014-11-07 Ferrero Trading Lux S.A.
 kinder
 
 // kindle : 2015-06-25 Amazon Registry Services, Inc.
 kindle
@@ -8775,15 +8278,15 @@
 
 // lanxess : 2015-07-30 LANXESS Corporation
 lanxess
 
 // lasalle : 2015-04-02 Jones Lang LaSalle Incorporated
 lasalle
 
-// lat : 2014-10-16 ECOM-LAC Federaciòn de Latinoamèrica y el Caribe para Internet y el Comercio Electrònico
+// lat : 2014-10-16 XYZ.COM LLC
 lat
 
 // latino : 2015-07-30 Dish DBS Corporation
 latino
 
 // latrobe : 2014-06-16 La Trobe University
 latrobe
@@ -8811,15 +8314,15 @@
 
 // lego : 2015-07-16 LEGO Juris A/S
 lego
 
 // lexus : 2015-04-23 TOYOTA MOTOR CORPORATION
 lexus
 
-// lgbt : 2014-05-08 Afilias Limited
+// lgbt : 2014-05-08 Identity Digital Limited
 lgbt
 
 // lidl : 2014-09-18 Schwarz Domains und Services GmbH & Co. KG
 lidl
 
 // life : 2014-02-06 Binky Moon, LLC
 life
@@ -8844,60 +8347,54 @@
 
 // limo : 2013-10-17 Binky Moon, LLC
 limo
 
 // lincoln : 2014-11-13 Ford Motor Company
 lincoln
 
-// linde : 2014-12-04 Linde Aktiengesellschaft
-linde
-
-// link : 2013-11-14 UNR Corp.
+// link : 2013-11-14 Nova Registry Ltd
 link
 
 // lipsy : 2015-06-25 Lipsy Ltd
 lipsy
 
 // live : 2014-12-04 Dog Beach, LLC
 live
 
 // living : 2015-07-30 Lifestyle Domain Holdings, Inc.
 living
 
-// llc : 2017-12-14 Afilias Limited
+// llc : 2017-12-14 Identity Digital Limited
 llc
 
-// llp : 2019-08-26 UNR Corp.
+// llp : 2019-08-26 Intercap Registry Inc.
 llp
 
 // loan : 2014-11-20 dot Loan Limited
 loan
 
 // loans : 2014-03-20 Binky Moon, LLC
 loans
 
 // locker : 2015-06-04 Dish DBS Corporation
 locker
 
 // locus : 2015-06-25 Locus Analytics LLC
 locus
 
-// loft : 2015-07-30 Annco, Inc.
-loft
-
 // lol : 2015-01-30 XYZ.COM LLC
 lol
 
 // london : 2013-11-14 Dot London Domains Limited
 london
 
 // lotte : 2014-11-07 Lotte Holdings Co., Ltd.
 lotte
 
-// lotto : 2014-04-10 Afilias Limited
+// lotto : 2014-04-10 Identity Digital Limited
 lotto
 
 // love : 2014-12-22 Merchant Law Group LLP
 love
 
 // lpl : 2015-07-30 LPL Holdings, Inc.
 lpl
@@ -8916,17 +8413,14 @@
 
 // luxe : 2014-01-09 Registry Services, LLC
 luxe
 
 // luxury : 2013-10-17 Luxury Partners, LLC
 luxury
 
-// macys : 2015-07-31 Macys, Inc.
-macys
-
 // madrid : 2014-05-01 Comunidad de Madrid
 madrid
 
 // maif : 2014-10-02 Mutuelle Assurance Instituteur France (MAIF)
 maif
 
 // maison : 2013-12-05 Binky Moon, LLC
@@ -9030,15 +8524,15 @@
 
 // mobile : 2016-06-02 Dish DBS Corporation
 mobile
 
 // moda : 2013-11-07 Dog Beach, LLC
 moda
 
-// moe : 2013-11-13 Interlink Co., Ltd.
+// moe : 2013-11-13 Interlink Systems Innovation Institute K.K.
 moe
 
 // moi : 2014-12-18 Amazon Registry Services, Inc.
 moi
 
 // mom : 2015-04-16 XYZ.COM LLC
 mom
@@ -9237,15 +8731,15 @@
 
 // oracle : 2014-06-19 Oracle Corporation
 oracle
 
 // orange : 2015-03-12 Orange Brand Services Limited
 orange
 
-// organic : 2014-03-27 Afilias Limited
+// organic : 2014-03-27 Identity Digital Limited
 organic
 
 // origins : 2015-10-01 The Estée Lauder Companies Inc.
 origins
 
 // osaka : 2014-09-04 Osaka Registry Co., Ltd.
 osaka
@@ -9258,15 +8752,15 @@
 
 // ovh : 2014-01-16 MédiaBC
 ovh
 
 // page : 2014-12-04 Charleston Road Registry Inc.
 page
 
-// panasonic : 2015-07-30 Panasonic Corporation
+// panasonic : 2015-07-30 Panasonic Holdings Corporation
 panasonic
 
 // paris : 2014-01-30 City of Paris
 paris
 
 // pars : 2014-09-04 Asia Green IT System Bilgisayar San. ve Tic. Ltd. Sti.
 pars
@@ -9285,15 +8779,15 @@
 
 // pay : 2015-08-27 Amazon Registry Services, Inc.
 pay
 
 // pccw : 2015-05-14 PCCW Enterprises Limited
 pccw
 
-// pet : 2015-05-07 Afilias Limited
+// pet : 2015-05-07 Identity Digital Limited
 pet
 
 // pfizer : 2015-09-11 Pfizer Inc.
 pfizer
 
 // pharmacy : 2014-06-19 National Association of Boards of Pharmacy
 pharmacy
@@ -9333,15 +8827,15 @@
 
 // pin : 2014-12-18 Amazon Registry Services, Inc.
 pin
 
 // ping : 2015-06-11 Ping Registry Provider, Inc.
 ping
 
-// pink : 2013-10-01 Afilias Limited
+// pink : 2013-10-01 Identity Digital Limited
 pink
 
 // pioneer : 2015-07-16 Pioneer Corporation
 pioneer
 
 // pizza : 2014-06-26 Binky Moon, LLC
 pizza
@@ -9363,15 +8857,15 @@
 
 // pnc : 2015-07-02 PNC Domain Co., LLC
 pnc
 
 // pohl : 2014-06-23 Deutsche Vermögensberatung Aktiengesellschaft DVAG
 pohl
 
-// poker : 2014-07-03 Afilias Limited
+// poker : 2014-07-03 Identity Digital Limited
 poker
 
 // politie : 2015-08-20 Politie Nederland
 politie
 
 // porn : 2014-10-16 ICM Registry PN LLC
 porn
@@ -9396,21 +8890,21 @@
 
 // prof : 2014-07-24 Charleston Road Registry Inc.
 prof
 
 // progressive : 2015-07-23 Progressive Casualty Insurance Company
 progressive
 
-// promo : 2014-12-18 Afilias Limited
+// promo : 2014-12-18 Identity Digital Limited
 promo
 
 // properties : 2013-12-05 Binky Moon, LLC
 properties
 
-// property : 2014-05-22 UNR Corp.
+// property : 2014-05-22 Internet Naming Company LLC
 property
 
 // protection : 2015-04-23 XYZ.COM LLC
 protection
 
 // pru : 2015-07-30 Prudential Financial, Inc.
 pru
@@ -9420,15 +8914,15 @@
 
 // pub : 2013-12-12 Dog Beach, LLC
 pub
 
 // pwc : 2015-10-29 PricewaterhouseCoopers LLP
 pwc
 
-// qpon : 2013-11-14 dotCOOL, Inc.
+// qpon : 2013-11-14 dotQPON LLC
 qpon
 
 // quebec : 2013-12-19 PointQuébec Inc
 quebec
 
 // quest : 2015-03-26 XYZ.COM LLC
 quest
@@ -9450,15 +8944,15 @@
 
 // realty : 2015-03-19 Dog Beach, LLC
 realty
 
 // recipes : 2013-10-17 Binky Moon, LLC
 recipes
 
-// red : 2013-11-07 Afilias Limited
+// red : 2013-11-07 Identity Digital Limited
 red
 
 // redstone : 2014-10-31 Redstone Haute Couture Co., Ltd.
 redstone
 
 // redumbrella : 2015-03-26 Travelers TLD, LLC
 redumbrella
@@ -9666,27 +9160,24 @@
 
 // sener : 2014-10-24 Sener Ingeniería y Sistemas, S.A.
 sener
 
 // services : 2014-02-27 Binky Moon, LLC
 services
 
-// ses : 2015-07-23 SES
-ses
-
 // seven : 2015-08-06 Seven West Media Ltd
 seven
 
 // sew : 2014-07-17 SEW-EURODRIVE GmbH & Co KG
 sew
 
 // sex : 2014-11-13 ICM Registry SX LLC
 sex
 
-// sexy : 2013-09-11 UNR Corp.
+// sexy : 2013-09-11 Internet Naming Company LLC
 sexy
 
 // sfr : 2015-08-13 Societe Francaise du Radiotelephone - SFR
 sfr
 
 // shangrila : 2015-09-03 Shangri‐La International Hotel Management Limited
 shangrila
@@ -9699,15 +9190,15 @@
 
 // shell : 2015-07-30 Shell Information Technology International Inc
 shell
 
 // shia : 2014-09-04 Asia Green IT System Bilgisayar San. ve Tic. Ltd. Sti.
 shia
 
-// shiksha : 2013-11-14 Afilias Limited
+// shiksha : 2013-11-14 Identity Digital Limited
 shiksha
 
 // shoes : 2013-10-02 Binky Moon, LLC
 shoes
 
 // shop : 2016-04-08 GMO Registry, Inc.
 shop
@@ -9732,15 +9223,15 @@
 
 // singles : 2013-08-27 Binky Moon, LLC
 singles
 
 // site : 2015-01-15 Radix FZC
 site
 
-// ski : 2015-04-09 Afilias Limited
+// ski : 2015-04-09 Identity Digital Limited
 ski
 
 // skin : 2015-01-15 XYZ.COM LLC
 skin
 
 // sky : 2014-06-19 Sky International AG
 sky
@@ -9753,15 +9244,15 @@
 
 // smart : 2015-07-09 Smart Communications, Inc. (SMART)
 smart
 
 // smile : 2014-12-18 Amazon Registry Services, Inc.
 smile
 
-// sncf : 2015-02-19 Société Nationale des Chemins de fer Francais S N C F
+// sncf : 2015-02-19 Société Nationale SNCF
 sncf
 
 // soccer : 2015-03-26 Binky Moon, LLC
 soccer
 
 // social : 2013-11-07 Dog Beach, LLC
 social
@@ -9837,15 +9328,15 @@
 
 // stream : 2016-01-08 dot Stream Limited
 stream
 
 // studio : 2015-02-11 Dog Beach, LLC
 studio
 
-// study : 2014-12-11 OPEN UNIVERSITIES AUSTRALIA PTY LTD
+// study : 2014-12-11 Registry Services, LLC
 study
 
 // style : 2014-12-04 Binky Moon, LLC
 style
 
 // sucks : 2014-12-22 Vox Populi Registry Ltd.
 sucks
@@ -9990,15 +9481,15 @@
 
 // toray : 2014-12-18 Toray Industries, Inc.
 toray
 
 // toshiba : 2014-04-10 TOSHIBA Corporation
 toshiba
 
-// total : 2015-08-06 TOTAL SE
+// total : 2015-08-06 TotalEnergies SE
 total
 
 // tours : 2015-01-22 Binky Moon, LLC
 tours
 
 // town : 2014-03-06 Binky Moon, LLC
 town
@@ -10026,15 +9517,15 @@
 
 // travelers : 2015-03-26 Travelers TLD, LLC
 travelers
 
 // travelersinsurance : 2015-03-26 Travelers TLD, LLC
 travelersinsurance
 
-// trust : 2014-10-16 UNR Corp.
+// trust : 2014-10-16 Internet Naming Company LLC
 trust
 
 // trv : 2015-03-26 Travelers TLD, LLC
 trv
 
 // tube : 2015-06-11 Latin American Telecom LLC
 tube
@@ -10173,15 +9664,15 @@
 
 // wanggou : 2014-12-18 Amazon Registry Services, Inc.
 wanggou
 
 // watch : 2013-11-14 Binky Moon, LLC
 watch
 
-// watches : 2014-12-22 Afilias Limited
+// watches : 2014-12-22 Identity Digital Limited
 watches
 
 // weather : 2015-01-08 International Business Machines Corporation
 weather
 
 // weatherchannel : 2015-03-12 International Business Machines Corporation
 weatherchannel
@@ -10308,15 +9799,15 @@
 
 // xn--5su34j936bgsg : 2015-09-03 Shangri‐La International Hotel Management Limited
 香格里拉
 
 // xn--5tzm5g : 2014-12-22 Global Website TLD Asia Limited
 网站
 
-// xn--6frz82g : 2013-09-23 Afilias Limited
+// xn--6frz82g : 2013-09-23 Identity Digital Limited
 移动
 
 // xn--6qq986b3xl : 2013-09-13 Tycoon Treasure Limited
 我爱你
 
 // xn--80adxhks : 2013-12-19 Foundation for Assistance for Internet Technologies and Infrastructure Development (FAITID)
 москва
@@ -10425,17 +9916,14 @@
 
 // xn--j1aef : 2015-01-15 VeriSign Sarl
 ком
 
 // xn--jlq480n2rg : 2019-12-19 Amazon Registry Services, Inc.
 亚马逊
 
-// xn--jlq61u9w7b : 2015-01-08 Nokia Corporation
-诺基亚
-
 // xn--jvr189m : 2015-02-26 Amazon Registry Services, Inc.
 食品
 
 // xn--kcrx77d1x4a : 2014-11-07 Koninklijke Philips N.V.
 飞利浦
 
 // xn--kput3i : 2014-02-13 Beijing RITT-Net Technology Development Co., Ltd
@@ -10615,37 +10103,68 @@
 // Submitted by Aaron Marais <its_me@aaronleem.co.za>
 graphox.us
 
 // accesso Technology Group, plc. : https://accesso.com/
 // Submitted by accesso Team <accessoecommerce@accesso.com>
 *.devcdnaccesso.com
 
+// Acorn Labs : https://acorn.io
+// Submitted by Craig Jellick <domains@acorn.io>
+*.on-acorn.io
+
+// ActiveTrail: https://www.activetrail.biz/
+// Submitted by Ofer Kalaora <postmaster@activetrail.com>
+activetrail.biz
+
 // Adobe : https://www.adobe.com/
 // Submitted by Ian Boston <boston@adobe.com> and Lars Trieloff <trieloff@adobe.com>
 adobeaemcloud.com
 *.dev.adobeaemcloud.com
 hlx.live
 adobeaemcloud.net
 hlx.page
 hlx3.page
 
+// Adobe Developer Platform : https://developer.adobe.com
+// Submitted by Jesse MacFadyen<jessem@adobe.com>
+adobeio-static.net
+adobeioruntime.net
+
 // Agnat sp. z o.o. : https://domena.pl
 // Submitted by Przemyslaw Plewa <it-admin@domena.pl>
 beep.pl
 
 // Airkit : https://www.airkit.com/
 // Submitted by Grant Cooksey <security@airkit.com>
 airkitapps.com
 airkitapps-au.com
 airkitapps.eu
 
 // Aiven: https://aiven.io/
 // Submitted by Etienne Stalmans <security@aiven.io>
 aivencloud.com
 
+// Akamai : https://www.akamai.com/
+// Submitted by Akamai Team <publicsuffixlist@akamai.com>
+akadns.net
+akamai.net
+akamai-staging.net
+akamaiedge.net
+akamaiedge-staging.net
+akamaihd.net
+akamaihd-staging.net
+akamaiorigin.net
+akamaiorigin-staging.net
+akamaized.net
+akamaized-staging.net
+edgekey.net
+edgekey-staging.net
+edgesuite.net
+edgesuite-staging.net
+
 // alboto.ca : http://alboto.ca
 // Submitted by Anton Avramov <avramov@alboto.ca>
 barsy.ca
 
 // Alces Software Ltd : http://alces-software.com
 // Submitted by Mark J. Titorenko <mark.titorenko@alces-software.com>
 *.compute.estate
@@ -10659,27 +10178,142 @@
 // Submitted by Carlo Cannas <tech_staff@altervista.it>
 altervista.org
 
 // alwaysdata : https://www.alwaysdata.com
 // Submitted by Cyril <admin@alwaysdata.com>
 alwaysdata.net
 
-// Amazon CloudFront : https://aws.amazon.com/cloudfront/
+// Amaze Software : https://amaze.co
+// Submitted by Domain Admin <domainadmin@amaze.co>
+myamaze.net
+
+// Amazon : https://www.amazon.com/
+// Submitted by AWS Security <psl-maintainers@amazon.com>
+// Subsections of Amazon/subsidiaries will appear until "concludes" tag
+
+// Amazon CloudFront
 // Submitted by Donavan Miller <donavanm@amazon.com>
+// Reference: 54144616-fd49-4435-8535-19c6a601bdb3
 cloudfront.net
 
-// Amazon Elastic Compute Cloud : https://aws.amazon.com/ec2/
+// Amazon EC2
 // Submitted by Luke Wells <psl-maintainers@amazon.com>
+// Reference: 4c38fa71-58ac-4768-99e5-689c1767e537
 *.compute.amazonaws.com
 *.compute-1.amazonaws.com
 *.compute.amazonaws.com.cn
 us-east-1.amazonaws.com
 
-// Amazon Elastic Beanstalk : https://aws.amazon.com/elasticbeanstalk/
+// Amazon S3
+// Submitted by Luke Wells <psl-maintainers@amazon.com>
+// Reference: d068bd97-f0a9-4838-a6d8-954b622ef4ae
+s3.cn-north-1.amazonaws.com.cn
+s3.dualstack.ap-northeast-1.amazonaws.com
+s3.dualstack.ap-northeast-2.amazonaws.com
+s3.ap-northeast-2.amazonaws.com
+s3-website.ap-northeast-2.amazonaws.com
+s3.dualstack.ap-south-1.amazonaws.com
+s3.ap-south-1.amazonaws.com
+s3-website.ap-south-1.amazonaws.com
+s3.dualstack.ap-southeast-1.amazonaws.com
+s3.dualstack.ap-southeast-2.amazonaws.com
+s3.dualstack.ca-central-1.amazonaws.com
+s3.ca-central-1.amazonaws.com
+s3-website.ca-central-1.amazonaws.com
+s3.dualstack.eu-central-1.amazonaws.com
+s3.eu-central-1.amazonaws.com
+s3-website.eu-central-1.amazonaws.com
+s3.dualstack.eu-west-1.amazonaws.com
+s3.dualstack.eu-west-2.amazonaws.com
+s3.eu-west-2.amazonaws.com
+s3-website.eu-west-2.amazonaws.com
+s3.dualstack.eu-west-3.amazonaws.com
+s3.eu-west-3.amazonaws.com
+s3-website.eu-west-3.amazonaws.com
+s3.amazonaws.com
+s3-ap-northeast-1.amazonaws.com
+s3-ap-northeast-2.amazonaws.com
+s3-ap-south-1.amazonaws.com
+s3-ap-southeast-1.amazonaws.com
+s3-ap-southeast-2.amazonaws.com
+s3-ca-central-1.amazonaws.com
+s3-eu-central-1.amazonaws.com
+s3-eu-west-1.amazonaws.com
+s3-eu-west-2.amazonaws.com
+s3-eu-west-3.amazonaws.com
+s3-external-1.amazonaws.com
+s3-fips-us-gov-west-1.amazonaws.com
+s3-sa-east-1.amazonaws.com
+s3-us-east-2.amazonaws.com
+s3-us-gov-west-1.amazonaws.com
+s3-us-west-1.amazonaws.com
+s3-us-west-2.amazonaws.com
+s3-website-ap-northeast-1.amazonaws.com
+s3-website-ap-southeast-1.amazonaws.com
+s3-website-ap-southeast-2.amazonaws.com
+s3-website-eu-west-1.amazonaws.com
+s3-website-sa-east-1.amazonaws.com
+s3-website-us-east-1.amazonaws.com
+s3-website-us-west-1.amazonaws.com
+s3-website-us-west-2.amazonaws.com
+s3.dualstack.sa-east-1.amazonaws.com
+s3.dualstack.us-east-1.amazonaws.com
+s3.dualstack.us-east-2.amazonaws.com
+s3.us-east-2.amazonaws.com
+s3-website.us-east-2.amazonaws.com
+
+// AWS Cloud9
+// Submitted by: AWS Security <psl-maintainers@amazon.com>
+// Reference: 2b6dfa9a-3a7f-4367-b2e7-0321e77c0d59
+vfs.cloud9.af-south-1.amazonaws.com
+webview-assets.cloud9.af-south-1.amazonaws.com
+vfs.cloud9.ap-east-1.amazonaws.com
+webview-assets.cloud9.ap-east-1.amazonaws.com
+vfs.cloud9.ap-northeast-1.amazonaws.com
+webview-assets.cloud9.ap-northeast-1.amazonaws.com
+vfs.cloud9.ap-northeast-2.amazonaws.com
+webview-assets.cloud9.ap-northeast-2.amazonaws.com
+vfs.cloud9.ap-northeast-3.amazonaws.com
+webview-assets.cloud9.ap-northeast-3.amazonaws.com
+vfs.cloud9.ap-south-1.amazonaws.com
+webview-assets.cloud9.ap-south-1.amazonaws.com
+vfs.cloud9.ap-southeast-1.amazonaws.com
+webview-assets.cloud9.ap-southeast-1.amazonaws.com
+vfs.cloud9.ap-southeast-2.amazonaws.com
+webview-assets.cloud9.ap-southeast-2.amazonaws.com
+vfs.cloud9.ca-central-1.amazonaws.com
+webview-assets.cloud9.ca-central-1.amazonaws.com
+vfs.cloud9.eu-central-1.amazonaws.com
+webview-assets.cloud9.eu-central-1.amazonaws.com
+vfs.cloud9.eu-north-1.amazonaws.com
+webview-assets.cloud9.eu-north-1.amazonaws.com
+vfs.cloud9.eu-south-1.amazonaws.com
+webview-assets.cloud9.eu-south-1.amazonaws.com
+vfs.cloud9.eu-west-1.amazonaws.com
+webview-assets.cloud9.eu-west-1.amazonaws.com
+vfs.cloud9.eu-west-2.amazonaws.com
+webview-assets.cloud9.eu-west-2.amazonaws.com
+vfs.cloud9.eu-west-3.amazonaws.com
+webview-assets.cloud9.eu-west-3.amazonaws.com
+vfs.cloud9.me-south-1.amazonaws.com
+webview-assets.cloud9.me-south-1.amazonaws.com
+vfs.cloud9.sa-east-1.amazonaws.com
+webview-assets.cloud9.sa-east-1.amazonaws.com
+vfs.cloud9.us-east-1.amazonaws.com
+webview-assets.cloud9.us-east-1.amazonaws.com
+vfs.cloud9.us-east-2.amazonaws.com
+webview-assets.cloud9.us-east-2.amazonaws.com
+vfs.cloud9.us-west-1.amazonaws.com
+webview-assets.cloud9.us-west-1.amazonaws.com
+vfs.cloud9.us-west-2.amazonaws.com
+webview-assets.cloud9.us-west-2.amazonaws.com
+
+// AWS Elastic Beanstalk
 // Submitted by Luke Wells <psl-maintainers@amazon.com>
+// Reference: aa202394-43a0-4857-b245-8db04549137e
 cn-north-1.eb.amazonaws.com.cn
 cn-northwest-1.eb.amazonaws.com.cn
 elasticbeanstalk.com
 ap-northeast-1.elasticbeanstalk.com
 ap-northeast-2.elasticbeanstalk.com
 ap-northeast-3.elasticbeanstalk.com
 ap-south-1.elasticbeanstalk.com
@@ -10693,79 +10327,32 @@
 sa-east-1.elasticbeanstalk.com
 us-east-1.elasticbeanstalk.com
 us-east-2.elasticbeanstalk.com
 us-gov-west-1.elasticbeanstalk.com
 us-west-1.elasticbeanstalk.com
 us-west-2.elasticbeanstalk.com
 
-// Amazon Elastic Load Balancing : https://aws.amazon.com/elasticloadbalancing/
+// (AWS) Elastic Load Balancing
 // Submitted by Luke Wells <psl-maintainers@amazon.com>
-*.elb.amazonaws.com
+// Reference: 12a3d528-1bac-4433-a359-a395867ffed2
 *.elb.amazonaws.com.cn
+*.elb.amazonaws.com
 
-// Amazon Global Accelerator : https://aws.amazon.com/global-accelerator/
+// AWS Global Accelerator
 // Submitted by Daniel Massaguer <psl-maintainers@amazon.com>
+// Reference: d916759d-a08b-4241-b536-4db887383a6a
 awsglobalaccelerator.com
 
-// Amazon S3 : https://aws.amazon.com/s3/
-// Submitted by Luke Wells <psl-maintainers@amazon.com>
-s3.amazonaws.com
-s3-ap-northeast-1.amazonaws.com
-s3-ap-northeast-2.amazonaws.com
-s3-ap-south-1.amazonaws.com
-s3-ap-southeast-1.amazonaws.com
-s3-ap-southeast-2.amazonaws.com
-s3-ca-central-1.amazonaws.com
-s3-eu-central-1.amazonaws.com
-s3-eu-west-1.amazonaws.com
-s3-eu-west-2.amazonaws.com
-s3-eu-west-3.amazonaws.com
-s3-external-1.amazonaws.com
-s3-fips-us-gov-west-1.amazonaws.com
-s3-sa-east-1.amazonaws.com
-s3-us-gov-west-1.amazonaws.com
-s3-us-east-2.amazonaws.com
-s3-us-west-1.amazonaws.com
-s3-us-west-2.amazonaws.com
-s3.ap-northeast-2.amazonaws.com
-s3.ap-south-1.amazonaws.com
-s3.cn-north-1.amazonaws.com.cn
-s3.ca-central-1.amazonaws.com
-s3.eu-central-1.amazonaws.com
-s3.eu-west-2.amazonaws.com
-s3.eu-west-3.amazonaws.com
-s3.us-east-2.amazonaws.com
-s3.dualstack.ap-northeast-1.amazonaws.com
-s3.dualstack.ap-northeast-2.amazonaws.com
-s3.dualstack.ap-south-1.amazonaws.com
-s3.dualstack.ap-southeast-1.amazonaws.com
-s3.dualstack.ap-southeast-2.amazonaws.com
-s3.dualstack.ca-central-1.amazonaws.com
-s3.dualstack.eu-central-1.amazonaws.com
-s3.dualstack.eu-west-1.amazonaws.com
-s3.dualstack.eu-west-2.amazonaws.com
-s3.dualstack.eu-west-3.amazonaws.com
-s3.dualstack.sa-east-1.amazonaws.com
-s3.dualstack.us-east-1.amazonaws.com
-s3.dualstack.us-east-2.amazonaws.com
-s3-website-us-east-1.amazonaws.com
-s3-website-us-west-1.amazonaws.com
-s3-website-us-west-2.amazonaws.com
-s3-website-ap-northeast-1.amazonaws.com
-s3-website-ap-southeast-1.amazonaws.com
-s3-website-ap-southeast-2.amazonaws.com
-s3-website-eu-west-1.amazonaws.com
-s3-website-sa-east-1.amazonaws.com
-s3-website.ap-northeast-2.amazonaws.com
-s3-website.ap-south-1.amazonaws.com
-s3-website.ca-central-1.amazonaws.com
-s3-website.eu-central-1.amazonaws.com
-s3-website.eu-west-2.amazonaws.com
-s3-website.eu-west-3.amazonaws.com
-s3-website.us-east-2.amazonaws.com
+// eero
+// Submitted by Yue Kang <eero-dynamic-dns@amazon.com>
+// Reference: 264afe70-f62c-4c02-8ab9-b5281ed24461
+eero.online
+eero-stage.online
+
+// concludes Amazon
 
 // Amune : https://amune.org/
 // Submitted by Team Amune <cert@amune.org>
 t3l3p0rt.net
 tele.amune.org
 
 // Apigee : https://apigee.com/
@@ -10814,14 +10401,18 @@
 // Submitted by Sam Smyth <devloop@atlassian.com>
 cdn.prod.atlassian-dev.net
 
 // Authentick UG (haftungsbeschränkt) : https://authentick.net
 // Submitted by Lukas Reschke <lukas@authentick.net>
 translated.page
 
+// Autocode : https://autocode.com
+// Submitted by Jacob Lee <jacob@autocode.com>
+autocode.dev
+
 // AVM : https://avm.de
 // Submitted by Andreas Weise <a.weise@avm.de>
 myfritz.net
 
 // AVStack Pte. Ltd. : https://avstack.io
 // Submitted by Jasper Hugo <jasper@avstack.io>
 onavstack.net
@@ -10867,14 +10458,18 @@
 handcrafted.jp
 kawaiishop.jp
 supersale.jp
 theshop.jp
 shopselect.net
 base.shop
 
+// BeagleBoard.org Foundation : https://beagleboard.org
+// Submitted by Jason Kridner <jkridner@beagleboard.org>
+beagleboard.io
+
 // Beget Ltd
 // Submitted by Lev Nekrasov <lnekrasov@beget.com>
 *.beget.app
 
 // BetaInABox
 // Submitted by Adrian <adrian@betainabox.com>
 betainabox.com
@@ -10938,14 +10533,19 @@
 // Submitted by Antonio Lain <antlai@cafjs.com>
 cafjs.com
 
 // callidomus : https://www.callidomus.com/
 // Submitted by Marcus Popp <admin@callidomus.com>
 mycd.eu
 
+// Canva Pty Ltd : https://canva.com/
+// Submitted by Joel Aquilina <publicsuffixlist@canva.com>
+canva-apps.cn
+canva-apps.com
+
 // Carrd : https://carrd.co
 // Submitted by AJ <aj@carrd.co>
 drr.ac
 uwu.ai
 carrd.co
 crd.co
 ju.mp
@@ -11067,16 +10667,19 @@
 
 // Cloudera, Inc. : https://www.cloudera.com/
 // Submitted by Kedarnath Waikar <security@cloudera.com>
 *.cloudera.site
 
 // Cloudflare, Inc. : https://www.cloudflare.com/
 // Submitted by Cloudflare Team <publicsuffixlist@cloudflare.com>
-pages.dev
+cf-ipfs.com
+cloudflare-ipfs.com
 trycloudflare.com
+pages.dev
+r2.dev
 workers.dev
 
 // Clovyr : https://clovyr.io
 // Submitted by Patrick Nielsen <patrick@clovyr.io>
 wnext.app
 
 // co.ca : http://registry.co.ca/
@@ -11645,18 +11248,18 @@
 // Submitted by Dominik Menke <dom@digineo.de>
 dynv6.net
 
 // E4YOU spol. s.r.o. : https://e4you.cz/
 // Submitted by Vladimir Dudr <info@e4you.cz>
 e4.cz
 
-// eero : https://eero.com/
-// Submitted by Yue Kang <eero-dynamic-dns@amazon.com>
-eero.online
-eero-stage.online
+// Easypanel : https://easypanel.io
+// Submitted by Andrei Canta <andrei@easypanel.io>
+easypanel.app
+easypanel.host
 
 // Elementor : Elementor Ltd.
 // Submitted by Anton Barkan <antonb@elementor.com>
 elementor.cloud
 elementor.cool
 
 // En root‽ : https://en-root.org
@@ -11852,25 +11455,30 @@
 // Submitted by Aman Gupta <aman@getchannels.com>
 channelsdvr.net
 u.channelsdvr.net
 
 // Fastly Inc. : http://www.fastly.com/
 // Submitted by Fastly Security <security@fastly.com>
 edgecompute.app
+fastly-edge.com
 fastly-terrarium.com
 fastlylb.net
 map.fastlylb.net
 freetls.fastly.net
 map.fastly.net
 a.prod.fastly.net
 global.prod.fastly.net
 a.ssl.fastly.net
 b.ssl.fastly.net
 global.ssl.fastly.net
 
+// Fastmail : https://www.fastmail.com/
+// Submitted by Marc Bradshaw <marc@fastmailteam.com>
+*.user.fm
+
 // FASTVPS EESTI OU : https://fastvps.ru/
 // Submitted by Likhachev Vasiliy <lihachev@fastvps.ru>
 fastvps-server.com
 fastvps.host
 myfast.host
 fastvps.site
 myfast.space
@@ -11939,14 +11547,18 @@
 forgeblocks.com
 id.forgerock.io
 
 // Framer : https://www.framer.com
 // Submitted by Koen Rouwhorst <koenrh@framer.com>
 framer.app
 framercanvas.com
+framer.media
+framer.photos
+framer.website
+framer.wiki
 
 // Frusky MEDIA&PR : https://www.frusky.de
 // Submitted by Victor Pupynin <hallo@frusky.de>
 *.frusky.de
 
 // RavPage : https://www.ravpage.co.il
 // Submitted by Roni Horowitz <roni@responder.co.il>
@@ -12107,14 +11719,15 @@
 itigo.jp
 jellybean.jp
 kikirara.jp
 kill.jp
 kilo.jp
 kuron.jp
 littlestar.jp
+lolipopmc.jp
 lolitapunk.jp
 lomo.jp
 lovepop.jp
 lovesick.jp
 main.jp
 mods.jp
 mond.jp
@@ -12277,14 +11890,18 @@
 blogspot.ug
 blogspot.vn
 
 // Goupile : https://goupile.fr
 // Submitted by Niels Martignene <hello@goupile.fr>
 goupile.fr
 
+// Government of the Netherlands: https://www.government.nl
+// Submitted by <domeinnaam@minaz.nl>
+gov.nl
+
 // Group 53, LLC : https://www.group53.com
 // Submitted by Tyler Todd <noc@nova53.net>
 awsmppl.com
 
 // GünstigBestellen : https://günstigbestellen.de
 // Submitted by Furkan Akkoc <info@hendelzon.de>
 günstigbestellen.de
@@ -12323,15 +11940,14 @@
 // Submitted by Tom Maher <tmaher@heroku.com>
 herokuapp.com
 herokussl.com
 
 // Hibernating Rhinos
 // Submitted by Oren Eini <oren@ravendb.net>
 ravendb.cloud
-myravendb.com
 ravendb.community
 ravendb.me
 development.run
 ravendb.run
 
 // home.pl S.A.: https://home.pl
 // Submitted by Krzysztof Wolski <krzysztof.wolski@home.eu>
@@ -12353,15 +11969,18 @@
 col.ng
 firm.ng
 gen.ng
 ltd.ng
 ngo.ng
 edu.scot
 sch.so
-org.yt
+
+// HostFly : https://www.ie.ua
+// Submitted by Bohdan Dub <support@hostfly.com.ua>
+ie.ua
 
 // HostyHosting (hostyhosting.com)
 hostyhosting.io
 
 // Häkkinen.fi
 // Submitted by Eero Häkkinen <Eero+psl@Häkkinen.fi>
 häkkinen.fi
@@ -12371,14 +11990,19 @@
 *.moonscale.io
 moonscale.net
 
 // iki.fi
 // Submitted by Hannu Aronsson <haa@iki.fi>
 iki.fi
 
+// iliad italia: https://www.iliad.it
+// Submitted by Marios Makassikis <mmakassikis@freebox.fr>
+ibxos.it
+iliadboxos.it
+
 // Impertrix Solutions : <https://impertrixcdn.com>
 // Submitted by Zhixiang Zhao <csuite@impertrix.com>
 impertrixcdn.com
 impertrix.com
 
 // Incsub, LLC: https://incsub.com/
 // Submitted by Aaron Edwards <sysadmins@incsub.com>
@@ -12451,17 +12075,19 @@
 // Submitted by Roman Azarenko <roman.azarenko@iopsys.eu>
 iopsys.se
 
 // IPiFony Systems, Inc. : https://www.ipifony.com/
 // Submitted by Matthew Hardeman <mhardeman@ipifony.com>
 ipifony.net
 
-// IServ GmbH : https://iserv.eu
-// Submitted by Kim-Alexander Brodowski <info@iserv.eu>
+// IServ GmbH : https://iserv.de
+// Submitted by Mario Hoberg <info@iserv.de>
+iservschule.de
 mein-iserv.de
+schulplattform.de
 schulserver.de
 test-iserv.de
 iserv.dev
 
 // I-O DATA DEVICE, INC. : http://www.iodata.com/
 // Submitted by Yuji Minagawa <domains-admin@iodata.jp>
 iobb.net
@@ -12775,14 +12401,18 @@
 hra.health
 
 // Memset hosting : https://www.memset.com
 // Submitted by Tom Whitwell <domains@memset.com>
 miniserver.com
 memset.net
 
+// Messerli Informatik AG : https://www.messerli.ch/
+// Submitted by Ruben Schmidmeister <psl-maintainers@messerli.ch>
+messerli.app
+
 // MetaCentrum, CESNET z.s.p.o. : https://www.metacentrum.cz/en/
 // Submitted by Zdeněk Šustr <zdenek.sustr@cesnet.cz>
 *.cloud.metacentrum.cz
 custom.metacentrum.cz
 
 // MetaCentrum, CESNET z.s.p.o. : https://www.metacentrum.cz/en/
 // Submitted by Radim Janča <janca@cesnet.cz>
@@ -12801,14 +12431,16 @@
 // Submitted by Public Suffix List Admin <msftpsladmin@microsoft.com>
 *.azurecontainer.io
 azurewebsites.net
 azure-mobile.net
 cloudapp.net
 azurestaticapps.net
 1.azurestaticapps.net
+2.azurestaticapps.net
+3.azurestaticapps.net
 centralus.azurestaticapps.net
 eastasia.azurestaticapps.net
 eastus2.azurestaticapps.net
 westeurope.azurestaticapps.net
 westus2.azurestaticapps.net
 
 // minion.systems : http://minion.systems
@@ -12853,48 +12485,41 @@
 yali.mythic-beasts.com
 cust.retrosnub.co.uk
 
 // Nabu Casa : https://www.nabucasa.com
 // Submitted by Paulus Schoutsen <infra@nabucasa.com>
 ui.nabu.casa
 
-// Names.of.London : https://names.of.london/
-// Submitted by James Stevens <registry[at]names.of.london> or <publiclist[at]jrcs.net>
-pony.club
-of.fashion
-in.london
-of.london
-from.marketing
-with.marketing
-for.men
-repair.men
-and.mom
-for.mom
-for.one
-under.one
-for.sale
-that.win
-from.work
-to.work
-
 // Net at Work Gmbh : https://www.netatwork.de
 // Submitted by Jan Jaeschke <jan.jaeschke@netatwork.de>
 cloud.nospamproxy.com
 
 // Netlify : https://www.netlify.com
 // Submitted by Jessica Parsons <jessica@netlify.com>
 netlify.app
 
 // Neustar Inc.
 // Submitted by Trung Tran <Trung.Tran@neustar.biz>
 4u.com
 
 // ngrok : https://ngrok.com/
 // Submitted by Alan Shreve <alan@ngrok.com>
+ngrok.app
+ngrok-free.app
+ngrok.dev
+ngrok-free.dev
 ngrok.io
+ap.ngrok.io
+au.ngrok.io
+eu.ngrok.io
+in.ngrok.io
+jp.ngrok.io
+sa.ngrok.io
+us.ngrok.io
+ngrok.pizza
 
 // Nimbus Hosting Ltd. : https://www.nimbushosting.co.uk/
 // Submitted by Nicholas Ford <nick@nimbushosting.co.uk>
 nh-serv.co.uk
 
 // NFSN, Inc. : https://www.NearlyFreeSpeech.NET/
 // Submitted by Jeff Wheelhouse <support@nearlyfreespeech.net>
@@ -13068,15 +12693,34 @@
 
 // OmniWe Limited: https://omniwe.com
 // Submitted by Vicary Archangel <vicary@omniwe.com>
 omniwe.site
 
 // One.com: https://www.one.com/
 // Submitted by Jacob Bunk Nielsen <jbn@one.com>
+123hjemmeside.dk
+123hjemmeside.no
+123homepage.it
+123kotisivu.fi
+123minsida.se
+123miweb.es
+123paginaweb.pt
+123sait.ru
+123siteweb.fr
+123webseite.at
+123webseite.de
+123website.be
+123website.ch
+123website.lu
+123website.nl
 service.one
+simplesite.com
+simplesite.com.br
+simplesite.gr
+simplesite.pl
 
 // One Fold Media : http://www.onefoldmedia.com/
 // Submitted by Eddie Jones <eddie@onefoldmedia.com>
 nid.io
 
 // Open Social : https://www.getopensocial.com/
 // Submitted by Alexander Varwijk <security@getopensocial.com>
@@ -13264,14 +12908,18 @@
 // Submitted by Jeffrey Phillips Freeman <jeffrey.freeman@qoto.org>
 qoto.io
 
 // Qualifio : https://qualifio.com/
 // Submitted by Xavier De Cock <xdecock@gmail.com>
 qualifioapp.com
 
+// Quality Unit: https://qualityunit.com
+// Submitted by Vasyl Tsalko <vtsalko@qualityunit.com>
+ladesk.com
+
 // QuickBackend: https://www.quickbackend.com
 // Submitted by Dani Biro <dani@pymet.com>
 qbuser.com
 
 // Rad Web Hosting: https://radwebhosting.com
 // Submitted by Scott Claeys <s.claeys@radwebhosting.com>
 cloudsite.builders
@@ -13337,15 +12985,17 @@
 
 // Render : https://render.com
 // Submitted by Anurag Goel <dev@render.com>
 app.render.com
 onrender.com
 
 // Repl.it : https://repl.it
-// Submitted by Mason Clayton <mason@repl.it>
+// Submitted by Lincoln Bergeson <lincoln@replit.com>
+firewalledreplit.co
+id.firewalledreplit.co
 repl.co
 id.repl.co
 repl.run
 
 // Resin.io : https://resin.io
 // Submitted by Tim Perry <tim@resin.io>
 resindevice.io
@@ -13385,14 +13035,70 @@
 мск.рус
 орг.рус
 самара.рус
 сочи.рус
 спб.рус
 я.рус
 
+// SAKURA Internet Inc. : https://www.sakura.ad.jp/
+// Submitted by Internet Service Department <rs-vendor-ml@sakura.ad.jp>
+180r.com
+dojin.com
+sakuratan.com
+sakuraweb.com
+x0.com
+2-d.jp
+bona.jp
+crap.jp
+daynight.jp
+eek.jp
+flop.jp
+halfmoon.jp
+jeez.jp
+matrix.jp
+mimoza.jp
+ivory.ne.jp
+mail-box.ne.jp
+mints.ne.jp
+mokuren.ne.jp
+opal.ne.jp
+sakura.ne.jp
+sumomo.ne.jp
+topaz.ne.jp
+netgamers.jp
+nyanta.jp
+o0o0.jp
+rdy.jp
+rgr.jp
+rulez.jp
+s3.isk01.sakurastorage.jp
+s3.isk02.sakurastorage.jp
+saloon.jp
+sblo.jp
+skr.jp
+tank.jp
+uh-oh.jp
+undo.jp
+rs.webaccel.jp
+user.webaccel.jp
+websozai.jp
+xii.jp
+squares.net
+jpn.org
+kirara.st
+x0.to
+from.tv
+sakura.tv
+
+// Salesforce.com, Inc. https://salesforce.com/
+// Submitted by Michael Biven <mbiven@salesforce.com>
+*.builder.code.com
+*.dev-builder.code.com
+*.stg-builder.code.com
+
 // Sandstorm Development Group, Inc. : https://sandcats.io/
 // Submitted by Asheesh Laroia <asheesh@sandstorm.io>
 sandcats.io
 
 // SBE network solutions GmbH : https://www.sbe.de/
 // Submitted by Norman Meilick <nm@sbe.de>
 logoip.de
@@ -13529,14 +13235,21 @@
 // Submitted by Aral Balkan <aral@small-tech.org>
 small-web.org
 
 // Smoove.io : https://www.smoove.io/
 // Submitted by Dan Kozak <dan@smoove.io>
 vp4.me
 
+// Snowflake Inc : https://www.snowflake.com/
+// Submitted by Faith Olapade <faith.olapade@snowflake.com>
+snowflake.app
+privatelink.snowflake.app
+streamlit.app
+streamlitapp.com
+
 // Snowplow Analytics : https://snowplowanalytics.com/
 // Submitted by Ian Streeter <ian@snowplowanalytics.com>
 try-snowplow.com
 
 // SourceHut : https://sourcehut.org
 // Submitted by Drew DeVault <sir@cmpwn.com>
 srht.site
@@ -13662,14 +13375,16 @@
 familyds.org
 vpnplus.to
 direct.quickconnect.to
 
 // Tabit Technologies Ltd. : https://tabit.cloud/
 // Submitted by Oren Agiv <oren@tabit.cloud>
 tabitorder.co.il
+mytabit.co.il
+mytabit.com
 
 // TAIFUN Software AG : http://taifun-software.de
 // Submitted by Bjoern Henke <dev-server@taifun-software.de>
 taifun-dns.de
 
 // Tailscale Inc. : https://www.tailscale.com
 // Submitted by David Anderson <danderson@tailscale.com>
@@ -13694,18 +13409,14 @@
 
 // Telebit : https://telebit.cloud
 // Submitted by AJ ONeal <aj@telebit.cloud>
 telebit.app
 telebit.io
 *.telebit.xyz
 
-// The Gwiddle Foundation : https://gwiddlefoundation.org.uk
-// Submitted by Joshua Bayfield <joshua.bayfield@gwiddlefoundation.org.uk>
-gwiddle.co.uk
-
 // Thingdust AG : https://thingdust.com/
 // Submitted by Adrian Imboden <adi@thingdust.com>
 *.firenet.ch
 *.svc.firenet.ch
 reservd.com
 thingdustdata.com
 cust.dev.thingdust.io
@@ -13732,18 +13443,14 @@
 pages.torproject.net
 
 // TownNews.com : http://www.townnews.com
 // Submitted by Dustin Ward <dward@townnews.com>
 bloxcms.com
 townnews-staging.com
 
-// TradableBits: https://tradablebits.com
-// Submitted by Dmitry Khrisanov dmitry@tradablebits.com
-tbits.me
-
 // TrafficPlex GmbH : https://www.trafficplex.de/
 // Submitted by Phillipp Röll <phillipp.roell@trafficplex.de>
 12hp.at
 2ix.at
 4lima.at
 lima-city.at
 12hp.ch
@@ -13808,14 +13515,27 @@
 // UDR Limited : http://www.udr.hk.com
 // Submitted by registry <hostmaster@udr.hk.com>
 hk.com
 hk.org
 ltd.hk
 inc.hk
 
+// UK Intis Telecom LTD : https://it.com
+// Submitted by ITComdomains <to@it.com>
+it.com
+
+// UNIVERSAL DOMAIN REGISTRY : https://www.udr.org.yt/
+// see also: whois -h whois.udr.org.yt help
+// Submitted by Atanunu Igbunuroghene <publicsuffixlist@udr.org.yt>
+name.pm
+sch.tf
+biz.wf
+sch.wf
+org.yt
+
 // United Gameserver GmbH : https://united-gameserver.de
 // Submitted by Stefan Schwarz <sysadm@united-gameserver.de>
 virtualuser.de
 virtual-user.de
 
 // Upli : https://upli.io
 // Submitted by Lenny Bakkalian <lenny.bakkalian@gmail.com>
```

### Comparing `tldextract-3.4.0/tldextract/cache.py` & `tldextract-3.4.1/tldextract/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             with open(cache_filepath) as cache_file:
                 return json.load(cache_file)
         except (OSError, ValueError) as exc:
             LOG.error("error reading TLD cache file %s: %s", cache_filepath, exc)
             raise KeyError("namespace: " + namespace + " key: " + repr(key)) from None
 
     def set(
-        self, namespace: str, key: Union[str, Dict[str, Hashable]], value: T
+        self, namespace: str, key: Union[str, Dict[str, Hashable]], value: object
     ) -> None:
         """Set a value in the disk cache"""
         if not self.enabled:
             return
 
         cache_filepath = self._key_to_cachefile_path(namespace, key)
```

### Comparing `tldextract-3.4.0/tldextract/cli.py` & `tldextract-3.4.1/tldextract/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,11 +82,10 @@
     tld_extract = TLDExtract(**obj_kwargs)
 
     if args.update:
         tld_extract.update(True)
     elif not args.input:
         parser.print_usage()
         sys.exit(1)
-        return
 
     for i in args.input:
         print(" ".join(tld_extract(i)))
```

### Comparing `tldextract-3.4.0/tldextract/remote.py` & `tldextract-3.4.1/tldextract/remote.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.0/tldextract/suffix_list.py` & `tldextract-3.4.1/tldextract/suffix_list.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.0/tldextract/tldextract.py` & `tldextract-3.4.1/tldextract/tldextract.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.0/tldextract.egg-info/PKG-INFO` & `tldextract-3.4.1/tldextract.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: tldextract
-Version: 3.4.0
+Version: 3.4.1
 Summary: Accurately separates a URL's subdomain, domain, and public suffix, using the Public Suffix List (PSL). By default, this includes the public ICANN TLDs and their exceptions. You can optionally support the Public Suffix List's private domains as well.
 Home-page: https://github.com/john-kurkowski/tldextract
 Author: John Kurkowski
 Author-email: john.kurkowski@gmail.com
-License: BSD License
+License: BSD-3-Clause
 Keywords: tld domain subdomain url parse extract urlparse urlsplit public suffix list publicsuffix publicsuffixlist
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  `tldextract` accurately separates a URL's subdomain, domain, and public suffix,
 using the Public Suffix List (PSL).
```

### Comparing `tldextract-3.4.0/tldextract.egg-info/SOURCES.txt` & `tldextract-3.4.1/tldextract.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 .travis.yml
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 conftest.py
-pylintrc
 pytest.ini
 setup.cfg
 setup.py
 tox.ini
 .github/FUNDING.yml
 tests/__init__.py
 tests/cli_test.py
```


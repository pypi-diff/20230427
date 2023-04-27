# Comparing `tmp/boringavatars-1.0.0.tar.gz` & `tmp/boringavatars-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boringavatars-1.0.0.tar", last modified: Thu Apr 27 14:52:12 2023, max compression
+gzip compressed data, was "boringavatars-1.0.1.tar", last modified: Thu Apr 27 21:29:57 2023, max compression
```

## Comparing `boringavatars-1.0.0.tar` & `boringavatars-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1715 2022-12-28 00:28:05.446313 boringavatars-1.0.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      160 2022-12-28 02:51:41.071111 boringavatars-1.0.0/.flake8
--rw-r--r--   0        0        0      232 2022-12-27 23:30:38.713764 boringavatars-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1799 2022-12-19 18:05:58.284258 boringavatars-1.0.0/.gitignore
--rw-r--r--   0        0        0     1481 2022-12-28 02:54:09.917879 boringavatars-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2022-12-19 18:05:58.284389 boringavatars-1.0.0/.pypirc
--rw-r--r--   0        0        0       99 2022-12-19 18:05:58.284480 boringavatars-1.0.0/.vscode/extensions.json
--rw-r--r--   0        0        0      127 2022-12-19 18:05:58.284537 boringavatars-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0     1133 2022-12-28 02:49:57.273427 boringavatars-1.0.0/LICENSE
--rw-r--r--   0        0        0      595 2022-12-28 04:17:59.054029 boringavatars-1.0.0/README.md
--rw-r--r--   0        0        0     1508 2023-04-27 14:48:30.715137 boringavatars-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       46 2022-12-28 00:17:00.765116 boringavatars-1.0.0/requirements.txt
--rw-r--r--   0        0        0      901 2023-04-27 14:49:22.705903 boringavatars-1.0.0/src/boringavatars/__init__.py
--rw-r--r--   0        0        0      961 2022-12-28 04:10:56.288387 boringavatars-1.0.0/src/boringavatars/bauhaus.py
--rw-r--r--   0        0        0     1849 2022-12-28 04:11:08.947816 boringavatars-1.0.0/src/boringavatars/beam.py
--rw-r--r--   0        0        0      950 2022-12-28 04:11:15.850865 boringavatars-1.0.0/src/boringavatars/marble.py
--rw-r--r--   0        0        0      621 2022-12-28 04:11:24.008327 boringavatars-1.0.0/src/boringavatars/pixel.py
--rw-r--r--   0        0        0        0 2023-03-10 05:08:45.843083 boringavatars-1.0.0/src/boringavatars/py.typed
--rw-r--r--   0        0        0      879 2022-12-28 04:11:44.524937 boringavatars-1.0.0/src/boringavatars/ring.py
--rw-r--r--   0        0        0      693 2022-12-28 04:11:33.663675 boringavatars-1.0.0/src/boringavatars/sunset.py
--rw-r--r--   0        0        0     1510 2023-03-28 18:26:32.049497 boringavatars-1.0.0/src/boringavatars/templates/bauhaus.svg
--rw-r--r--   0        0        0     1782 2023-03-28 18:23:50.460090 boringavatars-1.0.0/src/boringavatars/templates/beam.svg
--rw-r--r--   0        0        0     1794 2022-12-28 04:04:39.371872 boringavatars-1.0.0/src/boringavatars/templates/marble.svg
--rw-r--r--   0        0        0     5592 2022-12-28 04:04:45.953148 boringavatars-1.0.0/src/boringavatars/templates/pixel.svg
--rw-r--r--   0        0        0     1105 2022-12-28 04:04:49.621227 boringavatars-1.0.0/src/boringavatars/templates/ring.svg
--rw-r--r--   0        0        0     1340 2022-12-28 04:04:51.745639 boringavatars-1.0.0/src/boringavatars/templates/sunset.svg
--rw-r--r--   0        0        0     1381 2022-12-28 04:29:33.256766 boringavatars-1.0.0/src/boringavatars/utils.py
--rw-r--r--   0        0        0      214 2022-12-28 04:17:17.661063 boringavatars-1.0.0/tests/test_avatars.py
--rw-r--r--   0        0        0     2231 1970-01-01 00:00:00.000000 boringavatars-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1715 2022-12-28 00:28:05.446313 boringavatars-1.0.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      160 2022-12-28 02:51:41.071111 boringavatars-1.0.1/.flake8
+-rw-r--r--   0        0        0      232 2022-12-27 23:30:38.713764 boringavatars-1.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1799 2022-12-19 18:05:58.284258 boringavatars-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1481 2022-12-28 02:54:09.917879 boringavatars-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2022-12-19 18:05:58.284389 boringavatars-1.0.1/.pypirc
+-rw-r--r--   0        0        0       99 2022-12-19 18:05:58.284480 boringavatars-1.0.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      127 2022-12-19 18:05:58.284537 boringavatars-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1133 2022-12-28 02:49:57.273427 boringavatars-1.0.1/LICENSE
+-rw-r--r--   0        0        0      595 2022-12-28 04:17:59.054029 boringavatars-1.0.1/README.md
+-rw-r--r--   0        0        0     1508 2023-04-27 14:48:30.715137 boringavatars-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       46 2022-12-28 00:17:00.765116 boringavatars-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      901 2023-04-27 21:19:26.315811 boringavatars-1.0.1/src/boringavatars/__init__.py
+-rw-r--r--   0        0        0      961 2022-12-28 04:10:56.288387 boringavatars-1.0.1/src/boringavatars/bauhaus.py
+-rw-r--r--   0        0        0     1849 2022-12-28 04:11:08.947816 boringavatars-1.0.1/src/boringavatars/beam.py
+-rw-r--r--   0        0        0      950 2022-12-28 04:11:15.850865 boringavatars-1.0.1/src/boringavatars/marble.py
+-rw-r--r--   0        0        0      621 2022-12-28 04:11:24.008327 boringavatars-1.0.1/src/boringavatars/pixel.py
+-rw-r--r--   0        0        0        0 2023-03-10 05:08:45.843083 boringavatars-1.0.1/src/boringavatars/py.typed
+-rw-r--r--   0        0        0      879 2022-12-28 04:11:44.524937 boringavatars-1.0.1/src/boringavatars/ring.py
+-rw-r--r--   0        0        0      693 2022-12-28 04:11:33.663675 boringavatars-1.0.1/src/boringavatars/sunset.py
+-rw-r--r--   0        0        0     1510 2023-03-28 18:26:32.049497 boringavatars-1.0.1/src/boringavatars/templates/bauhaus.svg
+-rw-r--r--   0        0        0     1782 2023-03-28 18:23:50.460090 boringavatars-1.0.1/src/boringavatars/templates/beam.svg
+-rw-r--r--   0        0        0     1794 2022-12-28 04:04:39.371872 boringavatars-1.0.1/src/boringavatars/templates/marble.svg
+-rw-r--r--   0        0        0     5592 2022-12-28 04:04:45.953148 boringavatars-1.0.1/src/boringavatars/templates/pixel.svg
+-rw-r--r--   0        0        0     1105 2022-12-28 04:04:49.621227 boringavatars-1.0.1/src/boringavatars/templates/ring.svg
+-rw-r--r--   0        0        0     1340 2022-12-28 04:04:51.745639 boringavatars-1.0.1/src/boringavatars/templates/sunset.svg
+-rw-r--r--   0        0        0     1387 2023-04-27 21:16:18.231905 boringavatars-1.0.1/src/boringavatars/utils.py
+-rw-r--r--   0        0        0      214 2022-12-28 04:17:17.661063 boringavatars-1.0.1/tests/test_avatars.py
+-rw-r--r--   0        0        0     2231 1970-01-01 00:00:00.000000 boringavatars-1.0.1/PKG-INFO
```

### Comparing `boringavatars-1.0.0/.devcontainer/devcontainer.json` & `boringavatars-1.0.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/.gitignore` & `boringavatars-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/.pre-commit-config.yaml` & `boringavatars-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/LICENSE` & `boringavatars-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/README.md` & `boringavatars-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/pyproject.toml` & `boringavatars-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/__init__.py` & `boringavatars-1.0.1/src/boringavatars/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .bauhaus import bauhaus
 from .beam import beam
 from .marble import marble
 from .pixel import pixel
 from .ring import ring
 from .sunset import sunset
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 __all__ = ["avatar"]
 
 DEFAULT_COLORS = ["FFAD08", "EDD75A", "73B06F", "0C8F8F", "405059"]
 
 VARIANTS = {
     "beam": beam,
```

### Comparing `boringavatars-1.0.0/src/boringavatars/bauhaus.py` & `boringavatars-1.0.1/src/boringavatars/bauhaus.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/beam.py` & `boringavatars-1.0.1/src/boringavatars/beam.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/marble.py` & `boringavatars-1.0.1/src/boringavatars/marble.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/pixel.py` & `boringavatars-1.0.1/src/boringavatars/pixel.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/ring.py` & `boringavatars-1.0.1/src/boringavatars/ring.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/sunset.py` & `boringavatars-1.0.1/src/boringavatars/sunset.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/templates/bauhaus.svg` & `boringavatars-1.0.1/src/boringavatars/templates/bauhaus.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/templates/beam.svg` & `boringavatars-1.0.1/src/boringavatars/templates/beam.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/templates/marble.svg` & `boringavatars-1.0.1/src/boringavatars/templates/marble.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/templates/pixel.svg` & `boringavatars-1.0.1/src/boringavatars/templates/pixel.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/templates/ring.svg` & `boringavatars-1.0.1/src/boringavatars/templates/ring.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/templates/sunset.svg` & `boringavatars-1.0.1/src/boringavatars/templates/sunset.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.0/src/boringavatars/utils.py` & `boringavatars-1.0.1/src/boringavatars/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def hash_code(name):
     return int.from_bytes(hashlib.sha1(name.encode("utf-8")).digest(), byteorder="big")
 
 
 def get_digit(number, ntn):
-    return math.floor((number / math.pow(10, ntn)) % 10)
+    return math.floor((number // int(math.pow(10, ntn))) % 10)
 
 
 def get_boolean(number, ntn):
     return not ((get_digit(number, ntn)) % 2)
 
 
 def get_angle(x, y):
```

### Comparing `boringavatars-1.0.0/PKG-INFO` & `boringavatars-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boringavatars
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author-email: Federico Bond <federicobond@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boringavatars Version: 1.0.0 Summary: Author-email:
+Metadata-Version: 2.1 Name: boringavatars Version: 1.0.1 Summary: Author-email:
 Federico Bond
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```


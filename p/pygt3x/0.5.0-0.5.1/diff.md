# Comparing `tmp/pygt3x-0.5.0.tar.gz` & `tmp/pygt3x-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygt3x-0.5.0.tar", max compression
+gzip compressed data, was "pygt3x-0.5.1.tar", max compression
```

## Comparing `pygt3x-0.5.0.tar` & `pygt3x-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-02-22 13:23:41.054005 pygt3x-0.5.0/LICENSE
--rw-r--r--   0        0        0      765 2023-02-22 13:23:41.054005 pygt3x-0.5.0/README.md
--rw-r--r--   0        0        0      688 2023-02-22 13:23:41.054005 pygt3x-0.5.0/pygt3x/__init__.py
--rw-r--r--   0        0        0     3857 2023-02-22 13:23:41.054005 pygt3x-0.5.0/pygt3x/activity_payload.py
--rw-r--r--   0        0        0     2696 2023-02-22 13:23:41.054005 pygt3x-0.5.0/pygt3x/calibration.py
--rw-r--r--   0        0        0     4886 2023-02-22 13:23:41.054005 pygt3x-0.5.0/pygt3x/components.py
--rw-r--r--   0        0        0    15815 2023-02-22 13:23:41.054005 pygt3x-0.5.0/pygt3x/reader.py
--rw-r--r--   0        0        0      765 2023-02-22 13:23:41.054005 pygt3x-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 pygt3x-0.5.0/setup.py
--rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 pygt3x-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 15:24:01.356322 pygt3x-0.5.1/LICENSE
+-rw-r--r--   0        0        0      765 2023-04-27 15:24:01.356322 pygt3x-0.5.1/README.md
+-rw-r--r--   0        0        0      688 2023-04-27 15:24:01.356322 pygt3x-0.5.1/pygt3x/__init__.py
+-rw-r--r--   0        0        0     3857 2023-04-27 15:24:01.356322 pygt3x-0.5.1/pygt3x/activity_payload.py
+-rw-r--r--   0        0        0     2696 2023-04-27 15:24:01.356322 pygt3x-0.5.1/pygt3x/calibration.py
+-rw-r--r--   0        0        0     4886 2023-04-27 15:24:01.356322 pygt3x-0.5.1/pygt3x/components.py
+-rw-r--r--   0        0        0    15856 2023-04-27 15:24:01.356322 pygt3x-0.5.1/pygt3x/reader.py
+-rw-r--r--   0        0        0      765 2023-04-27 15:24:01.356322 pygt3x-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 pygt3x-0.5.1/setup.py
+-rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 pygt3x-0.5.1/PKG-INFO
```

### Comparing `pygt3x-0.5.0/LICENSE` & `pygt3x-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygt3x-0.5.0/README.md` & `pygt3x-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pygt3x-0.5.0/pygt3x/__init__.py` & `pygt3x-0.5.1/pygt3x/__init__.py`

 * *Files identical despite different names*

### Comparing `pygt3x-0.5.0/pygt3x/activity_payload.py` & `pygt3x-0.5.1/pygt3x/activity_payload.py`

 * *Files identical despite different names*

### Comparing `pygt3x-0.5.0/pygt3x/calibration.py` & `pygt3x-0.5.1/pygt3x/calibration.py`

 * *Files identical despite different names*

### Comparing `pygt3x-0.5.0/pygt3x/components.py` & `pygt3x-0.5.1/pygt3x/components.py`

 * *Files identical despite different names*

### Comparing `pygt3x-0.5.0/pygt3x/reader.py` & `pygt3x-0.5.1/pygt3x/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,17 @@
         timestamps = (
             np.arange(idle_sleep_mode_started, idle_sleep_mode_ended)
             .repeat(self.info.sample_rate)
             .reshape(-1, 1)
         )
         values = last_values.reshape((1, 3)).repeat(timestamps.shape[0], axis=0)
 
-        result = np.concatenate((timestamps, values), axis=1).reshape((-1, 30, 4))
+        result = np.concatenate((timestamps, values), axis=1).reshape(
+            (-1, self.info.sample_rate, 4)
+        )
         return result
 
     def _validate_payload(self, payload):
         shape = payload.shape
         expected_shape = (self.info.sample_rate, 4)
         if shape[1:] != expected_shape and shape != expected_shape:
             self.logger.warning(f"Unexpected payload shape {shape}")
```

### Comparing `pygt3x-0.5.0/pyproject.toml` & `pygt3x-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygt3x"
-version = "0.5.0"
+version = "0.5.1"
 description = "Python module for reading GT3X/AGDC file format data"
 authors = ["Mark Fogle <mark.fogle@theactigraph.com>"]
 maintainers = ["Ali Neishabouri <ali.neishabouri@theactigraph.com>"]
 license = "GPL-3.0-or-later"
 repository = "https://github.com/actigraph/pygt3x"
 readme = "README.md"
```

### Comparing `pygt3x-0.5.0/setup.py` & `pygt3x-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.21.2', 'pandas>=1.2.5']
 
 setup_kwargs = {
     'name': 'pygt3x',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'Python module for reading GT3X/AGDC file format data',
     'long_description': '# pygt3x\n![Tests](https://github.com/actigraph/pygt3x/actions/workflows/tests.yml/badge.svg)\n\nPython module for reading GT3X/AGDC file format data generated by ActiGraph devices.\n\n## Example Usage\n\nTo read calibrated accelerometer data, you can use the code snippet below:\n\n```python\nfrom pygt3x.reader import FileReader\n\n# Read raw data and calibrate, then export to pandas data frame\nwith FileReader("FILENAME") as reader:\n    was_idle_sleep_mode_used = reader.idle_sleep_mode_activated\n    df = reader.to_pandas()\n    print(df.head(5))\n```\n\nIf your AGDC file contains temperature data, you can read it using:\n\n```python\nfrom pygt3x.reader import FileReader\n\nwith FileReader("FILENAME") as reader:\n    df = reader.temperature_to_pandas()\n    print(df.head(5))\n```',
     'author': 'Mark Fogle',
     'author_email': 'mark.fogle@theactigraph.com',
     'maintainer': 'Ali Neishabouri',
     'maintainer_email': 'ali.neishabouri@theactigraph.com',
     'url': 'https://github.com/actigraph/pygt3x',
```

### Comparing `pygt3x-0.5.0/PKG-INFO` & `pygt3x-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygt3x
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python module for reading GT3X/AGDC file format data
 Home-page: https://github.com/actigraph/pygt3x
 License: GPL-3.0-or-later
 Author: Mark Fogle
 Author-email: mark.fogle@theactigraph.com
 Maintainer: Ali Neishabouri
 Maintainer-email: ali.neishabouri@theactigraph.com
```


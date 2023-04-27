# Comparing `tmp/micropython-icm20948-0.1.0.tar.gz` & `tmp/micropython-icm20948-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-icm20948-0.1.0.tar", last modified: Wed Apr 26 13:51:11 2023, max compression
+gzip compressed data, was "micropython-icm20948-0.2.0.tar", last modified: Thu Apr 27 00:11:46 2023, max compression
```

## Comparing `micropython-icm20948-0.1.0.tar` & `micropython-icm20948-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:51:11.111178 micropython-icm20948-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:51:11.103179 micropython-icm20948-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:51:11.107179 micropython-icm20948-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-26 13:51:11.111178 micropython-icm20948-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:51:11.107179 micropython-icm20948-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:51:11.107179 micropython-icm20948-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:51:11.107179 micropython-icm20948-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 13:50:59.000000 micropython-icm20948-0.1.0/examples/icm20948_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:51:11.107179 micropython-icm20948-0.1.0/micropython_icm20948/
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-26 13:50:59.000000 micropython-icm20948-0.1.0/micropython_icm20948/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-04-26 13:50:59.000000 micropython-icm20948-0.1.0/micropython_icm20948/icm20948.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:51:11.107179 micropython-icm20948-0.1.0/micropython_icm20948.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-26 13:51:11.000000 micropython-icm20948-0.1.0/micropython_icm20948.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-26 13:51:11.000000 micropython-icm20948-0.1.0/micropython_icm20948.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:51:11.000000 micropython-icm20948-0.1.0/micropython_icm20948.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 13:51:11.000000 micropython-icm20948-0.1.0/micropython_icm20948.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 13:51:11.000000 micropython-icm20948-0.1.0/micropython_icm20948.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-26 13:50:59.000000 micropython-icm20948-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 13:50:41.000000 micropython-icm20948-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 13:51:11.111178 micropython-icm20948-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.951321 micropython-icm20948-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.939321 micropython-icm20948-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.943321 micropython-icm20948-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-27 00:11:46.951321 micropython-icm20948-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.947321 micropython-icm20948-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.947321 micropython-icm20948-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.947321 micropython-icm20948-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-27 00:11:38.000000 micropython-icm20948-0.2.0/examples/icm20948_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.947321 micropython-icm20948-0.2.0/micropython_icm20948/
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-27 00:11:38.000000 micropython-icm20948-0.2.0/micropython_icm20948/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23466 2023-04-27 00:11:38.000000 micropython-icm20948-0.2.0/micropython_icm20948/icm20948.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.951321 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-27 00:11:46.000000 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-27 00:11:46.000000 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:11:46.000000 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 00:11:46.000000 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 00:11:46.000000 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-27 00:11:38.000000 micropython-icm20948-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 00:11:46.951321 micropython-icm20948-0.2.0/setup.cfg
```

### Comparing `micropython-icm20948-0.1.0/.gitignore` & `micropython-icm20948-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.1.0/.pre-commit-config.yaml` & `micropython-icm20948-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.1.0/.pylintrc` & `micropython-icm20948-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.1.0/LICENSE` & `micropython-icm20948-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.1.0/PKG-INFO` & `micropython-icm20948-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-icm20948
-Version: 0.1.0
+Version: 0.2.0
 Summary: MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
 Author-email: "Jose D. Montoya" <icm20948@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ICM20948
 Keywords: micropython,icm20948,gyro,accelerometer,acceleration,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -24,14 +24,17 @@
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-icm20948.svg
     :target: https://pypi.python.org/pypi/micropython-icm20948
     :alt: PyPi Package
 
+.. image:: https://static.pepy.tech/personalized-badge/micropython-icm20948?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-icm20948
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
```

### Comparing `micropython-icm20948-0.1.0/README.rst` & `micropython-icm20948-0.2.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-icm20948.svg
     :target: https://pypi.python.org/pypi/micropython-icm20948
     :alt: PyPi Package
 
+.. image:: https://static.pepy.tech/personalized-badge/micropython-icm20948?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-icm20948
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
```

### Comparing `micropython-icm20948-0.1.0/docs/_static/Logo.png` & `micropython-icm20948-0.2.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.1.0/docs/_static/favicon.ico` & `micropython-icm20948-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.1.0/docs/conf.py` & `micropython-icm20948-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.1.0/micropython_icm20948/i2c_helpers.py` & `micropython-icm20948-0.2.0/micropython_icm20948/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.1.0/micropython_icm20948.egg-info/PKG-INFO` & `micropython-icm20948-0.2.0/micropython_icm20948.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-icm20948
-Version: 0.1.0
+Version: 0.2.0
 Summary: MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
 Author-email: "Jose D. Montoya" <icm20948@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ICM20948
 Keywords: micropython,icm20948,gyro,accelerometer,acceleration,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -24,14 +24,17 @@
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-icm20948.svg
     :target: https://pypi.python.org/pypi/micropython-icm20948
     :alt: PyPi Package
 
+.. image:: https://static.pepy.tech/personalized-badge/micropython-icm20948?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-icm20948
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
```

### Comparing `micropython-icm20948-0.1.0/micropython_icm20948.egg-info/SOURCES.txt` & `micropython-icm20948-0.2.0/micropython_icm20948.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.1.0/pyproject.toml` & `micropython-icm20948-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-icm20948"
 description = "MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor"
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "icm20948@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_ICM20948"}
 keywords = [
     "micropython",
```


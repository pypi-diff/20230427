# Comparing `tmp/virtuaaliviivakoodi-1.0.0.tar.gz` & `tmp/virtuaaliviivakoodi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtuaaliviivakoodi-1.0.0.tar", max compression
+gzip compressed data, was "virtuaaliviivakoodi-1.0.1.tar", max compression
```

## Comparing `virtuaaliviivakoodi-1.0.0.tar` & `virtuaaliviivakoodi-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3704 2022-09-29 09:22:44.148534 virtuaaliviivakoodi-1.0.0/README.md
--rw-r--r--   0        0        0      704 2022-09-29 09:23:04.412413 virtuaaliviivakoodi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       53 2022-09-29 08:29:27.032739 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/__init__.py
--rw-r--r--   0        0        0       42 2022-09-29 05:58:17.359346 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/constants/__init__.py
--rw-r--r--   0        0        0       91 2022-09-29 07:05:12.302615 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/constants/symbol_version.py
--rw-r--r--   0        0        0      346 2022-09-29 07:12:08.173841 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/exceptions/__init__.py
--rw-r--r--   0        0        0      164 2022-09-29 06:45:27.310713 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/normalizers/__init__.py
--rw-r--r--   0        0        0      208 2022-09-29 06:39:05.498064 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/normalizers/due_date.py
--rw-r--r--   0        0        0      438 2022-09-29 08:36:20.696505 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/normalizers/euro_amount.py
--rw-r--r--   0        0        0      211 2022-09-29 08:36:22.995635 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/normalizers/iban.py
--rw-r--r--   0        0        0      640 2022-09-29 08:36:27.579519 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/normalizers/reference.py
--rw-r--r--   0        0        0      163 2022-09-29 06:59:56.504154 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/utils/__init__.py
--rw-r--r--   0        0        0      319 2022-09-29 08:36:34.261017 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/utils/detect_symbol_version.py
--rw-r--r--   0        0        0      115 2022-09-29 07:01:39.496574 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/utils/remove_whitespace.py
--rw-r--r--   0        0        0      286 2022-09-29 07:38:05.693084 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/utils/split_euros_and_cents.py
--rw-r--r--   0        0        0      160 2022-09-29 08:03:42.297757 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/validators/__init__.py
--rw-r--r--   0        0        0      252 2022-09-29 08:36:41.761394 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/validators/due_date.py
--rw-r--r--   0        0        0      559 2022-09-29 08:36:45.180418 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/validators/euro_amount.py
--rw-r--r--   0        0        0      521 2022-09-29 08:36:49.634278 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/validators/iban.py
--rw-r--r--   0        0        0      742 2022-09-29 08:36:54.787646 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/validators/reference.py
--rw-r--r--   0        0        0     1055 2022-09-29 08:36:04.480831 virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/virtuaaliviivakoodi.py
--rw-r--r--   0        0        0     4527 1970-01-01 00:00:00.000000 virtuaaliviivakoodi-1.0.0/setup.py
--rw-r--r--   0        0        0     4222 1970-01-01 00:00:00.000000 virtuaaliviivakoodi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3704 2022-09-29 09:22:44.148534 virtuaaliviivakoodi-1.0.1/README.md
+-rw-r--r--   0        0        0      687 2023-04-27 04:54:15.652402 virtuaaliviivakoodi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       53 2022-09-29 08:29:27.032739 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/__init__.py
+-rw-r--r--   0        0        0       42 2022-09-29 05:58:17.359346 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/constants/__init__.py
+-rw-r--r--   0        0        0       91 2022-09-29 07:05:12.302615 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/constants/symbol_version.py
+-rw-r--r--   0        0        0      346 2022-09-29 07:12:08.173841 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/exceptions/__init__.py
+-rw-r--r--   0        0        0      164 2022-09-29 06:45:27.310713 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/normalizers/__init__.py
+-rw-r--r--   0        0        0      208 2022-09-29 06:39:05.498064 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/normalizers/due_date.py
+-rw-r--r--   0        0        0      438 2022-09-29 08:36:20.696505 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/normalizers/euro_amount.py
+-rw-r--r--   0        0        0      211 2022-09-29 08:36:22.995635 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/normalizers/iban.py
+-rw-r--r--   0        0        0      640 2022-09-29 08:36:27.579519 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/normalizers/reference.py
+-rw-r--r--   0        0        0      163 2022-09-29 06:59:56.504154 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/utils/__init__.py
+-rw-r--r--   0        0        0      319 2022-09-29 08:36:34.261017 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/utils/detect_symbol_version.py
+-rw-r--r--   0        0        0      115 2022-09-29 07:01:39.496574 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/utils/remove_whitespace.py
+-rw-r--r--   0        0        0      286 2022-09-29 07:38:05.693084 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/utils/split_euros_and_cents.py
+-rw-r--r--   0        0        0      160 2022-09-29 08:03:42.297757 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/validators/__init__.py
+-rw-r--r--   0        0        0      252 2022-09-29 08:36:41.761394 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/validators/due_date.py
+-rw-r--r--   0        0        0      559 2022-09-29 08:36:45.180418 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/validators/euro_amount.py
+-rw-r--r--   0        0        0      521 2022-09-29 08:36:49.634278 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/validators/iban.py
+-rw-r--r--   0        0        0      742 2022-09-29 08:36:54.787646 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/validators/reference.py
+-rw-r--r--   0        0        0     1055 2022-09-29 08:36:04.480831 virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/virtuaaliviivakoodi.py
+-rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 virtuaaliviivakoodi-1.0.1/setup.py
+-rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 virtuaaliviivakoodi-1.0.1/PKG-INFO
```

### Comparing `virtuaaliviivakoodi-1.0.0/README.md` & `virtuaaliviivakoodi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `virtuaaliviivakoodi-1.0.0/pyproject.toml` & `virtuaaliviivakoodi-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "virtuaaliviivakoodi"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python library for generating Finnish virtuaaliviivakoodi's"
 authors = ["Juho Enala <juho.enala@nocfo.io>"]
 readme = "README.md"
 license = "MIT"
 
 [project.urls]
 "Homepage" = "https://github.com/nocfo/virtuaaliviivakoodi"
 "Bug Tracker" = "https://github.com/nocfo/virtuaaliviivakoodi/issues"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8"
 
 [tool.poetry.dev-dependencies]
-unittest = "^0.0"
 black = "^22.8.0"
 isort = "^5.10.1"
 parameterized = "^0.8.1"
 pre-commit = "^2.20.0"
 pylint = "^2.15.3"
 mypy = "^0.981"
```

### Comparing `virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/normalizers/reference.py` & `virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/normalizers/reference.py`

 * *Files identical despite different names*

### Comparing `virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/validators/euro_amount.py` & `virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/validators/euro_amount.py`

 * *Files identical despite different names*

### Comparing `virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/validators/iban.py` & `virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/validators/iban.py`

 * *Files identical despite different names*

### Comparing `virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/validators/reference.py` & `virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/validators/reference.py`

 * *Files identical despite different names*

### Comparing `virtuaaliviivakoodi-1.0.0/virtuaaliviivakoodi/virtuaaliviivakoodi.py` & `virtuaaliviivakoodi-1.0.1/virtuaaliviivakoodi/virtuaaliviivakoodi.py`

 * *Files identical despite different names*

### Comparing `virtuaaliviivakoodi-1.0.0/setup.py` & `virtuaaliviivakoodi-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
  'virtuaaliviivakoodi.validators']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'virtuaaliviivakoodi',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': "Python library for generating Finnish virtuaaliviivakoodi's",
     'long_description': '# Finnish virtuaaliviivakoodi generation\n\n[![PyPI version](https://badge.fury.io/py/virtuaaliviivakoodi.svg)](https://badge.fury.io/py/virtuaaliviivakoodi)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n\nVirtuaaliviivakoodi is a Python library for generating virtual barcodes based on Finanssiala\'s [pankkiviivakoodi spec](https://www.finanssiala.fi/wp-content/uploads/2021/03/Pankkiviivakoodi-opas.pdf).\n\n## Installation\n\n```bash\npip install virtuaaliviivakoodi\n```\n\n## Usage\n\n```python\nfrom virtuaaliviivakoodi import virtuaaliviivakoodi\n\nvirtuaaliviivakoodi(\n\tiban="FI49 5000 9420 0287 30",\n\treference="12345 67907",\n\tdue_date=date(2022, 12, 12),\n\teuro_amount=100.20,\n)\n\n# > "449500094200287300001002000000000000001234567907201212"\n\n```\n\n## Function arguments\n\n| Argument      | Type          | Description                                                                                                                                                                                                   |\n| ------------- | ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| `iban`        | `str`         | Mandatory. Payment receiver\'s IBAN. Must be in Finnish format. E.g.: `"FI49 5000 9420 0287 30"` or `"FI4950009420028730"`                                                                                     |\n| `reference`   | `str` `int`   | Mandatory. Invoice reference in Finnish or international (RF) format. May invluce whitespace characters. E.g. `"12345 67907"`, `"1234567907"`, `1234567907` or `"RF92 1234 2345"`                             |\n| `due_date`    | `date`        | Mandatory. Invoice due date as a Python date object.                                                                                                                                                          |\n| `euro_amount` | `float` `int` | Mandatory. Invoice total amount in Euros. Must be positive number. According [the spec](https://www.finanssiala.fi/wp-content/uploads/2021/03/Pankkiviivakoodi-opas.pdf) amount must be smaller than 1000000. |\n\n## Exceptions\n\nExceptions can be imported the following way:\n\n```python\nfrom virtuaaliviivakoodi.exceptions import (\n\tVirtuaaliviivakoodiException,\n\tInvalidIBANException,\n\tInvalidReferenceException,\n\tInvalidEuroAmountException,\n\tInvalidDueDateException,\n)\n```\n\n| Exception                      | Description                                               |\n| ------------------------------ | --------------------------------------------------------- |\n| `VirtuaaliviivakoodiException` | Base exception class for all of the following exceptions. |\n| `InvalidIBANException`         | Raised for invalid IBANs                                  |\n| `InvalidReferenceException`    | Raised for invalid references                             |\n| `InvalidEuroAmountException`   | Raised for invalid euro amounts                           |\n| `InvalidDueDateException`      | Raised for invalid due dates                              |\n',
     'author': 'Juho Enala',
     'author_email': 'juho.enala@nocfo.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `virtuaaliviivakoodi-1.0.0/PKG-INFO` & `virtuaaliviivakoodi-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: virtuaaliviivakoodi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library for generating Finnish virtuaaliviivakoodi's
 License: MIT
 Author: Juho Enala
 Author-email: juho.enala@nocfo.io
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Finnish virtuaaliviivakoodi generation
 
 [![PyPI version](https://badge.fury.io/py/virtuaaliviivakoodi.svg)](https://badge.fury.io/py/virtuaaliviivakoodi)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
```


# Comparing `tmp/camouflage_decryptor-0.0.1.tar.gz` & `tmp/camouflage_decryptor-0.1.1.tar.gz`

## Comparing `camouflage_decryptor-0.0.1.tar` & `camouflage_decryptor-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 camouflage_decryptor-0.0.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 camouflage_decryptor-0.0.1/src/camouflage_decryptor/__about__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 camouflage_decryptor-0.0.1/src/camouflage_decryptor/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 camouflage_decryptor-0.0.1/src/camouflage_decryptor/__main__.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 camouflage_decryptor-0.0.1/src/camouflage_decryptor/decryptor.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 camouflage_decryptor-0.0.1/src/camouflage_decryptor/cli/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 camouflage_decryptor-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 camouflage_decryptor-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 camouflage_decryptor-0.0.1/README.md
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 camouflage_decryptor-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 camouflage_decryptor-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 camouflage_decryptor-0.1.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 camouflage_decryptor-0.1.1/src/camouflage_decryptor/__about__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 camouflage_decryptor-0.1.1/src/camouflage_decryptor/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 camouflage_decryptor-0.1.1/src/camouflage_decryptor/__main__.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 camouflage_decryptor-0.1.1/src/camouflage_decryptor/decryptor.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 camouflage_decryptor-0.1.1/src/camouflage_decryptor/cli/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 camouflage_decryptor-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 camouflage_decryptor-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 camouflage_decryptor-0.1.1/README.md
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 camouflage_decryptor-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 camouflage_decryptor-0.1.1/PKG-INFO
```

### Comparing `camouflage_decryptor-0.0.1/.github/workflows/pypi-publish.yml` & `camouflage_decryptor-0.1.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `camouflage_decryptor-0.0.1/src/camouflage_decryptor/decryptor.py` & `camouflage_decryptor-0.1.1/src/camouflage_decryptor/decryptor.py`

 * *Files identical despite different names*

### Comparing `camouflage_decryptor-0.0.1/src/camouflage_decryptor/cli/__init__.py` & `camouflage_decryptor-0.1.1/src/camouflage_decryptor/cli/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 @click.group(context_settings={"help_option_names": ["-h", "--help"]})
 @click.version_option(version=__version__, prog_name="camouflage-decryptor")
 def camouflage_decryptor():
     pass
 
 
 @click.command()
-@click.argument('input', type=click.File('rb'))
+@click.argument('input', type=click.File('rb'), help="JPG file treated with camouflage"
 def get_key(input):
-    """Extract key from input file. """
+    """Extract key from JPG file treated with camouflage"""
     img_raw = input.read()
     extract_camouflage_password(img_raw)
 
 
 camouflage_decryptor.add_command(get_key)
```

### Comparing `camouflage_decryptor-0.0.1/LICENSE.txt` & `camouflage_decryptor-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `camouflage_decryptor-0.0.1/README.md` & `camouflage_decryptor-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 # camouflage-decryptor
 
 [![PyPI - Version](https://img.shields.io/pypi/v/camouflage-decryptor.svg)](https://pypi.org/project/camouflage-decryptor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/camouflage-decryptor.svg)](https://pypi.org/project/camouflage-decryptor)
 
 -----
+This is a tool to extract information from files that have been generated with camouflage. Currently only JPEG-files are supported.
 
 **Table of Contents**
 
 - [Installation](#installation)
+- [Usage](#usage)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install camouflage-decryptor
 ```
 
+## Usage
+
+To get the password from a stego image:
+```console
+camouflage-decryptor get-key my-stego-image.jpg
+```
+
+You might need to use the following syntax to call the script, e.g. if on Windows:
+```console
+python -m camouflage_decryptor get-key my-stego-image.jpg
+```
+
 ## License
 
 `camouflage-decryptor` is distributed under the terms of the [EUPL-1.2](https://spdx.org/licenses/EUPL-1.2.html) license.
```

### Comparing `camouflage_decryptor-0.0.1/pyproject.toml` & `camouflage_decryptor-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `camouflage_decryptor-0.0.1/PKG-INFO` & `camouflage_decryptor-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camouflage-decryptor
-Version: 0.0.1
+Version: 0.1.1
 Project-URL: Documentation, https://github.com/unknown/camouflage-decryptor#readme
 Project-URL: Issues, https://github.com/unknown/camouflage-decryptor/issues
 Project-URL: Source, https://github.com/unknown/camouflage-decryptor
 Author-email: anjomro <py@anjomro.de>
 License-Expression: EUPL-1.2
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -22,22 +22,36 @@
 
 # camouflage-decryptor
 
 [![PyPI - Version](https://img.shields.io/pypi/v/camouflage-decryptor.svg)](https://pypi.org/project/camouflage-decryptor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/camouflage-decryptor.svg)](https://pypi.org/project/camouflage-decryptor)
 
 -----
+This is a tool to extract information from files that have been generated with camouflage. Currently only JPEG-files are supported.
 
 **Table of Contents**
 
 - [Installation](#installation)
+- [Usage](#usage)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install camouflage-decryptor
 ```
 
+## Usage
+
+To get the password from a stego image:
+```console
+camouflage-decryptor get-key my-stego-image.jpg
+```
+
+You might need to use the following syntax to call the script, e.g. if on Windows:
+```console
+python -m camouflage_decryptor get-key my-stego-image.jpg
+```
+
 ## License
 
 `camouflage-decryptor` is distributed under the terms of the [EUPL-1.2](https://spdx.org/licenses/EUPL-1.2.html) license.
```


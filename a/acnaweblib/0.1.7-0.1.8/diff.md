# Comparing `tmp/acnaweblib-0.1.7.tar.gz` & `tmp/acnaweblib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/acnaweblib-0.1.7.tar", last modified: Wed Apr 26 06:59:42 2023, max compression
+gzip compressed data, was "dist/acnaweblib-0.1.8.tar", last modified: Wed Apr 26 07:08:47 2023, max compression
```

## Comparing `acnaweblib-0.1.7.tar` & `acnaweblib-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-04-26 06:59:42.912080 acnaweblib-0.1.7/
--rw-rw-r--   0 ac        (1000) ac        (1000)       18 2023-04-26 06:41:30.000000 acnaweblib-0.1.7/MANIFEST.in
--rw-rw-r--   0 ac        (1000) ac        (1000)     1154 2023-04-26 06:59:42.912080 acnaweblib-0.1.7/PKG-INFO
--rw-rw-r--   0 ac        (1000) ac        (1000)      872 2023-04-26 06:41:48.000000 acnaweblib-0.1.7/README.md
--rw-rw-rw-   0 ac        (1000) ac        (1000)      692 2023-04-26 06:59:35.000000 acnaweblib-0.1.7/README.rst
-drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-04-26 06:59:42.912080 acnaweblib-0.1.7/acnaweblib.egg-info/
--rw-rw-r--   0 ac        (1000) ac        (1000)     1154 2023-04-26 06:59:42.000000 acnaweblib-0.1.7/acnaweblib.egg-info/PKG-INFO
--rw-rw-r--   0 ac        (1000) ac        (1000)      177 2023-04-26 06:59:42.000000 acnaweblib-0.1.7/acnaweblib.egg-info/SOURCES.txt
--rw-rw-r--   0 ac        (1000) ac        (1000)        1 2023-04-26 06:59:42.000000 acnaweblib-0.1.7/acnaweblib.egg-info/dependency_links.txt
--rw-rw-r--   0 ac        (1000) ac        (1000)        1 2023-04-26 06:59:42.000000 acnaweblib-0.1.7/acnaweblib.egg-info/top_level.txt
--rw-rw-r--   0 ac        (1000) ac        (1000)       38 2023-04-26 06:59:42.912080 acnaweblib-0.1.7/setup.cfg
--rw-rw-r--   0 ac        (1000) ac        (1000)      788 2023-04-26 06:59:41.000000 acnaweblib-0.1.7/setup.py
+drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-04-26 07:08:47.555379 acnaweblib-0.1.8/
+-rw-rw-r--   0 ac        (1000) ac        (1000)       18 2023-04-26 06:41:30.000000 acnaweblib-0.1.8/MANIFEST.in
+-rw-rw-r--   0 ac        (1000) ac        (1000)     1173 2023-04-26 07:08:47.555379 acnaweblib-0.1.8/PKG-INFO
+-rw-rw-r--   0 ac        (1000) ac        (1000)      872 2023-04-26 06:41:48.000000 acnaweblib-0.1.8/README.md
+-rw-rw-rw-   0 ac        (1000) ac        (1000)      711 2023-04-26 07:08:45.000000 acnaweblib-0.1.8/README.rst
+drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-04-26 07:08:47.555379 acnaweblib-0.1.8/acnaweblib.egg-info/
+-rw-rw-r--   0 ac        (1000) ac        (1000)     1173 2023-04-26 07:08:47.000000 acnaweblib-0.1.8/acnaweblib.egg-info/PKG-INFO
+-rw-rw-r--   0 ac        (1000) ac        (1000)      177 2023-04-26 07:08:47.000000 acnaweblib-0.1.8/acnaweblib.egg-info/SOURCES.txt
+-rw-rw-r--   0 ac        (1000) ac        (1000)        1 2023-04-26 07:08:47.000000 acnaweblib-0.1.8/acnaweblib.egg-info/dependency_links.txt
+-rw-rw-r--   0 ac        (1000) ac        (1000)        1 2023-04-26 07:08:47.000000 acnaweblib-0.1.8/acnaweblib.egg-info/top_level.txt
+-rw-rw-r--   0 ac        (1000) ac        (1000)       38 2023-04-26 07:08:47.555379 acnaweblib-0.1.8/setup.cfg
+-rw-rw-r--   0 ac        (1000) ac        (1000)      788 2023-04-26 07:04:11.000000 acnaweblib-0.1.8/setup.py
```

### Comparing `acnaweblib-0.1.7/PKG-INFO` & `acnaweblib-0.1.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
 Name: acnaweblib
-Version: 0.1.7
+Version: 0.1.8
 Summary: Short description
 Home-page: https://github.com/acnaweb/acnaweb-lib
 Author: Antonio Carlos de Lima Junior
 Author-email: antonioclj.ac@gmail.com
 License: MIT
 Keywords: funniest joke comedy flying circus
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Text Processing :: Linguistic
 
-Acnaweblib
-------------
+==========
+acnaweblib
+==========
 
 acnaweblib is a Python library for testing
- 
+
 `Homepage <https://github.com/acnaweb/acnaweb-lib>`__
 --------------------------------------------------------
 
 Installation
 ------------
 
 Use the package manager `pip <https://pip.pypa.io/en/stable/>`__ to
 install acnaweblib.
 
 Install
 -------
 
-.. code:: bash
-
-   pip install acnaweblib
+.. code-block: python
+    pip install acnaweblib
 
 Usage
 -----
 
-.. code:: python
-
+.. code-block: python
    from acnaweblib import calculator
 
    # returns 6
    result = calculator.add(4,2)
 
 Author
 ------
```

### Comparing `acnaweblib-0.1.7/README.md` & `acnaweblib-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `acnaweblib-0.1.7/README.rst` & `acnaweblib-0.1.8/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-Acnaweblib
-------------
+==========
+acnaweblib
+==========
 
 acnaweblib is a Python library for testing
- 
+
 `Homepage <https://github.com/acnaweb/acnaweb-lib>`__
 --------------------------------------------------------
 
 Installation
 ------------
 
 Use the package manager `pip <https://pip.pypa.io/en/stable/>`__ to
 install acnaweblib.
 
 Install
 -------
 
-.. code:: bash
-
-   pip install acnaweblib
+.. code-block: python
+    pip install acnaweblib
 
 Usage
 -----
 
-.. code:: python
-
+.. code-block: python
    from acnaweblib import calculator
 
    # returns 6
    result = calculator.add(4,2)
 
 Author
 ------
```

### Comparing `acnaweblib-0.1.7/acnaweblib.egg-info/PKG-INFO` & `acnaweblib-0.1.8/acnaweblib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
 Name: acnaweblib
-Version: 0.1.7
+Version: 0.1.8
 Summary: Short description
 Home-page: https://github.com/acnaweb/acnaweb-lib
 Author: Antonio Carlos de Lima Junior
 Author-email: antonioclj.ac@gmail.com
 License: MIT
 Keywords: funniest joke comedy flying circus
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Text Processing :: Linguistic
 
-Acnaweblib
-------------
+==========
+acnaweblib
+==========
 
 acnaweblib is a Python library for testing
- 
+
 `Homepage <https://github.com/acnaweb/acnaweb-lib>`__
 --------------------------------------------------------
 
 Installation
 ------------
 
 Use the package manager `pip <https://pip.pypa.io/en/stable/>`__ to
 install acnaweblib.
 
 Install
 -------
 
-.. code:: bash
-
-   pip install acnaweblib
+.. code-block: python
+    pip install acnaweblib
 
 Usage
 -----
 
-.. code:: python
-
+.. code-block: python
    from acnaweblib import calculator
 
    # returns 6
    result = calculator.add(4,2)
 
 Author
 ------
```

### Comparing `acnaweblib-0.1.7/setup.py` & `acnaweblib-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('README.rst') as f:
         return f.read()
 
 requirements = []
 
 setup(
     name='acnaweblib',
-    version='0.1.7',
+    version='0.1.8',
     description='Short description',
     long_description=readme(),
     author='Antonio Carlos de Lima Junior',
     author_email='antonioclj.ac@gmail.com',
     url='https://github.com/acnaweb/acnaweb-lib',
     packages=find_packages(include=['acnaweblib', 'acnaweblib.*']),
     install_requires=requirements,
```


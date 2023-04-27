# Comparing `tmp/toml_tools-0.10.4-py2.py3-none-any.whl.zip` & `tmp/toml_tools-0.10.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 17289 bytes, number of entries: 10
+Zip file size: 18076 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat      700 b- defN 23-Apr-25 18:51 toml_tools/__init__.py
 -rw-rw-rw-  2.0 fat    39995 b- defN 23-Apr-25 14:18 toml_tools/decoder.py
 -rw-rw-rw-  2.0 fat    11307 b- defN 23-Apr-25 18:49 toml_tools/encoder.py
 -rw-rw-rw-  2.0 fat      363 b- defN 23-Apr-25 14:18 toml_tools/ordered.py
 -rw-rw-rw-  2.0 fat      795 b- defN 23-Apr-25 14:18 toml_tools/tz.py
--rw-rw-rw-  2.0 fat     1278 b- defN 23-Apr-25 18:57 toml_tools-0.10.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7698 b- defN 23-Apr-25 18:57 toml_tools-0.10.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-25 18:57 toml_tools-0.10.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-25 18:57 toml_tools-0.10.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      792 b- defN 23-Apr-25 18:57 toml_tools-0.10.4.dist-info/RECORD
-10 files, 63049 bytes uncompressed, 15947 bytes compressed:  74.7%
+-rw-rw-rw-  2.0 fat     1278 b- defN 23-Apr-26 21:51 toml_tools-0.10.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     8815 b- defN 23-Apr-26 21:51 toml_tools-0.10.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-26 21:51 toml_tools-0.10.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-26 21:51 toml_tools-0.10.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      792 b- defN 23-Apr-26 21:51 toml_tools-0.10.5.dist-info/RECORD
+10 files, 64166 bytes uncompressed, 16734 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: toml_tools/ordered.py
 Comment: 
 
 Filename: toml_tools/tz.py
 Comment: 
 
-Filename: toml_tools-0.10.4.dist-info/LICENSE
+Filename: toml_tools-0.10.5.dist-info/LICENSE
 Comment: 
 
-Filename: toml_tools-0.10.4.dist-info/METADATA
+Filename: toml_tools-0.10.5.dist-info/METADATA
 Comment: 
 
-Filename: toml_tools-0.10.4.dist-info/WHEEL
+Filename: toml_tools-0.10.5.dist-info/WHEEL
 Comment: 
 
-Filename: toml_tools-0.10.4.dist-info/top_level.txt
+Filename: toml_tools-0.10.5.dist-info/top_level.txt
 Comment: 
 
-Filename: toml_tools-0.10.4.dist-info/RECORD
+Filename: toml_tools-0.10.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `toml_tools-0.10.4.dist-info/LICENSE` & `toml_tools-0.10.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `toml_tools-0.10.4.dist-info/METADATA` & `toml_tools-0.10.5.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: toml-tools
-Version: 0.10.4
+Version: 0.10.5
 Summary: A fork of toml, a Python Library for TOML
 Home-page: https://github.com/JamesParrott/toml_tools
 Author: William Pearson, James Parrott
 Author-email: james.parrott@proton.me
 License: MIT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
@@ -24,242 +24,259 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.6, !=3.0.*, !=3.1.*, !=3.2.*
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-***************************
-TOML_tools, a fork of TOML.
-***************************
+# toml_tools, a fork of toml.
 
+    >>> toml_tools.dumps({'a': '\xad'})
+    'a = "\\u00ad"\n'
 
-::
+    >>> toml.dumps({'a': '\xad'})
+    IndexError
 
-  >>> toml_tools.dumps({'a': '\xad'})
-  'a = "\\u00ad"\n'
+Both the toml-tools module and its parent, the original toml module pass 253 / 336 tests from `the TOML test suite <https://github.com/BurntSushi/toml-test>`_[^2].
 
-  >>> toml.dumps({'a': '\xad'})
-  IndexError
+After working with configparser, discovering the [toml](https://github.com/uiri/toml) library was like a
+breath of fresh air.  It just worked.  With incredibly little effort in comparison to .ini files (with only one
+function call, and maybe a context manager) toml produced exactly the dictionary I wanted from my TOML file.  When I 
+later needed to write TOML files for users, it still had my back, and required hardly any additional work.
 
-Installation
-============
+So even though there are a few bugs (one of which I've already fixed - see above), and even though a few projects have 
+moved away towards [tomli-w](https://github.com/hukkin/tomli-w) (another great little opinionated library - it writes trailing commas to arrays) or even [tomlkit](https://github.com/sdispater/tomlkit) (I found it didn't write nested arrays of tables correctly), I think it's well worth fixing the bugs of the original toml project, and maintaining it [^0].  
 
+Please do submit bug reports for any issues you find.  Reading TOML is now natively supported in Python 3.11 [^1], but the 
+Python eco-system still has a need for a great TOML writer.
 
-::
+## Installation
 
-  pip install toml-tools
+    pip install toml-tools
 
+[^0]  Entirely coincidentally `;-)` a customer's application depends on toml.  It is
+undesirable to repeat all the testing and development work based on toml to date.  As it 
+happens, this application needs to run on Iron Python 2 as well.  So instead of submitting 
+more PRs to the original toml project mainly for my own needs, I've focussed my efforts on 
+this fork.  Hopefully I've not broken anything major, so perhaps it will even be of use 
+to you too.
 
+[^1] https://docs.python.org/3/library/tomllib.html
 
+[^2] Tested in a Ubuntu 22.04 WSL using Python 3.10, so currently both fail 83 `:(`.  On Windows 10 in Python 3.12, both 
+pass 249/336.
 
-****************************
-Parent project (TOML) Readme
-****************************
+# Parent project (TOML) Readme
 
-.. .. image:: https://img.shields.io/pypi/v/toml
-..     :target: https://pypi.org/project/toml/
-
-.. .. image:: https://travis-ci.org/uiri/toml.svg?branch=master
-..     :target: https://travis-ci.org/uiri/toml
-
-.. .. image:: https://img.shields.io/pypi/pyversions/toml.svg
-..     :target: https://pypi.org/project/toml/
+A Python library for parsing and creating
+[TOML](https://en.wikipedia.org/wiki/TOML).
 
+See also:
 
-A Python library for parsing and creating `TOML <https://en.wikipedia.org/wiki/TOML>`_.
+-   [The TOML Standard](https://github.com/toml-lang/toml)
+-   [The currently supported TOML
+    specification](https://github.com/toml-lang/toml/blob/v0.5.0/README.md)
+
+## Quick Tutorial
+
+*toml.loads* takes in a string containing standard TOML-formatted data
+and returns a dictionary containing the parsed data.
+
+```
+>>> import toml
+>>> toml_string = """
+... # This is a TOML document.
+...
+... title = "TOML Example"
+...
+... [owner]
+... name = "Tom Preston-Werner"
+... dob = 1979-05-27T07:32:00-08:00 # First class dates
+...
+... [database]
+... server = "192.168.1.1"
+... ports = [ 8001, 8001, 8002 ]
+... connection_max = 5000
+... enabled = true
+...
+... [servers]
+...
+...   # Indentation (tabs and/or spaces) is allowed but not required
+...   [servers.alpha]
+...   ip = "10.0.0.1"
+...   dc = "eqdc10"
+...
+...   [servers.beta]
+...   ip = "10.0.0.2"
+...   dc = "eqdc10"
+...
+... [clients]
+... data = [ ["gamma", "delta"], [1, 2] ]
+...
+... # Line breaks are OK when inside arrays
+... hosts = [
+...   "alpha",
+...   "omega"
+... ]
+... """
+>>> parsed_toml = toml.loads(toml_string)
+```
 
-.. The module passes `the TOML test suite <https://github.com/BurntSushi/toml-test>`_.
+*toml.dumps* takes a dictionary and returns a string containing the
+corresponding TOML-formatted data.
 
-See also:
+```
+>>> new_toml_string = toml.dumps(parsed_toml)
+>>> print(new_toml_string)
+title = "TOML Example"
+[owner]
+name = "Tom Preston-Werner"
+dob = 1979-05-27T07:32:00Z
+[database]
+server = "192.168.1.1"
+ports = [ 8001, 8001, 8002,]
+connection_max = 5000
+enabled = true
+[clients]
+data = [ [ "gamma", "delta",], [ 1, 2,],]
+hosts = [ "alpha", "omega",]
+[servers.alpha]
+ip = "10.0.0.1"
+dc = "eqdc10"
+[servers.beta]
+ip = "10.0.0.2"
+dc = "eqdc10"
+```
+
+*toml.dump* takes a dictionary and a file descriptor and returns a
+string containing the corresponding TOML-formatted data.
+
+```
+>>> with open('new_toml_file.toml', 'w') as f:
+...     new_toml_string = toml.dump(parsed_toml, f)
+>>> print(new_toml_string)
+title = "TOML Example"
+[owner]
+name = "Tom Preston-Werner"
+dob = 1979-05-27T07:32:00Z
+[database]
+server = "192.168.1.1"
+ports = [ 8001, 8001, 8002,]
+connection_max = 5000
+enabled = true
+[clients]
+data = [ [ "gamma", "delta",], [ 1, 2,],]
+hosts = [ "alpha", "omega",]
+[servers.alpha]
+ip = "10.0.0.1"
+dc = "eqdc10"
+[servers.beta]
+ip = "10.0.0.2"
+dc = "eqdc10"
+```
 
-* `The TOML Standard <https://github.com/toml-lang/toml>`_
-* `The currently supported TOML specification <https://github.com/toml-lang/toml/blob/v0.5.0/README.md>`_
+For more functions, view the API Reference below.
 
+### Note
 
+For Numpy users, by default the data types `np.floatX` will not be
+translated to floats by toml, but will instead be encoded as strings. To
+get around this, specify the `TomlNumpyEncoder` when saving your data.
 
-Quick Tutorial
-==============
+```
+>>> import toml
+>>> import numpy as np
+>>> a = np.arange(0, 10, dtype=np.double)
+>>> output = {'a': a}
+>>> toml.dumps(output)
+'a = [ "0.0", "1.0", "2.0", "3.0", "4.0", "5.0", "6.0", "7.0", "8.0", "9.0",]\n'
+>>> toml.dumps(output, encoder=toml.TomlNumpyEncoder())
+'a = [ 0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0,]\n'
+```
 
-*toml.loads* takes in a string containing standard TOML-formatted data and
-returns a dictionary containing the parsed data.
-
-.. code:: pycon
-
-  >>> import toml
-  >>> toml_string = """
-  ... # This is a TOML document.
-  ...
-  ... title = "TOML Example"
-  ...
-  ... [owner]
-  ... name = "Tom Preston-Werner"
-  ... dob = 1979-05-27T07:32:00-08:00 # First class dates
-  ...
-  ... [database]
-  ... server = "192.168.1.1"
-  ... ports = [ 8001, 8001, 8002 ]
-  ... connection_max = 5000
-  ... enabled = true
-  ...
-  ... [servers]
-  ...
-  ...   # Indentation (tabs and/or spaces) is allowed but not required
-  ...   [servers.alpha]
-  ...   ip = "10.0.0.1"
-  ...   dc = "eqdc10"
-  ...
-  ...   [servers.beta]
-  ...   ip = "10.0.0.2"
-  ...   dc = "eqdc10"
-  ...
-  ... [clients]
-  ... data = [ ["gamma", "delta"], [1, 2] ]
-  ...
-  ... # Line breaks are OK when inside arrays
-  ... hosts = [
-  ...   "alpha",
-  ...   "omega"
-  ... ]
-  ... """
-  >>> parsed_toml = toml.loads(toml_string)
+## API Reference
 
+### toml.load(f, _dict=dict)
 
-*toml.dumps* takes a dictionary and returns a string containing the
-corresponding TOML-formatted data.
+Parse a file or a list of files as TOML and return a dictionary.
 
-.. code:: pycon
+Args:
 
-  >>> new_toml_string = toml.dumps(parsed_toml)
-  >>> print(new_toml_string)
-  title = "TOML Example"
-  [owner]
-  name = "Tom Preston-Werner"
-  dob = 1979-05-27T07:32:00Z
-  [database]
-  server = "192.168.1.1"
-  ports = [ 8001, 8001, 8002,]
-  connection_max = 5000
-  enabled = true
-  [clients]
-  data = [ [ "gamma", "delta",], [ 1, 2,],]
-  hosts = [ "alpha", "omega",]
-  [servers.alpha]
-  ip = "10.0.0.1"
-  dc = "eqdc10"
-  [servers.beta]
-  ip = "10.0.0.2"
-  dc = "eqdc10"
+ - `f`: A path to a file, list of filepaths (to be read into
+single object) or a file descriptor
 
-*toml.dump* takes a dictionary and a file descriptor and returns a string containing the
-corresponding TOML-formatted data.
+ - `_dict`: The class of the dictionary object to be returned
 
-.. code:: pycon
+Returns:
 
-  >>> with open('new_toml_file.toml', 'w') as f:
-  ...     new_toml_string = toml.dump(parsed_toml, f)
-  >>> print(new_toml_string)
-  title = "TOML Example"
-  [owner]
-  name = "Tom Preston-Werner"
-  dob = 1979-05-27T07:32:00Z
-  [database]
-  server = "192.168.1.1"
-  ports = [ 8001, 8001, 8002,]
-  connection_max = 5000
-  enabled = true
-  [clients]
-  data = [ [ "gamma", "delta",], [ 1, 2,],]
-  hosts = [ "alpha", "omega",]
-  [servers.alpha]
-  ip = "10.0.0.1"
-  dc = "eqdc10"
-  [servers.beta]
-  ip = "10.0.0.2"
-  dc = "eqdc10"
+ - A dictionary (or object `_dict`) containing parsed TOML data
 
-For more functions, view the API Reference below.
+Raises:
 
-Note
-----
+ -   `TypeError`: When `f` is an invalid type or is a list
+            containing invalid types
+ -   `TomlDecodeError`: When an error occurs while decoding the
+            file(s)
 
-For Numpy users, by default the data types ``np.floatX`` will not be translated to floats by toml, but will instead be encoded as strings. To get around this, specify the ``TomlNumpyEncoder`` when saving your data.
+### toml.loads(s, _dict=dict)
 
-.. code:: pycon
+Parse a TOML-formatted string to a dictionary.
 
-  >>> import toml
-  >>> import numpy as np
-  >>> a = np.arange(0, 10, dtype=np.double)
-  >>> output = {'a': a}
-  >>> toml.dumps(output)
-  'a = [ "0.0", "1.0", "2.0", "3.0", "4.0", "5.0", "6.0", "7.0", "8.0", "9.0",]\n'
-  >>> toml.dumps(output, encoder=toml.TomlNumpyEncoder())
-  'a = [ 0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0,]\n'
+Args:
+ -   `s`: The TOML-formatted string to be parsed
+ -   `_dict`: Specifies the class of the returned toml dictionary
 
-API Reference
-=============
+Returns:
 
-``toml.load(f, _dict=dict)``
-  Parse a file or a list of files as TOML and return a dictionary.
+ - A dictionary (or object `_dict`) containing parsed TOML data
 
-  :Args:
-    * ``f``: A path to a file, list of filepaths (to be read into single
-      object) or a file descriptor
-    * ``_dict``: The class of the dictionary object to be returned
+Raises:
 
-  :Returns:
-    A dictionary (or object ``_dict``) containing parsed TOML data
+ -   `TypeError`: When a non-string object is passed
+ -   `TomlDecodeError`: When an error occurs while decoding the
+    TOML-formatted string
 
-  :Raises:
-    * ``TypeError``: When ``f`` is an invalid type or is a list containing
-      invalid types
-    * ``TomlDecodeError``: When an error occurs while decoding the file(s)
+### toml.dump(o, f, encoder=None)
 
-``toml.loads(s, _dict=dict)``
-  Parse a TOML-formatted string to a dictionary.
+Write a dictionary to a file containing TOML-formatted data
 
-  :Args:
-    * ``s``: The TOML-formatted string to be parsed
-    * ``_dict``: Specifies the class of the returned toml dictionary
+Args:
 
-  :Returns:
-    A dictionary (or object ``_dict``) containing parsed TOML data
+ -   `o`: An object to be converted into TOML
+ -   `f`: A File descriptor where the TOML-formatted output
+    should be stored
+ -   `encoder`: An instance of `TomlEncoder` (or subclass) for
+    encoding the object. If `None`, will default to
+    `TomlEncoder`
 
-  :Raises:
-    * ``TypeError``: When a non-string object is passed
-    * ``TomlDecodeError``: When an error occurs while decoding the
-      TOML-formatted string
+Returns:
 
-``toml.dump(o, f, encoder=None)``
-  Write a dictionary to a file containing TOML-formatted data
+ - A string containing the TOML-formatted data corresponding to
+        object `o`
 
-  :Args:
-    * ``o``: An object to be converted into TOML
-    * ``f``: A File descriptor where the TOML-formatted output should be stored
-    * ``encoder``: An instance of ``TomlEncoder`` (or subclass) for encoding the object. If ``None``, will default to ``TomlEncoder``
+Raises:
 
-  :Returns:
-    A string containing the TOML-formatted data corresponding to object ``o``
+ - `TypeError`: When anything other than file descriptor is
+            passed
 
-  :Raises:
-    * ``TypeError``: When anything other than file descriptor is passed
+### toml.dumps(o, encoder=None)
 
-``toml.dumps(o, encoder=None)``
-  Create a TOML-formatted string from an input object
+Create a TOML-formatted string from an input object
 
-  :Args:
-    * ``o``: An object to be converted into TOML
-    * ``encoder``: An instance of ``TomlEncoder`` (or subclass) for encoding the object. If ``None``, will default to ``TomlEncoder``
+Args:
 
-  :Returns:
-    A string containing the TOML-formatted data corresponding to object ``o``
+ -   `o`: An object to be converted into TOML
+ -   `encoder`: An instance of `TomlEncoder` (or subclass) for
+    encoding the object. If `None`, will default to
+    `TomlEncoder`
 
+Returns:
 
+ - A string containing the TOML-formatted data corresponding to object `o`
 
-Licensing
-=========
+## Licensing
 
-This project is released under the terms of the MIT Open Source License. View
-*LICENSE.txt* for more information.
+This project is released under the terms of the MIT Open Source License.
+View *LICENSE.txt* for more information.
```

## Comparing `toml_tools-0.10.4.dist-info/RECORD` & `toml_tools-0.10.5.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 toml_tools/__init__.py,sha256=F0esnPLv0T7o56KPshHpbwFrUUnY-8I83twCWtD3K0Y,700
 toml_tools/decoder.py,sha256=4y4QkzpCuhQzHl3cgJzHSm2Re2oePCXUNbuvny9jbvw,39995
 toml_tools/encoder.py,sha256=rV9JjMPmUJQPQYlH1aelDU9cTrguDaJq7fzAcpYku3E,11307
 toml_tools/ordered.py,sha256=igfUXPcTe8BtvnwImSCaHXKzLioVrXdvw6hP2oxnRg0,363
 toml_tools/tz.py,sha256=pPvvp9ViBuRBdWvkxzIqyeEMlu5zXRhWNP2cO4kWB4M,795
-toml_tools-0.10.4.dist-info/LICENSE,sha256=Y6yqdaS_YnXVg0iPzWS7JCt8RBXVomeUY2O6IHJ1nhQ,1278
-toml_tools-0.10.4.dist-info/METADATA,sha256=jsGQHCi9kalhL9WSKXioxVDtqWeC2SLHDhP_E0zIRjo,7698
-toml_tools-0.10.4.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-toml_tools-0.10.4.dist-info/top_level.txt,sha256=EB4mI4u4cEvE1f7T_nICLLOYAG92KM-Cg5nejqG0uw0,11
-toml_tools-0.10.4.dist-info/RECORD,,
+toml_tools-0.10.5.dist-info/LICENSE,sha256=Y6yqdaS_YnXVg0iPzWS7JCt8RBXVomeUY2O6IHJ1nhQ,1278
+toml_tools-0.10.5.dist-info/METADATA,sha256=wakYqlBj04sxD14utE9ctcZ_vtnDfsITMdk00WCVp5c,8815
+toml_tools-0.10.5.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+toml_tools-0.10.5.dist-info/top_level.txt,sha256=EB4mI4u4cEvE1f7T_nICLLOYAG92KM-Cg5nejqG0uw0,11
+toml_tools-0.10.5.dist-info/RECORD,,
```


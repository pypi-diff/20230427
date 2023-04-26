# Comparing `tmp/oblivious-6.0.0.tar.gz` & `tmp/oblivious-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oblivious-6.0.0.tar", last modified: Wed Sep 14 20:52:33 2022, max compression
+gzip compressed data, was "oblivious-7.0.0.tar", last modified: Wed Apr 26 22:59:46 2023, max compression
```

## Comparing `oblivious-6.0.0.tar` & `oblivious-7.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-09-14 20:52:33.700619 oblivious-6.0.0/
--rw-rw-rw-   0        0        0     1093 2022-09-09 03:13:24.000000 oblivious-6.0.0/LICENSE
--rw-rw-rw-   0        0        0    13390 2022-09-14 20:52:33.699742 oblivious-6.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    12753 2022-09-14 19:21:27.000000 oblivious-6.0.0/README.rst
--rw-rw-rw-   0        0        0     1276 2022-09-14 07:38:24.000000 oblivious-6.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-14 20:52:33.700681 oblivious-6.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-14 20:52:33.685740 oblivious-6.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-09-14 20:52:33.689803 oblivious-6.0.0/src/oblivious/
--rw-rw-rw-   0        0        0      360 2022-09-14 07:38:24.000000 oblivious-6.0.0/src/oblivious/__init__.py
--rw-rw-rw-   0        0        0   121956 2022-09-14 20:00:14.000000 oblivious-6.0.0/src/oblivious/bn254.py
--rw-rw-rw-   0        0        0    44565 2022-09-14 19:15:08.000000 oblivious-6.0.0/src/oblivious/ristretto.py
-drwxrwxrwx   0        0        0        0 2022-09-14 20:52:33.698500 oblivious-6.0.0/src/oblivious.egg-info/
--rw-rw-rw-   0        0        0    13390 2022-09-14 20:52:33.000000 oblivious-6.0.0/src/oblivious.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2022-09-14 20:52:33.000000 oblivious-6.0.0/src/oblivious.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-14 20:52:33.000000 oblivious-6.0.0/src/oblivious.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      322 2022-09-14 20:52:33.000000 oblivious-6.0.0/src/oblivious.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-09-14 20:52:33.000000 oblivious-6.0.0/src/oblivious.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-09-14 20:52:33.699742 oblivious-6.0.0/test/
--rw-rw-rw-   0        0        0    66024 2022-09-14 07:38:24.000000 oblivious-6.0.0/test/test_bn254.py
--rw-rw-rw-   0        0        0    32522 2022-09-14 07:38:24.000000 oblivious-6.0.0/test/test_ristretto.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 22:59:46.886145 oblivious-7.0.0/
+-rw-r--r--   0 alapets    (502) staff       (20)     1072 2022-09-12 19:03:24.000000 oblivious-7.0.0/LICENSE
+-rw-r--r--   0 alapets    (502) staff       (20)    13661 2023-04-26 22:59:46.885964 oblivious-7.0.0/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)    13050 2023-04-17 14:49:18.000000 oblivious-7.0.0/README.rst
+-rw-r--r--   0 alapets    (502) staff       (20)     1171 2023-04-26 19:43:09.000000 oblivious-7.0.0/pyproject.toml
+-rw-r--r--   0 alapets    (502) staff       (20)       38 2023-04-26 22:59:46.886183 oblivious-7.0.0/setup.cfg
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 22:59:46.881927 oblivious-7.0.0/src/
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 22:59:46.883772 oblivious-7.0.0/src/oblivious/
+-rw-r--r--   0 alapets    (502) staff       (20)      350 2022-09-14 16:31:49.000000 oblivious-7.0.0/src/oblivious/__init__.py
+-rw-r--r--   0 alapets    (502) staff       (20)   118940 2023-04-11 01:57:09.000000 oblivious-7.0.0/src/oblivious/bn254.py
+-rw-r--r--   0 alapets    (502) staff       (20)    43354 2022-09-14 19:20:14.000000 oblivious-7.0.0/src/oblivious/ristretto.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 22:59:46.884852 oblivious-7.0.0/src/oblivious.egg-info/
+-rw-r--r--   0 alapets    (502) staff       (20)    13661 2023-04-26 22:59:46.000000 oblivious-7.0.0/src/oblivious.egg-info/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)      335 2023-04-26 22:59:46.000000 oblivious-7.0.0/src/oblivious.egg-info/SOURCES.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        1 2023-04-26 22:59:46.000000 oblivious-7.0.0/src/oblivious.egg-info/dependency_links.txt
+-rw-r--r--   0 alapets    (502) staff       (20)      302 2023-04-26 22:59:46.000000 oblivious-7.0.0/src/oblivious.egg-info/requires.txt
+-rw-r--r--   0 alapets    (502) staff       (20)       10 2023-04-26 22:59:46.000000 oblivious-7.0.0/src/oblivious.egg-info/top_level.txt
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 22:59:46.885644 oblivious-7.0.0/test/
+-rw-r--r--   0 alapets    (502) staff       (20)    64472 2022-09-14 16:31:49.000000 oblivious-7.0.0/test/test_bn254.py
+-rw-r--r--   0 alapets    (502) staff       (20)    31790 2022-09-14 16:31:49.000000 oblivious-7.0.0/test/test_ristretto.py
```

### Comparing `oblivious-6.0.0/LICENSE` & `oblivious-7.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Nth Party, Ltd.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 Nth Party, Ltd.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `oblivious-6.0.0/PKG-INFO` & `oblivious-7.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,228 +1,266 @@
-Metadata-Version: 2.1
-Name: oblivious
-Version: 6.0.0
-Summary: Python library that serves as an API for common cryptographic primitives used to implement OPRF, OT, and PSI protocols.
-Author: Nth Party, Ltd.
-Author-email: team@nthparty.com
-License: MIT
-Project-URL: Repository, https://github.com/nthparty/oblivious
-Project-URL: Documentation, https://oblivious.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: rbcl
-Provides-Extra: mclbn256
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
-=========
-oblivious
-=========
-
-Python library that serves as an API for common cryptographic primitives used to implement OPRF, OT, and PSI protocols.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/oblivious.svg
-   :target: https://badge.fury.io/py/oblivious
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/oblivious/badge/?version=latest
-   :target: https://oblivious.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/oblivious/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/nthparty/oblivious/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/oblivious/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/oblivious?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides pure-Python implementations, Python wrappers for `libsodium <https://github.com/jedisct1/libsodium>`__ and `mcl <https://github.com/herumi/mcl>`__, and additional utility methods for cryptographic primitives that are often used to implement `oblivious pseudorandom function (OPRF) <https://en.wikipedia.org/wiki/Pseudorandom_function_family>`__, `oblivious transfer (OT) <https://en.wikipedia.org/wiki/Oblivious_transfer>`__, and `private set intersection (PSI) <https://en.wikipedia.org/wiki/Private_set_intersection>`__ protocols.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/oblivious>`__::
-
-    python -m pip install oblivious
-
-It is possible to install the library together with packages that bundle dynamic/shared libraries, such as `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__::
-
-    python -m pip install oblivious[rbcl]
-    python -m pip install oblivious[mclbn256]
-    python -m pip install oblivious[rbcl,mclbn256]
-
-The library can be imported in the usual ways::
-
-    import oblivious
-    from oblivious import ristretto
-    from oblivious import bn254
-
-Examples
-^^^^^^^^
-
-.. |ristretto| replace:: ``ristretto``
-.. _ristretto: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html
-
-This library supports concise construction of elliptic curve points and scalars. The examples below use the |ristretto|_ module that provides data structures for working with the `Ristretto <https://ristretto.group>`__ group::
-
-    >>> from oblivious.ristretto import point, scalar
-    >>> p = point.hash('abc'.encode()) # Point derived from a hash of a string.
-    >>> s = scalar() # Random scalar.
-    >>> t = scalar.from_int(0) # Scalar corresponding to the zero residue.
-
-Built-in Python operators are overloaded to support point operations (such as addition, subtraction, negation, and equality) and scalar operations (such as multiplication by a scalar and inversion of scalars)::
-
-    >>> q = s * p
-    >>> p == (~s) * q
-    True
-    >>> p == ((~s) * s) * p
-    True
-    >>> p + q == q + p
-    True
-    >>> t * p == p - p
-    True
-
-.. |point| replace:: ``point``
-.. _point: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point
-
-.. |scalar| replace:: ``scalar``
-.. _scalar: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.scalar
-
-.. |bytes| replace:: ``bytes``
-.. _bytes: https://docs.python.org/3/library/stdtypes.html#bytes
-
-The |point|_ and |scalar|_ classes have common conversion methods that correspond to those supported by |bytes|_ objects (and in some cases, these classes are themselves derived from |bytes|_)::
-
-    >>> hex = '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-    >>> s = scalar.fromhex(hex)
-    >>> s.hex()
-    '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-
-In addition, Base64 conversion methods are included to support concise encoding and decoding of |point|_ and |scalar|_ objects::
-
-    >>> s.to_base64()
-    'NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk='
-    >>> s == scalar.from_base64('NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk=')
-    True
-
-For more information and background about the underlying mathematical structures and primitives found in the |ristretto|_ module, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
-
-Using Pure Python or a Shared/Dynamic Library
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |python| replace:: ``python``
-.. _python: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.python
-
-.. |sodium| replace:: ``sodium``
-.. _sodium: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.sodium
-
-Each module within this library can export two variants of its primitives and data structures: one corresponding to pure-Python implementations and another corresponding to shared/dynamic library wrappers.
-
-For example, the |ristretto|_ module exports two container classes/namespaces: |python|_ and |sodium|_. These encapsulate pure-Python implementations and shared/dynamic library (*i.e.*, libsodium) wrappers, respectively, of all operations and classes available in the |ristretto|_ module. This makes it possible to explicitly choose whether an operation requires only Python or also requires the presence of a compiled copy of libsodium on the host system.
-
-The example below uses pure-Python implementations of the scalar multiplication operation (relying on the `ge25519 <https://pypi.org/project/ge25519>`__ library)::
-
-    >>> from oblivious.ristretto import python
-    >>> p = python.point.hash('abc'.encode())
-    >>> s = python.scalar.hash('123'.encode())
-    >>> (s * p).to_base64()
-    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
-
-To check whether an instance of the libsodium shared/dynamic library has been loaded successfully, the check below can be performed::
-
-    >>> from oblivious.ristretto import sodium
-    >>> sodium is not None # Was the dynamic/shared library loaded?
-    True
-
-In the example below, the scalar multiplication operation invokes a binding for the ``crypto_scalarmult_ristretto255`` function `exported by libsodium <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto>`__::
-
-    >>> p = sodium.point.hash('abc'.encode())
-    >>> s = sodium.scalar.hash('123'.encode())
-    >>> (s * p).to_base64()
-    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
-
-.. |add| replace:: ``__add__``
-.. _add: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point.__add__
-
-The class methods exported by the |ristretto|_ module directly (*e.g.*, the method |add|_ within the class |point|_ that is imported via the statement ``from oblivious.ristretto import point``) correspond either (A) to libsodium wrappers if an instance of libsodium is found and loaded or (B) to pure-Python implementations if all attempts to load a working instances of libsodium fail. The ordered list below summarizes what definitions are exported under various conditions and the ordered sequence of attempts to locate and load an instance of libsodium.
-
-1. Under all conditions, the wrapper class |python|_ is defined and encapsulates a pure-Python variant of every low-level operation and class available in the |ristretto|_ module. **As a starting default**, all classes exported directly by the |ristretto|_ module correspond to the pure-Python implementations.
-
-2. If a shared/dynamic library instance of libsodium is found on the system and successfully loaded during one of the attempts below, then the wrapper class |sodium|_ is defined:
-
-   a. the built-in ``ctypes.util.find_library`` function is able to locate ``'sodium'`` or ``'libsodium'`` and it is loaded successfully;
-   b. a file ``libsodium.so`` or ``libsodium.dll`` under the paths specified by the ``PATH`` and ``LD_LIBRARY_PATH`` environment variables is found and loaded successfully; or
-   c. the optional `rbcl <https://pypi.org/project/rbcl>`__ package is installed and the compiled subset of libsodium included in that package is loaded successfully.
-
-3. If ``sodium`` is **not** ``None``, then the |sodium|_ class encapsulates libsodium wrappers for low-level operations and for every class exported by the |ristretto|_ module. Furthermore, **those classes exported directly by the library are redefined** to use the bindings available in the loaded instance of libsodium. The |python|_ class is still exported, as well, and all operations and class methods encapsulated within |python|_ remain as-is (*i.e.*, pure-Python implementations).
-
-.. |bn254| replace:: ``bn254``
-.. _bn254: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.bn254.html
-
-The classes within the |bn254|_ module (both those that are pure-Python implementations and those that are wrappers for functions in the `mcl <https://github.com/herumi/mcl>`__ library) are organized in a similar manner. More information is available in the documentation for the |bn254|_ module.
-
-Development
------------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
-
-    python -m pip install .[docs,lint]
-
-Documentation
-^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
-
-    python -m pip install .[docs]
-    cd docs
-    sphinx-apidoc -f -e -E --templatedir=_templates -o _source .. && make html
-
-Testing and Conventions
-^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details, and note that unit tests that require `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__ are skipped if the corresponding optional package is not installed)::
-
-    python -m pip install .[test]
-    python -m pytest
-
-Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for the tests in a given testing module can be generated by running that testing module directly::
-
-    python test/test_ristretto.py
-    python test/test_bn254.py
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/oblivious test/test_ristretto.py test/test_bn254.py
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/oblivious>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/oblivious>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
-
-    python -m pip install .[publish]
-
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
-
-    git tag ?.?.?
-    git push origin ?.?.?
-
-Remove any old build/distribution files. Then, package the source into a distribution archive::
-
-    rm -rf build dist src/*.egg-info
-    python -m build --sdist --wheel .
-
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
-
-    python -m twine upload dist/*
+Metadata-Version: 2.1
+Name: oblivious
+Version: 7.0.0
+Summary: Python library that serves as an API for common cryptographic primitives used to implement OPRF, OT, and PSI protocols.
+Author: Nth Party
+Author-email: team@nthparty.com
+License: MIT
+Project-URL: Repository, https://github.com/nthparty/oblivious
+Project-URL: Documentation, https://oblivious.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: rbcl
+Provides-Extra: mclbn256
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
+=========
+oblivious
+=========
+
+Python library that serves as an API for common cryptographic primitives used to implement OPRF, OT, and PSI protocols.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/oblivious.svg
+   :target: https://badge.fury.io/py/oblivious
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/oblivious/badge/?version=latest
+   :target: https://oblivious.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/oblivious/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/nthparty/oblivious/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/oblivious/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/oblivious?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides pure-Python implementations, Python wrappers for `libsodium <https://github.com/jedisct1/libsodium>`__ and `mcl <https://github.com/herumi/mcl>`__, and additional utility methods for cryptographic primitives that are often used to implement `oblivious pseudorandom function (OPRF) <https://en.wikipedia.org/wiki/Pseudorandom_function_family>`__, `oblivious transfer (OT) <https://en.wikipedia.org/wiki/Oblivious_transfer>`__, and `private set intersection (PSI) <https://en.wikipedia.org/wiki/Private_set_intersection>`__ protocols.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/oblivious>`__:
+
+.. code-block:: bash
+
+    python -m pip install oblivious
+
+It is possible to install the library together with packages that bundle dynamic/shared libraries, such as `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__ (note that in some environments, the brackets and/or commas may need to be escaped):
+
+.. code-block:: bash
+
+    python -m pip install oblivious[rbcl]
+    python -m pip install oblivious[mclbn256]
+    python -m pip install oblivious[rbcl,mclbn256]
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import oblivious
+    from oblivious import ristretto
+    from oblivious import bn254
+
+Examples
+^^^^^^^^
+
+.. |ristretto| replace:: ``ristretto``
+.. _ristretto: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html
+
+This library supports concise construction of elliptic curve points and scalars. The examples below use the |ristretto|_ module that provides data structures for working with the `Ristretto <https://ristretto.group>`__ group:
+
+.. code-block:: python
+
+    >>> from oblivious.ristretto import point, scalar
+    >>> p = point.hash('abc'.encode()) # Point derived from a hash of a string.
+    >>> s = scalar() # Random scalar.
+    >>> t = scalar.from_int(0) # Scalar corresponding to the zero residue.
+
+Built-in Python operators are overloaded to support point operations (such as addition, subtraction, negation, and equality) and scalar operations (such as multiplication by a scalar and inversion of scalars):
+
+.. code-block:: python
+
+    >>> q = s * p
+    >>> p == (~s) * q
+    True
+    >>> p == ((~s) * s) * p
+    True
+    >>> p + q == q + p
+    True
+    >>> t * p == p - p
+    True
+
+.. |point| replace:: ``point``
+.. _point: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point
+
+.. |scalar| replace:: ``scalar``
+.. _scalar: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.scalar
+
+.. |bytes| replace:: ``bytes``
+.. _bytes: https://docs.python.org/3/library/stdtypes.html#bytes
+
+The |point|_ and |scalar|_ classes have common conversion methods that correspond to those supported by |bytes|_ objects (and in some cases, these classes are themselves derived from |bytes|_):
+
+.. code-block:: python
+
+    >>> hex = '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+    >>> s = scalar.from_hex(hex)
+    >>> s.hex()
+    '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+
+In addition, Base64 conversion methods are included to support concise encoding and decoding of |point|_ and |scalar|_ objects:
+
+.. code-block:: python
+
+    >>> s.to_base64()
+    'NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk='
+    >>> s == scalar.from_base64('NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk=')
+    True
+
+For more information and background about the underlying mathematical structures and primitives found in the |ristretto|_ module, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
+
+Using Pure Python or a Shared/Dynamic Library
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |python| replace:: ``python``
+.. _python: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.python
+
+.. |sodium| replace:: ``sodium``
+.. _sodium: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.sodium
+
+Each module within this library can export two variants of its primitives and data structures: one corresponding to pure-Python implementations and another corresponding to shared/dynamic library wrappers.
+
+For example, the |ristretto|_ module exports two container classes/namespaces: |python|_ and |sodium|_. These encapsulate pure-Python implementations and shared/dynamic library (*i.e.*, libsodium) wrappers, respectively, of all operations and classes available in the |ristretto|_ module. This makes it possible to explicitly choose whether an operation requires only Python or also requires the presence of a compiled copy of libsodium on the host system.
+
+The example below uses pure-Python implementations of the scalar multiplication operation (relying on the `ge25519 <https://pypi.org/project/ge25519>`__ library):
+
+.. code-block:: python
+
+    >>> from oblivious.ristretto import python
+    >>> p = python.point.hash('abc'.encode())
+    >>> s = python.scalar.hash('123'.encode())
+    >>> (s * p).to_base64()
+    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
+
+To check whether an instance of the libsodium shared/dynamic library has been loaded successfully, the check below can be performed:
+
+.. code-block:: python
+
+    >>> from oblivious.ristretto import sodium
+    >>> sodium is not None # Was the dynamic/shared library loaded?
+    True
+
+In the example below, the scalar multiplication operation invokes a binding for the ``crypto_scalarmult_ristretto255`` function `exported by libsodium <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto>`__:
+
+.. code-block:: python
+
+    >>> p = sodium.point.hash('abc'.encode())
+    >>> s = sodium.scalar.hash('123'.encode())
+    >>> (s * p).to_base64()
+    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
+
+.. |add| replace:: ``__add__``
+.. _add: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point.__add__
+
+The class methods exported by the |ristretto|_ module directly (*e.g.*, the method |add|_ within the class |point|_ that is imported via the statement ``from oblivious.ristretto import point``) correspond either (A) to libsodium wrappers if an instance of libsodium is found and loaded or (B) to pure-Python implementations if all attempts to load a working instances of libsodium fail. The ordered list below summarizes what definitions are exported under various conditions and the ordered sequence of attempts to locate and load an instance of libsodium.
+
+1. Under all conditions, the wrapper class |python|_ is defined and encapsulates a pure-Python variant of every low-level operation and class available in the |ristretto|_ module. **As a starting default**, all classes exported directly by the |ristretto|_ module correspond to the pure-Python implementations.
+
+2. If a shared/dynamic library instance of libsodium is found on the system and successfully loaded during one of the attempts below, then the wrapper class |sodium|_ is defined:
+
+   a. the built-in ``ctypes.util.find_library`` function is able to locate ``'sodium'`` or ``'libsodium'`` and it is loaded successfully;
+   b. a file ``libsodium.so`` or ``libsodium.dll`` under the paths specified by the ``PATH`` and ``LD_LIBRARY_PATH`` environment variables is found and loaded successfully; or
+   c. the optional `rbcl <https://pypi.org/project/rbcl>`__ package is installed and the compiled subset of libsodium included in that package is loaded successfully.
+
+3. If ``sodium`` is **not** ``None``, then the |sodium|_ class encapsulates libsodium wrappers for low-level operations and for every class exported by the |ristretto|_ module. Furthermore, **those classes exported directly by the library are redefined** to use the bindings available in the loaded instance of libsodium. The |python|_ class is still exported, as well, and all operations and class methods encapsulated within |python|_ remain as-is (*i.e.*, pure-Python implementations).
+
+.. |bn254| replace:: ``bn254``
+.. _bn254: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.bn254.html
+
+The classes within the |bn254|_ module (both those that are pure-Python implementations and those that are wrappers for functions in the `mcl <https://github.com/herumi/mcl>`__ library) are organized in a similar manner. More information is available in the documentation for the |bn254|_ module.
+
+Development
+-----------
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs,lint]
+
+Documentation
+^^^^^^^^^^^^^
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs]
+    cd docs
+    sphinx-apidoc -f -e -E --templatedir=_templates -o _source .. && make html
+
+Testing and Conventions
+^^^^^^^^^^^^^^^^^^^^^^^
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details, and note that unit tests that require `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__ are skipped if the corresponding optional package is not installed):
+
+.. code-block:: bash
+
+    python -m pip install .[test]
+    python -m pytest
+
+Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for the tests in a given testing module can be generated by running that testing module directly:
+
+.. code-block:: bash
+
+    python test/test_ristretto.py
+    python test/test_bn254.py
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/oblivious test/test_ristretto.py test/test_bn254.py
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/oblivious>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/oblivious>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
+
+    python -m pip install .[publish]
+
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
+
+    git tag ?.?.?
+    git push origin ?.?.?
+
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
+
+    rm -rf build dist src/*.egg-info
+    python -m build --sdist --wheel .
+
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
+
+    python -m twine upload dist/*
```

### Comparing `oblivious-6.0.0/README.rst` & `oblivious-7.0.0/src/oblivious.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,208 +1,266 @@
-=========
-oblivious
-=========
-
-Python library that serves as an API for common cryptographic primitives used to implement OPRF, OT, and PSI protocols.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/oblivious.svg
-   :target: https://badge.fury.io/py/oblivious
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/oblivious/badge/?version=latest
-   :target: https://oblivious.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/oblivious/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/nthparty/oblivious/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/oblivious/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/oblivious?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides pure-Python implementations, Python wrappers for `libsodium <https://github.com/jedisct1/libsodium>`__ and `mcl <https://github.com/herumi/mcl>`__, and additional utility methods for cryptographic primitives that are often used to implement `oblivious pseudorandom function (OPRF) <https://en.wikipedia.org/wiki/Pseudorandom_function_family>`__, `oblivious transfer (OT) <https://en.wikipedia.org/wiki/Oblivious_transfer>`__, and `private set intersection (PSI) <https://en.wikipedia.org/wiki/Private_set_intersection>`__ protocols.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/oblivious>`__::
-
-    python -m pip install oblivious
-
-It is possible to install the library together with packages that bundle dynamic/shared libraries, such as `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__::
-
-    python -m pip install oblivious[rbcl]
-    python -m pip install oblivious[mclbn256]
-    python -m pip install oblivious[rbcl,mclbn256]
-
-The library can be imported in the usual ways::
-
-    import oblivious
-    from oblivious import ristretto
-    from oblivious import bn254
-
-Examples
-^^^^^^^^
-
-.. |ristretto| replace:: ``ristretto``
-.. _ristretto: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html
-
-This library supports concise construction of elliptic curve points and scalars. The examples below use the |ristretto|_ module that provides data structures for working with the `Ristretto <https://ristretto.group>`__ group::
-
-    >>> from oblivious.ristretto import point, scalar
-    >>> p = point.hash('abc'.encode()) # Point derived from a hash of a string.
-    >>> s = scalar() # Random scalar.
-    >>> t = scalar.from_int(0) # Scalar corresponding to the zero residue.
-
-Built-in Python operators are overloaded to support point operations (such as addition, subtraction, negation, and equality) and scalar operations (such as multiplication by a scalar and inversion of scalars)::
-
-    >>> q = s * p
-    >>> p == (~s) * q
-    True
-    >>> p == ((~s) * s) * p
-    True
-    >>> p + q == q + p
-    True
-    >>> t * p == p - p
-    True
-
-.. |point| replace:: ``point``
-.. _point: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point
-
-.. |scalar| replace:: ``scalar``
-.. _scalar: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.scalar
-
-.. |bytes| replace:: ``bytes``
-.. _bytes: https://docs.python.org/3/library/stdtypes.html#bytes
-
-The |point|_ and |scalar|_ classes have common conversion methods that correspond to those supported by |bytes|_ objects (and in some cases, these classes are themselves derived from |bytes|_)::
-
-    >>> hex = '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-    >>> s = scalar.fromhex(hex)
-    >>> s.hex()
-    '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-
-In addition, Base64 conversion methods are included to support concise encoding and decoding of |point|_ and |scalar|_ objects::
-
-    >>> s.to_base64()
-    'NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk='
-    >>> s == scalar.from_base64('NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk=')
-    True
-
-For more information and background about the underlying mathematical structures and primitives found in the |ristretto|_ module, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
-
-Using Pure Python or a Shared/Dynamic Library
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |python| replace:: ``python``
-.. _python: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.python
-
-.. |sodium| replace:: ``sodium``
-.. _sodium: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.sodium
-
-Each module within this library can export two variants of its primitives and data structures: one corresponding to pure-Python implementations and another corresponding to shared/dynamic library wrappers.
-
-For example, the |ristretto|_ module exports two container classes/namespaces: |python|_ and |sodium|_. These encapsulate pure-Python implementations and shared/dynamic library (*i.e.*, libsodium) wrappers, respectively, of all operations and classes available in the |ristretto|_ module. This makes it possible to explicitly choose whether an operation requires only Python or also requires the presence of a compiled copy of libsodium on the host system.
-
-The example below uses pure-Python implementations of the scalar multiplication operation (relying on the `ge25519 <https://pypi.org/project/ge25519>`__ library)::
-
-    >>> from oblivious.ristretto import python
-    >>> p = python.point.hash('abc'.encode())
-    >>> s = python.scalar.hash('123'.encode())
-    >>> (s * p).to_base64()
-    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
-
-To check whether an instance of the libsodium shared/dynamic library has been loaded successfully, the check below can be performed::
-
-    >>> from oblivious.ristretto import sodium
-    >>> sodium is not None # Was the dynamic/shared library loaded?
-    True
-
-In the example below, the scalar multiplication operation invokes a binding for the ``crypto_scalarmult_ristretto255`` function `exported by libsodium <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto>`__::
-
-    >>> p = sodium.point.hash('abc'.encode())
-    >>> s = sodium.scalar.hash('123'.encode())
-    >>> (s * p).to_base64()
-    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
-
-.. |add| replace:: ``__add__``
-.. _add: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point.__add__
-
-The class methods exported by the |ristretto|_ module directly (*e.g.*, the method |add|_ within the class |point|_ that is imported via the statement ``from oblivious.ristretto import point``) correspond either (A) to libsodium wrappers if an instance of libsodium is found and loaded or (B) to pure-Python implementations if all attempts to load a working instances of libsodium fail. The ordered list below summarizes what definitions are exported under various conditions and the ordered sequence of attempts to locate and load an instance of libsodium.
-
-1. Under all conditions, the wrapper class |python|_ is defined and encapsulates a pure-Python variant of every low-level operation and class available in the |ristretto|_ module. **As a starting default**, all classes exported directly by the |ristretto|_ module correspond to the pure-Python implementations.
-
-2. If a shared/dynamic library instance of libsodium is found on the system and successfully loaded during one of the attempts below, then the wrapper class |sodium|_ is defined:
-
-   a. the built-in ``ctypes.util.find_library`` function is able to locate ``'sodium'`` or ``'libsodium'`` and it is loaded successfully;
-   b. a file ``libsodium.so`` or ``libsodium.dll`` under the paths specified by the ``PATH`` and ``LD_LIBRARY_PATH`` environment variables is found and loaded successfully; or
-   c. the optional `rbcl <https://pypi.org/project/rbcl>`__ package is installed and the compiled subset of libsodium included in that package is loaded successfully.
-
-3. If ``sodium`` is **not** ``None``, then the |sodium|_ class encapsulates libsodium wrappers for low-level operations and for every class exported by the |ristretto|_ module. Furthermore, **those classes exported directly by the library are redefined** to use the bindings available in the loaded instance of libsodium. The |python|_ class is still exported, as well, and all operations and class methods encapsulated within |python|_ remain as-is (*i.e.*, pure-Python implementations).
-
-.. |bn254| replace:: ``bn254``
-.. _bn254: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.bn254.html
-
-The classes within the |bn254|_ module (both those that are pure-Python implementations and those that are wrappers for functions in the `mcl <https://github.com/herumi/mcl>`__ library) are organized in a similar manner. More information is available in the documentation for the |bn254|_ module.
-
-Development
------------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
-
-    python -m pip install .[docs,lint]
-
-Documentation
-^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
-
-    python -m pip install .[docs]
-    cd docs
-    sphinx-apidoc -f -e -E --templatedir=_templates -o _source .. && make html
-
-Testing and Conventions
-^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details, and note that unit tests that require `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__ are skipped if the corresponding optional package is not installed)::
-
-    python -m pip install .[test]
-    python -m pytest
-
-Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for the tests in a given testing module can be generated by running that testing module directly::
-
-    python test/test_ristretto.py
-    python test/test_bn254.py
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/oblivious test/test_ristretto.py test/test_bn254.py
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/oblivious>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/oblivious>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
-
-    python -m pip install .[publish]
-
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
-
-    git tag ?.?.?
-    git push origin ?.?.?
-
-Remove any old build/distribution files. Then, package the source into a distribution archive::
-
-    rm -rf build dist src/*.egg-info
-    python -m build --sdist --wheel .
-
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
-
-    python -m twine upload dist/*
+Metadata-Version: 2.1
+Name: oblivious
+Version: 7.0.0
+Summary: Python library that serves as an API for common cryptographic primitives used to implement OPRF, OT, and PSI protocols.
+Author: Nth Party
+Author-email: team@nthparty.com
+License: MIT
+Project-URL: Repository, https://github.com/nthparty/oblivious
+Project-URL: Documentation, https://oblivious.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: rbcl
+Provides-Extra: mclbn256
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
+=========
+oblivious
+=========
+
+Python library that serves as an API for common cryptographic primitives used to implement OPRF, OT, and PSI protocols.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/oblivious.svg
+   :target: https://badge.fury.io/py/oblivious
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/oblivious/badge/?version=latest
+   :target: https://oblivious.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/oblivious/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/nthparty/oblivious/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/oblivious/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/oblivious?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides pure-Python implementations, Python wrappers for `libsodium <https://github.com/jedisct1/libsodium>`__ and `mcl <https://github.com/herumi/mcl>`__, and additional utility methods for cryptographic primitives that are often used to implement `oblivious pseudorandom function (OPRF) <https://en.wikipedia.org/wiki/Pseudorandom_function_family>`__, `oblivious transfer (OT) <https://en.wikipedia.org/wiki/Oblivious_transfer>`__, and `private set intersection (PSI) <https://en.wikipedia.org/wiki/Private_set_intersection>`__ protocols.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/oblivious>`__:
+
+.. code-block:: bash
+
+    python -m pip install oblivious
+
+It is possible to install the library together with packages that bundle dynamic/shared libraries, such as `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__ (note that in some environments, the brackets and/or commas may need to be escaped):
+
+.. code-block:: bash
+
+    python -m pip install oblivious[rbcl]
+    python -m pip install oblivious[mclbn256]
+    python -m pip install oblivious[rbcl,mclbn256]
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import oblivious
+    from oblivious import ristretto
+    from oblivious import bn254
+
+Examples
+^^^^^^^^
+
+.. |ristretto| replace:: ``ristretto``
+.. _ristretto: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html
+
+This library supports concise construction of elliptic curve points and scalars. The examples below use the |ristretto|_ module that provides data structures for working with the `Ristretto <https://ristretto.group>`__ group:
+
+.. code-block:: python
+
+    >>> from oblivious.ristretto import point, scalar
+    >>> p = point.hash('abc'.encode()) # Point derived from a hash of a string.
+    >>> s = scalar() # Random scalar.
+    >>> t = scalar.from_int(0) # Scalar corresponding to the zero residue.
+
+Built-in Python operators are overloaded to support point operations (such as addition, subtraction, negation, and equality) and scalar operations (such as multiplication by a scalar and inversion of scalars):
+
+.. code-block:: python
+
+    >>> q = s * p
+    >>> p == (~s) * q
+    True
+    >>> p == ((~s) * s) * p
+    True
+    >>> p + q == q + p
+    True
+    >>> t * p == p - p
+    True
+
+.. |point| replace:: ``point``
+.. _point: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point
+
+.. |scalar| replace:: ``scalar``
+.. _scalar: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.scalar
+
+.. |bytes| replace:: ``bytes``
+.. _bytes: https://docs.python.org/3/library/stdtypes.html#bytes
+
+The |point|_ and |scalar|_ classes have common conversion methods that correspond to those supported by |bytes|_ objects (and in some cases, these classes are themselves derived from |bytes|_):
+
+.. code-block:: python
+
+    >>> hex = '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+    >>> s = scalar.from_hex(hex)
+    >>> s.hex()
+    '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+
+In addition, Base64 conversion methods are included to support concise encoding and decoding of |point|_ and |scalar|_ objects:
+
+.. code-block:: python
+
+    >>> s.to_base64()
+    'NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk='
+    >>> s == scalar.from_base64('NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk=')
+    True
+
+For more information and background about the underlying mathematical structures and primitives found in the |ristretto|_ module, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
+
+Using Pure Python or a Shared/Dynamic Library
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |python| replace:: ``python``
+.. _python: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.python
+
+.. |sodium| replace:: ``sodium``
+.. _sodium: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.sodium
+
+Each module within this library can export two variants of its primitives and data structures: one corresponding to pure-Python implementations and another corresponding to shared/dynamic library wrappers.
+
+For example, the |ristretto|_ module exports two container classes/namespaces: |python|_ and |sodium|_. These encapsulate pure-Python implementations and shared/dynamic library (*i.e.*, libsodium) wrappers, respectively, of all operations and classes available in the |ristretto|_ module. This makes it possible to explicitly choose whether an operation requires only Python or also requires the presence of a compiled copy of libsodium on the host system.
+
+The example below uses pure-Python implementations of the scalar multiplication operation (relying on the `ge25519 <https://pypi.org/project/ge25519>`__ library):
+
+.. code-block:: python
+
+    >>> from oblivious.ristretto import python
+    >>> p = python.point.hash('abc'.encode())
+    >>> s = python.scalar.hash('123'.encode())
+    >>> (s * p).to_base64()
+    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
+
+To check whether an instance of the libsodium shared/dynamic library has been loaded successfully, the check below can be performed:
+
+.. code-block:: python
+
+    >>> from oblivious.ristretto import sodium
+    >>> sodium is not None # Was the dynamic/shared library loaded?
+    True
+
+In the example below, the scalar multiplication operation invokes a binding for the ``crypto_scalarmult_ristretto255`` function `exported by libsodium <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto>`__:
+
+.. code-block:: python
+
+    >>> p = sodium.point.hash('abc'.encode())
+    >>> s = sodium.scalar.hash('123'.encode())
+    >>> (s * p).to_base64()
+    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
+
+.. |add| replace:: ``__add__``
+.. _add: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point.__add__
+
+The class methods exported by the |ristretto|_ module directly (*e.g.*, the method |add|_ within the class |point|_ that is imported via the statement ``from oblivious.ristretto import point``) correspond either (A) to libsodium wrappers if an instance of libsodium is found and loaded or (B) to pure-Python implementations if all attempts to load a working instances of libsodium fail. The ordered list below summarizes what definitions are exported under various conditions and the ordered sequence of attempts to locate and load an instance of libsodium.
+
+1. Under all conditions, the wrapper class |python|_ is defined and encapsulates a pure-Python variant of every low-level operation and class available in the |ristretto|_ module. **As a starting default**, all classes exported directly by the |ristretto|_ module correspond to the pure-Python implementations.
+
+2. If a shared/dynamic library instance of libsodium is found on the system and successfully loaded during one of the attempts below, then the wrapper class |sodium|_ is defined:
+
+   a. the built-in ``ctypes.util.find_library`` function is able to locate ``'sodium'`` or ``'libsodium'`` and it is loaded successfully;
+   b. a file ``libsodium.so`` or ``libsodium.dll`` under the paths specified by the ``PATH`` and ``LD_LIBRARY_PATH`` environment variables is found and loaded successfully; or
+   c. the optional `rbcl <https://pypi.org/project/rbcl>`__ package is installed and the compiled subset of libsodium included in that package is loaded successfully.
+
+3. If ``sodium`` is **not** ``None``, then the |sodium|_ class encapsulates libsodium wrappers for low-level operations and for every class exported by the |ristretto|_ module. Furthermore, **those classes exported directly by the library are redefined** to use the bindings available in the loaded instance of libsodium. The |python|_ class is still exported, as well, and all operations and class methods encapsulated within |python|_ remain as-is (*i.e.*, pure-Python implementations).
+
+.. |bn254| replace:: ``bn254``
+.. _bn254: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.bn254.html
+
+The classes within the |bn254|_ module (both those that are pure-Python implementations and those that are wrappers for functions in the `mcl <https://github.com/herumi/mcl>`__ library) are organized in a similar manner. More information is available in the documentation for the |bn254|_ module.
+
+Development
+-----------
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs,lint]
+
+Documentation
+^^^^^^^^^^^^^
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs]
+    cd docs
+    sphinx-apidoc -f -e -E --templatedir=_templates -o _source .. && make html
+
+Testing and Conventions
+^^^^^^^^^^^^^^^^^^^^^^^
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details, and note that unit tests that require `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__ are skipped if the corresponding optional package is not installed):
+
+.. code-block:: bash
+
+    python -m pip install .[test]
+    python -m pytest
+
+Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for the tests in a given testing module can be generated by running that testing module directly:
+
+.. code-block:: bash
+
+    python test/test_ristretto.py
+    python test/test_bn254.py
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/oblivious test/test_ristretto.py test/test_bn254.py
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/oblivious>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/oblivious>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
+
+    python -m pip install .[publish]
+
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
+
+    git tag ?.?.?
+    git push origin ?.?.?
+
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
+
+    rm -rf build dist src/*.egg-info
+    python -m build --sdist --wheel .
+
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
+
+    python -m twine upload dist/*
```

### Comparing `oblivious-6.0.0/src/oblivious/bn254.py` & `oblivious-7.0.0/src/oblivious/bn254.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,3016 +1,3016 @@
-"""
-.. module:: bn254
-
-bn254 module
-============
-
-This module exports the classes :obj:`~oblivious.bn254.point`,
-:obj:`~oblivious.bn254.scalar`, :obj:`~oblivious.bn254.point2`,
-and :obj:`~oblivious.bn254.scalar2` for representing points and scalars. It
-also exports the two wrapper classes/namespaces :obj:`~oblivious.bn254.python`
-and :obj:`~oblivious.bn254.mcl` that encapsulate pure-Python and shared/dynamic
-library variants of the above (respectively) and also include low-level
-operations that correspond more directly to the functions found in the
-underlying libraries.
-
-* Under all conditions, the wrapper class :obj:`~oblivious.bn254.python`
-  is defined and encapsulates a pure-Python variant of class exported by this
-  module as a whole. It also includes pure-Python variants of low-level
-  operations that correspond to functions found in the underlying libraries.
-
-* If the `mclbn256 <https://pypi.org/project/mclbn256>`__ package is installed
-  (which includes a bundled copy of the `mcl <https://github.com/herumi/mcl>`__
-  dynamic/shared libray), then the wrapper class :obj:`~oblivious.bn254.mcl`
-  is defined. Otherwise, the exported variable ``mcl`` is assigned ``None``.
-
-* If the `mclbn256 <https://pypi.org/project/mclbn256>`__ package is installed,
-  all classes exported by this module correspond to the variants defined in
-  :obj:`~oblivious.bn254.mcl`. Otherwise, they correspond to the variants
-  defined in :obj:`~oblivious.bn254.python`.
-
-For most users, the classes :obj:`~oblivious.bn254.point`,
-:obj:`~oblivious.bn254.scalar`, :obj:`~oblivious.bn254.point2`,
-and :obj:`~oblivious.bn254.scalar2` should be sufficient.
-
-When using the classes within :obj:`~oblivious.bn254.python` and/or
-:obj:`~oblivious.bn254.mcl`, users should be aware that objects corresponding
-to one implementation (*e.g.*, instances of :obj:`oblivious.bn254.mcl.point`)
-are not compatible with instances corresponding to the other implementation
-(*e.g.*, the methods of the :obj:`oblivious.bn254.python.point` class). When
-using the primitive operations that correspond to a specific implementation
-(*e.g.*, :obj:`oblivious.bn254.mcl.add`), users are responsible for ensuring
-that inputs have the type and/or representation appropriate for that
-operation's internal implementation.
-"""
-from __future__ import annotations
-from typing import Any, NoReturn, Union, Optional
-import doctest
-import hashlib
-import base64
-import secrets
-from bn254.ecp import generator as get_base
-from bn254.ecp2 import generator as get_base2
-from bn254 import big as bn, Fp12 as Fp12_, Fp as _Fp, Fp2 as _Fp2
-from bn254.ecp import ECp as ECp_
-from bn254.ecp2 import ECp2 as ECp2_
-from bn254.curve import r
-
-#
-# An attempt will be made later to import mclbn256. If the mcl shared/dynamic
-# library file bundled with mclbn256 does not load, only pure-Python
-# implementations of the functions and methods will be available.
-#
-
-mclbn256 = None
-
-#
-# Use pure-Python implementations of primitives by default.
-#
-
-class _ECp(ECp_): # pylint: disable=invalid-name
-    """Internal class."""
-    # pylint: disable=missing-function-docstring
-    @classmethod
-    def random(cls) -> _ECp:
-        return cls(int(python.scalar.random()) * get_base())
-
-    @classmethod
-    def deserialize(cls, bs) -> _ECp:
-        p_mod = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
-        d_inv = 0x1a7344bac91f117ea513ec0ed5682406b6c15140174d61b28b762ae9cf6d3b46
-        decode = lambda ns: (int.from_bytes(ns, 'little') * d_inv) % p_mod
-        x, y, z = decode(bs[:32]), decode(bs[32:64]), decode(bs[-32:])
-
-        # Compute affine coordinates
-        inv_z = bn.invmodp(z, p_mod)
-        x = (x * inv_z) % p_mod
-        y = (y * inv_z) % p_mod
-
-        p = cls()
-        assert p.setxy(x, y) or (x == 0 and y == 0)
-        return p
-
-    @classmethod
-    def mapfrom(cls, bs) -> _ECp:
-        # pylint: disable=unnecessary-direct-lambda-call
-        p_mod = (
-            (lambda x: x * (x * (x * ((36 * x) - 36) + 24) - 6) + 1)
-            ((2 ** 62) + (2 ** 55) + 1)
-        )
-        while int.from_bytes(bs, 'little') >= p_mod:
-            bs = hashlib.sha256(bs).digest()
-            bs = bs[:-1] + bytes([bs[-1] & 0b00111111])
-
-        x = int.from_bytes(bs, 'little')# % p_mod
-        y = None
-        while True:
-            x3_2 = (pow(x, 3, p_mod) + 2) % p_mod
-            if pow(x3_2, (p_mod - 1) // 2, p_mod) == 1:
-                s = (p_mod-1) // 2
-                n = 2
-                while pow(n, (p_mod-1) // 2, p_mod) == -1 % p_mod:
-                    n += 1
-                y = pow(x3_2, (s + 1) // 2, p_mod)
-                b = pow(x3_2, s, p_mod)
-                g = pow(n, s, p_mod)
-                r_ = 1
-                while True:
-                    t = b
-                    m = 0
-                    for m in range(r_):
-                        if t == 1:
-                            break
-                        t = pow(t, 2, p_mod) # pragma: no cover
-                    if m == 0:
-                        break
-                    gs = pow(g, 2**(r_ - m - 1), p_mod) # pragma: no cover
-                    g = (gs * gs) % p_mod # pragma: no cover
-                    y = (y * gs) % p_mod # pragma: no cover
-                    b = (b * g) % p_mod # pragma: no cover
-                    r_ = m # pragma: no cover
-            if y is not None:
-                # pylint: disable=invalid-unary-operand-type
-                if y % 2 == 1:
-                    y = -y
-                break
-            x += 1
-
-        p = cls()
-        assert p.setxy(x, y) or (x == 0 and y == 0)
-        return p
-
-    def __new__(cls, *args, **kwargs):
-        p = ECp_.__new__(cls)
-        _ECp.__init__(p, *args, **kwargs)
-        return p
-
-    def __init__(self, p=None):
-        ECp_.__init__(self)
-        if isinstance(p, (ECp_, _ECp)):
-            self.setxy(*p.get())
-        elif isinstance(p, python.point):
-            self.setxy(*_ECp.deserialize(p).get()) # pragma: no cover
-
-    def serialize(self) -> bytes:
-        d = 0x212ba4f27ffffff5a2c62effffffffcdb939ffffffffff8a15ffffffffffff8e
-        p = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
-        x, y, z = (*self.get(), 1)
-        encode = lambda n: (n * d % p).to_bytes(32, 'little')
-        return encode(x) + encode(y) + encode(z)
-
-class _ECp2(ECp2_): # pylint: disable=invalid-name
-    """Internal class."""
-    # pylint: disable=missing-function-docstring
-    @classmethod
-    def random(cls) -> _ECp2:
-        return cls(int(python.scalar.random()) * get_base2())
-
-    @classmethod
-    def deserialize(cls, bs) -> _ECp2:
-        p_mod = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
-        d_inv = 0x1a7344bac91f117ea513ec0ed5682406b6c15140174d61b28b762ae9cf6d3b46
-        decode = lambda ns: (int.from_bytes(ns, 'little') * d_inv) % p_mod
-        x1, y1, x2, y2, z1, z2 = (decode(bs[:32]), decode(bs[32:64]), decode(bs[64:64+32]),
-                                  decode(bs[64+32:128]), decode(bs[128:128+32]), decode(bs[-32:]))
-        z2 = z2-(z2&1)+1  # 1 if z2==0 else z2
-
-        # Compute affine coordinates
-        inv_z1, inv_z2 = bn.invmodp(z1, p_mod), bn.invmodp(z2, p_mod)
-        x1, x2 = (x1 * inv_z1) % p_mod, (x2 * inv_z2) % p_mod
-        y1, y2 = (y1 * inv_z1) % p_mod, (y2 * inv_z2) % p_mod
-
-        q = cls()
-        # pylint: disable=invalid-name
-        assert q.set(_Fp2(_Fp(x1), _Fp(y1)), _Fp2(_Fp(x2), _Fp(y2))) \
-               or (x1 == 0 and y1 == 0 and x2 == 0 and y2 == 0)
-        return q
-
-    @classmethod
-    def mapfrom(cls, h) -> _ECp2:
-        return cls((int.from_bytes(h, 'little') % r) * get_base2())
-
-    def __new__(cls, *args, **kwargs):
-        q = ECp2_.__new__(cls)
-        _ECp2.__init__(q, *args, **kwargs)
-        return q
-
-    def __init__(self, q=None):
-        ECp2_.__init__(self)
-        if isinstance(q, (ECp2_, _ECp2)):
-            self.set(*q.get())
-        elif isinstance(q, python.point2):
-            self.set(*_ECp2.deserialize(bytes(q)).get()) # pragma: no cover
-
-    def serialize(self) -> bytes:
-        d = 0x212ba4f27ffffff5a2c62effffffffcdb939ffffffffff8a15ffffffffffff8e
-
-        # BN254 modulus of *F_p*.
-        p = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
-
-        p1, p2 = (*self.get(),)
-        x1, y1, z1, x2, y2, z2 = (*p1.get(), 1, *p2.get(), 0)
-
-        encode = lambda n: (n * d % p).to_bytes(32, 'little')
-        return encode(x1) + encode(y1) + encode(x2) + encode(y2) + encode(z1) + encode(z2)
-
-class _Fp12(Fp12_): # pylint: disable=invalid-name
-    """Internal class."""
-    # pylint: disable=missing-function-docstring
-    @classmethod
-    def deserialize(cls, bs) -> _Fp12:
-        p_mod = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
-        d_inv = 0x1a7344bac91f117ea513ec0ed5682406b6c15140174d61b28b762ae9cf6d3b46
-        decode = lambda ns: (int.from_bytes(ns, 'little') * d_inv) % p_mod
-        s = _Fp12()
-        s.a.a.a.x, s.a.a.b.x = decode(bs[32*0:(32*0)+32]), decode(bs[32*1:(32*1)+32])
-        s.c.a.a.x, s.c.a.b.x = decode(bs[32*2:(32*2)+32]), decode(bs[32*3:(32*3)+32])
-        s.b.b.a.x, s.b.b.b.x = decode(bs[32*4:(32*4)+32]), decode(bs[32*5:(32*5)+32])
-        s.b.a.a.x, s.b.a.b.x = decode(bs[32*6:(32*6)+32]), decode(bs[32*7:(32*7)+32])
-        s.a.b.a.x, s.a.b.b.x = decode(bs[32*8:(32*8)+32]), decode(bs[32*9:(32*9)+32])
-        s.c.b.a.x, s.c.b.b.x = decode(bs[32*10:(32*10)+32]), decode(bs[32*11:(32*11)+32])
-        return s
-
-    def __new__(cls, *args, **kwargs):
-        q = Fp12_.__new__(cls)
-        _Fp12.__init__(q, *args, **kwargs)
-        return q
-
-    def __init__(self, s=None):
-        Fp12_.__init__(self)
-        if isinstance(s, (Fp12_, _Fp12)):
-            self.set(*s.get())
-        elif isinstance(s, python.scalar2):
-            self.set(*_Fp12.deserialize(s).get()) # pragma: no cover
-
-    def serialize(self) -> bytes:
-        d = 0x212ba4f27ffffff5a2c62effffffffcdb939ffffffffff8a15ffffffffffff8e
-
-        # BN254 modulus of *F_p*.
-        p = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
-
-        encode = lambda n: (n * d % p).to_bytes(32, 'little')
-        return bytes(
-            encode(self.a.a.a.int()) + encode(self.a.a.b.int()) +
-            encode(self.c.a.a.int()) + encode(self.c.a.b.int()) +
-            encode(self.b.b.a.int()) + encode(self.b.b.b.int()) +
-            encode(self.b.a.a.int()) + encode(self.b.a.b.int()) +
-            encode(self.a.b.a.int()) + encode(self.a.b.b.int()) +
-            encode(self.c.b.a.int()) + encode(self.c.b.b.int())
-        )
-
-class python:
-    """
-    Wrapper class for pure-Python implementations of primitive operations.
-
-    This class encapsulates pure-Python variants of all classes exported by
-    this module and of all the underlying low-level operations:
-    :obj:`python.pnt <pnt>`, :obj:`python.bas <bas>`,
-    :obj:`python.can <can>`, :obj:`python.ser <ser>`,
-    :obj:`python.des <des>`, :obj:`python.mul <mul>`,
-    :obj:`python.add <add>`, :obj:`python.sub <sub>`,
-    :obj:`python.neg <neg>`, :obj:`python.par <par>`,
-    :obj:`python.rnd <rnd>`, :obj:`python.scl <scl>`,
-    :obj:`python.sse <sse>`, :obj:`python.sde <sde>`,
-    :obj:`python.inv <inv>`, :obj:`python.smu <smu>`,
-    :obj:`python.sad <sad>`, :obj:`python.ssu <ssu>`,
-    :obj:`python.sne <sne>`,
-    :obj:`python.pnt2 <pnt2>`, :obj:`python.bas2 <bas2>`,
-    :obj:`python.can2 <can2>`, :obj:`python.ser2 <ser2>`,
-    :obj:`python.des2 <des2>`, :obj:`python.mul2 <mul2>`,
-    :obj:`python.add2 <add2>`, :obj:`python.sub2 <sub2>`,
-    :obj:`python.neg2 <neg2>`,
-    :obj:`python.rnd2 <rnd2>`, :obj:`python.scl2 <scl2>`,
-    :obj:`python.sse2 <sse2>`, :obj:`python.sde2 <sde2>`,
-    :obj:`python.inv2 <inv2>`, :obj:`python.smu2 <smu2>`,
-    :obj:`python.sad2 <sad2>`,
-    :obj:`python.point <oblivious.bn254.python.point>`,
-    :obj:`python.scalar <oblivious.bn254.python.scalar>`,
-    :obj:`python.point2 <oblivious.bn254.python.point2>`, and
-    :obj:`python.scalar2 <oblivious.bn254.python.scalar2>`.
-    For example, you can perform multiplication of scalars
-    using the pure-Python scalar multiplication implementation.
-
-    >>> s = python.scl()
-    >>> t = python.scl()
-    >>> python.smu(s, t) == python.smu(t, s)
-    True
-
-    Pure-Python variants of the :obj:`python.point <point>`
-    and :obj:`python.scalar <scalar>` classes always employ pure
-    Python implementations of operations when their methods are
-    invoked.
-
-    >>> p = python.scalar()
-    >>> q = python.scalar()
-    >>> p * q == q * p
-    True
-    """
-    @staticmethod
-    def pnt(h: Optional[bytes] = None) -> point:
-        """
-        Construct a point from its 64-byte vector representation (normally
-        obtained via hashing).
-
-        >>> p = python.pnt(hashlib.sha512('123'.encode()).digest())
-        >>> p.hex()[:64]
-        '6d68495eb4d539db4df70fd24d54fae37c9adf7dfd8dc705ccb8de8630e7cf22'
-        """
-        return bytes.__new__(
-            python.point,
-            (_ECp.random() if h is None else _ECp.mapfrom(h)).serialize()
-        )
-
-    @staticmethod
-    def bas(s: scalar) -> point:
-        """
-        Return the base point multiplied by the supplied scalar.
-
-        >>> bytes(python.bas(python.scalar.hash('123'.encode()))).hex()[:64]
-        '2d66076815cda25556bab4a930244ac284412267e9345aceb98d71530308401a'
-        """
-        return s * python.point.from_base64(
-            'hQAAAAAAAJGJAAAAAADnpzoAAACAHm4XDAAAwI+/9wO'
-            'O////////FYr//////zm5zf////8uxqL1//9/8qQrIY'
-            '7///////8Viv//////ObnN/////y7GovX//3/ypCsh'
-        )
-
-    @staticmethod
-    def can(p: point) -> point:
-        """
-        Normalize the representation of a point into its canonical form
-        and return the result.
-
-        >>> a = python.point.hash('123'.encode())
-        >>> p = python.add(a, a)
-        >>> p_can = python.can(python.add(a, a))
-
-        It may be the case that ``ser(p_can) != ser(p)``, depending on the
-        implementation. It is the responsibility of the user to ensure
-        that only canonical forms are serialized if those serialized forms
-        must be compared.
-
-        >>> mclbn256 = p.__class__ != python.point
-        >>> (python.ser(p_can) != python.ser(p)) or not mclbn256
-        True
-
-        Normalization is idempotent.
-
-        >>> python.can(p) == python.can(p_can)
-        True
-        """
-        return p # This instance's coordinates are already in normal affine form.
-
-    @staticmethod
-    def ser(p: point) -> bytes:
-        """
-        Return the binary representation of a point.
-
-        >>> q = python.point2.hash('123'.encode())
-        >>> python.des(python.ser(q)) == q
-        True
-        """
-        return bytes(b for b in p)
-
-    @staticmethod
-    def des(bs: bytes) -> point:
-        """
-        Construct a point corresponding to the supplied binary representation.
-
-        >>> p = python.point.hash('123'.encode())
-        >>> python.ser_p = bytes.fromhex(
-        ...     '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
-        ...     'b03c992ec97868be765b98048118a96f42bdc466a963c243c223b95196304209'
-        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-        ... )
-        >>> python.des(python.ser_p) == p
-        True
-        >>> python.ser(python.des(python.ser_p)) == python.ser_p
-        True
-        """
-        # It may be useful to debug with ``_ECp.deserialize(bs).serialize()``
-        # in place of just ``bs``.
-        return bytes.__new__(python.point, bs)
-
-    @staticmethod
-    def mul(s: scalar, p: point) -> point:
-        """
-        Multiply a point by a scalar and return the result.
-
-        >>> p = python.pnt(hashlib.sha512('123'.encode()).digest())
-        >>> s = python.scl(bytes.fromhex(
-        ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-        ... ))
-        >>> python.mul(s, p).hex()[:64]
-        '68b5dd61adaa83f1511efe7b4749481cc9f86e11bf82d82960b6c56373de0d24'
-        """
-        return bytes.__new__(python.point, _ECp(int(s) * _ECp.deserialize(p)).serialize())
-
-    @staticmethod
-    def add(p: point, q: point) -> point:
-        """
-        Return the sum of the supplied points.
-
-        >>> p = python.point.hash('123'.encode())
-        >>> q = python.point.hash('456'.encode())
-        >>> python.point.to_bytes(python.add(p, q)).hex()[:64]
-        '1ea48cab238fece46bd0c9fb562c859e318e17a8fb75517a4750d30ca79b911c'
-        >>> python.add(python.sub(p, q), q) == p
-        True
-        """
-        return bytes.__new__(
-            python.point,
-            _ECp.serialize(_ECp.deserialize(p).add(_ECp.deserialize(q)))
-        )
-
-    @staticmethod
-    def sub(p: point, q: point) -> point:
-        """
-        Return the result of subtracting the right-hand point from the
-        left-hand point.
-
-        >>> p = python.point.hash('123'.encode())
-        >>> q = python.point.hash('456'.encode())
-        >>> python.sub(p, q).hex()[:64]
-        'a43a5ce1931b1300b62e5d7e1b0c691203bfd85fafd9585dc5e47a7e2acfea22'
-        >>> python.sub(python.add(p, q), q) == p
-        True
-        """
-        return bytes.__new__(
-            python.point,
-            _ECp.serialize(_ECp.deserialize(p).add(-1 * _ECp.deserialize(q)))
-        )
-
-    @staticmethod
-    def neg(p: point) -> point:
-        """
-        Return the additive inverse of a point.
-
-        >>> p = python.point.hash('123'.encode())
-        >>> python.point.to_bytes(python.neg(p)).hex()[:64]
-        '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
-        """
-        return bytes.__new__(python.point, _ECp.serialize(-1 * _ECp.deserialize(p)))
-
-    @staticmethod
-    def rnd() -> scalar:
-        """
-        Return random non-zero scalar.
-
-        >>> isinstance(python.rnd(), python.scalar)
-        True
-        """
-        # d = 0x212ba4f27ffffff5a2c62effffffffd00242ffffffffff9c39ffffffffffffb2
-        # return int.to_bytes(((secrets.randbelow(r-1)+1) * d) % r, 32, 'little')
-
-        return python.scalar(int.to_bytes(secrets.randbelow(r-1)+1, 32, 'little'))
-
-    @classmethod
-    def scl(cls, s: Union[bytes, bytearray, None] = None) -> Optional[scalar]:
-        """
-        Construct a scalar if the supplied bytes-like object represents
-        a valid scalar; otherwise, return ``None``. If no byte vector is
-        supplied, return a random scalar.
-
-        >>> s = python.scl()
-        >>> t = python.scl(s)
-        >>> s == t
-        True
-        >>> python.scl(bytes([255] * 32)) is None
-        True
-        """
-        if s is None:
-            return python.rnd()
-
-        if int.from_bytes(s, 'little') < r:
-            return bytes.__new__(python.scalar, s)
-
-        return None
-
-    @staticmethod
-    def sse(s: scalar) -> bytes:
-        """
-        Return the binary representation of a scalar.
-
-        >>> s = python.scalar.hash('123'.encode())
-        >>> python.sde(python.sse(s)) == s
-        True
-        """
-        return bytes(b for b in s)
-
-    @staticmethod
-    def sde(bs: bytes) -> scalar:
-        """
-        Construct a scalar from its binary representation.
-
-        >>> s = python.scalar.hash('123'.encode())
-        >>> bs = bytes.fromhex(
-        ...     '93d829354cb3592743174133104b5405ba6992b67bb219fbde3e394d70505913'
-        ... )
-        >>> python.sde(bs) == s
-        True
-        >>> python.sse(python.sde(bs)) == bs
-        True
-        """
-        return bytes.__new__(python.scalar, bs)
-
-    @staticmethod
-    def inv(s: scalar) -> scalar:
-        """
-        Return the inverse of a scalar (modulo
-        ``r = 16798108731015832284940804142231733909759579603404752749028378864165570215949``
-        in the prime field `F*_r`).
-
-        >>> s = python.scl()
-        >>> p = python.pnt()
-        >>> python.mul(python.inv(s), python.mul(s, p)) == p
-        True
-        """
-        return python.scalar.from_int(bn.invmodp(int(s), r))
-
-    @staticmethod
-    def smu(s: scalar, t: scalar) -> scalar:
-        """
-        Return the product of two scalars.
-
-        >>> s = python.scl()
-        >>> t = python.scl()
-        >>> python.smu(s, t) == python.smu(t, s)
-        True
-        """
-        n = (python.scalar.__int__(s) * python.scalar.__int__(t)) % r
-        return python.scalar.from_int(n)
-
-    @staticmethod
-    def sad(s: scalar, t: scalar) -> scalar:
-        """
-        Return the sum of two scalars.
-
-        >>> s = python.scl()  # Could be `python.scl()`.
-        >>> t = python.scl()
-        >>> python.sad(s, t) == python.sad(t, s)
-        True
-        """
-        return python.scalar.from_int((int(s) + int(t)) % r)
-
-    @staticmethod
-    def ssu(s: scalar, t: scalar) -> scalar:
-        """
-        Return the result of subtracting the right-hand scalar from the
-        left-hand scalar.
-
-        >>> s = python.scl()
-        >>> t = python.scl()
-        >>> python.ssu(s, t) == python.sad(s, python.sne(t))
-        True
-        >>> python.ssu(s, t) == python.sne(python.ssu(t, s))
-        True
-        """
-        return python.scalar.from_int((int(s) - int(t)) % r)
-
-    @staticmethod
-    def sne(s: scalar) -> scalar:
-        """
-        Return the additive inverse of a scalar.
-
-        >>> s = python.scl()
-        >>> t = python.scl()
-        >>> python.sne(python.sne(s)) == s
-        True
-        """
-        return python.scalar.from_int(r - int(s))
-
-    @staticmethod
-    def pnt2(h: Optional[bytes] = None) -> point2:
-        """
-        Construct a second-level point if the supplied bytes-like object
-        represents a valid second-level point; otherwise, return ``None``.
-        If no byte vector is supplied, return a random second-level point.
-
-        >>> p = python.pnt2(hashlib.sha512('123'.encode()).digest())
-        >>> python.point2.to_bytes(p).hex()[:128] == (
-        ...     '4c595542640a69c4a70bda55c27ef96c133cd1f4a5f83b3371e571960c018e19'
-        ...     'c54aaec2069f8f10a00f12bcbb3511cdb7356201f5277ec5e47da91405be2809'
-        ... )
-        True
-        """
-        return bytes.__new__(
-            python.point2,
-            (_ECp2.random() if h is None else _ECp2.mapfrom(h)).serialize()
-        )
-
-    @staticmethod
-    def bas2(s: scalar) -> point2:
-        """
-        Return the base second-level point multiplied by the supplied scalar.
-
-        >>> bytes(python.bas2(python.scalar.hash('123'.encode()))).hex()[:64]
-        'e7000fb12d206112c73fe1054e9d77b35c77881eba6598b7e035171d90b13e0c'
-        """
-        # return s * _ECp2.__new__(python.point2, get_base2())
-        return bytes.__new__(python.point2, _ECp2(int(s) * get_base2()).serialize())
-
-    @staticmethod
-    def can2(p: point2) -> point2:
-        """
-        Normalize the representation of a second-level point into its canonical
-        form and return the result.
-
-        >>> p = python.bas2(scalar.from_int(1))
-        >>> python.ser(python.can2(p)).hex()[:64]
-        '669e6563afaa45af7cbc013d23f092bb3763d4dc41b97aef555bdf61de713f17'
-        """
-        return p # This instance's coordinates are already in normal affine form.
-
-    @staticmethod
-    def ser2(p: point2) -> bytes:
-        """
-        Return the binary representation of a second-level point.
-
-        >>> p = python.point2.hash('123'.encode())
-        >>> python.des2(python.ser2(p)) == p
-        True
-
-        It is the responsibility of the user to ensure that only canonical
-        representations of points are serialized.
-        """
-        return bytes(b for b in p)
-
-    @staticmethod
-    def des2(bs: bytes) -> point2:
-        """
-        Return the second-level point corresponding to the supplied binary
-        representation thereof.
-
-        >>> p = python.point2.hash('123'.encode())
-        >>> ser_p = bytes.fromhex(
-        ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
-        ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
-        ...     '2c6a88bb448065eb748df632b1d872e02f54b6f56fdb84a7b1cb388fe551fb08'
-        ...     '04464efa186bd4b1371e53d6f31f0e2f50ff553b6264a43331b42c976a0c541f'
-        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-        ...     '0000000000000000000000000000000000000000000000000000000000000000'
-        ... )
-        >>> python.des2(ser_p) == p
-        True
-        >>> python.ser(python.des2(ser_p)) == ser_p
-        True
-        """
-        return bytes.__new__(python.point2, bs)
-        # It may be useful to debug with _ECp2.deserialize(bs).serialize() in place of just bs.
-
-    @staticmethod
-    def mul2(s: scalar, p: point2) -> point2:
-        """
-        Multiply a second-level point by a scalar.
-
-        >>> p = python.point2.hash('123'.encode())
-        >>> s = python.scl(bytes.fromhex(
-        ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-        ... ))
-        >>> python.point2.to_bytes(python.mul2(s, p)).hex() == (
-        ...     '5f6f2ace8566ca47354fbe244ae3e6a854c37011fb6d6ac56571c94169e4ab18'
-        ...     '650bea4cfed5c9603e5949fe3d7509b17e20db4ff1f05129aad0d0a3bffb0008'
-        ...     '3043c5a14b986882836b1c929952ea3881d04ca44d487d1ab2d4c0b171b87d14'
-        ...     '5dca6dabb4f0ea7be5c95a861ed319d146b15d70542d3952af995a8bb35b8314'
-        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-        ...     '0000000000000000000000000000000000000000000000000000000000000000'
-        ... )
-        True
-        """
-        return bytes.__new__(python.point2, _ECp2(int(s) * _ECp2.deserialize(p)).serialize())
-
-    @staticmethod
-    def add2(p: point2, q: point2) -> point2:
-        """
-        Return sum of the supplied second-level points.
-
-        >>> p = python.point2.hash('123'.encode())
-        >>> q = python.point2.hash('456'.encode())
-        >>> python.point2.to_bytes(python.add2(p, q)).hex() == (
-        ...     'cb0fc423c1bac2ac2df47bf5f5548a42b0d0a0da325bc77243d15dc587a7b221'
-        ...     '9808a1649991ddf770f0060333aab4d499580b123f109b5cb180f1f8a75a090e'
-        ...     '83dd34d9ecdd6fd639230f7f0cf44b218fae4d879111de6c6c037e6ffdcdc823'
-        ...     'f5a48318143873ca90ad512a2ea1854200eea5537cd0ac93691d5b94ff36b212'
-        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-        ...     '0000000000000000000000000000000000000000000000000000000000000000'
-        ... )
-        True
-        """
-        return bytes.__new__(
-            python.point2,
-            _ECp2(_ECp2.deserialize(p).add(_ECp2.deserialize(q))).serialize()
-        )
-
-    @staticmethod
-    def sub2(p: point2, q: point2) -> point2:
-        """
-        Return the result of subtracting right-hand second-level point from the
-        left-hand second-level point.
-
-        >>> p = python.point2.hash('123'.encode())
-        >>> q = python.point2.hash('456'.encode())
-        >>> python.point2.to_bytes(python.sub2(p, q)).hex() == (
-        ...     'e97a70c4e3a5369ebbb1dcf0cc1135c8c8e04a4ec7cffdf875ac429d66846d0b'
-        ...     '191b090909c40a723027b07ac44435a6ade3813d04b3632a17c92c5c98718902'
-        ...     '407c58ed13cc0c0aaa43d0eafd44080080c8199401fe4f8ed7dd0eb5fba86817'
-        ...     '141f74341ce3c4884f86a97f51f7c0b208fe52be336b7651252fa9881c93d203'
-        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-        ...     '0000000000000000000000000000000000000000000000000000000000000000'
-        ... )
-        True
-        """
-        return bytes.__new__(
-            python.point2,
-            _ECp2(_ECp2.deserialize(p).add(-1 * _ECp2.deserialize(q))).serialize()
-        )
-
-    @staticmethod
-    def neg2(p: point2) -> point2:
-        """
-        Return the negation of a second-level point.
-
-        >>> p = python.point2.hash('123'.encode())
-        >>> python.point2.to_bytes(python.neg2(p)).hex() == (
-        ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
-        ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
-        ...     'e7957744bb7f9abb9e7209cd4e27ae80d8ab490a1072af125034c7b09c12281c'
-        ...     '0fbab105e7942bf5dbe1ac290ce01232b800aac41de98f86d04bd3a81758cf05'
-        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-        ...     '0000000000000000000000000000000000000000000000000000000000000000'
-        ... )
-        True
-        """
-        return bytes.__new__(python.point2, _ECp2(-1 * _ECp2.deserialize(p)).serialize())
-
-    @staticmethod
-    def rnd2() -> scalar2:
-        """
-        Return random non-zero second-level scalar.
-
-        >>> isinstance(python.rnd2(), python.scalar2)
-        True
-        """
-        return python.scalar2.hash(secrets.token_bytes(384))
-
-    @staticmethod
-    def scl2(s: Union[bytes, bytearray, None] = None) -> Optional[scalar2]:
-        """
-        Construct a second-level scalar if the supplied bytes-like object
-        represents a valid second-level scalar; otherwise, return ``None``.
-        If no byte vector is supplied, return a random second-level scalar.
-
-        >>> bs = bytes.fromhex(
-        ...     '18d0e065798ffa4ecca0a7cc6e2b8d6d3269f7eb413525e59b731332b02ea805'
-        ...     '4b90c89ce93e4452557f53aae5f8f13221858dde2ea6a50373f1858f11287021'
-        ...     '09b3daf7a217a20a3d872632f8ced643d32649b241a67601bec855bd43f07710'
-        ...     '88df722bcacc8fd174f16ad7ef1b1d5e622d93b7cfec6385c353c13793a4e01c'
-        ...     '371ef54cd836a88e1b1f1e198d566d3bbe5aa225734305f14cac9af9c821351c'
-        ...     '86b365190105d1b7e71011d1362ed6ad9133a2c2c42898e9ebc3d1604a608f10'
-        ...     '8461d37b2463b4f88f0ccb427b5eea8714ee88f8c33daf7ee4a3f45ca8bca911'
-        ...     '87956abb4d27de1b49e5e059f904fbb475804715ab25a17306fa0e196f305215'
-        ...     '3a60dfa073ca78de49edeaac9c54cab3d0138750c23c0b68de7924a69d1ba002'
-        ...     'a24ac592622a45c59c1ded7133794292a09602bd57a36601d35438846fcb370f'
-        ...     '39c0fa7a15b34d14ab6f95ee5bf5b26bd5def1e7ed07350922d445da07d93622'
-        ...     '2db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
-        ... )
-        >>> python.scalar2.to_bytes(python.scl2(bs)).hex()[700:]
-        '36222db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
-        """
-        if s is None:
-            return python.rnd2()
-
-        try:
-            return python.sde2(s)
-        except ValueError: # pragma: no cover
-            return None
-
-    @staticmethod
-    def sse2(s: scalar2) -> bytes:
-        """
-        Return the binary representation of a second-level scalar.
-
-        >>> s = python.scalar2.hash('123'.encode())
-        >>> python.sde2(python.sse2(s)) == s
-        True
-        """
-        return bytes(b for b in s)
-
-    @staticmethod
-    def sde2(bs: bytes) -> scalar2:
-        """
-        Construct a second-level scalar from its binary representation.
-
-        >>> s = python.scalar2.hash('123'.encode())
-        >>> bs = bytes.fromhex(
-        ...     '36980a8359d40e106075488e80cf1479f2e6ba95d6a99a67832d21b7b94d8c1d'
-        ...     '5eb4d655f23e1d5d499d51d1c552b5e7df6943091427cd080f582e120613a021'
-        ...     '85898ef7d016e47a74a8df62316cc4ad975cb64bb63867ed9b5221f77bb9a121'
-        ...     '7bd89cd213eee0c3fdf2e0e13ef9e30383ea5607c8d13fc10e04448a6c964a00'
-        ...     '04a098a55beab09732220966319333608b2187ee2196eb5b4253bc2b1aea5303'
-        ...     '654260dd687a2eb176a494258ff7ef753f93105a6f0e9f46c926afdbe31ff124'
-        ...     '6bdd87c32537abcdb46ad542792edd74a229c9ba61abcd993f074237a91f5215'
-        ...     '8f6b07886895733edde15cb22129459162d89d3662826b74e4fcbe4e9e8c2420'
-        ...     'bd53586a09f91ff8f67f92cba72c5b64a9c3965c01e93710200ab4e084955316'
-        ...     'fb18950835b79fb4c2930efcc5fcaa9d82ee0faff036b80657daee233a445901'
-        ...     '7df3e57cb535ed26162b3ee0f8961131a93fe3198dc5393d277ed8bac5532411'
-        ...     '93b7ad15c52ca123fd26f592a2219b1bf118b3035893cc4abf614b422f978718'
-        ... )
-        >>> python.sde2(bs) == s
-        True
-        >>> python.sse(python.sde2(bs)) == bs
-        True
-        """
-        return bytes.__new__(python.scalar2, bs)
-
-    @staticmethod
-    def inv2(s: scalar2) -> scalar2:
-        """
-        Return the inverse of a second-level scalar.
-
-        >>> s = python.scl2()
-        >>> python.smu2(s, python.smu2(s, python.inv2(s))) == s
-        True
-        >>> python.smu2(python.smu2(s, s), python.inv2(s)) == s
-        True
-        """
-        return bytes.__new__(
-            python.scalar2,
-            _Fp12(_Fp12.deserialize(s).inverse()).serialize()
-        )
-
-    @staticmethod
-    def smu2(s: scalar2, t: scalar2) -> scalar2:
-        """
-        Return second-level scalar multiplied by another scalar.
-
-        >>> s = python.scalar2.random()
-        >>> t = python.scalar2.random()
-        >>> python.smu2(s, t) == python.smu2(t, s)
-        True
-        """
-        return bytes.__new__(
-            python.scalar2,
-            _Fp12(_Fp12.deserialize(s) * _Fp12.deserialize(t)).serialize()
-        )
-
-    @staticmethod
-    def sad2(s: scalar2, t: scalar2) -> scalar2:
-        """
-        Return scalar2 added to another scalar2.
-
-        >>> s = python.scl2()
-        >>> t = python.scl2()
-        >>> python.sad2(s, t) == python.sad2(t, s)
-        True
-        """
-        return bytes.__new__(
-            python.scalar2,
-            _Fp12(_Fp12.deserialize(s) + _Fp12.deserialize(t)).serialize()
-        )
-
-# Indicate that data structures based on the dynamic/shared library
-# in mclbn256 have not (yet, at least) been defined.
-mclbn256 = False
-
-#
-# Attempt to load primitives from mclbn256, if it is present;
-# otherwise, use the mclbn256 library.
-#
-
-try:
-    # Attempt to load mclbn256 with its (bundled) shared/dynamic library file.
-    from mclbn256 import Fr, G1, G2, GT # pylint: disable=import-error
-
-    # pylint: disable=C2801,W0621
-    class mcl:
-        """
-        Wrapper class for binary implementations of primitive
-        operations.
-
-        When this module is imported, it makes a number of attempts
-        to locate an instance of the shared/dynamic library file of the
-        `mclbn256 <https://doc.mclbn256.org>`__ library on the host
-        system. The sequence of attempts is listed below, in order.
-
-        1. It uses ``ctypes.util.find_library`` to look for ``'mcl'``
-           or ``'mclbn256'``.
-
-        2. It attempts to find a file ``mclbn256.so`` or ``mclbn256.dll``
-           in the paths specified by the ``PATH`` and ``LD_LIBRARY_PATH``
-           environment variables.
-
-        3. If the `mclbn256 <https://pypi.org/project/mclbn256>`__ package is
-           installed, it reverts to the compiled subset of mclbn256
-           included in that package.
-
-        If all of the above fail, then :obj:`mcl` is assigned
-        the value ``None`` and all classes exported by this module default
-        to their pure-Python variants (*i.e.*, those encapsulated within
-        :obj:`~oblivious.bn254.python`). One way to confirm that a
-        dynamic/shared library *has been found* when this module
-        is imported is to evaluate the expression ``mcl is not None``.
-
-        If a shared/dynamic library file has been loaded successfully,
-        this class encapsulates shared/dynamic library variants of all classes
-        exported by this module and of all the underlying low-level operations:
-        :obj:`mcl.pnt <pnt>`, :obj:`mcl.bas <bas>`,
-        :obj:`mcl.can <can>`, :obj:`mcl.ser <ser>`,
-        :obj:`mcl.des <des>`, :obj:`mcl.mul <mul>`,
-        :obj:`mcl.add <add>`, :obj:`mcl.sub <sub>`,
-        :obj:`mcl.neg <neg>`, :obj:`mcl.par <par>`,
-        :obj:`mcl.rnd <rnd>`, :obj:`mcl.scl <scl>`,
-        :obj:`mcl.sse <sse>`, :obj:`mcl.sde <sde>`,
-        :obj:`mcl.inv <inv>`, :obj:`mcl.smu <smu>`,
-        :obj:`mcl.sad <sad>`, :obj:`mcl.ssu <ssu>`,
-        :obj:`mcl.sne <sne>`,
-        :obj:`mcl.pnt2 <pnt2>`, :obj:`mcl.bas2 <bas2>`,
-        :obj:`mcl.can2 <can2>`, :obj:`mcl.ser2 <ser2>`,
-        :obj:`mcl.des2 <des2>`, :obj:`mcl.mul2 <mul2>`,
-        :obj:`mcl.add2 <add2>`, :obj:`mcl.sub2 <sub2>`,
-        :obj:`mcl.neg2 <neg2>`,
-        :obj:`mcl.rnd2 <rnd2>`, :obj:`mcl.scl2 <scl2>`,
-        :obj:`mcl.sse2 <sse2>`, :obj:`mcl.sde2 <sde2>`,
-        :obj:`mcl.inv2 <inv2>`, :obj:`mcl.smu2 <smu2>`,
-        :obj:`mcl.sad2 <sad2>`,
-        :obj:`mcl.point <oblivious.bn254.mcl.point>`,
-        :obj:`mcl.scalar <oblivious.bn254.mcl.scalar>`,
-        :obj:`mcl.point2 <oblivious.bn254.mcl.point2>`, and
-        :obj:`mcl.scalar2 <oblivious.bn254.mcl.scalar2>`.
-        For example, you can perform addition of points using the point
-        addition implementation found in the shared/dynamic library
-        bundled with the instance of the package
-        `mclbn256 <https://pypi.org/project/mclbn256>`__ that is found
-        on the host system.
-
-        >>> p = mcl.pnt()
-        >>> q = mcl.pnt()
-        >>> mcl.add(p, q) == mcl.add(q, p)
-        True
-
-        Methods found in the shared/dynamic library variants of the
-        :obj:`point`, :obj:`scalar`, :obj:`point2`, and :obj:`scalar2`
-        classes are wrappers for the shared/dynamic library
-        implementations of the underlying operations.
-
-        >>> p = mcl.point()
-        >>> q = mcl.point()
-        >>> p + q == q + p
-        True
-        """
-        # pylint: disable=too-many-public-methods
-
-        @staticmethod
-        def pnt(h: Union[bytes, bytearray, None] = None) -> G1:
-            """
-            Construct a point if the supplied bytes-like object represents
-            a valid point; otherwise, return ``None``. If no byte vector is
-            supplied, return a random point.
-
-            >>> p = mcl.pnt(hashlib.sha512('123'.encode()).digest())
-            >>> p.__class__ = point
-            >>> mcl.point.to_bytes(p).hex()[:64]
-            '6d68495eb4d539db4df70fd24d54fae37c9adf7dfd8dc705ccb8de8630e7cf22'
-            """
-            return G1.random() if h is None else G1.mapfrom(h)
-
-        @staticmethod
-        def bas(s: Fr) -> G1:
-            """
-            Return the base point multiplied by the supplied scalar.
-
-            >>> p = mcl.bas(mcl.scalar.hash('123'.encode())).normalize().normalize()
-            >>> p.__class__ = point
-            >>> mcl.point.to_bytes(p).hex()[:64]
-            '2d66076815cda25556bab4a930244ac284412267e9345aceb98d71530308401a'
-            """
-            return G1.base_point() * s
-
-        @staticmethod
-        def can(p: G1) -> G1:
-            """
-            Normalize the representation of a point into its canonical form and
-            return the result.
-
-            >>> a = mcl.point.hash('123'.encode())
-            >>> p = mcl.add(a, a)
-            >>> p_can = mcl.can(mcl.add(a, a))
-
-            We may have ``ser(p_can) != ser(p)`` here, depending on the backend
-            implementation.  Either normalization matters, or MCl is not the backend.
-
-            >>> (mcl.ser(p_can) != mcl.ser(p)) or not mclbn256
-            True
-
-            Normalization is idempotent.
-
-            >>> mcl.can(p) == mcl.can(p_can)
-            True
-            """
-            return p.normalize() # Sets ``(x, y, z)`` to unique vector ``(x/z, y/z, 1)``.
-
-        @staticmethod
-        def ser(p: G1) -> bytes:
-            """
-            Return the binary representation of a point.
-
-            >>> p = mcl.point.hash('123'.encode())
-            >>> mcl.des(mcl.ser(p)) == p
-            True
-            """
-            IoEcProj, IoArrayRaw = 1024, 64 # Constants from mcl library. # pylint: disable=C0103
-            return p.tostr(IoEcProj|IoArrayRaw)[1:]
-
-        @staticmethod
-        def des(bs: bytes) -> G1:
-            """
-            Construct a point corresponding to the supplied binary representation.
-
-            >>> p = mcl.point.hash('123'.encode())
-            >>> ser_p = bytes.fromhex(
-            ...     '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
-            ...     'b03c992ec97868be765b98048118a96f42bdc466a963c243c223b95196304209'
-            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-            ... )
-            >>> mcl.des(ser_p) == p
-            True
-            >>> mcl.ser(mcl.des(ser_p)) == ser_p
-            True
-            """
-            IoEcProj, IoArrayRaw = 1024, 64  # MCl constants  # pylint: disable=C0103
-            return G1.new_fromstr(b"4"+bs, IoEcProj|IoArrayRaw)
-
-        @staticmethod
-        def mul(s: Fr, p: G1) -> G1:
-            """
-            Multiply a point by a scalar and return the result.
-
-            >>> p = mcl.pnt(hashlib.sha512('123'.encode()).digest())
-            >>> s = mcl.scl(bytes.fromhex(
-            ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-            ... ))
-            >>> q = mcl.mul(s, p).normalize().normalize()
-            >>> q.__class__ = point
-            >>> mcl.point.to_bytes(q).hex()[:64]
-            '68b5dd61adaa83f1511efe7b4749481cc9f86e11bf82d82960b6c56373de0d24'
-            """
-            return G1.__mul__(p, s)
-
-        @staticmethod
-        def add(p: G1, q: G1) -> G1:
-            """
-            Return the sum of the supplied points.
-
-            >>> p = mcl.point.hash('123'.encode())
-            >>> q = mcl.point.hash('456'.encode())
-            >>> r = mcl.add(p, q).normalize().normalize()
-            >>> r.__class__ = point
-            >>> mcl.point.to_bytes(r).hex()[:64]
-            '1ea48cab238fece46bd0c9fb562c859e318e17a8fb75517a4750d30ca79b911c'
-            """
-            return G1.__add__(p, q)
-
-        @staticmethod
-        def sub(p: G1, q: G1) -> G1:
-            """
-            Return the result of subtracting the right-hand point from the
-            left-hand point.
-
-            >>> p = mcl.point.hash('123'.encode())
-            >>> q = mcl.point.hash('456'.encode())
-            >>> r = mcl.sub(p, q).normalize().normalize()
-            >>> r.__class__ = point
-            >>> mcl.point.to_bytes(r).hex()[:64]
-            'a43a5ce1931b1300b62e5d7e1b0c691203bfd85fafd9585dc5e47a7e2acfea22'
-            """
-            return G1.__sub__(p, q)
-
-        @staticmethod
-        def neg(p: G1) -> G1:
-            """
-            Return the additive inverse of a point.
-
-            >>> p = mcl.point.hash('123'.encode())
-            >>> q = mcl.neg(p)
-            >>> q.__class__ = point
-            >>> mcl.point.to_bytes(q).hex()[:64]
-            '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
-            """
-            return G1.__neg__(p)
-
-        @staticmethod
-        def par(p: Union[G1, G2], q: Union[G1, G2]) -> GT:
-            """
-            Compute the pairing function on two points.
-
-            >>> p = mcl.point.hash('123'.encode())
-            >>> q = mcl.point2.base(mcl.scalar.from_int(456))
-            >>> r = mcl.par(p, q)
-            >>> r.__class__ = mcl.scalar2
-            >>> mcl.scalar2.to_bytes(r).hex()[700:]
-            'd01f7e038b05acc5519eeda026c4aa111eb12f3483f274c60e34e6ec7571435df707'
-
-            The order of the two arguments is not important (as long as exactly
-            one argument is an instance of :obj:`point` and the other is an
-            instance of :obj:`point2`).
-
-            >>> r = mcl.par(q, p)
-            >>> r.__class__ = mcl.scalar2
-            >>> mcl.scalar2.to_bytes(r).hex()[700:]
-            'd01f7e038b05acc5519eeda026c4aa111eb12f3483f274c60e34e6ec7571435df707'
-
-            The pairing function is bilinear.
-
-            >>> p = mcl.point.random()
-            >>> s = mcl.scalar.random()
-
-            >>> t = mcl.scalar.random()
-            >>> q = mcl.point2.random()
-            >>> -((~s) * (s * p)) - p == mcl.scalar.from_int(-2) * p
-            True
-            >>> s * t * p @ q == s * p @ (t * q)
-            True
-
-            Suppose there are two points: one multiplied by the scalar ``s`` and the other
-            multiplied by the scalar ``t``. Their equality can be determined by using a
-            balancing point: ``g**(~s * t)``.  If the pairing of ``t * x`` with ``g`` is the
-            same as the pairing with ``s * y`` and ``g**(~s * t)``, then ``x`` equals ``y``.
-
-            >>> x = y = p
-            >>> g = mcl.point2.base(mcl.scalar.from_int(1))
-            >>> b = mcl.point2.base(~s * t)
-            >>> (t * x) @ g == (s * y) @ b
-            True
-
-            This operation is defined only for a point and a second-level point.
-            Any attempt to invoke the operation on values or objects of other types
-            raises an exception.
-
-            >>> p @ (p + p)
-            Traceback (most recent call last):
-              ...
-            TypeError: pairing is defined only for a point and a second-level point
-            >>> g @ b
-            Traceback (most recent call last):
-              ...
-            TypeError: pairing is defined only for a point and a second-level point
-
-            Pairing is intended to be nonsingular.
-
-            >>> p @ q.clear()
-            Traceback (most recent call last):
-              ...
-            TypeError: cannot meaningfully pair the infinity point
-            >>> p.clear() @ g
-            Traceback (most recent call last):
-              ...
-            TypeError: cannot meaningfully pair the infinity point
-            """
-            if p.zero() or q.zero():
-                raise TypeError('cannot meaningfully pair the infinity point')
-
-            if (
-                (isinstance(p, G1) and isinstance(q, G1)) or
-                (isinstance(p, G2) and isinstance(q, G2))
-            ):
-                raise TypeError(
-                    'pairing is defined only for a point and a second-level point'
-                )
-
-            if isinstance(p, G1):
-                return G1.__matmul__(G1.__new__(G1, p), G2.__new__(G2, q))
-
-            return G2.__matmul__(G2.__new__(G2, p), G1.__new__(G1, q))
-
-        @staticmethod
-        def rnd() -> Fr:
-            """
-            Return random non-zero scalar.
-
-            >>> s = mcl.rnd()
-            >>> isinstance(s, Fr)
-            True
-            >>> s.__class__ = scalar
-            >>> len(mcl.scalar.to_bytes(s))
-            32
-            """
-            return Fr().randomize()
-
-        @classmethod
-        def scl(cls, bs: Union[bytes, bytearray, None] = None) -> Optional[Fr]:
-            """
-            Construct a scalar if the supplied bytes-like object represents
-            a valid scalar; otherwise, return ``None``. If no byte vector is
-            supplied, return a random scalar.
-
-            >>> s = mcl.scl()
-            >>> s.__class__ = scalar
-            >>> t = mcl.scl(mcl.scalar.to_bytes(s))
-            >>> s == t
-            True
-            >>> mcl.scl(bytes([255] * 32)) is None
-            True
-            """
-            if bs is None:
-                return cls.rnd()
-
-            try:
-                s = cls.sde(bs)
-                return s
-            except ValueError: # pragma: no cover
-                return None
-
-        @staticmethod
-        def sse(s: Fr) -> bytes:
-            """
-            Return the binary representation of a scalar.
-
-            >>> s = mcl.scalar.hash('123'.encode())
-            >>> mcl.sde(mcl.sse(s)) == s
-            True
-            """
-            IoEcProj, IoArrayRaw = 1024, 64 # Constants from mcl library. # pylint: disable=C0103
-            return s.tostr(IoEcProj|IoArrayRaw)
-
-        @staticmethod
-        def sde(bs: bytes) -> Fr:
-            """
-            Return a scalar from its binary representation.
-
-            >>> s = mcl.scalar.hash('123'.encode())
-            >>> bs = bytes.fromhex(
-            ...     '93d829354cb3592743174133104b5405ba6992b67bb219fbde3e394d70505913'
-            ... )
-            >>> mcl.sde(bs) == s
-            True
-            >>> mcl.sse(mcl.sde(bs)) == bs
-            True
-            """
-            IoEcProj, IoArrayRaw = 1024, 64  # MCl constants  # pylint: disable=C0103
-            return Fr.new_fromstr(bs, IoEcProj|IoArrayRaw)
-
-        @staticmethod
-        def inv(s: Fr) -> Fr:
-            r"""
-            Return inverse of a scalar (modulo
-            ``r = 16798108731015832284940804142231733909759579603404752749028378864165570215949``
-            in the prime field *F*\_*r*).
-
-            >>> (s, p) = (mcl.scl(), mcl.pnt())
-            >>> mcl.mul(mcl.inv(s), mcl.mul(s, p)) == p
-            True
-            """
-            return Fr.__invert__(s)
-
-        @staticmethod
-        def smu(s: Fr, t: Fr) -> Fr:
-            """
-            Return scalar multiplied by another scalar.
-
-            >>> (s, t) = (mcl.scl(), mcl.scl())
-            >>> mcl.smu(s, t) == mcl.smu(t, s)
-            True
-            """
-            return Fr.__mul__(s, t)
-
-        @staticmethod
-        def sad(s: Fr, t: Fr) -> Fr:
-            """
-            Return scalar added to another scalar.
-
-            >>> (s, t) = (mcl.scl(), mcl.scl())
-            >>> mcl.sad(s, t) == mcl.sad(t, s)
-            True
-            """
-            return Fr.__add__(s, t)
-
-        @staticmethod
-        def ssu(s: Fr, t: Fr) -> Fr:
-            """
-            Return the result of one scalar subtracted from another scalar.
-
-            >>> (s, t) = (mcl.scl(), mcl.scl())
-            >>> mcl.ssu(s, t) == mcl.sad(s, mcl.sne(t))
-            True
-            >>> mcl.ssu(s, t) == mcl.sne(mcl.ssu(t, s))
-            True
-            """
-            return Fr.__sub__(s, t)
-
-        @staticmethod
-        def sne(s: Fr) -> Fr:
-            """
-            Return the additive inverse of a scalar.
-
-            >>> (s, t) = (mcl.scl(), mcl.scl())
-            >>> mcl.sne(mcl.sne(s)) == s
-            True
-            """
-            return Fr.__neg__(s)
-
-        @staticmethod
-        def pnt2(h: Optional[bytes] = None) -> G2:
-            """
-            Construct a second-level point if the supplied bytes-like object
-            represents a valid second-level point; otherwise, return ``None``.
-            If no byte vector is supplied, return a random second-level point.
-
-            >>> p = mcl.pnt2(hashlib.sha512('123'.encode()).digest())
-            >>> p.__class__ = point2
-            >>> mcl.point2.to_bytes(p.canonical().canonical()).hex()[:128] == (
-            ...     '4c595542640a69c4a70bda55c27ef96c133cd1f4a5f83b3371e571960c018e19'
-            ...     'c54aaec2069f8f10a00f12bcbb3511cdb7356201f5277ec5e47da91405be2809'
-            ... )
-            True
-            """
-            return G2.random() if h is None else G2.mapfrom(h)
-
-        @staticmethod
-        def bas2(s) -> G2:
-            """
-            Return the base second-level point multiplied by the supplied scalar.
-
-            >>> r = mcl.bas2(mcl.scalar.hash('123'.encode())).normalize().normalize()
-            >>> r.__class__ = point2
-            >>> mcl.point2.to_bytes(r).hex()[:64]
-            'e7000fb12d206112c73fe1054e9d77b35c77881eba6598b7e035171d90b13e0c'
-            """
-            # return s * G2.__new__(point2, G2.base_point())
-            return G2.base_point() * s
-
-        @staticmethod
-        def can2(p: G2) -> G2:
-            """
-            Normalize the representation of a second-level point into its
-            canonical form and return the result.
-
-            >>> p = mcl.bas2(scalar.from_int(1))
-            >>> mcl.ser(mcl.can2(p)).hex()[:64]
-            '669e6563afaa45af7cbc013d23f092bb3763d4dc41b97aef555bdf61de713f17'
-            """
-            return p.normalize() # Sets ``(x, y, z)`` to unique vector ``(x/z, y/z, 1)``.
-
-        @staticmethod
-        def ser2(p: G2) -> bytes:
-            """
-            Return the binary representation of a second-level point.
-
-            >>> p = mcl.point2.hash('123'.encode())
-            >>> mcl.des2(mcl.ser2(p)) == p
-            True
-
-            It is the responsibility of the user to ensure that only canonical
-            representations of points are serialized.
-            """
-            IoEcProj, IoArrayRaw = 1024, 64 # Constants from mcl library. # pylint: disable=C0103
-            return p.tostr(IoEcProj|IoArrayRaw)[1:]
-
-        @staticmethod
-        def des2(bs: bytes) -> G2:
-            """
-            Return the second-level point corresponding to the supplied binary
-            representation thereof.
-
-            >>> p = mcl.point2.hash('123'.encode())
-            >>> mcl.ser_p = bytes.fromhex(
-            ...     'b5b0a52e43ba71ae03317333da4ba9452dbdbbec353ade0c732348e0bea4ba1b'
-            ...     '8860718e5ba784d55799ab292459a638f6399738a6de348742e6a789674f300d'
-            ...     '7e59c60a595253ebf69bf0794b7a032e59b6b5037adba410d680b53ffac08517'
-            ...     'cf5bc3be9d850ec64ea6939904cf66b66b6b4b82be03ee4f10661fedaf83841f'
-            ...     'ba7e678442a658340a5b3c51eb5076d738cf88387ada6cbd1fe7f8d8a2268417'
-            ...     'bc8aedbc99808b0450025d0c75b5f1ccb34bc69934cc620d9ea51038a1d98721'
-            ... )
-            >>> mcl.des2(mcl.ser_p) == p
-            True
-            >>> mcl.ser(mcl.des2(mcl.ser_p)) == mcl.ser_p
-            True
-            """
-            IoEcProj, IoArrayRaw = 1024, 64  # MCl constants  # pylint: disable=C0103
-            return G2.new_fromstr(b"4"+bs, IoEcProj|IoArrayRaw)
-
-        @staticmethod
-        def mul2(s: Fr, p: G2) -> G2:
-            """
-            Multiply a second-level point by a scalar.
-
-            >>> p = mcl.point2.hash('123'.encode())
-            >>> s = mcl.scl(bytes.fromhex(
-            ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-            ... ))
-            >>> r = mcl.mul2(s, p).normalize().normalize()
-            >>> r.__class__ = point2
-            >>> mcl.point2.to_bytes(r).hex() == (
-            ...     '5f6f2ace8566ca47354fbe244ae3e6a854c37011fb6d6ac56571c94169e4ab18'
-            ...     '650bea4cfed5c9603e5949fe3d7509b17e20db4ff1f05129aad0d0a3bffb0008'
-            ...     '3043c5a14b986882836b1c929952ea3881d04ca44d487d1ab2d4c0b171b87d14'
-            ...     '5dca6dabb4f0ea7be5c95a861ed319d146b15d70542d3952af995a8bb35b8314'
-            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-            ...     '0000000000000000000000000000000000000000000000000000000000000000'
-            ... )
-            True
-            """
-            return G2.__mul__(p, s)
-
-        @staticmethod
-        def add2(p: G2, q: G2) -> G2:
-            """
-            Return sum of the supplied second-level points.
-
-            >>> p = mcl.point2.hash('123'.encode())
-            >>> q = mcl.point2.hash('456'.encode())
-            >>> r = mcl.add2(p, q).normalize().normalize()
-            >>> r.__class__ = point2
-            >>> mcl.point2.to_bytes(r).hex() == (
-            ...     'cb0fc423c1bac2ac2df47bf5f5548a42b0d0a0da325bc77243d15dc587a7b221'
-            ...     '9808a1649991ddf770f0060333aab4d499580b123f109b5cb180f1f8a75a090e'
-            ...     '83dd34d9ecdd6fd639230f7f0cf44b218fae4d879111de6c6c037e6ffdcdc823'
-            ...     'f5a48318143873ca90ad512a2ea1854200eea5537cd0ac93691d5b94ff36b212'
-            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-            ...     '0000000000000000000000000000000000000000000000000000000000000000'
-            ... )
-            True
-            """
-            return G2.__add__(p, q)
-
-        @staticmethod
-        def sub2(p: G2, q: G2) -> G2:
-            """
-            Return the result of subtracting the right-hand second-level point
-            from the left-hand second-level point.
-
-            >>> p = mcl.point2.hash('123'.encode())
-            >>> q = mcl.point2.hash('456'.encode())
-            >>> r = mcl.sub2(p, q).normalize().normalize()
-            >>> r.__class__ = point2
-            >>> mcl.point2.to_bytes(r).hex() == (
-            ...     'e97a70c4e3a5369ebbb1dcf0cc1135c8c8e04a4ec7cffdf875ac429d66846d0b'
-            ...     '191b090909c40a723027b07ac44435a6ade3813d04b3632a17c92c5c98718902'
-            ...     '407c58ed13cc0c0aaa43d0eafd44080080c8199401fe4f8ed7dd0eb5fba86817'
-            ...     '141f74341ce3c4884f86a97f51f7c0b208fe52be336b7651252fa9881c93d203'
-            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-            ...     '0000000000000000000000000000000000000000000000000000000000000000'
-            ... )
-            True
-            """
-            return G2.__sub__(p, q)
-
-        @staticmethod
-        def neg2(p: G2) -> G2:
-            """
-            Return the negation of a second-level point.
-
-            >>> p = mcl.point2.hash('123'.encode())
-            >>> r = mcl.neg2(p).normalize().normalize()
-            >>> r.__class__ = point2
-            >>> mcl.point2.to_bytes(r).hex() == (
-            ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
-            ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
-            ...     'e7957744bb7f9abb9e7209cd4e27ae80d8ab490a1072af125034c7b09c12281c'
-            ...     '0fbab105e7942bf5dbe1ac290ce01232b800aac41de98f86d04bd3a81758cf05'
-            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-            ...     '0000000000000000000000000000000000000000000000000000000000000000'
-            ... )
-            True
-            """
-            return G2.__neg__(p)
-
-        @staticmethod
-        def rnd2() -> GT:
-            """
-            Return random non-zero second-level scalar.
-
-            >>> isinstance(mcl.rnd2(), GT)
-            True
-            """
-            return mcl.scalar2.hash(secrets.token_bytes(384))
-
-        @staticmethod
-        def scl2(s: Union[bytes, bytearray, None] = None) -> Optional[GT]:
-            """
-            Construct a second-level scalar if the supplied bytes-like object
-            represents a valid second-level scalar; otherwise, return ``None``.
-            If no byte vector is supplied, return a random second-level scalar.
-
-            >>> bs = bytes.fromhex(
-            ...     '18d0e065798ffa4ecca0a7cc6e2b8d6d3269f7eb413525e59b731332b02ea805'
-            ...     '4b90c89ce93e4452557f53aae5f8f13221858dde2ea6a50373f1858f11287021'
-            ...     '09b3daf7a217a20a3d872632f8ced643d32649b241a67601bec855bd43f07710'
-            ...     '88df722bcacc8fd174f16ad7ef1b1d5e622d93b7cfec6385c353c13793a4e01c'
-            ...     '371ef54cd836a88e1b1f1e198d566d3bbe5aa225734305f14cac9af9c821351c'
-            ...     '86b365190105d1b7e71011d1362ed6ad9133a2c2c42898e9ebc3d1604a608f10'
-            ...     '8461d37b2463b4f88f0ccb427b5eea8714ee88f8c33daf7ee4a3f45ca8bca911'
-            ...     '87956abb4d27de1b49e5e059f904fbb475804715ab25a17306fa0e196f305215'
-            ...     '3a60dfa073ca78de49edeaac9c54cab3d0138750c23c0b68de7924a69d1ba002'
-            ...     'a24ac592622a45c59c1ded7133794292a09602bd57a36601d35438846fcb370f'
-            ...     '39c0fa7a15b34d14ab6f95ee5bf5b26bd5def1e7ed07350922d445da07d93622'
-            ...     '2db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
-            ... )
-            >>> s = mcl.scl2(bs)
-            >>> s.__class__ = mcl.scalar2
-            >>> mcl.scalar2.to_bytes(s).hex()[700:]
-            '36222db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
-            """
-            if s is None:
-                return mcl.rnd2()
-
-            try:
-                return mcl.sde2(s)
-            except ValueError: # pragma: no cover
-                return None
-
-        @staticmethod
-        def sse2(s: scalar2) -> bytes:
-            """
-            Return the binary representation of a second-level scalar.
-
-            >>> s = scalar2.hash('123'.encode())
-            >>> mcl.sde2(mcl.sse2(s)) == s
-            True
-            """
-            IoEcProj, IoArrayRaw = 1024, 64 # Constants from mcl library. # pylint: disable=C0103
-            return s.tostr(IoEcProj|IoArrayRaw)
-
-        @staticmethod
-        def sde2(bs: bytes) -> GT:
-            """
-            Return the second-level scalar corresponding to the supplied binary
-            representation thereof.
-
-            >>> s = mcl.scalar2.hash('123'.encode())
-            >>> bs = bytes.fromhex(
-            ...     '36980a8359d40e106075488e80cf1479f2e6ba95d6a99a67832d21b7b94d8c1d'
-            ...     '5eb4d655f23e1d5d499d51d1c552b5e7df6943091427cd080f582e120613a021'
-            ...     '85898ef7d016e47a74a8df62316cc4ad975cb64bb63867ed9b5221f77bb9a121'
-            ...     '7bd89cd213eee0c3fdf2e0e13ef9e30383ea5607c8d13fc10e04448a6c964a00'
-            ...     '04a098a55beab09732220966319333608b2187ee2196eb5b4253bc2b1aea5303'
-            ...     '654260dd687a2eb176a494258ff7ef753f93105a6f0e9f46c926afdbe31ff124'
-            ...     '6bdd87c32537abcdb46ad542792edd74a229c9ba61abcd993f074237a91f5215'
-            ...     '8f6b07886895733edde15cb22129459162d89d3662826b74e4fcbe4e9e8c2420'
-            ...     'bd53586a09f91ff8f67f92cba72c5b64a9c3965c01e93710200ab4e084955316'
-            ...     'fb18950835b79fb4c2930efcc5fcaa9d82ee0faff036b80657daee233a445901'
-            ...     '7df3e57cb535ed26162b3ee0f8961131a93fe3198dc5393d277ed8bac5532411'
-            ...     '93b7ad15c52ca123fd26f592a2219b1bf118b3035893cc4abf614b422f978718'
-            ... )
-            >>> mcl.sde2(bs) == s
-            True
-            >>> mcl.sse(mcl.sde2(bs)) == bs
-            True
-            """
-            IoEcProj, IoArrayRaw = 1024, 64  # MCl constants  # pylint: disable=C0103
-            return GT.new_fromstr(bs, IoEcProj|IoArrayRaw)
-
-        @staticmethod
-        def inv2(s: GT) -> GT:
-            """
-            Return the inverse of a second-level scalar.
-
-            >>> s = mcl.scl2()
-            >>> mcl.smu2(s, mcl.smu2(s, mcl.inv2(s))) == s
-            True
-            >>> mcl.smu2(mcl.smu2(s, s), mcl.inv2(s)) == s
-            True
-            """
-            return GT.__inv__(s)
-
-        @staticmethod
-        def smu2(s: GT, t: GT) -> GT:
-            """
-            Return the product of two second-level scalars.
-
-            >>> p1 = mcl.point.hash('123'.encode())
-            >>> p2 = mcl.point.hash('456'.encode())
-            >>> q1 = mcl.point2.base(mcl.scalar.hash('123'.encode()))
-            >>> q2 = mcl.point2.base(mcl.scalar.hash('456'.encode()))
-            >>> s = p1 @ q1
-            >>> t = p2 @ q2
-            >>> mcl.smu2(s, t) == mcl.smu2(t, s)
-            True
-            """
-            return GT.__mul__(s, t)
-
-        @staticmethod
-        def sad2(s: GT, t: GT) -> GT:
-            """
-            Return the sum of two second-level scalars.
-
-            >>> s = mcl.scl2()
-            >>> t = mcl.scl2()
-            >>> mcl.sad2(s, t) == mcl.sad2(t, s)
-            True
-            """
-            return GT.__add__(s, t)
-
-    # Indicate that data structures based on the dynamic/shared library have
-    # successfully been defined.
-    mclbn256 = True
-
-except: # pylint: disable=W0702 # pragma: no cover
-    mcl = None # Exported symbol.
-
-#
-# Dedicated point and scalar data structures for each implementation.
-#
-
-for (_implementation, _p_base_cls, _s_base_cls, _p2_base_cls, _s2_base_cls) in (
-    [(python, bytes, bytes, bytes, bytes)] +
-    ([(mcl, G1, Fr, G2, GT)] if mcl is not None else [])
-):
-    # pylint: disable=cell-var-from-loop
-
-    class point(_p_base_cls): # pylint: disable=W0621,E0102
-        """
-        Wrapper class for a bytes-like object that corresponds
-        to a point.
-        """
-        _implementation = _implementation
-
-        @classmethod
-        def random(cls) -> point:
-            """
-            Return random point object.
-
-            >>> len(point.random())
-            96
-            """
-            p = cls._implementation.pnt()
-            p.__class__ = cls
-            return p
-
-        @classmethod
-        def bytes(cls, bs: bytes) -> point:
-            """
-            Return point object obtained by transforming supplied bytes-like
-            object if it is possible to do so; otherwise, return ``None``.
-
-            The bytes-like object need not be the binary representation
-            of a point or its coordinate(s). For a strict deserialization
-            from a bytes-like object, use :obj:`point.from_bytes`.
-
-            >>> p = point.bytes(hashlib.sha512('123'.encode()).digest())
-            >>> p.hex()[:64]
-            '6d68495eb4d539db4df70fd24d54fae37c9adf7dfd8dc705ccb8de8630e7cf22'
-            """
-            p = cls._implementation.pnt(bs)
-            p.__class__ = cls
-            return p
-
-        @classmethod
-        def hash(cls, bs: bytes) -> point: # pylint: disable=arguments-differ
-            """
-            Return point object by hashing supplied bytes-like object.
-
-            >>> point.hash('123'.encode()).hex()[:64]
-            '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
-            """
-            p = cls._implementation.pnt(hashlib.sha512(bs).digest()[:32])
-            p.__class__ = cls
-            return p
-
-        @classmethod
-        def base(cls, s: scalar) -> point:
-            """
-            Return base point multiplied by supplied scalar
-            if the scalar is valid.
-
-            >>> point.base(scalar.hash('123'.encode())).canonical().hex()[:64]
-            '2d66076815cda25556bab4a930244ac284412267e9345aceb98d71530308401a'
-            """
-            p = cls._implementation.bas(s)
-            p.__class__ = cls
-            return p
-
-        @classmethod
-        def from_bytes(cls, bs: bytes) -> point:
-            """
-            Deserialize the supplied binary representation of an instance and
-            return that instance.
-
-            >>> p = point.hash('123'.encode())
-            >>> bs = p.to_bytes()
-            >>> point.from_bytes(bs) == p
-            True
-            >>> type(bs) is bytes
-            True
-            """
-            p = cls._implementation.des(bs)
-            p.__class__ = cls
-            return p
-
-        @classmethod
-        def fromhex(cls, s: str) -> point:
-            """
-            Construct an instance from its hexadecimal UTF-8 string representation.
-
-            >>> point.fromhex(
-            ...     'b89ec91191915a72d4ec4434be7b438893975880b21720995c2b2458962c4e0a'
-            ...     'd0efebb5c303e4d1f8461b44ec768c587eca8b0abc01d4cb0d878b076154940d'
-            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-            ... ).canonical().hex()[:64]
-            'b89ec91191915a72d4ec4434be7b438893975880b21720995c2b2458962c4e0a'
-            """
-            return cls.from_bytes(bytes.fromhex(s))
-
-        @classmethod
-        def from_base64(cls, s: str) -> point:
-            """
-            Construct an instance from its Base64 UTF-8 string representation.
-
-            >>> point.from_base64(
-            ...     'hQIYpQRHupyyfPFoEm8rfmKV6i6VUP7vmngQWpxS3AEJD29fKVMW39l2oDLB+Ece'
-            ...     '5PqBuRzCyiRb8xYIelEII47///////8Viv//////ObnN/////y7GovX//3/ypCsh'
-            ... ).canonical().hex()[:64]
-            '850218a50447ba9cb27cf168126f2b7e6295ea2e9550feef9a78105a9c52dc01'
-            """
-            return cls.from_bytes(base64.standard_b64decode(s))
-
-        def __new__( # pylint: disable=arguments-differ
-                cls,
-                bs: Union[bytes, bytearray, None] = None
-            ) -> point:
-            """
-            If a bytes-like object is supplied, return a point object
-            corresponding to the supplied bytes-like object (no checking
-            is performed to confirm that the bytes-like object is a valid
-            point). If no argument is supplied, return a random point
-            object.
-
-            >>> bs = bytes.fromhex(
-            ...     'a5db59a0a1450aee0e47e7226d992fded25f2eb5378493ba0eb3225fc7595809'
-            ...     'c76c3dc4ba5a827be515cef65823ab1b113626348415f85aa966bad842457c03'
-            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-            ... )
-            >>> point(bs).canonical().hex()[:64]
-            'a5db59a0a1450aee0e47e7226d992fded25f2eb5378493ba0eb3225fc7595809'
-            >>> len(point())
-            96
-            """
-            return cls.from_bytes(bs) if bs is not None else cls.random()
-
-        def canonical(self: point) -> point:
-            """
-            Normalize the representation of this point into its canonical form
-            and return the result. This takes the *z*-coordinate, which may not
-            always be equal to 1, and multiplies all coordinates *x*, *y*,
-            and *z* by *z*'s multiplicative inverse. The resulting canonical
-            representation is unique (*i.e.*, two points are equal if and only
-            if their canonical forms are equal) and in the form
-            (*x*/*z*, *y*/*z*, 1).
-
-            >>> a = point.hash('123'.encode())
-            >>> p = a + a + a + a
-            >>> p == p
-            True
-            >>> p.to_bytes() == p.to_bytes()
-            True
-            >>> p.to_bytes() == p.canonical().to_bytes() and p.__class__ != python.point
-            False
-            >>> p.canonical().to_bytes() == p.canonical().to_bytes()
-            True
-            >>> p.canonical().to_bytes() == p.canonical().canonical().to_bytes()
-            True
-            >>> point.from_bytes(p.to_bytes()) == p
-            True
-            >>> point.from_bytes(p.canonical().to_bytes()) == p
-            True
-            >>> point.from_bytes(p.to_bytes()) == point.from_bytes(p.canonical().to_bytes())
-            True
-            >>> type(p.canonical()) is point
-            True
-            """
-            p = self._implementation.can(self)
-            p.__class__ = self.__class__
-            return p
-
-        def __mul__(self: point, other: Any) -> NoReturn:
-            """
-            Use of this method is not permitted. A point cannot be a left-hand argument.
-
-            >>> point() * scalar()
-            Traceback (most recent call last):
-              ...
-            TypeError: point must be on right-hand side of multiplication operator
-            """
-            raise TypeError(
-                'point must be on right-hand side of multiplication operator'
-            )
-
-        def __rmul__(self: point, other: Any) -> NoReturn:
-            """
-            This functionality is implemented exclusively in the method
-            :obj:`scalar.__mul__`, as that method pre-empts this method
-            when the second argument has the correct type (*i.e.*, it is
-            a :obj:`scalar` instance). This method is included so that an
-            exception can be raised if an incorrect argument is supplied.
-
-            >>> p = point.hash('123'.encode())
-            >>> 2 * p
-            Traceback (most recent call last):
-              ...
-            TypeError: point can only be multiplied by a scalar
-            """
-            raise TypeError('point can only be multiplied by a scalar')
-
-        def __add__(self: point, other: point) -> point:
-            """
-            Return sum of this point and another point.
-
-            >>> p = point.hash('123'.encode())
-            >>> q = point.hash('456'.encode())
-            >>> (p + q).canonical().hex()[:64]
-            '1ea48cab238fece46bd0c9fb562c859e318e17a8fb75517a4750d30ca79b911c'
-            """
-            p = self._implementation.add(self, other)
-            p.__class__ = self.__class__
-            return p
-
-        def __sub__(self: point, other: point) -> point:
-            """
-            Return the result of subtracting another point from this point.
-
-            >>> p = point.hash('123'.encode())
-            >>> q = point.hash('456'.encode())
-            >>> (p - q).canonical().hex()[:64]
-            'a43a5ce1931b1300b62e5d7e1b0c691203bfd85fafd9585dc5e47a7e2acfea22'
-            """
-            p = self._implementation.sub(self, other)
-            p.__class__ = self.__class__
-            return p
-
-        def __neg__(self: point) -> point:
-            """
-            Return the negation (additive inverse) of this point
-
-            >>> p = point.hash('123'.encode())
-            >>> q = point.hash('456'.encode())
-            >>> (p + q).canonical().hex()[:64]
-            '1ea48cab238fece46bd0c9fb562c859e318e17a8fb75517a4750d30ca79b911c'
-            """
-            p = self._implementation.neg(self)
-            p.__class__ = self.__class__
-            return p
-
-        def __matmul__(self: point, other: point2) -> scalar2:
-            """
-            Return the result of pairing another second-level point with this
-            instance.
-
-            **This method is only defined for the classes**
-            :obj:`oblivious.bn254.mcl.point` **and** :obj:`oblivious.bn254.mcl.point2`
-            **that are available when the**
-            `mclbn256 <https://pypi.org/project/mclbn256>`__ **package is installed**.
-            Otherwise, :obj:`oblivious.bn254.point` and :obj:`oblivious.bn254.point2`
-            correspond to the pure-Python implementations of these classes (for which
-            this method is not defined).
-
-            >>> p = point.hash('123'.encode())
-            >>> q = point2.base(scalar.from_int(456))
-            >>> z = (p @ q).hex()[700:]
-            >>> z == 'd01f7e038b05acc5519eeda026c4aa111eb12f3483f274c60e34e6ec7571435df707'
-            True
-
-            The pairing function is bilinear.
-
-            >>> p = point.random()
-            >>> q = point2.random()
-            >>> s = scalar.random()
-            >>> t = scalar.random()
-            >>> -((~s) * (s * p)) - p == scalar.from_int(-2) * p
-            True
-            >>> (s * (t * p)) @ q == (s * p) @ (t * q)
-            True
-
-            Suppose there are two points: one multiplied by the scalar ``s`` and the other
-            multiplied by the scalar ``t``. Their equality can be determined by using a
-            balancing point: ``g**(~s * t)``.  If the pairing of ``t * x`` with ``g`` is the
-            same as the pairing with ``s * y`` and ``g**(~s * t)``, then ``x`` equals ``y``.
-
-            >>> x = y = p
-            >>> g = point2.base(scalar.from_int(1))
-            >>> b = point2.base(~s * t)
-            >>> (t * x) @ g == (s * y) @ b
-            True
-            """
-            s = self._implementation.par(self, other)
-            s.__class__ = self._implementation.scalar2
-            return s
-
-        def __len__(self: point) -> int:
-            """
-            Return length (in bytes) of the binary representation of this instance.
-
-            >>> len(point())
-            96
-            """
-            return bytes(self).__len__()
-
-        def __bytes__(self: point) -> bytes:
-            """
-            Serialize this instance and return its binary representation.
-
-            >>> p = point.hash('123'.encode())
-            >>> bs = bytes(p)
-            >>> point.from_bytes(bs) == p
-            True
-            >>> type(bs) is bytes
-            True
-            >>> len(bs)
-            96
-            """
-            return self._implementation.ser(self)
-
-        def to_bytes(self: point) -> bytes:
-            """
-            Serialize this instance and return its binary representation.
-
-            >>> p = point.hash('123'.encode())
-            >>> bs = p.to_bytes()
-            >>> point.from_bytes(bs) == p
-            True
-            >>> type(bs) is bytes
-            True
-            >>> len(bs)
-            96
-            """
-            return bytes(self)
-
-        def hex(self: point) -> str:
-            """
-            Return a hexadecimal representation of this instance.
-
-            >>> p = point.hash('123'.encode())
-            >>> p.hex()[:64]
-            '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
-            """
-            return bytes(self).hex()
-
-        def to_base64(self: point) -> str:
-            """
-            Return the Base64 UTF-8 string representation of this instance.
-
-            >>> p = point.from_base64(
-            ...     'hQIYpQRHupyyfPFoEm8rfmKV6i6VUP7vmngQWpxS3AEJD29fKVMW39l2oDLB+Ece'
-            ...     '5PqBuRzCyiRb8xYIelEII47///////8Viv//////ObnN/////y7GovX//3/ypCsh'
-            ... )
-            >>> p.to_base64()[-64:]
-            '5PqBuRzCyiRb8xYIelEII47///////8Viv//////ObnN/////y7GovX//3/ypCsh'
-            """
-            return base64.standard_b64encode(bytes(self)).decode('utf-8')
-
-    class scalar(_s_base_cls): # pylint: disable=E0102
-        """
-        Class for representing a scalar.
-        """
-        _implementation = _implementation
-
-        @classmethod
-        def random(cls) -> scalar:
-            """
-            Return random non-zero scalar object.
-
-            >>> len(scalar.random())
-            32
-            """
-            s = cls._implementation.rnd()
-            s.__class__ = cls
-            return s
-
-        @classmethod
-        def bytes(cls, bs: bytes) -> Optional[scalar]:
-            """
-            Return scalar object obtained by transforming supplied bytes-like
-            object if it is possible to do so; otherwise, return ``None``.
-
-            >>> s = scalar()
-            >>> t = scalar.bytes(bytes(s))
-            >>> s.hex() == t.hex()
-            True
-            """
-            s = cls._implementation.scl(bs)
-            if s is not None:
-                s.__class__ = cls
-            return s
-
-        @classmethod
-        def hash(cls, bs: bytes) -> scalar:
-            """
-            Return scalar object by hashing supplied bytes-like object.
-
-            >>> scalar.hash('123'.encode()).hex()[:64]
-            '93d829354cb3592743174133104b5405ba6992b67bb219fbde3e394d70505913'
-            """
-            h = hashlib.sha256(bs).digest()
-            s = cls._implementation.scl(h)
-            while s is None:
-                h = hashlib.sha256(h).digest()
-                s = cls._implementation.scl(h)
-
-            s.__class__ = cls
-            return s
-
-        @classmethod
-        def from_int(cls, i: int) -> scalar:
-            """
-            Construct an instance from its corresponding integer (*i.e.*, residue)
-            representation.
-
-            The integer can be in the range from
-            ``-16798108731015832284940804142231733909759579603404752749028378864165570215948``
-            to ``16798108731015832284940804142231733909759579603404752749028378864165570215948``
-            (or a corresponding one in the range from
-            ``-8399054365507916142470402071115866954879789801702376374514189432082785107974``
-            to ``8399054365507916142470402071115866954879789801702376374514189432082785107974``).
-            Any values outside of this range will not be reduced, may be truncated, or may raise
-            a :obj:`ValueError`.  Zero-valued scalars are technically allowed, but cannot be used
-            for point-scalar multiplication.
-
-            >>> int(scalar.from_int(
-            ...    16798108731015832284940804142231733909759579603404752749028378864165570215948
-            ... ))
-            -1
-            >>> int(scalar.from_int(
-            ...    -8399054365507916142470402071115866954879789801702376374514189432082785107974
-            ... ))
-            -8399054365507916142470402071115866954879789801702376374514189432082785107974
-            >>> int(scalar.from_int(
-            ...     12345678
-            ... ))
-            12345678
-            """
-            #r= 0x2523648240000001ba344d8000000007ff9f800000000010a10000000000000d
-            d = 0x212ba4f27ffffff5a2c62effffffffd00242ffffffffff9c39ffffffffffffb2
-            return cls.bytes(int.to_bytes((i * d) % r, 32, 'little'))
-
-        @classmethod
-        def from_bytes(cls, bs: bytes) -> scalar:
-            """
-            Deserialize the supplied binary representation of an instance and
-            return that instance.
-
-            >>> s = scalar.hash('123'.encode())
-            >>> bs = s.to_bytes()
-            >>> scalar.from_bytes(bs) == s
-            True
-            >>> type(bs) is bytes
-            True
-            """
-            s = cls._implementation.sde(bs)
-            s.__class__ = cls
-            return s
-
-        @classmethod
-        def fromhex(cls, s: str) -> scalar:
-            """
-            Construct an instance from its hexadecimal UTF-8 string representation.
-
-            >>> scalar.fromhex(
-            ...     '3ab45f5b1c9339f1d25b878cce1c053b5492b4dc1affe689cbe141769f655e1e'
-            ... ).hex()[:64]
-            '3ab45f5b1c9339f1d25b878cce1c053b5492b4dc1affe689cbe141769f655e1e'
-            """
-            return cls.from_bytes(bytes.fromhex(s))
-
-        @classmethod
-        def from_base64(cls, s: str) -> scalar:
-            """
-            Construct an instance from its Base64 UTF-8 string representation.
-
-            >>> scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=').hex()[:64]
-            '312d0c9130f69153bec9f5d0386a95135eb45eebf130af5f1fed1c6ed15f2500'
-            """
-            return cls.from_bytes(base64.standard_b64decode(s))
-
-        def __new__( # pylint: disable=arguments-differ
-                cls,
-                bs: Union[bytes, bytearray, None] = None
-            ) -> scalar:
-            """
-            If a bytes-like object is supplied, return a scalar object
-            corresponding to the supplied bytes-like object (no checking
-            is performed to confirm that the bytes-like object is a valid
-            scalar). If no argument is supplied, return a random scalar
-            object.
-
-            >>> s = scalar()
-            >>> t = scalar(bytes(s))
-            >>> s.hex() == t.hex()
-            True
-            >>> len(scalar())
-            32
-            """
-            return cls.from_bytes(bs) if bs is not None else cls.random()
-
-        def __invert__(self: scalar) -> scalar:
-            """
-            Return the inverse of a scalar.
-
-            >>> s = scalar()
-            >>> p = point()
-            >>> ((~s) * (s * p)) == p
-            True
-            """
-            s = self._implementation.inv(self)
-            s.__class__ = self.__class__
-            return s
-
-        def __mul__(
-                self: scalar,
-                other: Union[scalar, point, point2]
-            ) -> Optional[Union[scalar, point, point2]]:
-            """
-            Multiply supplied scalar, point, or second-level point by this
-            instance.
-
-            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
-            >>> (s * s).hex()[:64]
-            '0497a5b6a7992e7d77b59c07d4457e8bb3cf580603cfd19e05d1f31342141b00'
-            >>> isinstance(s * s, scalar)
-            True
-            >>> p = point.from_base64(
-            ...     'hQIYpQRHupyyfPFoEm8rfmKV6i6VUP7vmngQWpxS3AEJD29fKVMW39l2oDLB+Ece'
-            ...     '5PqBuRzCyiRb8xYIelEII47///////8Viv//////ObnN/////y7GovX//3/ypCsh'
-            ... )
-            >>> (s * p).canonical().hex()[:64]
-            'eee31d1780ea41771357da19a81eaddf2e7fa560142067b433764cbf98be9002'
-            >>> isinstance(s * p, point)
-            True
-
-            If the second argument is a :obj:`point2` object, this method
-            pre-empts :obj:`point2.__rmul__`.
-
-            >>> p = point2.hash('123'.encode())
-            >>> (s * p).canonical().hex()[:128] == (
-            ...     '451f144e06deecbfe5a1527f2b5cc6f12bbde91c1fdf0d5326ad79ffc53bb106'
-            ...     '6d800275af625de83d72d815335832027cc60c34f22e8c5f89f953740a409702'
-            ... )
-            True
-
-            Any attempt to multiply a value or object of an incompatible type by this
-            instance raises an exception.
-
-            >>> s * 2
-            Traceback (most recent call last):
-              ...
-            TypeError: multiplication by a scalar is defined only for scalars and points
-            """
-            if isinstance(other, self._implementation.scalar):
-                s = self._implementation.smu(self, other)
-                s.__class__ = self.__class__
-                return s
-
-            if isinstance(other, self._implementation.point):
-                p = self._implementation.mul(self, other)
-                p.__class__ = other.__class__
-                return p
-
-            if isinstance(other, self._implementation.point2):
-                p = self._implementation.mul2(self, other)
-                p.__class__ = other.__class__
-                return p
-
-            raise TypeError(
-                'multiplication by a scalar is defined only for scalars and points'
-            )
-
-        def __rmul__(self: scalar, other: Any) -> NoReturn:
-            """
-            A scalar cannot be on the right-hand side of a non-scalar.
-
-            >>> point() * scalar()
-            Traceback (most recent call last):
-              ...
-            TypeError: point must be on right-hand side of multiplication operator
-            """
-            raise TypeError(
-                'scalar must be on left-hand side of multiplication operator'
-            )
-
-        def __add__(self: scalar, other: scalar) -> scalar:
-            """
-            Add another scalar to this instance.
-
-            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
-            >>> (s + s).hex()[:64]
-            '625a182261ec23a77c93eba171d42a27bc68bdd6e3615ebf3eda39dca2bf4a00'
-            >>> isinstance(s + s, scalar)
-            True
-
-            >>> z = scalar2.from_base64(
-            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
-            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
-            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
-            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
-            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
-            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
-            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
-            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
-            ... )
-            >>> (z + z).hex()[700:]
-            '4a1f476a7553bd83a5dd5179f98d9acddae4c505e25e95df6734c901198d83ad9019'
-            >>> isinstance(z + z, scalar2)
-            True
-            """
-            s = self._implementation.sad(self, other)
-            s.__class__ = self.__class__
-            return s
-
-        def __sub__(self: scalar, other: scalar) -> scalar:
-            """
-            Subtract this instance from another scalar.
-
-            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
-            >>> (s - s).hex() == '00' * len(s)
-            True
-            >>> isinstance(s - s, scalar)
-            True
-            """
-            s = self._implementation.ssu(self, other)
-            s.__class__ = self.__class__
-            return s
-
-        def __neg__(self: scalar) -> scalar:
-            """
-            Negate this instance.
-
-            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
-            >>> (-s).hex()
-            'dcd2f36ecf096e4d52360a2fc7150aeca94ba1148e1c855ae212e3d1b004fe24'
-            >>> isinstance(-s, scalar)
-            True
-            """
-            s = self._implementation.sne(self)
-            s.__class__ = self.__class__
-            return s
-
-        def __len__(self: scalar) -> int:
-            """
-            Return length (in bytes) of the binary representation of this instance.
-
-            >>> len(scalar())
-            32
-            """
-            return bytes(self).__len__()
-
-        def __bytes__(self: scalar) -> bytes:
-            """
-            Serialize this instance and return its binary representation.
-
-            >>> s = scalar.hash('123'.encode())
-            >>> bs = bytes(s)
-            >>> scalar.from_bytes(bs) == s
-            True
-            >>> type(bs) is bytes
-            True
-            """
-            return self._implementation.sse(self)
-
-        def to_bytes(self: scalar) -> bytes:
-            """
-            Serialize this instance and return its binary representation.
-
-            >>> s = scalar.hash('123'.encode())
-            >>> bs = s.to_bytes()
-            >>> scalar.from_bytes(bs) == s
-            True
-            >>> type(bs) is bytes
-            True
-            """
-            return bytes(self)
-
-        def __int__(self: scalar) -> bytes:
-            """
-            Compute and return the numerical representation of this instance.
-
-            >>> s = scalar.from_int(123)
-            >>> n = int(s)
-            >>> scalar.from_int(n) == s
-            True
-            >>> type(n) is int
-            True
-            """
-            d_inv = 0x235f846d22752e25720e909a9e82a1b4ad47e882341d8fca46c142d23fa9bc45
-            n = (int.from_bytes(self._implementation.sse(self), 'little') * d_inv) % r
-            return n if (n <= r//2) else n - r
-
-        def to_int(self: scalar) -> bytes:
-            """
-            Compute and return the numerical representation of this instance.
-
-            >>> s = scalar.from_int(123)
-            >>> n = s.to_int()
-            >>> scalar.from_int(n) == s
-            True
-            >>> type(n) is int
-            True
-            """
-            return int(self)
-
-        def hex(self: scalar) -> str:
-            """
-            Return a hexadecimal representation of this instance.
-
-            >>> s = scalar.hash('123'.encode())
-            >>> s.hex()
-            '93d829354cb3592743174133104b5405ba6992b67bb219fbde3e394d70505913'
-            """
-            return self.to_bytes().hex()
-
-        def to_base64(self: scalar) -> str:
-            """
-            Return the Base64 UTF-8 string representation of this instance.
-
-            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
-            >>> s.to_base64()
-            'MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA='
-            """
-            return base64.standard_b64encode(self.to_bytes()).decode('utf-8')
-
-    class point2(_p2_base_cls): # pylint: disable=W0621,E0102
-        # pylint: disable=C0301 # Accommodate large outputs in doctests.
-        """
-        Wrapper class for a bytes-like object that corresponds
-        to a point.
-        """
-        _implementation = _implementation
-
-        @classmethod
-        def random(cls) -> point2:
-            """
-            Return random instance.
-
-            >>> len(point2.random())
-            192
-            """
-            p = cls._implementation.pnt2()
-            p.__class__ = cls
-            return p
-
-        @classmethod
-        def bytes(cls, bs: Union[bytes, bytearray]) -> point2:
-            """
-            Construct an instance that corresponds to the supplied binary
-            representation.
-
-            >>> p = point2.bytes(hashlib.sha512('123'.encode()).digest())
-            >>> p.canonical().hex()[:128] == (
-            ...     '4c595542640a69c4a70bda55c27ef96c133cd1f4a5f83b3371e571960c018e19'
-            ...     'c54aaec2069f8f10a00f12bcbb3511cdb7356201f5277ec5e47da91405be2809'
-            ... )
-            True
-            """
-            p = cls._implementation.pnt2(bs)
-            p.__class__ = cls
-            return p
-
-        @classmethod
-        def hash(cls, bs: Union[bytes, bytearray]) -> point2: # pylint: disable=W0221
-            """
-            Construct an instance by hashing the supplied bytes-like object.
-
-            >>> point2.hash('123'.encode()).canonical().hex()[:128] == (
-            ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
-            ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
-            ... )
-            True
-            """
-            p = cls._implementation.pnt2(hashlib.sha512(bs).digest()[:32])
-            p.__class__ = cls
-            return p
-
-        @classmethod
-        def base(cls, s: scalar) -> point2:
-            """
-            Return base second-level point multiplied by the supplied scalar
-            if the scalar is valid; otherwise, return ``None``.
-
-            >>> point2.base(scalar.hash('123'.encode())).canonical().hex()[:128] == (
-            ...     'e7000fb12d206112c73fe1054e9d77b35c77881eba6598b7e035171d90b13e0c'
-            ...     '33c8ad2c92acb446fa958f3001b6c15aaf0f00092534a9d567541f9fadc64e09'
-            ... )
-            True
-            """
-            p = cls._implementation.bas2(s)
-            p.__class__ = cls
-            return p
-
-        @classmethod
-        def from_bytes(cls, bs: bytes) -> point2:
-            """
-            Deserialize the supplied binary representation of an instance and
-            return that instance.
-
-            >>> p = point2.hash('123'.encode())
-            >>> bs = p.to_bytes()
-            >>> point2.from_bytes(bs) == p
-            True
-            >>> type(bs) is bytes
-            True
-            """
-            p = cls._implementation.des2(bs)
-            p.__class__ = cls
-            return p
-
-        @classmethod
-        def fromhex(cls, s: str) -> point2:
-            """
-            Construct an instance from its hexadecimal UTF-8 string representation.
-
-            >>> p = point2.fromhex(
-            ...     'ab4efa2bcdeb825a67b12a10132ae1addca840ed248f83ae7dd987370dd47a05'
-            ...     '31c10b08ada0e24c0327d85b108e826a55bf3dc3286488327fac75e05e293b20'
-            ...     '01cbf919b53884d02b85aab9b0091eeda114fa65ca5d75620da26c4d164aa509'
-            ...     '2a2d55b6f311bfe52d24adf7b4b0b6ce12ed486a37c474d35a2b373be8a3f71c'
-            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-            ...     '0000000000000000000000000000000000000000000000000000000000000000'
-            ... )
-            >>> p.canonical().hex()[:64]
-            'ab4efa2bcdeb825a67b12a10132ae1addca840ed248f83ae7dd987370dd47a05'
-            """
-            p = cls.from_bytes(bytes.fromhex(s))
-            p.__class__ = cls
-            return p
-
-        @classmethod
-        def from_base64(cls, s: str) -> point2:
-            """
-            Construct an instance from its Base64 UTF-8 string representation.
-
-            >>> p = point2.from_base64(
-            ...     'xRuTJv/OWkIPMxRoCQIqNYoSixnWfMxeYwSJnjdJwxlp9E9f6oKefvbfYlJeygmK'
-            ...     'YDQniir3r/EYExFuClZ7H5X00GEqz7TcoqDl5EpwLDAvrTW3GNA2lOpHvc1F/eQc'
-            ...     'obJoTn35OzzK7qd/87Y3pOKNQaNENKO19DMzw9Lt+hiO////////FYr//////zm5'
-            ...     'zf////8uxqL1//9/8qQrIQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA'
-            ... )
-            >>> p.to_base64()[-64:]
-            'zf////8uxqL1//9/8qQrIQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA'
-            """
-            p = cls.from_bytes(base64.standard_b64decode(s))
-            p.__class__ = cls
-            return p
-
-        def __new__( # pylint: disable=arguments-differ
-                cls,
-                bs: Union[bytes, bytearray, None] = None
-            ) -> point2:
-            """
-            If a bytes-like object is supplied, return a second-level point
-            object corresponding to the supplied bytes-like object (no check
-            is performed to confirm that the bytes-like object is a valid
-            point). If no argument is supplied, a random second-level point
-            is returned.
-
-            >>> bs = bytes.fromhex(
-            ...     'ab4efa2bcdeb825a67b12a10132ae1addca840ed248f83ae7dd987370dd47a05'
-            ...     '31c10b08ada0e24c0327d85b108e826a55bf3dc3286488327fac75e05e293b20'
-            ...     '01cbf919b53884d02b85aab9b0091eeda114fa65ca5d75620da26c4d164aa509'
-            ...     '2a2d55b6f311bfe52d24adf7b4b0b6ce12ed486a37c474d35a2b373be8a3f71c'
-            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-            ...     '0000000000000000000000000000000000000000000000000000000000000000'
-            ... )
-            >>> point2.from_bytes(bs).hex() == bs.hex()
-            True
-            >>> point2.from_bytes(bs).to_bytes() == bs
-            True
-            """
-            p = cls.from_bytes(bs) if bs is not None else cls.random()
-            p.__class__ = cls # = point2
-            return p
-
-        def canonical(self: point2) -> point2:
-            """
-            Normalize the representation of this point into its canonical form
-            and return the result. This takes the *z*-coordinate, which may not
-            always be equal to 1, and multiplies all coordinates *x*, *y*, and
-            *z* by *z*'s multiplicative inverse. The resulting canonical
-            representation is unique (*i.e.*, two second-level points are equal
-            if and only if their canonical forms are equal) and in the form
-            (*x1*/*z1*, *y1*/*z1*, *x2*/*z2*, *y2*/*z2*, 1, 0).
-
-            >>> a = point2.hash('123'.encode())
-            >>> q = a + a + a + a
-            >>> q == q
-            True
-            >>> q.to_bytes() == q.to_bytes()
-            True
-            >>> q.to_bytes() == q.canonical().to_bytes() and q.__class__ != python.point2
-            False
-            >>> q.canonical().to_bytes() == q.canonical().to_bytes()
-            True
-            >>> q.canonical().to_bytes() == q.canonical().canonical().to_bytes()
-            True
-            >>> point2.from_bytes(q.to_bytes()) == q
-            True
-            >>> point2.from_bytes(q.canonical().to_bytes()) == q
-            True
-            >>> point2.from_bytes(q.to_bytes()) == point2.from_bytes(bytes(q.canonical()))
-            True
-            >>> type(q.canonical()) is point2
-            True
-            """
-            p = self._implementation.can(self)
-            p.__class__ = self.__class__
-            return p
-
-        def __mul__(self: point2, other: Any) -> NoReturn:
-            """
-            Use of this method is not permitted. A point cannot be a left-hand argument.
-
-            >>> point2() * scalar()
-            Traceback (most recent call last):
-              ...
-            TypeError: second-level point must be on right-hand side of multiplication operator
-            """
-            raise TypeError(
-                'second-level point must be on right-hand side of multiplication operator'
-            )
-
-        def __rmul__(self: point2, other: Any) -> NoReturn:
-            """
-            This functionality is implemented exclusively in the method
-            :obj:`scalar.__mul__`, as that method pre-empts this method
-            when the second argument has the correct type (*i.e.*, it is
-            a :obj:`scalar` instance). This method is included so that an
-            exception can be raised if an incorrect argument is supplied.
-
-            >>> p = point2.hash('123'.encode())
-            >>> 2 * p
-            Traceback (most recent call last):
-              ...
-            TypeError: second-level point can only be multiplied by a scalar
-            """
-            raise TypeError('second-level point can only be multiplied by a scalar')
-
-        def __add__(self: point2, other: point2) -> Optional[point2]:
-            """
-            Return sum of this instance and another second-level point.
-
-            >>> p = point2.hash('123'.encode())
-            >>> q = point2.hash('456'.encode())
-            >>> (p + q).canonical().hex()[:128] == (
-            ...     'cb0fc423c1bac2ac2df47bf5f5548a42b0d0a0da325bc77243d15dc587a7b221'
-            ...     '9808a1649991ddf770f0060333aab4d499580b123f109b5cb180f1f8a75a090e'
-            ... )
-            True
-            """
-            p = self._implementation.add2(self, other)
-            p.__class__ = self.__class__
-            return p
-
-        def __sub__(self: point2, other: point2) -> Optional[point2]:
-            """
-            Return the result of subtracting another second-level point from
-            this instance.
-
-            >>> p = point2.hash('123'.encode())
-            >>> q = point2.hash('456'.encode())
-            >>> (p - q).canonical().hex()[:128] == (
-            ...     'e97a70c4e3a5369ebbb1dcf0cc1135c8c8e04a4ec7cffdf875ac429d66846d0b'
-            ...     '191b090909c40a723027b07ac44435a6ade3813d04b3632a17c92c5c98718902'
-            ... )
-            True
-            """
-            p = self._implementation.sub2(self, other)
-            p.__class__ = self.__class__
-            return p
-
-        def __neg__(self: point2) -> point2:
-            """
-            Return the negation (additive inverse) of this instance.
-
-            >>> p = point2.hash('123'.encode())
-            >>> (-p).canonical().hex()[:128] == (
-            ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
-            ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
-            ... )
-            True
-            """
-            p = self._implementation.neg2(self)
-            p.__class__ = self.__class__
-            return p
-
-        def __matmul__(self: point2, other: point) -> scalar2:
-            """
-            Return the result of pairing another point with this instance.
-
-            Input-swapped alias of :obj:`point.__matmul__`.
-            """
-            return self._implementation.point.__matmul__(other, self)
-
-        def __len__(self: point2) -> int:
-            """
-            Return length (in bytes) of the binary representation of this instance.
-
-            >>> len(point2())
-            192
-            """
-            return bytes(self).__len__()
-
-        def __bytes__(self: point2) -> bytes:
-            """
-            Serialize this instance and return its binary representation.
-
-            >>> len(bytes(point2()))
-            192
-            """
-            return self._implementation.ser(self)
-
-        def to_bytes(self: point2) -> bytes:
-            """
-            Serialize this instance and return its binary representation.
-
-            >>> p = point2.hash('123'.encode())
-            >>> bs = p.to_bytes()
-            >>> point2.from_bytes(bs) == p
-            True
-            >>> type(bs) is bytes
-            True
-            """
-            return bytes(self)
-
-        def hex(self: point2) -> str:
-            """
-            Return a hexadecimal representation of this instance.
-
-            >>> p = point2.hash('123'.encode())
-            >>> p.canonical().hex() == (
-            ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
-            ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
-            ...     '2c6a88bb448065eb748df632b1d872e02f54b6f56fdb84a7b1cb388fe551fb08'
-            ...     '04464efa186bd4b1371e53d6f31f0e2f50ff553b6264a43331b42c976a0c541f'
-            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
-            ...     '0000000000000000000000000000000000000000000000000000000000000000'
-            ... )
-            True
-            """
-            return self.to_bytes().hex()
-
-        def to_base64(self: point2) -> str:
-            """
-            Return the Base64 UTF-8 string representation of this instance.
-
-            >>> p = point2.from_base64(
-            ...     'zn07zy59PMhe396h9AQ+FY3LqfzmaRmbVmfwKaQqTxStH2ZPqGwBjv99STlWrenq'
-            ...     'Mkfc3PCxRgM1xVaJGN+WExXhuDn4V40nkdpxtU85VFgE4aj0CMUoD99bqTEqBSYD'
-            ...     '50haF1C7mDxMRxmMXZinYDEMynRY69C1vTQ5IgcCdh+O////////FYr//////zm5'
-            ...     'zf////8uxqL1//9/8qQrIQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA'
-            ... )
-            >>> p.to_base64()[-64:]
-            'zf////8uxqL1//9/8qQrIQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA'
-            """
-            return base64.standard_b64encode(self.to_bytes()).decode('utf-8')
-
-    class scalar2(_s2_base_cls): # pylint: disable=function-redefined
-        """
-        Class for representing second-level scalars.
-        """
-        _implementation = _implementation
-
-        @classmethod
-        def random(cls) -> scalar2:
-            """
-            Return random non-zero second-level scalar.
-
-            >>> isinstance(scalar2.random(), scalar2)
-            True
-            >>> len(scalar2.random())
-            384
-            """
-            s = cls._implementation.scl2()
-            s.__class__ = cls
-            return s
-
-        @classmethod
-        def bytes(cls, bs: bytes) -> Optional[scalar2]:
-            """
-            Return second-level scalar object obtained by transforming the
-            supplied bytes-like object if it is possible to do so; otherwise,
-            return ``None``.
-
-            >>> s = scalar2()
-            >>> t = scalar2.bytes(bytes(s))
-            >>> s.hex() == t.hex()
-            True
-            """
-            s = cls._implementation.scl2(bs)
-
-            if s is not None:
-                s.__class__ = cls
-
-            return s
-
-        @classmethod
-        def hash(cls, bs: Union[bytes, bytearray]) -> scalar2:
-            """
-            Return an instance derived by hashing the supplied bytes-like object.
-
-            >>> s = python.scalar2.hash(bytes([123]))
-            >>> s.hex()[700:]
-            'e91ed56ea67d29047d588ffaf78f9ed317ff13e7f63e53276ff32988c49184e17b22'
-
-            >>> s0 = python.scalar2.hash(secrets.token_bytes(64))
-            >>> s1 = python.scalar2.hash(secrets.token_bytes(64))
-            >>> python.sse(python.smu2(python.smu2(s0, python.inv2(s0)), s1)) == python.sse(s1)
-            True
-            """
-            def pick_exponent(bs):
-                i = int.from_bytes(bs, 'little')
-
-                # Use rejection sampling to get two valid components in F_p.
-                if i >= r-1:
-                    return pick_exponent(hashlib.sha512(bs).digest()[:32])
-
-                return i+1
-
-            bs = hashlib.sha512(bs).digest()
-            exponent = pick_exponent(bs[:32])
-
-            # Generator of paired ``scalar2`` codomain, computed from pairing
-            # the base points for ``point`` and ``point2``.
-            z = cls._implementation.scalar2.from_base64('X+CkvfROeA1SsbpkudwsTzqOGQC9BkDmNcYpI0GHGg'
-            'TPr7fTv0yO88u5bybAlDc4QTCji5RvpdhGkWLT5oysD7UX5qE2ymq+HJXrl5MkiPp4J6kfZ6Obdjr9J/G4qs4U'
-            'hNgtOCecKCgdEwI4KyCbtYu5Wv2M+IgvJbWUx4ihaB1HlDwFb6rTmaa8ckaoFtY6AoM5kbbDPgNN71441LrNC5'
-            'Fp2QGPRod8+0WJ9wzl6R6cWLSV14MzoqWY6ZNDAyUPMpUaUGbIKZ3QqlpxM5EOFTTYmPQqOBY3K+tNL94yZRIM'
-            'ChE3W1ph9ypDcdFNd9xloWOw/APAa4FE538HbMZFEix4XpNKKIl3WPbGhTb/iY7DuUqKXouNdw8wSvzIVEYjBY'
-            '6IuE7e3fr7GMvd6K/8qO3Cep7EeuFzdMKxMO21PhuhBm2KLDPbzuzoNrMfmiMOhFJadkIa8F0NmWEEKEpyCIph'
-            'CwjHidMthVF/l932N4LL6EVktec8TQrotfCCEA0O')
-
-            def square_and_multiply_exp(s, exponent):
-                if exponent == 1:
-                    return s
-
-                s = s * s
-
-                if exponent % 2 == 1:
-                    s = s * z
-
-                return square_and_multiply_exp(s, exponent // 2)
-
-            return square_and_multiply_exp(z, exponent)
-
-        @classmethod
-        def from_bytes(cls, bs: bytes) -> scalar2:
-            """
-            Deserialize the supplied binary representation of an instance and
-            return that instance.
-
-            >>> s = scalar2.hash('123'.encode())
-            >>> bs = s.to_bytes()
-            >>> scalar2.from_bytes(bs) == s
-            True
-            >>> type(bs) is bytes
-            True
-            """
-            s = cls._implementation.sde2(bs)
-            s.__class__ = cls
-            return s
-
-        @classmethod
-        def fromhex(cls, s: str) -> scalar2:
-            """
-            Construct an instance from its hexadecimal UTF-8 string representation.
-
-            >>> s_hex = (
-            ...     '18d0e065798ffa4ecca0a7cc6e2b8d6d3269f7eb413525e59b731332b02ea805'
-            ...     '4b90c89ce93e4452557f53aae5f8f13221858dde2ea6a50373f1858f11287021'
-            ...     '09b3daf7a217a20a3d872632f8ced643d32649b241a67601bec855bd43f07710'
-            ...     '88df722bcacc8fd174f16ad7ef1b1d5e622d93b7cfec6385c353c13793a4e01c'
-            ...     '371ef54cd836a88e1b1f1e198d566d3bbe5aa225734305f14cac9af9c821351c'
-            ...     '86b365190105d1b7e71011d1362ed6ad9133a2c2c42898e9ebc3d1604a608f10'
-            ...     '8461d37b2463b4f88f0ccb427b5eea8714ee88f8c33daf7ee4a3f45ca8bca911'
-            ...     '87956abb4d27de1b49e5e059f904fbb475804715ab25a17306fa0e196f305215'
-            ...     '3a60dfa073ca78de49edeaac9c54cab3d0138750c23c0b68de7924a69d1ba002'
-            ...     'a24ac592622a45c59c1ded7133794292a09602bd57a36601d35438846fcb370f'
-            ...     '39c0fa7a15b34d14ab6f95ee5bf5b26bd5def1e7ed07350922d445da07d93622'
-            ...     '2db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
-            ... )
-            >>> s = scalar2.fromhex(s_hex)
-            >>> s.hex() == s_hex
-            True
-            """
-            return cls.from_bytes(bytes.fromhex(s))
-
-        @classmethod
-        def from_base64(cls, s: str) -> scalar2:
-            """
-            Construct an instance from its Base64 UTF-8 string representation.
-
-            >>> b64s = (
-            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
-            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
-            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
-            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
-            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
-            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
-            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
-            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
-            ... )
-            >>> s = scalar2.from_base64(b64s)
-            >>> s.to_base64() == b64s
-            True
-            """
-            return cls.from_bytes(base64.standard_b64decode(s))
-
-        def __new__( # pylint: disable=arguments-differ
-                cls,
-                bs: Union[bytes, bytearray, None] = None
-            ) -> scalar2:
-            """
-            If a bytes-like object is supplied, return an instance that corresponds
-            to the supplied bytes-like object (no checking is performed to confirm
-            that the bytes-like object is a valid second-level scalar). If no
-            argument is supplied, return a random scalar object.
-            """
-            return cls.from_bytes(bs) if bs is not None else cls.random()
-
-        def __invert__(self: scalar2) -> scalar2:
-            """
-            Return the inverse of this instance.
-
-            >>> s = scalar2.hash('123'.encode())
-            >>> ~(~s) == s
-            True
-            >>> ~s == s
-            False
-            >>> bytes(~s).hex()[700:] == (
-            ...     'ff13804852ea3ad35e8316d90a6d5dde854517e74cfc27ba676f429eb4fd52cd9b0c'
-            ... )
-            True
-            """
-            s = self._implementation.inv2(self)
-            s.__class__ = self.__class__
-            return s
-
-        def __mul__(self: scalar2, other: scalar2) -> scalar2:
-            """
-            Multiply this instance by another second-level scalar.
-
-            >>> s = scalar2.from_base64(
-            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
-            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
-            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
-            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
-            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
-            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
-            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
-            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
-            ... )
-            >>> bytes(s * s).hex()[700:]
-            '6f11685b89b03431dac6dc9d129c6a31cc5e3036f7f781d7460ab9f532a06845bd15'
-            >>> scalar2() * point()
-            Traceback (most recent call last):
-              ...
-            TypeError: second-level scalar can only be multiplied by another second-level scalar
-            """
-            if isinstance(other, self._implementation.scalar2):
-                s = self._implementation.smu2(self, other)
-                s.__class__ = self.__class__
-                return s
-
-            raise TypeError(
-                'second-level scalar can only be multiplied by another second-level scalar'
-            )
-
-        def __rmul__(self: scalar2, other: Any) -> NoReturn:
-            """
-            A second-level scalar cannot be on the right-hand side of a non-scalar.
-
-            >>> 2 * scalar2()
-            Traceback (most recent call last):
-              ...
-            TypeError: second-level scalar must be on left-hand side of multiplication operator
-            """
-            raise TypeError(
-                'second-level scalar must be on left-hand side of multiplication operator'
-            )
-
-        def __add__(self: scalar2, other: scalar2) -> scalar2:
-            """
-            Add another second-level scalar to this instance.
-
-            >>> z = scalar2.from_base64(
-            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
-            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
-            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
-            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
-            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
-            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
-            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
-            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
-            ... )
-            >>> (z + z).hex()[700:]
-            '4a1f476a7553bd83a5dd5179f98d9acddae4c505e25e95df6734c901198d83ad9019'
-            >>> isinstance(z + z, scalar2)
-            True
-            """
-            s = self._implementation.sad2(self, other)
-            s.__class__ = self.__class__
-            return s
-
-        def __len__(self: scalar2) -> int:
-            """
-            Return length (in bytes) of the binary representation of this instance.
-
-            >>> len(scalar2.random())
-            384
-            """
-            return bytes(self).__len__()
-
-        def __bytes__(self: scalar2) -> bytes:
-            """
-            Serialize this instance and return its binary representation.
-
-            >>> s = scalar2.hash('123'.encode())
-            >>> bs = bytes(s)
-            >>> scalar2.from_bytes(bs) == s
-            True
-            >>> type(bs) is bytes
-            True
-            >>> len(bs)
-            384
-            """
-            self.__class__ = self.__class__._implementation.scalar2
-            return self._implementation.sse(self)
-
-        def to_bytes(self: scalar2) -> bytes:
-            """
-            Serialize this instance and return its binary representation.
-
-            >>> s = scalar2.hash('123'.encode())
-            >>> bs = s.to_bytes()
-            >>> scalar2.from_bytes(bs) == s
-            True
-            >>> type(bs) is bytes
-            True
-            >>> len(bs)
-            384
-            """
-            return bytes(self)
-
-        def hex(self: scalar2) -> str:
-            """
-            Return a hexadecimal representation of this instance.
-
-            >>> s = scalar2.from_base64(
-            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
-            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
-            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
-            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
-            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
-            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
-            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
-            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
-            ... )
-            >>> s.hex() == (
-            ...     '18d0e065798ffa4ecca0a7cc6e2b8d6d3269f7eb413525e59b731332b02ea805'
-            ...     '4b90c89ce93e4452557f53aae5f8f13221858dde2ea6a50373f1858f11287021'
-            ...     '09b3daf7a217a20a3d872632f8ced643d32649b241a67601bec855bd43f07710'
-            ...     '88df722bcacc8fd174f16ad7ef1b1d5e622d93b7cfec6385c353c13793a4e01c'
-            ...     '371ef54cd836a88e1b1f1e198d566d3bbe5aa225734305f14cac9af9c821351c'
-            ...     '86b365190105d1b7e71011d1362ed6ad9133a2c2c42898e9ebc3d1604a608f10'
-            ...     '8461d37b2463b4f88f0ccb427b5eea8714ee88f8c33daf7ee4a3f45ca8bca911'
-            ...     '87956abb4d27de1b49e5e059f904fbb475804715ab25a17306fa0e196f305215'
-            ...     '3a60dfa073ca78de49edeaac9c54cab3d0138750c23c0b68de7924a69d1ba002'
-            ...     'a24ac592622a45c59c1ded7133794292a09602bd57a36601d35438846fcb370f'
-            ...     '39c0fa7a15b34d14ab6f95ee5bf5b26bd5def1e7ed07350922d445da07d93622'
-            ...     '2db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
-            ... )
-            True
-            """
-            return self.to_bytes().hex()
-
-        def to_base64(self: scalar2) -> str:
-            """
-            Return the Base64 UTF-8 string representation of this instance.
-
-            >>> b64s = (
-            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
-            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
-            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
-            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
-            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
-            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
-            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
-            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
-            ... )
-            >>> s = scalar2.from_base64(b64s)
-            >>> s.to_base64() == b64s
-            True
-            """
-            return base64.standard_b64encode(bytes(self)).decode('utf-8')
-
-    # Encapsulate classes for this implementation, regardless of which are
-    # exported as the unqualified symbols.
-    _implementation.point = point
-    _implementation.scalar = scalar
-    _implementation.point2 = point2
-    _implementation.scalar2 = scalar2
-
-# Remove method for which no pure-Python implementation exists.
-delattr(python.point, '__matmul__')
-delattr(python.point2, '__matmul__')
-
-# Redefine top-level wrapper classes to ensure that they appear at the end of
-# the auto-generated documentation.
-python = python # pylint: disable=self-assigning-variable
-mcl = mcl # pylint: disable=self-assigning-variable
-
-if __name__ == '__main__':
-    doctest.testmod() # pragma: no cover
+"""
+.. module:: bn254
+
+bn254 module
+============
+
+This module exports the classes :obj:`~oblivious.bn254.point`,
+:obj:`~oblivious.bn254.scalar`, :obj:`~oblivious.bn254.point2`,
+and :obj:`~oblivious.bn254.scalar2` for representing points and scalars. It
+also exports the two wrapper classes/namespaces :obj:`~oblivious.bn254.python`
+and :obj:`~oblivious.bn254.mcl` that encapsulate pure-Python and shared/dynamic
+library variants of the above (respectively) and also include low-level
+operations that correspond more directly to the functions found in the
+underlying libraries.
+
+* Under all conditions, the wrapper class :obj:`~oblivious.bn254.python`
+  is defined and encapsulates a pure-Python variant of class exported by this
+  module as a whole. It also includes pure-Python variants of low-level
+  operations that correspond to functions found in the underlying libraries.
+
+* If the `mclbn256 <https://pypi.org/project/mclbn256>`__ package is installed
+  (which includes a bundled copy of the `mcl <https://github.com/herumi/mcl>`__
+  dynamic/shared libray), then the wrapper class :obj:`~oblivious.bn254.mcl`
+  is defined. Otherwise, the exported variable ``mcl`` is assigned ``None``.
+
+* If the `mclbn256 <https://pypi.org/project/mclbn256>`__ package is installed,
+  all classes exported by this module correspond to the variants defined in
+  :obj:`~oblivious.bn254.mcl`. Otherwise, they correspond to the variants
+  defined in :obj:`~oblivious.bn254.python`.
+
+For most users, the classes :obj:`~oblivious.bn254.point`,
+:obj:`~oblivious.bn254.scalar`, :obj:`~oblivious.bn254.point2`,
+and :obj:`~oblivious.bn254.scalar2` should be sufficient.
+
+When using the classes within :obj:`~oblivious.bn254.python` and/or
+:obj:`~oblivious.bn254.mcl`, users should be aware that objects corresponding
+to one implementation (*e.g.*, instances of :obj:`oblivious.bn254.mcl.point`)
+are not compatible with instances corresponding to the other implementation
+(*e.g.*, the methods of the :obj:`oblivious.bn254.python.point` class). When
+using the primitive operations that correspond to a specific implementation
+(*e.g.*, :obj:`oblivious.bn254.mcl.add`), users are responsible for ensuring
+that inputs have the type and/or representation appropriate for that
+operation's internal implementation.
+"""
+from __future__ import annotations
+from typing import Any, NoReturn, Union, Optional
+import doctest
+import hashlib
+import base64
+import secrets
+from bn254.ecp import generator as get_base
+from bn254.ecp2 import generator as get_base2
+from bn254 import big as bn, Fp12 as Fp12_, Fp as _Fp, Fp2 as _Fp2
+from bn254.ecp import ECp as ECp_
+from bn254.ecp2 import ECp2 as ECp2_
+from bn254.curve import r
+
+#
+# An attempt will be made later to import mclbn256. If the mcl shared/dynamic
+# library file bundled with mclbn256 does not load, only pure-Python
+# implementations of the functions and methods will be available.
+#
+
+mclbn256 = None
+
+#
+# Use pure-Python implementations of primitives by default.
+#
+
+class _ECp(ECp_): # pylint: disable=invalid-name
+    """Internal class."""
+    # pylint: disable=missing-function-docstring
+    @classmethod
+    def random(cls) -> _ECp:
+        return cls(int(python.scalar.random()) * get_base())
+
+    @classmethod
+    def deserialize(cls, bs) -> _ECp:
+        p_mod = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
+        d_inv = 0x1a7344bac91f117ea513ec0ed5682406b6c15140174d61b28b762ae9cf6d3b46
+        decode = lambda ns: (int.from_bytes(ns, 'little') * d_inv) % p_mod
+        x, y, z = decode(bs[:32]), decode(bs[32:64]), decode(bs[-32:])
+
+        # Compute affine coordinates
+        inv_z = bn.invmodp(z, p_mod)
+        x = (x * inv_z) % p_mod
+        y = (y * inv_z) % p_mod
+
+        p = cls()
+        assert p.setxy(x, y) or (x == 0 and y == 0)
+        return p
+
+    @classmethod
+    def mapfrom(cls, bs) -> _ECp:
+        # pylint: disable=unnecessary-direct-lambda-call
+        p_mod = (
+            (lambda x: x * (x * (x * ((36 * x) - 36) + 24) - 6) + 1)
+            ((2 ** 62) + (2 ** 55) + 1)
+        )
+        while int.from_bytes(bs, 'little') >= p_mod:
+            bs = hashlib.sha256(bs).digest()
+            bs = bs[:-1] + bytes([bs[-1] & 0b00111111])
+
+        x = int.from_bytes(bs, 'little')# % p_mod
+        y = None
+        while True:
+            x3_2 = (pow(x, 3, p_mod) + 2) % p_mod
+            if pow(x3_2, (p_mod - 1) // 2, p_mod) == 1:
+                s = (p_mod-1) // 2
+                n = 2
+                while pow(n, (p_mod-1) // 2, p_mod) == -1 % p_mod:
+                    n += 1
+                y = pow(x3_2, (s + 1) // 2, p_mod)
+                b = pow(x3_2, s, p_mod)
+                g = pow(n, s, p_mod)
+                r_ = 1
+                while True:
+                    t = b
+                    m = 0
+                    for m in range(r_):
+                        if t == 1:
+                            break
+                        t = pow(t, 2, p_mod) # pragma: no cover
+                    if m == 0:
+                        break
+                    gs = pow(g, 2**(r_ - m - 1), p_mod) # pragma: no cover
+                    g = (gs * gs) % p_mod # pragma: no cover
+                    y = (y * gs) % p_mod # pragma: no cover
+                    b = (b * g) % p_mod # pragma: no cover
+                    r_ = m # pragma: no cover
+            if y is not None:
+                # pylint: disable=invalid-unary-operand-type
+                if y % 2 == 1:
+                    y = -y
+                break
+            x += 1
+
+        p = cls()
+        assert p.setxy(x, y) or (x == 0 and y == 0)
+        return p
+
+    def __new__(cls, *args, **kwargs):
+        p = ECp_.__new__(cls)
+        _ECp.__init__(p, *args, **kwargs)
+        return p
+
+    def __init__(self, p=None):
+        ECp_.__init__(self)
+        if isinstance(p, (ECp_, _ECp)):
+            self.setxy(*p.get())
+        elif isinstance(p, python.point):
+            self.setxy(*_ECp.deserialize(p).get()) # pragma: no cover
+
+    def serialize(self) -> bytes:
+        d = 0x212ba4f27ffffff5a2c62effffffffcdb939ffffffffff8a15ffffffffffff8e
+        p = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
+        x, y, z = (*self.get(), 1)
+        encode = lambda n: (n * d % p).to_bytes(32, 'little')
+        return encode(x) + encode(y) + encode(z)
+
+class _ECp2(ECp2_): # pylint: disable=invalid-name
+    """Internal class."""
+    # pylint: disable=missing-function-docstring
+    @classmethod
+    def random(cls) -> _ECp2:
+        return cls(int(python.scalar.random()) * get_base2())
+
+    @classmethod
+    def deserialize(cls, bs) -> _ECp2:
+        p_mod = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
+        d_inv = 0x1a7344bac91f117ea513ec0ed5682406b6c15140174d61b28b762ae9cf6d3b46
+        decode = lambda ns: (int.from_bytes(ns, 'little') * d_inv) % p_mod
+        x1, y1, x2, y2, z1, z2 = (decode(bs[:32]), decode(bs[32:64]), decode(bs[64:64+32]),
+                                  decode(bs[64+32:128]), decode(bs[128:128+32]), decode(bs[-32:]))
+        z2 = z2-(z2&1)+1  # 1 if z2==0 else z2
+
+        # Compute affine coordinates
+        inv_z1, inv_z2 = bn.invmodp(z1, p_mod), bn.invmodp(z2, p_mod)
+        x1, x2 = (x1 * inv_z1) % p_mod, (x2 * inv_z2) % p_mod
+        y1, y2 = (y1 * inv_z1) % p_mod, (y2 * inv_z2) % p_mod
+
+        q = cls()
+        # pylint: disable=invalid-name
+        assert q.set(_Fp2(_Fp(x1), _Fp(y1)), _Fp2(_Fp(x2), _Fp(y2))) \
+               or (x1 == 0 and y1 == 0 and x2 == 0 and y2 == 0)
+        return q
+
+    @classmethod
+    def mapfrom(cls, h) -> _ECp2:
+        return cls((int.from_bytes(h, 'little') % r) * get_base2())
+
+    def __new__(cls, *args, **kwargs):
+        q = ECp2_.__new__(cls)
+        _ECp2.__init__(q, *args, **kwargs)
+        return q
+
+    def __init__(self, q=None):
+        ECp2_.__init__(self)
+        if isinstance(q, (ECp2_, _ECp2)):
+            self.set(*q.get())
+        elif isinstance(q, python.point2):
+            self.set(*_ECp2.deserialize(bytes(q)).get()) # pragma: no cover
+
+    def serialize(self) -> bytes:
+        d = 0x212ba4f27ffffff5a2c62effffffffcdb939ffffffffff8a15ffffffffffff8e
+
+        # BN254 modulus of *F_p*.
+        p = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
+
+        p1, p2 = (*self.get(),)
+        x1, y1, z1, x2, y2, z2 = (*p1.get(), 1, *p2.get(), 0)
+
+        encode = lambda n: (n * d % p).to_bytes(32, 'little')
+        return encode(x1) + encode(y1) + encode(x2) + encode(y2) + encode(z1) + encode(z2)
+
+class _Fp12(Fp12_): # pylint: disable=invalid-name
+    """Internal class."""
+    # pylint: disable=missing-function-docstring
+    @classmethod
+    def deserialize(cls, bs) -> _Fp12:
+        p_mod = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
+        d_inv = 0x1a7344bac91f117ea513ec0ed5682406b6c15140174d61b28b762ae9cf6d3b46
+        decode = lambda ns: (int.from_bytes(ns, 'little') * d_inv) % p_mod
+        s = _Fp12()
+        s.a.a.a.x, s.a.a.b.x = decode(bs[32*0:(32*0)+32]), decode(bs[32*1:(32*1)+32])
+        s.c.a.a.x, s.c.a.b.x = decode(bs[32*2:(32*2)+32]), decode(bs[32*3:(32*3)+32])
+        s.b.b.a.x, s.b.b.b.x = decode(bs[32*4:(32*4)+32]), decode(bs[32*5:(32*5)+32])
+        s.b.a.a.x, s.b.a.b.x = decode(bs[32*6:(32*6)+32]), decode(bs[32*7:(32*7)+32])
+        s.a.b.a.x, s.a.b.b.x = decode(bs[32*8:(32*8)+32]), decode(bs[32*9:(32*9)+32])
+        s.c.b.a.x, s.c.b.b.x = decode(bs[32*10:(32*10)+32]), decode(bs[32*11:(32*11)+32])
+        return s
+
+    def __new__(cls, *args, **kwargs):
+        q = Fp12_.__new__(cls)
+        _Fp12.__init__(q, *args, **kwargs)
+        return q
+
+    def __init__(self, s=None):
+        Fp12_.__init__(self)
+        if isinstance(s, (Fp12_, _Fp12)):
+            self.set(*s.get())
+        elif isinstance(s, python.scalar2):
+            self.set(*_Fp12.deserialize(s).get()) # pragma: no cover
+
+    def serialize(self) -> bytes:
+        d = 0x212ba4f27ffffff5a2c62effffffffcdb939ffffffffff8a15ffffffffffff8e
+
+        # BN254 modulus of *F_p*.
+        p = 0x2523648240000001ba344d80000000086121000000000013a700000000000013
+
+        encode = lambda n: (n * d % p).to_bytes(32, 'little')
+        return bytes(
+            encode(self.a.a.a.int()) + encode(self.a.a.b.int()) +
+            encode(self.c.a.a.int()) + encode(self.c.a.b.int()) +
+            encode(self.b.b.a.int()) + encode(self.b.b.b.int()) +
+            encode(self.b.a.a.int()) + encode(self.b.a.b.int()) +
+            encode(self.a.b.a.int()) + encode(self.a.b.b.int()) +
+            encode(self.c.b.a.int()) + encode(self.c.b.b.int())
+        )
+
+class python:
+    """
+    Wrapper class for pure-Python implementations of primitive operations.
+
+    This class encapsulates pure-Python variants of all classes exported by
+    this module and of all the underlying low-level operations:
+    :obj:`python.pnt <pnt>`, :obj:`python.bas <bas>`,
+    :obj:`python.can <can>`, :obj:`python.ser <ser>`,
+    :obj:`python.des <des>`, :obj:`python.mul <mul>`,
+    :obj:`python.add <add>`, :obj:`python.sub <sub>`,
+    :obj:`python.neg <neg>`, :obj:`python.par <par>`,
+    :obj:`python.rnd <rnd>`, :obj:`python.scl <scl>`,
+    :obj:`python.sse <sse>`, :obj:`python.sde <sde>`,
+    :obj:`python.inv <inv>`, :obj:`python.smu <smu>`,
+    :obj:`python.sad <sad>`, :obj:`python.ssu <ssu>`,
+    :obj:`python.sne <sne>`,
+    :obj:`python.pnt2 <pnt2>`, :obj:`python.bas2 <bas2>`,
+    :obj:`python.can2 <can2>`, :obj:`python.ser2 <ser2>`,
+    :obj:`python.des2 <des2>`, :obj:`python.mul2 <mul2>`,
+    :obj:`python.add2 <add2>`, :obj:`python.sub2 <sub2>`,
+    :obj:`python.neg2 <neg2>`,
+    :obj:`python.rnd2 <rnd2>`, :obj:`python.scl2 <scl2>`,
+    :obj:`python.sse2 <sse2>`, :obj:`python.sde2 <sde2>`,
+    :obj:`python.inv2 <inv2>`, :obj:`python.smu2 <smu2>`,
+    :obj:`python.sad2 <sad2>`,
+    :obj:`python.point <oblivious.bn254.python.point>`,
+    :obj:`python.scalar <oblivious.bn254.python.scalar>`,
+    :obj:`python.point2 <oblivious.bn254.python.point2>`, and
+    :obj:`python.scalar2 <oblivious.bn254.python.scalar2>`.
+    For example, you can perform multiplication of scalars
+    using the pure-Python scalar multiplication implementation.
+
+    >>> s = python.scl()
+    >>> t = python.scl()
+    >>> python.smu(s, t) == python.smu(t, s)
+    True
+
+    Pure-Python variants of the :obj:`python.point <point>`
+    and :obj:`python.scalar <scalar>` classes always employ pure
+    Python implementations of operations when their methods are
+    invoked.
+
+    >>> p = python.scalar()
+    >>> q = python.scalar()
+    >>> p * q == q * p
+    True
+    """
+    @staticmethod
+    def pnt(h: Optional[bytes] = None) -> point:
+        """
+        Construct a point from its 64-byte vector representation (normally
+        obtained via hashing).
+
+        >>> p = python.pnt(hashlib.sha512('123'.encode()).digest())
+        >>> p.hex()[:64]
+        '6d68495eb4d539db4df70fd24d54fae37c9adf7dfd8dc705ccb8de8630e7cf22'
+        """
+        return bytes.__new__(
+            python.point,
+            (_ECp.random() if h is None else _ECp.mapfrom(h)).serialize()
+        )
+
+    @staticmethod
+    def bas(s: scalar) -> point:
+        """
+        Return the base point multiplied by the supplied scalar.
+
+        >>> bytes(python.bas(python.scalar.hash('123'.encode()))).hex()[:64]
+        '2d66076815cda25556bab4a930244ac284412267e9345aceb98d71530308401a'
+        """
+        return s * python.point.from_base64(
+            'hQAAAAAAAJGJAAAAAADnpzoAAACAHm4XDAAAwI+/9wO'
+            'O////////FYr//////zm5zf////8uxqL1//9/8qQrIY'
+            '7///////8Viv//////ObnN/////y7GovX//3/ypCsh'
+        )
+
+    @staticmethod
+    def can(p: point) -> point:
+        """
+        Normalize the representation of a point into its canonical form
+        and return the result.
+
+        >>> a = python.point.hash('123'.encode())
+        >>> p = python.add(a, a)
+        >>> p_can = python.can(python.add(a, a))
+
+        It may be the case that ``ser(p_can) != ser(p)``, depending on the
+        implementation. It is the responsibility of the user to ensure
+        that only canonical forms are serialized if those serialized forms
+        must be compared.
+
+        >>> mclbn256 = p.__class__ != python.point
+        >>> (python.ser(p_can) != python.ser(p)) or not mclbn256
+        True
+
+        Normalization is idempotent.
+
+        >>> python.can(p) == python.can(p_can)
+        True
+        """
+        return p # This instance's coordinates are already in normal affine form.
+
+    @staticmethod
+    def ser(p: point) -> bytes:
+        """
+        Return the binary representation of a point.
+
+        >>> q = python.point2.hash('123'.encode())
+        >>> python.des(python.ser(q)) == q
+        True
+        """
+        return bytes(b for b in p)
+
+    @staticmethod
+    def des(bs: bytes) -> point:
+        """
+        Construct a point corresponding to the supplied binary representation.
+
+        >>> p = python.point.hash('123'.encode())
+        >>> python.ser_p = bytes.fromhex(
+        ...     '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
+        ...     'b03c992ec97868be765b98048118a96f42bdc466a963c243c223b95196304209'
+        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+        ... )
+        >>> python.des(python.ser_p) == p
+        True
+        >>> python.ser(python.des(python.ser_p)) == python.ser_p
+        True
+        """
+        # It may be useful to debug with ``_ECp.deserialize(bs).serialize()``
+        # in place of just ``bs``.
+        return bytes.__new__(python.point, bs)
+
+    @staticmethod
+    def mul(s: scalar, p: point) -> point:
+        """
+        Multiply a point by a scalar and return the result.
+
+        >>> p = python.pnt(hashlib.sha512('123'.encode()).digest())
+        >>> s = python.scl(bytes.fromhex(
+        ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+        ... ))
+        >>> python.mul(s, p).hex()[:64]
+        '68b5dd61adaa83f1511efe7b4749481cc9f86e11bf82d82960b6c56373de0d24'
+        """
+        return bytes.__new__(python.point, _ECp(int(s) * _ECp.deserialize(p)).serialize())
+
+    @staticmethod
+    def add(p: point, q: point) -> point:
+        """
+        Return the sum of the supplied points.
+
+        >>> p = python.point.hash('123'.encode())
+        >>> q = python.point.hash('456'.encode())
+        >>> python.point.to_bytes(python.add(p, q)).hex()[:64]
+        '1ea48cab238fece46bd0c9fb562c859e318e17a8fb75517a4750d30ca79b911c'
+        >>> python.add(python.sub(p, q), q) == p
+        True
+        """
+        return bytes.__new__(
+            python.point,
+            _ECp.serialize(_ECp.deserialize(p).add(_ECp.deserialize(q)))
+        )
+
+    @staticmethod
+    def sub(p: point, q: point) -> point:
+        """
+        Return the result of subtracting the right-hand point from the
+        left-hand point.
+
+        >>> p = python.point.hash('123'.encode())
+        >>> q = python.point.hash('456'.encode())
+        >>> python.sub(p, q).hex()[:64]
+        'a43a5ce1931b1300b62e5d7e1b0c691203bfd85fafd9585dc5e47a7e2acfea22'
+        >>> python.sub(python.add(p, q), q) == p
+        True
+        """
+        return bytes.__new__(
+            python.point,
+            _ECp.serialize(_ECp.deserialize(p).add(-1 * _ECp.deserialize(q)))
+        )
+
+    @staticmethod
+    def neg(p: point) -> point:
+        """
+        Return the additive inverse of a point.
+
+        >>> p = python.point.hash('123'.encode())
+        >>> python.point.to_bytes(python.neg(p)).hex()[:64]
+        '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
+        """
+        return bytes.__new__(python.point, _ECp.serialize(-1 * _ECp.deserialize(p)))
+
+    @staticmethod
+    def rnd() -> scalar:
+        """
+        Return random non-zero scalar.
+
+        >>> isinstance(python.rnd(), python.scalar)
+        True
+        """
+        # d = 0x212ba4f27ffffff5a2c62effffffffd00242ffffffffff9c39ffffffffffffb2
+        # return int.to_bytes(((secrets.randbelow(r-1)+1) * d) % r, 32, 'little')
+
+        return python.scalar(int.to_bytes(secrets.randbelow(r-1)+1, 32, 'little'))
+
+    @classmethod
+    def scl(cls, s: Union[bytes, bytearray, None] = None) -> Optional[scalar]:
+        """
+        Construct a scalar if the supplied bytes-like object represents
+        a valid scalar; otherwise, return ``None``. If no byte vector is
+        supplied, return a random scalar.
+
+        >>> s = python.scl()
+        >>> t = python.scl(s)
+        >>> s == t
+        True
+        >>> python.scl(bytes([255] * 32)) is None
+        True
+        """
+        if s is None:
+            return python.rnd()
+
+        if int.from_bytes(s, 'little') < r:
+            return bytes.__new__(python.scalar, s)
+
+        return None
+
+    @staticmethod
+    def sse(s: scalar) -> bytes:
+        """
+        Return the binary representation of a scalar.
+
+        >>> s = python.scalar.hash('123'.encode())
+        >>> python.sde(python.sse(s)) == s
+        True
+        """
+        return bytes(b for b in s)
+
+    @staticmethod
+    def sde(bs: bytes) -> scalar:
+        """
+        Construct a scalar from its binary representation.
+
+        >>> s = python.scalar.hash('123'.encode())
+        >>> bs = bytes.fromhex(
+        ...     '93d829354cb3592743174133104b5405ba6992b67bb219fbde3e394d70505913'
+        ... )
+        >>> python.sde(bs) == s
+        True
+        >>> python.sse(python.sde(bs)) == bs
+        True
+        """
+        return bytes.__new__(python.scalar, bs)
+
+    @staticmethod
+    def inv(s: scalar) -> scalar:
+        """
+        Return the inverse of a scalar (modulo
+        ``r = 16798108731015832284940804142231733909759579603404752749028378864165570215949``
+        in the prime field `F*_r`).
+
+        >>> s = python.scl()
+        >>> p = python.pnt()
+        >>> python.mul(python.inv(s), python.mul(s, p)) == p
+        True
+        """
+        return python.scalar.from_int(bn.invmodp(int(s), r))
+
+    @staticmethod
+    def smu(s: scalar, t: scalar) -> scalar:
+        """
+        Return the product of two scalars.
+
+        >>> s = python.scl()
+        >>> t = python.scl()
+        >>> python.smu(s, t) == python.smu(t, s)
+        True
+        """
+        n = (python.scalar.__int__(s) * python.scalar.__int__(t)) % r
+        return python.scalar.from_int(n)
+
+    @staticmethod
+    def sad(s: scalar, t: scalar) -> scalar:
+        """
+        Return the sum of two scalars.
+
+        >>> s = python.scl()  # Could be `python.scl()`.
+        >>> t = python.scl()
+        >>> python.sad(s, t) == python.sad(t, s)
+        True
+        """
+        return python.scalar.from_int((int(s) + int(t)) % r)
+
+    @staticmethod
+    def ssu(s: scalar, t: scalar) -> scalar:
+        """
+        Return the result of subtracting the right-hand scalar from the
+        left-hand scalar.
+
+        >>> s = python.scl()
+        >>> t = python.scl()
+        >>> python.ssu(s, t) == python.sad(s, python.sne(t))
+        True
+        >>> python.ssu(s, t) == python.sne(python.ssu(t, s))
+        True
+        """
+        return python.scalar.from_int((int(s) - int(t)) % r)
+
+    @staticmethod
+    def sne(s: scalar) -> scalar:
+        """
+        Return the additive inverse of a scalar.
+
+        >>> s = python.scl()
+        >>> t = python.scl()
+        >>> python.sne(python.sne(s)) == s
+        True
+        """
+        return python.scalar.from_int(r - int(s))
+
+    @staticmethod
+    def pnt2(h: Optional[bytes] = None) -> point2:
+        """
+        Construct a second-level point if the supplied bytes-like object
+        represents a valid second-level point; otherwise, return ``None``.
+        If no byte vector is supplied, return a random second-level point.
+
+        >>> p = python.pnt2(hashlib.sha512('123'.encode()).digest())
+        >>> python.point2.to_bytes(p).hex()[:128] == (
+        ...     '4c595542640a69c4a70bda55c27ef96c133cd1f4a5f83b3371e571960c018e19'
+        ...     'c54aaec2069f8f10a00f12bcbb3511cdb7356201f5277ec5e47da91405be2809'
+        ... )
+        True
+        """
+        return bytes.__new__(
+            python.point2,
+            (_ECp2.random() if h is None else _ECp2.mapfrom(h)).serialize()
+        )
+
+    @staticmethod
+    def bas2(s: scalar) -> point2:
+        """
+        Return the base second-level point multiplied by the supplied scalar.
+
+        >>> bytes(python.bas2(python.scalar.hash('123'.encode()))).hex()[:64]
+        'e7000fb12d206112c73fe1054e9d77b35c77881eba6598b7e035171d90b13e0c'
+        """
+        # return s * _ECp2.__new__(python.point2, get_base2())
+        return bytes.__new__(python.point2, _ECp2(int(s) * get_base2()).serialize())
+
+    @staticmethod
+    def can2(p: point2) -> point2:
+        """
+        Normalize the representation of a second-level point into its canonical
+        form and return the result.
+
+        >>> p = python.bas2(scalar.from_int(1))
+        >>> python.ser(python.can2(p)).hex()[:64]
+        '669e6563afaa45af7cbc013d23f092bb3763d4dc41b97aef555bdf61de713f17'
+        """
+        return p # This instance's coordinates are already in normal affine form.
+
+    @staticmethod
+    def ser2(p: point2) -> bytes:
+        """
+        Return the binary representation of a second-level point.
+
+        >>> p = python.point2.hash('123'.encode())
+        >>> python.des2(python.ser2(p)) == p
+        True
+
+        It is the responsibility of the user to ensure that only canonical
+        representations of points are serialized.
+        """
+        return bytes(b for b in p)
+
+    @staticmethod
+    def des2(bs: bytes) -> point2:
+        """
+        Return the second-level point corresponding to the supplied binary
+        representation thereof.
+
+        >>> p = python.point2.hash('123'.encode())
+        >>> ser_p = bytes.fromhex(
+        ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
+        ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
+        ...     '2c6a88bb448065eb748df632b1d872e02f54b6f56fdb84a7b1cb388fe551fb08'
+        ...     '04464efa186bd4b1371e53d6f31f0e2f50ff553b6264a43331b42c976a0c541f'
+        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+        ...     '0000000000000000000000000000000000000000000000000000000000000000'
+        ... )
+        >>> python.des2(ser_p) == p
+        True
+        >>> python.ser(python.des2(ser_p)) == ser_p
+        True
+        """
+        return bytes.__new__(python.point2, bs)
+        # It may be useful to debug with _ECp2.deserialize(bs).serialize() in place of just bs.
+
+    @staticmethod
+    def mul2(s: scalar, p: point2) -> point2:
+        """
+        Multiply a second-level point by a scalar.
+
+        >>> p = python.point2.hash('123'.encode())
+        >>> s = python.scl(bytes.fromhex(
+        ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+        ... ))
+        >>> python.point2.to_bytes(python.mul2(s, p)).hex() == (
+        ...     '5f6f2ace8566ca47354fbe244ae3e6a854c37011fb6d6ac56571c94169e4ab18'
+        ...     '650bea4cfed5c9603e5949fe3d7509b17e20db4ff1f05129aad0d0a3bffb0008'
+        ...     '3043c5a14b986882836b1c929952ea3881d04ca44d487d1ab2d4c0b171b87d14'
+        ...     '5dca6dabb4f0ea7be5c95a861ed319d146b15d70542d3952af995a8bb35b8314'
+        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+        ...     '0000000000000000000000000000000000000000000000000000000000000000'
+        ... )
+        True
+        """
+        return bytes.__new__(python.point2, _ECp2(int(s) * _ECp2.deserialize(p)).serialize())
+
+    @staticmethod
+    def add2(p: point2, q: point2) -> point2:
+        """
+        Return sum of the supplied second-level points.
+
+        >>> p = python.point2.hash('123'.encode())
+        >>> q = python.point2.hash('456'.encode())
+        >>> python.point2.to_bytes(python.add2(p, q)).hex() == (
+        ...     'cb0fc423c1bac2ac2df47bf5f5548a42b0d0a0da325bc77243d15dc587a7b221'
+        ...     '9808a1649991ddf770f0060333aab4d499580b123f109b5cb180f1f8a75a090e'
+        ...     '83dd34d9ecdd6fd639230f7f0cf44b218fae4d879111de6c6c037e6ffdcdc823'
+        ...     'f5a48318143873ca90ad512a2ea1854200eea5537cd0ac93691d5b94ff36b212'
+        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+        ...     '0000000000000000000000000000000000000000000000000000000000000000'
+        ... )
+        True
+        """
+        return bytes.__new__(
+            python.point2,
+            _ECp2(_ECp2.deserialize(p).add(_ECp2.deserialize(q))).serialize()
+        )
+
+    @staticmethod
+    def sub2(p: point2, q: point2) -> point2:
+        """
+        Return the result of subtracting right-hand second-level point from the
+        left-hand second-level point.
+
+        >>> p = python.point2.hash('123'.encode())
+        >>> q = python.point2.hash('456'.encode())
+        >>> python.point2.to_bytes(python.sub2(p, q)).hex() == (
+        ...     'e97a70c4e3a5369ebbb1dcf0cc1135c8c8e04a4ec7cffdf875ac429d66846d0b'
+        ...     '191b090909c40a723027b07ac44435a6ade3813d04b3632a17c92c5c98718902'
+        ...     '407c58ed13cc0c0aaa43d0eafd44080080c8199401fe4f8ed7dd0eb5fba86817'
+        ...     '141f74341ce3c4884f86a97f51f7c0b208fe52be336b7651252fa9881c93d203'
+        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+        ...     '0000000000000000000000000000000000000000000000000000000000000000'
+        ... )
+        True
+        """
+        return bytes.__new__(
+            python.point2,
+            _ECp2(_ECp2.deserialize(p).add(-1 * _ECp2.deserialize(q))).serialize()
+        )
+
+    @staticmethod
+    def neg2(p: point2) -> point2:
+        """
+        Return the negation of a second-level point.
+
+        >>> p = python.point2.hash('123'.encode())
+        >>> python.point2.to_bytes(python.neg2(p)).hex() == (
+        ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
+        ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
+        ...     'e7957744bb7f9abb9e7209cd4e27ae80d8ab490a1072af125034c7b09c12281c'
+        ...     '0fbab105e7942bf5dbe1ac290ce01232b800aac41de98f86d04bd3a81758cf05'
+        ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+        ...     '0000000000000000000000000000000000000000000000000000000000000000'
+        ... )
+        True
+        """
+        return bytes.__new__(python.point2, _ECp2(-1 * _ECp2.deserialize(p)).serialize())
+
+    @staticmethod
+    def rnd2() -> scalar2:
+        """
+        Return random non-zero second-level scalar.
+
+        >>> isinstance(python.rnd2(), python.scalar2)
+        True
+        """
+        return python.scalar2.hash(secrets.token_bytes(384))
+
+    @staticmethod
+    def scl2(s: Union[bytes, bytearray, None] = None) -> Optional[scalar2]:
+        """
+        Construct a second-level scalar if the supplied bytes-like object
+        represents a valid second-level scalar; otherwise, return ``None``.
+        If no byte vector is supplied, return a random second-level scalar.
+
+        >>> bs = bytes.fromhex(
+        ...     '18d0e065798ffa4ecca0a7cc6e2b8d6d3269f7eb413525e59b731332b02ea805'
+        ...     '4b90c89ce93e4452557f53aae5f8f13221858dde2ea6a50373f1858f11287021'
+        ...     '09b3daf7a217a20a3d872632f8ced643d32649b241a67601bec855bd43f07710'
+        ...     '88df722bcacc8fd174f16ad7ef1b1d5e622d93b7cfec6385c353c13793a4e01c'
+        ...     '371ef54cd836a88e1b1f1e198d566d3bbe5aa225734305f14cac9af9c821351c'
+        ...     '86b365190105d1b7e71011d1362ed6ad9133a2c2c42898e9ebc3d1604a608f10'
+        ...     '8461d37b2463b4f88f0ccb427b5eea8714ee88f8c33daf7ee4a3f45ca8bca911'
+        ...     '87956abb4d27de1b49e5e059f904fbb475804715ab25a17306fa0e196f305215'
+        ...     '3a60dfa073ca78de49edeaac9c54cab3d0138750c23c0b68de7924a69d1ba002'
+        ...     'a24ac592622a45c59c1ded7133794292a09602bd57a36601d35438846fcb370f'
+        ...     '39c0fa7a15b34d14ab6f95ee5bf5b26bd5def1e7ed07350922d445da07d93622'
+        ...     '2db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
+        ... )
+        >>> python.scalar2.to_bytes(python.scl2(bs)).hex()[700:]
+        '36222db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
+        """
+        if s is None:
+            return python.rnd2()
+
+        try:
+            return python.sde2(s)
+        except ValueError: # pragma: no cover
+            return None
+
+    @staticmethod
+    def sse2(s: scalar2) -> bytes:
+        """
+        Return the binary representation of a second-level scalar.
+
+        >>> s = python.scalar2.hash('123'.encode())
+        >>> python.sde2(python.sse2(s)) == s
+        True
+        """
+        return bytes(b for b in s)
+
+    @staticmethod
+    def sde2(bs: bytes) -> scalar2:
+        """
+        Construct a second-level scalar from its binary representation.
+
+        >>> s = python.scalar2.hash('123'.encode())
+        >>> bs = bytes.fromhex(
+        ...     '36980a8359d40e106075488e80cf1479f2e6ba95d6a99a67832d21b7b94d8c1d'
+        ...     '5eb4d655f23e1d5d499d51d1c552b5e7df6943091427cd080f582e120613a021'
+        ...     '85898ef7d016e47a74a8df62316cc4ad975cb64bb63867ed9b5221f77bb9a121'
+        ...     '7bd89cd213eee0c3fdf2e0e13ef9e30383ea5607c8d13fc10e04448a6c964a00'
+        ...     '04a098a55beab09732220966319333608b2187ee2196eb5b4253bc2b1aea5303'
+        ...     '654260dd687a2eb176a494258ff7ef753f93105a6f0e9f46c926afdbe31ff124'
+        ...     '6bdd87c32537abcdb46ad542792edd74a229c9ba61abcd993f074237a91f5215'
+        ...     '8f6b07886895733edde15cb22129459162d89d3662826b74e4fcbe4e9e8c2420'
+        ...     'bd53586a09f91ff8f67f92cba72c5b64a9c3965c01e93710200ab4e084955316'
+        ...     'fb18950835b79fb4c2930efcc5fcaa9d82ee0faff036b80657daee233a445901'
+        ...     '7df3e57cb535ed26162b3ee0f8961131a93fe3198dc5393d277ed8bac5532411'
+        ...     '93b7ad15c52ca123fd26f592a2219b1bf118b3035893cc4abf614b422f978718'
+        ... )
+        >>> python.sde2(bs) == s
+        True
+        >>> python.sse(python.sde2(bs)) == bs
+        True
+        """
+        return bytes.__new__(python.scalar2, bs)
+
+    @staticmethod
+    def inv2(s: scalar2) -> scalar2:
+        """
+        Return the inverse of a second-level scalar.
+
+        >>> s = python.scl2()
+        >>> python.smu2(s, python.smu2(s, python.inv2(s))) == s
+        True
+        >>> python.smu2(python.smu2(s, s), python.inv2(s)) == s
+        True
+        """
+        return bytes.__new__(
+            python.scalar2,
+            _Fp12(_Fp12.deserialize(s).inverse()).serialize()
+        )
+
+    @staticmethod
+    def smu2(s: scalar2, t: scalar2) -> scalar2:
+        """
+        Return second-level scalar multiplied by another scalar.
+
+        >>> s = python.scalar2.random()
+        >>> t = python.scalar2.random()
+        >>> python.smu2(s, t) == python.smu2(t, s)
+        True
+        """
+        return bytes.__new__(
+            python.scalar2,
+            _Fp12(_Fp12.deserialize(s) * _Fp12.deserialize(t)).serialize()
+        )
+
+    @staticmethod
+    def sad2(s: scalar2, t: scalar2) -> scalar2:
+        """
+        Return scalar2 added to another scalar2.
+
+        >>> s = python.scl2()
+        >>> t = python.scl2()
+        >>> python.sad2(s, t) == python.sad2(t, s)
+        True
+        """
+        return bytes.__new__(
+            python.scalar2,
+            _Fp12(_Fp12.deserialize(s) + _Fp12.deserialize(t)).serialize()
+        )
+
+# Indicate that data structures based on the dynamic/shared library
+# in mclbn256 have not (yet, at least) been defined.
+mclbn256 = False
+
+#
+# Attempt to load primitives from mclbn256, if it is present;
+# otherwise, use the mclbn256 library.
+#
+
+try:
+    # Attempt to load mclbn256 with its (bundled) shared/dynamic library file.
+    from mclbn256 import Fr, G1, G2, GT # pylint: disable=import-error
+
+    # pylint: disable=C2801,W0621
+    class mcl:
+        """
+        Wrapper class for binary implementations of primitive
+        operations.
+
+        When this module is imported, it makes a number of attempts
+        to locate an instance of the shared/dynamic library file of the
+        `mclbn256 <https://doc.mclbn256.org>`__ library on the host
+        system. The sequence of attempts is listed below, in order.
+
+        1. It uses ``ctypes.util.find_library`` to look for ``'mcl'``
+           or ``'mclbn256'``.
+
+        2. It attempts to find a file ``mclbn256.so`` or ``mclbn256.dll``
+           in the paths specified by the ``PATH`` and ``LD_LIBRARY_PATH``
+           environment variables.
+
+        3. If the `mclbn256 <https://pypi.org/project/mclbn256>`__ package is
+           installed, it reverts to the compiled subset of mclbn256
+           included in that package.
+
+        If all of the above fail, then :obj:`mcl` is assigned
+        the value ``None`` and all classes exported by this module default
+        to their pure-Python variants (*i.e.*, those encapsulated within
+        :obj:`~oblivious.bn254.python`). One way to confirm that a
+        dynamic/shared library *has been found* when this module
+        is imported is to evaluate the expression ``mcl is not None``.
+
+        If a shared/dynamic library file has been loaded successfully,
+        this class encapsulates shared/dynamic library variants of all classes
+        exported by this module and of all the underlying low-level operations:
+        :obj:`mcl.pnt <pnt>`, :obj:`mcl.bas <bas>`,
+        :obj:`mcl.can <can>`, :obj:`mcl.ser <ser>`,
+        :obj:`mcl.des <des>`, :obj:`mcl.mul <mul>`,
+        :obj:`mcl.add <add>`, :obj:`mcl.sub <sub>`,
+        :obj:`mcl.neg <neg>`, :obj:`mcl.par <par>`,
+        :obj:`mcl.rnd <rnd>`, :obj:`mcl.scl <scl>`,
+        :obj:`mcl.sse <sse>`, :obj:`mcl.sde <sde>`,
+        :obj:`mcl.inv <inv>`, :obj:`mcl.smu <smu>`,
+        :obj:`mcl.sad <sad>`, :obj:`mcl.ssu <ssu>`,
+        :obj:`mcl.sne <sne>`,
+        :obj:`mcl.pnt2 <pnt2>`, :obj:`mcl.bas2 <bas2>`,
+        :obj:`mcl.can2 <can2>`, :obj:`mcl.ser2 <ser2>`,
+        :obj:`mcl.des2 <des2>`, :obj:`mcl.mul2 <mul2>`,
+        :obj:`mcl.add2 <add2>`, :obj:`mcl.sub2 <sub2>`,
+        :obj:`mcl.neg2 <neg2>`,
+        :obj:`mcl.rnd2 <rnd2>`, :obj:`mcl.scl2 <scl2>`,
+        :obj:`mcl.sse2 <sse2>`, :obj:`mcl.sde2 <sde2>`,
+        :obj:`mcl.inv2 <inv2>`, :obj:`mcl.smu2 <smu2>`,
+        :obj:`mcl.sad2 <sad2>`,
+        :obj:`mcl.point <oblivious.bn254.mcl.point>`,
+        :obj:`mcl.scalar <oblivious.bn254.mcl.scalar>`,
+        :obj:`mcl.point2 <oblivious.bn254.mcl.point2>`, and
+        :obj:`mcl.scalar2 <oblivious.bn254.mcl.scalar2>`.
+        For example, you can perform addition of points using the point
+        addition implementation found in the shared/dynamic library
+        bundled with the instance of the package
+        `mclbn256 <https://pypi.org/project/mclbn256>`__ that is found
+        on the host system.
+
+        >>> p = mcl.pnt()
+        >>> q = mcl.pnt()
+        >>> mcl.add(p, q) == mcl.add(q, p)
+        True
+
+        Methods found in the shared/dynamic library variants of the
+        :obj:`point`, :obj:`scalar`, :obj:`point2`, and :obj:`scalar2`
+        classes are wrappers for the shared/dynamic library
+        implementations of the underlying operations.
+
+        >>> p = mcl.point()
+        >>> q = mcl.point()
+        >>> p + q == q + p
+        True
+        """
+        # pylint: disable=too-many-public-methods
+
+        @staticmethod
+        def pnt(h: Union[bytes, bytearray, None] = None) -> G1:
+            """
+            Construct a point if the supplied bytes-like object represents
+            a valid point; otherwise, return ``None``. If no byte vector is
+            supplied, return a random point.
+
+            >>> p = mcl.pnt(hashlib.sha512('123'.encode()).digest())
+            >>> p.__class__ = point
+            >>> mcl.point.to_bytes(p).hex()[:64]
+            '6d68495eb4d539db4df70fd24d54fae37c9adf7dfd8dc705ccb8de8630e7cf22'
+            """
+            return G1.random() if h is None else G1.mapfrom(h)
+
+        @staticmethod
+        def bas(s: Fr) -> G1:
+            """
+            Return the base point multiplied by the supplied scalar.
+
+            >>> p = mcl.bas(mcl.scalar.hash('123'.encode())).normalize().normalize()
+            >>> p.__class__ = point
+            >>> mcl.point.to_bytes(p).hex()[:64]
+            '2d66076815cda25556bab4a930244ac284412267e9345aceb98d71530308401a'
+            """
+            return G1.base_point() * s
+
+        @staticmethod
+        def can(p: G1) -> G1:
+            """
+            Normalize the representation of a point into its canonical form and
+            return the result.
+
+            >>> a = mcl.point.hash('123'.encode())
+            >>> p = mcl.add(a, a)
+            >>> p_can = mcl.can(mcl.add(a, a))
+
+            We may have ``ser(p_can) != ser(p)`` here, depending on the backend
+            implementation.  Either normalization matters, or MCl is not the backend.
+
+            >>> (mcl.ser(p_can) != mcl.ser(p)) or not mclbn256
+            True
+
+            Normalization is idempotent.
+
+            >>> mcl.can(p) == mcl.can(p_can)
+            True
+            """
+            return p.normalize() # Sets ``(x, y, z)`` to unique vector ``(x/z, y/z, 1)``.
+
+        @staticmethod
+        def ser(p: G1) -> bytes:
+            """
+            Return the binary representation of a point.
+
+            >>> p = mcl.point.hash('123'.encode())
+            >>> mcl.des(mcl.ser(p)) == p
+            True
+            """
+            IoEcProj, IoArrayRaw = 1024, 64 # Constants from mcl library. # pylint: disable=C0103
+            return p.tostr(IoEcProj|IoArrayRaw)[1:]
+
+        @staticmethod
+        def des(bs: bytes) -> G1:
+            """
+            Construct a point corresponding to the supplied binary representation.
+
+            >>> p = mcl.point.hash('123'.encode())
+            >>> ser_p = bytes.fromhex(
+            ...     '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
+            ...     'b03c992ec97868be765b98048118a96f42bdc466a963c243c223b95196304209'
+            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+            ... )
+            >>> mcl.des(ser_p) == p
+            True
+            >>> mcl.ser(mcl.des(ser_p)) == ser_p
+            True
+            """
+            IoEcProj, IoArrayRaw = 1024, 64  # MCl constants  # pylint: disable=C0103
+            return G1.new_fromstr(b"4"+bs, IoEcProj|IoArrayRaw)
+
+        @staticmethod
+        def mul(s: Fr, p: G1) -> G1:
+            """
+            Multiply a point by a scalar and return the result.
+
+            >>> p = mcl.pnt(hashlib.sha512('123'.encode()).digest())
+            >>> s = mcl.scl(bytes.fromhex(
+            ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+            ... ))
+            >>> q = mcl.mul(s, p).normalize().normalize()
+            >>> q.__class__ = point
+            >>> mcl.point.to_bytes(q).hex()[:64]
+            '68b5dd61adaa83f1511efe7b4749481cc9f86e11bf82d82960b6c56373de0d24'
+            """
+            return G1.__mul__(p, s)
+
+        @staticmethod
+        def add(p: G1, q: G1) -> G1:
+            """
+            Return the sum of the supplied points.
+
+            >>> p = mcl.point.hash('123'.encode())
+            >>> q = mcl.point.hash('456'.encode())
+            >>> r = mcl.add(p, q).normalize().normalize()
+            >>> r.__class__ = point
+            >>> mcl.point.to_bytes(r).hex()[:64]
+            '1ea48cab238fece46bd0c9fb562c859e318e17a8fb75517a4750d30ca79b911c'
+            """
+            return G1.__add__(p, q)
+
+        @staticmethod
+        def sub(p: G1, q: G1) -> G1:
+            """
+            Return the result of subtracting the right-hand point from the
+            left-hand point.
+
+            >>> p = mcl.point.hash('123'.encode())
+            >>> q = mcl.point.hash('456'.encode())
+            >>> r = mcl.sub(p, q).normalize().normalize()
+            >>> r.__class__ = point
+            >>> mcl.point.to_bytes(r).hex()[:64]
+            'a43a5ce1931b1300b62e5d7e1b0c691203bfd85fafd9585dc5e47a7e2acfea22'
+            """
+            return G1.__sub__(p, q)
+
+        @staticmethod
+        def neg(p: G1) -> G1:
+            """
+            Return the additive inverse of a point.
+
+            >>> p = mcl.point.hash('123'.encode())
+            >>> q = mcl.neg(p)
+            >>> q.__class__ = point
+            >>> mcl.point.to_bytes(q).hex()[:64]
+            '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
+            """
+            return G1.__neg__(p)
+
+        @staticmethod
+        def par(p: Union[G1, G2], q: Union[G1, G2]) -> GT:
+            """
+            Compute the pairing function on two points.
+
+            >>> p = mcl.point.hash('123'.encode())
+            >>> q = mcl.point2.base(mcl.scalar.from_int(456))
+            >>> r = mcl.par(p, q)
+            >>> r.__class__ = mcl.scalar2
+            >>> mcl.scalar2.to_bytes(r).hex()[700:]
+            'd01f7e038b05acc5519eeda026c4aa111eb12f3483f274c60e34e6ec7571435df707'
+
+            The order of the two arguments is not important (as long as exactly
+            one argument is an instance of :obj:`point` and the other is an
+            instance of :obj:`point2`).
+
+            >>> r = mcl.par(q, p)
+            >>> r.__class__ = mcl.scalar2
+            >>> mcl.scalar2.to_bytes(r).hex()[700:]
+            'd01f7e038b05acc5519eeda026c4aa111eb12f3483f274c60e34e6ec7571435df707'
+
+            The pairing function is bilinear.
+
+            >>> p = mcl.point.random()
+            >>> s = mcl.scalar.random()
+
+            >>> t = mcl.scalar.random()
+            >>> q = mcl.point2.random()
+            >>> -((~s) * (s * p)) - p == mcl.scalar.from_int(-2) * p
+            True
+            >>> s * t * p @ q == s * p @ (t * q)
+            True
+
+            Suppose there are two points: one multiplied by the scalar ``s`` and the other
+            multiplied by the scalar ``t``. Their equality can be determined by using a
+            balancing point: ``g**(~s * t)``.  If the pairing of ``t * x`` with ``g`` is the
+            same as the pairing with ``s * y`` and ``g**(~s * t)``, then ``x`` equals ``y``.
+
+            >>> x = y = p
+            >>> g = mcl.point2.base(mcl.scalar.from_int(1))
+            >>> b = mcl.point2.base(~s * t)
+            >>> (t * x) @ g == (s * y) @ b
+            True
+
+            This operation is defined only for a point and a second-level point.
+            Any attempt to invoke the operation on values or objects of other types
+            raises an exception.
+
+            >>> p @ (p + p)
+            Traceback (most recent call last):
+              ...
+            TypeError: pairing is defined only for a point and a second-level point
+            >>> g @ b
+            Traceback (most recent call last):
+              ...
+            TypeError: pairing is defined only for a point and a second-level point
+
+            Pairing is intended to be nonsingular.
+
+            >>> p @ q.clear()
+            Traceback (most recent call last):
+              ...
+            TypeError: cannot meaningfully pair the infinity point
+            >>> p.clear() @ g
+            Traceback (most recent call last):
+              ...
+            TypeError: cannot meaningfully pair the infinity point
+            """
+            if p.zero() or q.zero():
+                raise TypeError('cannot meaningfully pair the infinity point')
+
+            if (
+                (isinstance(p, G1) and isinstance(q, G1)) or
+                (isinstance(p, G2) and isinstance(q, G2))
+            ):
+                raise TypeError(
+                    'pairing is defined only for a point and a second-level point'
+                )
+
+            if isinstance(p, G1):
+                return G1.__matmul__(G1.__new__(G1, p), G2.__new__(G2, q))
+
+            return G2.__matmul__(G2.__new__(G2, p), G1.__new__(G1, q))
+
+        @staticmethod
+        def rnd() -> Fr:
+            """
+            Return random non-zero scalar.
+
+            >>> s = mcl.rnd()
+            >>> isinstance(s, Fr)
+            True
+            >>> s.__class__ = scalar
+            >>> len(mcl.scalar.to_bytes(s))
+            32
+            """
+            return Fr().randomize()
+
+        @classmethod
+        def scl(cls, bs: Union[bytes, bytearray, None] = None) -> Optional[Fr]:
+            """
+            Construct a scalar if the supplied bytes-like object represents
+            a valid scalar; otherwise, return ``None``. If no byte vector is
+            supplied, return a random scalar.
+
+            >>> s = mcl.scl()
+            >>> s.__class__ = scalar
+            >>> t = mcl.scl(mcl.scalar.to_bytes(s))
+            >>> s == t
+            True
+            >>> mcl.scl(bytes([255] * 32)) is None
+            True
+            """
+            if bs is None:
+                return cls.rnd()
+
+            try:
+                s = cls.sde(bs)
+                return s
+            except ValueError: # pragma: no cover
+                return None
+
+        @staticmethod
+        def sse(s: Fr) -> bytes:
+            """
+            Return the binary representation of a scalar.
+
+            >>> s = mcl.scalar.hash('123'.encode())
+            >>> mcl.sde(mcl.sse(s)) == s
+            True
+            """
+            IoEcProj, IoArrayRaw = 1024, 64 # Constants from mcl library. # pylint: disable=C0103
+            return s.tostr(IoEcProj|IoArrayRaw)
+
+        @staticmethod
+        def sde(bs: bytes) -> Fr:
+            """
+            Return a scalar from its binary representation.
+
+            >>> s = mcl.scalar.hash('123'.encode())
+            >>> bs = bytes.fromhex(
+            ...     '93d829354cb3592743174133104b5405ba6992b67bb219fbde3e394d70505913'
+            ... )
+            >>> mcl.sde(bs) == s
+            True
+            >>> mcl.sse(mcl.sde(bs)) == bs
+            True
+            """
+            IoEcProj, IoArrayRaw = 1024, 64  # MCl constants  # pylint: disable=C0103
+            return Fr.new_fromstr(bs, IoEcProj|IoArrayRaw)
+
+        @staticmethod
+        def inv(s: Fr) -> Fr:
+            r"""
+            Return inverse of a scalar (modulo
+            ``r = 16798108731015832284940804142231733909759579603404752749028378864165570215949``
+            in the prime field *F*\_*r*).
+
+            >>> (s, p) = (mcl.scl(), mcl.pnt())
+            >>> mcl.mul(mcl.inv(s), mcl.mul(s, p)) == p
+            True
+            """
+            return Fr.__invert__(s)
+
+        @staticmethod
+        def smu(s: Fr, t: Fr) -> Fr:
+            """
+            Return scalar multiplied by another scalar.
+
+            >>> (s, t) = (mcl.scl(), mcl.scl())
+            >>> mcl.smu(s, t) == mcl.smu(t, s)
+            True
+            """
+            return Fr.__mul__(s, t)
+
+        @staticmethod
+        def sad(s: Fr, t: Fr) -> Fr:
+            """
+            Return scalar added to another scalar.
+
+            >>> (s, t) = (mcl.scl(), mcl.scl())
+            >>> mcl.sad(s, t) == mcl.sad(t, s)
+            True
+            """
+            return Fr.__add__(s, t)
+
+        @staticmethod
+        def ssu(s: Fr, t: Fr) -> Fr:
+            """
+            Return the result of one scalar subtracted from another scalar.
+
+            >>> (s, t) = (mcl.scl(), mcl.scl())
+            >>> mcl.ssu(s, t) == mcl.sad(s, mcl.sne(t))
+            True
+            >>> mcl.ssu(s, t) == mcl.sne(mcl.ssu(t, s))
+            True
+            """
+            return Fr.__sub__(s, t)
+
+        @staticmethod
+        def sne(s: Fr) -> Fr:
+            """
+            Return the additive inverse of a scalar.
+
+            >>> (s, t) = (mcl.scl(), mcl.scl())
+            >>> mcl.sne(mcl.sne(s)) == s
+            True
+            """
+            return Fr.__neg__(s)
+
+        @staticmethod
+        def pnt2(h: Optional[bytes] = None) -> G2:
+            """
+            Construct a second-level point if the supplied bytes-like object
+            represents a valid second-level point; otherwise, return ``None``.
+            If no byte vector is supplied, return a random second-level point.
+
+            >>> p = mcl.pnt2(hashlib.sha512('123'.encode()).digest())
+            >>> p.__class__ = point2
+            >>> mcl.point2.to_bytes(p.canonical().canonical()).hex()[:128] == (
+            ...     '4c595542640a69c4a70bda55c27ef96c133cd1f4a5f83b3371e571960c018e19'
+            ...     'c54aaec2069f8f10a00f12bcbb3511cdb7356201f5277ec5e47da91405be2809'
+            ... )
+            True
+            """
+            return G2.random() if h is None else G2.mapfrom(h)
+
+        @staticmethod
+        def bas2(s) -> G2:
+            """
+            Return the base second-level point multiplied by the supplied scalar.
+
+            >>> r = mcl.bas2(mcl.scalar.hash('123'.encode())).normalize().normalize()
+            >>> r.__class__ = point2
+            >>> mcl.point2.to_bytes(r).hex()[:64]
+            'e7000fb12d206112c73fe1054e9d77b35c77881eba6598b7e035171d90b13e0c'
+            """
+            # return s * G2.__new__(point2, G2.base_point())
+            return G2.base_point() * s
+
+        @staticmethod
+        def can2(p: G2) -> G2:
+            """
+            Normalize the representation of a second-level point into its
+            canonical form and return the result.
+
+            >>> p = mcl.bas2(scalar.from_int(1))
+            >>> mcl.ser(mcl.can2(p)).hex()[:64]
+            '669e6563afaa45af7cbc013d23f092bb3763d4dc41b97aef555bdf61de713f17'
+            """
+            return p.normalize() # Sets ``(x, y, z)`` to unique vector ``(x/z, y/z, 1)``.
+
+        @staticmethod
+        def ser2(p: G2) -> bytes:
+            """
+            Return the binary representation of a second-level point.
+
+            >>> p = mcl.point2.hash('123'.encode())
+            >>> mcl.des2(mcl.ser2(p)) == p
+            True
+
+            It is the responsibility of the user to ensure that only canonical
+            representations of points are serialized.
+            """
+            IoEcProj, IoArrayRaw = 1024, 64 # Constants from mcl library. # pylint: disable=C0103
+            return p.tostr(IoEcProj|IoArrayRaw)[1:]
+
+        @staticmethod
+        def des2(bs: bytes) -> G2:
+            """
+            Return the second-level point corresponding to the supplied binary
+            representation thereof.
+
+            >>> p = mcl.point2.hash('123'.encode())
+            >>> mcl.ser_p = bytes.fromhex(
+            ...     'b5b0a52e43ba71ae03317333da4ba9452dbdbbec353ade0c732348e0bea4ba1b'
+            ...     '8860718e5ba784d55799ab292459a638f6399738a6de348742e6a789674f300d'
+            ...     '7e59c60a595253ebf69bf0794b7a032e59b6b5037adba410d680b53ffac08517'
+            ...     'cf5bc3be9d850ec64ea6939904cf66b66b6b4b82be03ee4f10661fedaf83841f'
+            ...     'ba7e678442a658340a5b3c51eb5076d738cf88387ada6cbd1fe7f8d8a2268417'
+            ...     'bc8aedbc99808b0450025d0c75b5f1ccb34bc69934cc620d9ea51038a1d98721'
+            ... )
+            >>> mcl.des2(mcl.ser_p) == p
+            True
+            >>> mcl.ser(mcl.des2(mcl.ser_p)) == mcl.ser_p
+            True
+            """
+            IoEcProj, IoArrayRaw = 1024, 64  # MCl constants  # pylint: disable=C0103
+            return G2.new_fromstr(b"4"+bs, IoEcProj|IoArrayRaw)
+
+        @staticmethod
+        def mul2(s: Fr, p: G2) -> G2:
+            """
+            Multiply a second-level point by a scalar.
+
+            >>> p = mcl.point2.hash('123'.encode())
+            >>> s = mcl.scl(bytes.fromhex(
+            ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+            ... ))
+            >>> r = mcl.mul2(s, p).normalize().normalize()
+            >>> r.__class__ = point2
+            >>> mcl.point2.to_bytes(r).hex() == (
+            ...     '5f6f2ace8566ca47354fbe244ae3e6a854c37011fb6d6ac56571c94169e4ab18'
+            ...     '650bea4cfed5c9603e5949fe3d7509b17e20db4ff1f05129aad0d0a3bffb0008'
+            ...     '3043c5a14b986882836b1c929952ea3881d04ca44d487d1ab2d4c0b171b87d14'
+            ...     '5dca6dabb4f0ea7be5c95a861ed319d146b15d70542d3952af995a8bb35b8314'
+            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+            ...     '0000000000000000000000000000000000000000000000000000000000000000'
+            ... )
+            True
+            """
+            return G2.__mul__(p, s)
+
+        @staticmethod
+        def add2(p: G2, q: G2) -> G2:
+            """
+            Return sum of the supplied second-level points.
+
+            >>> p = mcl.point2.hash('123'.encode())
+            >>> q = mcl.point2.hash('456'.encode())
+            >>> r = mcl.add2(p, q).normalize().normalize()
+            >>> r.__class__ = point2
+            >>> mcl.point2.to_bytes(r).hex() == (
+            ...     'cb0fc423c1bac2ac2df47bf5f5548a42b0d0a0da325bc77243d15dc587a7b221'
+            ...     '9808a1649991ddf770f0060333aab4d499580b123f109b5cb180f1f8a75a090e'
+            ...     '83dd34d9ecdd6fd639230f7f0cf44b218fae4d879111de6c6c037e6ffdcdc823'
+            ...     'f5a48318143873ca90ad512a2ea1854200eea5537cd0ac93691d5b94ff36b212'
+            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+            ...     '0000000000000000000000000000000000000000000000000000000000000000'
+            ... )
+            True
+            """
+            return G2.__add__(p, q)
+
+        @staticmethod
+        def sub2(p: G2, q: G2) -> G2:
+            """
+            Return the result of subtracting the right-hand second-level point
+            from the left-hand second-level point.
+
+            >>> p = mcl.point2.hash('123'.encode())
+            >>> q = mcl.point2.hash('456'.encode())
+            >>> r = mcl.sub2(p, q).normalize().normalize()
+            >>> r.__class__ = point2
+            >>> mcl.point2.to_bytes(r).hex() == (
+            ...     'e97a70c4e3a5369ebbb1dcf0cc1135c8c8e04a4ec7cffdf875ac429d66846d0b'
+            ...     '191b090909c40a723027b07ac44435a6ade3813d04b3632a17c92c5c98718902'
+            ...     '407c58ed13cc0c0aaa43d0eafd44080080c8199401fe4f8ed7dd0eb5fba86817'
+            ...     '141f74341ce3c4884f86a97f51f7c0b208fe52be336b7651252fa9881c93d203'
+            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+            ...     '0000000000000000000000000000000000000000000000000000000000000000'
+            ... )
+            True
+            """
+            return G2.__sub__(p, q)
+
+        @staticmethod
+        def neg2(p: G2) -> G2:
+            """
+            Return the negation of a second-level point.
+
+            >>> p = mcl.point2.hash('123'.encode())
+            >>> r = mcl.neg2(p).normalize().normalize()
+            >>> r.__class__ = point2
+            >>> mcl.point2.to_bytes(r).hex() == (
+            ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
+            ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
+            ...     'e7957744bb7f9abb9e7209cd4e27ae80d8ab490a1072af125034c7b09c12281c'
+            ...     '0fbab105e7942bf5dbe1ac290ce01232b800aac41de98f86d04bd3a81758cf05'
+            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+            ...     '0000000000000000000000000000000000000000000000000000000000000000'
+            ... )
+            True
+            """
+            return G2.__neg__(p)
+
+        @staticmethod
+        def rnd2() -> GT:
+            """
+            Return random non-zero second-level scalar.
+
+            >>> isinstance(mcl.rnd2(), GT)
+            True
+            """
+            return mcl.scalar2.hash(secrets.token_bytes(384))
+
+        @staticmethod
+        def scl2(s: Union[bytes, bytearray, None] = None) -> Optional[GT]:
+            """
+            Construct a second-level scalar if the supplied bytes-like object
+            represents a valid second-level scalar; otherwise, return ``None``.
+            If no byte vector is supplied, return a random second-level scalar.
+
+            >>> bs = bytes.fromhex(
+            ...     '18d0e065798ffa4ecca0a7cc6e2b8d6d3269f7eb413525e59b731332b02ea805'
+            ...     '4b90c89ce93e4452557f53aae5f8f13221858dde2ea6a50373f1858f11287021'
+            ...     '09b3daf7a217a20a3d872632f8ced643d32649b241a67601bec855bd43f07710'
+            ...     '88df722bcacc8fd174f16ad7ef1b1d5e622d93b7cfec6385c353c13793a4e01c'
+            ...     '371ef54cd836a88e1b1f1e198d566d3bbe5aa225734305f14cac9af9c821351c'
+            ...     '86b365190105d1b7e71011d1362ed6ad9133a2c2c42898e9ebc3d1604a608f10'
+            ...     '8461d37b2463b4f88f0ccb427b5eea8714ee88f8c33daf7ee4a3f45ca8bca911'
+            ...     '87956abb4d27de1b49e5e059f904fbb475804715ab25a17306fa0e196f305215'
+            ...     '3a60dfa073ca78de49edeaac9c54cab3d0138750c23c0b68de7924a69d1ba002'
+            ...     'a24ac592622a45c59c1ded7133794292a09602bd57a36601d35438846fcb370f'
+            ...     '39c0fa7a15b34d14ab6f95ee5bf5b26bd5def1e7ed07350922d445da07d93622'
+            ...     '2db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
+            ... )
+            >>> s = mcl.scl2(bs)
+            >>> s.__class__ = mcl.scalar2
+            >>> mcl.scalar2.to_bytes(s).hex()[700:]
+            '36222db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
+            """
+            if s is None:
+                return mcl.rnd2()
+
+            try:
+                return mcl.sde2(s)
+            except ValueError: # pragma: no cover
+                return None
+
+        @staticmethod
+        def sse2(s: scalar2) -> bytes:
+            """
+            Return the binary representation of a second-level scalar.
+
+            >>> s = scalar2.hash('123'.encode())
+            >>> mcl.sde2(mcl.sse2(s)) == s
+            True
+            """
+            IoEcProj, IoArrayRaw = 1024, 64 # Constants from mcl library. # pylint: disable=C0103
+            return s.tostr(IoEcProj|IoArrayRaw)
+
+        @staticmethod
+        def sde2(bs: bytes) -> GT:
+            """
+            Return the second-level scalar corresponding to the supplied binary
+            representation thereof.
+
+            >>> s = mcl.scalar2.hash('123'.encode())
+            >>> bs = bytes.fromhex(
+            ...     '36980a8359d40e106075488e80cf1479f2e6ba95d6a99a67832d21b7b94d8c1d'
+            ...     '5eb4d655f23e1d5d499d51d1c552b5e7df6943091427cd080f582e120613a021'
+            ...     '85898ef7d016e47a74a8df62316cc4ad975cb64bb63867ed9b5221f77bb9a121'
+            ...     '7bd89cd213eee0c3fdf2e0e13ef9e30383ea5607c8d13fc10e04448a6c964a00'
+            ...     '04a098a55beab09732220966319333608b2187ee2196eb5b4253bc2b1aea5303'
+            ...     '654260dd687a2eb176a494258ff7ef753f93105a6f0e9f46c926afdbe31ff124'
+            ...     '6bdd87c32537abcdb46ad542792edd74a229c9ba61abcd993f074237a91f5215'
+            ...     '8f6b07886895733edde15cb22129459162d89d3662826b74e4fcbe4e9e8c2420'
+            ...     'bd53586a09f91ff8f67f92cba72c5b64a9c3965c01e93710200ab4e084955316'
+            ...     'fb18950835b79fb4c2930efcc5fcaa9d82ee0faff036b80657daee233a445901'
+            ...     '7df3e57cb535ed26162b3ee0f8961131a93fe3198dc5393d277ed8bac5532411'
+            ...     '93b7ad15c52ca123fd26f592a2219b1bf118b3035893cc4abf614b422f978718'
+            ... )
+            >>> mcl.sde2(bs) == s
+            True
+            >>> mcl.sse(mcl.sde2(bs)) == bs
+            True
+            """
+            IoEcProj, IoArrayRaw = 1024, 64  # MCl constants  # pylint: disable=C0103
+            return GT.new_fromstr(bs, IoEcProj|IoArrayRaw)
+
+        @staticmethod
+        def inv2(s: GT) -> GT:
+            """
+            Return the inverse of a second-level scalar.
+
+            >>> s = mcl.scl2()
+            >>> mcl.smu2(s, mcl.smu2(s, mcl.inv2(s))) == s
+            True
+            >>> mcl.smu2(mcl.smu2(s, s), mcl.inv2(s)) == s
+            True
+            """
+            return GT.__inv__(s)
+
+        @staticmethod
+        def smu2(s: GT, t: GT) -> GT:
+            """
+            Return the product of two second-level scalars.
+
+            >>> p1 = mcl.point.hash('123'.encode())
+            >>> p2 = mcl.point.hash('456'.encode())
+            >>> q1 = mcl.point2.base(mcl.scalar.hash('123'.encode()))
+            >>> q2 = mcl.point2.base(mcl.scalar.hash('456'.encode()))
+            >>> s = p1 @ q1
+            >>> t = p2 @ q2
+            >>> mcl.smu2(s, t) == mcl.smu2(t, s)
+            True
+            """
+            return GT.__mul__(s, t)
+
+        @staticmethod
+        def sad2(s: GT, t: GT) -> GT:
+            """
+            Return the sum of two second-level scalars.
+
+            >>> s = mcl.scl2()
+            >>> t = mcl.scl2()
+            >>> mcl.sad2(s, t) == mcl.sad2(t, s)
+            True
+            """
+            return GT.__add__(s, t)
+
+    # Indicate that data structures based on the dynamic/shared library have
+    # successfully been defined.
+    mclbn256 = True
+
+except: # pylint: disable=W0702 # pragma: no cover
+    mcl = None # Exported symbol.
+
+#
+# Dedicated point and scalar data structures for each implementation.
+#
+
+for (_implementation, _p_base_cls, _s_base_cls, _p2_base_cls, _s2_base_cls) in (
+    [(python, bytes, bytes, bytes, bytes)] +
+    ([(mcl, G1, Fr, G2, GT)] if mcl is not None else [])
+):
+    # pylint: disable=cell-var-from-loop
+
+    class point(_p_base_cls): # pylint: disable=W0621,E0102
+        """
+        Wrapper class for a bytes-like object that corresponds
+        to a point.
+        """
+        _implementation = _implementation
+
+        @classmethod
+        def random(cls) -> point:
+            """
+            Return random point object.
+
+            >>> len(point.random())
+            96
+            """
+            p = cls._implementation.pnt()
+            p.__class__ = cls
+            return p
+
+        @classmethod
+        def bytes(cls, bs: bytes) -> point:
+            """
+            Return point object obtained by transforming supplied bytes-like
+            object if it is possible to do so; otherwise, return ``None``.
+
+            The bytes-like object need not be the binary representation
+            of a point or its coordinate(s). For a strict deserialization
+            from a bytes-like object, use :obj:`point.from_bytes`.
+
+            >>> p = point.bytes(hashlib.sha512('123'.encode()).digest())
+            >>> p.hex()[:64]
+            '6d68495eb4d539db4df70fd24d54fae37c9adf7dfd8dc705ccb8de8630e7cf22'
+            """
+            p = cls._implementation.pnt(bs)
+            p.__class__ = cls
+            return p
+
+        @classmethod
+        def hash(cls, bs: bytes) -> point: # pylint: disable=arguments-differ
+            """
+            Return point object by hashing supplied bytes-like object.
+
+            >>> point.hash('123'.encode()).hex()[:64]
+            '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
+            """
+            p = cls._implementation.pnt(hashlib.sha512(bs).digest()[:32])
+            p.__class__ = cls
+            return p
+
+        @classmethod
+        def base(cls, s: scalar) -> point:
+            """
+            Return base point multiplied by supplied scalar
+            if the scalar is valid.
+
+            >>> point.base(scalar.hash('123'.encode())).canonical().hex()[:64]
+            '2d66076815cda25556bab4a930244ac284412267e9345aceb98d71530308401a'
+            """
+            p = cls._implementation.bas(s)
+            p.__class__ = cls
+            return p
+
+        @classmethod
+        def from_bytes(cls, bs: bytes) -> point:
+            """
+            Deserialize the supplied binary representation of an instance and
+            return that instance.
+
+            >>> p = point.hash('123'.encode())
+            >>> bs = p.to_bytes()
+            >>> point.from_bytes(bs) == p
+            True
+            >>> type(bs) is bytes
+            True
+            """
+            p = cls._implementation.des(bs)
+            p.__class__ = cls
+            return p
+
+        @classmethod
+        def fromhex(cls, s: str) -> point:
+            """
+            Construct an instance from its hexadecimal UTF-8 string representation.
+
+            >>> point.fromhex(
+            ...     'b89ec91191915a72d4ec4434be7b438893975880b21720995c2b2458962c4e0a'
+            ...     'd0efebb5c303e4d1f8461b44ec768c587eca8b0abc01d4cb0d878b076154940d'
+            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+            ... ).canonical().hex()[:64]
+            'b89ec91191915a72d4ec4434be7b438893975880b21720995c2b2458962c4e0a'
+            """
+            return cls.from_bytes(bytes.fromhex(s))
+
+        @classmethod
+        def from_base64(cls, s: str) -> point:
+            """
+            Construct an instance from its Base64 UTF-8 string representation.
+
+            >>> point.from_base64(
+            ...     'hQIYpQRHupyyfPFoEm8rfmKV6i6VUP7vmngQWpxS3AEJD29fKVMW39l2oDLB+Ece'
+            ...     '5PqBuRzCyiRb8xYIelEII47///////8Viv//////ObnN/////y7GovX//3/ypCsh'
+            ... ).canonical().hex()[:64]
+            '850218a50447ba9cb27cf168126f2b7e6295ea2e9550feef9a78105a9c52dc01'
+            """
+            return cls.from_bytes(base64.standard_b64decode(s))
+
+        def __new__( # pylint: disable=arguments-differ
+                cls,
+                bs: Union[bytes, bytearray, None] = None
+            ) -> point:
+            """
+            If a bytes-like object is supplied, return a point object
+            corresponding to the supplied bytes-like object (no checking
+            is performed to confirm that the bytes-like object is a valid
+            point). If no argument is supplied, return a random point
+            object.
+
+            >>> bs = bytes.fromhex(
+            ...     'a5db59a0a1450aee0e47e7226d992fded25f2eb5378493ba0eb3225fc7595809'
+            ...     'c76c3dc4ba5a827be515cef65823ab1b113626348415f85aa966bad842457c03'
+            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+            ... )
+            >>> point(bs).canonical().hex()[:64]
+            'a5db59a0a1450aee0e47e7226d992fded25f2eb5378493ba0eb3225fc7595809'
+            >>> len(point())
+            96
+            """
+            return cls.from_bytes(bs) if bs is not None else cls.random()
+
+        def canonical(self: point) -> point:
+            """
+            Normalize the representation of this point into its canonical form
+            and return the result. This takes the *z*-coordinate, which may not
+            always be equal to 1, and multiplies all coordinates *x*, *y*,
+            and *z* by *z*'s multiplicative inverse. The resulting canonical
+            representation is unique (*i.e.*, two points are equal if and only
+            if their canonical forms are equal) and in the form
+            (*x*/*z*, *y*/*z*, 1).
+
+            >>> a = point.hash('123'.encode())
+            >>> p = a + a + a + a
+            >>> p == p
+            True
+            >>> p.to_bytes() == p.to_bytes()
+            True
+            >>> p.to_bytes() == p.canonical().to_bytes() and p.__class__ != python.point
+            False
+            >>> p.canonical().to_bytes() == p.canonical().to_bytes()
+            True
+            >>> p.canonical().to_bytes() == p.canonical().canonical().to_bytes()
+            True
+            >>> point.from_bytes(p.to_bytes()) == p
+            True
+            >>> point.from_bytes(p.canonical().to_bytes()) == p
+            True
+            >>> point.from_bytes(p.to_bytes()) == point.from_bytes(p.canonical().to_bytes())
+            True
+            >>> type(p.canonical()) is point
+            True
+            """
+            p = self._implementation.can(self)
+            p.__class__ = self.__class__
+            return p
+
+        def __mul__(self: point, other: Any) -> NoReturn:
+            """
+            Use of this method is not permitted. A point cannot be a left-hand argument.
+
+            >>> point() * scalar()
+            Traceback (most recent call last):
+              ...
+            TypeError: point must be on right-hand side of multiplication operator
+            """
+            raise TypeError(
+                'point must be on right-hand side of multiplication operator'
+            )
+
+        def __rmul__(self: point, other: Any) -> NoReturn:
+            """
+            This functionality is implemented exclusively in the method
+            :obj:`scalar.__mul__`, as that method pre-empts this method
+            when the second argument has the correct type (*i.e.*, it is
+            a :obj:`scalar` instance). This method is included so that an
+            exception can be raised if an incorrect argument is supplied.
+
+            >>> p = point.hash('123'.encode())
+            >>> 2 * p
+            Traceback (most recent call last):
+              ...
+            TypeError: point can only be multiplied by a scalar
+            """
+            raise TypeError('point can only be multiplied by a scalar')
+
+        def __add__(self: point, other: point) -> point:
+            """
+            Return sum of this point and another point.
+
+            >>> p = point.hash('123'.encode())
+            >>> q = point.hash('456'.encode())
+            >>> (p + q).canonical().hex()[:64]
+            '1ea48cab238fece46bd0c9fb562c859e318e17a8fb75517a4750d30ca79b911c'
+            """
+            p = self._implementation.add(self, other)
+            p.__class__ = self.__class__
+            return p
+
+        def __sub__(self: point, other: point) -> point:
+            """
+            Return the result of subtracting another point from this point.
+
+            >>> p = point.hash('123'.encode())
+            >>> q = point.hash('456'.encode())
+            >>> (p - q).canonical().hex()[:64]
+            'a43a5ce1931b1300b62e5d7e1b0c691203bfd85fafd9585dc5e47a7e2acfea22'
+            """
+            p = self._implementation.sub(self, other)
+            p.__class__ = self.__class__
+            return p
+
+        def __neg__(self: point) -> point:
+            """
+            Return the negation (additive inverse) of this point
+
+            >>> p = point.hash('123'.encode())
+            >>> q = point.hash('456'.encode())
+            >>> (p + q).canonical().hex()[:64]
+            '1ea48cab238fece46bd0c9fb562c859e318e17a8fb75517a4750d30ca79b911c'
+            """
+            p = self._implementation.neg(self)
+            p.__class__ = self.__class__
+            return p
+
+        def __matmul__(self: point, other: point2) -> scalar2:
+            """
+            Return the result of pairing another second-level point with this
+            instance.
+
+            **This method is only defined for the classes**
+            :obj:`oblivious.bn254.mcl.point` **and** :obj:`oblivious.bn254.mcl.point2`
+            **that are available when the**
+            `mclbn256 <https://pypi.org/project/mclbn256>`__ **package is installed**.
+            Otherwise, :obj:`oblivious.bn254.point` and :obj:`oblivious.bn254.point2`
+            correspond to the pure-Python implementations of these classes (for which
+            this method is not defined).
+
+            >>> p = point.hash('123'.encode())
+            >>> q = point2.base(scalar.from_int(456))
+            >>> z = (p @ q).hex()[700:]
+            >>> z == 'd01f7e038b05acc5519eeda026c4aa111eb12f3483f274c60e34e6ec7571435df707'
+            True
+
+            The pairing function is bilinear.
+
+            >>> p = point.random()
+            >>> q = point2.random()
+            >>> s = scalar.random()
+            >>> t = scalar.random()
+            >>> -((~s) * (s * p)) - p == scalar.from_int(-2) * p
+            True
+            >>> (s * (t * p)) @ q == (s * p) @ (t * q)
+            True
+
+            Suppose there are two points: one multiplied by the scalar ``s`` and the other
+            multiplied by the scalar ``t``. Their equality can be determined by using a
+            balancing point: ``g**(~s * t)``.  If the pairing of ``t * x`` with ``g`` is the
+            same as the pairing with ``s * y`` and ``g**(~s * t)``, then ``x`` equals ``y``.
+
+            >>> x = y = p
+            >>> g = point2.base(scalar.from_int(1))
+            >>> b = point2.base(~s * t)
+            >>> (t * x) @ g == (s * y) @ b
+            True
+            """
+            s = self._implementation.par(self, other)
+            s.__class__ = self._implementation.scalar2
+            return s
+
+        def __len__(self: point) -> int:
+            """
+            Return length (in bytes) of the binary representation of this instance.
+
+            >>> len(point())
+            96
+            """
+            return bytes(self).__len__()
+
+        def __bytes__(self: point) -> bytes:
+            """
+            Serialize this instance and return its binary representation.
+
+            >>> p = point.hash('123'.encode())
+            >>> bs = bytes(p)
+            >>> point.from_bytes(bs) == p
+            True
+            >>> type(bs) is bytes
+            True
+            >>> len(bs)
+            96
+            """
+            return self._implementation.ser(self)
+
+        def to_bytes(self: point) -> bytes:
+            """
+            Serialize this instance and return its binary representation.
+
+            >>> p = point.hash('123'.encode())
+            >>> bs = p.to_bytes()
+            >>> point.from_bytes(bs) == p
+            True
+            >>> type(bs) is bytes
+            True
+            >>> len(bs)
+            96
+            """
+            return bytes(self)
+
+        def hex(self: point) -> str:
+            """
+            Return a hexadecimal representation of this instance.
+
+            >>> p = point.hash('123'.encode())
+            >>> p.hex()[:64]
+            '825aa78af4c88d6de4abaebabf1a96f668956b92876cfb5d3a44829899cb480f'
+            """
+            return bytes(self).hex()
+
+        def to_base64(self: point) -> str:
+            """
+            Return the Base64 UTF-8 string representation of this instance.
+
+            >>> p = point.from_base64(
+            ...     'hQIYpQRHupyyfPFoEm8rfmKV6i6VUP7vmngQWpxS3AEJD29fKVMW39l2oDLB+Ece'
+            ...     '5PqBuRzCyiRb8xYIelEII47///////8Viv//////ObnN/////y7GovX//3/ypCsh'
+            ... )
+            >>> p.to_base64()[-64:]
+            '5PqBuRzCyiRb8xYIelEII47///////8Viv//////ObnN/////y7GovX//3/ypCsh'
+            """
+            return base64.standard_b64encode(bytes(self)).decode('utf-8')
+
+    class scalar(_s_base_cls): # pylint: disable=E0102
+        """
+        Class for representing a scalar.
+        """
+        _implementation = _implementation
+
+        @classmethod
+        def random(cls) -> scalar:
+            """
+            Return random non-zero scalar object.
+
+            >>> len(scalar.random())
+            32
+            """
+            s = cls._implementation.rnd()
+            s.__class__ = cls
+            return s
+
+        @classmethod
+        def bytes(cls, bs: bytes) -> Optional[scalar]:
+            """
+            Return scalar object obtained by transforming supplied bytes-like
+            object if it is possible to do so; otherwise, return ``None``.
+
+            >>> s = scalar()
+            >>> t = scalar.bytes(bytes(s))
+            >>> s.hex() == t.hex()
+            True
+            """
+            s = cls._implementation.scl(bs)
+            if s is not None:
+                s.__class__ = cls
+            return s
+
+        @classmethod
+        def hash(cls, bs: bytes) -> scalar:
+            """
+            Return scalar object by hashing supplied bytes-like object.
+
+            >>> scalar.hash('123'.encode()).hex()[:64]
+            '93d829354cb3592743174133104b5405ba6992b67bb219fbde3e394d70505913'
+            """
+            h = hashlib.sha256(bs).digest()
+            s = cls._implementation.scl(h)
+            while s is None:
+                h = hashlib.sha256(h).digest()
+                s = cls._implementation.scl(h)
+
+            s.__class__ = cls
+            return s
+
+        @classmethod
+        def from_int(cls, i: int) -> scalar:
+            """
+            Construct an instance from its corresponding integer (*i.e.*, residue)
+            representation.
+
+            The integer can be in the range from
+            ``-16798108731015832284940804142231733909759579603404752749028378864165570215948``
+            to ``16798108731015832284940804142231733909759579603404752749028378864165570215948``
+            (or a corresponding one in the range from
+            ``-8399054365507916142470402071115866954879789801702376374514189432082785107974``
+            to ``8399054365507916142470402071115866954879789801702376374514189432082785107974``).
+            Any values outside of this range will not be reduced, may be truncated, or may raise
+            a :obj:`ValueError`.  Zero-valued scalars are technically allowed, but cannot be used
+            for point-scalar multiplication.
+
+            >>> int(scalar.from_int(
+            ...    16798108731015832284940804142231733909759579603404752749028378864165570215948
+            ... ))
+            -1
+            >>> int(scalar.from_int(
+            ...    -8399054365507916142470402071115866954879789801702376374514189432082785107974
+            ... ))
+            -8399054365507916142470402071115866954879789801702376374514189432082785107974
+            >>> int(scalar.from_int(
+            ...     12345678
+            ... ))
+            12345678
+            """
+            #r= 0x2523648240000001ba344d8000000007ff9f800000000010a10000000000000d
+            d = 0x212ba4f27ffffff5a2c62effffffffd00242ffffffffff9c39ffffffffffffb2
+            return cls.bytes(int.to_bytes((i * d) % r, 32, 'little'))
+
+        @classmethod
+        def from_bytes(cls, bs: bytes) -> scalar:
+            """
+            Deserialize the supplied binary representation of an instance and
+            return that instance.
+
+            >>> s = scalar.hash('123'.encode())
+            >>> bs = s.to_bytes()
+            >>> scalar.from_bytes(bs) == s
+            True
+            >>> type(bs) is bytes
+            True
+            """
+            s = cls._implementation.sde(bs)
+            s.__class__ = cls
+            return s
+
+        @classmethod
+        def fromhex(cls, s: str) -> scalar:
+            """
+            Construct an instance from its hexadecimal UTF-8 string representation.
+
+            >>> scalar.fromhex(
+            ...     '3ab45f5b1c9339f1d25b878cce1c053b5492b4dc1affe689cbe141769f655e1e'
+            ... ).hex()[:64]
+            '3ab45f5b1c9339f1d25b878cce1c053b5492b4dc1affe689cbe141769f655e1e'
+            """
+            return cls.from_bytes(bytes.fromhex(s))
+
+        @classmethod
+        def from_base64(cls, s: str) -> scalar:
+            """
+            Construct an instance from its Base64 UTF-8 string representation.
+
+            >>> scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=').hex()[:64]
+            '312d0c9130f69153bec9f5d0386a95135eb45eebf130af5f1fed1c6ed15f2500'
+            """
+            return cls.from_bytes(base64.standard_b64decode(s))
+
+        def __new__( # pylint: disable=arguments-differ
+                cls,
+                bs: Union[bytes, bytearray, None] = None
+            ) -> scalar:
+            """
+            If a bytes-like object is supplied, return a scalar object
+            corresponding to the supplied bytes-like object (no checking
+            is performed to confirm that the bytes-like object is a valid
+            scalar). If no argument is supplied, return a random scalar
+            object.
+
+            >>> s = scalar()
+            >>> t = scalar(bytes(s))
+            >>> s.hex() == t.hex()
+            True
+            >>> len(scalar())
+            32
+            """
+            return cls.from_bytes(bs) if bs is not None else cls.random()
+
+        def __invert__(self: scalar) -> scalar:
+            """
+            Return the inverse of a scalar.
+
+            >>> s = scalar()
+            >>> p = point()
+            >>> ((~s) * (s * p)) == p
+            True
+            """
+            s = self._implementation.inv(self)
+            s.__class__ = self.__class__
+            return s
+
+        def __mul__(
+                self: scalar,
+                other: Union[scalar, point, point2]
+            ) -> Optional[Union[scalar, point, point2]]:
+            """
+            Multiply supplied scalar, point, or second-level point by this
+            instance.
+
+            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
+            >>> (s * s).hex()[:64]
+            '0497a5b6a7992e7d77b59c07d4457e8bb3cf580603cfd19e05d1f31342141b00'
+            >>> isinstance(s * s, scalar)
+            True
+            >>> p = point.from_base64(
+            ...     'hQIYpQRHupyyfPFoEm8rfmKV6i6VUP7vmngQWpxS3AEJD29fKVMW39l2oDLB+Ece'
+            ...     '5PqBuRzCyiRb8xYIelEII47///////8Viv//////ObnN/////y7GovX//3/ypCsh'
+            ... )
+            >>> (s * p).canonical().hex()[:64]
+            'eee31d1780ea41771357da19a81eaddf2e7fa560142067b433764cbf98be9002'
+            >>> isinstance(s * p, point)
+            True
+
+            If the second argument is a :obj:`point2` object, this method
+            pre-empts :obj:`point2.__rmul__`.
+
+            >>> p = point2.hash('123'.encode())
+            >>> (s * p).canonical().hex()[:128] == (
+            ...     '451f144e06deecbfe5a1527f2b5cc6f12bbde91c1fdf0d5326ad79ffc53bb106'
+            ...     '6d800275af625de83d72d815335832027cc60c34f22e8c5f89f953740a409702'
+            ... )
+            True
+
+            Any attempt to multiply a value or object of an incompatible type by this
+            instance raises an exception.
+
+            >>> s * 2
+            Traceback (most recent call last):
+              ...
+            TypeError: multiplication by a scalar is defined only for scalars and points
+            """
+            if isinstance(other, self._implementation.scalar):
+                s = self._implementation.smu(self, other)
+                s.__class__ = self.__class__
+                return s
+
+            if isinstance(other, self._implementation.point):
+                p = self._implementation.mul(self, other)
+                p.__class__ = other.__class__
+                return p
+
+            if isinstance(other, self._implementation.point2):
+                p = self._implementation.mul2(self, other)
+                p.__class__ = other.__class__
+                return p
+
+            raise TypeError(
+                'multiplication by a scalar is defined only for scalars and points'
+            )
+
+        def __rmul__(self: scalar, other: Any) -> NoReturn:
+            """
+            A scalar cannot be on the right-hand side of a non-scalar.
+
+            >>> point() * scalar()
+            Traceback (most recent call last):
+              ...
+            TypeError: point must be on right-hand side of multiplication operator
+            """
+            raise TypeError(
+                'scalar must be on left-hand side of multiplication operator'
+            )
+
+        def __add__(self: scalar, other: scalar) -> scalar:
+            """
+            Add another scalar to this instance.
+
+            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
+            >>> (s + s).hex()[:64]
+            '625a182261ec23a77c93eba171d42a27bc68bdd6e3615ebf3eda39dca2bf4a00'
+            >>> isinstance(s + s, scalar)
+            True
+
+            >>> z = scalar2.from_base64(
+            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
+            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
+            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
+            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
+            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
+            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
+            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
+            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
+            ... )
+            >>> (z + z).hex()[700:]
+            '4a1f476a7553bd83a5dd5179f98d9acddae4c505e25e95df6734c901198d83ad9019'
+            >>> isinstance(z + z, scalar2)
+            True
+            """
+            s = self._implementation.sad(self, other)
+            s.__class__ = self.__class__
+            return s
+
+        def __sub__(self: scalar, other: scalar) -> scalar:
+            """
+            Subtract this instance from another scalar.
+
+            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
+            >>> (s - s).hex() == '00' * len(s)
+            True
+            >>> isinstance(s - s, scalar)
+            True
+            """
+            s = self._implementation.ssu(self, other)
+            s.__class__ = self.__class__
+            return s
+
+        def __neg__(self: scalar) -> scalar:
+            """
+            Negate this instance.
+
+            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
+            >>> (-s).hex()
+            'dcd2f36ecf096e4d52360a2fc7150aeca94ba1148e1c855ae212e3d1b004fe24'
+            >>> isinstance(-s, scalar)
+            True
+            """
+            s = self._implementation.sne(self)
+            s.__class__ = self.__class__
+            return s
+
+        def __len__(self: scalar) -> int:
+            """
+            Return length (in bytes) of the binary representation of this instance.
+
+            >>> len(scalar())
+            32
+            """
+            return bytes(self).__len__()
+
+        def __bytes__(self: scalar) -> bytes:
+            """
+            Serialize this instance and return its binary representation.
+
+            >>> s = scalar.hash('123'.encode())
+            >>> bs = bytes(s)
+            >>> scalar.from_bytes(bs) == s
+            True
+            >>> type(bs) is bytes
+            True
+            """
+            return self._implementation.sse(self)
+
+        def to_bytes(self: scalar) -> bytes:
+            """
+            Serialize this instance and return its binary representation.
+
+            >>> s = scalar.hash('123'.encode())
+            >>> bs = s.to_bytes()
+            >>> scalar.from_bytes(bs) == s
+            True
+            >>> type(bs) is bytes
+            True
+            """
+            return bytes(self)
+
+        def __int__(self: scalar) -> bytes:
+            """
+            Compute and return the numerical representation of this instance.
+
+            >>> s = scalar.from_int(123)
+            >>> n = int(s)
+            >>> scalar.from_int(n) == s
+            True
+            >>> type(n) is int
+            True
+            """
+            d_inv = 0x235f846d22752e25720e909a9e82a1b4ad47e882341d8fca46c142d23fa9bc45
+            n = (int.from_bytes(self._implementation.sse(self), 'little') * d_inv) % r
+            return n if (n <= r//2) else n - r
+
+        def to_int(self: scalar) -> bytes:
+            """
+            Compute and return the numerical representation of this instance.
+
+            >>> s = scalar.from_int(123)
+            >>> n = s.to_int()
+            >>> scalar.from_int(n) == s
+            True
+            >>> type(n) is int
+            True
+            """
+            return int(self)
+
+        def hex(self: scalar) -> str:
+            """
+            Return a hexadecimal representation of this instance.
+
+            >>> s = scalar.hash('123'.encode())
+            >>> s.hex()
+            '93d829354cb3592743174133104b5405ba6992b67bb219fbde3e394d70505913'
+            """
+            return self.to_bytes().hex()
+
+        def to_base64(self: scalar) -> str:
+            """
+            Return the Base64 UTF-8 string representation of this instance.
+
+            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
+            >>> s.to_base64()
+            'MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA='
+            """
+            return base64.standard_b64encode(self.to_bytes()).decode('utf-8')
+
+    class point2(_p2_base_cls): # pylint: disable=W0621,E0102
+        # pylint: disable=C0301 # Accommodate large outputs in doctests.
+        """
+        Wrapper class for a bytes-like object that corresponds
+        to a point.
+        """
+        _implementation = _implementation
+
+        @classmethod
+        def random(cls) -> point2:
+            """
+            Return random instance.
+
+            >>> len(point2.random())
+            192
+            """
+            p = cls._implementation.pnt2()
+            p.__class__ = cls
+            return p
+
+        @classmethod
+        def bytes(cls, bs: Union[bytes, bytearray]) -> point2:
+            """
+            Construct an instance that corresponds to the supplied binary
+            representation.
+
+            >>> p = point2.bytes(hashlib.sha512('123'.encode()).digest())
+            >>> p.canonical().hex()[:128] == (
+            ...     '4c595542640a69c4a70bda55c27ef96c133cd1f4a5f83b3371e571960c018e19'
+            ...     'c54aaec2069f8f10a00f12bcbb3511cdb7356201f5277ec5e47da91405be2809'
+            ... )
+            True
+            """
+            p = cls._implementation.pnt2(bs)
+            p.__class__ = cls
+            return p
+
+        @classmethod
+        def hash(cls, bs: Union[bytes, bytearray]) -> point2: # pylint: disable=W0221
+            """
+            Construct an instance by hashing the supplied bytes-like object.
+
+            >>> point2.hash('123'.encode()).canonical().hex()[:128] == (
+            ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
+            ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
+            ... )
+            True
+            """
+            p = cls._implementation.pnt2(hashlib.sha512(bs).digest()[:32])
+            p.__class__ = cls
+            return p
+
+        @classmethod
+        def base(cls, s: scalar) -> point2:
+            """
+            Return base second-level point multiplied by the supplied scalar
+            if the scalar is valid; otherwise, return ``None``.
+
+            >>> point2.base(scalar.hash('123'.encode())).canonical().hex()[:128] == (
+            ...     'e7000fb12d206112c73fe1054e9d77b35c77881eba6598b7e035171d90b13e0c'
+            ...     '33c8ad2c92acb446fa958f3001b6c15aaf0f00092534a9d567541f9fadc64e09'
+            ... )
+            True
+            """
+            p = cls._implementation.bas2(s)
+            p.__class__ = cls
+            return p
+
+        @classmethod
+        def from_bytes(cls, bs: bytes) -> point2:
+            """
+            Deserialize the supplied binary representation of an instance and
+            return that instance.
+
+            >>> p = point2.hash('123'.encode())
+            >>> bs = p.to_bytes()
+            >>> point2.from_bytes(bs) == p
+            True
+            >>> type(bs) is bytes
+            True
+            """
+            p = cls._implementation.des2(bs)
+            p.__class__ = cls
+            return p
+
+        @classmethod
+        def fromhex(cls, s: str) -> point2:
+            """
+            Construct an instance from its hexadecimal UTF-8 string representation.
+
+            >>> p = point2.fromhex(
+            ...     'ab4efa2bcdeb825a67b12a10132ae1addca840ed248f83ae7dd987370dd47a05'
+            ...     '31c10b08ada0e24c0327d85b108e826a55bf3dc3286488327fac75e05e293b20'
+            ...     '01cbf919b53884d02b85aab9b0091eeda114fa65ca5d75620da26c4d164aa509'
+            ...     '2a2d55b6f311bfe52d24adf7b4b0b6ce12ed486a37c474d35a2b373be8a3f71c'
+            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+            ...     '0000000000000000000000000000000000000000000000000000000000000000'
+            ... )
+            >>> p.canonical().hex()[:64]
+            'ab4efa2bcdeb825a67b12a10132ae1addca840ed248f83ae7dd987370dd47a05'
+            """
+            p = cls.from_bytes(bytes.fromhex(s))
+            p.__class__ = cls
+            return p
+
+        @classmethod
+        def from_base64(cls, s: str) -> point2:
+            """
+            Construct an instance from its Base64 UTF-8 string representation.
+
+            >>> p = point2.from_base64(
+            ...     'xRuTJv/OWkIPMxRoCQIqNYoSixnWfMxeYwSJnjdJwxlp9E9f6oKefvbfYlJeygmK'
+            ...     'YDQniir3r/EYExFuClZ7H5X00GEqz7TcoqDl5EpwLDAvrTW3GNA2lOpHvc1F/eQc'
+            ...     'obJoTn35OzzK7qd/87Y3pOKNQaNENKO19DMzw9Lt+hiO////////FYr//////zm5'
+            ...     'zf////8uxqL1//9/8qQrIQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA'
+            ... )
+            >>> p.to_base64()[-64:]
+            'zf////8uxqL1//9/8qQrIQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA'
+            """
+            p = cls.from_bytes(base64.standard_b64decode(s))
+            p.__class__ = cls
+            return p
+
+        def __new__( # pylint: disable=arguments-differ
+                cls,
+                bs: Union[bytes, bytearray, None] = None
+            ) -> point2:
+            """
+            If a bytes-like object is supplied, return a second-level point
+            object corresponding to the supplied bytes-like object (no check
+            is performed to confirm that the bytes-like object is a valid
+            point). If no argument is supplied, a random second-level point
+            is returned.
+
+            >>> bs = bytes.fromhex(
+            ...     'ab4efa2bcdeb825a67b12a10132ae1addca840ed248f83ae7dd987370dd47a05'
+            ...     '31c10b08ada0e24c0327d85b108e826a55bf3dc3286488327fac75e05e293b20'
+            ...     '01cbf919b53884d02b85aab9b0091eeda114fa65ca5d75620da26c4d164aa509'
+            ...     '2a2d55b6f311bfe52d24adf7b4b0b6ce12ed486a37c474d35a2b373be8a3f71c'
+            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+            ...     '0000000000000000000000000000000000000000000000000000000000000000'
+            ... )
+            >>> point2.from_bytes(bs).hex() == bs.hex()
+            True
+            >>> point2.from_bytes(bs).to_bytes() == bs
+            True
+            """
+            p = cls.from_bytes(bs) if bs is not None else cls.random()
+            p.__class__ = cls # = point2
+            return p
+
+        def canonical(self: point2) -> point2:
+            """
+            Normalize the representation of this point into its canonical form
+            and return the result. This takes the *z*-coordinate, which may not
+            always be equal to 1, and multiplies all coordinates *x*, *y*, and
+            *z* by *z*'s multiplicative inverse. The resulting canonical
+            representation is unique (*i.e.*, two second-level points are equal
+            if and only if their canonical forms are equal) and in the form
+            (*x1*/*z1*, *y1*/*z1*, *x2*/*z2*, *y2*/*z2*, 1, 0).
+
+            >>> a = point2.hash('123'.encode())
+            >>> q = a + a + a + a
+            >>> q == q
+            True
+            >>> q.to_bytes() == q.to_bytes()
+            True
+            >>> q.to_bytes() == q.canonical().to_bytes() and q.__class__ != python.point2
+            False
+            >>> q.canonical().to_bytes() == q.canonical().to_bytes()
+            True
+            >>> q.canonical().to_bytes() == q.canonical().canonical().to_bytes()
+            True
+            >>> point2.from_bytes(q.to_bytes()) == q
+            True
+            >>> point2.from_bytes(q.canonical().to_bytes()) == q
+            True
+            >>> point2.from_bytes(q.to_bytes()) == point2.from_bytes(bytes(q.canonical()))
+            True
+            >>> type(q.canonical()) is point2
+            True
+            """
+            p = self._implementation.can(self)
+            p.__class__ = self.__class__
+            return p
+
+        def __mul__(self: point2, other: Any) -> NoReturn:
+            """
+            Use of this method is not permitted. A point cannot be a left-hand argument.
+
+            >>> point2() * scalar()
+            Traceback (most recent call last):
+              ...
+            TypeError: second-level point must be on right-hand side of multiplication operator
+            """
+            raise TypeError(
+                'second-level point must be on right-hand side of multiplication operator'
+            )
+
+        def __rmul__(self: point2, other: Any) -> NoReturn:
+            """
+            This functionality is implemented exclusively in the method
+            :obj:`scalar.__mul__`, as that method pre-empts this method
+            when the second argument has the correct type (*i.e.*, it is
+            a :obj:`scalar` instance). This method is included so that an
+            exception can be raised if an incorrect argument is supplied.
+
+            >>> p = point2.hash('123'.encode())
+            >>> 2 * p
+            Traceback (most recent call last):
+              ...
+            TypeError: second-level point can only be multiplied by a scalar
+            """
+            raise TypeError('second-level point can only be multiplied by a scalar')
+
+        def __add__(self: point2, other: point2) -> Optional[point2]:
+            """
+            Return sum of this instance and another second-level point.
+
+            >>> p = point2.hash('123'.encode())
+            >>> q = point2.hash('456'.encode())
+            >>> (p + q).canonical().hex()[:128] == (
+            ...     'cb0fc423c1bac2ac2df47bf5f5548a42b0d0a0da325bc77243d15dc587a7b221'
+            ...     '9808a1649991ddf770f0060333aab4d499580b123f109b5cb180f1f8a75a090e'
+            ... )
+            True
+            """
+            p = self._implementation.add2(self, other)
+            p.__class__ = self.__class__
+            return p
+
+        def __sub__(self: point2, other: point2) -> Optional[point2]:
+            """
+            Return the result of subtracting another second-level point from
+            this instance.
+
+            >>> p = point2.hash('123'.encode())
+            >>> q = point2.hash('456'.encode())
+            >>> (p - q).canonical().hex()[:128] == (
+            ...     'e97a70c4e3a5369ebbb1dcf0cc1135c8c8e04a4ec7cffdf875ac429d66846d0b'
+            ...     '191b090909c40a723027b07ac44435a6ade3813d04b3632a17c92c5c98718902'
+            ... )
+            True
+            """
+            p = self._implementation.sub2(self, other)
+            p.__class__ = self.__class__
+            return p
+
+        def __neg__(self: point2) -> point2:
+            """
+            Return the negation (additive inverse) of this instance.
+
+            >>> p = point2.hash('123'.encode())
+            >>> (-p).canonical().hex()[:128] == (
+            ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
+            ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
+            ... )
+            True
+            """
+            p = self._implementation.neg2(self)
+            p.__class__ = self.__class__
+            return p
+
+        def __matmul__(self: point2, other: point) -> scalar2:
+            """
+            Return the result of pairing another point with this instance.
+
+            Input-swapped alias of :obj:`point.__matmul__`.
+            """
+            return self._implementation.point.__matmul__(other, self)
+
+        def __len__(self: point2) -> int:
+            """
+            Return length (in bytes) of the binary representation of this instance.
+
+            >>> len(point2())
+            192
+            """
+            return bytes(self).__len__()
+
+        def __bytes__(self: point2) -> bytes:
+            """
+            Serialize this instance and return its binary representation.
+
+            >>> len(bytes(point2()))
+            192
+            """
+            return self._implementation.ser(self)
+
+        def to_bytes(self: point2) -> bytes:
+            """
+            Serialize this instance and return its binary representation.
+
+            >>> p = point2.hash('123'.encode())
+            >>> bs = p.to_bytes()
+            >>> point2.from_bytes(bs) == p
+            True
+            >>> type(bs) is bytes
+            True
+            """
+            return bytes(self)
+
+        def hex(self: point2) -> str:
+            """
+            Return a hexadecimal representation of this instance.
+
+            >>> p = point2.hash('123'.encode())
+            >>> p.canonical().hex() == (
+            ...     '30326199f303fce7a77cff6d2fb0b3de8cd409d1d562f3543f7d064cdc58d309'
+            ...     '7e88038ad76e85e5df26e4a9486a657b0431c8e7e09b0a1abf90fc874c515207'
+            ...     '2c6a88bb448065eb748df632b1d872e02f54b6f56fdb84a7b1cb388fe551fb08'
+            ...     '04464efa186bd4b1371e53d6f31f0e2f50ff553b6264a43331b42c976a0c541f'
+            ...     '8effffffffffff158affffffffff39b9cdffffffff2ec6a2f5ffff7ff2a42b21'
+            ...     '0000000000000000000000000000000000000000000000000000000000000000'
+            ... )
+            True
+            """
+            return self.to_bytes().hex()
+
+        def to_base64(self: point2) -> str:
+            """
+            Return the Base64 UTF-8 string representation of this instance.
+
+            >>> p = point2.from_base64(
+            ...     'zn07zy59PMhe396h9AQ+FY3LqfzmaRmbVmfwKaQqTxStH2ZPqGwBjv99STlWrenq'
+            ...     'Mkfc3PCxRgM1xVaJGN+WExXhuDn4V40nkdpxtU85VFgE4aj0CMUoD99bqTEqBSYD'
+            ...     '50haF1C7mDxMRxmMXZinYDEMynRY69C1vTQ5IgcCdh+O////////FYr//////zm5'
+            ...     'zf////8uxqL1//9/8qQrIQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA'
+            ... )
+            >>> p.to_base64()[-64:]
+            'zf////8uxqL1//9/8qQrIQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA'
+            """
+            return base64.standard_b64encode(self.to_bytes()).decode('utf-8')
+
+    class scalar2(_s2_base_cls): # pylint: disable=function-redefined
+        """
+        Class for representing second-level scalars.
+        """
+        _implementation = _implementation
+
+        @classmethod
+        def random(cls) -> scalar2:
+            """
+            Return random non-zero second-level scalar.
+
+            >>> isinstance(scalar2.random(), scalar2)
+            True
+            >>> len(scalar2.random())
+            384
+            """
+            s = cls._implementation.scl2()
+            s.__class__ = cls
+            return s
+
+        @classmethod
+        def bytes(cls, bs: bytes) -> Optional[scalar2]:
+            """
+            Return second-level scalar object obtained by transforming the
+            supplied bytes-like object if it is possible to do so; otherwise,
+            return ``None``.
+
+            >>> s = scalar2()
+            >>> t = scalar2.bytes(bytes(s))
+            >>> s.hex() == t.hex()
+            True
+            """
+            s = cls._implementation.scl2(bs)
+
+            if s is not None:
+                s.__class__ = cls
+
+            return s
+
+        @classmethod
+        def hash(cls, bs: Union[bytes, bytearray]) -> scalar2:
+            """
+            Return an instance derived by hashing the supplied bytes-like object.
+
+            >>> s = python.scalar2.hash(bytes([123]))
+            >>> s.hex()[700:]
+            'e91ed56ea67d29047d588ffaf78f9ed317ff13e7f63e53276ff32988c49184e17b22'
+
+            >>> s0 = python.scalar2.hash(secrets.token_bytes(64))
+            >>> s1 = python.scalar2.hash(secrets.token_bytes(64))
+            >>> python.sse(python.smu2(python.smu2(s0, python.inv2(s0)), s1)) == python.sse(s1)
+            True
+            """
+            def pick_exponent(bs):
+                i = int.from_bytes(bs, 'little')
+
+                # Use rejection sampling to get two valid components in F_p.
+                if i >= r-1:
+                    return pick_exponent(hashlib.sha512(bs).digest()[:32])
+
+                return i+1
+
+            bs = hashlib.sha512(bs).digest()
+            exponent = pick_exponent(bs[:32])
+
+            # Generator of paired ``scalar2`` codomain, computed from pairing
+            # the base points for ``point`` and ``point2``.
+            z = cls._implementation.scalar2.from_base64('X+CkvfROeA1SsbpkudwsTzqOGQC9BkDmNcYpI0GHGg'
+            'TPr7fTv0yO88u5bybAlDc4QTCji5RvpdhGkWLT5oysD7UX5qE2ymq+HJXrl5MkiPp4J6kfZ6Obdjr9J/G4qs4U'
+            'hNgtOCecKCgdEwI4KyCbtYu5Wv2M+IgvJbWUx4ihaB1HlDwFb6rTmaa8ckaoFtY6AoM5kbbDPgNN71441LrNC5'
+            'Fp2QGPRod8+0WJ9wzl6R6cWLSV14MzoqWY6ZNDAyUPMpUaUGbIKZ3QqlpxM5EOFTTYmPQqOBY3K+tNL94yZRIM'
+            'ChE3W1ph9ypDcdFNd9xloWOw/APAa4FE538HbMZFEix4XpNKKIl3WPbGhTb/iY7DuUqKXouNdw8wSvzIVEYjBY'
+            '6IuE7e3fr7GMvd6K/8qO3Cep7EeuFzdMKxMO21PhuhBm2KLDPbzuzoNrMfmiMOhFJadkIa8F0NmWEEKEpyCIph'
+            'CwjHidMthVF/l932N4LL6EVktec8TQrotfCCEA0O')
+
+            def square_and_multiply_exp(s, exponent):
+                if exponent == 1:
+                    return s
+
+                s = s * s
+
+                if exponent % 2 == 1:
+                    s = s * z
+
+                return square_and_multiply_exp(s, exponent // 2)
+
+            return square_and_multiply_exp(z, exponent)
+
+        @classmethod
+        def from_bytes(cls, bs: bytes) -> scalar2:
+            """
+            Deserialize the supplied binary representation of an instance and
+            return that instance.
+
+            >>> s = scalar2.hash('123'.encode())
+            >>> bs = s.to_bytes()
+            >>> scalar2.from_bytes(bs) == s
+            True
+            >>> type(bs) is bytes
+            True
+            """
+            s = cls._implementation.sde2(bs)
+            s.__class__ = cls
+            return s
+
+        @classmethod
+        def fromhex(cls, s: str) -> scalar2:
+            """
+            Construct an instance from its hexadecimal UTF-8 string representation.
+
+            >>> s_hex = (
+            ...     '18d0e065798ffa4ecca0a7cc6e2b8d6d3269f7eb413525e59b731332b02ea805'
+            ...     '4b90c89ce93e4452557f53aae5f8f13221858dde2ea6a50373f1858f11287021'
+            ...     '09b3daf7a217a20a3d872632f8ced643d32649b241a67601bec855bd43f07710'
+            ...     '88df722bcacc8fd174f16ad7ef1b1d5e622d93b7cfec6385c353c13793a4e01c'
+            ...     '371ef54cd836a88e1b1f1e198d566d3bbe5aa225734305f14cac9af9c821351c'
+            ...     '86b365190105d1b7e71011d1362ed6ad9133a2c2c42898e9ebc3d1604a608f10'
+            ...     '8461d37b2463b4f88f0ccb427b5eea8714ee88f8c33daf7ee4a3f45ca8bca911'
+            ...     '87956abb4d27de1b49e5e059f904fbb475804715ab25a17306fa0e196f305215'
+            ...     '3a60dfa073ca78de49edeaac9c54cab3d0138750c23c0b68de7924a69d1ba002'
+            ...     'a24ac592622a45c59c1ded7133794292a09602bd57a36601d35438846fcb370f'
+            ...     '39c0fa7a15b34d14ab6f95ee5bf5b26bd5def1e7ed07350922d445da07d93622'
+            ...     '2db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
+            ... )
+            >>> s = scalar2.fromhex(s_hex)
+            >>> s.hex() == s_hex
+            True
+            """
+            return cls.from_bytes(bytes.fromhex(s))
+
+        @classmethod
+        def from_base64(cls, s: str) -> scalar2:
+            """
+            Construct an instance from its Base64 UTF-8 string representation.
+
+            >>> b64s = (
+            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
+            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
+            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
+            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
+            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
+            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
+            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
+            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
+            ... )
+            >>> s = scalar2.from_base64(b64s)
+            >>> s.to_base64() == b64s
+            True
+            """
+            return cls.from_bytes(base64.standard_b64decode(s))
+
+        def __new__( # pylint: disable=arguments-differ
+                cls,
+                bs: Union[bytes, bytearray, None] = None
+            ) -> scalar2:
+            """
+            If a bytes-like object is supplied, return an instance that corresponds
+            to the supplied bytes-like object (no checking is performed to confirm
+            that the bytes-like object is a valid second-level scalar). If no
+            argument is supplied, return a random scalar object.
+            """
+            return cls.from_bytes(bs) if bs is not None else cls.random()
+
+        def __invert__(self: scalar2) -> scalar2:
+            """
+            Return the inverse of this instance.
+
+            >>> s = scalar2.hash('123'.encode())
+            >>> ~(~s) == s
+            True
+            >>> ~s == s
+            False
+            >>> bytes(~s).hex()[700:] == (
+            ...     'ff13804852ea3ad35e8316d90a6d5dde854517e74cfc27ba676f429eb4fd52cd9b0c'
+            ... )
+            True
+            """
+            s = self._implementation.inv2(self)
+            s.__class__ = self.__class__
+            return s
+
+        def __mul__(self: scalar2, other: scalar2) -> scalar2:
+            """
+            Multiply this instance by another second-level scalar.
+
+            >>> s = scalar2.from_base64(
+            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
+            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
+            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
+            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
+            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
+            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
+            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
+            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
+            ... )
+            >>> bytes(s * s).hex()[700:]
+            '6f11685b89b03431dac6dc9d129c6a31cc5e3036f7f781d7460ab9f532a06845bd15'
+            >>> scalar2() * point()
+            Traceback (most recent call last):
+              ...
+            TypeError: second-level scalar can only be multiplied by another second-level scalar
+            """
+            if isinstance(other, self._implementation.scalar2):
+                s = self._implementation.smu2(self, other)
+                s.__class__ = self.__class__
+                return s
+
+            raise TypeError(
+                'second-level scalar can only be multiplied by another second-level scalar'
+            )
+
+        def __rmul__(self: scalar2, other: Any) -> NoReturn:
+            """
+            A second-level scalar cannot be on the right-hand side of a non-scalar.
+
+            >>> 2 * scalar2()
+            Traceback (most recent call last):
+              ...
+            TypeError: second-level scalar must be on left-hand side of multiplication operator
+            """
+            raise TypeError(
+                'second-level scalar must be on left-hand side of multiplication operator'
+            )
+
+        def __add__(self: scalar2, other: scalar2) -> scalar2:
+            """
+            Add another second-level scalar to this instance.
+
+            >>> z = scalar2.from_base64(
+            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
+            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
+            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
+            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
+            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
+            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
+            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
+            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
+            ... )
+            >>> (z + z).hex()[700:]
+            '4a1f476a7553bd83a5dd5179f98d9acddae4c505e25e95df6734c901198d83ad9019'
+            >>> isinstance(z + z, scalar2)
+            True
+            """
+            s = self._implementation.sad2(self, other)
+            s.__class__ = self.__class__
+            return s
+
+        def __len__(self: scalar2) -> int:
+            """
+            Return length (in bytes) of the binary representation of this instance.
+
+            >>> len(scalar2.random())
+            384
+            """
+            return bytes(self).__len__()
+
+        def __bytes__(self: scalar2) -> bytes:
+            """
+            Serialize this instance and return its binary representation.
+
+            >>> s = scalar2.hash('123'.encode())
+            >>> bs = bytes(s)
+            >>> scalar2.from_bytes(bs) == s
+            True
+            >>> type(bs) is bytes
+            True
+            >>> len(bs)
+            384
+            """
+            self.__class__ = self.__class__._implementation.scalar2
+            return self._implementation.sse(self)
+
+        def to_bytes(self: scalar2) -> bytes:
+            """
+            Serialize this instance and return its binary representation.
+
+            >>> s = scalar2.hash('123'.encode())
+            >>> bs = s.to_bytes()
+            >>> scalar2.from_bytes(bs) == s
+            True
+            >>> type(bs) is bytes
+            True
+            >>> len(bs)
+            384
+            """
+            return bytes(self)
+
+        def hex(self: scalar2) -> str:
+            """
+            Return a hexadecimal representation of this instance.
+
+            >>> s = scalar2.from_base64(
+            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
+            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
+            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
+            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
+            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
+            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
+            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
+            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
+            ... )
+            >>> s.hex() == (
+            ...     '18d0e065798ffa4ecca0a7cc6e2b8d6d3269f7eb413525e59b731332b02ea805'
+            ...     '4b90c89ce93e4452557f53aae5f8f13221858dde2ea6a50373f1858f11287021'
+            ...     '09b3daf7a217a20a3d872632f8ced643d32649b241a67601bec855bd43f07710'
+            ...     '88df722bcacc8fd174f16ad7ef1b1d5e622d93b7cfec6385c353c13793a4e01c'
+            ...     '371ef54cd836a88e1b1f1e198d566d3bbe5aa225734305f14cac9af9c821351c'
+            ...     '86b365190105d1b7e71011d1362ed6ad9133a2c2c42898e9ebc3d1604a608f10'
+            ...     '8461d37b2463b4f88f0ccb427b5eea8714ee88f8c33daf7ee4a3f45ca8bca911'
+            ...     '87956abb4d27de1b49e5e059f904fbb475804715ab25a17306fa0e196f305215'
+            ...     '3a60dfa073ca78de49edeaac9c54cab3d0138750c23c0b68de7924a69d1ba002'
+            ...     'a24ac592622a45c59c1ded7133794292a09602bd57a36601d35438846fcb370f'
+            ...     '39c0fa7a15b34d14ab6f95ee5bf5b26bd5def1e7ed07350922d445da07d93622'
+            ...     '2db5baa9dec152c2b2bcfc46cde6fd22e70271af8a164e77e5808ce602095a1f'
+            ... )
+            True
+            """
+            return self.to_bytes().hex()
+
+        def to_base64(self: scalar2) -> str:
+            """
+            Return the Base64 UTF-8 string representation of this instance.
+
+            >>> b64s = (
+            ...     'GNDgZXmP+k7MoKfMbiuNbTJp9+tBNSXlm3MTMrAuqAVLkMic6T5EUlV/U6rl+PEy'
+            ...     'IYWN3i6mpQNz8YWPEShwIQmz2veiF6IKPYcmMvjO1kPTJkmyQaZ2Ab7IVb1D8HcQ'
+            ...     'iN9yK8rMj9F08WrX7xsdXmItk7fP7GOFw1PBN5Ok4Bw3HvVM2DaojhsfHhmNVm07'
+            ...     'vlqiJXNDBfFMrJr5yCE1HIazZRkBBdG35xAR0TYu1q2RM6LCxCiY6evD0WBKYI8Q'
+            ...     'hGHTeyRjtPiPDMtCe17qhxTuiPjDPa9+5KP0XKi8qRGHlWq7TSfeG0nl4Fn5BPu0'
+            ...     'dYBHFasloXMG+g4ZbzBSFTpg36BzynjeSe3qrJxUyrPQE4dQwjwLaN55JKadG6AC'
+            ...     'okrFkmIqRcWcHe1xM3lCkqCWAr1Xo2YB01Q4hG/LNw85wPp6FbNNFKtvle5b9bJr'
+            ...     '1d7x5+0HNQki1EXaB9k2Ii21uqnewVLCsrz8Rs3m/SLnAnGvihZOd+WAjOYCCVof'
+            ... )
+            >>> s = scalar2.from_base64(b64s)
+            >>> s.to_base64() == b64s
+            True
+            """
+            return base64.standard_b64encode(bytes(self)).decode('utf-8')
+
+    # Encapsulate classes for this implementation, regardless of which are
+    # exported as the unqualified symbols.
+    _implementation.point = point
+    _implementation.scalar = scalar
+    _implementation.point2 = point2
+    _implementation.scalar2 = scalar2
+
+# Remove method for which no pure-Python implementation exists.
+delattr(python.point, '__matmul__')
+delattr(python.point2, '__matmul__')
+
+# Redefine top-level wrapper classes to ensure that they appear at the end of
+# the auto-generated documentation.
+python = python # pylint: disable=self-assigning-variable
+mcl = mcl # pylint: disable=self-assigning-variable
+
+if __name__ == '__main__':
+    doctest.testmod() # pragma: no cover
```

### Comparing `oblivious-6.0.0/src/oblivious/ristretto.py` & `oblivious-7.0.0/src/oblivious/ristretto.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,1211 +1,1211 @@
-"""
-.. module:: ristretto
-
-ristretto module
-================
-
-This module exports the classes :obj:`~oblivious.ristretto.point` and
-:obj:`~oblivious.ristretto.scalar` for representing points and scalars. It
-also exports the two wrapper classes/namespaces
-:obj:`~oblivious.ristretto.python` and :obj:`~oblivious.ristretto.sodium`
-that encapsulate pure-Python and shared/dynamic library variants of the
-above (respectively) and also include low-level operations that correspond
-more directly to the functions found in the underlying libraries.
-
-* Under all conditions, the wrapper class :obj:`~oblivious.ristretto.python`
-  is defined and encapsulates a pure-Python variant of every class exported
-  by this module as a whole. It also includes pure-Python variants of low-level
-  operations that correspond to functions found in the underlying libraries.
-
-* If a shared/dynamic library instance of the
-  `libsodium <https://doc.libsodium.org>`__ library is found on the system
-  (and successfully loaded at the time this module is imported) or the
-  optional `rbcl <https://pypi.org/project/rbcl>`__ package is installed,
-  then the wrapper class :obj:`~oblivious.ristretto.sodium` is defined.
-  Otherwise, the exported variable ``sodium`` is assigned ``None``.
-
-* If a dynamic/shared library instance is loaded, all classes exported by
-  this module correspond to the variants defined within
-  :obj:`~oblivious.ristretto.sodium`. Otherwise, they correspond to the
-  variants defined within :obj:`~oblivious.ristretto.python`.
-
-For most users, the classes :obj:`~oblivious.ristretto.point` and
-:obj:`~oblivious.ristretto.scalar` should be sufficient. When using the
-low-level operations that correspond to a specific implementation (*e.g.*,
-:obj:`oblivious.ristretto.sodium.add`), users are responsible for ensuring
-that inputs have the type and/or representation appropriate for that
-operation.
-"""
-from __future__ import annotations
-from typing import Any, NoReturn, Union, Optional
-import doctest
-import platform
-import os
-import hashlib
-import ctypes
-import ctypes.util
-import secrets
-import base64
-import ge25519
-
-#
-# Attempt to load rbcl. If no local libsodium shared/dynamic library file
-# is found, only pure-Python implementations of the functions and methods
-# will be available.
-#
-
-try: # pragma: no cover
-    import rbcl # pylint: disable=E0401
-
-    # Add synonyms to deal with variations in capitalization of function names.
-    setattr(
-        rbcl,
-        'crypto_core_ristretto255_scalarbytes',
-        lambda: rbcl.crypto_core_ristretto255_SCALARBYTES
-    )
-    setattr(
-        rbcl,
-        'crypto_core_ristretto255_bytes',
-        lambda: rbcl.crypto_core_ristretto255_BYTES
-    )
-except: # pylint: disable=W0702 # pragma: no cover
-    rbcl = None
-
-#
-# Use pure-Python implementations of primitives by default.
-#
-
-def _zero(n: bytes) -> bool:
-    d = 0
-    for b in n:
-        d |= b
-    return ((d - 1) >> 8) % 2 == 1
-
-_sc25519_is_canonical_L = [ # 2^252+27742317777372353535851937790883648493.
-    0xed, 0xd3, 0xf5, 0x5c, 0x1a, 0x63, 0x12, 0x58, 0xd6, 0x9c, 0xf7,
-    0xa2, 0xde, 0xf9, 0xde, 0x14, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
-    0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x10
-]
-
-def _sc25519_is_canonical(s: bytes) -> bool:
-    """
-    Confirm that the bytes-like object represents a canonical
-    scalar.
-    """
-    c = 0
-    n = 1
-    for i in range(31, -1, -1):
-        c |= ((s[i] - _sc25519_is_canonical_L[i]) >> 8) & n
-        n &= ((s[i] ^ _sc25519_is_canonical_L[i]) - 1) >> 8
-    return c != 0
-
-def _sc25519_mul(a: bytes, b: bytes) -> bytes:
-    """
-    Multiply the two scalars represented by the bytes-like objects
-    """
-    (a, b) = (int.from_bytes(a, 'little'), int.from_bytes(b, 'little'))
-    return (
-        (a * b) % (pow(2, 252) + 27742317777372353535851937790883648493)
-    ).to_bytes(32, 'little')
-
-def _sc25519_sqmul(s: bytes, n: int, a: bytes) -> bytes:
-    """
-    Perform repeated squaring of a scalar for the designated number
-    of iterations, then multiply the result by another scalar.
-    """
-    for _ in range(n):
-        s = _sc25519_mul(s, s)
-    return _sc25519_mul(s, a)
-
-def _sc25519_invert(s: bytes) -> bytes:
-    """
-    Invert the scalar represented by the bytes-like object.
-    """
-    b_10 = _sc25519_mul(s, s)
-    b_100 = _sc25519_mul(b_10, b_10)
-    b_11 = _sc25519_mul(b_10, s)
-    b_101 = _sc25519_mul(b_10, b_11)
-    b_111 = _sc25519_mul(b_10, b_101)
-    b_1001 = _sc25519_mul(b_10, b_111)
-    b_1011 = _sc25519_mul(b_10, b_1001)
-    b_1111 = _sc25519_mul(b_100, b_1011)
-    recip = _sc25519_mul(b_1111, s)
-
-    recip = _sc25519_sqmul(recip, 123 + 3, b_101)
-    recip = _sc25519_sqmul(recip, 2 + 2, b_11)
-    recip = _sc25519_sqmul(recip, 1 + 4, b_1111)
-    recip = _sc25519_sqmul(recip, 1 + 4, b_1111)
-    recip = _sc25519_sqmul(recip, 4, b_1001)
-    recip = _sc25519_sqmul(recip, 2, b_11)
-    recip = _sc25519_sqmul(recip, 1 + 4, b_1111)
-    recip = _sc25519_sqmul(recip, 1 + 3, b_101)
-    recip = _sc25519_sqmul(recip, 3 + 3, b_101)
-    recip = _sc25519_sqmul(recip, 3, b_111)
-    recip = _sc25519_sqmul(recip, 1 + 4, b_1111)
-    recip = _sc25519_sqmul(recip, 2 + 3, b_111)
-    recip = _sc25519_sqmul(recip, 2 + 2, b_11)
-    recip = _sc25519_sqmul(recip, 1 + 4, b_1011)
-    recip = _sc25519_sqmul(recip, 2 + 4, b_1011)
-    recip = _sc25519_sqmul(recip, 6 + 4, b_1001)
-    recip = _sc25519_sqmul(recip, 2 + 2, b_11)
-    recip = _sc25519_sqmul(recip, 3 + 2, b_11)
-    recip = _sc25519_sqmul(recip, 3 + 2, b_11)
-    recip = _sc25519_sqmul(recip, 1 + 4, b_1001)
-    recip = _sc25519_sqmul(recip, 1 + 3, b_111)
-    recip = _sc25519_sqmul(recip, 2 + 4, b_1111)
-    recip = _sc25519_sqmul(recip, 1 + 4, b_1011)
-    recip = _sc25519_sqmul(recip, 3, b_101)
-    recip = _sc25519_sqmul(recip, 2 + 4, b_1111)
-    recip = _sc25519_sqmul(recip, 3, b_101)
-    recip = _sc25519_sqmul(recip, 1 + 2, b_11)
-
-    return recip
-
-def _ristretto255_is_canonical(s: bytes) -> bool:
-    """
-    Confirm that the bytes-like object represents a canonical
-    Ristretto point.
-    """
-    c = ((s[31] & 0x7f) ^ 0x7f) % 256
-    for i in range(30, 0, -1):
-        c |= (s[i] ^ 0xff) % 256
-    c = (c - 1) >> 8
-    d = ((0xed - 1 - s[0]) >> 8) % 256
-    return (1 - (((c & d) | s[0]) & 1)) == 1
-
-class python:
-    """
-    Wrapper class for pure-Python implementations of primitive operations.
-
-    This class encapsulates pure-Python variants of all low-level operations
-    and of both classes exported by this module:
-    :obj:`python.scl <scl>`, :obj:`python.rnd <rnd>`,
-    :obj:`python.inv <inv>`, :obj:`python.smu <smu>`,
-    :obj:`python.pnt <pnt>`, :obj:`python.bas <bas>`,
-    :obj:`python.can <can>`, :obj:`python.mul <mul>`,
-    :obj:`python.add <add>`, :obj:`python.sub <sub>`,
-    :obj:`python.neg <neg>`,
-    :obj:`python.point <oblivious.ristretto.python.point>`, and
-    :obj:`python.scalar <oblivious.ristretto.python.scalar>`.
-    For example, you can perform addition of points using
-    the pure-Python point addition implementation.
-
-    >>> p = python.pnt()
-    >>> q = python.pnt()
-    >>> python.add(p, q) == python.add(q, p)
-    True
-
-    Pure-Python variants of the :obj:`python.point <point>` and
-    :obj:`python.scalar <scalar>` classes always employ pure-Python
-    implementations of operations when their methods are invoked.
-
-    >>> p = python.point()
-    >>> q = python.point()
-    >>> p + q == q + p
-    True
-
-    Nevertheless, all bytes-like objects, :obj:`point` objects, and
-    :obj:`scalar` objects accepted and emitted by the various operations and
-    class methods in :obj:`python` are compatible with those accepted and
-    emitted by the operations and class methods in :obj:`sodium`.
-    """
-    @staticmethod
-    def pnt(h: bytes = None) -> bytes:
-        """
-        Return point from 64-byte vector (normally obtained via hashing).
-
-        >>> p = python.pnt(hashlib.sha512('123'.encode()).digest())
-        >>> p.hex()
-        '047f39a6c6dd156531a25fa605f017d4bec13b0b6c42f0e9b641c8ee73359c5f'
-        """
-        return ge25519.ge25519_p3.from_hash_ristretto255(
-            hashlib.sha512(python.rnd()).digest() if h is None else h
-        )
-
-    @staticmethod
-    def bas(s: bytes) -> bytes:
-        """
-        Return base point multiplied by supplied scalar.
-
-        >>> python.bas(scalar.hash('123'.encode())).hex()
-        '4c207a5377f3badf358914f20b505cd1e2a6396720a9c240e5aff522e2446005'
-        """
-        t = bytearray(s)
-        t[31] &= 127
-
-        return ge25519.ge25519_p3.scalar_mult_base(t).to_bytes_ristretto255()
-
-    @staticmethod
-    def can(p: bytes) -> bytes:
-        """
-        Normalize the representation of a point into its canonical form.
-
-        >>> p = point.hash('123'.encode())
-        >>> python.can(p) == p
-        True
-        """
-        return p # In this module, the canonical representation is used at all times.
-
-    @staticmethod
-    def mul(s: bytes, p: bytes) -> bytes:
-        """
-        Multiply the point by the supplied scalar and return the result.
-
-        >>> p = python.pnt(hashlib.sha512('123'.encode()).digest())
-        >>> s = python.scl(bytes.fromhex(
-        ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-        ... ))
-        >>> python.mul(s, p).hex()
-        '183a06e0fe6af5d7913afb40baefc4dd52ae718fee77a3a0af8777c89fe16210'
-        """
-        p3 = ge25519.ge25519_p3.from_bytes_ristretto255(p)
-        if not _ristretto255_is_canonical(p) or p3 is None:
-            return bytes(32) # pragma: no cover
-
-        t = bytearray(s)
-        t[31] &= 127
-
-        return p3.scalar_mult(t).to_bytes_ristretto255()
-
-    @staticmethod
-    def add(p: bytes, q: bytes) -> bytes:
-        """
-        Return sum of the supplied points.
-
-        >>> p = point.hash('123'.encode())
-        >>> q = point.hash('456'.encode())
-        >>> python.add(p, q).hex()
-        '7076739c9df665d416e68b9512f5513bf1d0181a2aacefdeb1b7244528a4dd77'
-        """
-        p_p3 = ge25519.ge25519_p3.from_bytes_ristretto255(p)
-        q_p3 = ge25519.ge25519_p3.from_bytes_ristretto255(q)
-        if (
-            not _ristretto255_is_canonical(p) or p_p3 is None or
-            not _ristretto255_is_canonical(q) or q_p3 is None
-        ):
-            return bytes(32) # pragma: no cover
-
-        q_cached = ge25519.ge25519_cached.from_p3(q_p3)
-        r_p1p1 = ge25519.ge25519_p1p1.add(p_p3, q_cached)
-        r_p3 = ge25519.ge25519_p3.from_p1p1(r_p1p1)
-        return r_p3.to_bytes_ristretto255()
-
-    @staticmethod
-    def sub(p: bytes, q: bytes) -> bytes:
-        """
-        Return result of subtracting second point from first point.
-
-        >>> p = point.hash('123'.encode())
-        >>> q = point.hash('456'.encode())
-        >>> python.sub(p, q).hex()
-        '1a3199ca7debfe31a90171696d8bab91b99eb23a541b822a7061b09776e1046c'
-        """
-        p_p3 = ge25519.ge25519_p3.from_bytes_ristretto255(p)
-        q_p3 = ge25519.ge25519_p3.from_bytes_ristretto255(q)
-        if (
-            not _ristretto255_is_canonical(p) or p_p3 is None or
-            not _ristretto255_is_canonical(q) or q_p3 is None
-        ):
-            return bytes(32) # pragma: no cover
-
-        q_cached = ge25519.ge25519_cached.from_p3(q_p3)
-        r_p1p1 = ge25519.ge25519_p1p1.sub(p_p3, q_cached)
-        r_p3 = ge25519.ge25519_p3.from_p1p1(r_p1p1)
-        return r_p3.to_bytes_ristretto255()
-
-    @staticmethod
-    def neg(p: bytes) -> bytes:
-        """
-        Return the additive inverse of a point.
-
-        >>> p = point.hash('123'.encode())
-        >>> q = point.hash('456'.encode())
-        >>> python.add(python.neg(p), python.add(p, q)) == q
-        True
-        """
-        return python.sub(bytes(32), p)
-
-    @staticmethod
-    def rnd() -> bytes:
-        """
-        Return random non-zero scalar.
-
-        >>> len(python.rnd())
-        32
-        """
-        while True:
-            r = bytearray(secrets.token_bytes(32))
-            r[-1] &= 0x1f
-            if _sc25519_is_canonical(r) and not _zero(r):
-                return r
-
-    @classmethod
-    def scl(cls, s: bytes = None) -> Optional[bytes]:
-        """
-        Return supplied byte vector if it is a valid scalar; otherwise, return
-        ``None``. If no byte vector is supplied, return a random scalar.
-
-        >>> s = python.scl()
-        >>> t = python.scl(s)
-        >>> s == t
-        True
-        >>> python.scl(bytes([255] * 32)) is None
-        True
-        """
-        if s is None:
-            return cls.rnd()
-
-        s = bytearray(s)
-        s[-1] &= 0x1f
-
-        return bytes(s) if _sc25519_is_canonical(s) else None
-
-    @staticmethod
-    def inv(s: bytes) -> bytes:
-        """
-        Return the inverse of a scalar (modulo
-        ``2**252 + 27742317777372353535851937790883648493``).
-
-        >>> s = python.scl()
-        >>> p = python.pnt()
-        >>> python.mul(python.inv(s), python.mul(s, p)) == p
-        True
-        """
-        return _sc25519_invert(s)
-
-    @staticmethod
-    def smu(s: bytes, t: bytes) -> bytes:
-        """
-        Return scalar multiplied by another scalar.
-
-        >>> s = python.scl()
-        >>> t = python.scl()
-        >>> python.smu(s, t) == python.smu(t, s)
-        True
-        """
-        return _sc25519_mul(s, t)
-
-#
-# Attempt to load primitives from libsodium, if it is present;
-# otherwise, use the rbcl library, if it is present. Otherwise,
-# silently assign ``None`` to ``sodium``.
-#
-
-try:
-    def _call_variant_unwrapped(length, function, x=None, y=None):
-        """
-        Wrapper to invoke external function.
-        """
-        buf = ctypes.create_string_buffer(length)
-        if y is not None:
-            function(buf, x, y)
-        elif x is not None:
-            function(buf, x)
-        else:
-            function(buf)
-        return buf.raw
-
-    def _call_variant_wrapped(_, function, x=None, y=None): # pragma: no cover
-        """
-        Wrapper to invoke external (wrapped) function.
-        """
-        if y is not None:
-            return function(x, y)
-        if x is not None:
-            return function(x)
-        return function()
-
-    _sodium = None
-    _call_variant = _call_variant_unwrapped
-
-    # Attempt to load libsodium shared/dynamic library file.
-    xdll = ctypes.cdll if platform.system() != 'Windows' else ctypes.windll
-    libf = ctypes.util.find_library('sodium') or ctypes.util.find_library('libsodium')
-    if libf is not None:
-        _sodium = xdll.LoadLibrary(libf)
-    else: # pragma: no cover
-        # Perform explicit search in case `ld` is not present in environment.
-        libf = 'libsodium.so' if platform.system() != 'Windows' else 'libsodium.dll'
-        for var in ['PATH', 'LD_LIBRARY_PATH']:
-            if var in os.environ:
-                for path in os.environ[var].split(os.pathsep):
-                    try:
-                        _sodium = ctypes.cdll.LoadLibrary(path + os.path.sep + libf)
-                        break
-                    except: # pylint: disable=W0702
-                        continue
-
-        # Default to bindings exported by the rbcl library if the above attempts
-        # failed and rbcl is available.
-        if _sodium is None and rbcl is not None: # pragma: no cover
-            _sodium = rbcl
-            _call_variant = _call_variant_wrapped
-
-    # Add method variants that are not present in libsodium.
-    if _sodium is not rbcl and _sodium is not None: # pragma: no cover
-
-        def _crypto_scalarmult_ristretto255_allow_scalar_zero(buf, s, p):
-            """
-            Variant of scalar-point multiplication function that permits
-            a scalar corresponding to the zero residue.
-            """
-            r = _sodium.crypto_scalarmult_ristretto255(buf, s, p)
-
-            if (1 - _zero(s)) * int(r == -1):
-                raise RuntimeError('libsodium error (possibly due to invalid input)')
-
-            return buf
-
-        def _crypto_scalarmult_ristretto255_base_allow_scalar_zero(buf, s):
-            """
-            Variant of scalar-point multiplication function that permits
-            a scalar corresponding to the zero residue.
-            """
-            r = _sodium.crypto_scalarmult_ristretto255_base(buf, s)
-
-            if (1 - _zero(s)) * int(r == -1):
-                raise RuntimeError('libsodium error (possibly due to invalid input)')
-
-            return buf
-
-        setattr(
-            _sodium,
-            'crypto_scalarmult_ristretto255_allow_scalar_zero',
-            _crypto_scalarmult_ristretto255_allow_scalar_zero
-        )
-        setattr(
-            _sodium,
-            'crypto_scalarmult_ristretto255_base_allow_scalar_zero',
-            _crypto_scalarmult_ristretto255_base_allow_scalar_zero
-        )
-
-    # Ensure the chosen version of libsodium (or its substitute) has the
-    # necessary primitives.
-    assert hasattr(_sodium, 'crypto_core_ristretto255_bytes')
-    assert hasattr(_sodium, 'crypto_core_ristretto255_scalarbytes')
-    assert hasattr(_sodium, 'crypto_core_ristretto255_scalar_random')
-    assert hasattr(_sodium, 'crypto_core_ristretto255_scalar_invert')
-    assert hasattr(_sodium, 'crypto_core_ristretto255_scalar_mul')
-    assert hasattr(_sodium, 'crypto_core_ristretto255_from_hash')
-    assert hasattr(_sodium, 'crypto_scalarmult_ristretto255_base')
-    assert hasattr(_sodium, 'crypto_scalarmult_ristretto255')
-    assert hasattr(_sodium, 'crypto_core_ristretto255_add')
-    assert hasattr(_sodium, 'crypto_core_ristretto255_sub')
-
-    # Exported symbol.
-    class sodium:
-        """
-        Wrapper class for binary implementations of primitive operations.
-
-        When this module is imported, it makes a number of attempts to
-        locate an instance of the shared/dynamic library file of the
-        `libsodium <https://doc.libsodium.org>`__ library on the host
-        system. The sequence of attempts is listed below, in order.
-
-        1. It uses ``ctypes.util.find_library`` to look for ``'sodium'`` or
-        ``'libsodium'``.
-
-        2. It attempts to find a file ``libsodium.so`` or ``libsodium.dll`` in
-           the paths specified by the ``PATH`` and ``LD_LIBRARY_PATH``
-           environment variables.
-
-        3. If the `rbcl <https://pypi.org/project/rbcl>`__ package is
-           installed, it reverts to the compiled subset of libsodium included
-           in that package.
-
-        If all of the above fail, then :obj:`sodium` is assigned the value
-        ``None`` and all classes exported by this module default to their
-        pure-Python variants (*i.e.*, those encapsulated within :obj:`python`).
-        To confirm that a dynamic/shared library *has been found* when this
-        module is imported, evaluate the expression ``sodium is not None``.
-
-        If a shared/dynamic library file has been loaded successfully, this
-        class encapsulates shared/dynamic library variants of both classes
-        exported by this module and of all the underlying low-level operations:
-        :obj:`sodium.scl <scl>`, :obj:`sodium.rnd <rnd>`,
-        :obj:`sodium.inv <inv>`, :obj:`sodium.smu <smu>`,
-        :obj:`sodium.pnt <pnt>`, :obj:`sodium.bas <bas>`,
-        :obj:`sodium.can <can>`, :obj:`sodium.mul <mul>`,
-        :obj:`sodium.add <add>`, :obj:`sodium.sub <sub>`,
-        :obj:`sodium.neg <neg>`,
-        :obj:`sodium.point <oblivious.ristretto.sodium.point>`, and
-        :obj:`sodium.scalar <oblivious.ristretto.sodium.scalar>`.
-        For example, you can perform addition of points using
-        the point addition implementation found in the libsodium
-        shared/dynamic library found on the host system.
-
-        >>> p = sodium.pnt()
-        >>> q = sodium.pnt()
-        >>> sodium.add(p, q) == sodium.add(q, p)
-        True
-
-        Methods found in the shared/dynamic library variants of the
-        :obj:`point` and :obj:`scalar` classes are wrappers for the
-        shared/dynamic library implementations of the underlying
-        operations.
-
-        >>> p = sodium.point()
-        >>> q = sodium.point()
-        >>> p + q == q + p
-        True
-
-        Nevertheless, all bytes-like objects, :obj:`point` objects, and
-        :obj:`scalar` objects accepted and emitted by the various operations
-        and class methods in :obj:`sodium` are compatible with those accepted
-        and emitted by the operations and class methods in :obj:`python`.
-        """
-        _lib = _sodium
-        _call_unwrapped = _call_variant_unwrapped
-        _call_wrapped = _call_variant_wrapped
-        _call = _call_variant
-
-        @staticmethod
-        def pnt(h: bytes = None) -> bytes:
-            """
-            Construct a point from its 64-byte vector representation (normally
-            obtained via hashing).
-
-            >>> p = sodium.pnt(hashlib.sha512('123'.encode()).digest())
-            >>> p.hex()
-            '047f39a6c6dd156531a25fa605f017d4bec13b0b6c42f0e9b641c8ee73359c5f'
-            """
-            return sodium._call(
-                sodium._lib.crypto_core_ristretto255_bytes(),
-                sodium._lib.crypto_core_ristretto255_from_hash,
-                bytes(
-                    hashlib.sha512(sodium.rnd()).digest() if h is None else h
-                )
-            )
-
-        @staticmethod
-        def bas(s: bytes) -> bytes:
-            """
-            Return the base point multiplied by the supplied scalar.
-
-            >>> sodium.bas(scalar.hash('123'.encode())).hex()
-            '4c207a5377f3badf358914f20b505cd1e2a6396720a9c240e5aff522e2446005'
-            """
-            return sodium._call(
-                sodium._lib.crypto_core_ristretto255_scalarbytes(),
-                sodium._lib.crypto_scalarmult_ristretto255_base_allow_scalar_zero,
-                bytes(s)
-            )
-
-        @staticmethod
-        def can(p: bytes) -> bytes:
-            """
-            Normalize the representation of a point into its canonical form.
-
-            >>> p = point.hash('123'.encode())
-            >>> sodium.can(p) == p
-            True
-            """
-            # In this module, the canonical representation is used at all times.
-            return p
-
-        @staticmethod
-        def mul(s: bytes, p: bytes) -> bytes:
-            """
-            Multiply a point by a scalar and return the result.
-
-            >>> p = sodium.pnt(hashlib.sha512('123'.encode()).digest())
-            >>> s = sodium.scl(bytes.fromhex(
-            ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-            ... ))
-            >>> sodium.mul(s, p).hex()
-            '183a06e0fe6af5d7913afb40baefc4dd52ae718fee77a3a0af8777c89fe16210'
-            """
-            return sodium._call(
-                sodium._lib.crypto_core_ristretto255_scalarbytes(),
-                sodium._lib.crypto_scalarmult_ristretto255_allow_scalar_zero,
-                bytes(s), bytes(p)
-            )
-
-        @staticmethod
-        def add(p: bytes, q: bytes) -> bytes:
-            """
-            Return the sum of the supplied points.
-
-            >>> p = point.hash('123'.encode())
-            >>> q = point.hash('456'.encode())
-            >>> sodium.add(p, q).hex()
-            '7076739c9df665d416e68b9512f5513bf1d0181a2aacefdeb1b7244528a4dd77'
-            """
-            return sodium._call(
-                sodium._lib.crypto_core_ristretto255_scalarbytes(),
-                sodium._lib.crypto_core_ristretto255_add,
-                bytes(p), bytes(q)
-            )
-
-        @staticmethod
-        def sub(p: bytes, q: bytes) -> bytes:
-            """
-            Return the result of subtracting the right-hand point from the
-            left-hand point.
-
-            >>> p = point.hash('123'.encode())
-            >>> q = point.hash('456'.encode())
-            >>> sodium.sub(p, q).hex()
-            '1a3199ca7debfe31a90171696d8bab91b99eb23a541b822a7061b09776e1046c'
-            """
-            return sodium._call(
-                _sodium.crypto_core_ristretto255_scalarbytes(),
-                sodium._lib.crypto_core_ristretto255_sub,
-                bytes(p), bytes(q)
-            )
-
-        @staticmethod
-        def neg(p: bytes) -> bytes:
-            """
-            Return the additive inverse of a point.
-
-            >>> p = point.hash('123'.encode())
-            >>> q = point.hash('456'.encode())
-            >>> sodium.add(sodium.neg(p), sodium.add(p, q)) == q
-            True
-            """
-            return sodium.sub(bytes(32), p)
-
-        @staticmethod
-        def rnd() -> bytes:
-            """
-            Return random non-zero scalar.
-
-            >>> len(sodium.rnd())
-            32
-            """
-            return sodium._call(
-                sodium._lib.crypto_core_ristretto255_scalarbytes(),
-                sodium._lib.crypto_core_ristretto255_scalar_random
-            )
-
-        @classmethod
-        def scl(cls, s: bytes = None) -> Optional[bytes]:
-            """
-            Return supplied byte vector if it is a valid scalar; otherwise,
-            return ``None``. If no byte vector is supplied, return a random
-            scalar.
-
-            >>> s = sodium.scl()
-            >>> t = sodium.scl(s)
-            >>> s == t
-            True
-            >>> sodium.scl(bytes([255] * 32)) is None
-            True
-            """
-            if s is None:
-                return cls.rnd()
-
-            s = bytearray(s)
-            s[-1] &= 0x1f
-
-            return bytes(s) if _sc25519_is_canonical(s) else None
-
-        @staticmethod
-        def inv(s: bytes) -> bytes:
-            """
-            Return the inverse of a scalar (modulo
-            ``2**252 + 27742317777372353535851937790883648493``).
-
-            >>> s = sodium.scl()
-            >>> p = sodium.pnt()
-            >>> sodium.mul(sodium.inv(s), sodium.mul(s, p)) == p
-            True
-            """
-            return sodium._call(
-                sodium._lib.crypto_core_ristretto255_scalarbytes(),
-                sodium._lib.crypto_core_ristretto255_scalar_invert,
-                bytes(s)
-            )
-
-        @staticmethod
-        def smu(s: bytes, t: bytes) -> bytes:
-            """
-            Return the product of two scalars.
-
-            >>> s = sodium.scl()
-            >>> t = sodium.scl()
-            >>> sodium.smu(s, t) == sodium.smu(t, s)
-            True
-            """
-            return sodium._call(
-                sodium._lib.crypto_core_ristretto255_scalarbytes(),
-                sodium._lib.crypto_core_ristretto255_scalar_mul,
-                bytes(s), bytes(t)
-            )
-
-except: # pylint: disable=W0702 # pragma: no cover
-    # Exported symbol.
-    sodium = None # pragma: no cover
-
-#
-# Dedicated point and scalar data structures derived from `bytes`.
-#
-
-for _implementation in [python] + ([sodium] if sodium is not None else []):
-    # pylint: disable=cell-var-from-loop
-    class point(bytes): # pylint: disable=E0102
-        """
-        Class for representing a point. Because this class is derived from
-        :obj:`bytes`, it inherits methods such as :obj:`bytes.hex` and
-        :obj:`bytes.fromhex`.
-
-        >>> len(point.random())
-        32
-        >>> p = point.hash('123'.encode())
-        >>> p.hex()
-        '047f39a6c6dd156531a25fa605f017d4bec13b0b6c42f0e9b641c8ee73359c5f'
-        >>> point.fromhex(p.hex()) == p
-        True
-        """
-        _implementation = _implementation
-
-        @classmethod
-        def random(cls) -> point:
-            """
-            Return random point object.
-
-            >>> len(point.random())
-            32
-            """
-            return bytes.__new__(cls, cls._implementation.pnt())
-
-        @classmethod
-        def bytes(cls, bs: bytes) -> point:
-            """
-            Return the point object obtained by transforming the supplied
-            bytes-like object.
-
-            >>> p = point.bytes(hashlib.sha512('123'.encode()).digest())
-            >>> p.hex()
-            '047f39a6c6dd156531a25fa605f017d4bec13b0b6c42f0e9b641c8ee73359c5f'
-            """
-            return bytes.__new__(cls, cls._implementation.pnt(bs))
-
-        @classmethod
-        def hash(cls, bs: bytes) -> point:
-            """
-            Return point object by hashing supplied bytes-like object.
-
-            >>> point.hash('123'.encode()).hex()
-            '047f39a6c6dd156531a25fa605f017d4bec13b0b6c42f0e9b641c8ee73359c5f'
-            """
-            return bytes.__new__(cls, cls._implementation.pnt(hashlib.sha512(bs).digest()))
-
-        @classmethod
-        def base(cls, s: scalar) -> Optional[point]:
-            """
-            Return base point multiplied by supplied scalar if the scalar is valid;
-            otherwise, return ``None``.
-
-            >>> point.base(scalar.hash('123'.encode())).hex()
-            '4c207a5377f3badf358914f20b505cd1e2a6396720a9c240e5aff522e2446005'
-
-            Use of the scalar corresponding to the zero residue is permitted.
-
-            >>> p = point()
-            >>> point.base(scalar.from_int(0)) + p == p
-            True
-            """
-            return bytes.__new__(cls, cls._implementation.bas(s))
-
-        @classmethod
-        def from_bytes(cls, bs: bytes) -> point:
-            """
-            Return the instance corresponding to the supplied bytes-like object.
-
-            >>> p = point.bytes(hashlib.sha512('123'.encode()).digest())
-            >>> p == point.from_bytes(p.to_bytes())
-            True
-            """
-            return bytes(bs)
-
-        @classmethod
-        def from_base64(cls, s: str) -> point:
-            """
-            Construct an instance from its Base64 UTF-8 string representation.
-
-            >>> point.from_base64('hoVaKq3oIlxEndP2Nqv3Rdbmiu4iinZE6Iwo+kcKAik=').hex()
-            '86855a2aade8225c449dd3f636abf745d6e68aee228a7644e88c28fa470a0229'
-            """
-            return bytes.__new__(cls, base64.standard_b64decode(s))
-
-        def __new__(cls, bs: bytes = None) -> point:
-            """
-            If a bytes-like object is supplied, return a point object
-            corresponding to the supplied bytes-like object (no checking
-            is performed to confirm that the bytes-like object is a valid
-            point). If no argument is supplied, return a random point
-            object.
-
-            >>> bs = bytes.fromhex(
-            ...     '86855a2aade8225c449dd3f636abf745d6e68aee228a7644e88c28fa470a0229'
-            ... )
-            >>> point(bs).hex()
-            '86855a2aade8225c449dd3f636abf745d6e68aee228a7644e88c28fa470a0229'
-            >>> len(point())
-            32
-            """
-            return bytes.__new__(cls, bs) if bs is not None else cls.random()
-
-        def canonical(self: point) -> point:
-            """
-            Normalize the representation of this instance into its canonical form.
-
-            >>> p = point.hash('123'.encode())
-            >>> p.canonical() == p
-            True
-            """
-            # In this module, the canonical representation is used at all times.
-            return self
-
-        def __mul__(self: point, other: Any) -> NoReturn:
-            """
-            A point cannot be a left-hand argument for a multiplication operation.
-
-            >>> point() * scalar()
-            Traceback (most recent call last):
-              ...
-            TypeError: point must be on right-hand side of multiplication operator
-            """
-            raise TypeError('point must be on right-hand side of multiplication operator')
-
-        def __rmul__(self: point, other: Any) -> NoReturn:
-            """
-            This functionality is implemented exclusively in the method
-            :obj:`scalar.__mul__`, as that method pre-empts this method
-            when the second argument has the correct type (*i.e.*, it is
-            a :obj:`scalar` instance). This method is included so that an
-            exception can be raised if an incorrect argument is supplied.
-
-            >>> p = point.hash('123'.encode())
-            >>> 2 * p
-            Traceback (most recent call last):
-              ...
-            TypeError: point can only be multiplied by a scalar
-            """
-            raise TypeError('point can only be multiplied by a scalar')
-
-        def __add__(self: point, other: point) -> Optional[point]:
-            """
-            Return the sum of this instance and another point.
-
-            >>> p = point.hash('123'.encode())
-            >>> q = point.hash('456'.encode())
-            >>> (p + q).hex()
-            '7076739c9df665d416e68b9512f5513bf1d0181a2aacefdeb1b7244528a4dd77'
-            >>> p + (q - q) == p
-            True
-            """
-            return self._implementation.point(self._implementation.add(self, other))
-
-        def __sub__(self: point, other: point) -> Optional[point]:
-            """
-            Return the result of subtracting another point from this instance.
-
-            >>> p = point.hash('123'.encode())
-            >>> q = point.hash('456'.encode())
-            >>> (p - q).hex()
-            '1a3199ca7debfe31a90171696d8bab91b99eb23a541b822a7061b09776e1046c'
-            >>> p - p == point.base(scalar.from_int(0))
-            True
-            """
-            return self._implementation.point(self._implementation.sub(self, other))
-
-        def __neg__(self: point) -> point:
-            """
-            Return the negation of this instance.
-
-            >>> p = point.hash('123'.encode())
-            >>> q = point.hash('456'.encode())
-            >>> ((p + q) + (-q)) == p
-            True
-            """
-            return (self - self) - self
-
-        def to_bytes(self: point) -> bytes:
-            """
-            Return the bytes-like object that represents this instance.
-
-            >>> p = point()
-            >>> p.to_bytes() == p
-            True
-            """
-            return bytes(self)
-
-        def to_base64(self: point) -> str:
-            """
-            Return the Base64 UTF-8 string representation of this instance.
-
-            >>> p = point.from_base64('hoVaKq3oIlxEndP2Nqv3Rdbmiu4iinZE6Iwo+kcKAik=')
-            >>> p.to_base64()
-            'hoVaKq3oIlxEndP2Nqv3Rdbmiu4iinZE6Iwo+kcKAik='
-            """
-            return base64.standard_b64encode(self).decode('utf-8')
-
-    class scalar(bytes):
-        """
-        Class for representing a scalar. Because this class is derived from
-        :obj:`bytes`, it inherits methods such as :obj:`bytes.hex` and
-        :obj:`bytes.fromhex`.
-
-        >>> len(scalar.random())
-        32
-        >>> s = scalar.hash('123'.encode())
-        >>> s.hex()
-        'a665a45920422f9d417e4867efdc4fb8a04a1f3fff1fa07e998e86f7f7a27a03'
-        >>> scalar.fromhex(s.hex()) == s
-        True
-        """
-        _implementation = _implementation
-
-        @classmethod
-        def random(cls) -> scalar:
-            """
-            Return random non-zero scalar object.
-
-            >>> len(scalar.random())
-            32
-            """
-            return bytes.__new__(cls, cls._implementation.rnd())
-
-        @classmethod
-        def bytes(cls, bs: bytes) -> Optional[scalar]:
-            """
-            Return scalar object obtained by transforming supplied bytes-like
-            object if it is possible to do; otherwise, return ``None``.
-
-            >>> s = python.scl()
-            >>> t = scalar.bytes(s)
-            >>> s.hex() == t.hex()
-            True
-            """
-            s = cls._implementation.scl(bs)
-            return bytes.__new__(cls, s) if s is not None else None
-
-        @classmethod
-        def hash(cls, bs: bytes) -> scalar:
-            """
-            Return scalar object by hashing supplied bytes-like object.
-
-            >>> scalar.hash('123'.encode()).hex()
-            'a665a45920422f9d417e4867efdc4fb8a04a1f3fff1fa07e998e86f7f7a27a03'
-            """
-            h = hashlib.sha256(bs).digest()
-            s = cls._implementation.scl(h)
-            while s is None:
-                h = hashlib.sha256(h).digest()
-                s = cls._implementation.scl(h)
-            return bytes.__new__(cls, s)
-
-        @classmethod
-        def from_int(cls, i: int) -> scalar:
-            """
-            Construct an instance from its integer (*i.e.*, residue) representation.
-
-            >>> p = point()
-            >>> zero = scalar.from_int(0)
-            >>> zero * p == p - p
-            True
-            >>> one = scalar.from_int(1)
-            >>> one * p == p
-            True
-            >>> two = scalar.from_int(2)
-            >>> two * p == p + p
-            True
-
-            Negative integers are supported (and automatically converted into their
-            corresponding least nonnegative residues).
-
-            >>> q = point()
-            >>> p - p == scalar.from_int(0) * p
-            True
-            >>> q - p - p == q + (scalar.from_int(-2) * p)
-            True
-            """
-            return bytes.__new__(
-                cls,
-                (
-                    i % (pow(2, 252) + 27742317777372353535851937790883648493)
-                ).to_bytes(32, 'little')
-            )
-
-        @classmethod
-        def from_bytes(cls, bs: bytes) -> Optional[scalar]:
-            """
-            Return the instance corresponding to the supplied bytes-like object.
-
-            >>> s = python.scl()
-            >>> t = scalar.from_bytes(s)
-            >>> s.hex() == t.hex()
-            True
-            """
-            return cls(bs)
-
-        @classmethod
-        def from_base64(cls, s: str) -> scalar:
-            """
-            Construct an instance from its Base64 UTF-8 string representation.
-
-            >>> scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=').hex()
-            '312d0c9130f69153bec9f5d0386a95135eb45eebf130af5f1fed1c6ed15f2500'
-            """
-            return bytes.__new__(cls, base64.standard_b64decode(s))
-
-        def __new__(cls, bs: bytes = None) -> scalar:
-            """
-            If a bytes-like object is supplied, return a scalar object
-            corresponding to the supplied bytes-like object (no checking
-            is performed to confirm that the bytes-like object is a valid
-            scalar). If no argument is supplied, return a random scalar
-            object.
-
-            >>> s = python.scl()
-            >>> t = scalar(s)
-            >>> s.hex() == t.hex()
-            True
-            >>> len(scalar())
-            32
-            """
-            return bytes.__new__(cls, bs) if bs is not None else cls.random()
-
-        def __invert__(self: scalar) -> scalar:
-            """
-            Return the inverse of this instance (modulo
-            ``2**252 + 27742317777372353535851937790883648493``).
-
-            >>> s = scalar()
-            >>> p = point()
-            >>> ((~s) * (s * p)) == p
-            True
-
-            The scalar corresponding to the zero residue cannot be inverted.
-
-            >>> ~scalar.from_int(0)
-            Traceback (most recent call last):
-              ...
-            ValueError: cannot invert scalar corresponding to zero
-            """
-            if _zero(self):
-                raise ValueError('cannot invert scalar corresponding to zero')
-
-            return self._implementation.scalar(self._implementation.inv(self))
-
-        def __mul__(self: scalar, other: Union[scalar, point]) -> Union[scalar, point]:
-            """
-            Multiply the supplied scalar or point by this instance.
-
-            >>> p = point.hash('123'.encode())
-            >>> s = scalar.hash('456'.encode())
-            >>> (s * p).hex()
-            'f61b377aa86050aaa88c90f4a4a0f1e36b0000cf46f6a34232c2f1da7a799f16'
-            >>> p = point.from_base64('hoVaKq3oIlxEndP2Nqv3Rdbmiu4iinZE6Iwo+kcKAik=')
-            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
-            >>> (s * s).hex()
-            'd4aecf034f60edc5cb32cdd5a4be6d069959aa9fd133c51c9dcfd960ee865e0f'
-            >>> isinstance(s * s, scalar)
-            True
-            >>> (s * p).hex()
-            '2208082412921a67f42ea399748190d2b889228372509f2f2d9929813d074e1b'
-            >>> isinstance(s * p, point)
-            True
-
-            Multiplying any point or scalar by the scalar corresponding to the
-            zero residue yields the point or scalar corresponding to zero.
-
-            >>> scalar.from_int(0) * point() == p - p
-            True
-            >>> scalar.from_int(0) * scalar() == scalar.from_int(0)
-            True
-
-            Any attempt to multiply a value or object of an incompatible type by this
-            instance raises an exception.
-
-            >>> s * 2
-            Traceback (most recent call last):
-              ...
-            TypeError: multiplication by a scalar is defined only for scalars and points
-            """
-            if (
-                isinstance(other, python.scalar) or
-                (sodium is not None and isinstance(other, sodium.scalar))
-            ):
-                return self._implementation.scalar(self._implementation.smu(self, other))
-
-            if (
-                isinstance(other, python.point) or
-                (sodium is not None and isinstance(other, sodium.point))
-            ):
-                return self._implementation.point(self._implementation.mul(self, other))
-
-            raise TypeError(
-                'multiplication by a scalar is defined only for scalars and points'
-            )
-
-        def __rmul__(self: scalar, other: Union[scalar, point]):
-            """
-            A scalar cannot be on the right-hand side of a non-scalar.
-
-            >>> point() * scalar()
-            Traceback (most recent call last):
-              ...
-            TypeError: point must be on right-hand side of multiplication operator
-            """
-            raise TypeError(
-                'scalar must be on left-hand side of multiplication operator'
-            )
-
-        def to_bytes(self: scalar) -> bytes:
-            """
-            Return the bytes-like object that represents this instance.
-
-            >>> s = scalar()
-            >>> s.to_bytes() == s
-            True
-            """
-            return bytes(self)
-
-        def __int__(self: scalar) ->  int:
-            """
-            Return the integer (*i.e.*, least nonnegative residue) representation
-            of this instance.
-
-            >>> s = scalar()
-            >>> int(s * (~s))
-            1
-            """
-            return int.from_bytes(self, 'little')
-
-        def to_int(self: scalar) ->  int:
-            """
-            Return the integer (*i.e.*, least nonnegative residue) representation
-            of this instance.
-
-            >>> s = scalar()
-            >>> (s * (~s)).to_int()
-            1
-            """
-            return int(self)
-
-        def to_base64(self: scalar) -> str:
-            """
-            Return the Base64 UTF-8 string representation of this instance.
-
-            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
-            >>> s.to_base64()
-            'MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA='
-            """
-            return base64.standard_b64encode(self).decode('utf-8')
-
-    # Encapsulate classes for this implementation, regardless of which are
-    # exported as the unqualified symbols.
-    _implementation.point = point
-    _implementation.scalar = scalar
-
-# Redefine top-level wrapper classes to ensure that they appear at the end of
-# the auto-generated documentation.
-python = python # pylint: disable=self-assigning-variable
-sodium = sodium # pylint: disable=self-assigning-variable
-
-if __name__ == '__main__':
-    doctest.testmod() # pragma: no cover
+"""
+.. module:: ristretto
+
+ristretto module
+================
+
+This module exports the classes :obj:`~oblivious.ristretto.point` and
+:obj:`~oblivious.ristretto.scalar` for representing points and scalars. It
+also exports the two wrapper classes/namespaces
+:obj:`~oblivious.ristretto.python` and :obj:`~oblivious.ristretto.sodium`
+that encapsulate pure-Python and shared/dynamic library variants of the
+above (respectively) and also include low-level operations that correspond
+more directly to the functions found in the underlying libraries.
+
+* Under all conditions, the wrapper class :obj:`~oblivious.ristretto.python`
+  is defined and encapsulates a pure-Python variant of every class exported
+  by this module as a whole. It also includes pure-Python variants of low-level
+  operations that correspond to functions found in the underlying libraries.
+
+* If a shared/dynamic library instance of the
+  `libsodium <https://doc.libsodium.org>`__ library is found on the system
+  (and successfully loaded at the time this module is imported) or the
+  optional `rbcl <https://pypi.org/project/rbcl>`__ package is installed,
+  then the wrapper class :obj:`~oblivious.ristretto.sodium` is defined.
+  Otherwise, the exported variable ``sodium`` is assigned ``None``.
+
+* If a dynamic/shared library instance is loaded, all classes exported by
+  this module correspond to the variants defined within
+  :obj:`~oblivious.ristretto.sodium`. Otherwise, they correspond to the
+  variants defined within :obj:`~oblivious.ristretto.python`.
+
+For most users, the classes :obj:`~oblivious.ristretto.point` and
+:obj:`~oblivious.ristretto.scalar` should be sufficient. When using the
+low-level operations that correspond to a specific implementation (*e.g.*,
+:obj:`oblivious.ristretto.sodium.add`), users are responsible for ensuring
+that inputs have the type and/or representation appropriate for that
+operation.
+"""
+from __future__ import annotations
+from typing import Any, NoReturn, Union, Optional
+import doctest
+import platform
+import os
+import hashlib
+import ctypes
+import ctypes.util
+import secrets
+import base64
+import ge25519
+
+#
+# Attempt to load rbcl. If no local libsodium shared/dynamic library file
+# is found, only pure-Python implementations of the functions and methods
+# will be available.
+#
+
+try: # pragma: no cover
+    import rbcl # pylint: disable=E0401
+
+    # Add synonyms to deal with variations in capitalization of function names.
+    setattr(
+        rbcl,
+        'crypto_core_ristretto255_scalarbytes',
+        lambda: rbcl.crypto_core_ristretto255_SCALARBYTES
+    )
+    setattr(
+        rbcl,
+        'crypto_core_ristretto255_bytes',
+        lambda: rbcl.crypto_core_ristretto255_BYTES
+    )
+except: # pylint: disable=W0702 # pragma: no cover
+    rbcl = None
+
+#
+# Use pure-Python implementations of primitives by default.
+#
+
+def _zero(n: bytes) -> bool:
+    d = 0
+    for b in n:
+        d |= b
+    return ((d - 1) >> 8) % 2 == 1
+
+_sc25519_is_canonical_L = [ # 2^252+27742317777372353535851937790883648493.
+    0xed, 0xd3, 0xf5, 0x5c, 0x1a, 0x63, 0x12, 0x58, 0xd6, 0x9c, 0xf7,
+    0xa2, 0xde, 0xf9, 0xde, 0x14, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
+    0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x10
+]
+
+def _sc25519_is_canonical(s: bytes) -> bool:
+    """
+    Confirm that the bytes-like object represents a canonical
+    scalar.
+    """
+    c = 0
+    n = 1
+    for i in range(31, -1, -1):
+        c |= ((s[i] - _sc25519_is_canonical_L[i]) >> 8) & n
+        n &= ((s[i] ^ _sc25519_is_canonical_L[i]) - 1) >> 8
+    return c != 0
+
+def _sc25519_mul(a: bytes, b: bytes) -> bytes:
+    """
+    Multiply the two scalars represented by the bytes-like objects
+    """
+    (a, b) = (int.from_bytes(a, 'little'), int.from_bytes(b, 'little'))
+    return (
+        (a * b) % (pow(2, 252) + 27742317777372353535851937790883648493)
+    ).to_bytes(32, 'little')
+
+def _sc25519_sqmul(s: bytes, n: int, a: bytes) -> bytes:
+    """
+    Perform repeated squaring of a scalar for the designated number
+    of iterations, then multiply the result by another scalar.
+    """
+    for _ in range(n):
+        s = _sc25519_mul(s, s)
+    return _sc25519_mul(s, a)
+
+def _sc25519_invert(s: bytes) -> bytes:
+    """
+    Invert the scalar represented by the bytes-like object.
+    """
+    b_10 = _sc25519_mul(s, s)
+    b_100 = _sc25519_mul(b_10, b_10)
+    b_11 = _sc25519_mul(b_10, s)
+    b_101 = _sc25519_mul(b_10, b_11)
+    b_111 = _sc25519_mul(b_10, b_101)
+    b_1001 = _sc25519_mul(b_10, b_111)
+    b_1011 = _sc25519_mul(b_10, b_1001)
+    b_1111 = _sc25519_mul(b_100, b_1011)
+    recip = _sc25519_mul(b_1111, s)
+
+    recip = _sc25519_sqmul(recip, 123 + 3, b_101)
+    recip = _sc25519_sqmul(recip, 2 + 2, b_11)
+    recip = _sc25519_sqmul(recip, 1 + 4, b_1111)
+    recip = _sc25519_sqmul(recip, 1 + 4, b_1111)
+    recip = _sc25519_sqmul(recip, 4, b_1001)
+    recip = _sc25519_sqmul(recip, 2, b_11)
+    recip = _sc25519_sqmul(recip, 1 + 4, b_1111)
+    recip = _sc25519_sqmul(recip, 1 + 3, b_101)
+    recip = _sc25519_sqmul(recip, 3 + 3, b_101)
+    recip = _sc25519_sqmul(recip, 3, b_111)
+    recip = _sc25519_sqmul(recip, 1 + 4, b_1111)
+    recip = _sc25519_sqmul(recip, 2 + 3, b_111)
+    recip = _sc25519_sqmul(recip, 2 + 2, b_11)
+    recip = _sc25519_sqmul(recip, 1 + 4, b_1011)
+    recip = _sc25519_sqmul(recip, 2 + 4, b_1011)
+    recip = _sc25519_sqmul(recip, 6 + 4, b_1001)
+    recip = _sc25519_sqmul(recip, 2 + 2, b_11)
+    recip = _sc25519_sqmul(recip, 3 + 2, b_11)
+    recip = _sc25519_sqmul(recip, 3 + 2, b_11)
+    recip = _sc25519_sqmul(recip, 1 + 4, b_1001)
+    recip = _sc25519_sqmul(recip, 1 + 3, b_111)
+    recip = _sc25519_sqmul(recip, 2 + 4, b_1111)
+    recip = _sc25519_sqmul(recip, 1 + 4, b_1011)
+    recip = _sc25519_sqmul(recip, 3, b_101)
+    recip = _sc25519_sqmul(recip, 2 + 4, b_1111)
+    recip = _sc25519_sqmul(recip, 3, b_101)
+    recip = _sc25519_sqmul(recip, 1 + 2, b_11)
+
+    return recip
+
+def _ristretto255_is_canonical(s: bytes) -> bool:
+    """
+    Confirm that the bytes-like object represents a canonical
+    Ristretto point.
+    """
+    c = ((s[31] & 0x7f) ^ 0x7f) % 256
+    for i in range(30, 0, -1):
+        c |= (s[i] ^ 0xff) % 256
+    c = (c - 1) >> 8
+    d = ((0xed - 1 - s[0]) >> 8) % 256
+    return (1 - (((c & d) | s[0]) & 1)) == 1
+
+class python:
+    """
+    Wrapper class for pure-Python implementations of primitive operations.
+
+    This class encapsulates pure-Python variants of all low-level operations
+    and of both classes exported by this module:
+    :obj:`python.scl <scl>`, :obj:`python.rnd <rnd>`,
+    :obj:`python.inv <inv>`, :obj:`python.smu <smu>`,
+    :obj:`python.pnt <pnt>`, :obj:`python.bas <bas>`,
+    :obj:`python.can <can>`, :obj:`python.mul <mul>`,
+    :obj:`python.add <add>`, :obj:`python.sub <sub>`,
+    :obj:`python.neg <neg>`,
+    :obj:`python.point <oblivious.ristretto.python.point>`, and
+    :obj:`python.scalar <oblivious.ristretto.python.scalar>`.
+    For example, you can perform addition of points using
+    the pure-Python point addition implementation.
+
+    >>> p = python.pnt()
+    >>> q = python.pnt()
+    >>> python.add(p, q) == python.add(q, p)
+    True
+
+    Pure-Python variants of the :obj:`python.point <point>` and
+    :obj:`python.scalar <scalar>` classes always employ pure-Python
+    implementations of operations when their methods are invoked.
+
+    >>> p = python.point()
+    >>> q = python.point()
+    >>> p + q == q + p
+    True
+
+    Nevertheless, all bytes-like objects, :obj:`point` objects, and
+    :obj:`scalar` objects accepted and emitted by the various operations and
+    class methods in :obj:`python` are compatible with those accepted and
+    emitted by the operations and class methods in :obj:`sodium`.
+    """
+    @staticmethod
+    def pnt(h: bytes = None) -> bytes:
+        """
+        Return point from 64-byte vector (normally obtained via hashing).
+
+        >>> p = python.pnt(hashlib.sha512('123'.encode()).digest())
+        >>> p.hex()
+        '047f39a6c6dd156531a25fa605f017d4bec13b0b6c42f0e9b641c8ee73359c5f'
+        """
+        return ge25519.ge25519_p3.from_hash_ristretto255(
+            hashlib.sha512(python.rnd()).digest() if h is None else h
+        )
+
+    @staticmethod
+    def bas(s: bytes) -> bytes:
+        """
+        Return base point multiplied by supplied scalar.
+
+        >>> python.bas(scalar.hash('123'.encode())).hex()
+        '4c207a5377f3badf358914f20b505cd1e2a6396720a9c240e5aff522e2446005'
+        """
+        t = bytearray(s)
+        t[31] &= 127
+
+        return ge25519.ge25519_p3.scalar_mult_base(t).to_bytes_ristretto255()
+
+    @staticmethod
+    def can(p: bytes) -> bytes:
+        """
+        Normalize the representation of a point into its canonical form.
+
+        >>> p = point.hash('123'.encode())
+        >>> python.can(p) == p
+        True
+        """
+        return p # In this module, the canonical representation is used at all times.
+
+    @staticmethod
+    def mul(s: bytes, p: bytes) -> bytes:
+        """
+        Multiply the point by the supplied scalar and return the result.
+
+        >>> p = python.pnt(hashlib.sha512('123'.encode()).digest())
+        >>> s = python.scl(bytes.fromhex(
+        ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+        ... ))
+        >>> python.mul(s, p).hex()
+        '183a06e0fe6af5d7913afb40baefc4dd52ae718fee77a3a0af8777c89fe16210'
+        """
+        p3 = ge25519.ge25519_p3.from_bytes_ristretto255(p)
+        if not _ristretto255_is_canonical(p) or p3 is None:
+            return bytes(32) # pragma: no cover
+
+        t = bytearray(s)
+        t[31] &= 127
+
+        return p3.scalar_mult(t).to_bytes_ristretto255()
+
+    @staticmethod
+    def add(p: bytes, q: bytes) -> bytes:
+        """
+        Return sum of the supplied points.
+
+        >>> p = point.hash('123'.encode())
+        >>> q = point.hash('456'.encode())
+        >>> python.add(p, q).hex()
+        '7076739c9df665d416e68b9512f5513bf1d0181a2aacefdeb1b7244528a4dd77'
+        """
+        p_p3 = ge25519.ge25519_p3.from_bytes_ristretto255(p)
+        q_p3 = ge25519.ge25519_p3.from_bytes_ristretto255(q)
+        if (
+            not _ristretto255_is_canonical(p) or p_p3 is None or
+            not _ristretto255_is_canonical(q) or q_p3 is None
+        ):
+            return bytes(32) # pragma: no cover
+
+        q_cached = ge25519.ge25519_cached.from_p3(q_p3)
+        r_p1p1 = ge25519.ge25519_p1p1.add(p_p3, q_cached)
+        r_p3 = ge25519.ge25519_p3.from_p1p1(r_p1p1)
+        return r_p3.to_bytes_ristretto255()
+
+    @staticmethod
+    def sub(p: bytes, q: bytes) -> bytes:
+        """
+        Return result of subtracting second point from first point.
+
+        >>> p = point.hash('123'.encode())
+        >>> q = point.hash('456'.encode())
+        >>> python.sub(p, q).hex()
+        '1a3199ca7debfe31a90171696d8bab91b99eb23a541b822a7061b09776e1046c'
+        """
+        p_p3 = ge25519.ge25519_p3.from_bytes_ristretto255(p)
+        q_p3 = ge25519.ge25519_p3.from_bytes_ristretto255(q)
+        if (
+            not _ristretto255_is_canonical(p) or p_p3 is None or
+            not _ristretto255_is_canonical(q) or q_p3 is None
+        ):
+            return bytes(32) # pragma: no cover
+
+        q_cached = ge25519.ge25519_cached.from_p3(q_p3)
+        r_p1p1 = ge25519.ge25519_p1p1.sub(p_p3, q_cached)
+        r_p3 = ge25519.ge25519_p3.from_p1p1(r_p1p1)
+        return r_p3.to_bytes_ristretto255()
+
+    @staticmethod
+    def neg(p: bytes) -> bytes:
+        """
+        Return the additive inverse of a point.
+
+        >>> p = point.hash('123'.encode())
+        >>> q = point.hash('456'.encode())
+        >>> python.add(python.neg(p), python.add(p, q)) == q
+        True
+        """
+        return python.sub(bytes(32), p)
+
+    @staticmethod
+    def rnd() -> bytes:
+        """
+        Return random non-zero scalar.
+
+        >>> len(python.rnd())
+        32
+        """
+        while True:
+            r = bytearray(secrets.token_bytes(32))
+            r[-1] &= 0x1f
+            if _sc25519_is_canonical(r) and not _zero(r):
+                return r
+
+    @classmethod
+    def scl(cls, s: bytes = None) -> Optional[bytes]:
+        """
+        Return supplied byte vector if it is a valid scalar; otherwise, return
+        ``None``. If no byte vector is supplied, return a random scalar.
+
+        >>> s = python.scl()
+        >>> t = python.scl(s)
+        >>> s == t
+        True
+        >>> python.scl(bytes([255] * 32)) is None
+        True
+        """
+        if s is None:
+            return cls.rnd()
+
+        s = bytearray(s)
+        s[-1] &= 0x1f
+
+        return bytes(s) if _sc25519_is_canonical(s) else None
+
+    @staticmethod
+    def inv(s: bytes) -> bytes:
+        """
+        Return the inverse of a scalar (modulo
+        ``2**252 + 27742317777372353535851937790883648493``).
+
+        >>> s = python.scl()
+        >>> p = python.pnt()
+        >>> python.mul(python.inv(s), python.mul(s, p)) == p
+        True
+        """
+        return _sc25519_invert(s)
+
+    @staticmethod
+    def smu(s: bytes, t: bytes) -> bytes:
+        """
+        Return scalar multiplied by another scalar.
+
+        >>> s = python.scl()
+        >>> t = python.scl()
+        >>> python.smu(s, t) == python.smu(t, s)
+        True
+        """
+        return _sc25519_mul(s, t)
+
+#
+# Attempt to load primitives from libsodium, if it is present;
+# otherwise, use the rbcl library, if it is present. Otherwise,
+# silently assign ``None`` to ``sodium``.
+#
+
+try:
+    def _call_variant_unwrapped(length, function, x=None, y=None):
+        """
+        Wrapper to invoke external function.
+        """
+        buf = ctypes.create_string_buffer(length)
+        if y is not None:
+            function(buf, x, y)
+        elif x is not None:
+            function(buf, x)
+        else:
+            function(buf)
+        return buf.raw
+
+    def _call_variant_wrapped(_, function, x=None, y=None): # pragma: no cover
+        """
+        Wrapper to invoke external (wrapped) function.
+        """
+        if y is not None:
+            return function(x, y)
+        if x is not None:
+            return function(x)
+        return function()
+
+    _sodium = None
+    _call_variant = _call_variant_unwrapped
+
+    # Attempt to load libsodium shared/dynamic library file.
+    xdll = ctypes.cdll if platform.system() != 'Windows' else ctypes.windll
+    libf = ctypes.util.find_library('sodium') or ctypes.util.find_library('libsodium')
+    if libf is not None:
+        _sodium = xdll.LoadLibrary(libf)
+    else: # pragma: no cover
+        # Perform explicit search in case `ld` is not present in environment.
+        libf = 'libsodium.so' if platform.system() != 'Windows' else 'libsodium.dll'
+        for var in ['PATH', 'LD_LIBRARY_PATH']:
+            if var in os.environ:
+                for path in os.environ[var].split(os.pathsep):
+                    try:
+                        _sodium = ctypes.cdll.LoadLibrary(path + os.path.sep + libf)
+                        break
+                    except: # pylint: disable=W0702
+                        continue
+
+        # Default to bindings exported by the rbcl library if the above attempts
+        # failed and rbcl is available.
+        if _sodium is None and rbcl is not None: # pragma: no cover
+            _sodium = rbcl
+            _call_variant = _call_variant_wrapped
+
+    # Add method variants that are not present in libsodium.
+    if _sodium is not rbcl and _sodium is not None: # pragma: no cover
+
+        def _crypto_scalarmult_ristretto255_allow_scalar_zero(buf, s, p):
+            """
+            Variant of scalar-point multiplication function that permits
+            a scalar corresponding to the zero residue.
+            """
+            r = _sodium.crypto_scalarmult_ristretto255(buf, s, p)
+
+            if (1 - _zero(s)) * int(r == -1):
+                raise RuntimeError('libsodium error (possibly due to invalid input)')
+
+            return buf
+
+        def _crypto_scalarmult_ristretto255_base_allow_scalar_zero(buf, s):
+            """
+            Variant of scalar-point multiplication function that permits
+            a scalar corresponding to the zero residue.
+            """
+            r = _sodium.crypto_scalarmult_ristretto255_base(buf, s)
+
+            if (1 - _zero(s)) * int(r == -1):
+                raise RuntimeError('libsodium error (possibly due to invalid input)')
+
+            return buf
+
+        setattr(
+            _sodium,
+            'crypto_scalarmult_ristretto255_allow_scalar_zero',
+            _crypto_scalarmult_ristretto255_allow_scalar_zero
+        )
+        setattr(
+            _sodium,
+            'crypto_scalarmult_ristretto255_base_allow_scalar_zero',
+            _crypto_scalarmult_ristretto255_base_allow_scalar_zero
+        )
+
+    # Ensure the chosen version of libsodium (or its substitute) has the
+    # necessary primitives.
+    assert hasattr(_sodium, 'crypto_core_ristretto255_bytes')
+    assert hasattr(_sodium, 'crypto_core_ristretto255_scalarbytes')
+    assert hasattr(_sodium, 'crypto_core_ristretto255_scalar_random')
+    assert hasattr(_sodium, 'crypto_core_ristretto255_scalar_invert')
+    assert hasattr(_sodium, 'crypto_core_ristretto255_scalar_mul')
+    assert hasattr(_sodium, 'crypto_core_ristretto255_from_hash')
+    assert hasattr(_sodium, 'crypto_scalarmult_ristretto255_base')
+    assert hasattr(_sodium, 'crypto_scalarmult_ristretto255')
+    assert hasattr(_sodium, 'crypto_core_ristretto255_add')
+    assert hasattr(_sodium, 'crypto_core_ristretto255_sub')
+
+    # Exported symbol.
+    class sodium:
+        """
+        Wrapper class for binary implementations of primitive operations.
+
+        When this module is imported, it makes a number of attempts to
+        locate an instance of the shared/dynamic library file of the
+        `libsodium <https://doc.libsodium.org>`__ library on the host
+        system. The sequence of attempts is listed below, in order.
+
+        1. It uses ``ctypes.util.find_library`` to look for ``'sodium'`` or
+        ``'libsodium'``.
+
+        2. It attempts to find a file ``libsodium.so`` or ``libsodium.dll`` in
+           the paths specified by the ``PATH`` and ``LD_LIBRARY_PATH``
+           environment variables.
+
+        3. If the `rbcl <https://pypi.org/project/rbcl>`__ package is
+           installed, it reverts to the compiled subset of libsodium included
+           in that package.
+
+        If all of the above fail, then :obj:`sodium` is assigned the value
+        ``None`` and all classes exported by this module default to their
+        pure-Python variants (*i.e.*, those encapsulated within :obj:`python`).
+        To confirm that a dynamic/shared library *has been found* when this
+        module is imported, evaluate the expression ``sodium is not None``.
+
+        If a shared/dynamic library file has been loaded successfully, this
+        class encapsulates shared/dynamic library variants of both classes
+        exported by this module and of all the underlying low-level operations:
+        :obj:`sodium.scl <scl>`, :obj:`sodium.rnd <rnd>`,
+        :obj:`sodium.inv <inv>`, :obj:`sodium.smu <smu>`,
+        :obj:`sodium.pnt <pnt>`, :obj:`sodium.bas <bas>`,
+        :obj:`sodium.can <can>`, :obj:`sodium.mul <mul>`,
+        :obj:`sodium.add <add>`, :obj:`sodium.sub <sub>`,
+        :obj:`sodium.neg <neg>`,
+        :obj:`sodium.point <oblivious.ristretto.sodium.point>`, and
+        :obj:`sodium.scalar <oblivious.ristretto.sodium.scalar>`.
+        For example, you can perform addition of points using
+        the point addition implementation found in the libsodium
+        shared/dynamic library found on the host system.
+
+        >>> p = sodium.pnt()
+        >>> q = sodium.pnt()
+        >>> sodium.add(p, q) == sodium.add(q, p)
+        True
+
+        Methods found in the shared/dynamic library variants of the
+        :obj:`point` and :obj:`scalar` classes are wrappers for the
+        shared/dynamic library implementations of the underlying
+        operations.
+
+        >>> p = sodium.point()
+        >>> q = sodium.point()
+        >>> p + q == q + p
+        True
+
+        Nevertheless, all bytes-like objects, :obj:`point` objects, and
+        :obj:`scalar` objects accepted and emitted by the various operations
+        and class methods in :obj:`sodium` are compatible with those accepted
+        and emitted by the operations and class methods in :obj:`python`.
+        """
+        _lib = _sodium
+        _call_unwrapped = _call_variant_unwrapped
+        _call_wrapped = _call_variant_wrapped
+        _call = _call_variant
+
+        @staticmethod
+        def pnt(h: bytes = None) -> bytes:
+            """
+            Construct a point from its 64-byte vector representation (normally
+            obtained via hashing).
+
+            >>> p = sodium.pnt(hashlib.sha512('123'.encode()).digest())
+            >>> p.hex()
+            '047f39a6c6dd156531a25fa605f017d4bec13b0b6c42f0e9b641c8ee73359c5f'
+            """
+            return sodium._call(
+                sodium._lib.crypto_core_ristretto255_bytes(),
+                sodium._lib.crypto_core_ristretto255_from_hash,
+                bytes(
+                    hashlib.sha512(sodium.rnd()).digest() if h is None else h
+                )
+            )
+
+        @staticmethod
+        def bas(s: bytes) -> bytes:
+            """
+            Return the base point multiplied by the supplied scalar.
+
+            >>> sodium.bas(scalar.hash('123'.encode())).hex()
+            '4c207a5377f3badf358914f20b505cd1e2a6396720a9c240e5aff522e2446005'
+            """
+            return sodium._call(
+                sodium._lib.crypto_core_ristretto255_scalarbytes(),
+                sodium._lib.crypto_scalarmult_ristretto255_base_allow_scalar_zero,
+                bytes(s)
+            )
+
+        @staticmethod
+        def can(p: bytes) -> bytes:
+            """
+            Normalize the representation of a point into its canonical form.
+
+            >>> p = point.hash('123'.encode())
+            >>> sodium.can(p) == p
+            True
+            """
+            # In this module, the canonical representation is used at all times.
+            return p
+
+        @staticmethod
+        def mul(s: bytes, p: bytes) -> bytes:
+            """
+            Multiply a point by a scalar and return the result.
+
+            >>> p = sodium.pnt(hashlib.sha512('123'.encode()).digest())
+            >>> s = sodium.scl(bytes.fromhex(
+            ...     '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+            ... ))
+            >>> sodium.mul(s, p).hex()
+            '183a06e0fe6af5d7913afb40baefc4dd52ae718fee77a3a0af8777c89fe16210'
+            """
+            return sodium._call(
+                sodium._lib.crypto_core_ristretto255_scalarbytes(),
+                sodium._lib.crypto_scalarmult_ristretto255_allow_scalar_zero,
+                bytes(s), bytes(p)
+            )
+
+        @staticmethod
+        def add(p: bytes, q: bytes) -> bytes:
+            """
+            Return the sum of the supplied points.
+
+            >>> p = point.hash('123'.encode())
+            >>> q = point.hash('456'.encode())
+            >>> sodium.add(p, q).hex()
+            '7076739c9df665d416e68b9512f5513bf1d0181a2aacefdeb1b7244528a4dd77'
+            """
+            return sodium._call(
+                sodium._lib.crypto_core_ristretto255_scalarbytes(),
+                sodium._lib.crypto_core_ristretto255_add,
+                bytes(p), bytes(q)
+            )
+
+        @staticmethod
+        def sub(p: bytes, q: bytes) -> bytes:
+            """
+            Return the result of subtracting the right-hand point from the
+            left-hand point.
+
+            >>> p = point.hash('123'.encode())
+            >>> q = point.hash('456'.encode())
+            >>> sodium.sub(p, q).hex()
+            '1a3199ca7debfe31a90171696d8bab91b99eb23a541b822a7061b09776e1046c'
+            """
+            return sodium._call(
+                _sodium.crypto_core_ristretto255_scalarbytes(),
+                sodium._lib.crypto_core_ristretto255_sub,
+                bytes(p), bytes(q)
+            )
+
+        @staticmethod
+        def neg(p: bytes) -> bytes:
+            """
+            Return the additive inverse of a point.
+
+            >>> p = point.hash('123'.encode())
+            >>> q = point.hash('456'.encode())
+            >>> sodium.add(sodium.neg(p), sodium.add(p, q)) == q
+            True
+            """
+            return sodium.sub(bytes(32), p)
+
+        @staticmethod
+        def rnd() -> bytes:
+            """
+            Return random non-zero scalar.
+
+            >>> len(sodium.rnd())
+            32
+            """
+            return sodium._call(
+                sodium._lib.crypto_core_ristretto255_scalarbytes(),
+                sodium._lib.crypto_core_ristretto255_scalar_random
+            )
+
+        @classmethod
+        def scl(cls, s: bytes = None) -> Optional[bytes]:
+            """
+            Return supplied byte vector if it is a valid scalar; otherwise,
+            return ``None``. If no byte vector is supplied, return a random
+            scalar.
+
+            >>> s = sodium.scl()
+            >>> t = sodium.scl(s)
+            >>> s == t
+            True
+            >>> sodium.scl(bytes([255] * 32)) is None
+            True
+            """
+            if s is None:
+                return cls.rnd()
+
+            s = bytearray(s)
+            s[-1] &= 0x1f
+
+            return bytes(s) if _sc25519_is_canonical(s) else None
+
+        @staticmethod
+        def inv(s: bytes) -> bytes:
+            """
+            Return the inverse of a scalar (modulo
+            ``2**252 + 27742317777372353535851937790883648493``).
+
+            >>> s = sodium.scl()
+            >>> p = sodium.pnt()
+            >>> sodium.mul(sodium.inv(s), sodium.mul(s, p)) == p
+            True
+            """
+            return sodium._call(
+                sodium._lib.crypto_core_ristretto255_scalarbytes(),
+                sodium._lib.crypto_core_ristretto255_scalar_invert,
+                bytes(s)
+            )
+
+        @staticmethod
+        def smu(s: bytes, t: bytes) -> bytes:
+            """
+            Return the product of two scalars.
+
+            >>> s = sodium.scl()
+            >>> t = sodium.scl()
+            >>> sodium.smu(s, t) == sodium.smu(t, s)
+            True
+            """
+            return sodium._call(
+                sodium._lib.crypto_core_ristretto255_scalarbytes(),
+                sodium._lib.crypto_core_ristretto255_scalar_mul,
+                bytes(s), bytes(t)
+            )
+
+except: # pylint: disable=W0702 # pragma: no cover
+    # Exported symbol.
+    sodium = None # pragma: no cover
+
+#
+# Dedicated point and scalar data structures derived from `bytes`.
+#
+
+for _implementation in [python] + ([sodium] if sodium is not None else []):
+    # pylint: disable=cell-var-from-loop
+    class point(bytes): # pylint: disable=E0102
+        """
+        Class for representing a point. Because this class is derived from
+        :obj:`bytes`, it inherits methods such as :obj:`bytes.hex` and
+        :obj:`bytes.fromhex`.
+
+        >>> len(point.random())
+        32
+        >>> p = point.hash('123'.encode())
+        >>> p.hex()
+        '047f39a6c6dd156531a25fa605f017d4bec13b0b6c42f0e9b641c8ee73359c5f'
+        >>> point.fromhex(p.hex()) == p
+        True
+        """
+        _implementation = _implementation
+
+        @classmethod
+        def random(cls) -> point:
+            """
+            Return random point object.
+
+            >>> len(point.random())
+            32
+            """
+            return bytes.__new__(cls, cls._implementation.pnt())
+
+        @classmethod
+        def bytes(cls, bs: bytes) -> point:
+            """
+            Return the point object obtained by transforming the supplied
+            bytes-like object.
+
+            >>> p = point.bytes(hashlib.sha512('123'.encode()).digest())
+            >>> p.hex()
+            '047f39a6c6dd156531a25fa605f017d4bec13b0b6c42f0e9b641c8ee73359c5f'
+            """
+            return bytes.__new__(cls, cls._implementation.pnt(bs))
+
+        @classmethod
+        def hash(cls, bs: bytes) -> point:
+            """
+            Return point object by hashing supplied bytes-like object.
+
+            >>> point.hash('123'.encode()).hex()
+            '047f39a6c6dd156531a25fa605f017d4bec13b0b6c42f0e9b641c8ee73359c5f'
+            """
+            return bytes.__new__(cls, cls._implementation.pnt(hashlib.sha512(bs).digest()))
+
+        @classmethod
+        def base(cls, s: scalar) -> Optional[point]:
+            """
+            Return base point multiplied by supplied scalar if the scalar is valid;
+            otherwise, return ``None``.
+
+            >>> point.base(scalar.hash('123'.encode())).hex()
+            '4c207a5377f3badf358914f20b505cd1e2a6396720a9c240e5aff522e2446005'
+
+            Use of the scalar corresponding to the zero residue is permitted.
+
+            >>> p = point()
+            >>> point.base(scalar.from_int(0)) + p == p
+            True
+            """
+            return bytes.__new__(cls, cls._implementation.bas(s))
+
+        @classmethod
+        def from_bytes(cls, bs: bytes) -> point:
+            """
+            Return the instance corresponding to the supplied bytes-like object.
+
+            >>> p = point.bytes(hashlib.sha512('123'.encode()).digest())
+            >>> p == point.from_bytes(p.to_bytes())
+            True
+            """
+            return bytes(bs)
+
+        @classmethod
+        def from_base64(cls, s: str) -> point:
+            """
+            Construct an instance from its Base64 UTF-8 string representation.
+
+            >>> point.from_base64('hoVaKq3oIlxEndP2Nqv3Rdbmiu4iinZE6Iwo+kcKAik=').hex()
+            '86855a2aade8225c449dd3f636abf745d6e68aee228a7644e88c28fa470a0229'
+            """
+            return bytes.__new__(cls, base64.standard_b64decode(s))
+
+        def __new__(cls, bs: bytes = None) -> point:
+            """
+            If a bytes-like object is supplied, return a point object
+            corresponding to the supplied bytes-like object (no checking
+            is performed to confirm that the bytes-like object is a valid
+            point). If no argument is supplied, return a random point
+            object.
+
+            >>> bs = bytes.fromhex(
+            ...     '86855a2aade8225c449dd3f636abf745d6e68aee228a7644e88c28fa470a0229'
+            ... )
+            >>> point(bs).hex()
+            '86855a2aade8225c449dd3f636abf745d6e68aee228a7644e88c28fa470a0229'
+            >>> len(point())
+            32
+            """
+            return bytes.__new__(cls, bs) if bs is not None else cls.random()
+
+        def canonical(self: point) -> point:
+            """
+            Normalize the representation of this instance into its canonical form.
+
+            >>> p = point.hash('123'.encode())
+            >>> p.canonical() == p
+            True
+            """
+            # In this module, the canonical representation is used at all times.
+            return self
+
+        def __mul__(self: point, other: Any) -> NoReturn:
+            """
+            A point cannot be a left-hand argument for a multiplication operation.
+
+            >>> point() * scalar()
+            Traceback (most recent call last):
+              ...
+            TypeError: point must be on right-hand side of multiplication operator
+            """
+            raise TypeError('point must be on right-hand side of multiplication operator')
+
+        def __rmul__(self: point, other: Any) -> NoReturn:
+            """
+            This functionality is implemented exclusively in the method
+            :obj:`scalar.__mul__`, as that method pre-empts this method
+            when the second argument has the correct type (*i.e.*, it is
+            a :obj:`scalar` instance). This method is included so that an
+            exception can be raised if an incorrect argument is supplied.
+
+            >>> p = point.hash('123'.encode())
+            >>> 2 * p
+            Traceback (most recent call last):
+              ...
+            TypeError: point can only be multiplied by a scalar
+            """
+            raise TypeError('point can only be multiplied by a scalar')
+
+        def __add__(self: point, other: point) -> Optional[point]:
+            """
+            Return the sum of this instance and another point.
+
+            >>> p = point.hash('123'.encode())
+            >>> q = point.hash('456'.encode())
+            >>> (p + q).hex()
+            '7076739c9df665d416e68b9512f5513bf1d0181a2aacefdeb1b7244528a4dd77'
+            >>> p + (q - q) == p
+            True
+            """
+            return self._implementation.point(self._implementation.add(self, other))
+
+        def __sub__(self: point, other: point) -> Optional[point]:
+            """
+            Return the result of subtracting another point from this instance.
+
+            >>> p = point.hash('123'.encode())
+            >>> q = point.hash('456'.encode())
+            >>> (p - q).hex()
+            '1a3199ca7debfe31a90171696d8bab91b99eb23a541b822a7061b09776e1046c'
+            >>> p - p == point.base(scalar.from_int(0))
+            True
+            """
+            return self._implementation.point(self._implementation.sub(self, other))
+
+        def __neg__(self: point) -> point:
+            """
+            Return the negation of this instance.
+
+            >>> p = point.hash('123'.encode())
+            >>> q = point.hash('456'.encode())
+            >>> ((p + q) + (-q)) == p
+            True
+            """
+            return (self - self) - self
+
+        def to_bytes(self: point) -> bytes:
+            """
+            Return the bytes-like object that represents this instance.
+
+            >>> p = point()
+            >>> p.to_bytes() == p
+            True
+            """
+            return bytes(self)
+
+        def to_base64(self: point) -> str:
+            """
+            Return the Base64 UTF-8 string representation of this instance.
+
+            >>> p = point.from_base64('hoVaKq3oIlxEndP2Nqv3Rdbmiu4iinZE6Iwo+kcKAik=')
+            >>> p.to_base64()
+            'hoVaKq3oIlxEndP2Nqv3Rdbmiu4iinZE6Iwo+kcKAik='
+            """
+            return base64.standard_b64encode(self).decode('utf-8')
+
+    class scalar(bytes):
+        """
+        Class for representing a scalar. Because this class is derived from
+        :obj:`bytes`, it inherits methods such as :obj:`bytes.hex` and
+        :obj:`bytes.fromhex`.
+
+        >>> len(scalar.random())
+        32
+        >>> s = scalar.hash('123'.encode())
+        >>> s.hex()
+        'a665a45920422f9d417e4867efdc4fb8a04a1f3fff1fa07e998e86f7f7a27a03'
+        >>> scalar.fromhex(s.hex()) == s
+        True
+        """
+        _implementation = _implementation
+
+        @classmethod
+        def random(cls) -> scalar:
+            """
+            Return random non-zero scalar object.
+
+            >>> len(scalar.random())
+            32
+            """
+            return bytes.__new__(cls, cls._implementation.rnd())
+
+        @classmethod
+        def bytes(cls, bs: bytes) -> Optional[scalar]:
+            """
+            Return scalar object obtained by transforming supplied bytes-like
+            object if it is possible to do; otherwise, return ``None``.
+
+            >>> s = python.scl()
+            >>> t = scalar.bytes(s)
+            >>> s.hex() == t.hex()
+            True
+            """
+            s = cls._implementation.scl(bs)
+            return bytes.__new__(cls, s) if s is not None else None
+
+        @classmethod
+        def hash(cls, bs: bytes) -> scalar:
+            """
+            Return scalar object by hashing supplied bytes-like object.
+
+            >>> scalar.hash('123'.encode()).hex()
+            'a665a45920422f9d417e4867efdc4fb8a04a1f3fff1fa07e998e86f7f7a27a03'
+            """
+            h = hashlib.sha256(bs).digest()
+            s = cls._implementation.scl(h)
+            while s is None:
+                h = hashlib.sha256(h).digest()
+                s = cls._implementation.scl(h)
+            return bytes.__new__(cls, s)
+
+        @classmethod
+        def from_int(cls, i: int) -> scalar:
+            """
+            Construct an instance from its integer (*i.e.*, residue) representation.
+
+            >>> p = point()
+            >>> zero = scalar.from_int(0)
+            >>> zero * p == p - p
+            True
+            >>> one = scalar.from_int(1)
+            >>> one * p == p
+            True
+            >>> two = scalar.from_int(2)
+            >>> two * p == p + p
+            True
+
+            Negative integers are supported (and automatically converted into their
+            corresponding least nonnegative residues).
+
+            >>> q = point()
+            >>> p - p == scalar.from_int(0) * p
+            True
+            >>> q - p - p == q + (scalar.from_int(-2) * p)
+            True
+            """
+            return bytes.__new__(
+                cls,
+                (
+                    i % (pow(2, 252) + 27742317777372353535851937790883648493)
+                ).to_bytes(32, 'little')
+            )
+
+        @classmethod
+        def from_bytes(cls, bs: bytes) -> Optional[scalar]:
+            """
+            Return the instance corresponding to the supplied bytes-like object.
+
+            >>> s = python.scl()
+            >>> t = scalar.from_bytes(s)
+            >>> s.hex() == t.hex()
+            True
+            """
+            return cls(bs)
+
+        @classmethod
+        def from_base64(cls, s: str) -> scalar:
+            """
+            Construct an instance from its Base64 UTF-8 string representation.
+
+            >>> scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=').hex()
+            '312d0c9130f69153bec9f5d0386a95135eb45eebf130af5f1fed1c6ed15f2500'
+            """
+            return bytes.__new__(cls, base64.standard_b64decode(s))
+
+        def __new__(cls, bs: bytes = None) -> scalar:
+            """
+            If a bytes-like object is supplied, return a scalar object
+            corresponding to the supplied bytes-like object (no checking
+            is performed to confirm that the bytes-like object is a valid
+            scalar). If no argument is supplied, return a random scalar
+            object.
+
+            >>> s = python.scl()
+            >>> t = scalar(s)
+            >>> s.hex() == t.hex()
+            True
+            >>> len(scalar())
+            32
+            """
+            return bytes.__new__(cls, bs) if bs is not None else cls.random()
+
+        def __invert__(self: scalar) -> scalar:
+            """
+            Return the inverse of this instance (modulo
+            ``2**252 + 27742317777372353535851937790883648493``).
+
+            >>> s = scalar()
+            >>> p = point()
+            >>> ((~s) * (s * p)) == p
+            True
+
+            The scalar corresponding to the zero residue cannot be inverted.
+
+            >>> ~scalar.from_int(0)
+            Traceback (most recent call last):
+              ...
+            ValueError: cannot invert scalar corresponding to zero
+            """
+            if _zero(self):
+                raise ValueError('cannot invert scalar corresponding to zero')
+
+            return self._implementation.scalar(self._implementation.inv(self))
+
+        def __mul__(self: scalar, other: Union[scalar, point]) -> Union[scalar, point]:
+            """
+            Multiply the supplied scalar or point by this instance.
+
+            >>> p = point.hash('123'.encode())
+            >>> s = scalar.hash('456'.encode())
+            >>> (s * p).hex()
+            'f61b377aa86050aaa88c90f4a4a0f1e36b0000cf46f6a34232c2f1da7a799f16'
+            >>> p = point.from_base64('hoVaKq3oIlxEndP2Nqv3Rdbmiu4iinZE6Iwo+kcKAik=')
+            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
+            >>> (s * s).hex()
+            'd4aecf034f60edc5cb32cdd5a4be6d069959aa9fd133c51c9dcfd960ee865e0f'
+            >>> isinstance(s * s, scalar)
+            True
+            >>> (s * p).hex()
+            '2208082412921a67f42ea399748190d2b889228372509f2f2d9929813d074e1b'
+            >>> isinstance(s * p, point)
+            True
+
+            Multiplying any point or scalar by the scalar corresponding to the
+            zero residue yields the point or scalar corresponding to zero.
+
+            >>> scalar.from_int(0) * point() == p - p
+            True
+            >>> scalar.from_int(0) * scalar() == scalar.from_int(0)
+            True
+
+            Any attempt to multiply a value or object of an incompatible type by this
+            instance raises an exception.
+
+            >>> s * 2
+            Traceback (most recent call last):
+              ...
+            TypeError: multiplication by a scalar is defined only for scalars and points
+            """
+            if (
+                isinstance(other, python.scalar) or
+                (sodium is not None and isinstance(other, sodium.scalar))
+            ):
+                return self._implementation.scalar(self._implementation.smu(self, other))
+
+            if (
+                isinstance(other, python.point) or
+                (sodium is not None and isinstance(other, sodium.point))
+            ):
+                return self._implementation.point(self._implementation.mul(self, other))
+
+            raise TypeError(
+                'multiplication by a scalar is defined only for scalars and points'
+            )
+
+        def __rmul__(self: scalar, other: Union[scalar, point]):
+            """
+            A scalar cannot be on the right-hand side of a non-scalar.
+
+            >>> point() * scalar()
+            Traceback (most recent call last):
+              ...
+            TypeError: point must be on right-hand side of multiplication operator
+            """
+            raise TypeError(
+                'scalar must be on left-hand side of multiplication operator'
+            )
+
+        def to_bytes(self: scalar) -> bytes:
+            """
+            Return the bytes-like object that represents this instance.
+
+            >>> s = scalar()
+            >>> s.to_bytes() == s
+            True
+            """
+            return bytes(self)
+
+        def __int__(self: scalar) ->  int:
+            """
+            Return the integer (*i.e.*, least nonnegative residue) representation
+            of this instance.
+
+            >>> s = scalar()
+            >>> int(s * (~s))
+            1
+            """
+            return int.from_bytes(self, 'little')
+
+        def to_int(self: scalar) ->  int:
+            """
+            Return the integer (*i.e.*, least nonnegative residue) representation
+            of this instance.
+
+            >>> s = scalar()
+            >>> (s * (~s)).to_int()
+            1
+            """
+            return int(self)
+
+        def to_base64(self: scalar) -> str:
+            """
+            Return the Base64 UTF-8 string representation of this instance.
+
+            >>> s = scalar.from_base64('MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA=')
+            >>> s.to_base64()
+            'MS0MkTD2kVO+yfXQOGqVE160XuvxMK9fH+0cbtFfJQA='
+            """
+            return base64.standard_b64encode(self).decode('utf-8')
+
+    # Encapsulate classes for this implementation, regardless of which are
+    # exported as the unqualified symbols.
+    _implementation.point = point
+    _implementation.scalar = scalar
+
+# Redefine top-level wrapper classes to ensure that they appear at the end of
+# the auto-generated documentation.
+python = python # pylint: disable=self-assigning-variable
+sodium = sodium # pylint: disable=self-assigning-variable
+
+if __name__ == '__main__':
+    doctest.testmod() # pragma: no cover
```

### Comparing `oblivious-6.0.0/src/oblivious.egg-info/PKG-INFO` & `oblivious-7.0.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,228 +1,246 @@
-Metadata-Version: 2.1
-Name: oblivious
-Version: 6.0.0
-Summary: Python library that serves as an API for common cryptographic primitives used to implement OPRF, OT, and PSI protocols.
-Author: Nth Party, Ltd.
-Author-email: team@nthparty.com
-License: MIT
-Project-URL: Repository, https://github.com/nthparty/oblivious
-Project-URL: Documentation, https://oblivious.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: rbcl
-Provides-Extra: mclbn256
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
-=========
-oblivious
-=========
-
-Python library that serves as an API for common cryptographic primitives used to implement OPRF, OT, and PSI protocols.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/oblivious.svg
-   :target: https://badge.fury.io/py/oblivious
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/oblivious/badge/?version=latest
-   :target: https://oblivious.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/oblivious/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/nthparty/oblivious/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/oblivious/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/oblivious?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides pure-Python implementations, Python wrappers for `libsodium <https://github.com/jedisct1/libsodium>`__ and `mcl <https://github.com/herumi/mcl>`__, and additional utility methods for cryptographic primitives that are often used to implement `oblivious pseudorandom function (OPRF) <https://en.wikipedia.org/wiki/Pseudorandom_function_family>`__, `oblivious transfer (OT) <https://en.wikipedia.org/wiki/Oblivious_transfer>`__, and `private set intersection (PSI) <https://en.wikipedia.org/wiki/Private_set_intersection>`__ protocols.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/oblivious>`__::
-
-    python -m pip install oblivious
-
-It is possible to install the library together with packages that bundle dynamic/shared libraries, such as `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__::
-
-    python -m pip install oblivious[rbcl]
-    python -m pip install oblivious[mclbn256]
-    python -m pip install oblivious[rbcl,mclbn256]
-
-The library can be imported in the usual ways::
-
-    import oblivious
-    from oblivious import ristretto
-    from oblivious import bn254
-
-Examples
-^^^^^^^^
-
-.. |ristretto| replace:: ``ristretto``
-.. _ristretto: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html
-
-This library supports concise construction of elliptic curve points and scalars. The examples below use the |ristretto|_ module that provides data structures for working with the `Ristretto <https://ristretto.group>`__ group::
-
-    >>> from oblivious.ristretto import point, scalar
-    >>> p = point.hash('abc'.encode()) # Point derived from a hash of a string.
-    >>> s = scalar() # Random scalar.
-    >>> t = scalar.from_int(0) # Scalar corresponding to the zero residue.
-
-Built-in Python operators are overloaded to support point operations (such as addition, subtraction, negation, and equality) and scalar operations (such as multiplication by a scalar and inversion of scalars)::
-
-    >>> q = s * p
-    >>> p == (~s) * q
-    True
-    >>> p == ((~s) * s) * p
-    True
-    >>> p + q == q + p
-    True
-    >>> t * p == p - p
-    True
-
-.. |point| replace:: ``point``
-.. _point: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point
-
-.. |scalar| replace:: ``scalar``
-.. _scalar: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.scalar
-
-.. |bytes| replace:: ``bytes``
-.. _bytes: https://docs.python.org/3/library/stdtypes.html#bytes
-
-The |point|_ and |scalar|_ classes have common conversion methods that correspond to those supported by |bytes|_ objects (and in some cases, these classes are themselves derived from |bytes|_)::
-
-    >>> hex = '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-    >>> s = scalar.fromhex(hex)
-    >>> s.hex()
-    '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
-
-In addition, Base64 conversion methods are included to support concise encoding and decoding of |point|_ and |scalar|_ objects::
-
-    >>> s.to_base64()
-    'NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk='
-    >>> s == scalar.from_base64('NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk=')
-    True
-
-For more information and background about the underlying mathematical structures and primitives found in the |ristretto|_ module, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
-
-Using Pure Python or a Shared/Dynamic Library
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. |python| replace:: ``python``
-.. _python: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.python
-
-.. |sodium| replace:: ``sodium``
-.. _sodium: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.sodium
-
-Each module within this library can export two variants of its primitives and data structures: one corresponding to pure-Python implementations and another corresponding to shared/dynamic library wrappers.
-
-For example, the |ristretto|_ module exports two container classes/namespaces: |python|_ and |sodium|_. These encapsulate pure-Python implementations and shared/dynamic library (*i.e.*, libsodium) wrappers, respectively, of all operations and classes available in the |ristretto|_ module. This makes it possible to explicitly choose whether an operation requires only Python or also requires the presence of a compiled copy of libsodium on the host system.
-
-The example below uses pure-Python implementations of the scalar multiplication operation (relying on the `ge25519 <https://pypi.org/project/ge25519>`__ library)::
-
-    >>> from oblivious.ristretto import python
-    >>> p = python.point.hash('abc'.encode())
-    >>> s = python.scalar.hash('123'.encode())
-    >>> (s * p).to_base64()
-    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
-
-To check whether an instance of the libsodium shared/dynamic library has been loaded successfully, the check below can be performed::
-
-    >>> from oblivious.ristretto import sodium
-    >>> sodium is not None # Was the dynamic/shared library loaded?
-    True
-
-In the example below, the scalar multiplication operation invokes a binding for the ``crypto_scalarmult_ristretto255`` function `exported by libsodium <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto>`__::
-
-    >>> p = sodium.point.hash('abc'.encode())
-    >>> s = sodium.scalar.hash('123'.encode())
-    >>> (s * p).to_base64()
-    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
-
-.. |add| replace:: ``__add__``
-.. _add: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point.__add__
-
-The class methods exported by the |ristretto|_ module directly (*e.g.*, the method |add|_ within the class |point|_ that is imported via the statement ``from oblivious.ristretto import point``) correspond either (A) to libsodium wrappers if an instance of libsodium is found and loaded or (B) to pure-Python implementations if all attempts to load a working instances of libsodium fail. The ordered list below summarizes what definitions are exported under various conditions and the ordered sequence of attempts to locate and load an instance of libsodium.
-
-1. Under all conditions, the wrapper class |python|_ is defined and encapsulates a pure-Python variant of every low-level operation and class available in the |ristretto|_ module. **As a starting default**, all classes exported directly by the |ristretto|_ module correspond to the pure-Python implementations.
-
-2. If a shared/dynamic library instance of libsodium is found on the system and successfully loaded during one of the attempts below, then the wrapper class |sodium|_ is defined:
-
-   a. the built-in ``ctypes.util.find_library`` function is able to locate ``'sodium'`` or ``'libsodium'`` and it is loaded successfully;
-   b. a file ``libsodium.so`` or ``libsodium.dll`` under the paths specified by the ``PATH`` and ``LD_LIBRARY_PATH`` environment variables is found and loaded successfully; or
-   c. the optional `rbcl <https://pypi.org/project/rbcl>`__ package is installed and the compiled subset of libsodium included in that package is loaded successfully.
-
-3. If ``sodium`` is **not** ``None``, then the |sodium|_ class encapsulates libsodium wrappers for low-level operations and for every class exported by the |ristretto|_ module. Furthermore, **those classes exported directly by the library are redefined** to use the bindings available in the loaded instance of libsodium. The |python|_ class is still exported, as well, and all operations and class methods encapsulated within |python|_ remain as-is (*i.e.*, pure-Python implementations).
-
-.. |bn254| replace:: ``bn254``
-.. _bn254: https://oblivious.readthedocs.io/en/6.0.0/_source/oblivious.bn254.html
-
-The classes within the |bn254|_ module (both those that are pure-Python implementations and those that are wrappers for functions in the `mcl <https://github.com/herumi/mcl>`__ library) are organized in a similar manner. More information is available in the documentation for the |bn254|_ module.
-
-Development
------------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
-
-    python -m pip install .[docs,lint]
-
-Documentation
-^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
-
-    python -m pip install .[docs]
-    cd docs
-    sphinx-apidoc -f -e -E --templatedir=_templates -o _source .. && make html
-
-Testing and Conventions
-^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details, and note that unit tests that require `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__ are skipped if the corresponding optional package is not installed)::
-
-    python -m pip install .[test]
-    python -m pytest
-
-Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for the tests in a given testing module can be generated by running that testing module directly::
-
-    python test/test_ristretto.py
-    python test/test_bn254.py
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/oblivious test/test_ristretto.py test/test_bn254.py
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/oblivious>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/oblivious>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
-
-    python -m pip install .[publish]
-
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
-
-    git tag ?.?.?
-    git push origin ?.?.?
-
-Remove any old build/distribution files. Then, package the source into a distribution archive::
-
-    rm -rf build dist src/*.egg-info
-    python -m build --sdist --wheel .
-
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
-
-    python -m twine upload dist/*
+=========
+oblivious
+=========
+
+Python library that serves as an API for common cryptographic primitives used to implement OPRF, OT, and PSI protocols.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/oblivious.svg
+   :target: https://badge.fury.io/py/oblivious
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/oblivious/badge/?version=latest
+   :target: https://oblivious.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/oblivious/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/nthparty/oblivious/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/oblivious/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/oblivious?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides pure-Python implementations, Python wrappers for `libsodium <https://github.com/jedisct1/libsodium>`__ and `mcl <https://github.com/herumi/mcl>`__, and additional utility methods for cryptographic primitives that are often used to implement `oblivious pseudorandom function (OPRF) <https://en.wikipedia.org/wiki/Pseudorandom_function_family>`__, `oblivious transfer (OT) <https://en.wikipedia.org/wiki/Oblivious_transfer>`__, and `private set intersection (PSI) <https://en.wikipedia.org/wiki/Private_set_intersection>`__ protocols.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/oblivious>`__:
+
+.. code-block:: bash
+
+    python -m pip install oblivious
+
+It is possible to install the library together with packages that bundle dynamic/shared libraries, such as `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__ (note that in some environments, the brackets and/or commas may need to be escaped):
+
+.. code-block:: bash
+
+    python -m pip install oblivious[rbcl]
+    python -m pip install oblivious[mclbn256]
+    python -m pip install oblivious[rbcl,mclbn256]
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import oblivious
+    from oblivious import ristretto
+    from oblivious import bn254
+
+Examples
+^^^^^^^^
+
+.. |ristretto| replace:: ``ristretto``
+.. _ristretto: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html
+
+This library supports concise construction of elliptic curve points and scalars. The examples below use the |ristretto|_ module that provides data structures for working with the `Ristretto <https://ristretto.group>`__ group:
+
+.. code-block:: python
+
+    >>> from oblivious.ristretto import point, scalar
+    >>> p = point.hash('abc'.encode()) # Point derived from a hash of a string.
+    >>> s = scalar() # Random scalar.
+    >>> t = scalar.from_int(0) # Scalar corresponding to the zero residue.
+
+Built-in Python operators are overloaded to support point operations (such as addition, subtraction, negation, and equality) and scalar operations (such as multiplication by a scalar and inversion of scalars):
+
+.. code-block:: python
+
+    >>> q = s * p
+    >>> p == (~s) * q
+    True
+    >>> p == ((~s) * s) * p
+    True
+    >>> p + q == q + p
+    True
+    >>> t * p == p - p
+    True
+
+.. |point| replace:: ``point``
+.. _point: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point
+
+.. |scalar| replace:: ``scalar``
+.. _scalar: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.scalar
+
+.. |bytes| replace:: ``bytes``
+.. _bytes: https://docs.python.org/3/library/stdtypes.html#bytes
+
+The |point|_ and |scalar|_ classes have common conversion methods that correspond to those supported by |bytes|_ objects (and in some cases, these classes are themselves derived from |bytes|_):
+
+.. code-block:: python
+
+    >>> hex = '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+    >>> s = scalar.from_hex(hex)
+    >>> s.hex()
+    '35c141f1c2c43543de9d188805a210abca3cd39a1e986304991ceded42b11709'
+
+In addition, Base64 conversion methods are included to support concise encoding and decoding of |point|_ and |scalar|_ objects:
+
+.. code-block:: python
+
+    >>> s.to_base64()
+    'NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk='
+    >>> s == scalar.from_base64('NcFB8cLENUPenRiIBaIQq8o805oemGMEmRzt7UKxFwk=')
+    True
+
+For more information and background about the underlying mathematical structures and primitives found in the |ristretto|_ module, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
+
+Using Pure Python or a Shared/Dynamic Library
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. |python| replace:: ``python``
+.. _python: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.python
+
+.. |sodium| replace:: ``sodium``
+.. _sodium: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.sodium
+
+Each module within this library can export two variants of its primitives and data structures: one corresponding to pure-Python implementations and another corresponding to shared/dynamic library wrappers.
+
+For example, the |ristretto|_ module exports two container classes/namespaces: |python|_ and |sodium|_. These encapsulate pure-Python implementations and shared/dynamic library (*i.e.*, libsodium) wrappers, respectively, of all operations and classes available in the |ristretto|_ module. This makes it possible to explicitly choose whether an operation requires only Python or also requires the presence of a compiled copy of libsodium on the host system.
+
+The example below uses pure-Python implementations of the scalar multiplication operation (relying on the `ge25519 <https://pypi.org/project/ge25519>`__ library):
+
+.. code-block:: python
+
+    >>> from oblivious.ristretto import python
+    >>> p = python.point.hash('abc'.encode())
+    >>> s = python.scalar.hash('123'.encode())
+    >>> (s * p).to_base64()
+    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
+
+To check whether an instance of the libsodium shared/dynamic library has been loaded successfully, the check below can be performed:
+
+.. code-block:: python
+
+    >>> from oblivious.ristretto import sodium
+    >>> sodium is not None # Was the dynamic/shared library loaded?
+    True
+
+In the example below, the scalar multiplication operation invokes a binding for the ``crypto_scalarmult_ristretto255`` function `exported by libsodium <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto>`__:
+
+.. code-block:: python
+
+    >>> p = sodium.point.hash('abc'.encode())
+    >>> s = sodium.scalar.hash('123'.encode())
+    >>> (s * p).to_base64()
+    'SrC7vA9sSR5f4E27ALxk14MPotTYR6B33B4ZN+mQXFA='
+
+.. |add| replace:: ``__add__``
+.. _add: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.ristretto.html#oblivious.ristretto.point.__add__
+
+The class methods exported by the |ristretto|_ module directly (*e.g.*, the method |add|_ within the class |point|_ that is imported via the statement ``from oblivious.ristretto import point``) correspond either (A) to libsodium wrappers if an instance of libsodium is found and loaded or (B) to pure-Python implementations if all attempts to load a working instances of libsodium fail. The ordered list below summarizes what definitions are exported under various conditions and the ordered sequence of attempts to locate and load an instance of libsodium.
+
+1. Under all conditions, the wrapper class |python|_ is defined and encapsulates a pure-Python variant of every low-level operation and class available in the |ristretto|_ module. **As a starting default**, all classes exported directly by the |ristretto|_ module correspond to the pure-Python implementations.
+
+2. If a shared/dynamic library instance of libsodium is found on the system and successfully loaded during one of the attempts below, then the wrapper class |sodium|_ is defined:
+
+   a. the built-in ``ctypes.util.find_library`` function is able to locate ``'sodium'`` or ``'libsodium'`` and it is loaded successfully;
+   b. a file ``libsodium.so`` or ``libsodium.dll`` under the paths specified by the ``PATH`` and ``LD_LIBRARY_PATH`` environment variables is found and loaded successfully; or
+   c. the optional `rbcl <https://pypi.org/project/rbcl>`__ package is installed and the compiled subset of libsodium included in that package is loaded successfully.
+
+3. If ``sodium`` is **not** ``None``, then the |sodium|_ class encapsulates libsodium wrappers for low-level operations and for every class exported by the |ristretto|_ module. Furthermore, **those classes exported directly by the library are redefined** to use the bindings available in the loaded instance of libsodium. The |python|_ class is still exported, as well, and all operations and class methods encapsulated within |python|_ remain as-is (*i.e.*, pure-Python implementations).
+
+.. |bn254| replace:: ``bn254``
+.. _bn254: https://oblivious.readthedocs.io/en/7.0.0/_source/oblivious.bn254.html
+
+The classes within the |bn254|_ module (both those that are pure-Python implementations and those that are wrappers for functions in the `mcl <https://github.com/herumi/mcl>`__ library) are organized in a similar manner. More information is available in the documentation for the |bn254|_ module.
+
+Development
+-----------
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs,lint]
+
+Documentation
+^^^^^^^^^^^^^
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs]
+    cd docs
+    sphinx-apidoc -f -e -E --templatedir=_templates -o _source .. && make html
+
+Testing and Conventions
+^^^^^^^^^^^^^^^^^^^^^^^
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details, and note that unit tests that require `rbcl <https://pypi.org/project/rbcl>`__ and/or `mclbn256 <https://pypi.org/project/mclbn256>`__ are skipped if the corresponding optional package is not installed):
+
+.. code-block:: bash
+
+    python -m pip install .[test]
+    python -m pytest
+
+Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for the tests in a given testing module can be generated by running that testing module directly:
+
+.. code-block:: bash
+
+    python test/test_ristretto.py
+    python test/test_bn254.py
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/oblivious test/test_ristretto.py test/test_bn254.py
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/oblivious>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/oblivious>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
+
+    python -m pip install .[publish]
+
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
+
+    git tag ?.?.?
+    git push origin ?.?.?
+
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
+
+    rm -rf build dist src/*.egg-info
+    python -m build --sdist --wheel .
+
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
+
+    python -m twine upload dist/*
```

### Comparing `oblivious-6.0.0/test/test_bn254.py` & `oblivious-7.0.0/test/test_bn254.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,1552 +1,1552 @@
-"""
-Test suite containing functional unit tests for the exported primitives and
-classes in the :obj:`oblivious.bn254` module, as well as unit tests
-confirming algebraic relationships among primitives.
-"""
-# pylint: disable=missing-function-docstring
-from unittest import TestCase
-import importlib
-import base64
-from bitlist import bitlist
-from fountains import fountains
-
-try:
-    from oblivious import bn254 # pylint: disable=import-error
-except: # pylint: disable=bare-except
-    # To support generation of reference specifications for unit tests.
-    spec = importlib.util.spec_from_file_location("bn254", "src/oblivious/bn254.py")
-    bn254 = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(bn254)
-
-# Constants for the number of input-output pairs to include in each test and for
-# representation sizes of data structures (in their binary form).
-TRIALS_PER_TEST = 16
-POINT_HASH_LEN = 64 # Size of raw hash digest required to construct a point.
-POINT_LEN = 32 * 3 # Three 32-byte coordinate values (*x*, *y*, and *z* in projective coordinates).
-POINT2_LEN = 192
-SCALAR_LEN = 32
-SCALAR2_LEN = 384
-
-# To simulate an environment in which the mcl library is absent, some tests set
-# ``bn254.mcl`` to ``None``; the references below are used for restoration.
-mcl_restore = bn254.mcl
-
-def api_functions():
-    """
-    Low-level functions that should be available to users within each of the two
-    namespaces.
-    """
-    return {
-        'pnt', 'bas', 'can', 'ser', 'des', 'mul', 'add', 'sub', 'neg', 'par',
-        'rnd', 'scl', 'sse', 'sde', 'inv', 'smu', 'sad', 'ssu', 'sne',
-        'pnt2', 'bas2', 'can2', 'ser2', 'des2', 'mul2', 'add2', 'sub2', 'neg2',
-        'rnd2', 'scl2', 'sse2', 'sde2', 'inv2', 'smu2', 'sad2'
-    }
-
-def api_classes():
-    """
-    Classes that should be available to users upon module import.
-    """
-    return {'point', 'scalar', 'point2', 'scalar2'}
-
-class Test_namespace(TestCase):
-    """
-    Check that namespaces provide access to the expected
-    classes and functions.
-    """
-    def test_init(self):
-        init = importlib.import_module('oblivious.__init__')
-        self.assertTrue('bn254' in init.__dict__)
-
-    def test_modules(self):
-        module = importlib.import_module('oblivious.bn254')
-        self.assertTrue('python' in module.__dict__)
-        self.assertTrue('mcl' in module.__dict__)
-        self.assertTrue(api_classes().issubset(module.__dict__.keys()))
-
-    def test_python(self):
-        self.assertTrue(
-            (api_functions() - {'par'}).issubset(set(dir(bn254.python)))
-        )
-        self.assertTrue(api_classes().issubset(set(dir(bn254.python))))
-
-    def test_mcl(self):
-        if bn254.mcl is not None:
-            self.assertTrue(api_functions().issubset(set(dir(bn254.mcl))))
-            self.assertTrue(api_classes().issubset(set(dir(bn254.mcl))))
-
-def check_or_generate_operation(test, fun, lengths, bits):
-    """
-    This function does either of two things depending on the parameter ``bits``:
-    * checks that test inputs drawn from the :obj:`fountains` input bit stream
-      produce the bits provided in the reference output bit vector, or
-    * generates a reference output bit vector by applying the function
-      to the :obj:`fountains` input bit stream.
-    """
-    def get_bytes(o):
-        if type(o) in (bytes, bytearray, bitlist):
-            return o
-
-        cls = bn254.python if isinstance(o, bytes) else bn254.mcl
-
-        # Transform points to canonical form.
-        cls_str = str(o.__class__)
-        if 'point2' in cls_str or 'G2' in cls_str:
-            o = cls.can2(o)
-        elif 'point' in cls_str or 'G1' in cls_str:
-            o = cls.can(o)
-
-        return (
-            cls.ser(o)
-            if ('point' in str(o.__class__) or 'G' in str(o.__class__)) else
-            cls.sse(o)
-        )
-
-    fs = fountains( # Generate the input bit stream.
-        sum(lengths),
-        seed=bytes(0), # This is also the default; explicit for clarity.
-        limit=min(TRIALS_PER_TEST, (len(bits) * 4) if bits is not None else 256),
-        bits=bits[:(TRIALS_PER_TEST // 4)] if bits is not None else None,
-        function=lambda *args, **kwargs: get_bytes(fun(*args, **kwargs))
-    )
-
-    if bits is None: # There is no output reference bit vector, so test is not possible.
-        return bitlist(list(fs)).hex() # Return reference output bits for test.
-
-    test.assertTrue(all(fs)) # Check that all outputs match.
-
-def mcl_hidden_and_fallback(hidden=False, fallback=False):
-    """
-    Return binary wrapper class definition that conforms to the
-    scenario being tested.
-    """
-    if hidden:
-        bn254.mcl = None
-    elif fallback:
-        bn254.mcl = mcl_restore
-    else:
-        bn254.mcl = mcl_restore
-
-def define_classes(cls, hidden=False, fallback=False): # pylint: disable=too-many-statements
-    """
-    Define and return four classes of unit tests given a wrapper
-    class (``python`` or ``mcl``) for primitive operations.
-    """
-    class Test_primitives(TestCase):
-        """
-        Direct tests of primitive operators that operate on bytes-like objects.
-        """
-        def test_pnt(
-                self,
-                bits='bc3d'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.pnt, [POINT_HASH_LEN], bits)
-
-        def test_pnt_none(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                self.assertTrue(len(cls.ser(cls.pnt())) == POINT_LEN)
-
-        def test_bas(
-                self,
-                bits='82d6'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00111111 # Improve chance of testing with a valid scalar.
-                bs = bytes(bs)
-                s = cls.scl(bs)
-                return cls.bas(s) if s is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_can(
-                self,
-                bits='bc3d'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.can(cls.pnt(bs))
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_ser(
-                self,
-                bits='bc3d'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.ser(cls.pnt(bs))
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_des(
-                self,
-                bits='bc3d'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.des(cls.ser(cls.pnt(bs)))
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_mul(
-                self,
-                bits='b9e1'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00111111 # Improve chance of testing with a valid scalar.
-                bs[SCALAR_LEN - 1] &= 0b00011111
-                bs = bytes(bs)
-                (s, p) = (cls.scl(bs[:SCALAR_LEN]), cls.pnt(bs[SCALAR_LEN:]))
-                return cls.mul(s, p) if (s is not None and p is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
-
-        def test_add(
-                self,
-                bits='40d9'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (cls.pnt(bs[:POINT_HASH_LEN]), cls.pnt(bs[POINT_HASH_LEN:]))
-                return cls.add(p1, p2) if (p1 is not None and p2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_sub(
-                self,
-                bits='71df'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (cls.pnt(bs[:POINT_HASH_LEN]), cls.pnt(bs[POINT_HASH_LEN:]))
-                return cls.sub(p1, p2) if (p1 is not None and p2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_neg(
-                self,
-                bits='bc3d'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.neg(cls.pnt(bs))
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_par(
-                self,
-                bits='49f2'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (cls.point.hash(bs), cls.point2.hash(bs))
-                return cls.sse2(cls.par(p1, p2))
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_rnd(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.rnd()
-                self.assertTrue(cls.scl(bytes(s)))
-
-        def test_scl(
-                self,
-                bits='ffff'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00111111 # Improve chances of testing with a valid scalar.
-                bs = bytes(bs)
-                r = 0x2523648240000001ba344d8000000007ff9f800000000010a10000000000000d
-                return bitlist([
-                    1
-                    if (bool(cls.scl(bs)) == (int.from_bytes(bs, 'little') < r)) is not None else
-                    0
-                ])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_scl_none(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                bs = bytes([255] * 32) # Representation value above the maximum scalar value.
-                s = cls.scl(bs)
-                self.assertTrue(s is None)
-
-        def test_sse(
-                self,
-                bits='ab29'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
-                s = cls.scl(bytes(bs))
-                return cls.sse(s) if s is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_sde(
-                self,
-                bits='ab29'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
-                s = cls.scl(bytes(bs))
-                return cls.sde(cls.sse(s)) if s is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_inv(
-                self,
-                bits='0aea'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
-                bs = bytes(bs)
-                s = cls.scl(bs)
-                return cls.inv(s) if s is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_smu(
-                self,
-                bits='dfad'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
-                bs[SCALAR_LEN - 1] &= 0b00011111
-                bs = bytes(bs)
-                (s1, s2) = (cls.scl(bs[:SCALAR_LEN]), cls.scl(bs[SCALAR_LEN:]))
-                return cls.smu(s1, s2) if (s1 is not None and s2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
-
-        def test_sad(
-                self,
-                bits='6c5b'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
-                bs[SCALAR_LEN - 1] &= 0b00011111
-                bs = bytes(bs)
-                (s1, s2) = (cls.scl(bs[:SCALAR_LEN]), cls.scl(bs[SCALAR_LEN:]))
-                return cls.sad(s1, s2) if (s1 is not None and s2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
-
-        def test_ssu(
-                self,
-                bits='dc34'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
-                bs[SCALAR_LEN - 1] &= 0b00011111
-                bs = bytes(bs)
-                (s1, s2) = (cls.scl(bs[:SCALAR_LEN]), cls.scl(bs[SCALAR_LEN:]))
-                return cls.ssu(s1, s2) if (s1 is not None and s2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
-
-        def test_sne(
-                self,
-                bits='66d6'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
-                bs = bytes(bs)
-                s = cls.scl(bs)
-                return cls.sne(s) if s is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_pnt2(
-                self,
-                bits='d28c'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.pnt2, [POINT_HASH_LEN], bits)
-
-        def test_bas2(
-                self,
-                bits='1ed0'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.bas2(cls.scalar.hash(bs))
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_can2(
-                self,
-                bits='d28c'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.ser2(cls.can2(cls.pnt2(bs)))
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_ser2(
-                self,
-                bits='d28c'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.ser2(cls.can2(cls.pnt2(bs)))
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_des2(
-                self,
-                bits='d28c'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.des2(cls.ser2(cls.can2(cls.pnt2(bs))))
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_mul2(
-                self,
-                bits='1e5c'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (s, p) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.pnt2(bs[SCALAR_LEN:]))
-                return cls.mul2(s, p)
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
-
-        def test_add2(
-                self,
-                bits='424e'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (cls.pnt2(bs[:POINT_HASH_LEN]), cls.pnt2(bs[POINT_HASH_LEN:]))
-                return cls.add2(p1, p2)
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_sub2(
-                self,
-                bits='15c9'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (cls.pnt2(bs[:POINT_HASH_LEN]), cls.pnt2(bs[POINT_HASH_LEN:]))
-                return cls.sub2(p1, p2)
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_neg2(
-                self,
-                bits='d28c'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.neg2(cls.pnt2(bs))
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_rnd2(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.rnd2()
-                self.assertTrue(cls.scl2(bytes(s)) is not None)
-
-        def test_scl2(
-                self,
-                bits='a567'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.sse2(cls.scl2(cls.scalar2.hash(bs).to_bytes()))
-            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
-
-        def test_sse2(
-                self,
-                bits='a567'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.sse2(cls.scalar2.hash(bs))
-            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
-
-        def test_sde2(
-                self,
-                bits='a567'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.sse2(cls.sde2(cls.sse2(cls.scalar2.hash(bs))))
-            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
-
-        def test_inv2(
-                self,
-                bits='a567'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.sse2(cls.inv2(cls.scalar2.hash(bs)))
-            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
-
-        def test_smu2(
-                self,
-                bits='ed98'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (s1, s2) = (cls.scalar2.hash(bs[:SCALAR2_LEN]), cls.scalar2.hash(bs[SCALAR2_LEN:]))
-                return cls.sse2(cls.smu2(s1, s2))
-            return check_or_generate_operation(self, fun, [SCALAR2_LEN, SCALAR2_LEN], bits)
-
-        def test_sad2(
-                self,
-                bits='1d51'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (s1, s2) = (cls.scalar2.hash(bs[:SCALAR2_LEN]), cls.scalar2.hash(bs[SCALAR2_LEN:]))
-                return cls.sse2(cls.sad2(s1, s2))
-            return check_or_generate_operation(self, fun, [SCALAR2_LEN, SCALAR2_LEN], bits)
-
-    class Test_classes(TestCase): # pylint: disable=too-many-public-methods
-        """
-        Tests of point and scalar wrapper classes and their methods.
-        """
-        def test_point_random(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                self.assertTrue(len(cls.point.random()) == POINT_LEN)
-
-        def test_point_bytes(
-                self,
-                bits='bc3d'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.point.bytes, [POINT_HASH_LEN], bits)
-
-        def test_point_hash(
-                self,
-                bits='c8ea'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.point.hash, [POINT_HASH_LEN], bits)
-
-        def test_point_base(
-                self,
-                bits='ebed'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00011111 # Improve chance of testing with a valid scalar.
-                s = cls.scalar.bytes(bytes(bs))
-                return cls.point.base(s) if s is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_point_to_bytes_from_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                p = cls.point()
-                self.assertEqual(cls.point.from_bytes(p.to_bytes()), p)
-
-        def test_point_hex_fromhex(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                p = cls.point()
-                self.assertEqual(cls.point.fromhex(p.hex()), p)
-
-        def test_point_to_base64_from_base64(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                p = cls.point()
-                p_b64 = base64.standard_b64encode(p.to_bytes()).decode('utf-8')
-                self.assertEqual(p.to_base64(), p_b64)
-                self.assertEqual(cls.point.from_base64(p.to_base64()), p)
-                self.assertEqual(cls.point.from_base64(p_b64), p)
-
-        def test_point(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                self.assertTrue(len(cls.point()) == POINT_LEN)
-
-        def test_point_canonical(
-                self,
-                bits='bc3d'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.point.bytes(bs).canonical()
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_point_scalar_mul(
-                self,
-                bits='b9e1'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00111111 # Improve chance of testing with a valid scalar.
-                bs[SCALAR_LEN - 1] &= 0b00011111
-                bs = bytes(bs)
-                (s, p) = (cls.scalar.bytes(bs[:SCALAR_LEN]), cls.point.bytes(bs[SCALAR_LEN:]))
-                # Below, ``*`` invokes :obj:`scalar.__mul__`, which delegates to :obj:`mul`
-                # due to the type of the second argument.
-                return s * p if (s is not None and p is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
-
-        def test_point_add(
-                self,
-                bits='40d9'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (
-                    cls.point.bytes(bs[:POINT_HASH_LEN]),
-                    cls.point.bytes(bs[POINT_HASH_LEN:])
-                )
-                return p1 + p2 if (p1 is not None and p2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_point_sub(
-                self,
-                bits='71df'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (
-                    cls.point.bytes(bs[:POINT_HASH_LEN]),
-                    cls.point.bytes(bs[POINT_HASH_LEN:])
-                )
-                return p1 - p2 if (p1 is not None and p2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_point_neg(
-                self,
-                bits='bc3d'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                p = cls.point.bytes(bs)
-                return -p if p is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_point_pair(
-                self,
-                bits='9cd3'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (
-                    cls.point.hash(bs[:POINT_HASH_LEN]),
-                    cls.point2.hash(bs[POINT_HASH_LEN:])
-                )
-                return p1 @ p2
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_scalar_random(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar.random()
-                self.assertTrue(cls.scalar.bytes(bytes(s)) is not None)
-                self.assertTrue(len(s) == SCALAR_LEN and len(s.to_bytes()) == SCALAR_LEN)
-
-        def test_scalar_bytes(
-                self,
-                bits='ab29'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = bytearray(bs)
-                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
-                s = cls.scalar.bytes(bytes(bs))
-                return s.to_bytes() if s is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_scalar_hash(
-                self,
-                bits='1c21'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.scalar.hash, [SCALAR_LEN], bits)
-
-        def test_scalar_to_int(
-                self,
-                bits='6969'
-            ):
-            def fun(bs):
-                s = cls.scalar.hash(bs)
-                return abs(s.to_int()).to_bytes(32, 'little')
-            return check_or_generate_operation(self, fun, [32], bits)
-
-        def test_scalar_from_int(
-                self,
-                bits='d27b'
-            ):
-            def fun(bs):
-                s = cls.scalar.from_int(int.from_bytes(bs, 'little'))
-                return s if (s is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [32], bits)
-
-        def test_scalar_to_bytes_from_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar()
-                self.assertEqual(cls.scalar.from_bytes(s.to_bytes()), s)
-
-        def test_scalar_hex_fromhex(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar()
-                self.assertEqual(cls.scalar.fromhex(s.hex()), s)
-
-        def test_scalar_to_base64_from_base64(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar()
-                s_b64 = base64.standard_b64encode(s.to_bytes()).decode('utf-8')
-                self.assertEqual(s.to_base64(), s_b64)
-                self.assertEqual(cls.scalar.from_base64(s_b64), s)
-                self.assertEqual(cls.scalar.from_base64(s.to_base64()), s)
-
-        def test_scalar(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar()
-                self.assertTrue(len(s) == SCALAR_LEN and cls.scalar.bytes(bytes(s)) is not None)
-                self.assertTrue(len(bytes(s)) == SCALAR_LEN and len(s.to_bytes()) == SCALAR_LEN)
-
-        def test_scalar_invert(
-                self,
-                bits='c4e3'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                s = cls.scalar.hash(bs)
-                return ~s
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_scalar_mul(
-                self,
-                bits='93d3'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (s1, s2) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.scalar.hash(bs[SCALAR_LEN:]))
-                return s1 * s2 if (s1 is not None and s2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
-
-        def test_scalar_add(
-                self,
-                bits='debe'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                s = cls.scalar.hash(bs[SCALAR_LEN:])
-                t = cls.scalar.hash(bs[:SCALAR_LEN])
-                return s + t
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
-
-        def test_scalar_sub(
-                self,
-                bits='7fc9'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                s = cls.scalar.hash(bs[SCALAR_LEN:])
-                t = cls.scalar.hash(bs[:SCALAR_LEN])
-                return s - t
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
-
-        def test_scalar_neg(
-                self,
-                bits='a1de'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                s = cls.scalar.hash(bs)
-                return -s
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_point2_random(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                self.assertTrue(len(cls.point2.random()) == POINT2_LEN)
-
-        def test_point2_bytes(
-                self,
-                bits='d28c'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.point2.bytes, [POINT_HASH_LEN], bits)
-
-        def test_point2_hash(
-                self,
-                bits='d51b'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.point2.hash, [POINT_HASH_LEN], bits)
-
-        def test_point2_base(
-                self,
-                bits='1ed0'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.point2.base(cls.scalar.hash(bs))
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_point2_to_bytes_from_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                p = cls.point2()
-                self.assertEqual(cls.point2.from_bytes(p.to_bytes()), p)
-
-        def test_point2_hex_fromhex(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                p = cls.point2()
-                self.assertEqual(cls.point2.fromhex(p.hex()), p)
-
-        def test_point2_to_base64_from_base64(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                p = cls.point2()
-                p_b64 = base64.standard_b64encode(p.to_bytes()).decode('utf-8')
-                self.assertEqual(p.to_base64(), p_b64)
-                self.assertEqual(cls.point2.from_base64(p.to_base64()), p)
-                self.assertEqual(cls.point2.from_base64(p_b64), p)
-
-        def test_point2(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                self.assertTrue(len(cls.point2()) == POINT2_LEN)
-
-        def test_point2_canonical(
-                self,
-                bits='d28c'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.point2.bytes(bs).canonical()
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_point2_scalar_mul(
-                self,
-                bits='1e5c'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (s, p) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.point2.bytes(bs[SCALAR_LEN:]))
-                # Below, ``*`` invokes :obj:`scalar.__mul__`, which delegates to :obj:`mul`
-                # due to the type of the second argument.
-                return s * p
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
-
-        def test_point2_add(
-                self,
-                bits='424e'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (cls.point2.bytes(bs[:POINT_HASH_LEN]), cls.point2.bytes(bs[POINT_HASH_LEN:]))
-                return p1 + p2
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_point2_sub(
-                self,
-                bits='15c9'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (cls.point2.bytes(bs[:POINT_HASH_LEN]), cls.point2.bytes(bs[POINT_HASH_LEN:]))
-                return p1 - p2
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_point2_neg(
-                self,
-                bits='d28c'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return -cls.point2.bytes(bs)
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_scalar2_random(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar2.random()
-                self.assertTrue(cls.scalar2.bytes(s.to_bytes()) is not None)
-                self.assertTrue(len(s) == SCALAR2_LEN and len(s.to_bytes()) == SCALAR2_LEN)
-
-        def test_scalar2_bytes(
-                self,
-                bits='a567'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                bs = cls.scalar2.hash(bs).to_bytes()
-                s = cls.scalar2.bytes(bs)
-                return s.to_bytes()
-            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
-
-        def test_scalar2_hash(
-                self,
-                bits='a567'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.scalar2.hash, [SCALAR2_LEN], bits)
-
-        def test_scalar2_to_bytes_from_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar2()
-                self.assertEqual(cls.scalar2.from_bytes(s.to_bytes()), s)
-
-        def test_scalar2_hex_fromhex(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar2()
-                self.assertEqual(cls.scalar2.fromhex(s.hex()), s)
-
-        def test_scalar2_to_base64_from_base64(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar2()
-                s_b64 = base64.standard_b64encode(s.to_bytes()).decode('utf-8')
-                self.assertEqual(s.to_base64(), s_b64)
-                self.assertEqual(cls.scalar2.from_base64(s_b64), s)
-                self.assertEqual(cls.scalar2.from_base64(s.to_base64()), s)
-
-        def test_scalar2(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar2()
-                self.assertTrue(cls.scalar2(s.to_bytes()) is not None)
-                self.assertTrue(len(s) == SCALAR2_LEN and len(s.to_bytes()) == SCALAR2_LEN)
-
-        def test_scalar2_invert(
-                self,
-                bits='a567'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                s = cls.scalar2.hash(bs)
-                return ~s
-            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
-
-        def test_scalar2_mul(
-                self,
-                bits='b0f7'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (s1, s2) = (cls.scalar2.hash(bs[:SCALAR_LEN]), cls.scalar2.hash(bs[SCALAR_LEN:]))
-                return s1 * s2
-            return check_or_generate_operation(self, fun, [SCALAR2_LEN, SCALAR2_LEN], bits)
-
-        def test_scalar2_add(
-                self,
-                bits='015e'
-            ):
-            mcl_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (s1, s2) = (cls.scalar2.hash(bs[:SCALAR_LEN]), cls.scalar2.hash(bs[SCALAR_LEN:]))
-                return s1 + s2
-            return check_or_generate_operation(self, fun, [SCALAR2_LEN, SCALAR2_LEN], bits)
-
-    class Test_types(TestCase): # pylint: disable=too-many-public-methods
-        """
-        Tests verifying that methods that should return point and scalar classes
-        do indeed return point and scalar objects of the expected types.
-        """
-        def test_types_point_random(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            p = cls.point.random()
-            self.assertTrue(isinstance(p, cls.point))
-
-        def test_types_point_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN, limit=1)
-            p = cls.point.bytes(bs)
-            self.assertTrue(isinstance(p, cls.point))
-
-        def test_types_point_hash(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN, limit=1)
-            p = cls.point.hash(bs)
-            self.assertTrue(isinstance(p, cls.point))
-
-        def test_types_point_base(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            p = cls.point.base(cls.scalar.random())
-            self.assertTrue(isinstance(p, cls.point))
-
-        def test_types_point_to_bytes_from_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            bs = cls.point.random().to_bytes()
-            self.assertTrue(isinstance(cls.point.from_bytes(bs), cls.point))
-
-        def test_types_point_hex_fromhex(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.point.random().hex()
-            self.assertTrue(isinstance(cls.point.fromhex(s), cls.point))
-
-        def test_types_point_to_base64_from_base64(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.point.random().to_base64()
-            self.assertTrue(isinstance(cls.point.from_base64(s), cls.point))
-
-        def test_types_point_canonical(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            p = cls.point.base(cls.scalar.random())
-            self.assertTrue(isinstance(p.canonical(), cls.point))
-
-        def test_types_point_mul(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(SCALAR_LEN + POINT_HASH_LEN, limit=1)
-            (s, p) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.point.hash(bs[SCALAR_LEN:]))
-            self.assertTrue(isinstance(s * p, cls.point))
-
-        def test_types_point_add(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
-            (p0, p1) = (cls.point.hash(bs[:POINT_HASH_LEN]), cls.point.hash(bs[POINT_HASH_LEN:]))
-            self.assertTrue(isinstance(p0 + p1, cls.point))
-
-        def test_types_point_sub(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
-            (p0, p1) = (cls.point.hash(bs[:POINT_HASH_LEN]), cls.point.hash(bs[POINT_HASH_LEN:]))
-            self.assertTrue(isinstance(p0 - p1, cls.point))
-
-        def test_types_point_neg(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN, limit=1)
-            p = cls.point.hash(bs)
-            self.assertTrue(isinstance(-p, cls.point))
-
-        def test_types_point_point2_matmul(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
-            (p0, p1) = (cls.point.hash(bs[:POINT_HASH_LEN]), cls.point2.hash(bs[POINT_HASH_LEN:]))
-            self.assertTrue(isinstance(p0 @ p1, cls.scalar2))
-
-        def test_types_scalar_random(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            self.assertTrue(isinstance(cls.scalar.random(), cls.scalar))
-
-        def test_types_scalar_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            bs = cls.scalar.random().to_bytes()
-            self.assertTrue(isinstance(cls.scalar.bytes(bs), cls.scalar))
-
-        def test_types_scalar_hash(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(SCALAR_LEN, limit=1)
-            self.assertTrue(isinstance(cls.scalar.hash(bs), cls.scalar))
-
-        def test_types_scalar_to_int_from_int(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            n = cls.scalar.random().to_int()
-            self.assertTrue(isinstance(cls.scalar.from_int(n), cls.scalar))
-
-        def test_types_scalar_to_bytes_from_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            bs = cls.scalar.random().to_bytes()
-            self.assertTrue(isinstance(cls.scalar.from_bytes(bs), cls.scalar))
-
-        def test_types_scalar_hex_fromhex(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar.random().hex()
-            self.assertTrue(isinstance(cls.scalar.fromhex(s), cls.scalar))
-
-        def test_types_scalar_to_base64_from_base64(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar.random().to_base64()
-            self.assertTrue(isinstance(cls.scalar.from_base64(s), cls.scalar))
-
-        def test_types_scalar_invert(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            self.assertTrue(isinstance(~cls.scalar.random(), cls.scalar))
-
-        def test_types_scalar_mul_scalar(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (s0, s1) = (cls.scalar.random(), cls.scalar.random())
-            self.assertTrue(isinstance(s0 * s1, cls.scalar))
-
-        def test_types_scalar_add_scalar(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (s0, s1) = (cls.scalar.random(), cls.scalar.random())
-            self.assertTrue(isinstance(s0 + s1, cls.scalar))
-
-        def test_types_scalar_sub_scalar(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (s0, s1) = (cls.scalar.random(), cls.scalar.random())
-            self.assertTrue(isinstance(s0 - s1, cls.scalar))
-
-        def test_types_scalar_neg(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar.random()
-            self.assertTrue(isinstance(-s, cls.scalar))
-
-        def test_types_scalar_mul_point(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            self.assertTrue(isinstance(cls.scalar() * cls.point(), cls.point))
-
-        def test_types_point2_random(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            p = cls.point2.random()
-            self.assertTrue(isinstance(p, cls.point2))
-
-        def test_types_point2_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN, limit=1)
-            p = cls.point2.bytes(bs)
-            self.assertTrue(isinstance(p, cls.point2))
-
-        def test_types_point2_hash(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN, limit=1)
-            p = cls.point2.hash(bs)
-            self.assertTrue(isinstance(p, cls.point2))
-
-        def test_types_point2_base(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            p = cls.point2.base(cls.scalar.random())
-            self.assertTrue(isinstance(p, cls.point2))
-
-        def test_types_point2_to_bytes_from_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            bs = cls.point2.random().to_bytes()
-            self.assertTrue(isinstance(cls.point2.from_bytes(bs), cls.point2))
-
-        def test_types_point2_hex_fromhex(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.point2.random().hex()
-            self.assertTrue(isinstance(cls.point2.fromhex(s), cls.point2))
-
-        def test_types_point2_to_base64_from_base64(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.point2.random().to_base64()
-            self.assertTrue(isinstance(cls.point2.from_base64(s), cls.point2))
-
-        def test_types_point2_canonical(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            p = cls.point2.base(cls.scalar.random())
-            self.assertTrue(isinstance(p.canonical(), cls.point2))
-
-        def test_types_point2_mul(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(SCALAR_LEN + POINT_HASH_LEN, limit=1)
-            (s, p) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.point2.hash(bs[SCALAR_LEN:]))
-            self.assertTrue(isinstance(s * p, cls.point2))
-
-        def test_types_point2_add(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
-            (p0, p1) = (cls.point2.hash(bs[:POINT_HASH_LEN]), cls.point2.hash(bs[POINT_HASH_LEN:]))
-            self.assertTrue(isinstance(p0 + p1, cls.point2))
-
-        def test_types_point2_sub(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
-            (p0, p1) = (cls.point2.hash(bs[:POINT_HASH_LEN]), cls.point2.hash(bs[POINT_HASH_LEN:]))
-            self.assertTrue(isinstance(p0 - p1, cls.point2))
-
-        def test_types_point2_neg(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN, limit=1)
-            self.assertTrue(isinstance(-cls.point2.hash(bs), cls.point2))
-
-        def test_types_scalar2_random(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            self.assertTrue(isinstance(cls.scalar2.random(), cls.scalar2))
-
-        def test_types_scalar2_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            bs = cls.scalar2.random().to_bytes()
-            self.assertTrue(isinstance(cls.scalar2.bytes(bs), cls.scalar2))
-
-        def test_types_scalar2_hash(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(SCALAR2_LEN, limit=1)
-            self.assertTrue(isinstance(cls.scalar2.hash(bs), cls.scalar2))
-
-        def test_types_scalar2_to_bytes_from_bytes(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            bs = cls.scalar2.random().to_bytes()
-            self.assertTrue(isinstance(cls.scalar2.from_bytes(bs), cls.scalar2))
-
-        def test_types_scalar2_hex_fromhex(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar2.random().hex()
-            self.assertTrue(isinstance(cls.scalar2.fromhex(s), cls.scalar2))
-
-        def test_types_scalar2_to_base64_from_base64(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar2.random().to_base64()
-            self.assertTrue(isinstance(cls.scalar2.from_base64(s), cls.scalar2))
-
-        def test_types_scalar2_invert(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            self.assertTrue(isinstance(~cls.scalar2.random(), cls.scalar2))
-
-        def test_types_scalar2_mul_scalar2(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (s0, s1) = (cls.scalar2.random(), cls.scalar2.random())
-            self.assertTrue(isinstance(s0 * s1, cls.scalar2))
-
-        def test_types_scalar2_add_scalar2(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            (s0, s1) = (cls.scalar2.random(), cls.scalar2.random())
-            self.assertTrue(isinstance(s0 + s1, cls.scalar2))
-
-    class Test_algebra(TestCase):
-        """
-        Tests of common algebraic properties of low-level operations (for all classes).
-        """
-        def test_algebra_point_add_commute(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point.hash(bs[:POINT_HASH_LEN]),
-                    cls.point.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.add(p0, p1), cls.add(p1, p0))
-
-        def test_algebra_point_add_sub_cancel(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point.hash(bs[:POINT_HASH_LEN]),
-                    cls.point.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.add(cls.sub(p0, p1), p1), p0)
-
-        def test_algebra_point_add_neg_cancel(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point.hash(bs[:POINT_HASH_LEN]),
-                    cls.point.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.add(cls.neg(p0), cls.add(p0, p1)), p1)
-
-        def test_algebra_point_neg_neg_cancel(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                p = cls.point.hash(bs[:POINT_HASH_LEN])
-                self.assertEqual(cls.neg(cls.neg(p)), p)
-
-        def test_algebra_point_add_neg_sub_identity(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point.hash(bs[:POINT_HASH_LEN]),
-                    cls.point.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.add(p0, cls.neg(p1)), cls.sub(p0, p1))
-
-        def test_algebra_point_identity(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                z = cls.point.base(cls.scalar.from_int(0))
-                p = cls.point.hash(bs)
-                self.assertEqual(cls.add(z, p), p)
-                self.assertEqual(cls.add(p, z), p)
-
-        def test_algebra_scalar_inverse_inverse_cancel(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN, limit=TRIALS_PER_TEST):
-                s = cls.scalar.hash(bs)
-                self.assertEqual(cls.inv(cls.inv(s)), s)
-
-        def test_algebra_scalar_inverse_identity(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN, limit=TRIALS_PER_TEST):
-                s = cls.scalar.hash(bs)
-                self.assertEqual(cls.inv(cls.inv(s)), s)
-
-        def test_algebra_scalar_inverse_mul_cancel(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (s, p) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.point.hash(bs[SCALAR_LEN:])
-                )
-                self.assertEqual(cls.mul(cls.inv(s), cls.mul(s, p)), p)
-
-        def test_algebra_scalar_mul_point_scalar_zero(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                z = cls.point.base(cls.scalar.from_int(0))
-                p = cls.point.hash(bs)
-                self.assertEqual(cls.mul(cls.scalar.from_int(0), p), z)
-
-        def test_algebra_scalar_mul_point_scalar_identity(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                p = cls.point.hash(bs)
-                self.assertEqual(cls.mul(cls.scalar.from_int(1), p), p)
-
-        def test_algebra_scalar_mul_point_mul_commute(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains((2 * SCALAR_LEN) + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (s0, s1, p0) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
-                    cls.point.hash(bs[SCALAR_LEN + SCALAR_LEN:])
-                )
-                self.assertEqual(
-                    cls.mul(s0, cls.mul(s1, p0)),
-                    cls.mul(s1, cls.mul(s0, p0))
-                )
-
-        def test_algebra_scalar_add_commute(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN + SCALAR_LEN, limit=TRIALS_PER_TEST):
-                (s0, s1) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.scalar.hash(bs[SCALAR_LEN:])
-                )
-                self.assertEqual(cls.sad(s0, s1), cls.sad(s1, s0))
-
-        def test_algebra_scalar_add_neg_add_identity(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN + SCALAR_LEN, limit=TRIALS_PER_TEST):
-                (s0, s1) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.scalar.hash(bs[SCALAR_LEN:])
-                )
-                self.assertEqual(cls.sad(cls.sad(s0, cls.sne(s0)), s1), s1)
-
-        def test_algebra_scalar_mul_point_mul_associate(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN + SCALAR_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (s0, s1, p0) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
-                    cls.point.hash(bs[SCALAR_LEN + SCALAR_LEN:])
-                )
-                self.assertEqual(
-                    cls.mul(s0, cls.mul(s1, p0)),
-                    cls.mul(cls.smu(s0, s1), p0)
-                )
-
-        def test_algebra_scalar_mul_point_add_distribute(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN + (2 * POINT_HASH_LEN), limit=TRIALS_PER_TEST):
-                (s0, p0, p1) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.point.hash(bs[SCALAR_LEN: SCALAR_LEN + POINT_HASH_LEN]),
-                    cls.point.hash(bs[SCALAR_LEN + POINT_HASH_LEN:])
-                )
-                self.assertEqual(
-                    cls.add(cls.mul(s0, p0), cls.mul(s0, p1)),
-                    cls.mul(s0, cls.add(p0, p1))
-                )
-
-        def test_algebra_scalar_mul_scalar_on_right_hand_side_of_non_scalar(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar.random()
-            self.assertRaises(TypeError, lambda: bytes([0]) * s)
-
-        def test_algebra_scalar_mul_point_on_left_hand_side(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar.random()
-            p = cls.point.hash(bytes(POINT_LEN))
-            self.assertRaises(TypeError, lambda: p * s)
-
-        def test_algebra_point2_add_commute(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point2.hash(bs[:POINT_HASH_LEN]),
-                    cls.point2.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.can2(cls.add2(p0, p1)), cls.can2(cls.add2(p1, p0)))
-
-        def test_algebra_point2_add_sub_cancel(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point2.hash(bs[:POINT_HASH_LEN]),
-                    cls.point2.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.add2(cls.sub2(p0, p1), p1), p0)
-
-        def test_algebra_point2_add_neg_cancel(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point2.hash(bs[:POINT_HASH_LEN]),
-                    cls.point2.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.add2(cls.neg2(p0), cls.add2(p0, p1)), p1)
-
-        def test_algebra_point2_neg_neg_cancel(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                p = cls.point2.hash(bs[:POINT_HASH_LEN])
-                self.assertEqual(cls.neg2(cls.neg2(p)), p)
-
-        def test_algebra_point2_add_neg_sub_identity(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point2.hash(bs[:POINT_HASH_LEN]),
-                    cls.point2.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.add2(p0, cls.neg2(p1)), cls.sub2(p0, p1))
-
-        def test_algebra_point2_identity(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                z = cls.point2.base(cls.scalar.from_int(0))
-                p = cls.point2.hash(bs)
-                self.assertEqual(cls.add2(z, p), p)
-                self.assertEqual(cls.add2(p, z), p)
-
-        def test_algebra_scalar_mul_point2_mul_commute(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains((2 * SCALAR_LEN) + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (s0, s1, p0) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
-                    cls.point2.hash(bs[SCALAR_LEN + SCALAR_LEN:])
-                )
-                self.assertEqual(
-                    cls.mul(s0, cls.mul2(s1, p0)),
-                    cls.mul(s1, cls.mul2(s0, p0))
-                )
-
-        def test_algebra_scalar_mul_point2_mul_associate(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN + SCALAR_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (s0, s1, p0) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
-                    cls.point2.hash(bs[SCALAR_LEN + SCALAR_LEN:])
-                )
-                self.assertEqual(
-                    cls.mul2(s0, cls.mul2(s1, p0)),
-                    cls.mul2(cls.smu(s0, s1), p0)
-                )
-
-        def test_algebra_scalar_mul_point2_add_distribute(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN + (2 * POINT_HASH_LEN), limit=TRIALS_PER_TEST):
-                (s0, p0, p1) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.point2.hash(bs[SCALAR_LEN: SCALAR_LEN + POINT_HASH_LEN]),
-                    cls.point2.hash(bs[SCALAR_LEN + POINT_HASH_LEN:])
-                )
-                self.assertEqual(
-                    cls.add2(cls.mul2(s0, p0), cls.mul2(s0, p1)),
-                    cls.mul2(s0, cls.add2(p0, p1))
-                )
-
-        def test_algebra_scalar_mul_point2_on_left_hand_side(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar.random()
-            p = cls.point2.hash(bytes(POINT2_LEN))
-            self.assertRaises(TypeError, lambda: p * s)
-
-        def test_algebra_scalar2_inverse_inverse_cancel(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR2_LEN, limit=TRIALS_PER_TEST):
-                s = cls.scalar2.hash(bs)
-                self.assertEqual(cls.inv2(cls.inv2(s)), s)
-
-        def test_algebra_scalar2_inverse_identity(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN, limit=TRIALS_PER_TEST):
-                s = cls.scalar2.hash(bs)
-                self.assertEqual(cls.inv2(cls.inv2(s)), s)
-
-        def test_algebra_scalar2_mul_commute(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR2_LEN + SCALAR2_LEN, limit=TRIALS_PER_TEST):
-                (s0, s1) = (
-                    cls.scalar2.hash(bs[:SCALAR2_LEN]),
-                    cls.scalar2.hash(bs[SCALAR2_LEN:])
-                )
-                self.assertEqual(cls.smu2(s0, s1), cls.smu2(s1, s0))
-
-        def test_algebra_scalar2_mul_inverse_mul_identity(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR2_LEN + SCALAR2_LEN, limit=TRIALS_PER_TEST):
-                (s0, s1) = (
-                    cls.scalar2.hash(bs[:SCALAR2_LEN]),
-                    cls.scalar2.hash(bs[SCALAR2_LEN:])
-                )
-                self.assertEqual(cls.smu2(cls.smu2(s0, cls.inv2(s0)), s1), s1)
-
-        def test_algebra_scalar2_add_commute(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR2_LEN + SCALAR2_LEN, limit=TRIALS_PER_TEST):
-                (s0, s1) = (
-                    cls.scalar2.hash(bs[:SCALAR2_LEN]),
-                    cls.scalar2.hash(bs[SCALAR2_LEN:])
-                )
-                self.assertEqual(cls.sad2(s0, s1), cls.sad2(s1, s0))
-
-        def test_algebra_scalar2_mul_scalar_on_right_hand_side_of_non_scalar(self):
-            mcl_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar2.random()
-            self.assertRaises(TypeError, lambda: bytes([0]) * s)
-
-    # Remove tests for functions/methods for which no pure-Python implementation
-    # exists.
-    if cls == bn254.python:
-        delattr(Test_primitives, 'test_par')
-        delattr(Test_classes, 'test_point_pair')
-        delattr(Test_types, 'test_types_point_point2_matmul')
-
-    return (
-        Test_primitives,
-        Test_classes,
-        Test_types,
-        Test_algebra
-    )
-
-# The instantiated test classes below are discovered by the testing framework and
-# executed in alphabetical order.
-(
-    Test_primitives_python_no_mcl,
-    Test_classes_python_no_mcl,
-    Test_types_python_no_mcl,
-    Test_algebra_python_no_mcl
-) = define_classes(bn254.python, hidden=True)
-
-if bn254.mcl is not None and bn254.mclbn256 is True:
-    (
-        Test_primitives_mcl_mclbn256_no_mcl,
-        Test_classes_mcl_mclbn256_no_mcl,
-        Test_types_mcl_mclbn256_no_mcl,
-        Test_algebra_mcl_mclbn256_no_mcl
-    ) = define_classes(bn254.mcl, fallback=True)
-
-(Test_primitives_python, Test_classes_python, Test_types_python, Test_algebra_python) = \
-    define_classes(bn254.python)
-
-if bn254.mcl is not None:
-    (Test_primitives_mcl, Test_classes_mcl, Test_types_mcl, Test_algebra_mcl) = \
-        define_classes(bn254.mcl)
-
-if __name__ == "__main__":
-    # Generate reference bit lists for tests.
-    implementation_test_ensembles = (
-        [Test_primitives_python(), Test_classes_python()]
-        if bn254.mcl is None else
-        [Test_primitives_mcl(), Test_classes_mcl()]
-    )
-
-    for tests in implementation_test_ensembles:
-        print(
-            '\nUnit test reference bit vectors for ' +
-            tests.__class__.__name__ + ' methods...'
-        )
-        for m in [m for m in dir(tests) if m.startswith('test_')]:
-            method = getattr(tests, m)
-            if 'bits' in method.__code__.co_varnames:
-                print('* ' + m + ": '" + method(bits=None) + "'")
+"""
+Test suite containing functional unit tests for the exported primitives and
+classes in the :obj:`oblivious.bn254` module, as well as unit tests
+confirming algebraic relationships among primitives.
+"""
+# pylint: disable=missing-function-docstring
+from unittest import TestCase
+import importlib
+import base64
+from bitlist import bitlist
+from fountains import fountains
+
+try:
+    from oblivious import bn254 # pylint: disable=import-error
+except: # pylint: disable=bare-except
+    # To support generation of reference specifications for unit tests.
+    spec = importlib.util.spec_from_file_location("bn254", "src/oblivious/bn254.py")
+    bn254 = importlib.util.module_from_spec(spec)
+    spec.loader.exec_module(bn254)
+
+# Constants for the number of input-output pairs to include in each test and for
+# representation sizes of data structures (in their binary form).
+TRIALS_PER_TEST = 16
+POINT_HASH_LEN = 64 # Size of raw hash digest required to construct a point.
+POINT_LEN = 32 * 3 # Three 32-byte coordinate values (*x*, *y*, and *z* in projective coordinates).
+POINT2_LEN = 192
+SCALAR_LEN = 32
+SCALAR2_LEN = 384
+
+# To simulate an environment in which the mcl library is absent, some tests set
+# ``bn254.mcl`` to ``None``; the references below are used for restoration.
+mcl_restore = bn254.mcl
+
+def api_functions():
+    """
+    Low-level functions that should be available to users within each of the two
+    namespaces.
+    """
+    return {
+        'pnt', 'bas', 'can', 'ser', 'des', 'mul', 'add', 'sub', 'neg', 'par',
+        'rnd', 'scl', 'sse', 'sde', 'inv', 'smu', 'sad', 'ssu', 'sne',
+        'pnt2', 'bas2', 'can2', 'ser2', 'des2', 'mul2', 'add2', 'sub2', 'neg2',
+        'rnd2', 'scl2', 'sse2', 'sde2', 'inv2', 'smu2', 'sad2'
+    }
+
+def api_classes():
+    """
+    Classes that should be available to users upon module import.
+    """
+    return {'point', 'scalar', 'point2', 'scalar2'}
+
+class Test_namespace(TestCase):
+    """
+    Check that namespaces provide access to the expected
+    classes and functions.
+    """
+    def test_init(self):
+        init = importlib.import_module('oblivious.__init__')
+        self.assertTrue('bn254' in init.__dict__)
+
+    def test_modules(self):
+        module = importlib.import_module('oblivious.bn254')
+        self.assertTrue('python' in module.__dict__)
+        self.assertTrue('mcl' in module.__dict__)
+        self.assertTrue(api_classes().issubset(module.__dict__.keys()))
+
+    def test_python(self):
+        self.assertTrue(
+            (api_functions() - {'par'}).issubset(set(dir(bn254.python)))
+        )
+        self.assertTrue(api_classes().issubset(set(dir(bn254.python))))
+
+    def test_mcl(self):
+        if bn254.mcl is not None:
+            self.assertTrue(api_functions().issubset(set(dir(bn254.mcl))))
+            self.assertTrue(api_classes().issubset(set(dir(bn254.mcl))))
+
+def check_or_generate_operation(test, fun, lengths, bits):
+    """
+    This function does either of two things depending on the parameter ``bits``:
+    * checks that test inputs drawn from the :obj:`fountains` input bit stream
+      produce the bits provided in the reference output bit vector, or
+    * generates a reference output bit vector by applying the function
+      to the :obj:`fountains` input bit stream.
+    """
+    def get_bytes(o):
+        if type(o) in (bytes, bytearray, bitlist):
+            return o
+
+        cls = bn254.python if isinstance(o, bytes) else bn254.mcl
+
+        # Transform points to canonical form.
+        cls_str = str(o.__class__)
+        if 'point2' in cls_str or 'G2' in cls_str:
+            o = cls.can2(o)
+        elif 'point' in cls_str or 'G1' in cls_str:
+            o = cls.can(o)
+
+        return (
+            cls.ser(o)
+            if ('point' in str(o.__class__) or 'G' in str(o.__class__)) else
+            cls.sse(o)
+        )
+
+    fs = fountains( # Generate the input bit stream.
+        sum(lengths),
+        seed=bytes(0), # This is also the default; explicit for clarity.
+        limit=min(TRIALS_PER_TEST, (len(bits) * 4) if bits is not None else 256),
+        bits=bits[:(TRIALS_PER_TEST // 4)] if bits is not None else None,
+        function=lambda *args, **kwargs: get_bytes(fun(*args, **kwargs))
+    )
+
+    if bits is None: # There is no output reference bit vector, so test is not possible.
+        return bitlist(list(fs)).hex() # Return reference output bits for test.
+
+    test.assertTrue(all(fs)) # Check that all outputs match.
+
+def mcl_hidden_and_fallback(hidden=False, fallback=False):
+    """
+    Return binary wrapper class definition that conforms to the
+    scenario being tested.
+    """
+    if hidden:
+        bn254.mcl = None
+    elif fallback:
+        bn254.mcl = mcl_restore
+    else:
+        bn254.mcl = mcl_restore
+
+def define_classes(cls, hidden=False, fallback=False): # pylint: disable=too-many-statements
+    """
+    Define and return four classes of unit tests given a wrapper
+    class (``python`` or ``mcl``) for primitive operations.
+    """
+    class Test_primitives(TestCase):
+        """
+        Direct tests of primitive operators that operate on bytes-like objects.
+        """
+        def test_pnt(
+                self,
+                bits='bc3d'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.pnt, [POINT_HASH_LEN], bits)
+
+        def test_pnt_none(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                self.assertTrue(len(cls.ser(cls.pnt())) == POINT_LEN)
+
+        def test_bas(
+                self,
+                bits='82d6'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00111111 # Improve chance of testing with a valid scalar.
+                bs = bytes(bs)
+                s = cls.scl(bs)
+                return cls.bas(s) if s is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_can(
+                self,
+                bits='bc3d'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.can(cls.pnt(bs))
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_ser(
+                self,
+                bits='bc3d'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.ser(cls.pnt(bs))
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_des(
+                self,
+                bits='bc3d'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.des(cls.ser(cls.pnt(bs)))
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_mul(
+                self,
+                bits='b9e1'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00111111 # Improve chance of testing with a valid scalar.
+                bs[SCALAR_LEN - 1] &= 0b00011111
+                bs = bytes(bs)
+                (s, p) = (cls.scl(bs[:SCALAR_LEN]), cls.pnt(bs[SCALAR_LEN:]))
+                return cls.mul(s, p) if (s is not None and p is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
+
+        def test_add(
+                self,
+                bits='40d9'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (cls.pnt(bs[:POINT_HASH_LEN]), cls.pnt(bs[POINT_HASH_LEN:]))
+                return cls.add(p1, p2) if (p1 is not None and p2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_sub(
+                self,
+                bits='71df'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (cls.pnt(bs[:POINT_HASH_LEN]), cls.pnt(bs[POINT_HASH_LEN:]))
+                return cls.sub(p1, p2) if (p1 is not None and p2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_neg(
+                self,
+                bits='bc3d'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.neg(cls.pnt(bs))
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_par(
+                self,
+                bits='49f2'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (cls.point.hash(bs), cls.point2.hash(bs))
+                return cls.sse2(cls.par(p1, p2))
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_rnd(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.rnd()
+                self.assertTrue(cls.scl(bytes(s)))
+
+        def test_scl(
+                self,
+                bits='ffff'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00111111 # Improve chances of testing with a valid scalar.
+                bs = bytes(bs)
+                r = 0x2523648240000001ba344d8000000007ff9f800000000010a10000000000000d
+                return bitlist([
+                    1
+                    if (bool(cls.scl(bs)) == (int.from_bytes(bs, 'little') < r)) is not None else
+                    0
+                ])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_scl_none(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                bs = bytes([255] * 32) # Representation value above the maximum scalar value.
+                s = cls.scl(bs)
+                self.assertTrue(s is None)
+
+        def test_sse(
+                self,
+                bits='ab29'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
+                s = cls.scl(bytes(bs))
+                return cls.sse(s) if s is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_sde(
+                self,
+                bits='ab29'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
+                s = cls.scl(bytes(bs))
+                return cls.sde(cls.sse(s)) if s is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_inv(
+                self,
+                bits='0aea'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
+                bs = bytes(bs)
+                s = cls.scl(bs)
+                return cls.inv(s) if s is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_smu(
+                self,
+                bits='dfad'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
+                bs[SCALAR_LEN - 1] &= 0b00011111
+                bs = bytes(bs)
+                (s1, s2) = (cls.scl(bs[:SCALAR_LEN]), cls.scl(bs[SCALAR_LEN:]))
+                return cls.smu(s1, s2) if (s1 is not None and s2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
+
+        def test_sad(
+                self,
+                bits='6c5b'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
+                bs[SCALAR_LEN - 1] &= 0b00011111
+                bs = bytes(bs)
+                (s1, s2) = (cls.scl(bs[:SCALAR_LEN]), cls.scl(bs[SCALAR_LEN:]))
+                return cls.sad(s1, s2) if (s1 is not None and s2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
+
+        def test_ssu(
+                self,
+                bits='dc34'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
+                bs[SCALAR_LEN - 1] &= 0b00011111
+                bs = bytes(bs)
+                (s1, s2) = (cls.scl(bs[:SCALAR_LEN]), cls.scl(bs[SCALAR_LEN:]))
+                return cls.ssu(s1, s2) if (s1 is not None and s2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
+
+        def test_sne(
+                self,
+                bits='66d6'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
+                bs = bytes(bs)
+                s = cls.scl(bs)
+                return cls.sne(s) if s is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_pnt2(
+                self,
+                bits='d28c'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.pnt2, [POINT_HASH_LEN], bits)
+
+        def test_bas2(
+                self,
+                bits='1ed0'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.bas2(cls.scalar.hash(bs))
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_can2(
+                self,
+                bits='d28c'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.ser2(cls.can2(cls.pnt2(bs)))
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_ser2(
+                self,
+                bits='d28c'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.ser2(cls.can2(cls.pnt2(bs)))
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_des2(
+                self,
+                bits='d28c'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.des2(cls.ser2(cls.can2(cls.pnt2(bs))))
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_mul2(
+                self,
+                bits='1e5c'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (s, p) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.pnt2(bs[SCALAR_LEN:]))
+                return cls.mul2(s, p)
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
+
+        def test_add2(
+                self,
+                bits='424e'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (cls.pnt2(bs[:POINT_HASH_LEN]), cls.pnt2(bs[POINT_HASH_LEN:]))
+                return cls.add2(p1, p2)
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_sub2(
+                self,
+                bits='15c9'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (cls.pnt2(bs[:POINT_HASH_LEN]), cls.pnt2(bs[POINT_HASH_LEN:]))
+                return cls.sub2(p1, p2)
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_neg2(
+                self,
+                bits='d28c'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.neg2(cls.pnt2(bs))
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_rnd2(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.rnd2()
+                self.assertTrue(cls.scl2(bytes(s)) is not None)
+
+        def test_scl2(
+                self,
+                bits='a567'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.sse2(cls.scl2(cls.scalar2.hash(bs).to_bytes()))
+            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
+
+        def test_sse2(
+                self,
+                bits='a567'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.sse2(cls.scalar2.hash(bs))
+            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
+
+        def test_sde2(
+                self,
+                bits='a567'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.sse2(cls.sde2(cls.sse2(cls.scalar2.hash(bs))))
+            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
+
+        def test_inv2(
+                self,
+                bits='a567'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.sse2(cls.inv2(cls.scalar2.hash(bs)))
+            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
+
+        def test_smu2(
+                self,
+                bits='ed98'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (s1, s2) = (cls.scalar2.hash(bs[:SCALAR2_LEN]), cls.scalar2.hash(bs[SCALAR2_LEN:]))
+                return cls.sse2(cls.smu2(s1, s2))
+            return check_or_generate_operation(self, fun, [SCALAR2_LEN, SCALAR2_LEN], bits)
+
+        def test_sad2(
+                self,
+                bits='1d51'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (s1, s2) = (cls.scalar2.hash(bs[:SCALAR2_LEN]), cls.scalar2.hash(bs[SCALAR2_LEN:]))
+                return cls.sse2(cls.sad2(s1, s2))
+            return check_or_generate_operation(self, fun, [SCALAR2_LEN, SCALAR2_LEN], bits)
+
+    class Test_classes(TestCase): # pylint: disable=too-many-public-methods
+        """
+        Tests of point and scalar wrapper classes and their methods.
+        """
+        def test_point_random(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                self.assertTrue(len(cls.point.random()) == POINT_LEN)
+
+        def test_point_bytes(
+                self,
+                bits='bc3d'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.point.bytes, [POINT_HASH_LEN], bits)
+
+        def test_point_hash(
+                self,
+                bits='c8ea'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.point.hash, [POINT_HASH_LEN], bits)
+
+        def test_point_base(
+                self,
+                bits='ebed'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00011111 # Improve chance of testing with a valid scalar.
+                s = cls.scalar.bytes(bytes(bs))
+                return cls.point.base(s) if s is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_point_to_bytes_from_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                p = cls.point()
+                self.assertEqual(cls.point.from_bytes(p.to_bytes()), p)
+
+        def test_point_hex_fromhex(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                p = cls.point()
+                self.assertEqual(cls.point.fromhex(p.hex()), p)
+
+        def test_point_to_base64_from_base64(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                p = cls.point()
+                p_b64 = base64.standard_b64encode(p.to_bytes()).decode('utf-8')
+                self.assertEqual(p.to_base64(), p_b64)
+                self.assertEqual(cls.point.from_base64(p.to_base64()), p)
+                self.assertEqual(cls.point.from_base64(p_b64), p)
+
+        def test_point(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                self.assertTrue(len(cls.point()) == POINT_LEN)
+
+        def test_point_canonical(
+                self,
+                bits='bc3d'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.point.bytes(bs).canonical()
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_point_scalar_mul(
+                self,
+                bits='b9e1'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00111111 # Improve chance of testing with a valid scalar.
+                bs[SCALAR_LEN - 1] &= 0b00011111
+                bs = bytes(bs)
+                (s, p) = (cls.scalar.bytes(bs[:SCALAR_LEN]), cls.point.bytes(bs[SCALAR_LEN:]))
+                # Below, ``*`` invokes :obj:`scalar.__mul__`, which delegates to :obj:`mul`
+                # due to the type of the second argument.
+                return s * p if (s is not None and p is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
+
+        def test_point_add(
+                self,
+                bits='40d9'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (
+                    cls.point.bytes(bs[:POINT_HASH_LEN]),
+                    cls.point.bytes(bs[POINT_HASH_LEN:])
+                )
+                return p1 + p2 if (p1 is not None and p2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_point_sub(
+                self,
+                bits='71df'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (
+                    cls.point.bytes(bs[:POINT_HASH_LEN]),
+                    cls.point.bytes(bs[POINT_HASH_LEN:])
+                )
+                return p1 - p2 if (p1 is not None and p2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_point_neg(
+                self,
+                bits='bc3d'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                p = cls.point.bytes(bs)
+                return -p if p is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_point_pair(
+                self,
+                bits='9cd3'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (
+                    cls.point.hash(bs[:POINT_HASH_LEN]),
+                    cls.point2.hash(bs[POINT_HASH_LEN:])
+                )
+                return p1 @ p2
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_scalar_random(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar.random()
+                self.assertTrue(cls.scalar.bytes(bytes(s)) is not None)
+                self.assertTrue(len(s) == SCALAR_LEN and len(s.to_bytes()) == SCALAR_LEN)
+
+        def test_scalar_bytes(
+                self,
+                bits='ab29'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = bytearray(bs)
+                bs[-1] &= 0b00011111 # Improve chances of testing with a valid scalar.
+                s = cls.scalar.bytes(bytes(bs))
+                return s.to_bytes() if s is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_scalar_hash(
+                self,
+                bits='1c21'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.scalar.hash, [SCALAR_LEN], bits)
+
+        def test_scalar_to_int(
+                self,
+                bits='6969'
+            ):
+            def fun(bs):
+                s = cls.scalar.hash(bs)
+                return abs(s.to_int()).to_bytes(32, 'little')
+            return check_or_generate_operation(self, fun, [32], bits)
+
+        def test_scalar_from_int(
+                self,
+                bits='d27b'
+            ):
+            def fun(bs):
+                s = cls.scalar.from_int(int.from_bytes(bs, 'little'))
+                return s if (s is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [32], bits)
+
+        def test_scalar_to_bytes_from_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar()
+                self.assertEqual(cls.scalar.from_bytes(s.to_bytes()), s)
+
+        def test_scalar_hex_fromhex(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar()
+                self.assertEqual(cls.scalar.fromhex(s.hex()), s)
+
+        def test_scalar_to_base64_from_base64(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar()
+                s_b64 = base64.standard_b64encode(s.to_bytes()).decode('utf-8')
+                self.assertEqual(s.to_base64(), s_b64)
+                self.assertEqual(cls.scalar.from_base64(s_b64), s)
+                self.assertEqual(cls.scalar.from_base64(s.to_base64()), s)
+
+        def test_scalar(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar()
+                self.assertTrue(len(s) == SCALAR_LEN and cls.scalar.bytes(bytes(s)) is not None)
+                self.assertTrue(len(bytes(s)) == SCALAR_LEN and len(s.to_bytes()) == SCALAR_LEN)
+
+        def test_scalar_invert(
+                self,
+                bits='c4e3'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                s = cls.scalar.hash(bs)
+                return ~s
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_scalar_mul(
+                self,
+                bits='93d3'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (s1, s2) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.scalar.hash(bs[SCALAR_LEN:]))
+                return s1 * s2 if (s1 is not None and s2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
+
+        def test_scalar_add(
+                self,
+                bits='debe'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                s = cls.scalar.hash(bs[SCALAR_LEN:])
+                t = cls.scalar.hash(bs[:SCALAR_LEN])
+                return s + t
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
+
+        def test_scalar_sub(
+                self,
+                bits='7fc9'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                s = cls.scalar.hash(bs[SCALAR_LEN:])
+                t = cls.scalar.hash(bs[:SCALAR_LEN])
+                return s - t
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
+
+        def test_scalar_neg(
+                self,
+                bits='a1de'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                s = cls.scalar.hash(bs)
+                return -s
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_point2_random(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                self.assertTrue(len(cls.point2.random()) == POINT2_LEN)
+
+        def test_point2_bytes(
+                self,
+                bits='d28c'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.point2.bytes, [POINT_HASH_LEN], bits)
+
+        def test_point2_hash(
+                self,
+                bits='d51b'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.point2.hash, [POINT_HASH_LEN], bits)
+
+        def test_point2_base(
+                self,
+                bits='1ed0'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.point2.base(cls.scalar.hash(bs))
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_point2_to_bytes_from_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                p = cls.point2()
+                self.assertEqual(cls.point2.from_bytes(p.to_bytes()), p)
+
+        def test_point2_hex_fromhex(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                p = cls.point2()
+                self.assertEqual(cls.point2.fromhex(p.hex()), p)
+
+        def test_point2_to_base64_from_base64(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                p = cls.point2()
+                p_b64 = base64.standard_b64encode(p.to_bytes()).decode('utf-8')
+                self.assertEqual(p.to_base64(), p_b64)
+                self.assertEqual(cls.point2.from_base64(p.to_base64()), p)
+                self.assertEqual(cls.point2.from_base64(p_b64), p)
+
+        def test_point2(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                self.assertTrue(len(cls.point2()) == POINT2_LEN)
+
+        def test_point2_canonical(
+                self,
+                bits='d28c'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.point2.bytes(bs).canonical()
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_point2_scalar_mul(
+                self,
+                bits='1e5c'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (s, p) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.point2.bytes(bs[SCALAR_LEN:]))
+                # Below, ``*`` invokes :obj:`scalar.__mul__`, which delegates to :obj:`mul`
+                # due to the type of the second argument.
+                return s * p
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
+
+        def test_point2_add(
+                self,
+                bits='424e'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (cls.point2.bytes(bs[:POINT_HASH_LEN]), cls.point2.bytes(bs[POINT_HASH_LEN:]))
+                return p1 + p2
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_point2_sub(
+                self,
+                bits='15c9'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (cls.point2.bytes(bs[:POINT_HASH_LEN]), cls.point2.bytes(bs[POINT_HASH_LEN:]))
+                return p1 - p2
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_point2_neg(
+                self,
+                bits='d28c'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return -cls.point2.bytes(bs)
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_scalar2_random(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar2.random()
+                self.assertTrue(cls.scalar2.bytes(s.to_bytes()) is not None)
+                self.assertTrue(len(s) == SCALAR2_LEN and len(s.to_bytes()) == SCALAR2_LEN)
+
+        def test_scalar2_bytes(
+                self,
+                bits='a567'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                bs = cls.scalar2.hash(bs).to_bytes()
+                s = cls.scalar2.bytes(bs)
+                return s.to_bytes()
+            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
+
+        def test_scalar2_hash(
+                self,
+                bits='a567'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.scalar2.hash, [SCALAR2_LEN], bits)
+
+        def test_scalar2_to_bytes_from_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar2()
+                self.assertEqual(cls.scalar2.from_bytes(s.to_bytes()), s)
+
+        def test_scalar2_hex_fromhex(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar2()
+                self.assertEqual(cls.scalar2.fromhex(s.hex()), s)
+
+        def test_scalar2_to_base64_from_base64(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar2()
+                s_b64 = base64.standard_b64encode(s.to_bytes()).decode('utf-8')
+                self.assertEqual(s.to_base64(), s_b64)
+                self.assertEqual(cls.scalar2.from_base64(s_b64), s)
+                self.assertEqual(cls.scalar2.from_base64(s.to_base64()), s)
+
+        def test_scalar2(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar2()
+                self.assertTrue(cls.scalar2(s.to_bytes()) is not None)
+                self.assertTrue(len(s) == SCALAR2_LEN and len(s.to_bytes()) == SCALAR2_LEN)
+
+        def test_scalar2_invert(
+                self,
+                bits='a567'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                s = cls.scalar2.hash(bs)
+                return ~s
+            return check_or_generate_operation(self, fun, [SCALAR2_LEN], bits)
+
+        def test_scalar2_mul(
+                self,
+                bits='b0f7'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (s1, s2) = (cls.scalar2.hash(bs[:SCALAR_LEN]), cls.scalar2.hash(bs[SCALAR_LEN:]))
+                return s1 * s2
+            return check_or_generate_operation(self, fun, [SCALAR2_LEN, SCALAR2_LEN], bits)
+
+        def test_scalar2_add(
+                self,
+                bits='015e'
+            ):
+            mcl_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (s1, s2) = (cls.scalar2.hash(bs[:SCALAR_LEN]), cls.scalar2.hash(bs[SCALAR_LEN:]))
+                return s1 + s2
+            return check_or_generate_operation(self, fun, [SCALAR2_LEN, SCALAR2_LEN], bits)
+
+    class Test_types(TestCase): # pylint: disable=too-many-public-methods
+        """
+        Tests verifying that methods that should return point and scalar classes
+        do indeed return point and scalar objects of the expected types.
+        """
+        def test_types_point_random(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            p = cls.point.random()
+            self.assertTrue(isinstance(p, cls.point))
+
+        def test_types_point_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN, limit=1)
+            p = cls.point.bytes(bs)
+            self.assertTrue(isinstance(p, cls.point))
+
+        def test_types_point_hash(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN, limit=1)
+            p = cls.point.hash(bs)
+            self.assertTrue(isinstance(p, cls.point))
+
+        def test_types_point_base(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            p = cls.point.base(cls.scalar.random())
+            self.assertTrue(isinstance(p, cls.point))
+
+        def test_types_point_to_bytes_from_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            bs = cls.point.random().to_bytes()
+            self.assertTrue(isinstance(cls.point.from_bytes(bs), cls.point))
+
+        def test_types_point_hex_fromhex(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.point.random().hex()
+            self.assertTrue(isinstance(cls.point.fromhex(s), cls.point))
+
+        def test_types_point_to_base64_from_base64(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.point.random().to_base64()
+            self.assertTrue(isinstance(cls.point.from_base64(s), cls.point))
+
+        def test_types_point_canonical(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            p = cls.point.base(cls.scalar.random())
+            self.assertTrue(isinstance(p.canonical(), cls.point))
+
+        def test_types_point_mul(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(SCALAR_LEN + POINT_HASH_LEN, limit=1)
+            (s, p) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.point.hash(bs[SCALAR_LEN:]))
+            self.assertTrue(isinstance(s * p, cls.point))
+
+        def test_types_point_add(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
+            (p0, p1) = (cls.point.hash(bs[:POINT_HASH_LEN]), cls.point.hash(bs[POINT_HASH_LEN:]))
+            self.assertTrue(isinstance(p0 + p1, cls.point))
+
+        def test_types_point_sub(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
+            (p0, p1) = (cls.point.hash(bs[:POINT_HASH_LEN]), cls.point.hash(bs[POINT_HASH_LEN:]))
+            self.assertTrue(isinstance(p0 - p1, cls.point))
+
+        def test_types_point_neg(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN, limit=1)
+            p = cls.point.hash(bs)
+            self.assertTrue(isinstance(-p, cls.point))
+
+        def test_types_point_point2_matmul(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
+            (p0, p1) = (cls.point.hash(bs[:POINT_HASH_LEN]), cls.point2.hash(bs[POINT_HASH_LEN:]))
+            self.assertTrue(isinstance(p0 @ p1, cls.scalar2))
+
+        def test_types_scalar_random(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            self.assertTrue(isinstance(cls.scalar.random(), cls.scalar))
+
+        def test_types_scalar_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            bs = cls.scalar.random().to_bytes()
+            self.assertTrue(isinstance(cls.scalar.bytes(bs), cls.scalar))
+
+        def test_types_scalar_hash(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(SCALAR_LEN, limit=1)
+            self.assertTrue(isinstance(cls.scalar.hash(bs), cls.scalar))
+
+        def test_types_scalar_to_int_from_int(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            n = cls.scalar.random().to_int()
+            self.assertTrue(isinstance(cls.scalar.from_int(n), cls.scalar))
+
+        def test_types_scalar_to_bytes_from_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            bs = cls.scalar.random().to_bytes()
+            self.assertTrue(isinstance(cls.scalar.from_bytes(bs), cls.scalar))
+
+        def test_types_scalar_hex_fromhex(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar.random().hex()
+            self.assertTrue(isinstance(cls.scalar.fromhex(s), cls.scalar))
+
+        def test_types_scalar_to_base64_from_base64(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar.random().to_base64()
+            self.assertTrue(isinstance(cls.scalar.from_base64(s), cls.scalar))
+
+        def test_types_scalar_invert(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            self.assertTrue(isinstance(~cls.scalar.random(), cls.scalar))
+
+        def test_types_scalar_mul_scalar(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (s0, s1) = (cls.scalar.random(), cls.scalar.random())
+            self.assertTrue(isinstance(s0 * s1, cls.scalar))
+
+        def test_types_scalar_add_scalar(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (s0, s1) = (cls.scalar.random(), cls.scalar.random())
+            self.assertTrue(isinstance(s0 + s1, cls.scalar))
+
+        def test_types_scalar_sub_scalar(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (s0, s1) = (cls.scalar.random(), cls.scalar.random())
+            self.assertTrue(isinstance(s0 - s1, cls.scalar))
+
+        def test_types_scalar_neg(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar.random()
+            self.assertTrue(isinstance(-s, cls.scalar))
+
+        def test_types_scalar_mul_point(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            self.assertTrue(isinstance(cls.scalar() * cls.point(), cls.point))
+
+        def test_types_point2_random(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            p = cls.point2.random()
+            self.assertTrue(isinstance(p, cls.point2))
+
+        def test_types_point2_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN, limit=1)
+            p = cls.point2.bytes(bs)
+            self.assertTrue(isinstance(p, cls.point2))
+
+        def test_types_point2_hash(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN, limit=1)
+            p = cls.point2.hash(bs)
+            self.assertTrue(isinstance(p, cls.point2))
+
+        def test_types_point2_base(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            p = cls.point2.base(cls.scalar.random())
+            self.assertTrue(isinstance(p, cls.point2))
+
+        def test_types_point2_to_bytes_from_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            bs = cls.point2.random().to_bytes()
+            self.assertTrue(isinstance(cls.point2.from_bytes(bs), cls.point2))
+
+        def test_types_point2_hex_fromhex(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.point2.random().hex()
+            self.assertTrue(isinstance(cls.point2.fromhex(s), cls.point2))
+
+        def test_types_point2_to_base64_from_base64(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.point2.random().to_base64()
+            self.assertTrue(isinstance(cls.point2.from_base64(s), cls.point2))
+
+        def test_types_point2_canonical(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            p = cls.point2.base(cls.scalar.random())
+            self.assertTrue(isinstance(p.canonical(), cls.point2))
+
+        def test_types_point2_mul(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(SCALAR_LEN + POINT_HASH_LEN, limit=1)
+            (s, p) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.point2.hash(bs[SCALAR_LEN:]))
+            self.assertTrue(isinstance(s * p, cls.point2))
+
+        def test_types_point2_add(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
+            (p0, p1) = (cls.point2.hash(bs[:POINT_HASH_LEN]), cls.point2.hash(bs[POINT_HASH_LEN:]))
+            self.assertTrue(isinstance(p0 + p1, cls.point2))
+
+        def test_types_point2_sub(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
+            (p0, p1) = (cls.point2.hash(bs[:POINT_HASH_LEN]), cls.point2.hash(bs[POINT_HASH_LEN:]))
+            self.assertTrue(isinstance(p0 - p1, cls.point2))
+
+        def test_types_point2_neg(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN, limit=1)
+            self.assertTrue(isinstance(-cls.point2.hash(bs), cls.point2))
+
+        def test_types_scalar2_random(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            self.assertTrue(isinstance(cls.scalar2.random(), cls.scalar2))
+
+        def test_types_scalar2_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            bs = cls.scalar2.random().to_bytes()
+            self.assertTrue(isinstance(cls.scalar2.bytes(bs), cls.scalar2))
+
+        def test_types_scalar2_hash(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(SCALAR2_LEN, limit=1)
+            self.assertTrue(isinstance(cls.scalar2.hash(bs), cls.scalar2))
+
+        def test_types_scalar2_to_bytes_from_bytes(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            bs = cls.scalar2.random().to_bytes()
+            self.assertTrue(isinstance(cls.scalar2.from_bytes(bs), cls.scalar2))
+
+        def test_types_scalar2_hex_fromhex(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar2.random().hex()
+            self.assertTrue(isinstance(cls.scalar2.fromhex(s), cls.scalar2))
+
+        def test_types_scalar2_to_base64_from_base64(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar2.random().to_base64()
+            self.assertTrue(isinstance(cls.scalar2.from_base64(s), cls.scalar2))
+
+        def test_types_scalar2_invert(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            self.assertTrue(isinstance(~cls.scalar2.random(), cls.scalar2))
+
+        def test_types_scalar2_mul_scalar2(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (s0, s1) = (cls.scalar2.random(), cls.scalar2.random())
+            self.assertTrue(isinstance(s0 * s1, cls.scalar2))
+
+        def test_types_scalar2_add_scalar2(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            (s0, s1) = (cls.scalar2.random(), cls.scalar2.random())
+            self.assertTrue(isinstance(s0 + s1, cls.scalar2))
+
+    class Test_algebra(TestCase):
+        """
+        Tests of common algebraic properties of low-level operations (for all classes).
+        """
+        def test_algebra_point_add_commute(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point.hash(bs[:POINT_HASH_LEN]),
+                    cls.point.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.add(p0, p1), cls.add(p1, p0))
+
+        def test_algebra_point_add_sub_cancel(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point.hash(bs[:POINT_HASH_LEN]),
+                    cls.point.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.add(cls.sub(p0, p1), p1), p0)
+
+        def test_algebra_point_add_neg_cancel(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point.hash(bs[:POINT_HASH_LEN]),
+                    cls.point.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.add(cls.neg(p0), cls.add(p0, p1)), p1)
+
+        def test_algebra_point_neg_neg_cancel(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                p = cls.point.hash(bs[:POINT_HASH_LEN])
+                self.assertEqual(cls.neg(cls.neg(p)), p)
+
+        def test_algebra_point_add_neg_sub_identity(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point.hash(bs[:POINT_HASH_LEN]),
+                    cls.point.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.add(p0, cls.neg(p1)), cls.sub(p0, p1))
+
+        def test_algebra_point_identity(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                z = cls.point.base(cls.scalar.from_int(0))
+                p = cls.point.hash(bs)
+                self.assertEqual(cls.add(z, p), p)
+                self.assertEqual(cls.add(p, z), p)
+
+        def test_algebra_scalar_inverse_inverse_cancel(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN, limit=TRIALS_PER_TEST):
+                s = cls.scalar.hash(bs)
+                self.assertEqual(cls.inv(cls.inv(s)), s)
+
+        def test_algebra_scalar_inverse_identity(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN, limit=TRIALS_PER_TEST):
+                s = cls.scalar.hash(bs)
+                self.assertEqual(cls.inv(cls.inv(s)), s)
+
+        def test_algebra_scalar_inverse_mul_cancel(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (s, p) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.point.hash(bs[SCALAR_LEN:])
+                )
+                self.assertEqual(cls.mul(cls.inv(s), cls.mul(s, p)), p)
+
+        def test_algebra_scalar_mul_point_scalar_zero(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                z = cls.point.base(cls.scalar.from_int(0))
+                p = cls.point.hash(bs)
+                self.assertEqual(cls.mul(cls.scalar.from_int(0), p), z)
+
+        def test_algebra_scalar_mul_point_scalar_identity(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                p = cls.point.hash(bs)
+                self.assertEqual(cls.mul(cls.scalar.from_int(1), p), p)
+
+        def test_algebra_scalar_mul_point_mul_commute(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains((2 * SCALAR_LEN) + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (s0, s1, p0) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
+                    cls.point.hash(bs[SCALAR_LEN + SCALAR_LEN:])
+                )
+                self.assertEqual(
+                    cls.mul(s0, cls.mul(s1, p0)),
+                    cls.mul(s1, cls.mul(s0, p0))
+                )
+
+        def test_algebra_scalar_add_commute(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN + SCALAR_LEN, limit=TRIALS_PER_TEST):
+                (s0, s1) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.scalar.hash(bs[SCALAR_LEN:])
+                )
+                self.assertEqual(cls.sad(s0, s1), cls.sad(s1, s0))
+
+        def test_algebra_scalar_add_neg_add_identity(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN + SCALAR_LEN, limit=TRIALS_PER_TEST):
+                (s0, s1) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.scalar.hash(bs[SCALAR_LEN:])
+                )
+                self.assertEqual(cls.sad(cls.sad(s0, cls.sne(s0)), s1), s1)
+
+        def test_algebra_scalar_mul_point_mul_associate(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN + SCALAR_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (s0, s1, p0) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
+                    cls.point.hash(bs[SCALAR_LEN + SCALAR_LEN:])
+                )
+                self.assertEqual(
+                    cls.mul(s0, cls.mul(s1, p0)),
+                    cls.mul(cls.smu(s0, s1), p0)
+                )
+
+        def test_algebra_scalar_mul_point_add_distribute(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN + (2 * POINT_HASH_LEN), limit=TRIALS_PER_TEST):
+                (s0, p0, p1) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.point.hash(bs[SCALAR_LEN: SCALAR_LEN + POINT_HASH_LEN]),
+                    cls.point.hash(bs[SCALAR_LEN + POINT_HASH_LEN:])
+                )
+                self.assertEqual(
+                    cls.add(cls.mul(s0, p0), cls.mul(s0, p1)),
+                    cls.mul(s0, cls.add(p0, p1))
+                )
+
+        def test_algebra_scalar_mul_scalar_on_right_hand_side_of_non_scalar(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar.random()
+            self.assertRaises(TypeError, lambda: bytes([0]) * s)
+
+        def test_algebra_scalar_mul_point_on_left_hand_side(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar.random()
+            p = cls.point.hash(bytes(POINT_LEN))
+            self.assertRaises(TypeError, lambda: p * s)
+
+        def test_algebra_point2_add_commute(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point2.hash(bs[:POINT_HASH_LEN]),
+                    cls.point2.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.can2(cls.add2(p0, p1)), cls.can2(cls.add2(p1, p0)))
+
+        def test_algebra_point2_add_sub_cancel(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point2.hash(bs[:POINT_HASH_LEN]),
+                    cls.point2.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.add2(cls.sub2(p0, p1), p1), p0)
+
+        def test_algebra_point2_add_neg_cancel(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point2.hash(bs[:POINT_HASH_LEN]),
+                    cls.point2.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.add2(cls.neg2(p0), cls.add2(p0, p1)), p1)
+
+        def test_algebra_point2_neg_neg_cancel(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                p = cls.point2.hash(bs[:POINT_HASH_LEN])
+                self.assertEqual(cls.neg2(cls.neg2(p)), p)
+
+        def test_algebra_point2_add_neg_sub_identity(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point2.hash(bs[:POINT_HASH_LEN]),
+                    cls.point2.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.add2(p0, cls.neg2(p1)), cls.sub2(p0, p1))
+
+        def test_algebra_point2_identity(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                z = cls.point2.base(cls.scalar.from_int(0))
+                p = cls.point2.hash(bs)
+                self.assertEqual(cls.add2(z, p), p)
+                self.assertEqual(cls.add2(p, z), p)
+
+        def test_algebra_scalar_mul_point2_mul_commute(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains((2 * SCALAR_LEN) + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (s0, s1, p0) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
+                    cls.point2.hash(bs[SCALAR_LEN + SCALAR_LEN:])
+                )
+                self.assertEqual(
+                    cls.mul(s0, cls.mul2(s1, p0)),
+                    cls.mul(s1, cls.mul2(s0, p0))
+                )
+
+        def test_algebra_scalar_mul_point2_mul_associate(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN + SCALAR_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (s0, s1, p0) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
+                    cls.point2.hash(bs[SCALAR_LEN + SCALAR_LEN:])
+                )
+                self.assertEqual(
+                    cls.mul2(s0, cls.mul2(s1, p0)),
+                    cls.mul2(cls.smu(s0, s1), p0)
+                )
+
+        def test_algebra_scalar_mul_point2_add_distribute(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN + (2 * POINT_HASH_LEN), limit=TRIALS_PER_TEST):
+                (s0, p0, p1) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.point2.hash(bs[SCALAR_LEN: SCALAR_LEN + POINT_HASH_LEN]),
+                    cls.point2.hash(bs[SCALAR_LEN + POINT_HASH_LEN:])
+                )
+                self.assertEqual(
+                    cls.add2(cls.mul2(s0, p0), cls.mul2(s0, p1)),
+                    cls.mul2(s0, cls.add2(p0, p1))
+                )
+
+        def test_algebra_scalar_mul_point2_on_left_hand_side(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar.random()
+            p = cls.point2.hash(bytes(POINT2_LEN))
+            self.assertRaises(TypeError, lambda: p * s)
+
+        def test_algebra_scalar2_inverse_inverse_cancel(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR2_LEN, limit=TRIALS_PER_TEST):
+                s = cls.scalar2.hash(bs)
+                self.assertEqual(cls.inv2(cls.inv2(s)), s)
+
+        def test_algebra_scalar2_inverse_identity(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN, limit=TRIALS_PER_TEST):
+                s = cls.scalar2.hash(bs)
+                self.assertEqual(cls.inv2(cls.inv2(s)), s)
+
+        def test_algebra_scalar2_mul_commute(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR2_LEN + SCALAR2_LEN, limit=TRIALS_PER_TEST):
+                (s0, s1) = (
+                    cls.scalar2.hash(bs[:SCALAR2_LEN]),
+                    cls.scalar2.hash(bs[SCALAR2_LEN:])
+                )
+                self.assertEqual(cls.smu2(s0, s1), cls.smu2(s1, s0))
+
+        def test_algebra_scalar2_mul_inverse_mul_identity(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR2_LEN + SCALAR2_LEN, limit=TRIALS_PER_TEST):
+                (s0, s1) = (
+                    cls.scalar2.hash(bs[:SCALAR2_LEN]),
+                    cls.scalar2.hash(bs[SCALAR2_LEN:])
+                )
+                self.assertEqual(cls.smu2(cls.smu2(s0, cls.inv2(s0)), s1), s1)
+
+        def test_algebra_scalar2_add_commute(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR2_LEN + SCALAR2_LEN, limit=TRIALS_PER_TEST):
+                (s0, s1) = (
+                    cls.scalar2.hash(bs[:SCALAR2_LEN]),
+                    cls.scalar2.hash(bs[SCALAR2_LEN:])
+                )
+                self.assertEqual(cls.sad2(s0, s1), cls.sad2(s1, s0))
+
+        def test_algebra_scalar2_mul_scalar_on_right_hand_side_of_non_scalar(self):
+            mcl_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar2.random()
+            self.assertRaises(TypeError, lambda: bytes([0]) * s)
+
+    # Remove tests for functions/methods for which no pure-Python implementation
+    # exists.
+    if cls == bn254.python:
+        delattr(Test_primitives, 'test_par')
+        delattr(Test_classes, 'test_point_pair')
+        delattr(Test_types, 'test_types_point_point2_matmul')
+
+    return (
+        Test_primitives,
+        Test_classes,
+        Test_types,
+        Test_algebra
+    )
+
+# The instantiated test classes below are discovered by the testing framework and
+# executed in alphabetical order.
+(
+    Test_primitives_python_no_mcl,
+    Test_classes_python_no_mcl,
+    Test_types_python_no_mcl,
+    Test_algebra_python_no_mcl
+) = define_classes(bn254.python, hidden=True)
+
+if bn254.mcl is not None and bn254.mclbn256 is True:
+    (
+        Test_primitives_mcl_mclbn256_no_mcl,
+        Test_classes_mcl_mclbn256_no_mcl,
+        Test_types_mcl_mclbn256_no_mcl,
+        Test_algebra_mcl_mclbn256_no_mcl
+    ) = define_classes(bn254.mcl, fallback=True)
+
+(Test_primitives_python, Test_classes_python, Test_types_python, Test_algebra_python) = \
+    define_classes(bn254.python)
+
+if bn254.mcl is not None:
+    (Test_primitives_mcl, Test_classes_mcl, Test_types_mcl, Test_algebra_mcl) = \
+        define_classes(bn254.mcl)
+
+if __name__ == "__main__":
+    # Generate reference bit lists for tests.
+    implementation_test_ensembles = (
+        [Test_primitives_python(), Test_classes_python()]
+        if bn254.mcl is None else
+        [Test_primitives_mcl(), Test_classes_mcl()]
+    )
+
+    for tests in implementation_test_ensembles:
+        print(
+            '\nUnit test reference bit vectors for ' +
+            tests.__class__.__name__ + ' methods...'
+        )
+        for m in [m for m in dir(tests) if m.startswith('test_')]:
+            method = getattr(tests, m)
+            if 'bits' in method.__code__.co_varnames:
+                print('* ' + m + ": '" + method(bits=None) + "'")
```

### Comparing `oblivious-6.0.0/test/test_ristretto.py` & `oblivious-7.0.0/test/test_ristretto.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,732 +1,732 @@
-"""
-Test suite containing functional unit tests for the exported primitives and
-classes in the :obj:`oblivious.ristretto` module, as well as unit tests
-confirming algebraic relationships among primitives.
-"""
-# pylint: disable=missing-function-docstring
-from unittest import TestCase
-import importlib
-import base64
-from bitlist import bitlist
-from fountains import fountains
-
-try:
-    from oblivious import ristretto # pylint: disable=import-error
-except: # pylint: disable=bare-except
-    # To support generation of reference specifications for unit tests.
-    spec = importlib.util.spec_from_file_location("ristretto", "src/oblivious/ristretto.py")
-    ristretto = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(ristretto)
-
-# Constants for the number of input-output pairs to include in each test and for
-# representation sizes of data structures (in their binary form).
-TRIALS_PER_TEST = 16
-POINT_HASH_LEN = 64 # Size of raw hash digest required to construct a point.
-POINT_LEN = 32
-SCALAR_LEN = 32
-
-# To simulate an environment in which sodium is absent, some tests set
-# `ristretto.sodium` to `None` or modify `ristretto.sodium._sodium`;
-# the references below are used for restoration.
-sodium_lib_restore = ristretto.sodium._lib # pylint: disable=protected-access
-sodium_restore = ristretto.sodium
-
-def api_functions():
-    """
-    Low-level functions that should be available to users within each of the two
-    namespaces.
-    """
-    return {
-        'pnt', 'bas', 'can', 'mul', 'add', 'sub', 'neg',
-        'scl', 'rnd', 'inv', 'smu'
-    }
-
-def api_classes():
-    """
-    Classes that should be available to users upon module import.
-    """
-    return {'point', 'scalar'}
-
-class Test_namespace(TestCase):
-    """
-    Check that namespaces provide access to the expected
-    classes and functions.
-    """
-    def test_init(self):
-        init = importlib.import_module('oblivious.__init__')
-        self.assertTrue('ristretto' in init.__dict__)
-
-    def test_modules(self):
-        module = importlib.import_module('oblivious.ristretto')
-        self.assertTrue('python' in module.__dict__)
-        self.assertTrue('sodium' in module.__dict__)
-        self.assertTrue(api_classes().issubset(module.__dict__.keys()))
-
-    def test_python(self):
-        self.assertTrue(api_functions().issubset(set(dir(ristretto.python))))
-        self.assertTrue(api_classes().issubset(set(dir(ristretto.python))))
-
-    def test_sodium(self):
-        if ristretto.sodium is not None:
-            self.assertTrue(api_functions().issubset(set(dir(ristretto.sodium))))
-            self.assertTrue(api_classes().issubset(set(dir(ristretto.sodium))))
-
-def check_or_generate_operation(test, fun, lengths, bits):
-    """
-    This function does either of two things depending on `bits`:
-    * checks that test inputs drawn from the fountains input bit stream
-      produce the bits provided in the reference output bit vector, or
-    * generates a reference output bit vector by applying the function
-      to the fountains input bit stream.
-    """
-    fs = fountains( # Generate the input bit stream.
-        sum(lengths),
-        seed=bytes(0), # This is also the default; explicit for clarity.
-        limit=min(TRIALS_PER_TEST, (len(bits) * 4) if bits is not None else 256),
-        bits=bits[:(TRIALS_PER_TEST // 4)] if bits is not None else None,
-        function=fun
-    )
-
-    if bits is None: # There is no output reference bit vector, so test is not possible.
-        return bitlist(list(fs)).hex() # Return reference output bits for test.
-
-    test.assertTrue(all(fs)) # Check that all outputs match.
-    return None
-
-def sodium_hidden_and_fallback(hidden=False, fallback=False):
-    """
-    Return binary wrapper class definition that conforms to the
-    scenario being tested.
-    """
-    # pylint: disable=protected-access
-    if hidden:
-        ristretto.sodium = None
-    elif fallback:
-        ristretto.sodium = sodium_restore
-        ristretto.sodium._lib = ristretto.rbcl
-        ristretto.sodium._call = ristretto.sodium._call_wrapped
-    else:
-        ristretto.sodium = sodium_restore
-        ristretto.sodium._lib = sodium_lib_restore
-        ristretto.sodium._call = ristretto.sodium._call_unwrapped
-
-def define_classes(cls, hidden=False, fallback=False): # pylint: disable=too-many-statements
-    """
-    Define and return four classes of unit tests given a wrapper
-    class (``python`` or ``sodium``) for primitive operations.
-    """
-    class Test_primitives(TestCase):
-        """
-        Direct tests of primitive operators that operate on bytes-like objects.
-        """
-        def test_pnt(
-                self,
-                bits='baf12de24e54deae0aa116816bf5eee23b1168c78e892372e08a9884de9d4c1b'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.pnt, [POINT_HASH_LEN], bits)
-
-        def test_pnt_none(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                self.assertTrue(len(cls.pnt()) == POINT_LEN)
-
-        def test_bas(
-                self,
-                bits='00386671840148d05620421002a2110aa800e289010040404cb2101c20e165a0'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                s = cls.scl(bs)
-                return cls.bas(s) if s is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_can(
-                self,
-                bits='baf12de24e54deae0aa116816bf5eee23b1168c78e892372e08a9884de9d4c1b'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                p = cls.pnt(bs)
-                return cls.can(p)
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_mul(
-                self,
-                bits='0240281c2c0429000440190404c00003082024e160cca1002800a00108100002'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (s, p) = (cls.scl(bs[:SCALAR_LEN]), cls.pnt(bs[SCALAR_LEN:]))
-                return cls.mul(s, p) if (s is not None and p is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
-
-        def test_add(
-                self,
-                bits='0ce3cd934a855c343cb16371dc8dffe999168117d8952b53ad3b5ed8af59a01f'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (cls.pnt(bs[:POINT_HASH_LEN]), cls.pnt(bs[POINT_HASH_LEN:]))
-                return cls.add(p1, p2) if (p1 is not None and p2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_sub(
-                self,
-                bits='64edf78ce6a904bfbb4184005b76b8f9614ea0aefb0f7ef00c882b155acbb968'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (cls.pnt(bs[:POINT_HASH_LEN]), cls.pnt(bs[POINT_HASH_LEN:]))
-                return cls.sub(p1, p2) if (p1 is not None and p2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_neg(
-                self,
-                bits='b286f3e258d599d88d01f2c61c19f09874e44defc3fc110d1cf2d55e4e9cd474'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                return cls.neg(cls.pnt(bs))
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_rnd(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.rnd()
-                self.assertTrue(len(s) == SCALAR_LEN and cls.scl(s))
-
-        def test_scl(
-                self,
-                bits='4df8fe738c097afa7f255b10c3ab118eeb73e38935605042ccb7581c73f1e5e9'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            fun = lambda bs: bitlist([1 if cls.scl(bs) is not None else 0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_scl_none(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scl()
-                self.assertTrue(len(s) == SCALAR_LEN and cls.scl(s))
-
-        def test_inv(
-                self,
-                bits='41c07230000960b274044a0080a8018aa0114380150000028c2700006081e1e1'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                s = cls.scl(bs)
-                return cls.inv(s) if s is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_smu(
-                self,
-                bits='2ca120487000010295804000850254008018000000008000080100008400000c'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (s1, s2) = (cls.scl(bs[:SCALAR_LEN]), cls.scl(bs[SCALAR_LEN:]))
-                return cls.smu(s1, s2) if (s1 is not None and s2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
-
-    class Test_classes(TestCase):
-        """
-        Tests of point and scalar wrapper classes and their methods.
-        """
-        def test_point_random(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                self.assertTrue(len(cls.point.random()) == POINT_LEN)
-
-        def test_point_bytes(
-                self,
-                bits='baf12de24e54deae0aa116816bf5eee23b1168c78e892372e08a9884de9d4c1b'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.point.bytes, [POINT_HASH_LEN], bits)
-
-        def test_point_hash(
-                self,
-                bits='10cb044c737b034d5755f8ba0e29432745ed4fb1a78ea22a15b2d1113492841b'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.point.hash, [POINT_HASH_LEN], bits)
-
-        def test_point_base(
-                self,
-                bits='00386671840148d05620421002a2110aa800e289010040404cb2101c20e165a0'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                s = cls.scalar.bytes(bs)
-                return cls.point.base(s) if s is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_point_to_bytes_from_bytes(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                p = cls.point()
-                self.assertEqual(cls.point.from_bytes(p.to_bytes()), p)
-
-        def test_point_hex_fromhex(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                p = cls.point()
-                self.assertEqual(cls.point.fromhex(p.hex()), p)
-
-        def test_point_to_base64_from_base64(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                p = cls.point()
-                p_b64 = base64.standard_b64encode(p.to_bytes()).decode('utf-8')
-                self.assertEqual(p.to_base64(), p_b64)
-                self.assertEqual(cls.point.from_base64(p.to_base64()), p)
-                self.assertEqual(cls.point.from_base64(p_b64), p)
-
-        def test_point(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                self.assertTrue(len(cls.point()) == POINT_LEN)
-
-        def test_point_canonical(
-                self,
-                bits='baf12de24e54deae0aa116816bf5eee23b1168c78e892372e08a9884de9d4c1b'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                p = cls.point.bytes(bs)
-                return p.canonical()
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_point_scalar_mul(
-                self,
-                bits='0240281c2c0429000440190404c00003082024e160cca1002800a00108100002'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (s, p) = (cls.scalar.bytes(bs[:SCALAR_LEN]), cls.point.bytes(bs[SCALAR_LEN:]))
-                # Below, ``*`` invokes :obj:`scalar.__mul__`, which delegates to :obj:`mul`
-                # due to the type of the second argument.
-                return s * p if (s is not None and p is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
-
-        def test_point_add(
-                self,
-                bits='0ce3cd934a855c343cb16371dc8dffe999168117d8952b53ad3b5ed8af59a01f'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (
-                    cls.point.bytes(bs[:POINT_HASH_LEN]),
-                    cls.point.bytes(bs[POINT_HASH_LEN:])
-                )
-                return p1 + p2 if (p1 is not None and p2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_point_sub(
-                self,
-                bits='64edf78ce6a904bfbb4184005b76b8f9614ea0aefb0f7ef00c882b155acbb968'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (p1, p2) = (
-                    cls.point.bytes(bs[:POINT_HASH_LEN]),
-                    cls.point.bytes(bs[POINT_HASH_LEN:])
-                )
-                return p1 - p2 if (p1 is not None and p2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
-
-        def test_point_neg(
-                self,
-                bits='b286f3e258d599d88d01f2c61c19f09874e44defc3fc110d1cf2d55e4e9cd474'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                p = cls.point.bytes(bs)
-                return -p
-            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
-
-        def test_scalar_random(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar.random()
-                self.assertTrue(len(s) == SCALAR_LEN)
-                self.assertTrue(cls.scalar.bytes(s) is not None)
-
-        def test_scalar_bytes(
-                self,
-                bits='4df8fe738c097afa7f255b10c3ab118eeb73e38935605042ccb7581c73f1e5e9'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            fun = lambda bs: bitlist([1 if cls.scalar.bytes(bs) is not None else 0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_scalar_hash(
-                self,
-                bits='09991cc13ab3799d9c05e0c75968859298977fb7b78efa2dcb6e1689e927ac0e'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            return check_or_generate_operation(self, cls.scalar.hash, [SCALAR_LEN], bits)
-
-        def test_scalar_to_int(
-                self,
-                bits='0928da0180005ae247051210c18310046141618834405000c497480453000461'
-            ):
-            def fun(bs):
-                s = cls.scalar.bytes(bs)
-                return int(s).to_bytes(32, 'little') if (s is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [32], bits)
-
-        def test_scalar_from_int(
-                self,
-                bits='ed35aa7069cffb53b6a86e5b9c4ae0e78ccc7d514dcfd672a8584e00ceacba03'
-            ):
-            def fun(bs):
-                s = cls.scalar.from_int(int.from_bytes(bs, 'little'))
-                return s if (s is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [32], bits)
-
-        def test_scalar_to_bytes_from_bytes(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar()
-                self.assertEqual(cls.point.from_bytes(s.to_bytes()), s)
-
-        def test_scalar_hex_fromhex(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar()
-                self.assertEqual(cls.scalar.fromhex(s.hex()), s)
-
-        def test_scalar_to_base64_from_base64(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar()
-                s_b64 = base64.standard_b64encode(s.to_bytes()).decode('utf-8')
-                self.assertEqual(s.to_base64(), s_b64)
-                self.assertEqual(cls.scalar.from_base64(s_b64), s)
-                self.assertEqual(cls.scalar.from_base64(s.to_base64()), s)
-
-        def test_scalar(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for _ in range(TRIALS_PER_TEST):
-                s = cls.scalar()
-                self.assertTrue(len(s) == SCALAR_LEN and cls.scalar.bytes(s) is not None)
-
-        def test_scalar_invert(
-                self,
-                bits='5dc66e5b233363b178154a0aebee957038ef1dbbad4455f332c2b7bc50886008'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                s = cls.scalar.hash(bs)
-                return ~s if s is not None else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
-
-        def test_scalar_mul(
-                self,
-                bits='e54eda3b0689089cc453b8cb6c90621ebca97462a0865811bc86087f6810da06'
-            ):
-            sodium_hidden_and_fallback(hidden, fallback)
-            def fun(bs):
-                (s1, s2) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.scalar.hash(bs[SCALAR_LEN:]))
-                return s1 * s2 if (s1 is not None and s2 is not None) else bytes([0])
-            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
-
-    class Test_types(TestCase):
-        """
-        Tests verifying that methods return objects of the appropriate type.
-        """
-        def test_types_point_random(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            p = cls.point.random()
-            self.assertTrue(isinstance(p, cls.point))
-
-        def test_types_point_bytes(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN, limit=1)
-            p = cls.point.bytes(bs)
-            self.assertTrue(isinstance(p, cls.point))
-
-        def test_types_point_hash(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN, limit=1)
-            p = cls.point.hash(bs)
-            self.assertTrue(isinstance(p, cls.point))
-
-        def test_types_point_base(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            p = cls.point.base(cls.scalar.random())
-            self.assertTrue(isinstance(p, cls.point))
-
-        def test_types_point_to_bytes_from_bytes(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            bs = cls.point.random().to_bytes()
-            self.assertTrue(isinstance(cls.point(bs), cls.point))
-
-        def test_types_point_hex_fromhex(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            s = cls.point.random().hex()
-            self.assertTrue(isinstance(cls.point.fromhex(s), cls.point))
-
-        def test_types_point_to_base64_from_base64(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            s = cls.point.random().to_base64()
-            self.assertTrue(isinstance(cls.point.from_base64(s), cls.point))
-
-        def test_types_point_canonical(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            p = cls.point.base(cls.scalar.random())
-            self.assertTrue(isinstance(p.canonical(), cls.point))
-
-        def test_types_point_mul(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(SCALAR_LEN + POINT_HASH_LEN, limit=1)
-            (s, p) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.point.hash(bs[SCALAR_LEN:]))
-            self.assertTrue(isinstance(s * p, cls.point))
-
-        def test_types_point_add(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
-            (p0, p1) = (cls.point.hash(bs[:POINT_HASH_LEN]), cls.point.hash(bs[POINT_HASH_LEN:]))
-            self.assertTrue(isinstance(p0 + p1, cls.point))
-
-        def test_types_point_sub(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
-            (p0, p1) = (cls.point.hash(bs[:POINT_HASH_LEN]), cls.point.hash(bs[POINT_HASH_LEN:]))
-            self.assertTrue(isinstance(p0 - p1, cls.point))
-
-        def test_types_point_neg(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(POINT_HASH_LEN, limit=1)
-            p = cls.point.hash(bs)
-            self.assertTrue(isinstance(-p, cls.point))
-
-        def test_types_scalar_random(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            self.assertTrue(isinstance(cls.scalar.random(), cls.scalar))
-
-        def test_types_scalar_bytes(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            bs = cls.scalar.random().to_bytes()
-            self.assertTrue(isinstance(cls.scalar.bytes(bs), cls.scalar))
-
-        def test_types_scalar_hash(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            (bs,) = fountains(SCALAR_LEN, limit=1)
-            self.assertTrue(isinstance(cls.scalar.hash(bs), cls.scalar))
-
-        def test_types_scalar_to_int_from_int(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            n = cls.scalar.random().to_int()
-            self.assertTrue(isinstance(cls.scalar.from_int(n), cls.scalar))
-
-        def test_types_scalar_to_bytes_from_bytes(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            bs = cls.scalar.random().to_bytes()
-            self.assertTrue(isinstance(cls.scalar.from_bytes(bs), cls.scalar))
-
-        def test_types_scalar_hex_fromhex(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar.random().hex()
-            self.assertTrue(isinstance(cls.scalar.fromhex(s), cls.scalar))
-
-        def test_types_scalar_to_base64_from_base64(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar.random().to_base64()
-            self.assertTrue(isinstance(cls.scalar.from_base64(s), cls.scalar))
-
-        def test_types_scalar_invert(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            self.assertTrue(isinstance(~cls.scalar.random(), cls.scalar))
-
-        def test_types_scalar_mul_scalar(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            (s0, s1) = (cls.scalar.random(), cls.scalar.random())
-            self.assertTrue(isinstance(s0 * s1, cls.scalar))
-
-        def test_types_scalar_mul_point(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            self.assertTrue(isinstance(cls.scalar() * cls.point(), cls.point))
-
-    class Test_algebra(TestCase):
-        """
-        Tests of algebraic properties of primitive operations and class methods.
-        """
-        def test_algebra_point_add_commute(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point.hash(bs[:POINT_HASH_LEN]),
-                    cls.point.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.add(p0, p1), cls.add(p1, p0))
-
-        def test_algebra_point_add_sub_cancel(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point.hash(bs[:POINT_HASH_LEN]),
-                    cls.point.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.add(cls.sub(p0, p1), p1), p0)
-
-        def test_algebra_point_add_neg_cancel(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point.hash(bs[:POINT_HASH_LEN]),
-                    cls.point.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.add(cls.neg(p0), cls.add(p0, p1)), p1)
-
-        def test_algebra_point_neg_neg_cancel(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                p = cls.point.hash(bs[:POINT_HASH_LEN])
-                self.assertEqual(cls.neg(cls.neg(p)), p)
-
-        def test_algebra_point_add_neg_sub_identity(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (p0, p1) = (
-                    cls.point.hash(bs[:POINT_HASH_LEN]),
-                    cls.point.hash(bs[POINT_HASH_LEN:])
-                )
-                self.assertEqual(cls.add(p0, cls.neg(p1)), cls.sub(p0, p1))
-
-        def test_algebra_point_identity(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                z = cls.point.base(cls.scalar.from_int(0))
-                p = cls.point.hash(bs)
-                self.assertEqual(cls.add(z, p), p)
-                self.assertEqual(cls.add(p, z), p)
-
-        def test_algebra_scalar_inverse_inverse_cancel(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN, limit=TRIALS_PER_TEST):
-                s = cls.scalar.hash(bs)
-                self.assertEqual(cls.inv(cls.inv(s)), s)
-
-        def test_algebra_scalar_inverse_identity(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN, limit=TRIALS_PER_TEST):
-                s = cls.scalar.hash(bs)
-                self.assertEqual(cls.inv(cls.inv(s)), s)
-
-        def test_algebra_scalar_inverse_mul_cancel(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (s, p) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.point.hash(bs[SCALAR_LEN:])
-                )
-                self.assertEqual(cls.mul(cls.inv(s), cls.mul(s, p)), p)
-
-        def test_algebra_scalar_mul_point_scalar_zero(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                z = cls.point.base(cls.scalar.from_int(0))
-                p = cls.point.hash(bs)
-                self.assertEqual(cls.mul(cls.scalar.from_int(0), p), z)
-
-        def test_algebra_scalar_mul_point_scalar_identity(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                p = cls.point.hash(bs)
-                self.assertEqual(cls.mul(cls.scalar.from_int(1), p), p)
-
-        def test_algebra_scalar_mul_point_mul_commute(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains((2 * SCALAR_LEN) + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (s0, s1, p0) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
-                    cls.point.hash(bs[SCALAR_LEN + SCALAR_LEN:])
-                )
-                self.assertEqual(
-                    cls.mul(s0, cls.mul(s1, p0)),
-                    cls.mul(s1, cls.mul(s0, p0))
-                )
-
-        def test_algebra_scalar_mul_point_mul_associate(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN + SCALAR_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
-                (s0, s1, p0) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
-                    cls.point.hash(bs[SCALAR_LEN + SCALAR_LEN:])
-                )
-                self.assertEqual(
-                    cls.mul(s0, cls.mul(s1, p0)),
-                    cls.mul(cls.smu(s0, s1), p0)
-                )
-
-        def test_algebra_scalar_mul_point_add_distribute(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            for bs in fountains(SCALAR_LEN + (2 * POINT_HASH_LEN), limit=TRIALS_PER_TEST):
-                (s0, p0, p1) = (
-                    cls.scalar.hash(bs[:SCALAR_LEN]),
-                    cls.point.hash(bs[SCALAR_LEN: SCALAR_LEN + POINT_HASH_LEN]),
-                    cls.point.hash(bs[SCALAR_LEN + POINT_HASH_LEN:])
-                )
-                self.assertEqual(
-                    cls.add(cls.mul(s0, p0), cls.mul(s0, p1)),
-                    cls.mul(s0, cls.add(p0, p1))
-                )
-
-        def test_algebra_scalar_mul_scalar_on_right_hand_side_of_non_scalar(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar.random()
-            self.assertRaises(TypeError, lambda: bytes([0]) * s)
-
-        def test_algebra_scalar_mul_point_on_left_hand_side(self):
-            sodium_hidden_and_fallback(hidden, fallback)
-            s = cls.scalar.random()
-            p = cls.point.hash(bytes(POINT_LEN))
-            self.assertRaises(TypeError, lambda: p * s)
-
-    return (
-        Test_primitives,
-        Test_classes,
-        Test_types,
-        Test_algebra
-    )
-
-# The instantiated test classes below are discovered by the testing framework and
-# executed in alphabetical order.
-(
-    Test_primitives_python_no_sodium,
-    Test_classes_python_no_sodium,
-    Test_types_python_no_sodium,
-    Test_algebra_python_no_sodium
-) = define_classes(ristretto.python, hidden=True)
-
-if ristretto.rbcl is not None:
-    (
-        Test_primitives_sodium_rbcl_no_sodium,
-        Test_classes_sodium_rbcl_no_sodium,
-        Test_types_sodium_rbcl_no_sodium,
-        Test_algebra_sodium_rbcl_no_sodium
-    ) = define_classes(ristretto.sodium, fallback=True)
-
-(Test_primitives_python, Test_classes_python, Test_types_python, Test_algebra_python) = \
-    define_classes(ristretto.python)
-
-(Test_primitives_sodium, Test_classes_sodium, Test_types_sodium, Test_algebra_sodium) = \
-    define_classes(ristretto.sodium)
-
-if __name__ == "__main__":
-    # Generate reference bit lists for tests.
-    for tests in [Test_primitives_python(), Test_classes_python()]:
-        print(
-            '\nUnit test reference bit vectors for ' +
-            tests.__class__.__name__ + ' methods...'
-        )
-        for m in [m for m in dir(tests) if m.startswith('test_')]:
-            method = getattr(tests, m)
-            if 'bits' in method.__code__.co_varnames:
-                print('* ' + m + ': ' + method(bits=None))
+"""
+Test suite containing functional unit tests for the exported primitives and
+classes in the :obj:`oblivious.ristretto` module, as well as unit tests
+confirming algebraic relationships among primitives.
+"""
+# pylint: disable=missing-function-docstring
+from unittest import TestCase
+import importlib
+import base64
+from bitlist import bitlist
+from fountains import fountains
+
+try:
+    from oblivious import ristretto # pylint: disable=import-error
+except: # pylint: disable=bare-except
+    # To support generation of reference specifications for unit tests.
+    spec = importlib.util.spec_from_file_location("ristretto", "src/oblivious/ristretto.py")
+    ristretto = importlib.util.module_from_spec(spec)
+    spec.loader.exec_module(ristretto)
+
+# Constants for the number of input-output pairs to include in each test and for
+# representation sizes of data structures (in their binary form).
+TRIALS_PER_TEST = 16
+POINT_HASH_LEN = 64 # Size of raw hash digest required to construct a point.
+POINT_LEN = 32
+SCALAR_LEN = 32
+
+# To simulate an environment in which sodium is absent, some tests set
+# `ristretto.sodium` to `None` or modify `ristretto.sodium._sodium`;
+# the references below are used for restoration.
+sodium_lib_restore = ristretto.sodium._lib # pylint: disable=protected-access
+sodium_restore = ristretto.sodium
+
+def api_functions():
+    """
+    Low-level functions that should be available to users within each of the two
+    namespaces.
+    """
+    return {
+        'pnt', 'bas', 'can', 'mul', 'add', 'sub', 'neg',
+        'scl', 'rnd', 'inv', 'smu'
+    }
+
+def api_classes():
+    """
+    Classes that should be available to users upon module import.
+    """
+    return {'point', 'scalar'}
+
+class Test_namespace(TestCase):
+    """
+    Check that namespaces provide access to the expected
+    classes and functions.
+    """
+    def test_init(self):
+        init = importlib.import_module('oblivious.__init__')
+        self.assertTrue('ristretto' in init.__dict__)
+
+    def test_modules(self):
+        module = importlib.import_module('oblivious.ristretto')
+        self.assertTrue('python' in module.__dict__)
+        self.assertTrue('sodium' in module.__dict__)
+        self.assertTrue(api_classes().issubset(module.__dict__.keys()))
+
+    def test_python(self):
+        self.assertTrue(api_functions().issubset(set(dir(ristretto.python))))
+        self.assertTrue(api_classes().issubset(set(dir(ristretto.python))))
+
+    def test_sodium(self):
+        if ristretto.sodium is not None:
+            self.assertTrue(api_functions().issubset(set(dir(ristretto.sodium))))
+            self.assertTrue(api_classes().issubset(set(dir(ristretto.sodium))))
+
+def check_or_generate_operation(test, fun, lengths, bits):
+    """
+    This function does either of two things depending on `bits`:
+    * checks that test inputs drawn from the fountains input bit stream
+      produce the bits provided in the reference output bit vector, or
+    * generates a reference output bit vector by applying the function
+      to the fountains input bit stream.
+    """
+    fs = fountains( # Generate the input bit stream.
+        sum(lengths),
+        seed=bytes(0), # This is also the default; explicit for clarity.
+        limit=min(TRIALS_PER_TEST, (len(bits) * 4) if bits is not None else 256),
+        bits=bits[:(TRIALS_PER_TEST // 4)] if bits is not None else None,
+        function=fun
+    )
+
+    if bits is None: # There is no output reference bit vector, so test is not possible.
+        return bitlist(list(fs)).hex() # Return reference output bits for test.
+
+    test.assertTrue(all(fs)) # Check that all outputs match.
+    return None
+
+def sodium_hidden_and_fallback(hidden=False, fallback=False):
+    """
+    Return binary wrapper class definition that conforms to the
+    scenario being tested.
+    """
+    # pylint: disable=protected-access
+    if hidden:
+        ristretto.sodium = None
+    elif fallback:
+        ristretto.sodium = sodium_restore
+        ristretto.sodium._lib = ristretto.rbcl
+        ristretto.sodium._call = ristretto.sodium._call_wrapped
+    else:
+        ristretto.sodium = sodium_restore
+        ristretto.sodium._lib = sodium_lib_restore
+        ristretto.sodium._call = ristretto.sodium._call_unwrapped
+
+def define_classes(cls, hidden=False, fallback=False): # pylint: disable=too-many-statements
+    """
+    Define and return four classes of unit tests given a wrapper
+    class (``python`` or ``sodium``) for primitive operations.
+    """
+    class Test_primitives(TestCase):
+        """
+        Direct tests of primitive operators that operate on bytes-like objects.
+        """
+        def test_pnt(
+                self,
+                bits='baf12de24e54deae0aa116816bf5eee23b1168c78e892372e08a9884de9d4c1b'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.pnt, [POINT_HASH_LEN], bits)
+
+        def test_pnt_none(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                self.assertTrue(len(cls.pnt()) == POINT_LEN)
+
+        def test_bas(
+                self,
+                bits='00386671840148d05620421002a2110aa800e289010040404cb2101c20e165a0'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                s = cls.scl(bs)
+                return cls.bas(s) if s is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_can(
+                self,
+                bits='baf12de24e54deae0aa116816bf5eee23b1168c78e892372e08a9884de9d4c1b'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                p = cls.pnt(bs)
+                return cls.can(p)
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_mul(
+                self,
+                bits='0240281c2c0429000440190404c00003082024e160cca1002800a00108100002'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (s, p) = (cls.scl(bs[:SCALAR_LEN]), cls.pnt(bs[SCALAR_LEN:]))
+                return cls.mul(s, p) if (s is not None and p is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
+
+        def test_add(
+                self,
+                bits='0ce3cd934a855c343cb16371dc8dffe999168117d8952b53ad3b5ed8af59a01f'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (cls.pnt(bs[:POINT_HASH_LEN]), cls.pnt(bs[POINT_HASH_LEN:]))
+                return cls.add(p1, p2) if (p1 is not None and p2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_sub(
+                self,
+                bits='64edf78ce6a904bfbb4184005b76b8f9614ea0aefb0f7ef00c882b155acbb968'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (cls.pnt(bs[:POINT_HASH_LEN]), cls.pnt(bs[POINT_HASH_LEN:]))
+                return cls.sub(p1, p2) if (p1 is not None and p2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_neg(
+                self,
+                bits='b286f3e258d599d88d01f2c61c19f09874e44defc3fc110d1cf2d55e4e9cd474'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                return cls.neg(cls.pnt(bs))
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_rnd(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.rnd()
+                self.assertTrue(len(s) == SCALAR_LEN and cls.scl(s))
+
+        def test_scl(
+                self,
+                bits='4df8fe738c097afa7f255b10c3ab118eeb73e38935605042ccb7581c73f1e5e9'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            fun = lambda bs: bitlist([1 if cls.scl(bs) is not None else 0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_scl_none(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scl()
+                self.assertTrue(len(s) == SCALAR_LEN and cls.scl(s))
+
+        def test_inv(
+                self,
+                bits='41c07230000960b274044a0080a8018aa0114380150000028c2700006081e1e1'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                s = cls.scl(bs)
+                return cls.inv(s) if s is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_smu(
+                self,
+                bits='2ca120487000010295804000850254008018000000008000080100008400000c'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (s1, s2) = (cls.scl(bs[:SCALAR_LEN]), cls.scl(bs[SCALAR_LEN:]))
+                return cls.smu(s1, s2) if (s1 is not None and s2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
+
+    class Test_classes(TestCase):
+        """
+        Tests of point and scalar wrapper classes and their methods.
+        """
+        def test_point_random(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                self.assertTrue(len(cls.point.random()) == POINT_LEN)
+
+        def test_point_bytes(
+                self,
+                bits='baf12de24e54deae0aa116816bf5eee23b1168c78e892372e08a9884de9d4c1b'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.point.bytes, [POINT_HASH_LEN], bits)
+
+        def test_point_hash(
+                self,
+                bits='10cb044c737b034d5755f8ba0e29432745ed4fb1a78ea22a15b2d1113492841b'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.point.hash, [POINT_HASH_LEN], bits)
+
+        def test_point_base(
+                self,
+                bits='00386671840148d05620421002a2110aa800e289010040404cb2101c20e165a0'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                s = cls.scalar.bytes(bs)
+                return cls.point.base(s) if s is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_point_to_bytes_from_bytes(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                p = cls.point()
+                self.assertEqual(cls.point.from_bytes(p.to_bytes()), p)
+
+        def test_point_hex_fromhex(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                p = cls.point()
+                self.assertEqual(cls.point.fromhex(p.hex()), p)
+
+        def test_point_to_base64_from_base64(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                p = cls.point()
+                p_b64 = base64.standard_b64encode(p.to_bytes()).decode('utf-8')
+                self.assertEqual(p.to_base64(), p_b64)
+                self.assertEqual(cls.point.from_base64(p.to_base64()), p)
+                self.assertEqual(cls.point.from_base64(p_b64), p)
+
+        def test_point(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                self.assertTrue(len(cls.point()) == POINT_LEN)
+
+        def test_point_canonical(
+                self,
+                bits='baf12de24e54deae0aa116816bf5eee23b1168c78e892372e08a9884de9d4c1b'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                p = cls.point.bytes(bs)
+                return p.canonical()
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_point_scalar_mul(
+                self,
+                bits='0240281c2c0429000440190404c00003082024e160cca1002800a00108100002'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (s, p) = (cls.scalar.bytes(bs[:SCALAR_LEN]), cls.point.bytes(bs[SCALAR_LEN:]))
+                # Below, ``*`` invokes :obj:`scalar.__mul__`, which delegates to :obj:`mul`
+                # due to the type of the second argument.
+                return s * p if (s is not None and p is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, POINT_HASH_LEN], bits)
+
+        def test_point_add(
+                self,
+                bits='0ce3cd934a855c343cb16371dc8dffe999168117d8952b53ad3b5ed8af59a01f'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (
+                    cls.point.bytes(bs[:POINT_HASH_LEN]),
+                    cls.point.bytes(bs[POINT_HASH_LEN:])
+                )
+                return p1 + p2 if (p1 is not None and p2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_point_sub(
+                self,
+                bits='64edf78ce6a904bfbb4184005b76b8f9614ea0aefb0f7ef00c882b155acbb968'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (p1, p2) = (
+                    cls.point.bytes(bs[:POINT_HASH_LEN]),
+                    cls.point.bytes(bs[POINT_HASH_LEN:])
+                )
+                return p1 - p2 if (p1 is not None and p2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN, POINT_HASH_LEN], bits)
+
+        def test_point_neg(
+                self,
+                bits='b286f3e258d599d88d01f2c61c19f09874e44defc3fc110d1cf2d55e4e9cd474'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                p = cls.point.bytes(bs)
+                return -p
+            return check_or_generate_operation(self, fun, [POINT_HASH_LEN], bits)
+
+        def test_scalar_random(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar.random()
+                self.assertTrue(len(s) == SCALAR_LEN)
+                self.assertTrue(cls.scalar.bytes(s) is not None)
+
+        def test_scalar_bytes(
+                self,
+                bits='4df8fe738c097afa7f255b10c3ab118eeb73e38935605042ccb7581c73f1e5e9'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            fun = lambda bs: bitlist([1 if cls.scalar.bytes(bs) is not None else 0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_scalar_hash(
+                self,
+                bits='09991cc13ab3799d9c05e0c75968859298977fb7b78efa2dcb6e1689e927ac0e'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            return check_or_generate_operation(self, cls.scalar.hash, [SCALAR_LEN], bits)
+
+        def test_scalar_to_int(
+                self,
+                bits='0928da0180005ae247051210c18310046141618834405000c497480453000461'
+            ):
+            def fun(bs):
+                s = cls.scalar.bytes(bs)
+                return int(s).to_bytes(32, 'little') if (s is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [32], bits)
+
+        def test_scalar_from_int(
+                self,
+                bits='ed35aa7069cffb53b6a86e5b9c4ae0e78ccc7d514dcfd672a8584e00ceacba03'
+            ):
+            def fun(bs):
+                s = cls.scalar.from_int(int.from_bytes(bs, 'little'))
+                return s if (s is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [32], bits)
+
+        def test_scalar_to_bytes_from_bytes(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar()
+                self.assertEqual(cls.point.from_bytes(s.to_bytes()), s)
+
+        def test_scalar_hex_fromhex(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar()
+                self.assertEqual(cls.scalar.fromhex(s.hex()), s)
+
+        def test_scalar_to_base64_from_base64(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar()
+                s_b64 = base64.standard_b64encode(s.to_bytes()).decode('utf-8')
+                self.assertEqual(s.to_base64(), s_b64)
+                self.assertEqual(cls.scalar.from_base64(s_b64), s)
+                self.assertEqual(cls.scalar.from_base64(s.to_base64()), s)
+
+        def test_scalar(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for _ in range(TRIALS_PER_TEST):
+                s = cls.scalar()
+                self.assertTrue(len(s) == SCALAR_LEN and cls.scalar.bytes(s) is not None)
+
+        def test_scalar_invert(
+                self,
+                bits='5dc66e5b233363b178154a0aebee957038ef1dbbad4455f332c2b7bc50886008'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                s = cls.scalar.hash(bs)
+                return ~s if s is not None else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN], bits)
+
+        def test_scalar_mul(
+                self,
+                bits='e54eda3b0689089cc453b8cb6c90621ebca97462a0865811bc86087f6810da06'
+            ):
+            sodium_hidden_and_fallback(hidden, fallback)
+            def fun(bs):
+                (s1, s2) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.scalar.hash(bs[SCALAR_LEN:]))
+                return s1 * s2 if (s1 is not None and s2 is not None) else bytes([0])
+            return check_or_generate_operation(self, fun, [SCALAR_LEN, SCALAR_LEN], bits)
+
+    class Test_types(TestCase):
+        """
+        Tests verifying that methods return objects of the appropriate type.
+        """
+        def test_types_point_random(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            p = cls.point.random()
+            self.assertTrue(isinstance(p, cls.point))
+
+        def test_types_point_bytes(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN, limit=1)
+            p = cls.point.bytes(bs)
+            self.assertTrue(isinstance(p, cls.point))
+
+        def test_types_point_hash(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN, limit=1)
+            p = cls.point.hash(bs)
+            self.assertTrue(isinstance(p, cls.point))
+
+        def test_types_point_base(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            p = cls.point.base(cls.scalar.random())
+            self.assertTrue(isinstance(p, cls.point))
+
+        def test_types_point_to_bytes_from_bytes(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            bs = cls.point.random().to_bytes()
+            self.assertTrue(isinstance(cls.point(bs), cls.point))
+
+        def test_types_point_hex_fromhex(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            s = cls.point.random().hex()
+            self.assertTrue(isinstance(cls.point.fromhex(s), cls.point))
+
+        def test_types_point_to_base64_from_base64(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            s = cls.point.random().to_base64()
+            self.assertTrue(isinstance(cls.point.from_base64(s), cls.point))
+
+        def test_types_point_canonical(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            p = cls.point.base(cls.scalar.random())
+            self.assertTrue(isinstance(p.canonical(), cls.point))
+
+        def test_types_point_mul(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(SCALAR_LEN + POINT_HASH_LEN, limit=1)
+            (s, p) = (cls.scalar.hash(bs[:SCALAR_LEN]), cls.point.hash(bs[SCALAR_LEN:]))
+            self.assertTrue(isinstance(s * p, cls.point))
+
+        def test_types_point_add(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
+            (p0, p1) = (cls.point.hash(bs[:POINT_HASH_LEN]), cls.point.hash(bs[POINT_HASH_LEN:]))
+            self.assertTrue(isinstance(p0 + p1, cls.point))
+
+        def test_types_point_sub(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=1)
+            (p0, p1) = (cls.point.hash(bs[:POINT_HASH_LEN]), cls.point.hash(bs[POINT_HASH_LEN:]))
+            self.assertTrue(isinstance(p0 - p1, cls.point))
+
+        def test_types_point_neg(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(POINT_HASH_LEN, limit=1)
+            p = cls.point.hash(bs)
+            self.assertTrue(isinstance(-p, cls.point))
+
+        def test_types_scalar_random(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            self.assertTrue(isinstance(cls.scalar.random(), cls.scalar))
+
+        def test_types_scalar_bytes(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            bs = cls.scalar.random().to_bytes()
+            self.assertTrue(isinstance(cls.scalar.bytes(bs), cls.scalar))
+
+        def test_types_scalar_hash(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            (bs,) = fountains(SCALAR_LEN, limit=1)
+            self.assertTrue(isinstance(cls.scalar.hash(bs), cls.scalar))
+
+        def test_types_scalar_to_int_from_int(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            n = cls.scalar.random().to_int()
+            self.assertTrue(isinstance(cls.scalar.from_int(n), cls.scalar))
+
+        def test_types_scalar_to_bytes_from_bytes(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            bs = cls.scalar.random().to_bytes()
+            self.assertTrue(isinstance(cls.scalar.from_bytes(bs), cls.scalar))
+
+        def test_types_scalar_hex_fromhex(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar.random().hex()
+            self.assertTrue(isinstance(cls.scalar.fromhex(s), cls.scalar))
+
+        def test_types_scalar_to_base64_from_base64(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar.random().to_base64()
+            self.assertTrue(isinstance(cls.scalar.from_base64(s), cls.scalar))
+
+        def test_types_scalar_invert(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            self.assertTrue(isinstance(~cls.scalar.random(), cls.scalar))
+
+        def test_types_scalar_mul_scalar(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            (s0, s1) = (cls.scalar.random(), cls.scalar.random())
+            self.assertTrue(isinstance(s0 * s1, cls.scalar))
+
+        def test_types_scalar_mul_point(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            self.assertTrue(isinstance(cls.scalar() * cls.point(), cls.point))
+
+    class Test_algebra(TestCase):
+        """
+        Tests of algebraic properties of primitive operations and class methods.
+        """
+        def test_algebra_point_add_commute(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point.hash(bs[:POINT_HASH_LEN]),
+                    cls.point.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.add(p0, p1), cls.add(p1, p0))
+
+        def test_algebra_point_add_sub_cancel(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point.hash(bs[:POINT_HASH_LEN]),
+                    cls.point.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.add(cls.sub(p0, p1), p1), p0)
+
+        def test_algebra_point_add_neg_cancel(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point.hash(bs[:POINT_HASH_LEN]),
+                    cls.point.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.add(cls.neg(p0), cls.add(p0, p1)), p1)
+
+        def test_algebra_point_neg_neg_cancel(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                p = cls.point.hash(bs[:POINT_HASH_LEN])
+                self.assertEqual(cls.neg(cls.neg(p)), p)
+
+        def test_algebra_point_add_neg_sub_identity(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(2 * POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (p0, p1) = (
+                    cls.point.hash(bs[:POINT_HASH_LEN]),
+                    cls.point.hash(bs[POINT_HASH_LEN:])
+                )
+                self.assertEqual(cls.add(p0, cls.neg(p1)), cls.sub(p0, p1))
+
+        def test_algebra_point_identity(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                z = cls.point.base(cls.scalar.from_int(0))
+                p = cls.point.hash(bs)
+                self.assertEqual(cls.add(z, p), p)
+                self.assertEqual(cls.add(p, z), p)
+
+        def test_algebra_scalar_inverse_inverse_cancel(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN, limit=TRIALS_PER_TEST):
+                s = cls.scalar.hash(bs)
+                self.assertEqual(cls.inv(cls.inv(s)), s)
+
+        def test_algebra_scalar_inverse_identity(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN, limit=TRIALS_PER_TEST):
+                s = cls.scalar.hash(bs)
+                self.assertEqual(cls.inv(cls.inv(s)), s)
+
+        def test_algebra_scalar_inverse_mul_cancel(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (s, p) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.point.hash(bs[SCALAR_LEN:])
+                )
+                self.assertEqual(cls.mul(cls.inv(s), cls.mul(s, p)), p)
+
+        def test_algebra_scalar_mul_point_scalar_zero(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                z = cls.point.base(cls.scalar.from_int(0))
+                p = cls.point.hash(bs)
+                self.assertEqual(cls.mul(cls.scalar.from_int(0), p), z)
+
+        def test_algebra_scalar_mul_point_scalar_identity(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                p = cls.point.hash(bs)
+                self.assertEqual(cls.mul(cls.scalar.from_int(1), p), p)
+
+        def test_algebra_scalar_mul_point_mul_commute(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains((2 * SCALAR_LEN) + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (s0, s1, p0) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
+                    cls.point.hash(bs[SCALAR_LEN + SCALAR_LEN:])
+                )
+                self.assertEqual(
+                    cls.mul(s0, cls.mul(s1, p0)),
+                    cls.mul(s1, cls.mul(s0, p0))
+                )
+
+        def test_algebra_scalar_mul_point_mul_associate(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN + SCALAR_LEN + POINT_HASH_LEN, limit=TRIALS_PER_TEST):
+                (s0, s1, p0) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.scalar.hash(bs[SCALAR_LEN: SCALAR_LEN + SCALAR_LEN]),
+                    cls.point.hash(bs[SCALAR_LEN + SCALAR_LEN:])
+                )
+                self.assertEqual(
+                    cls.mul(s0, cls.mul(s1, p0)),
+                    cls.mul(cls.smu(s0, s1), p0)
+                )
+
+        def test_algebra_scalar_mul_point_add_distribute(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            for bs in fountains(SCALAR_LEN + (2 * POINT_HASH_LEN), limit=TRIALS_PER_TEST):
+                (s0, p0, p1) = (
+                    cls.scalar.hash(bs[:SCALAR_LEN]),
+                    cls.point.hash(bs[SCALAR_LEN: SCALAR_LEN + POINT_HASH_LEN]),
+                    cls.point.hash(bs[SCALAR_LEN + POINT_HASH_LEN:])
+                )
+                self.assertEqual(
+                    cls.add(cls.mul(s0, p0), cls.mul(s0, p1)),
+                    cls.mul(s0, cls.add(p0, p1))
+                )
+
+        def test_algebra_scalar_mul_scalar_on_right_hand_side_of_non_scalar(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar.random()
+            self.assertRaises(TypeError, lambda: bytes([0]) * s)
+
+        def test_algebra_scalar_mul_point_on_left_hand_side(self):
+            sodium_hidden_and_fallback(hidden, fallback)
+            s = cls.scalar.random()
+            p = cls.point.hash(bytes(POINT_LEN))
+            self.assertRaises(TypeError, lambda: p * s)
+
+    return (
+        Test_primitives,
+        Test_classes,
+        Test_types,
+        Test_algebra
+    )
+
+# The instantiated test classes below are discovered by the testing framework and
+# executed in alphabetical order.
+(
+    Test_primitives_python_no_sodium,
+    Test_classes_python_no_sodium,
+    Test_types_python_no_sodium,
+    Test_algebra_python_no_sodium
+) = define_classes(ristretto.python, hidden=True)
+
+if ristretto.rbcl is not None:
+    (
+        Test_primitives_sodium_rbcl_no_sodium,
+        Test_classes_sodium_rbcl_no_sodium,
+        Test_types_sodium_rbcl_no_sodium,
+        Test_algebra_sodium_rbcl_no_sodium
+    ) = define_classes(ristretto.sodium, fallback=True)
+
+(Test_primitives_python, Test_classes_python, Test_types_python, Test_algebra_python) = \
+    define_classes(ristretto.python)
+
+(Test_primitives_sodium, Test_classes_sodium, Test_types_sodium, Test_algebra_sodium) = \
+    define_classes(ristretto.sodium)
+
+if __name__ == "__main__":
+    # Generate reference bit lists for tests.
+    for tests in [Test_primitives_python(), Test_classes_python()]:
+        print(
+            '\nUnit test reference bit vectors for ' +
+            tests.__class__.__name__ + ' methods...'
+        )
+        for m in [m for m in dir(tests) if m.startswith('test_')]:
+            method = getattr(tests, m)
+            if 'bits' in method.__code__.co_varnames:
+                print('* ' + m + ': ' + method(bits=None))
```


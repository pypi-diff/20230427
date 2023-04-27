# Comparing `tmp/dtsh-0.1.0a4.tar.gz` & `tmp/dtsh-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtsh-0.1.0a4.tar", last modified: Tue Nov  8 04:51:43 2022, max compression
+gzip compressed data, was "dtsh-0.1.0a6.tar", last modified: Thu Apr 27 04:55:44 2023, max compression
```

## Comparing `dtsh-0.1.0a4.tar` & `dtsh-0.1.0a6.tar`

### file list

```diff
@@ -1,37 +1,48 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-08 04:51:43.917049 dtsh-0.1.0a4/
--rw-rw-r--   0 chris     (1000) chris     (1000)    11357 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)     2610 2022-11-08 04:51:43.917049 dtsh-0.1.0a4/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1589 2022-11-08 03:56:28.000000 dtsh-0.1.0a4/README.rst
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2022-11-08 04:51:43.917049 dtsh-0.1.0a4/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)     9194 2022-11-08 03:56:28.000000 dtsh-0.1.0a4/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-08 04:51:43.917049 dtsh-0.1.0a4/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-08 04:51:43.917049 dtsh-0.1.0a4/src/dtsh/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4856 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/autocomp.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4457 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/builtin_alias.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4085 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/builtin_cat.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1758 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/builtin_cd.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4617 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/builtin_chosen.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    24317 2022-11-08 03:56:28.000000 dtsh-0.1.0a4/src/dtsh/builtin_find.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10350 2022-11-08 03:56:28.000000 dtsh-0.1.0a4/src/dtsh/builtin_ls.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4821 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/builtin_man.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1172 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/builtin_pwd.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5768 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/builtin_tree.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    15357 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/builtin_uname.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      643 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    50772 2022-11-08 03:56:28.000000 dtsh-0.1.0a4/src/dtsh/dtsh.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    22943 2022-11-08 03:56:28.000000 dtsh-0.1.0a4/src/dtsh/man.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    13541 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/session.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3311 2022-11-08 03:56:28.000000 dtsh-0.1.0a4/src/dtsh/shell.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8452 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/systools.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3550 2022-11-04 19:33:05.000000 dtsh-0.1.0a4/src/dtsh/term.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2576 2022-11-07 02:14:37.000000 dtsh-0.1.0a4/src/dtsh/theme
--rw-rw-r--   0 chris     (1000) chris     (1000)    60814 2022-11-08 03:56:28.000000 dtsh-0.1.0a4/src/dtsh/tui.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-08 04:51:43.917049 dtsh-0.1.0a4/src/dtsh.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     2610 2022-11-08 04:51:43.000000 dtsh-0.1.0a4/src/dtsh.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      681 2022-11-08 04:51:43.000000 dtsh-0.1.0a4/src/dtsh.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2022-11-08 04:51:43.000000 dtsh-0.1.0a4/src/dtsh.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2022-11-08 04:51:43.000000 dtsh-0.1.0a4/src/dtsh.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       60 2022-11-08 04:51:43.000000 dtsh-0.1.0a4/src/dtsh.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        5 2022-11-08 04:51:43.000000 dtsh-0.1.0a4/src/dtsh.egg-info/top_level.txt
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.924066 dtsh-0.1.0a6/
+-rw-r--r--   0 chris     (1000) chris     (1000)    11357 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)     2580 2023-04-27 04:55:44.924066 dtsh-0.1.0a6/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     1589 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/README.rst
+-rw-r--r--   0 chris     (1000) chris     (1000)       81 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2023-04-27 04:55:44.924066 dtsh-0.1.0a6/setup.cfg
+-rw-r--r--   0 chris     (1000) chris     (1000)     6619 2023-04-27 04:21:52.000000 dtsh-0.1.0a6/setup.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.920066 dtsh-0.1.0a6/src/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.921066 dtsh-0.1.0a6/src/devicetree/
+-rw-r--r--   0 chris     (1000) chris     (1000)      115 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/devicetree/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    73804 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/devicetree/dtlib.py
+-rw-r--r--   0 chris     (1000) chris     (1000)   110651 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/devicetree/edtlib.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5815 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/devicetree/grutils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.923066 dtsh-0.1.0a6/src/dtsh/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/src/dtsh/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4895 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/autocomp.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4277 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_alias.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4003 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_cat.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1676 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_cd.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4445 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_chosen.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    24126 2023-04-27 04:05:16.000000 dtsh-0.1.0a6/src/dtsh/builtin_find.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    10044 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_ls.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4755 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_man.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1104 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_pwd.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5637 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_tree.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    15188 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_uname.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      643 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/src/dtsh/cli.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3914 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/config.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    52057 2023-04-27 04:21:39.000000 dtsh-0.1.0a6/src/dtsh/dtsh.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    22997 2023-04-27 04:14:38.000000 dtsh-0.1.0a6/src/dtsh/man.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      989 2023-04-27 02:02:51.000000 dtsh-0.1.0a6/src/dtsh/rl.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    13355 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/session.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3351 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/shell.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     8540 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/systools.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3595 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/term.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2576 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/src/dtsh/theme
+-rw-r--r--   0 chris     (1000) chris     (1000)    60671 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/tui.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.924066 dtsh-0.1.0a6/src/dtsh.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     2580 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      879 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)      149 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       16 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/top_level.txt
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.924066 dtsh-0.1.0a6/tests/
+-rw-r--r--   0 chris     (1000) chris     (1000)     3702 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/tests/test_autocomp.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    13172 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/tests/test_dtsh.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1887 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/tests/test_shell.py
```

### Comparing `dtsh-0.1.0a4/LICENSE` & `dtsh-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a4/PKG-INFO` & `dtsh-0.1.0a6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: dtsh
-Version: 0.1.0a4
+Version: 0.1.0a6
 Summary: Shell-like interface with Zephyr devicetree and bindings
 Home-page: https://github.com/dottspina/dtsh
 Author: Chris Duf
 Author-email: chris@openmarl.org
 License: Apache License version 2.0
 Project-URL: Bug Reports, https://github.com/dottspina/dtsh/issues
 Project-URL: Source, https://github.com/dottspina/dtsh
 Keywords: devicetree,zephyr,dts,embedded
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
+Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: dist
 License-File: LICENSE
 
 ====
 dtsh
 ====
```

### Comparing `dtsh-0.1.0a4/README.rst` & `dtsh-0.1.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a4/setup.py` & `dtsh-0.1.0a6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,116 +1,74 @@
 """Project configuration (setuptools).
-
-See:
-https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#setup-args
-https://github.com/pypa/sampleproject
 """
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
-# Get the long description from the README file
 long_description = (here / "README.rst").read_text(encoding="utf-8")
 
-# Arguments marked as "Required" below must be included for upload to PyPI.
-# Fields marked as "Optional" may be commented out.
 setup(
-    # This is the name of your project. The first time you publish this
-    # package, this name will be registered for you. It will determine how
-    # users can install this project, e.g.:
-    #
-    # $ pip install sampleproject
-    #
-    # And where it will live on PyPI: https://pypi.org/project/sampleproject/
-    #
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     #
-    # Required.
     name="dtsh",
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
     #
     # See also: https://peps.python.org/pep-0440/
     #
-    # Required.
-    version="0.1.0a4",
+    version="0.1.0a6",
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     #
-    # Optional.
     description="Shell-like interface with Zephyr devicetree and bindings",
 
-    # This is an optional longer description of your project that represents
-    # the body of text which users will see when they visit PyPI.
-    #
-    # Often, this is the same as your README, so you can just read it in from
-    # that file directly (as we have already done above)
-    #
     # This field corresponds to the "Description" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#description-optional
     #
-    # Optional.
     long_description=long_description,
 
     # Denotes that our long_description is in Markdown; valid values are
     # text/plain, text/x-rst, and text/markdown
     #
     # Optional if long_description is written in reStructuredText (rst) but
     # required for plain-text or Markdown; if unspecified, "applications should
     # attempt to render [the long_description] as text/x-rst; charset=UTF-8 and
     # fall back to text/plain if it is not valid rst" (see link below)
     #
     # This field corresponds to the "Description-Content-Type" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
     #
-    # Optional (see note above).
     #long_description_content_type="text/markdown",
 
-    # This should be a valid link to your project's main homepage.
-    #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
     #
-    # Optional.
     url="https://github.com/dottspina/dtsh",
 
-    # This should be your name or the name of the organization which owns the
-    # project.
-    #
-    # Optional.
     author="Chris Duf",
-
-    # This should be a valid email address corresponding to the author listed
-    # above.
-    #
-    # Optional.
     author_email="chris@openmarl.org",
 
-    # The license argument is more typically used to indicate differences from well-known licenses.
-    #
-    # Optional.
     license="Apache License version 2.0",
 
     # Classifiers help users find your project by categorizing it.
     #
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     #
-    # Optional.
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
         "Development Status :: 3 - Alpha",
         # Indicate who your project is intended for
@@ -118,125 +76,96 @@
         "Topic :: Software Development :: Embedded Systems",
         # Pick your license as you wish
         "License :: OSI Approved :: Apache Software License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate you support Python 3. These classifiers are *not*
         # checked by 'pip install'. See instead 'python_requires' below.
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
 
-    # This field adds keywords for your project which will appear on the
-    # project page. What does your project relate to?
-    #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
     # larger catalog.
     #
-    # Optional.
     keywords="devicetree, zephyr, dts, embedded",
 
-    # When your source code is in a subdirectory under the project root, e.g.
-    # `src/`, it is necessary to specify the `package_dir` argument.
-    #
-    # Optional.
     package_dir={"": "src"},
-
-    # You can just specify package directories manually here if your project is
-    # simple. Or you can use find_packages().
-    #
-    # Alternatively, if you just want to distribute a single Python file, use
-    # the `py_modules` argument instead as follows, which will expect a file
-    # called `my_module.py` to exist:
-    #
-    #   py_modules=["my_module"],
-    #
-    # Required.
     packages=find_packages(where="src"),
 
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. See
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-    python_requires=">=3.7, <4",
+    python_requires=">=3.8, <4",
 
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     #
-    # Optional.
-    install_requires=["devicetree", "rich", "Pygments"],
+    # Requirements for both devicetree and dtsh.
+    install_requires=[
+        "PyYAML>=5.1", "rich", "Pygments",
+        # Preferred GNU readline support for macOS.
+        "gnureadline;sys_platform=='darwin'",
+    ],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
     # projects.
     #
     # Optional.
     extras_require={
+        "dev":  ["mypy", "types-PyYAML", "pyright", "pylint", "pytest"],
         "test": ["pytest"],
         "dist": ["build", "twine"],
     },
 
     # If there are data files included in your packages that need to be
     # installed, specify them here.
-    # package_data={  # Optional
-    #     "sample": ["package_data.dat"],
-    # },
     package_data={
          "dtsh": ["theme"],
     },
 
-
     # Although 'package_data' is the preferred approach, in some case you may
     # need to place data files outside of your packages. See:
     # http://docs.python.org/distutils/setupscript.html#installing-additional-files
     #
     # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
     #
     # Optional.
     # data_files=[("my_data", ["data/data_file"])],  # Optional
 
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # `pip` to create the appropriate form of executable for the target
     # platform.
     #
-    # For example, the following would provide a command called `sample` which
-    # executes the function `main` from this package when invoked:
-    #
-    # Optional.
     entry_points={
         "console_scripts": [
             "dtsh=dtsh.cli:run",
         ],
     },
 
     # List additional URLs that are relevant to your project as a dict.
     #
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     #
-    # Examples listed include a pattern for specifying where the package tracks
-    # issues, where the source is hosted, where to say thanks to the package
-    # maintainers, and where to support the project financially. The key is
-    # what's used to render the link text on PyPI.
-    #
-    # Optional.
     project_urls={
         # 'Documentation': 'https://packaging.python.org/tutorials/distributing-packages/',
         "Bug Reports": "https://github.com/dottspina/dtsh/issues",
         # "Funding": "https://donate.pypi.org",
         # "Say Thanks!": "http://saythanks.io/to/example",
         "Source": "https://github.com/dottspina/dtsh",
     },
```

### Comparing `dtsh-0.1.0a4/src/dtsh/autocomp.py` & `dtsh-0.1.0a6/src/dtsh/autocomp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Auto-completion with GNU readline for devicetree shells."""
 
-from collections import OrderedDict
+from typing import cast, Any, Dict, List
 
 from devicetree.edtlib import Node, Binding, Property
 
 from dtsh.dtsh import Dtsh, DtshCommand, DtshAutocomp
 
 
 class DevicetreeAutocomp(DtshAutocomp):
     """Devicetree shell commands auto-completion support with GNU readline.
     """
 
     # Maps completion state (strings) and model (objects).
     #
-    _autocomp_state: OrderedDict[str, object]
+    _autocomp_state: Dict[str, Any]
 
     # Autocomp mode.
     #
     _mode: int
 
     def __init__(self, shell: Dtsh) -> None:
         """Initialize the completion engine.
         """
         self._dtsh = shell
         self._mode = DtshAutocomp.MODE_ANY
-        self._autocomp_state = OrderedDict[str, object]()
+        self._autocomp_state = {}
 
     @property
     def count(self) -> int:
         """Implements DtshAutocomp.count().
         """
         return len(self._autocomp_state)
 
     @property
-    def hints(self) -> list[str]:
+    def hints(self) -> List[str]:
         """Implements DtshAutocomp.hints().
         """
         return list(self._autocomp_state.keys())
 
     @property
-    def model(self) -> list:
+    def model(self) -> List[Any]:
         """Implements DtshAutocomp.model().
         """
         return list(self._autocomp_state.values())
 
     @property
     def mode(self) -> int:
         """Implements DtshAutocomp.mode().
@@ -59,15 +59,15 @@
         """
         self._mode = DtshAutocomp.MODE_ANY
         self._autocomp_state.clear()
 
     def autocomplete(self,
                      cmdline: str,
                      prefix: str,
-                     cursor: int = 0) -> list[str]:
+                     cursor: int = 0) -> List[str]: # pyright: ignore reportUnusedVariable
         """Implements DtshAutocomp.autocomplete().
         """
         self.reset()
         cmdline_vstr = cmdline.lstrip().split()
 
         if len(cmdline_vstr) == 0:
             self._autocomp_empty_cmdline()
@@ -108,28 +108,28 @@
                 self._autocomp_state[f'-{opt.shortname}'] = opt
             elif opt.longname:
                 self._autocomp_state[f'--{opt.longname}'] = opt
 
     def _autocomp_with_params(self, cmd:DtshCommand, prefix: str) -> None:
         self._mode, model = cmd.autocomplete_param(prefix)
         if self._mode == DtshAutocomp.MODE_DT_NODE:
-            for node in list[Node](model):
+            for node in cast(List[Node], model):
                 hint = node.path
                 if node.children:
                     # Prepare auto-completion state for TABing
                     # the node's children enumeration.
                     # See readline_completions_hook(() in dtsh.session.
                     hint += '/'
                 self._autocomp_state[hint] = node
         elif self._mode == DtshAutocomp.MODE_DT_PROP:
-            for prop in list[Property](model):
+            for prop in cast(List[Property], model):
                 hint = f'{prop.node.path}${prop.name}'
                 self._autocomp_state[hint] = prop
         elif self._mode == DtshAutocomp.MODE_DT_BINDING:
-            for binding in list[Binding](model):
+            for binding in cast(List[Binding], model):
                 self._autocomp_state[binding.compatible] = binding
         elif self._mode == DtshAutocomp.MODE_DTSH_CMD:
-            for cmd in list[DtshCommand](model):
+            for cmd in cast(List[DtshCommand], model):
                 self._autocomp_state[cmd.name] = cmd
         else:
             for completion in model:
                 self._autocomp_state[str(completion)] = completion
```

### Comparing `dtsh-0.1.0a4/src/dtsh/builtin_alias.py` & `dtsh-0.1.0a6/src/dtsh/builtin_alias.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Built-in 'alias' command."""
 
 
-from typing import Tuple
+from typing import Tuple, List
 
 from rich.table import Table
 
-from dtsh.dtsh import Dtsh, DtshCommand, DtshCommandOption, DtshAutocomp, DtshVt
+from dtsh.dtsh import Dtsh, DtshCommand, DtshAutocomp, DtshVt
 from dtsh.dtsh import DtshError, DtshCommandUsageError
+from dtsh.dtsh import DtshCommandFlagLongFmt
 from dtsh.tui import DtshTui
 
 
 class DtshBuiltinAlias(DtshCommand):
     """Print defined aliases.
 
 DESCRIPTION
@@ -48,68 +49,60 @@
 """
     def __init__(self, shell: Dtsh):
         super().__init__(
             'alias',
             "print defined aliases",
             True,
             [
-                DtshCommandOption('use rich listing format', 'l', None, None),
+                DtshCommandFlagLongFmt(),
             ]
         )
         self._dtsh = shell
 
     @property
     def usage(self) -> str:
         """Overrides DtshCommand.usage().
         """
         return super().usage + ' [ALIAS]'
 
-    @property
-    def with_rich_fmt(self) -> bool:
-        return self.with_flag('-l')
-
-    def parse_argv(self, argv: list[str]) -> None:
+    def parse_argv(self, argv: List[str]) -> None:
         """Overrides DtshCommand.parse_argv().
         """
         super().parse_argv(argv)
+        if len(self._params) > 1:
+            raise DtshCommandUsageError(self, 'too many parameters')
 
     def execute(self, vt: DtshVt) -> None:
         """Implements DtshCommand.execute().
         """
-        if self.with_usage_summary:
-            vt.write(self.usage)
-            return
-        if len(self._params) > 1:
-            raise DtshCommandUsageError(self, 'too many parameters')
-
         if self._params:
             arg_aliases = [self._params[0]]
         else:
             arg_aliases = list(self._dtsh.dt_aliases.keys())
 
         if self.with_pager:
             vt.pager_enter()
-        if self.with_rich_fmt:
+        if self.with_longfmt:
             grid = self._mk_grid_aliases_rich(arg_aliases)
         else:
             grid = self._mk_grid_aliases(arg_aliases)
         vt.write(grid)
         if self.with_pager:
             vt.pager_exit()
 
-    def autocomplete_param(self, prefix: str) -> Tuple[int,list]:
+    def autocomplete_param(self, prefix: str) -> Tuple[int, List]:
         """Overrides DtshCommand.autocomplete_param().
         """
-        completions = list[str]()
+        completions: List[str] = []
         for alias in self._dtsh.dt_aliases:
             if alias.startswith(prefix) and (len(alias) > len(prefix)):
                 completions.append(alias)
         return (DtshAutocomp.MODE_ANY, completions)
 
-    def _mk_grid_aliases(self, arg_aliases: list[str]) -> Table:
+    def _mk_grid_aliases(self, arg_aliases: List[str]) -> Table:
         grid = DtshTui.mk_grid(3)
         for alias in arg_aliases:
             try:
                 node = self._dtsh.dt_aliases[alias]
             except KeyError:
                 raise DtshError(f'no such alias: {arg_aliases[0]}')
             txt_alias = DtshTui.mk_txt(alias)
@@ -118,15 +111,15 @@
             if node.status != 'okay':
                 DtshTui.txt_dim(txt_alias)
                 DtshTui.txt_dim(txt_arrow)
                 DtshTui.txt_dim(txt_path)
             grid.add_row(txt_alias, txt_arrow, txt_path)
         return grid
 
-    def _mk_grid_aliases_rich(self, arg_aliases: list[str]) -> Table:
+    def _mk_grid_aliases_rich(self, arg_aliases: List[str]) -> Table:
         grid = DtshTui.mk_grid(4)
         for alias in arg_aliases:
             try:
                 node = self._dtsh.dt_aliases[alias]
             except KeyError:
                 raise DtshError(f'no such alias: {arg_aliases[0]}')
             txt_alias = DtshTui.mk_txt(alias, DtshTui.style(DtshTui.STYLE_DT_ALIAS))
```

### Comparing `dtsh-0.1.0a4/src/dtsh/builtin_cat.py` & `dtsh-0.1.0a6/src/dtsh/builtin_cat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Built-in 'cat' command."""
 
 
-from typing import Tuple
+from typing import Tuple, List
 
 from dtsh.dtsh import Dtsh, DtshError, DtshVt, DtshCommand, DtshAutocomp
 from dtsh.dtsh import DtshCommandUsageError
 from dtsh.tui import DtNodeView, DtPropertyView
 
 
 class DtshBuiltinCat(DtshCommand):
@@ -74,30 +74,26 @@
 
     @property
     def usage(self) -> str:
         """Overrides DtshCommand.usage().
         """
         return super().usage + ' PATH'
 
-    def parse_argv(self, argv: list[str]) -> None:
+    def parse_argv(self, argv: List[str]) -> None:
         """Overrides Dtsh.parse_argv().
         """
         super().parse_argv(argv)
-
-    def execute(self, vt: DtshVt) -> None:
-        """Implements DtshCommand.execute().
-        """
-        if self.with_usage_summary:
-            vt.write(self.usage)
-            return
         if len(self._params) == 0:
             raise DtshCommandUsageError(self, 'what do you want to cat?')
         if len(self._params) > 1:
             raise DtshCommandUsageError(self, 'too many parameters')
 
+    def execute(self, vt: DtshVt) -> None:
+        """Implements DtshCommand.execute().
+        """
         if self._params:
             arg_path = self._dtsh.realpath(self._params[0])
         else:
             arg_path = self._dtsh.pwd
 
         i_prop = arg_path.rfind('$')
         if i_prop != -1:
@@ -108,15 +104,15 @@
             view = DtPropertyView(prop)
         else:
             node = self._dtsh.path2node(arg_path)
             view = DtNodeView(node, self._dtsh)
 
         view.show(vt, self.with_pager)
 
-    def autocomplete_param(self, prefix: str) -> Tuple[int,list]:
+    def autocomplete_param(self, prefix: str) -> Tuple[int, List]:
         """Overrides DtshCommand.autocomplete_param().
         """
         # <node-path> := /<node-name>/.../<node-name>
         # <node-name> := <name>[@<unit-addr>]
         # <name> may contain alphanum, and: , . _ + -
         #
         # Property names may additionaly contain ? and #.
```

### Comparing `dtsh-0.1.0a4/src/dtsh/builtin_cd.py` & `dtsh-0.1.0a6/src/dtsh/builtin_cd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Built-in 'cd' command."""
 
 
-from typing import Tuple
+from typing import List, Tuple
 from dtsh.dtsh import Dtsh, DtshVt, DtshCommand, DtshAutocomp
 from dtsh.dtsh import DtshCommandUsageError
 
 
 class DtshBuiltinCd(DtshCommand):
     """Change current working node.
 
@@ -40,33 +40,29 @@
 
     @property
     def usage(self) -> str:
         """Overrides DtshCommand.usage().
         """
         return super().usage + ' [PATH]'
 
-    def parse_argv(self, argv: list[str]) -> None:
+    def parse_argv(self, argv: List[str]) -> None:
         """Overrides Dtsh.parse_argv().
         """
         super().parse_argv(argv)
+        if len(self._params) > 1:
+            raise DtshCommandUsageError(self, 'too many parameters')
 
     def execute(self, vt: DtshVt) -> None:
         """Implements DtshCommand.execute().
         """
-        if self.with_usage_summary:
-            vt.write(self.usage)
-            return
-        if len(self._params) > 1:
-            raise DtshCommandUsageError(self, 'too many parameters')
-
         if self._params:
             arg_path = self._dtsh.realpath(self._params[0])
         else:
             arg_path = '/'
 
         self._dtsh.cd(arg_path)
 
-    def autocomplete_param(self, prefix: str) -> Tuple[int,list]:
+    def autocomplete_param(self, prefix: str) -> Tuple[int, List]:
         """Overrides DtshCommand.autocomplete_param().
         """
         return (DtshAutocomp.MODE_DT_NODE,
                 DtshAutocomp.autocomplete_with_nodes(prefix, self._dtsh))
```

### Comparing `dtsh-0.1.0a4/src/dtsh/builtin_chosen.py` & `dtsh-0.1.0a6/src/dtsh/builtin_chosen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Built-in 'chosen' command."""
 
 
-from typing import Tuple
+from typing import List, Tuple
 
 from rich.table import Table
 
-from dtsh.dtsh import Dtsh, DtshCommand, DtshCommandOption, DtshAutocomp, DtshVt
+from dtsh.dtsh import Dtsh, DtshCommand, DtshAutocomp, DtshVt
 from dtsh.dtsh import DtshError, DtshCommandUsageError
+from dtsh.dtsh import DtshCommandFlagLongFmt
 from dtsh.tui import DtshTui
 
 
 class DtshBuiltinChosen(DtshCommand):
     """Print chosen system configuration.
 
 DESCRIPTION
@@ -44,68 +45,60 @@
 """
     def __init__(self, shell: Dtsh):
         super().__init__(
             'chosen',
             "print chosen configuration",
             True,
             [
-                DtshCommandOption('use rich output', 'l', None, None),
+                DtshCommandFlagLongFmt(),
             ]
         )
         self._dtsh = shell
 
     @property
     def usage(self) -> str:
         """Overrides DtshCommand.usage().
         """
         return super().usage + ' [CHOICE]'
 
-    @property
-    def with_rich_fmt(self) -> bool:
-        return self.with_flag('-l')
-
-    def parse_argv(self, argv: list[str]) -> None:
+    def parse_argv(self, argv: List[str]) -> None:
         """Overrides DtshCommand.parse_argv().
         """
         super().parse_argv(argv)
+        if len(self._params) > 1:
+            raise DtshCommandUsageError(self, 'too many parameters')
 
     def execute(self, vt: DtshVt) -> None:
         """Implements DtshCommand.execute().
         """
-        if self.with_usage_summary:
-            vt.write(self.usage)
-            return
-        if len(self._params) > 1:
-            raise DtshCommandUsageError(self, 'too many parameters')
-
         if self._params:
             arg_chosen = [self._params[0]]
         else:
             arg_chosen = list(self._dtsh.dt_chosen.keys())
 
         if self.with_pager:
             vt.pager_enter()
-        if self.with_rich_fmt:
+        if self.with_longfmt:
             grid = self._mk_grid_chosen_rich(arg_chosen)
         else:
             grid = self._mk_grid_chosen(arg_chosen)
         vt.write(grid)
         if self.with_pager:
             vt.pager_exit()
 
-    def autocomplete_param(self, prefix: str) -> Tuple[int,list]:
+    def autocomplete_param(self, prefix: str) -> Tuple[int, List]:
         """Overrides DtshCommand.autocomplete_param().
         """
-        completions = list[str]()
+        completions: List[str] = []
         for choice in self._dtsh.dt_chosen:
             if choice.startswith(prefix) and (len(choice) > len(prefix)):
                 completions.append(choice)
         return (DtshAutocomp.MODE_ANY, completions)
 
-    def _mk_grid_chosen(self, arg_chosen: list[str]) -> Table:
+    def _mk_grid_chosen(self, arg_chosen: List[str]) -> Table:
         grid = DtshTui.mk_grid(3)
         for choice in arg_chosen:
             try:
                 node = self._dtsh.dt_chosen[choice]
             except KeyError:
                 raise DtshError(f'no such configuration choice: {arg_chosen[0]}')
             txt_choice = DtshTui.mk_txt(choice)
@@ -114,15 +107,15 @@
             if node.status != 'okay':
                 DtshTui.txt_dim(txt_choice)
                 DtshTui.txt_dim(txt_arrow)
                 DtshTui.txt_dim(txt_path)
             grid.add_row(txt_choice, txt_arrow, txt_path)
         return grid
 
-    def _mk_grid_chosen_rich(self, arg_chosen: list[str]) -> Table:
+    def _mk_grid_chosen_rich(self, arg_chosen: List[str]) -> Table:
         grid = DtshTui.mk_grid(4)
         for choice in arg_chosen:
             try:
                 node = self._dtsh.dt_chosen[choice]
             except KeyError:
                 raise DtshError(f'no such configuration choice: {arg_chosen[0]}')
             txt_choice = DtshTui.mk_txt(choice, DtshTui.style(DtshTui.STYLE_DT_ALIAS))
```

### Comparing `dtsh-0.1.0a4/src/dtsh/builtin_find.py` & `dtsh-0.1.0a6/src/dtsh/builtin_find.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 
 """Built-in 'find' command."""
 
 
 import re
 
 from abc import abstractmethod
-from typing import Tuple
+from typing import Tuple, List, Union
 
 from devicetree.edtlib import Node
 
 from dtsh.dtsh import DtshCommand, DtshCommandOption, Dtsh, DtshAutocomp, DtshVt
+from dtsh.dtsh import DtshCommandFlagLongFmt, DtshCommandArgLongFmt
 from dtsh.dtsh import DtshCommandUsageError
 from dtsh.tui import LsNodeTable, DtshTui
 
 
 class FindCriterion(object):
     """Interface for search criteria.
     """
@@ -334,71 +335,63 @@
 
 ```
 /
 ❯ find -c --enabled-only --bus * --interrupt * -f naibcd > interrupts.txt
 ```
 """
     # Search criteria.
-    _criteria: list[FindCriterion]
+    _criteria: List[FindCriterion]
 
     # Nodes matched during the last search.
-    _found: list[Node]
+    _found: List[Node]
 
     def __init__(self, shell: Dtsh) -> None:
         super().__init__(
             'find',
             'find devicetree nodes',
             True,
             [
                 DtshCommandOption('find by name',       None,  'name', 'pattern'),
                 DtshCommandOption('find by compatible', None,  'compat', 'pattern'),
                 DtshCommandOption('find by bus device', None,  'bus', 'pattern'),
                 DtshCommandOption('find by interrupt',  None,  'interrupt', 'pattern'),
                 DtshCommandOption('search only enabled nodes', None, 'enabled-only', None),
                 DtshCommandOption('print nodes count',  'c',    None, None),
                 DtshCommandOption('quiet, only print nodes count',  'q',    None, None),
-                DtshCommandOption('use rich listing format', 'l', None, None),
-                DtshCommandOption('visible columns format string', 'f', None, 'fmt'),
+                DtshCommandFlagLongFmt(),
+                DtshCommandArgLongFmt()
             ]
         )
         self._dtsh = shell
-        self._criteria = list[FindCriterion]()
-        self._found = list[Node]()
+        self._criteria = []
+        self._found = []
 
     @property
     def usage(self) -> str:
         """Overrides DtshCommand.usage().
         """
         return super().usage + ' [PATH]'
 
     @property
-    def arg_pattern_name(self) -> str | None:
+    def arg_pattern_name(self) -> Union[str, None]:
         return self.arg_value('--name')
 
     @property
-    def arg_pattern_compat(self) -> str | None:
+    def arg_pattern_compat(self) -> Union[str, None]:
         return self.arg_value('--compat')
 
     @property
-    def arg_pattern_bus(self) -> str | None:
+    def arg_pattern_bus(self) -> Union[str, None]:
         return self.arg_value('--bus')
 
     @property
-    def arg_pattern_irq(self) -> str | None:
+    def arg_pattern_irq(self) -> Union[str, None]:
         return self.arg_value('--interrupt')
 
     @property
-    def arg_fmt(self) -> str | None:
-        return self.arg_value('-f')
-
-    @property
-    def with_rich_fmt(self) -> bool:
-        return (self.arg_fmt is not None) or self.with_flag('-l')
-
-    @property
     def with_only_enabled(self) -> bool:
         return self.with_flag('--enabled-only')
 
     @property
     def with_node_count(self) -> bool:
         return self.with_flag('-c')
 
@@ -409,62 +402,62 @@
     def reset(self) -> None:
         """Overrides DtshCommand.reset().
         """
         super().reset()
         self._found.clear()
         self._criteria.clear()
 
-    def parse_argv(self, argv: list[str]) -> None:
+    def parse_argv(self, argv: List[str]) -> None:
         """Overrides DtshCommand.parse_argv().
         """
         super().parse_argv(argv)
+        if len(self._params) > 1:
+            raise DtshCommandUsageError(self, 'too many parameters')
         if self.arg_pattern_name:
             self._criteria.append(FindByNameCriterion(self.arg_pattern_name))
         if self.arg_pattern_compat:
             self._criteria.append(FindByCompatCriterion(self.arg_pattern_compat))
         if self.arg_pattern_bus:
             self._criteria.append(FindByBusCriterion(self.arg_pattern_bus))
         if self.arg_pattern_irq:
             self._criteria.append(FindByIrqCriterion(self.arg_pattern_irq))
 
     def execute(self, vt: DtshVt) -> None:
         """Implements DtshCommand.execute().
         """
-        if self.with_usage_summary:
-            vt.write(self.usage)
-            return
-        if len(self._params) > 1:
-            raise DtshCommandUsageError(self, 'too many parameters')
-
         if self._params:
             arg_path = self._dtsh.realpath(self._params[0])
         else:
             arg_path = self._dtsh.pwd
 
         self._find_nodes(self._dtsh.path2node(arg_path))
         # Like the POSIX find command, does not touch stdout if no match.
         if len(self._found) > 0:
 
             if self.with_pager:
                 vt.pager_enter()
 
             if not self.with_quiet:
-                if self.with_rich_fmt:
-                    self._write_found_long(vt)
+                longfmt = self.arg_longfmt
+                if self.with_longfmt and not longfmt:
+                   longfmt = self._mk_default_longmt()
+
+                if longfmt:
+                    self._write_found_long(vt, longfmt)
                 else:
                     self._write_found_default(vt)
 
             if self.with_node_count:
                 vt.write()
                 vt.write(f"{len(self._found)} nodes.")
 
             if self.with_pager:
                 vt.pager_exit()
 
-    def autocomplete_param(self, prefix: str) -> Tuple[int,list]:
+    def autocomplete_param(self, prefix: str) -> Tuple[int, List]:
         """Overrides DtshCommand.autocomplete_param().
         """
         return (DtshAutocomp.MODE_DT_NODE,
                 DtshAutocomp.autocomplete_with_nodes(prefix, self._dtsh))
 
     def _find_nodes(self, root: Node) -> None:
         if self.with_only_enabled and not Dtsh.is_node_enabled(root):
@@ -480,34 +473,33 @@
                 return False
         return True
 
     def _write_found_default(self, vt: DtshVt) -> None:
         for node in self._found:
             vt.write(node.path)
 
-    def _write_found_long(self, vt: DtshVt) -> None:
-        lsfmt = self.arg_fmt
-        if not lsfmt:
-            # Set visible columns depending on command options.
-            lsfmt = 'p'
-            if self.arg_pattern_name:
-                lsfmt += 'A'
-                lsfmt += 'L'
-            if self.arg_pattern_irq:
-                lsfmt += 'i'
-            if self.arg_pattern_bus:
-                lsfmt += 'b'
-            if self.arg_pattern_compat:
-                lsfmt += 'c'
-                lsfmt += 'd'
-        ls_table = LsNodeTable(self._dtsh, lsfmt)
+    def _write_found_long(self, vt: DtshVt, longfmt: str) -> None:
+        ls_table = LsNodeTable(self._dtsh, longfmt)
         for node in self._found:
             ls_table.add_node_row(node)
         vt.write(ls_table.as_view())
 
+    def _mk_default_longmt(self) -> str:
+        longfmt = 'p'
+        if self.arg_pattern_name:
+            longfmt += 'A'
+            longfmt += 'L'
+        if self.arg_pattern_irq:
+            longfmt += 'i'
+        if self.arg_pattern_bus:
+            longfmt += 'b'
+        if self.arg_pattern_compat:
+            longfmt += 'c'
+            longfmt += 'd'
+        return longfmt
 
 class FindByNameCriterion(FindCriterion):
     """Find nodes by names.
 
     Match nodes by the node-name component (DTSpec 2.2.1).
 
     If the search pattern does not contain any wildcard,
@@ -526,15 +518,15 @@
       and ends with <postfix>
     """
 
     # Character class for node names (DTSpec 2.2.1).
     CLASS_NODE_NAME = r'[\w,.+\-]*'
 
     # Pattern for regular expression type search, None for plain text search.
-    _re: re.Pattern | None
+    _re: Union[re.Pattern, None]
 
     def __init__(self, pattern: str) -> None:
         """Initialize criterion.
 
         Arguments:
         pattern - the search pattern
         """
@@ -575,15 +567,15 @@
       and ends with <postfix>
     """
 
     # Character class for 'compatible' property (DTSpec 2.3.1).
     CLASS_COMPATIBLE = r'[a-z0-9\-,]*'
 
     # Pattern for regular expression type search, None for plain text search.
-    _re: re.Pattern | None
+    _re: Union[re.Pattern, None]
 
     def __init__(self, pattern: str) -> None:
         """Initialize criterion.
 
         Arguments:
         pattern - the search pattern
         """
@@ -626,15 +618,15 @@
       and ends with <postfix>
     """
 
     # Character class for bus name (alphanumeric ? lowercase ?).
     CLASS_BUS = r'[\w]*'
 
     # Pattern for regular expression type search, None for plain text search.
-    _re: re.Pattern | None
+    _re: Union[re.Pattern, None]
 
     def __init__(self, pattern: str) -> None:
         """Initialize criterion.
 
         Arguments:
         pattern - the search pattern
         """
@@ -642,27 +634,27 @@
         self._re = None
         if pattern.find('*') != -1:
             pattern = pattern.replace('*', FindByBusCriterion.CLASS_BUS)
             re_expr = f'^{pattern}$'
             self._re = re.compile(re_expr)
 
     def match(self, node: Node) -> bool:
-        if node.bus:
+        for bus in node.buses:
             if self._re:
-                if self._re.match(node.bus) is not None:
+                if self._re.match(bus) is not None:
                     return True
             else:
-                if node.bus.find(self._pattern) != -1:
+                if bus.find(self._pattern) != -1:
                     return True
-        if node.on_bus:
+        for bus in node.on_buses:
             if self._re:
-                if self._re.match(node.on_bus) is not None:
+                if self._re.match(bus) is not None:
                     return True
             else:
-                if node.on_bus.find(self._pattern) != -1:
+                if bus.find(self._pattern) != -1:
                     return True
         return False
 
 
 class FindByIrqCriterion(FindCriterion):
     """Find nodes by interrupts.
 
@@ -687,19 +679,19 @@
       and ends with <postfix>
     """
 
     # Character class for IRQ names (empiric ?).
     CLASS_IRQ_NAME = r'[\w\-]*'
 
     # Search by IRQ number, None for search by IRQ name.
-    _irq_num: int | None
+    _irq_num: Union[int, None]
 
     # Search by IRQ name: pattern for regular expression type search,
     # None for plain text search.
-    _re: re.Pattern | None
+    _re: Union[re.Pattern, None]
 
     def __init__(self, pattern: str) -> None:
         """Initialize criterion.
 
         Arguments:
         pattern - the search pattern
         """
```

### Comparing `dtsh-0.1.0a4/src/dtsh/builtin_ls.py` & `dtsh-0.1.0a6/src/dtsh/builtin_ls.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Built-in 'ls' command."""
 
 
-from typing import Tuple
+from typing import Tuple, Dict, List
 from devicetree.edtlib import Node
 
 from dtsh.dtsh import DtshCommand, DtshCommandOption, Dtsh, DtshAutocomp, DtshVt
+from dtsh.dtsh import DtshCommandFlagLongFmt, DtshCommandArgLongFmt
 from dtsh.dtsh import DtshCommandUsageError
 from dtsh.tui import DtNodeListView
 
 
 class DtshBuiltinLs(DtshCommand):
     """List devicetree nodes.
 
@@ -183,18 +184,18 @@
     def __init__(self, shell: Dtsh) -> None:
         super().__init__(
             'ls',
             'list devicetree nodes',
             True,
             [
                 DtshCommandOption('list node itself, not its content', 'd', None, None),
-                DtshCommandOption('use rich listing format', 'l', None, None),
                 DtshCommandOption('reverse order while sorting', 'r', None, None),
                 DtshCommandOption('list node contents recursively', 'R', None, None),
-                DtshCommandOption('visible columns format string', 'f', 'format', 'fmt'),
+                DtshCommandFlagLongFmt(),
+                DtshCommandArgLongFmt()
             ]
         )
         self._dtsh = shell
 
     @property
     def usage(self) -> str:
         """Overrides DtshCommand.usage().
@@ -209,36 +210,24 @@
     def with_recursive(self) -> bool:
         return self.with_flag('-R')
 
     @property
     def with_reverse(self) -> bool:
         return self.with_flag('-r')
 
-    @property
-    def with_rich_fmt(self) -> bool:
-        return (self.arg_fmt is not None) or self.with_flag('-l')
-
-    @property
-    def arg_fmt(self) -> str | None:
-        return self.arg_value('-f')
-
-    def parse_argv(self, argv: list[str]) -> None:
+    def parse_argv(self, argv: List[str]) -> None:
         """Overrides DtshCommand.parse_argv().
         """
         super().parse_argv(argv)
+        if len(self._params) > 1:
+            raise DtshCommandUsageError(self, 'too many parameters')
 
     def execute(self, vt: DtshVt) -> None:
         """Implements DtshCommand.execute().
         """
-        if self.with_usage_summary:
-            vt.write(self.usage)
-            return
-        if len(self._params) > 1:
-            raise DtshCommandUsageError(self, 'too many parameters')
-
         if self._params:
             arg_path = self._dtsh.realpath(self._params[0])
         else:
             arg_path = self._dtsh.pwd
 
         if arg_path.endswith('*'):
             # Globing.
@@ -247,15 +236,15 @@
             roots = [
                 self._dtsh.path2node(arg_path)
             ]
 
         if self.with_reverse:
             roots.reverse()
 
-        node_map = dict[str, list[Node]]()
+        node_map: Dict[str, List[Node]] = {}
         for root in roots:
             if self.with_no_content:
                 node_map[root.path] = []
             else:
                 if self.with_recursive:
                     self._follow_node_content(root, node_map)
                 else:
@@ -264,24 +253,24 @@
         if self.with_reverse:
             for _, contents in node_map.items():
                 contents.reverse()
 
         view = DtNodeListView(node_map,
                               self._dtsh,
                               self.with_no_content,
-                              self.with_rich_fmt,
-                              self.arg_fmt)
+                              self.with_longfmt,
+                              self.arg_longfmt)
         view.show(vt, self.with_pager)
 
-    def autocomplete_param(self, prefix: str) -> Tuple[int,list]:
+    def autocomplete_param(self, prefix: str) -> Tuple[int, List]:
         """Overrides DtshCommand.autocomplete_param().
         """
         return (DtshAutocomp.MODE_DT_NODE,
                 DtshAutocomp.autocomplete_with_nodes(prefix, self._dtsh))
 
     def _follow_node_content(self,
                              parent: Node,
-                             node_map: dict[str, list[Node]]) -> None:
-        node_map[parent.path] = list[Node]()
+                             node_map: Dict[str, List[Node]]) -> None:
+        node_map[parent.path] = []
         for _, node in parent.children.items():
             node_map[parent.path].append(node)
             self._follow_node_content(node, node_map)
```

### Comparing `dtsh-0.1.0a4/src/dtsh/builtin_man.py` & `dtsh-0.1.0a6/src/dtsh/builtin_man.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Built-in 'man' command."""
 
-import readline
-from typing import Tuple
+from typing import Tuple, List
 
 from devicetree.edtlib import Binding
 
+from dtsh.rl import readline
 from dtsh.dtsh import Dtsh, DtshCommand, DtshCommandOption, DtshAutocomp, DtshVt
 from dtsh.dtsh import DtshError, DtshCommandUsageError, DtshCommandFailedError
 from dtsh.man import DtshManPageBinding, DtshManPageBuiltin, DtshManPageDtsh
 
 
 class DtshBuiltinMan(DtshCommand):
     """Print current working node's path.
@@ -69,32 +69,27 @@
     def with_compat(self) -> bool:
         return self.with_flag('--compat')
 
     @property
     def with_no_pager(self) -> bool:
         return self.with_flag('--no-pager')
 
-    def parse_argv(self, argv: list[str]) -> None:
+    def parse_argv(self, argv: List[str]) -> None:
         """Overrides DtshCommand.parse_argv().
         """
         super().parse_argv(argv)
-
-    def execute(self, vt: DtshVt) -> None:
-        """Implements DtshCommand.execute().
-        """
-        if self.with_usage_summary:
-            vt.write(self.usage)
-            return
         if len(self._params) == 0:
             raise DtshCommandUsageError(self, 'what manual page do you want?')
         if len(self._params) > 1:
             raise DtshCommandUsageError(self, 'too many parameters')
 
+    def execute(self, vt: DtshVt) -> None:
+        """Implements DtshCommand.execute().
+        """
         arg_page = self._params[0]
-
         man_page = None
 
         if self.with_compat:
             binding = self._dtsh.dt_bindings.get(arg_page)
             if binding:
                 man_page = DtshManPageBinding(binding)
         else:
@@ -106,15 +101,15 @@
             man_page = DtshManPageDtsh()
 
         if man_page is not None:
             man_page.show(vt, self.with_no_pager)
         else:
             raise DtshCommandFailedError(self, f'page not found: {arg_page}')
 
-    def autocomplete_param(self, prefix: str) -> Tuple[int,list]:
+    def autocomplete_param(self, prefix: str) -> Tuple[int, List]:
         """Overrides DtshCommand.autocomplete_param().
         """
         # 1st, complete according to flags.
         cmdline = readline.get_line_buffer()
         cmdline_vstr = cmdline.split()
         if len(cmdline_vstr) > 1:
             argv = cmdline_vstr[1:]
@@ -131,24 +126,24 @@
         # Then, try command name (default).
         completions = self._autocomplete_dtsh_cmd(prefix)
         if completions:
             return (DtshAutocomp.MODE_DTSH_CMD, completions)
 
         return (DtshAutocomp.MODE_ANY, [])
 
-    def _autocomplete_dtsh_cmd(self, prefix: str) -> list[DtshCommand]:
-        completions = list[DtshCommand]()
+    def _autocomplete_dtsh_cmd(self, prefix: str) -> List[DtshCommand]:
+        completions: List[DtshCommand] = []
         if prefix.find('/') == -1:
             for cmd in self._dtsh.builtins:
                 if (not prefix) or (cmd.name.startswith(prefix) and (len(cmd.name) > len(prefix))):
                     completions.append(cmd)
         return completions
 
-    def _autocomplete_dt_binding(self, prefix: str) -> list[Binding]:
-        completions = list[Binding]()
+    def _autocomplete_dt_binding(self, prefix: str) -> List[Binding]:
+        completions: List[Binding] = []
         for compat, binding in self._dtsh.dt_bindings.items():
             if prefix:
                 if compat.startswith(prefix) and (len(compat) > len(prefix)):
                     completions.append(binding)
             else:
                 completions.append(binding)
         return completions
```

### Comparing `dtsh-0.1.0a4/src/dtsh/builtin_pwd.py` & `dtsh-0.1.0a6/src/dtsh/builtin_pwd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Built-in 'pwd' command."""
 
 
+from typing import List
+
 from dtsh.dtsh import Dtsh, DtshCommand, DtshVt
 from dtsh.dtsh import DtshCommandUsageError
 
 
 class DtshBuiltinPwd(DtshCommand):
     """Print current working node's path.
 
@@ -38,22 +40,18 @@
     def __init__(self, shell: Dtsh):
         super().__init__(
             'pwd',
             "print current working node's path"
         )
         self._dtsh = shell
 
-    def parse_argv(self, argv: list[str]) -> None:
+    def parse_argv(self, argv: List[str]) -> None:
         """Overrides DtshCommand.parse_argv().
         """
         super().parse_argv(argv)
+        if len(self._params) > 0:
+            raise DtshCommandUsageError(self, 'too many parameters')
 
     def execute(self, stdout: DtshVt) -> None:
         """Implements DtshCommand.execute().
         """
-        if self.with_usage_summary:
-            stdout.write(self.usage)
-            return
-        if len(self._params) > 0:
-            raise DtshCommandUsageError(self, 'too many parameters')
-
         stdout.write(self._dtsh.pwd)
```

### Comparing `dtsh-0.1.0a4/src/dtsh/builtin_tree.py` & `dtsh-0.1.0a6/src/dtsh/builtin_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Built-in 'tree' command."""
 
 
-from typing import Tuple
+from typing import Tuple, List, Union
 
 from dtsh.dtsh import Dtsh, DtshVt, DtshCommand, DtshCommandOption, DtshAutocomp
+from dtsh.dtsh import DtshCommandFlagLongFmt
 from dtsh.dtsh import DtshCommandUsageError
 
 from dtsh.tui import DtNodeTreeView
 
 
 class DtshBuiltinTree(DtshCommand):
     """List devicetree nodes in tree-like format.
@@ -103,85 +104,76 @@
 
 ├──  connector        GPIO pins exposed on Arduino Uno (R3) headers…
 └──  analog-connector ADC channels exposed on Arduino Uno (R3) headers…
 ```
 """
 
     # Maximum display depth, 0 to follow all non disabled nodes.
-    _level: int = 0
+    _level: int
 
     def __init__(self, shell: Dtsh):
         super().__init__(
             'tree',
             'list devicetree nodes in tree-like format',
             True,
             [
-                DtshCommandOption('use rich listing format', 'l', None, None),
                 DtshCommandOption('max display depth of the tree', 'L', 'depth', 'level'),
+                DtshCommandFlagLongFmt(),
             ]
         )
         self._dtsh = shell
+        self._level = 0
 
     @property
     def usage(self) -> str:
         """Overrides DtshCommand.usage().
         """
         return super().usage + ' [PATH]'
 
     @property
-    def with_rich_fmt(self) -> bool:
-        return self.with_flag('-l')
-
-    @property
-    def arg_level(self) -> int:
+    def arg_level(self) -> Union[str, None]:
         """Maximum display depth, 0 to follow all non disabled nodes.
         """
-        return self._level
+        return self.arg_value('-L')
 
     def reset(self) -> None:
         """Overrides DtshCommand.reset().
         """
         super().reset()
         self._level = 0
 
-    def parse_argv(self, argv: list[str]) -> None:
+    def parse_argv(self, argv: List[str]) -> None:
         """Overrides DtshCommand.parse_argv().
         """
         super().parse_argv(argv)
-
-        opt = self.option('-L')
-        if opt and opt.value:
+        if len(self._params) > 1:
+            raise DtshCommandUsageError(self, 'too many parameters')
+        if self.arg_level is not None:
             try:
-                self._level = int(opt.value)
+                self._level = int(self.arg_level)
             except ValueError:
                 raise DtshCommandUsageError(
                     self,
-                    f"'{opt.value}' is not a valid level"
+                    f"'{self.arg_level}' is not a valid level"
                 )
 
     def execute(self, vt: DtshVt) -> None:
         """Implements DtshCommand.execute().
         """
-        if self.with_usage_summary:
-            vt.write(self.usage)
-            return
-        if len(self._params) > 1:
-            raise DtshCommandUsageError(self, 'too many parameters')
-
         if self._params:
             arg_path = self._dtsh.realpath(self._params[0])
         else:
             arg_path = self._dtsh.pwd
 
         root = self._dtsh.path2node(arg_path)
 
         view = DtNodeTreeView(root,
                               self._dtsh,
-                              self.arg_level,
-                              self.with_rich_fmt)
+                              self._level,
+                              self.with_longfmt)
         view.show(vt, self.with_pager)
 
-    def autocomplete_param(self, prefix: str) -> Tuple[int,list]:
+    def autocomplete_param(self, prefix: str) -> Tuple[int, List]:
         """Overrides DtshCommand.autocomplete_param().
         """
         return (DtshAutocomp.MODE_DT_NODE,
                 DtshAutocomp.autocomplete_with_nodes(prefix, self._dtsh))
```

### Comparing `dtsh-0.1.0a4/src/dtsh/builtin_uname.py` & `dtsh-0.1.0a6/src/dtsh/builtin_uname.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Built-in 'uname' command."""
 
 
+from typing import List, Union
+
 import os
 
 from rich.table import Table
 from rich.text import Text
 
 from dtsh.dtsh import Dtsh, DtshCommand, DtshCommandOption, DtshUname, DtshVt
+from dtsh.dtsh import DtshCommandFlagLongFmt
 from dtsh.dtsh import DtshCommandUsageError
 from dtsh.systools import GitHub, YamlFile
 from dtsh.tui import DtshTui, DtshTuiBulletList, DtshTuiForm, DtshTuiMemo, DtshTuiYaml
 
 
 class DtshBuiltinUname(DtshCommand):
     """Print current working node's path.
@@ -119,15 +122,14 @@
 """
     def __init__(self, shell: Dtsh):
         super().__init__(
             'uname',
             "print system information",
             True,
             [
-                DtshCommandOption('use rich format', 'l', None, None),
                 DtshCommandOption('print Zephyr kernel version',
                                   'v',
                                   'kernel-version',
                                   None),
                 DtshCommandOption('print board',
                                   'm',
                                   'machine',
@@ -136,23 +138,20 @@
                                   't',
                                   'toolchain',
                                   None),
                 DtshCommandOption("print all information",
                                   'a',
                                   'all',
                                   None),
+                DtshCommandFlagLongFmt(),
             ]
         )
         self._dtsh = shell
 
     @property
-    def with_long_fmt(self) -> bool:
-        return self.with_flag('-l')
-
-    @property
     def with_kernel_version(self) -> bool:
         return self.with_flag('-v')
 
     @property
     def with_machine(self) -> bool:
         return self.with_flag('-m')
 
@@ -160,29 +159,25 @@
     def with_toolchain(self) -> bool:
         return self.with_flag('-t')
 
     @property
     def with_all(self) -> bool:
         return self.with_flag('-a')
 
-    def parse_argv(self, argv: list[str]) -> None:
+    def parse_argv(self, argv: List[str]) -> None:
         """Overrides DtshCommand.parse_argv().
         """
         super().parse_argv(argv)
+        if len(self._params) > 0:
+            raise DtshCommandUsageError(self, 'too many parameters')
 
     def execute(self, vt: DtshVt) -> None:
         """Implements DtshCommand.execute().
         """
-        if self.with_usage_summary:
-            vt.write(self.usage)
-            return
-        if len(self._params) > 0:
-            raise DtshCommandUsageError(self, 'too many parameters')
-
-        if self.with_long_fmt:
+        if self.with_longfmt:
             self._uname_long(vt)
         else:
             self._uname_brief(vt)
 
     def _uname_brief(self, vt: DtshVt) -> None:
         msg = ""
         no_with = not (
@@ -236,15 +231,15 @@
             view.add_entry("toolchain", content)
 
         if self.with_all or def_all or self.with_machine:
             view.add_entry("board", self._mk_layout_board())
 
         view.show(vt, self.with_pager)
 
-    def _mk_layout_zephyr_kernel(self) -> Table | None:
+    def _mk_layout_zephyr_kernel(self) -> Union[Table, None]:
         if self._dtsh.uname.zephyr_base:
             layout = DtshTui.mk_grid(1)
             layout.add_row(ZephyrKernelForm(self._dtsh.uname).as_renderable())
             layout.add_row()
             if self._dtsh.uname.dt_binding_dirs:
                 r_list = DtshTuiBulletList("Bindings search path:")
                 for path in self._dtsh.uname.dt_binding_dirs:
@@ -254,15 +249,15 @@
                 layout.add_row(r_list.as_renderable())
             else:
                 r_warn = DtshTui.mk_txt_warn("Empty bindings search path !")
                 layout.add_row(r_warn)
             return layout
         return None
 
-    def _mk_layout_board(self) -> Table | None:
+    def _mk_layout_board(self) -> Union[Table, None]:
         if self._dtsh.uname.board:
             layout = DtshTui.mk_grid(1)
             layout.add_row(ZephyrBoardForm(self._dtsh.uname).as_renderable())
             if self._dtsh.uname.board_binding_file:
                 if os.path.isfile(self._dtsh.uname.board_binding_file):
                     w_yaml = DtshTuiYaml(self._dtsh.uname.board_binding_file,
                                          with_title=True)
@@ -429,16 +424,13 @@
                     r_name.append_text(DtshTui.mk_txt(')'))
         else:
             r_name = DtshTui.mk_txt_dim("Unknown")
         self.add_field_rich("Name", r_name)
 
         r_board = DtshTui.mk_txt(uname.board, style='dtsh.board')
         if uname.board_dts_file:
-            r_dts = DtshTui.mk_txt_link(
-                "DTS",
-                f'file:{uname.board_dts_file}',
-                style='dtsh.default'
-            )
+            r_dts = DtshTui.mk_txt("DTS")
+            DtshTui.txt_update_link_file(r_dts, uname.board_dts_file)
             r_board.append_text(DtshTui.mk_txt(' ('))
             r_board.append_text(r_dts)
             r_board.append_text(DtshTui.mk_txt(')'))
         self.add_field_rich("Board", r_board)
```

### Comparing `dtsh-0.1.0a4/src/dtsh/cli.py` & `dtsh-0.1.0a6/src/dtsh/cli.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a4/src/dtsh/dtsh.py` & `dtsh-0.1.0a6/src/dtsh/dtsh.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import getopt
 import os
 import re
 from pathlib import Path
 
 from abc import abstractmethod
-from typing import ClassVar, Tuple
+from typing import Any, ClassVar, Dict, List, Optional, Tuple, Union
 
 from devicetree.edtlib import EDT, EDTError, Node, Binding, Property
 
 from dtsh.systools import Git, CMakeCache, GCCArm
 
 
 class DtshVt(object):
@@ -80,24 +80,24 @@
     An option that expects a named value is an argument.
 
     An option may admit a short name (e.g. 'v'),
     and/or a long name (e.g. 'verbose').
     """
 
     _desc: str
-    _shortname: str | None
-    _longname: str | None
-    _arg: str | None
-    _value: bool | str | None
+    _shortname: Union[str, None]
+    _longname: Union[str, None]
+    _arg: Union[str, None]
+    _value: Union[str, bool, None]
 
     def __init__(self,
                  desc: str,
-                 shortname: str | None,
-                 longname: str | None,
-                 arg: str | None = None) -> None:
+                 shortname: Optional[str],
+                 longname: Optional[str],
+                 arg: Optional[str] = None) -> None:
         """Define a command option.
 
         Arguments:
         desc -- short description, e.g. 'use a long listing format'
         shortname -- short option name (e.g. the 'v' in '-v),
                      or None if the option does not admit a short name
         longname -- long option name (e.g. 'verbose' in '--verbose'),
@@ -114,39 +114,39 @@
     @property
     def desc(self) -> str:
         """The option's description.
         """
         return self._desc
 
     @property
-    def shortname(self) -> str | None:
+    def shortname(self) -> Union[str, None]:
         """The option's short name, e.g. 'v'.
 
         This name does not include the '-' prefix,
         neither the ':' postfix when an argument is expected.
 
         Retutns the option's short name, or None if the option does not admit
         a short name.
         """
         return self._shortname
 
     @property
-    def longname(self) -> str | None:
+    def longname(self) -> Union[str, None]:
         """The option's long name, e.g. 'verbose'.
 
         This name does not include the '--' prefix,
         neither the '=' postfix when an argument is expected.
 
         Returns the option's long name, or None if the option does not admit
         a long name.
         """
         return self._longname
 
     @property
-    def argname(self) -> str | None:
+    def argname(self) -> Union[str, None]:
         """The option's argument name, or None if the options is a flag.
         """
         return self._arg
 
     @property
     def usage(self) -> str:
         """The option's usage string, e.g. '-a <alias> -v --verbose'.
@@ -160,87 +160,122 @@
             else:
                 txt = f"--{self._longname}"
         if self._arg:
             txt += f" <{self._arg}>"
         return txt
 
     @property
-    def value(self) -> bool | str | None:
+    def value(self) -> Union[str, bool, None]:
         """The option's value.
 
         Before a command's options are parsed, this value is None.
 
         After the command string is successfully parsed, an option value is:
         - True (set) or False (unset) for a flag
         - a string value for an argument
         """
         return self._value
 
     @value.setter
-    def value(self, v: bool | str):
+    def value(self, v: Union[bool, str]) -> None:
         """Set the option's value.
 
         The options values are typically set when parsing a command string.
 
         Arguments:
         v -- True (False) to set (unset) a flag,
              or a string value to set an argument
         """
         self._value = v
 
-
     def is_flag(self) -> bool:
         """Returns True if the option does not expect any value.
         """
         return self._arg is None
 
     def reset(self):
         """Reset this option's value, typically before parsing a command string.
         """
         self._value = None
 
 
+class DtshCommandFlagHelp(DtshCommandOption):
+    """Common "help" flag ('-h', '--help).
+
+    If True, print usage summary.
+    """
+
+    def __init__(self) -> None:
+        super().__init__('print usage summary', 'h', 'help', None)
+
+
+class DtshCommandFlagLongFmt(DtshCommandOption):
+    """Common "long format" flag ('-l')
+
+    If True, use long (aka rich) listing format.
+    """
+
+    def __init__(self) -> None:
+        super().__init__('use long (rich) listing format', 'l', None, None)
+
+
+class DtshCommandArgLongFmt(DtshCommandOption):
+    """Common "long format" command argument ('-f')
+
+    Specifies columns for a node table.
+    """
+
+    def __init__(self) -> None:
+        super().__init__('visible columns format string', 'f', None, 'fmt')
+
+
+class DtshCommandFlagPager(DtshCommandOption):
+    """Common "page output" flag ('--pager')
+
+    If True, page command output.
+    """
+
+    def __init__(self) -> None:
+        super().__init__('page command output', None, 'pager', None)
+
+
 class DtshCommand(object):
     """Devicetree shell command.
     """
 
     # Name, e.g. 'ls'.
     _name: str
     # Description, e.g. 'list nodes content'.
     _desc: str
     # Supported options.
-    _options: list[DtshCommandOption]
+    _options: List[DtshCommandOption]
     # Parsed parameters (command string components that are not parsed options).
-    _params: list[str]
+    _params: List[str]
 
     def __init__(self,
                  name: str,
                  desc: str,
                  with_pager: bool = False,
-                 options: list[DtshCommandOption] = []) -> None:
+                 options: List[DtshCommandOption] = []) -> None:
         """Defines a devicetree shell command.
 
         Arguments:
         name -- the command's name (e.g. 'ls')
         desc -- the command's description
         with_pager -- if True, enables pager option support
         options -- the command's options
         """
         self._name = name
         self._desc= desc
-        self._params = list[str]()
-        self._options = list[DtshCommandOption]()
+        self._params = []
+        self._options = []
         self._options.extend(options)
         if with_pager:
-            self._options.append(
-                DtshCommandOption('page command output', None, 'pager', None)
-            )
-        self._options.append(
-            DtshCommandOption('print usage summary', 'h', 'help', None)
-        )
+            self._options.append(DtshCommandFlagPager())
+        self._options.append(DtshCommandFlagHelp())
 
     @property
     def name(self) -> str:
         """Command's name, e.g. 'ls'.
         """
         return self._name
 
@@ -256,15 +291,15 @@
         """
         txt = self._name
         for opt in self._options:
             txt += f" [{opt.usage}]"
         return txt
 
     @property
-    def options(self) -> list[DtshCommandOption]:
+    def options(self) -> List[DtshCommandOption]:
         """Available options.
         """
         return self._options
 
     @property
     def getopt_short(self) -> str:
         """Short options specification string compatible with GNU getopt.
@@ -277,15 +312,15 @@
             if opt.shortname:
                 shortopts += opt.shortname
                 if opt.argname:
                     shortopts += ':'
         return shortopts
 
     @property
-    def getopt_long(self) -> list[str]:
+    def getopt_long(self) -> List[str]:
         """Long options specification list compatible with GNU getopt.
 
         e.g. ['help','alias='] when the option supports a flag '--help',
         and an argument '--alias='.
         """
         longopts = []
         for opt in self._options:
@@ -297,18 +332,26 @@
         return longopts
 
     @property
     def with_pager(self) -> bool:
         return self.with_flag('--pager')
 
     @property
-    def with_usage_summary(self) -> bool:
+    def with_help(self) -> bool:
         return self.with_flag('-h')
 
-    def option(self, name: str) -> DtshCommandOption | None:
+    @property
+    def with_longfmt(self) -> bool:
+        return self.with_flag('-l')
+
+    @property
+    def arg_longfmt(self) -> Union[str, None]:
+        return self.arg_value('-f')
+
+    def option(self, name: str) -> Union[DtshCommandOption, None]:
         """Access a supported option.
 
         Arguments:
         name -- an option's name, either a short form (e.g. '-h'),
                 or a long form (e.g. '--help')
 
         Returns None if the option is not supported by this command.
@@ -332,15 +375,15 @@
         Returns True if name refers to a set flag, False otherwise.
         """
         opt = self.option(name)
         if opt:
             return opt.is_flag() and (opt.value == True)
         return False
 
-    def arg_value(self, name) -> str | None:
+    def arg_value(self, name) -> Union[str, None]:
         """Access an argument value.
 
         Arguments:
         name -- the option name
 
         Returns the argument value, None if the option was not provided on
         the command line, or if the option is a flag.
@@ -355,15 +398,15 @@
     def reset(self) -> None:
         """Reset command options and parameters.
         """
         for opt in self._options:
             opt.reset()
         self._params.clear()
 
-    def parse_argv(self, argv: list[str]) -> None:
+    def parse_argv(self, argv: List[str]) -> None:
         """Parse command line arguments, setting options and parameters.
 
         Arguments:
         argv -- the command's arguments
 
         Raises DtshCommandUsageError when the arguments do not match the
         command's usage (getopt).
@@ -380,23 +423,27 @@
             opt = self.option(opt_name)
             if opt:
                 if opt.argname:
                     opt.value = opt_arg
                 else:
                     opt.value = True
 
-    def autocomplete_option(self, prefix: str) -> list[DtshCommandOption]:
+        if self.with_help:
+            # Should print usage summary, see DevicetreeShellSession.run().
+            raise DtshCommandUsageError(self)
+
+    def autocomplete_option(self, prefix: str) -> List[DtshCommandOption]:
         """Auto-complete a command's options name.
 
         Arguments:
         prefix -- the option's name prefix, starting with '-' or '--'
 
         Returns a list of matching options.
         """
-        completions = list[DtshCommandOption]()
+        completions: List[DtshCommandOption] = []
 
         if prefix == '-':
             # Match all options, sorting with short names first.
             shortopts = [o for o in self._options if o.shortname]
             completions.extend(shortopts)
             # Then options with long names only.
             otheropts = [
@@ -415,27 +462,27 @@
                     continue
                 if opt.longname.startswith(p) and (len(opt.longname) > len(p)):
                     completions.append(opt)
 
         return completions
 
     def autocomplete_argument(self,
-                              arg: DtshCommandOption,
-                              prefix: str) -> list[str]:
+                              arg: DtshCommandOption, # pyright: ignore reportUnusedVariable
+                              prefix: str) -> List[str]: # pyright: ignore reportUnusedVariable
         """Auto-complete a command's option value (aka argument).
 
         Arguments:
         arg -- the option expecting a value
         prefix -- the option's name prefix, starting with '-' or '--'
 
         Returns a list of matching arguments.
         """
         return []
 
-    def autocomplete_param(self, prefix: str) -> Tuple[int,list]:
+    def autocomplete_param(self, prefix: str) -> Tuple[int, List]: # pyright: ignore reportUnusedVariable
         """Auto-complete a command's parameter value.
 
         Completions are represented by the tagged list of possible
         parameter objects.
 
         The tag will help client code to interpret (type) these parameter values.
 
@@ -465,44 +512,44 @@
     “..” components are also eliminated).
     """
 
     # Resolved DTS file path.
     _dts_path: str
 
     # Resolved binding directories.
-    _binding_dirs: list[str]
+    _binding_dirs: List[str]
 
     # Resolved $ZEPHYR_BASE.
-    _zephyr_base: str | None
+    _zephyr_base: Union[str, None]
 
     # Resolved $ZEPHYR_SDK_INSTALL_DIR.
-    _zephyr_sdk_dir: str | None
+    _zephyr_sdk_dir: Union[str, None]
 
     # Cached $ZEPHYR_SDK_INSTALL_DIR/sdk_version file content.
-    _zephyr_sdk_version: str | None
+    _zephyr_sdk_version: Union[str, None]
 
     # Resolved $GNUARMEMB_TOOLCHAIN_PATH.
-    _gnuarm_dir: str | None
+    _gnuarm_dir: Union[str, None]
 
     # $ZEPHYR_TOOLCHAIN_VARIANT ('gnuarmemb' or 'zephyr').
-    _zephyr_toolchain: str | None
+    _zephyr_toolchain: Union[str, None]
 
     # git -C $ZEPHYR_BASE log -n 1 --pretty=format:"%h"
-    _zephyr_rev: str | None
+    _zephyr_rev: Union[str, None]
 
     # git tag --points-at HEAD
-    _zephyr_tags: list[str]
+    _zephyr_tags: List[str]
 
     # Resolved BOARD_DIR (CMake).
-    _board_dir: str | None
+    _board_dir: Union[str, None]
 
     # CMake cached variables.
     _cmake_cache: CMakeCache
 
-    def __init__(self, dts_path:str, binding_dirs: list[str] | None) -> None:
+    def __init__(self, dts_path:str, binding_dirs: Optional[List[str]]) -> None:
         """Initialize system info.
 
         Arguments:
         dts_path -- Path to a devicetree source file.
         binding_dirs -- List of path to search for DT bindings.
                         If unspecified, and ZEPHYR_BASE is set,
                         defaults to Zephyr's DT bindings.
@@ -510,16 +557,16 @@
         Raises DtshError when a specified path is invalid.
         """
         try:
             self._dts_path = str(Path(dts_path).resolve(strict=True))
         except FileNotFoundError as e:
             raise DtshError(f"DTS file not found: {dts_path}", e)
 
-        self._binding_dirs = list[str]()
-        self._zephyr_tags = list[str]()
+        self._binding_dirs = []
+        self._zephyr_tags = []
         self._zephyr_base = None
         self._zephyr_sdk_dir = None
         self._zephyr_sdk_version = None
         self._gnuarm_dir = None
         self._zephyr_toolchain = None
         self._zephyr_rev = None
         self._board_dir = None
@@ -545,15 +592,15 @@
     @property
     def dts_path(self) -> str:
         """Returns the resolved path to the session's DT source file.
         """
         return self._dts_path
 
     @property
-    def dt_binding_dirs(self) -> list[str]:
+    def dt_binding_dirs(self) -> List[str]:
         """Returns the DT bindings search path as a list of resolved path.
 
         When no bindings are specified by the dtsh command line,
         and the environment variable ZEPHYR_BASE is set,
         we'll try to default to the bindings Zephyr would use (has used)
         at build-time.
 
@@ -590,61 +637,61 @@
         See:
         - $ZEPHYR_BASE/cmake/modules/dts.cmake
         - https://docs.zephyrproject.org/latest/build/dts/bindings.html#where-bindings-are-located
         """
         return self._binding_dirs
 
     @property
-    def zephyr_base(self) -> str | None:
+    def zephyr_base(self) -> Union[str, None]:
         """Returns the resolved path to the Zephyr kernel repository set by
         the environment variable ZEPHYR_BASE, or None if unset.
         """
         return self._zephyr_base
 
     @property
-    def zephyr_toolchain(self) -> str | None:
+    def zephyr_toolchain(self) -> Union[str, None]:
         """Returns the toolchain variant ('zephyr' or 'gnuarmemb') set by the
         environment variable ZEPHYR_TOOLCHAIN_VARIANT, or None if unset.
         """
         return self._zephyr_toolchain
 
     @property
-    def zephyr_sdk_dir(self) -> str | None:
+    def zephyr_sdk_dir(self) -> Union[str, None]:
         """Returns resolved path the Zephyr SDK directory set by the environment
         variable ZEPHYR_SDK_INSTALL_DIR, or None if unset.
         """
         return self._zephyr_sdk_dir
 
     @property
-    def gnuarm_dir(self) -> str | None:
+    def gnuarm_dir(self) -> Union[str, None]:
         """Value of the environment variable GNUARMEMB_TOOLCHAIN_PATH, or None.
         """
         """Returns the GCC Arm base directory set by the environment variable
         GNUARMEMB_TOOLCHAIN_PATH, or None if unset.
         """
         return self._gnuarm_dir
 
     @property
-    def zephyr_kernel_rev(self) -> str | None:
+    def zephyr_kernel_rev(self) -> Union[str, None]:
         """Returns the Zephyr kernel revision as given by
         git -C $ZEPHYR_BASE log -n 1 --pretty=format:"%h",
         or None when unavailable.
         """
         return self._zephyr_rev
 
     @property
-    def zephyr_kernel_tags(self) -> list[str]:
+    def zephyr_kernel_tags(self) -> List[str]:
         """Returns the Zephyr kernel tags for the current
         repository state, as given by git tag --points-at HEAD,
         or None when unavailable.
         """
         return self._zephyr_tags
 
     @property
-    def zephyr_kernel_version(self) -> str | None:
+    def zephyr_kernel_version(self) -> Union[str, None]:
         """Returns the Zephyr kernel version tag for the current
         repository state, e.g. 'zephyr-v3.1.0',
         or None if the state does not match a tagged Zephyr kernel release.
         """
         version = None
         if self.zephyr_kernel_tags:
             # Include stable and RC releases.
@@ -653,15 +700,15 @@
                 m = regex.match(tag)
                 if m:
                     version = tag
                     break
         return version
 
     @property
-    def zephyr_sdk_version(self) -> str | None:
+    def zephyr_sdk_version(self) -> Union[str, None]:
         """Returns the Zephyr SDK version set in the file
         $ZEPHYR_SDK_INSTALL_DIR/sdk_version, or None if unavailable.
         """
         if self._zephyr_sdk_version is None:
             if self._zephyr_sdk_dir:
                 path = os.path.join(self._zephyr_sdk_dir, 'sdk_version')
                 try:
@@ -669,30 +716,30 @@
                         self._zephyr_sdk_version = f.read().strip()
                 except IOError:
                     # Silently fail.
                     pass
         return self._zephyr_sdk_version
 
     @property
-    def gnuarm_version(self) -> str | None:
+    def gnuarm_version(self) -> Union[str, None]:
         """Returns GCC Arm toolchain version, or None if unavailable.
         """
         if self._gnuarm_dir:
             return GCCArm(self._gnuarm_dir).version
         return None
 
     @property
-    def board_dir(self) -> str | None:
+    def board_dir(self) -> Union[str, None]:
         """Returns the resolved path to the board directory set by
         the CMake cached variable BOARD_DIR, or None if unavailable.
         """
         return self._board_dir
 
     @property
-    def board(self) -> str | None:
+    def board(self) -> Union[str, None]:
         """Returns the best guess fo the board (try BOARD environment variable
         and CMake cache) or None if unavailable.
         """
         # 1st, try environmant variable.
         found_board = os.getenv('BOARD')
         if not found_board:
             # Then try CMake cache.
@@ -702,26 +749,26 @@
                 found_board = self._cmake_cache.get('CACHED_BOARD')
                 if (not found_board) and self.board_dir:
                     # Fallback: extract BOARD from BOARD_DIR
                     found_board = os.path.basename(self.board_dir)
         return found_board
 
     @property
-    def board_dts_file(self) -> str | None:
+    def board_dts_file(self) -> Union[str, None]:
         """Returns the best guess for the the DTS file path (relies on
         CMake cache), or None if unavailable.
         """
         if self.board_dir and self.board:
             path = os.path.join(self.board_dir, f'{self.board}.dts')
             if os.path.isfile(path):
                 return path
         return None
 
     @property
-    def board_binding_file(self) -> str | None:
+    def board_binding_file(self) -> Union[str, None]:
         """Returns the best guess for the board binding file path (relies on
         CMake cache), or None if unavailable.
         """
         if self.board_dir and self.board:
             path = os.path.join(self.board_dir, f'{self.board}.yaml')
             if os.path.isfile(path):
                 return path
@@ -798,36 +845,36 @@
     """Shell-like interface to a devicetree.
 
     The global metaphor is:
     - a filesystem-like view of the devicetree model
     - a command string interface to POSIX-like shell commands (aka built-ins)
     """
 
-    API_VERSION = '0.1.0a4'
+    API_VERSION = '0.1.0a6'
     """API version for the dtsh module.
 
     Should match 'version' in setup.py.
     """
 
     # Devicetree model (edtlib).
     _edt: EDT
 
     # Current working node.
     _cwd: Node
 
     # Built-in commands.
-    _builtins: dict[str, DtshCommand]
+    _builtins: Dict[str, DtshCommand]
 
     # Cached bindings map.
-    _bindings: dict[str, Binding]
+    _bindings: Dict[str, Binding]
 
     # Cached available DT binding paths (including YAML files that do
     # not describe a compatible).
     # Memory trade-off: this map may contain about 2000 entries.
-    _binding2path: dict[str, str]
+    _binding2path: Dict[str, str]
 
     # Sysinfo.
     _uname: DtshUname
 
     def __init__(self, edt: EDT, uname: DtshUname) -> None:
         """Initialize a shell-like interface to a devicetree.
 
@@ -839,17 +886,17 @@
         edt -- devicetree model (sources and bindings), provided by edtlib
         uname -- system information inferred from environment variables,
                  CMake cached variables, Zephyr's Git repository state.
         """
         self._edt = edt
         self._uname = uname
         self._cwd = self._edt.get_node('/')
-        self._builtins = dict[str, DtshCommand]()
-        self._bindings = dict[str, Binding]()
-        self._binding2path = dict[str, str]()
+        self._builtins = {}
+        self._bindings = {}
+        self._binding2path = {}
         self._init_binding_paths()
         self._init_bindings()
 
     @property
     def uname(self) -> DtshUname:
         """System information inferred from environment variables,
         CMake cached variables and Zephyr's Git repository state.
@@ -868,74 +915,74 @@
     @property
     def pwd(self) -> str:
         """Current working node's path.
         """
         return self._cwd.path
 
     @property
-    def builtins(self) -> list[DtshCommand]:
+    def builtins(self) -> List[DtshCommand]:
         """Available shell built-ins as a list.
         """
         return [cmd for _, cmd in self._builtins.items()]
 
     @property
-    def dt_bindings(self) -> dict[str, Binding]:
+    def dt_bindings(self) -> Dict[str, Binding]:
         """Map each compatible to its binding.
 
         This collection should include all compatibles that are both:
         - matched (by a node's "compatible" property)
         - described (by a corresponding YAML file)
 
         However, the current implementation of the devicetree model initialization
         may filter out bindings that never appear first (i.e. as most specific)
         in the "compatible" list of a node.
         For example, the binding for "nordic,nrf-swi" is likely to
         always be masked by a more specific compatible, e.g. "nordic,nrf-egu".
         """
         return self._bindings
 
-    def dt_binding(self, compat: str) -> Binding | None:
+    def dt_binding(self, compat: str) -> Union[Binding, None]:
         """Access bindings by their compatible.
 
         See Dtsh.dt_bindings() for limitations.
 
         Arguments:
         compat -- a compatible (DTSpec 2.3.1)
 
         Returns the binding describing this compatible,
         or None when this compatible is either unmatched or not described.
         """
         return self._bindings.get(compat)
 
-    def dt_binding_path(self, fname: str) -> str | None:
+    def dt_binding_path(self, fname: str) -> Union[str, None]:
         """Search binding directories for a given DT specification file name.
 
         Contrary to the Dtsh.dt_binding() API, this search is not limited
         to bindings that describe a compatible.
 
         Arguments
         fname -- the YAML file name, e.g. "nordic,nrf-swi.yaml"
 
         Returns the full path of the YAML file, or None when not found.
         """
         return self._binding2path.get(fname)
 
     @property
-    def dt_aliases(self) -> dict[str, Node]:
-        aliases = dict[str, Node]()
+    def dt_aliases(self) -> Dict[str, Node]:
+        aliases: Dict[str, Node] = {}
         for alias, dt_node in self._edt._dt.alias2node.items():
             edt_node = self._edt.get_node(dt_node.path)
             aliases[alias] = edt_node
         return aliases
 
     @property
-    def dt_chosen(self) -> dict[str, Node]:
+    def dt_chosen(self) -> Dict[str, Node]:
         return self._edt.chosen_nodes
 
-    def builtin(self, name: str) -> DtshCommand | None:
+    def builtin(self, name: str) -> Union[DtshCommand, None]:
         """Access a built-in by command name.
 
         Arguments:
         name -- a command name
 
         Returns None if this  built-in name is not supported by this command.
         """
@@ -1048,15 +1095,15 @@
         Raises:
         - ValueError when path is unspecified
         - DtshError when the destination node does not exist
         """
         path = self.realpath(path)
         self._cwd = self.path2node(path)
 
-    def ls(self, path: str) -> list[Node]:
+    def ls(self, path: str) -> List[Node]:
         """List a devicetree node's children.
 
         The path is first resolved (see `Dtsh.realpath()`) to:
 
            <directory>[<filter>]
 
            <filter> := [/][<prefix>]'*'
@@ -1101,15 +1148,15 @@
 
         if path.endswith('*'):
             dirpath = Dtsh.dirname(path)
             prefix = path[:-1]
             return [n for n in self.ls(dirpath) if n.path.startswith(prefix)]
         else:
             dirnode = self.path2node(path)
-            return list[Node](dirnode.children.values())
+            return list(dirnode.children.values())
 
     def exec_command_string(self, cmd_str: str, vt: DtshVt) -> None:
         """Execute a command string.
 
         Note that the command string content after any '--' token
         will be interpreted as command parameters.
 
@@ -1239,22 +1286,14 @@
         if not path_prefix.endswith('/'):
             path_prefix += '/'
         if path.endswith('/'):
             path = path[:-1]
 
         return path_prefix + path
 
-    @staticmethod
-    def cfg_dir_path() -> str:
-        xdg_cfg_dir = os.environ.get('XDG_CONFIG_HOME')
-        if not xdg_cfg_dir:
-            home = os.path.expanduser('~')
-            xdg_cfg_dir = os.path.join(home, '.config')
-        return os.path.join(xdg_cfg_dir, 'dtsh')
-
     def _init_bindings(self) -> None:
         # EDT.compat2nodes includes all compatibles matched by a devicetree node.
         # See also EDT._init_luts().
         for compat, nodes in self._edt.compat2nodes.items():
             # A compatible may not map to any binding in the devicetree
             # underlying model:
             # - a compatible that represents a board, for which the binding
@@ -1306,15 +1345,15 @@
                     binding = Binding(path, self._binding2path)
             if binding:
                 self._bindings[compat] = binding
 
     def _init_binding_paths(self) -> None:
         # Mostly duplicates code from edtlib._binding_paths()
         # and edtlib.EDT._init_compat2binding().
-        yaml_paths = list[str]()
+        yaml_paths: List[str] = []
         for bindings_dir in self._edt.bindings_dirs:
             for root, _, filenames in os.walk(bindings_dir):
                 for filename in filenames:
                     if filename.endswith(".yaml") or filename.endswith(".yml"):
                         yaml_paths.append(os.path.join(root, filename))
         for path in yaml_paths:
             self._binding2path[os.path.basename(path)] = path
@@ -1347,24 +1386,24 @@
     @abstractmethod
     def count(self) -> int:
         """Current completions count.
         """
 
     @property
     @abstractmethod
-    def hints(self) -> list[str]:
+    def hints(self) -> List[str]:
         """Current completion state.
 
         This is the list of completion strings that match the last prefix
         provided to autocomplete().
         """
 
     @property
     @abstractmethod
-    def model(self) -> list:
+    def model(self) -> List[Any]:
         """Current completion model.
 
         This is the model objects correponding to the current completion hints.
 
         Permits rich implementation of the rl_completion_display_matches_hook()
         callback.
         """
@@ -1382,37 +1421,37 @@
         """Reset current completion state and model.
         """
 
     @abstractmethod
     def autocomplete(self,
                      cmdline: str,
                      prefix: str,
-                     cursor: int = -1) -> list[str]:
+                     cursor: int = -1) -> List[str]:
         """Auto-complete command line.
 
         Arguments:
         cmdline -- the command line's current content
         prefix -- the prefix word to complete
         cursor -- required to get the full command line's state,
                   but unsupported
 
         Returns the completion state (hint strings) matching the prefix.
         """
 
     @staticmethod
-    def autocomplete_with_nodes(prefix: str, shell: Dtsh) -> list[Node]:
+    def autocomplete_with_nodes(prefix: str, shell: Dtsh) -> List[Node]:
         """Helper function to auto-complete with a list of nodes.
 
         Arguments:
         prefix -- the node path prefix
         shell -- the shell instance the nodes belong to
 
         Returns a list of matching nodes.
         """
-        completions = list[Node]()
+        completions: List[Node] = []
 
         if prefix:
             path_prefix = shell.realpath(prefix)
             if prefix.endswith('/'):
                 path = path_prefix
             else:
                 path = Dtsh.dirname(path_prefix)
@@ -1430,65 +1469,67 @@
             pass
 
         return completions
 
     @staticmethod
     def autocomplete_with_properties(node_prefix: str,
                                      prop_prefix: str,
-                                     shell: Dtsh) -> list[Property]:
+                                     shell: Dtsh) -> List[Property]:
 
-        completions = list[Property]()
+        completions: List[Property] = []
         path_prefix = shell.realpath(node_prefix)
         if shell.isnode(path_prefix):
             node = shell.path2node(path_prefix)
             for _, p in node.props.items():
                 if p.name.startswith(prop_prefix) and len(p.name) > len(prop_prefix):
                     completions.append(p)
         return completions
 
 
 class DtshError(Exception):
     """Base exception for devicetree shell errors.
     """
 
-    _msg: str
-    _cause: Exception | None
+    _msg: Union[str, None]
+    _cause: Union[Exception, None]
 
-    def __init__(self, msg: str, cause: Exception | None = None) -> None:
+    def __init__(self,
+                 msg: Optional[str],
+                 cause: Optional[Exception] = None) -> None:
         """Create an error.
 
         Arguments:
         msg -- the error message
         cause -- the exception that caused this error, if any
         """
         super().__init__(msg)
         self._msg = msg
         self._cause = cause
 
     @property
     def msg(self) -> str:
         """The error message.
         """
-        return self._msg
+        return self._msg or ''
 
     @property
-    def cause(self) -> Exception | None:
+    def cause(self) -> Union[Exception, None]:
         """The error cause as an exception, or None.
         """
         return self._cause
 
 
 class DtshCommandUsageError(DtshError):
     """A devicetree shell command execution has failed.
     """
 
     def __init__(self,
                  command: DtshCommand,
-                 msg: str,
-                 cause: Exception | None = None) -> None:
+                 msg: Optional[str] = None,
+                 cause: Optional[Exception] = None) -> None:
         """Create a new error.
 
         Arguments:
         command -- the failed command
         msg -- a message describing the usage error
         cause -- the cause exception, if any
         """
@@ -1505,15 +1546,15 @@
 class DtshCommandFailedError(DtshError):
     """A devicetree shell command execution has failed.
     """
 
     def __init__(self,
                  command: DtshCommand,
                  msg: str,
-                 cause: Exception | None = None) -> None:
+                 cause: Optional[Exception] = None) -> None:
         """Create a new error.
 
         Arguments:
         command -- the failed command
         msg -- the failure message
         cause -- the failure cause, if any
         """
@@ -1567,15 +1608,15 @@
     @abstractmethod
     def autocomp(self) -> DtshAutocomp:
         """The session's command line completer.
         """
 
     @property
     @abstractmethod
-    def last_err(self) -> DtshError | None:
+    def last_err(self) -> Union[DtshError, None]:
         """Last error triggered by a command execution.
         """
 
     @abstractmethod
     def run(self):
         """Enter interactive mode main loop.
         """
```

### Comparing `dtsh-0.1.0a4/src/dtsh/man.py` & `dtsh-0.1.0a6/src/dtsh/man.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """Manual pages for devicetree shells."""
 
 import re
 
 from abc import abstractmethod
+from typing import List, Union
 
 from devicetree.edtlib import Binding
 
 from rich.console import RenderableType
 from rich.markdown import Markdown
 from rich.padding import Padding
 from rich.table import Table
@@ -147,37 +148,37 @@
             content_vstr = content.splitlines()
             # Skip until 1st section
             for i, line in enumerate(content_vstr):
                 if self._is_section_header(line):
                     content_vstr = content_vstr[i:]
                     break
             # Parse all sections.
-            sec_name: str | None = None
-            sec_vstr: list[str] | None = None
+            sec_name: Union[str, None] = None
+            sec_vstr: Union[List[str], None] = None
             for line in content_vstr:
                 line = line.rstrip()
                 if self._is_section_header(line):
                     # Add current section's content to view if any.
                     if sec_name and sec_vstr:
                         self._add_section(sec_name, sec_vstr)
                     # Init new section's content.
-                    sec_vstr = list[str]()
+                    sec_vstr = []
                     sec_name = line
                 else:
                     # Append line to current section.
                     if sec_vstr is not None:
                         sec_vstr.append(line)
 
             if sec_name and sec_vstr:
                 self._add_section(sec_name, sec_vstr)
 
     def _is_section_header(self, line: str) -> bool:
         return self._re.match(line) is not None
 
-    def _add_section(self, name: str, vstr: list[str]) -> None:
+    def _add_section(self, name: str, vstr: List[str]) -> None:
         md_src = '\n'.join(vstr)
         md = Markdown(md_src)
         self._add_named_content(name, md)
 
 
 class DtshManPageBinding(DtshManPage):
     """
@@ -206,20 +207,20 @@
         self._add_named_content('binding', grid)
 
     def _add_content_desc(self) -> None:
         self._add_named_content('description',
                                 DtshTui.mk_txt_desc(self._binding.description))
 
     def _add_content_bus(self) -> None:
-        if not (self._binding.bus or self._binding.on_bus):
+        if not (self._binding.buses or self._binding.on_bus):
             return
 
-        if self._binding.bus:
-            str_label = "Nodes with this compatible's binding describe bus"
-            str_bus = self._binding.bus
+        if self._binding.buses:
+            str_label = "Nodes with this compatible's binding support buses"
+            str_bus = " ".join(self._binding.buses)
         else:
             str_label = "Nodes with this compatible's binding appear on bus"
             str_bus = self._binding.on_bus
 
         txt = DtshTui.mk_txt(f'{str_label}: ')
         txt.append_text(
             DtshTui.mk_txt(str_bus, DtshTui.style(DtshTui.STYLE_DT_BUS))
@@ -283,39 +284,39 @@
         md_src = _DTSH_MAN_PAGE.strip()
         md = Markdown(md_src)
         self._view.add_row(Padding(md, (0,8)))
         self._view.add_row(None)
 
     def _add_content_as_sections(self):
         # Parse all sections.
-        sec_name: str | None = None
-        sec_vstr: list[str] | None = None
+        sec_name: Union[str, None] = None
+        sec_vstr: Union[List[str], None] = None
         content_vstr = _DTSH_MAN_PAGE.strip().splitlines()
         for line in content_vstr:
             line = line.rstrip()
             if self._is_section_header(line):
                 # Add current section's content to view if any.
                 if sec_name and sec_vstr:
                     self._add_section(sec_name, sec_vstr)
                 # Init new section's content.
-                sec_vstr = list[str]()
+                sec_vstr = []
                 sec_name = line
             else:
                 # Append line to current section.
                 if sec_vstr is not None:
                     sec_vstr.append(line)
 
         if sec_name and sec_vstr:
             self._add_section(sec_name, sec_vstr)
 
 
     def _is_section_header(self, line: str) -> bool:
         return self._re.match(line) is not None
 
-    def _add_section(self, name: str, vstr: list[str]) -> None:
+    def _add_section(self, name: str, vstr: List[str]) -> None:
         md_src = '\n'.join(vstr)
         md = Markdown(md_src)
         self._add_named_content(name, md)
 
 
 _DTSH_MAN_PAGE="""
 # dtsh
```

### Comparing `dtsh-0.1.0a4/src/dtsh/session.py` & `dtsh-0.1.0a6/src/dtsh/session.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Devicetree shell session."""
 
 
+from typing import cast, List, Optional, Union
+
 import os
 import re
-import readline
 import signal
 import sys
 
 from devicetree.edtlib import Node, Binding, Property
 
 from rich.console import Console
 from rich.text import Text
 
+from dtsh.rl import readline
 from dtsh.dtsh import Dtsh, DtshAutocomp, DtshCommand, DtshCommandOption, DtshSession, DtshVt
 from dtsh.dtsh import DtshError, DtshCommandNotFoundError, DtshCommandUsageError, DtshCommandFailedError
 from dtsh.shell import DevicetreeShell
 from dtsh.term import DevicetreeTerm
 from dtsh.autocomp import DevicetreeAutocomp
 from dtsh.tui import DtshTui
+from dtsh.config import DtshConfig
 
 
 class DevicetreeShellSession(DtshSession):
     """Shell session with GNU readline history support.
     """
 
     _dtsh: Dtsh
     _term: DevicetreeTerm
-    _last_err: DtshError | None
+    _last_err: Union[DtshError, None]
 
     def __init__(self, shell: Dtsh, term: DevicetreeTerm) -> None:
         """Creates a session.
 
         Arguments:
         shell - the session's shell instance
         term - the session's rich VT
         """
         self._dtsh = shell
         self._term = term
         self._last_err = None
 
-        self.readline_read_history()
+        DtshConfig.readline_read_history()
 
     @property
     def term(self) -> DevicetreeTerm:
         """Session's VT."""
         return self._term
 
     @property
-    def last_err(self) -> DtshError | None:
+    def last_err(self) -> Union[DtshError, None]:
         return self._last_err
 
     def run(self):
         """Overrides DtshSession.run().
         """
         self._term.clear()
         self.banner()
@@ -79,16 +82,19 @@
                     else:
                         self._dtsh.exec_command_string(cmdline, self._term)
 
             except DtshCommandNotFoundError as e:
                 self._last_err = e
                 self._term.write(f'dtsh: Command not found: {e.name}')
             except DtshCommandUsageError as e:
-                self._last_err = e
-                self._term.write(f'{e.command.name}: {e.msg}')
+                if e.command.with_help:
+                    self._term.write(e.command.usage)
+                else:
+                    self._last_err = e
+                    self._term.write(f'{e.command.name}: {e.msg}')
             except DtshCommandFailedError as e:
                 self._last_err = e
                 self._term.write(f'{e.command.name}: {e.msg}')
             except EOFError:
                 self._term.abort()
                 self.close()
 
@@ -99,15 +105,15 @@
             if DtshTui.PROMPT_SPARSE:
                 self._term.write()
 
     def close(self) -> None:
         """Overrides DtshSession.close().
         """
         self._term.write('bye.', style=DtshTui.style_italic())
-        self.readline_write_history()
+        DtshConfig.readline_write_history()
         sys.exit(0)
 
     def banner(self):
         """
         """
         self._term.write(
             Text().append_tokens(
@@ -138,31 +144,17 @@
                     (', or press ', DtshTui.style_default()),
                     ('Ctrl-D', DtshTui.style_bold()),
                 ]
             )
         )
         self._term.write()
 
-    def readline_hist_path(self) -> str:
-        return os.path.join(Dtsh.cfg_dir_path(), 'history')
-
-    def readline_read_history(self):
-        hist_path = self.readline_hist_path()
-        if os.path.isfile(hist_path):
-            readline.read_history_file(hist_path)
-
-    def readline_write_history(self):
-        cfg_path = Dtsh.cfg_dir_path()
-        if not os.path.isdir(cfg_path):
-            os.mkdir(cfg_path)
-        readline.write_history_file(self.readline_hist_path())
-
     @staticmethod
-    def open(dt_source_path: str | None = None,
-             dt_bindings_path: list[str] | None = None) -> DtshSession:
+    def open(dt_source_path: Optional[str] = None,
+             dt_bindings_path: Optional[List[str]] = None) -> DtshSession:
         """
         """
         global _session
         global _autocomp
 
         if _session is not None:
             raise DtshError('Session already opened')
@@ -178,21 +170,21 @@
         # We disable SIGINT (CTRL-C event).
         signal.signal(signal.SIGINT, dtsh_session_sig_handler)
 
         return _session
 
 
 # Shell session singleton state.
-_session: DevicetreeShellSession | None = None
-_autocomp: DevicetreeAutocomp | None = None
+_session: Union[DevicetreeShellSession, None] = None
+_autocomp: Union[DevicetreeAutocomp, None] = None
 
 
 # GNU readline completer function callback for rl_completion_matches().
 # MUST answer completions that actually match te given prefix.
-def readline_completions_hook(text: str, state: int) -> str | None:
+def readline_completions_hook(text: str, state: int) -> Union[str, None]:
     if _autocomp is None:
         return None
 
     cmdline = readline.get_line_buffer()
     completions = _autocomp.autocomplete(cmdline, text, 0)
 
     if state < len(completions):
@@ -223,27 +215,27 @@
     cmdline = readline.get_line_buffer()
 
     # Go bellow input line
     _session.term.write()
 
     if _autocomp.model:
         if _autocomp.mode == DtshAutocomp.MODE_DTSH_CMD:
-            model = list[DtshCommand](_autocomp.model)
+            model = cast(List[DtshCommand], _autocomp.model)
             view = DtshTui.mk_command_hints_display(model)
         elif _autocomp.mode == DtshAutocomp.MODE_DTSH_OPT:
-            model = list[DtshCommandOption](_autocomp.model)
+            model = cast(List[DtshCommandOption], _autocomp.model)
             view = DtshTui.mk_option_hints_display(model)
         elif _autocomp.mode == DtshAutocomp.MODE_DT_BINDING:
-            model = list[Binding](_autocomp.model)
+            model = cast(List[Binding], _autocomp.model)
             view = DtshTui.mk_binding_hints_display(model)
         elif _autocomp.mode == DtshAutocomp.MODE_DT_NODE:
-            model = list[Node](_autocomp.model)
+            model = cast(List[Node], _autocomp.model)
             view = DtshTui.mk_node_hints_display(model)
         elif _autocomp.mode == DtshAutocomp.MODE_DT_PROP:
-            model = list[Property](_autocomp.model)
+            model = cast(List[Property], _autocomp.model)
             view = DtshTui.mk_property_hints_display(model)
         else:
             # Autcomp mode MODE_ANY.
             view = DtshTui.mk_grid(1)
             for m in _autocomp.model:
                 view.add_row(DtshTui.mk_txt(str(m)))
         _session.term.write(view)
@@ -349,15 +341,15 @@
     def _write_svg(self):
         svg = self._console.export_svg(title='')
         # Remove macOS-ish windows buttons.
         s = re.search(_RE_SVG_BUTTONS, svg)
         if s:
             svg = svg[:s.start()] + svg[s.end() + 1:]
         # Remove top padding
-        svg_vstr = list[str]()
+        svg_vstr: List[str] = []
         re_view = re.compile(_RE_SVG_VIEWPORT)
         re_rect = re.compile(_RE_SVG_RECT)
         re_trans = re.compile(_RE_SVG_TRANSFORM)
         for line in svg.splitlines(keepends=True):
             # Substract hard coded padding to viewport's height.
             m = re_view.match(line)
             if m and m.groups():
```

### Comparing `dtsh-0.1.0a4/src/dtsh/shell.py` & `dtsh-0.1.0a6/src/dtsh/shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Devicetree shell PoC implementation."""
 
 import os
+from typing import List, Optional
 
 from devicetree.edtlib import EDT
-from dtsh.builtin_find import DtshBuiltinFind
 
 from dtsh.dtsh import Dtsh, DtshUname, DtshError
 from dtsh.builtin_pwd import DtshBuiltinPwd
 from dtsh.builtin_alias import DtshBuiltinAlias
 from dtsh.builtin_chosen import DtshBuiltinChosen
 from dtsh.builtin_cd import DtshBuiltinCd
 from dtsh.builtin_ls import DtshBuiltinLs
 from dtsh.builtin_tree import DtshBuiltinTree
+from dtsh.builtin_find import DtshBuiltinFind
 from dtsh.builtin_cat import DtshBuiltinCat
 from dtsh.builtin_man import DtshBuiltinMan
 from dtsh.builtin_uname import DtshBuiltinUname
 
 
 class DevicetreeShell(Dtsh):
     """Devicetree shell PoC implementation.
@@ -43,16 +44,16 @@
                 DtshBuiltinUname(self),
                 DtshBuiltinFind(self),
                 DtshBuiltinMan(self)
                 ]:
             self._builtins[cmd.name] = cmd
 
     @staticmethod
-    def create(dt_source_path: str | None = None,
-               dt_bindings_path: list[str] | None = None) -> Dtsh:
+    def create(dt_source_path: Optional[str] = None,
+               dt_bindings_path: Optional[List[str]] = None) -> Dtsh:
         """Create a shell-like interface to a devicetree .
 
         Factory method that loads a devicetree source file and its bindings
         to build a devicetree model (EDT).
         On success, creates a shell-like interface to this devicetree.
 
         Arguments:
```

### Comparing `dtsh-0.1.0a4/src/dtsh/systools.py` & `dtsh-0.1.0a6/src/dtsh/systools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Host system tools helpers."""
 
 
-from typing import Any
+from typing import Any, Dict, List, Union
 
 import os
 import re
 import sys
 import yaml
 from pathlib import Path
 from subprocess import Popen, PIPE
@@ -18,26 +18,26 @@
 
 
 class CMakeCache(object):
     """Access CMake cached variables.
     """
 
     # CMake cached variables name to value.
-    _cache: dict[str,str]
+    _cache: Dict[str,str]
 
     def __init__(self, build_dir: str) -> None:
         """Initialize the CMake helper with a build directory content.
 
         Will silently fail with an empty cache if the CMake binary is not found,
         or the build directory is invalid.
 
         Argument:
         build_dir -- path to a valid CMake build directory
         """
-        self._cache = dict[str,str]()
+        self._cache = {}
         try:
             argv = [
                 'cmake.exe' if os.name == 'nt' else 'cmake',
                 # List non-advanced cached variables.
                 '-L',
                 # Only load the cache. Do not actually run configure and generate steps.
                 '-N',
@@ -50,15 +50,15 @@
             else:
                 # Dump CMake error.
                 print(stderr, file=sys.stderr)
         except Exception:
             # Silently fail (cmake is probably unavailable).
             pass
 
-    def get(self, name: str) -> str | None:
+    def get(self, name: str) -> Union[str, None]:
         """Access CMake cached variables.
 
         Arguments:
         name -- the variable name, e.g. APPLICATION_SOURCE_DIR
 
         Returns the variable value or None.
         """
@@ -77,15 +77,15 @@
     """
 
     def __init__(self) -> None:
         """Initialize helper for host operating system.
         """
         self._git = 'git.exe' if os.name == 'nt' else 'git'
 
-    def get_head_commit(self, repo_path: str) -> str | None:
+    def get_head_commit(self, repo_path: str) -> Union[str, None]:
         """Returns git -C $ZEPHYR_BASE log -n 1 --pretty=format:"%h", or None.
         """
         rev = None
         try:
             argv = [
                 self._git,
                 '-C', f'{repo_path}',
@@ -101,18 +101,18 @@
                 # Dump git error.
                 print(stderr, file=sys.stderr)
         except Exception:
             # Silently fail (git is probably unavailable).
             pass
         return rev
 
-    def get_head_tags(self, repo_path: str) -> list[str]:
+    def get_head_tags(self, repo_path: str) -> List[str]:
         """Returns git tag --points-at HEAD, or None.
         """
-        tags = list[str]()
+        tags: List[str] = []
         try:
             argv = [
                 self._git,
                 '-C', f'{repo_path}',
                 'tag',
                 '--points-at', 'HEAD',
             ]
@@ -131,24 +131,24 @@
 
 
 class GCCArm(object):
     """GCC Arm Embedded Toolchain helper.
     """
 
     # Resolved path to arm-none-eabi-gcc.
-    _gcc: str | None
+    _gcc: Union[str, None]
 
     # Toolchain, e.g.: GNU Arm Embedded Toolchain 10.3-2021.10
-    _toolchain: str | None
+    _toolchain: Union[str, None]
 
     # GCC version.
-    _version: str | None
+    _version: Union[str, None]
 
     # Build date, e.g. 20210824
-    _build_date: str | None
+    _build_date: Union[str, None]
 
     def __init__(self, gnuarm_dir: str) -> None:
         """Initialize helper for host operating system.
         """
         self._gcc = None
         self._toolchain = None
         self._version = None
@@ -169,23 +169,23 @@
                     # Dump gcc error.
                     print(stderr, file=sys.stderr)
             except Exception:
                 # Silently fail (gcc is probably unavailable).
                 pass
 
     @property
-    def toolchain(self) -> str | None:
+    def toolchain(self) -> Union[str, None]:
         return self._toolchain
 
     @property
-    def version(self) -> str | None:
+    def version(self) -> Union[str, None]:
         return self._version
 
     @property
-    def build_date(self) -> str | None:
+    def build_date(self) -> Union[str, None]:
         return self._build_date
 
     def _init_version(self, cmake_stdout: str) -> None:
         # GCC Arm 10:
         # arm-none-eabi-gcc (GNU Arm Embedded Toolchain 10.3-2021.10) 10.3.1 20210824 (release)
         #
         # GCC Arm 11:
@@ -232,16 +232,16 @@
         return f"{self.home}/commit/{commit}"
 
 
 class YamlFile(object):
     """YAML binding file.
     """
 
-    _yaml: Any | None
-    _content: str | None
+    _yaml: Union[Any, None]
+    _content: Union[str, None]
 
     def __init__(self, path: str):
         """
         """
         yaml_file = None
         try:
             yaml_file = open(path, mode='r', encoding="utf-8")
@@ -251,34 +251,34 @@
             self._content = None
             self._yaml = None
         finally:
             if yaml_file:
                 yaml_file.close()
 
     @property
-    def content(self) -> str | None:
+    def content(self) -> Union[str, None]:
         """Returns the YAML file content, or None.
         """
         return self._content
 
     @property
-    def include(self) -> list[str]:
+    def include(self) -> List[str]:
         """Returns the list of included YAML files.
         """
-        inc_names = list[str]()
+        inc_names: List[str] = []
         if self._yaml:
             yaml_include = self._yaml.get('include')
             if isinstance(yaml_include, str):
                 inc_names.append(yaml_include)
             elif isinstance(yaml_include, list):
                 for name in yaml_include:
                     inc_names.append(name)
         return inc_names
 
-    def get(self, key: str) -> Any | None:
+    def get(self, key: str) -> Union[Any, None]:
         """Access YAML content by key.
 
         Argument:
         key -- the YAML key
         Returns the mapped content value, or None.
         """
         if self._yaml:
```

### Comparing `dtsh-0.1.0a4/src/dtsh/term.py` & `dtsh-0.1.0a6/src/dtsh/term.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # Copyright (c) 2022 Chris Duf <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Rich terminal for devicetree shells."""
 
-import readline
+from typing import Union
+
 
 from rich.console import Console, PagerContext
 
+from dtsh.rl import readline
 from dtsh.dtsh import DtshVt
 from dtsh.tui import DtshTui
 
 
 class DevicetreeTerm(DtshVt):
     """Rich terminal for devicetree shells.
 
     Rich standard output and pager support with the Python rich library,
     standard input with GNU readline completion.
     """
 
     _console: Console
-    _pager: PagerContext | None
+    _pager: Union[PagerContext, None]
 
     def __init__(self,
                  readline_comp_hook = None,
                  readline_display_hook = None) -> None:
         """Initialize a rich terminal.
 
         Creates a rich console and setup GNU readline completion support.
```

### Comparing `dtsh-0.1.0a4/src/dtsh/theme` & `dtsh-0.1.0a6/src/dtsh/theme`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a4/src/dtsh/tui.py` & `dtsh-0.1.0a6/src/dtsh/tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Devicetree shell UI components."""
 
 
 from abc import abstractmethod
-from typing import ClassVar
+from typing import ClassVar, Optional, Union, List, Dict
 
 import configparser
 import os
+import pathlib
 import yaml
 
 from devicetree.edtlib import ControllerAndData, Loader as edtlib_YamlLoader
 from devicetree.edtlib import Node, Binding, Property, PropertySpec, Register
 
 from rich import box
 from rich.console import RenderableType
@@ -22,20 +23,21 @@
 from rich.syntax import Syntax
 from rich.table import Table
 from rich.text import Text
 from rich.theme import Theme
 from rich.tree import Tree
 
 from dtsh.dtsh import Dtsh, DtshCommand, DtshCommandOption, DtshVt, DtshError
+from dtsh.config import DtshConfig
 
 
 class DtshTui:
 
     # DTSH theme.
-    _theme: ClassVar[Theme|None] = None
+    _theme: ClassVar[Union[Theme, None]] = None
 
     # Common UTF-8 symbols.
     #
     WCHAR_ELLIPSIS = '\u2026'
     WCHAR_COPYRIGHT = '\u00a9'
     WCHAR_HYPHEN = '\u2014'
     WCHAR_DASH = '\ufe4d'
@@ -208,50 +210,51 @@
         return Text(val_str, style)
 
     @staticmethod
     def mk_txt_warn(msg: str) -> Text:
         return Text(msg, style='dtsh.warning')
 
     @staticmethod
-    def mk_txt_desc(desc: str | None) -> Text:
+    def mk_txt_desc(desc: Optional[str]) -> Text:
         if not desc:
             return Text("No description available.",
                         DtshTui.style(DtshTui.STYLE_APOLOGY))
         return Text(desc.strip(), DtshTui.style(DtshTui.STYLE_DT_DESC))
 
     @staticmethod
-    def mk_txt_desc_short(desc: str | None) -> Text:
+    def mk_txt_desc_short(desc: Optional[str]) -> Text:
         if not desc:
             return Text()
         desc_lines = desc.strip().split('\n')
         desc_short = desc_lines[0]
         if len(desc_lines) > 1:
             if desc_short.endswith('.'):
                 desc_short = desc_short[:-1]
             desc_short += DtshTui.WCHAR_ELLIPSIS
         return Text(desc_short, DtshTui.style(DtshTui.STYLE_DT_DESC))
 
     @staticmethod
     def mk_txt_link(label: str,
                     url: str,
-                    style: StyleType | None = None) -> Text:
+                    style: Optional[StyleType] = None) -> Text:
         """Returns a text link.
 
         Arguments:
         label - the link label
         link - the link URL, e.g. https://docs.zephyrproject.org/
         style - the label's style
         """
         txt = Text(label, style=style or 'default')
         txt.stylize(Style(link=f'{url}'))
         return txt
 
     @staticmethod
     def txt_update_link_file(txt: Text, path: str) -> None:
-        txt.stylize(Style(link=f'file:{path}'))
+        uri = pathlib.Path(path).as_uri()
+        txt.stylize(Style(link=uri))
 
     @staticmethod
     def txt_dim(txt: Text) -> None:
         if isinstance(txt.style, Style):
             style = txt.style.without_color
         else:
             style = Style.parse(txt.style).without_color
@@ -280,63 +283,54 @@
         if with_status and (node.status != 'okay'):
             DtshTui.txt_dim(txt)
         return txt
 
     @staticmethod
     def mk_txt_node_bus_device(node: Node, with_status: bool = False) -> Text:
         txt = Text()
-        if node.bus:
+        if node.buses:
+            buses: List[str] = node.buses
             txt = txt.append_text(
-                DtshTui.mk_txt(node.bus, DtshTui.style(DtshTui.STYLE_DT_BUS))
+                DtshTui.mk_txt(' '.join(buses),
+                               DtshTui.style(DtshTui.STYLE_DT_BUS))
             )
-        if node.on_bus:
+        if node.on_buses:
+            buses: List[str] = node.on_buses
             prefix = "on "
             if len(txt.plain) > 0:
                 prefix = " " + prefix
             txt = txt.append_text(DtshTui.mk_txt(prefix))
             txt = txt.append_text(
-                DtshTui.mk_txt(str(node.on_bus),
+                DtshTui.mk_txt(' '.join(buses),
                                DtshTui.style(DtshTui.STYLE_DT_ON_BUS))
             )
         if (len(txt.plain) > 0) and with_status and (node.status != 'okay'):
             DtshTui.txt_dim(txt)
         return txt
 
     @staticmethod
-    def mk_txt_node_registers(node: Node,
-                              with_status: bool = False) -> RenderableType:
-        if not node.regs:
-            return Text()
-        reg_rows = list[Text]()
+    def mk_txt_node_register(node: Node,
+                             with_status: bool = False) -> Text:
         for reg in node.regs:
-            txt = DtshTui.mk_txt_node_register(reg)
-            if with_status and (node.status != 'okay'):
-                DtshTui.txt_dim(txt)
-            reg_rows.append(txt)
-        if len (reg_rows) == 1:
-            return reg_rows[0]
-        grid = DtshTui.mk_grid(1)
-        for reg_row in reg_rows:
-            grid.add_row(reg_row)
-        return grid
-
-    @staticmethod
-    def mk_txt_node_register(reg: Register) -> Text:
-        reg_addr = hex(reg.addr) if (reg.addr is not None) else hex(0)
-        reg_size = hex(reg.size) if (reg.size is not None) else None
-        if reg_size is not None:
-            return Text(f"<{reg_addr} {reg_size}>")
-        return Text(f"<{reg_addr}>")
+            if (reg.addr is not None) and (reg.addr == node.unit_addr):
+                if reg.size is not None:
+                    txt = Text(f"<{hex(reg.addr)} {hex(reg.size)}>")
+                else:
+                    txt = Text(f"<{hex(reg.addr)}>")
+                if with_status and not Dtsh.is_node_enabled(reg.node):
+                    DtshTui.txt_dim(txt)
+                return txt
+        return Text()
 
     @staticmethod
     def mk_txt_node_interrupts(node: Node,
                                with_status: bool = False) -> RenderableType:
         if not node.interrupts:
             return Text()
-        irq_rows = list[Text]()
+        irq_rows: List[Text] = []
         for irq in node.interrupts:
             txt = DtshTui.mk_txt_node_irq(irq)
             if with_status and (node.status != 'okay'):
                 DtshTui.txt_dim(txt)
             irq_rows.append(txt)
         if len(irq_rows) == 1:
             return irq_rows[0]
@@ -353,15 +347,15 @@
             if ctrl_data.name:
                 txt = Text(f"{ctrl_data.name}[{irq}]",
                            DtshTui.style(DtshTui.STYLE_DT_IRQ))
             else:
                 txt = Text(f"IRQ_{irq}", DtshTui.style(DtshTui.STYLE_DT_IRQ))
             txt.append_text(DtshTui.mk_txt(f"/{level}"))
         else:
-            irq_data = list[Text]()
+            irq_data: List[Text] = []
             for k, v in ctrl_data.data.items():
                 irq_data.append(DtshTui.mk_txt(f"{k}:{str(v)}"))
             txt = Text(" ").join(irq_data)
         return txt
 
     @staticmethod
     def mk_txt_node_path(path:str) -> Text:
@@ -375,15 +369,15 @@
         if path == '/':
             return Text('/', DtshTui.style('dtsh.path.anchor'))
 
         path_segments = path.split('/')
         # Skip path_segments[0] == ''.
         path_segments = path_segments[1:]
 
-        txt_segments = list[Text]()
+        txt_segments: List[Text] = []
         for i, seg in enumerate(path_segments):
             if (i == 0) or (i == len(path_segments) - 1):
                 txt_segments.append(
                     DtshTui.mk_txt(seg, DtshTui.style('dtsh.path.anchor'))
                 )
             else:
                 txt_segments.append(
@@ -418,15 +412,15 @@
     @staticmethod
     def mk_txt_node_compats(node: Node,
                             shell: Dtsh,
                             with_link: bool = True,
                             with_status: bool = False) -> Text:
         if not node.compats:
             return Text()
-        txt_bindings = list[Text]()
+        txt_bindings: List[Text] = []
         for compat in node.compats:
             txt = Text(compat, DtshTui.style(DtshTui.STYLE_DT_COMPATS))
             if compat == node.matching_compat:
                 txt.stylize(DtshTui.style('bold'))
             if with_link:
                 binding = shell.dt_binding(compat)
                 if binding and binding.path:
@@ -451,15 +445,15 @@
     @staticmethod
     def mk_txt_node_labels(node: Node, with_status: bool = False) -> Text:
         """Returns a rich Text element with all DT labels for the node,
         in the order they appear in the DT source, or an empty Text().
         """
         if not node.labels:
             return Text()
-        txt_labels = list[Text]()
+        txt_labels: List[Text] = []
         for label in node.labels:
             txt = Text(label, DtshTui.style(DtshTui.STYLE_DT_LABELS))
             if with_status and (node.status != 'okay'):
                 DtshTui.txt_dim(txt)
             txt_labels.append(txt)
         txt = Text(', ', DtshTui.style(DtshTui.STYLE_DEFAULT)).join(txt_labels)
         return txt
@@ -479,15 +473,15 @@
         txt.append_text(DtshTui.mk_txt_node_labels(node, with_status=with_status))
         return txt
 
     @staticmethod
     def mk_txt_node_aliases(node: Node, with_status: bool = False) -> Text:
         if not node.aliases:
             return Text()
-        txt_aliases = list[Text]()
+        txt_aliases: List[Text] = []
         for alias in node.aliases:
             txt_aliases.append(Text(alias, DtshTui.style(DtshTui.STYLE_DT_ALIAS)))
         txt = Text(' ').join(txt_aliases)
         if with_status and (node.status != 'okay'):
             DtshTui.txt_dim(txt)
         return txt
 
@@ -575,43 +569,43 @@
         return Text(str(dt_val))
 
     ############################################################################
     # Autocomp hints.
     ############################################################################
 
     @staticmethod
-    def mk_command_hints_display(model: list[DtshCommand]) -> Table:
+    def mk_command_hints_display(model: List[DtshCommand]) -> Table:
         """Layout command completion hints.
 
         Arguments:
         model -- a command list to display as hints
 
         Returns a rich table.
         """
         tab = DtshTui.mk_grid(2)
         for cmd in model:
             tab.add_row(DtshTui.mk_txt(cmd.name), DtshTui.mk_txt_dim(cmd.desc))
         return tab
 
     @staticmethod
-    def mk_option_hints_display(model: list[DtshCommandOption]) -> Table:
+    def mk_option_hints_display(model: List[DtshCommandOption]) -> Table:
         """Layout option completion hints.
 
         Arguments:
         model -- an option list to display as hints
 
         Returns a rich table.
         """
         tab = DtshTui.mk_grid(2)
         for opt in model:
             tab.add_row(DtshTui.mk_txt(opt.usage), DtshTui.mk_txt_dim(opt.desc))
         return tab
 
     @staticmethod
-    def mk_node_hints_display(model: list[Node]) -> Table:
+    def mk_node_hints_display(model: List[Node]) -> Table:
         """Layout node completion hints.
 
         Arguments:
         model -- a node list to display as hints
 
         Returns a rich table.
         """
@@ -628,15 +622,15 @@
                 )
             else:
                 txt_desc = None
             tab.add_row(txt_name, txt_desc)
         return tab
 
     @staticmethod
-    def mk_property_hints_display(model: list[Property]) -> Table:
+    def mk_property_hints_display(model: List[Property]) -> Table:
         """Layout property completion hints.
 
         Arguments:
         model -- a property list to display as hints
 
         Returns a rich table.
         """
@@ -649,15 +643,15 @@
                 txt_desc = DtshTui.mk_txt_dim(
                     DtshTui.get_text_summary(prop.spec.description)
                 )
             tab.add_row(DtshTui.mk_txt(prop.name), txt_desc)
         return tab
 
     @staticmethod
-    def mk_binding_hints_display(model: list[Binding]) -> Table:
+    def mk_binding_hints_display(model: List[Binding]) -> Table:
         """Layout bindings completion hints.
 
         Arguments:
         model -- a binding list to display as hints
 
         Returns a rich table.
         """
@@ -791,15 +785,15 @@
                 'Default:',
                 DtshTui.mk_txt_dt_value(prop_spec.default, prop_spec.type)
             )
         return form
 
     @staticmethod
     def mk_node_tree_item(node: Node,
-                          width: list[int],
+                          width: List[int],
                           with_status: bool = False) -> Table:
         grid = DtshTui.mk_grid(3)
         for i, w in enumerate(width):
             if w > 0:
                 grid.columns[i].width = w
         grid.add_row(
             DtshTui.mk_txt_node_addr(node, with_status=with_status),
@@ -852,17 +846,17 @@
         DtshTui.txt_update_link_file(anchor, path)
 
         branch = tree.add(anchor)
         for inc_path in DtshTui._yaml_include_as_paths(yaml_py, shell):
             DtshTui.mk_branch_binding_path(inc_path, branch, shell)
 
     @staticmethod
-    def _yaml_include_as_paths(yaml_py, shell: Dtsh) -> list[str]:
+    def _yaml_include_as_paths(yaml_py, shell: Dtsh) -> List[str]:
         # Paths for the YAML files included with "include:" statements.
-        inc_paths = list[str]()
+        inc_paths: List[str] = []
         # See edtlib.Binding._merge_includes()
         yaml_inc = yaml_py.get('include')
         if isinstance(yaml_inc, str):
             path = shell.dt_binding_path(yaml_inc)
             if path:
                 inc_paths.append(path)
         elif isinstance(yaml_inc, list):
@@ -914,29 +908,29 @@
     def mk_grid(cols: int) -> Table:
         grid = Table.grid(padding=(0, 1))
         for _ in range(0, cols):
             grid.add_column()
         return grid
 
     @staticmethod
-    def mk_form(name_style: Style | None = None,
-                value_style: Style | None = None ) -> Table:
+    def mk_form(name_style: Optional[Style] = None,
+                value_style: Optional[Style] = None ) -> Table:
         form = DtshTui.mk_grid(2)
         if name_style:
             form.columns[0].style = name_style
         if value_style:
             form.columns[1].style = value_style
         return form
 
     @staticmethod
     def form_add(form: Table, name: str, val: str):
         form.add_row(name, val)
 
     @staticmethod
-    def mk_grid_simple_head(cols: list[str]) -> Table:
+    def mk_grid_simple_head(cols: List[str]) -> Table:
         grid = Table.grid(padding=(0, 1))
         grid.box = box.SIMPLE_HEAD
         grid.show_header = True
         grid.header_style = DtshTui.style(DtshTui.STYLE_DEFAULT)
         for header in cols:
             grid.add_column(header=header)
         return grid
@@ -951,27 +945,18 @@
 
     ############################################################################
     # Internals
     ############################################################################
 
     @staticmethod
     def _load_theme() -> Theme:
-        theme = None
-        theme_path = os.path.join(Dtsh.cfg_dir_path(), 'theme')
-        if os.path.isfile(theme_path):
-            try:
-                theme = Theme.from_file(open(theme_path))
-            except Exception:
-                pass
-        if not theme:
-            theme_path = os.path.join(os.path.dirname(__file__), 'theme')
-            theme = Theme.from_file(open(theme_path))
+        theme = DtshConfig.rich_read_theme()
         # load custom dtsh config
         config = configparser.ConfigParser()
-        config.read_file(open(theme_path))
+        config.read_file(open(DtshConfig.get_theme_path()))
         for name, value in config.items('dtsh'):
             if name == 'dtsh.prompt.wchar':
                 DtshTui.PROMPT_WCHAR = value
             elif name == 'dtsh.bullet.wchar':
                 DtshTui.WCHAR_BULLET = value
             elif name == 'dtsh.prompt.color':
                 DtshTui.PROMPT_COLOR = value
@@ -1002,28 +987,28 @@
     # List layout.
     _grid: Table
 
     # List item prefix, default to "    - ".
     _bullet: str
 
     def __init__(self,
-                 label: str | Text,
-                 bullet: str  | None = None) -> None:
+                 label: Union[str, Text],
+                 bullet: Optional[str] = None) -> None:
         """Initialize the widget.
 
         Arguments:
         label -- the list label (typically ends with ":"),
                  as a string or a rich Text
         bulet -- the bullet symbol, defaults to "-"
         """
         self._grid = Table.grid(padding=(0, 1))
         self._bullet = bullet or f"    {DtshTui.WCHAR_BULLET} "
         self._grid.add_row(label)
 
-    def add_item(self, item: str | Text) -> None:
+    def add_item(self, item: Union[str, Text]) -> None:
         """
         """
         r_item = DtshTui.mk_txt(self._bullet)
         if isinstance(item, Text):
             r_item = r_item.append_text(item)
         else:
             r_item.append(item)
@@ -1042,19 +1027,17 @@
     _grid: Table
 
     def __init__(self, path:str, with_title: bool = True) -> None:
         """Initialize YAML layout.
         """
         self._grid = DtshTui.mk_grid(1)
         if with_title:
-            r_name = DtshTui.mk_txt_link(
-                os.path.basename(path),
-                f"file:{path}",
-                style='dtsh.basename'
-            )
+            r_name = DtshTui.mk_txt(os.path.basename(path),
+                                    style='dtsh.basename')
+            DtshTui.txt_update_link_file(r_name, path)
             self._grid.add_row(r_name)
             self._grid.add_row()
         self._grid.add_row(DtshTui.mk_yaml(path))
 
     def as_renderable(self) -> RenderableType:
         """Implements DtshTuiWidget.as_renderable().
         """
@@ -1074,32 +1057,32 @@
     # Style for all field labels.
     _label_style: StyleType
 
     # Default style for field values.
     _value_style: StyleType
 
     def __init__(self,
-                 label_style: StyleType | None = None,
-                 value_style: StyleType | None = None) -> None:
+                 label_style: Optional[StyleType] = None,
+                 value_style: Optional[StyleType] = None) -> None:
         """
         Arguments:
         label_style --
         value_style --
         """
         self._label_style = label_style or DtshTui.style_default()
         self._value_style = value_style or DtshTui.style_default()
         self._form = Table.grid(padding=(0, 1))
         self._form.add_column()
         self._form.add_column()
 
     def add_field(self,
                   label: str,
-                  value: str | None,
+                  value: Optional[str],
                   default: str = "Unknown",
-                  style: StyleType | None = None) -> None:
+                  style: Optional[StyleType] = None) -> None:
         """Add a string field.
 
         Arguments:
         label -- the field label
         value -- the field value as a rich Text
         default -- value string representing None values
         style --
@@ -1110,15 +1093,15 @@
             r_value = Text(value, style=style or self._value_style)
         else:
             r_value = DtshTui.mk_txt_dim(default)
         self._form.add_row(r_label, r_value)
 
     def add_field_rich(self,
                        label: str,
-                       value: Text | None,
+                       value: Optional[Text],
                        default: str = "Unknown") -> None:
         """Add a rich field.
 
         Arguments:
         label -- the field label
         value -- the field value as a rich Text
         default -- value string representing None values
@@ -1343,18 +1326,18 @@
 class LsColumnNodeReg(LsNodeColumn):
     """The bus device information for the node.
 
     Format specifier is "r".
     """
 
     def __init__(self) -> None:
-        super().__init__("r", "Registers")
+        super().__init__("r", "Register")
 
     def mk_view(self, node: Node, shell: Dtsh) -> RenderableType:
-        return DtshTui.mk_txt_node_registers(node, with_status=True)
+        return DtshTui.mk_txt_node_register(node, with_status=True)
 
 
 class LsColumnNodeInterrupts(LsNodeColumn):
     """The interrupts generated by this node.
 
     Format specifier is "i".
     """
@@ -1390,33 +1373,31 @@
         | `r`       | The node 'reg' property                   | 2.3.6   |
         | `i`       | The interrupts generated by the node      | 2.4.1.1 |
     """
 
     _dtsh: Dtsh
 
     # The columns for the requested format.
-    _cols: list[LsNodeColumn]
+    _cols: List[LsNodeColumn]
 
     # The actual view.
     _grid: Table
 
-    DEFAULT_FMT = "naLAcd"
-
-    def __init__(self, shell: Dtsh, fmt: str | None = None) -> None:
+    def __init__(self, shell: Dtsh, longfmt: str) -> None:
         """Initialize a new node table.
 
         Arguments:
         shell -- the client DT shell
-        fmt -- the format string, defaults to "naLAcd".
+        longfmt -- the visible columns format string
 
         Raises DtshError when the format specifiers string is invalid.
         """
         self._dtsh = shell
-        self._cols = list[LsNodeColumn]()
-        for spec in (fmt or LsNodeTable.DEFAULT_FMT):
+        self._cols = []
+        for spec in longfmt:
             col = LsNodeTable._colspecs.get(spec)
             if not col:
                 raise DtshError(f"unknwon format specifier {spec}")
             self._cols.append(col)
         self._grid = DtshTui.mk_grid_simple_head(
             [col.header for col in self._cols]
         )
@@ -1429,15 +1410,15 @@
 
     def as_view(self) -> Table:
         """Returns the view for the node table.
         """
         return self._grid
 
     # Available columns.
-    _colspecs: dict[str, LsNodeColumn] = {
+    _colspecs: Dict[str, LsNodeColumn] = {
         col.spec: col for col in [
             LsColumnNodeName(),
             LsColumnNodeAddr(),
             LsColumnNodeNick(),
             LsColumnNodeDesc(),
             LsColumnNodePath(),
             LsColumnNodeLabel(),
@@ -1575,15 +1556,15 @@
                        defaults to 8
         expand -- if True, axpand the layout to fit the available horizontal
                   space, defaults to False
         """
         super().__init__(expand=expand)
         self._indent_size = indent_size
 
-    def add_entry(self, name: str, content: RenderableType | None) -> None:
+    def add_entry(self, name: str, content: Optional[RenderableType]) -> None:
         """Add a named entry to the memo.
 
         Arguments:
         name -- the entry's label (will be uppercased)
         content -- the rich content to add
         is_last -- if False, an empty row is appended bellow the content row
         """
@@ -1671,44 +1652,53 @@
 
     This view handles both the default and "rich output" cases.
     """
 
     # View rich table layout.
     _view: Table
 
+    # Default columns.
+    DEFAULT_LONGFMT = 'naLAcd'
+
     def __init__(self,
-                 node_map: dict[str, list[Node]],
+                 node_map: Dict[str, List[Node]],
                  shell: Dtsh,
                  with_no_content: bool = False,
-                 with_rich_fmt: bool = False,
-                 fmt: str | None = None) -> None:
+                 with_longfmt: bool = False,
+                 longfmt: Optional[str] = None) -> None:
         """Initialize the view.
 
         Arguments:
         node_map -- maps node paths to contents (aka child nodes)
         shell -- the context shell
         with_no_content -- if True, will show nodes, not their content
-        with_rich_fmt -- if True, will produce "rich output"
+        with_longfmt -- if True, use long (aka rich) listing format
+        longfmt -- specifies visible columns, implies long format if not None
         """
-        if with_rich_fmt:
-            self._init_rich_view(node_map, shell, with_no_content, fmt)
+        if with_longfmt and not longfmt:
+            # '-l' defaults columns.
+            longfmt = DtNodeListView.DEFAULT_LONGFMT
+        
+        if longfmt:
+            # '-f' implies '-l'.
+            self._init_view_longfmt(node_map, shell, with_no_content, longfmt)
         else:
-            self._init_default_view(node_map, with_no_content)
+            self._init_view_default(node_map, with_no_content)
 
     def show(self, vt: DtshVt, with_pager: bool = False) -> None:
         """Implements DtshTView.show().
         """
         if with_pager:
             vt.pager_enter()
         vt.write(self._view)
         if with_pager:
             vt.pager_exit()
 
-    def _init_default_view(self,
-                           node_map: dict[str, list[Node]],
+    def _init_view_default(self,
+                           node_map: Dict[str, List[Node]],
                            with_no_content: bool) -> None:
         self._view = DtshTui.mk_grid(1)
         N = len(node_map)
         n = 0
         for path, nodes in node_map.items():
             if with_no_content:
                 self._view.add_row(f'{path}')
@@ -1717,33 +1707,33 @@
                     self._view.add_row(f'{path}:')
                 for node in nodes:
                     self._view.add_row(f'{node.path}')
                 if n < (N - 1):
                     self._view.add_row(None)
                 n += 1
 
-    def _init_rich_view(self,
-                        node_map: dict[str, list[Node]],
-                        shell: Dtsh,
-                        with_no_content: bool,
-                        fmt: str | None) -> None:
+    def _init_view_longfmt(self,
+                           node_map: Dict[str, List[Node]],
+                           shell: Dtsh,
+                           with_no_content: bool,
+                           longfmt: str) -> None:
         if with_no_content:
-            ls_table = LsNodeTable(shell, fmt)
+            ls_table = LsNodeTable(shell, longfmt)
             for path, _ in node_map.items():
                 node = shell.path2node(path)
                 ls_table.add_node_row(node)
             self._view = ls_table.as_view()
         else:
             self._view = DtshTui.mk_grid(1)
             N = len(node_map)
             n = 0
             for path, content in node_map.items():
                 self._view.add_row(Text(f"{path}:", DtshTui.style('bold')))
                 if content:
-                    ls_table = LsNodeTable(shell, fmt)
+                    ls_table = LsNodeTable(shell, longfmt)
                     for node in content:
                         ls_table.add_node_row(node)
                     self._view.add_row(ls_table.as_view())
                 if n < (N - 1):
                     self._view.add_row(None)
                 n += 1
 
@@ -1806,15 +1796,15 @@
             if (self._level == 0) or (self._depth < self._level):
                 if node.status != 'disabled':
                     self._follow_node_branch(node, branch)
 
         # Decrease depth on return.
         self._depth -= 1
 
-    def _get_branch_width(self, root: Node) -> list[int]:
+    def _get_branch_width(self, root: Node) -> List[int]:
         width_addr = 0
         width_nick = 0
         for _, node in root.children.items():
             nick = DtshTui.get_node_nick(node)
             w = len(nick)
             if w > width_nick:
                 width_nick = w
```

### Comparing `dtsh-0.1.0a4/src/dtsh.egg-info/PKG-INFO` & `dtsh-0.1.0a6/src/dtsh.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: dtsh
-Version: 0.1.0a4
+Version: 0.1.0a6
 Summary: Shell-like interface with Zephyr devicetree and bindings
 Home-page: https://github.com/dottspina/dtsh
 Author: Chris Duf
 Author-email: chris@openmarl.org
 License: Apache License version 2.0
 Project-URL: Bug Reports, https://github.com/dottspina/dtsh/issues
 Project-URL: Source, https://github.com/dottspina/dtsh
 Keywords: devicetree,zephyr,dts,embedded
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
+Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: dist
 License-File: LICENSE
 
 ====
 dtsh
 ====
```


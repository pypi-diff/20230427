# Comparing `tmp/pyconch-0.0.3.tar.gz` & `tmp/pyconch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyconch-0.0.3.tar", last modified: Sat Jul 25 13:21:57 2020, max compression
+gzip compressed data, was "pyconch-0.0.4.tar", last modified: Thu Apr 27 08:17:52 2023, max compression
```

## Comparing `pyconch-0.0.3.tar` & `pyconch-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-07-25 13:21:57.147544 pyconch-0.0.3/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2020-06-03 13:38:19.000000 pyconch-0.0.3/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1396 2020-07-25 13:21:57.147544 pyconch-0.0.3/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      309 2020-07-25 13:21:44.000000 pyconch-0.0.3/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-07-25 13:21:57.146544 pyconch-0.0.3/pyconch/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-06-03 13:33:54.000000 pyconch-0.0.3/pyconch/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      253 2020-07-25 13:21:03.000000 pyconch-0.0.3/pyconch/configs.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-07-25 13:21:57.147544 pyconch-0.0.3/pyconch/endpoints/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-06-03 13:34:16.000000 pyconch-0.0.3/pyconch/endpoints/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      623 2020-07-25 13:21:26.000000 pyconch-0.0.3/pyconch/endpoints/group_default.py
--rw-r--r--   0 mark      (1000) mark      (1000)      542 2020-07-25 13:21:20.000000 pyconch-0.0.3/pyconch/endpoints/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)       83 2020-07-25 13:21:44.000000 pyconch-0.0.3/pyconch/version.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-07-25 13:21:57.147544 pyconch-0.0.3/pyconch.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1396 2020-07-25 13:21:57.000000 pyconch-0.0.3/pyconch.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      378 2020-07-25 13:21:57.000000 pyconch-0.0.3/pyconch.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2020-07-25 13:21:57.000000 pyconch-0.0.3/pyconch.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       57 2020-07-25 13:21:57.000000 pyconch-0.0.3/pyconch.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       18 2020-07-25 13:21:57.000000 pyconch-0.0.3/pyconch.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        8 2020-07-25 13:21:57.000000 pyconch-0.0.3/pyconch.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2020-07-25 13:21:57.147544 pyconch-0.0.3/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1604 2020-07-25 13:21:44.000000 pyconch-0.0.3/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:17:52.371605 pyconch-0.0.4/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-27 08:17:38.000000 pyconch-0.0.4/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1327 2023-04-27 08:17:52.371605 pyconch-0.0.4/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      384 2023-04-27 08:17:38.000000 pyconch-0.0.4/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:17:52.371605 pyconch-0.0.4/pyconch/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-06-03 13:33:54.000000 pyconch-0.0.4/pyconch/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      253 2020-07-25 13:21:03.000000 pyconch-0.0.4/pyconch/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      405 2023-04-27 08:17:23.000000 pyconch-0.0.4/pyconch/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      187 2023-04-27 08:17:38.000000 pyconch-0.0.4/pyconch/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:17:52.371605 pyconch-0.0.4/pyconch.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1327 2023-04-27 08:17:52.000000 pyconch-0.0.4/pyconch.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      298 2023-04-27 08:17:52.000000 pyconch-0.0.4/pyconch.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-27 08:17:52.000000 pyconch-0.0.4/pyconch.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       56 2023-04-27 08:17:52.000000 pyconch-0.0.4/pyconch.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       18 2023-04-27 08:17:52.000000 pyconch-0.0.4/pyconch.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        8 2023-04-27 08:17:52.000000 pyconch-0.0.4/pyconch.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-27 08:17:52.372605 pyconch-0.0.4/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1511 2023-04-27 08:17:38.000000 pyconch-0.0.4/setup.py
```

### Comparing `pyconch-0.0.3/setup.py` & `pyconch-0.0.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,56 +5,51 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyconch",
-    version="0.0.3",
+    version="0.0.4",
     packages=[
-        'pyconch',
-        'pyconch.endpoints',
+        "pyconch",
     ],
     # from here all is optional
     description="Pyconch is a wrapper for a shell in python",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
-        'make',
-        'scons',
+        "shell",
+        "bash",
+        "tcsh",
     ],
     url="https://veltzer.github.io/pyconch",
     download_url="https://github.com/veltzer/pyconch",
     license="MIT",
     platforms=[
-        'python3',
+        "python3",
     ],
     install_requires=[
-        'pytconf',
-        'pylogconf',
+        "pytconf",
+        "pylogconf",
     ],
-    extras_require={
-    },
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Environment :: Console',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Topic :: Utilities',
-        'License :: OSI Approved :: MIT License',
-    ],
-    data_files=[
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Utilities",
+        "License :: OSI Approved :: MIT License",
     ],
     entry_points={"console_scripts": [
-        'pyconch=pyconch.endpoints.main:main',
+        "pyconch=pyconch.endpoints.main:main",
     ]},
-    python_requires=">=3.6",
 )
```


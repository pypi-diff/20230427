# Comparing `tmp/htools-7.5.0.tar.gz` & `tmp/htools-7.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/htools-7.5.0.tar", last modified: Thu Mar  9 03:24:41 2023, max compression
+gzip compressed data, was "dist/htools-7.6.0.tar", last modified: Thu Apr 27 04:45:56 2023, max compression
```

## Comparing `htools-7.5.0.tar` & `htools-7.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-03-09 03:24:41.000000 htools-7.5.0/
--rw-r--r--   0 hmamin     (501) staff       (20)     1070 2019-10-25 22:10:07.000000 htools-7.5.0/LICENSE.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       73 2020-11-21 05:39:35.000000 htools-7.5.0/MANIFEST.in
--rw-r--r--   0 hmamin     (501) staff       (20)      228 2023-03-09 03:24:41.000000 htools-7.5.0/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)      118 2020-12-27 20:57:55.000000 htools-7.5.0/README.md
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-03-09 03:24:41.000000 htools-7.5.0/htools/
--rw-r--r--   0 hmamin     (501) staff       (20)      136 2023-03-09 03:24:21.000000 htools-7.5.0/htools/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1776 2023-03-01 03:21:56.000000 htools-7.5.0/htools/autodebug.py
--rw-r--r--   0 hmamin     (501) staff       (20)    24235 2022-12-10 03:26:09.000000 htools-7.5.0/htools/cli.py
--rw-r--r--   0 hmamin     (501) staff       (20)     2875 2021-03-27 04:17:11.000000 htools-7.5.0/htools/config.py
--rw-r--r--   0 hmamin     (501) staff       (20)    58779 2023-03-09 02:53:28.000000 htools-7.5.0/htools/core.py
--rw-r--r--   0 hmamin     (501) staff       (20)    10220 2021-03-31 22:50:53.000000 htools-7.5.0/htools/magics.py
--rw-r--r--   0 hmamin     (501) staff       (20)   111802 2023-02-20 20:22:33.000000 htools-7.5.0/htools/meta.py
--rw-r--r--   0 hmamin     (501) staff       (20)    23969 2022-07-03 20:07:39.000000 htools-7.5.0/htools/pd_tools.py
--rw-r--r--   0 hmamin     (501) staff       (20)    43594 2022-06-19 23:36:58.000000 htools-7.5.0/htools/structures.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-03-09 03:24:41.000000 htools-7.5.0/htools.egg-info/
--rw-r--r--   0 hmamin     (501) staff       (20)      228 2023-03-09 03:24:40.000000 htools-7.5.0/htools.egg-info/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)      437 2023-03-09 03:24:41.000000 htools-7.5.0/htools.egg-info/SOURCES.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-03-09 03:24:40.000000 htools-7.5.0/htools.egg-info/dependency_links.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       42 2023-03-09 03:24:40.000000 htools-7.5.0/htools.egg-info/entry_points.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        1 2020-01-08 05:14:40.000000 htools-7.5.0/htools.egg-info/not-zip-safe
--rw-r--r--   0 hmamin     (501) staff       (20)      172 2023-03-09 03:24:41.000000 htools-7.5.0/htools.egg-info/requires.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        7 2023-03-09 03:24:41.000000 htools-7.5.0/htools.egg-info/top_level.txt
--rw-r--r--   0 hmamin     (501) staff       (20)      194 2022-07-03 20:07:46.000000 htools-7.5.0/requirements.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       79 2023-03-09 03:24:41.000000 htools-7.5.0/setup.cfg
--rw-r--r--   0 hmamin     (501) staff       (20)      954 2021-08-14 03:10:29.000000 htools-7.5.0/setup.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-04-27 04:45:56.000000 htools-7.6.0/
+-rw-r--r--   0 hmamin     (501) staff       (20)     1070 2019-10-25 22:10:07.000000 htools-7.6.0/LICENSE.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       73 2020-11-21 05:39:35.000000 htools-7.6.0/MANIFEST.in
+-rw-r--r--   0 hmamin     (501) staff       (20)      228 2023-04-27 04:45:56.000000 htools-7.6.0/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)      118 2020-12-27 20:57:55.000000 htools-7.6.0/README.md
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-04-27 04:45:56.000000 htools-7.6.0/htools/
+-rw-r--r--   0 hmamin     (501) staff       (20)      136 2023-04-27 04:45:12.000000 htools-7.6.0/htools/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1776 2023-03-01 03:21:56.000000 htools-7.6.0/htools/autodebug.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    24235 2022-12-10 03:26:09.000000 htools-7.6.0/htools/cli.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     2875 2021-03-27 04:17:11.000000 htools-7.6.0/htools/config.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    59137 2023-04-27 04:42:59.000000 htools-7.6.0/htools/core.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    10220 2021-03-31 22:50:53.000000 htools-7.6.0/htools/magics.py
+-rw-r--r--   0 hmamin     (501) staff       (20)   111802 2023-02-20 20:22:33.000000 htools-7.6.0/htools/meta.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    23969 2022-07-03 20:07:39.000000 htools-7.6.0/htools/pd_tools.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    43594 2022-06-19 23:36:58.000000 htools-7.6.0/htools/structures.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-04-27 04:45:56.000000 htools-7.6.0/htools.egg-info/
+-rw-r--r--   0 hmamin     (501) staff       (20)      228 2023-04-27 04:45:54.000000 htools-7.6.0/htools.egg-info/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)      437 2023-04-27 04:45:55.000000 htools-7.6.0/htools.egg-info/SOURCES.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-04-27 04:45:54.000000 htools-7.6.0/htools.egg-info/dependency_links.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       42 2023-04-27 04:45:55.000000 htools-7.6.0/htools.egg-info/entry_points.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        1 2020-01-08 05:14:40.000000 htools-7.6.0/htools.egg-info/not-zip-safe
+-rw-r--r--   0 hmamin     (501) staff       (20)      172 2023-04-27 04:45:55.000000 htools-7.6.0/htools.egg-info/requires.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        7 2023-04-27 04:45:55.000000 htools-7.6.0/htools.egg-info/top_level.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)      194 2022-07-03 20:07:46.000000 htools-7.6.0/requirements.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       79 2023-04-27 04:45:56.000000 htools-7.6.0/setup.cfg
+-rw-r--r--   0 hmamin     (501) staff       (20)     1084 2023-04-18 05:22:07.000000 htools-7.6.0/setup.py
```

### Comparing `htools-7.5.0/LICENSE.txt` & `htools-7.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `htools-7.5.0/htools/autodebug.py` & `htools-7.6.0/htools/autodebug.py`

 * *Files identical despite different names*

### Comparing `htools-7.5.0/htools/cli.py` & `htools-7.6.0/htools/cli.py`

 * *Files identical despite different names*

### Comparing `htools-7.5.0/htools/config.py` & `htools-7.6.0/htools/config.py`

 * *Files identical despite different names*

### Comparing `htools-7.5.0/htools/core.py` & `htools-7.6.0/htools/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1740,28 +1740,34 @@
     -------
     str: `length` characters long.
     """
     text = ''.join(choices(valid, k=length))
     return text.lower() if lower else text
 
 
-def is_ipy_name(name):
+def is_ipy_name(name, check_in_out=False):
     """Check if a variable name looks like an ipython output cell, e.g.
     "_49", "_", or "__".
     
     Parameters
     ----------
     name: str
+    check_in_out: bool
+        If True, check if name is in ['In', 'Out'] (i.e. we consider those to
+        be ipy names as well). If False (the default), skip this check.
 
     Returns
     -------
     bool: True if it looks like an ipython output cell name, False otherwise.
     """
     stripped = name.lstrip('_')
-    return name[0] == '_' and (stripped.isdigit() or not stripped)
+    # First check if it fits the standard leading underscore format.
+    is_under = name[0] == '_' and (stripped.isdigit() or not stripped)
+    is_in_out = check_in_out and stripped in ('In', 'Out')
+    return is_under or is_in_out
 
 
 def varname(x, *skip, skip_ipy_names=True, strict=True):
     """Try to guess name of a variable.
 
     Parameters
     ----------
```

### Comparing `htools-7.5.0/htools/magics.py` & `htools-7.6.0/htools/magics.py`

 * *Files identical despite different names*

### Comparing `htools-7.5.0/htools/meta.py` & `htools-7.6.0/htools/meta.py`

 * *Files identical despite different names*

### Comparing `htools-7.5.0/htools/pd_tools.py` & `htools-7.6.0/htools/pd_tools.py`

 * *Files identical despite different names*

### Comparing `htools-7.5.0/htools/structures.py` & `htools-7.6.0/htools/structures.py`

 * *Files identical despite different names*

### Comparing `htools-7.5.0/setup.py` & `htools-7.6.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,12 +22,14 @@
     description='Harrison\'s custom functions.',
     packages=find_packages(include=['htools']),
     author='Harrison Mamin',
     zip_safe=False,
     install_requires=requirements(),
     # If installing speedup causes gcc error in docker image, try
     # adding `apt install build-essentials`.
+    # TODO: maybe move this dep out of extras. Fuzzywuzzy gets imported by
+    # meta module so it's not really optional anymore.
     extras_require={'fuzzy': ['fuzzywuzzy'],
                     'speedup': ['fuzzywuzzy[speedup]']},
     entry_points={'console_scripts': ['htools=htools.cli:cli']}
 )
```


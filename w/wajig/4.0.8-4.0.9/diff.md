# Comparing `tmp/wajig-4.0.8.tar.gz` & `tmp/wajig-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wajig-4.0.8.tar", last modified: Wed Feb  1 21:53:50 2023, max compression
+gzip compressed data, was "wajig-4.0.9.tar", last modified: Thu Feb  2 00:59:38 2023, max compression
```

## Comparing `wajig-4.0.8.tar` & `wajig-4.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-01 21:53:50.324536 wajig-4.0.8/
--rw-r-----   0 gjw       (1000) gjw       (1000)    35149 2020-07-07 02:15:20.000000 wajig-4.0.8/LICENSE
--rw-r-----   0 gjw       (1000) gjw       (1000)       82 2020-07-25 22:22:49.000000 wajig-4.0.8/MANIFEST.in
--rw-r-----   0 gjw       (1000) gjw       (1000)    32951 2023-02-01 21:53:50.324536 wajig-4.0.8/PKG-INFO
--rw-r-----   0 gjw       (1000) gjw       (1000)    32069 2021-10-29 05:34:34.000000 wajig-4.0.8/README.rst
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-01 21:53:50.320536 wajig-4.0.8/docs/
--rw-r-----   0 gjw       (1000) gjw       (1000)    32372 2020-08-02 08:52:34.000000 wajig-4.0.8/docs/README.md
--rw-r-----   0 gjw       (1000) gjw       (1000)       50 2023-02-01 21:53:50.324536 wajig-4.0.8/setup.cfg
--rw-r-----   0 gjw       (1000) gjw       (1000)     2491 2023-02-01 21:53:49.000000 wajig-4.0.8/setup.py
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-01 21:53:50.320536 wajig-4.0.8/wajig/
--rwxr-x---   0 gjw       (1000) gjw       (1000)    38335 2022-08-16 19:43:34.000000 wajig-4.0.8/wajig/__init__.py
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-01 21:53:50.324536 wajig-4.0.8/wajig/bash_completion.d/
--rw-r-----   0 gjw       (1000) gjw       (1000)     4972 2022-09-09 01:07:27.000000 wajig-4.0.8/wajig/bash_completion.d/wajig.bash
--rw-r-----   0 gjw       (1000) gjw       (1000)    51081 2023-02-01 21:48:21.000000 wajig-4.0.8/wajig/commands.py
--rw-r-----   0 gjw       (1000) gjw       (1000)      289 2023-02-01 21:53:49.000000 wajig-4.0.8/wajig/constants.py
--rw-r-----   0 gjw       (1000) gjw       (1000)     1586 2020-06-11 00:25:18.000000 wajig-4.0.8/wajig/debfile-deps.py
--rw-r-----   0 gjw       (1000) gjw       (1000)     1224 2020-07-26 06:53:41.000000 wajig-4.0.8/wajig/debfile.py
--rw-r-----   0 gjw       (1000) gjw       (1000)     4429 2021-10-24 21:34:57.000000 wajig-4.0.8/wajig/perform.py
--rwxr-x---   0 gjw       (1000) gjw       (1000)     2990 2022-11-06 19:20:40.000000 wajig-4.0.8/wajig/shell.py
--rw-r-----   0 gjw       (1000) gjw       (1000)    22441 2022-11-06 19:20:40.000000 wajig-4.0.8/wajig/util.py
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-01 21:53:50.324536 wajig-4.0.8/wajig.egg-info/
--rw-r-----   0 gjw       (1000) gjw       (1000)    32951 2023-02-01 21:53:50.000000 wajig-4.0.8/wajig.egg-info/PKG-INFO
--rw-r-----   0 gjw       (1000) gjw       (1000)      415 2023-02-01 21:53:50.000000 wajig-4.0.8/wajig.egg-info/SOURCES.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)        1 2023-02-01 21:53:50.000000 wajig-4.0.8/wajig.egg-info/dependency_links.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)       38 2023-02-01 21:53:50.000000 wajig-4.0.8/wajig.egg-info/entry_points.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)       36 2023-02-01 21:53:50.000000 wajig-4.0.8/wajig.egg-info/requires.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)        6 2023-02-01 21:53:50.000000 wajig-4.0.8/wajig.egg-info/top_level.txt
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-02 00:59:38.972858 wajig-4.0.9/
+-rw-r-----   0 gjw       (1000) gjw       (1000)    35149 2020-07-07 02:15:20.000000 wajig-4.0.9/LICENSE
+-rw-r-----   0 gjw       (1000) gjw       (1000)       82 2020-07-25 22:22:49.000000 wajig-4.0.9/MANIFEST.in
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32951 2023-02-02 00:59:38.972858 wajig-4.0.9/PKG-INFO
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32069 2021-10-29 05:34:34.000000 wajig-4.0.9/README.rst
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-02 00:59:38.968858 wajig-4.0.9/docs/
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32372 2020-08-02 08:52:34.000000 wajig-4.0.9/docs/README.md
+-rw-r-----   0 gjw       (1000) gjw       (1000)       50 2023-02-02 00:59:38.972858 wajig-4.0.9/setup.cfg
+-rw-r-----   0 gjw       (1000) gjw       (1000)     2491 2023-02-02 00:59:38.000000 wajig-4.0.9/setup.py
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-02 00:59:38.968858 wajig-4.0.9/wajig/
+-rwxr-x---   0 gjw       (1000) gjw       (1000)    38335 2022-08-16 19:43:34.000000 wajig-4.0.9/wajig/__init__.py
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-02 00:59:38.972858 wajig-4.0.9/wajig/bash_completion.d/
+-rw-r-----   0 gjw       (1000) gjw       (1000)     4972 2022-09-09 01:07:27.000000 wajig-4.0.9/wajig/bash_completion.d/wajig.bash
+-rw-r-----   0 gjw       (1000) gjw       (1000)    51078 2023-02-02 00:58:04.000000 wajig-4.0.9/wajig/commands.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)      289 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig/constants.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)     1586 2020-06-11 00:25:18.000000 wajig-4.0.9/wajig/debfile-deps.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)     1224 2020-07-26 06:53:41.000000 wajig-4.0.9/wajig/debfile.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)     4429 2021-10-24 21:34:57.000000 wajig-4.0.9/wajig/perform.py
+-rwxr-x---   0 gjw       (1000) gjw       (1000)     2990 2022-11-06 19:20:40.000000 wajig-4.0.9/wajig/shell.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)    22441 2022-11-06 19:20:40.000000 wajig-4.0.9/wajig/util.py
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-02 00:59:38.972858 wajig-4.0.9/wajig.egg-info/
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32951 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/PKG-INFO
+-rw-r-----   0 gjw       (1000) gjw       (1000)      415 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/SOURCES.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)        1 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/dependency_links.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)       38 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/entry_points.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)       36 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/requires.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)        6 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/top_level.txt
```

### Comparing `wajig-4.0.8/LICENSE` & `wajig-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wajig-4.0.8/PKG-INFO` & `wajig-4.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wajig
-Version: 4.0.8
+Version: 4.0.9
 Summary: Ubunut admin managemetn tool
 Home-page: https://wajig.togaware.com
 Author: Graham Williams
 Author-email: wajig@togaware.com
 License: UNKNOWN
 Keywords: debian ubuntu admin
 Platform: UNKNOWN
```

### Comparing `wajig-4.0.8/README.rst` & `wajig-4.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `wajig-4.0.8/docs/README.md` & `wajig-4.0.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `wajig-4.0.8/setup.py` & `wajig-4.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # Get the long description from the README file.
 
 with open(path.join(here, 'docs/README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='wajig',
-    version='4.0.8',  # DO NOT MODIFY. Managed from Makefile.
+    version='4.0.9',  # DO NOT MODIFY. Managed from Makefile.
     description='Ubunut admin managemetn tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Graham Williams',
     author_email='wajig@togaware.com',
     url='https://wajig.togaware.com',
     classifiers=[
```

### Comparing `wajig-4.0.8/wajig/__init__.py` & `wajig-4.0.9/wajig/__init__.py`

 * *Files identical despite different names*

### Comparing `wajig-4.0.8/wajig/bash_completion.d/wajig.bash` & `wajig-4.0.9/wajig/bash_completion.d/wajig.bash`

 * *Files identical despite different names*

### Comparing `wajig-4.0.8/wajig/commands.py` & `wajig-4.0.9/wajig/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -788,15 +788,15 @@
         command = f"cat /dev/urandom | tr -cd '[:graph:]' | head -c {length}; echo"
         perform.execute(command, teach=args.teach, noop=args.noop)
         if not args.noop:
             for i in range(1, int(number)):
                 perform.execute(command)
     else:
         util.requires_package("pwgen")
-        command = f"pwgen -s -y {length} {number} | tr ' ' '\n'"
+        command = f"pwgen -s {length} {number} | tr ' ' '\n'"
         perform.execute(command, teach=args.teach, noop=args.noop)
 
 # POLICY
     
 def policy(args):
     """From preferences file show priorities/policy (available)"""
     perform.execute("apt-cache policy " + " ".join(args.packages), teach=args.teach, noop=args.noop)
```

### Comparing `wajig-4.0.8/wajig/debfile-deps.py` & `wajig-4.0.9/wajig/debfile-deps.py`

 * *Files identical despite different names*

### Comparing `wajig-4.0.8/wajig/debfile.py` & `wajig-4.0.9/wajig/debfile.py`

 * *Files identical despite different names*

### Comparing `wajig-4.0.8/wajig/perform.py` & `wajig-4.0.9/wajig/perform.py`

 * *Files identical despite different names*

### Comparing `wajig-4.0.8/wajig/shell.py` & `wajig-4.0.9/wajig/shell.py`

 * *Files identical despite different names*

### Comparing `wajig-4.0.8/wajig/util.py` & `wajig-4.0.9/wajig/util.py`

 * *Files identical despite different names*

### Comparing `wajig-4.0.8/wajig.egg-info/PKG-INFO` & `wajig-4.0.9/wajig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wajig
-Version: 4.0.8
+Version: 4.0.9
 Summary: Ubunut admin managemetn tool
 Home-page: https://wajig.togaware.com
 Author: Graham Williams
 Author-email: wajig@togaware.com
 License: UNKNOWN
 Keywords: debian ubuntu admin
 Platform: UNKNOWN
```


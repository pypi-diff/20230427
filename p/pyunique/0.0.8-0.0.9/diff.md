# Comparing `tmp/pyunique-0.0.8.tar.gz` & `tmp/pyunique-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyunique-0.0.8.tar", last modified: Wed Aug 12 07:55:35 2020, max compression
+gzip compressed data, was "pyunique-0.0.9.tar", last modified: Sun May  1 04:12:10 2022, max compression
```

## Comparing `pyunique-0.0.8.tar` & `pyunique-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-08-12 07:55:35.826406 pyunique-0.0.8/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2020-05-24 13:27:20.000000 pyunique-0.0.8/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1410 2020-08-12 07:55:35.826406 pyunique-0.0.8/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      315 2020-08-12 07:55:15.000000 pyunique-0.0.8/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-08-12 07:55:35.825406 pyunique-0.0.8/pyunique/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2020-08-12 01:46:25.000000 pyunique-0.0.8/pyunique/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2743 2020-08-12 07:49:04.000000 pyunique-0.0.8/pyunique/archive.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1061 2020-08-12 07:46:38.000000 pyunique-0.0.8/pyunique/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      409 2020-08-12 02:07:58.000000 pyunique-0.0.8/pyunique/digest.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-08-12 07:55:35.826406 pyunique-0.0.8/pyunique/endpoints/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-21 06:45:14.000000 pyunique-0.0.8/pyunique/endpoints/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3731 2020-08-12 07:50:39.000000 pyunique-0.0.8/pyunique/endpoints/group_default.py
--rw-r--r--   0 mark      (1000) mark      (1000)      546 2020-07-25 13:00:45.000000 pyunique-0.0.8/pyunique/endpoints/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      280 2020-08-12 02:19:11.000000 pyunique-0.0.8/pyunique/utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)       83 2020-08-12 07:55:15.000000 pyunique-0.0.8/pyunique/version.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-08-12 07:55:35.825406 pyunique-0.0.8/pyunique.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1410 2020-08-12 07:55:35.000000 pyunique-0.0.8/pyunique.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      447 2020-08-12 07:55:35.000000 pyunique-0.0.8/pyunique.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2020-08-12 07:55:35.000000 pyunique-0.0.8/pyunique.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       59 2020-08-12 07:55:35.000000 pyunique-0.0.8/pyunique.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       28 2020-08-12 07:55:35.000000 pyunique-0.0.8/pyunique.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2020-08-12 07:55:35.000000 pyunique-0.0.8/pyunique.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2020-08-12 07:55:35.826406 pyunique-0.0.8/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1659 2020-08-12 07:55:15.000000 pyunique-0.0.8/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-05-01 04:12:10.603814 pyunique-0.0.9/
+-rw-r--r--   0 mark      (1000) mark      (1000)       25 2020-05-24 13:27:20.000000 pyunique-0.0.9/MANIFEST.in
+-rw-r--r--   0 mark      (1000) mark      (1000)     1310 2022-05-01 04:12:10.604813 pyunique-0.0.9/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      315 2022-05-01 04:11:56.000000 pyunique-0.0.9/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-05-01 04:12:10.603814 pyunique-0.0.9/pyunique/
+-rw-r--r--   0 mark      (1000) mark      (1000)       25 2020-08-12 01:46:25.000000 pyunique-0.0.9/pyunique/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2743 2020-08-12 07:49:04.000000 pyunique-0.0.9/pyunique/archive.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1061 2020-10-03 02:26:40.000000 pyunique-0.0.9/pyunique/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      409 2020-08-12 02:07:58.000000 pyunique-0.0.9/pyunique/digest.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3453 2020-11-15 05:59:04.000000 pyunique-0.0.9/pyunique/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      182 2022-05-01 04:11:56.000000 pyunique-0.0.9/pyunique/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      282 2020-10-03 02:26:57.000000 pyunique-0.0.9/pyunique/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-05-01 04:12:10.603814 pyunique-0.0.9/pyunique.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1310 2022-05-01 04:12:10.000000 pyunique-0.0.9/pyunique.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      369 2022-05-01 04:12:10.000000 pyunique-0.0.9/pyunique.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-05-01 04:12:10.000000 pyunique-0.0.9/pyunique.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       49 2022-05-01 04:12:10.000000 pyunique-0.0.9/pyunique.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       28 2022-05-01 04:12:10.000000 pyunique-0.0.9/pyunique.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2022-05-01 04:12:10.000000 pyunique-0.0.9/pyunique.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2022-05-01 04:12:10.604813 pyunique-0.0.9/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1521 2022-05-01 04:11:56.000000 pyunique-0.0.9/setup.py
```

### Comparing `pyunique-0.0.8/PKG-INFO` & `pyunique-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunique
-Version: 0.0.8
+Version: 0.0.9
 Summary: help you get rid of duplicate files
 Home-page: https://veltzer.github.io/pyunique
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
@@ -19,26 +19,24 @@
         
         .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
         
         project website: https://veltzer.github.io/pyunique
         
         author: Mark Veltzer
         
-        version: 0.0.8
+        version: 0.0.9
         
         
         
 Keywords: duplicates,remove,hash
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `pyunique-0.0.8/pyunique/archive.py` & `pyunique-0.0.9/pyunique/archive.py`

 * *Files identical despite different names*

### Comparing `pyunique-0.0.8/pyunique/configs.py` & `pyunique-0.0.9/pyunique/configs.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 All configurations for pyunique
 """
-from pytconf import Config, ParamCreator
 import hashlib
+from pytconf import Config, ParamCreator
 
 
 class ConfigScan(Config):
     """
     Parameters that control the scanning phase
     """
     folder = ParamCreator.create_existing_folder(
```

### Comparing `pyunique-0.0.8/pyunique/endpoints/group_default.py` & `pyunique-0.0.9/pyunique/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,61 @@
 """
-The default group of operations that pyunique has
+main entry point to the program
 """
 import os
 
+import pylogconf.core
 import tqdm
-from pytconf import register_endpoint, register_function_group
+from pytconf import register_main, config_arg_parse_and_launch, register_endpoint
 
-import pyunique.version
 from pyunique.archive import get_archive
 from pyunique.configs import ConfigScan, ConfigAlgo, ConfigLMDB
 from pyunique.digest import digest_file_bytes
-from pyunique.utils import get_logger, get_number_of_files
-
-GROUP_NAME_DEFAULT = "default"
-GROUP_DESCRIPTION_DEFAULT = "all pyunique commands"
-
-
-def register_group_default():
-    """
-    register the name and description of this group
-    """
-    register_function_group(
-        function_group_name=GROUP_NAME_DEFAULT,
-        function_group_description=GROUP_DESCRIPTION_DEFAULT,
-    )
+from pyunique.static import VERSION_STR
 
-
-@register_endpoint(
-    group=GROUP_NAME_DEFAULT,
-)
-def version() -> None:
-    """
-    Print version
-    """
-    print(pyunique.version.VERSION_STR)
+from pyunique.utils import get_logger, get_number_of_files
 
 
 @register_endpoint(
-    group=GROUP_NAME_DEFAULT,
+    description="Scan a folder and register it's checksums",
     configs=[
         ConfigScan,
         ConfigAlgo,
         ConfigLMDB,
     ],
 )
 def scan() -> None:
-    """
-    Scan a folder and register it's checksums
-    """
     archive = get_archive()
     archive.start_write()
     logger = get_logger()
     logger.info("Scanning for number of files...")
     num_files = get_number_of_files(folder=ConfigScan.folder)
     with tqdm.tqdm(total=num_files) as progress_bar:
-        for root, directories, files in os.walk(ConfigScan.folder):
+        for root, _directories, files in os.walk(ConfigScan.folder):
             for file in files:
                 filename = os.path.join(root, file)
                 filename = os.path.abspath(filename)
                 logger.debug(f"doing {filename}")
                 if archive.get_digest(filename=filename) is None:
                     digest = digest_file_bytes(filename=filename)
                     archive.add_digest(filename=filename, digest=digest)
                 progress_bar.update()
     archive.end_write()
     archive.close()
 
 
 @register_endpoint(
-    group=GROUP_NAME_DEFAULT,
+    description="Scan the DB and remove any entries which are no longer valid",
     configs=[
         ConfigScan,
         ConfigAlgo,
         ConfigLMDB,
     ],
 )
 def clean_db() -> None:
-    """
-    Scan the DB and remove any entries which are no longer valid
-    """
     logger = get_logger()
     archive = get_archive()
     archive.start_write()
     count = archive.count()
     errors = 0
     with tqdm.tqdm(total=count) as progress_bar:
         for filename, _digest in archive.yield_all_items():
@@ -93,38 +66,49 @@
             progress_bar.update()
     archive.end_write()
     archive.close()
     logger.info(f"number of errors is {errors}")
 
 
 @register_endpoint(
-    group=GROUP_NAME_DEFAULT,
+    description="Check filenames in a certain folder",
     configs=[
         ConfigScan,
         ConfigAlgo,
         ConfigLMDB,
     ],
 )
 def check_filenames() -> None:
-    """
-    Check filenames in a certain folder
-    """
     logger = get_logger()
     errors = 0
     error_filenames = []
     logger.info("Scanning for number of files...")
     num_files = get_number_of_files(folder=ConfigScan.folder)
     with tqdm.tqdm(total=num_files) as progress_bar:
-        for root, directories, files in os.walk(ConfigScan.folder):
+        for root, _directories, files in os.walk(ConfigScan.folder):
             for file in files:
                 filename = os.path.join(root, file)
                 filename = os.path.abspath(filename)
                 logger.debug(f"doing {filename}")
                 try:
                     filename.encode(ConfigAlgo.encoding)
                 except UnicodeEncodeError:
                     errors += 1
                     error_filenames.append(filename)
                 progress_bar.update()
     logger.info(f"number of errors is {errors}")
     for error_filename in error_filenames:
         logger.info(error_filename)
+
+
+@register_main(
+    main_description="pyunique will help you remove duplicate files",
+    app_name="pyunique",
+    version=VERSION_STR,
+)
+def main():
+    pylogconf.core.setup()
+    config_arg_parse_and_launch()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `pyunique-0.0.8/pyunique.egg-info/PKG-INFO` & `pyunique-0.0.9/pyunique.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunique
-Version: 0.0.8
+Version: 0.0.9
 Summary: help you get rid of duplicate files
 Home-page: https://veltzer.github.io/pyunique
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
@@ -19,26 +19,24 @@
         
         .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
         
         project website: https://veltzer.github.io/pyunique
         
         author: Mark Veltzer
         
-        version: 0.0.8
+        version: 0.0.9
         
         
         
 Keywords: duplicates,remove,hash
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `pyunique-0.0.8/setup.py` & `pyunique-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,17 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyunique",
-    version="0.0.8",
+    version="0.0.9",
     packages=[
         'pyunique',
-        'pyunique.endpoints',
     ],
     # from here all is optional
     description="help you get rid of duplicate files",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
@@ -44,20 +43,18 @@
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Topic :: Utilities',
         'License :: OSI Approved :: MIT License',
     ],
     data_files=[
     ],
     entry_points={"console_scripts": [
-        'pyunique=pyunique.endpoints.main:main',
+        'pyunique=pyunique.main:main',
     ]},
-    python_requires=">=3.6",
+    python_requires=">=3.9",
 )
```


# Comparing `tmp/pyawskit-0.1.71.tar.gz` & `tmp/pyawskit-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyawskit-0.1.71.tar", last modified: Wed Apr 19 20:13:06 2023, max compression
+gzip compressed data, was "pyawskit-0.1.72.tar", last modified: Thu Apr 27 08:16:43 2023, max compression
```

## Comparing `pyawskit-0.1.71.tar` & `pyawskit-0.1.72.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:13:06.763088 pyawskit-0.1.71/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-19 20:12:50.000000 pyawskit-0.1.71/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-19 20:13:06.763088 pyawskit-0.1.71/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      415 2023-04-19 20:12:50.000000 pyawskit-0.1.71/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:13:06.762088 pyawskit-0.1.71/pyawskit/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.71/pyawskit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.71/pyawskit/aws.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3499 2023-04-16 18:29:08.000000 pyawskit-0.1.71/pyawskit/aws_codeartifact_npm_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-16 17:13:39.000000 pyawskit-0.1.71/pyawskit/aws_codeartifact_pip_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1826 2023-04-19 20:12:23.000000 pyawskit-0.1.71/pyawskit/aws_ecr_login_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.71/pyawskit/common.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2093 2023-04-19 19:52:43.000000 pyawskit-0.1.71/pyawskit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)    14844 2023-04-19 20:03:40.000000 pyawskit-0.1.71/pyawskit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.71/pyawskit/os_utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)      211 2023-04-19 20:12:50.000000 pyawskit-0.1.71/pyawskit/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.71/pyawskit/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:13:06.763088 pyawskit-0.1.71/pyawskit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      104 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-19 20:13:06.763088 pyawskit-0.1.71/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1787 2023-04-19 20:12:50.000000 pyawskit-0.1.71/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:16:43.971326 pyawskit-0.1.72/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-27 08:16:32.000000 pyawskit-0.1.72/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1380 2023-04-27 08:16:43.971326 pyawskit-0.1.72/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      415 2023-04-27 08:16:32.000000 pyawskit-0.1.72/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:16:43.971326 pyawskit-0.1.72/pyawskit/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.72/pyawskit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.72/pyawskit/aws.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3499 2023-04-16 18:29:08.000000 pyawskit-0.1.72/pyawskit/aws_codeartifact_npm_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-16 17:13:39.000000 pyawskit-0.1.72/pyawskit/aws_codeartifact_pip_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1826 2023-04-20 17:09:19.000000 pyawskit-0.1.72/pyawskit/aws_ecr_login_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.72/pyawskit/common.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2093 2023-04-19 19:52:43.000000 pyawskit-0.1.72/pyawskit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    14829 2023-04-27 08:16:18.000000 pyawskit-0.1.72/pyawskit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.72/pyawskit/os_utils.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      190 2023-04-27 08:16:32.000000 pyawskit-0.1.72/pyawskit/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.72/pyawskit/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:16:43.971326 pyawskit-0.1.72/pyawskit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1380 2023-04-27 08:16:43.000000 pyawskit-0.1.72/pyawskit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-04-27 08:16:43.000000 pyawskit-0.1.72/pyawskit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-27 08:16:43.000000 pyawskit-0.1.72/pyawskit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-27 08:16:43.000000 pyawskit-0.1.72/pyawskit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      104 2023-04-27 08:16:43.000000 pyawskit-0.1.72/pyawskit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-27 08:16:43.000000 pyawskit-0.1.72/pyawskit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-27 08:16:43.972326 pyawskit-0.1.72/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1766 2023-04-27 08:16:32.000000 pyawskit-0.1.72/setup.py
```

### Comparing `pyawskit-0.1.71/LICENSE` & `pyawskit-0.1.72/LICENSE`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.71/PKG-INFO` & `pyawskit-0.1.72/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.71
-Summary: pyawskit is a collection of utilities to help interact with aws
+Version: 0.1.72
+Summary: ('Pyawskit is your AWS Swiss Army Knife',)
 Home-page: https://veltzer.github.io/pyawskit
 Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyawskit
 
 author: Mark Veltzer
 
-version: 0.1.71
+version: 0.1.72
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.71/pyawskit/aws.py` & `pyawskit-0.1.72/pyawskit/aws.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.71/pyawskit/aws_codeartifact_npm_env_config_code.py` & `pyawskit-0.1.72/pyawskit/aws_codeartifact_npm_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.71/pyawskit/aws_codeartifact_pip_env_config_code.py` & `pyawskit-0.1.72/pyawskit/aws_codeartifact_pip_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.71/pyawskit/aws_ecr_login_code.py` & `pyawskit-0.1.72/pyawskit/aws_ecr_login_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.71/pyawskit/common.py` & `pyawskit-0.1.72/pyawskit/common.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.71/pyawskit/configs.py` & `pyawskit-0.1.72/pyawskit/configs.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.71/pyawskit/main.py` & `pyawskit-0.1.72/pyawskit/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pyawskit.common
 from pyawskit.aws import ProcessData, request_spot_instances, tag_resources, poll_instances_till_done, wait_for_ssh, \
     attach_disks
 from pyawskit.common import update_etc_hosts, update_ssh_config, update_file, do_hush_login, wait_net_service, \
     get_disks, erase_partition_table, reread_partition_table, format_device, mount_disk
 from pyawskit.configs import ConfigFilter, ConfigName, ConfigWork, ConfigAwsCodeartifactNpm, ConfigAwsCodeartifactPip
 
-from pyawskit.static import APP_NAME, VERSION_STR
+from pyawskit.static import APP_NAME, VERSION_STR, DESCRIPTION
 from pyawskit.utils import object_exists, compress_one_file, print_exception
 
 import pyawskit.aws_codeartifact_npm_env_config_code
 import pyawskit.aws_codeartifact_pip_env_config_code
 import pyawskit.aws_ecr_login_code
 
 
@@ -380,15 +380,15 @@
             logger.info("adding line to [%s]", ConfigWork.fstab_filename)
             with open(ConfigWork.fstab_filename, "at") as file_handle:
                 file_handle.write(line_to_add + "\n")
     # create ubuntu folder and chown it to ubuntu
 
 
 @register_main(
-    main_description="Pyawskit is your AWS Swiss Army Knife",
+    main_description=DESCRIPTION,
     app_name=APP_NAME,
     version=VERSION_STR,
 )
 def main():
     setup()
     config_arg_parse_and_launch()
```

### Comparing `pyawskit-0.1.71/pyawskit/os_utils.py` & `pyawskit-0.1.72/pyawskit/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.71/pyawskit/utils.py` & `pyawskit-0.1.72/pyawskit/utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.71/pyawskit.egg-info/PKG-INFO` & `pyawskit-0.1.72/pyawskit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.71
-Summary: pyawskit is a collection of utilities to help interact with aws
+Version: 0.1.72
+Summary: ('Pyawskit is your AWS Swiss Army Knife',)
 Home-page: https://veltzer.github.io/pyawskit
 Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyawskit
 
 author: Mark Veltzer
 
-version: 0.1.71
+version: 0.1.72
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.71/setup.py` & `pyawskit-0.1.72/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,20 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyawskit",
-    version="0.1.71",
+    version="0.1.72",
     packages=[
         "pyawskit",
     ],
     # from here all is optional
-    description="pyawskit is a collection of utilities to help interact with aws",
+    description="('Pyawskit is your AWS Swiss Army Knife',)",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
```


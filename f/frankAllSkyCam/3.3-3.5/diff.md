# Comparing `tmp/frankAllSkyCam-3.3.tar.gz` & `tmp/frankAllSkyCam-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-3.3.tar", last modified: Wed Apr 26 22:08:01 2023, max compression
+gzip compressed data, was "frankAllSkyCam-3.5.tar", last modified: Wed Apr 26 22:39:45 2023, max compression
```

## Comparing `frankAllSkyCam-3.3.tar` & `frankAllSkyCam-3.5.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 22:08:01.879125 frankAllSkyCam-3.3/
--rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-04-26 22:08:01.879125 frankAllSkyCam-3.3/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 22:08:01.879125 frankAllSkyCam-3.3/frankAllSkyCam/
--rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-04-26 20:17:19.311764 frankAllSkyCam-3.3/frankAllSkyCam/__init__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3154 2023-04-26 21:40:07.492942 frankAllSkyCam-3.3/frankAllSkyCam/__main__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)      731 2023-04-26 21:40:11.166841 frankAllSkyCam-3.3/frankAllSkyCam/allskycamdelete.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     2935 2023-04-26 21:40:25.125048 frankAllSkyCam-3.3/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     1313 2023-04-25 21:31:56.286444 frankAllSkyCam-3.3/frankAllSkyCam/drawtext.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2318 2021-07-23 08:29:59.174829 frankAllSkyCam-3.3/frankAllSkyCam/fileManager.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)    17461 2023-04-26 21:42:03.411875 frankAllSkyCam-3.3/frankAllSkyCam/imageHeader.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     2827 2023-04-26 21:41:21.120601 frankAllSkyCam-3.3/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-26 16:50:47.955578 frankAllSkyCam-3.3/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.3/frankAllSkyCam/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.3/frankAllSkyCam/test_suncalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     4181 2023-04-26 21:42:02.987609 frankAllSkyCam-3.3/frankAllSkyCam/timelapse.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1319 2023-04-26 21:42:02.547265 frankAllSkyCam-3.3/frankAllSkyCam/watchDog.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-3.3/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     2249 2023-04-26 22:07:47.891276 frankAllSkyCam-3.3/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 22:08:01.879125 frankAllSkyCam-3.3/test/
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.3/test/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.3/test/test_suncalc.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 22:39:45.264971 frankAllSkyCam-3.5/
+-rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-04-26 22:39:45.264971 frankAllSkyCam-3.5/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 22:39:45.264971 frankAllSkyCam-3.5/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-04-26 20:17:19.311764 frankAllSkyCam-3.5/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3154 2023-04-26 21:40:07.492942 frankAllSkyCam-3.5/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)      731 2023-04-26 21:40:11.166841 frankAllSkyCam-3.5/frankAllSkyCam/allskycamdelete.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2935 2023-04-26 21:40:25.125048 frankAllSkyCam-3.5/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     1313 2023-04-25 21:31:56.286444 frankAllSkyCam-3.5/frankAllSkyCam/drawtext.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2318 2021-07-23 08:29:59.174829 frankAllSkyCam-3.5/frankAllSkyCam/fileManager.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 22:39:45.264971 frankAllSkyCam-3.5/frankAllSkyCam/helper/
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2142 2023-04-26 16:02:38.467378 frankAllSkyCam-3.5/frankAllSkyCam/helper/config.txt
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-04-16 22:11:11.734516 frankAllSkyCam-3.5/frankAllSkyCam/helper/index.html
+-rwxrwxrw-   0 pi        (1000) pi        (1000)    17461 2023-04-26 21:42:03.411875 frankAllSkyCam-3.5/frankAllSkyCam/imageHeader.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2827 2023-04-26 21:41:21.120601 frankAllSkyCam-3.5/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-26 16:50:47.955578 frankAllSkyCam-3.5/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.5/frankAllSkyCam/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.5/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4181 2023-04-26 21:42:02.987609 frankAllSkyCam-3.5/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1319 2023-04-26 21:42:02.547265 frankAllSkyCam-3.5/frankAllSkyCam/watchDog.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-3.5/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2249 2023-04-26 22:36:55.902808 frankAllSkyCam-3.5/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 22:39:45.264971 frankAllSkyCam-3.5/test/
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.5/test/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.5/test/test_suncalc.py
```

### Comparing `frankAllSkyCam-3.3/PKG-INFO` & `frankAllSkyCam-3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: frankAllSkyCam
-Version: 3.3
+Version: 3.5
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.3.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.5.tar.gz
 Description: UNKNOWN
 Keywords: AllSkyCamera,Astronomy,AllSky
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/__main__.py` & `frankAllSkyCam-3.5/frankAllSkyCam/__main__.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-3.5/frankAllSkyCam/allskycamdelete.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/crontab.py` & `frankAllSkyCam-3.5/frankAllSkyCam/crontab.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-3.5/frankAllSkyCam/drawtext.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-3.5/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-3.5/frankAllSkyCam/imageHeader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/startrail.py` & `frankAllSkyCam-3.5/frankAllSkyCam/startrail.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-3.5/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/test_sqm.py` & `frankAllSkyCam-3.5/frankAllSkyCam/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-3.5/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-3.5/frankAllSkyCam/timelapse.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-3.5/frankAllSkyCam/watchDog.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/setup.py` & `frankAllSkyCam-3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import shutil
 from distutils.core import setup
 
 homepath = os.path.expanduser("~")
 setup(
   name = 'frankAllSkyCam',         # How you named your package folder (MyLib)
   packages = ['frankAllSkyCam'],   # Chose the same as "name"
-  version = '3.3',      # Start with a small number and increase it with every change you make
+  version = '3.5',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',   # Give a short description about your library
   author = 'Francesco Sferlazza',                   # Type in your name
   author_email = 'sferlazza@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/sferlix/frankAllSkyCam',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.3.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.5.tar.gz',    # I explain this later on
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'pytz',
           'numpy',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

### Comparing `frankAllSkyCam-3.3/test/test_sqm.py` & `frankAllSkyCam-3.5/test/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.3/test/test_suncalc.py` & `frankAllSkyCam-3.5/test/test_suncalc.py`

 * *Files identical despite different names*


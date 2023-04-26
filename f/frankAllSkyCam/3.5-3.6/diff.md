# Comparing `tmp/frankAllSkyCam-3.5.tar.gz` & `tmp/frankAllSkyCam-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-3.5.tar", last modified: Wed Apr 26 22:39:45 2023, max compression
+gzip compressed data, was "frankAllSkyCam-3.6.tar", last modified: Wed Apr 26 23:06:35 2023, max compression
```

## Comparing `frankAllSkyCam-3.5.tar` & `frankAllSkyCam-3.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 22:39:45.264971 frankAllSkyCam-3.5/
--rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-04-26 22:39:45.264971 frankAllSkyCam-3.5/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 22:39:45.264971 frankAllSkyCam-3.5/frankAllSkyCam/
--rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-04-26 20:17:19.311764 frankAllSkyCam-3.5/frankAllSkyCam/__init__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3154 2023-04-26 21:40:07.492942 frankAllSkyCam-3.5/frankAllSkyCam/__main__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)      731 2023-04-26 21:40:11.166841 frankAllSkyCam-3.5/frankAllSkyCam/allskycamdelete.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     2935 2023-04-26 21:40:25.125048 frankAllSkyCam-3.5/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     1313 2023-04-25 21:31:56.286444 frankAllSkyCam-3.5/frankAllSkyCam/drawtext.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2318 2021-07-23 08:29:59.174829 frankAllSkyCam-3.5/frankAllSkyCam/fileManager.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 22:39:45.264971 frankAllSkyCam-3.5/frankAllSkyCam/helper/
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2142 2023-04-26 16:02:38.467378 frankAllSkyCam-3.5/frankAllSkyCam/helper/config.txt
--rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-04-16 22:11:11.734516 frankAllSkyCam-3.5/frankAllSkyCam/helper/index.html
--rwxrwxrw-   0 pi        (1000) pi        (1000)    17461 2023-04-26 21:42:03.411875 frankAllSkyCam-3.5/frankAllSkyCam/imageHeader.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     2827 2023-04-26 21:41:21.120601 frankAllSkyCam-3.5/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-26 16:50:47.955578 frankAllSkyCam-3.5/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.5/frankAllSkyCam/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.5/frankAllSkyCam/test_suncalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     4181 2023-04-26 21:42:02.987609 frankAllSkyCam-3.5/frankAllSkyCam/timelapse.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1319 2023-04-26 21:42:02.547265 frankAllSkyCam-3.5/frankAllSkyCam/watchDog.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-3.5/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     2249 2023-04-26 22:36:55.902808 frankAllSkyCam-3.5/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 22:39:45.264971 frankAllSkyCam-3.5/test/
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.5/test/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.5/test/test_suncalc.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 23:06:35.924337 frankAllSkyCam-3.6/
+-rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-04-26 23:06:35.924337 frankAllSkyCam-3.6/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 23:06:35.924337 frankAllSkyCam-3.6/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-04-26 22:51:55.451988 frankAllSkyCam-3.6/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3153 2023-04-26 22:49:40.237588 frankAllSkyCam-3.6/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)      730 2023-04-26 22:50:07.983517 frankAllSkyCam-3.6/frankAllSkyCam/allskycamdelete.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2934 2023-04-26 22:51:27.057114 frankAllSkyCam-3.6/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     1313 2023-04-25 21:31:56.286444 frankAllSkyCam-3.6/frankAllSkyCam/drawtext.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2318 2021-07-23 08:29:59.174829 frankAllSkyCam-3.6/frankAllSkyCam/fileManager.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 23:06:35.924337 frankAllSkyCam-3.6/frankAllSkyCam/helper/
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2142 2023-04-26 16:02:38.467378 frankAllSkyCam-3.6/frankAllSkyCam/helper/config.txt
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-04-16 22:11:11.734516 frankAllSkyCam-3.6/frankAllSkyCam/helper/index.html
+-rwxrwxrw-   0 pi        (1000) pi        (1000)    17460 2023-04-26 22:50:29.253456 frankAllSkyCam-3.6/frankAllSkyCam/imageHeader.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2826 2023-04-26 22:52:05.228968 frankAllSkyCam-3.6/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-26 16:50:47.955578 frankAllSkyCam-3.6/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.6/frankAllSkyCam/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.6/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4180 2023-04-26 22:50:41.282739 frankAllSkyCam-3.6/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1318 2023-04-26 22:50:52.037675 frankAllSkyCam-3.6/frankAllSkyCam/watchDog.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-3.6/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2443 2023-04-26 23:06:24.024492 frankAllSkyCam-3.6/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 23:06:35.924337 frankAllSkyCam-3.6/test/
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.6/test/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.6/test/test_suncalc.py
```

### Comparing `frankAllSkyCam-3.5/PKG-INFO` & `frankAllSkyCam-3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: frankAllSkyCam
-Version: 3.5
+Version: 3.6
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.5.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.6.tar.gz
 Description: UNKNOWN
 Keywords: AllSkyCamera,Astronomy,AllSky
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/__main__.py` & `frankAllSkyCam-3.6/frankAllSkyCam/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 from pytz import timezone
 from importlib import resources  # Python 3.7+
 from configparser import ConfigParser
 from frankAllSkyCam import imageHeader, fileManager, drawtext
 
 config = ConfigParser()
-config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt')
 time_zone = str(config['site']['time_zone'])
 inte = str(config['site']['inte'])
 
 outputFolder = str(config['system']['otuputFolder'])
 outputLocalWebFile = str(config['system']['outputLocalWebFile'])
 horiz = str(config['resolution']['horiz'])
 vert = str(config['resolution']['vert'])
```

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-3.6/frankAllSkyCam/allskycamdelete.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import os
 from pytz import timezone
 from configparser import ConfigParser
 
 config = ConfigParser()
-config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt')
 
 time_zone = str(config['site']['time_zone'])
 outputFolder = str(config['system']['otuputFolder'])
 days_retention = int(config['system']['days_retention'])
 
 def main():
     tz = timezone(time_zone)
```

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/crontab.py` & `frankAllSkyCam-3.6/frankAllSkyCam/crontab.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import math
 import os
 from importlib import resources  # Python 3.7+
 from configparser import ConfigParser
 import socket
 
 config = ConfigParser()
-config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt')
 latitude  = float(config['site']['latitude'])
 longitude = float(config['site']['longitude'])
 timeZone = str(config['site']['time_zone'])
 
 def getTimes():
 
     try:
```

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-3.6/frankAllSkyCam/drawtext.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-3.6/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/helper/config.txt` & `frankAllSkyCam-3.6/frankAllSkyCam/helper/config.txt`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-3.6/frankAllSkyCam/imageHeader.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import math
 import os
 from importlib import resources  # Python 3.7+
 from configparser import ConfigParser
 import socket
 
 config = ConfigParser()
-config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt')
 latitude  = float(config['site']['latitude'])
 longitude = float(config['site']['longitude'])
 timeZone = str(config['site']['time_zone'])
 
 full_moon_reduc = float(config['moon']['full_moon_reduc'])
 ms_offset = float(config['moon']['ms_offset'])
 ms_duration = float(config['moon']['ms_duration'])
```

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/startrail.py` & `frankAllSkyCam-3.6/frankAllSkyCam/startrail.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 from pytz import timezone
 from os import path
 from configparser import ConfigParser
 from frankAllSkyCam import fileManager
 
 config = ConfigParser()
-config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt')
 time_zone = str(config['site']['time_zone'])
 
 outputFolder = str(config['system']['otuputFolder'])
 
 isFTP = str(config['ftp']['isFTP'])=='True'
 FTP_server = str(config['ftp']['FTP_server'])
 FTP_login = str(config['ftp']['FTP_login'])
```

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-3.6/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/test_sqm.py` & `frankAllSkyCam-3.6/frankAllSkyCam/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-3.6/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-3.6/frankAllSkyCam/timelapse.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from pytz import timezone
 from os import path
 from configparser import ConfigParser
 from frankAllSkyCam import fileManager
 
 config = ConfigParser()
-config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt')
 time_zone = str(config['site']['time_zone'])
 
 outputFolder = str(config['system']['otuputFolder'])
 tl_horiz = str(config['timelapse']['tl_horiz'])
 tl_vert = str(config['timelapse']['tl_vert'])
 framerate = str(config['timelapse']['framerate'])
 nightTL = str(config['timelapse']['nightTL'])=='True'
```

### Comparing `frankAllSkyCam-3.5/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-3.6/frankAllSkyCam/watchDog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os.path, time, datetime
 from configparser import ConfigParser
 from frankAllSkyCam import fileManager
 import subprocess
 
 config = ConfigParser()
-config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt')
 logFolder = str(config['system']['logFolder'])
 myfile = str(config['system']['outputLocalWebFile'])
 maxMinutes = int(config['system']['rebootAfter'])
 
 def getOutput(command):
    output=subprocess.getoutput(command)
    space = "\n\n\n\n\n"
```

### Comparing `frankAllSkyCam-3.5/setup.py` & `frankAllSkyCam-3.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import shutil
 from distutils.core import setup
 
 homepath = os.path.expanduser("~")
 setup(
   name = 'frankAllSkyCam',         # How you named your package folder (MyLib)
   packages = ['frankAllSkyCam'],   # Chose the same as "name"
-  version = '3.5',      # Start with a small number and increase it with every change you make
+  version = '3.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',   # Give a short description about your library
   author = 'Francesco Sferlazza',                   # Type in your name
   author_email = 'sferlazza@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/sferlix/frankAllSkyCam',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.5.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.6.tar.gz',    # I explain this later on
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'pytz',
           'numpy',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
@@ -28,19 +28,23 @@
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.9',
   ],
 )
 
+if os.path.exists(homepath+"/frankAllSkyCam") == False:
+    os.mkdir(homepath+"/frankAllSkyCam")
 
-os.mkdir(homepath+"/frankAllSkyCam")
-os.mkdir(homepath+"/frankAllSkyCam/img")
-os.mkdir(homepath+"/frankAllSkyCam/logs")
+if os.path.exists(homepath+"/frankAllSkyCam/img") == False:
+    os.mkdir(homepath+"/frankAllSkyCam/img")
 
+if os.path.exists(homepath+"/frankAllSkyCam/logs") == False:
+    os.mkdir(homepath+"/frankAllSkyCam/logs")
+
+sorg1 = 'frankAllSkyCam/helper/config.txt'
 dest1 = homepath +'/frankAllSkyCam/config.txt'
-oldf1 = 'frankAllSkyCam/helper/config.txt'
-shutil.copy(oldf1, dest1)
+shutil.copy(sorg1, dest1)
 
+sorg2 = 'frankAllSkyCam/helper/index.html'
 dest2 = homepath +'/frankAllSkyCam/index.html'
-oldf2 = 'frankAllSkyCam/helper/index.html'
-shutil.copy(oldf2, dest2)
+shutil.copy(sorg2, dest2)
```

### Comparing `frankAllSkyCam-3.5/test/test_sqm.py` & `frankAllSkyCam-3.6/test/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.5/test/test_suncalc.py` & `frankAllSkyCam-3.6/test/test_suncalc.py`

 * *Files identical despite different names*


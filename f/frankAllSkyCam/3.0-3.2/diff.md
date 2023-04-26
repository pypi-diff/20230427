# Comparing `tmp/frankAllSkyCam-3.0.tar.gz` & `tmp/frankAllSkyCam-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-3.0.tar", last modified: Wed Apr 26 19:13:52 2023, max compression
+gzip compressed data, was "frankAllSkyCam-3.2.tar", last modified: Wed Apr 26 21:53:01 2023, max compression
```

## Comparing `frankAllSkyCam-3.0.tar` & `frankAllSkyCam-3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 19:13:52.861343 frankAllSkyCam-3.0/
--rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-04-26 19:13:52.861343 frankAllSkyCam-3.0/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 19:13:52.861343 frankAllSkyCam-3.0/frankAllSkyCam/
--rwxrw-rw-   0 pi        (1000) pi        (1000)       76 2023-04-26 16:49:39.397362 frankAllSkyCam-3.0/frankAllSkyCam/__init__.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3145 2023-04-25 20:05:24.252764 frankAllSkyCam-3.0/frankAllSkyCam/__main__.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      727 2023-04-05 15:29:11.223398 frankAllSkyCam-3.0/frankAllSkyCam/allskycamdelete.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2886 2023-04-26 00:07:13.329324 frankAllSkyCam-3.0/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     1313 2023-04-25 21:31:56.286444 frankAllSkyCam-3.0/frankAllSkyCam/drawtext.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2318 2021-07-23 08:29:59.174829 frankAllSkyCam-3.0/frankAllSkyCam/fileManager.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)    17452 2023-04-26 13:16:28.627084 frankAllSkyCam-3.0/frankAllSkyCam/imageHeader.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2818 2023-04-26 00:06:10.958114 frankAllSkyCam-3.0/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-26 16:50:47.955578 frankAllSkyCam-3.0/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.0/frankAllSkyCam/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.0/frankAllSkyCam/test_suncalc.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     4172 2021-05-27 13:40:12.531380 frankAllSkyCam-3.0/frankAllSkyCam/timelapse.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     1310 2021-05-31 16:22:46.426304 frankAllSkyCam-3.0/frankAllSkyCam/watchDog.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-3.0/setup.cfg
--rwxrw-rw-   0 pi        (1000) pi        (1000)     1816 2023-04-26 19:13:31.865560 frankAllSkyCam-3.0/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 19:13:52.861343 frankAllSkyCam-3.0/test/
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.0/test/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.0/test/test_suncalc.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 21:53:01.628286 frankAllSkyCam-3.2/
+-rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-04-26 21:53:01.628286 frankAllSkyCam-3.2/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 21:53:01.628286 frankAllSkyCam-3.2/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-04-26 20:17:19.311764 frankAllSkyCam-3.2/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3154 2023-04-26 21:40:07.492942 frankAllSkyCam-3.2/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)      731 2023-04-26 21:40:11.166841 frankAllSkyCam-3.2/frankAllSkyCam/allskycamdelete.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2935 2023-04-26 21:40:25.125048 frankAllSkyCam-3.2/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     1313 2023-04-25 21:31:56.286444 frankAllSkyCam-3.2/frankAllSkyCam/drawtext.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2318 2021-07-23 08:29:59.174829 frankAllSkyCam-3.2/frankAllSkyCam/fileManager.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)    17461 2023-04-26 21:42:03.411875 frankAllSkyCam-3.2/frankAllSkyCam/imageHeader.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2827 2023-04-26 21:41:21.120601 frankAllSkyCam-3.2/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-26 16:50:47.955578 frankAllSkyCam-3.2/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.2/frankAllSkyCam/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.2/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4181 2023-04-26 21:42:02.987609 frankAllSkyCam-3.2/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1319 2023-04-26 21:42:02.547265 frankAllSkyCam-3.2/frankAllSkyCam/watchDog.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-3.2/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2249 2023-04-26 21:52:03.592364 frankAllSkyCam-3.2/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-26 21:53:01.628286 frankAllSkyCam-3.2/test/
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-3.2/test/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-3.2/test/test_suncalc.py
```

### Comparing `frankAllSkyCam-3.0/PKG-INFO` & `frankAllSkyCam-3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: frankAllSkyCam
-Version: 3.0
+Version: 3.2
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.0.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.2.tar.gz
 Description: UNKNOWN
 Keywords: AllSkyCamera,Astronomy,AllSky
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/__main__.py` & `frankAllSkyCam-3.2/frankAllSkyCam/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import sys
 import datetime
 from fractions import Fraction
 import time
 from pytz import timezone
 from importlib import resources  # Python 3.7+
 from configparser import ConfigParser
-from allskycam import imageHeader, fileManager, drawtext
+from frankAllSkyCam import imageHeader, fileManager, drawtext
 
 config = ConfigParser()
-config.read(os.path.join(os.path.dirname(__file__), '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
 time_zone = str(config['site']['time_zone'])
 inte = str(config['site']['inte'])
 
 outputFolder = str(config['system']['otuputFolder'])
 outputLocalWebFile = str(config['system']['outputLocalWebFile'])
 horiz = str(config['resolution']['horiz'])
 vert = str(config['resolution']['vert'])
```

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-3.2/frankAllSkyCam/allskycamdelete.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import os
 from pytz import timezone
 from configparser import ConfigParser
 
 config = ConfigParser()
-config.read(os.path.join(os.path.dirname(__file__), '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
 
 time_zone = str(config['site']['time_zone'])
 outputFolder = str(config['system']['otuputFolder'])
 days_retention = int(config['system']['days_retention'])
 
 def main():
     tz = timezone(time_zone)
```

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/crontab.py` & `frankAllSkyCam-3.2/frankAllSkyCam/crontab.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import datetime
 import time
 import traceback
 from datetime import datetime, timedelta
-from allskycam import suncalc2
+from frankAllSkyCam import suncalc2
 from pytz import timezone
 import pytz
 import sys
 import math
 import os
 from importlib import resources  # Python 3.7+
 from configparser import ConfigParser
 import socket
 
 config = ConfigParser()
-config.read(os.path.join(os.path.dirname(__file__), '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
 latitude  = float(config['site']['latitude'])
 longitude = float(config['site']['longitude'])
 timeZone = str(config['site']['time_zone'])
 
 def getTimes():
 
     try:
@@ -50,22 +50,22 @@
        if dusk.minute > 30:
           ser = dusk.hour + 1
        else:
           ser = dusk.hour
 
        try:
            with open('./AllSkyCrontab.txt', 'w') as f:
-              f.write("*/1 " + str(mat) +"-" + str(ser-1)+ " * * * python3 -m allskycam >/dev/null 2>&1\n")
-              f.write("*/3 " + str(ser) +"-23 * * * python3 -m allskycam >/dev/null 2>&1\n")
-              f.write("*/3 0-" + str(mat-1)+" * * *  python3 -m allskycam >/dev/null 2>&1\n")
-              f.write("0 1 * * * python3 -m allskycam.allskycamdelete >/dev/null 2>&1\n")   
-              f.write("0 8 * * * python3 -m allskycam.timelapse >/dev/null 2>&1\n")
-              f.write("0 8 * * * python3 -m allskycam.startrail >/dev/null 2>&1\n")
-              f.write("*/15 * * * * python3 -m allskycam.watchDog >/dev/null 2>&1\n")
-              f.write("0 0 1 1 * python3 -m allskycam.crontab >/dev/null 2>&1\n")
+              f.write("*/1 " + str(mat) +"-" + str(ser-1)+ " * * * python3 -m frankAllSkyCam >/dev/null 2>&1\n")
+              f.write("*/3 " + str(ser) +"-23 * * * python3 -m frankAllSkyCam >/dev/null 2>&1\n")
+              f.write("*/3 0-" + str(mat-1)+" * * *  python3 -m frankAllSkyCam >/dev/null 2>&1\n")
+              f.write("0 1 * * * python3 -m frankAllSkyCam.allskycamdelete >/dev/null 2>&1\n")   
+              f.write("0 8 * * * python3 -m frankAllSkyCam.timelapse >/dev/null 2>&1\n")
+              f.write("0 8 * * * python3 -m frankAllSkyCam.startrail >/dev/null 2>&1\n")
+              f.write("*/15 * * * * python3 -m frankAllSkyCam.watchDog >/dev/null 2>&1\n")
+              f.write("0 0 1 1 * python3 -m frankAllSkyCam.crontab >/dev/null 2>&1\n")
               f.close()
               os.system("crontab -r")
               os.system("crontab ./AllSkyCrontab.txt")
               os.system("rm ./AllSkyCrontab.txt")
 
        except Exception as e:
            print("error while creating crontab: " + str(e))
```

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-3.2/frankAllSkyCam/drawtext.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-3.2/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-3.2/frankAllSkyCam/imageHeader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import datetime
 import time
 import traceback
 from datetime import datetime, timedelta
-from allskycam import suncalc2
+from frankAllSkyCam import suncalc2
 from pytz import timezone
 import pytz
 import sys
 import math
 import os
 from importlib import resources  # Python 3.7+
 from configparser import ConfigParser
 import socket
 
 config = ConfigParser()
-config.read(os.path.join(os.path.dirname(__file__), '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
 latitude  = float(config['site']['latitude'])
 longitude = float(config['site']['longitude'])
 timeZone = str(config['site']['time_zone'])
 
 full_moon_reduc = float(config['moon']['full_moon_reduc'])
 ms_offset = float(config['moon']['ms_offset'])
 ms_duration = float(config['moon']['ms_duration'])
```

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/startrail.py` & `frankAllSkyCam-3.2/frankAllSkyCam/startrail.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import ftplib
 import datetime
 import time
 import os
 from pytz import timezone
 from os import path
 from configparser import ConfigParser
-from allskycam import fileManager
+from frankAllSkyCam import fileManager
 
 config = ConfigParser()
-config.read(os.path.join(os.path.dirname(__file__), '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
 time_zone = str(config['site']['time_zone'])
 
 outputFolder = str(config['system']['otuputFolder'])
 
 isFTP = str(config['ftp']['isFTP'])=='True'
 FTP_server = str(config['ftp']['FTP_server'])
 FTP_login = str(config['ftp']['FTP_login'])
```

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-3.2/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/test_sqm.py` & `frankAllSkyCam-3.2/frankAllSkyCam/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-3.2/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-3.2/frankAllSkyCam/timelapse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import ftplib
 import datetime
 import time
 import os
 from pytz import timezone
 from os import path
 from configparser import ConfigParser
-from allskycam import fileManager
+from frankAllSkyCam import fileManager
 
 config = ConfigParser()
-config.read(os.path.join(os.path.dirname(__file__), '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
 time_zone = str(config['site']['time_zone'])
 
 outputFolder = str(config['system']['otuputFolder'])
 tl_horiz = str(config['timelapse']['tl_horiz'])
 tl_vert = str(config['timelapse']['tl_vert'])
 framerate = str(config['timelapse']['framerate'])
 nightTL = str(config['timelapse']['nightTL'])=='True'
```

### Comparing `frankAllSkyCam-3.0/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-3.2/frankAllSkyCam/watchDog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os.path, time, datetime
 from configparser import ConfigParser
-from allskycam import fileManager
+from frankAllSkyCam import fileManager
 import subprocess
 
 config = ConfigParser()
-config.read(os.path.join(os.path.dirname(__file__), '', 'config.txt'))
+config.read(os.path.expanduser("~")+"/frankAllSkyCam/", '', 'config.txt'))
 logFolder = str(config['system']['logFolder'])
 myfile = str(config['system']['outputLocalWebFile'])
 maxMinutes = int(config['system']['rebootAfter'])
 
 def getOutput(command):
    output=subprocess.getoutput(command)
    space = "\n\n\n\n\n"
```

### Comparing `frankAllSkyCam-3.0/setup.py` & `frankAllSkyCam-3.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+import os
+import shutil
 from distutils.core import setup
+
+homepath = os.path.expanduser("~")
 setup(
   name = 'frankAllSkyCam',         # How you named your package folder (MyLib)
   packages = ['frankAllSkyCam'],   # Chose the same as "name"
-  version = '3.0',      # Start with a small number and increase it with every change you make
+  version = '3.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',   # Give a short description about your library
   author = 'Francesco Sferlazza',                   # Type in your name
   author_email = 'sferlazza@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/sferlix/frankAllSkyCam',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.0.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/3.2.tar.gz',    # I explain this later on
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'pytz',
           'numpy',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
@@ -23,7 +27,20 @@
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.9',
   ],
 )
+
+
+os.mkdir(homepath+"/frankAllSkyCam")
+os.mkdir(homepath+"/frankAllSkyCam/img")
+os.mkdir(homepath+"/frankAllSkyCam/logs")
+
+dest1 = homepath +'/frankAllSkyCam/config.txt'
+oldf1 = 'frankAllSkyCam/helper/config.txt'
+shutil.copy(oldf1, dest1)
+
+dest2 = homepath +'/frankAllSkyCam/index.html'
+oldf2 = 'frankAllSkyCam/helper/index.html'
+shutil.copy(oldf2, dest2)
```

### Comparing `frankAllSkyCam-3.0/test/test_sqm.py` & `frankAllSkyCam-3.2/test/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-3.0/test/test_suncalc.py` & `frankAllSkyCam-3.2/test/test_suncalc.py`

 * *Files identical despite different names*


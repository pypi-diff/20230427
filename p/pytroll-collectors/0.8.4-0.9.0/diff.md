# Comparing `tmp/pytroll_collectors-0.8.4.tar.gz` & `tmp/pytroll_collectors-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytroll_collectors-0.8.4.tar", last modified: Thu Jan 16 10:16:25 2020, max compression
+gzip compressed data, was "dist/pytroll_collectors-0.9.0.tar", last modified: Wed Apr 15 10:45:31 2020, max compression
```

## Comparing `pytroll_collectors-0.8.4.tar` & `pytroll_collectors-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,38 @@
-drwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)        0 2020-01-16 10:16:25.018552 pytroll_collectors-0.8.4/
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      662 2020-01-16 10:16:25.018552 pytroll_collectors-0.8.4/PKG-INFO
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)       51 2020-01-16 10:14:49.000000 pytroll_collectors-0.8.4/README.md
-drwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)        0 2020-01-16 10:16:25.014552 pytroll_collectors-0.8.4/bin/
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     7393 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/bin/cat.py
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     4752 2020-01-16 10:14:49.000000 pytroll_collectors-0.8.4/bin/catter.py
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)      972 2020-01-16 10:14:49.000000 pytroll_collectors-0.8.4/bin/create_global_mosaic.py
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     9226 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/bin/gatherer.py
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)    11427 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/bin/geo_gatherer.py
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     2900 2020-01-16 10:14:49.000000 pytroll_collectors-0.8.4/bin/scale_images.py
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     2963 2020-01-16 10:14:49.000000 pytroll_collectors-0.8.4/bin/scisys_receiver.py
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     3003 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/bin/segment_gatherer.py
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)    18164 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/bin/trollstalker.py
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     8151 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/bin/trollstalker2.py
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     9388 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/bin/zipcollector_runner.py
-drwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)        0 2020-01-16 10:16:25.014552 pytroll_collectors-0.8.4/pytroll_collectors/
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      820 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/__init__.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     2477 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/file_notifiers.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    12760 2020-01-16 10:14:49.000000 pytroll_collectors-0.8.4/pytroll_collectors/global_mosaic.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     5963 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/helper_functions.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    36221 2020-01-16 10:14:49.000000 pytroll_collectors-0.8.4/pytroll_collectors/image_scaler.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    10943 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/region_collector.py
--rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)    20418 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/scisys.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    21567 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/segments.py
-drwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)        0 2020-01-16 10:16:25.018552 pytroll_collectors-0.8.4/pytroll_collectors/tests/
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     1678 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/tests/__init__.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     9460 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/tests/test_global_mosaic.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     4897 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/tests/test_helper_functions.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    20103 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/tests/test_image_scaler.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    12453 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/tests/test_scisys.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    18553 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/tests/test_segments.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     2293 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/tests/test_trigger.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    15205 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/pytroll_collectors/trigger.py
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      838 2020-01-16 10:14:49.000000 pytroll_collectors-0.8.4/pytroll_collectors/version.py
-drwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)        0 2020-01-16 10:16:25.018552 pytroll_collectors-0.8.4/pytroll_collectors.egg-info/
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      662 2020-01-16 10:16:24.000000 pytroll_collectors-0.8.4/pytroll_collectors.egg-info/PKG-INFO
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     1142 2020-01-16 10:16:24.000000 pytroll_collectors-0.8.4/pytroll_collectors.egg-info/SOURCES.txt
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)        1 2020-01-16 10:16:24.000000 pytroll_collectors-0.8.4/pytroll_collectors.egg-info/dependency_links.txt
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)        1 2020-01-16 10:16:24.000000 pytroll_collectors-0.8.4/pytroll_collectors.egg-info/not-zip-safe
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      185 2020-01-16 10:16:24.000000 pytroll_collectors-0.8.4/pytroll_collectors.egg-info/requires.txt
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)       19 2020-01-16 10:16:24.000000 pytroll_collectors-0.8.4/pytroll_collectors.egg-info/top_level.txt
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      222 2020-01-16 10:16:25.018552 pytroll_collectors-0.8.4/setup.cfg
--rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     3039 2020-01-16 10:15:27.000000 pytroll_collectors-0.8.4/setup.py
+drwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)        0 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)       61 2020-03-23 12:21:29.000000 pytroll_collectors-0.9.0/MANIFEST.in
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      583 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/PKG-INFO
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)       51 2016-11-28 10:37:12.000000 pytroll_collectors-0.9.0/README.md
+drwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)        0 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/bin/
+-rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     8596 2020-04-15 09:56:58.000000 pytroll_collectors-0.9.0/bin/cat.py
+-rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     4752 2019-11-25 12:57:51.000000 pytroll_collectors-0.9.0/bin/catter.py
+-rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)    10071 2020-03-23 12:21:29.000000 pytroll_collectors-0.9.0/bin/gatherer.py
+-rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     4950 2020-04-15 09:56:55.000000 pytroll_collectors-0.9.0/bin/scisys_receiver.py
+-rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     3015 2019-11-25 12:57:51.000000 pytroll_collectors-0.9.0/bin/segment_gatherer.py
+-rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)    18299 2019-11-25 12:57:51.000000 pytroll_collectors-0.9.0/bin/trollstalker.py
+-rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     8285 2019-11-25 12:57:51.000000 pytroll_collectors-0.9.0/bin/trollstalker2.py
+-rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)     9407 2019-11-25 12:57:51.000000 pytroll_collectors-0.9.0/bin/zipcollector_runner.py
+drwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)        0 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/pytroll_collectors/
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      912 2020-03-23 12:21:29.000000 pytroll_collectors-0.9.0/pytroll_collectors/__init__.py
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      497 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/pytroll_collectors/_version.py
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     3332 2019-11-25 12:57:51.000000 pytroll_collectors-0.9.0/pytroll_collectors/file_notifiers.py
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     6102 2019-11-25 12:57:51.000000 pytroll_collectors-0.9.0/pytroll_collectors/helper_functions.py
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    10936 2019-11-25 12:57:51.000000 pytroll_collectors-0.9.0/pytroll_collectors/region_collector.py
+-rwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)    21477 2020-04-15 09:56:55.000000 pytroll_collectors-0.9.0/pytroll_collectors/scisys.py
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    27559 2020-04-15 09:56:55.000000 pytroll_collectors-0.9.0/pytroll_collectors/segments.py
+drwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)        0 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/pytroll_collectors/tests/
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     1449 2020-04-15 09:56:55.000000 pytroll_collectors-0.9.0/pytroll_collectors/tests/__init__.py
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     4747 2019-11-25 12:57:51.000000 pytroll_collectors-0.9.0/pytroll_collectors/tests/test_helper_functions.py
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    12526 2019-11-25 12:57:51.000000 pytroll_collectors-0.9.0/pytroll_collectors/tests/test_scisys.py
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    25117 2020-04-15 09:56:55.000000 pytroll_collectors-0.9.0/pytroll_collectors/tests/test_segments.py
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     4375 2020-04-15 09:56:55.000000 pytroll_collectors-0.9.0/pytroll_collectors/tests/test_trigger.py
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    16124 2020-04-15 09:56:55.000000 pytroll_collectors-0.9.0/pytroll_collectors/trigger.py
+drwxr-xr-x   0 lahtinep  (3254) tut-uha   (5600)        0 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/pytroll_collectors.egg-info/
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      583 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/pytroll_collectors.egg-info/PKG-INFO
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      937 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/pytroll_collectors.egg-info/SOURCES.txt
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)        1 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/pytroll_collectors.egg-info/dependency_links.txt
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)        1 2020-04-15 10:35:47.000000 pytroll_collectors-0.9.0/pytroll_collectors.egg-info/not-zip-safe
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      112 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/pytroll_collectors.egg-info/requires.txt
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)       19 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/pytroll_collectors.egg-info/top_level.txt
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)      444 2020-04-15 10:45:31.000000 pytroll_collectors-0.9.0/setup.cfg
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)     2610 2020-04-15 09:56:55.000000 pytroll_collectors-0.9.0/setup.py
+-rw-r--r--   0 lahtinep  (3254) tut-uha   (5600)    68611 2020-03-23 12:21:29.000000 pytroll_collectors-0.9.0/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pytroll_collectors-0.8.4/PKG-INFO` & `pytroll_collectors-0.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: pytroll_collectors
-Version: 0.8.4
+Version: 0.9.0
 Summary: Pytroll data collectors
 Home-page: https://github.com/pytroll/pytroll-collectors
 Author: Martin Raspaud
 Author-email: martin.raspaud@smhi.se
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
-Provides-Extra: image_scaler
-Provides-Extra: global_mosaic
-Provides-Extra: all
```

### Comparing `pytroll_collectors-0.8.4/bin/catter.py` & `pytroll_collectors-0.9.0/bin/catter.py`

 * *Files identical despite different names*

### Comparing `pytroll_collectors-0.8.4/bin/gatherer.py` & `pytroll_collectors-0.9.0/bin/gatherer.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,16 +72,15 @@
         res["uri"] = fname
         res["filename"] = os.path.basename(fname)
 
     return res
 
 
 def terminator(metadata, publish_topic=None):
-    """Dummy terminator function.
-    """
+    """Terminate the gathering."""
     sorted_mda = sorted(metadata, key=lambda x: x["start_time"])
 
     mda = metadata[0].copy()
 
     if publish_topic is not None:
         LOGGER.info("Composing topic.")
         subject = compose(publish_topic, mda)
@@ -117,36 +116,39 @@
         LOGGER.info("sending %s", str(msg))
         PUB.send(str(msg))
     else:
         LOGGER.warning("Malformed metadata, no key: %s", "uri")
 
 
 def arg_parse():
-    """Handle input arguments.
-    """
+    """Handle input arguments."""
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument("-l", "--log",
                         help="File to log to (defaults to stdout)",
                         default=None)
     parser.add_argument("-v", "--verbose", help="print debug messages too",
                         action="store_true")
     parser.add_argument("-c", "--config-item",
                         help="config item to use (all by default). Can be specified multiply times",
                         action="append")
+    parser.add_argument("-p", "--publish-port", default=0, type=int,
+                        help="Port to publish the messages on. Default: automatic")
+    parser.add_argument("-n", "--nameservers",
+                        help=("Connect publisher to given nameservers: "
+                              "'-n localhost -n 123.456.789.0'. Default: localhost"),
+                        action="append")
     parser.add_argument("config", help="config file to be used")
 
     return parser.parse_args()
 
 
 def setup(decoder):
-    """Setup the granule triggerer.
-    """
-
+    """Set up the granule triggerer."""
     granule_triggers = []
 
     for section in CONFIG.sections():
         regions = [get_area_def(region)
                    for region in CONFIG.get(section, "regions").split()]
 
         timeliness = timedelta(minutes=CONFIG.getint(section, "timeliness"))
@@ -189,29 +191,33 @@
                                         decoder,
                                         [glob],
                                         observer_class,
                                         publish_topic=publish_topic)
 
         else:
             LOGGER.debug("Using posttroll for %s", section)
+            try:
+                duration = CONFIG.getfloat(section, "duration")
+            except NoOptionError:
+                duration = None
+
             granule_trigger = trigger.PostTrollTrigger(
                 collectors, terminator,
                 CONFIG.get(section, 'service').split(','),
                 CONFIG.get(section, 'topics').split(','),
+                duration=duration,
                 publish_topic=publish_topic, nameserver=nameserver,
                 publish_message_after_each_reception=publish_message_after_each_reception)
         granule_triggers.append(granule_trigger)
 
     return granule_triggers
 
 
 def main():
-    """Main() for gatherer.
-    """
-
+    """Run the gatherer."""
     global LOGGER
     global PUB
 
     opts = arg_parse()
     CONFIG.read(opts.config)
 
     print("Setting timezone to UTC")
@@ -248,18 +254,25 @@
                     "No config item called %s found in config file.", section)
         for section in CONFIG.sections():
             if section not in opts.config_item:
                 CONFIG.remove_section(section)
         if len(CONFIG.sections()) == 0:
             LOGGER.error("No valid config item provided")
             return
+        publisher_name = "gatherer_" + "_".join(opts.config_item)
+    else:
+        publisher_name = "gatherer"
+
+    publish_port = opts.publish_port
+    publisher_nameservers = opts.nameservers
 
     decoder = get_metadata
 
-    PUB = publisher.NoisyPublisher("gatherer")
+    PUB = publisher.NoisyPublisher(publisher_name, port=publish_port,
+                                   nameservers=publisher_nameservers)
 
     granule_triggers = setup(decoder)
 
     PUB.start()
 
     for granule_trigger in granule_triggers:
         granule_trigger.start()
```

### Comparing `pytroll_collectors-0.8.4/bin/scisys_receiver.py` & `pytroll_collectors-0.9.0/bin/segment_gatherer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,96 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2012, 2013, 2014, 2017 SMHI
+# Copyright (c) 2015, 2016 Panu Lahtinen
 
-# Author(s):
+# Author(s): Panu Lahtinen
 
-#   Martin Raspaud <martin.raspaud@smhi.se>
+#   Panu Lahtinen <panu.lahtinen@fmi.fi>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""Segment gatherer."""
 
-"""Receiver for 2met messages, through zeromq.
-
-Outputs messages with the following metadata:
-satellite, format, start_time, end_time, filename, uri, type, orbit_number, [instrument, number]
-
-"""
+import argparse
+import os
 import logging
-from pytroll_collectors.scisys import receive_from_zmq
+import logging.handlers
+import time
 
-if __name__ == '__main__':
+from pytroll_collectors.segments import SegmentGatherer
+from pytroll_collectors.segments import ini_to_dict
+from pytroll_collectors.helper_functions import read_yaml
 
-    import argparse
 
+def arg_parse():
+    """Handle input arguments."""
     parser = argparse.ArgumentParser()
-    parser.add_argument("host", help="GMC host")
-    parser.add_argument("port", help="Port to listen to", type=int)
-    parser.add_argument("-s", "--station", help="Name of the station",
-                        default="unknown")
-    parser.add_argument("-x", "--excluded_satellites", nargs='*',
-                        help="List of platform names to exclude",
-                        default=[])
-    parser.add_argument("-e", "--environment",
-                        help="Name of the environment (e.g. dev, test, oper)",
-                        default="dev")
-    parser.add_argument("-l", "--log", help="File to log to", default=None)
-    opts = parser.parse_args()
-
-    no_sats = opts.excluded_satellites
-
-    if opts.log:
-        import logging.handlers
-        handler = logging.handlers.TimedRotatingFileHandler(opts.log,
-                                                            "midnight",
-                                                            backupCount=7)
+    parser.add_argument("-l", "--log",
+                        help="File to log to (defaults to stdout)",
+                        default=None)
+    parser.add_argument("-v", "--verbose", help="print debug messages too",
+                        action="store_true")
+    parser.add_argument("-c", "--config", help="config file to be used")
+    parser.add_argument("-C", "--config_item",
+                        help="config item to use with .ini files")
+
+    return parser.parse_args()
+
+
+def main():
+    """Parse cmdline, read config etc."""
+    args = arg_parse()
+
+    if args.config_item:
+        config = ini_to_dict(args.config, args.config_item)
     else:
-        handler = logging.StreamHandler()
+        config = read_yaml(args.config)
+
+    print("Setting timezone to UTC")
+    os.environ["TZ"] = "UTC"
+    time.tzset()
+
+    handlers = []
+    if args.log:
+        handlers.append(
+            logging.handlers.TimedRotatingFileHandler(args.log,
+                                                      "midnight",
+                                                      backupCount=7))
+
+    handlers.append(logging.StreamHandler())
+
+    if args.verbose:
+        loglevel = logging.DEBUG
+    else:
+        loglevel = logging.INFO
+    for handler in handlers:
+        handler.setFormatter(logging.Formatter("[%(levelname)s: %(asctime)s :"
+                                               " %(name)s] %(message)s",
+                                               '%Y-%m-%d %H:%M:%S'))
+        handler.setLevel(loglevel)
+        logging.getLogger('').setLevel(loglevel)
+        logging.getLogger('').addHandler(handler)
 
-    handler.setFormatter(logging.Formatter("[%(levelname)s: %(asctime)s :"
-                                           " %(name)s] %(message)s",
-                                           '%Y-%m-%d %H:%M:%S'))
-    handler.setLevel(logging.DEBUG)
-    logging.getLogger('').setLevel(logging.DEBUG)
-    logging.getLogger('').addHandler(handler)
     logging.getLogger("posttroll").setLevel(logging.INFO)
-    logger = logging.getLogger("receiver")
+    logger = logging.getLogger("segment_gatherer")
 
+    gatherer = SegmentGatherer(config)
+    gatherer.set_logger(logger)
     try:
-        receive_from_zmq(opts.host, opts.port,
-                         opts.station, opts.environment, no_sats, 1)
-    except KeyboardInterrupt:
-        pass
-    except:
-        logger.exception("Something wrong happened...")
+        gatherer.run()
     finally:
-        print("Thank you for using pytroll/receiver."
-              " See you soon on pytroll.org!")
+        gatherer.stop()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pytroll_collectors-0.8.4/bin/trollstalker.py` & `pytroll_collectors-0.9.0/bin/trollstalker.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,20 +52,20 @@
     """
     Event handler class for inotify.
      *topic* - topic of the published messages
      *posttroll_port* - port number to publish the messages on
      *filepattern* - filepattern for finding information from the filename
     """
 
-    def __init__(self, topic, instrument, posttroll_port=0, filepattern=None,
+    def __init__(self, topic, instrument, config_item, posttroll_port=0, filepattern=None,
                  aliases=None, tbus_orbit=False, history=0, granule_length=0,
                  custom_vars=None, nameservers=[], watchManager=None):
         super(EventHandler, self).__init__()
 
-        self._pub = NoisyPublisher("trollstalker", posttroll_port, topic,
+        self._pub = NoisyPublisher("trollstalker_" + config_item, posttroll_port, topic,
                                    nameservers=nameservers)
         self.pub = self._pub.start()
         self.topic = topic
         self.info = OrderedDict()
         if filepattern is None:
             filepattern = '{filename}'
         self.file_parser = Parser(filepattern)
@@ -256,15 +256,15 @@
 
     def stop(self, *args, **kwargs):
         self._default_proc_fun.stop()
         ThreadedNotifier.stop(self, *args, **kwargs)
 
 
 def create_notifier(topic, instrument, posttroll_port, filepattern,
-                    event_names, monitored_dirs, aliases=None,
+                    event_names, monitored_dirs, config_item, aliases=None,
                     tbus_orbit=False, history=0, granule_length=0,
                     custom_vars=None, nameservers=[]):
     '''Create new notifier'''
 
     # Event handler observes the operations in defined folder
     manager = WatchManager()
 
@@ -275,14 +275,15 @@
     for event in event_names:
         try:
             event_mask |= getattr(pyinotify, event)
         except AttributeError:
             LOGGER.warning('Event ' + event + ' not found in pyinotify')
 
     event_handler = EventHandler(topic, instrument,
+                                 config_item,
                                  posttroll_port=posttroll_port,
                                  filepattern=filepattern,
                                  aliases=aliases,
                                  tbus_orbit=tbus_orbit,
                                  history=history,
                                  granule_length=granule_length,
                                  custom_vars=custom_vars,
@@ -377,14 +378,15 @@
         monitored_dirs = None
 
     posttroll_port = args.posttroll_port
     topic = args.topic
     event_names = args.event_names
     instrument = args.instrument
     nameservers = args.nameservers
+    config_item = args.config_item
 
     filepattern = args.filepattern
     if args.filepattern == '':
         filepattern = None
 
     if args.configuration_file is not None:
         config_fname = args.configuration_file
@@ -467,15 +469,15 @@
     if nameservers:
         nameservers = nameservers.split(',')
     else:
         nameservers = []
 
     # Start watching for new files
     notifier = create_notifier(topic, instrument, posttroll_port, filepattern,
-                               event_names, monitored_dirs, aliases=aliases,
+                               event_names, monitored_dirs, config_item, aliases=aliases,
                                tbus_orbit=tbus_orbit, history=history,
                                granule_length=granule_length,
                                custom_vars=custom_vars,
                                nameservers=nameservers)
     notifier.start()
 
     try:
```

### Comparing `pytroll_collectors-0.8.4/bin/trollstalker2.py` & `pytroll_collectors-0.9.0/bin/trollstalker2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2013 - 2018 PyTroll Community
+# Copyright (c) 2013 - 2019 PyTroll Community
 
 # Author(s):
 
 #   Joonas Karjalainen <joonas.karjalainen@fmi.fi>
 #   Panu Lahtinen <panu.lahtinen@fmi.fi>
 #   Martin Raspaud <martin.raspaud@smhi.se>
 #   Adam Dybbroe <adam.dybbroe@smhi.se
@@ -25,35 +25,41 @@
 
 """./trollstalker.py -c /path/to/trollstalker_config.ini -C noaa_hrpt
 """
 
 import argparse
 import sys
 import time
-from six.moves.configparser import ConfigParser
+from six.moves.configparser import RawConfigParser
 import logging
 import logging.config
 import os.path
 import datetime as dt
 
 from posttroll.publisher import NoisyPublisher
 from posttroll.message import Message
 from trollsift import Parser
 
 LOGGER = logging.getLogger(__name__)
 
+try:
+    # Python 2
+    str_or_unicode = (str, unicode)
+except NameError:
+    # Pyton 3
+    str_or_unicode = (str, bytes)
 
 from pytroll_collectors.trigger import AbstractWatchDogProcessor
 
 
 class FilePublisher(AbstractWatchDogProcessor):
 
     def __init__(self, config):
         self.config = config.copy()
-        if isinstance(config["filepattern"], (str, unicode)):
+        if isinstance(config["filepattern"], str_or_unicode):
             self.config["filepattern"] = [self.config["filepattern"]]
 
         self.parsers = [Parser(filepattern)
                         for filepattern in self.config["filepattern"]]
 
         self.aliases = parse_aliases(config)
 
@@ -71,15 +77,15 @@
                                    int(self.config["posttroll_port"]),
                                    self.config["topic"])
         self.pub = None
 
         obsolete_keys = ["topic", "filepattern", "tbus_orbit",
                          "posttroll_port", "watch", "config_item", "configuration_file"]
 
-        for key in self.config.keys():
+        for key in list(self.config.keys()):
             if key.startswith("alias_") or key in obsolete_keys:
                 del self.config[key]
 
     def start(self):
         AbstractWatchDogProcessor.start(self)
         self.pub = self._pub.start()
 
@@ -187,15 +193,15 @@
         config_fname = args.configuration_file
 
         if "template" in config_fname:
             print("Template file given as trollstalker logging config,"
                   " aborting!")
             sys.exit()
 
-        cparser = ConfigParser()
+        cparser = RawConfigParser()
         cparser.read(config_fname)
         config = dict(cparser.items(args.config_item, vars=args_dict))
 
     config.update(args_dict)
 
     config.update({k: config[k].split(",")
                    for k in config if "," in config[k]})
```

### Comparing `pytroll_collectors-0.8.4/bin/zipcollector_runner.py` & `pytroll_collectors-0.9.0/bin/zipcollector_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,57 +16,58 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Posttroll runner for the zipcollector: Listen to messages with datasets
-(from gatherer) and zip files in the dataset together into one tar file and
-store on disk in configurable destination directory
+"""Posttroll runner for the zipcollector.
+
+Listen to messages with datasets (from gatherer) and zip files in the dataset
+together into one tar file and store on disk in configurable destination directory.
 
 """
 
+import logging
 import os
-import yaml
 import shutil
+import sys
 import tarfile
+from datetime import timedelta
+
+import yaml
+from six.moves.urllib.parse import urlparse
+
+import posttroll.subscriber
+from posttroll.publisher import Publish
+from trollsift.parser import compose
 
-import logging
 LOG = logging.getLogger(__name__)
 
 #: Default time format
 _DEFAULT_TIME_FORMAT = '%Y-%m-%d %H:%M:%S'
 
 #: Default log format
 _DEFAULT_LOG_FORMAT = '[%(levelname)s: %(asctime)s : %(name)s] %(message)s'
 
 ENV_MODE = os.getenv("ENV_MODE")
 if ENV_MODE is None:
     ENV_MODE = "offline"
 
-import sys
-from six.moves.urllib.parse import urlparse
-from datetime import timedelta
-
-import posttroll.subscriber
-from posttroll.publisher import Publish
-from trollsift.parser import compose
 
 PLATFORM_NAME = {'Meteosat-10': 'met10',
                  'Meteosat-11': 'met11',
                  'Meteosat-9': 'met09',
                  'Meteosat-8': 'met08'}
 
 
 def get_arguments():
-    """
-    Get command line arguments
-    Return
-    name of the service and the config filepath
+    """Get command line arguments.
+
+    Return name of the service and the config filepath
     """
     import argparse
 
     parser = argparse.ArgumentParser()
 
     parser.add_argument('-c', '--config_file',
                         type=str,
@@ -98,16 +99,15 @@
         print("Template file given as master config, aborting!")
         sys.exit()
 
     return service, args.config_file
 
 
 def get_config(configfile, service, procenv):
-    """Get the configuration from file"""
-
+    """Get the configuration from file."""
     with open(configfile, 'r') as fp_:
         config = yaml.load(fp_)
 
     options = {}
     for item in config:
         if not isinstance(config[item], dict):
             options[item] = config[item]
@@ -119,16 +119,15 @@
                     for memb in config[service][key]:
                         options[memb] = config[service][key][memb]
 
     return options
 
 
 def start_zipcollector(registry, message, options, **kwargs):
-    """From a posttroll (gatherer) message start the pytroll zip collector"""
-
+    """From a posttroll (gatherer) message start the pytroll zip collector."""
     del kwargs
     outdir_destination = options['destination_output_dir']
     outdir_local = options['local_output_dir']
     requested_tslots = options['requested_timeslots']
 
     LOG.info("")
     LOG.info("registry dict: " + str(registry))
@@ -150,15 +149,15 @@
         start_time = None
         return registry
 
     if 'end_time' in message.data:
         end_time = message.data['end_time']
     else:
         LOG.warning("No end time in message!")
-        end_time = start_time + timedelta(seconds=60 * 12)
+        end_time = start_time + timedelta(seconds=60 * 12)  # noqa
 
     if 'seviri' not in message.data['sensor']:
         LOG.debug("Scene is not supported")
         LOG.warning(
             "Sensor {0} is not SEVIRI! Continue".format(str(message.data['sensor'])))
         return registry
     else:
@@ -208,31 +207,31 @@
     else:
         LOG.info("Time slot {0} NOT requested. Do nothing".format(start_time))
 
     return registry
 
 
 def copy_file_to_destination(inpath, outpath):
-    """Copy a file from one destination (typical local disk or a SAN type disk
-    storage) to another (typically NFS based filesystem) using tempfile
+    """Copy a file.
 
-    """
+    Copy a file from one destination (typical local disk or a SAN type disk storage)
+    to another (typically NFS based filesystem) using tempfile
 
+    """
     import tempfile
     tmp_filepath = tempfile.mktemp(suffix='_' + os.path.basename(outpath),
                                    dir=os.path.dirname(outpath))
     shutil.copy(inpath, tmp_filepath)
     os.rename(tmp_filepath, outpath)
 
     return
 
 
 def zipcollector_live_runner(options):
-    """Listens and triggers processing"""
-
+    """Listen and trigger processing."""
     LOG.info("*** Start the zipcollector runner:")
     LOG.debug("Listens for messages of type: %s", options['message_type'])
     with posttroll.subscriber.Subscribe('', [options['message_type'], ], True) as subscr:
         with Publish('zipcollector_runner', 0) as publisher:
             file_reg = {}
             for msg in subscr.recv():
                 file_reg = start_zipcollector(
```

### Comparing `pytroll_collectors-0.8.4/pytroll_collectors/__init__.py` & `pytroll_collectors-0.9.0/pytroll_collectors/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,9 +16,11 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""The place where everything starts :)
-"""
+"""The place where everything starts :)."""
+from ._version import get_versions
+__version__ = get_versions()['version']
+del get_versions
```

### Comparing `pytroll_collectors-0.8.4/pytroll_collectors/helper_functions.py` & `pytroll_collectors-0.9.0/pytroll_collectors/helper_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-'''Helper functions
-'''
+"""Helper functions."""
 
 import os
 import datetime as dt
 import re
 import logging
 from six.moves.urllib.parse import urlparse
 import netifaces
@@ -35,20 +34,21 @@
 
 from trollsift import compose
 
 LOG = logging.getLogger(__name__)
 
 
 def create_aligned_datetime_var(var_pattern, info_dict):
-    """
-    uses *var_patterns* like "{time:%Y%m%d%H%M|align(15)}"
+    """Create an aligned datetime variable.
+
+    Uses *var_patterns* like "{time:%Y%m%d%H%M|align(15)}"
     to new datetime including support for temporal
     alignment (Ceil/Round a datetime object to a multiple of a timedelta.
     Useful to equalize small time differences in name of files
-    belonging to the same timeslot)
+    belonging to the same timeslot).
     """
     mtch = re.match(
         '{(.*?)(!(.*?))?(\\:(.*?))?(\\|(.*?))?}',
         var_pattern)
 
     if mtch is None:
         return None
@@ -72,24 +72,21 @@
                 dt.timedelta(minutes=align_params[0]),
                 dt.timedelta(minutes=align_params[1]),
                 align_params[2])
 
     if res is None:
         # fallback to default compose when no special handling needed
         # NOTE: This will fail, there's no `var_val`!!!
-        res = compose(var_val, self.info)
+        res = compose(var_val, self.info)  # noqa
 
     return res
 
 
 def _parse_align_time_transform(transform_spec):
-    """
-    Parse the align-time transformation string "align(15,0,-1)"
-    and returns *(steps, offset, intv_add)*
-    """
+    """Parse the align-time transformation string "align(15,0,-1)" and returns *(steps, offset, intv_add)*."""
     match = re.search('align\\((.*)\\)', transform_spec)
     if match:
         al_args = match.group(1).split(',')
         steps = int(al_args[0])
         if len(al_args) > 1:
             offset = int(al_args[1])
         else:
@@ -99,47 +96,50 @@
         else:
             intv_add = 0
         return (steps, offset, intv_add)
     else:
         return None
 
 
-def align_time(input_val, steps=dt.timedelta(minutes=5),
-               offset=dt.timedelta(minutes=0), intervals_to_add=0):
-    """
-    Ceil/Round a datetime object to a multiple of a timedelta.
+def align_time(input_val, steps=None,
+               offset=None, intervals_to_add=0):
+    """Ceil/Round a datetime object to a multiple of a timedelta.
+
     Useful to equalize small time differences in name of files
     belonging to the same timeslot
     """
+    offset = offset or dt.timedelta(minutes=0)
+    steps = steps or dt.timedelta(minutes=5)
+
     try:
         stepss = steps.total_seconds()
     # Python 2.6 compatibility hack
-    except AttributError:
+    except AttributeError:
         stepss = steps.days * 86400. + \
             steps.seconds + steps.microseconds * 1e-6
     val = input_val - offset
     vals = (val - val.min).seconds
     result = val - dt.timedelta(seconds=(vals - (vals // stepss) * stepss))
     result = result + (intervals_to_add * steps)
     return result
 
 
 def parse_aliases(config):
-    '''Parse aliases from the config.
+    """Parse aliases from the config.
 
     Aliases are given in the config as:
 
     {'alias_<name>': 'value:alias'}, or
     {'alias_<name>': 'value1:alias1|value2:alias2'},
 
     where <name> is the name of the key which value will be
     replaced. The later form is there to support several possible
     substitutions (eg. '2' -> '9' and '3' -> '10' in the case of MSG).
 
-    '''
+    """
     aliases = {}
 
     for key in config:
         if 'alias' in key:
             alias = config[key]
             new_key = key.replace('alias_', '')
             if '|' in alias or ':' in alias:
@@ -150,14 +150,15 @@
                     aliases2[key2] = val2
                 alias = aliases2
             aliases[new_key] = alias
     return aliases
 
 
 def get_local_ips():
+    """Get the local ips."""
     inet_addrs = [netifaces.ifaddresses(iface).get(netifaces.AF_INET)
                   for iface in netifaces.interfaces()]
     ips = []
     for addr in inet_addrs:
         if addr is not None:
             for add in addr:
                 ips.append(add['addr'])
@@ -197,14 +198,14 @@
                 os.stat(url.path)
             except OSError:
                 return False
     return True
 
 
 def read_yaml(fname):
-    """Read YAML file"""
+    """Read YAML file."""
     import yaml
 
     with open(fname, 'r') as fid:
-        data = yaml.load(fid)
+        data = yaml.load(fid, Loader=yaml.SafeLoader)
 
     return data
```

### Comparing `pytroll_collectors-0.8.4/pytroll_collectors/region_collector.py` & `pytroll_collectors-0.9.0/pytroll_collectors/region_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,62 +18,58 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Region collector.
-"""
+"""Region collector."""
 
 import os
 from datetime import timedelta, datetime
 
 from trollsched.satpass import Pass
 
 import logging
 
 LOG = logging.getLogger(__name__)
 
 PLOT = False
 
 
 class RegionCollector(object):
+    """This is the region collector.
 
-    """This is the region collector. It collects granules that overlap on a
-    region of interest and return the collection of granules when it's done.
+    It collects granules that overlap on a region of interest and return the
+    collection of granules when it's done.
 
     *timeliness* defines the max allowed age of the granule.
 
     """
 
     def __init__(self, region,
-                 timeliness=timedelta(seconds=600),
+                 timeliness=None,
                  granule_duration=None):
+        """Initialize the region collector."""
         self.region = region  # area def
         self.granule_times = set()
         self.granules = []
         self.planned_granule_times = set()
-        self.timeliness = timeliness
+        self.timeliness = timeliness or timedelta(seconds=600)
         self.timeout = None
         self.granule_duration = granule_duration
         self.last_file_added = False
         self.sensor = None
 
     def __call__(self, granule_metadata):
+        """Perform the collection on the granule."""
         return self.collect(granule_metadata)
 
     def collect(self, granule_metadata):
-        """ 
-            Parameters:
-
-                granule_metadata : metadata
-
-        """
-
+        """Do the collection."""
         # Check if input data is being waited for
 
         if "tle_platform_name" in granule_metadata:
             platform = granule_metadata['tle_platform_name']
         else:
             platform = granule_metadata['platform_name']
 
@@ -217,15 +213,15 @@
         # If last granule return swath and cleanup
         if self.is_swath_complete():
             LOG.debug("Collection finished for area: %s",
                       str(self.region.area_id))
             return self.finish()
 
     def is_swath_complete(self):
-        '''Check if the swath is complete'''
+        """Check if the swath is complete."""
         if self.granule_times:
             if self.planned_granule_times.issubset(self.granule_times):
                 return True
             try:
                 new_timeout = (max(self.planned_granule_times -
                                    self.granule_times) +
                                self.granule_duration +
@@ -239,44 +235,37 @@
             if new_timeout < self.timeout:
                 self.timeout = new_timeout
                 LOG.info("Adjusted timeout: %s", self.timeout.isoformat())
 
         return False
 
     def cleanup(self):
-        '''Clear members.
-        '''
+        """Clear members."""
         self.granule_times = set()
         self.granules = []
         self.planned_granule_times = set()
         self.timeout = None
 
     def finish(self):
-        '''Finish collection, add area ID to metadata, cleanup and return
-        granule metadata.
-        '''
+        """Finish collection, add area ID to metadata, cleanup and return granule metadata."""
         granules = self.granules
         self.cleanup()
         return granules
 
     def finish_without_reset(self):
-        '''Finish collection, add area ID to metadata, DON'T cleanup and return
-        granule metadata.
-        '''
+        """Finish collection, add area ID to metadata, DON'T cleanup and return granule metadata."""
         return self.granules
 
     def is_last_file_added(self):
-        '''Return if last file was added to the region
-        '''
+        """Return if last file was added to the region."""
         return self.last_file_added
 
 
 def read_granule_metadata(filename):
-    """Read granule metadata.
-    """
+    """Read granule metadata."""
     import json
     with open(filename) as jfp:
         metadata = json.load(jfp)[0]
 
     metadata['uri'] = "file://" + os.path.abspath(filename)
 
     for attr in ["start_time", "end_time"]:
```

### Comparing `pytroll_collectors-0.8.4/pytroll_collectors/scisys.py` & `pytroll_collectors-0.9.0/pytroll_collectors/scisys.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-
-# Copyright (c) 2012-2018 Pytroll Developers
-
+#
+# Copyright (c) 2012-2020 Pytroll Developers
+#
 # Author(s):
-
+#
 #   Martin Raspaud <martin.raspaud@smhi.se>
-
+#   Janne Kotro <janne.kotro@fmi.fi>
+#   Panu Lahtinen <panu.lahtinen@fmi.fi>
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-
+#
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Receiver for 2met messages, through zeromq.
 
 Outputs messages with the following metadata:
 - satellite
@@ -42,15 +44,15 @@
 from time import sleep
 from six.moves.urllib.parse import SplitResult, urlsplit, urlunsplit
 
 from posttroll.message import Message
 from posttroll.publisher import Publish
 from pytroll_collectors.helper_functions import is_uri_on_server
 
-LOGGER = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 JPSS_INSTRUMENTS_FROM_FILENAMES = {"RATMS-RNSCA_": "atms",
                                    "RCRIS-RNSCA_": "cris",
                                    "RNSCA-RVIRS_": "viirs",
                                    "RATMS_": "atms",
                                    "RCRIS_": "cris"}
 JPSS_PLATFORM_NAME = {'npp': 'Suomi-NPP',
@@ -61,152 +63,149 @@
 
 SCISYS_NAMES = {'Suomi-NPP': 'NPP',
                 'NOAA-20': 'NOAA 20',
                 'NOAA-21': 'NOAA 21'}
 
 
 class TwoMetMessage(object):
-
-    """Interperter for 2met! messages.
-    """
+    """Interperter for 2met! messages."""
 
     def __init__(self, mstring=None):
+        """Init the message."""
         self._id = 0
         self._type = ""
         self._time = datetime.utcnow()
         self.body = ''
         if mstring is not None:
             self._decode(mstring.strip())
         self._attrs = {}
 
     def _internal_decode(self, mstring):
-        """Decode 2met! messages, internal format.
-        """
+        """Decode 2met! messages, internal format."""
         dummy, content = mstring.split("[", 1)
         content = content.rsplit("]", 1)[0]
         dic = dict((item.split("=", 1) for item in content.split(", ", 3)))
         self._id = eval(dic["ID"])
         self._time = datetime.strptime(
             eval(dic["time"]), "%d %m %Y - %H:%M:%S")
         try:
             self.body = eval(dic["body"])
         except SyntaxError:
             self.body = str(dic["body"])
         self._type = eval(dic["type"])
 
     def _xml_decode(self, mstring):
-        """Decode xml 2met! messages.
-        """
+        """Decode xml 2met! messages."""
         root = etree.fromstring(mstring)
         self._attrs = dict(root.items())
 
         self._id = int(root.get("sequence"))
         self._type = root.get("type")
         self._time = datetime.strptime(root.get("timestamp"),
                                        "%Y-%m-%dT%H:%M:%S")
         for child in root:
             if child.tag == "body":
                 self.body = child.text
 
     def _decode(self, mstring):
-        """Decode 2met! messages.
-        """
-
+        """Decode 2met! messages."""
         if mstring.startswith("Message["):
             self._internal_decode(mstring)
         elif mstring.startswith("<message"):
             try:
                 self._xml_decode(mstring)
-            except:
-                LOGGER.exception("Spurious message! %s", str(mstring))
+            except Exception:
+                logger.exception("Spurious message! %s", str(mstring))
         else:
-            LOGGER.warning("Don't know how to decode message: %s",
+            logger.warning("Don't know how to decode message: %s",
                            str(mstring))
 
 
 def pass_name(utctime, satellite):
-    """Construct a unique pass name from a risetime and a satellite name.
-    """
+    """Construct a unique pass name from a risetime and a satellite name."""
     # return utctime.strftime("%Y%m%dT%H%M%S") + "_".join(satellite.split(" "))
     return utctime, "_".join(satellite.split(" "))
 
 
 class PassRecorder(dict):
+    """Recorder for passes."""
 
     def iter(self):
+        """Return an iterator over the passes."""
         if hasattr(self, 'iteritems'):
-            return self.iteritems()
+            return self.iteritems()  # noqa
         else:
             return self.items()
 
     def get(self, key, default=None):
+        """Get a pass."""
         utctime, satellite = key
         for (rectime, recsat), val in self.iter():
             if(recsat == satellite and
                (abs(rectime - utctime)).seconds < 30 * 60 and
                (abs(rectime - utctime)).days == 0):
                 return val
         return default
 
 
 class MessageReceiver(object):
+    """Interprets received messages between stop reception and file dispatch."""
 
-    """Interprets received messages between stop reception and file dispatch.
-    """
-
-    def __init__(self, emitter, excluded_satellite_list=None):
+    def __init__(self, emitter, excluded_satellite_list=None,
+                 target_server=None, ftp_prefix=None):
+        """Init the receiver."""
         self._received_passes = PassRecorder()
         self._distributed_files = {}
         self._emitter = emitter
         if excluded_satellite_list is not None:
             self._excluded_platforms = excluded_satellite_list
         else:
             self._excluded_platforms = []
+        self._target_server = target_server
+        self._ftp_prefix = ftp_prefix
 
     def add_pass(self, message):
-        """Formats pass info and adds it to the object.
-        """
+        """Format pass info and add it to the object."""
         info = dict((item.split(": ", 1) for item in message.split(", ", 3)))
-        LOGGER.info("Adding pass: %s", str(info))
+        logger.info("Adding pass: %s", str(info))
         pass_info = {}
         for key, val in info.items():
             pass_info[key.lower()] = val
         pass_info["start_time"] = datetime.strptime(pass_info["risetime"],
                                                     "%Y-%m-%d %H:%M:%S")
         del pass_info['risetime']
         pass_info["end_time"] = datetime.strptime(pass_info["falltime"],
                                                   "%Y-%m-%d %H:%M:%S")
         del pass_info['falltime']
 
         if 'orbit number' in pass_info:
             pass_info['orbit_number'] = int(pass_info['orbit number'])
             del pass_info['orbit number']
         else:
-            LOGGER.warning("No 'orbit number' in message!")
+            logger.warning("No 'orbit number' in message!")
 
         pname = pass_name(pass_info["start_time"], pass_info["satellite"])
         self._received_passes[pname] = pass_info
 
     def clean_passes(self, days=1):
-        """Clean old passes from the pass dict (_received_passes).
-        """
+        """Clean old passes from the pass dict (`_received_passes`)."""
         oldies = []
 
         for key, val in self._received_passes.items():
             if (datetime.utcnow() - val["start_time"]).days >= days:
                 oldies.append(key)
 
         for key in oldies:
             del self._received_passes[key]
 
     def handle_distrib(self, url):
         """React to a file dispatch message."""
         url = urlsplit(url)
         dummy, filename = os.path.split(url.path)
-        LOGGER.debug("filename = %s", filename)
+        logger.debug("filename = %s", filename)
         # TODO: Should not make any assumptions on filename formats, should
         # load a description of it from a config file instead.
         if filename.endswith(".hmf"):
             risestr, satellite = filename[:-4].split("_", 1)
             risetime = datetime.strptime(risestr, "%Y%m%d%H%M%S")
             pname = pass_name(risetime, satellite)
             satellite = satellite.replace("_", "-")
@@ -242,15 +241,15 @@
                 satellite = "EOS-Aqua"
                 pname = pass_name(risetime, 'AQUA')
             else:
                 raise ValueError(
                     "Unrecognized satellite ID: " + pds["apid1"][:3])
 
             if not satellite or satellite in self._excluded_platforms:
-                LOGGER.debug("Platform name %s is excluded...", str(satellite))
+                logger.debug("Platform name %s is excluded...", str(satellite))
                 return None
 
             swath = self._received_passes.get(pname, {}).copy()
             swath.pop('satellite', None)
             swath['platform_name'] = satellite
             swath['start_time'] = risetime
             instruments = {"0064": "modis",
@@ -291,22 +290,22 @@
                     end_time_item = filename.strip(prefix).split('_')[3]
                     satellite = JPSS_PLATFORM_NAME.get(filename.strip(prefix).split('_')[0], None)
                     orbit = filename.strip(prefix).split('_')[4].strip('b')
                     file_ok = True
                     break
 
             if not file_ok:
-                LOGGER.warning("Seems to be a NPP/JPSS RDR "
+                logger.warning("Seems to be a NPP/JPSS RDR "
                                "file but name is not standard!")
-                LOGGER.warning("filename = %s", filename)
+                logger.warning("filename = %s", filename)
                 return None
 
             # satellite = "Suomi-NPP, NOAA-20, NOAA-21,..."
             if not satellite or satellite in self._excluded_platforms:
-                LOGGER.debug("Platform name %s is excluded...", str(satellite))
+                logger.debug("Platform name %s is excluded...", str(satellite))
                 return None
 
             mda["start_time"] = \
                 datetime.strptime(start_time_items[0] + start_time_items[1],
                                   "d%Y%m%dt%H%M%S%f")
             end_time = \
                 datetime.strptime(start_time_items[0] + end_time_item,
@@ -352,15 +351,15 @@
                           "M03": "Metop-C"}
 
             satellite = satellites[filename[12:15]]
             risetime = datetime.strptime(filename[16:31], "%Y%m%d%H%M%SZ")
             falltime = datetime.strptime(filename[32:47], "%Y%m%d%H%M%SZ")
 
             pname = pass_name(risetime, satellite.upper())
-            LOGGER.debug("pname= % s", str(pname))
+            logger.debug("pname= % s", str(pname))
             swath = self._received_passes.get(pname, {}).copy()
             swath.pop('satellite', None)
             swath["start_time"] = risetime
             swath["end_time"] = falltime
             swath["platform_name"] = satellite
             swath["sensor"] = instruments[filename[:4]]
             swath["format"] = "EPS"
@@ -382,15 +381,15 @@
             netloc = url.hostname
             uri = urlunsplit(SplitResult(scheme,
                                          netloc,
                                          url.path,
                                          url.query,
                                          url.fragment))
         else:
-            LOGGER.debug("url.scheme not expected: %s", url.scheme)
+            logger.debug("url.scheme not expected: %s", url.scheme)
 
         swath["uid"] = os.path.split(url.path)[1]
         swath["uri"] = uri
         swath['variant'] = 'DR'
         return swath
 
     def receive(self, message):
@@ -406,68 +405,78 @@
         elif message.body.startswith(dispatch_prefix):
             # Check hostname in message:
             filename, url = message.body[len(dispatch_prefix):].split(" ")
             url = compose_dest_url(filename, url)
             if is_uri_on_server(url, strict=True):
                 return self.handle_distrib(url)
         elif message.body.startswith(dispatch_prefix2):
-            filename, arr, url = message.body[len(dispatch_prefix2):].split(" ")
-            url = 'ftp://' + url.replace(':', '')
-            del arr
-            LOGGER.debug("filename = <%s> url = <%s>", filename, url)
-            url = compose_dest_url(filename, url)
-            LOGGER.debug("url = %s", url)
-            if is_uri_on_server(url, strict=True):
+            filename, _, url = message.body[len(dispatch_prefix2):].split(" ")
+            ip_address, path = url.split(":")
+            logger.debug("Sent to IP: %s", str(ip_address))
+            logger.debug("Target server IPs: %s ", str(self._target_server))
+            if ip_address in self._target_server:
+                logger.debug("Found correct target server: %s", ip_address)
+                if self._ftp_prefix is not None:
+                    path = os.path.join(self._ftp_prefix, path)
+                    logger.debug("ftp_prefix added: %s", path)
+                url = 'ftp://' + ip_address + path
+                logger.debug("filename = <%s> url = <%s>", filename, url)
+                url = compose_dest_url(filename, url)
+                logger.debug("url = %s", url)
                 return self.handle_distrib(url)
+            else:
+                logger.debug("File is not on targer server.")
+                return None
 
 
 def compose_dest_url(source, dest):
     """Take the filename from *source* and append it to *dest* if needed."""
     filename = os.path.split(source)[1]
     if not dest.endswith(filename):
         dest = urlsplit(dest)
         dest = urlunsplit((dest[0], dest[1],
                            os.path.join(dest[2], filename),
                            dest[3], dest[4]))
     return dest
 
 
 class GMCSubscriber(object):
+    """Listener for GMC messages."""
 
     def __init__(self, host, port):
+        """Init the subscriber."""
         self._host = host
         self._port = port
         self._sock = None
         self.msg = ""
         self._bufsize = 256
         self.loop = True
 
     def recv(self):
-        """Receive messages.
-        """
+        """Receive messages."""
         while self.loop:
             self._sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             try:
                 self._sock.connect((self._host, self._port))
             except socket.error:
-                LOGGER.error("Cannot connect to %s, retrying in 60 seconds.",
+                logger.error("Cannot connect to %s, retrying in 60 seconds.",
                              str((self._host, self._port)))
                 sleep(60)
                 continue
             self._sock.settimeout(1.0)
             try:
                 while self.loop:
                     try:
                         data = self._sock.recv(self._bufsize)
                     except socket.timeout:
                         pass
                     else:
                         if not data:
                             break
-                        self.msg += data
+                        self.msg += data.decode('utf-8')
                         messages = self.msg.split("</message>")
                         if len(messages) > 1:
                             for mess in messages[:-1]:
                                 yield mess + "</message>"
                             if messages[-1].endswith("</body>"):
                                 yield messages[-1] + "</message>"
                                 self.msg = ""
@@ -476,48 +485,55 @@
                         elif self.msg.endswith("</message>"):
                             yield self.msg
                             self.msg = ""
             finally:
                 self._sock.close()
 
     def stop(self):
+        """Stop the listener."""
         self.loop = False
 
 
-def receive_from_zmq(host, port, station, environment, excluded_platforms, days=1):
-    """Receive 2met! messages from zeromq.
-    """
+def receive_from_zmq(host, port, station, environment, excluded_platforms,
+                     target_server, ftp_prefix, topic_postfix,
+                     publish_port=0, nameservers=None, days=1):
+    """Receive 2met! messages from zeromq."""
+    logger.debug("target_server: %s", str(target_server))
+    logger.debug("ftp_prefix: %s", str(ftp_prefix))
+    logger.debug("topic_postfix: %s", str(topic_postfix))
+    logger.debug("station %s", str(station))
+    logger.debug(type(target_server))
 
     # socket = Subscriber(["tcp://localhost:9331"], ["2met!"])
     sock = GMCSubscriber(host, port)
-    msg_rec = MessageReceiver(host, excluded_platforms)
+    msg_rec = MessageReceiver(host, excluded_platforms,
+                              target_server, ftp_prefix)
 
-    with Publish("receiver", 0, ["HRPT 0", "PDS", "RDR", "EPS 0"]) as pub:
+    with Publish("receiver", port=publish_port,
+                 aliases=["HRPT 0", "PDS", "RDR", "EPS 0"],
+                 nameservers=nameservers) as pub:
         for rawmsg in sock.recv():
             # TODO:
             # - Watch for idle time in order to detect a hangout
-            LOGGER.debug("receive from 2met! %s", str(rawmsg))
+            logger.debug("receive from 2met! %s", str(rawmsg))
             string = TwoMetMessage(rawmsg)
             to_send = msg_rec.receive(string)
+            logger.debug("to_send: %s", str(to_send))
             if to_send is None:
                 continue
-            subject = "/".join(("", to_send['format'],
-                                to_send['data_processing_level'],
-                                station, environment,
-                                "polar", "direct_readout"))
+            if topic_postfix is not None:
+                subject = "/".join(("", to_send['format'],
+                                   to_send['data_processing_level'],
+                                   topic_postfix))
+            else:
+                subject = "/".join(("", to_send['format'],
+                                   to_send['data_processing_level'],
+                                   station, environment,
+                                   "polar", "direct_readout"))
+            logger.debug("Subject: %s", str(subject))
             msg = Message(subject,
                           "file",
                           to_send).encode()
-            LOGGER.debug("publishing %s", str(msg))
+            logger.debug("publishing %s", str(msg))
             pub.send(msg)
             if days:
                 msg_rec.clean_passes(days)
-
-
-if __name__ == '__main__':
-    rawmsg = '<message timestamp="2018-02-07T02:06:05" sequence="152" severity="INFO" messageID="0" type="2met.dispat.suctrn.info" sourcePU="MERLIN" sourceSU="Dispatch" sourceModule="DISPAT" sourceInstance="1"><body>SUCTRN RATMS-RNSCA_npp_d20180207_t0205166_e0205486_b00001_c20180207020559052000_all-_dev.h5 -&gt; 10.120.1.66:/tmp</body></message>'
-    rawmsg = '<message timestamp="2018-02-12T11:14:06" sequence="9194" severity="INFO" messageID="0" type="2met.dispat.suctrn.info" sourcePU="MERLIN" sourceSU="Dispatch" sourceModule="DISPAT" sourceInstance="1"><body>SUCTRN 20180212110043_NOAA_19.hmf -&gt; 192.168.122.1:/tmp</body></message>'
-
-    string = TwoMetMessage(rawmsg)
-    msg_rec = MessageReceiver('merlin')
-    ret = msg_rec.receive(string)
-    print(ret)
```

### Comparing `pytroll_collectors-0.8.4/pytroll_collectors/segments.py` & `pytroll_collectors-0.9.0/pytroll_collectors/segments.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,50 +16,49 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Gather GEO stationary segments, or polar satellite granules for one
-timestep, and send them in a bunch as a dataset.
+"""Gather segments.
+
+Gather GEO stationary segments, or polar satellite granules for one timestep,
+and send them in a bunch as a dataset.
 """
 
 import datetime as dt
 import logging
 import logging.handlers
-import os.path
-from six.moves.queue import Empty as queue_empty
-import time
+from six.moves.queue import Empty
 from collections import OrderedDict
-from six.moves.urllib.parse import urlparse, urlunparse
+from six.moves.urllib.parse import urlparse
 
 from posttroll import message, publisher
 from posttroll.listener import ListenerContainer
-from trollsift import Parser, compose
+from trollsift import Parser
 
 SLOT_NOT_READY = 0
 SLOT_NONCRITICAL_NOT_READY = 1
 SLOT_READY = 2
 SLOT_READY_BUT_WAIT_FOR_MORE = 3
 SLOT_OBSOLETE_TIMEOUT = 4
 
 DO_NOT_COPY_KEYS = ("uid", "uri", "channel_name", "segment", "sensor")
 REMOVE_TAGS = {'path', 'segment'}
 
 
 class SegmentGatherer(object):
-
-    """Gatherer for geostationary satellite segments and multifile polar
-    satellite granules."""
+    """Gatherer for geostationary satellite segments and multifile polar satellite granules."""
 
     _listener = None
     _publisher = None
 
     def __init__(self, config):
+        """Initialize the segment gatherer."""
         self._config = config
         self._subject = None
         self._patterns = config['patterns']
 
         self._time_tolerance = config.get("time_tolerance", 30)
         self._timeliness = dt.timedelta(seconds=config.get("timeliness", 1200))
 
@@ -68,25 +67,58 @@
 
         self.slots = OrderedDict()
 
         self._parsers = {key: Parser(self._patterns[key]['pattern']) for
                          key in self._patterns}
 
         self.time_name = config.get('time_name', 'start_time')
+        # Floor the scene start time to the given full minutes
+        self._group_by_minutes = config.get('group_by_minutes', None)
+
+        # This get the 'keep_parsed_keys' valid for all patterns
+        self._keep_parsed_keys = config.get('keep_parsed_keys', [])
 
         self.logger = logging.getLogger("segment_gatherer")
         self._loop = False
+        self._providing_server = config.get('providing_server')
+
+        # Convert check time into int minutes variables
+        for key in self._patterns:
+            if "start_time_pattern" in self._patterns[key]:
+                time_conf = self._patterns[key]["start_time_pattern"]
+                start_time_str = time_conf.get("start_time", "00:00")
+                end_time_str = time_conf.get("end_time", "23:59")
+                delta_time_str = time_conf.get("delta_time", "00:01")
+
+                start_h, start_m = start_time_str.split(':')
+                end_h, end_m = end_time_str.split(':')
+                delta_h, delta_m = delta_time_str.split(':')
+                interval = {}
+                interval["start"] = (60 * int(start_h)) + int(start_m)
+                interval["end"] = (60 * int(end_h)) + int(end_m)
+                interval["delta"] = (60 * int(delta_h)) + int(delta_m)
+
+                # Start-End time across midnight
+                interval["midnight"] = False
+                if interval["start"] > interval["end"]:
+                    interval["end"] += 24 * 60
+                    interval["midnight"] = True
+                self._patterns[key]["_start_time_pattern"] = interval
+                self.logger.info("Start Time pattern '%s' " +
+                                 "filter start:%s end:%s delta:%s",
+                                 key, start_time_str, end_time_str,
+                                 delta_time_str)
 
     def _clear_data(self, time_slot):
         """Clear data."""
         if time_slot in self.slots:
             del self.slots[time_slot]
 
     def _init_data(self, mda):
-        """Init wanted, all and critical files"""
+        """Init wanted, all and critical files."""
         # Init metadata struct
         metadata = mda.copy()
 
         time_slot = str(metadata[self.time_name])
         self.logger.debug("Adding new slot: %s", time_slot)
         self.slots[time_slot] = {}
         self.slots[time_slot]['metadata'] = metadata.copy()
@@ -141,16 +173,17 @@
             # Name of all the files
             all_segments = patterns[key].get("all_files", None)
             slot['all_files'].update(
                 self._compose_filenames(key, time_slot, all_segments))
 
     def _compose_filenames(self, key, time_slot, itm_str):
         """Compose filename set()s based on a pattern and item string.
-        itm_str is formated like ':PRO,:EPI' or 'VIS006:8,VIS008:1-8,...'"""
 
+        itm_str is formated like ':PRO,:EPI' or 'VIS006:8,VIS008:1-8,...'
+        """
         # Empty set
         result = set()
 
         # Handle missing itm_str
         if itm_str in (None, ''):
             itm_str = ':'
 
@@ -168,15 +201,15 @@
         for itm in itm_str.split(','):
             channel_name, segments = itm.split(':')
             if channel_name == '' and segments == '':
                 # If the filename pattern has no segments/channels,
                 # add the "plain" globified filename to the filename
                 # set
                 if ('channel_name' not in parser.fmt and
-                    'segment' not in parser.fmt):
+                        'segment' not in parser.fmt):
                     result.add(parser.globify(meta))
                 continue
             segments = segments.split('-')
             if len(segments) > 1:
                 format_string = '%d'
                 if len(segments[0]) > 1 and segments[0][0] == '0':
                     format_string = '%0' + str(len(segments[0])) + 'd'
@@ -190,15 +223,14 @@
 
                 result.add(fname)
 
         return result
 
     def _publish(self, time_slot, missing_files_check=True):
         """Publish file dataset and reinitialize gatherer."""
-
         data = self.slots[time_slot]
 
         # Diagnostic logging about delayed ...
         delayed_files = {}
         for key in self._parsers:
             delayed_files.update(data[key]['delayed_files'])
         if len(delayed_files) > 0:
@@ -235,14 +267,15 @@
         # self._clear_data(time_slot)
 
     def set_logger(self, logger):
         """Set logger."""
         self.logger = logger
 
     def update_timeout(self, time_slot):
+        """Update the timeout."""
         timeout = dt.datetime.utcnow() + self._timeliness
         self.slots[time_slot]['timeout'] = timeout
         self.logger.info("Setting timeout to %s for slot %s.",
                          str(timeout), time_slot)
 
     def slot_ready(self, time_slot):
         """Determine if slot is ready to be published."""
@@ -276,20 +309,19 @@
                     slot[key]['received_files']):
                 status[key] = SLOT_READY
 
         # Determine overall status
         return self.get_collection_status(status, slot['timeout'], time_slot)
 
     def get_collection_status(self, status, timeout, time_slot):
-        """Determine the overall status of the collection"""
+        """Determine the overall status of the collection."""
         if len(status) == 0:
             return SLOT_NOT_READY
 
         status_values = list(status.values())
-
         if all([val == SLOT_READY for val in status_values]):
             self.logger.info("Required files received "
                              "for slot %s.", time_slot)
             return SLOT_READY
 
         if dt.datetime.utcnow() > timeout:
             if (SLOT_NONCRITICAL_NOT_READY in status_values and
@@ -315,29 +347,39 @@
         if SLOT_NOT_READY in status_values:
             return SLOT_NOT_READY
         if SLOT_NONCRITICAL_NOT_READY in status_values:
             return SLOT_NONCRITICAL_NOT_READY
         if SLOT_READY_BUT_WAIT_FOR_MORE in status_values:
             return SLOT_READY_BUT_WAIT_FOR_MORE
 
+    def _generate_publish_service_name(self):
+        publish_service_name = "segment_gatherer"
+        for key in sorted(self._patterns):
+            publish_service_name += "_" + str(key)
+        return publish_service_name
+
     def _setup_messaging(self):
-        """Setup messaging"""
+        """Set up messaging."""
         self._subject = self._config['posttroll']['publish_topic']
         topics = self._config['posttroll'].get('topics')
         addresses = self._config['posttroll'].get('addresses')
         publish_port = self._config['posttroll'].get('publish_port', 0)
         nameservers = self._config['posttroll'].get('nameservers', [])
-        self._listener = ListenerContainer(topics=topics, addresses=addresses)
-        self._publisher = publisher.NoisyPublisher("segment_gatherer",
+        services = self._config['posttroll'].get('services')
+        self._listener = ListenerContainer(topics=topics, addresses=addresses, services=services)
+        # Name each segment_gatherer with the section/patterns name.
+        # This way the user can subscribe to a specific segment_gatherer service instead of all.
+        publish_service_name = self._generate_publish_service_name()
+        self._publisher = publisher.NoisyPublisher(publish_service_name,
                                                    port=publish_port,
                                                    nameservers=nameservers)
         self._publisher.start()
 
     def run(self):
-        """Run SegmentGatherer"""
+        """Run SegmentGatherer."""
         self._setup_messaging()
 
         self._loop = True
         while self._loop:
             # Check if there are slots ready for publication
             slots = self.slots.copy()
             for slot in slots:
@@ -362,33 +404,36 @@
             try:
                 msg = self._listener.output_queue.get(True, 1)
             except AttributeError:
                 msg = self._listener.queue.get(True, 1)
             except KeyboardInterrupt:
                 self.stop()
                 continue
-            except queue_empty:
+            except Empty:
                 continue
 
             if msg.type == "file":
+                # If providing server is configured skip message if not from providing server
+                if self._providing_server and self._providing_server != msg.host:
+                    continue
                 self.logger.info("New message received: %s", str(msg))
                 self.process(msg)
 
     def stop(self):
         """Stop gatherer."""
         self.logger.info("Stopping gatherer.")
         self._loop = False
         if self._listener is not None:
             if self._listener.thread is not None:
                 self._listener.stop()
         if self._publisher is not None:
             self._publisher.stop()
 
     def process(self, msg):
-        """Process message"""
+        """Process message."""
         mda = None
 
         try:
             uid = msg.data['uid']
         except KeyError:
             self.logger.debug("Ignoring: %s", str(msg))
             return
@@ -397,28 +442,66 @@
         key = self.key_from_fname(uid)
         if key is None:
             self.logger.debug("Unknown file, skipping.")
             return
 
         parser = self._parsers[key]
         mda = parser.parse(msg.data["uid"])
+        mda = self._floor_time(mda, key)
 
-        metadata = copy_metadata(mda, msg)
+        # Check if each pattern contains a seperate 'keep_parsed_keys'
+        local_keep_parsed_keys = self._patterns[key].get('keep_parsed_keys', [])
+        metadata = copy_metadata(mda, msg,
+                                 keep_parsed_keys=self._keep_parsed_keys,
+                                 local_keep_parsed_keys=local_keep_parsed_keys)
+
+        # Check if time of the raw is in scheduled range
+        if "_start_time_pattern" in self._patterns[key]:
+            schedule_ok = self.check_schedule_time(
+                self._patterns[key]["_start_time_pattern"],
+                metadata[self.time_name])
+            if not schedule_ok:
+                self.logger.info("Hour pattern '%s' skip: %s" +
+                                 " for start_time: %s:%s",
+                                 key, msg.data["uid"],
+                                 metadata[self.time_name].hour,
+                                 metadata[self.time_name].minute)
+                return
 
-        time_slot = self._find_time_slot(metadata["start_time"])
+        time_slot = self._find_time_slot(metadata[self.time_name])
 
         # Init metadata etc if this is the first file
         if time_slot not in self.slots:
             self._init_data(metadata)
 
         # Check if this file has been received already
         self.add_file(time_slot, key, mda, msg.data)
 
+    def _floor_time(self, mda, key=None):
+        """Floor time to full minutes."""
+        # This is the 'group_by_minutes' for all patterns
+        group_by_minutes = self._group_by_minutes
+
+        # Check if 'group_by_minutes' is given in the \key\ pattern
+        if key is not None and 'group_by_minutes' in self._patterns[key]:
+            group_by_minutes = self._patterns[key]['group_by_minutes']
+        elif self._group_by_minutes is None:
+            return mda
+
+        start_time = mda[self.time_name]
+        mins = start_time.minute
+        fl_mins = int(mins / group_by_minutes) * group_by_minutes
+        start_time = dt.datetime(start_time.year, start_time.month,
+                                 start_time.day, start_time.hour, fl_mins, 0)
+        mda[self.time_name] = start_time
+
+        return mda
+
     def add_file(self, time_slot, key, mda, msg_data):
-        """Add file to the correct filelist"""
+        """Add file to the correct filelist."""
         uri = urlparse(msg_data['uri']).path
         uid = msg_data['uid']
         slot = self.slots[time_slot][key]
         meta = self.slots[time_slot]['metadata']
 
         # Replace variable tags (such as processing time) with
         # wildcards, as these can't be forecasted.
@@ -465,40 +548,56 @@
                 slot['delayed_files'][uid] = delay.total_seconds()
 
         # Add to received files
         slot['received_files'].add(mask)
         self.logger.info("%s processed", uid)
 
     def key_from_fname(self, uid):
-        """"""
+        """Get the keys from a filename."""
         for key in self._parsers:
             try:
                 _ = self._parsers[key].parse(uid)
                 return key
             except ValueError:
                 pass
 
     def _find_time_slot(self, time_obj):
-        """Find time slot and return the slot as a string.  If no slots are
-        close enough, return *str(time_obj)*"""
+        """Find time slot and return the slot as a string.
+
+        If no slots are close enough, return *str(time_obj)*
+        """
         for slot in self.slots:
             time_slot = self.slots[slot]['metadata'][self.time_name]
             time_diff = time_obj - time_slot
             if abs(time_diff.total_seconds()) < self._time_tolerance:
                 self.logger.debug("Found existing time slot, using that")
                 return str(time_slot)
 
         return str(time_obj)
 
+    def check_schedule_time(self, check_time, raw_start_time):
+        """Check if raw time is inside configured interval."""
+        time_ok = False
+
+        # Convert check time into int variables
+        raw_time = (60 * raw_start_time.hour) + raw_start_time.minute
+        if check_time["midnight"] and raw_time < check_time["start"]:
+            raw_time += 24 * 60
+
+        # Check start and end time
+        if raw_time >= check_time["start"] and raw_time <= check_time["end"]:
+            # Raw time in range, check interval
+            if ((raw_time - check_time["start"]) % check_time["delta"]) == 0:
+                time_ok = True
+
+        return time_ok
+
 
 def _copy_without_ignore_items(the_dict, ignored_keys='ignore'):
-    """
-    get a copy of *the_dict* without entries having substring
-    'ignore' in key
-    """
+    """Get a copy of *the_dict* without entries having substring 'ignore' in key."""
     if not isinstance(ignored_keys, (list, tuple, set)):
         ignored_keys = [ignored_keys, ]
     new_dict = {}
     for (key, val) in list(the_dict.items()):
         if key not in ignored_keys:
             new_dict[key] = val
     return new_dict
@@ -512,28 +611,35 @@
     config.read(fname)
 
     conf = {}
     conf['posttroll'] = {}
     posttroll = conf['posttroll']
     posttroll['topics'] = config.get(section, 'topics').split()
     try:
-        nameservers = config.get(section, 'nameserver')
+        nameservers = config.get(section, 'nameservers')
         nameservers = nameservers.split()
     except (NoOptionError, ValueError):
         nameservers = None
     posttroll['nameservers'] = nameservers
 
     try:
         addresses = config.get(section, 'addresses')
         addresses = addresses.split()
     except (NoOptionError, ValueError):
         addresses = None
     posttroll['addresses'] = addresses
 
     try:
+        services = config.get(section, 'services')
+        services = services.split()
+    except (NoOptionError, ValueError):
+        services = ""
+    posttroll['services'] = services
+
+    try:
         publish_port = config.get(section, 'publish_port')
     except NoOptionError:
         publish_port = 0
     posttroll['publish_port'] = publish_port
 
     posttroll['publish_topic'] = config.get(section, "publish_topic")
 
@@ -562,24 +668,45 @@
 
     try:
         conf['num_files_premature_publish'] = \
             config.getint(section, "num_files_premature_publish")
     except (NoOptionError, ValueError):
         conf['num_files_premature_publish'] = -1
 
+    try:
+        conf['group_by_minutes'] = config.getint(section, 'group_by_minutes')
+    except (NoOptionError, ValueError):
+        pass
+
+    try:
+        kps = config.get(section, 'keep_parsed_keys')
+        conf['keep_parsed_keys'] = kps.split()
+    except NoOptionError:
+        pass
+
+    try:
+        conf['providing_server'] = config.get(section, "providing_server")
+    except (NoOptionError, ValueError):
+        conf['providing_server'] = None
+
     return conf
 
 
-def copy_metadata(mda, msg):
-    """Copy metada from filename and message to a combined dictionary"""
+def copy_metadata(mda, msg, keep_parsed_keys=None, local_keep_parsed_keys=None):
+    """Copy metada from filename and message to a combined dictionary."""
+    if keep_parsed_keys is None:
+        keep_parsed_keys = []
+    if local_keep_parsed_keys is None:
+        local_keep_parsed_keys = []
     metadata = {}
     # Use values parsed from the filename as basis
     for key in mda:
         if key not in DO_NOT_COPY_KEYS:
             metadata[key] = mda[key]
 
     # Update with data given in the message
     for key in msg.data:
-        if key not in DO_NOT_COPY_KEYS:
+        # If time name is given, do not overwrite it
+        if key not in DO_NOT_COPY_KEYS and key not in keep_parsed_keys and key not in local_keep_parsed_keys:
             metadata[key] = msg.data[key]
 
     return metadata
```

### Comparing `pytroll_collectors-0.8.4/pytroll_collectors/tests/__init__.py` & `pytroll_collectors-0.9.0/pytroll_collectors/tests/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,35 +16,29 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""The tests package.
-"""
+"""The tests package."""
 
 import unittest
 # import doctest
 from pytroll_collectors.tests import (test_helper_functions,
                                       test_scisys,
                                       test_trigger,
-                                      test_global_mosaic,
-                                      test_image_scaler,
                                       test_segments)
 
 
 def suite():
-    """The global test suite.
-    """
+    """Test suite."""
     mysuite = unittest.TestSuite()
     # Test the documentation strings
     # mysuite.addTests(doctest.DocTestSuite(image))
     # Use the unittests also
     mysuite.addTests(test_helper_functions.suite())
     mysuite.addTests(test_scisys.suite())
     mysuite.addTests(test_trigger.suite())
-    mysuite.addTests(test_global_mosaic.suite())
-    mysuite.addTests(test_image_scaler.suite())
     mysuite.addTests(test_segments.suite())
 
     return mysuite
```

### Comparing `pytroll_collectors-0.8.4/pytroll_collectors/tests/test_helper_functions.py` & `pytroll_collectors-0.9.0/pytroll_collectors/tests/test_helper_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,32 +16,27 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit testing some general purpose helper functions
-"""
+"""Unit testing some general purpose helper functions."""
 
 import unittest
 from datetime import datetime
 
 from pytroll_collectors.helper_functions import create_aligned_datetime_var
 
 
 class TestTimeUtilities(unittest.TestCase):
-
-    def setUp(self):
-        """Setting up the testing
-        """
-        pass
+    """Time utilities."""
 
     def test_create_aligned_datetime_var(self):
-        """Test the create_aligned_datetime_var function"""
+        """Test the create_aligned_datetime_var function."""
         # Run
         filepattern = "{start_time:%Y%m%d%H%M%S|align(5)}"
         result = create_aligned_datetime_var(filepattern,
                                              {'start_time':
                                               datetime(2015, 1, 9, 17, 10, 48)})
         # Assert
         self.assertEqual(result, datetime(2015, 1, 9, 17, 10, 0))
@@ -66,15 +61,15 @@
         result = create_aligned_datetime_var(filepattern,
                                              {'start_time':
                                               datetime(2015, 1, 9, 16, 59, 0)})
         # Assert
         self.assertEqual(result, datetime(2015, 1, 9, 16, 45, 0))
 
     def test_create_aligned_datetime_var_offsets(self):
-        """Test the create_aligned_datetime_var function"""
+        """Test the create_aligned_datetime_var function."""
         # Run
         filepattern = "{start_time:%Y%m%d%H%M%S|align(15,-2)}"
         result = create_aligned_datetime_var(filepattern,
                                              {'start_time':
                                               datetime(2015, 1, 9, 16, 59, 0)})
         # Assert
         self.assertEqual(result, datetime(2015, 1, 9, 17, 0, 0))
@@ -83,15 +78,15 @@
         result = create_aligned_datetime_var(filepattern,
                                              {'start_time':
                                               datetime(2015, 1, 9, 17, 16, 0)})
         # Assert
         self.assertEqual(result, datetime(2015, 1, 9, 17, 0, 0))
 
     def test_parse_time_with_timeslot_aligment_intervals_add(self):
-        """Test the create_aligned_datetime_var function"""
+        """Test the create_aligned_datetime_var function."""
         # Run
         filepattern = "{start_time:%Y%m%d%H%M%S|align(15,0,1)}"
         result = create_aligned_datetime_var(filepattern,
                                              {'start_time':
                                               datetime(2015, 1, 9, 16, 59, 0)})
         # Assert
         self.assertEqual(result, datetime(2015, 1, 9, 17, 0, 0))
@@ -108,24 +103,19 @@
         filepattern = "{start_time:%Y%m%d%H%M%S|align(15,0,-1)}"
         result = create_aligned_datetime_var(filepattern,
                                              {'start_time':
                                               datetime(2015, 1, 9, 16, 59, 0)})
         # Assert
         self.assertEqual(result, datetime(2015, 1, 9, 16, 30, 0))
 
-    def tearDown(self):
-        """Closing down
-        """
-        pass
-
 
 def suite():
-    """The suite for test_trollduction
-    """
+    """Test suite."""
     loader = unittest.TestLoader()
     mysuite = unittest.TestSuite()
     mysuite.addTest(loader.loadTestsFromTestCase(TestTimeUtilities))
 
     return mysuite
 
+
 if __name__ == "__main__":
     unittest.TextTestRunner(verbosity=2).run(suite())
```

### Comparing `pytroll_collectors-0.8.4/pytroll_collectors/tests/test_scisys.py` & `pytroll_collectors-0.9.0/pytroll_collectors/tests/test_scisys.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,127 +16,124 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Test suite for the scisys receiver.
-"""
+"""Test suite for the scisys receiver."""
 
 
 # Test cases.
 
 import datetime
 import os
-import socket
 import unittest
 
 from pytroll_collectors.scisys import MessageReceiver, TwoMetMessage
 
-if os.environ.get('TRAVIS', False) == 'true':
-    # gethostbyname doesn't work on travis nodes
-    hostname = 'localhost'
-else:
-    hostname = socket.gethostname()
+hostname = 'localhost'
 
-input_stoprc = '<message timestamp="2013-02-18T09:21:35" sequence="7482" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="POESAcquisition" sourceModule="POES" sourceInstance="1"><body>STOPRC Stop reception: Satellite: NPP, Orbit number: 6796, Risetime: 2013-02-18 09:08:09, Falltime: 2013-02-18 09:21:33</body></message>'
+input_stoprc = '<message timestamp="2013-02-18T09:21:35" sequence="7482" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="POESAcquisition" sourceModule="POES" sourceInstance="1"><body>STOPRC Stop reception: Satellite: NPP, Orbit number: 6796, Risetime: 2013-02-18 09:08:09, Falltime: 2013-02-18 09:21:33</body></message>'  # noqa
 
-input_dispatch_viirs = '<message timestamp="2013-02-18T09:24:20" sequence="27098" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/npp/RNSCA-RVIRS_npp_d20130218_t0908103_e0921256_b00001_c20130218092411165000_nfts_drl.h5 ftp://{hostname}:21/tmp/RNSCA-RVIRS_npp_d20130218_t0908103_e0921256_b00001_c20130218092411165000_nfts_drl.h5</body></message>'.format(
+input_dispatch_viirs = '<message timestamp="2013-02-18T09:24:20" sequence="27098" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/npp/RNSCA-RVIRS_npp_d20130218_t0908103_e0921256_b00001_c20130218092411165000_nfts_drl.h5 ftp://{hostname}:21/tmp/RNSCA-RVIRS_npp_d20130218_t0908103_e0921256_b00001_c20130218092411165000_nfts_drl.h5</body></message>'.format(  # noqa
     hostname=hostname)
 
-input_dispatch_atms = '<message timestamp="2013-02-18T09:24:21" sequence="27100" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/npp/RATMS-RNSCA_npp_d20130218_t0908194_e0921055_b00001_c20130218092411244000_nfts_drl.h5 ftp://{hostname}:21/tmp/RATMS-RNSCA_npp_d20130218_t0908194_e0921055_b00001_c20130218092411244000_nfts_drl.h5</body></message>'.format(
+input_dispatch_atms = '<message timestamp="2013-02-18T09:24:21" sequence="27100" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/npp/RATMS-RNSCA_npp_d20130218_t0908194_e0921055_b00001_c20130218092411244000_nfts_drl.h5 ftp://{hostname}:21/tmp/RATMS-RNSCA_npp_d20130218_t0908194_e0921055_b00001_c20130218092411244000_nfts_drl.h5</body></message>'.format(  # noqa
     hostname=hostname)
 
 viirs = {'platform_name': 'Suomi-NPP', 'format': 'RDR',
          'start_time': datetime.datetime(2013, 2, 18, 9, 8, 10, 300000),
          'data_processing_level': '0', 'orbit_number': 6796,
-         'uri': 'ssh://{hostname}/tmp/RNSCA-RVIRS_npp_d20130218_t0908103_e0921256_b00001_c20130218092411165000_nfts_drl.h5'.format(hostname=hostname),
+         'uri': 'ssh://{hostname}/tmp/RNSCA-RVIRS_npp_d20130218_t0908103_e0921256_b00001_c20130218092411165000_nfts_drl.h5'.format(hostname=hostname),  # noqa
          'uid': 'RNSCA-RVIRS_npp_d20130218_t0908103_e0921256_b00001_c20130218092411165000_nfts_drl.h5',
          'sensor': 'viirs',
          'end_time': datetime.datetime(2013, 2, 18, 9, 21, 25, 600000),
          'type': 'HDF5', 'variant': 'DR'}
 
 atms = {'platform_name': 'Suomi-NPP', 'format': 'RDR', 'start_time':
         datetime.datetime(2013, 2, 18, 9, 8, 19, 400000),
         'data_processing_level': '0', 'orbit_number': 6796, 'uri':
-        'ssh://{hostname}/tmp/RATMS-RNSCA_npp_d20130218_t0908194_e0921055_b00001_c20130218092411244000_nfts_drl.h5'.format(
+        'ssh://{hostname}/tmp/RATMS-RNSCA_npp_d20130218_t0908194_e0921055_b00001_c20130218092411244000_nfts_drl.h5'.format(  # noqa
             hostname=hostname),
         'uid':
         'RATMS-RNSCA_npp_d20130218_t0908194_e0921055_b00001_c20130218092411244000_nfts_drl.h5',
         'sensor': 'atms',
         'end_time': datetime.datetime(2013, 2, 18, 9, 21, 5, 500000),
         'type': 'HDF5', 'variant': 'DR'}
 
-stoprc_terra = '<message timestamp="2014-10-30T21:03:50" sequence="6153" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="POESAcquisition" sourceModule="POES" sourceInstance="1"><body>STOPRC Stop reception: Satellite: TERRA, Orbit number: 79082, Risetime: 2014-10-30 20:49:50, Falltime: 2014-10-30 21:03:50</body></message>'
+stoprc_terra = '<message timestamp="2014-10-30T21:03:50" sequence="6153" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="POESAcquisition" sourceModule="POES" sourceInstance="1"><body>STOPRC Stop reception: Satellite: TERRA, Orbit number: 79082, Risetime: 2014-10-30 20:49:50, Falltime: 2014-10-30 21:03:50</body></message>'  # noqa
 
-fildis_terra = '<message timestamp="2014-10-30T21:03:57" sequence="213208" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/modis/P0420064AAAAAAAAAAAAAA14303204950001.PDS ftp://{hostname}:21/tmp/P0420064AAAAAAAAAAAAAA14303204950001.PDS</body></message>'.format(
+fildis_terra = '<message timestamp="2014-10-30T21:03:57" sequence="213208" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/modis/P0420064AAAAAAAAAAAAAA14303204950001.PDS ftp://{hostname}:21/tmp/P0420064AAAAAAAAAAAAAA14303204950001.PDS</body></message>'.format(  # noqa
     hostname=hostname)
 
 msg_terra = {"platform_name": "EOS-Terra", "uri":
              "ssh://{hostname}/tmp/P0420064AAAAAAAAAAAAAA14303204950001.PDS".format(hostname=hostname), "format": "PDS",
              "start_time": datetime.datetime(2014, 10, 30, 20, 49, 50),
              "data_processing_level": "0", "orbit_number": 79082, "uid":
              "P0420064AAAAAAAAAAAAAA14303204950001.PDS",
              "sensor": "modis",
              "end_time": datetime.datetime(2014, 10, 30, 21, 3, 50),
              "type": "binary", 'variant': 'DR'}
 
-stoprc_n19 = '<message timestamp="2014-10-28T07:25:37" sequence="472" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="HRPTAcquisition" sourceModule="FSSRVC" sourceInstance="1"><body>STOPRC Stop reception: Satellite: NOAA 19, Orbit number: 29477, Risetime: 2014-10-28 07:16:01, Falltime: 2014-10-28 07:25:37</body></message>'
+stoprc_n19 = '<message timestamp="2014-10-28T07:25:37" sequence="472" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="HRPTAcquisition" sourceModule="FSSRVC" sourceInstance="1"><body>STOPRC Stop reception: Satellite: NOAA 19, Orbit number: 29477, Risetime: 2014-10-28 07:16:01, Falltime: 2014-10-28 07:25:37</body></message>'  # noqa
 
-fildis_n19 = '<message timestamp="2014-10-28T07:25:43" sequence="203257" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/hrpt/20141028071601_NOAA_19.hmf ftp://{hostname}:21/tmp/20141028071601_NOAA_19.hmf</body></message>'.format(
+fildis_n19 = '<message timestamp="2014-10-28T07:25:43" sequence="203257" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/hrpt/20141028071601_NOAA_19.hmf ftp://{hostname}:21/tmp/20141028071601_NOAA_19.hmf</body></message>'.format(  # noqa
     hostname=hostname)
 
 msg_n19 = {"platform_name": "NOAA-19", "format": "HRPT",
            "start_time": datetime.datetime(2014, 10, 28, 7, 16, 1),
            "data_processing_level": "0", "orbit_number": 29477,
            "uri": "ssh://{hostname}/tmp/20141028071601_NOAA_19.hmf".format(hostname=hostname),
            "uid": "20141028071601_NOAA_19.hmf",
            "sensor": ("avhrr/3", "mhs", "amsu-a", "hirs/4"),
            "end_time": datetime.datetime(2014, 10, 28, 7, 25, 37),
            "type": "binary", 'variant': 'DR'}
 
-stoprc_m01 = '<message timestamp="2014-10-28T08:45:22" sequence="1157" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="HRPTAcquisition" sourceModule="FSSRVC" sourceInstance="1"><body>STOPRC Stop reception: Satellite: METOP-B, Orbit number: 10948, Risetime: 2014-10-28 08:30:10, Falltime: 2014-10-28 08:45:22</body></message>'
+stoprc_m01 = '<message timestamp="2014-10-28T08:45:22" sequence="1157" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="HRPTAcquisition" sourceModule="FSSRVC" sourceInstance="1"><body>STOPRC Stop reception: Satellite: METOP-B, Orbit number: 10948, Risetime: 2014-10-28 08:30:10, Falltime: 2014-10-28 08:45:22</body></message>'  # noqa
 
-fildis_m01 = '<message timestamp="2014-10-28T08:45:27" sequence="203535" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/metop/MHSx_HRP_00_M01_20141028083003Z_20141028084510Z_N_O_20141028083010Z ftp://{hostname}:21/tmp/MHSx_HRP_00_M01_20141028083003Z_20141028084510Z_N_O_20141028083010Z</body></message>'.format(
+fildis_m01 = '<message timestamp="2014-10-28T08:45:27" sequence="203535" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/metop/MHSx_HRP_00_M01_20141028083003Z_20141028084510Z_N_O_20141028083010Z ftp://{hostname}:21/tmp/MHSx_HRP_00_M01_20141028083003Z_20141028084510Z_N_O_20141028083010Z</body></message>'.format( # noqa
     hostname=hostname)
 
 msg_m01 = {"platform_name": "Metop-B", "format": "EPS",
            "start_time": datetime.datetime(2014, 10, 28, 8, 30, 3),
            "data_processing_level": "0", "orbit_number": 10948,
-           "uri": "ssh://{hostname}/tmp/MHSx_HRP_00_M01_20141028083003Z_20141028084510Z_N_O_20141028083010Z".format(hostname=hostname),
+           "uri": "ssh://{hostname}/tmp/MHSx_HRP_00_M01_20141028083003Z_20141028084510Z_N_O_20141028083010Z".format(hostname=hostname),  # noqa
            "uid": "MHSx_HRP_00_M01_20141028083003Z_20141028084510Z_N_O_20141028083010Z",
            "sensor": "mhs",
            "end_time": datetime.datetime(2014, 10, 28, 8, 45, 10),
            "type": "binary", 'variant': 'DR'}
 
-startrc_npp2 = '<message timestamp="2014-10-31T08:53:52" sequence="9096" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="POESAcquisition" sourceModule="POES" sourceInstance="1"><body>STRTRC Start reception: Satellite: NPP, Orbit number: 15591, Risetime: 2014-10-31 08:53:52, Falltime: 2014-10-31 09:06:28</body></message>'
+startrc_npp2 = '<message timestamp="2014-10-31T08:53:52" sequence="9096" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="POESAcquisition" sourceModule="POES" sourceInstance="1"><body>STRTRC Start reception: Satellite: NPP, Orbit number: 15591, Risetime: 2014-10-31 08:53:52, Falltime: 2014-10-31 09:06:28</body></message>'  # noqa
 
-stoprc_npp2 = '<message timestamp="2014-10-31T09:06:28" sequence="9340" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="POESAcquisition" sourceModule="POES" sourceInstance="1"><body>STOPRC Stop reception: Satellite: NPP, Orbit number: 15591, Risetime: 2014-10-31 08:53:52, Falltime: 2014-10-31 09:06:28</body></message>'
+stoprc_npp2 = '<message timestamp="2014-10-31T09:06:28" sequence="9340" severity="INFO" messageID="0" type="2met.message" sourcePU="SMHI-Linux" sourceSU="POESAcquisition" sourceModule="POES" sourceInstance="1"><body>STOPRC Stop reception: Satellite: NPP, Orbit number: 15591, Risetime: 2014-10-31 08:53:52, Falltime: 2014-10-31 09:06:28</body></message>'  # noqa
 
-fildis_npp2 = '<message timestamp="2014-10-31T09:06:25" sequence="216010" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/npp/RCRIS-RNSCA_npp_d20141031_t0905166_e0905484_b00001_c20141031090623200000_nfts_drl.h5 ftp://{hostname}:21//tmp</body></message>'.format(
+fildis_npp2 = '<message timestamp="2014-10-31T09:06:25" sequence="216010" severity="INFO" messageID="8250" type="2met.filehandler.sink.success" sourcePU="SMHI-Linux" sourceSU="GMCSERVER" sourceModule="GMCSERVER" sourceInstance="1"><body>FILDIS File Dispatch: /data/npp/RCRIS-RNSCA_npp_d20141031_t0905166_e0905484_b00001_c20141031090623200000_nfts_drl.h5 ftp://{hostname}:21//tmp</body></message>'.format(  # noqa
     hostname=hostname)
 
 msg_npp2 = {"orbit_number": 15591,
             "uid": "RCRIS-RNSCA_npp_d20141031_t0905166_e0905484_b00001_c20141031090623200000_nfts_drl.h5",
             "format": "RDR", "sensor": "cris",
             "start_time": datetime.datetime(2014, 10, 31, 9, 5, 16, 600000),
-            "uri": "ssh://{hostname}//tmp/RCRIS-RNSCA_npp_d20141031_t0905166_e0905484_b00001_c20141031090623200000_nfts_drl.h5".format(hostname=hostname),
+            "uri": "ssh://{hostname}//tmp/RCRIS-RNSCA_npp_d20141031_t0905166_e0905484_b00001_c20141031090623200000_nfts_drl.h5".format(hostname=hostname),  # noqa
             "platform_name": "Suomi-NPP",
             "end_time": datetime.datetime(2014, 10, 31, 9, 5, 48, 400000),
             "type": "HDF5", "data_processing_level": "0", 'variant': 'DR'}
 
 
 def touch(fname):
+    """Create an empty file."""
     open(fname, 'a').close()
 
 
 class ScisysReceiverTest(unittest.TestCase):
+    """Testing the Scisys receiver."""
 
     def test_reception(self):
+        """Test the reception."""
         msg_rec = MessageReceiver("nimbus")
 
         # NPP
 
         string = TwoMetMessage(input_stoprc)
         to_send = msg_rec.receive(string)
         self.assertTrue(to_send is None)
@@ -216,16 +213,15 @@
         string = TwoMetMessage(fildis_m01)
         to_send = msg_rec.receive(string)
         self.assertDictEqual(to_send, msg_m01)
         os.remove(filename)
 
 
 def suite():
-    """The suite for test_scisys
-    """
+    """Test suite for test_scisys."""
     loader = unittest.TestLoader()
     mysuite = unittest.TestSuite()
     mysuite.addTest(loader.loadTestsFromTestCase(ScisysReceiverTest))
 
     return mysuite
```

### Comparing `pytroll_collectors-0.8.4/pytroll_collectors/tests/test_segments.py` & `pytroll_collectors-0.9.0/pytroll_collectors/tests/test_segments.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit testing for segment gatherer
-"""
+"""Unit testing for segment gatherer."""
 
 import unittest
 import datetime as dt
 import os
 import os.path
 import logging
 
@@ -38,37 +37,40 @@
                                          SLOT_READY_BUT_WAIT_FOR_MORE,
                                          SLOT_OBSOLETE_TIMEOUT)
 
 
 THIS_DIR = os.path.dirname(os.path.abspath(__file__))
 CONFIG_SINGLE = read_yaml(os.path.join(THIS_DIR, "data/segments_single.yaml"))
 CONFIG_DOUBLE = read_yaml(os.path.join(THIS_DIR, "data/segments_double.yaml"))
+CONFIG_DOUBLE_DIFFERENT = read_yaml(os.path.join(THIS_DIR, "data/segments_double_different.yaml"))
 CONFIG_NO_SEG = read_yaml(os.path.join(THIS_DIR,
                                        "data/segments_double_no_segments.yaml"))
 CONFIG_INI = ini_to_dict(os.path.join(THIS_DIR, "data/segments.ini"), "msg")
 CONFIG_INI_NO_SEG = ini_to_dict(os.path.join(THIS_DIR, "data/segments.ini"),
                                 "goes16")
+CONFIG_INI_HIMAWARI = ini_to_dict(os.path.join(THIS_DIR, "data/segments.ini"),
+                                  "himawari-8")
 
 
 class TestSegmentGatherer(unittest.TestCase):
+    """Tests for the segment gatherer."""
 
     def setUp(self):
-        """Setting up the testing
-        """
-        self.mda_msg0deg = {"segment": "EPI", "uid": "H-000-MSG3__-MSG3________-_________-EPI______-201611281100-__", "platform_shortname": "MSG3", "start_time": dt.datetime(2016, 11, 28, 11, 0, 0), "nominal_time": dt.datetime(
-            2016, 11, 28, 11, 0, 0), "uri": "/home/lahtinep/data/satellite/geo/msg/H-000-MSG3__-MSG3________-_________-EPI______-201611281100-__", "platform_name": "Meteosat-10", "channel_name": "", "path": "", "sensor": ["seviri"], "hrit_format": "MSG3"}
+        """Set up the testing."""
+        self.mda_msg0deg = {"segment": "EPI", "uid": "H-000-MSG3__-MSG3________-_________-EPI______-201611281100-__", "platform_shortname": "MSG3", "start_time": dt.datetime(2016, 11, 28, 11, 0, 0), "nominal_time": dt.datetime(  # noqa
+            2016, 11, 28, 11, 0, 0), "uri": "/home/lahtinep/data/satellite/geo/msg/H-000-MSG3__-MSG3________-_________-EPI______-201611281100-__", "platform_name": "Meteosat-10", "channel_name": "", "path": "", "sensor": ["seviri"], "hrit_format": "MSG3"}  # noqa
 
-        self.mda_iodc = {"segment": "EPI", "uid": "H-000-MSG2__-MSG2_IODC___-_________-EPI______-201611281100-__", "platform_shortname": "MSG2", "start_time": dt.datetime(2016, 11, 28, 11, 0, 0), "nominal_time": dt.datetime(
-            2016, 11, 28, 11, 0, 0), "uri": "/home/lahtinep/data/satellite/geo/msg/H-000-MSG2__-MSG2_IODC___-_________-EPI______-201611281100-__", "platform_name": "Meteosat-9", "channel_name": "", "path": "", "sensor": ["seviri"]}
+        self.mda_iodc = {"segment": "EPI", "uid": "H-000-MSG2__-MSG2_IODC___-_________-EPI______-201611281100-__", "platform_shortname": "MSG2", "start_time": dt.datetime(2016, 11, 28, 11, 0, 0), "nominal_time": dt.datetime(  # noqa
+            2016, 11, 28, 11, 0, 0), "uri": "/home/lahtinep/data/satellite/geo/msg/H-000-MSG2__-MSG2_IODC___-_________-EPI______-201611281100-__", "platform_name": "Meteosat-9", "channel_name": "", "path": "", "sensor": ["seviri"]}  # noqa
 
-        self.mda_pps = {"end_tenths": 4, "uid": "S_NWC_CMA_metopb_28538_20180319T0955387Z_20180319T1009544Z.nc", "platform_shortname": "metopb", "start_time": dt.datetime(2018, 3, 19, 9, 55, 0), "start_tenths": 7, "orbit_number": 28538, "uri":
-                        "/home/lahtinep/data/satellite/hrpt-pps/S_NWC_CMA_metopb_28538_20180319T0955387Z_20180319T1009544Z.nc", "start_seconds": 38, "platform_name": "Metop-B", "end_seconds": 54, "end_time": dt.datetime(2018, 3, 19, 10, 9, 0), "path": "", "sensor": ["avhrr/3"]}
+        self.mda_pps = {"end_tenths": 4, "uid": "S_NWC_CMA_metopb_28538_20180319T0955387Z_20180319T1009544Z.nc", "platform_shortname": "metopb", "start_time": dt.datetime(2018, 3, 19, 9, 55, 0), "start_tenths": 7, "orbit_number": 28538, "uri":  # noqa
+                        "/home/lahtinep/data/satellite/hrpt-pps/S_NWC_CMA_metopb_28538_20180319T0955387Z_20180319T1009544Z.nc", "start_seconds": 38, "platform_name": "Metop-B", "end_seconds": 54, "end_time": dt.datetime(2018, 3, 19, 10, 9, 0), "path": "", "sensor": ["avhrr/3"]}  # noqa
 
-        self.mda_hrpt = {"uid": "hrpt_metop01_20180319_0955_28538.l1b", "platform_shortname": "metop01", "start_time": dt.datetime(2018, 3, 19, 9, 55, 0), "orbit_number":
-                         28538, "uri": "/home/lahtinep/data/satellite/new/hrpt_metop01_20180319_0955_28538.l1b", "platform_name": "Metop-B", "path": "", "sensor": ["avhrr/3"]}
+        self.mda_hrpt = {"uid": "hrpt_metop01_20180319_0955_28538.l1b", "platform_shortname": "metop01", "start_time": dt.datetime(2018, 3, 19, 9, 55, 0), "orbit_number":  # noqa
+                         28538, "uri": "/home/lahtinep/data/satellite/new/hrpt_metop01_20180319_0955_28538.l1b", "platform_name": "Metop-B", "path": "", "sensor": ["avhrr/3"]}  # noqa
 
         self.mda_goes16 = {"uid": "OR_ABI-L1b-RadF-M3C08_G16_s20190320600324_e20190320611091_c20190320611138.nc",
                            "creation_time": "20190320611138",
                            "start_time": dt.datetime(2019, 2, 1, 6, 0, 0),
                            "area_code": "F", "mission_id": "ABI", "path": "",
                            "system_environment": "OR", "scan_mode": "M3",
                            "uri": "/path/OR_ABI-L1b-RadF-M3C08_G16_s20190320600324_e20190320611091_c20190320611138.nc",
@@ -76,32 +78,42 @@
                            "platform_name": "GOES-16",
                            "end_time": dt.datetime(2019, 2, 1, 6, 11, 9, 100000),
                            "orig_platform_name": "G16", "dataset_name": "Rad",
                            "sensor": ["abi"], "channel": "C08"}
 
         self.msg0deg = SegmentGatherer(CONFIG_SINGLE)
         self.msg0deg_iodc = SegmentGatherer(CONFIG_DOUBLE)
+        self.iodc_himawari = SegmentGatherer(CONFIG_DOUBLE_DIFFERENT)
         self.hrpt_pps = SegmentGatherer(CONFIG_NO_SEG)
         self.msg_ini = SegmentGatherer(CONFIG_INI)
         self.goes_ini = SegmentGatherer(CONFIG_INI_NO_SEG)
+        self.himawari_ini = SegmentGatherer(CONFIG_INI_HIMAWARI)
 
     def test_init(self):
+        """Test init."""
         self.assertTrue(self.msg0deg._config == CONFIG_SINGLE)
         self.assertTrue(self.msg0deg._subject is None)
         self.assertEqual(list(self.msg0deg._patterns.keys()), ['msg'])
         self.assertEqual(list(self.msg0deg._parsers.keys()), ['msg'])
         self.assertEqual(len(self.msg0deg.slots.keys()), 0)
         self.assertEqual(self.msg0deg.time_name, 'start_time')
         self.assertFalse(self.msg0deg._loop)
         self.assertEqual(self.msg0deg._time_tolerance, 30)
         self.assertEqual(self.msg0deg._timeliness.total_seconds(), 10)
         self.assertEqual(self.msg0deg._listener, None)
         self.assertEqual(self.msg0deg._publisher, None)
 
+        # Tests using two filesets start_time_pattern
+        self.assertTrue('start_time_pattern' in self.msg0deg_iodc._patterns['msg'])
+        self.assertTrue('_start_time_pattern' in self.msg0deg_iodc._patterns['msg'])
+        self.assertTrue('start_time_pattern' in self.msg0deg_iodc._patterns['iodc'])
+        self.assertTrue('_start_time_pattern' in self.msg0deg_iodc._patterns['iodc'])
+
     def test_init_data(self):
+        """Test initializing the data."""
         mda = self.mda_msg0deg.copy()
         self.msg0deg._init_data(mda)
 
         slot_str = str(mda["start_time"])
         self.assertEqual(list(self.msg0deg.slots.keys())[0], slot_str)
         slot = self.msg0deg.slots[slot_str]
         for key in mda:
@@ -133,14 +145,15 @@
         self.msg_ini._init_data(mda)
         slot = self.msg_ini.slots[slot_str]
         self.assertEqual(len(slot['msg']['critical_files']), 2)
         self.assertEqual(len(slot['msg']['wanted_files']), 38)
         self.assertEqual(len(slot['msg']['all_files']), 114)
 
     def test_compose_filenames(self):
+        """Test composing the filenames."""
         mda = self.mda_msg0deg.copy()
         self.msg0deg._init_data(mda)
         slot_str = str(mda["start_time"])
         fname_set = self.msg0deg._compose_filenames(
             'msg', slot_str,
             self.msg0deg._config['patterns']['msg']['critical_files'])
         self.assertTrue(fname_set, set)
@@ -170,52 +183,55 @@
         self.assertEqual(len(fname_set), 1)
         self.assertTrue("hrpt_*_20180319_0955_28538.l1b" in fname_set)
         fname_set = self.hrpt_pps._compose_filenames(
             'pps', slot_str,
             self.hrpt_pps._config['patterns']['pps']['critical_files'])
         self.assertEqual(len(fname_set), 1)
         self.assertTrue(
-            "S_NWC_CMA_*_28538_20180319T0955???Z_????????T???????Z.nc" in \
-            fname_set)
+            "S_NWC_CMA_*_28538_20180319T0955???Z_????????T???????Z.nc" in fname_set)
 
         # Tests using filesets with no segments, INI config
         mda = self.mda_goes16.copy()
         self.goes_ini._init_data(mda)
         slot_str = str(mda["start_time"])
         fname_set = self.goes_ini._compose_filenames(
             'goes16', slot_str,
             self.goes_ini._config['patterns']['goes16']['critical_files'])
         self.assertEqual(len(fname_set), 0)
 
     def test_set_logger(self):
+        """Test setting the logger."""
         logger = logging.getLogger('foo')
         self.msg0deg.set_logger(logger)
         self.assertTrue(logger is self.msg0deg.logger)
 
     def test_update_timeout(self):
+        """Test updating the timeout."""
         mda = self.mda_msg0deg.copy()
         slot_str = str(mda["start_time"])
         self.msg0deg._init_data(mda)
         now = dt.datetime.utcnow()
         self.msg0deg.update_timeout(slot_str)
         diff = self.msg0deg.slots[slot_str]['timeout'] - now
         self.assertAlmostEqual(diff.total_seconds(), 10.0, places=3)
 
     def test_slot_ready(self):
+        """Test if a slot is ready."""
         mda = self.mda_msg0deg.copy()
         slot_str = str(mda["start_time"])
         self.msg0deg._init_data(mda)
         func = self.msg0deg.slot_ready
         self.assertTrue(self.msg0deg.slots[slot_str]['timeout'] is None)
         res = func(slot_str)
         self.assertEqual(res, SLOT_NOT_READY)
         self.assertTrue(self.msg0deg.slots[slot_str]['timeout'] is not None)
         # TODO
 
     def test_get_collection_status(self):
+        """Test getting the collection status."""
         mda = self.mda_msg0deg.copy()
         slot_str = str(mda["start_time"])
 
         now = dt.datetime.utcnow()
         future = now + dt.timedelta(minutes=1)
         past = now - dt.timedelta(minutes=1)
         func = self.msg0deg.get_collection_status
@@ -289,14 +305,15 @@
         status = {'foo': SLOT_READY_BUT_WAIT_FOR_MORE,
                   'bar': SLOT_READY_BUT_WAIT_FOR_MORE}
         self.assertEqual(func(status, past, slot_str), SLOT_READY)
         self.assertEqual(func(status, future, slot_str),
                          SLOT_READY_BUT_WAIT_FOR_MORE)
 
     def test_add_file(self):
+        """Test adding a file."""
         # Single fileset
         msg_data = self.mda_msg0deg.copy()
         col = self.msg0deg
         col._init_data(msg_data)
         time_slot = list(col.slots.keys())[0]
         key = list(CONFIG_SINGLE['patterns'].keys())[0]
         mda = col._parsers[key].parse(msg_data['uid'])
@@ -340,14 +357,15 @@
             self.assertEqual(len(col.slots[time_slot][key]['received_files']),
                              1)
             meta = col.slots[time_slot]['metadata']
             self.assertEqual(len(meta['collection'][key]['dataset']), 1)
             i += 1
 
     def test_ini_to_dict(self):
+        """Test ini conversion to dict."""
         config = ini_to_dict(os.path.join(THIS_DIR, "data/segments.ini"), "msg")
         self.assertTrue('patterns' in config)
         self.assertTrue('posttroll' in config)
         self.assertTrue('time_tolerance' in config)
         self.assertTrue('timeliness' in config)
         self.assertTrue('num_files_premature_publish' in config)
 
@@ -362,24 +380,135 @@
         self.assertTrue('pattern' in config['patterns']['msg'])
         self.assertTrue('critical_files' in config['patterns']['msg'])
         self.assertTrue('wanted_files' in config['patterns']['msg'])
         self.assertTrue('all_files' in config['patterns']['msg'])
         self.assertTrue('is_critical_set' in config['patterns']['msg'])
         self.assertTrue('variable_tags' in config['patterns']['msg'])
 
-    def tearDown(self):
-        """Closing down
-        """
-        pass
+    def test_check_schedule_time(self):
+        """Test Check Schedule Time."""
+        import datetime
+
+        hour = self.msg0deg_iodc._patterns['msg']['_start_time_pattern']
+        self.assertTrue(self.msg0deg.check_schedule_time(hour, datetime.time(9, 0)))
+        self.assertFalse(self.msg0deg.check_schedule_time(hour, datetime.time(9, 30)))
+        self.assertFalse(self.msg0deg.check_schedule_time(hour, datetime.time(23, 0)))
+        hour = self.msg0deg_iodc._patterns['iodc']['_start_time_pattern']
+        self.assertTrue(self.msg0deg.check_schedule_time(hour, datetime.time(4, 15)))
+        self.assertFalse(self.msg0deg.check_schedule_time(hour, datetime.time(4, 30)))
+        self.assertFalse(self.msg0deg.check_schedule_time(hour, datetime.time(11, 0)))
+
+    def test_floor_time(self):
+        """Test that flooring the time to set minutes work."""
+        parser = self.himawari_ini._parsers['himawari-8']
+        mda = parser.parse("IMG_DK01IR4_201712081129_010")
+        self.assertEqual(mda['start_time'].minute, 29)
+        mda2 = self.himawari_ini._floor_time(mda.copy())
+        self.assertEqual(mda2['start_time'].minute, 20)
+        self.himawari_ini._group_by_minutes = 15
+        mda2 = self.himawari_ini._floor_time(mda.copy())
+        self.assertEqual(mda2['start_time'].minute, 15)
+        self.himawari_ini._group_by_minutes = 2
+        mda2 = self.himawari_ini._floor_time(mda.copy())
+        self.assertEqual(mda2['start_time'].minute, 28)
+        # Add seconds
+        mod_mda = mda.copy()
+        start_time = mda['start_time']
+        mod_mda['start_time'] = dt.datetime(start_time.year, start_time.month,
+                                            start_time.day, start_time.hour,
+                                            start_time.minute, 42)
+        # The seconds should also be zero'd
+        mda2 = self.himawari_ini._floor_time(mda.copy())
+        self.assertEqual(mda2['start_time'].minute, 28)
+        self.assertEqual(mda2['start_time'].second, 0)
+
+        # Test that nothing is changed when groub_by_minutes has not
+        # been configured
+        self.himawari_ini._group_by_minutes = None
+        mda2 = self.himawari_ini._floor_time(mod_mda.copy())
+        self.assertEqual(mda2['start_time'], mod_mda['start_time'])
+
+    def test_floor_time_different(self):
+        """Test that flooring the time to set minutes work."""
+        key = 'himawari'
+        parser = self.iodc_himawari._parsers[key]
+        mda = parser.parse("IMG_DK01IR4_201712081129_010")
+        self.assertEqual(mda['start_time'].minute, 29)
+
+        # Here the floor time (group_by_minutes)is read from the yaml config file
+        # specific for himawari. You dont want to group_by_minutes for IODC
+        mda2 = self.iodc_himawari._floor_time(mda.copy(), key)
+        self.assertEqual(mda2['start_time'].minute, 20)
+        # Add seconds
+        mod_mda = mda.copy()
+        start_time = mda['start_time']
+        mod_mda['start_time'] = dt.datetime(start_time.year, start_time.month,
+                                            start_time.day, start_time.hour,
+                                            start_time.minute, 42)
+        # The seconds should also be zero'd ( group_by_minutes from config file)
+        mda2 = self.iodc_himawari._floor_time(mda.copy(), key)
+        self.assertEqual(mda2['start_time'].minute, 20)
+        self.assertEqual(mda2['start_time'].second, 0)
+
+        # Test that nothing is changed when groub_by_minutes has not
+        # been configured
+        self.iodc_himawari._group_by_minutes = None
+        mda2 = self.iodc_himawari._floor_time(mod_mda.copy())
+        self.assertEqual(mda2['start_time'], mod_mda['start_time'])
+
+        key = 'iodc'
+        parser = self.iodc_himawari._parsers[key]
+        mda = parser.parse("H-000-MSG2__-MSG2_IODC___-_________-EPI______-201611281115-__")
+        self.assertEqual(mda['start_time'].minute, 15)
+
+        # Here the floor time (group_by_minutes)is read from the yaml config file
+        # but it is not given for IODC
+        mda2 = self.iodc_himawari._floor_time(mda.copy(), key)
+        self.assertEqual(mda2['start_time'].minute, 15)
+
+    def test_copy_metadata(self):
+        """Test combining metadata from a message and parsed from filename."""
+        from pytroll_collectors.segments import copy_metadata
+        try:
+            from unittest import mock
+        except ImportError:
+            import mock
+
+        mda = {'a': 1, 'b': 2}
+        msg = mock.MagicMock()
+        msg.data = {'a': 2, 'c': 3}
+
+        res = copy_metadata(mda, msg)
+        self.assertEqual(res['a'], 2)
+        self.assertEqual(res['b'], 2)
+        self.assertEqual(res['c'], 3)
+
+        # Keep 'a' from parsed metadata
+        res = copy_metadata(mda, msg, keep_parsed_keys=['a'])
+        self.assertEqual(res['a'], 1)
+        self.assertEqual(res['b'], 2)
+        self.assertEqual(res['c'], 3)
+
+        # Keep 'a' from parsed metadata configured for one of more patterns
+        res = copy_metadata(mda, msg, local_keep_parsed_keys=['a'])
+        self.assertEqual(res['a'], 1)
+        self.assertEqual(res['b'], 2)
+        self.assertEqual(res['c'], 3)
+
+    def test_publish_service_name(self):
+        """Test publish service name. Need to be equal each time"""
+        col = self.msg0deg_iodc
+        publish_service_name = col._generate_publish_service_name()
+        self.assertEqual(publish_service_name, "segment_gatherer_iodc_msg")
 
 
 def suite():
-    """The suite for test_trollduction
-    """
+    """Test suite for test_trollduction."""
     loader = unittest.TestLoader()
     mysuite = unittest.TestSuite()
     mysuite.addTest(loader.loadTestsFromTestCase(TestSegmentGatherer))
 
     return mysuite
 
+
 if __name__ == "__main__":
     unittest.TextTestRunner(verbosity=2).run(suite())
```

### Comparing `pytroll_collectors-0.8.4/pytroll_collectors/trigger.py` & `pytroll_collectors-0.9.0/pytroll_collectors/trigger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2012, 2014, 2015 Martin Raspaud
+# Copyright (c) 2012, 2014, 2015, 2019 Martin Raspaud
 
 # Author(s):
 
 #   Kristian Rune Larsen <krl@dmi.dk>
 #   Martin Raspaud <martin.raspaud@smhi.se>
 #   Panu Lahtinen <panu.lahtinen@fmi.fi>
 
@@ -20,22 +20,23 @@
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Triggers for region_collectors."""
 
-from pyinotify import (ProcessEvent, Notifier, WatchManager,
-                       IN_CLOSE_WRITE, IN_MOVED_TO)
 import logging
+import os.path
 from datetime import datetime, timedelta
 from fnmatch import fnmatch
-import os.path
-from posttroll.subscriber import NSSubscriber
+from threading import Event, Thread
 
+from posttroll.subscriber import NSSubscriber
+from pyinotify import (IN_CLOSE_WRITE, IN_MOVED_TO, Notifier, ProcessEvent,
+                       WatchManager)
 
 LOG = logging.getLogger(__name__)
 
 
 def total_seconds(tdef):
     """Calculate total time in seconds."""
     return ((tdef.microseconds +
@@ -64,66 +65,58 @@
     if "duration" in mda:
         del mda["duration"]
 
     return mda
 
 
 class Trigger(object):
-
-    """Abstract trigger class.
-    """
+    """Abstract trigger class."""
 
     def __init__(self, collectors, terminator, publish_topic=None):
+        """Init the trigger."""
         self.collectors = collectors
         self.terminator = terminator
         self.publish_topic = publish_topic
 
     def _do(self, metadata):
-        """Execute the collectors and terminator.
-        """
+        """Execute the collectors and terminator."""
         if not metadata:
             LOG.warning("No metadata")
             return
         for collector in self.collectors:
             res = collector(metadata.copy())
             if res:
                 return self.terminator(res, publish_topic=self.publish_topic)
 
 
-from threading import Thread, Event
-
-
 class FileTrigger(Trigger, Thread):
-
-    """File trigger, acting upon inotify events.
-    """
+    """File trigger, acting upon inotify events."""
 
     def __init__(self, collectors, terminator, decoder, publish_topic=None, publish_message_after_each_reception=False):
+        """Init the file trigger."""
         Thread.__init__(self)
         Trigger.__init__(self, collectors, terminator,
                          publish_topic=publish_topic)
         self.decoder = decoder
         self._running = True
         self.new_file = Event()
         self.publish_message_after_each_reception = publish_message_after_each_reception
 
     def _do(self, pathname):
         mda = self.decoder(pathname)
         LOG.debug("mda: %s", str(mda))
         Trigger._do(self, mda)
 
     def add_file(self, pathname):
-        """On arrival of a file.
-        """
+        """React to arrival of a file."""
         self._do(pathname)
         self.new_file.set()
 
     def run(self):
-        """The timeouts are handled here.
-        """
+        """Handle the timeouts."""
         # The wait for new files is handled through the event mechanism of the
         # threading module:
         # - first a new file arrives, and an event is triggered
         # - then the new timeouts are computed
         # - if a timeout occurs during the wait, the wait is interrupted and
         #   the timeout is handled.
         while self._running:
@@ -163,57 +156,52 @@
                                                      datetime.utcnow()))
                     self.new_file.clear()
             else:
                 self.new_file.wait()
                 self.new_file.clear()
 
     def stop(self):
-        """Stopping everything.
-        """
+        """Stop everything."""
         self._running = False
         self.new_file.set()
 
 
 class InotifyTrigger(ProcessEvent, FileTrigger):
-
-    """File trigger, acting upon inotify events.
-    """
+    """File trigger, acting upon inotify events."""
 
     def __init__(self, collectors, terminator, decoder, patterns,
                  publish_topic=None):
+        """Init the inotify trigger."""
         ProcessEvent.__init__(self)
         FileTrigger.__init__(self, collectors, terminator, decoder,
                              publish_topic=publish_topic)
         self.input_dirs = []
         for pattern in patterns:
             self.input_dirs.append(os.path.dirname(pattern))
         self.patterns = patterns
         self.new_file = Event()
 
     def process_IN_CLOSE_WRITE(self, event):
-        """On closing a file.
-        """
+        """Process a closing file."""
         for pattern in self.patterns:
             if fnmatch(event.src_path, pattern):
                 LOG.debug("New file detected (close write): %s",
                           event.pathname)
                 self.add_file(event.pathname)
 
     def process_IN_MOVED_TO(self, event):
-        """On moving a file into the directory.
-        """
+        """Process a file moving into the directory."""
         for pattern in self.patterns:
             if fnmatch(event.src_path, pattern):
                 LOG.debug("New file detected (moved to): %s",
                           event.pathname)
                 self.add_file(event.pathname)
 
     def loop(self):
-        """The main function.
-        """
+        """Loop until done."""
         self.start()
         try:
             # inotify interface
             wm_ = WatchManager()
             mask = IN_CLOSE_WRITE | IN_MOVED_TO
 
             # create notifier
@@ -225,225 +213,232 @@
 
             # loop forever
             notifier.loop()
         finally:
             self.stop()
             self.join()
 
+
 try:
     from watchdog.events import FileSystemEventHandler
     from watchdog.observers.polling import PollingObserver
     from watchdog.observers import Observer
 
-    class WatchDogTriggerOld(FileSystemEventHandler, FileTrigger):
-
-        """File trigger, acting upon inotify events.
-        """
-
-        cases = {"PollingObserver": PollingObserver,
-                 "Observer": Observer}
-
-        def __init__(self, collectors, terminator, decoder, patterns,
-                     observer_class_name, publish_topic=None):
-            FileSystemEventHandler.__init__(self)
-            FileTrigger.__init__(self, collectors, terminator, decoder,
-                                 publish_topic=publish_topic)
-            self.input_dirs = []
-            for pattern in patterns:
-                self.input_dirs.append(os.path.dirname(pattern))
-            self.patterns = patterns
-
-            self.new_file = Event()
-            self.observer = self.cases.get(observer_class_name, Observer)()
-
-        def on_created(self, event):
-            """On creating a file.
-            """
-            try:
-                for pattern in self.patterns:
-                    if fnmatch(event.src_path, pattern):
-                        LOG.debug("New file detected (created): %s",
-                                  event.src_path)
-                        self.add_file(event.src_path)
-                        LOG.debug("Done adding")
-                        return
-            except Exception as e:
-                LOG.exception(
-                    "Something wrong happened in the event processing: %s",
-                    e.message)
-
-        def start(self):
-            """Start trigger.
-            """
-            # add watches
-            for idir in self.input_dirs:
-                self.observer.schedule(self, idir)
-            self.observer.start()
-
-            FileTrigger.start(self)
-            LOG.debug("Started polling")
-
-        def stop(self):
-            self.observer.stop()
-            FileTrigger.stop(self)
-            self.observer.join()
-            self.join()
+    # class WatchDogTriggerOld(FileSystemEventHandler, FileTrigger):
+    #     """File trigger, acting upon inotify events."""
+    #
+    #     cases = {"PollingObserver": PollingObserver,
+    #              "Observer": Observer}
+    #
+    #     def __init__(self, collectors, terminator, decoder, patterns,
+    #                  observer_class_name, publish_topic=None):
+    #         """Init the watchdog trigger."""
+    #         FileSystemEventHandler.__init__(self)
+    #         FileTrigger.__init__(self, collectors, terminator, decoder,
+    #                              publish_topic=publish_topic)
+    #         self.input_dirs = []
+    #         for pattern in patterns:
+    #             self.input_dirs.append(os.path.dirname(pattern))
+    #         self.patterns = patterns
+    #
+    #         self.new_file = Event()
+    #         self.observer = self.cases.get(observer_class_name, Observer)()
+    #
+    #     def on_created(self, event):
+    #         """Process file creation."""
+    #         try:
+    #             for pattern in self.patterns:
+    #                 if fnmatch(event.src_path, pattern):
+    #                     LOG.debug("New file detected (created): %s",
+    #                               event.src_path)
+    #                     self.add_file(event.src_path)
+    #                     LOG.debug("Done adding")
+    #                     return
+    #         except Exception as e:
+    #             LOG.exception(
+    #                 "Something wrong happened in the event processing: %s",
+    #                 e.message)
+    #
+    #     def start(self):
+    #         """Start trigger."""
+    #         # add watches
+    #         for idir in self.input_dirs:
+    #             self.observer.schedule(self, idir)
+    #         self.observer.start()
+    #
+    #         FileTrigger.start(self)
+    #         LOG.debug("Started polling")
+    #
+    #     def stop(self):
+    #         """Stop the trigger."""
+    #         self.observer.stop()
+    #         FileTrigger.stop(self)
+    #         self.observer.join()
+    #         self.join()
 
     class AbstractWatchDogProcessor(FileSystemEventHandler):
-
-        """File trigger, acting upon file system events.
-        """
+        """File trigger, acting upon file system events."""
 
         cases = {"PollingObserver": PollingObserver,
                  "Observer": Observer}
 
         def __init__(self, patterns, observer_class_name="Observer"):
+            """Init the processor."""
             FileSystemEventHandler.__init__(self)
             self.input_dirs = []
             for pattern in patterns:
                 self.input_dirs.append(os.path.dirname(pattern))
                 LOG.debug("watching " + str(os.path.dirname(pattern)))
             self.patterns = patterns
 
             self.new_file = Event()
             self.observer = self.cases.get(observer_class_name, Observer)()
 
         def on_created(self, event):
-            """On creating a file.
-            """
+            """Process creating a file."""
             self._process(event.src_path)
 
         def on_moved(self, event):
-            """On a file been moved to the destination directory.
-            """
+            """Process a file being moved to the destination directory."""
             self._process(event.dest_path)
 
         def _process(self, pathname):
+            """Process a file."""
             try:
                 for pattern in self.patterns:
                     if fnmatch(pathname, pattern):
                         LOG.debug("New file detected : " + pathname)
                         self.process(pathname)
                         LOG.debug("Done processing file")
                         return
-            except:
+            except Exception:
                 LOG.exception(
                     "Something wrong happened in the event processing!")
 
         def process(self, pathname):
+            """Process, abstract."""
             raise NotImplementedError
 
         def start(self):
-            """Start processor"""
+            """Start processor."""
             # add watches
             for idir in self.input_dirs:
                 self.observer.schedule(self, idir)
             self.observer.start()
 
             LOG.debug("Started watching filesystem")
 
         def stop(self):
-            """Stop processor"""
+            """Stop processor."""
             self.observer.stop()
             self.observer.join()
 
     class WatchDogTrigger(FileTrigger):
-
-        """File trigger, acting upon filesystem events.
-        """
+        """File trigger, acting upon filesystem events."""
 
         def __init__(self, collectors, terminator, decoder,
                      patterns, observer_class_name, publish_topic=None):
+            """Init the trigger."""
             self.wdp = AbstractWatchDogProcessor(patterns, observer_class_name)
             FileTrigger.__init__(self, collectors, terminator, decoder,
                                  publish_topic=publish_topic)
             self.wdp.process = self.add_file
 
         def start(self):
-
+            """Start the trigger."""
             # add watches
             self.wdp.start()
 
             FileTrigger.start(self)
             LOG.debug("Started polling")
 
         def stop(self):
+            """Stop the trigger."""
             FileTrigger.stop(self)
             self.wdp.stop()
             self.join()
 
 
 except ImportError:
-    LOG.error("Watchdog import failed!")
+    LOG.exception("Watchdog import failed!")
     WatchDogTrigger = None
 
 
 class AbstractMessageProcessor(Thread):
-
-    """Process Messages
-    """
+    """Process Messages."""
 
     def __init__(self, services, topics, nameserver="localhost"):
+        """Init the message processor."""
         Thread.__init__(self)
         LOG.debug("Nameserver: {}".format(nameserver))
         self.nssub = NSSubscriber(services, topics, True, nameserver=nameserver)
         self.sub = None
         self.loop = True
 
     def start(self):
+        """Start the processor."""
         self.sub = self.nssub.start()
         Thread.start(self)
 
     def process(self, msg):
-        """Process the message.
-        """
+        """Process the message."""
         del msg
         raise NotImplementedError("process is not implemented!")
 
     def run(self):
-        """Run the trigger.
-        """
+        """Run the trigger."""
         try:
             for msg in self.sub.recv(2):
                 if not self.loop:
                     break
                 if msg is None:
                     continue
+                if msg.type not in ('file', 'collection', 'dataset'):
+                    continue
                 self.process(msg)
         finally:
             self.stop()
 
     def stop(self):
-        """Stop the trigger.
-        """
+        """Stop the trigger."""
         self.nssub.stop()
         self.loop = False
 
 
 class PostTrollTrigger(FileTrigger):
+    """Get posttroll messages."""
 
-    """Get posttroll messages.
-    """
-
-    def __init__(self, collectors, terminator, services, topics,
+    def __init__(self, collectors, terminator, services, topics, duration=None,
                  publish_topic=None, nameserver="localhost",
                  publish_message_after_each_reception=False):
+        """Init the posttroll trigger."""
+        self.duration = duration
         self.msgproc = AbstractMessageProcessor(services, topics, nameserver=nameserver)
         self.msgproc.process = self.add_file
         FileTrigger.__init__(self, collectors, terminator, self.decode_message,
                              publish_topic=publish_topic,
                              publish_message_after_each_reception=publish_message_after_each_reception)
 
     def start(self):
         """Start the posttroll trigger."""
         FileTrigger.start(self)
         self.msgproc.start()
 
-    @staticmethod
-    def decode_message(message):
+    def decode_message(self, message):
         """Return the message data."""
-        return fix_start_end_time(message.data)
+
+        # Include file duration in message data
+        if self.duration:
+            message.data["duration"] = self.duration
+
+        # Fix start and end time
+        try:
+            mgs_data = fix_start_end_time(message.data)
+        except KeyError:
+            LOG.exception("Something went wrong!")
+        else:
+            return mgs_data
 
     def stop(self):
         """Stop the posttroll trigger."""
         self.msgproc.stop()
         FileTrigger.stop(self)
```

### Comparing `pytroll_collectors-0.8.4/pytroll_collectors.egg-info/PKG-INFO` & `pytroll_collectors-0.9.0/pytroll_collectors.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: pytroll-collectors
-Version: 0.8.4
+Version: 0.9.0
 Summary: Pytroll data collectors
 Home-page: https://github.com/pytroll/pytroll-collectors
 Author: Martin Raspaud
 Author-email: martin.raspaud@smhi.se
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
-Provides-Extra: image_scaler
-Provides-Extra: global_mosaic
-Provides-Extra: all
```

### Comparing `pytroll_collectors-0.8.4/setup.py` & `pytroll_collectors-0.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2013 - 2018 PyTroll Community
+# Copyright (c) 2013 - 2019 PyTroll Community
 
 # Author(s):
 
 #   Martin Raspaud <martin.raspaud@smhi.se>
 #   Adam Dybbroe <adam.dybbroe@smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
@@ -17,39 +17,27 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Setup for pytroll_collectors.
-"""
+"""Setup for pytroll_collectors."""
 from setuptools import setup
-import imp
+import versioneer
 import os
 
 THIS_DIR = os.path.dirname(os.path.abspath(__file__))
 # Set PPP_CONFIG_DIR for tests
 os.environ['PPP_CONFIG_DIR'] = os.path.join(THIS_DIR, 'pytroll_collectors', 'tests', 'data')
 
-version = imp.load_source(
-    'pytroll_collectors.version', 'pytroll_collectors/version.py')
-
-extras_require = {
-    'image_scaler': ['satpy>=v0.8.0'],
-    'global_mosaic': ['satpy>=v0.8.0'],
-}
-all_extras = []
-for extra_deps in extras_require.values():
-    all_extras.extend(extra_deps)
-extras_require['all'] = list(set(all_extras))
-
 
 setup(name="pytroll_collectors",
-      version=version.__version__,
+      version=versioneer.get_version(),
+      cmdclass=versioneer.get_cmdclass(),
       description='Pytroll data collectors',
       author='Martin Raspaud',
       author_email='martin.raspaud@smhi.se',
       classifiers=["Development Status :: 3 - Alpha",
                    "Intended Audience :: Science/Research",
                    "License :: OSI Approved :: GNU General Public License v3 " +
                    "or later (GPLv3+)",
@@ -58,26 +46,22 @@
                    "Topic :: Scientific/Engineering"],
       url="https://github.com/pytroll/pytroll-collectors",
       packages=['pytroll_collectors',
                 'pytroll_collectors.tests', ],
       scripts=['bin/trollstalker.py',
                'bin/trollstalker2.py',
                'bin/gatherer.py',
-               'bin/geo_gatherer.py',
                'bin/segment_gatherer.py',
                'bin/cat.py',
                'bin/catter.py',
                'bin/scisys_receiver.py',
-               'bin/create_global_mosaic.py',
-               'bin/scale_images.py',
                'bin/zipcollector_runner.py'
                ],
       data_files=[],
       zip_safe=False,
       install_requires=['pykdtree', 'pyinotify', 'posttroll>=1.3.0',
-                        'trollsift', 'netifaces',
+                        'trollsift', 'netifaces', 'watchdog',
                         'pytroll-schedule', 'pyresample',
                         'pillow', 'pycoast', 'six'],
       tests_require=['mock', 'scipy', 'trollsift', 'pillow', 'six'],
       test_suite='pytroll_collectors.tests.suite',
-      extras_require=extras_require,
       )
```


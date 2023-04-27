# Comparing `tmp/axis-8.tar.gz` & `tmp/axis-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/axis-8.tar", last modified: Thu May 25 20:16:37 2017, max compression
+gzip compressed data, was "dist/axis-9.tar", last modified: Fri Sep  1 20:49:20 2017, max compression
```

## Comparing `axis-8.tar` & `axis-9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2017-05-25 20:16:37.000000 axis-8/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2017-05-25 20:16:37.000000 axis-8/axis.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)        9 2017-05-25 20:16:36.000000 axis-8/axis.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      179 2017-05-25 20:16:37.000000 axis-8/axis.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        5 2017-05-25 20:16:36.000000 axis-8/axis.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      410 2017-05-25 20:16:36.000000 axis-8/axis.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2017-05-25 20:16:36.000000 axis-8/axis.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      712 2017-05-25 19:59:09.000000 axis-8/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2017-05-25 20:16:37.000000 axis-8/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      410 2017-05-25 20:16:37.000000 axis-8/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2017-05-25 20:16:37.000000 axis-8/axis/
--rw-r--r--   0 pi        (1000) pi        (1000)     3744 2017-05-21 17:25:29.000000 axis-8/axis/stream.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9228 2017-05-21 20:47:10.000000 axis-8/axis/__init__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2017-09-01 20:49:20.000000 axis-9/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2017-09-01 20:49:20.000000 axis-9/axis.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)        9 2017-09-01 20:49:19.000000 axis-9/axis.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      192 2017-09-01 20:49:19.000000 axis-9/axis.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        5 2017-09-01 20:49:19.000000 axis-9/axis.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      410 2017-09-01 20:49:19.000000 axis-9/axis.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2017-09-01 20:49:18.000000 axis-9/axis.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      712 2017-09-01 20:45:20.000000 axis-9/setup.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2017-09-01 20:49:20.000000 axis-9/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      410 2017-09-01 20:49:20.000000 axis-9/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2017-09-01 20:49:20.000000 axis-9/axis/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3747 2017-07-12 12:44:18.000000 axis-9/axis/stream.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    12277 2017-09-01 09:31:41.000000 axis-9/axis/rtsp.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9830 2017-09-01 20:29:08.000000 axis-9/axis/__init__.py
```

### Comparing `axis-8/setup.py` & `axis-9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # python setup.py sdist upload -r pypi
 
 from setuptools import setup
 
 setup(
   name='axis',
   packages=['axis'],
-  version='8',
+  version='9',
   description='A python library for communicating with devices from Axis Communications',
   author='Robert Svensson',
   author_email='Kane610@users.noreply.github.com',
   license='MIT',
   url='https://github.com/Kane610/axis',
-  download_url='https://github.com/Kane610/axis/archive/v8.tar.gz',
+  download_url='https://github.com/Kane610/axis/archive/v9.tar.gz',
   install_requires=['requests'],
   keywords=['axis', 'vapix', 'onvif', 'event stream', 'homeassistant'],
   classifiers=[],
 )
```

### Comparing `axis-8/axis/stream.py` & `axis-9/axis/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,9 +100,9 @@
             self.signal_parent()
             _LOGGER.info('No connection to device')
 
         if message.type == Gst.MessageType.ERROR:
             err, _ = message.parse_error()
             _LOGGER.debug('%s', err)
         else:
-            _LOGGER.debug('metadatastream bus message type:', message.type)
+            _LOGGER.debug('metadatastream bus message type: %s', message.type)
         return Gst.BusSyncReply.PASS
```

### Comparing `axis-8/axis/__init__.py` & `axis-9/axis/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         return r.text
 
     @property
     def metadata_url(self):
         """Set up url for metadatastream"""
         rtsp = "rtsp://{0}:{1}@{2}/axis-media/media.amp?".format(
             self._username, self._password, self._url)
-        source = 'video={0}&audio={1}&even=on&eventtopic={2}'.format(
+        source = 'video={0}&audio={1}&event=on&eventtopic={2}'.format(
             self._video, self._audio, self._event_topics)
         return rtsp + source
 
     @property
     def name(self):
         """Device name"""
         return self._name
@@ -116,18 +116,27 @@
         """Add new event topic to subscribe to on metadatastream"""
         if self._event_topics is None:
             self._event_topics = event_topic
         else:
             self._event_topics = '{}|{}'.format(self._event_topics,
                                                 event_topic)
 
+    def minimum_firmware(self, constraint):
+        """Checks that firmwware isn't older than constraint."""
+        from packaging import version
+        return version.parse(self._version) >= version.parse(constraint)
+
     def initiate_metadatastream(self):
         """Set up gstreamer pipeline and data callback for metadatastream"""
+        if not self.minimum_firmware('5.50'):
+            _LOGGER.info("Too old firmware for metadatastream")
+            #return False
         try:
             from .stream import MetaDataStream
+            #from .rtsp import MetaDataStream
         except ImportError as err:
             _LOGGER.error("Missing dependency: %s, check documentation", err)
             return False
         self._metadatastream = MetaDataStream(self.metadata_url)
         self._metadatastream.signal_parent = self.stream_signal
         self._metadatastream.start()
         self._retry_timer = None
@@ -202,14 +211,15 @@
 
         elif data['Operation'] == 'Changed':
             event_name = '{}_{}'.format(data['Topic'], data['Source_value'])
             self.events[event_name].state = data['Data_value']
 
         elif data['Operation'] == 'Deleted':
             _LOGGER.debug("Deleted event from stream")
+            # ToDo:
             # keep a list of deleted events and a follow up timer of X,
             # then clean up. This should also take care of rebooting a camera
 
         else:
             _LOGGER.warning("Unexpected response: %s", data)
 
 
@@ -276,7 +286,14 @@
         else:
             _LOGGER.info("state.setter has no callback")
 
     @property
     def is_tripped(self):
         """Event is tripped now."""
         return self._state == '1'
+
+    def as_dict(self):
+        """Callback for __dict__."""
+        cdict = self.__dict__.copy()
+        del cdict['callback']
+        del cdict['_device']
+        return cdict
```


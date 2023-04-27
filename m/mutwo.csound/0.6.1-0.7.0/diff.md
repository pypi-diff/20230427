# Comparing `tmp/mutwo.csound-0.6.1.tar.gz` & `tmp/mutwo.csound-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.csound-0.6.1.tar", last modified: Sun Aug 14 12:49:01 2022, max compression
+gzip compressed data, was "mutwo.csound-0.7.0.tar", last modified: Thu Apr 27 07:14:47 2023, max compression
```

## Comparing `mutwo.csound-0.6.1.tar` & `mutwo.csound-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:49:01.839150 mutwo.csound-0.6.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2022-08-14 12:48:52.000000 mutwo.csound-0.6.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1238 2022-08-14 12:49:01.839150 mutwo.csound-0.6.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      783 2022-08-14 12:48:52.000000 mutwo.csound-0.6.1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:49:01.835150 mutwo.csound-0.6.1/mutwo/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:49:01.839150 mutwo.csound-0.6.1/mutwo/csound_converters/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      159 2022-08-14 12:48:52.000000 mutwo.csound-0.6.1/mutwo/csound_converters/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      496 2022-08-14 12:48:52.000000 mutwo.csound-0.6.1/mutwo/csound_converters/configurations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      871 2022-08-14 12:48:52.000000 mutwo.csound-0.6.1/mutwo/csound_converters/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12669 2022-08-14 12:48:52.000000 mutwo.csound-0.6.1/mutwo/csound_converters/csound.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:49:01.839150 mutwo.csound-0.6.1/mutwo/csound_version/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      144 2022-08-14 12:48:52.000000 mutwo.csound-0.6.1/mutwo/csound_version/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:49:01.835150 mutwo.csound-0.6.1/mutwo.csound.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1238 2022-08-14 12:49:01.000000 mutwo.csound-0.6.1/mutwo.csound.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      402 2022-08-14 12:49:01.000000 mutwo.csound-0.6.1/mutwo.csound.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-08-14 12:49:01.000000 mutwo.csound-0.6.1/mutwo.csound.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2022-08-14 12:49:01.000000 mutwo.csound-0.6.1/mutwo.csound.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-08-14 12:49:01.000000 mutwo.csound-0.6.1/mutwo.csound.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      104 2022-08-14 12:48:52.000000 mutwo.csound-0.6.1/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-08-14 12:49:01.839150 mutwo.csound-0.6.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1124 2022-08-14 12:48:52.000000 mutwo.csound-0.6.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1239 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      783 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 07:14:47.715942 mutwo.csound-0.7.0/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/mutwo/csound_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      159 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/mutwo/csound_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/mutwo/csound_converters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      871 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/mutwo/csound_converters/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12721 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/mutwo/csound_converters/csound.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/mutwo/csound_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/mutwo/csound_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/mutwo.csound.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1239 2023-04-27 07:14:47.000000 mutwo.csound-0.7.0/mutwo.csound.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-04-27 07:14:47.000000 mutwo.csound-0.7.0/mutwo.csound.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-27 07:14:47.000000 mutwo.csound-0.7.0/mutwo.csound.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-04-27 07:14:47.000000 mutwo.csound-0.7.0/mutwo.csound.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-04-27 07:14:47.000000 mutwo.csound-0.7.0/mutwo.csound.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1120 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/setup.py
```

### Comparing `mutwo.csound-0.6.1/LICENSE` & `mutwo.csound-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.csound-0.6.1/PKG-INFO` & `mutwo.csound-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mutwo.csound
-Version: 0.6.1
+Version: 0.7.0
 Summary: csound extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.ext-csound
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo.readthedocs.io/en/latest/
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # mutwo.csound
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.csound.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.csound)
```

### Comparing `mutwo.csound-0.6.1/README.md` & `mutwo.csound-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.csound-0.6.1/mutwo/csound_converters/constants.py` & `mutwo.csound-0.7.0/mutwo/csound_converters/constants.py`

 * *Files identical despite different names*

### Comparing `mutwo.csound-0.6.1/mutwo/csound_converters/csound.py` & `mutwo.csound-0.7.0/mutwo/csound_converters/csound.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,18 +59,18 @@
     or a number). If the returned type is a string, :class:`EventToCsoundScore`
     automatically adds quotations marks around the string in the score file.
 
     All p-fields can be overwritten in the following manner:
 
     >>> from mutwo import csound_converters
     >>> my_converter = csound_converters.EventToCsoundScore(
-    >>>     p1=lambda event: 2,
-    >>>     p4=lambda event: event.pitch.frequency,
-    >>>     p5=lambda event: event.volume
-    >>> )
+    ...     p1=lambda event: 2,
+    ...     p4=lambda event: event.pitch.frequency,
+    ...     p5=lambda event: event.volume
+    ... )
 
     For easier debugging of faulty score files, :mod:`mutwo` adds annotations
     when a new :class:`SequentialEvent` or a new :class:`SimultaneousEvent`
     starts.
     """
 
     _default_p_field_dict: PFieldDict = {
@@ -244,26 +244,29 @@
         :type event_to_convert: core_events.abc.Event
         :param path: where to write the csound score file
         :type path: str
 
         >>> import random
         >>> from mutwo import core_events
         >>> from mutwo import csound_converters
-        >>> from mutwo import music_parameters
         >>> converter = csound_converters.EventToCsoundScore(
-        >>>    p4=lambda event: event.pitch.frequency
-        >>> )
-        >>> events = core_events.SequentialEvent(
-        >>>    [
-        >>>        core_events.SimpleEvent(random.uniform(0.3, 1.2)) for _ in range(15)
-        >>>    ]
-        >>> )
-        >>> for event in events:
-        >>>     event.pitch = music_parameters.DirectPitch(random.uniform(100, 500))
-        >>> converter.convert(events, 'score.sco')
+        ...    p4=lambda event: event.tempo_envelope.duration
+        ... )
+        >>> event = core_events.SequentialEvent(
+        ...    [
+        ...        core_events.SimpleEvent(
+        ...             random.uniform(0.3, 1.2)
+        ...        ) for _ in range(15)
+        ...    ]
+        ... )
+        >>> for e in event:
+        ...     e.tempo_envelope = core_events.TempoEnvelope(
+        ...         [[0, 1], [random.uniform(10, 20), 0]]
+        ...     )
+        >>> converter.convert(event, 'score.sco')
         """
 
         csound_score_line_tuple = self._convert_event(
             event_to_convert, core_parameters.DirectDuration(0)
         )
         # convert events to strings (where each string represents one csound score line)
         # write csound score lines to file
```

### Comparing `mutwo.csound-0.6.1/mutwo.csound.egg-info/PKG-INFO` & `mutwo.csound-0.7.0/mutwo.csound.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mutwo.csound
-Version: 0.6.1
+Version: 0.7.0
 Summary: csound extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.ext-csound
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo.readthedocs.io/en/latest/
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # mutwo.csound
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.csound.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.csound)
```

### Comparing `mutwo.csound-0.6.1/setup.py` & `mutwo.csound-0.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("mutwo/csound_version/__init__.py") as fp:
     exec(fp.read(), version)
 
 VERSION = version["VERSION"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-extras_require = {"testing": ["nose", "coveralls"]}
+extras_require = {"testing": ["pytest>=7.1.1"]}
 
 setuptools.setup(
     name="mutwo.csound",
     version=VERSION,
     license="GPL",
     description="csound extension for event based framework for generative art",
     long_description=long_description,
@@ -24,13 +24,13 @@
     packages=[
         package
         for package in setuptools.find_namespace_packages(include=["mutwo.*"])
         if package[:5] != "tests"
     ],
     setup_requires=[],
     install_requires=[
-        "mutwo.core>=0.61.2, <1.0.0",
-        "natsort>=5.3.3, <6.0.0",
+        "mutwo.core>=1.0.0, <2.0.0",
+        "natsort>=8.0.0, <9.0.0",
     ],
     extras_require=extras_require,
-    python_requires=">=3.9, <4",
+    python_requires=">=3.10, <4",
 )
```


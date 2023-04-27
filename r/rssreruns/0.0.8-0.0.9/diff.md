# Comparing `tmp/rssreruns-0.0.8.tar.gz` & `tmp/rssreruns-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssreruns-0.0.8.tar", last modified: Thu Mar 16 20:07:31 2023, max compression
+gzip compressed data, was "rssreruns-0.0.9.tar", last modified: Tue Mar 21 19:05:00 2023, max compression
```

## Comparing `rssreruns-0.0.8.tar` & `rssreruns-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hannah    (1000) hannah    (1000)        0 2023-03-16 20:07:31.652896 rssreruns-0.0.8/
--rw-rw-r--   0 hannah    (1000) hannah    (1000)     1071 2023-01-21 05:04:09.000000 rssreruns-0.0.8/LICENSE.txt
--rw-rw-r--   0 hannah    (1000) hannah    (1000)     2030 2023-03-16 20:07:31.652896 rssreruns-0.0.8/PKG-INFO
--rw-rw-r--   0 hannah    (1000) hannah    (1000)      100 2023-01-21 18:47:33.000000 rssreruns-0.0.8/README.md
--rw-rw-r--   0 hannah    (1000) hannah    (1000)      961 2023-03-16 20:05:01.000000 rssreruns-0.0.8/pyproject.toml
--rw-rw-r--   0 hannah    (1000) hannah    (1000)     2221 2023-01-24 21:39:08.000000 rssreruns-0.0.8/requirements-dev.txt
--rw-rw-r--   0 hannah    (1000) hannah    (1000)      437 2023-01-24 21:48:37.000000 rssreruns-0.0.8/requirements.txt
--rw-rw-r--   0 hannah    (1000) hannah    (1000)       38 2023-03-16 20:07:31.652896 rssreruns-0.0.8/setup.cfg
-drwxrwxr-x   0 hannah    (1000) hannah    (1000)        0 2023-03-16 20:07:31.648896 rssreruns-0.0.8/src/
-drwxrwxr-x   0 hannah    (1000) hannah    (1000)        0 2023-03-16 20:07:31.652896 rssreruns-0.0.8/src/rssreruns/
--rw-rw-r--   0 hannah    (1000) hannah    (1000)      276 2023-01-21 21:52:33.000000 rssreruns-0.0.8/src/rssreruns/__init__.py
--rw-rw-r--   0 hannah    (1000) hannah    (1000)    14081 2023-01-21 22:00:20.000000 rssreruns-0.0.8/src/rssreruns/elementwrapper.py
--rw-rw-r--   0 hannah    (1000) hannah    (1000)    28406 2023-03-16 20:04:08.000000 rssreruns-0.0.8/src/rssreruns/feedmodifier.py
-drwxrwxr-x   0 hannah    (1000) hannah    (1000)        0 2023-03-16 20:07:31.652896 rssreruns-0.0.8/src/rssreruns.egg-info/
--rw-rw-r--   0 hannah    (1000) hannah    (1000)     2030 2023-03-16 20:07:31.000000 rssreruns-0.0.8/src/rssreruns.egg-info/PKG-INFO
--rw-rw-r--   0 hannah    (1000) hannah    (1000)      400 2023-03-16 20:07:31.000000 rssreruns-0.0.8/src/rssreruns.egg-info/SOURCES.txt
--rw-rw-r--   0 hannah    (1000) hannah    (1000)        1 2023-03-16 20:07:31.000000 rssreruns-0.0.8/src/rssreruns.egg-info/dependency_links.txt
--rw-rw-r--   0 hannah    (1000) hannah    (1000)      823 2023-03-16 20:07:31.000000 rssreruns-0.0.8/src/rssreruns.egg-info/requires.txt
--rw-rw-r--   0 hannah    (1000) hannah    (1000)       10 2023-03-16 20:07:31.000000 rssreruns-0.0.8/src/rssreruns.egg-info/top_level.txt
-drwxrwxr-x   0 hannah    (1000) hannah    (1000)        0 2023-03-16 20:07:31.652896 rssreruns-0.0.8/test/
--rw-rw-r--   0 hannah    (1000) hannah    (1000)     9593 2023-02-28 21:28:05.000000 rssreruns-0.0.8/test/test_elementwrapper.py
--rw-rw-r--   0 hannah    (1000) hannah    (1000)    17811 2023-03-16 19:52:27.000000 rssreruns-0.0.8/test/test_feedmodifier.py
+drwxrwxr-x   0 hannah    (1000) hannah    (1000)        0 2023-03-21 19:05:00.712442 rssreruns-0.0.9/
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)     1071 2023-01-21 05:04:09.000000 rssreruns-0.0.9/LICENSE.txt
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)     2030 2023-03-21 19:05:00.712442 rssreruns-0.0.9/PKG-INFO
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)      100 2023-01-21 18:47:33.000000 rssreruns-0.0.9/README.md
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)      961 2023-03-21 19:02:17.000000 rssreruns-0.0.9/pyproject.toml
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)     2221 2023-01-24 21:39:08.000000 rssreruns-0.0.9/requirements-dev.txt
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)      437 2023-01-24 21:48:37.000000 rssreruns-0.0.9/requirements.txt
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)       38 2023-03-21 19:05:00.712442 rssreruns-0.0.9/setup.cfg
+drwxrwxr-x   0 hannah    (1000) hannah    (1000)        0 2023-03-21 19:05:00.704442 rssreruns-0.0.9/src/
+drwxrwxr-x   0 hannah    (1000) hannah    (1000)        0 2023-03-21 19:05:00.708442 rssreruns-0.0.9/src/rssreruns/
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)      276 2023-01-21 21:52:33.000000 rssreruns-0.0.9/src/rssreruns/__init__.py
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)    14081 2023-01-21 22:00:20.000000 rssreruns-0.0.9/src/rssreruns/elementwrapper.py
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)    30178 2023-03-21 18:57:24.000000 rssreruns-0.0.9/src/rssreruns/feedmodifier.py
+drwxrwxr-x   0 hannah    (1000) hannah    (1000)        0 2023-03-21 19:05:00.712442 rssreruns-0.0.9/src/rssreruns.egg-info/
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)     2030 2023-03-21 19:05:00.000000 rssreruns-0.0.9/src/rssreruns.egg-info/PKG-INFO
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)      400 2023-03-21 19:05:00.000000 rssreruns-0.0.9/src/rssreruns.egg-info/SOURCES.txt
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)        1 2023-03-21 19:05:00.000000 rssreruns-0.0.9/src/rssreruns.egg-info/dependency_links.txt
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)      823 2023-03-21 19:05:00.000000 rssreruns-0.0.9/src/rssreruns.egg-info/requires.txt
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)       10 2023-03-21 19:05:00.000000 rssreruns-0.0.9/src/rssreruns.egg-info/top_level.txt
+drwxrwxr-x   0 hannah    (1000) hannah    (1000)        0 2023-03-21 19:05:00.712442 rssreruns-0.0.9/test/
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)     9593 2023-02-28 21:28:05.000000 rssreruns-0.0.9/test/test_elementwrapper.py
+-rw-rw-r--   0 hannah    (1000) hannah    (1000)    17811 2023-03-21 18:57:19.000000 rssreruns-0.0.9/test/test_feedmodifier.py
```

### Comparing `rssreruns-0.0.8/LICENSE.txt` & `rssreruns-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rssreruns-0.0.8/PKG-INFO` & `rssreruns-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssreruns
-Version: 0.0.8
+Version: 0.0.9
 Summary: Rebroadcast old RSS/Atom feed items to a new feed, in shuffled or chronological order.
 Author-email: Hannah Connolly <hannah.d.connolly@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hannah Connolly
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rssreruns-0.0.8/pyproject.toml` & `rssreruns-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rssreruns"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Hannah Connolly", email="hannah.d.connolly@gmail.com" },
 ]
 description = "Rebroadcast old RSS/Atom feed items to a new feed, in shuffled or chronological order."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
```

### Comparing `rssreruns-0.0.8/requirements-dev.txt` & `rssreruns-0.0.9/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `rssreruns-0.0.8/src/rssreruns/elementwrapper.py` & `rssreruns-0.0.9/src/rssreruns/elementwrapper.py`

 * *Files identical despite different names*

### Comparing `rssreruns-0.0.8/src/rssreruns/feedmodifier.py` & `rssreruns-0.0.9/src/rssreruns/feedmodifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Modify a given XML-based feed (RSS or Atom)."""
 from __future__ import annotations
 
 import copy
 import email.utils
 import random
+import uuid
 from abc import ABC, abstractmethod
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Any, Optional
 
 import requests
 from dateutil import parser
@@ -72,14 +73,15 @@
 
         # Default meta channel values:
         meta_channel_defaults = {
             "order": "chronological",
             "rate": "1",
             "run_forever": "True",
             "original_title": self._channel["title"].text or "",
+            "original_self_link": self.source_url(),
             "title_prefix": None,
             "title_suffix": None,
             "entry_title_prefix": None,
             "entry_title_suffix": None,
         }
         self._create_defaults_if_missing(self._meta_channel, meta_channel_defaults)
 
@@ -443,14 +445,15 @@
         else:
             dt = (
                 use_datetime
                 if isinstance(use_datetime, datetime)
                 else parser.parse(use_datetime)
             )
         self.update_entry_pubdate(entry, dt)
+        self._update_entry_uuid(entry)
         entry[self._meta_entry_tag]["reran"].text = "True"
 
     def write(
         self,
         path: str | Path | None,
         with_reruns_data: bool = True,
         pretty_print: bool = True,
@@ -528,14 +531,36 @@
         elif "atom" in self.__class__.__name__.lower():
             return "Atom"
         else:
             raise RuntimeError(
                 f"Feed format of {self} instance could not be determined."
             )
 
+    def _generate_entry_uuid(self, entry: ElementWrapper) -> str:
+        """Generate a UUID for a given entry.
+
+        The generated UUID will not be the same as the atom:id or rss:guid for the entry
+        (if one is already present.)
+
+        It may not technically be "correct" to replace an item's existing uuid if one
+        considers the republished entry to be "the same" as the original. Unfortunately,
+        some feed readers cache the entry's information (including publication date)
+        with the uuid as the key -- as a result, the reader won't recognize that an
+        entry has had its publication date changed if the entry's uuid remains the same.
+        """
+        return uuid.uuid4().urn
+
+    @abstractmethod
+    def _update_entry_uuid(self, entry: ElementWrapper) -> ElementWrapper:
+        """Update the entry's uuid (the guid or id for RSS or Atom respectively).
+
+        Returns the element (<guid> or <id>) containing the new uuid.
+        """
+        pass
+
     @abstractmethod
     def feed_channel(self) -> ElementWrapper:
         """Returns the `feed` (Atom) or `channel` (RSS) element of the tree."""
         pass
 
     @abstractmethod
     def feed_entries(self) -> list[ElementWrapper]:
@@ -610,14 +635,23 @@
         self._channel["lastBuildDate"].text = formatted_date
         return [self._channel["pubDate"], self._channel["lastBuildDate"]]
 
     def source_url(self) -> str:
         """Return the original feed's url."""
         return self._channel["link"].text
 
+    def _update_entry_uuid(self, entry: ElementWrapper) -> ElementWrapper:
+        """Update the entry's uuid in the <guid> subelement.
+
+        Returns the subelement containing the new uuid.
+        """
+        entry["guid"].text = self._generate_entry_uuid(entry)
+        entry["guid"].isPermaLink = "false"
+        return entry["guid"]
+
     @staticmethod
     def format_datetime(date: datetime) -> str:
         """Format a datetime as a string, in the format required for RSS.
 
         The RSS 2.0 specification stipulates:
 
         "All date-times in RSS conform to the Date and Time Specification of RFC 822,
@@ -696,14 +730,23 @@
         # The only reason to not just immediately return
         #
         #    (self_links or links)[0].href
         #
         # in the above is edge cases resolving uris relative to xml:base
         return "".join([link.base or "", link.href])
 
+    def _update_entry_uuid(self, entry: ElementWrapper) -> ElementWrapper:
+        """Update the entry's uuid in the <id> subelement.
+
+        Returns the subelement containing the new uuid.
+        """
+        entry["id"].text = self._generate_entry_uuid(entry)
+        entry["guid"].isPermaLink = "false"
+        return entry["id"]
+
     @staticmethod
     def format_datetime(date: datetime) -> str:
         """Format a datetime as a string, in the format required for Atom.
 
         The Atom specification stipulates:
 
         "A Date construct is an element whose content MUST conform to the "date-time"
```

### Comparing `rssreruns-0.0.8/src/rssreruns.egg-info/PKG-INFO` & `rssreruns-0.0.9/src/rssreruns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssreruns
-Version: 0.0.8
+Version: 0.0.9
 Summary: Rebroadcast old RSS/Atom feed items to a new feed, in shuffled or chronological order.
 Author-email: Hannah Connolly <hannah.d.connolly@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hannah Connolly
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rssreruns-0.0.8/src/rssreruns.egg-info/requires.txt` & `rssreruns-0.0.9/src/rssreruns.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rssreruns-0.0.8/test/test_elementwrapper.py` & `rssreruns-0.0.9/test/test_elementwrapper.py`

 * *Files identical despite different names*

### Comparing `rssreruns-0.0.8/test/test_feedmodifier.py` & `rssreruns-0.0.9/test/test_feedmodifier.py`

 * *Files identical despite different names*


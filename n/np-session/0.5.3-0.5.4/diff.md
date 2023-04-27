# Comparing `tmp/np-session-0.5.3.tar.gz` & `tmp/np-session-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-session-0.5.3.tar", last modified: Tue Apr 25 05:42:53 2023, max compression
+gzip compressed data, was "np-session-0.5.4.tar", last modified: Thu Apr 27 01:08:25 2023, max compression
```

## Comparing `np-session-0.5.3.tar` & `np-session-0.5.4.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     2194 2023-04-25 05:42:45.850824 np-session-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1373 2023-02-14 03:16:07.068541 np-session-0.5.3/README.md
--rw-r--r--   0        0        0      170 2023-03-17 05:14:59.145709 np-session-0.5.3/src/np_session/__init__.py
--rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.5.3/src/np_session/components/__init__.py
--rw-r--r--   0        0        0     8087 2023-04-25 01:32:31.553377 np-session-0.5.3/src/np_session/components/info.py
--rw-r--r--   0        0        0     7708 2023-03-23 23:41:50.844242 np-session-0.5.3/src/np_session/components/lims_manifests.py
--rw-r--r--   0        0        0     1390 2023-04-04 00:25:44.745816 np-session-0.5.3/src/np_session/components/paths.py
--rw-r--r--   0        0        0    10785 2023-03-17 05:14:59.154649 np-session-0.5.3/src/np_session/components/platform_json.py
--rw-r--r--   0        0        0     5019 2023-03-17 05:14:59.155648 np-session-0.5.3/src/np_session/components/settings_xml.py
--rw-r--r--   0        0        0      189 2023-03-19 18:40:51.970936 np-session-0.5.3/src/np_session/databases/__init__.py
--rw-r--r--   0        0        0    21233 2023-03-21 02:25:36.728269 np-session-0.5.3/src/np_session/databases/data_getters.py
--rw-r--r--   0        0        0     2716 2023-03-19 17:40:22.225142 np-session-0.5.3/src/np_session/databases/firebase_state.py
--rw-r--r--   0        0        0    12022 2023-03-17 05:14:59.159645 np-session-0.5.3/src/np_session/databases/lims2.py
--rw-r--r--   0        0        0    12644 2023-03-17 05:14:59.161647 np-session-0.5.3/src/np_session/databases/mtrain.py
--rw-r--r--   0        0        0     3687 2023-03-19 17:40:06.274698 np-session-0.5.3/src/np_session/databases/redis_state.py
--rw-r--r--   0        0        0     9863 2023-03-17 05:16:43.438094 np-session-0.5.3/src/np_session/databases/sql_alchemy.py
--rw-r--r--   0        0        0       83 2023-03-17 05:16:43.454095 np-session-0.5.3/src/np_session/jobs/__init__.py
--rw-r--r--   0        0        0      423 2023-03-19 18:45:17.801626 np-session-0.5.3/src/np_session/jobs/find_missing_files.py
--rw-r--r--   0        0        0        0 2023-03-19 18:03:04.930628 np-session-0.5.3/src/np_session/jobs/generate_session_summaries.py
--rw-r--r--   0        0        0     4123 2023-03-19 01:12:39.701848 np-session-0.5.3/src/np_session/jobs/lims_upload.py
--rw-r--r--   0        0        0     5710 2023-03-17 05:16:43.439093 np-session-0.5.3/src/np_session/jobs/probes.py
--rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.5.3/src/np_session/jobs/sessions.json
--rw-r--r--   0        0        0      551 2023-03-19 18:00:31.176404 np-session-0.5.3/src/np_session/jobs/sync_states.py
--rw-r--r--   0        0        0    26133 2023-04-20 20:34:24.850399 np-session-0.5.3/src/np_session/session.py
--rw-r--r--   0        0        0     8357 2023-04-20 17:27:28.627831 np-session-0.5.3/src/np_session/utils.py
--rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.5.3/tests/__init__.py
--rw-r--r--   0        0        0      406 2023-03-17 05:16:43.457095 np-session-0.5.3/tests/test_np_session.py
--rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.5.3/tests/test_platform_json.py
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 np-session-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     2217 2023-04-27 01:08:21.001459 np-session-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1373 2023-02-14 03:16:07.068541 np-session-0.5.4/README.md
+-rw-r--r--   0        0        0      170 2023-03-17 05:14:59.145709 np-session-0.5.4/src/np_session/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.5.4/src/np_session/components/__init__.py
+-rw-r--r--   0        0        0     8069 2023-04-27 00:58:03.330699 np-session-0.5.4/src/np_session/components/info.py
+-rw-r--r--   0        0        0     8823 2023-04-27 00:05:53.424367 np-session-0.5.4/src/np_session/components/lims_manifests.py
+-rw-r--r--   0        0        0     1390 2023-04-04 00:25:44.745816 np-session-0.5.4/src/np_session/components/paths.py
+-rw-r--r--   0        0        0    10785 2023-03-17 05:14:59.154649 np-session-0.5.4/src/np_session/components/platform_json.py
+-rw-r--r--   0        0        0     5019 2023-03-17 05:14:59.155648 np-session-0.5.4/src/np_session/components/settings_xml.py
+-rw-r--r--   0        0        0      189 2023-03-19 18:40:51.970936 np-session-0.5.4/src/np_session/databases/__init__.py
+-rw-r--r--   0        0        0    21233 2023-03-21 02:25:36.728269 np-session-0.5.4/src/np_session/databases/data_getters.py
+-rw-r--r--   0        0        0     2716 2023-03-19 17:40:22.225142 np-session-0.5.4/src/np_session/databases/firebase_state.py
+-rw-r--r--   0        0        0    12022 2023-03-17 05:14:59.159645 np-session-0.5.4/src/np_session/databases/lims2.py
+-rw-r--r--   0        0        0    12644 2023-03-17 05:14:59.161647 np-session-0.5.4/src/np_session/databases/mtrain.py
+-rw-r--r--   0        0        0     3687 2023-03-19 17:40:06.274698 np-session-0.5.4/src/np_session/databases/redis_state.py
+-rw-r--r--   0        0        0     9863 2023-03-17 05:16:43.438094 np-session-0.5.4/src/np_session/databases/sql_alchemy.py
+-rw-r--r--   0        0        0       83 2023-03-17 05:16:43.454095 np-session-0.5.4/src/np_session/jobs/__init__.py
+-rw-r--r--   0        0        0      423 2023-03-19 18:45:17.801626 np-session-0.5.4/src/np_session/jobs/find_missing_files.py
+-rw-r--r--   0        0        0     4123 2023-03-19 01:12:39.701848 np-session-0.5.4/src/np_session/jobs/lims_upload.py
+-rw-r--r--   0        0        0     5710 2023-03-17 05:16:43.439093 np-session-0.5.4/src/np_session/jobs/probes.py
+-rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.5.4/src/np_session/jobs/sessions.json
+-rw-r--r--   0        0        0      551 2023-03-19 18:00:31.176404 np-session-0.5.4/src/np_session/jobs/sync_states.py
+-rw-r--r--   0        0        0    26133 2023-04-26 15:19:15.269851 np-session-0.5.4/src/np_session/session.py
+-rw-r--r--   0        0        0     8357 2023-04-20 17:27:28.627831 np-session-0.5.4/src/np_session/utils.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.5.4/tests/__init__.py
+-rw-r--r--   0        0        0      406 2023-03-17 05:16:43.457095 np-session-0.5.4/tests/test_np_session.py
+-rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.5.4/tests/test_platform_json.py
+-rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 np-session-0.5.4/PKG-INFO
```

### Comparing `np-session-0.5.3/pyproject.toml` & `np-session-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np-session"
-version = "0.5.3"
+version = "0.5.4"
 description = "Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -18,14 +18,15 @@
     "requests>=2",
     "np_logging>=0.3.8",
     "np_config>=0.4.17",
     "backports.cached-property",
     "firebase-admin>=6.1.0",
     "redis>=4.5.1",
     "pydantic>=1.10.5",
+    "np-tools>=0.1.4",
 ]
 
 [project.urls]
 Repository = "https://github.com/alleninstitute/np_session"
 "Bug Tracker" = "https://github.com/alleninstitute/np_session/issues"
 
 [project.optional-dependencies]
```

### Comparing `np-session-0.5.3/README.md` & `np-session-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/components/info.py` & `np-session-0.5.4/src/np_session/components/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import abc
 import datetime
 import enum
 import functools
 import time
 from typing import Any, ClassVar, MutableMapping, Optional
 
-import np_config
 import np_logging
 from backports.cached_property import cached_property
 from typing_extensions import Literal
 
 from np_session.databases import State
 from np_session.databases.lims2 import (LIMS2MouseInfo, LIMS2ProjectInfo,
                                         LIMS2UserInfo)
```

### Comparing `np-session-0.5.3/src/np_session/components/lims_manifests.py` & `np-session-0.5.4/src/np_session/components/lims_manifests.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,31 @@
         
         if self.session:
             self.assign_props_from_session()
         elif self.session_type is None:
             self.session_type = 'D1'
             
         self.fetch_from_zk()
+        self.remove_non_inserted_probes() # does nothing if no self.session 
     
+    def remove_non_inserted_probes(self) -> None:
+        if self.session is None:
+            return
+        probes_inserted = self.session.probes_inserted
+        include_idx = tuple(
+                i
+                for i, name in enumerate(self.names)
+                if (
+                    'probe_' not in name # not a probe field - skip
+                    or any(f'probe_{letter.upper()}' in name for letter in probes_inserted)
+                )
+            )
+        self.names, self.globs, self.types = (tuple(_[i] for i in include_idx) for _ in (self.names, self.globs, self.types))
+
+                
     @property
     def files(self) -> dict[str, dict[str, str]]:
         """Upload manifest for platform json: `{name: {type: session + glob}}, ...}`"""
         if not self.session:
             return {k: {v: g} for k, v, g in zip(self.names, self.types, self.globs)}
         return {k: {v: (p.name if p else None)} for k, v, p in zip(self.names, self.types, self.paths)}
     
@@ -96,19 +112,22 @@
         return tuple(n for n, p in zip(self.names, self.paths) if p is None)
     
     
     def get_sorted_data(self) -> None:
         self._names_sorted_data = []
         self._paths_sorted_data = []
         self._globs_sorted_data = []
-        for probe in 'ABCDEF':
+        for probe in ('ABCDEF' if self.session is None else self.session.probes_inserted):
             for name, glob in MANIFESTS['_name_glob']['sorted_data'].items():
                 probe_glob =f'*_probe{probe}{glob}'
                 self._globs_sorted_data.append(probe_glob)
                 self._names_sorted_data.append(f'{name}_probe{probe}')
+                if self.session is None:
+                    logger.warning(f'No session provided to {self.__class__} - cannot get sorted data paths.')
+                    return
                 hits = tuple(self.session.npexp_path.glob(probe_glob))
                 if len(hits) == 0:
                     logger.debug(f'No files found for glob: {self.session.npexp_path / probe_glob}')
                 if len(hits) > 1:
                     logger.debug(f'Multiple files found for glob: {self.session.npexp_path / probe_glob} - {hits} - using first.')
                 self._paths_sorted_data.append(hits[0] if hits else None)
         
@@ -131,14 +150,17 @@
         with contextlib.suppress(AttributeError):
             return tuple(self._globs_sorted_data)
         self.get_sorted_data()
         return self.globs_sorted_data
     
     @property
     def missing_sorted_data(self) -> tuple[str]:
+        if self.session is None:
+            logger.warning(f'No session provided to {self.__class__} - cannot get sorted data paths.')
+            return tuple()
         return tuple(n for n, p in zip(self.names_sorted_data, self.paths_sorted_data) if p is None)
     
     def parse_input_args(self, *args, **kwargs) -> None:
         for _ in (*args, *kwargs.values()):
             if isinstance(_, np_session.session.Session):
                 self.session = _
                 break
```

### Comparing `np-session-0.5.3/src/np_session/components/paths.py` & `np-session-0.5.4/src/np_session/components/paths.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/components/platform_json.py` & `np-session-0.5.4/src/np_session/components/platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/components/settings_xml.py` & `np-session-0.5.4/src/np_session/components/settings_xml.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/databases/data_getters.py` & `np-session-0.5.4/src/np_session/databases/data_getters.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/databases/firebase_state.py` & `np-session-0.5.4/src/np_session/databases/firebase_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/databases/lims2.py` & `np-session-0.5.4/src/np_session/databases/lims2.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/databases/mtrain.py` & `np-session-0.5.4/src/np_session/databases/mtrain.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/databases/redis_state.py` & `np-session-0.5.4/src/np_session/databases/redis_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/databases/sql_alchemy.py` & `np-session-0.5.4/src/np_session/databases/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/jobs/lims_upload.py` & `np-session-0.5.4/src/np_session/jobs/lims_upload.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/jobs/probes.py` & `np-session-0.5.4/src/np_session/jobs/probes.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/jobs/sessions.json` & `np-session-0.5.4/src/np_session/jobs/sessions.json`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/jobs/sync_states.py` & `np-session-0.5.4/src/np_session/jobs/sync_states.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/session.py` & `np-session-0.5.4/src/np_session/session.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/src/np_session/utils.py` & `np-session-0.5.4/src/np_session/utils.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/tests/test_platform_json.py` & `np-session-0.5.4/tests/test_platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.3/PKG-INFO` & `np-session-0.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-session
-Version: 0.5.3
+Version: 0.5.4
 Summary: Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
```


# Comparing `tmp/captif_cpx_db-0.1.tar.gz` & `tmp/captif_cpx_db-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_db-0.1.tar", max compression
+gzip compressed data, was "captif_cpx_db-0.2.tar", max compression
```

## Comparing `captif_cpx_db-0.1.tar` & `captif_cpx_db-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-04-04 00:16:15.869925 captif_cpx_db-0.1/LICENSE
--rw-r--r--   0        0        0       16 2023-04-04 00:16:15.869925 captif_cpx_db-0.1/README.md
--rw-r--r--   0        0        0      257 2023-04-04 00:16:15.869925 captif_cpx_db-0.1/captif_cpx_db/__init__.py
--rw-r--r--   0        0        0       30 2023-04-04 00:16:15.869925 captif_cpx_db-0.1/captif_cpx_db/constants.py
--rw-r--r--   0        0        0     2060 2023-04-04 00:16:15.869925 captif_cpx_db-0.1/captif_cpx_db/models/__init__.py
--rw-r--r--   0        0        0      244 2023-04-04 00:16:15.869925 captif_cpx_db-0.1/captif_cpx_db/models/sa_helpers.py
--rw-r--r--   0        0        0    10680 2023-04-04 00:16:15.869925 captif_cpx_db-0.1/captif_cpx_db/models/segment.py
--rw-r--r--   0        0        0     7648 2023-04-04 00:16:15.869925 captif_cpx_db-0.1/captif_cpx_db/models/session.py
--rw-r--r--   0        0        0      504 2023-04-04 00:16:15.869925 captif_cpx_db-0.1/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/LICENSE
+-rw-r--r--   0        0        0       16 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/README.md
+-rw-r--r--   0        0        0      257 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/constants.py
+-rw-r--r--   0        0        0     2060 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/models/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/models/sa_helpers.py
+-rw-r--r--   0        0        0    10435 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/models/segment.py
+-rw-r--r--   0        0        0     7648 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/models/session.py
+-rw-r--r--   0        0        0      504 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.2/PKG-INFO
```

### Comparing `captif_cpx_db-0.1/LICENSE` & `captif_cpx_db-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_db-0.1/captif_cpx_db/models/__init__.py` & `captif_cpx_db-0.2/captif_cpx_db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `captif_cpx_db-0.1/captif_cpx_db/models/segment.py` & `captif_cpx_db-0.2/captif_cpx_db/models/segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,7 @@
         nullable=False,
         description=(
             "one-third octave LCPX with all corrections applied (including "
             "the device-related correction) in dB (refer ISO 11819-2:2017 "
             "Formula C.8 and C.9)"
         ),
     )
-    lcpx_db_corrected: float = Field(
-        nullable=False,
-        description=(
-            "one-third octave LCPX (see 'lcpx_db' field) corrected for "
-            "averaging effects (refer ISO 11819-2:2017 C.10 and C.11)"
-        ),
-    )
```

### Comparing `captif_cpx_db-0.1/captif_cpx_db/models/session.py` & `captif_cpx_db-0.2/captif_cpx_db/models/session.py`

 * *Files identical despite different names*


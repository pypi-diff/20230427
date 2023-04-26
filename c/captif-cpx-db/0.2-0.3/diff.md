# Comparing `tmp/captif_cpx_db-0.2.tar.gz` & `tmp/captif_cpx_db-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_db-0.2.tar", max compression
+gzip compressed data, was "captif_cpx_db-0.3.tar", max compression
```

## Comparing `captif_cpx_db-0.2.tar` & `captif_cpx_db-0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/LICENSE
--rw-r--r--   0        0        0       16 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/README.md
--rw-r--r--   0        0        0      257 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/__init__.py
--rw-r--r--   0        0        0       30 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/constants.py
--rw-r--r--   0        0        0     2060 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/models/__init__.py
--rw-r--r--   0        0        0      244 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/models/sa_helpers.py
--rw-r--r--   0        0        0    10435 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/models/segment.py
--rw-r--r--   0        0        0     7648 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/captif_cpx_db/models/session.py
--rw-r--r--   0        0        0      504 2023-04-26 22:13:52.087750 captif_cpx_db-0.2/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/LICENSE
+-rw-r--r--   0        0        0       16 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/README.md
+-rw-r--r--   0        0        0      257 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/constants.py
+-rw-r--r--   0        0        0     2060 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/models/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/models/sa_helpers.py
+-rw-r--r--   0        0        0    10574 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/models/segment.py
+-rw-r--r--   0        0        0     7648 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/models/session.py
+-rw-r--r--   0        0        0      504 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.3/PKG-INFO
```

### Comparing `captif_cpx_db-0.2/LICENSE` & `captif_cpx_db-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_db-0.2/captif_cpx_db/models/__init__.py` & `captif_cpx_db-0.3/captif_cpx_db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `captif_cpx_db-0.2/captif_cpx_db/models/segment.py` & `captif_cpx_db-0.3/captif_cpx_db/models/segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,14 +150,18 @@
     wheel_bay_name: str = Field(
         primary_key=True,
         description="wheel_bay name ('left' or 'right')",
     )
     ir_temperatures: List["IRTemperature"] = Relationship()
     microphone_details: List["SegmentMicrophoneDetails"] = Relationship()
     wheel_bay_third_octave_levels: List["WheelBayThirdOctaveLevels"] = Relationship()
+    laeq_db: float = Field(
+        nullable=False,
+        description="LAeq for the wheel bay in dB (no CPX corrections applied)",
+    )
     lcpx_db: float = Field(
         nullable=False,
         description="LCPX for the wheel bay in dB",
     )
 
 
 class IRTemperature(SQLModel, table=True):
```

### Comparing `captif_cpx_db-0.2/captif_cpx_db/models/session.py` & `captif_cpx_db-0.3/captif_cpx_db/models/session.py`

 * *Files identical despite different names*


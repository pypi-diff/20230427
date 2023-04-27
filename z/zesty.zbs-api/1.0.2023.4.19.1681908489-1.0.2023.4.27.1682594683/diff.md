# Comparing `tmp/zesty.zbs-api-1.0.2023.4.19.1681908489.tar.gz` & `tmp/zesty.zbs-api-1.0.2023.4.27.1682594683.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-1.0.2023.4.19.1681908489.tar", last modified: Wed Apr 19 12:48:09 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-1.0.2023.4.27.1682594683.tar", last modified: Thu Apr 27 11:24:43 2023, max compression
```

## Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489.tar` & `zesty.zbs-api-1.0.2023.4.27.1682594683.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:48:09.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1166 2023-04-19 12:48:09.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-19 12:48:09.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:48:09.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14353 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:48:09.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3540 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     8818 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7367 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    15025 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    11605 2023-04-19 12:43:02.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/src/protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 12:48:09.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/zesty.zbs_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1166 2023-04-19 12:48:09.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/zesty.zbs_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      599 2023-04-19 12:48:09.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/zesty.zbs_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 12:48:09.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/zesty.zbs_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-19 12:48:09.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/zesty.zbs_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-19 12:48:09.000000 zesty.zbs-api-1.0.2023.4.19.1681908489/zesty.zbs_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:24:43.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-04-27 11:24:43.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-27 11:24:43.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:24:43.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14353 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:24:43.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     8818 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7367 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    16027 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    11605 2023-04-27 11:24:19.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/src/protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:24:43.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/zesty.zbs_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-04-27 11:24:43.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/zesty.zbs_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      599 2023-04-27 11:24:43.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/zesty.zbs_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:24:43.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/zesty.zbs_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-27 11:24:43.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/zesty.zbs_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-27 11:24:43.000000 zesty.zbs-api-1.0.2023.4.27.1682594683/zesty.zbs_api.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/PKG-INFO` & `zesty.zbs-api-1.0.2023.4.27.1682594683/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api
-Version: 1.0.2023.4.19.1681908489
+Version: 1.0.2023.4.27.1682594683
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/README.md` & `zesty.zbs-api-1.0.2023.4.27.1682594683/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/setup.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/actions.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/actions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/BlockDevice.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/BlockDevice.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/EbsVolume.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/EbsVolume.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/FileSystem.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/InstancesTags.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/ManagedFS.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/ManagedFS.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import datetime
 import time
-from typing import Any, Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union
 from uuid import UUID as _UUID
 from uuid import uuid4
 
-from sqlalchemy import INT, ForeignKey
-from sqlalchemy.dialects.postgresql import ARRAY, TIME, UUID
-from sqlalchemy.orm import relationship
+from sqlalchemy import TIMESTAMP, INT
+from sqlalchemy.dialects.postgresql import ARRAY, UUID
 
 try:
-    from sqlalchemy import (Column, String, case, cast, engine, func, or_,
-                            select, text)
+    from sqlalchemy import Column, String, case, cast, engine, func, or_
     from sqlalchemy.dialects.postgresql import (BIGINT, BOOLEAN, FLOAT, JSON,
                                                 TIMESTAMP, VARCHAR)
     from sqlalchemy.ext.declarative import declarative_base
     from sqlalchemy.orm import Query, Session, aliased, sessionmaker
 except ImportError:
     raise ImportError(
         "sqlalchemy is required by zesty.zbs-api but needs to be vendored separately. Add postgres-utils to your project's requirements that depend on zbs-api.")
@@ -284,47 +281,59 @@
 
     fs_id = Column(VARCHAR)
     migration_uuid = Column(UUID(as_uuid=True), nullable=False, primary_key=True)
 
     reboot = Column(BOOLEAN, default=False)
     # array of day numbers when reboot is allowed 0-6
     days = Column(ARRAY(VARCHAR))
-    # timeframe from-to
+    # timeframe from-to in %I:%M %p
     from_ = Column(VARCHAR)
     to = Column(VARCHAR)
+
     is_rebooting = Column(BOOLEAN, default=False)
     is_aborted = Column(BOOLEAN, default=False)
+    # Snapshot and ebs deletion in days
+    ebs_remove_after = Column(INT, nullable=True)
+    snapshot_remove_after = Column(INT, nullable=True)
 
     def __init__(
             self,
             fs_id: str,
             migration_uuid: _UUID,
             days: Optional[List[int]] = None,
-            from_: Optional[datetime.time] = None,
-            to: Optional[datetime.time] = None,
-            reboot: bool = False):
+            from_: Optional[str] = None,
+            to: Optional[str] = None,
+            reboot: bool = False,
+            ebs_remove_after: int = 1,
+            snapshot_remove_after: int = 7):
         self.migration_uuid = migration_uuid
         self.fs_id = fs_id
         self.days = days
         self.from_ = from_
         self.to = to
         self.reboot = reboot
+        self.ebs_remove_after = ebs_remove_after
+        self.snapshot_remove_after = snapshot_remove_after
 
     @staticmethod
     def new_migration(
             fs_id,
             days: Optional[List[int]] = None,
-            from_: Optional[datetime.time] = None,
-            to: Optional[datetime.time] = None,
-            reboot: bool = False) -> 'RunningMigrations':
+            from_: Optional[str] = None,
+            to: Optional[str] = None,
+            reboot: bool = False,
+            ebs_remove_after: int = 1,
+            snapshot_remove_after: int = 7) -> 'RunningMigrations':
         return RunningMigrations(
             fs_id,
             uuid4(),
             days, from_,
-            to, reboot
+            to, reboot,
+            ebs_remove_after,
+            snapshot_remove_after,
         )
 
 
 class MigrationHistory(BaseMixin, Base):
     __tablename__ = "migration_history"
 
     time_start = Column(TIMESTAMP)
@@ -395,9 +404,27 @@
 
     def set_action(self, action):
         if action not in self.allowed_actions:
             raise WrongActionException
         self.action = action
 
 
+class MigrationOrigin(BaseMixin, Base):
+    __tablename__ = 'migration_origins'
+
+    fs_id = Column(VARCHAR(255))
+    migration_uuid = Column(UUID(as_uuid=True), nullable=False, primary_key=True)
+
+    region = Column(VARCHAR(255))
+    snapshot_id = Column(VARCHAR(255))
+    snapshot_expire_after_days = Column(INT, nullable=True)
+    snapshot_create_started_at = Column(TIMESTAMP, nullable=True)
+    snapshot_deleted_at = Column(TIMESTAMP, nullable=True)
+
+    ebs_id = Column(VARCHAR(255))
+    ebs_expire_after_days = Column(INT, nullable=True)
+    ebs_detached_at = Column(TIMESTAMP, nullable=True)
+    ebs_deleted_at = Column(TIMESTAMP, nullable=True)
+
+
 def create_tables(engine: engine.base.Engine) -> None:
     Base.metadata.create_all(engine, checkfirst=True)
```

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/Usage.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/agent_report.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/cpu_mon.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/disk_mon.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/hf_interface.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/models/overview.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/src/protocol.py` & `zesty.zbs-api-1.0.2023.4.27.1682594683/src/protocol.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/zesty.zbs_api.egg-info/PKG-INFO` & `zesty.zbs-api-1.0.2023.4.27.1682594683/zesty.zbs_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api
-Version: 1.0.2023.4.19.1681908489
+Version: 1.0.2023.4.27.1682594683
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-1.0.2023.4.19.1681908489/zesty.zbs_api.egg-info/SOURCES.txt` & `zesty.zbs-api-1.0.2023.4.27.1682594683/zesty.zbs_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

